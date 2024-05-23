# Comparing `tmp/cocoro-0.1.4.tar.gz` & `tmp/cocoro-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cocoro-0.1.4.tar", last modified: Tue Feb 23 19:45:10 2021, max compression
+gzip compressed data, was "cocoro-0.1.5.tar", max compression
```

## Comparing `cocoro-0.1.4.tar` & `cocoro-0.1.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2021-02-23 02:35:21.204748 cocoro-0.1.4/LICENSE
--rw-r--r--   0        0        0     4653 2021-02-23 19:40:57.394748 cocoro-0.1.4/README.md
--rw-r--r--   0        0        0      590 2021-02-23 14:32:22.654749 cocoro-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      112 2021-02-23 05:54:31.414749 cocoro-0.1.4/src/cocoro/__init__.py
--rw-r--r--   0        0        0       87 2021-02-23 02:35:21.204748 cocoro-0.1.4/src/cocoro/__main__.py
--rw-r--r--   0        0        0       22 2021-02-23 14:32:10.904749 cocoro-0.1.4/src/cocoro/__version__.py
--rw-r--r--   0        0        0     1455 2021-02-23 19:44:15.324748 cocoro-0.1.4/src/cocoro/cli.py
--rw-r--r--   0        0        0     9524 2021-02-23 19:40:06.484748 cocoro-0.1.4/src/cocoro/core.py
--rw-r--r--   0        0        0     5644 2021-02-23 19:45:10.847363 cocoro-0.1.4/setup.py
--rw-r--r--   0        0        0     5434 2021-02-23 19:45:10.847702 cocoro-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11355 2023-09-05 06:55:16.011506 cocoro-0.1.5/LICENSE
+-rw-r--r--   0        0        0     4699 2023-09-05 06:55:16.012062 cocoro-0.1.5/README.md
+-rw-r--r--   0        0        0      592 2024-05-23 00:19:36.708439 cocoro-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      112 2023-09-05 06:55:16.014693 cocoro-0.1.5/src/cocoro/__init__.py
+-rw-r--r--   0        0        0       87 2023-09-05 06:55:16.014852 cocoro-0.1.5/src/cocoro/__main__.py
+-rw-r--r--   0        0        0       22 2023-09-05 06:55:16.015014 cocoro-0.1.5/src/cocoro/__version__.py
+-rw-r--r--   0        0        0     1455 2023-09-05 06:55:16.015200 cocoro-0.1.5/src/cocoro/cli.py
+-rw-r--r--   0        0        0     9524 2023-09-05 06:55:16.015440 cocoro-0.1.5/src/cocoro/core.py
+-rw-r--r--   0        0        0        0 2024-05-23 00:19:21.213333 cocoro-0.1.5/src/cocoro/py.typed
+-rw-r--r--   0        0        0     5533 1970-01-01 00:00:00.000000 cocoro-0.1.5/PKG-INFO
```

### Comparing `cocoro-0.1.4/LICENSE` & `cocoro-0.1.5/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright [yyyy] [name of copyright owner]
+   Copyright 2021 rcmdnk <rcmdnk@gmail.com>
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `cocoro-0.1.4/README.md` & `cocoro-0.1.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,16 @@
 
 
     POST https://hms.cloudlabs.sharp.co.jp/hems/pfApi/ta/setting/login/?appSecret=XXXXXXXXX…
            ← 200 application/json 38b 308ms
 
 Open this command and you will see following in `Request tab:
 
+![pic](https://github.com/rcmdnk/cocoro/blob/main/pic/getcookie.jpg?raw=true)
+
 
     2021-02-21 21:55:40 POST https://hms.cloudlabs.sharp.co.jp/hems/pfApi/ta/setting/login/?app
                              Secret=<*************appSecret**********************>&serviceName=
                              iClub
                              ← 200 OK application/json 38b 308ms
                 Request                         Response                        Detail
     Host:             hms.cloudlabs.sharp.co.jp
@@ -84,15 +86,15 @@
 Available commands (`<cmd>`) are:
 
 * `switch <target>`: Control switch. Available targets: `on`, `off`.
 * `humidification <target>`: Control humidification. Available targets: `on`, `off`.
 * `humi <target>`  : Alias of humidification.
 * `mode <target>`  : Control mode. Available targets: `auto`, `sleep`, `pollen`,
                      `quiet`, `medium`, `high`, `recommendation`, `effective`
-* `info [key]      : Show the appliance information. The available keys are:
+* `info [key]`     : Show the appliance information. The available keys are:
                      `full`(full echonetData), `labelData`, `maker`, `model`,
                      `deviceType`, `name`, `place`, `yomi`, `zipCd`
                      If no key is give, labelData is shown.
 * `version`: Show   version.
 * `help`: Show help.
 
 Other options:
@@ -102,19 +104,19 @@
 * `--terminalAppIdKey <terminalAppIdKey>`: Set terminalAppIdKey (overwrite the value of config_file).
 * `--name <name>`: Set name of the device. If no name is given, the first device is used.
 * `--log_level <level>`: Set log level. The available levels are: `debug`, `info`, `warning` `fatal`.
 
 
 ## Examples
 
-    $ poetry run cocoro switch on
+    $ cocoro switch on
     [INFO][Cocoro] Succeeded to control js50: switch on
-    $ poetry run cocoro humi off
+    $ cocoro humi off
     [INFO][Cocoro] Succeeded to control js50: humidification off
-    $ poetry run cocoro mode auto
+    $ cocoro mode auto
     [INFO][Cocoro] Succeeded to control js50: mode auto
 
 
     $ cocoro info
     [INFO][Cocoro] Device information
     {'id': 123456, 'place': 'リビング', 'name': 'my js50', 'deviceType': 'AIR_CLEANER', 'zipCd': '7890123', 'yomi': '', 'lSubInfo': '{"room_data":{"size": 10.0, "struct": "prefab", "unit": "tatami"}}'}
     $ cocoro info model --log_level=warning
```

### Comparing `cocoro-0.1.4/pyproject.toml` & `cocoro-0.1.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "cocoro"
-version = "0.1.4"
+version = "0.1.5"
 description = "Utilities to use Sharp, COCORO API"
 authors = ["rcmdnk <rcmdnk@gmail.com>"]
 repository = "https://github.com/rcmdnk/cocoro"
 homepage = "https://github.com/rcmdnk/cocoro"
 readme = "README.md"
 license = "Apache-2.0"
 keywords = ['Sharp', 'API']
 
 [tool.poetry.dependencies]
-python = "^3.6"
-fire = "^0.4.0"
+python = "^3.8"
+fire = "^0.5.0"
 requests = "^2.25.1"
-PyYAML = "^5.4.1"
+PyYAML = "^6.0.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^5.2"
+pytest = "^8.0.0"
 
 [tool.poetry.scripts]
 cocoro = "cocoro:main"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `cocoro-0.1.4/src/cocoro/cli.py` & `cocoro-0.1.5/src/cocoro/cli.py`

 * *Files identical despite different names*

### Comparing `cocoro-0.1.4/src/cocoro/core.py` & `cocoro-0.1.5/src/cocoro/core.py`

 * *Files identical despite different names*

### Comparing `cocoro-0.1.4/setup.py` & `cocoro-0.1.5/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,149 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: cocoro
+Version: 0.1.5
+Summary: Utilities to use Sharp, COCORO API
+Home-page: https://github.com/rcmdnk/cocoro
+License: Apache-2.0
+Keywords: Sharp,API
+Author: rcmdnk
+Author-email: rcmdnk@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: PyYAML (>=6.0.0,<7.0.0)
+Requires-Dist: fire (>=0.5.0,<0.6.0)
+Requires-Dist: requests (>=2.25.1,<3.0.0)
+Project-URL: Repository, https://github.com/rcmdnk/cocoro
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+# cocoro
 
-packages = \
-['cocoro']
+[![PyPI version](https://badge.fury.io/py/cocoro.svg)](https://badge.fury.io/py/cocoro)
+[![COCORO test](https://github.com/rcmdnk/cocoro/actions/workflows/cocoro-test.yml/badge.svg)](https://github.com/rcmdnk/cocoro/actions/workflows/cocoro-test.yml)
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['PyYAML>=5.4.1,<6.0.0', 'fire>=0.4.0,<0.5.0', 'requests>=2.25.1,<3.0.0']
-
-entry_points = \
-{'console_scripts': ['cocoro = cocoro:main']}
-
-setup_kwargs = {
-    'name': 'cocoro',
-    'version': '0.1.4',
-    'description': 'Utilities to use Sharp, COCORO API',
-    'long_description': '# cocoro\n\n[![PyPI version](https://badge.fury.io/py/cocoro.svg)](https://badge.fury.io/py/cocoro)\n[![COCORO test](https://github.com/rcmdnk/cocoro/actions/workflows/cocoro-test.yml/badge.svg)](https://github.com/rcmdnk/cocoro/actions/workflows/cocoro-test.yml)\n\nTools for COCORO API (SHARP products).\n\n## Install and Usage\n\n### Using pip\n\n    $ pip install cocoro\n\n### Using source code\n\nUse poetry to setup the environment.\n\n    $ pip install poetry\n    $ git clone https://github.com/rcmdnk/cocoro.git\n    $ cd cocoro\n    $ poetry install\n\n## Appliances\n\nAPI commands were taken for Sharp, KI-JS50 (humidifying air purifier, [KI-JS50 加湿空気清浄機/空気清浄機：シャープ](https://jp.sharp/kuusei/products/kijs50/)).\n\nIt may work for other (humidifying) air purifiers.\n\n## Requirement\n\nYou need to get `appSecret` and `terminalAppIdKey` to control appliances.\n\nTo get them, you can use [mitmproxy](https://mitmproxy.org/).\n\nBy using mitmproxy, you will see following `POST` command while you are controlling COCORO in your smart phone:\n\n\n    POST https://hms.cloudlabs.sharp.co.jp/hems/pfApi/ta/setting/login/?appSecret=XXXXXXXXX…\n           ← 200 application/json 38b 308ms\n\nOpen this command and you will see following in `Request tab:\n\n\n    2021-02-21 21:55:40 POST https://hms.cloudlabs.sharp.co.jp/hems/pfApi/ta/setting/login/?app\n                             Secret=<*************appSecret**********************>&serviceName=\n                             iClub\n                             ← 200 OK application/json 38b 308ms\n                Request                         Response                        Detail\n    Host:             hms.cloudlabs.sharp.co.jp\n    Content-Type:     application/json; charset=utf-8\n    Connection:       keep-alive\n    Accept:           */*\n    User-Agent:       smartlink_v200i Mozilla/5.0 (iPhone; CPU iPhone OS 14_4 like Mac OS X)\n                      AppleWebKit/605.1.15 (KHTML, like Gecko) Mobile/15E148\n    Content-Length:   110\n    Accept-Language:  ja-jp\n    Accept-Encoding:  gzip, deflate, br\n    JSON                                                                                  [m:auto]\n    {\n        "terminalAppId":\n    "https://db.cloudlabs.sharp.co.jp/clpf/key/<************terminalAppIdKey*************>"\n    }\n\nFind `appSecret` and `terminalAppIdKey` values from above details.\n\nThen, make following configuration file as **~/.config/cocoro/config.yml**:\n\n```yml\n---\nappSecret: <*************appSecret**********************>\nterminalAppIdKey: <************terminalAppIdKey*************>\n```\n\n## Usage\n\nIf you installed cocoro by `pip`, do:\n\n    $ cocoro <cmd> [options]\n\nIf you installed from source code, go to cocoro directory, then do:\n\n    $ poetry run cocoro <cmd> [options]\n\nAvailable commands (`<cmd>`) are:\n\n* `switch <target>`: Control switch. Available targets: `on`, `off`.\n* `humidification <target>`: Control humidification. Available targets: `on`, `off`.\n* `humi <target>`  : Alias of humidification.\n* `mode <target>`  : Control mode. Available targets: `auto`, `sleep`, `pollen`,\n                     `quiet`, `medium`, `high`, `recommendation`, `effective`\n* `info [key]      : Show the appliance information. The available keys are:\n                     `full`(full echonetData), `labelData`, `maker`, `model`,\n                     `deviceType`, `name`, `place`, `yomi`, `zipCd`\n                     If no key is give, labelData is shown.\n* `version`: Show   version.\n* `help`: Show help.\n\nOther options:\n\n* `--config_file <file>`: Set configuration file. Default file path is `~/.config/cocoro/config.yml`.\n* `--appSecret <appSecret>`: Set appSecret (overwrite the value of config_file).\n* `--terminalAppIdKey <terminalAppIdKey>`: Set terminalAppIdKey (overwrite the value of config_file).\n* `--name <name>`: Set name of the device. If no name is given, the first device is used.\n* `--log_level <level>`: Set log level. The available levels are: `debug`, `info`, `warning` `fatal`.\n\n\n## Examples\n\n    $ poetry run cocoro switch on\n    [INFO][Cocoro] Succeeded to control js50: switch on\n    $ poetry run cocoro humi off\n    [INFO][Cocoro] Succeeded to control js50: humidification off\n    $ poetry run cocoro mode auto\n    [INFO][Cocoro] Succeeded to control js50: mode auto\n\n\n    $ cocoro info\n    [INFO][Cocoro] Device information\n    {\'id\': 123456, \'place\': \'リビング\', \'name\': \'my js50\', \'deviceType\': \'AIR_CLEANER\', \'zipCd\': \'7890123\', \'yomi\': \'\', \'lSubInfo\': \'{"room_data":{"size": 10.0, "struct": "prefab", "unit": "tatami"}}\'}\n    $ cocoro info model --log_level=warning\n    KIJS50\n    $ cocoro info maker --log_level=warning\n    SHARP\n',
-    'author': 'rcmdnk',
-    'author_email': 'rcmdnk@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/rcmdnk/cocoro',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.6,<4.0',
-}
+Tools for COCORO API (SHARP products).
 
+## Install and Usage
+
+### Using pip
+
+    $ pip install cocoro
+
+### Using source code
+
+Use poetry to setup the environment.
+
+    $ pip install poetry
+    $ git clone https://github.com/rcmdnk/cocoro.git
+    $ cd cocoro
+    $ poetry install
+
+## Appliances
+
+API commands were taken for Sharp, KI-JS50 (humidifying air purifier, [KI-JS50 加湿空気清浄機/空気清浄機：シャープ](https://jp.sharp/kuusei/products/kijs50/)).
+
+It may work for other (humidifying) air purifiers.
+
+## Requirement
+
+You need to get `appSecret` and `terminalAppIdKey` to control appliances.
+
+To get them, you can use [mitmproxy](https://mitmproxy.org/).
+
+By using mitmproxy, you will see following `POST` command while you are controlling COCORO in your smart phone:
+
+
+    POST https://hms.cloudlabs.sharp.co.jp/hems/pfApi/ta/setting/login/?appSecret=XXXXXXXXX…
+           ← 200 application/json 38b 308ms
+
+Open this command and you will see following in `Request tab:
+
+![pic](https://github.com/rcmdnk/cocoro/blob/main/pic/getcookie.jpg?raw=true)
+
+
+    2021-02-21 21:55:40 POST https://hms.cloudlabs.sharp.co.jp/hems/pfApi/ta/setting/login/?app
+                             Secret=<*************appSecret**********************>&serviceName=
+                             iClub
+                             ← 200 OK application/json 38b 308ms
+                Request                         Response                        Detail
+    Host:             hms.cloudlabs.sharp.co.jp
+    Content-Type:     application/json; charset=utf-8
+    Connection:       keep-alive
+    Accept:           */*
+    User-Agent:       smartlink_v200i Mozilla/5.0 (iPhone; CPU iPhone OS 14_4 like Mac OS X)
+                      AppleWebKit/605.1.15 (KHTML, like Gecko) Mobile/15E148
+    Content-Length:   110
+    Accept-Language:  ja-jp
+    Accept-Encoding:  gzip, deflate, br
+    JSON                                                                                  [m:auto]
+    {
+        "terminalAppId":
+    "https://db.cloudlabs.sharp.co.jp/clpf/key/<************terminalAppIdKey*************>"
+    }
+
+Find `appSecret` and `terminalAppIdKey` values from above details.
+
+Then, make following configuration file as **~/.config/cocoro/config.yml**:
+
+```yml
+---
+appSecret: <*************appSecret**********************>
+terminalAppIdKey: <************terminalAppIdKey*************>
+```
+
+## Usage
+
+If you installed cocoro by `pip`, do:
+
+    $ cocoro <cmd> [options]
+
+If you installed from source code, go to cocoro directory, then do:
+
+    $ poetry run cocoro <cmd> [options]
+
+Available commands (`<cmd>`) are:
+
+* `switch <target>`: Control switch. Available targets: `on`, `off`.
+* `humidification <target>`: Control humidification. Available targets: `on`, `off`.
+* `humi <target>`  : Alias of humidification.
+* `mode <target>`  : Control mode. Available targets: `auto`, `sleep`, `pollen`,
+                     `quiet`, `medium`, `high`, `recommendation`, `effective`
+* `info [key]`     : Show the appliance information. The available keys are:
+                     `full`(full echonetData), `labelData`, `maker`, `model`,
+                     `deviceType`, `name`, `place`, `yomi`, `zipCd`
+                     If no key is give, labelData is shown.
+* `version`: Show   version.
+* `help`: Show help.
+
+Other options:
+
+* `--config_file <file>`: Set configuration file. Default file path is `~/.config/cocoro/config.yml`.
+* `--appSecret <appSecret>`: Set appSecret (overwrite the value of config_file).
+* `--terminalAppIdKey <terminalAppIdKey>`: Set terminalAppIdKey (overwrite the value of config_file).
+* `--name <name>`: Set name of the device. If no name is given, the first device is used.
+* `--log_level <level>`: Set log level. The available levels are: `debug`, `info`, `warning` `fatal`.
+
+
+## Examples
+
+    $ cocoro switch on
+    [INFO][Cocoro] Succeeded to control js50: switch on
+    $ cocoro humi off
+    [INFO][Cocoro] Succeeded to control js50: humidification off
+    $ cocoro mode auto
+    [INFO][Cocoro] Succeeded to control js50: mode auto
+
+
+    $ cocoro info
+    [INFO][Cocoro] Device information
+    {'id': 123456, 'place': 'リビング', 'name': 'my js50', 'deviceType': 'AIR_CLEANER', 'zipCd': '7890123', 'yomi': '', 'lSubInfo': '{"room_data":{"size": 10.0, "struct": "prefab", "unit": "tatami"}}'}
+    $ cocoro info model --log_level=warning
+    KIJS50
+    $ cocoro info maker --log_level=warning
+    SHARP
 
-setup(**setup_kwargs)
```

