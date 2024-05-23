# Comparing `tmp/jupyter_environment_manager-0.2.0rc9.tar.gz` & `tmp/jupyter_environment_manager-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter_environment_manager-0.2.0rc9.tar", last modified: Fri Apr 19 22:02:51 2024, max compression
+gzip compressed data, was "jupyter_environment_manager-0.2.1.tar", last modified: Thu May 23 20:37:50 2024, max compression
```

## Comparing `jupyter_environment_manager-0.2.0rc9.tar` & `jupyter_environment_manager-0.2.1.tar`

### file list

```diff
@@ -1,127 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:02:51.954205 jupyter_environment_manager-0.2.0rc9/
--rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-04-19 22:02:51.954205 jupyter_environment_manager-0.2.0rc9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/install.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:02:51.890205 jupyter_environment_manager-0.2.0rc9/jupyter-config/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:02:51.902205 jupyter_environment_manager-0.2.0rc9/jupyter-config/nb-config/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/jupyter-config/nb-config/jupyter_environment_manager.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:02:51.902205 jupyter_environment_manager-0.2.0rc9/jupyter-config/server-config/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/jupyter-config/server-config/jupyter_environment_manager.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:02:51.910205 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/configure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/devices.py
--rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/envs_create.py
--rw-r--r--   0 runner    (1001) docker     (127)    12843 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/envs_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/envs_pkgs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7129 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/envs_remove.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/envs_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/kernels.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:02:51.910205 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/
--rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:02:51.930205 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (127)    94749 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/0.99dd872e735721a05b18.js
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/0.99dd872e735721a05b18.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    17291 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/113.063bb6057d77be1f85f3.js
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/113.063bb6057d77be1f85f3.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/151.18af1747c52fa1890fce.js
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/174.7b162c87cb727f7c2712.js
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/174.7b162c87cb727f7c2712.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)   202661 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/185.c2e096475cfee897e1f9.js
--rw-r--r--   0 runner    (1001) docker     (127)  3944216 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/24.a6fec73552ceb9bdb6aa.js
--rw-r--r--   0 runner    (1001) docker     (127)   300035 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/313.f6abbabc37aacd77b555.js
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/313.f6abbabc37aacd77b555.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11262 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/378.8fdd4b1246fb17037bb3.js
--rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/478.b1efc8dc1ed4a16150ef.js
--rw-r--r--   0 runner    (1001) docker     (127)    22112 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/554.3ee5e631ee6f4d8c24e2.js
--rw-r--r--   0 runner    (1001) docker     (127)    22640 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/569.110780388cdcc5605903.js
--rw-r--r--   0 runner    (1001) docker     (127)    37522 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/588.634556691591dc1dac9b.js
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/588.634556691591dc1dac9b.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    37522 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/66.715eff54360a4988967a.js
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/66.715eff54360a4988967a.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/697.61315fde7050f7a02689.js
--rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/747.6d49dfe38d298a9d88e1.js
--rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/813.4baf0234297462c92d8b.js
--rw-r--r--   0 runner    (1001) docker     (127)   454999 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/909.c50074d4e4be5aa7c06a.js
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/909.c50074d4e4be5aa7c06a.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)   446062 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/981.f54a04f7142174f18f0d.js
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/981.f54a04f7142174f18f0d.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/991.b0c652da28634799e4d5.js
--rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/remoteEntry.5fd255ae2892e93a3890.js
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-19 22:02:02.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (127)   509524 2024-04-19 22:02:47.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:02:51.954205 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-04-19 22:02:51.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-04-19 22:02:51.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 22:02:51.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 22:01:42.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-19 22:02:51.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-19 22:02:51.000000 jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-19 22:01:29.000000 jupyter_environment_manager-0.2.0rc9/package.json
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 22:02:51.954205 jupyter_environment_manager-0.2.0rc9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:02:51.930205 jupyter_environment_manager-0.2.0rc9/src/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/EnvironmentsSidebarWidget.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/Flux.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:02:51.934205 jupyter_environment_manager-0.2.0rc9/src/actions/
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/actions/ApiActions.js
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/actions/AuthActions.js
--rw-r--r--   0 runner    (1001) docker     (127)    29226 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/actions/EnvironmentActions.js
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/actions/JupyterApiActions.js
--rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/actions/UserActions.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:02:51.894205 jupyter_environment_manager-0.2.0rc9/src/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:02:51.942205 jupyter_environment_manager-0.2.0rc9/src/assets/icons/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/assets/icons/BackIcon.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/assets/icons/CloseIcon.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/assets/icons/ConfirmIcon.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/assets/icons/DescriptionIcon.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/assets/icons/EnvIcon.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/assets/icons/IconString.js
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/assets/icons/LinkIcon.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/assets/icons/Loading.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/assets/icons/RefreshIcon.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/assets/icons/SearchIcon.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/assets/icons/UserIcon.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/assets/icons/WhiteCube.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/assets.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:02:51.946205 jupyter_environment_manager-0.2.0rc9/src/components/
--rw-r--r--   0 runner    (1001) docker     (127)     8469 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/components/EndUserAgreement.js
--rw-r--r--   0 runner    (1001) docker     (127)   107258 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/components/EnvironmentEditor.js
--rw-r--r--   0 runner    (1001) docker     (127)    13095 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/components/EnvironmentTile.js
--rw-r--r--   0 runner    (1001) docker     (127)    99350 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/components/EnvironmentsSidebar.js
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/components/Loading.js
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/components/LogoLoader.js
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/components/MuiStyledComponents.js
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/components/UserNotFound.js
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/contextTypes.js
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/global.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/index.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:02:51.946205 jupyter_environment_manager-0.2.0rc9/src/stores/
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/stores/AuthStore.js
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/stores/EnvironmentStore.js
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/stores/UserStore.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:02:51.950205 jupyter_environment_manager-0.2.0rc9/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/utils/googleAnalytics.js
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/src/utils/theme.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:02:51.950205 jupyter_environment_manager-0.2.0rc9/style/
--rw-r--r--   0 runner    (1001) docker     (127)    19450 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/style/EnvironmentEditor.css
--rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/style/EnvironmentTile.css
--rw-r--r--   0 runner    (1001) docker     (127)    11934 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/style/EnvironmentsSidebar.css
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/style/Loading.css
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/style/LogoLoader.css
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/style/base.css
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/style/index.css
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/style/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 22:02:51.954205 jupyter_environment_manager-0.2.0rc9/tools/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2564 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/tools/create_dev_build.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     3841 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/tools/stamp_pre_release.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/tsconfig.json
--rw-r--r--   0 runner    (1001) docker     (127)   607255 2024-04-19 22:00:43.000000 jupyter_environment_manager-0.2.0rc9/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:37:50.293902 jupyter_environment_manager-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5774 2024-05-23 20:37:50.293902 jupyter_environment_manager-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/install.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:37:50.257902 jupyter_environment_manager-0.2.1/jupyter-config/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:37:50.265902 jupyter_environment_manager-0.2.1/jupyter-config/nb-config/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/jupyter-config/nb-config/jupyter_environment_manager.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:37:50.265902 jupyter_environment_manager-0.2.1/jupyter-config/server-config/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/jupyter-config/server-config/jupyter_environment_manager.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:37:50.265902 jupyter_environment_manager-0.2.1/jupyter_environment_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/jupyter_environment_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/jupyter_environment_manager/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/jupyter_environment_manager/configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/jupyter_environment_manager/devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/jupyter_environment_manager/envs_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12843 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/jupyter_environment_manager/envs_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/jupyter_environment_manager/envs_pkgs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7129 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/jupyter_environment_manager/envs_remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/jupyter_environment_manager/envs_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/jupyter_environment_manager/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/jupyter_environment_manager/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/jupyter_environment_manager/kernels.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:37:50.269903 jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/
+-rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-05-23 20:37:44.000000 jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:37:50.281902 jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    94749 2024-05-23 20:37:44.000000 jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/0.99dd872e735721a05b18.js
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-23 20:37:44.000000 jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/0.99dd872e735721a05b18.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17291 2024-05-23 20:37:44.000000 jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/113.063bb6057d77be1f85f3.js
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-23 20:37:44.000000 jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/113.063bb6057d77be1f85f3.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-23 20:37:44.000000 jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/151.18af1747c52fa1890fce.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-23 20:37:44.000000 jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/174.7b162c87cb727f7c2712.js
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-23 20:37:44.000000 jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/174.7b162c87cb727f7c2712.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   213514 2024-05-23 20:37:44.000000 jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/227.bba2b52e5695cc9b34b7.js
+-rw-r--r--   0 runner    (1001) docker     (127)  3944216 2024-05-23 20:37:44.000000 jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/24.a6fec73552ceb9bdb6aa.js
+-rw-r--r--   0 runner    (1001) docker     (127)   300035 2024-05-23 20:37:44.000000 jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/313.f6abbabc37aacd77b555.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-23 20:37:44.000000 jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/313.f6abbabc37aacd77b555.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11262 2024-05-23 20:37:44.000000 jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/378.8fdd4b1246fb17037bb3.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-05-23 20:37:44.000000 jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/478.b1efc8dc1ed4a16150ef.js
+-rw-r--r--   0 runner    (1001) docker     (127)    22112 2024-05-23 20:37:44.000000 jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/554.3ee5e631ee6f4d8c24e2.js
+-rw-r--r--   0 runner    (1001) docker     (127)    22640 2024-05-23 20:37:44.000000 jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/569.110780388cdcc5605903.js
+-rw-r--r--   0 runner    (1001) docker     (127)    37522 2024-05-23 20:37:44.000000 jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/588.634556691591dc1dac9b.js
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-23 20:37:44.000000 jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/588.634556691591dc1dac9b.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    37522 2024-05-23 20:37:44.000000 jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/66.715eff54360a4988967a.js
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-23 20:37:44.000000 jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/66.715eff54360a4988967a.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-23 20:37:44.000000 jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/697.61315fde7050f7a02689.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-05-23 20:37:44.000000 jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/747.6d49dfe38d298a9d88e1.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-05-23 20:37:44.000000 jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/813.4baf0234297462c92d8b.js
+-rw-r--r--   0 runner    (1001) docker     (127)   454999 2024-05-23 20:37:44.000000 jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/909.c50074d4e4be5aa7c06a.js
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-23 20:37:44.000000 jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/909.c50074d4e4be5aa7c06a.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   446062 2024-05-23 20:37:44.000000 jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/981.f54a04f7142174f18f0d.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-23 20:37:44.000000 jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/981.f54a04f7142174f18f0d.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-05-23 20:37:44.000000 jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/991.b0c652da28634799e4d5.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10665 2024-05-23 20:37:44.000000 jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/remoteEntry.df30dcda2252f4ea7597.js
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-23 20:36:55.000000 jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (127)   509524 2024-05-23 20:37:44.000000 jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:37:50.293902 jupyter_environment_manager-0.2.1/jupyter_environment_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5774 2024-05-23 20:37:50.000000 jupyter_environment_manager-0.2.1/jupyter_environment_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-05-23 20:37:50.000000 jupyter_environment_manager-0.2.1/jupyter_environment_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 20:37:50.000000 jupyter_environment_manager-0.2.1/jupyter_environment_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 20:36:34.000000 jupyter_environment_manager-0.2.1/jupyter_environment_manager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-23 20:37:50.000000 jupyter_environment_manager-0.2.1/jupyter_environment_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-23 20:37:50.000000 jupyter_environment_manager-0.2.1/jupyter_environment_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 20:37:50.293902 jupyter_environment_manager-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:37:50.285902 jupyter_environment_manager-0.2.1/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/src/EnvironmentsSidebarWidget.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/src/Flux.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:37:50.285902 jupyter_environment_manager-0.2.1/src/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/src/actions/ApiActions.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/src/actions/AuthActions.js
+-rw-r--r--   0 runner    (1001) docker     (127)    29470 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/src/actions/EnvironmentActions.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/src/actions/JupyterApiActions.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/src/actions/UserActions.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:37:50.261902 jupyter_environment_manager-0.2.1/src/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:37:50.289903 jupyter_environment_manager-0.2.1/src/assets/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/src/assets/icons/BackIcon.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/src/assets/icons/CloseIcon.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/src/assets/icons/ConfirmIcon.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/src/assets/icons/DescriptionIcon.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/src/assets/icons/EnvIcon.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/src/assets/icons/IconString.js
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/src/assets/icons/LinkIcon.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/src/assets/icons/Loading.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/src/assets/icons/RefreshIcon.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/src/assets/icons/SearchIcon.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/src/assets/icons/UserIcon.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/src/assets/icons/WhiteCube.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/src/assets.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:37:50.289903 jupyter_environment_manager-0.2.1/src/components/
+-rw-r--r--   0 runner    (1001) docker     (127)     8469 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/src/components/EndUserAgreement.js
+-rw-r--r--   0 runner    (1001) docker     (127)   119515 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/src/components/EnvironmentEditor.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13191 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/src/components/EnvironmentTile.js
+-rw-r--r--   0 runner    (1001) docker     (127)   100308 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/src/components/EnvironmentsSidebar.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/src/components/Loading.js
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/src/components/LogoLoader.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/src/components/MuiStyledComponents.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/src/components/PublishSlider.js
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/src/components/UserNotFound.js
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/src/contextTypes.js
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/src/global.d.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/src/index.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:37:50.289903 jupyter_environment_manager-0.2.1/src/stores/
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/src/stores/AuthStore.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/src/stores/EnvironmentStore.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/src/stores/UserStore.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:37:50.289903 jupyter_environment_manager-0.2.1/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/src/utils/googleAnalytics.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/src/utils/theme.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:37:50.293902 jupyter_environment_manager-0.2.1/style/
+-rw-r--r--   0 runner    (1001) docker     (127)    19450 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/style/EnvironmentEditor.css
+-rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/style/EnvironmentTile.css
+-rw-r--r--   0 runner    (1001) docker     (127)    12049 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/style/EnvironmentsSidebar.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/style/Loading.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/style/LogoLoader.css
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/style/base.css
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/style/index.css
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/style/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:37:50.293902 jupyter_environment_manager-0.2.1/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2564 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/tools/create_dev_build.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2730 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/tools/stamp_pre_release.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/tsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (127)   607255 2024-05-23 20:35:35.000000 jupyter_environment_manager-0.2.1/yarn.lock
```

### Comparing `jupyter_environment_manager-0.2.0rc9/CONTRIBUTING.md` & `jupyter_environment_manager-0.2.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/LICENSE` & `jupyter_environment_manager-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/MANIFEST.in` & `jupyter_environment_manager-0.2.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/PKG-INFO` & `jupyter_environment_manager-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_environment_manager
-Version: 0.2.0rc9
+Version: 0.2.1
 Summary: JupyterLab extension for managing execution environments, packages, and kernels.
 Home-page: https://github.com/qBraid/qBraid-Lab
 Author: qBraid Development Team
 Author-email: contact@qbraid.com
 License: Proprietary
 Project-URL: Documentation, https://docs.qbraid.com/projects/lab/en/latest/lab/environments.html
 Project-URL: Bug Tracker, https://github.com/qBraid/qBraid-Lab/issues
```

### Comparing `jupyter_environment_manager-0.2.0rc9/README.md` & `jupyter_environment_manager-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/__init__.py` & `jupyter_environment_manager-0.2.1/jupyter_environment_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/_version.py` & `jupyter_environment_manager-0.2.1/jupyter_environment_manager/_version.py`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/configure.py` & `jupyter_environment_manager-0.2.1/jupyter_environment_manager/configure.py`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/devices.py` & `jupyter_environment_manager-0.2.1/jupyter_environment_manager/devices.py`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/envs_create.py` & `jupyter_environment_manager-0.2.1/jupyter_environment_manager/envs_create.py`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/envs_list.py` & `jupyter_environment_manager-0.2.1/jupyter_environment_manager/envs_list.py`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/envs_pkgs.py` & `jupyter_environment_manager-0.2.1/jupyter_environment_manager/envs_pkgs.py`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/envs_remove.py` & `jupyter_environment_manager-0.2.1/jupyter_environment_manager/envs_remove.py`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/envs_state.py` & `jupyter_environment_manager-0.2.1/jupyter_environment_manager/envs_state.py`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/handlers.py` & `jupyter_environment_manager-0.2.1/jupyter_environment_manager/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/jobs.py` & `jupyter_environment_manager-0.2.1/jupyter_environment_manager/jobs.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from pathlib import Path
 from typing import Dict, Tuple, Union
 
 import tornado
 from notebook.base.handlers import APIHandler
 from qbraid_core.services.environments import get_env_path, update_install_status, which_python
 from qbraid_core.services.quantum import quantum_lib_proxy_state
-from qbraid_core.services.quantum.proxy_braket import add_braket, disable_braket, enable_braket
+from qbraid_core.services.quantum.proxy_braket import disable_braket, enable_braket
 from qbraid_core.system.executables import python_paths_equivalent
 from qbraid_core.system.packages import (
     extract_include_sys_site_pkgs_value,
     set_include_sys_site_pkgs_value,
 )
 
 logging.basicConfig(
@@ -139,61 +139,13 @@
                 _, enabled_out = quantum_jobs_supported_enabled(slug)
                 success = enabled_in != enabled_out
                 if success:
                     message = f"Successfully {action}d Amazon Braket quantum jobs."
                 else:
                     message = f"Failed to {action} Amazon Braket quantum jobs."
 
-            update_install_status(slug_path, 1, int(success), message=message)
+            update_install_status(slug_path, 1, 1, message=message)
         except Exception as err:  # pylint: disable=broad-exception-caught
-            update_install_status(slug_path, 1, 0, message=err)
-
-            if flip_site_packages:
-                safe_set_include_sys_packages(True, cfg)
-
-    @tornado.web.authenticated
-    def post(self):
-        """Adds quantum jobs functionality to environment."""
-        input_data = self.get_json_body()
-        slug = input_data.get("slug")
-        slug_path = get_env_path(slug)
-        update_install_status(slug_path, 0, 0)
-        thread = threading.Thread(
-            target=self.add_quantum_jobs,
-            args=(
-                slug,
-                slug_path,
-            ),
-        )
-        thread.start()
-
-        data = {"success": True, "stdout": "Adding quantum jobs", "stderr": ""}
-        self.finish(json.dumps(data))
-
-    def add_quantum_jobs(self, slug: str, slug_path: Path) -> Dict[str, Union[int, str]]:
-        """Adds quantum jobs functionality using subprocess."""
-        try:
-            python_exe = which_python(slug)
-            cfg = slug_path / "pyenv" / "pyvenv.cfg"
-            flip_site_packages = flip_include_sys_packages(python_exe, cfg)
-
-            if flip_site_packages:
-                safe_set_include_sys_packages(False, cfg)
-
-            add_braket(python_exe)
-
-            if flip_site_packages:
-                safe_set_include_sys_packages(True, cfg)
-
-            _, enabled = quantum_jobs_supported_enabled(slug)
-
-            if enabled:
-                message = "Successfully added Amazon Braket quantum jobs."
-            else:
-                message = "Failed to add Amazon Braket quantum jobs."
-
-            update_install_status(slug_path, 1, int(enabled), message=message)
-        except Exception as err:  # pylint: disable=broad-exception-caught
-            update_install_status(slug_path, 1, 0, message=err)
+            update_install_status(slug_path, 1, 1, message=err)
 
             if flip_site_packages:
                 safe_set_include_sys_packages(True, cfg)
```

### Comparing `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/kernels.py` & `jupyter_environment_manager-0.2.1/jupyter_environment_manager/kernels.py`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/package.json` & `jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9778079710144927%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.df30dcda2252f4ea7597.js'}}",*

 * * "'version'": "'0.2.1'"}*

```diff
@@ -51,15 +51,15 @@
                 "jlpm"
             ]
         }
     },
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.5fd255ae2892e93a3890.js",
+            "load": "static/remoteEntry.df30dcda2252f4ea7597.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyter_environment_manager"
                 },
@@ -112,9 +112,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.2.0-rc.9"
+    "version": "0.2.1"
 }
```

### Comparing `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/0.99dd872e735721a05b18.js` & `jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/0.99dd872e735721a05b18.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/113.063bb6057d77be1f85f3.js` & `jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/113.063bb6057d77be1f85f3.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/174.7b162c87cb727f7c2712.js` & `jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/174.7b162c87cb727f7c2712.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/185.c2e096475cfee897e1f9.js` & `jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/227.bba2b52e5695cc9b34b7.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,18 +1,18 @@
 "use strict";
 (self.webpackChunk_qbraid_jupyter_environment_manager = self.webpackChunk_qbraid_jupyter_environment_manager || []).push([
-    [185], {
-        4185: (e, t, n) => {
+    [227], {
+        3227: (e, t, n) => {
             n.r(t), n.d(t, {
                 default: () => Fe
             });
-            var i = n(6880),
-                a = n(6271),
-                s = n.n(a),
-                o = n(7583),
+            var i = n(7583),
+                a = n(6880),
+                s = n(6271),
+                o = n.n(s),
                 r = n(5697),
                 l = n.n(r);
             const c = {
                 getActions: l().func,
                 getStore: l().func,
                 apiBaseUrl: l().string,
                 jupyterlab: l().any
@@ -57,17 +57,17 @@
                     "/" === e.url[0] && (e.url = `${this.alt.apiBaseUrl}${e.url}`);
                     const t = (e => {
                         const t = {
                                 domain: E
                             },
                             n = e.getStore("AuthStore").getState().user,
                             i = e.getStore("UserStore").getState().config;
-                        if (null == n ? void 0 : n.signInUserSession) t["id-token"] = n.signInUserSession.idToken.jwtToken;
-                        else if ((null == i ? void 0 : i.email) && (null == i ? void 0 : i.refreshToken)) t.email = i.email, t["refresh-token"] = i.refreshToken;
+                        if ((null == i ? void 0 : i.email) && (null == i ? void 0 : i.refreshToken)) t.email = i.email, t["refresh-token"] = i.refreshToken;
                         else if (null == i ? void 0 : i.apiKey) t["api-key"] = i.apiKey;
+                        else if (null == n ? void 0 : n.signInUserSession) t["id-token"] = n.signInUserSession.idToken.jwtToken;
                         else {
                             const e = Object.fromEntries(document.cookie.split(";").map((e => e.split("=").map((e => e.trim()))))),
                                 {
                                     EMAIL: n,
                                     REFRESH: i
                                 } = e;
                             n && i && (t.email = n, t["refresh-token"] = i)
@@ -75,45 +75,45 @@
                         return t
                     })(this.alt);
                     return Object.assign(e.header, t), e
                 }))), this.agent)
             }
 
             function S(e) {
-                return a.createElement("svg", Object.assign({
+                return s.createElement("svg", Object.assign({
                     xmlns: "http://www.w3.org/2000/svg",
                     width: "1em",
                     height: "1em",
                     viewBox: "0 0 24 24"
-                }, e), a.createElement("g", {
+                }, e), s.createElement("g", {
                     stroke: "currentColor"
-                }, a.createElement("circle", {
+                }, s.createElement("circle", {
                     cx: "12",
                     cy: "12",
                     r: "9.5",
                     fill: "none",
                     strokeLinecap: "round",
                     strokeWidth: "3"
-                }, a.createElement("animate", {
+                }, s.createElement("animate", {
                     attributeName: "stroke-dasharray",
                     calcMode: "spline",
                     dur: "1.5s",
                     keySplines: "0.42,0,0.58,1;0.42,0,0.58,1;0.42,0,0.58,1",
                     keyTimes: "0;0.475;0.95;1",
                     repeatCount: "indefinite",
                     values: "0 150;42 150;42 150;42 150"
-                }), a.createElement("animate", {
+                }), s.createElement("animate", {
                     attributeName: "stroke-dashoffset",
                     calcMode: "spline",
                     dur: "1.5s",
                     keySplines: "0.42,0,0.58,1;0.42,0,0.58,1;0.42,0,0.58,1",
                     keyTimes: "0;0.475;0.95;1",
                     repeatCount: "indefinite",
                     values: "0;-16;-59;-59"
-                })), a.createElement("animateTransform", {
+                })), s.createElement("animateTransform", {
                     attributeName: "transform",
                     dur: "2s",
                     repeatCount: "indefinite",
                     type: "rotate",
                     values: "0 12 12;360 12 12"
                 })))
             }
@@ -128,71 +128,71 @@
                     logo_class: ""
                 }, {
                     url: "https://qbraid-static.s3.amazonaws.com/logos/amd.png",
                     name: "amd",
                     logo_class: "invert"
                 }],
                 I = () => {
-                    const [e, t] = (0, a.useState)();
-                    return (0, a.useEffect)((() => {
+                    const [e, t] = (0, s.useState)();
+                    return (0, s.useEffect)((() => {
                         let e = 0;
                         t(C[e++ % C.length]);
                         const n = setInterval((() => {
                             t(C[e++ % C.length])
                         }), 1500);
                         return () => clearInterval(n)
-                    }), []), s().createElement("div", {
+                    }), []), o().createElement("div", {
                         className: null == e ? void 0 : e.name
-                    }, s().createElement("img", {
+                    }, o().createElement("img", {
                         src: null == e ? void 0 : e.url,
                         width: 200,
                         height: 40,
                         className: null == e ? void 0 : e.logo_class
                     }))
                 },
                 P = {
                     qsharp_b54crn: "qbraid.environments.qsharp"
                 };
-            class N extends a.Component {
+            class T extends s.Component {
                 constructor(e, t) {
                     super(e, t), this.toggleCollapsed = e => {
                         const {
                             isInstalled: t,
                             packageInstallingEnv: n,
                             environment: i,
                             isInstalling: a,
                             expandedEnvs: s
                         } = this.props, o = null == s ? void 0 : s.includes(e), r = n === e, l = i.sysPython;
                         a || !t || !o || r || l || this.props.flux.getActions("EnvironmentActions").updatePackagesList(e).catch((e => {
                             console.log("Error at update package in toggle collapsed at envTile ", e)
                         })), this.props.onToggleExpand(e)
-                    }, this.renderVerifyLoader = () => s().createElement(v.Box, {
+                    }, this.renderVerifyLoader = () => o().createElement(v.Box, {
                         position: "absolute",
                         width: "100%",
                         height: "100%",
                         className: "env_verification-loader",
                         display: "flex",
                         flexDirection: "column",
                         alignItems: "center",
                         justifyContent: "center",
                         gap: 3,
                         sx: {
                             cursor: "wait"
                         }
-                    }, s().createElement(I, null), s().createElement(v.Stack, {
+                    }, o().createElement(I, null), o().createElement(v.Stack, {
                         flexDirection: "row",
                         gap: 1
-                    }, s().createElement(S, {
+                    }, o().createElement(S, {
                         width: 20,
                         height: 20,
                         className: "env_loader"
-                    }), s().createElement(v.Typography, {
+                    }), o().createElement(v.Typography, {
                         fontSize: 14,
                         color: "text.primary"
-                    }, "Verifying GPU configuration..."))), this.renderTags = () => this.props.environment.tags.map(((e, t) => s().createElement("p", {
+                    }, "Verifying GPU configuration..."))), this.renderTags = () => this.props.environment.tags.map(((e, t) => o().createElement("p", {
                         key: t,
                         className: "env-tag"
                     }, e))), this.state = {
                         collapsed: !0,
                         lockedTile: !0
                     }
                 }
@@ -217,352 +217,435 @@
                             lockedTile: !1
                         }) : Object.assign(Object.assign({}, t), {
                             lockedTile: !0
                         })
                     }
                 }
                 render() {
-                    var e, t, n, i, a, o, r, l, c, m, g, u;
+                    var e, t, n, i, a, s, r, l, c, m, g, u;
                     let b = this.props.environment,
                         {
                             user: f
                         } = this.props.qbUser,
                         x = {};
-                    return this.props.isActive && (x.backgroundColor = "#dad4e7", x.border = "1px solid #673ab7"), this.state.lockedTile && (x.border = "none"), this.props.isNewEnv || (null === (e = this.props.expandedEnvs) || void 0 === e ? void 0 : e.includes(b._id)) ? (x.maxHeight = 9999, x.padding = "0 10px 60px 10px") : (x.maxHeight = 0, x.padding = "0 10px 40px 10px"), s().createElement("div", {
+                    return this.props.isActive && (x.backgroundColor = "#dad4e7", x.border = "1px solid #673ab7"), this.state.lockedTile && (x.border = "none"), this.props.isNewEnv || (null === (e = this.props.expandedEnvs) || void 0 === e ? void 0 : e.includes(b._id)) ? (x.maxHeight = 9999, x.padding = "0 10px 60px 10px") : (x.maxHeight = 0, x.padding = "0 10px 40px 10px"), o().createElement("div", {
                         className: "env-tile",
                         style: Object.assign({}, x)
-                    }, s().createElement("div", {
+                    }, o().createElement("div", {
                         className: `env-name flex-box ${(this.props.isNewEnv||(null===(t=this.props.expandedEnvs)||void 0===t?void 0:t.includes(b._id)))&&"env-name-border"}`,
                         style: {
                             color: this.props.isActive ? "black" : "var(--jp-ui-font-color0)"
                         }
-                    }, s().createElement("span", {
+                    }, o().createElement("span", {
                         className: "env-tile-display-name flex-box_start",
                         style: {
                             cursor: "pointer"
                         },
                         onClick: () => this.toggleCollapsed(b._id)
-                    }, (null == b ? void 0 : b.logo) && "object" == typeof(null == b ? void 0 : b.logo) && !Array.isArray(null == b ? void 0 : b.logo) && null !== (null == b ? void 0 : b.logo) ? s().createElement("span", {
+                    }, (null == b ? void 0 : b.logo) && "object" == typeof(null == b ? void 0 : b.logo) && !Array.isArray(null == b ? void 0 : b.logo) && null !== (null == b ? void 0 : b.logo) ? o().createElement("span", {
                         onClick: () => this.toggleCollapsed(b._id)
-                    }, s().createElement("img", {
+                    }, o().createElement("img", {
                         style: {
                             height: 18,
                             maxWidth: 45,
                             marginRight: 5
                         },
                         src: (null === (n = null == this ? void 0 : this.props) || void 0 === n ? void 0 : n.isDarkTheme) ? b.logo.dark : b.logo.light
-                    })) : s().createElement("span", {
+                    })) : o().createElement("span", {
                         onClick: () => this.toggleCollapsed(b._id)
-                    }, s().createElement("img", {
+                    }, o().createElement("img", {
                         key: 0,
                         style: {
                             height: 18,
                             maxWidth: 45,
                             marginRight: 5
                         },
-                        src: localStorage.getItem(b.displayName) || (null === (i = null == this ? void 0 : this.props) || void 0 === i ? void 0 : i.isDarkTheme) ? null === (a = null == b ? void 0 : b.logo) || void 0 === a ? void 0 : a.dark : null === (o = null == b ? void 0 : b.logo) || void 0 === o ? void 0 : o.light
-                    })), s().createElement("p", {
+                        src: localStorage.getItem(b.displayName) || (null === (i = null == this ? void 0 : this.props) || void 0 === i ? void 0 : i.isDarkTheme) ? null === (a = null == b ? void 0 : b.logo) || void 0 === a ? void 0 : a.dark : null === (s = null == b ? void 0 : b.logo) || void 0 === s ? void 0 : s.light
+                    })), o().createElement("p", {
                         className: "env-tile-display-name"
-                    }, b.displayName), this.state.lockedTile && s().createElement(v.Tooltip, {
+                    }, b.displayName), this.state.lockedTile && o().createElement(v.Tooltip, {
                         title: this.props.isInstalled ? "Upgrade to access environment" : "Upgrade to install environment",
                         arrow: !0
-                    }, s().createElement(p.Z, {
+                    }, o().createElement(p.Z, {
                         sx: {
                             fontSize: "1rem!important",
                             color: "var(--jp-ui-font-color0)",
                             marginLeft: "5px",
                             zIndex: "99",
                             cursor: "pointer"
                         }
-                    }))), s().createElement("span", {
+                    }))), o().createElement("span", {
                         className: "env-tile_right-flex-box"
-                    }, this.props.isActive && s().createElement("span", {
+                    }, this.props.isActive && o().createElement("span", {
                         className: "env-tile-active-label"
-                    }, "active"), s().createElement("img", {
+                    }, "active"), o().createElement("img", {
                         src: b.pinned ? "https://qbraid-static.s3.amazonaws.com/bookmark-solid-pink.svg" : "https://qbraid-static.s3.amazonaws.com/bookmark-solid-gray.svg",
                         style: {
                             width: 15,
                             height: 15,
                             cursor: this.state.lockedTile ? "not-allowed" : "pointer"
                         },
                         onClick: () => {
                             this.state.lockedTile || this.props.onTogglePinned(b._id)
                         }
-                    }), s().createElement(d.Z, {
+                    }), o().createElement(d.Z, {
                         sx: {
                             fontSize: "1rem!important",
                             transform: this.props.isNewEnv || (null === (r = this.props.expandedEnvs) || void 0 === r ? void 0 : r.includes(b._id)) ? "rotateX(180deg)" : "rotateX(0deg)",
                             transition: "transform 300ms ease",
                             cursor: "pointer",
                             zIndex: "99"
                         },
                         onClick: () => this.toggleCollapsed(b._id)
-                    }))), s().createElement("span", {
+                    }))), o().createElement("span", {
                         style: {
                             visibility: this.props.isNewEnv || (null === (l = this.props.expandedEnvs) || void 0 === l ? void 0 : l.includes(b._id)) ? "visible" : "hidden"
                         }
-                    }, s().createElement("div", {
+                    }, o().createElement("div", {
                         className: "env-content"
-                    }, (null === (m = null === (c = this.props) || void 0 === c ? void 0 : c.verifyLoading) || void 0 === m ? void 0 : m.loading) && (null === (u = null === (g = this.props) || void 0 === g ? void 0 : g.verifyLoading) || void 0 === u ? void 0 : u.envId) === b._id && this.renderVerifyLoader(), s().createElement("div", {
+                    }, (null === (m = null === (c = this.props) || void 0 === c ? void 0 : c.verifyLoading) || void 0 === m ? void 0 : m.loading) && (null === (u = null === (g = this.props) || void 0 === g ? void 0 : g.verifyLoading) || void 0 === u ? void 0 : u.envId) === b._id && this.renderVerifyLoader(), o().createElement("div", {
                         className: "env-tags"
-                    }, s().createElement("div", null, this.renderTags()), s().createElement("div", null, s().createElement(v.Tooltip, {
+                    }, o().createElement("div", null, this.renderTags()), o().createElement("div", null, o().createElement(v.Tooltip, {
                         title: "Clone",
                         arrow: !0
-                    }, s().createElement(h.Z, {
+                    }, o().createElement(h.Z, {
                         onClick: () => {
                             this.state.lockedTile || this.props.cloneEnvironment(b)
                         },
                         sx: {
                             cursor: this.state.lockedTile ? "not-allowed" : "pointer",
                             color: "gray",
                             fontSize: "1.5em"
                         }
-                    })))), s().createElement("div", {
+                    })))), o().createElement("div", {
                         className: "env-details"
-                    }, s().createElement("p", {
+                    }, o().createElement("p", {
                         className: "env-description",
                         style: {
                             color: this.props.isActive ? "rgba(0, 0, 0, 0.54)" : "var(--jp-ui-font-color2)"
                         }
-                    }, b.description || "No description"), this.props.packageInstallingEnv === b._id && this.props.packageProgress > 0 ? s().createElement("div", null, s().createElement("div", {
+                    }, b.description || "No description"), this.props.packageInstallingEnv === b._id && this.props.packageProgress > 0 ? o().createElement("div", null, o().createElement("div", {
                         style: {
                             display: "flex",
                             justifyContent: "flex-start",
                             alignItems: "center"
                         }
-                    }, s().createElement("img", {
+                    }, o().createElement("img", {
                         src: "https://qbraid-static.s3.amazonaws.com/python.svg",
                         style: {
                             width: "20px",
                             height: "20px"
                         }
-                    }), s().createElement("p", {
+                    }), o().createElement("p", {
                         className: "env-packages",
                         style: {
                             color: this.props.isActive ? "black" : "var(--jp-ui-font-color1)"
                         }
-                    }, "Installing Packages...")), s().createElement("div", {
+                    }, "Installing Packages...")), o().createElement("div", {
                         style: {
                             marginTop: "5px"
                         }
-                    }, s().createElement(v.LinearProgress, {
+                    }, o().createElement(v.LinearProgress, {
                         variant: "determinate",
                         sx: {
                             backgroundColor: "#edcefd",
                             "& .MuiLinearProgress-bar": {
                                 backgroundColor: "#673ab7"
                             }
                         },
                         value: this.props.packageProgress
-                    }))) : s().createElement("div", {
+                    }))) : o().createElement("div", {
                         className: "env-config"
-                    }, s().createElement("p", {
+                    }, o().createElement("p", {
                         className: "env-packages",
                         style: {
                             color: this.props.isActive ? "black" : "var(--jp-ui-font-color1)"
                         }
-                    }, s().createElement("span", {
+                    }, o().createElement("span", {
                         style: {
                             verticalAlign: "middle"
                         }
-                    }, s().createElement("img", {
+                    }, o().createElement("img", {
                         src: "https://qbraid-static.s3.amazonaws.com/python.svg"
-                    })), s().createElement("span", null, `${b.packagesInImage.length} packages`))))), s().createElement("div", {
+                    })), o().createElement("span", null, `${b.packagesInImage.length} ${1===b.packagesInImage.length?"package":"packages"}`))))), o().createElement("div", {
                         className: "env-actions"
-                    }, this.state.lockedTile ? s().createElement("p", {
+                    }, this.state.lockedTile ? o().createElement("p", {
                         className: "env-action",
                         style: {
                             width: "100%",
                             marginRight: 10,
                             background: "#673AB7",
                             cursor: "pointer",
                             zIndex: "100"
                         },
                         onClick: () => {
                             window.open(`${y}/billing`, "_blank")
                         }
-                    }, "Upgrade") : this.props.activateButton, s().createElement("p", {
+                    }, "Upgrade") : this.props.activateButton, o().createElement("p", {
                         className: `env-action env-button-outlined ${this.props.isActive&&"kernel-activated-button"}`,
                         onClick: this.props.edit
                     }, "More..."))))
                 }
             }
-            N.contextTypes = c;
-            var T = n(1858);
-            g()(T.Z, {
+            T.contextTypes = c;
+            var N = n(1858);
+            g()(N.Z, {
                 insert: "head",
                 singleton: !1
-            }), T.Z.locals;
-            const j = ({
+            }), N.Z.locals;
+            const O = ({
                 width: e,
                 height: t,
                 color: n
-            }) => s().createElement("svg", {
+            }) => o().createElement("svg", {
                 width: e,
                 height: t,
                 viewBox: "0 0 34 34",
                 fill: "none",
                 xmlns: "http://www.w3.org/2000/svg"
-            }, s().createElement("path", {
+            }, o().createElement("path", {
                 d: "M32.2501 32.25L25.1472 25.1345M29.0834 15.625C29.0834 19.1944 27.6655 22.6176 25.1416 25.1415C22.6176 27.6654 19.1945 29.0833 15.6251 29.0833C12.0557 29.0833 8.63253 27.6654 6.1086 25.1415C3.58468 22.6176 2.16675 19.1944 2.16675 15.625C2.16675 12.0556 3.58468 8.63245 6.1086 6.10852C8.63253 3.5846 12.0557 2.16667 15.6251 2.16667C19.1945 2.16667 22.6176 3.5846 25.1416 6.10852C27.6655 8.63245 29.0834 12.0556 29.0834 15.625V15.625Z",
                 stroke: n,
                 strokeWidth: "3",
                 strokeLinecap: "round"
             }));
-            j.defaultProps = {
+            O.defaultProps = {
                 width: "16",
                 height: "16",
                 color: "#ABABAB"
             };
-            const U = j,
-                O = e => s().createElement("svg", {
+            const j = O,
+                U = e => o().createElement("svg", {
                     width: e.width,
                     height: e.height,
                     style: {
                         minHeight: e.height,
                         minWidth: e.width,
                         filter: e.filter
                     },
                     viewBox: "0 0 37.5 35.624999",
                     xmlns: "http://www.w3.org/2000/svg"
-                }, s().createElement("g", {
+                }, o().createElement("g", {
                     transform: "translate(-592.72335,-420.20756)"
-                }, s().createElement("g", {
+                }, o().createElement("g", {
                     transform: "matrix(0.5935466,0,0,0.59354645,250.33305,172.30823)"
-                }, s().createElement("g", {
+                }, o().createElement("g", {
                     transform: "translate(-67.857146,-23.035712)"
-                }, s().createElement("path", {
+                }, o().createElement("path", {
                     fill: "#f3f3f0",
                     fillOpacity: "1",
                     stroke: "#c4c4c4",
                     strokeWidth: "0.355076",
                     strokeLinejoin: "bevel",
                     strokeMiterlimit: "4",
                     d: "m 660.75803,449.15562 15.55544,5.66172 15.78565,-5.74552 -15.55544,-5.66172 z"
-                }), s().createElement("path", {
+                }), o().createElement("path", {
                     fill: "#ffffff",
                     fillOpacity: "1",
                     stroke: "#c4c4c4",
                     strokeWidth: "0.355076",
                     strokeLinejoin: "bevel",
                     strokeMiterlimit: "4",
                     d: "m 676.31347,454.81734 v 18.28268 l 15.78565,-5.74551 v -18.28269 z"
-                }), s().createElement("path", {
+                }), o().createElement("path", {
                     fill: "#e7e6e2",
                     fillOpacity: "1",
                     stroke: "#c4c4c4",
                     strokeWidth: "0.355076",
                     strokeLinejoin: "bevel",
                     strokeMiterlimit: "4",
                     d: "m 660.75803,449.15562 15.55544,5.66172 v 18.28268 l -15.55544,-5.66171 z"
-                })), s().createElement("g", {
+                })), o().createElement("g", {
                     transform: "translate(-83.545471,1.0197198)"
-                }, s().createElement("path", {
+                }, o().createElement("path", {
                     fill: "#f3f3f0",
                     fillOpacity: "1",
                     stroke: "#c4c4c4",
                     strokeWidth: "0.355076",
                     strokeLinejoin: "bevel",
                     strokeMiterlimit: "4",
                     d: "m 660.75803,449.15562 15.55544,5.66172 15.78565,-5.74552 -15.55544,-5.66172 z"
-                }), s().createElement("path", {
+                }), o().createElement("path", {
                     fill: "#ffffff",
                     fillOpacity: "1",
                     stroke: "#c4c4c4",
                     strokeWidth: "0.355076",
                     strokeLinejoin: "bevel",
                     strokeMiterlimit: "4",
                     d: "m 676.31347,454.81734 v 18.28268 l 15.78565,-5.74551 v -18.28269 z"
-                }), s().createElement("path", {
+                }), o().createElement("path", {
                     id: "path271",
                     fill: "#e7e6e2",
                     fillOpacity: "1",
                     stroke: "#c4c4c4",
                     strokeWidth: "0.355076",
                     strokeLinejoin: "bevel",
                     strokeMiterlimit: "4",
                     d: "m 660.75803,449.15562 15.55544,5.66172 v 18.28268 l -15.55544,-5.66171 z"
-                })), s().createElement("g", {
+                })), o().createElement("g", {
                     transform: "translate(-52.377998,1.0197198)"
-                }, s().createElement("path", {
+                }, o().createElement("path", {
                     fill: "#f3f3f0",
                     fillOpacity: "1",
                     stroke: "#c4c4c4",
                     strokeWidth: "0.355076",
                     strokeLinejoin: "bevel",
                     strokeMiterlimit: "4",
                     d: "m 660.75803,449.15562 15.55544,5.66172 15.78565,-5.74552 -15.55544,-5.66172 z"
-                }), s().createElement("path", {
+                }), o().createElement("path", {
                     fill: "#ffffff",
                     fillOpacity: "1",
                     stroke: "#c4c4c4",
                     strokeWidth: "0.355076",
                     strokeLinejoin: "bevel",
                     strokeMiterlimit: "4",
                     d: "m 676.31347,454.81734 v 18.28268 l 15.78565,-5.74551 v -18.28269 z"
-                }), s().createElement("path", {
+                }), o().createElement("path", {
                     fill: "#e7e6e2",
                     fillOpacity: "1",
                     stroke: "#c4c4c4",
                     strokeWidth: "0.355076",
                     strokeLinejoin: "bevel",
                     strokeMiterlimit: "4",
                     d: "m 660.75803,449.15562 15.55544,5.66172 v 18.28268 l -15.55544,-5.66171 z"
                 })))));
-            O.defaultProps = {
+            U.defaultProps = {
                 width: "34",
                 height: "36",
                 filter: "none"
             };
-            const L = O;
+            const L = U;
             var z = n(9845);
 
-            function _(e) {
-                return a.createElement("svg", Object.assign({
+            function q(e) {
+                return s.createElement("svg", Object.assign({
                     xmlns: "http://www.w3.org/2000/svg",
                     width: "1em",
                     height: "1em",
                     viewBox: "0 0 24 24"
-                }, e), a.createElement("path", {
+                }, e), s.createElement("path", {
                     fill: "none",
                     stroke: "currentColor",
                     strokeDasharray: "24",
                     strokeDashoffset: "24",
                     strokeLinecap: "round",
                     strokeLinejoin: "round",
                     strokeWidth: "2",
                     d: "M5 11L11 17L21 7"
-                }, a.createElement("animate", {
+                }, s.createElement("animate", {
                     fill: "freeze",
                     attributeName: "stroke-dashoffset",
                     dur: "0.4s",
                     values: "24;0"
                 })))
             }
-            var D = n(6486),
-                q = n.n(D);
-            const B = 2500,
+            var B = n(6486),
+                _ = n.n(B);
+            const D = (0, v.styled)(v.Slider)((e => {
+                var {
+                    theme: t
+                } = e, n = function(e, t) {
+                    var n = {};
+                    for (var i in e) Object.prototype.hasOwnProperty.call(e, i) && t.indexOf(i) < 0 && (n[i] = e[i]);
+                    if (null != e && "function" == typeof Object.getOwnPropertySymbols) {
+                        var a = 0;
+                        for (i = Object.getOwnPropertySymbols(e); a < i.length; a++) t.indexOf(i[a]) < 0 && Object.prototype.propertyIsEnumerable.call(e, i[a]) && (n[i[a]] = e[i[a]])
+                    }
+                    return n
+                }(e, ["theme"]);
+                return {
+                    color: t.palette.primary.main,
+                    height: 5,
+                    marginBottom: 0,
+                    marginTop: 25,
+                    [`& .${v.sliderClasses.rail}`]: {},
+                    [`& .${v.sliderClasses.track}`]: {
+                        border: "none",
+                        backgroundColor: "error" === n.color ? t.palette.error.main : t.palette.success.main
+                    },
+                    [`& .${v.sliderClasses.thumb}`]: {
+                        display: "none"
+                    },
+                    [`& .${v.sliderClasses.markLabel}`]: {
+                        top: "-20px",
+                        fontSize: 12,
+                        padding: "1px 8px",
+                        borderRadius: "4px",
+                        color: t.palette.common.white,
+                        backgroundColor: t.palette.text.disabled
+                    },
+                    [`& .${v.sliderClasses.markLabelActive}`]: {
+                        color: t.palette.common.white,
+                        backgroundColor: "error" === n.color ? t.palette.error.main : t.palette.success.main
+                    },
+                    [`& [data-index="0"].${v.sliderClasses.markLabel}`]: {
+                        left: "9%!important"
+                    },
+                    [`& [data-index="2"].${v.sliderClasses.markLabel}`]: {
+                        left: "94%!important"
+                    },
+                    [`& .${v.sliderClasses.mark}`]: {
+                        width: 10,
+                        height: 10,
+                        borderRadius: "100vw",
+                        backgroundColor: t.palette.text.disabled,
+                        outlineColor: t.palette.text.disabled,
+                        outlineWidth: "1px",
+                        outlineStyle: "solid",
+                        outlineOffset: "4px"
+                    },
+                    [`& .${v.sliderClasses.markActive}`]: {
+                        backgroundColor: "error" === n.color ? t.palette.error.main : t.palette.success.main,
+                        outlineColor: "error" === n.color ? t.palette.error.main : t.palette.success.main
+                    }
+                }
+            }));
+
+            function M({
+                env: e
+            }) {
+                const t = [{
+                    label: "Requested",
+                    value: 0
+                }, {
+                    label: "Under Review",
+                    value: 50
+                }, {
+                    label: "denied" === (null == e ? void 0 : e.reviewStatus) ? "Denied" : "Published",
+                    value: 100
+                }];
+                return o().createElement(D, {
+                    valueLabelDisplay: "off",
+                    defaultValue: (n = null == e ? void 0 : e.visibility, i = null == e ? void 0 : e.reviewStatus, "public" === n && "approved" === i ? 100 : "private" === n && "pending" === i ? 50 : "private" === n && "requested" === i ? 1 : "private" === n && "denied" === i ? 100 : 0),
+                    step: 33.33,
+                    color: "denied" === (null == e ? void 0 : e.reviewStatus) ? "error" : "success",
+                    marks: t,
+                    disabled: !0
+                });
+                var n, i
+            }
+            const R = "62e88a24b996354861298ab2",
                 F = {
                     qsharp_b54crn: "qbraid.environments.qsharp"
                 };
 
-            function M(e) {
+            function W(e) {
                 return new Date(e).toLocaleString("en-US", {
                     year: "numeric",
                     month: "2-digit",
                     day: "2-digit",
                     hour: "2-digit",
                     minute: "2-digit",
                     hour12: !1,
                     timeZone: "UTC"
                 })
             }
-            class R extends a.Component {
+            class G extends s.Component {
                 constructor(e, t) {
-                    var n, i, a, o, r, l;
+                    var n, i, a, s, r, l;
                     super(e, t), this.load = () => this.setState({
                         loaded: !0
                     }), this.shareEnvironment = e => {
                         this.setState({
                             shareEmailBtnDis: !0
                         });
                         let t = {
@@ -580,28 +663,28 @@
                                 }
                             }), setTimeout((() => {
                                 this.setState({
                                     shareSuccess: !1,
                                     shareEmail: "",
                                     shareEmailBtnDis: !1
                                 })
-                            }), B)), 202 === t.status && (this.setState({
+                            }), 2500)), 202 === t.status && (this.setState({
                                 shareSuccess: !0,
                                 sharePopupOpen: !0,
                                 sharePopupMsg: {
                                     msg: "Environment Sharing Started",
                                     type: "success"
                                 }
                             }), setTimeout((() => {
                                 this.setState({
                                     shareEmail: "",
                                     shareEmailBtnDis: !1,
                                     shareSuccess: !1
                                 })
-                            }), B)), 304 !== t.status || e || this.setState({
+                            }), 2500)), 304 !== t.status || e || this.setState({
                                 resharePopUp: !0,
                                 resharePopUpContent: {
                                     content: "reShareEnv",
                                     title: "Update Shared Environment?",
                                     body: `You have already shared this environment with ${this.state.shareEmail?`${this.state.shareEmail}, or another user`:"one or more users"}. Would you like to update the existing version? Doing so will overwrite the globally shared environment, but will not affect any local copies that users have already installed.`
                                 }
                             })
@@ -637,14 +720,129 @@
                                 sharePopupOpen: !0,
                                 sharePopupMsg: {
                                     msg: t,
                                     type: "error"
                                 }
                             })
                         }))
+                    }, this.requestPublishEnvironment = () => {
+                        if (!this.state.isCustom) return void this.setState({
+                            sharePopupOpen: !0,
+                            sharePopupMsg: {
+                                msg: "Only custom environment can be published",
+                                type: "error"
+                            }
+                        });
+                        if (this.state.uninstalling || this.state.cancelling || this.state.deleting || this.props.installing || this.props.packageInstallingEnv === this.props.env._id) return void this.setState({
+                            sharePopupOpen: !0,
+                            sharePopupMsg: {
+                                msg: "Blocked during state transition",
+                                type: "error"
+                            }
+                        });
+                        this.setState({
+                            publishLoading: !0
+                        });
+                        let e = {
+                            environmentId: this.props.env._id,
+                            collabEmail: "contact@qbraid.com",
+                            overwrite: !0
+                        };
+                        this.context.getActions("EnvironmentActions").shareEnvironment(e).then((e => {
+                            200 !== e.status && 202 !== e.status || (this.setState({
+                                sharePopupOpen: !0,
+                                sharePopupMsg: {
+                                    msg: "Submitting your request! Please wait...",
+                                    type: "success"
+                                }
+                            }), this.context.getActions("EnvironmentActions").updatePublishStatus(this.props.env.slug, "requested").then((e => {
+                                200 === (null == e ? void 0 : e.status) && this.setState({
+                                    sharePopupOpen: !0,
+                                    sharePopupMsg: {
+                                        msg: "Successfully Requested to publish",
+                                        type: "success"
+                                    }
+                                })
+                            })))
+                        })).then((() => {
+                            this.props.flux.getActions("EnvironmentActions").updateAll().then((() => {
+                                this.props.updateReadUserAccessData(this.props.env._id), this.props.flux.getActions("EnvironmentActions").registerInstalled().then((() => {
+                                    this.setState({
+                                        publishLoading: !1
+                                    })
+                                }))
+                            }))
+                        })).catch((e => {
+                            console.warn(e), this.setState({
+                                sharePopupOpen: !0,
+                                sharePopupMsg: {
+                                    msg: "Request to publish failed",
+                                    type: "error"
+                                },
+                                publishLoading: !1
+                            })
+                        }))
+                    }, this.denyPublishingEnvironment = () => {
+                        this.state.isMount && ("contact@qbraid.com" === this.state.user.email ? this.props.flux.getActions("EnvironmentActions").updatePublishStatus(this.props.env.slug, "denied").then((e => {
+                            200 === e.status && this.setState({
+                                sharePopupOpen: !0,
+                                sharePopupMsg: {
+                                    msg: "Publishing request denied!",
+                                    type: "error"
+                                }
+                            })
+                        })).then((() => {
+                            this.props.flux.getActions("EnvironmentActions").updateAll().then((() => {
+                                this.props.flux.getActions("EnvironmentActions").registerInstalled()
+                            }))
+                        })).catch((e => {
+                            console.warn(e), this.setState({
+                                sharePopupOpen: !0,
+                                sharePopupMsg: {
+                                    msg: "Publish failed",
+                                    type: "error"
+                                },
+                                publishLoading: !1
+                            })
+                        })) : this.setState({
+                            sharePopupOpen: !0,
+                            sharePopupMsg: {
+                                msg: "Only contact@qbraid.com can deny publishing this environment",
+                                type: "error"
+                            }
+                        }))
+                    }, this.publishEnvironment = () => {
+                        this.state.isMount && ("contact@qbraid.com" === this.state.user.email ? this.props.flux.getActions("EnvironmentActions").publishEnvironment(this.props.env.slug).then((e => {
+                            200 === e.status && this.setState({
+                                sharePopupOpen: !0,
+                                sharePopupMsg: {
+                                    msg: "Environment published successfully",
+                                    type: "success"
+                                }
+                            })
+                        })).then((() => {
+                            this.props.flux.getActions("EnvironmentActions").updateAll().then((() => {
+                                this.props.flux.getActions("EnvironmentActions").registerInstalled()
+                            }))
+                        })).catch((e => {
+                            console.warn(e), this.setState({
+                                sharePopupOpen: !0,
+                                sharePopupMsg: {
+                                    msg: "Publish failed",
+                                    type: "error"
+                                },
+                                publishLoading: !1
+                            })
+                        })) : this.setState({
+                            sharePopupOpen: !0,
+                            sharePopupMsg: {
+                                msg: "Only contact@qbraid.com can publish environment",
+                                type: "error"
+                            }
+                        }))
                     }, this.toggleWriteAccess = e => {
                         let {
                             readAccessUsers: t,
                             writeAccessUsers: n
                         } = this.state;
                         return e.write ? (delete e.write, t = t.filter((t => t._id !== e._id)), t.push(e), n = n.filter((t => t._id !== e._id)), this.setState({
                             readAccessUsers: t,
@@ -721,34 +919,39 @@
                                 packages: [e],
                                 upgradePip: !1,
                                 systemSitePackages: null === (t = this.props.env.systemSitePackages) || void 0 === t || t
                             },
                             i = `Error installing package ${e}.`;
                         try {
                             const t = await this.context.getActions("EnvironmentActions").installPackagesPyvenv(n);
-                            !t || 200 !== t.status && 202 !== t.status || (this.props.setPackageInstallingEnv(this.props.env._id), await this.registerInstalling(e, i, void 0) && this.updateCustomPackageListInMongo())
+                            !t || 200 !== t.status && 202 !== t.status || (this.props.setPackageInstallingEnv(this.props.env._id), await this.registerInstalling(e, i, void 0) && this.updateCustomPackageListInMongo(), e.startsWith("amazon-braket-sdk") && this.setState({
+                                quantumJobs: !0
+                            }))
                         } catch (e) {
                             this.props.finishPackageInstalling(), console.log(e), alert(i)
                         }
                     }, this.removePackage = e => {
                         this.setState({
                             loadingPackages: !1
                         });
                         const t = e.split(/(==|~=|<|<=|>|>=)/)[0],
                             n = this.props.env.slug;
                         if (!t || !n) return void alert("Failed to uninstall package: environment slug or package name not found");
                         const i = {
                             slug: n,
                             package: t
                         };
-                        return new Promise((t => {
-                            this.props.flux.getActions("EnvironmentActions").uninstallPackagePyvenv(i).then((n => {
-                                202 === n ? (this.setState({
+                        return new Promise((n => {
+                            this.props.flux.getActions("EnvironmentActions").uninstallPackagePyvenv(i).then((i => {
+                                202 === i ? ("amazon-braket-sdk" !== t && "botocore" !== t || this.setState({
+                                    quantumJobs: !1,
+                                    quantumJobsEnabled: !1
+                                }), this.setState({
                                     packagesInImage: this.state.packagesInImage.filter((t => t !== e))
-                                }), t(!0)) : reject(n)
+                                }), n(!0)) : reject(i)
                             })).catch((e => {
                                 reject(e)
                             }))
                         }))
                     }, this.handleRemovePkg = async e => {
                         const t = e.split("==")[0];
                         await this.removePackage(e) ? (this.setState({
@@ -769,15 +972,15 @@
                         if (this.state.isCustom) {
                             const n = (await this.context.getActions("EnvironmentActions").fetchAllEnv()).filter((e => e.slug === c.slug))[0];
                             this.comparePackageList(n) || await this.context.getActions("EnvironmentActions").updateCustomPackageListInMongoDB({
                                 slug: null === (t = null === (e = null == this ? void 0 : this.props) || void 0 === e ? void 0 : e.env) || void 0 === t ? void 0 : t.slug,
                                 packageList: this.state.packagesInImage
                             })
                         }
-                    }, this.comparePackageList = e => q().isEqual(null == e ? void 0 : e.packagesInImage, this.state.packagesInImage), this.handleChangePackageFilter = (e, t) => {
+                    }, this.comparePackageList = e => _().isEqual(null == e ? void 0 : e.packagesInImage, this.state.packagesInImage), this.handleChangePackageFilter = (e, t) => {
                         this.setState({
                             packageFilter: e.target.value.trim().toLowerCase()
                         }, (() => {
                             "" !== this.state.packageFilter && this.props.env.installed && (0 !== this.state.packagesInImage.filter((e => -1 !== e.split("=")[0].toLowerCase().trim().indexOf(this.state.packageFilter.replaceAll("-", "")))).length || this.props.env.isPreInstalled || (this.setState({
                                 addPackageDialogOpen: !0,
                                 packageListLoading: !0,
                                 searchInput: this.state.packageFilter
@@ -887,15 +1090,15 @@
                                 availableVersions: Object.keys(e.releases).map((e => e.replace(/\d+/g, (e => +e + 1e5)))).sort().reverse().map((e => e.replace(/\d+/g, (e => +e - 1e5))))
                             })
                         })).then((e => {
                             const t = this.state.packagesInImage.filter((e => {
                                 var t, n;
                                 return e.includes(null === (n = null === (t = this.state.searchResults) || void 0 === t ? void 0 : t.info) || void 0 === n ? void 0 : n.name)
                             }))[0];
-                            q().isEmpty(t) ? this.setState({
+                            _().isEmpty(t) ? this.setState({
                                 selectedPkgVersion: "any"
                             }) : this.setState({
                                 selectedPkgVersion: t.split("==")[1]
                             })
                         })).catch((e => (this.setState({
                             searchResults: {},
                             selectedPkgVersion: "",
@@ -916,15 +1119,15 @@
                         this.setState({
                             searchInput: e.target.value
                         }), this.handleChangePackageFilter(e, !0), this.state.searchInput.length <= 3 && this.setState({
                             isDropdownVisible: !1
                         })
                     }, this.handleAddPackageToList = async e => {
                         var t, n;
-                        if (!q().isEmpty(this.state.selectedPkg)) {
+                        if (!_().isEmpty(this.state.selectedPkg)) {
                             this.setState({
                                 pkgListBusy: !0
                             }), this.closeAddPackageDialog();
                             let i = e;
                             const a = /(==|~=|<|<=|>|>=)/,
                                 s = /[\d|,|.|e|E|\+]+/g,
                                 o = this.state.packagesInImage.map((e => {
@@ -1025,28 +1228,35 @@
                                 }
                             })
                         }), 2500)
                     }, this.handleQuantumJobsToggle = () => {
                         if (this.state.lockedEnv) return null;
                         if (this.props.env) {
                             const e = this.state.quantumJobsEnabled;
-                            this.context.getActions("EnvironmentActions").toggleQuantumJobs({
+                            this.setState({
+                                pkgListBusy: !0
+                            }), this.context.getActions("EnvironmentActions").toggleQuantumJobs({
                                 slug: this.props.env.slug,
                                 action: this.state.quantumJobsEnabled ? "disable" : "enable"
                             }).then((t => {
-                                t.success && (this.setState({
-                                    quantumJobsEnabled: !e,
+                                const {
+                                    success: n
+                                } = t, i = {
+                                    pkgListBusy: !1,
+                                    quantumJobsEnabled: n ? !e : e,
                                     qjobsStatus: {
                                         open: !0,
-                                        error: !1,
-                                        message: e ? "Disabled" : "Enabled"
+                                        error: !n,
+                                        message: n ? e ? "Disabled" : "Enabled" : e ? "Enabled" : "Disabled"
                                     }
-                                }), this.resetQjobsStatus())
+                                };
+                                this.setState(i), this.resetQjobsStatus()
                             })).catch((e => {
                                 console.log("Quantum Jobs Toggle Error: ", e), this.setState({
+                                    pkgListBusy: !1,
                                     qjobsStatus: {
                                         open: !0,
                                         error: !0,
                                         message: "Error: failed to enable Quantum Jobs"
                                     }
                                 }), this.resetQjobsStatus()
                             }))
@@ -1083,73 +1293,73 @@
                             uninstallAlert: !1
                         }), this.handleExtraUninsConfirmOpen()) : this.handleUninstall()
                     }, this.handleCancelReq = () => {
                         this.setState({
                             cancelRequest: !0
                         }), this.handleUninstallAlertOpen()
                     }, this.renderEditTags = () => {
-                        if (this.state.isOwner) return this.state.editOpen ? s().createElement(s().Fragment, null, s().createElement(v.Tooltip, {
+                        if (this.state.isOwner) return this.state.editOpen ? o().createElement(o().Fragment, null, o().createElement(v.Tooltip, {
                             title: "Turn editing tags off"
-                        }, s().createElement(z.EditOff, {
+                        }, o().createElement(z.EditOff, {
                             className: "env-edit-icon",
                             onClick: this.handleEditState
-                        })), this.renderAddTags()) : s().createElement(v.Tooltip, {
+                        })), this.renderAddTags()) : o().createElement(v.Tooltip, {
                             title: "Turn editing tags on"
-                        }, s().createElement(z.Edit, {
+                        }, o().createElement(z.Edit, {
                             className: "env-edit-icon",
                             onClick: this.handleEditState
                         }))
-                    }, this.renderAddTags = () => s().createElement("div", {
+                    }, this.renderAddTags = () => o().createElement("div", {
                         className: "env-add-tags",
                         style: {
                             backgroundColor: this.state.inputBoxVisible && "#673ab7"
                         }
-                    }, s().createElement(v.IconButton, {
+                    }, o().createElement(v.IconButton, {
                         size: "small",
                         onClick: () => {
                             this.setState((e => ({
                                 inputBoxVisible: !e.inputBoxVisible
                             })))
                         },
                         sx: {
                             padding: 0,
                             fontSize: 14,
                             color: this.state.inputBoxVisible && "white"
                         }
-                    }, s().createElement(z.AddCircleOutlined, {
+                    }, o().createElement(z.AddCircleOutlined, {
                         fontSize: "inherit",
                         color: "inherit"
-                    })), this.state.inputBoxVisible && s().createElement("input", {
+                    })), this.state.inputBoxVisible && o().createElement("input", {
                         className: "env-tags-input",
                         type: "text",
                         value: this.state.tagInput,
                         placeholder: "Enter tags",
                         onChange: e => this.setState({
                             tagInput: e.target.value
                         }),
                         onKeyDown: e => this.handleAddTags(e)
                     })), this.renderQuantumJobsToggle = () => {
                         const e = this.state.quantumJobs;
-                        return s().createElement(v.Stack, {
+                        return o().createElement(v.Stack, {
                             flexDirection: "row",
                             alignItems: "center",
                             flexWrap: "wrap",
                             gap: 1,
                             px: "12px",
                             pb: "12px"
-                        }, s().createElement(v.Typography, {
+                        }, o().createElement(v.Typography, {
                             fontSize: 14,
                             fontWeight: 600,
                             color: e ? "text.primary" : "text.disabled",
                             sx: {
                                 userSelect: "none"
                             }
-                        }, "Quantum Jobs"), e && s().createElement(v.FormGroup, null, s().createElement(v.FormControlLabel, {
+                        }, "Quantum Jobs"), e && o().createElement(v.FormGroup, null, o().createElement(v.FormControlLabel, {
                             disabled: !e,
-                            control: s().createElement(v.Switch, {
+                            control: o().createElement(v.Switch, {
                                 disabled: this.state.lockedEnv,
                                 checked: this.state.quantumJobsEnabled,
                                 onChange: this.handleQuantumJobsToggle,
                                 size: "small",
                                 inputProps: {
                                     "aria-label": "controlled"
                                 },
@@ -1161,15 +1371,15 @@
                             sx: {
                                 margin: 0,
                                 "& .MuiFormControlLabel-label": {
                                     fontSize: "12px",
                                     color: this.state.qjobsStatus.error ? "error.main" : this.state.quantumJobsEnabled ? "success.main" : "text.disabled"
                                 }
                             }
-                        })), !e && !this.state.quantumJobsAdditionSuccess && s().createElement(v.Tooltip, {
+                        })), !e && !this.state.quantumJobsAdditionSuccess && o().createElement(v.Tooltip, {
                             title: "Quantum jobs are not supported for this environment!",
                             arrow: !0,
                             placement: "right",
                             PopperProps: {
                                 sx: e => ({
                                     "& .MuiTooltip-tooltip": {
                                         backgroundColor: e.palette.warning.main,
@@ -1178,21 +1388,21 @@
                                         fontSize: "12px"
                                     },
                                     "& .MuiTooltip-arrow": {
                                         color: e.palette.warning.main
                                     }
                                 })
                             }
-                        }, s().createElement(z.ReportProblemOutlined, {
+                        }, o().createElement(z.ReportProblemOutlined, {
                             color: "inherit",
                             sx: {
                                 color: "warning.main",
                                 fontSize: "16px"
                             }
-                        })), !e && !this.state.quantumJobsAdditionSuccess && s().createElement(v.Tooltip, {
+                        })), !e && !this.state.quantumJobsAdditionSuccess && o().createElement(v.Tooltip, {
                             title: "Add quantum jobs",
                             arrow: !0,
                             placement: "right",
                             PopperProps: {
                                 sx: e => ({
                                     "& .MuiTooltip-tooltip": {
                                         backgroundColor: e.palette.background.paper,
@@ -1201,73 +1411,71 @@
                                         fontSize: "12px"
                                     },
                                     "& .MuiTooltip-arrow": {
                                         color: e.palette.background.paper
                                     }
                                 })
                             }
-                        }, s().createElement(v.IconButton, {
+                        }, o().createElement(v.IconButton, {
                             size: "small",
                             color: "text.secondary",
                             disabled: this.props.installing || this.props.env.isPreInstalled || this.state.lockedEnv,
                             onClick: !this.props.env.isPreInstalled && (async () => {
-                                try {
-                                    (await this.context.getActions("EnvironmentActions").addQuantumJobs(this.props.env.slug)).success && (this.setState({
+                                this.addPackage("amazon-braket-sdk").then((() => {
+                                    this.setState({
                                         quantumJobsAdditionSuccess: !0
                                     }), setTimeout((() => {
-                                        this.context.getActions("EnvironmentActions").updateAll().then((() => {
-                                            this.setState({
-                                                quantumJobsAdditionSuccess: !1,
-                                                quantumJobs: !0,
-                                                quantumJobsEnabled: !0
-                                            })
-                                        }))
-                                    }), 1750))
-                                } catch (e) {
+                                        this.setState({
+                                            quantumJobsAdditionSuccess: !1,
+                                            quantumJobs: !0,
+                                            quantumJobsEnabled: !1
+                                        })
+                                    }), 1750)
+                                })).catch((e => {
                                     console.log("Error adding quantum jobs. ", e), alert("Unable to add quantum jobs at this time. Please try again later, and verify that qbraid-core is installed and configured correctly.")
-                                }
+                                }))
                             })
-                        }, s().createElement(z.AddCircleOutlineOutlined, {
+                        }, o().createElement(z.AddCircleOutlineOutlined, {
                             fontSize: "inherit"
-                        }))), this.state.quantumJobsAdditionSuccess && s().createElement(v.Box, {
+                        }))), this.state.quantumJobsAdditionSuccess && o().createElement(v.Box, {
                             display: "flex",
                             alignItems: "center",
                             justifyContent: "center",
                             gap: 1,
                             borderRadius: 1,
                             px: 1,
                             sx: e => ({
                                 userSelect: "none"
                             })
-                        }, s().createElement(_, {
+                        }, o().createElement(q, {
                             color: "green"
-                        }), s().createElement(v.Typography, {
+                        }), o().createElement(v.Typography, {
                             fontSize: 14,
                             sx: e => ({
                                 color: e.palette.success.main
                             })
                         }, "Successfully added!")))
-                    }, this.renderInfoPane = () => s().createElement("div", {
+                    }, this.renderInfoPane = () => o().createElement("div", {
                         className: "env-editor-pane",
                         id: "general-info-pane"
-                    }, s().createElement("p", {
+                    }, o().createElement("p", {
                         className: "env-editor-pane-title"
-                    }, "General Info"), s().createElement(v.TextField, {
+                    }, "General Info"), o().createElement(v.TextField, {
                         inputRef: e => this._nameInput = e,
                         class: "env-editor-input-data-text",
                         placeHolder: "Name",
                         fullWidth: !0,
                         size: "small",
                         sx: {
                             padding: "0"
                         },
                         spellCheck: "false",
                         disabled: !0,
                         InputProps: {
-                            endAdornment: s().createElement(v.InputAdornment, {
+                            endAdornment: o().createElement(v.InputAdornment, {
                                 position: "end",
                                 sx: {
                                     textDecoration: this.state.showCopyIcon ? "underline" : "none",
                                     cursor: "pointer"
                                 },
                                 onMouseEnter: () => {
                                     this.setState({
@@ -1275,17 +1483,17 @@
                                     })
                                 },
                                 onMouseLeave: () => {
                                     this.setState({
                                         showCopyIcon: !1
                                     })
                                 }
-                            }, `ID: ${this.props.env.slug}`, this.state.showCopyIcon && s().createElement(v.Tooltip, {
+                            }, `ID: ${this.props.env.slug}`, this.state.showCopyIcon && o().createElement(v.Tooltip, {
                                 title: this.state.textCopied ? "Slug Copied" : "Click to copy the Slug ID"
-                            }, s().createElement(z.Link, {
+                            }, o().createElement(z.Link, {
                                 sx: {
                                     fontSize: "1rem",
                                     transform: "rotateZ(-45deg)",
                                     marginLeft: "5px",
                                     cursor: "pointer"
                                 },
                                 onClick: () => {
@@ -1295,76 +1503,76 @@
                                         this.setState({
                                             textCopied: !1
                                         })
                                     }), 2e3)
                                 }
                             })))
                         }
-                    }), s().createElement("textarea", {
+                    }), o().createElement("textarea", {
                         ref: e => this._descriptionInput = e,
                         className: "env-info-input",
                         style: {
                             marginBottom: 10,
                             flex: 1
                         },
                         type: "text",
                         placeholder: "No Description",
                         spellCheck: "false",
                         rows: "4",
                         disabled: !this.state.isOwner || !this.state.editOpen
-                    }), this.props.env.installed && this.renderQuantumJobsToggle(), s().createElement(v.Box, {
+                    }), this.props.env.installed && this.renderQuantumJobsToggle(), o().createElement(v.Box, {
                         display: "flex",
                         flexDirection: "row",
                         flexWrap: "wrap",
                         gap: .5,
                         paddingX: "10px",
                         paddingBottom: "10px"
-                    }, this.state.tags.map(((e, t) => s().createElement(v.Chip, {
+                    }, this.state.tags.map(((e, t) => o().createElement(v.Chip, {
                         key: t,
                         label: e,
                         size: "small",
                         variant: "filled",
                         onDelete: "custom" === e.toLowerCase() ? "" : this.state.editOpen ? () => this.handleRemoveTags(t) : ""
-                    }))), this.state.isOwner && this.state.editOpen && this.renderAddTags()), this.state.canModify && s().createElement(v.Stack, {
+                    }))), this.state.isOwner && this.state.editOpen && this.renderAddTags()), this.state.canModify && o().createElement(v.Stack, {
                         flexDirection: "row",
                         gap: 1,
                         justifyContent: "flex-end"
-                    }, this.state.saveSuccess ? s().createElement(_, {
+                    }, this.state.saveSuccess ? o().createElement(q, {
                         width: "2em",
                         height: "2em",
                         color: "green",
                         style: {
                             paddingRight: "8px"
                         }
-                    }) : s().createElement(v.Tooltip, {
+                    }) : o().createElement(v.Tooltip, {
                         title: this.state.editOpen ? "Turn Edit off" : "Edit",
                         arrow: !0,
                         placement: "left"
-                    }, s().createElement(v.IconButton, {
+                    }, o().createElement(v.IconButton, {
                         size: "small",
                         variant: "slide",
                         color: "text.secondary",
                         onClick: this.state.editOpen ? () => this.handleEditStateClose() : () => this.handleEditStateOpen()
-                    }, this.state.editOpen ? s().createElement(z.EditOff, {
+                    }, this.state.editOpen ? o().createElement(z.EditOff, {
                         fontSize: "inherit",
                         color: "inherit"
-                    }) : s().createElement(z.Edit, {
+                    }) : o().createElement(z.Edit, {
                         fontSize: "inherit",
                         color: "inherit"
-                    }))), this.state.editOpen && s().createElement(v.Tooltip, {
+                    }))), this.state.editOpen && o().createElement(v.Tooltip, {
                         title: "Save",
                         arrow: !0,
                         placement: "top"
-                    }, s().createElement(v.IconButton, {
+                    }, o().createElement(v.IconButton, {
                         size: "small",
                         variant: "slide",
                         color: "text.secondary",
                         disabled: this.state.saveLoading,
                         onClick: this.handleSubmit
-                    }, this.state.saveLoading ? s().createElement(S, null) : s().createElement(z.SaveOutlined, {
+                    }, this.state.saveLoading ? o().createElement(S, null) : o().createElement(z.SaveOutlined, {
                         fontSize: "inherit"
                     }))))), this.handleGenerateAccessKey = e => {
                         this.setState({
                             accessKeyLoading: !0
                         }), this.context.getActions("EnvironmentActions").generateAccessKey(e).then((t => {
                             var n;
                             this.setState({
@@ -1428,107 +1636,107 @@
                                             resharePopUp: !1,
                                             shareEmail: "",
                                             shareEmailBtnDis: !1
                                         })
                                     }
                                 }
                             };
-                        return s().createElement("div", {
+                        return o().createElement("div", {
                             className: "env-editor-pane",
                             id: "sharing-pane",
                             style: {
                                 marginTop: "0px !important"
                             }
-                        }, s().createElement("p", {
+                        }, o().createElement("p", {
                             className: "env-editor-pane-title"
-                        }, "Share Environment"), s().createElement(v.Box, {
+                        }, "Share Environment"), o().createElement(v.Box, {
                             className: "env-pane-content",
                             flex: 1,
                             mt: 0
-                        }, this.state.isCustom && this.state.isOwner && this.state.isInstalled && this.state.isMount && s().createElement(v.Typography, {
+                        }, this.state.isCustom && this.state.isOwner && this.state.isInstalled && this.state.isMount && o().createElement(v.Typography, {
                             fontSize: 14
-                        }, "Enable other qBraid users to discover this environment and install a copy into their own Lab instance."), this.state.isMount ? this.state.isOwner ? this.state.isCustom ? this.state.isInstalled ? s().createElement(v.Grid, {
+                        }, "Enable other qBraid users to discover this environment and install a copy into their own Lab instance."), this.state.isMount ? this.state.isOwner ? this.state.isCustom ? this.state.isInstalled ? o().createElement(v.Grid, {
                             container: !0,
                             justifyContent: "space-between",
                             alignItems: "flex-start",
                             position: "relative",
                             spacing: 1,
                             mt: 1
-                        }, s().createElement(v.Grid, {
+                        }, o().createElement(v.Grid, {
                             item: !0,
                             container: !0,
                             xs: 12,
                             spacing: 1,
                             position: "relative"
-                        }, s().createElement(v.Grid, {
+                        }, o().createElement(v.Grid, {
                             item: !0,
                             xs: 12,
                             sm: 12,
                             md: 8,
                             lg: 8
-                        }, s().createElement(v.Autocomplete, {
+                        }, o().createElement(v.Autocomplete, {
                             id: "env-email-input",
                             size: "small",
                             fullWidth: !0,
                             freeSolo: !0,
                             options: this.state.recentEmails,
                             value: this.state.optionValue,
                             onChange: (e, t) => {
                                 this.setState({
                                     optionValue: t
                                 })
                             },
-                            renderOption: (e, n) => s().createElement(v.Stack, Object.assign({
+                            renderOption: (e, n) => o().createElement(v.Stack, Object.assign({
                                 component: "li",
                                 flexDirection: "row",
                                 gap: 2,
                                 py: 3
-                            }, e), s().createElement(v.Avatar, Object.assign({}, (e => {
+                            }, e), o().createElement(v.Avatar, Object.assign({}, (e => {
                                 var n;
                                 return {
                                     sx: {
                                         bgcolor: t(e),
                                         width: "26px",
                                         height: "26px",
                                         fontSize: "18px"
                                     },
                                     children: `${null===(n=null==e?void 0:e.slice(0,1))||void 0===n?void 0:n.toUpperCase()}`
                                 }
-                            })(n))), s().createElement(v.Typography, {
+                            })(n))), o().createElement(v.Typography, {
                                 fontSize: 14,
                                 color: "text.primary"
                             }, n)),
                             inputValue: this.state.shareEmail,
                             onInputChange: (e, t) => {
                                 this.setState((() => ({
                                     shareEmail: t,
                                     shareEmailApiError: ""
                                 }))), "" === t || (null == t ? void 0 : t.match(/^[A-Za-z\._\-[0-9]*[@][A-Za-z]*[\.][a-z]{2,4}$/)) ? this.setState({
                                     shareEmailError: ""
                                 }) : this.setState({
                                     shareEmailError: "Invalid email format"
                                 })
                             },
-                            renderInput: e => s().createElement(v.TextField, Object.assign({}, e, {
+                            renderInput: e => o().createElement(v.TextField, Object.assign({}, e, {
                                 error: this.state.shareEmailError,
                                 helperText: this.state.shareEmail.length > 2 && this.state.shareEmailError || " ",
                                 placeholder: "Enter qBraid user email"
                             })),
                             sx: {
                                 "& .MuiOutlinedInput-root.MuiInputBase-sizeSmall": {
                                     fontSize: "14px"
                                 }
                             }
-                        })), s().createElement(v.Grid, {
+                        })), o().createElement(v.Grid, {
                             item: !0,
                             xs: 12,
                             sm: 12,
                             md: 4,
                             lg: 4
-                        }, s().createElement(v.Button, {
+                        }, o().createElement(v.Button, {
                             fullWidth: !0,
                             className: "env-editor-pane-action",
                             onClick: () => {
                                 this.setState({
                                     shareEmailApiError: ""
                                 }), "" !== this.state.shareEmail ? this.state.isCustom ? this.state.uninstalling || this.state.cancelling || this.state.deleting || this.props.installing || this.props.packageInstallingEnv === this.props.env._id ? this.setState({
                                     shareEmailError: "Blocked during state transition",
@@ -1555,135 +1763,135 @@
                             style: {
                                 background: this.state.shareSuccess ? "green" : "#673AB7",
                                 cursor: this.state.shareEmailBtnDis ? "not-allowed !important" : "pointer !important",
                                 marginBottom: (null === (e = this.state.shareEmail) || void 0 === e ? void 0 : e.length) > 2 && !this.state.shareEmail.match(/^[A-Za-z\._\-[0-9]*[@][A-Za-z]*[\.][a-z]{2,4}$/) ? "25px" : "0px"
                             },
                             disabled: this.state.shareEmailBtnDis,
                             size: "small",
-                            startIcon: this.state.shareSuccess ? s().createElement(z.Check, {
+                            startIcon: this.state.shareSuccess ? o().createElement(z.Check, {
                                 color: "green"
-                            }) : s().createElement(z.Send, {
+                            }) : o().createElement(z.Send, {
                                 sx: {
                                     transform: "rotateZ(-45deg)"
                                 }
                             })
-                        }, this.state.shareSuccess ? "Sent" : "Share")), s().createElement(v.Grid, {
+                        }, this.state.shareSuccess ? "Sent" : "Share")), o().createElement(v.Grid, {
                             item: !0,
                             xs: 12,
                             position: "absolute",
                             bottom: "4px"
-                        }, this.state.isCustom && this.state.isOwner && this.state.isInstalled && this.state.isMount && this.state.shareEmailApiError && s().createElement("p", {
+                        }, this.state.isCustom && this.state.isOwner && this.state.isInstalled && this.state.isMount && this.state.shareEmailApiError && o().createElement("p", {
                             className: "env-pane-email-error"
-                        }, this.state.shareEmailApiError), this.state.isCustom && this.state.isOwner && this.state.isInstalled && this.state.isMount && this.state.shareSuccess && s().createElement("p", {
+                        }, this.state.shareEmailApiError), this.state.isCustom && this.state.isOwner && this.state.isInstalled && this.state.isMount && this.state.shareSuccess && o().createElement("p", {
                             className: "env-pane-email-success"
-                        }, "Environment shared succesfully..."))), s().createElement(v.Grid, {
+                        }, "Environment shared succesfully..."))), o().createElement(v.Grid, {
                             item: !0,
                             xs: 12
-                        }, s().createElement(v.Divider, {
+                        }, o().createElement(v.Divider, {
                             textAlign: "center"
-                        }, "OR")), s().createElement(v.Grid, {
+                        }, "OR")), o().createElement(v.Grid, {
                             item: !0,
                             display: "flex",
                             justifyContent: "center",
                             alignItems: "center",
                             xs: 12
-                        }, "" === this.state.accessKey ? s().createElement(v.Button, {
+                        }, "" === this.state.accessKey ? o().createElement(v.Button, {
                             fullWidth: !0,
                             variant: "outlined",
                             color: "success",
                             onClick: () => this.handleGenerateAccessKey(this.props.env._id),
                             sx: {
                                 textTransform: "none",
                                 fontSize: 12,
                                 cursor: this.state.accessKeyLoading ? "progress" : "pointer"
                             },
                             disabled: this.state.accessKeyLoading
-                        }, this.state.accessKeyLoading ? "Generating ..." : "Generate Access Code") : s().createElement(v.Grid, {
+                        }, this.state.accessKeyLoading ? "Generating ..." : "Generate Access Code") : o().createElement(v.Grid, {
                             item: !0,
                             xs: 12
-                        }, s().createElement(v.Paper, {
+                        }, o().createElement(v.Paper, {
                             elevation: 0,
                             sx: e => ({
                                 display: "flex",
                                 alignItems: "center",
                                 width: "100%",
                                 backgroundColor: `${e.palette.success.light}30`
                             })
-                        }, s().createElement(v.Typography, {
+                        }, o().createElement(v.Typography, {
                             fontSize: 12,
                             color: "success",
                             px: 1.5
-                        }, "Share via access code"), s().createElement(v.Divider, {
+                        }, "Share via access code"), o().createElement(v.Divider, {
                             orientation: "vertical",
                             sx: {
                                 m: .5,
                                 height: 28
                             }
-                        }), s().createElement(v.InputBase, {
+                        }), o().createElement(v.InputBase, {
                             size: "small",
                             sx: {
                                 ml: 1,
                                 flex: 1,
                                 fontSize: 12,
                                 fontWeight: 600,
                                 "&.MuiInputBase-input": {
                                     p: 0
                                 }
                             },
                             value: this.state.accessKey,
                             type: this.state.accessKeyVisibility ? "text" : "password"
-                        }), s().createElement(v.IconButton, {
+                        }), o().createElement(v.IconButton, {
                             size: "small",
                             onClick: () => {
                                 this.setState((e => ({
                                     accessKeyVisibility: !e.accessKeyVisibility
                                 })))
                             }
-                        }, this.state.accessKeyVisibility ? s().createElement(z.VisibilityOff, {
+                        }, this.state.accessKeyVisibility ? o().createElement(z.VisibilityOff, {
                             fontSize: "inherit"
-                        }) : s().createElement(z.Visibility, {
+                        }) : o().createElement(z.Visibility, {
                             fontSize: "inherit"
-                        })), s().createElement(v.Divider, {
+                        })), o().createElement(v.Divider, {
                             orientation: "vertical",
                             sx: {
                                 m: .5,
                                 height: 28
                             }
-                        }), s().createElement(v.Tooltip, {
+                        }), o().createElement(v.Tooltip, {
                             arrow: !0,
                             placement: "left",
                             title: "Copy"
-                        }, s().createElement(v.IconButton, {
+                        }, o().createElement(v.IconButton, {
                             size: "small",
                             sx: {
                                 mx: 1.5
                             },
                             onClick: () => {
                                 this.setState({
                                     copyCooldown: !0
                                 }), navigator.clipboard.writeText(this.state.accessKey), setTimeout((() => this.setState({
                                     copyCooldown: !1
                                 })), 1500)
                             }
-                        }, this.state.copyCooldown ? s().createElement(_, {
+                        }, this.state.copyCooldown ? o().createElement(q, {
                             color: "green"
-                        }) : s().createElement(z.ContentCopy, {
+                        }) : o().createElement(z.ContentCopy, {
                             fontSize: "inherit"
-                        })))))), s().createElement(v.Grid, {
+                        })))))), o().createElement(v.Grid, {
                             item: !0,
                             xs: 12,
                             display: "flex",
                             justifyContent: "flex-end",
                             alignItems: "center",
                             gap: 1
-                        }, "" !== this.state.accessKey && s().createElement(s().Fragment, null, s().createElement(v.Button, {
+                        }, "" !== this.state.accessKey && o().createElement(o().Fragment, null, o().createElement(v.Button, {
                             variant: "text",
                             color: "success",
                             size: "small",
-                            startIcon: s().createElement(z.Refresh, {
+                            startIcon: o().createElement(z.Refresh, {
                                 fontSize: "inherit"
                             }),
                             sx: {
                                 padding: "0px !important",
                                 textTransform: "none"
                             },
                             onClick: () => {
@@ -1692,285 +1900,290 @@
                                     resharePopUpContent: {
                                         content: "accessCode",
                                         title: "Are you sure?",
                                         body: "Generating a new access code will invalidate the current code, and update the global shared copy of this environment."
                                     }
                                 })
                             }
-                        }, "Regenerate access code?"), s().createElement(v.Tooltip, {
-                            title: s().createElement(s().Fragment, null, "The existing access code will be invalidated and your current environment will replace the global shared copy."),
+                        }, "Regenerate access code?"), o().createElement(v.Tooltip, {
+                            title: o().createElement(o().Fragment, null, "The existing access code will be invalidated and your current environment will replace the global shared copy."),
                             PopperProps: {
                                 sx: e => ({
                                     [`& .${v.tooltipClasses.tooltip}`]: {
                                         background: e.palette.background.alternate,
                                         color: e.palette.text.primary,
                                         fontSize: 12,
                                         boxShadow: e.shadows[10]
                                     }
                                 })
                             }
-                        }, s().createElement(z.InfoOutlined, {
+                        }, o().createElement(z.InfoOutlined, {
                             fontSize: "small",
                             color: "action",
                             sx: {
                                 width: 14,
                                 height: 14
                             }
-                        }))))) : s().createElement(v.Grid, {
+                        }))))) : o().createElement(v.Grid, {
                             container: !0
-                        }, s().createElement(v.Grid, {
+                        }, o().createElement(v.Grid, {
                             item: !0,
                             xs: 12
-                        }, s().createElement("p", {
+                        }, o().createElement("p", {
                             className: "env-pane-prompt"
-                        }, "To share an environment, it must be installed. To install this environment, click ", s().createElement("b", null, "Install"), " in the panel drop-down."))) : s().createElement(v.Grid, {
+                        }, "To share an environment, it must be installed. To install this environment, click ", o().createElement("b", null, "Install"), " in the panel drop-down."))) : o().createElement(v.Grid, {
                             container: !0
-                        }, s().createElement(v.Grid, {
+                        }, o().createElement(v.Grid, {
                             item: !0,
                             xs: 12
-                        }, s().createElement("p", {
+                        }, o().createElement("p", {
                             className: "env-pane-prompt"
-                        }, "This environment is not shareable. To create a shareable, custom environment, click", " ", s().createElement("b", null, "Add ", "→", " Create Environment"), " in the environments sidebar."))) : s().createElement(v.Grid, {
+                        }, "This environment is not shareable. To create a shareable, custom environment, click", " ", o().createElement("b", null, "Add ", "→", " Create Environment"), " in the environments sidebar."))) : o().createElement(v.Grid, {
                             container: !0
-                        }, s().createElement(v.Grid, {
+                        }, o().createElement(v.Grid, {
                             item: !0,
                             xs: 12
-                        }, s().createElement("p", {
+                        }, o().createElement("p", {
                             className: "env-pane-prompt"
-                        }, "To share an environment, you must be the environment owner. To create your own shareable, custom environment, click", " ", s().createElement("b", null, "Add ", "→", " Create Environment"), " in the environments sidebar."))) : s().createElement(v.Grid, {
+                        }, "To share an environment, you must be the environment owner. To create your own shareable, custom environment, click", " ", o().createElement("b", null, "Add ", "→", " Create Environment"), " in the environments sidebar."))) : o().createElement(v.Grid, {
                             container: !0
-                        }, s().createElement(v.Grid, {
+                        }, o().createElement(v.Grid, {
                             item: !0,
                             xs: 12
-                        }, s().createElement("p", {
+                        }, o().createElement("p", {
                             className: "env-pane-prompt"
-                        }, "Sharing environments is only available within the cloud-based qBraid Lab platform. Launch an instance at", " ", s().createElement("a", {
+                        }, "Sharing environments is only available within the cloud-based qBraid Lab platform. Launch an instance at", " ", o().createElement("a", {
                             href: "https://lab.qbraid.com",
                             style: {
                                 color: "blue"
                             },
                             target: "_blank",
                             rel: "noopener noreferrer"
                         }, "lab.qbraid.com"), " ", "to share environments with other users."))), this.renderReshareEnvModal({
                             action: n
                         }), this.renderUpgradeEnvModal()))
-                    }, this.renderUpgradeEnvModal = () => s().createElement(v.Modal, {
+                    }, this.renderUpgradeEnvModal = () => o().createElement(v.Modal, {
                         open: this.state.upgradePopUp,
                         onClose: () => this.setState({
                             upgradePopUp: !1
                         }),
                         sx: {
                             display: "flex",
                             justifyContent: "center",
                             alignItems: "center",
                             padding: "1em",
                             zIndex: "1301"
                         }
-                    }, s().createElement(v.Grid, {
+                    }, o().createElement(v.Grid, {
                         container: !0,
                         sx: {
                             width: "700px",
                             minWidth: "200px",
                             minHeight: "150px",
                             padding: "1em"
                         },
                         className: "env-pane-re-share"
-                    }, s().createElement(v.Grid, {
+                    }, o().createElement(v.Grid, {
                         item: !0,
                         xs: 12
-                    }, s().createElement("h3", {
+                    }, o().createElement("h3", {
                         style: {
                             margin: "0px"
                         }
-                    }, "Upgrade to Continue")), s().createElement(v.Grid, {
+                    }, "Upgrade to Continue")), o().createElement(v.Grid, {
                         item: !0,
                         xs: 12
-                    }, s().createElement("p", {
+                    }, o().createElement("p", {
                         className: "env-pane-email-normal"
-                    }, "Upgrade your account to unlock premium environment manager features.")), s().createElement(v.Grid, {
+                    }, "Upgrade your account to unlock premium environment manager features.")), o().createElement(v.Grid, {
                         item: !0,
                         container: !0,
                         xs: 12,
                         sx: {
                             display: "flex",
                             justifyContent: "flex-end",
                             alignItems: "center",
                             gap: "10px"
                         }
-                    }, s().createElement(v.Grid, {
+                    }, o().createElement(v.Grid, {
                         item: !0,
                         xs: 3,
                         sm: 3,
                         md: 2,
                         lg: 2,
                         xl: 2
-                    }, s().createElement(v.Button, {
+                    }, o().createElement(v.Button, {
                         variant: "slide",
                         type: "decline",
                         fullWidth: !0,
                         sx: {
                             textTransform: "none",
                             minWidth: "120px"
                         },
                         onClick: () => this.setState({
                             upgradePopUp: !1
                         })
-                    }, "Maybe later")), s().createElement(v.Grid, {
+                    }, "Maybe later")), o().createElement(v.Grid, {
                         item: !0,
                         xs: 2
-                    }, s().createElement(v.Button, {
+                    }, o().createElement(v.Button, {
                         variant: "slide",
                         sx: {
                             textTransform: "none",
                             minWidth: "120px"
                         },
                         fullWidth: !0,
                         onClick: () => window.open(`${y}/billing`, "_blank")
                     }, "Upgrade"))))), this.renderReshareEnvModal = ({
                         action: e
                     }) => {
                         var t, n;
-                        return s().createElement(v.Modal, {
+                        return o().createElement(v.Modal, {
                             open: this.state.resharePopUp,
                             onClose: () => this.setState({
                                 resharePopUp: !1,
                                 shareEmailBtnDis: !1,
                                 shareEmail: ""
                             }),
                             sx: {
                                 display: "flex",
                                 justifyContent: "center",
                                 alignItems: "center",
                                 padding: "1em",
                                 zIndex: "1301"
                             }
-                        }, s().createElement(v.Grid, {
+                        }, o().createElement(v.Grid, {
                             container: !0,
                             sx: {
                                 width: "700px",
                                 minWidth: "200px",
                                 minHeight: "150px",
                                 padding: "1em"
                             },
                             className: "env-pane-re-share",
                             spacing: 1
-                        }, s().createElement(v.Grid, {
+                        }, o().createElement(v.Grid, {
                             item: !0,
                             xs: 12
-                        }, s().createElement(v.Typography, {
+                        }, o().createElement(v.Typography, {
                             fontSize: 18,
                             fontWeight: 600,
                             color: "text.primary"
-                        }, this.state.resharePopUpContent.title)), s().createElement(v.Grid, {
+                        }, this.state.resharePopUpContent.title)), o().createElement(v.Grid, {
                             item: !0,
                             xs: 12
-                        }, s().createElement(v.Typography, {
+                        }, o().createElement(v.Typography, {
                             fontSize: 14,
                             color: "text.primary"
-                        }, this.state.resharePopUpContent.body)), s().createElement(v.Grid, {
+                        }, this.state.resharePopUpContent.body)), o().createElement(v.Grid, {
                             item: !0,
                             container: !0,
                             xs: 12,
                             justifyContent: "flex-end",
                             alignItems: "center",
                             spacing: 1
-                        }, s().createElement(v.Grid, {
+                        }, o().createElement(v.Grid, {
                             item: !0
-                        }, s().createElement(v.Button, {
+                        }, o().createElement(v.Button, {
                             variant: "slide",
                             type: "decline",
                             sx: {
                                 textTransform: "none",
                                 minWidth: "120px"
                             },
                             onClick: null === (t = e[this.state.resharePopUpContent.content]) || void 0 === t ? void 0 : t.cancel
-                        }, "Cancel")), s().createElement(v.Grid, {
+                        }, "Cancel")), o().createElement(v.Grid, {
                             item: !0
-                        }, s().createElement(v.Button, {
+                        }, o().createElement(v.Button, {
                             variant: "slide",
                             sx: {
                                 textTransform: "none",
                                 minWidth: "120px"
                             },
                             onClick: null === (n = e[this.state.resharePopUpContent.content]) || void 0 === n ? void 0 : n.confirm
                         }, "Confirm")))))
-                    }, this.renderShareMsg = ({
-                        msg: e,
-                        type: t
-                    }) => s().createElement(v.Snackbar, {
+                    }, this.renderShareMsg = () => o().createElement(v.Snackbar, {
                         open: this.state.sharePopupOpen,
-                        autoHideDuration: B,
+                        autoHideDuration: 2500,
                         onClose: this.handleSharePopupClose,
                         sx: {
                             position: "sticky",
                             width: "300px",
+                            bottom: "10px!important",
+                            left: "40px!important"
+                        }
+                    }, o().createElement(v.Alert, {
+                        severity: this.state.sharePopupMsg.type,
+                        variant: "filled",
+                        sx: {
+                            position: "absolute",
+                            width: "100%",
+                            fontSize: "14px",
                             bottom: "10px"
                         }
-                    }, s().createElement("div", {
-                        className: `env-pane-msg-popup ${t} slide-in-bottom`
-                    }, e)), this.renderCollaboratorRows = () => {
-                        let e = [s().createElement("tr", {
+                    }, this.state.sharePopupMsg.msg)), this.renderCollaboratorRows = () => {
+                        let e = [o().createElement("tr", {
                                 key: -1,
                                 style: {
                                     borderColor: "#ececec"
                                 }
-                            }, s().createElement("td", {
+                            }, o().createElement("td", {
                                 className: "env-table-filter"
-                            }, s().createElement("input", {
+                            }, o().createElement("input", {
                                 placeholder: "Filter...",
                                 onChange: this.handleChangeCollaboratorFilter
-                            })), s().createElement("td", null), s().createElement("td", null))],
-                            t = this.state.readAccessUsers.concat(this.state.writeAccessUsers.map((e => (e.write = !0, e)))).filter((e => !this.state.collaboratorFilter || -1 !== e.jupyterUsername.toLowerCase().indexOf(this.state.collaboratorFilter))).sort(((e, t) => e.jupyterUsername.toLowerCase() > t.jupyterUsername.toLowerCase() ? 1 : -1)).map(((e, t) => s().createElement("tr", {
+                            })), o().createElement("td", null), o().createElement("td", null))],
+                            t = this.state.readAccessUsers.concat(this.state.writeAccessUsers.map((e => (e.write = !0, e)))).filter((e => !this.state.collaboratorFilter || -1 !== e.jupyterUsername.toLowerCase().indexOf(this.state.collaboratorFilter))).sort(((e, t) => e.jupyterUsername.toLowerCase() > t.jupyterUsername.toLowerCase() ? 1 : -1)).map(((e, t) => o().createElement("tr", {
                                 key: e.jupyterUsername + t,
                                 style: {
                                     borderColor: "#ececec"
                                 }
-                            }, s().createElement("td", {
+                            }, o().createElement("td", {
                                 style: {
                                     width: 180,
                                     maxWidth: 180
                                 }
-                            }, e.jupyterUsername), s().createElement("td", {
+                            }, e.jupyterUsername), o().createElement("td", {
                                 style: {
                                     width: 70,
                                     textAlign: "center"
                                 }
-                            }, s().createElement("input", {
+                            }, o().createElement("input", {
                                 type: "checkbox",
                                 disabled: !0,
                                 checked: !0
-                            })), s().createElement("td", {
+                            })), o().createElement("td", {
                                 style: {
                                     width: 70,
                                     textAlign: "center"
                                 }
-                            }, s().createElement("input", {
+                            }, o().createElement("input", {
                                 type: "checkbox",
                                 defaultChecked: e.write,
                                 onChange: () => this.toggleWriteAccess(e)
                             })))));
                         return e.concat(t)
                     }, this.renderPackagesPane = () => {
                         let e = this.state.packagesInImage.length;
-                        return s().createElement("div", {
+                        return o().createElement("div", {
                             className: "env-editor-pane"
-                        }, s().createElement("p", {
+                        }, o().createElement("p", {
                             className: "env-editor-pane-title"
-                        }, "Packages"), s().createElement("div", {
+                        }, "Packages"), o().createElement("div", {
                             className: "env-pane-content",
                             style: {
                                 flex: 1
                             }
-                        }, s().createElement(v.Box, {
+                        }, o().createElement(v.Box, {
                             sx: e => ({
                                 overflow: "hidden",
                                 border: `1px solid ${e.palette.divider}`,
                                 borderRadius: 2
                             })
-                        }, s().createElement(v.TableContainer, {
+                        }, o().createElement(v.TableContainer, {
                             sx: {
                                 maxHeight: "60vh",
                                 height: (() => {
                                     var e, t;
                                     const n = null === (e = document.getElementById("general-info-pane")) || void 0 === e ? void 0 : e.offsetHeight,
                                         i = null === (t = document.getElementById("sharing-pane")) || void 0 === t ? void 0 : t.offsetHeight,
                                         a = Number(+n + +i) - 137;
@@ -1989,117 +2202,117 @@
                                 position: "relative",
                                 backgroundColor: "var(--jp-layout-color1)",
                                 overflowY: "auto",
                                 overflowX: "hidden",
                                 flex: 1
                             },
                             component: v.Paper
-                        }, s().createElement(v.Table, {
+                        }, o().createElement(v.Table, {
                             stickyHeader: !0,
                             size: "small"
-                        }, s().createElement(v.TableHead, {
+                        }, o().createElement(v.TableHead, {
                             sx: {
                                 color: "var(--jp-ui-font-color0)"
                             }
-                        }, s().createElement(v.TableRow, null, s().createElement(v.TableCell, null, "Name"), s().createElement(v.TableCell, null, "Version"), this.props.env.installed && s().createElement(v.TableCell, null, "Remove")), e > 0 && !this.state.addPackageDialogOpen && s().createElement(v.TableRow, null, s().createElement(v.TableCell, {
+                        }, o().createElement(v.TableRow, null, o().createElement(v.TableCell, null, "Name"), o().createElement(v.TableCell, null, "Version"), this.props.env.installed && o().createElement(v.TableCell, null, "Remove")), e > 0 && !this.state.addPackageDialogOpen && o().createElement(v.TableRow, null, o().createElement(v.TableCell, {
                             colSpan: 3,
                             sx: {
                                 top: "37px"
                             }
-                        }, s().createElement("div", {
+                        }, o().createElement("div", {
                             className: "env-pane-search-container"
-                        }, s().createElement("div", {
+                        }, o().createElement("div", {
                             className: "env-pane-searchbox"
-                        }, s().createElement("input", {
+                        }, o().createElement("input", {
                             style: {
                                 width: "100%"
                             },
                             placeholder: "Search packages...",
                             onChange: e => this.handleChangePackageFilter(e, !1),
                             className: "env-pane-input-bar"
-                        }))))), this.state.addPackageDialogOpen && s().createElement(v.TableRow, {
+                        }))))), this.state.addPackageDialogOpen && o().createElement(v.TableRow, {
                             sx: {
                                 position: "relative",
                                 zIndex: 100
                             }
-                        }, s().createElement(v.TableCell, {
+                        }, o().createElement(v.TableCell, {
                             colSpan: 3,
                             sx: {
                                 top: "37px"
                             }
-                        }, this.renderSeachPackagePane()))), s().createElement(v.TableBody, null, 0 === e ? s().createElement(v.TableRow, null, s().createElement(v.TableCell, {
+                        }, this.renderSeachPackagePane()))), o().createElement(v.TableBody, null, 0 === e ? o().createElement(v.TableRow, null, o().createElement(v.TableCell, {
                             colSpan: 3
-                        }, s().createElement("p", {
+                        }, o().createElement("p", {
                             className: "env-pane-prompt",
                             style: {
                                 textAlign: "center"
                             }
                         }, "No packages have been added to this environment"))) : !this.props.packageLoading && this.state.packagesInImage.filter((e => !this.state.packageFilter || -1 !== e.split("=")[0].toLowerCase().trim().indexOf(this.state.packageFilter))).sort(((e, t) => e.toLowerCase() > t.toLowerCase() ? 1 : -1)).map(((e, t) => {
                             let n = e.split("=="),
                                 i = n[0],
                                 a = n[1];
-                            return s().createElement(v.TableRow, {
+                            return o().createElement(v.TableRow, {
                                 key: i,
                                 sx: {
                                     "&:last-child td, &:last-child th": {
                                         border: 0
                                     }
                                 }
-                            }, s().createElement(v.TableCell, {
+                            }, o().createElement(v.TableCell, {
                                 component: "th",
                                 scope: "row"
-                            }, i), s().createElement(v.TableCell, {
+                            }, i), o().createElement(v.TableCell, {
                                 sx: {
                                     wordBreak: "break-word",
                                     wordWrap: "break-word",
                                     overflowWrap: "break-word",
                                     textWrap: "balance"
                                 }
-                            }, a), this.props.env.installed && s().createElement(v.TableCell, {
+                            }, a), this.props.env.installed && o().createElement(v.TableCell, {
                                 sx: {
                                     textAlign: "right",
                                     color: "indianred"
                                 }
-                            }, s().createElement(v.Tooltip, {
+                            }, o().createElement(v.Tooltip, {
                                 title: "Remove package",
                                 arrow: !0,
                                 placement: "right"
-                            }, s().createElement(v.IconButton, {
+                            }, o().createElement(v.IconButton, {
                                 size: "small",
                                 color: "error",
                                 disabled: this.props.installing || this.props.env.isPreInstalled || this.state.lockedEnv,
                                 onClick: () => {
                                     !this.props.installing && !this.props.env.isPreInstalled && this.handleRemovePkg(e)
                                 }
-                            }, s().createElement(z.Close, null)))))
+                            }, o().createElement(z.Close, null)))))
                         })), (this.props.packageLoading || this.state.packageListLoading) && Array.from({
                             length: 4
-                        }, ((e, t) => t + 1)).map((e => s().createElement(v.TableRow, {
+                        }, ((e, t) => t + 1)).map((e => o().createElement(v.TableRow, {
                             key: e
-                        }, s().createElement(v.TableCell, {
+                        }, o().createElement(v.TableCell, {
                             colSpan: 3
-                        }, s().createElement(v.Skeleton, {
+                        }, o().createElement(v.Skeleton, {
                             variant: "text"
-                        })))))))), this.renderPopupMsg(this.state.popupMsg)), !this.state.addPackageDialogOpen && this.props.env.installed && s().createElement("div", {
+                        })))))))), this.renderPopupMsg(this.state.popupMsg)), !this.state.addPackageDialogOpen && this.props.env.installed && o().createElement("div", {
                             className: "env-pane-button-group",
                             style: {
                                 paddingTop: 10,
                                 paddingBottom: 5
                             }
-                        }, s().createElement("button", {
+                        }, o().createElement("button", {
                             className: "env-pane-button " + (this.state.pkgListBusy || this.props.env.isPreInstalled ? "disabled" : "filled"),
                             onClick: !this.props.env.isPreInstalled && this.openAddPackageDialog,
                             disabled: this.state.pkgListBusy || this.props.env.isPreInstalled
-                        }, "+ Add a package")), this.state.addPackageDialogOpen && this.props.env.installed && s().createElement("div", {
+                        }, "+ Add a package")), this.state.addPackageDialogOpen && this.props.env.installed && o().createElement("div", {
                             className: "env-pane-button-group",
                             style: {
                                 paddingTop: 10,
                                 paddingBottom: 5
                             }
-                        }, s().createElement(v.Tooltip, {
+                        }, o().createElement(v.Tooltip, {
                             title: "Click to return back",
                             open: this.state.packageNotInList,
                             arrow: !0,
                             placement: "top",
                             componentsProps: {
                                 tooltip: {
                                     sx: {
@@ -2107,18 +2320,18 @@
                                         bgcolor: "#673ab7",
                                         "& .MuiTooltip-arrow": {
                                             color: "#673ab7"
                                         }
                                     }
                                 }
                             }
-                        }, s().createElement("button", {
+                        }, o().createElement("button", {
                             className: "env-pane-button outlined",
                             onClick: this.closeAddPackageDialog
-                        }, "Cancel")), s().createElement(v.Tooltip, {
+                        }, "Cancel")), o().createElement(v.Tooltip, {
                             title: "Click to Add Package",
                             open: this.state.packageNotInList,
                             arrow: !0,
                             placement: "top",
                             componentsProps: {
                                 tooltip: {
                                     sx: {
@@ -2126,36 +2339,36 @@
                                         bgcolor: "#673ab7",
                                         "& .MuiTooltip-arrow": {
                                             color: "#673ab7"
                                         }
                                     }
                                 }
                             }
-                        }, s().createElement("button", {
-                            className: "env-pane-button " + (q().isEmpty(this.state.selectedPkg) || this.props.installing ? "disabled" : "filled"),
+                        }, o().createElement("button", {
+                            className: "env-pane-button " + (_().isEmpty(this.state.selectedPkg) || this.props.installing ? "disabled" : "filled"),
                             onClick: () => {
                                 var e, t;
                                 return this.handleAddPackageToList((null === (t = null === (e = this.state.selectedPkg) || void 0 === e ? void 0 : e.info) || void 0 === t ? void 0 : t.name) + this.state.selectedOperator + this.state.selectedPkgVersion)
                             },
-                            disabled: q().isEmpty(this.state.selectedPkg) || this.props.installing
+                            disabled: _().isEmpty(this.state.selectedPkg) || this.props.installing
                         }, "+ Add")))))
-                    }, this.renderSeachPackagePane = () => s().createElement("div", {
+                    }, this.renderSeachPackagePane = () => o().createElement("div", {
                         className: "env-pane-search-container env-edior-slide-in-top"
-                    }, s().createElement("div", {
+                    }, o().createElement("div", {
                         className: "env-pane-searchbox"
-                    }, s().createElement("input", {
+                    }, o().createElement("input", {
                         type: "text",
                         name: "searchbar",
                         value: this.state.searchInput,
                         className: "env-pane-input-bar",
                         placeholder: "Add package...",
                         onChange: this.handleInputChanges,
                         onKeyDown: this.handleEnterKeypress,
                         autoFocus: !0
-                    }), s().createElement(v.Tooltip, {
+                    }), o().createElement(v.Tooltip, {
                         title: "Click to Search Packages",
                         open: this.state.packageNotInList,
                         arrow: !0,
                         placement: "top",
                         componentsProps: {
                             tooltip: {
                                 sx: {
@@ -2164,52 +2377,52 @@
                                     "& .MuiTooltip-arrow": {
                                         color: "#673ab7"
                                     },
                                     marginBottom: "-8px !important"
                                 }
                             }
                         }
-                    }, s().createElement("div", {
+                    }, o().createElement("div", {
                         onClick: this.handleSearchSubmit,
                         className: this.state.searchInput.length >= 3 ? "shake-bottom" : ""
-                    }, s().createElement(U, {
+                    }, o().createElement(j, {
                         color: this.state.searchInput.length >= 3 ? "#673ab7" : "#ABABAB"
-                    })))), q().isEmpty(this.state.searchResults) && this.state.isDropdownVisible && this.renderErrorDropdown(), !q().isEmpty(this.state.searchResults) && this.state.isDropdownVisible && this.renderDropdown(), this.state.packageNotInList && this.renderAlertDropDown()), this.renderDropdown = () => {
-                        var e, t, n, i, a, o, r, l, c, d, p, h, m;
+                    })))), _().isEmpty(this.state.searchResults) && this.state.isDropdownVisible && this.renderErrorDropdown(), !_().isEmpty(this.state.searchResults) && this.state.isDropdownVisible && this.renderDropdown(), this.state.packageNotInList && this.renderAlertDropDown()), this.renderDropdown = () => {
+                        var e, t, n, i, a, s, r, l, c, d, p, h, m;
                         const g = ["==", "~=", "<", "<=", ">", ">="];
-                        return s().createElement("div", {
+                        return o().createElement("div", {
                             className: "env-pane-dropdown slide-in-top"
-                        }, s().createElement("ul", {
+                        }, o().createElement("ul", {
                             className: "env-pane-dropdown-list"
-                        }, s().createElement("li", {
+                        }, o().createElement("li", {
                             className: (null === (e = this.state.selectedPkg) || void 0 === e ? void 0 : e.last_serial) === (null === (t = this.state.searchResults) || void 0 === t ? void 0 : t.last_serial) ? "filled" : "",
                             onClick: () => this.handleSelectPackage(this.state.searchResults)
-                        }, s().createElement(L, {
+                        }, o().createElement(L, {
                             width: "34",
                             height: "36",
                             filter: (null === (n = this.state.selectedPkg) || void 0 === n ? void 0 : n.last_serial) === (null === (i = this.state.searchResults) || void 0 === i ? void 0 : i.last_serial) ? "drop-shadow(2px 4px 6px rgba(0,0,0,0.2))" : ""
-                        }), s().createElement("span", {
+                        }), o().createElement("span", {
                             className: "env-pane-flexrow"
-                        }, s().createElement("p", {
+                        }, o().createElement("p", {
                             className: "env-pane-dropdown-name"
-                        }, null === (o = null === (a = this.state.searchResults) || void 0 === a ? void 0 : a.info) || void 0 === o ? void 0 : o.name), s().createElement("p", {
+                        }, null === (s = null === (a = this.state.searchResults) || void 0 === a ? void 0 : a.info) || void 0 === s ? void 0 : s.name), o().createElement("p", {
                             className: "env-pane-dropdown-version"
-                        }, s().createElement("select", {
+                        }, o().createElement("select", {
                             className: "operator-selector",
                             name: "operatorSelector",
                             value: this.state.selectedOperator,
                             disabled: "any" === this.state.selectedPkgVersion,
                             onChange: e => this.setState({
                                 selectedOperator: e.target.value
                             })
-                        }, g.map((e => s().createElement("option", {
+                        }, g.map((e => o().createElement("option", {
                             value: e
-                        }, e))))), s().createElement("p", {
+                        }, e))))), o().createElement("p", {
                             className: "env-pane-dropdown-version"
-                        }, s().createElement("select", {
+                        }, o().createElement("select", {
                             style: {
                                 fontWeight: "600",
                                 width: "70px",
                                 padding: ".3em",
                                 border: (null === (r = this.state.selectedPkg) || void 0 === r ? void 0 : r.last_serial) === (null === (l = this.state.searchResults) || void 0 === l ? void 0 : l.last_serial) ? "1px solid white" : "1px solid #673ab7",
                                 backgroundColor: (null === (c = this.state.selectedPkg) || void 0 === c ? void 0 : c.last_serial) === (null === (d = this.state.searchResults) || void 0 === d ? void 0 : d.last_serial) ? "#ffffff" : "#673ab7",
                                 borderRadius: "5px",
@@ -2222,367 +2435,504 @@
                             onChange: e => {
                                 this.setState({
                                     selectedPkgVersion: e.target.value
                                 }), "any" === e.target.value && this.setState({
                                     selectedOperator: g[0]
                                 })
                             }
-                        }, s().createElement("option", {
+                        }, o().createElement("option", {
                             value: "any"
-                        }, "Any"), null === (m = this.state.availableVersions) || void 0 === m ? void 0 : m.map((e => s().createElement("option", {
+                        }, "Any"), null === (m = this.state.availableVersions) || void 0 === m ? void 0 : m.map((e => o().createElement("option", {
                             value: e
                         }, e)))))))))
-                    }, this.renderErrorDropdown = () => s().createElement("div", {
+                    }, this.renderErrorDropdown = () => o().createElement("div", {
                         className: "env-pane-dropdown slide-in-top"
-                    }, s().createElement("ul", {
+                    }, o().createElement("ul", {
                         className: "env-pane-dropdown-list"
-                    }, s().createElement("li", null, s().createElement(L, {
+                    }, o().createElement("li", null, o().createElement(L, {
                         width: "34",
                         height: "36"
-                    }), s().createElement("span", {
+                    }), o().createElement("span", {
                         className: "env-pane-flexrow"
-                    }, s().createElement("p", {
+                    }, o().createElement("p", {
                         className: "env-pane-dropdown-name"
-                    }, "No package found!"))))), this.renderAlertDropDown = () => s().createElement("div", {
+                    }, "No package found!"))))), this.renderAlertDropDown = () => o().createElement("div", {
                         className: "env-pane-dropdown slide-in-top"
-                    }, s().createElement("ul", {
+                    }, o().createElement("ul", {
                         className: "env-pane-dropdown-list"
-                    }, s().createElement("li", {
+                    }, o().createElement("li", {
                         className: "env-pane-dropdown-over-ride"
-                    }, s().createElement(z.InfoOutlined, {
+                    }, o().createElement(z.InfoOutlined, {
                         width: "34",
                         height: "36"
-                    }), s().createElement("span", null, s().createElement("p", {
+                    }), o().createElement("span", null, o().createElement("p", {
                         style: {
                             fontSize: "12px",
                             fontWeight: "400"
                         }
-                    }, "The package is not installed, once query is completed, press the", " ", s().createElement("b", {
+                    }, "The package is not installed, once query is completed, press the", " ", o().createElement("b", {
                         style: {
                             color: "#673ab7"
                         }
-                    }, '"Enter"'), " key or", " ", s().createElement("b", {
+                    }, '"Enter"'), " key or", " ", o().createElement("b", {
                         style: {
                             color: "#673ab7"
                         }
                     }, '"Search Icon"'), " to retrieve the package"))))), this.renderPopupMsg = ({
                         msg: e,
                         type: t
-                    }) => s().createElement(v.Snackbar, {
-                        open: !0,
+                    }) => o().createElement(v.Snackbar, {
                         open: this.state.popupOpen,
                         autoHideDuration: 2500,
                         onClose: this.handlePopupClose,
                         sx: {
                             position: "sticky",
                             width: "300px",
                             bottom: "10px"
                         }
-                    }, s().createElement(v.Alert, {
+                    }, o().createElement(v.Alert, {
                         severity: t,
                         variant: "filled",
                         sx: {
                             position: "absolute",
                             width: "calc(100% - 3em)",
                             fontSize: "14px",
                             bottom: "10px"
                         }
-                    }, e)), this.renderInstallInfoPane = () => s().createElement(v.Grid, {
+                    }, e)), this.renderInstallInfoPane = () => o().createElement(v.Grid, {
                         item: !0,
                         xs: 12
-                    }, s().createElement("div", {
+                    }, o().createElement("div", {
                         className: "env-editor-pane-new",
                         style: {
                             minHeight: 150
                         }
-                    }, s().createElement("div", {
+                    }, o().createElement("div", {
                         className: "env-pane-content"
-                    }, this.props.packageInstallingEnv === this.props.env._id ? s().createElement(v.Stack, {
+                    }, this.props.packageInstallingEnv === this.props.env._id ? o().createElement(v.Stack, {
                         sx: {
                             width: "100%",
                             color: "grey.500"
                         },
                         spacing: 1
-                    }, s().createElement(v.Typography, {
+                    }, o().createElement(v.Typography, {
                         className: "env-pane-prompt"
-                    }, "Package is being installed"), s().createElement(v.LinearProgress, {
+                    }, "Package is being installed"), o().createElement(v.LinearProgress, {
                         variant: "determinate",
                         value: this.props.packageProgress,
                         sx: {
                             backgroundColor: "#edcefd",
                             "& .MuiLinearProgress-bar": {
                                 backgroundColor: "#673ab7"
                             }
                         }
-                    })) : s().createElement(v.Stack, {
+                    })) : o().createElement(v.Stack, {
                         sx: {
                             width: "100%",
                             color: "grey.500"
                         },
                         spacing: 1
-                    }, s().createElement(v.Typography, {
+                    }, o().createElement(v.Typography, {
                         className: "env-pane-prompt"
-                    }, this.state.cancelling ? "Cancelling installation" : "Environment is being installed/updated"), s().createElement(v.LinearProgress, {
+                    }, this.state.cancelling ? "Cancelling installation" : "Environment is being installed/updated"), o().createElement(v.LinearProgress, {
                         sx: {
                             backgroundColor: this.state.cancelling ? "red" : "#9909e091",
                             "& .MuiLinearProgress-bar": {
                                 backgroundColor: this.state.cancelling ? "darkred" : "#673ab7"
                             }
                         }
                     }))))), this.renderUpdatePane = () => {
-                        var e, t;
+                        var e, t, n;
                         if (this.props.env.isPreInstalled) return null;
-                        let n;
+                        let i;
                         if (this.state.isCustom) {
-                            const i = M(this.props.env.createdAt),
-                                a = M(this.props.env.updatedAt),
-                                s = null !== (t = null === (e = this.state.readAccessUsers) || void 0 === e ? void 0 : e.length) && void 0 !== t ? t : 0;
-                            n = `createdAt: ${i} UTC\n\nupdatedAt: ${a} UTC\n\nsharedWith: ${s} user${1===s?"":"s"}`
-                        } else n = this.props.env.canUpdate ? `An updated version of the ${this.props.env.displayName} environment is available!` : `Your ${this.props.env.displayName} environment is up-to-date with the latest version.`;
-                        const i = this.state.isInstalled ? 150 : 105;
-                        return s().createElement(v.Grid, {
+                            const n = W(this.props.env.createdAt),
+                                a = W(this.props.env.updatedAt),
+                                s = null !== (t = null === (e = this.state.readAccessUsers) || void 0 === e ? void 0 : e.length) && void 0 !== t ? t : 0,
+                                r = `${s} user${1===s?"":"s"}`;
+                            i = o().createElement(v.Typography, {
+                                fontSize: 14,
+                                color: "text.secondary"
+                            }, "createdAt: ", n, " UTC", o().createElement("br", null), "updatedAt: ", a, " UTC", o().createElement("br", null), "sharedWith: ", r)
+                        } else i = this.props.env.canUpdate ? o().createElement(v.Typography, {
+                            fontSize: 14,
+                            color: "text.secondary"
+                        }, "An updated version of the ", this.props.env.displayName, " environment is available!") : o().createElement(v.Typography, {
+                            fontSize: 14,
+                            color: "text.secondary"
+                        }, "Your ", this.props.env.displayName, " environment is up-to-date with the latest version.");
+                        const a = this.state.isInstalled ? 150 : 105;
+                        return o().createElement(v.Grid, {
                             item: !0,
                             xs: 12
-                        }, s().createElement("div", {
+                        }, o().createElement("div", {
                             className: "env-editor-pane-new",
                             style: {
-                                minHeight: i
+                                minHeight: a
+                            }
+                        }, o().createElement("div", {
+                            className: "env-pane-content",
+                            style: {
+                                gap: "8px"
                             }
-                        }, s().createElement("div", {
-                            className: "env-pane-content"
-                        }, s().createElement(v.Stack, {
+                        }, o().createElement(v.Stack, {
                             direction: "row",
                             alignItems: "flex-start",
                             gap: 2
-                        }, this.props.env.canUpdate ? s().createElement(z.Update, null) : s().createElement(z.UpdateDisabled, null), s().createElement(v.Typography, {
-                            className: "env-pane-prompt"
-                        }, n)), this.state.uninstalling && s().createElement(v.Stack, {
+                        }, this.props.env.canUpdate ? o().createElement(z.Update, {
+                            color: "action",
+                            fontSize: "small"
+                        }) : o().createElement(z.UpdateDisabled, {
+                            color: "action",
+                            fontSize: "small"
+                        }), i), o().createElement(v.Grid, {
+                            container: !0,
+                            spacing: 1
+                        }, this.state.isMount && this.props.env.installed && [R, this.props.qbUser.user._id].includes(this.props.env.owner) && o().createElement(o().Fragment, null, o().createElement(v.Grid, {
+                            item: !0,
+                            xs: 12
+                        }, o().createElement(v.Divider, {
+                            orientation: "horizontal"
+                        })), "pending" === (null === (n = this.props.env) || void 0 === n ? void 0 : n.reviewStatus) && "contact@qbraid.com" === this.props.qbUser.user.email && o().createElement(v.Grid, {
+                            item: !0,
+                            container: !0,
+                            xs: 12,
+                            spacing: 1
+                        }, o().createElement(v.Grid, {
+                            item: !0,
+                            xs: 5
+                        }, o().createElement(v.Button, {
+                            fullWidth: !0,
+                            variant: "outlined",
+                            size: "small",
+                            color: "error",
+                            sx: {
+                                textTransform: "none",
+                                fontSize: 13
+                            },
+                            startIcon: o().createElement(z.CloudOffTwoTone, null),
+                            onClick: this.denyPublishingEnvironment
+                        }, "Deny Request")), o().createElement(v.Grid, {
+                            item: !0,
+                            xs: 7
+                        }, o().createElement(v.Button, {
+                            fullWidth: !0,
+                            variant: "contained",
+                            size: "small",
+                            color: "secondary",
+                            sx: {
+                                textTransform: "none",
+                                fontSize: 13
+                            },
+                            startIcon: o().createElement(z.CloudDoneTwoTone, null),
+                            onClick: this.publishEnvironment
+                        }, "Approve publish request"))), o().createElement(v.Grid, {
+                            item: !0,
+                            xs: 12
+                        }, this.props.env.readAccessUsers.includes(R) ? o().createElement(M, {
+                            env: this.props.env
+                        }) : o().createElement(v.Button, {
+                            fullWidth: !0,
+                            variant: "contained",
+                            size: "small",
+                            color: "secondary",
+                            sx: {
+                                textTransform: "none"
+                            },
+                            startIcon: this.state.publishLoading ? o().createElement(z.CloudSyncTwoTone, null) : o().createElement(z.BackupTwoTone, null),
+                            onClick: () => {
+                                this.setState({
+                                    actionAlertContext: {
+                                        content: "publish",
+                                        title: "Confirm Environment Publish Request",
+                                        body: "Are you sure you want to submit your custom environment for review? By requesting to publish, you are agreeing to transfer ownership of your environment to qBraid. If approved, it will be made publicly available for all qBraid Lab users to install. Please confirm your submission or cancel if you wish to make any further changes.",
+                                        confirmButtonText: "Submit for Review",
+                                        cancelButtonText: "Cancel"
+                                    }
+                                }, (() => {
+                                    this.handleActionAlertOpen()
+                                }))
+                            },
+                            disabled: this.state.publishLoading
+                        }, this.state.publishLoading ? "Processing publish request..." : "Request to publish")))), this.state.uninstalling && o().createElement(v.Stack, {
                             gap: 1
-                        }, s().createElement(v.Typography, {
+                        }, o().createElement(v.Typography, {
                             className: "env-pane-prompt"
-                        }, `Uninstalling ${this.props.env.displayName}`), s().createElement(v.LinearProgress, {
+                        }, `Uninstalling ${this.props.env.displayName}`), o().createElement(v.LinearProgress, {
                             sx: {
                                 backgroundColor: this.state.uninstalling ? "red" : "#9909e091",
                                 "& .MuiLinearProgress-bar": {
                                     backgroundColor: this.state.uninstalling ? "darkred" : "#673ab7"
                                 }
                             }
-                        })))))
-                    }, this.renderDeletePane = () => s().createElement(v.Grid, {
+                        })))), this.renderShareMsg())
+                    }, this.renderDeletePane = () => o().createElement(v.Grid, {
                         item: !0,
                         xs: 12
-                    }, s().createElement("div", {
+                    }, o().createElement("div", {
                         className: "env-editor-pane-new"
-                    }, s().createElement("div", {
+                    }, o().createElement("div", {
                         className: "env-pane-content"
-                    }, s().createElement("p", {
+                    }, o().createElement("p", {
                         className: "editor-action-alt",
                         style: this.state.deleting || this.props.installing ? {
                             backgroundColor: "#b67d7d",
                             cursor: "not-allowed"
                         } : null,
                         onClick: this.state.deleting || this.props.installing ? null : this.handleDeleteAlertOpen
-                    }, s().createElement("span", null, s().createElement("img", {
+                    }, o().createElement("span", null, o().createElement("img", {
                         style: {
                             marginRight: 8,
                             height: 14,
                             filter: "invert(1)"
                         },
                         src: "https://qbraid-static.s3.amazonaws.com/trash.svg"
-                    })), s().createElement("span", {
+                    })), o().createElement("span", {
                         style: {
                             verticalAlign: "text-bottom"
                         }
-                    }, this.state.deleting ? "Deleting..." : "Delete")), s().createElement("p", {
+                    }, this.state.deleting ? "Deleting..." : "Delete")), o().createElement("p", {
                         className: "env-pane-prompt"
-                    }, "Deleting an environment will remove it permanently.")))), this.renderUninstallPane = () => !this.props.env.installed && this.state.isOwner ? this.renderDeletePane() : !this.props.env || this.props.env.installed && !this.props.env.isPreInstalled ? s().createElement(v.Grid, {
+                    }, "Deleting an environment will remove it permanently.")))), this.renderUninstallPane = () => !this.props.env.installed && this.state.isOwner ? this.renderDeletePane() : !this.props.env || this.props.env.installed && !this.props.env.isPreInstalled ? o().createElement(v.Grid, {
                         item: !0,
                         xs: 12
-                    }, s().createElement("div", {
+                    }, o().createElement("div", {
                         className: "env-editor-pane-new"
-                    }, s().createElement("div", {
+                    }, o().createElement("div", {
                         className: "env-pane-content"
-                    }, s().createElement("p", {
+                    }, o().createElement("p", {
                         className: "editor-action-alt",
                         style: this.state.uninstalling || this.props.installing ? {
                             backgroundColor: "#b67d7d",
                             cursor: "not-allowed"
                         } : null,
                         onClick: this.state.uninstalling || this.props.installing ? null : this.handleUninstallAlertOpen
-                    }, s().createElement("span", null, s().createElement("img", {
+                    }, o().createElement("span", null, o().createElement("img", {
                         style: {
                             marginRight: 8,
                             height: 14,
                             filter: "invert(1)"
                         },
                         src: "https://qbraid-static.s3.amazonaws.com/trash.svg"
-                    })), s().createElement("span", {
+                    })), o().createElement("span", {
                         style: {
                             verticalAlign: "text-bottom"
                         }
-                    }, this.state.uninstalling ? "Uninstalling..." : "Uninstall")), s().createElement("p", {
+                    }, this.state.uninstalling ? "Uninstalling..." : "Uninstall")), o().createElement("p", {
                         className: "env-pane-prompt"
-                    }, "Uninstalling an environment will remove it from your file system, freeing up disk space, and allow you to reinstall the most up-to-date version, if applicable.")))) : null, this.renderUninstallAlert = () => s().createElement(v.Dialog, {
+                    }, "Uninstalling an environment will remove it from your file system, freeing up disk space, and allow you to reinstall the most up-to-date version, if applicable.")))) : null, this.handleActionAlertOpen = () => {
+                        this.setState({
+                            actionAlert: !0
+                        })
+                    }, this.handleActionAlertClose = () => {
+                        this.setState({
+                            actionAlert: !1,
+                            actionAlertContext: {
+                                content: "",
+                                title: "",
+                                body: "",
+                                confirmButtonText: "",
+                                cancelButtonText: ""
+                            }
+                        })
+                    }, this.confirmButtonAction = () => {
+                        "publish" === this.state.actionAlertContext.content && (this.requestPublishEnvironment(), this.handleActionAlertClose())
+                    }, this.cancelButtonAction = () => {
+                        "publish" === this.state.actionAlertContext.content && this.handleActionAlertClose()
+                    }, this.actionAlert = () => o().createElement(v.Dialog, {
+                        open: this.state.actionAlert,
+                        onClose: this.handleActionAlertClose,
+                        "aria-labelledby": "alert-dialog-title",
+                        "aria-describedby": "alert-dialog-description",
+                        className: "action-alert-dialog-box",
+                        transitionDuration: 100
+                    }, o().createElement(v.DialogTitle, {
+                        id: "alert-dialog-title"
+                    }, this.state.actionAlertContext.title), o().createElement(v.DialogContent, {
+                        id: "alert-dialog-content"
+                    }, o().createElement(v.DialogContentText, {
+                        id: "alert-dialog-description"
+                    }, this.state.actionAlertContext.body)), o().createElement(v.DialogActions, {
+                        id: "alert-dialog-actions"
+                    }, o().createElement(v.Button, {
+                        variant: "outlined",
+                        color: "error",
+                        onClick: this.cancelButtonAction,
+                        sx: {
+                            textTransform: "none",
+                            minWidth: "120px"
+                        }
+                    }, this.state.actionAlertContext.cancelButtonText), o().createElement(v.Button, {
+                        color: "secondary",
+                        variant: "contained",
+                        sx: {
+                            textTransform: "none",
+                            minWidth: "120px"
+                        },
+                        onClick: this.confirmButtonAction,
+                        autoFocus: !0,
+                        disableFocusRipple: !0
+                    }, this.state.actionAlertContext.confirmButtonText))), this.renderUninstallAlert = () => o().createElement(v.Dialog, {
                         open: this.state.uninstallAlert,
                         onClose: this.handleUninstallAlertClose,
                         "aria-labelledby": "alert-dialog-title",
                         "aria-describedby": "alert-dialog-description",
                         className: "env-unins-dialog-box",
                         transitionDuration: 100
-                    }, s().createElement(v.DialogTitle, {
+                    }, o().createElement(v.DialogTitle, {
                         id: "alert-dialog-title"
-                    }, this.state.cancelRequest ? "Confirm Cancellation" : "Confirm Uninstall"), s().createElement(v.DialogContent, {
+                    }, this.state.cancelRequest ? "Confirm Cancellation" : "Confirm Uninstall"), o().createElement(v.DialogContent, {
                         id: "alert-dialog-content"
-                    }, s().createElement(v.DialogContentText, {
+                    }, o().createElement(v.DialogContentText, {
                         id: "alert-dialog-description"
-                    }, this.state.cancelRequest ? "Are you sure you want to cancel installing this environment?" : "Are you sure you want to uninstall this environment?")), s().createElement(v.DialogActions, {
+                    }, this.state.cancelRequest ? "Are you sure you want to cancel installing this environment?" : "Are you sure you want to uninstall this environment?")), o().createElement(v.DialogActions, {
                         id: "alert-dialog-actions"
-                    }, s().createElement(v.Button, {
+                    }, o().createElement(v.Button, {
                         variant: "slide",
                         type: "decline",
                         onClick: this.handleUninstallAlertClose,
                         sx: {
                             textTransform: "none",
                             minWidth: "120px"
                         }
-                    }, "Cancel"), s().createElement(v.Button, {
+                    }, "Cancel"), o().createElement(v.Button, {
                         className: "env-unins-alert-box-uninstall-button",
                         variant: "slide",
                         sx: {
                             textTransform: "none",
                             minWidth: "120px"
                         },
                         onClick: this.handleCustomUninstall,
                         autoFocus: !0,
                         disableFocusRipple: !0
-                    }, this.state.cancelRequest ? "Cancel Installation" : "Uninstall"))), this.renderDeleteAlert = () => s().createElement(v.Dialog, {
+                    }, this.state.cancelRequest ? "Cancel Installation" : "Uninstall"))), this.renderDeleteAlert = () => o().createElement(v.Dialog, {
                         open: this.state.deleteAlert,
                         onClose: this.handleDeleteAlertClose,
                         "aria-labelledby": "alert-dialog-title",
                         "aria-describedby": "alert-dialog-description",
                         className: "env-unins-dialog-box",
                         transitionDuration: 100
-                    }, s().createElement(v.DialogTitle, {
+                    }, o().createElement(v.DialogTitle, {
                         id: "alert-dialog-title",
                         fontWeight: 600
-                    }, "Are you sure?"), s().createElement(v.DialogContent, {
+                    }, "Are you sure?"), o().createElement(v.DialogContent, {
                         id: "alert-dialog-content"
-                    }, s().createElement(v.DialogContentText, {
+                    }, o().createElement(v.DialogContentText, {
                         id: "alert-dialog-description"
-                    }, "Proceeding will lead to permanent deletion of environment", " ", s().createElement("b", null, this.props.env.displayName), ". This action cannot be undone.")), s().createElement(v.DialogActions, {
+                    }, "Proceeding will lead to permanent deletion of environment", " ", o().createElement("b", null, this.props.env.displayName), ". This action cannot be undone.")), o().createElement(v.DialogActions, {
                         id: "alert-dialog-actions"
-                    }, s().createElement(v.Button, {
+                    }, o().createElement(v.Button, {
                         variant: "slide",
                         type: "decline",
                         onClick: this.handleDeleteAlertClose,
                         sx: {
                             textTransform: "none",
                             minWidth: "120px"
                         }
-                    }, "Cancel"), s().createElement(v.Button, {
+                    }, "Cancel"), o().createElement(v.Button, {
                         className: "env-unins-alert-box-uninstall-button",
                         variant: "slide",
                         sx: {
                             textTransform: "none",
                             minWidth: "120px"
                         },
                         onClick: this.handleDelete,
                         autoFocus: !0,
                         disableFocusRipple: !0
-                    }, "Delete"))), this.renderCancelInstallPane = () => this.props.env && this.props.env.isPreInstalled ? null : s().createElement(v.Grid, {
+                    }, "Delete"))), this.renderCancelInstallPane = () => this.props.env && this.props.env.isPreInstalled ? null : o().createElement(v.Grid, {
                         item: !0,
                         xs: 12
-                    }, s().createElement("div", {
+                    }, o().createElement("div", {
                         className: "env-editor-pane-new",
                         style: {
                             minHeight: 150
                         }
-                    }, s().createElement("div", {
+                    }, o().createElement("div", {
                         className: "env-pane-content"
-                    }, s().createElement(v.Button, {
+                    }, o().createElement(v.Button, {
                         fullWidth: !0,
                         variant: "contained",
                         size: "medium",
                         sx: {
                             textTransform: "none",
                             backgroundColor: "darkred",
                             borderRadius: "6px",
                             "&:hover": {
                                 backgroundColor: "red"
                             }
                         },
-                        startIcon: s().createElement(z.NotInterested, null),
+                        startIcon: o().createElement(z.NotInterested, null),
                         onClick: !this.state.cancelling && this.handleCancelReq,
                         disabled: this.state.cancelling || this.props.packageInstallingEnv === this.props.env._id
                     }, this.state.cancelling ? "Cancelling..." : "Cancel Installation")))), this.renderExtraUninsConfirmAlert = () => {
                         var e;
-                        return s().createElement(v.Dialog, {
+                        return o().createElement(v.Dialog, {
                             open: this.state.extraUninstallAlert,
                             onClose: this.handleExtraUninsConfirmClose,
                             "aria-labelledby": "alert-dialog-title",
                             "aria-describedby": "alert-dialog-description",
                             className: "env-unins-dialog-box",
                             transitionDuration: 100
-                        }, s().createElement(v.DialogTitle, {
+                        }, o().createElement(v.DialogTitle, {
                             id: "alert-dialog-title"
-                        }, "Are you sure?"), s().createElement(v.DialogContent, {
+                        }, "Are you sure?"), o().createElement(v.DialogContent, {
                             id: "alert-dialog-content"
-                        }, s().createElement(v.DialogContentText, {
+                        }, o().createElement(v.DialogContentText, {
                             id: "alert-dialog-description"
-                        }, `${this.state.cancelRequest?"Cancelling":"Uninstalling"} will lead to permanent deletion of environment '${c.displayName}'${(null===(e=this.props.env.readAccessUsers)||void 0===e?void 0:e.length)>0?" and remove access from all users that it has been shared with":""}. This action cannot be undone.`)), s().createElement(v.DialogActions, {
+                        }, `${this.state.cancelRequest?"Cancelling":"Uninstalling"} will lead to permanent deletion of environment '${c.displayName}'${(null===(e=this.props.env.readAccessUsers)||void 0===e?void 0:e.length)>0?" and remove access from all users that it has been shared with":""}. This action cannot be undone.`)), o().createElement(v.DialogActions, {
                             id: "alert-dialog-actions"
-                        }, s().createElement(v.Button, {
+                        }, o().createElement(v.Button, {
                             variant: "slide",
                             type: "decline",
                             onClick: this.handleExtraUninsConfirmClose,
                             sx: {
                                 textTransform: "none",
                                 minWidth: "120px"
                             }
-                        }, "Cancel"), s().createElement(v.Button, {
+                        }, "Cancel"), o().createElement(v.Button, {
                             className: "env-unins-alert-box-uninstall-button",
                             sx: {
                                 textTransform: "none",
                                 minWidth: "120px"
                             },
                             onClick: this.handleUninstall,
                             variant: "slide",
                             autoFocus: !0,
                             disableFocusRipple: !0
                         }, "Permanently Delete")))
-                    }, this.renderDialogFooter = () => this.state.canModify ? s().createElement(v.DialogActions, {
+                    }, this.renderDialogFooter = () => this.state.canModify ? o().createElement(v.DialogActions, {
                         sx: {
                             justifyContent: "center",
                             padding: "10px",
                             background: "linear-gradient(120deg, #35383a 10%, #5e5f61 100%)"
                         }
-                    }, s().createElement(v.Button, {
+                    }, o().createElement(v.Button, {
                         sx: {
                             padding: "0.3rem 2.5rem",
                             minWidth: "100px"
                         },
                         variant: "slide",
                         type: "decline",
                         onClick: () => {
                             this.props.onClose()
                         }
-                    }, "cancel"), s().createElement(v.Button, {
+                    }, "cancel"), o().createElement(v.Button, {
                         sx: {
                             padding: "0.3rem 2.5rem",
                             minWidth: "100px"
                         },
                         variant: "slide",
                         onClick: this.handleSubmit
-                    }, c ? "Save" : "Create")) : s().createElement(v.DialogActions, {
+                    }, c ? "Save" : "Create")) : o().createElement(v.DialogActions, {
                         sx: {
                             justifyContent: "center",
                             padding: "10px",
                             background: "linear-gradient(120deg, #35383a 10%, #5e5f61 100%)"
                         }
-                    }, s().createElement(v.Button, {
+                    }, o().createElement(v.Button, {
                         sx: {
                             padding: "0.3rem 2.5rem",
                             minWidth: "100px"
                         },
                         variant: "slide",
                         type: "decline",
                         onClick: () => {
@@ -2644,15 +2994,15 @@
                         upgradePopUp: !1,
                         qjobsStatus: {
                             open: !1,
                             error: !1,
                             message: ""
                         },
                         isCustom: null !== (i = c.tags.includes("custom")) && void 0 !== i && i,
-                        isShareNode: null !== (o = null === (a = null == h ? void 0 : h.permissionsNodes) || void 0 === a ? void 0 : a.includes("qbraid.environments.share")) && void 0 !== o && o,
+                        isShareNode: null !== (s = null === (a = null == h ? void 0 : h.permissionsNodes) || void 0 === a ? void 0 : a.includes("qbraid.environments.share")) && void 0 !== s && s,
                         textCopied: !1,
                         isInstalled: !!(null === (r = null == d ? void 0 : d.environmentCache[null == c ? void 0 : c._id]) || void 0 === r ? void 0 : r.installed),
                         showCopyIcon: !1,
                         cancelling: !1,
                         cancelRequest: !1,
                         inputBoxVisible: !1,
                         saveSuccess: !1,
@@ -2665,14 +3015,23 @@
                         accessKey: (null === (l = this.props.env) || void 0 === l ? void 0 : l.accessKey) || "",
                         accessKeyLoading: !1,
                         copyCooldown: !1,
                         resharePopUpContent: {
                             content: "",
                             title: "",
                             body: ""
+                        },
+                        publishLoading: !1,
+                        actionAlert: !1,
+                        actionAlertContext: {
+                            content: "",
+                            title: "",
+                            body: "",
+                            confirmButtonText: "",
+                            cancelButtonText: ""
                         }
                     }
                 }
                 componentDidMount() {
                     setTimeout(this.load, 1), this.props.env && setTimeout((() => {
                         this._nameInput && (this._nameInput.value = this.props.env.displayName || ""), this._descriptionInput && (this._descriptionInput.value = this.props.env.description || "")
                     }), 1);
@@ -2685,15 +3044,15 @@
                 }
                 static getDerivedStateFromProps(e, t) {
                     var n, i;
                     if (t.loadingPackages && e.env.packagesInImage.length !== t.packagesInImage.length) return Object.assign(Object.assign({}, t), {
                         loadingPackages: !1,
                         packagesInImage: e.env.packagesInImage
                     });
-                    if (!q().isEqual(e.env.readAccessUsers.sort(), t.readAccessUsers.sort())) return Object.assign(Object.assign({}, t), {
+                    if (!_().isEqual(e.env.readAccessUsers.sort(), t.readAccessUsers.sort())) return Object.assign(Object.assign({}, t), {
                         readAccessUsers: e.env.readAccessUsers
                     });
                     if (e.env.installed) {
                         const n = F[e.env.slug];
                         return !n || e.qbUser.user && e.qbUser.user.permissionsNodes && -1 !== e.qbUser.user.permissionsNodes.indexOf(n) ? Object.assign(Object.assign({}, t), {
                             lockedEnv: !1
                         }) : Object.assign(Object.assign({}, t), {
@@ -2714,97 +3073,97 @@
                         })
                     }
                 }
                 render() {
                     let {
                         env: e
                     } = this.props, t = this.props.darkmode;
-                    return s().createElement(v.Dialog, {
+                    return o().createElement(v.Dialog, {
                         fullWidth: !0,
                         maxWidth: "md",
                         open: this.state.loaded,
                         style: Object.assign(t ? {
                             backgroundColor: "#464646"
                         } : {}),
                         onClose: () => {
                             this.props.onClose()
                         }
-                    }, s().createElement(v.DialogTitle, {
+                    }, o().createElement(v.DialogTitle, {
                         className: "editor-header",
                         sx: {
                             m: 0,
                             p: 2
                         }
-                    }, e ? `${e.displayName} Environment` : "New environment", s().createElement(v.IconButton, {
+                    }, e ? `${e.displayName} Environment` : "New environment", o().createElement(v.IconButton, {
                         "aria-label": "close",
                         onClick: () => {
                             this.props.onClose()
                         },
                         sx: {
                             position: "absolute",
                             right: 8,
                             top: 12
                         }
-                    }, s().createElement(z.Close, null))), s().createElement(v.DialogContent, {
+                    }, o().createElement(z.Close, null))), o().createElement(v.DialogContent, {
                         sx: {
                             backgroundColor: "var(--jp-layout-color2)",
                             padding: "16px"
                         },
                         dividers: !0
-                    }, s().createElement(v.Grid, {
+                    }, o().createElement(v.Grid, {
                         container: !0,
                         spacing: 2
-                    }, s().createElement(v.Grid, {
+                    }, o().createElement(v.Grid, {
                         item: !0,
                         container: !0,
                         xs: 12,
                         md: 6,
                         spacing: 2
-                    }, s().createElement(v.Grid, {
+                    }, o().createElement(v.Grid, {
                         item: !0,
                         xs: 12
-                    }, this.renderInfoPane()), s().createElement(v.Grid, {
+                    }, this.renderInfoPane()), o().createElement(v.Grid, {
                         item: !0,
                         xs: 12
-                    }, this.renderSharingPane()), this.props.installing || this.state.cancelling || this.state.cancelRequest ? this.renderInstallInfoPane() : (this.state.isInstalled || this.state.isCustom) && this.renderUpdatePane()), s().createElement(v.Grid, {
+                    }, this.renderSharingPane()), this.props.installing || this.state.cancelling || this.state.cancelRequest ? this.renderInstallInfoPane() : (this.state.isInstalled || this.state.isCustom) && this.renderUpdatePane()), o().createElement(v.Grid, {
                         item: !0,
                         container: !0,
                         xs: 12,
                         md: 6,
                         spacing: 2
-                    }, s().createElement(v.Grid, {
+                    }, o().createElement(v.Grid, {
                         item: !0,
                         xs: 12
-                    }, this.renderPackagesPane()), this.props.installing || this.state.cancelling || this.state.cancelRequest ? this.renderCancelInstallPane() : this.renderUninstallPane()))), this.renderUninstallAlert(), this.renderExtraUninsConfirmAlert(), this.renderDeleteAlert())
+                    }, this.renderPackagesPane()), this.props.installing || this.state.cancelling || this.state.cancelRequest ? this.renderCancelInstallPane() : this.renderUninstallPane()))), this.actionAlert(), this.renderUninstallAlert(), this.renderExtraUninsConfirmAlert(), this.renderDeleteAlert())
                 }
             }
-            R.contextTypes = c;
-            var W = n(101);
-            g()(W.Z, {
+            G.contextTypes = c;
+            var $ = n(101);
+            g()($.Z, {
                 insert: "head",
                 singleton: !1
-            }), W.Z.locals;
-            const G = e => a.createElement("svg", {
+            }), $.Z.locals;
+            const V = e => s.createElement("svg", {
                 className: "refresh-btn",
                 xmlns: "http://www.w3.org/2000/svg",
                 x: "0px",
                 y: "0px",
                 width: "25",
                 height: "20",
                 viewBox: "0 0 30 30"
-            }, a.createElement("path", {
+            }, s.createElement("path", {
                 d: "M 15 3 C 12.031398 3 9.3028202 4.0834384 7.2070312 5.875 A 1.0001 1.0001 0 1 0 8.5058594 7.3945312 C 10.25407 5.9000929 12.516602 5 15 5 C 20.19656 5 24.450989 8.9379267 24.951172 14 L 22 14 L 26 20 L 30 14 L 26.949219 14 C 26.437925 7.8516588 21.277839 3 15 3 z M 4 10 L 0 16 L 3.0507812 16 C 3.562075 22.148341 8.7221607 27 15 27 C 17.968602 27 20.69718 25.916562 22.792969 24.125 A 1.0001 1.0001 0 1 0 21.494141 22.605469 C 19.74593 24.099907 17.483398 25 15 25 C 9.80344 25 5.5490109 21.062074 5.0488281 16 L 8 16 L 4 10 z"
             }));
-            var $ = n(2761),
-                V = n(3343),
-                H = n(5384),
-                J = n(3888),
-                K = n.n(J),
-                Y = (n(4007), n(2270), n(49), n(787), n(471));
-            const Z = {
+            var H = n(2761),
+                J = n(3343),
+                K = n(5384),
+                Y = n(3888),
+                Z = n.n(Y),
+                Q = (n(4007), n(2270), n(49), n(787), n(471));
+            const X = {
                     palette: {
                         mode: "light",
                         primary: {
                             main: "#d30982"
                         },
                         secondary: {
                             main: "#673ab7",
@@ -2863,15 +3222,15 @@
                                         color: "white"
                                     }
                                 }
                             }]
                         }
                     }
                 },
-                Q = Object.assign(Object.assign({}, Z), {
+                ee = Object.assign(Object.assign({}, X), {
                     palette: {
                         mode: "dark",
                         primary: {
                             main: "#d30982"
                         },
                         secondary: {
                             main: "#673ab7",
@@ -2885,133 +3244,133 @@
                             fontFamily: ["var(--jp-ui-font-family)"].join(",")
                         },
                         background: {
                             alternate: "#1e1e1e"
                         }
                     }
                 }),
-                X = (0, Y.Z)(Z),
-                ee = (0, Y.Z)(Q);
-            var te = n(6513);
-            g()(te.Z, {
+                te = (0, Q.Z)(X),
+                ne = (0, Q.Z)(ee);
+            var ie = n(6513);
+            g()(ie.Z, {
                 insert: "head",
                 singleton: !1
-            }), te.Z.locals;
-            const ne = ({
+            }), ie.Z.locals;
+            const ae = ({
                 timeOverMsg: e,
                 timeOverDesc: t
             }) => {
-                const [n, i] = (0, a.useState)(0);
-                return (0, a.useEffect)((() => {
+                const [n, i] = (0, s.useState)(0);
+                return (0, s.useEffect)((() => {
                     let e;
                     return n < 3 && (e = setInterval((() => {
                         i((e => e + 1))
                     }), 1e3)), () => {
                         clearInterval(e)
                     }
-                }), [n]), n < 3 ? s().createElement(v.List, {
+                }), [n]), n < 3 ? o().createElement(v.List, {
                     sx: {
                         marginX: "8px"
                     }
                 }, Array.from({
                     length: 10
-                }, ((e, t) => t + 1)).map((e => s().createElement(s().Fragment, {
+                }, ((e, t) => t + 1)).map((e => o().createElement(o().Fragment, {
                     key: e
-                }, s().createElement(v.ListItem, {
+                }, o().createElement(v.ListItem, {
                     sx: {
                         marginBottom: "8px",
                         padding: "8px !important",
                         backgroundColor: "var(--jp-layout-color2)",
                         borderRadius: "10px"
                     }
-                }, s().createElement(v.ListItemAvatar, {
+                }, o().createElement(v.ListItemAvatar, {
                     sx: {
                         minWidth: "45px !important"
                     }
-                }, s().createElement(v.Skeleton, {
+                }, o().createElement(v.Skeleton, {
                     variant: "circular",
                     height: "30px",
                     width: "30px"
-                })), s().createElement(v.ListItemText, null, s().createElement(v.Typography, {
+                })), o().createElement(v.ListItemText, null, o().createElement(v.Typography, {
                     fontSize: 16
-                }, s().createElement(v.Skeleton, {
+                }, o().createElement(v.Skeleton, {
                     variant: "text",
                     height: "16px",
                     width: "180px"
-                }))), s().createElement(v.ListItemAvatar, {
+                }))), o().createElement(v.ListItemAvatar, {
                     sx: {
                         minWidth: "30px"
                     },
                     edge: "end"
-                }, s().createElement(v.Skeleton, {
+                }, o().createElement(v.Skeleton, {
                     variant: "circular",
                     height: "30px"
-                }))))))) : s().createElement("div", {
+                }))))))) : o().createElement("div", {
                     className: "env-lds-time-over"
-                }, s().createElement("h2", null, e), s().createElement("p", null, t))
+                }, o().createElement("h2", null, e), o().createElement("p", null, t))
             };
-            ne.defaultProps = {
+            ae.defaultProps = {
                 timeOverMsg: "WORKSPACE EMPTY",
                 timeOverDesc: "Add or create an environment to get started!"
             };
-            const ie = ne,
-                ae = () => s().createElement(v.Stack, {
+            const se = ae,
+                oe = () => o().createElement(v.Stack, {
                     maxHeight: 500,
                     gap: "14px",
                     overflow: "hidden",
                     bgcolor: "var(--jp-layout-color2)",
                     pl: "14px",
                     pt: "14px",
                     borderRadius: 2,
                     sx: {
                         overflowY: "scroll"
                     }
-                }, s().createElement(v.Typography, {
+                }, o().createElement(v.Typography, {
                     fontSize: 14
-                }, 'LICENSE. qBraid is authorized by Intel® Corporation ("Intel") to enable qBraid Customers to access Intel\'s Software in binary form, (with the accompanying documentation, the "Software") solely from qBraid\'s servers for the internal use of the qBraid Customer, subject to the following conditions:'), s().createElement(v.List, {
+                }, 'LICENSE. qBraid is authorized by Intel® Corporation ("Intel") to enable qBraid Customers to access Intel\'s Software in binary form, (with the accompanying documentation, the "Software") solely from qBraid\'s servers for the internal use of the qBraid Customer, subject to the following conditions:'), o().createElement(v.List, {
                     sx: {
                         pt: 0,
                         pb: 0
                     }
-                }, s().createElement(v.ListItem, null, s().createElement(v.Typography, {
+                }, o().createElement(v.ListItem, null, o().createElement(v.Typography, {
                     fontSize: 14
-                }, "(a) qBraid Customer may not disclose, distribute or transfer any part of the Software except as provided in this Agreement, and qBraid Customer agrees to prevent unauthorized copying of the Software.")), s().createElement(v.ListItem, null, s().createElement(v.Typography, {
+                }, "(a) qBraid Customer may not disclose, distribute or transfer any part of the Software except as provided in this Agreement, and qBraid Customer agrees to prevent unauthorized copying of the Software.")), o().createElement(v.ListItem, null, o().createElement(v.Typography, {
                     fontSize: 14
-                }, "(b) qBraid Customer may not reverse engineer, decompile, or disassemble the Software.")), s().createElement(v.ListItem, null, s().createElement(v.Typography, {
+                }, "(b) qBraid Customer may not reverse engineer, decompile, or disassemble the Software.")), o().createElement(v.ListItem, null, o().createElement(v.Typography, {
                     fontSize: 14
-                }, "(c) qBraid Customer may not sublicense the Software.")), s().createElement(v.ListItem, null, s().createElement(v.Typography, {
+                }, "(c) qBraid Customer may not sublicense the Software.")), o().createElement(v.ListItem, null, o().createElement(v.Typography, {
                     fontSize: 14
-                }, "(d) The Software may contain the software and other property of third-party suppliers, some of which may be identified in, and licensed in accordance with, an enclosed license.txt file or other text or file.")), s().createElement(v.ListItem, null, s().createElement(v.Typography, {
+                }, "(d) The Software may contain the software and other property of third-party suppliers, some of which may be identified in, and licensed in accordance with, an enclosed license.txt file or other text or file.")), o().createElement(v.ListItem, null, o().createElement(v.Typography, {
                     fontSize: 14
-                }, "(e) Intel has no obligation to provide any support, technical assistance or updates for the Software."))), s().createElement(v.Typography, {
+                }, "(e) Intel has no obligation to provide any support, technical assistance or updates for the Software."))), o().createElement(v.Typography, {
                     fontSize: 14
-                }, "OWNERSHIP OF SOFTWARE AND COPYRIGHTS. Title to all copies of the Software remains with Intel or its suppliers. The Software is copyrighted and protected by the laws of the United States and other countries, and international treaty provisions. qBraid Customer may not remove any copyright notices from the Software. Except as otherwise expressly provided above, Intel grants no express or implied right under Intel patents, copyrights, trademarks, or other intellectual property rights. Transfer of the license terminates qBraid Customer's right to use the Software."), s().createElement(v.Typography, {
+                }, "OWNERSHIP OF SOFTWARE AND COPYRIGHTS. Title to all copies of the Software remains with Intel or its suppliers. The Software is copyrighted and protected by the laws of the United States and other countries, and international treaty provisions. qBraid Customer may not remove any copyright notices from the Software. Except as otherwise expressly provided above, Intel grants no express or implied right under Intel patents, copyrights, trademarks, or other intellectual property rights. Transfer of the license terminates qBraid Customer's right to use the Software."), o().createElement(v.Typography, {
                     fontSize: 14
-                }, 'DISCLAIMER OF WARRANTY. The Software is provided "AS IS" without warranty of any kind, EITHER EXPRESS OR IMPLIED, INCLUDING WITHOUT LIMITATION, WARRANTIES OF MERCHANTABILITY OR FITNESS FOR ANY PARTICULAR PURPOSE.'), s().createElement(v.Typography, {
+                }, 'DISCLAIMER OF WARRANTY. The Software is provided "AS IS" without warranty of any kind, EITHER EXPRESS OR IMPLIED, INCLUDING WITHOUT LIMITATION, WARRANTIES OF MERCHANTABILITY OR FITNESS FOR ANY PARTICULAR PURPOSE.'), o().createElement(v.Typography, {
                     fontSize: 14,
                     textTransform: "uppercase"
-                }, "LIMITATION OF LIABILITY. NEITHER INTEL NOR ITS SUPPLIERS WILL BE LIABLE FOR ANY LOSS OF PROFITS, LOSS OF USE, INTERRUPTION OF BUSINESS, OR INDIRECT, SPECIAL, INCIDENTAL, OR CONSEQUENTIAL DAMAGES OF ANY KIND WHETHER UNDER THIS AGREEMENT OR OTHERWISE, EVEN IF INTEL HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES."), s().createElement(v.Typography, {
+                }, "LIMITATION OF LIABILITY. NEITHER INTEL NOR ITS SUPPLIERS WILL BE LIABLE FOR ANY LOSS OF PROFITS, LOSS OF USE, INTERRUPTION OF BUSINESS, OR INDIRECT, SPECIAL, INCIDENTAL, OR CONSEQUENTIAL DAMAGES OF ANY KIND WHETHER UNDER THIS AGREEMENT OR OTHERWISE, EVEN IF INTEL HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES."), o().createElement(v.Typography, {
                     fontSize: 14
-                }, "LICENSE TO USE COMMENTS AND SUGGESTIONS. This Agreement does NOT obligate qBraid Customer to provide Intel with comments or suggestions regarding the Software. However, if the qBraid Customer provides Intel with comments or suggestions for the modification, correction, improvement or enhancement of (a) the Software or (b) Intel products or processes that work with the Software, qBraid Customer grants to Intel a non-exclusive, worldwide, perpetual, irrevocable, transferable, royalty-free license, with the right to sublicense, under qBraid's Customer's intellectual property rights, to incorporate or otherwise utilize those comments and suggestions."), s().createElement(v.Typography, {
+                }, "LICENSE TO USE COMMENTS AND SUGGESTIONS. This Agreement does NOT obligate qBraid Customer to provide Intel with comments or suggestions regarding the Software. However, if the qBraid Customer provides Intel with comments or suggestions for the modification, correction, improvement or enhancement of (a) the Software or (b) Intel products or processes that work with the Software, qBraid Customer grants to Intel a non-exclusive, worldwide, perpetual, irrevocable, transferable, royalty-free license, with the right to sublicense, under qBraid's Customer's intellectual property rights, to incorporate or otherwise utilize those comments and suggestions."), o().createElement(v.Typography, {
                     fontSize: 14
-                }, "TERMINATION OF THIS LICENSE. Intel or the sublicensor may terminate this license at any time if You are in breach of any of its terms or conditions. Upon termination, qBraid Customer will immediately destroy the Software, and return to Intel all copies of the Software. THIRD PARTY BENEFICIARY. Intel is an intended beneficiary of the End User License Agreement and has the right to enforce all of its terms."), s().createElement(v.Typography, {
+                }, "TERMINATION OF THIS LICENSE. Intel or the sublicensor may terminate this license at any time if You are in breach of any of its terms or conditions. Upon termination, qBraid Customer will immediately destroy the Software, and return to Intel all copies of the Software. THIRD PARTY BENEFICIARY. Intel is an intended beneficiary of the End User License Agreement and has the right to enforce all of its terms."), o().createElement(v.Typography, {
                     fontSize: 14
-                }, 'U.S. GOVERNMENT RESTRICTED RIGHTS. No Government procurement regulation or contract clauses or provision will be considered a part of any transaction between the Parties under this Agreement unless its inclusion is required by statute, or mutually agreed upon in writing by the Parties in connection with a specific transaction. The technical data and computer software covered by this license is a "Commercial Item," as that term is defined by the FAR 2.101 (48 C.F.R. 2.101) and is “commercial computer software” and "commercial computer software documentation" as specified under FAR 12.212 (48 C.F.R. 12.212) or DFARS 227.7202 (48 C.F.R. 227.7202), as applicable. This commercial computer software and related documentation is provided to end users for use by and on behalf of the U.S. Government, with only those rights as are granted to all other end users under the terms and conditions in this Agreement. Use for or on behalf of the U.S. Government is permitted only if the party acquiring or using this Software is properly authorized by an appropriate U.S. Government official. This use by or for the U.S. Government clause is in lieu of, and supersedes, any other FAR, DFARS, or other provision that addresses Government rights in the computer Software or documentation covered by this license. All copyright licenses granted to the U.S. Government are coextensive with the technical data and computer Software licenses granted in this Agreement. The U.S. Government will only have the right to reproduce, distribute, perform, display, and prepare Derivative Works as needed to implement those rights.'), s().createElement(v.Typography, {
+                }, 'U.S. GOVERNMENT RESTRICTED RIGHTS. No Government procurement regulation or contract clauses or provision will be considered a part of any transaction between the Parties under this Agreement unless its inclusion is required by statute, or mutually agreed upon in writing by the Parties in connection with a specific transaction. The technical data and computer software covered by this license is a "Commercial Item," as that term is defined by the FAR 2.101 (48 C.F.R. 2.101) and is “commercial computer software” and "commercial computer software documentation" as specified under FAR 12.212 (48 C.F.R. 12.212) or DFARS 227.7202 (48 C.F.R. 227.7202), as applicable. This commercial computer software and related documentation is provided to end users for use by and on behalf of the U.S. Government, with only those rights as are granted to all other end users under the terms and conditions in this Agreement. Use for or on behalf of the U.S. Government is permitted only if the party acquiring or using this Software is properly authorized by an appropriate U.S. Government official. This use by or for the U.S. Government clause is in lieu of, and supersedes, any other FAR, DFARS, or other provision that addresses Government rights in the computer Software or documentation covered by this license. All copyright licenses granted to the U.S. Government are coextensive with the technical data and computer Software licenses granted in this Agreement. The U.S. Government will only have the right to reproduce, distribute, perform, display, and prepare Derivative Works as needed to implement those rights.'), o().createElement(v.Typography, {
                     fontSize: 14
-                }, "EXPORT LAWS. The Software and all related technical information or materials are subject to export controls and (are or may be) licensable under U.S. Government export regulations. qBraid Customer will not export, re-export, divert, transfer or disclose, directly or indirectly, the Software, Documentation and any related technical information or materials without complying strictly with all legal requirements including, without limitation, obtaining the prior approval of the U.S. Department of Commerce and, if necessary, other agencies or departments of the U.S. Government. Upon request, Intel will provide qBraid Customer with information regarding the export classification of the Software that may be necessary to assist qBraid Customer's compliance with this provision. qBraid Customer will execute and deliver to Intel “Letters of Assurance,” confirming compliance with applicable export regulations. qBraid Customer will indemnify Intel against any loss related to qBraid Customer's failure to conform to these requirements."), s().createElement(v.Typography, {
+                }, "EXPORT LAWS. The Software and all related technical information or materials are subject to export controls and (are or may be) licensable under U.S. Government export regulations. qBraid Customer will not export, re-export, divert, transfer or disclose, directly or indirectly, the Software, Documentation and any related technical information or materials without complying strictly with all legal requirements including, without limitation, obtaining the prior approval of the U.S. Department of Commerce and, if necessary, other agencies or departments of the U.S. Government. Upon request, Intel will provide qBraid Customer with information regarding the export classification of the Software that may be necessary to assist qBraid Customer's compliance with this provision. qBraid Customer will execute and deliver to Intel “Letters of Assurance,” confirming compliance with applicable export regulations. qBraid Customer will indemnify Intel against any loss related to qBraid Customer's failure to conform to these requirements."), o().createElement(v.Typography, {
                     fontSize: 14
-                }, "APPLICABLE LAWS. This Agreement is governed by the laws of the state of Delaware, excluding its principles of conflict of laws and the United Nations Convention on Contracts for the Sale of Goods. qBraid Customer may not export the Software in violation of applicable export laws and regulations."), s().createElement(v.Typography, {
+                }, "APPLICABLE LAWS. This Agreement is governed by the laws of the state of Delaware, excluding its principles of conflict of laws and the United Nations Convention on Contracts for the Sale of Goods. qBraid Customer may not export the Software in violation of applicable export laws and regulations."), o().createElement(v.Typography, {
                     fontSize: 14
                 }, "qBraid Customer's specific rights may vary from country to country."));
-            var se = n(948),
-                oe = n(1596),
-                re = n(6532),
-                le = n(1250),
-                ce = n(3083);
-            const de = (0, se.ZP)((e => a.createElement(re.Z, Object.assign({
+            var re = n(948),
+                le = n(1596),
+                ce = n(6532),
+                de = n(1250),
+                pe = n(3083);
+            const he = (0, re.ZP)((e => s.createElement(ce.Z, Object.assign({
                     disableGutters: !0,
                     elevation: 0,
                     square: !0
                 }, e))))((({
                     theme: e
                 }) => ({
                     border: 0,
@@ -3020,16 +3379,16 @@
                     "&:not(:last-child)": {
                         borderBottom: 0
                     },
                     "&:before": {
                         display: "none"
                     }
                 }))),
-                pe = (0, se.ZP)((e => a.createElement(le.Z, Object.assign({
-                    expandIcon: a.createElement(oe.Z, {
+                me = (0, re.ZP)((e => s.createElement(de.Z, Object.assign({
+                    expandIcon: s.createElement(le.Z, {
                         sx: {
                             fontSize: "1.5rem",
                             color: "var(--jp-layout-color4)"
                         }
                     })
                 }, e))))((({
                     theme: e
@@ -3041,43 +3400,43 @@
                     "& .MuiAccordionSummary-content": {
                         margin: 0,
                         marginLeft: "8px"
                     },
                     minHeight: "35px",
                     padding: "0px 5px"
                 }))),
-                he = (0, se.ZP)(ce.Z)((({
+                ge = (0, re.ZP)(pe.Z)((({
                     theme: e
                 }) => ({
                     padding: "0px 10px 10px 10px"
                 }))),
-                me = () => s().createElement(v.Box, {
+                ue = () => o().createElement(v.Box, {
                     display: "flex",
                     flexDirection: "column",
                     justifyContent: "center",
                     alignItems: "center",
                     position: "absolute",
                     top: "45%",
                     left: "35%"
-                }, s().createElement(z.PersonOff, {
+                }, o().createElement(z.PersonOff, {
                     color: "disabled",
                     sx: {
                         width: "64px",
                         height: "64px"
                     }
-                }), s().createElement(v.Typography, {
+                }), o().createElement(v.Typography, {
                     color: "InactiveCaptionText",
                     sx: {
                         userSelect: "none"
                     }
                 }, "User not found")),
-                ge = "qbraid.environments.install",
-                ue = "qbraid-env-gpu-check-alert",
-                ve = "https://qbraid-static.s3.amazonaws.com/logos/qbraid.png",
-                be = [{
+                ve = "qbraid.environments.install",
+                be = "qbraid-env-gpu-check-alert",
+                fe = "https://qbraid-static.s3.amazonaws.com/logos/qbraid.png",
+                xe = [{
                     value: "highest_to_lowest_priority",
                     label: "Most Relevant"
                 }, {
                     value: "newest_to_oldest",
                     label: "Most Recent"
                 }, {
                     value: "most_to_least_installed",
@@ -3085,15 +3444,15 @@
                 }, {
                     value: "alphabetically_a_z",
                     label: "Alphabetically (A-Z)"
                 }, {
                     value: "alphabetically_z_a",
                     label: "Alphabetically (Z-A)"
                 }],
-                fe = [{
+                Ee = [{
                     value: "py39",
                     label: "Python 3.9.18",
                     isLocked: !0
                 }, {
                     value: "py310",
                     label: "Python 3.10.13",
                     isLocked: !0
@@ -3103,30 +3462,30 @@
                     isLocked: !0
                 }, {
                     value: "py312",
                     label: "Python 3.12.1",
                     isLocked: !0
                 }];
 
-            function xe(e, t) {
+            function ye(e, t) {
                 var n;
                 const i = (null === (n = e.flux.getStore("UserStore").getState().config) || void 0 === n ? void 0 : n.pythonVersion) || t[0].label;
                 return t.map((e => {
                     const t = e.label.match(/Python (\d+\.\d+)\./),
                         n = i.match(/Python (\d+\.\d+)\./);
                     return t && n && t[1] === n[1] ? Object.assign(Object.assign({}, e), {
                         label: i,
                         isLocked: !1
                     }) : e
                 })).reduce(((e, t, n) => (!t.isLocked && n > 0 ? e.unshift(t) : e.push(t), e)), [])
             }
-            var Ee;
-            class ye extends s().Component {
+            var we;
+            class ke extends o().Component {
                 constructor(e) {
-                    var t, n, i, a, r, l, c, d;
+                    var t, n, a, s, r, l, c, d;
                     super(e), this.resizeEditor = () => {
                         var e, t, n;
                         null === (n = null === (t = null === (e = this.aceRef) || void 0 === e ? void 0 : e.current) || void 0 === t ? void 0 : t.editor) || void 0 === n || n.resize()
                     }, this.handleChangeCode = e => {
                         this.setState({
                             newEnvCode: e
                         }, (() => {
@@ -3199,25 +3558,25 @@
                                     currentEnv: e
                                 })
                             }
                             if (null === (t = null == e ? void 0 : e.tags) || void 0 === t ? void 0 : t.includes("gpu")) {
                                 const e = await this.props.flux.getActions("EnvironmentActions").checkGPU({
                                         delayed: !1
                                     }),
-                                    t = localStorage.getItem(ue);
+                                    t = localStorage.getItem(be);
                                 if (!e && !t) {
                                     const e = await this.showWarnDialog({
                                         withCheckbox: !0,
                                         titleText: "GPU is not configured in your system",
                                         bodyText: "Proceed to add kernel anyway?",
                                         submitButtonText: "Add",
                                         cancelButtonText: "Cancel"
                                     });
                                     if (!e.button.accept) return;
-                                    e.button.accept && e.isChecked && localStorage.setItem(ue, !0)
+                                    e.button.accept && e.isChecked && localStorage.setItem(be, !0)
                                 }
                             }
                         }
                         this.handleToggleActiveEnvironment(e)
                     }, this.handleToggleActiveEnvironment = e => {
                         this.props.flux.getActions("EnvironmentActions").toggleActive(e._id).then((() => this.highlightKernelSelector(e.active))).catch((e => {
                             "string" == typeof e && e.length > 0 ? alert(e) : alert("Sorry, unable to add/remove kernel at this time. Please try again later.")
@@ -3236,21 +3595,21 @@
                         try {
                             return await this.props.flux.getActions("EnvironmentActions").pollStatusLocal()
                         } catch (e) {
                             return console.log(e), this.handleFinishInstallFailure()
                         }
                     }, this.handleInstallProgress = async e => {
                         let t = 0;
-                        Ee = setInterval((() => {
+                        we = setInterval((() => {
                             t++;
                             const e = 100 * ((t / 50) ** 1.5 + .05);
                             this.setState({
                                 progress: this.state.progress <= 100 ? Math.min(e, 100) : 100
                             }, (() => {
-                                this.state.progress >= 90 && (clearInterval(Ee), this.pollStatusLocal().then((e => {
+                                this.state.progress >= 90 && (clearInterval(we), this.pollStatusLocal().then((e => {
                                     if (e) return !0 === e.success ? (this.setState({
                                         progress: 100
                                     }), this.handleFinishInstallSuccess()) : this.handleFinishInstallFailure()
                                 })))
                             }))
                         }), 1e3 * e / 50)
                     }, this.handleInstallProgressStream = async (e, t) => {
@@ -3276,20 +3635,20 @@
                         } catch (t) {
                             alert(`Your environment ${e.displayName} could not be installed at this time.`)
                         }
                     }, this.showWarnDialog = async ({
                         withCheckbox: e,
                         cancelButtonText: t,
                         submitButtonText: n,
-                        bodyText: i,
-                        titleText: a
+                        bodyText: a,
+                        titleText: s
                     }) => {
-                        let s = {
-                            title: a,
-                            body: i,
+                        let o = {
+                            title: s,
+                            body: a,
                             buttons: [{
                                 iconLabel: "",
                                 label: t,
                                 caption: "Cancel",
                                 className: "env_dialog-btn_cancel",
                                 accept: !1,
                                 displayType: "default"
@@ -3298,22 +3657,22 @@
                                 label: n,
                                 caption: "Ok",
                                 className: "env_dialog-btn_confirm",
                                 accept: !0,
                                 displayType: "default"
                             }]
                         };
-                        return e && (s = Object.assign(Object.assign({}, s), {
+                        return e && (o = Object.assign(Object.assign({}, o), {
                             checkbox: {
                                 label: "Don't ask me again",
                                 caption: "Reminder",
                                 className: "gpu_warn_dialog-checkbox",
                                 checked: !1
                             }
-                        })), (0, o.showDialog)(s)
+                        })), (0, i.showDialog)(o)
                     }, this.handleOpenIntelPermissionModal = () => {
                         this.setState({
                             intelPermissionModal: !0
                         })
                     }, this.handleCloseIntelPermissionModal = () => {
                         this.setState({
                             intelPermissionModal: !1
@@ -3322,64 +3681,64 @@
                         try {
                             await this.props.flux.getActions("EnvironmentActions").acceptAgreement() && (await this.props.flux.getActions("UserActions").getUser(), this.handleToggleActiveEnvironment(this.state.currentEnv))
                         } catch (e) {
                             console.log(e)
                         } finally {
                             this.handleCloseIntelPermissionModal()
                         }
-                    }, this.renderIntelTermsAndConditionModal = () => s().createElement(v.Dialog, {
+                    }, this.renderIntelTermsAndConditionModal = () => o().createElement(v.Dialog, {
                         open: this.state.intelPermissionModal,
                         onClose: () => this.handleCloseIntelPermissionModal()
-                    }, s().createElement(v.Stack, {
+                    }, o().createElement(v.Stack, {
                         px: "24px",
                         pt: "16px",
                         gap: 1,
                         sx: {
                             userSelect: "none"
                         }
-                    }, s().createElement(z.ReceiptLongOutlined, {
+                    }, o().createElement(z.ReceiptLongOutlined, {
                         fontSize: "inherit",
                         sx: e => ({
                             width: 48,
                             height: 48,
                             marginInline: "auto",
                             rotate: "25deg",
                             color: e.palette.secondary.light
                         })
-                    }), s().createElement(v.Divider, null, s().createElement(v.Typography, {
+                    }), o().createElement(v.Divider, null, o().createElement(v.Typography, {
                         fontSize: 22,
                         textTransform: "uppercase",
                         fontWeight: 600,
                         sx: e => ({
                             WebkitTextFillColor: "transparent",
                             textFillColor: "transparent",
                             background: `linear-gradient( 45deg, ${e.palette.primary.main}, ${e.palette.secondary.main} )`,
                             WebkitBackgroundClip: "text",
                             backgroundClip: "text"
                         })
-                    }, "End User Agreement Terms")), s().createElement(v.Typography, {
+                    }, "End User Agreement Terms")), o().createElement(v.Typography, {
                         fontSize: 16,
                         textAlign: "center",
                         color: "text.secondary"
-                    }, "qBraid Customer")), s().createElement(v.DialogContent, {
+                    }, "qBraid Customer")), o().createElement(v.DialogContent, {
                         sx: {
                             overflow: "hidden"
                         }
-                    }, s().createElement(ae, null)), s().createElement(v.DialogActions, {
+                    }, o().createElement(oe, null)), o().createElement(v.DialogActions, {
                         sx: {
                             gap: 1
                         }
-                    }, s().createElement(v.Button, {
+                    }, o().createElement(v.Button, {
                         variant: "outlined",
                         size: "small",
                         sx: {
                             borderRadius: "6px"
                         },
                         onClick: () => this.handleCloseIntelPermissionModal()
-                    }, "Decline"), s().createElement(v.Button, {
+                    }, "Decline"), o().createElement(v.Button, {
                         size: "small",
                         variant: "contained",
                         sx: {
                             borderRadius: "6px",
                             background: "rgb(103, 58, 183)"
                         },
                         onClick: this.handleAcceptTermsAndCondition
@@ -3392,15 +3751,15 @@
                             const [n, i] = t[e.slug];
                             return alert("The {} environment is available only from the {} Lab image.".replace("{}", n).replace("{}", i))
                         }
                         if (e.isPreInstalled) return alert("This environment comes pre-installed and is not available for installation via the Environment Manager. To access this environment, launch the appropriate qBraid Lab instance from the Computer Manager. If you believe you are seeing this message in error, please use the Help drop-down to report a bug.");
                         let {
                             user: n
                         } = this.props.flux.getStore("UserStore").getState();
-                        if (!(n && n.permissionsNodes && -1 !== n.permissionsNodes.indexOf(ge) || e.tags.includes("free"))) return this.openNoPermsDialog();
+                        if (!(n && n.permissionsNodes && -1 !== n.permissionsNodes.indexOf(ve) || e.tags.includes("free"))) return this.openNoPermsDialog();
                         this.installEnvironment(e)
                     }, this.installEnvironment = async e => {
                         var t;
                         if (null === (t = null == e ? void 0 : e.tags) || void 0 === t ? void 0 : t.includes("gpu"))
                             if (this.setState({
                                     verifyLoading: {
                                         loading: !0,
@@ -3424,18 +3783,23 @@
                                 titleText: "GPU is not configured in your system",
                                 bodyText: "Do you want to proceed?",
                                 cancelButtonText: "Cancel",
                                 submitButtonText: "Install"
                             })).button.accept) return;
                         try {
                             const t = await this.props.flux.getActions("EnvironmentActions").startInstall(e._id);
-                            t && (this.setState({
-                                progress: 10,
-                                timeToInstall: t
-                            }), this.registerInstalled(e, t))
+                            if (t && (this.setState({
+                                    progress: 10,
+                                    timeToInstall: t
+                                }), this.registerInstalled(e, t)), "requested" === (null == e ? void 0 : e.reviewStatus)) {
+                                let {
+                                    user: t
+                                } = this.props.flux.getStore("UserStore").getState();
+                                "contact@qbraid.com" === t.email && this.props.flux.getActions("EnvironmentActions").updatePublishStatus(e.slug, "pending")
+                            }
                         } catch (t) {
                             return console.log(`Error: ${t}`), alert("Your environment " + e.displayName + " could not be installed at this time.")
                         }
                     }, this.handleFinishInstallSuccess = () => {
                         const e = this.state.installingEnvironment;
                         e && (this.setState({
                             progress: 0,
@@ -3666,25 +4030,25 @@
                             newEnvCode: ""
                         }
                     }), this.cloneEnvironment = e => {
                         var t, n;
                         let {
                             user: i
                         } = this.props.flux.getStore("UserStore").getState();
-                        if (!i || !i.permissionsNodes || -1 === i.permissionsNodes.indexOf("qbraid.environments.clone") || !e.installed && !e.tags.includes("free") && -1 === i.permissionsNodes.indexOf(ge)) return this.openNoPermsDialog();
+                        if (!i || !i.permissionsNodes || -1 === i.permissionsNodes.indexOf("qbraid.environments.clone") || !e.installed && !e.tags.includes("free") && -1 === i.permissionsNodes.indexOf(ve)) return this.openNoPermsDialog();
                         const a = e.displayName.includes("(Copy)") ? e.displayName.substr(0, e.displayName.lastIndexOf(" ")) : e.displayName,
                             s = this.state.environments.filter((t => t.displayName.includes(a) && t.slug !== e.slug)).length;
                         this.setState({
                             returnToMyenv: !this.state.browsing && !0,
                             browsing: !0,
                             newEnvName: `${a} (Copy)${s>0?` (${s})`:""}`,
                             newEnvDescription: e.description,
                             tags: [...e.tags].filter((e => "custom" !== e)),
                             newEnvCode: (null == e ? void 0 : e.packagesInImage) ? [...null == e ? void 0 : e.packagesInImage].join("\n") : "",
-                            img: null !== (n = null === (t = null == e ? void 0 : e.logo) || void 0 === t ? void 0 : t.light) && void 0 !== n ? n : ve,
+                            img: null !== (n = null === (t = null == e ? void 0 : e.logo) || void 0 === t ? void 0 : t.light) && void 0 !== n ? n : fe,
                             filterQuery: "",
                             filteredEnvironments: [],
                             editingNewEnvForm: !0,
                             tagFilter: !1
                         })
                     }, this.closeNewEnvironmentForm = () => {
                         !0 !== this.state.qbUser.isMount ? this.setState({
@@ -3694,15 +4058,15 @@
                         }), this.setState({
                             returnToMyenv: !1,
                             editingNewEnvForm: !1,
                             newEnvDescription: "",
                             newEnvName: "",
                             tags: [],
                             tagsInputText: "",
-                            img: ve,
+                            img: fe,
                             newEnvCode: "",
                             filterQuery: "",
                             filteredEnvironments: [],
                             tagFilter: !1
                         })
                     }, this.resetNewEnvData = () => this.setState({
                         newEnvCode: "",
@@ -3746,15 +4110,15 @@
                         })))];
                         this.setState({
                             tags: t
                         })
                     }, this.handleImageUploadBoxClose = () => {
                         this.setState({
                             imageUploadBox: !1
-                        }), this.state.img !== ve && localStorage.setItem(this.state.newEnvName, this.state.img), this.closeImgUploadError()
+                        }), this.state.img !== fe && localStorage.setItem(this.state.newEnvName, this.state.img), this.closeImgUploadError()
                     }, this.handleImageUploadBoxOpen = () => {
                         this.setState({
                             imageUploadBox: !0
                         })
                     }, this.handleImageUpload = e => {
                         const t = new FileReader,
                             n = e.target.files[0];
@@ -3778,16 +4142,16 @@
                         })
                     }, this.handleUseAsIpykernelLogoChange = () => {
                         this.setState((e => ({
                             imgAsIpykernelLogo: !e.imgAsIpykernelLogo
                         })))
                     }, this.handleResetImg = () => {
                         this.setState({
-                            img: ve,
-                            imgFile: ve,
+                            img: fe,
+                            imgFile: fe,
                             imgAsIpykernelLogo: !1
                         }, (() => {
                             var e;
                             (null === (e = this.imageInputRef) || void 0 === e ? void 0 : e.current) && (this.imageInputRef.current.value = "")
                         }))
                     }, this.compareEnvs = (e, t) => {
                         if (e.pinned || t.pinned) return !e.pinned - !t.pinned;
@@ -3834,96 +4198,96 @@
                         this.setState({
                             packageProgress: 0,
                             packageInstallingEnv: ""
                         })
                     }, this.renderPopupMsg = ({
                         msg: e,
                         type: t
-                    }) => s().createElement(v.Snackbar, {
+                    }) => o().createElement(v.Snackbar, {
                         open: this.state.popupOpen,
                         autoHideDuration: 4e3,
                         onClose: this.handlePopupClose,
                         sx: {
                             position: "absolute",
                             width: "100%",
                             left: "0px !important",
                             bottom: "0px !important"
                         }
-                    }, s().createElement("div", {
+                    }, o().createElement("div", {
                         className: `env-sidebar-msg-popup ${t} slide-in-bottom stay-longer`
-                    }, e)), this.renderImageUploadModal = () => s().createElement(v.Dialog, {
+                    }, e)), this.renderImageUploadModal = () => o().createElement(v.Dialog, {
                         open: this.state.imageUploadBox,
                         onClose: this.handleImageUploadBoxClose,
                         "aria-labelledby": "uploadImg-dialog-title",
                         "aria-describedby": "uploadImg-dialog-description",
                         className: ""
-                    }, s().createElement(v.DialogTitle, {
+                    }, o().createElement(v.DialogTitle, {
                         id: "uploadImg-dialog-title",
                         className: "env-dialog-img-title"
-                    }, "Upload Environment Image"), s().createElement(v.DialogContent, {
+                    }, "Upload Environment Image"), o().createElement(v.DialogContent, {
                         id: "uploadImg-dialog-content",
                         className: "env-dialog-img-content"
-                    }, s().createElement("img", {
+                    }, o().createElement("img", {
                         src: this.state.img,
                         alt: "icon",
                         className: "env-dialog-img"
-                    }), s().createElement(v.DialogContentText, {
+                    }), o().createElement(v.DialogContentText, {
                         id: "uploadImg-dialog-description"
-                    }, "Please upload a square PNG < ", 500, "KB")), this.state.img !== ve && s().createElement(v.DialogActions, {
+                    }, "Please upload a square PNG < ", 500, "KB")), this.state.img !== fe && o().createElement(v.DialogActions, {
                         id: "uploadImg-dialog-options",
                         className: "env-dialog-img-options"
-                    }, s().createElement(v.FormControlLabel, {
-                        control: s().createElement(v.Checkbox, {
+                    }, o().createElement(v.FormControlLabel, {
+                        control: o().createElement(v.Checkbox, {
                             checked: this.state.imgAsIpykernelLogo,
                             onChange: this.handleUseAsIpykernelLogoChange,
                             name: "imgAsIpykernelLogo",
                             color: "primary"
                         }),
                         label: "Override ipykernel logo"
-                    })), s().createElement(v.DialogActions, {
+                    })), o().createElement(v.DialogActions, {
                         id: "uploadImg-dialog-actions"
-                    }, this.state.imgUploadError.open && s().createElement(v.Typography, {
+                    }, this.state.imgUploadError.open && o().createElement(v.Typography, {
                         className: "uploadImg-error-text"
-                    }, this.state.imgUploadError.msg), s().createElement(v.Button, {
-                        onClick: this.state.img === ve ? this.handleImageUploadBoxClose : this.handleResetImg
-                    }, this.state.img === ve ? "Cancel" : "Reset"), s().createElement(v.Button, {
+                    }, this.state.imgUploadError.msg), o().createElement(v.Button, {
+                        onClick: this.state.img === fe ? this.handleImageUploadBoxClose : this.handleResetImg
+                    }, this.state.img === fe ? "Cancel" : "Reset"), o().createElement(v.Button, {
                         component: "label",
                         variant: "contained",
                         sx: {
                             backgroundColor: "#673ab7!important",
                             borderColor: "#673ab7!important"
                         }
-                    }, this.state.img === ve ? "Browse" : "Modify", s().createElement("input", {
+                    }, this.state.img === fe ? "Browse" : "Modify", o().createElement("input", {
                         id: "image-upload",
                         hidden: !0,
                         ref: this.imageInputRef,
                         accept: "image/*",
                         type: "file",
                         onChange: this.handleImageUpload
-                    })), this.state.img !== ve && s().createElement(v.Button, {
+                    })), this.state.img !== fe && o().createElement(v.Button, {
                         variant: "contained",
                         sx: {
                             backgroundColor: "#673ab7!important"
                         },
                         onClick: this.handleImageUploadBoxClose
-                    }, "Save"))), this.renderInstalledEnvironments = () => (this.state.environments.sort(((e, t) => e.pinned || t.pinned ? !e.pinned - !t.pinned : (t.priority || 0) - (e.priority || 0))), this.state.environments.filter((e => e.installed)).length < 1 ? s().createElement(ie, null) : this.state.environments.filter((e => e.installed)).map((e => {
+                    }, "Save"))), this.renderInstalledEnvironments = () => (this.state.environments.sort(((e, t) => e.pinned || t.pinned ? !e.pinned - !t.pinned : (t.priority || 0) - (e.priority || 0))), this.state.environments.filter((e => e.installed)).length < 1 ? o().createElement(se, null) : this.state.environments.filter((e => e.installed)).map((e => {
                         let t = e.active,
                             n = this.state.installingEnvironment && (this.state.installingEnvironment._id === e._id || this.state.newEnvSlug === (null == e ? void 0 : e.slug));
-                        return s().createElement(N, {
+                        return o().createElement(T, {
                             qbUser: this.state.qbUser,
                             key: e._id,
                             expandedEnvs: this.state.expandedEnvs,
                             onTogglePinned: this.onTogglePinned,
                             onToggleExpand: this.onToggleExpand,
                             environment: e,
                             isActive: t,
                             isNewEnv: e._id === this.state.newCustomEnvId,
                             isInstalling: n,
                             isInstalled: !n,
-                            activateButton: s().createElement("p", {
+                            activateButton: o().createElement("p", {
                                 className: "env-action",
                                 style: {
                                     width: "100%",
                                     marginRight: 10,
                                     background: n ? `linear-gradient(to right ,#673AB7 ${this.state.progress}% , #9070C8 0%)` : "#673AB7",
                                     cursor: n || "qbraid_000000" === e.slug ? "not-allowed" : "pointer"
                                 },
@@ -3965,19 +4329,21 @@
                             }))
                         })).catch((e => {
                             var t, n;
                             this.handleOpenPopup(null === (n = null === (t = null == e ? void 0 : e.response) || void 0 === t ? void 0 : t.body) || void 0 === n ? void 0 : n.message, "error"), this.setState({
                                 accessCodeLoading: !1
                             })
                         })))
+                    }, this.handleOpenDocs = () => {
+                        this.props.app && this.props.app.commands.execute("docs:qbraid-env-manager")
                     }, this.renderUninstalledEnvironments = () => {
                         let e = this.state.filterQuery || this.state.tagFilter ? this.state.filteredEnvironments : this.state.environments;
-                        return e.sort(((e, t) => this.compareEnvs(e, t))), [s().createElement(v.Box, {
+                        return e.sort(((e, t) => this.compareEnvs(e, t))), [o().createElement(v.Box, {
                             m: "10px"
-                        }, s().createElement(v.Paper, {
+                        }, o().createElement(v.Paper, {
                             elevation: 0,
                             sx: e => ({
                                 display: "flex",
                                 flexDirection: "row",
                                 flex: 1,
                                 borderWidth: "1px",
                                 borderStyle: "solid",
@@ -3987,15 +4353,15 @@
                                     borderColor: `${e.palette.action}!important`
                                 },
                                 "&:focus-within, &:focus-visible": {
                                     borderColor: e.palette.primary.main,
                                     outline: `1px solid ${e.palette.primary.main}`
                                 }
                             })
-                        }, s().createElement(v.InputBase, {
+                        }, o().createElement(v.InputBase, {
                             sx: {
                                 ml: 1,
                                 flex: 1,
                                 fontSize: 18,
                                 fontWeight: 400
                             },
                             inputProps: {
@@ -4004,54 +4370,54 @@
                                     fontSize: "14px"
                                 }
                             },
                             value: this.state.accessCodeInput,
                             placeholder: "Discover via access code...",
                             onChange: this.handleAccessCodeInputChange,
                             type: this.state.accessCodeInputVisible ? "text" : "password"
-                        }), s().createElement(v.IconButton, {
+                        }), o().createElement(v.IconButton, {
                             size: "small",
                             onClick: this.handleAccessCodeVisibility
-                        }, this.state.accessCodeInputVisible ? s().createElement(z.Visibility, {
+                        }, this.state.accessCodeInputVisible ? o().createElement(z.Visibility, {
                             fontSize: "inherit"
-                        }) : s().createElement(z.VisibilityOff, {
+                        }) : o().createElement(z.VisibilityOff, {
                             fontSize: "inherit"
-                        })), s().createElement(v.Button, {
+                        })), o().createElement(v.Button, {
                             color: "secondary",
                             variant: "contained",
                             size: "small",
                             sx: {
                                 fontSize: 14,
                                 textTransform: "inherit",
                                 ml: 1,
                                 cursor: this.state.accessCodeLoading ? "wait" : "pointer"
                             },
                             onClick: this.handleDiscoverEnvWithAccessCode,
                             disabled: this.state.accessCodeLoading
-                        }, s().createElement(z.AddCircleOutline, null)))), s().createElement("div", {
+                        }, o().createElement(z.AddCircleOutline, null)))), o().createElement("div", {
                             className: "environments-sidebar-create-env",
                             onClick: this.handleNewEnvironmentClick
-                        }, s().createElement("p", {
+                        }, o().createElement("p", {
                             style: {
                                 marginRight: 8,
                                 fontSize: 24,
                                 paddingBottom: 4
                             }
-                        }, "+"), s().createElement("p", null, "Create Environment"))].concat(e.filter((e => !e.installed)).map((e => s().createElement(N, {
+                        }, "+"), o().createElement("p", null, "Create Environment"))].concat(e.filter((e => !e.installed)).map((e => o().createElement(T, {
                             qbUser: this.state.qbUser,
                             key: e._id,
                             expandedEnvs: this.state.expandedEnvs,
                             onToggleExpand: this.onToggleExpand,
                             onTogglePinned: this.onTogglePinned,
                             environment: e,
                             isInstalling: !1,
                             isNewEnv: !1,
                             isInstalled: !1,
                             verifyLoading: this.state.verifyLoading,
-                            activateButton: s().createElement("p", {
+                            activateButton: o().createElement("p", {
                                 className: "env-action",
                                 style: {
                                     width: "100%",
                                     marginRight: 10,
                                     backgroundColor: this.state.installingEnvironment || !e.isAvailable ? "#a696c3" : "#673ab7",
                                     cursor: this.state.installingEnvironment || !e.isAvailable ? "not-allowed" : "pointer"
                                 },
@@ -4061,97 +4427,97 @@
                             }, e.isAvailable ? "Install" : "Unavailable"),
                             edit: () => this.openEnvironmentEditor(e),
                             flux: this.props.flux,
                             packageInstallingEnv: this.state.packageInstallingEnv,
                             packageProgress: this.state.packageProgress,
                             cloneEnvironment: this.cloneEnvironment,
                             isDarkTheme: this.state.isDarkTheme
-                        })))).concat([e.length <= 0 && s().createElement("div", {
+                        })))).concat([e.length <= 0 && o().createElement("div", {
                             style: {
                                 padding: "1em"
                             }
-                        }, s().createElement("p", {
+                        }, o().createElement("p", {
                             style: {
                                 fontSize: 18,
                                 color: "var(--jp-ui-font-color2)",
                                 textAlign: "center"
                             }
                         }, "No pre-configured environments found. Create a custom environment to get started."))])
-                    }, this.renderUpgradeDialogue = () => s().createElement(v.Dialog, {
+                    }, this.renderUpgradeDialogue = () => o().createElement(v.Dialog, {
                         open: this.state.showNoPermsDialog,
                         onClose: this.closeNoPermsDialog,
                         "aria-labelledby": "noPerms-dialog-title",
                         "aria-describedby": "noPerms-dialog-description",
                         className: ""
-                    }, s().createElement(v.DialogTitle, {
+                    }, o().createElement(v.DialogTitle, {
                         id: "noPerms-dialog-title"
-                    }, "Upgrade to continue"), s().createElement(v.DialogContent, {
+                    }, "Upgrade to continue"), o().createElement(v.DialogContent, {
                         id: "noPerms-dialog-content"
-                    }, s().createElement(v.DialogContentText, {
+                    }, o().createElement(v.DialogContentText, {
                         id: "noPerms-dialog-description"
-                    }, "Upgrade your account to unlock premium environment manager features.")), s().createElement(v.DialogActions, {
+                    }, "Upgrade your account to unlock premium environment manager features.")), o().createElement(v.DialogActions, {
                         id: "noPerms-dialog-actions"
-                    }, s().createElement(v.Button, {
+                    }, o().createElement(v.Button, {
                         onClick: this.closeNoPermsDialog,
                         variant: "slide",
                         type: "decline",
                         sx: {
                             minWidth: "120px"
                         }
-                    }, "Maybe later"), s().createElement(v.Button, {
+                    }, "Maybe later"), o().createElement(v.Button, {
                         variant: "slide",
                         onClick: () => {
                             window.open(`${y}/billing`, "_blank")
                         },
                         sx: {
                             minWidth: "120px"
                         }
-                    }, "Upgrade"))), this.aceContainerRef = s().createRef(), this.aceRef = s().createRef(), this.imageInputRef = s().createRef(), this.state = {
+                    }, "Upgrade"))), this.aceContainerRef = o().createRef(), this.aceRef = o().createRef(), this.imageInputRef = o().createRef(), this.state = {
                         progress: 0,
                         tags: [],
                         tagsInputText: "",
                         togglesCount: 0,
                         isClickedRefresh: !1,
                         installingEnvironment: e.flux.getStore("EnvironmentStore").getState().installingEnvironment || null,
                         environments: e.flux.getStore("EnvironmentStore").getState().environments || [],
                         qbUser: e.flux.getStore("UserStore").getState() || {},
-                        pythonVersions: xe(e, fe),
+                        pythonVersions: ye(e, Ee),
                         browsing: !1,
                         filterQuery: "",
                         filteredEnvironments: [],
                         editing: !1,
                         editingNewEnvForm: !1,
                         newEnvCode: "",
                         newEnvName: "",
                         newEnvDescription: "",
                         newEnvSlug: "",
                         newEnvKernelName: "",
                         newEnvShellPrompt: "",
-                        newEnvPythonVersion: (null === (t = e.flux.getStore("UserStore").getState().config) || void 0 === t ? void 0 : t.pythonVersion) || fe[0].label,
+                        newEnvPythonVersion: (null === (t = e.flux.getStore("UserStore").getState().config) || void 0 === t ? void 0 : t.pythonVersion) || Ee[0].label,
                         newEnvExpandAdvanced: !1,
                         newEnvFormHelperTexts: {
                             newEnvName: "",
                             newEnvCode: ""
                         },
                         selectedEnvironment: null,
                         showNoPermsDialog: !1,
                         imageUploadBox: !1,
-                        img: ve,
+                        img: fe,
                         imgFile: null,
                         imgUploadError: {
                             open: !1,
                             msg: ""
                         },
                         imgAsIpykernelLogo: !1,
                         popupOpen: !1,
                         popupMsg: {
                             msg: "",
                             type: ""
                         },
-                        currentTheme: (null === (a = null === (i = null === (n = null === document || void 0 === document ? void 0 : document.getElementsByTagName("BODY")[0]) || void 0 === n ? void 0 : n.getAttribute("data-jp-theme-name")) || void 0 === i ? void 0 : i.toLowerCase()) || void 0 === a ? void 0 : a.includes("dark")) ? ee : X,
+                        currentTheme: (null === (s = null === (a = null === (n = null === document || void 0 === document ? void 0 : document.getElementsByTagName("BODY")[0]) || void 0 === n ? void 0 : n.getAttribute("data-jp-theme-name")) || void 0 === a ? void 0 : a.toLowerCase()) || void 0 === s ? void 0 : s.includes("dark")) ? ne : te,
                         isDarkTheme: !!(null === (c = null === (l = null === (r = null === document || void 0 === document ? void 0 : document.getElementsByTagName("BODY")[0]) || void 0 === r ? void 0 : r.getAttribute("data-jp-theme-name")) || void 0 === l ? void 0 : l.toLowerCase()) || void 0 === c ? void 0 : c.includes("dark")),
                         newCustomEnvId: null,
                         refreshEnvData: !1,
                         makeNewEnv: !1,
                         timeToInstall: 0,
                         showFilter: !1,
                         sortBy: "highest_to_lowest_priority",
@@ -4187,18 +4553,18 @@
                 }
                 componentDidMount() {
                     var e, t;
                     this.props.flux.getStore("EnvironmentStore").listen(this.handleUpdateEnvironments);
                     let n = document.getElementsByTagName("BODY")[0];
                     new MutationObserver((() => {
                         n.getAttribute("data-jp-theme-name").toLowerCase().includes("dark") ? this.setState({
-                            currentTheme: ee,
+                            currentTheme: ne,
                             isDarkTheme: !0
                         }) : this.setState({
-                            currentTheme: X,
+                            currentTheme: te,
                             isDarkTheme: !1
                         })
                     })).observe(n, {
                         attributesFilter: ["data-jp-theme-name"],
                         attributeOldValue: !0
                     }), this.setState({
                         containerWidth: null === (t = null === (e = this.aceContainerRef) || void 0 === e ? void 0 : e.current) || void 0 === t ? void 0 : t.offsetWidth
@@ -4210,86 +4576,101 @@
                         containerWidth: null === (o = null === (s = this.aceContainerRef) || void 0 === s ? void 0 : s.current) || void 0 === o ? void 0 : o.offsetWidth
                     }))
                 }
                 componentWillUnmount() {
                     this.props.flux.getStore("EnvironmentStore").unlisten(this.handleUpdateEnvironments)
                 }
                 render() {
-                    return s().createElement(v.ThemeProvider, {
+                    return o().createElement(v.ThemeProvider, {
                         theme: this.state.currentTheme
-                    }, s().createElement("div", {
+                    }, o().createElement("div", {
                         className: "environments-sidebar"
-                    }, s().createElement("div", {
+                    }, o().createElement("div", {
                         className: "environments-sidebar-header"
-                    }, s().createElement("span", null, this.state.editingNewEnvForm ? s().createElement("div", {
+                    }, o().createElement("span", null, this.state.editingNewEnvForm ? o().createElement("div", {
                         className: "environments-sidebar-back-btn",
                         style: this.state.browsing ? null : {
                             opacity: 0,
                             cursor: "default"
                         },
                         onClick: this.closeNewEnvironmentForm
-                    }, s().createElement("span", {
+                    }, o().createElement("span", {
                         className: "environments-sidebar-left-arrow"
-                    }, "‹ "), "Create Environment") : this.state.browsing ? s().createElement("div", {
+                    }, "‹ "), "Create Environment") : this.state.browsing ? o().createElement("div", {
                         className: "environments-sidebar-back-btn",
                         style: this.state.browsing ? null : {
                             opacity: 0,
                             cursor: "default"
                         },
                         onClick: this.closeEnvironmentBrowser
-                    }, s().createElement("span", {
+                    }, o().createElement("span", {
                         className: "environments-sidebar-left-arrow"
-                    }, "‹ "), "Browse Environments") : s().createElement("div", {
-                        style: {
-                            lineHeight: "20px",
-                            display: "inline-flex"
+                    }, "‹ "), "Browse Environments") : o().createElement(v.Box, {
+                        display: "inline-flex",
+                        alignItems: "center",
+                        gap: .5,
+                        sx: {
+                            lineHeight: "20px"
                         }
-                    }, "My Environments", s().createElement("div", {
+                    }, "Environments", o().createElement("div", {
                         style: {
                             transition: "transform 1s",
                             transform: `rotateZ(${180*this.state.togglesCount+"deg"})`
                         },
                         onClick: () => this.handleRefreshEnvironments({
                             clickedRefresh: !0
                         }),
                         className: "div-refresh-btn"
-                    }, s().createElement(G, null)))), s().createElement("span", {
+                    }, o().createElement(V, null)), o().createElement(v.Tooltip, {
+                        title: "Read Environment Manager docs",
+                        arrow: !0
+                    }, o().createElement(v.IconButton, {
+                        size: "small",
+                        color: "primary",
+                        sx: {
+                            ml: .5
+                        },
+                        onClick: this.handleOpenDocs
+                    }, o().createElement(z.ReceiptLongTwoTone, {
+                        color: "inherit",
+                        fontSize: "inherit"
+                    }))))), o().createElement("span", {
                         className: "environments-sidebar-add-btn",
                         style: this.state.browsing ? {
                             opacity: 0,
                             cursor: "default"
                         } : this.state.noUser ? {
                             color: "darkgray !important",
                             cursor: "not-allowed"
                         } : null,
                         onClick: this.state.browsing || this.state.noUser ? null : () => this.handleAddButton()
-                    }, this.state.qbUser.isMount ? "+ Add" : "+ Create")), s().createElement("div", {
+                    }, this.state.qbUser.isMount ? "+ Add" : "+ Create")), o().createElement("div", {
                         className: "environments-sidebar-spacer"
-                    }), this.state.isClickedRefresh ? s().createElement(ie, null) : this.state.noUser ? s().createElement(me, null) : s().createElement("div", {
+                    }), this.state.isClickedRefresh ? o().createElement(se, null) : this.state.noUser ? o().createElement(ue, null) : o().createElement("div", {
                         className: "environments-sidebar-list-pane",
                         style: this.state.browsing ? {
                             overflow: "hidden",
                             right: "100%"
                         } : null
-                    }, s().createElement("div", {
+                    }, o().createElement("div", {
                         className: "environments-sidebar-environment-list"
-                    }, this.renderInstalledEnvironments())), s().createElement("div", {
+                    }, this.renderInstalledEnvironments())), o().createElement("div", {
                         className: "environments-sidebar-search-pane",
                         style: {
                             width: this.state.browsing && !this.state.editingNewEnvForm ? "100%" : "0%"
                         }
-                    }, s().createElement("span", {
+                    }, o().createElement("span", {
                         className: "envoronments-sidebar-search-wrapper"
-                    }, s().createElement(v.Grid, {
+                    }, o().createElement(v.Grid, {
                         container: !0
-                    }, s().createElement(v.Grid, {
+                    }, o().createElement(v.Grid, {
                         item: !0,
                         xs: 12,
                         padding: 1
-                    }, s().createElement(v.TextField, {
+                    }, o().createElement(v.TextField, {
                         placeholder: "Search Environments",
                         id: "filled-search",
                         size: "small",
                         sx: {
                             "& .MuiOutlinedInput-root": {
                                 "&.Mui-focused fieldset": {
                                     borderColor: "#d30982"
@@ -4301,68 +4682,68 @@
                         inputProps: {
                             style: {
                                 height: "19px",
                                 fontSize: "14px"
                             }
                         },
                         InputProps: {
-                            startAdornment: s().createElement(v.InputAdornment, {
+                            startAdornment: o().createElement(v.InputAdornment, {
                                 position: "start"
-                            }, s().createElement(v.IconButton, {
+                            }, o().createElement(v.IconButton, {
                                 "aria-label": "search icon",
                                 edge: "start"
-                            }, s().createElement($.Z, null))),
-                            endAdornment: s().createElement(v.InputAdornment, {
+                            }, o().createElement(H.Z, null))),
+                            endAdornment: o().createElement(v.InputAdornment, {
                                 position: "end"
-                            }, this.state.filterQuery.length > 1 && s().createElement(v.Tooltip, {
+                            }, this.state.filterQuery.length > 1 && o().createElement(v.Tooltip, {
                                 title: "Clear Search",
                                 arrow: !0
-                            }, s().createElement(v.IconButton, {
+                            }, o().createElement(v.IconButton, {
                                 "aria-label": "clear icon",
                                 edge: "end",
                                 onClick: () => this.setState({
                                     filterQuery: "",
                                     filteredEnvironments: [],
                                     tagFilter: !1,
                                     tags: []
                                 })
-                            }, s().createElement(V.Z, {
+                            }, o().createElement(J.Z, {
                                 sx: {
                                     fontSize: "1rem"
                                 }
-                            }))), s().createElement(v.Tooltip, {
+                            }))), o().createElement(v.Tooltip, {
                                 title: "Filters",
                                 arrow: !0
-                            }, s().createElement(v.IconButton, {
+                            }, o().createElement(v.IconButton, {
                                 "aria-label": "filter icon",
                                 edge: "end",
                                 onClick: () => this.setState((e => ({
                                     showFilter: !e.showFilter
                                 })))
-                            }, s().createElement(z.FilterList, null))))
+                            }, o().createElement(z.FilterList, null))))
                         },
                         variant: "outlined",
                         fullWidth: !0,
                         onChange: this.handleChangeFilterQuery,
                         value: this.state.filterQuery
-                    })), this.state.showFilter && s().createElement(v.Grid, {
+                    })), this.state.showFilter && o().createElement(v.Grid, {
                         item: !0,
                         xs: 12,
                         padding: 1
-                    }, s().createElement(v.Grid, {
+                    }, o().createElement(v.Grid, {
                         item: !0,
                         xs: 12,
                         sx: {
                             backgroundColor: "var(--jp-layout-color1)",
                             color: "var(--jp-ui-font-color1)"
                         },
                         paddingBottom: 0
-                    }, s().createElement("form", {
+                    }, o().createElement("form", {
                         onSubmit: this.handleAddChips
-                    }, s().createElement(v.TextField, {
+                    }, o().createElement(v.TextField, {
                         fullWidth: !0,
                         size: "small",
                         label: "Tagged with",
                         variant: "outlined",
                         placeholder: "Filter environments by tag",
                         InputProps: {
                             sx: {
@@ -4396,33 +4777,33 @@
                             this.setState({
                                 tagsInputText: e.target.value
                             })
                         },
                         onKeyDown: e => {
                             "Space" === e.code && this.handleAddChips(e)
                         }
-                    }))), this.state.tags.length > 0 && s().createElement(v.Grid, {
+                    }))), this.state.tags.length > 0 && o().createElement(v.Grid, {
                         item: !0,
                         xs: 12,
                         padding: 1
-                    }, this.state.tags.map((e => s().createElement(v.Chip, {
+                    }, this.state.tags.map((e => o().createElement(v.Chip, {
                         size: "small",
                         sx: {
                             p: 1,
                             m: .3,
                             textTransform: "lowercase"
                         },
                         key: e,
                         label: e,
                         onDelete: this.handleDeleteChips(e)
-                    })))), s().createElement(v.Grid, {
+                    })))), o().createElement(v.Grid, {
                         item: !0,
                         xs: 12,
                         paddingTop: 1
-                    }, s().createElement(v.TextField, {
+                    }, o().createElement(v.TextField, {
                         id: "outlined-select-currency",
                         select: !0,
                         fullWidth: !0,
                         size: "small",
                         label: "Sorted by",
                         value: this.state.sortBy,
                         sx: {
@@ -4449,70 +4830,70 @@
                         onChange: e => {
                             this.setState({
                                 sortBy: e.target.value
                             }, (() => {
                                 this.handleSorting()
                             }))
                         }
-                    }, be.map((e => s().createElement(v.MenuItem, {
+                    }, xe.map((e => o().createElement(v.MenuItem, {
                         key: e.value,
                         value: e.value,
                         sx: {
                             backgroundColor: "var(--jp-layout-color1)",
                             color: "var(--jp-ui-font-color1)",
                             fontSize: "14px !important",
                             "&.Mui-selected": {
                                 backgroundColor: "rgba(211, 9, 130, 0.16)"
                             }
                         }
-                    }, e.label)))))))), s().createElement("div", {
+                    }, e.label)))))))), o().createElement("div", {
                         className: "environments-sidebar-spacer"
-                    }), s().createElement("div", {
+                    }), o().createElement("div", {
                         className: "environments-sidebar-environment-list"
-                    }, this.renderUninstalledEnvironments())), this.state.editing && s().createElement("div", {
+                    }, this.renderUninstalledEnvironments())), this.state.editing && o().createElement("div", {
                         className: "overlay-background"
-                    }, s().createElement(R, {
+                    }, o().createElement(G, {
                         qbUser: this.state.qbUser,
                         onToggleExpand: this.onToggleExpand,
                         env: this.state.selectedEnvironment,
                         installing: this.state.installingEnvironment && (this.state.installingEnvironment._id == this.state.selectedEnvironment._id || this.state.newEnvSlug == this.state.selectedEnvironment.slug),
                         onSave: this.handleSaveEnvironment,
                         onClose: this.closeEnvironmentEditor,
                         flux: this.props.flux,
                         setPackageInstallingEnv: this.setPackageInstallingEnv,
                         finishPackageInstalling: this.finishPackageInstalling,
                         updateReadUserAccessData: this.updateReadUserAccessData,
                         packageInstallingEnv: this.state.packageInstallingEnv,
                         packageProgress: this.state.packageProgress,
                         packageLoading: this.state.packageLoading
-                    })), this.state.editingNewEnvForm && s().createElement("div", {
+                    })), this.state.editingNewEnvForm && o().createElement("div", {
                         className: "environments-sidebar-search-pane",
                         style: {
                             width: this.state.editingNewEnvForm ? "100%" : "0%"
                         }
-                    }, s().createElement("div", {
+                    }, o().createElement("div", {
                         className: "environments-sidebar-environment-list"
-                    }, s().createElement("div", {
+                    }, o().createElement("div", {
                         className: "environment-editor"
-                    }, s().createElement(v.Grid, {
+                    }, o().createElement(v.Grid, {
                         container: !0,
                         sx: {
                             padding: "5px 10px",
                             gap: "1em"
                         }
-                    }, s().createElement(v.Grid, {
+                    }, o().createElement(v.Grid, {
                         item: !0,
                         xs: 12
-                    }, s().createElement(v.Typography, {
+                    }, o().createElement(v.Typography, {
                         variant: "subtitle2",
                         fontSize: 12,
                         fontWeight: 400,
                         color: "var(--jp-layout-color4)",
                         gutterBottom: !0
-                    }, "Name *"), s().createElement(v.TextField, {
+                    }, "Name *"), o().createElement(v.TextField, {
                         fullWidth: !0,
                         placeholder: "My Custom Environment",
                         value: this.state.newEnvName,
                         onChange: e => {
                             this.setState(Object.assign(Object.assign({}, this.state), {
                                 newEnvName: e.target.value
                             }), (() => {
@@ -4542,131 +4923,131 @@
                                 textTransform: "lowercase"
                             }
                         },
                         inputProps: {
                             maxLength: 50
                         },
                         autoFocus: !0
-                    }), s().createElement("div", {
+                    }), o().createElement("div", {
                         className: "text-area-warning"
-                    }, s().createElement("p", {
+                    }, o().createElement("p", {
                         className: "environment-editor-section-label text-area-warning-text"
-                    }, this.state.newEnvName.length >= 50 && "Max length = 50"), s().createElement("p", {
+                    }, this.state.newEnvName.length >= 50 && "Max length = 50"), o().createElement("p", {
                         className: `environment-editor-section-label text-area-warning-text ${this.state.newEnvName.length>=50&&"text-area-error-text"}`
-                    }, 50 - this.state.newEnvName.length)))), s().createElement("div", {
+                    }, 50 - this.state.newEnvName.length)))), o().createElement("div", {
                         className: "environment-editor-section-label"
-                    }, "Description", " ", s().createElement("span", {
+                    }, "Description", " ", o().createElement("span", {
                         style: {
                             color: "var(--jp-layout-color4)"
                         }
-                    }, "(optional)")), s().createElement("textarea", {
+                    }, "(optional)")), o().createElement("textarea", {
                         className: `environment-editor-input ${this.state.newEnvDescription.length>=300&&"text-area-error-input"}`,
                         placeholder: "My custom environment description",
                         spellCheck: "false",
                         rows: 4,
                         maxLength: 300,
                         value: this.state.newEnvDescription,
                         onChange: e => {
                             this.setState(Object.assign(Object.assign({}, this.state), {
                                 newEnvDescription: e.target.value
                             }))
                         }
-                    }), s().createElement("div", {
+                    }), o().createElement("div", {
                         className: "text-area-warning"
-                    }, s().createElement("p", {
+                    }, o().createElement("p", {
                         className: "environment-editor-section-label text-area-warning-text"
-                    }, this.state.newEnvDescription.length >= 300 && "Max length = 300"), s().createElement("p", {
+                    }, this.state.newEnvDescription.length >= 300 && "Max length = 300"), o().createElement("p", {
                         className: `environment-editor-section-label text-area-warning-text ${this.state.newEnvDescription.length>=300&&"text-area-error-text"}`
-                    }, 300 - this.state.newEnvDescription.length)), s().createElement("p", {
+                    }, 300 - this.state.newEnvDescription.length)), o().createElement("p", {
                         className: "environment-editor-section-label"
-                    }, "Tags", " ", s().createElement("span", {
+                    }, "Tags", " ", o().createElement("span", {
                         style: {
                             color: "var(--jp-layout-color4)"
                         }
-                    }, "(optional)")), s().createElement("form", {
+                    }, "(optional)")), o().createElement("form", {
                         onSubmit: this.handleAddChips,
                         style: {
                             display: "grid"
                         }
-                    }, s().createElement("input", {
+                    }, o().createElement("input", {
                         className: "environment-editor-input all_lowercase",
                         placeholder: "Enter tags (e.g. qiskit, braket)",
                         type: "text",
                         spellCheck: "false",
                         value: this.state.tagsInputText,
                         onChange: this.handleChangeTags,
                         onKeyDown: e => {
                             "Space" === e.code && this.handleAddChips(e)
                         }
-                    })), s().createElement(v.Grid, {
+                    })), o().createElement(v.Grid, {
                         container: !0,
                         sx: {
                             padding: "0px 8px"
                         }
-                    }, s().createElement(v.Grid, {
+                    }, o().createElement(v.Grid, {
                         item: !0,
                         xs: 12
-                    }, this.state.tags.map(((e, t) => s().createElement(v.Chip, {
+                    }, this.state.tags.map(((e, t) => o().createElement(v.Chip, {
                         sx: {
                             p: 1,
                             m: .3,
                             textTransform: "lowercase"
                         },
                         size: "small",
                         key: t,
                         label: e,
                         onDelete: !this.state.pythonVersions.map((e => e.value)).includes(e) && this.handleDeleteChips(e)
-                    }))))), s().createElement("p", {
+                    }))))), o().createElement("p", {
                         className: "environment-editor-section-label"
-                    }, "Upload icon", " ", s().createElement("span", {
+                    }, "Upload icon", " ", o().createElement("span", {
                         style: {
                             color: "var(--jp-layout-color4)"
                         }
-                    }, "(optional)")), s().createElement(v.Stack, {
+                    }, "(optional)")), o().createElement(v.Stack, {
                         flexDirection: "row",
                         gap: 1,
                         padding: 1.25,
                         alignItems: "center"
-                    }, s().createElement(v.Avatar, {
+                    }, o().createElement(v.Avatar, {
                         alt: "",
                         src: this.state.img,
                         sx: {
                             ".MuiAvatar-img": {
                                 width: "80%",
                                 height: "80%"
                             }
                         }
-                    }), s().createElement("button", {
+                    }), o().createElement("button", {
                         className: "envSidebar-custom-button envSidebar-flex-btn envSidebar-btn-upload " + (this.state.newEnvName.length < 1 ? "envSidebar-btn-disabled" : ""),
                         onClick: this.handleImageUploadBoxOpen,
                         disabled: this.state.newEnvName.length < 1
-                    }, "Upload Icon", s().createElement(z.FileUpload, {
+                    }, "Upload Icon", o().createElement(z.FileUpload, {
                         fontSize: "16px"
-                    })), this.renderImageUploadModal()), s().createElement("p", {
+                    })), this.renderImageUploadModal()), o().createElement("p", {
                         className: "environment-editor-section-label"
-                    }, "Python Packages", " ", s().createElement("span", {
+                    }, "Python Packages", " ", o().createElement("span", {
                         style: {
                             color: "var(--jp-layout-color4)"
                         }
-                    }, "(optional)")), s().createElement("p", {
+                    }, "(optional)")), o().createElement("p", {
                         style: {
                             color: "var(--jp-error-color1)",
                             fontSize: "0.7em",
                             marginTop: "5px",
                             marginLeft: "10px"
                         }
-                    }, "Warning: Environment creation will fail in the case of dependency conflicts or installation errors."), s().createElement("div", {
+                    }, "Warning: Environment creation will fail in the case of dependency conflicts or installation errors."), o().createElement("div", {
                         ref: this.aceContainerRef,
                         className: `environment-editor-ace-wrapper ${this.state.newEnvFormHelperTexts.newEnvCode.length&&"environment-editor-ace-wrapper-error"}`
-                    }, s().createElement(K(), {
+                    }, o().createElement(Z(), {
                         ref: this.aceRef,
                         onChange: this.handleChangeCode,
                         placeholder: "# requirements.txt",
                         mode: "python",
-                        theme: this.state.currentTheme === X ? "github" : "monokai",
+                        theme: this.state.currentTheme === te ? "github" : "monokai",
                         name: "newEnvCode",
                         style: {
                             position: "relative",
                             flex: 1,
                             paddingBottom: 60,
                             margin: 0,
                             maxHeight: "unset",
@@ -4680,38 +5061,38 @@
                         highlightActiveLine: !0,
                         value: this.state.newEnvCode,
                         setOptions: {
                             showLineNumbers: !0,
                             tabSize: 2,
                             showPrintMargin: !1
                         }
-                    })), s().createElement("p", {
+                    })), o().createElement("p", {
                         className: "environment-editor-code-error"
-                    }, this.state.newEnvFormHelperTexts.newEnvCode), s().createElement(de, {
+                    }, this.state.newEnvFormHelperTexts.newEnvCode), o().createElement(he, {
                         expanded: this.state.newEnvExpandAdvanced,
                         onChange: () => this.setState({
                             newEnvExpandAdvanced: !this.state.newEnvExpandAdvanced
                         })
-                    }, s().createElement(pe, null, s().createElement(v.Typography, {
+                    }, o().createElement(me, null, o().createElement(v.Typography, {
                         color: "var(--jp-layout-color4)"
-                    }, "Advanced customizations")), s().createElement(he, null, s().createElement(v.Grid, {
+                    }, "Advanced customizations")), o().createElement(ge, null, o().createElement(v.Grid, {
                         container: !0,
                         sx: {
                             gap: "1em"
                         }
-                    }, s().createElement(v.Grid, {
+                    }, o().createElement(v.Grid, {
                         item: !0,
                         xs: 12
-                    }, s().createElement(v.Typography, {
+                    }, o().createElement(v.Typography, {
                         variant: "subtitle2",
                         fontSize: 12,
                         fontWeight: 400,
                         color: "var(--jp-layout-color4)",
                         gutterBottom: !0
-                    }, "Kernel Name (optional)"), s().createElement(v.TextField, {
+                    }, "Kernel Name (optional)"), o().createElement(v.TextField, {
                         fullWidth: !0,
                         placeholder: "Python 3 [MyEnv]",
                         value: this.state.newEnvKernelName,
                         onChange: e => {
                             this.setState(Object.assign(Object.assign({}, this.state), {
                                 newEnvKernelName: e.target.value
                             }))
@@ -4733,30 +5114,30 @@
                                 height: "28px",
                                 textTransform: "lowercase"
                             }
                         },
                         inputProps: {
                             maxLength: 30
                         }
-                    }), s().createElement("div", {
+                    }), o().createElement("div", {
                         className: "text-area-warning"
-                    }, s().createElement("p", {
+                    }, o().createElement("p", {
                         className: "environment-editor-section-label text-area-warning-text"
-                    }, this.state.newEnvKernelName.length >= 30 && "Max length = 30"), s().createElement("p", {
+                    }, this.state.newEnvKernelName.length >= 30 && "Max length = 30"), o().createElement("p", {
                         className: `environment-editor-section-label text-area-warning-text ${this.state.newEnvKernelName.length>=30&&"text-area-error-text"}`
-                    }, 30 - this.state.newEnvKernelName.length))), s().createElement(v.Grid, {
+                    }, 30 - this.state.newEnvKernelName.length))), o().createElement(v.Grid, {
                         item: !0,
                         xs: 12
-                    }, s().createElement(v.Typography, {
+                    }, o().createElement(v.Typography, {
                         variant: "subtitle2",
                         fontSize: 12,
                         fontWeight: 400,
                         color: "var(--jp-layout-color4)",
                         gutterBottom: !0
-                    }, "Shell Prompt (PS1) (optional)"), s().createElement(v.TextField, {
+                    }, "Shell Prompt (PS1) (optional)"), o().createElement(v.TextField, {
                         fullWidth: !0,
                         placeholder: "e.g 'myenv' ➞ (myenv) $... when active",
                         value: this.state.newEnvShellPrompt,
                         onChange: e => {
                             this.setState(Object.assign(Object.assign({}, this.state), {
                                 newEnvShellPrompt: e.target.value
                             }))
@@ -4778,26 +5159,26 @@
                                 height: "28px",
                                 textTransform: "lowercase"
                             }
                         },
                         inputProps: {
                             maxLength: 20
                         }
-                    }), s().createElement("div", {
+                    }), o().createElement("div", {
                         className: "text-area-warning"
-                    }, s().createElement("p", {
+                    }, o().createElement("p", {
                         className: "environment-editor-section-label text-area-warning-text"
-                    }, this.state.newEnvShellPrompt.length >= 20 && "Max length = 20"), s().createElement("p", {
+                    }, this.state.newEnvShellPrompt.length >= 20 && "Max length = 20"), o().createElement("p", {
                         className: `environment-editor-section-label text-area-warning-text ${this.state.newEnvShellPrompt.length>=20&&"text-area-error-text"}`
-                    }, 20 - this.state.newEnvShellPrompt.length))), s().createElement(v.Grid, {
+                    }, 20 - this.state.newEnvShellPrompt.length))), o().createElement(v.Grid, {
                         item: !0,
                         xs: 12
-                    }, s().createElement(v.FormControl, {
+                    }, o().createElement(v.FormControl, {
                         fullWidth: !0
-                    }, s().createElement(v.Select, {
+                    }, o().createElement(v.Select, {
                         onChange: e => {
                             e.preventDefault(), this.state.pythonVersions.filter((t => t.label === e.target.value))[0].isLocked || this.setState({
                                 newEnvPythonVersion: e.target.value
                             }, (() => {
                                 this.handlePythonVersionChange(e.target.value)
                             }))
                         },
@@ -4809,85 +5190,85 @@
                             fontSize: "14px",
                             "& .MuiSelect-select": {
                                 display: "flex",
                                 alignItems: "center",
                                 padding: "4.5px 3px"
                             }
                         }
-                    }, this.state.pythonVersions.map((e => s().createElement(v.MenuItem, {
+                    }, this.state.pythonVersions.map((e => o().createElement(v.MenuItem, {
                         key: e.label,
                         value: e.label,
                         sx: {
                             backgroundColor: "var(--jp-layout-color1)",
                             color: "var(--jp-ui-font-color1)",
                             fontSize: "14px !important",
                             "&.Mui-selected": {
                                 backgroundColor: "rgba(211, 9, 130, 0.16)"
                             }
                         }
-                    }, e.isLocked ? s().createElement(s().Fragment, null, e.label, s().createElement(v.Tooltip, {
+                    }, e.isLocked ? o().createElement(o().Fragment, null, e.label, o().createElement(v.Tooltip, {
                         title: "Versioned Python environments coming soon!",
                         arrow: !0
-                    }, s().createElement(p.Z, {
+                    }, o().createElement(p.Z, {
                         sx: {
                             fontSize: "14px",
                             marginLeft: "0.5rem"
                         }
-                    }))) : e.label))))))))), s().createElement("div", {
+                    }))) : e.label))))))))), o().createElement("div", {
                         className: "envSidebar-flex-container"
-                    }, s().createElement("button", {
+                    }, o().createElement("button", {
                         className: "envSidebar-custom-button envSidebar-flex-btn envSidebar-btn-discard",
                         onClick: this.closeNewEnvironmentForm
-                    }, s().createElement(V.Z, {
+                    }, o().createElement(J.Z, {
                         fontSize: "16px"
-                    }), "Cancel"), s().createElement("button", {
+                    }), "Cancel"), o().createElement("button", {
                         className: "envSidebar-custom-button envSidebar-flex-btn envSidebar-btn-save " + (this.state.makeNewEnv ? "environment-editor-active" : ""),
                         onClick: this.handleCreateEnvironmentClick,
                         disabled: this.state.installingEnvironment
-                    }, s().createElement(H.Z, {
+                    }, o().createElement(K.Z, {
                         fontSize: "16px"
                     }), this.state.makeNewEnv ? "Creating..." : "Create"))))), this.renderIntelTermsAndConditionModal(), this.renderUpgradeDialogue(), this.renderPopupMsg(this.state.popupMsg)))
                 }
             }
-            ye.childContextTypes = c;
-            class we extends o.ReactWidget {
+            ke.childContextTypes = c;
+            class Se extends i.ReactWidget {
                 constructor(e, t) {
                     super(), this.flux = e, this.app = t
                 }
                 render() {
-                    return s().createElement(ye, {
+                    return o().createElement(ke, {
                         flux: this.flux,
                         app: this.app
                     })
                 }
             }
-            var ke = n(7386),
-                Se = n.n(ke),
-                Ae = n(7758),
-                Ce = n.n(Ae);
-            Ce().configure({
+            var Ae = n(7386),
+                Ce = n.n(Ae),
+                Ie = n(7758),
+                Pe = n.n(Ie);
+            Pe().configure({
                 region: "us-east-1",
                 userPoolId: "us-east-1_7hq9OmpnT",
                 userPoolWebClientId: "70fo00fpob1sd133m98k7b0jan",
                 authenticationFlowType: "USER_SRP_AUTH"
             });
-            const Ie = function() {
+            const Te = function() {
                     this.registerAlt = e => {
                         this.alt = e, this.actions = e.getActions(this.__proto__.constructor.__proto__.name)
                     }, this._updateUser = e => e, this._signOut = () => {}, this.getUser = e => (this.alt.dispatch(this, e), new Promise(((t, n) => {
-                        Ce().currentAuthenticatedUser({
+                        Pe().currentAuthenticatedUser({
                             bypassCache: e
                         }).then((e => {
                             this.actions._updateUser(e), t(e)
                         })).catch((e => {
                             this.actions._signOut(), t()
                         }))
                     })))
                 },
-                Pe = function() {
+                Ne = function() {
                     this.registerAlt = e => {
                         this.alt = e, this.actions = e.getActions(this.__proto__.constructor.__proto__.name)
                     }, this._updateAll = e => e, this._registerActivated = e => e, this._registerInstalling = e => e, this.updateAll = () => (this.alt.dispatch(this), new Promise(((e, t) => {
                         this.alt.getActions("ApiActions").query().get("/environments").end(((n, i) => {
                             if (n) t(n);
                             else {
                                 let t = i.body;
@@ -5145,32 +5526,14 @@
                             })).catch((e => {
                                 const t = `Error in getQuantumJobStatus: ${e.message}`;
                                 return n(t)
                             }))
                         } catch (e) {
                             return n("Quantum jobs not added.")
                         }
-                    }))), this.addQuantumJobs = e => (this.alt.dispatch(this), new Promise(((t, n) => {
-                        try {
-                            this.alt.getActions("JupyterApiActions").query("quantum-jobs", {
-                                body: JSON.stringify({
-                                    slug: e
-                                }),
-                                method: "POST"
-                            }).then((e => {
-                                e.success ? t({
-                                    success: e.success,
-                                    stdout: e.stdout
-                                }) : (console.log(`Failed to add quantum jobs: ${e.stderr}`), n(e.stderr))
-                            })).catch((e => {
-                                console.log(`Failed to add quantum jobs: ${e.message}`), n(e)
-                            }))
-                        } catch (e) {
-                            console.log(`Failed to add quantum jobs: ${e.message}`), n(e)
-                        }
                     }))), this.uninstallPackagePyvenv = e => (this.alt.dispatch(this), new Promise(((t, n) => {
                         let i = {
                             slug: `${e.slug}`,
                             package: `${e.package}`
                         };
                         this.alt.getActions("JupyterApiActions").query("uninstall-package", {
                             body: JSON.stringify(i),
@@ -5310,39 +5673,63 @@
                                 200 === (null == e ? void 0 : e.status) ? t(e) : n(e.message)
                             })).catch((e => {
                                 n(e)
                             }))
                         } catch (e) {
                             console.log(e), n(e)
                         }
+                    }))), this.publishEnvironment = e => (this.alt.dispatch(this), new Promise(((t, n) => {
+                        try {
+                            this.alt.getActions("ApiActions").query().post("/environments/publish").send({
+                                slug: e
+                            }).then((e => {
+                                200 === (null == e ? void 0 : e.status) ? t(e) : n(e.message)
+                            })).catch((e => {
+                                n(e)
+                            }))
+                        } catch (e) {
+                            console.log(e), n(e)
+                        }
+                    }))), this.updatePublishStatus = (e, t) => (this.alt.dispatch(this), new Promise(((n, i) => {
+                        try {
+                            this.alt.getActions("ApiActions").query().put(`/environments/publish/status/${t}`).send({
+                                slug: e
+                            }).then((e => {
+                                200 === (null == e ? void 0 : e.status) ? n(e) : i(e.message)
+                            })).catch((e => {
+                                i(e)
+                            }))
+                        } catch (e) {
+                            console.log(e), i(e)
+                        }
                     })))
                 };
-            var Ne = n(2046),
-                Te = n(4582);
+            var Oe = n(2046),
+                je = n(4582);
 
-            function je() {
+            function Ue() {
                 this.registerAlt = e => {
                     this.alt = e
                 }, this.query = (e, t) => new Promise((async (n, i) => {
-                    const a = Te.ServerConnection.makeSettings(),
-                        s = Ne.URLExt.join(a.baseUrl, "jupyter-environment-manager", e);
+                    const a = je.ServerConnection.makeSettings(),
+                        s = Oe.URLExt.join(a.baseUrl, "jupyter-environment-manager", e);
                     let o;
                     try {
-                        o = await Te.ServerConnection.makeRequest(s, t, a)
+                        o = await je.ServerConnection.makeRequest(s, t, a)
                     } catch (e) {
                         console.log(e), i(e)
                     }
                     const r = await o.json();
                     o.ok || i({
                         response: o,
                         data: r
                     }), n(r)
                 }))
             }
-            const Ue = function() {
+            const Le = function() {
                     this.registerAlt = e => {
                         this.alt = e, this.actions = e.getActions(this.__proto__.constructor.__proto__.name)
                     }, this._updateUser = e => e, this._updateConfig = e => e, this._updateIsMount = e => e, this.getUser = () => (this.alt.dispatch(this), new Promise(((e, t) => {
                         this.alt.getActions("ApiActions").query().get("/identity").end(((t, n) => {
                             t ? (this.actions._updateUser(null), e(null)) : (this.actions._updateUser(n.body), e(n.body))
                         }))
                     }))), this.getLocalConfig = () => (this.alt.dispatch(this), new Promise(((e, t) => {
@@ -5378,26 +5765,24 @@
                         }))
                     }, this.verifyUserSession = () => (this.alt.dispatch(this), new Promise(((e, t) => {
                         try {
                             const {
                                 user: t,
                                 config: n
                             } = this.alt.getStore("UserStore").getState(), i = null == t ? void 0 : t.email, a = null == n ? void 0 : n.email;
-                            i && a && i !== a && setTimeout((() => {
-                                alert("WARNING: User Mismatch\n\nThe logged-in email '" + a + "' does not match the email '" + i + "' associated with your current session.\n\nPlease clear your browser cookies and refresh the page, or use a private browsing window to ensure qBraid Lab functions correctly.")
-                            }), 3e3), e({
+                            i && a && i !== a && console.log("WARNING: User Mismatch\n\nThe logged-in email '" + a + "' does not match the email '" + i + "' associated with your current session.\n\nPlease clear your browser cookies and refresh the page, or use a private browsing window to ensure qBraid Lab functions correctly."), e({
                                 status: "Success",
                                 message: "User session verification complete."
                             })
                         } catch (t) {
                             console.error(t), e(null)
                         }
                     })))
                 },
-                Oe = function e() {
+                ze = function e() {
                     this.state = {
                         isAuthenticated: !1,
                         user: null
                     }, e.prototype.handleUpdateUser = e => {
                         this.setState({
                             isAuthenticated: !0,
                             user: e
@@ -5413,15 +5798,15 @@
                         _signOut: n
                     } = this.alt.getActions("AuthActions");
                     this.bindListeners({
                         handleUpdateUser: t,
                         handleSignOut: n
                     })
                 },
-                Le = function e() {
+                qe = function e() {
                     this.state = {
                         installingEnvironment: null,
                         environmentCache: {},
                         environments: []
                     }, e.prototype.handleUpdateAll = e => {
                         let {
                             environmentCache: t
@@ -5440,15 +5825,15 @@
                         _registerInstalling: n
                     } = this.alt.getActions("EnvironmentActions");
                     this.bindListeners({
                         handleUpdateAll: t,
                         handleRegisterInstalling: n
                     })
                 },
-                ze = function e() {
+                Be = function e() {
                     this.state = {
                         user: null,
                         config: null,
                         isMount: null
                     }, e.prototype.handleUpdateUser = e => {
                         this.setState({
                             user: e
@@ -5469,87 +5854,109 @@
                     } = this.alt.getActions("UserActions");
                     this.bindListeners({
                         handleUpdateUser: t,
                         handleUpdateConfig: n,
                         handleUpdateIsMount: i
                     })
                 };
-            class _e extends(Se()) {
+            class _e extends(Ce()) {
                 constructor(e) {
                     super(), this.registerAltWithActions = () => {
                         for (const e in this.actions) "global" !== e && this.actions[e].registerAlt(this)
-                    }, this.apiBaseUrl = e.apiBaseUrl, this.jupyterlab = e.jupyterlab, this.addActions("ApiActions", k), this.addActions("AuthActions", Ie), this.addActions("EnvironmentActions", Pe), this.addActions("JupyterApiActions", je), this.addActions("UserActions", Ue), this.registerAltWithActions(), this.addStore("AuthStore", Oe), this.addStore("EnvironmentStore", Le), this.addStore("UserStore", ze)
+                    }, this.apiBaseUrl = e.apiBaseUrl, this.jupyterlab = e.jupyterlab, this.addActions("ApiActions", k), this.addActions("AuthActions", Te), this.addActions("EnvironmentActions", Ne), this.addActions("JupyterApiActions", Ue), this.addActions("UserActions", Le), this.registerAltWithActions(), this.addStore("AuthStore", ze), this.addStore("EnvironmentStore", qe), this.addStore("UserStore", Be)
                 }
             }
             const De = _e,
-                qe = new i.LabIcon({
+                Me = new a.LabIcon({
                     name: "environments-sidebar:icon",
                     svgstr: '<svg class="env_icon" height="512pt" viewBox="0 0 512 512" width="512pt" xmlns="http://www.w3.org/2000/svg" fill="white"><path d="m306 150c0-27.570312-22.429688-50-50-50s-50 22.429688-50 50 22.429688 50 50 50 50-22.429688 50-50zm-80 0c0-16.542969 13.457031-30 30-30s30 13.457031 30 30-13.457031 30-30 30-30-13.457031-30-30zm0 0"/><path d="m266.003906 150c0-5.523438-4.476562-10-10-10h-.007812c-5.523438 0-9.996094 4.476562-9.996094 10s4.480469 10 10.003906 10c5.523438 0 10-4.476562 10-10zm0 0"/><path d="m110 402h-30v-31c0-5.515625 4.484375-10 10-10h20c5.523438 0 10-4.476562 10-10s-4.476562-10-10-10h-20c-16.542969 0-30 13.457031-30 30v31h-30c-16.542969 0-30 13.457031-30 30v50c0 16.542969 13.457031 30 30 30h80c16.542969 0 30-13.457031 30-30v-50c0-16.542969-13.457031-30-30-30zm10 80c0 5.515625-4.488281 10-10 10h-80c-5.515625 0-10-4.484375-10-10v-50c0-5.511719 4.484375-10 10-10h80c5.511719 0 10 4.488281 10 10zm0 0"/><path d="m482 402h-30v-31c0-16.542969-13.457031-30-30-30h-156v-41h13.332031c5.523438 0 10-4.476562 10-10v-23.828125c8.789063-2.515625 17.230469-6.015625 25.234375-10.464844l16.855469 16.855469c1.875 1.875 4.421875 2.929688 7.074219 2.929688s5.195312-1.054688 7.070312-2.929688l32.996094-33c3.90625-3.902344 3.90625-10.234375 0-14.140625l-16.855469-16.855469c4.445313-8.003906 7.945313-16.445312 10.460938-25.234375h23.832031c5.519531 0 10-4.476562 10-10v-46.667969c0-5.523437-4.480469-10-10-10h-23.828125c-2.511719-8.789062-6.015625-17.230468-10.464844-25.238281l16.855469-16.851562c1.875-1.875 2.929688-4.417969 2.929688-7.070313s-1.054688-5.195312-2.929688-7.070312l-32.996094-33c-1.875-1.875-4.421875-2.929688-7.074218-2.929688-2.652344 0-5.195313 1.054688-7.070313 2.929688l-16.851563 16.855468c-8.007812-4.449218-16.449218-7.949218-25.238281-10.464843v-23.824219c0-5.523438-4.476562-10-10-10h-46.664062c-5.523438 0-10 4.476562-10 10v23.828125c-8.789063 2.515625-17.230469 6.015625-25.234375 10.464844l-16.859375-16.859375c-1.875-1.875-4.417969-2.925782-7.070313-2.925782s-5.195312 1.050782-7.070312 2.925782l-33 33c-3.902344 3.902344-3.902344 10.234375 0 14.140625l16.859375 16.859375c-4.445313 8-7.945313 16.445312-10.460938 25.234375h-23.832031c-5.523438 0-10 4.476562-10 10v46.664062c0 5.523438 4.476562 10 10 10h23.828125c2.511719 8.789063 6.011719 17.230469 10.460937 25.238281l-16.855468 16.851563c-3.902344 3.90625-3.902344 10.238281 0 14.144531l33 33c1.875 1.875 4.417968 2.925782 7.070312 2.925782s5.195313-1.050782 7.070313-2.925782l16.855469-16.855468c8.003906 4.449218 16.445312 7.949218 25.234374 10.464843v23.824219c0 5.523438 4.476563 10 10 10h13.332032v41h-45.996094c-5.523438 0-10 4.476562-10 10s4.476562 10 10 10h45.996094v41h-29.996094c-16.542969 0-30 13.457031-30 30v50c0 16.542969 13.457031 30 30 30h79.996094c16.542968 0 30-13.457031 30-30v-50c0-16.542969-13.457032-30-30-30h-30v-41h156.003906c5.511719 0 10 4.484375 10 10v31h-30c-16.542969 0-30 13.457031-30 30v50c0 13.65625 9.242188 25.601562 22.476562 29.039062 5.347657 1.390626 10.808594-1.816406 12.195313-7.160156 1.390625-5.347656-1.816406-10.804687-7.160156-12.195312-4.425781-1.148438-7.511719-5.132813-7.511719-9.683594v-50c0-5.511719 4.484375-10 10-10h80c5.511719 0 10 4.488281 10 10v50c0 4.554688-3.09375 8.535156-7.519531 9.683594-5.34375 1.390625-8.550781 6.847656-7.164063 12.195312 1.167969 4.5 5.226563 7.488282 9.671875 7.488282.832031 0 1.679688-.105469 2.519531-.324219 13.242188-3.4375 22.488282-15.382813 22.488282-29.042969v-50c.003906-16.542969-13.453125-30-29.996094-30zm-247.238281-153.40625c-11.921875-2.558594-23.179688-7.222656-33.453125-13.871094-3.957032-2.5625-9.167969-2.007812-12.503906 1.324219l-15.300782 15.304687-18.855468-18.855468 15.300781-15.304688c3.335937-3.332031 3.886719-8.542968 1.324219-12.503906-6.644532-10.269531-11.3125-21.527344-13.867188-33.449219-.988281-4.609375-5.0625-7.90625-9.777344-7.90625h-21.628906v-26.664062h21.636719c4.714843 0 8.789062-3.296875 9.777343-7.90625 2.554688-11.925781 7.21875-23.179688 13.863282-33.449219 2.5625-3.957031 2.011718-9.167969-1.324219-12.503906l-15.304687-15.304688 18.855468-18.855468 15.304688 15.304687c3.335937 3.335937 8.546875 3.886719 12.503906 1.324219 10.273438-6.644532 21.527344-11.3125 33.453125-13.871094 4.609375-.988281 7.902344-5.0625 7.902344-9.777344v-21.628906h26.664062v21.628906c0 4.714844 3.292969 8.789063 7.90625 9.777344 11.921875 2.554688 23.179688 7.222656 33.453125 13.871094 3.957032 2.558594 9.167969 2.007812 12.5-1.328125l15.304688-15.300781 18.855468 18.855468-15.304687 15.300782c-3.332031 3.335937-3.882813 8.546874-1.324219 12.503906 6.648438 10.273437 11.316406 21.527344 13.871094 33.453125.988281 4.609375 5.0625 7.902343 9.777344 7.902343h21.628906v26.667969h-21.636719c-4.714843 0-8.789062 3.292969-9.777343 7.90625-2.554688 11.921875-7.21875 23.179688-13.863282 33.449219-2.5625 3.957031-2.011718 9.167969 1.324219 12.5l15.304687 15.304688-18.855468 18.855468-15.304688-15.304687c-3.335937-3.332031-8.546875-3.886719-12.503906-1.324219-10.273438 6.648438-21.527344 11.316406-33.449219 13.871094-4.613281.988281-7.90625 5.0625-7.90625 9.777344v21.632812h-26.664062v-21.628906c0-4.714844-3.292969-8.789063-7.90625-9.777344zm71.238281 183.40625v50c0 5.511719-4.484375 10-10 10h-80c-5.515625 0-10-4.488281-10-10v-50c0-5.515625 4.484375-10 10-10h80c5.515625 0 10 4.488281 10 10zm0 0"/><path d="m155.003906 341h-.007812c-5.523438 0-9.996094 4.476562-9.996094 10s4.480469 10 10.003906 10c5.523438 0 10-4.476562 10-10s-4.476562-10-10-10zm0 0"/><path d="m442 492h-.007812c-5.523438 0-9.996094 4.476562-9.996094 10s4.480468 10 10.003906 10 10-4.476562 10-10-4.476562-10-10-10zm0 0"/></svg>'
                 }),
-                Be = (e, t) => {
-                    const n = new we(e, t);
-                    return n.id = "environments-sidebar", n.title.label = "ENVS", n.title.caption = "Environment Manager", n.title.className = "environment_sidebar_li", n.title.icon = qe, n.title.iconClass = "env_icon_parent", n
+                Re = (e, t) => {
+                    const n = new Se(e, t);
+                    return n.id = "environments-sidebar", n.title.label = "ENVS", n.title.caption = "Environment Manager", n.title.className = "environment_sidebar_li", n.title.icon = Me, n.title.iconClass = "env_icon_parent", n
                 },
                 Fe = {
                     id: "@qbraid/jupyter-environment-manager",
                     autoStart: !0,
                     activate: async (e, t) => {
                         const {
-                            commands: n
-                        } = e, i = new De({
+                            commands: n,
+                            shell: a
+                        } = e, s = new De({
                             apiBaseUrl: w,
                             jupyterlab: e
                         });
                         try {
-                            const a = i.getActions("AuthActions"),
-                                s = i.getActions("UserActions"),
-                                o = i.getActions("EnvironmentActions");
-                            await a.getUser(), await s.getLocalConfig(), await s.getUser(), await s.checkFileMount();
+                            const o = s.getActions("AuthActions"),
+                                r = s.getActions("UserActions"),
+                                l = s.getActions("EnvironmentActions");
+                            await o.getUser(), await r.getLocalConfig(), await r.getUser(), await r.checkFileMount();
                             try {
-                                await o.updateAll(), await o.registerInstalled(), s.verifyUserSession()
+                                await l.updateAll(), await l.registerInstalled(), r.verifyUserSession()
                             } catch (e) {
                                 console.error("Error updating environments", e)
                             }
-                            let r = Be(i, e);
-                            e.shell.add(r, "right", {
+                            let c = Re(s, e);
+                            e.shell.add(c, "right", {
                                 rank: 1
                             }), e.shell.activateById("environments-sidebar");
-                            const l = "environment-manager:open-sidebar";
-                            n.addCommand(l, {
+                            const d = "environment-manager:open-sidebar";
+                            n.addCommand(d, {
                                 caption: "Environments",
                                 label: "Environments",
                                 icon: null,
                                 execute: () => {
-                                    r && r.dispose(), r = Be(i, e), e.shell.add(r, "right", {
+                                    c && c.dispose(), c = Re(s, e), e.shell.add(c, "right", {
                                         rank: 1
                                     }), e.shell.activateById("environments-sidebar")
                                 }
                             }), t && t.addItem({
-                                command: l,
+                                command: d,
                                 category: "qBraid Ecosystem",
                                 args: {
                                     origin: "from the palette"
                                 }
                             });
-                            const c = "environment-manager:close-sidebar";
-                            n.addCommand(c, {
+                            const p = "environment-manager:close-sidebar";
+                            n.addCommand(p, {
                                 caption: "Environments",
                                 label: "Environments",
                                 icon: null,
                                 execute: () => {
-                                    r && r.dispose(), r = Be(i, e), e.shell.add(r, "right", {
+                                    c && c.dispose(), c = Re(s, e), e.shell.add(c, "right", {
                                         rank: 1
                                     })
                                 }
                             }), t && t.addItem({
-                                command: c,
+                                command: p,
                                 category: "qBraid Ecosystem",
                                 args: {
                                     origin: "from the palette"
                                 }
+                            });
+                            const h = (e, t) => {
+                                    const n = new i.IFrame({
+                                        sandbox: ["allow-scripts", "allow-forms", "allow-same-origin", "allow-presentation", "allow-top-navigation", "allow-storage-access-by-user-activation"]
+                                    });
+                                    return n.url = e, n.title.label = t, n.title.icon = Me, n.title.iconClass = "env-manager_browser-icon-parent", n.id = `${m} - ${++g}`, new i.MainAreaWidget({
+                                        content: n
+                                    })
+                                },
+                                m = "qbraid-docs";
+                            let g = 0;
+                            const u = new i.WidgetTracker({
+                                    namespace: m
+                                }),
+                                v = "docs:qbraid-env-manager";
+                            n.addCommand(v, {
+                                label: "qbraid environment manager reference",
+                                execute: () => {
+                                    const e = h("https://docs.qbraid.com/projects/lab/en/latest/lab/environments.html", "Environment manager");
+                                    return u.add(e), a.add(e, "main"), e
+                                }
                             })
                         } catch (e) {
                             console.log("\n[!] Failed to activate environment-manager [!]\n"), console.error(e)
                         }
                     }
                 }
         },
@@ -5579,15 +5986,15 @@
             n.d(t, {
                 Z: () => s
             });
             var i = n(3645),
                 a = n.n(i)()((function(e) {
                     return e[1]
                 }));
-            a.push([e.id, "#environments-sidebar {\n  min-width: 300px !important;\n  background-color: red !important;\n}\n/* side bar formating start */\n\n/* these classes are over riden in ui tweeks,\nif ui tweeks is not available, while working with this extension,\n uncomment bellow code to format right side bar */\n\n/* .jp-SideBar.lm-TabBar.jp-mod-right {\n  width: 60px !important;\n  max-width: 60px !important;\n  min-width: 60px !important;\n  left: unset !important;\n  right: 0 !important;\n}\n.jp-mod-right > ul > li {\n  display: flex !important;\n  flex-direction: column !important;\n  justify-content: center !important;\n  align-items: center !important;\n  width: 60px !important;\n  max-width: 60px !important;\n  min-width: 60px !important;\n  height: 60px !important;\n  max-height: 60px !important;\n  min-height: 60px !important;\n  align-items: center !important;\n  margin: 0 !important;\n  padding: 0 !important;\n  text-align: center;\n  color: var(--jp-ui-font-color1) !important;\n  transform: rotate(-90deg) translateX(28px) !important;\n  border-right: var(--jp-border-width) solid var(--jp-border-color1) !important;\n  border-left: unset !important;\n} */\n\n.env_icon_parent {\n  transition: none !important;\n  transform: rotate(0deg) !important;\n}\nbody[data-jp-theme-light='true'] .env_icon {\n  filter: invert(0.6);\n}\n.env_icon {\n  width: 30px;\n  height: 30px;\n  min-width: 30px;\n  min-height: 30px;\n  margin-top: 5px !important;\n}\n/* this class is for the right side bar list item for environment manger extesion\n.environment_sidebar_li {\n } */\n\n.environment_sidebar_li div:nth-child(2) {\n  text-align: center !important;\n  min-width: fit-content !important;\n  font-size: 10px !important;\n  text-transform: uppercase !important;\n  flex: 0 1 auto !important;\n  margin-top: -5px !important;\n}\n\n/* side bar formating end  */\n\n.environments-sidebar {\n  /* position: relative; */\n  position: absolute;\n  height: 100%;\n  width: 100%;\n  /* width: 420px; */\n  background-color: var(--jp-layout-color1) !important;\n  /* overflow-x: visible; */\n}\n\n.environments-sidebar-header {\n  padding: 15px 10px;\n  color: #d30982;\n  font-weight: 600;\n  text-transform: uppercase;\n  letter-spacing: 1px;\n}\n\n.environments-sidebar-spacer {\n  width: 100%;\n  height: var(--jp-border-width);\n  background-color: var(--jp-border-color2);\n}\n\n.environments-sidebar-list-pane,\n.environments-sidebar-search-pane {\n  position: absolute;\n  right: 0%;\n  height: calc(100% - 50px);\n  overflow-x: hidden;\n  overflow-y: auto;\n  /* height: 100%; */\n}\n\n.environments-sidebar-list-pane {\n  width: 100%;\n  transition: 300ms right ease;\n}\n\n.environments-sidebar-search-pane {\n  width: 0%;\n  transition: width 300ms ease;\n}\n\n.environments-sidebar-environment-list {\n  padding-bottom: 200px;\n  background-color: var(--jp-layout-color1);\n}\n\n.envoronments-sidebar-search-wrapper {\n  position: relative;\n}\n\n.environments-sidebar-search-icon {\n  position: absolute;\n  width: 16px;\n  top: 0px;\n  left: 1rem;\n  color: var(--jp-ui-font-color2);\n}\n\n.environments-sidebar-search-bar {\n  width: calc(100% - 62px);\n  /* 62px accounts for horizontal margin and padding */\n  margin: 10px;\n  font-size: 14px;\n  border: 1px solid var(--jp-border-color2);\n  border-radius: 2px;\n  color: var(--jp-ui-font-color2);\n  /* background: url(https://qbraid-static.s3.amazonaws.com/search.svg) no-repeat */\n  /* scroll 8px 10px; */\n  background-color: var(--jp-input-background);\n  padding: 10px 10px 10px 32px;\n  /* background-size: 16px; */\n  box-sizing: content-box !important;\n  transition: all 0.2s linear;\n}\n\n.environments-sidebar-search-bar:hover {\n  border-color: var(--jp-border-color1);\n}\n\n.environments-sidebar-search-bar:focus {\n  outline: none;\n  border-color: var(--jp-border-color1);\n  background-color: var(--jp-input-active-background);\n}\n\n.refresh-btn {\n  fill: #d30982;\n  border-radius: 50%;\n  height: 20px;\n  width: 20px;\n}\n\n.refresh-btn:hover {\n  cursor: pointer;\n  fill: #ff24a7;\n  /* border-radius: 50%;\n  box-shadow: 0px 1px 3px 2px rgb(0 0 0 / 40%); */\n}\n\n.div-refresh-btn {\n  height: 20px;\n  margin-left: 5px;\n}\n\n.environments-sidebar-refresh-btn {\n  cursor: pointer;\n  height: 20px;\n  margin-left: 4px;\n  transition: 300ms opacity ease;\n}\n\n.environments-sidebar-add-btn {\n  float: right;\n  color: #d30982;\n  /* color: #ff24a7; */\n  /* color: #aaa; */\n  cursor: pointer;\n  opacity: 1;\n  transition: 300ms opacity ease;\n}\n\n.environments-sidebar-left-arrow {\n  font-size: 20px;\n  margin-top: -2px;\n}\n\n.environments-sidebar-add-btn:hover {\n  color: #ff24a7;\n}\n\n.environments-sidebar-back-btn {\n  vertical-align: baseline;\n  display: inline-block;\n  margin-right: 5px;\n  height: 0;\n  transition: 300ms opacity ease;\n  margin-top: -22px;\n  cursor: pointer;\n}\n\n.environments-sidebar-back-btn:hover {\n  color: #ff24a7;\n}\n\n.environments-sidebar-tab-empty {\n  color: var(--jp-ui-font-color3);\n  margin-top: 20px;\n  text-align: center;\n  font-style: italic;\n}\n\n.environments-sidebar-create-env {\n  position: relative;\n  display: flex;\n  flex-direction: row;\n  justify-content: center;\n  align-items: center;\n  margin: 10px;\n  padding: 4px 10px;\n  border: 2px solid transparent;\n  border-radius: 10px;\n  box-sizing: content-box !important;\n  /* overrides jupyterhub, which sets box-sizing: border-box */\n  background-color: #845bc3;\n  background-color: #673ab7;\n  color: white;\n  box-shadow: 0px 1px 4px -2px #555;\n  cursor: pointer;\n}\n\n.environment-tile {\n  margin: 10px;\n  padding: 10px;\n  background-color: var(--jp-layout-color2);\n  border-radius: 4px;\n  border-bottom: 1px solid var(--jp-layout-color3);\n  cursor: pointer;\n}\n\n.environment-tile-name {\n  color: var(--jp-ui-font-color2);\n}\n\n.environment-tile-active-flag {\n  float: right;\n  /* color: #d20882; */\n  color: #742857;\n}\n\n.qbraid-splash-background {\n  position: fixed;\n  top: 0px;\n  bottom: 0px;\n  left: 0px;\n  right: 0px;\n  z-index: 999999;\n  background-color: #212121;\n  opacity: 1;\n  transition: 500ms opacity linear;\n}\n\n.qbraid-splash-foreground {\n  position: fixed;\n  top: calc(50vh - 200px);\n  width: 100vw;\n  text-align: center;\n  user-select: none;\n}\n\n.qbraid-splash-logo {\n  position: relative;\n  width: 200px;\n}\n\n.qbraid-splash-text {\n  position: relative;\n  margin-top: 20px;\n  font-size: 24px;\n  font-family: Helvetica;\n  color: #8c357d;\n}\n\n.overlay-background {\n  position: fixed;\n  display: flex;\n  flex-direction: column;\n  justify-content: center;\n  align-items: center;\n  height: 100vh;\n  width: 100vw;\n  top: 0;\n  left: 0;\n  background-color: rgba(0, 0, 0, 0.5);\n  z-index: 999998;\n}\n\n.overlay-dialog {\n  position: relative;\n  width: 50%;\n  margin-top: -40px;\n  border-radius: 25px;\n  background-color: #f5f5f5;\n  box-shadow: 0 5px 5px -3px rgba(0, 0, 0, 0.2),\n    0 8px 10px 1px rgba(0, 0, 0, 0.14), 0 3px 14px 2px rgba(0, 0, 0, 0.12);\n  z-index: 999999;\n}\n\n.overlay-title {\n  background: linear-gradient(90deg, #7643be 5.23%, #b469e0 84.11%);\n  border-radius: 25px 25px 0px 0px;\n}\n\n.overlay-backicon-wrapper {\n  padding: 5px;\n}\n\n.overlay-backicon {\n  cursor: pointer;\n}\n\n.overlay-content {\n  padding: 10px 20px 20px 20px;\n}\n\n.overlay-closeicon-wrapper {\n  position: absolute;\n  right: -24px;\n  top: -24px;\n}\n\n.overlay-closeicon {\n  cursor: pointer;\n}\n\n.overlay-icon-wrapper {\n  display: flex;\n  justify-content: center;\n  align-items: center;\n  width: 32px;\n  height: 32px;\n  background: #fb9b2a;\n  border-radius: 16px;\n  margin-right: 15px;\n}\n\n.overlay-icon-vector {\n  width: 16px;\n  height: 16px;\n}\n\n.overlay-input-wrapper {\n  display: flex;\n  margin-top: 5px;\n  background: #ffffff;\n  border-radius: 8px;\n  padding: 9px 20px;\n  align-items: center;\n}\n\n.overlay-inputgroup {\n  margin-top: 10px;\n}\n\n.overlay-input {\n  border: none;\n  flex-grow: 1;\n  padding-left: 9px;\n  border-left: 1px solid #d1d1d1;\n}\n\n.overlay-textfield {\n  border: none;\n  flex-grow: 1;\n}\n\n.overlay-button {\n  padding: 12px 20px;\n  border: none;\n  border-radius: 8px;\n  cursor: pointer;\n}\n\n.overlay-buttongroup {\n  display: flex;\n  margin-top: 20px;\n  background: #f5f5f5;\n  border: 1px solid #7f49c3;\n  border-radius: 8px;\n  box-sizing: border-box;\n}\n\n.overlay-toggle-button {\n  flex-grow: 1;\n  color: #7f49c3;\n}\n\n.overlay-toggle-active-button {\n  background: #7f49c3;\n  color: white;\n}\n\n.overlay-close-button {\n  background: #515254;\n  color: white;\n}\n\n.overlay-confirm-button {\n  background: #515254;\n  color: white;\n}\n\n.overlay-confirm-button-wrapper {\n  display: flex;\n  justify-content: end;\n  margin-top: 20px;\n}\n\n.editor-ace-wrapper {\n  flex: 1;\n  overflow: auto;\n  margin-top: 5px;\n}\n\n.env-dialog-img-title {\n  display: flex;\n  flex-direction: column;\n  justify-content: center;\n  align-items: center;\n}\n\n.env-dialog-img-content {\n  display: flex;\n  flex-direction: column;\n  justify-content: center;\n  align-items: center;\n  gap: 8px;\n}\n\n.env-dialog-img {\n  position: relative;\n  margin-inline: auto;\n  width: 250px;\n  height: 250px;\n  object-fit: scale-down;\n  border: 2px dashed #555;\n}\n\n.uploadImg-dialog-description {\n  font-size: 0.8rem !important;\n}\n\n.uploadImg-error-text {\n  flex: 1;\n  text-align: left;\n  color: indianred;\n  padding-left: 1em;\n  font-size: 0.8rem !important;\n}\n\n.env-sidebar-msg-popup {\n  position: absolute;\n  width: calc(100% - 4em);\n  margin: 0px 1em;\n  height: 3rem;\n  display: flex;\n  align-items: center;\n  justify-content: center;\n  border-radius: 10px;\n  bottom: 10px;\n  padding: 0.25em 1em;\n}\n.success {\n  background-color: green;\n  color: white;\n}\n.error {\n  background-color: indianred;\n  color: white;\n}\n.stay-longer {\n  animation-duration: 4s !important;\n}\n\n.highlight-kernel {\n  border: 1px solid #883ae8;\n  border-radius: 4px;\n  animation: blip-notify 3s alternate both;\n  animation-timing-function: cubic-bezier(0.47, 0, 0.75, 0.72);\n  --_text-clr: var(--jp-ui-font-color0);\n}\n\n.highlight-kernel .jp-ToolbarButtonComponent-label {\n  color: var(--_text-clr) !important;\n}\n\n.pos-fixed-kernel_message {\n  position: fixed;\n  top: 6rem;\n  right: 20rem;\n  background-color: var(--jp-layout-color1);\n  border: 1px solid var(--jp-border-color1);\n  border-radius: 4px;\n  padding: 8px;\n  color: var(--jp-ui-font-color0);\n  font-size: 14px;\n  box-shadow: var(--jp-elevation-z6);\n  opacity: 0;\n  transition: right 150ms ease, opacity 250ms ease;\n}\n\n.pos-fixed-kernel_message::after {\n  content: '';\n  position: absolute;\n  width: 15px;\n  height: 15px;\n  background-color: var(--jp-layout-color1);\n  top: -14px;\n  right: 15px;\n  clip-path: polygon(50% 0%, 0% 100%, 100% 100%);\n  box-shadow: var(--jp-elevation-z6);\n}\n\n.env_dialog-btn_cancel {\n  background-color: transparent !important;\n  border: 1px solid #6640b3 !important;\n  border-radius: 6px;\n  color: #6640b3 !important;\n}\n\n.env_dialog-btn_confirm {\n  background-color: #6640b3 !important;\n  border-radius: 6px;\n  color: white !important;\n}\n\n.gpu_warn_dialog-checkbox {\n  width: 100%;\n  padding-bottom: 8px;\n}\n\n.jp-Dialog-footer {\n  flex-wrap: wrap;\n}\n\n/* animation css */\n.slide-in-bottom {\n  -webkit-animation: slide-in-bottom 2.5s cubic-bezier(0.645, 0.045, 0.355, 1)\n    both;\n  animation: slide-in-bottom 2.5s cubic-bezier(0.645, 0.045, 0.355, 1) both;\n  /* animation-iteration-count: infinite; */\n}\n\n/**\n * ----------------------------------------\n * animation slide-in-bottom\n * ----------------------------------------\n */\n\n@keyframes slide-in-bottom {\n  0% {\n    -webkit-transform: translateY(40px);\n    transform: translateY(40px);\n    opacity: 0;\n  }\n  30% {\n    -webkit-transform: translateY(0);\n    transform: translateY(0);\n    opacity: 1;\n  }\n  80% {\n    -webkit-transform: translateY(0);\n    transform: translateY(0);\n    opacity: 1;\n  }\n  100% {\n    -webkit-transform: translateY(40px);\n    transform: translateY(40px);\n    opacity: 0;\n  }\n}\n\n/**\n * ----------------------------------------\n * animation pulsing-notification\n * ----------------------------------------\n */\n\n@keyframes blip-notify {\n  from {\n    background: #673ab7;\n    --_text-clr: white;\n  }\n  to {\n    background: #aa89e438;\n    --_text-clr: var(--jp-ui-font-color0);\n  }\n}\n", ""]);
+            a.push([e.id, "#environments-sidebar {\n  min-width: 300px !important;\n  background-color: red !important;\n}\n/* side bar formating start */\n\n/* these classes are over riden in ui tweeks,\nif ui tweeks is not available, while working with this extension,\n uncomment bellow code to format right side bar */\n\n/* .jp-SideBar.lm-TabBar.jp-mod-right {\n  width: 60px !important;\n  max-width: 60px !important;\n  min-width: 60px !important;\n  left: unset !important;\n  right: 0 !important;\n}\n.jp-mod-right > ul > li {\n  display: flex !important;\n  flex-direction: column !important;\n  justify-content: center !important;\n  align-items: center !important;\n  width: 60px !important;\n  max-width: 60px !important;\n  min-width: 60px !important;\n  height: 60px !important;\n  max-height: 60px !important;\n  min-height: 60px !important;\n  align-items: center !important;\n  margin: 0 !important;\n  padding: 0 !important;\n  text-align: center;\n  color: var(--jp-ui-font-color1) !important;\n  transform: rotate(-90deg) translateX(28px) !important;\n  border-right: var(--jp-border-width) solid var(--jp-border-color1) !important;\n  border-left: unset !important;\n} */\n\n.env_icon_parent {\n  transition: none !important;\n  transform: rotate(0deg) !important;\n}\nbody[data-jp-theme-light='true'] .env_icon {\n  filter: invert(0.6);\n}\n\n.env_icon_parent .env_icon {\n  width: 30px;\n  height: 30px;\n  min-width: 30px;\n  min-height: 30px;\n  margin-top: 5px !important;\n}\n/* this class is for the right side bar list item for environment manger extesion\n.environment_sidebar_li {\n } */\n\n.environment_sidebar_li div:nth-child(2) {\n  text-align: center !important;\n  min-width: fit-content !important;\n  font-size: 10px !important;\n  text-transform: uppercase !important;\n  flex: 0 1 auto !important;\n  margin-top: -5px !important;\n}\n\n/* side bar formating end  */\n\n.environments-sidebar {\n  /* position: relative; */\n  position: absolute;\n  height: 100%;\n  width: 100%;\n  /* width: 420px; */\n  background-color: var(--jp-layout-color1) !important;\n  /* overflow-x: visible; */\n}\n\n.environments-sidebar-header {\n  padding: 15px 10px;\n  color: #d30982;\n  font-weight: 600;\n  text-transform: uppercase;\n  letter-spacing: 1px;\n  display: flex;\n  flex-direction: row;\n  align-items: center;\n  justify-content: space-between;\n}\n\n.environments-sidebar-spacer {\n  width: 100%;\n  height: var(--jp-border-width);\n  background-color: var(--jp-border-color2);\n}\n\n.environments-sidebar-list-pane,\n.environments-sidebar-search-pane {\n  position: absolute;\n  right: 0%;\n  height: calc(100% - 50px);\n  overflow-x: hidden;\n  overflow-y: auto;\n  /* height: 100%; */\n}\n\n.environments-sidebar-list-pane {\n  width: 100%;\n  transition: 300ms right ease;\n}\n\n.environments-sidebar-search-pane {\n  width: 0%;\n  transition: width 300ms ease;\n}\n\n.environments-sidebar-environment-list {\n  padding-bottom: 200px;\n  background-color: var(--jp-layout-color1);\n}\n\n.envoronments-sidebar-search-wrapper {\n  position: relative;\n}\n\n.environments-sidebar-search-icon {\n  position: absolute;\n  width: 16px;\n  top: 0px;\n  left: 1rem;\n  color: var(--jp-ui-font-color2);\n}\n\n.environments-sidebar-search-bar {\n  width: calc(100% - 62px);\n  /* 62px accounts for horizontal margin and padding */\n  margin: 10px;\n  font-size: 14px;\n  border: 1px solid var(--jp-border-color2);\n  border-radius: 2px;\n  color: var(--jp-ui-font-color2);\n  /* background: url(https://qbraid-static.s3.amazonaws.com/search.svg) no-repeat */\n  /* scroll 8px 10px; */\n  background-color: var(--jp-input-background);\n  padding: 10px 10px 10px 32px;\n  /* background-size: 16px; */\n  box-sizing: content-box !important;\n  transition: all 0.2s linear;\n}\n\n.environments-sidebar-search-bar:hover {\n  border-color: var(--jp-border-color1);\n}\n\n.environments-sidebar-search-bar:focus {\n  outline: none;\n  border-color: var(--jp-border-color1);\n  background-color: var(--jp-input-active-background);\n}\n\n.refresh-btn {\n  fill: #d30982;\n  border-radius: 50%;\n  height: 20px;\n  width: 20px;\n}\n\n.refresh-btn:hover {\n  cursor: pointer;\n  fill: #ff24a7;\n  /* border-radius: 50%;\n  box-shadow: 0px 1px 3px 2px rgb(0 0 0 / 40%); */\n}\n\n.div-refresh-btn {\n  height: 20px;\n  margin-left: 5px;\n}\n\n.environments-sidebar-refresh-btn {\n  cursor: pointer;\n  height: 20px;\n  margin-left: 4px;\n  transition: 300ms opacity ease;\n}\n\n.environments-sidebar-add-btn {\n  float: right;\n  color: #d30982;\n  /* color: #ff24a7; */\n  /* color: #aaa; */\n  cursor: pointer;\n  opacity: 1;\n  transition: 300ms opacity ease;\n}\n\n.environments-sidebar-left-arrow {\n  font-size: 20px;\n  margin-top: -2px;\n}\n\n.environments-sidebar-add-btn:hover {\n  color: #ff24a7;\n}\n\n.environments-sidebar-back-btn {\n  vertical-align: baseline;\n  display: inline-block;\n  margin-right: 5px;\n  height: 0;\n  transition: 300ms opacity ease;\n  margin-top: -22px;\n  cursor: pointer;\n}\n\n.environments-sidebar-back-btn:hover {\n  color: #ff24a7;\n}\n\n.environments-sidebar-tab-empty {\n  color: var(--jp-ui-font-color3);\n  margin-top: 20px;\n  text-align: center;\n  font-style: italic;\n}\n\n.environments-sidebar-create-env {\n  position: relative;\n  display: flex;\n  flex-direction: row;\n  justify-content: center;\n  align-items: center;\n  margin: 10px;\n  padding: 4px 10px;\n  border: 2px solid transparent;\n  border-radius: 10px;\n  box-sizing: content-box !important;\n  /* overrides jupyterhub, which sets box-sizing: border-box */\n  background-color: #845bc3;\n  background-color: #673ab7;\n  color: white;\n  box-shadow: 0px 1px 4px -2px #555;\n  cursor: pointer;\n}\n\n.environment-tile {\n  margin: 10px;\n  padding: 10px;\n  background-color: var(--jp-layout-color2);\n  border-radius: 4px;\n  border-bottom: 1px solid var(--jp-layout-color3);\n  cursor: pointer;\n}\n\n.environment-tile-name {\n  color: var(--jp-ui-font-color2);\n}\n\n.environment-tile-active-flag {\n  float: right;\n  /* color: #d20882; */\n  color: #742857;\n}\n\n.qbraid-splash-background {\n  position: fixed;\n  top: 0px;\n  bottom: 0px;\n  left: 0px;\n  right: 0px;\n  z-index: 999999;\n  background-color: #212121;\n  opacity: 1;\n  transition: 500ms opacity linear;\n}\n\n.qbraid-splash-foreground {\n  position: fixed;\n  top: calc(50vh - 200px);\n  width: 100vw;\n  text-align: center;\n  user-select: none;\n}\n\n.qbraid-splash-logo {\n  position: relative;\n  width: 200px;\n}\n\n.qbraid-splash-text {\n  position: relative;\n  margin-top: 20px;\n  font-size: 24px;\n  font-family: Helvetica;\n  color: #8c357d;\n}\n\n.overlay-background {\n  position: fixed;\n  display: flex;\n  flex-direction: column;\n  justify-content: center;\n  align-items: center;\n  height: 100vh;\n  width: 100vw;\n  top: 0;\n  left: 0;\n  background-color: rgba(0, 0, 0, 0.5);\n  z-index: 999998;\n}\n\n.overlay-dialog {\n  position: relative;\n  width: 50%;\n  margin-top: -40px;\n  border-radius: 25px;\n  background-color: #f5f5f5;\n  box-shadow: 0 5px 5px -3px rgba(0, 0, 0, 0.2),\n    0 8px 10px 1px rgba(0, 0, 0, 0.14), 0 3px 14px 2px rgba(0, 0, 0, 0.12);\n  z-index: 999999;\n}\n\n.overlay-title {\n  background: linear-gradient(90deg, #7643be 5.23%, #b469e0 84.11%);\n  border-radius: 25px 25px 0px 0px;\n}\n\n.overlay-backicon-wrapper {\n  padding: 5px;\n}\n\n.overlay-backicon {\n  cursor: pointer;\n}\n\n.overlay-content {\n  padding: 10px 20px 20px 20px;\n}\n\n.overlay-closeicon-wrapper {\n  position: absolute;\n  right: -24px;\n  top: -24px;\n}\n\n.overlay-closeicon {\n  cursor: pointer;\n}\n\n.overlay-icon-wrapper {\n  display: flex;\n  justify-content: center;\n  align-items: center;\n  width: 32px;\n  height: 32px;\n  background: #fb9b2a;\n  border-radius: 16px;\n  margin-right: 15px;\n}\n\n.overlay-icon-vector {\n  width: 16px;\n  height: 16px;\n}\n\n.overlay-input-wrapper {\n  display: flex;\n  margin-top: 5px;\n  background: #ffffff;\n  border-radius: 8px;\n  padding: 9px 20px;\n  align-items: center;\n}\n\n.overlay-inputgroup {\n  margin-top: 10px;\n}\n\n.overlay-input {\n  border: none;\n  flex-grow: 1;\n  padding-left: 9px;\n  border-left: 1px solid #d1d1d1;\n}\n\n.overlay-textfield {\n  border: none;\n  flex-grow: 1;\n}\n\n.overlay-button {\n  padding: 12px 20px;\n  border: none;\n  border-radius: 8px;\n  cursor: pointer;\n}\n\n.overlay-buttongroup {\n  display: flex;\n  margin-top: 20px;\n  background: #f5f5f5;\n  border: 1px solid #7f49c3;\n  border-radius: 8px;\n  box-sizing: border-box;\n}\n\n.overlay-toggle-button {\n  flex-grow: 1;\n  color: #7f49c3;\n}\n\n.overlay-toggle-active-button {\n  background: #7f49c3;\n  color: white;\n}\n\n.overlay-close-button {\n  background: #515254;\n  color: white;\n}\n\n.overlay-confirm-button {\n  background: #515254;\n  color: white;\n}\n\n.overlay-confirm-button-wrapper {\n  display: flex;\n  justify-content: end;\n  margin-top: 20px;\n}\n\n.editor-ace-wrapper {\n  flex: 1;\n  overflow: auto;\n  margin-top: 5px;\n}\n\n.env-dialog-img-title {\n  display: flex;\n  flex-direction: column;\n  justify-content: center;\n  align-items: center;\n}\n\n.env-dialog-img-content {\n  display: flex;\n  flex-direction: column;\n  justify-content: center;\n  align-items: center;\n  gap: 8px;\n}\n\n.env-dialog-img {\n  position: relative;\n  margin-inline: auto;\n  width: 250px;\n  height: 250px;\n  object-fit: scale-down;\n  border: 2px dashed #555;\n}\n\n.uploadImg-dialog-description {\n  font-size: 0.8rem !important;\n}\n\n.uploadImg-error-text {\n  flex: 1;\n  text-align: left;\n  color: indianred;\n  padding-left: 1em;\n  font-size: 0.8rem !important;\n}\n\n.env-sidebar-msg-popup {\n  position: absolute;\n  width: calc(100% - 4em);\n  margin: 0px 1em;\n  height: 3rem;\n  display: flex;\n  align-items: center;\n  justify-content: center;\n  border-radius: 10px;\n  bottom: 10px;\n  padding: 0.25em 1em;\n}\n.success {\n  background-color: green;\n  color: white;\n}\n.error {\n  background-color: indianred;\n  color: white;\n}\n.stay-longer {\n  animation-duration: 4s !important;\n}\n\n.highlight-kernel {\n  border: 1px solid #883ae8;\n  border-radius: 4px;\n  animation: blip-notify 3s alternate both;\n  animation-timing-function: cubic-bezier(0.47, 0, 0.75, 0.72);\n  --_text-clr: var(--jp-ui-font-color0);\n}\n\n.highlight-kernel .jp-ToolbarButtonComponent-label {\n  color: var(--_text-clr) !important;\n}\n\n.pos-fixed-kernel_message {\n  position: fixed;\n  top: 6rem;\n  right: 20rem;\n  background-color: var(--jp-layout-color1);\n  border: 1px solid var(--jp-border-color1);\n  border-radius: 4px;\n  padding: 8px;\n  color: var(--jp-ui-font-color0);\n  font-size: 14px;\n  box-shadow: var(--jp-elevation-z6);\n  opacity: 0;\n  transition: right 150ms ease, opacity 250ms ease;\n}\n\n.pos-fixed-kernel_message::after {\n  content: '';\n  position: absolute;\n  width: 15px;\n  height: 15px;\n  background-color: var(--jp-layout-color1);\n  top: -14px;\n  right: 15px;\n  clip-path: polygon(50% 0%, 0% 100%, 100% 100%);\n  box-shadow: var(--jp-elevation-z6);\n}\n\n.env_dialog-btn_cancel {\n  background-color: transparent !important;\n  border: 1px solid #6640b3 !important;\n  border-radius: 6px;\n  color: #6640b3 !important;\n}\n\n.env_dialog-btn_confirm {\n  background-color: #6640b3 !important;\n  border-radius: 6px;\n  color: white !important;\n}\n\n.gpu_warn_dialog-checkbox {\n  width: 100%;\n  padding-bottom: 8px;\n}\n\n.jp-Dialog-footer {\n  flex-wrap: wrap;\n}\n\n/* animation css */\n.slide-in-bottom {\n  -webkit-animation: slide-in-bottom 2.5s cubic-bezier(0.645, 0.045, 0.355, 1)\n    both;\n  animation: slide-in-bottom 2.5s cubic-bezier(0.645, 0.045, 0.355, 1) both;\n  /* animation-iteration-count: infinite; */\n}\n\n/**\n * ----------------------------------------\n * animation slide-in-bottom\n * ----------------------------------------\n */\n\n@keyframes slide-in-bottom {\n  0% {\n    -webkit-transform: translateY(40px);\n    transform: translateY(40px);\n    opacity: 0;\n  }\n  30% {\n    -webkit-transform: translateY(0);\n    transform: translateY(0);\n    opacity: 1;\n  }\n  80% {\n    -webkit-transform: translateY(0);\n    transform: translateY(0);\n    opacity: 1;\n  }\n  100% {\n    -webkit-transform: translateY(40px);\n    transform: translateY(40px);\n    opacity: 0;\n  }\n}\n\n/**\n * ----------------------------------------\n * animation pulsing-notification\n * ----------------------------------------\n */\n\n@keyframes blip-notify {\n  from {\n    background: #673ab7;\n    --_text-clr: white;\n  }\n  to {\n    background: #aa89e438;\n    --_text-clr: var(--jp-ui-font-color0);\n  }\n}\n", ""]);
             const s = a
         },
         6513: (e, t, n) => {
             n.d(t, {
                 Z: () => s
             });
             var i = n(3645),
```

### Comparing `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/24.a6fec73552ceb9bdb6aa.js` & `jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/24.a6fec73552ceb9bdb6aa.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/313.f6abbabc37aacd77b555.js` & `jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/313.f6abbabc37aacd77b555.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/313.f6abbabc37aacd77b555.js.LICENSE.txt` & `jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/313.f6abbabc37aacd77b555.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/378.8fdd4b1246fb17037bb3.js` & `jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/378.8fdd4b1246fb17037bb3.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/478.b1efc8dc1ed4a16150ef.js` & `jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/478.b1efc8dc1ed4a16150ef.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/554.3ee5e631ee6f4d8c24e2.js` & `jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/554.3ee5e631ee6f4d8c24e2.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/569.110780388cdcc5605903.js` & `jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/569.110780388cdcc5605903.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/588.634556691591dc1dac9b.js` & `jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/588.634556691591dc1dac9b.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/66.715eff54360a4988967a.js` & `jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/66.715eff54360a4988967a.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/697.61315fde7050f7a02689.js` & `jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/697.61315fde7050f7a02689.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/747.6d49dfe38d298a9d88e1.js` & `jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/747.6d49dfe38d298a9d88e1.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/813.4baf0234297462c92d8b.js` & `jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/813.4baf0234297462c92d8b.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/909.c50074d4e4be5aa7c06a.js` & `jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/909.c50074d4e4be5aa7c06a.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/981.f54a04f7142174f18f0d.js` & `jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/981.f54a04f7142174f18f0d.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/981.f54a04f7142174f18f0d.js.LICENSE.txt` & `jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/981.f54a04f7142174f18f0d.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/991.b0c652da28634799e4d5.js` & `jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/991.b0c652da28634799e4d5.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/remoteEntry.5fd255ae2892e93a3890.js` & `jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/remoteEntry.df30dcda2252f4ea7597.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, a, n, o, i, d, c, f, l, u, s, b, p, h, m, v, g, y, w = {
+    var e, r, t, a, n, o, i, d, f, c, l, u, s, b, p, h, m, v, g, y, w = {
             7413: (e, r, t) => {
                 var a = {
-                        "./index": () => Promise.all([t.e(66), t.e(588), t.e(0), t.e(271), t.e(222), t.e(456), t.e(185)]).then((() => () => t(4185))),
-                        "./extension": () => Promise.all([t.e(66), t.e(588), t.e(0), t.e(271), t.e(222), t.e(456), t.e(185)]).then((() => () => t(4185))),
+                        "./index": () => Promise.all([t.e(66), t.e(588), t.e(0), t.e(271), t.e(222), t.e(456), t.e(227)]).then((() => () => t(3227))),
+                        "./extension": () => Promise.all([t.e(66), t.e(588), t.e(0), t.e(271), t.e(222), t.e(456), t.e(227)]).then((() => () => t(3227))),
                         "./style": () => t.e(747).then((() => () => t(9747)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     o = (e, r) => {
                         if (t.S) {
@@ -52,17 +52,17 @@
     }, j.f = {}, j.e = e => Promise.all(Object.keys(j.f).reduce(((r, t) => (j.f[t](e, r), r)), [])), j.u = e => e + "." + {
         0: "99dd872e735721a05b18",
         24: "a6fec73552ceb9bdb6aa",
         66: "715eff54360a4988967a",
         113: "063bb6057d77be1f85f3",
         151: "18af1747c52fa1890fce",
         174: "7b162c87cb727f7c2712",
-        185: "c2e096475cfee897e1f9",
         211: "600bba662ff9e624e2f6",
         222: "6dffdbe65a2e7cc44707",
+        227: "bba2b52e5695cc9b34b7",
         271: "36aa2c7fc0a5419d0981",
         313: "f6abbabc37aacd77b555",
         378: "8fdd4b1246fb17037bb3",
         456: "31436070dfbf8e0b6319",
         478: "b1efc8dc1ed4a16150ef",
         554: "3ee5e631ee6f4d8c24e2",
         569: "110780388cdcc5605903",
@@ -77,17 +77,17 @@
     } [e] + ".js?v=" + {
         0: "99dd872e735721a05b18",
         24: "a6fec73552ceb9bdb6aa",
         66: "715eff54360a4988967a",
         113: "063bb6057d77be1f85f3",
         151: "18af1747c52fa1890fce",
         174: "7b162c87cb727f7c2712",
-        185: "c2e096475cfee897e1f9",
         211: "600bba662ff9e624e2f6",
         222: "6dffdbe65a2e7cc44707",
+        227: "bba2b52e5695cc9b34b7",
         271: "36aa2c7fc0a5419d0981",
         313: "f6abbabc37aacd77b555",
         378: "8fdd4b1246fb17037bb3",
         456: "31436070dfbf8e0b6319",
         478: "b1efc8dc1ed4a16150ef",
         554: "3ee5e631ee6f4d8c24e2",
         569: "110780388cdcc5605903",
@@ -107,16 +107,16 @@
             if ("object" == typeof window) return window
         }
     }(), j.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@qbraid/jupyter-environment-manager:", j.l = (t, a, n, o) => {
         if (e[t]) e[t].push(a);
         else {
             var i, d;
             if (void 0 !== n)
-                for (var c = document.getElementsByTagName("script"), f = 0; f < c.length; f++) {
-                    var l = c[f];
+                for (var f = document.getElementsByTagName("script"), c = 0; c < f.length; c++) {
+                    var l = f[c];
                     if (l.getAttribute("src") == t || l.getAttribute("data-webpack") == r + n) {
                         i = l;
                         break
                     }
                 }
             i || (d = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, j.nc && i.setAttribute("nonce", j.nc), i.setAttribute("data-webpack", r + n), i.src = t), e[t] = [a];
             var u = (r, a) => {
@@ -153,16 +153,16 @@
                             d = n[r];
                         (!d || !d.loaded && (!a != !d.eager ? a : i > d.from)) && (n[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
-                    c = [];
-                return "default" === t && (d("@aws-amplify/auth", "4.6.0", (() => Promise.all([j.e(313), j.e(151)]).then((() => () => j(8313))))), d("@emotion/react", "11.10.0", (() => Promise.all([j.e(113), j.e(271), j.e(991)]).then((() => () => j(3113))))), d("@emotion/styled", "11.10.0", (() => Promise.all([j.e(378), j.e(271), j.e(211), j.e(799)]).then((() => () => j(4378))))), d("@mui/icons-material", "5.8.4", (() => Promise.all([j.e(66), j.e(24), j.e(271), j.e(222)]).then((() => () => j(4024))))), d("@mui/material", "5.15.10", (() => Promise.all([j.e(66), j.e(909), j.e(588), j.e(271), j.e(211), j.e(222), j.e(456)]).then((() => () => j(1909))))), d("@qbraid/jupyter-environment-manager", "0.2.0-rc.9", (() => Promise.all([j.e(66), j.e(588), j.e(0), j.e(271), j.e(222), j.e(456), j.e(185)]).then((() => () => j(4185))))), d("alt", "0.17.9", (() => j.e(554).then((() => () => j(4554))))), d("react-ace", "9.5.0", (() => Promise.all([j.e(981), j.e(271), j.e(697)]).then((() => () => j(4981))))), d("superagent-use", "0.1.0", (() => j.e(174).then((() => () => j(3738))))), d("superagent", "5.3.1", (() => j.e(569).then((() => () => j(569)))))), e[t] = c.length ? Promise.all(c).then((() => e[t] = 1)) : 1
+                    f = [];
+                return "default" === t && (d("@aws-amplify/auth", "4.6.0", (() => Promise.all([j.e(313), j.e(151)]).then((() => () => j(8313))))), d("@emotion/react", "11.10.0", (() => Promise.all([j.e(113), j.e(271), j.e(991)]).then((() => () => j(3113))))), d("@emotion/styled", "11.10.0", (() => Promise.all([j.e(378), j.e(271), j.e(211), j.e(799)]).then((() => () => j(4378))))), d("@mui/icons-material", "5.8.4", (() => Promise.all([j.e(66), j.e(24), j.e(271), j.e(222)]).then((() => () => j(4024))))), d("@mui/material", "5.15.10", (() => Promise.all([j.e(66), j.e(909), j.e(588), j.e(271), j.e(211), j.e(222), j.e(456)]).then((() => () => j(1909))))), d("@qbraid/jupyter-environment-manager", "0.2.1", (() => Promise.all([j.e(66), j.e(588), j.e(0), j.e(271), j.e(222), j.e(456), j.e(227)]).then((() => () => j(3227))))), d("alt", "0.17.9", (() => j.e(554).then((() => () => j(4554))))), d("react-ace", "9.5.0", (() => Promise.all([j.e(981), j.e(271), j.e(697)]).then((() => () => j(4981))))), d("superagent-use", "0.1.0", (() => j.e(174).then((() => () => j(3738))))), d("superagent", "5.3.1", (() => j.e(569).then((() => () => j(569)))))), e[t] = f.length ? Promise.all(f).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         j.g.importScripts && (e = j.g.location + "");
         var r = j.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -197,47 +197,47 @@
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
             for (var a = 1, o = 1; o < e.length; o++) a--, t += "u" == (typeof(d = e[o]))[0] ? "-" : (a > 0 ? "." : "") + (a = 2, d);
             return t
         }
         var i = [];
         for (o = 1; o < e.length; o++) {
             var d = e[o];
-            i.push(0 === d ? "not(" + c() + ")" : 1 === d ? "(" + c() + " || " + c() + ")" : 2 === d ? i.pop() + " " + i.pop() : n(d))
+            i.push(0 === d ? "not(" + f() + ")" : 1 === d ? "(" + f() + " || " + f() + ")" : 2 === d ? i.pop() + " " + i.pop() : n(d))
         }
-        return c();
+        return f();
 
-        function c() {
+        function f() {
             return i.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var a = e[0],
                 n = a < 0;
             n && (a = -a - 1);
-            for (var i = 0, d = 1, c = !0;; d++, i++) {
-                var f, l, u = d < e.length ? (typeof e[d])[0] : "";
-                if (i >= r.length || "o" == (l = (typeof(f = r[i]))[0])) return !c || ("u" == u ? d > a && !n : "" == u != n);
+            for (var i = 0, d = 1, f = !0;; d++, i++) {
+                var c, l, u = d < e.length ? (typeof e[d])[0] : "";
+                if (i >= r.length || "o" == (l = (typeof(c = r[i]))[0])) return !f || ("u" == u ? d > a && !n : "" == u != n);
                 if ("u" == l) {
-                    if (!c || "u" != u) return !1
-                } else if (c)
+                    if (!f || "u" != u) return !1
+                } else if (f)
                     if (u == l)
                         if (d <= a) {
-                            if (f != e[d]) return !1
+                            if (c != e[d]) return !1
                         } else {
-                            if (n ? f > e[d] : f < e[d]) return !1;
-                            f != e[d] && (c = !1)
+                            if (n ? c > e[d] : c < e[d]) return !1;
+                            c != e[d] && (f = !1)
                         }
                 else if ("s" != u && "n" != u) {
                     if (n || d <= a) return !1;
-                    c = !1, d--
+                    f = !1, d--
                 } else {
                     if (d <= a || l < u != n) return !1;
-                    c = !1
-                } else "s" != u && "n" != u && (c = !1, d--)
+                    f = !1
+                } else "s" != u && "n" != u && (f = !1, d--)
             }
         }
         var s = [],
             b = s.pop.bind(s);
         for (i = 1; i < e.length; i++) {
             var p = e[i];
             s.push(1 == p ? b() | b() : 2 == p ? b() & b() : p ? o(p, r) : !b())
@@ -246,20 +246,20 @@
     }, i = (e, r) => {
         var t = j.S[e];
         if (!t || !j.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, d = (e, r) => {
         var t = e[r];
         return (r = Object.keys(t).reduce(((e, r) => !e || a(e, r) ? r : e), 0)) && t[r]
-    }, c = (e, r) => {
+    }, f = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && a(e, r) ? r : e), 0)
-    }, f = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(a) + ")", l = (e, r, t, a) => {
-        var n = c(e, t);
-        return o(a, n) || "undefined" != typeof console && console.warn && console.warn(f(e, t, n, a)), s(e[t][n])
+    }, c = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(a) + ")", l = (e, r, t, a) => {
+        var n = f(e, t);
+        return o(a, n) || "undefined" != typeof console && console.warn && console.warn(c(e, t, n, a)), s(e[t][n])
     }, u = (e, r, t) => {
         var n = e[r];
         return (r = Object.keys(n).reduce(((e, r) => !o(t, r) || e && !a(e, r) ? e : r), 0)) && n[r]
     }, s = e => (e.loaded = 1, e.get()), p = (b = e => function(r, t, a, n) {
         var o = j.I(r);
         return o && o.then ? o.then(e.bind(e, r, j.S[r], t, a, n)) : e(r, j.S[r], t, a, n)
     })(((e, r, t, a) => r && j.o(r, t) ? s(d(r, t)) : a())), h = b(((e, r, t, a) => (i(e, t), l(r, 0, t, a)))), m = b(((e, r, t, a, n) => {
@@ -280,17 +280,17 @@
         7583: () => h("default", "@jupyterlab/apputils", [1, 3, 6, 7]),
         7758: () => m("default", "@aws-amplify/auth", [1, 4, 3, 11], (() => Promise.all([j.e(313), j.e(151)]).then((() => () => j(8313))))),
         8654: () => m("default", "superagent-use", [2, 0, 1, 0], (() => j.e(174).then((() => () => j(3738))))),
         9845: () => m("default", "@mui/icons-material", [1, 5, 8, 4], (() => j.e(24).then((() => () => j(4024))))),
         5211: () => p("default", "@emotion/react", (() => Promise.all([j.e(113), j.e(478)]).then((() => () => j(3113))))),
         799: () => m("default", "@emotion/react", [1, 11, 0, 0, , "rc", 0], (() => j.e(113).then((() => () => j(3113)))))
     }, y = {
-        185: [2046, 3888, 4582, 6772, 6880, 7169, 7386, 7583, 7758, 8654, 9845],
         211: [5211],
         222: [2148, 8800],
+        227: [2046, 3888, 4582, 6772, 6880, 7169, 7386, 7583, 7758, 8654, 9845],
         271: [6271],
         456: [4456],
         799: [799]
     }, j.f.consumes = (e, r) => {
         j.o(y, e) && y[e].forEach((e => {
             if (j.o(v, e)) return r.push(v[e]);
             var t = r => {
@@ -331,20 +331,20 @@
                         i.message = "Loading chunk " + r + " failed.\n(" + n + ": " + o + ")", i.name = "ChunkLoadError", i.type = n, i.request = o, a[1](i)
                     }
                 }), "chunk-" + r, r)
             }
         };
         var r = (r, t) => {
                 var a, n, [o, i, d] = t,
-                    c = 0;
+                    f = 0;
                 if (o.some((r => 0 !== e[r]))) {
                     for (a in i) j.o(i, a) && (j.m[a] = i[a]);
                     d && d(j)
                 }
-                for (r && r(t); c < o.length; c++) n = o[c], j.o(e, n) && e[n] && e[n][0](), e[n] = 0
+                for (r && r(t); f < o.length; f++) n = o[f], j.o(e, n) && e[n] && e[n][0](), e[n] = 0
             },
             t = self.webpackChunk_qbraid_jupyter_environment_manager = self.webpackChunk_qbraid_jupyter_environment_manager || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), j.nc = void 0;
     var S = j(7413);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@qbraid/jupyter-environment-manager"] = S
 })();
```

### Comparing `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager/labextension/static/third-party-licenses.json` & `jupyter_environment_manager-0.2.1/jupyter_environment_manager/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager.egg-info/PKG-INFO` & `jupyter_environment_manager-0.2.1/jupyter_environment_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_environment_manager
-Version: 0.2.0rc9
+Version: 0.2.1
 Summary: JupyterLab extension for managing execution environments, packages, and kernels.
 Home-page: https://github.com/qBraid/qBraid-Lab
 Author: qBraid Development Team
 Author-email: contact@qbraid.com
 License: Proprietary
 Project-URL: Documentation, https://docs.qbraid.com/projects/lab/en/latest/lab/environments.html
 Project-URL: Bug Tracker, https://github.com/qBraid/qBraid-Lab/issues
```

### Comparing `jupyter_environment_manager-0.2.0rc9/jupyter_environment_manager.egg-info/SOURCES.txt` & `jupyter_environment_manager-0.2.1/jupyter_environment_manager.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 jupyter_environment_manager/labextension/static/0.99dd872e735721a05b18.js
 jupyter_environment_manager/labextension/static/0.99dd872e735721a05b18.js.LICENSE.txt
 jupyter_environment_manager/labextension/static/113.063bb6057d77be1f85f3.js
 jupyter_environment_manager/labextension/static/113.063bb6057d77be1f85f3.js.LICENSE.txt
 jupyter_environment_manager/labextension/static/151.18af1747c52fa1890fce.js
 jupyter_environment_manager/labextension/static/174.7b162c87cb727f7c2712.js
 jupyter_environment_manager/labextension/static/174.7b162c87cb727f7c2712.js.LICENSE.txt
-jupyter_environment_manager/labextension/static/185.c2e096475cfee897e1f9.js
+jupyter_environment_manager/labextension/static/227.bba2b52e5695cc9b34b7.js
 jupyter_environment_manager/labextension/static/24.a6fec73552ceb9bdb6aa.js
 jupyter_environment_manager/labextension/static/313.f6abbabc37aacd77b555.js
 jupyter_environment_manager/labextension/static/313.f6abbabc37aacd77b555.js.LICENSE.txt
 jupyter_environment_manager/labextension/static/378.8fdd4b1246fb17037bb3.js
 jupyter_environment_manager/labextension/static/478.b1efc8dc1ed4a16150ef.js
 jupyter_environment_manager/labextension/static/554.3ee5e631ee6f4d8c24e2.js
 jupyter_environment_manager/labextension/static/569.110780388cdcc5605903.js
@@ -53,15 +53,15 @@
 jupyter_environment_manager/labextension/static/747.6d49dfe38d298a9d88e1.js
 jupyter_environment_manager/labextension/static/813.4baf0234297462c92d8b.js
 jupyter_environment_manager/labextension/static/909.c50074d4e4be5aa7c06a.js
 jupyter_environment_manager/labextension/static/909.c50074d4e4be5aa7c06a.js.LICENSE.txt
 jupyter_environment_manager/labextension/static/981.f54a04f7142174f18f0d.js
 jupyter_environment_manager/labextension/static/981.f54a04f7142174f18f0d.js.LICENSE.txt
 jupyter_environment_manager/labextension/static/991.b0c652da28634799e4d5.js
-jupyter_environment_manager/labextension/static/remoteEntry.5fd255ae2892e93a3890.js
+jupyter_environment_manager/labextension/static/remoteEntry.df30dcda2252f4ea7597.js
 jupyter_environment_manager/labextension/static/style.js
 jupyter_environment_manager/labextension/static/third-party-licenses.json
 src/EnvironmentsSidebarWidget.tsx
 src/Flux.js
 src/assets.d.ts
 src/contextTypes.js
 src/global.d.ts
@@ -86,14 +86,15 @@
 src/components/EndUserAgreement.js
 src/components/EnvironmentEditor.js
 src/components/EnvironmentTile.js
 src/components/EnvironmentsSidebar.js
 src/components/Loading.js
 src/components/LogoLoader.js
 src/components/MuiStyledComponents.js
+src/components/PublishSlider.js
 src/components/UserNotFound.js
 src/stores/AuthStore.js
 src/stores/EnvironmentStore.js
 src/stores/UserStore.js
 src/utils/googleAnalytics.js
 src/utils/theme.js
 style/EnvironmentEditor.css
```

### Comparing `jupyter_environment_manager-0.2.0rc9/package.json` & `jupyter_environment_manager-0.2.1/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9782608695652174%*

 * *Differences: {"'version'": "'0.2.1'"}*

```diff
@@ -107,9 +107,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.2.0-rc.9"
+    "version": "0.2.1"
 }
```

### Comparing `jupyter_environment_manager-0.2.0rc9/pyproject.toml` & `jupyter_environment_manager-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/setup.py` & `jupyter_environment_manager-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/src/EnvironmentsSidebarWidget.tsx` & `jupyter_environment_manager-0.2.1/src/EnvironmentsSidebarWidget.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/src/Flux.js` & `jupyter_environment_manager-0.2.1/src/Flux.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/src/actions/ApiActions.js` & `jupyter_environment_manager-0.2.1/src/actions/ApiActions.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -27,15 +27,15 @@
         break;
     default:
         // For local testing, uncomment desired apiURL.
         // Before release, switch back to production URL.
         accountURL = 'https://account.qbraid.com';
         apiURL = 'https://api.qbraid.com/api';
         // apiURL = 'https://api-staging-1.qbraid.com/api';
-        // apiURL = 'http://localhost:8080/api';
+        // apiURL = 'http://localhost:3001/api';
         apiUserPool = 'qbraid';
         break;
 }
 
 export const ACCOUNT_URL = accountURL;
 export const API_URL = apiURL;
 
@@ -43,21 +43,21 @@
     const headers = {
         domain: apiUserPool
     };
 
     const user = alt.getStore('AuthStore').getState().user;
     const config = alt.getStore('UserStore').getState().config;
 
-    if (user?.signInUserSession) {
-        headers['id-token'] = user.signInUserSession.idToken.jwtToken;
-    } else if (config?.email && config?.refreshToken) {
+    if (config?.email && config?.refreshToken) {
         headers['email'] = config.email;
         headers['refresh-token'] = config.refreshToken;
     } else if (config?.apiKey) {
         headers['api-key'] = config.apiKey;
+    } else if (user?.signInUserSession) {
+        headers['id-token'] = user.signInUserSession.idToken.jwtToken;
     } else {
         const cookies = Object.fromEntries(
             document.cookie
             .split(';')
             .map(cookie => cookie.split('=').map(c => c.trim()))
         );
         const {
```

### Comparing `jupyter_environment_manager-0.2.0rc9/src/actions/AuthActions.js` & `jupyter_environment_manager-0.2.1/src/actions/AuthActions.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/src/actions/EnvironmentActions.js` & `jupyter_environment_manager-0.2.1/src/actions/EnvironmentActions.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -642,50 +642,14 @@
                     });
             } catch (err) {
                 return reject('Quantum jobs not added.');
             }
         });
     };
 
-    this.addQuantumJobs = slug => {
-        // This function is used to make a call to a JupyterAPI route that
-        // will add qbraid quantum jobs for an environment.
-        this.alt.dispatch(this);
-        return new Promise((resolve, reject) => {
-            try {
-                this.alt
-                    .getActions('JupyterApiActions')
-                    .query('quantum-jobs', {
-                        body: JSON.stringify({
-                            slug: slug
-                        }),
-                        method: 'POST'
-                    })
-                    .then(data => {
-                        if (data.success) {
-                            resolve({
-                                success: data.success,
-                                stdout: data.stdout
-                            });
-                        } else {
-                            console.log(`Failed to add quantum jobs: ${data.stderr}`);
-                            reject(data.stderr);
-                        }
-                    })
-                    .catch(err => {
-                        console.log(`Failed to add quantum jobs: ${err.message}`);
-                        reject(err);
-                    });
-            } catch (err) {
-                console.log(`Failed to add quantum jobs: ${err.message}`);
-                reject(err);
-            }
-        });
-    };
-
     this.uninstallPackagePyvenv = uninstallData => {
         // This function is used to make a call to a JupyterAPI
         // route that will uninstall a package from an environment.
         this.alt.dispatch(this);
         return new Promise((resolve, reject) => {
             let requestBody = {
                 slug: `${uninstallData.slug}`,
@@ -1011,11 +975,68 @@
                     });
             } catch (err) {
                 console.log(err);
                 reject(err);
             }
         });
     };
+
+    this.publishEnvironment = slug => {
+        this.alt.dispatch(this);
+        return new Promise((resolve, reject) => {
+            try {
+                this.alt
+                    .getActions('ApiActions')
+                    .query()
+                    .post('/environments/publish')
+                    .send({
+                        slug: slug
+                    })
+                    .then(res => {
+                        if (res?.status === 200) {
+                            resolve(res);
+                        } else {
+                            reject(res.message);
+                        }
+                    })
+                    .catch(err => {
+                        reject(err);
+                    });
+            } catch (err) {
+                console.log(err);
+                reject(err);
+            }
+        });
+    };
+
+    this.updatePublishStatus = (slug, status) => {
+        this.alt.dispatch(this);
+        return new Promise((resolve, reject) => {
+            try {
+                this.alt
+                    .getActions('ApiActions')
+                    .query()
+                    .put(`/environments/publish/status/${status}`)
+                    .send({
+                        slug: slug
+                    })
+                    .then(res => {
+                        if (res?.status === 200) {
+                            resolve(res);
+                        } else {
+                            reject(res.message);
+                        }
+                    })
+                    .catch(err => {
+                        reject(err);
+                    });
+            } catch (err) {
+                console.log(err);
+                reject(err);
+            }
+        });
+    };
+
     // END ACTION CREATORS
 }
 
 export default EnvironmentActions;
```

### Comparing `jupyter_environment_manager-0.2.0rc9/src/actions/JupyterApiActions.js` & `jupyter_environment_manager-0.2.1/src/actions/JupyterApiActions.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/src/actions/UserActions.js` & `jupyter_environment_manager-0.2.1/src/actions/UserActions.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -128,26 +128,23 @@
                 } = this.alt.getStore('UserStore').getState();
 
                 const userEmail = user?.email;
                 const configEmail = config?.email;
 
                 // Check if both emails exist and do not match
                 if (userEmail && configEmail && userEmail !== configEmail) {
-                    // Delay the alert by 3 seconds
-                    setTimeout(() => {
-                        alert(
-                            'WARNING: User Mismatch\n\n' +
-                            "The logged-in email '" +
-                            configEmail +
-                            "' does not match the email '" +
-                            userEmail +
-                            "' associated with your current session.\n\n" +
-                            'Please clear your browser cookies and refresh the page, or use a private browsing window to ensure qBraid Lab functions correctly.'
-                        );
-                    }, 3000); // 3000 milliseconds = 3 seconds
+                    console.log(
+                        'WARNING: User Mismatch\n\n' +
+                        "The logged-in email '" +
+                        configEmail +
+                        "' does not match the email '" +
+                        userEmail +
+                        "' associated with your current session.\n\n" +
+                        'Please clear your browser cookies and refresh the page, or use a private browsing window to ensure qBraid Lab functions correctly.'
+                    );
                 }
 
                 resolve({
                     status: 'Success',
                     message: 'User session verification complete.'
                 });
             } catch (error) {
```

### Comparing `jupyter_environment_manager-0.2.0rc9/src/assets/icons/BackIcon.tsx` & `jupyter_environment_manager-0.2.1/src/assets/icons/BackIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/src/assets/icons/CloseIcon.tsx` & `jupyter_environment_manager-0.2.1/src/assets/icons/CloseIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/src/assets/icons/ConfirmIcon.tsx` & `jupyter_environment_manager-0.2.1/src/assets/icons/ConfirmIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/src/assets/icons/DescriptionIcon.tsx` & `jupyter_environment_manager-0.2.1/src/assets/icons/DescriptionIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/src/assets/icons/EnvIcon.tsx` & `jupyter_environment_manager-0.2.1/src/assets/icons/EnvIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/src/assets/icons/IconString.js` & `jupyter_environment_manager-0.2.1/src/assets/icons/IconString.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/src/assets/icons/LinkIcon.tsx` & `jupyter_environment_manager-0.2.1/src/assets/icons/LinkIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/src/assets/icons/Loading.tsx` & `jupyter_environment_manager-0.2.1/src/assets/icons/Loading.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/src/assets/icons/RefreshIcon.tsx` & `jupyter_environment_manager-0.2.1/src/assets/icons/RefreshIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/src/assets/icons/SearchIcon.tsx` & `jupyter_environment_manager-0.2.1/src/assets/icons/SearchIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/src/assets/icons/UserIcon.tsx` & `jupyter_environment_manager-0.2.1/src/assets/icons/UserIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/src/assets/icons/WhiteCube.tsx` & `jupyter_environment_manager-0.2.1/src/assets/icons/WhiteCube.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/src/components/EndUserAgreement.js` & `jupyter_environment_manager-0.2.1/src/components/EndUserAgreement.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/src/components/EnvironmentEditor.js` & `jupyter_environment_manager-0.2.1/src/components/EnvironmentEditor.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -43,16 +43,20 @@
     tooltipClasses
 } from '@mui/material';
 import SearchIcon from '../assets/icons/SearchIcon';
 import WhiteCube from '../assets/icons/WhiteCube';
 import {
     AddCircleOutlined,
     AddCircleOutlineOutlined,
+    BackupTwoTone,
     Check,
     Close,
+    CloudDoneTwoTone,
+    CloudOffTwoTone,
+    CloudSyncTwoTone,
     ContentCopy,
     Edit,
     EditOff,
     InfoOutlined,
     Link,
     NotInterested,
     Refresh,
@@ -73,15 +77,18 @@
 import {
     ConfirmIcon
 } from '../assets/icons/ConfirmIcon';
 import {
     Loading
 } from '../assets/icons/Loading';
 import _ from 'lodash';
+import EnvIcon from '../assets/icons/EnvIcon';
+import PublishSlider from './PublishSlider';
 
+const PUBLISH_REQUEST_READACCESSID = '62e88a24b996354861298ab2'; // contact@qbraid.com uid
 const SHARE_ENV_PERMS_NODE = 'qbraid.environments.share';
 const RECENT_EMAIL_KEY = 'recent-email';
 const SHARE_ENV_TIMER = 2500;
 const INSTALL_ENV_PERMS_NODE = 'qbraid.environments.install';
 const QSHARP_ENV_PERMS_NODE = 'qbraid.environments.qsharp';
 const premiumEnvPermsNodeMap = {
     qsharp_b54crn: QSHARP_ENV_PERMS_NODE
@@ -196,14 +203,23 @@
             accessKey: this.props.env?.accessKey || '',
             accessKeyLoading: false,
             copyCooldown: false,
             resharePopUpContent: {
                 content: '',
                 title: '',
                 body: ''
+            },
+            publishLoading: false,
+            actionAlert: false,
+            actionAlertContext: {
+                content: '',
+                title: '',
+                body: '',
+                confirmButtonText: '',
+                cancelButtonText: ''
             }
         };
     }
 
     componentDidMount() {
         setTimeout(this.load, 1);
         if (this.props.env) {
@@ -420,14 +436,208 @@
                             type: 'error'
                         }
                     });
                 }
             });
     };
 
+    requestPublishEnvironment = () => {
+        if (!this.state.isCustom) {
+            this.setState({
+                sharePopupOpen: true,
+                sharePopupMsg: {
+                    msg: 'Only custom environment can be published',
+                    type: 'error'
+                }
+            });
+            return;
+        }
+        if (
+            this.state.uninstalling ||
+            this.state.cancelling ||
+            this.state.deleting ||
+            this.props.installing ||
+            this.props.packageInstallingEnv === this.props.env._id
+        ) {
+            this.setState({
+                sharePopupOpen: true,
+                sharePopupMsg: {
+                    msg: 'Blocked during state transition',
+                    type: 'error'
+                }
+            });
+            return;
+        }
+        this.setState({
+            publishLoading: true
+        });
+        let publishData = {
+            environmentId: this.props.env._id,
+            collabEmail: 'contact@qbraid.com',
+            overwrite: true
+        };
+        this.context
+            .getActions('EnvironmentActions')
+            .shareEnvironment(publishData)
+            .then(response => {
+                if (response.status === 200 || response.status === 202) {
+                    this.setState({
+                        sharePopupOpen: true,
+                        sharePopupMsg: {
+                            msg: 'Submitting your request! Please wait...',
+                            type: 'success'
+                        }
+                    });
+                    this.context
+                        .getActions('EnvironmentActions')
+                        .updatePublishStatus(this.props.env.slug, 'requested')
+                        .then(resp => {
+                            if (resp?.status === 200) {
+                                this.setState({
+                                    sharePopupOpen: true,
+                                    sharePopupMsg: {
+                                        msg: 'Successfully Requested to publish',
+                                        type: 'success'
+                                    }
+                                });
+                            }
+                        });
+                }
+            })
+            .then(() => {
+                this.props.flux
+                    .getActions('EnvironmentActions')
+                    .updateAll()
+                    .then(() => {
+                        this.props.updateReadUserAccessData(this.props.env._id);
+                        this.props.flux
+                            .getActions('EnvironmentActions')
+                            .registerInstalled()
+                            .then(() => {
+                                this.setState({
+                                    publishLoading: false
+                                });
+                            });
+                    });
+            })
+            .catch(error => {
+                console.warn(error);
+                this.setState({
+                    sharePopupOpen: true,
+                    sharePopupMsg: {
+                        msg: 'Request to publish failed',
+                        type: 'error'
+                    },
+                    publishLoading: false
+                });
+            });
+    };
+    denyPublishingEnvironment = () => {
+        if (!this.state.isMount) {
+            return;
+        }
+
+        if (this.state.user.email !== 'contact@qbraid.com') {
+            this.setState({
+                sharePopupOpen: true,
+                sharePopupMsg: {
+                    msg: 'Only contact@qbraid.com can deny publishing this environment',
+                    type: 'error'
+                }
+            });
+            return;
+        }
+        this.props.flux
+            .getActions('EnvironmentActions')
+            .updatePublishStatus(this.props.env.slug, 'denied')
+            .then(res => {
+                if (res.status === 200) {
+                    this.setState({
+                        sharePopupOpen: true,
+                        sharePopupMsg: {
+                            msg: 'Publishing request denied!',
+                            type: 'error'
+                        }
+                    });
+                }
+            })
+            .then(() => {
+                this.props.flux
+                    .getActions('EnvironmentActions')
+                    .updateAll()
+                    .then(() => {
+                        this.props.flux
+                            .getActions('EnvironmentActions')
+                            .registerInstalled();
+                    });
+            })
+            .catch(error => {
+                console.warn(error);
+                this.setState({
+                    sharePopupOpen: true,
+                    sharePopupMsg: {
+                        msg: 'Publish failed',
+                        type: 'error'
+                    },
+                    publishLoading: false
+                });
+            });
+    };
+
+    publishEnvironment = () => {
+        if (!this.state.isMount) {
+            return;
+        }
+        if (this.state.user.email !== 'contact@qbraid.com') {
+            this.setState({
+                sharePopupOpen: true,
+                sharePopupMsg: {
+                    msg: 'Only contact@qbraid.com can publish environment',
+                    type: 'error'
+                }
+            });
+            return;
+        }
+        this.props.flux
+            .getActions('EnvironmentActions')
+            .publishEnvironment(this.props.env.slug)
+            .then(res => {
+                if (res.status === 200) {
+                    this.setState({
+                        sharePopupOpen: true,
+                        sharePopupMsg: {
+                            msg: 'Environment published successfully',
+                            type: 'success'
+                        }
+                    });
+                }
+            })
+            .then(() => {
+                this.props.flux
+                    .getActions('EnvironmentActions')
+                    .updateAll()
+                    .then(() => {
+                        this.props.flux
+                            .getActions('EnvironmentActions')
+                            .registerInstalled();
+                    });
+            })
+            .catch(error => {
+                console.warn(error);
+                this.setState({
+                    sharePopupOpen: true,
+                    sharePopupMsg: {
+                        msg: 'Publish failed',
+                        type: 'error'
+                    },
+                    publishLoading: false
+                });
+            });
+    };
+
     toggleWriteAccess = user => {
         let {
             readAccessUsers,
             writeAccessUsers
         } = this.state;
         if (user.write) {
             // remove write access
@@ -591,26 +801,32 @@
                     pkgToAdd,
                     errMsg,
                     installMessage
                 );
                 if (response) {
                     this.updateCustomPackageListInMongo();
                 }
+                if (pkgToAdd.startsWith('amazon-braket-sdk')) {
+                    this.setState({
+                        quantumJobs: true
+                    });
+                }
             }
         } catch (err) {
             this.props.finishPackageInstalling();
             console.log(err);
             alert(errMsg);
         }
     };
 
     removePackage = pkgToRemove => {
         this.setState({
             loadingPackages: false
         });
+
         const pattern = /(==|~=|<|<=|>|>=)/;
         const name = pkgToRemove.split(pattern)[0];
         const slug = this.props.env.slug;
         if (!name || !slug) {
             alert(
                 'Failed to uninstall package: environment slug or package name not found'
             );
@@ -624,14 +840,21 @@
         return new Promise(resolve => {
             this.props.flux
                 .getActions('EnvironmentActions')
                 .uninstallPackagePyvenv(uninstallData)
                 .then(status => {
                     // only 202 is considered, other status codes need to be handled according to backend update
                     if (status === 202) {
+                        if (name === 'amazon-braket-sdk' || name === 'botocore') {
+                            this.setState({
+                                quantumJobs: false,
+                                quantumJobsEnabled: false
+                            });
+                        }
+
                         this.setState({
                             packagesInImage: this.state.packagesInImage.filter(
                                 pkg => pkg !== pkgToRemove
                             )
                         });
                         resolve(true);
                     } else {
@@ -1172,48 +1395,59 @@
         }, 2500);
     };
 
     handleQuantumJobsToggle = () => {
         if (this.state.lockedEnv) return null;
         if (this.props.env) {
             const initialJobsState = this.state.quantumJobsEnabled;
+            this.setState({
+                pkgListBusy: true
+            });
             this.context
                 .getActions('EnvironmentActions')
                 .toggleQuantumJobs({
                     slug: this.props.env.slug,
                     action: this.state.quantumJobsEnabled ? 'disable' : 'enable'
                 })
                 .then(data => {
-                    if (data.success) {
-                        this.setState({
-                            quantumJobsEnabled: !initialJobsState,
-                            qjobsStatus: {
-                                open: true,
-                                error: false,
-                                message: `${initialJobsState ? 'Disabled' : 'Enabled'}`
-                            }
-                        });
-                        this.resetQjobsStatus();
-                    }
-                    // this.context
-                    //   .getActions('EnvironmentActions')
-                    //   .registerInstalled()
-                    //   .catch(err => {
-                    //     throw new Error(err);
-                    //   });
+                    const {
+                        success
+                    } = data;
+                    const newState = {
+                        pkgListBusy: false,
+                        quantumJobsEnabled: success ? !initialJobsState : initialJobsState,
+                        qjobsStatus: {
+                            open: true,
+                            error: !success,
+                            message: success ?
+                                initialJobsState ?
+                                'Disabled' :
+                                'Enabled' :
+                                initialJobsState ?
+                                'Enabled' :
+                                'Disabled'
+                        }
+                    };
+
+                    // Set the new Quantum Jobs state
+                    this.setState(newState);
+                    this.resetQjobsStatus();
                 })
                 .catch(err => {
                     console.log('Quantum Jobs Toggle Error: ', err);
                     this.setState({
+                        pkgListBusy: false,
                         qjobsStatus: {
                             open: true,
                             error: true,
                             message: 'Error: failed to enable Quantum Jobs'
                         }
                     });
+
+                    // Reset the Quantum Jobs state
                     this.resetQjobsStatus();
                 });
         }
     };
 
     handleUninstallAlertOpen = () => {
         this.setState({
@@ -1355,47 +1589,35 @@
         );
     };
 
     renderQuantumJobsToggle = () => {
         const hasQuantumJobs = this.state.quantumJobs;
 
         const handleAddQuantumJobs = async () => {
-            try {
-                const data = await this.context
-                    .getActions('EnvironmentActions')
-                    .addQuantumJobs(this.props.env.slug);
-                if (data.success) {
+            this.addPackage('amazon-braket-sdk')
+                .then(() => {
                     this.setState({
                         quantumJobsAdditionSuccess: true
                     });
                     setTimeout(() => {
-                        this.context
-                            .getActions('EnvironmentActions')
-                            .updateAll()
-                            .then(() => {
-                                // this.context
-                                //   .getActions('EnvironmentActions')
-                                //   .registerInstalled();
-
-                                this.setState({
-                                    quantumJobsAdditionSuccess: false,
-                                    quantumJobs: true,
-                                    quantumJobsEnabled: true
-                                });
-                            });
+                        this.setState({
+                            quantumJobsAdditionSuccess: false,
+                            quantumJobs: true,
+                            quantumJobsEnabled: false
+                        });
                     }, 1750);
-                }
-            } catch (err) {
-                console.log('Error adding quantum jobs. ', err);
-                alert(
-                    'Unable to add quantum jobs at this time. ' +
-                    'Please try again later, and verify that qbraid-core ' +
-                    'is installed and configured correctly.'
-                );
-            }
+                })
+                .catch(err => {
+                    console.log('Error adding quantum jobs. ', err);
+                    alert(
+                        'Unable to add quantum jobs at this time. ' +
+                        'Please try again later, and verify that qbraid-core ' +
+                        'is installed and configured correctly.'
+                    );
+                });
         };
 
         return ( <
             Stack flexDirection = "row"
             alignItems = "center"
             flexWrap = "wrap"
             gap = {
@@ -2759,45 +2981,54 @@
             /Grid> <
             /Grid> <
             /Grid> <
             /Modal>
         );
     };
     // snack bar for share environment.
-    renderShareMsg = ({
-        msg,
-        type
-    }) => {
+    renderShareMsg = () => {
         return ( <
             Snackbar open = {
                 this.state.sharePopupOpen
             }
             autoHideDuration = {
-                SHARE_ENV_TIMER
+                2500
             }
             onClose = {
                 this.handleSharePopupClose
             }
             sx = {
                 {
                     position: 'sticky',
                     width: '300px',
-                    bottom: '10px'
+                    bottom: '10px!important',
+                    left: '40px!important'
                 }
             } >
             <
-            div className = {
-                `env-pane-msg-popup ${type} slide-in-bottom`
-            } > {
-                msg
+            Alert severity = {
+                this.state.sharePopupMsg.type
+            }
+            variant = "filled"
+            sx = {
+                {
+                    position: 'absolute',
+                    width: '100%',
+                    fontSize: '14px',
+                    bottom: '10px'
+                }
+            } >
+            {
+                this.state.sharePopupMsg.msg
             } <
-            /div> <
+            /Alert> <
             /Snackbar>
         );
     };
+
     renderCollaboratorRows = () => {
         let filterRow = [ <
             tr key = {
                 -1
             }
             style = {
                 {
@@ -3546,17 +3777,14 @@
 
         renderPopupMsg = ({
             msg,
             type
         }) => {
             return ( <
                 Snackbar open = {
-                    true
-                }
-                open = {
                     this.state.popupOpen
                 }
                 autoHideDuration = {
                     2500
                 }
                 onClose = {
                     this.handlePopupClose
@@ -3679,48 +3907,232 @@
             let displayText;
 
             if (this.state.isCustom) {
                 const createdAt = formatUTCDateTime(this.props.env.createdAt);
                 const updatedAt = formatUTCDateTime(this.props.env.updatedAt);
                 const sharedWith = this.state.readAccessUsers?.length ?? 0;
                 const sharedWithText = `${sharedWith} user${sharedWith === 1 ? '' : 's'}`;
-                displayText = `createdAt: ${createdAt} UTC\n\nupdatedAt: ${updatedAt} UTC\n\nsharedWith: ${sharedWithText}`;
+                displayText = ( <
+                    Typography fontSize = {
+                        14
+                    }
+                    color = "text.secondary" >
+                    createdAt: {
+                        createdAt
+                    }
+                    UTC <
+                    br / >
+                    updatedAt: {
+                        updatedAt
+                    }
+                    UTC <
+                    br / >
+                    sharedWith: {
+                        sharedWithText
+                    } <
+                    /Typography>
+                );
             } else if (this.props.env.canUpdate) {
-                displayText = `An updated version of the ${this.props.env.displayName} environment is available!`;
+                displayText = ( <
+                    Typography fontSize = {
+                        14
+                    }
+                    color = "text.secondary" >
+                    An updated version of the {
+                        this.props.env.displayName
+                    }
+                    environment is available!
+                    <
+                    /Typography>
+                );
             } else {
-                displayText = `Your ${this.props.env.displayName} environment is up-to-date with the latest version.`;
+                displayText = ( <
+                    Typography fontSize = {
+                        14
+                    }
+                    color = "text.secondary" >
+                    Your {
+                        this.props.env.displayName
+                    }
+                    environment is up - to - date with the latest version. <
+                    /Typography>
+                );
             }
 
             const minHeight = this.state.isInstalled ? 150 : 105;
 
+            const handleOpenAlert = () => {
+                this.setState({
+                        actionAlertContext: {
+                            content: 'publish',
+                            title: 'Confirm Environment Publish Request',
+                            body: 'Are you sure you want to submit your custom environment for review? By requesting to publish, you are agreeing to transfer ownership of your environment to qBraid. If approved, it will be made publicly available for all qBraid Lab users to install. Please confirm your submission or cancel if you wish to make any further changes.',
+                            confirmButtonText: 'Submit for Review',
+                            cancelButtonText: 'Cancel'
+                        }
+                    },
+                    () => {
+                        this.handleActionAlertOpen();
+                    }
+                );
+            };
+
             return ( <
                 Grid item xs = {
                     12
                 } >
                 <
                 div className = "env-editor-pane-new"
                 style = {
                     {
                         minHeight: minHeight
                     }
                 } >
                 <
-                div className = "env-pane-content" >
+                div className = "env-pane-content"
+                style = {
+                    {
+                        gap: '8px'
+                    }
+                } >
                 <
                 Stack direction = "row"
                 alignItems = "flex-start"
                 gap = {
                     2
                 } > {
-                    this.props.env.canUpdate ? < Update / > : < UpdateDisabled / >
-                } <
-                Typography className = "env-pane-prompt" > {
+                    this.props.env.canUpdate ? ( <
+                        Update color = "action"
+                        fontSize = "small" / >
+                    ) : ( <
+                        UpdateDisabled color = "action"
+                        fontSize = "small" / >
+                    )
+                } {
                     displayText
-                } < /Typography> <
-                /Stack> {
+                } <
+                /Stack> <
+                Grid container spacing = {
+                    1
+                } > {
+                    this.state.isMount &&
+                    this.props.env.installed && [
+                        PUBLISH_REQUEST_READACCESSID,
+                        this.props.qbUser.user._id
+                    ].includes(this.props.env.owner) && ( <
+                        >
+                        <
+                        Grid item xs = {
+                            12
+                        } >
+                        <
+                        Divider orientation = "horizontal" / >
+                        <
+                        /Grid> {
+                            this.props.env?.reviewStatus === 'pending' &&
+                                this.props.qbUser.user.email === 'contact@qbraid.com' && ( <
+                                    Grid item container xs = {
+                                        12
+                                    }
+                                    spacing = {
+                                        1
+                                    } >
+                                    <
+                                    Grid item xs = {
+                                        5
+                                    } >
+                                    <
+                                    Button fullWidth variant = "outlined"
+                                    size = "small"
+                                    color = "error"
+                                    sx = {
+                                        {
+                                            textTransform: 'none',
+                                            fontSize: 13
+                                        }
+                                    }
+                                    startIcon = {
+                                        < CloudOffTwoTone / >
+                                    }
+                                    onClick = {
+                                        this.denyPublishingEnvironment
+                                    } >
+                                    Deny Request <
+                                    /Button> <
+                                    /Grid> <
+                                    Grid item xs = {
+                                        7
+                                    } >
+                                    <
+                                    Button fullWidth variant = "contained"
+                                    size = "small"
+                                    color = "secondary"
+                                    sx = {
+                                        {
+                                            textTransform: 'none',
+                                            fontSize: 13
+                                        }
+                                    }
+                                    startIcon = {
+                                        < CloudDoneTwoTone / >
+                                    }
+                                    onClick = {
+                                        this.publishEnvironment
+                                    } >
+                                    Approve publish request <
+                                    /Button> <
+                                    /Grid> <
+                                    /Grid>
+                                )
+                        } <
+                        Grid item xs = {
+                            12
+                        } > {
+                            this.props.env.readAccessUsers.includes(
+                                PUBLISH_REQUEST_READACCESSID
+                            ) ? ( <
+                                PublishSlider env = {
+                                    this.props.env
+                                }
+                                />
+                            ) : ( <
+                                Button fullWidth variant = "contained"
+                                size = "small"
+                                color = "secondary"
+                                sx = {
+                                    {
+                                        textTransform: 'none'
+                                    }
+                                }
+                                startIcon = {
+                                    this.state.publishLoading ? ( <
+                                        CloudSyncTwoTone / >
+                                    ) : ( <
+                                        BackupTwoTone / >
+                                    )
+                                }
+                                onClick = {
+                                    handleOpenAlert
+                                }
+                                disabled = {
+                                    this.state.publishLoading
+                                } >
+                                {
+                                    this.state.publishLoading ?
+                                    'Processing publish request...' :
+                                        'Request to publish'
+                                } <
+                                /Button>
+                            )
+                        } <
+                        /Grid> <
+                        />
+                    )
+                } <
+                /Grid> {
                     this.state.uninstalling && ( <
                         Stack gap = {
                             1
                         } >
                         <
                         Typography className = "env-pane-prompt" > {
                             `Uninstalling ${this.props.env.displayName}`
@@ -3738,15 +4150,17 @@
                             }
                         }
                         /> <
                         /Stack>
                     )
                 } <
                 /div> <
-                /div> <
+                /div> {
+                    this.renderShareMsg()
+                } <
                 /Grid>
             );
         };
 
         renderDeletePane = () => {
             return ( <
                 Grid item xs = {
@@ -3872,14 +4286,111 @@
                 if applicable. <
                 /p> <
                 /div> <
                 /div> <
                 /Grid>
             );
         };
+
+        handleActionAlertOpen = () => {
+            this.setState({
+                actionAlert: true
+            });
+        };
+
+        handleActionAlertClose = () => {
+            this.setState({
+                actionAlert: false,
+                actionAlertContext: {
+                    content: '',
+                    title: '',
+                    body: '',
+                    confirmButtonText: '',
+                    cancelButtonText: ''
+                }
+            });
+        };
+
+        confirmButtonAction = () => {
+            if (this.state.actionAlertContext.content === 'publish') {
+                this.requestPublishEnvironment();
+                this.handleActionAlertClose();
+            }
+        };
+
+        cancelButtonAction = () => {
+            if (this.state.actionAlertContext.content === 'publish') {
+                this.handleActionAlertClose();
+            }
+        };
+
+        actionAlert = () => {
+            return ( <
+                Dialog open = {
+                    this.state.actionAlert
+                }
+                onClose = {
+                    this.handleActionAlertClose
+                }
+                aria - labelledby = "alert-dialog-title"
+                aria - describedby = "alert-dialog-description"
+                className = "action-alert-dialog-box"
+                transitionDuration = {
+                    100
+                } >
+                <
+                DialogTitle id = "alert-dialog-title" > {
+                    this.state.actionAlertContext.title
+                } <
+                /DialogTitle> <
+                DialogContent id = "alert-dialog-content" >
+                <
+                DialogContentText id = "alert-dialog-description" > {
+                    this.state.actionAlertContext.body
+                } <
+                /DialogContentText> <
+                /DialogContent> <
+                DialogActions id = "alert-dialog-actions" >
+                <
+                Button variant = "outlined"
+                color = "error"
+                onClick = {
+                    this.cancelButtonAction
+                }
+                sx = {
+                    {
+                        textTransform: 'none',
+                        minWidth: '120px'
+                    }
+                } >
+                {
+                    this.state.actionAlertContext.cancelButtonText
+                } <
+                /Button> <
+                Button color = "secondary"
+                variant = "contained"
+                sx = {
+                    {
+                        textTransform: 'none',
+                        minWidth: '120px'
+                    }
+                }
+                onClick = {
+                    this.confirmButtonAction
+                }
+                autoFocus disableFocusRipple >
+                {
+                    this.state.actionAlertContext.confirmButtonText
+                } <
+                /Button> <
+                /DialogActions> <
+                /Dialog>
+            );
+        };
+
         renderUninstallAlert = () => {
             return ( <
                 Dialog open = {
                     this.state.uninstallAlert
                 }
                 onClose = {
                     this.handleUninstallAlertClose
@@ -4318,17 +4829,17 @@
                         this.state.cancelling ||
                         this.state.cancelRequest ?
                         this.renderCancelInstallPane() :
                         this.renderUninstallPane()
                 } <
                 /Grid> <
                 /Grid> <
-                /DialogContent>
-
-                {
+                /DialogContent> {
+                    this.actionAlert()
+                } {
                     this.renderUninstallAlert()
                 } {
                     this.renderExtraUninsConfirmAlert()
                 } {
                     this.renderDeleteAlert()
                 } <
                 /Dialog>
```

### Comparing `jupyter_environment_manager-0.2.0rc9/src/components/EnvironmentTile.js` & `jupyter_environment_manager-0.2.1/src/components/EnvironmentTile.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -494,15 +494,17 @@
                             }
                         } > {
                             /* src=https://qbraid-static.s3.amazonaws.com/logos/xcpp.png if slug === xcpp_d6z3gv */ } <
                         img src = "https://qbraid-static.s3.amazonaws.com/python.svg" / >
                         <
                         /span> <
                         span > {
-                            `${env.packagesInImage.length} packages`
+                            `${env.packagesInImage.length} ${
+                      env.packagesInImage.length === 1 ? 'package' : 'packages'
+                    }`
                         } < /span> <
                         /p> <
                         /div>
                     )
             } <
             /div> <
             /div> <
```

### Comparing `jupyter_environment_manager-0.2.0rc9/src/components/EnvironmentsSidebar.js` & `jupyter_environment_manager-0.2.1/src/components/EnvironmentsSidebar.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -52,14 +52,15 @@
 import 'ace-builds/src-noconflict/theme-kuroir';
 import 'ace-builds/src-noconflict/theme-terminal';
 import {
     AddCircleOutline,
     FileUpload,
     FilterList,
     ReceiptLongOutlined,
+    ReceiptLongTwoTone,
     Visibility,
     VisibilityOff
 } from '@mui/icons-material';
 import {
     darkTheme,
     lightTheme
 } from '../utils/theme';
@@ -920,14 +921,24 @@
             if (installTime) {
                 this.setState({
                     progress: 10,
                     timeToInstall: installTime
                 });
                 this.registerInstalled(env, installTime);
             }
+            if (env?.reviewStatus === 'requested') {
+                let {
+                    user
+                } = this.props.flux.getStore('UserStore').getState();
+                if (user.email === 'contact@qbraid.com') {
+                    this.props.flux
+                        .getActions('EnvironmentActions')
+                        .updatePublishStatus(env.slug, 'pending');
+                }
+            }
         } catch (err) {
             console.log(`Error: ${err}`);
             return alert(
                 'Your environment ' +
                 env.displayName +
                 ' could not be installed at this time.'
             );
@@ -2074,14 +2085,20 @@
                 this.handleOpenPopup(err?.response?.body?.message, 'error');
                 this.setState({
                     accessCodeLoading: false
                 });
             });
     };
 
+    handleOpenDocs = () => {
+        if (this.props.app) {
+            this.props.app.commands.execute('docs:qbraid-env-manager');
+        }
+    };
+
     // Shows the list of all public packages that are not installed
     renderUninstalledEnvironments = () => {
         let envs =
             this.state.filterQuery || this.state.tagFilter ?
             this.state.filteredEnvironments :
             this.state.environments;
         envs.sort((a, b) => this.compareEnvs(a, b));
@@ -2394,21 +2411,25 @@
                         this.closeEnvironmentBrowser
                     } >
                     <
                     span className = "environments-sidebar-left-arrow" > ‹ < /span>
                     Browse Environments <
                     /div>
                 ) : ( <
-                    div style = {
+                    Box display = "inline-flex"
+                    alignItems = "center"
+                    gap = {
+                        0.5
+                    }
+                    sx = {
                         {
-                            lineHeight: '20px',
-                            display: 'inline-flex'
+                            lineHeight: '20px'
                         }
                     } >
-                    My Environments <
+                    Environments <
                     div style = {
                         {
                             transition: 'transform 1s',
                             transform: `rotateZ(${`${
                         this.state.togglesCount * 180
                       }deg`})`
                         }
@@ -2420,15 +2441,34 @@
                         })
                     }
                     className = "div-refresh-btn" >
                     <
                     RefreshIcon / >
                     <
                     /div> <
-                    /div>
+                    Tooltip title = "Read Environment Manager docs"
+                    arrow >
+                    <
+                    IconButton size = "small"
+                    color = "primary"
+                    sx = {
+                        {
+                            ml: 0.5
+                        }
+                    }
+                    onClick = {
+                        this.handleOpenDocs
+                    } >
+                    <
+                    ReceiptLongTwoTone color = "inherit"
+                    fontSize = "inherit" / >
+                    <
+                    /IconButton> <
+                    /Tooltip> <
+                    /Box>
                 )
             } <
             /span> <
             span className = "environments-sidebar-add-btn"
             style = {
                 this.state.browsing ?
                 {
```

### Comparing `jupyter_environment_manager-0.2.0rc9/src/components/Loading.js` & `jupyter_environment_manager-0.2.1/src/components/Loading.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/src/components/LogoLoader.js` & `jupyter_environment_manager-0.2.1/src/components/LogoLoader.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/src/components/MuiStyledComponents.js` & `jupyter_environment_manager-0.2.1/src/components/MuiStyledComponents.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/src/components/UserNotFound.js` & `jupyter_environment_manager-0.2.1/src/components/UserNotFound.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/src/index.ts` & `jupyter_environment_manager-0.2.1/src/index.ts`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 import {
   JupyterFrontEnd,
   JupyterFrontEndPlugin
 } from '@jupyterlab/application';
 
-import { ICommandPalette } from '@jupyterlab/apputils';
+import {
+  ICommandPalette,
+  IFrame,
+  MainAreaWidget,
+  WidgetTracker
+} from '@jupyterlab/apputils';
 import svgString from './assets/icons/IconString';
 import { LabIcon } from '@jupyterlab/ui-components';
 import { EnvironmentsSidebarWidget } from './EnvironmentsSidebarWidget';
 import Flux from './Flux';
 import { API_URL } from './actions/ApiActions';
 
 const envsIcon = new LabIcon({
@@ -27,15 +32,15 @@
   return envsSidebarWidget;
 };
 
 const extension: JupyterFrontEndPlugin<void> = {
   id: '@qbraid/jupyter-environment-manager',
   autoStart: true,
   activate: async (app: JupyterFrontEnd, palette: ICommandPalette) => {
-    const { commands } = app;
+    const { commands, shell } = app;
 
     const flux = new Flux({
       apiBaseUrl: API_URL,
       jupyterlab: app
     });
     try {
       const authActions = flux.getActions('AuthActions');
@@ -113,16 +118,61 @@
 
       if (palette) {
         palette.addItem({
           command: cmdCloseEnvironmentsSidebar,
           category: 'qBraid Ecosystem',
           args: { origin: 'from the palette' }
         });
-        // END environments sidebar widget
       }
+      // END environments sidebar widget
+
+      // function returns a widget that creates a browser sandbox inside jupyter lab
+      const browserSandboxWidget = (
+        url: string,
+        text: string
+      ): MainAreaWidget<IFrame> => {
+        const content = new IFrame({
+          sandbox: [
+            'allow-scripts',
+            'allow-forms',
+            'allow-same-origin',
+            'allow-presentation',
+            'allow-top-navigation',
+            'allow-storage-access-by-user-activation'
+          ]
+        });
+        content.url = url;
+        content.title.label = text;
+        content.title.icon = envsIcon;
+        content.title.iconClass = 'env-manager_browser-icon-parent';
+        content.id = `${namespace} - ${++counter}`;
+        const widget = new MainAreaWidget({ content });
+        return widget;
+      };
+
+      const namespace = 'qbraid-docs';
+      let counter = 0;
+      const tracker = new WidgetTracker<MainAreaWidget<IFrame>>({
+        namespace
+      });
+
+      // Opens quantum device docs inside jupyter lab inbuild browser
+      const cmdEnvMangerDocsReference = 'docs:qbraid-env-manager';
+      commands.addCommand(cmdEnvMangerDocsReference, {
+        label: 'qbraid environment manager reference',
+        execute: () => {
+          const url =
+            'https://docs.qbraid.com/projects/lab/en/latest/lab/environments.html';
+          const text = 'Environment manager';
+          const widget = browserSandboxWidget(url, text);
+          void tracker.add(widget);
+          shell.add(widget, 'main');
+          return widget;
+        }
+      });
     } catch (err) {
       console.log('\n[!] Failed to activate environment-manager [!]\n');
       console.error(err);
     }
   }
 };
```

### Comparing `jupyter_environment_manager-0.2.0rc9/src/stores/AuthStore.js` & `jupyter_environment_manager-0.2.1/src/stores/AuthStore.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/src/stores/EnvironmentStore.js` & `jupyter_environment_manager-0.2.1/src/stores/EnvironmentStore.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/src/stores/UserStore.js` & `jupyter_environment_manager-0.2.1/src/stores/UserStore.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/src/utils/googleAnalytics.js` & `jupyter_environment_manager-0.2.1/src/utils/googleAnalytics.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/src/utils/theme.js` & `jupyter_environment_manager-0.2.1/src/utils/theme.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/style/EnvironmentEditor.css` & `jupyter_environment_manager-0.2.1/style/EnvironmentEditor.css`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/style/EnvironmentTile.css` & `jupyter_environment_manager-0.2.1/style/EnvironmentTile.css`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/style/EnvironmentsSidebar.css` & `jupyter_environment_manager-0.2.1/style/EnvironmentsSidebar.css`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,16 @@
 .env_icon_parent {
   transition: none !important;
   transform: rotate(0deg) !important;
 }
 body[data-jp-theme-light='true'] .env_icon {
   filter: invert(0.6);
 }
-.env_icon {
+
+.env_icon_parent .env_icon {
   width: 30px;
   height: 30px;
   min-width: 30px;
   min-height: 30px;
   margin-top: 5px !important;
 }
 /* this class is for the right side bar list item for environment manger extesion
@@ -77,14 +78,18 @@
 
 .environments-sidebar-header {
   padding: 15px 10px;
   color: #d30982;
   font-weight: 600;
   text-transform: uppercase;
   letter-spacing: 1px;
+  display: flex;
+  flex-direction: row;
+  align-items: center;
+  justify-content: space-between;
 }
 
 .environments-sidebar-spacer {
   width: 100%;
   height: var(--jp-border-width);
   background-color: var(--jp-border-color2);
 }
```

### Comparing `jupyter_environment_manager-0.2.0rc9/style/Loading.css` & `jupyter_environment_manager-0.2.1/style/Loading.css`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/style/LogoLoader.css` & `jupyter_environment_manager-0.2.1/style/LogoLoader.css`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/tools/create_dev_build.sh` & `jupyter_environment_manager-0.2.1/tools/create_dev_build.sh`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/tsconfig.json` & `jupyter_environment_manager-0.2.1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc9/yarn.lock` & `jupyter_environment_manager-0.2.1/yarn.lock`

 * *Files identical despite different names*

