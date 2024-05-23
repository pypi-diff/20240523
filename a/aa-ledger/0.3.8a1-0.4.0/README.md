# Comparing `tmp/aa_ledger-0.3.8a1.tar.gz` & `tmp/aa_ledger-0.4.0.tar.gz`

## Comparing `aa_ledger-0.3.8a1.tar` & `aa_ledger-0.4.0.tar`

### file list

```diff
@@ -1,79 +1,80 @@
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/__init__.py
--rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/admin.py
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/app_settings.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/apps.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/auth_hooks.py
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/decorators.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/errors.py
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/hooks.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/providers.py
--rw-r--r--   0        0        0     4956 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/tasks.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/urls.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/api/__init__.py
--rw-r--r--   0        0        0     7185 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/api/helpers.py
--rw-r--r--   0        0        0    21348 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/api/ledgermanager.py
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/api/schema.py
--rw-r--r--   0        0        0    16190 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/api/templatemanager.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/api/character/__init__.py
--rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/api/character/ledger.py
--rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/api/character/template.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/api/corporation/__init__.py
--rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/api/corporation/ledger.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/api/corporation/template.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/managers/charaudit_manager.py
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/managers/corpaudit_manager.py
--rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/managers/general_manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/migrations/__init__.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/models/__init__.py
--rw-r--r--   0        0        0     5771 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/models/characteraudit.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/models/corporationaudit.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/models/events.py
--rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/models/general.py
--rw-r--r--   0        0        0     5416 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/static/ledger/css/billboards_dark.css
--rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/static/ledger/css/cards.css
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/static/ledger/css/custom.css
--rw-r--r--   0        0        0   236145 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/static/ledger/guides/ledger-1.png
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/static/ledger/guides/ledger-2.png
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/static/ledger/guides/ledger-3.png
--rw-r--r--   0        0        0    43262 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/static/ledger/images/Spinner-1s-64px-dark.gif
--rw-r--r--   0        0        0    43381 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/static/ledger/images/Spinner-1s-64px-light.gif
--rw-r--r--   0        0        0    22096 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/static/ledger/js/charledger.js
--rw-r--r--   0        0        0    18853 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/static/ledger/js/corpledger.js
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/static/ledger/js/img.js
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/task_helpers/__init__.py
--rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/task_helpers/char_helpers.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/task_helpers/core_helpers.py
--rw-r--r--   0        0        0     8398 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/task_helpers/corp_helpers.py
--rw-r--r--   0        0        0     8434 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/task_helpers/etag_helpers.py
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/templates/ledger/base.html
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/templates/ledger/error.html
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/templates/ledger/bundles/ledger-css.html
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/templates/ledger/ledger/base.html
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/templates/ledger/ledger/index.html
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/templates/ledger/ledger/menu.html
--rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/templates/ledger/ledger/charledger/char_ledger.html
--rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/templates/ledger/ledger/charledger/month.html
--rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/templates/ledger/ledger/charledger/year.html
--rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/templates/ledger/ledger/corpledger/corp_ledger.html
--rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/templates/ledger/ledger/corpledger/month.html
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/templates/ledger/ledger/corpledger/year.html
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/templates/ledger/modals/modal-full.html
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/templates/ledger/modals/modal-xl.html
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/templates/ledger/modals/modal.html
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/templates/ledger/modals/modal_dialog.html
--rw-r--r--   0        0        0    17677 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/templates/ledger/modals/pve/view_character_content.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/templatetags/__init__.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/templatetags/ledger.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/view_helpers/__init__.py
--rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/view_helpers/core.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/views/__init__.py
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/views/pve.py
--rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/views/character/char_audit.py
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/views/corporation/corp_audit.py
--rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/views/corporation/corp_events.py
--rw-r--r--   0        0        0     8919 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/views/corporation/corp_tax.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/LICENSE
--rw-r--r--   0        0        0     5523 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/README.md
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/pyproject.toml
--rw-r--r--   0        0        0     8314 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/PKG-INFO
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/__init__.py
+-rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/admin.py
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/app_settings.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/apps.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/auth_hooks.py
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/decorators.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/errors.py
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/hooks.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/providers.py
+-rw-r--r--   0        0        0     4956 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/tasks.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/urls.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/api/__init__.py
+-rw-r--r--   0        0        0     7470 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/api/helpers.py
+-rw-r--r--   0        0        0    22614 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/api/ledgermanager.py
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/api/schema.py
+-rw-r--r--   0        0        0    16190 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/api/templatemanager.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/api/character/__init__.py
+-rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/api/character/ledger.py
+-rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/api/character/template.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/api/corporation/__init__.py
+-rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/api/corporation/ledger.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/api/corporation/template.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/locate/__init__.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/locate/de.po
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/managers/charaudit_manager.py
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/managers/corpaudit_manager.py
+-rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/managers/general_manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/migrations/__init__.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/models/__init__.py
+-rw-r--r--   0        0        0     5771 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/models/characteraudit.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/models/corporationaudit.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/models/events.py
+-rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/models/general.py
+-rw-r--r--   0        0        0     5416 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/static/ledger/css/billboards_dark.css
+-rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/static/ledger/css/cards.css
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/static/ledger/css/custom.css
+-rw-r--r--   0        0        0   236145 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/static/ledger/guides/ledger-1.png
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/static/ledger/guides/ledger-2.png
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/static/ledger/guides/ledger-3.png
+-rw-r--r--   0        0        0    43262 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/static/ledger/images/Spinner-1s-64px-dark.gif
+-rw-r--r--   0        0        0    43381 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/static/ledger/images/Spinner-1s-64px-light.gif
+-rw-r--r--   0        0        0    22096 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/static/ledger/js/charledger.js
+-rw-r--r--   0        0        0    18853 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/static/ledger/js/corpledger.js
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/static/ledger/js/img.js
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/task_helpers/__init__.py
+-rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/task_helpers/char_helpers.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/task_helpers/core_helpers.py
+-rw-r--r--   0        0        0     8398 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/task_helpers/corp_helpers.py
+-rw-r--r--   0        0        0     8434 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/task_helpers/etag_helpers.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/templates/ledger/base.html
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/templates/ledger/error.html
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/templates/ledger/index.html
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/templates/ledger/menu.html
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/templates/ledger/bundles/ledger-css.html
+-rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/templates/ledger/charledger/char_ledger.html
+-rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/templates/ledger/charledger/month.html
+-rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/templates/ledger/charledger/year.html
+-rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/templates/ledger/corpledger/corp_ledger.html
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/templates/ledger/corpledger/month.html
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/templates/ledger/corpledger/year.html
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/templates/ledger/modals/modal-full.html
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/templates/ledger/modals/modal-xl.html
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/templates/ledger/modals/modal.html
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/templates/ledger/modals/modal_dialog.html
+-rw-r--r--   0        0        0    17987 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/templates/ledger/modals/pve/view_character_content.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/templatetags/__init__.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/templatetags/ledger.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/view_helpers/__init__.py
+-rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/view_helpers/core.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/views/__init__.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/views/pve.py
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/views/character/char_audit.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/views/corporation/corp_audit.py
+-rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/views/corporation/corp_events.py
+-rw-r--r--   0        0        0     8919 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/views/corporation/corp_tax.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/LICENSE
+-rw-r--r--   0        0        0     5602 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/README.md
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     8381 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/PKG-INFO
```

### Comparing `aa_ledger-0.3.8a1/ledger/admin.py` & `aa_ledger-0.4.0/ledger/admin.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8a1/ledger/app_settings.py` & `aa_ledger-0.4.0/ledger/app_settings.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8a1/ledger/auth_hooks.py` & `aa_ledger-0.4.0/ledger/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8a1/ledger/decorators.py` & `aa_ledger-0.4.0/ledger/decorators.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8a1/ledger/hooks.py` & `aa_ledger-0.4.0/ledger/hooks.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8a1/ledger/tasks.py` & `aa_ledger-0.4.0/ledger/tasks.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8a1/ledger/urls.py` & `aa_ledger-0.4.0/ledger/urls.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8a1/ledger/api/__init__.py` & `aa_ledger-0.4.0/ledger/api/__init__.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8a1/ledger/api/helpers.py` & `aa_ledger-0.4.0/ledger/api/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from django.core.exceptions import ObjectDoesNotExist
 from django.db.models import QuerySet
 
 from allianceauth.authentication.models import UserProfile
 from allianceauth.eveonline.models import EveCharacter
 
 from ledger import app_settings, models
+from ledger.errors import LedgerImportError
 
 if app_settings.LEDGER_CORPSTATS_TWO:
     from corpstats.models import CorpMember
 else:
     from allianceauth.corputils.models import CorpMember
 
 from ledger.hooks import get_extension_logger
@@ -39,24 +40,29 @@
             "count": self._items_count(queryset),
         }
 
 
 # pylint: disable=import-outside-toplevel
 def get_models_and_string():
     if app_settings.LEDGER_MEMBERAUDIT_USE:
-        from memberaudit.models import (
-            CharacterMiningLedgerEntry as CharacterMiningLedger,
-        )
-        from memberaudit.models import CharacterWalletJournalEntry
-
-        return (
-            CharacterMiningLedger,
-            CharacterWalletJournalEntry,
-            "character__eve_character",
-        )
+        try:
+            from memberaudit.models import (
+                CharacterMiningLedgerEntry as CharacterMiningLedger,
+            )
+            from memberaudit.models import CharacterWalletJournalEntry
+
+            return (
+                CharacterMiningLedger,
+                CharacterWalletJournalEntry,
+                "character__eve_character",
+            )
+        except Exception as exc:
+            logger.error("Memberaudit is enabled but not installed")
+            raise LedgerImportError("Memberaudit is enabled but not installed") from exc
+
     from ledger.models.characteraudit import (
         CharacterMiningLedger,
         CharacterWalletJournalEntry,
     )
 
     return (
         CharacterMiningLedger,
```

### Comparing `aa_ledger-0.3.8a1/ledger/api/ledgermanager.py` & `aa_ledger-0.4.0/ledger/api/ledgermanager.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,32 +15,63 @@
 
 CharacterMiningLedger, CharacterWalletJournalEntry, SR_CHAR = get_models_and_string()
 
 
 class LedgerDataCore:
     """LedgerDataCore class to store the core data."""
 
-    def __init__(self, models):
-        self.ess_entries, self.entries, self.mining_data = models
+    def __init__(self):
         self.total_bounty = 0
         self.total_ess_payout = 0
+        self.total_mining = 0
         self.total_miscellaneous = 0
         self.total_isk = 0
 
 
 class LedgerData(LedgerDataCore):
     """LedgerData class to store the data."""
 
-    def __init__(self, models):
-        super().__init__(models)
+    def __init__(self):
+        super().__init__()
+        self.total_cost = 0
+        self.total_production_cost = 0
+        self.total_market = 0
+
+    def reset_values(self):
+        self.total_bounty = 0
+        self.total_ess_payout = 0
+        self.total_mining = 0
+        self.total_miscellaneous = 0
+        self.total_isk = 0
         self.total_cost = 0
         self.total_production_cost = 0
         self.total_market = 0
 
 
+class LedgerModels:
+    """LedgerModels class to store the models."""
+
+    def __init__(
+        self, character_journal=None, corporation_journal=None, mining_journal=None
+    ):
+        self.char_journal = character_journal
+        self.corp_journal = corporation_journal
+        self.mining_journal = mining_journal
+
+    def to_values(self, journal):
+        logger.debug(type(journal))
+        return journal.values(
+            "amount", "ref_type", "first_party_id", "second_party_id", "date"
+        )
+
+    def to_values_mining(self, journal):
+        logger.debug(type(journal))
+        return journal.values("total", "date")
+
+
 class LedgerDate:
     """LedgerDate class to store the date data."""
 
     def __init__(self, year, month):
         self.year = year
         self.month = month
         self.monthly = month == 0
@@ -153,15 +184,15 @@
         chars = [char.character_id for char in self.chars]
         for char in self.chars:
             char_id = char.character_id
             char_name = char.character_name
 
             # Core Filters
             filters = {
-                "ledger": Q(second_party_id=char_id),
+                "ledger": Q(second_party_id=char_id),  # Fetch All Entries
                 "market": Q(second_party_id=char_id, ref_type="market_transaction"),
                 "contracts": Q(
                     second_party_id=char_id,
                     ref_type__in=[
                         "contract_price_payment_corp",
                         "contract_reward",
                         "contract_price",
@@ -246,43 +277,50 @@
             filter_date &= Q(date__month=self.month)
 
         chars = [char.character_id for char in self.chars]
 
         entries_filter = Q(second_party_id__in=chars) | Q(first_party_id__in=chars)
 
         # Filter the entries for the current day/month
-        character_journal = (
-            CharacterWalletJournalEntry.objects.filter(filters, filter_date)
-            .select_related("first_party", "second_party", SR_CHAR)
-            .order_by("-date")
-        )
-
-        corporation_journal = (
-            CorporationWalletJournalEntry.objects.filter(entries_filter, filter_date)
-            .select_related("first_party", "second_party")
-            .order_by("-date")
+        character_journal = CharacterWalletJournalEntry.objects.filter(
+            filters, filter_date
+        ).select_related("first_party", "second_party", SR_CHAR)
+
+        corporation_journal = CorporationWalletJournalEntry.objects.filter(
+            entries_filter, filter_date
+        ).select_related(
+            "division",
+            "division__corporation",
+            "division__corporation__corporation",
+            "first_party",
+            "second_party",
         )
 
         # Exclude Events to avoid wrong stats
         corporation_journal = events_filter(corporation_journal)
         mining_journal = (
-            CharacterMiningLedger.objects.filter(filters, filter_date)
-            .select_related(SR_CHAR)
-            .order_by("-date")
+            CharacterMiningLedger.objects.filter(filters, filter_date).select_related(
+                SR_CHAR
+            )
         ).annotate_pricing()
 
         self.process_character_chars(
             corporation_journal, character_journal, mining_journal
         )
 
         # Use Only Corporation Ledger
         models = corporation_journal, character_journal, mining_journal
         # Create the Ledger
         date_data = LedgerDate(self.year, self.month)
-        ledger = BillboardLedger(models, date_data, corp=False)
+        models = LedgerModels(
+            character_journal=character_journal,
+            corporation_journal=corporation_journal,
+            mining_journal=mining_journal,
+        )
+        ledger = BillboardLedger(date_data, models, corp=False)
         billboard_dict = ledger.billboard_char_ledger()
 
         output = []
         output.append(
             {
                 "ratting": sorted(
                     list(self.character_dict.values()), key=lambda x: x["main_name"]
@@ -298,32 +336,30 @@
         filters = Q(division__corporation__corporation__corporation_id__in=corporations)
         filters &= Q(second_party_id__in=chars_list)
         filter_date = Q(date__year=self.year)
 
         if not self.month == 0:
             filter_date &= Q(date__month=self.month)
 
-        corporation_journal = (
-            CorporationWalletJournalEntry.objects.filter(filters, filter_date)
-            .select_related(
-                "division",
-                "division__corporation",
-                "division__corporation__corporation",
-                "first_party",
-                "second_party",
-            )
-            .order_by("-date")
+        corporation_journal = CorporationWalletJournalEntry.objects.filter(
+            filters, filter_date
+        ).select_related(
+            "division",
+            "division__corporation",
+            "division__corporation__corporation",
+            "first_party",
+            "second_party",
         )
         self.process_corporation_chars(corporation_journal)
 
-        # Use Only Corporation Ledger
-        models = corporation_journal, None, None
         # Create the Ledger
         date_data = LedgerDate(self.year, self.month)
-        ledger = BillboardLedger(models, date_data, corp=True)
+        models = LedgerModels(corporation_journal=corporation_journal)
+        ledger = BillboardLedger(date_data, models, corp=True)
+
         billboard_dict = ledger.billboard_corp_ledger(
             self.corporation_dict, self.summary_total.total_amount
         )
 
         output = []
         output.append(
             {
@@ -335,129 +371,118 @@
             }
         )
 
         return output
 
 
 class BillboardLedger:
-    def __init__(self, models, date_data, corp=False):
+    def __init__(self, date_data: LedgerDate, models: LedgerModels, corp=False):
         self.is_corp = corp
+        self.data = LedgerData()
         self.models = models
-        self.data = LedgerData(models)
         self.date = date_data
         self.sum = LedgerSum()
         self.billboard_dict = {
             "walletcharts": [],
             "charts": [],
             "rattingbar": [],
             "workflowgauge": [],
         }
         self.date_billboard = ["x"]
 
-    def set_filters(self, filter_date):
-        if self.is_corp:
-            return Q(date__year=self.date.year, date__month=filter_date)
-        return Q(
-            date__year=self.date.year,
-            date__month=self.date.month,
-            date__day=filter_date,
-        )
+    def aggregate_corp(self, journal, range_):
+        """Aggregate the journal entries for the corporation."""
+        for entry in journal:
+            if entry["date"].year == self.date.year:
+                if (self.date.month == 0 and entry["date"].month == range_) or (
+                    self.date.month != 0 and entry["date"].day == range_
+                ):
+                    if self.is_corp:
+                        if entry["ref_type"] == "bounty_prizes":
+                            self.data.total_bounty += entry["amount"]
+                    if entry["ref_type"] == "ess_escrow_transfer":
+                        self.data.total_ess_payout += entry["amount"]
+
+    def aggregate_char(self, journal, range_):
+        """Aggregate the journal entries for the character."""
+        for entry in journal:
+            if entry["date"].year == self.date.year:
+                if (self.date.month == 0 and entry["date"].month == range_) or (
+                    self.date.month != 0 and entry["date"].day == range_
+                ):
+                    # Bounty Filter
+                    if entry["ref_type"] == "bounty_prizes":
+                        self.data.total_bounty += entry["amount"]
+                    # Misc Filter
+                    # TODO Add player_donation to the Billboard
+                    if (
+                        entry["ref_type"]
+                        in [
+                            "market_transaction",
+                            "contract_price_payment_corp",
+                            "contract_reward",
+                            "contract_price",
+                        ]
+                        and entry["amount"] > 0
+                    ):
+                        self.data.total_miscellaneous += entry["amount"]
+                    # Total ISK
+                    if entry["amount"] > 0:
+                        self.data.total_isk += entry["amount"]
+                    else:
+                        self.data.total_cost += entry["amount"]
+                    # Total Market
+                    if entry["ref_type"] in [
+                        "market_escrow",
+                        "transaction_tax",
+                        "market_provider_tax",
+                        "brokers_fee",
+                    ]:
+                        self.data.total_market += entry["amount"]
+                    # Production Cost
+                    if entry["ref_type"] in ["industry_job_tax", "manufacturing"]:
+                        self.data.total_production_cost += entry["amount"]
+
+    def aggregate_mining(self, journal, range_):
+        """Aggregate the journal entries for the mining."""
+        for entry in journal:
+            if entry["date"].year == self.date.year:
+                if (self.date.month == 0 and entry["date"].month == range_) or (
+                    self.date.month != 0 and entry["date"].day == range_
+                ):
+                    self.data.total_mining += entry["total"]
+
+    # pylint: disable=too-many-branches
+    def process_day(
+        self, range_, corp_journal=None, char_journal=None, mining_journal=None
+    ):
+        """Process the day for the journal entries."""
+        date = datetime.now()
 
-    def aggregate_journal(self, journal):
-        result = journal.aggregate(
-            total_amount=Coalesce(Sum(F("amount")), 0, output_field=DecimalField())
-        )
-        return result["total_amount"]
+        # Reset the values
+        self.data.reset_values()
 
-    def process_day(self, range_):
-        date = datetime.now()
         if self.date.monthly:
             date = date.replace(day=1)
-            # Core
-        filters = {
-            "date": (
-                Q(date__year=self.date.year, date__month=range_)
-                if self.date.monthly
-                else Q(
-                    date__year=self.date.year,
-                    date__month=self.date.month,
-                    date__day=range_,
-                )
-            ),
-            "miscellaneous": Q(
-                ref_type__in=[
-                    "market_transaction",
-                    "contract_price_payment_corp",
-                    "contract_reward",
-                    "contract_price",
-                ],
-                amount__gt=0,
-            ),
-            "market_cost": Q(
-                ref_type__in=[
-                    "market_escrow",
-                    "transaction_tax",
-                    "market_provider_tax",
-                    "brokers_fee",
-                ],
-                amount__lt=0,
-            ),
-            "production_cost": Q(
-                ref_type__in=["industry_job_tax", "manufacturing"], amount__lt=0
-            ),
-            "bounty": Q(ref_type="bounty_prizes"),
-            "ess": Q(ref_type="ess_escrow_transfer"),
-        }
-        # Calculate the totals for Character Billboard
-        if not self.is_corp:
-            mining_query = self.data.mining_data.filter(filters["date"]).values(
-                "total", "date"
-            )
-            mining_aggregated = mining_query.aggregate(total_amount=Sum(F("total")))
-            total_amount_mining = mining_aggregated["total_amount"] or 0
-            # Calculate the total bounty, ESS payout, and miscellaneous amounts
-            self.data.total_bounty = self.aggregate_journal(
-                self.data.entries.filter(filters["bounty"], filters["date"])
-            )
-            # Calculate the total market escrow, transaction tax, market provider tax, and broker's fee
-            self.data.total_market = self.aggregate_journal(
-                self.data.entries.filter(filters["market_cost"], filters["date"])
-            )
-            # Calculate the total production cost
-            self.data.total_production_cost = self.aggregate_journal(
-                self.data.entries.filter(filters["production_cost"], filters["date"])
-            )
-            # Calculate the total miscellaneous
-            self.data.total_miscellaneous = self.aggregate_journal(
-                self.data.entries.filter(filters["miscellaneous"], filters["date"])
-            )
-            self.data.total_isk = self.aggregate_journal(
-                self.data.entries.filter(Q(amount__gt=0))
-            )
-            self.data.total_cost = self.aggregate_journal(
-                self.data.entries.filter(Q(amount__lt=0))
-            )
-        # Calculate the totals for Corporation Billboard
-        if self.is_corp:
-            self.data.total_ess_payout = (
-                self.aggregate_journal(
-                    self.data.ess_entries.filter(filters["ess"], filters["date"])
-                )
-                / app_settings.LEDGER_CORP_TAX
-            ) * (100 - app_settings.LEDGER_CORP_TAX)
-            self.data.total_bounty = self.aggregate_journal(
-                self.data.ess_entries.filter(filters["bounty"], filters["date"])
-            )
+
+        logger.debug(self.date.month)
+
+        if corp_journal:
+            self.aggregate_corp(corp_journal, range_)
+        if char_journal:
+            self.aggregate_char(char_journal, range_)
+        if mining_journal:
+            self.aggregate_mining(mining_journal, range_)
 
         # Add the totals to the respective lists
         self.sum.sum_amount.append(int(self.data.total_bounty))
         self.sum.sum_amount_ess.append(int(self.data.total_ess_payout))
         if not self.is_corp:
             self.sum.sum_amount_misc.append(int(self.data.total_miscellaneous))
-            self.sum.sum_amount_mining.append(int(total_amount_mining))
+            self.sum.sum_amount_mining.append(int(self.data.total_mining))
         # Add the date to the date list
         self.date_billboard.append(
             date.replace(day=range_).strftime("%Y-%m-%d")
             if not self.date.monthly
             else date.replace(month=range_).strftime("%Y-%m")
         )
 
@@ -553,38 +578,44 @@
             sorted(self.billboard_dict["charts"], key=lambda x: x[0])
             if self.billboard_dict["charts"]
             else None
         )
 
     # Create the Billboard Char Ledger
     def billboard_char_ledger(self):
-        for range_ in self.date.day_checks:
-            try:
-                self.process_day(range_)
-            except ValueError:
-                continue
+        corp_journal_values = self.models.corp_journal.values(
+            "amount", "ref_type", "first_party_id", "second_party_id", "date"
+        )
+        char_journal_values = self.models.char_journal.values(
+            "amount", "ref_type", "first_party_id", "second_party_id", "date"
+        )
+        mining_journal_values = self.models.mining_journal.values("total", "date")
+        for day in self.date.day_checks:
+            self.process_day(
+                day, corp_journal_values, char_journal_values, mining_journal_values
+            )
 
         self.calculate_total_sum()
 
         rounded_percentages = self.calculate_percentages()
         self.generate_gauge_data(rounded_percentages)
 
         self.generate_wallet_ratting_bar()
 
         self.generate_wallet_charts_data()
 
         return self.billboard_dict
 
     # Create the Billboard Corp Ledger
     def billboard_corp_ledger(self, corporation_dict, summary_dict_all):
-        for range_ in self.date.day_checks:
-            try:
-                self.process_day(range_)
-            except ValueError:
-                continue
+        corp_journal_values = self.models.corp_journal.values(
+            "amount", "ref_type", "first_party_id", "second_party_id", "date"
+        )
+        for day in self.date.day_checks:
+            self.process_day(day, corp_journal_values)
 
         self.calculate_total_sum()
 
         self.generate_wallet_ratting_bar()
 
         self.generate_wallet_corps_data(corporation_dict, summary_dict_all)
```

### Comparing `aa_ledger-0.3.8a1/ledger/api/schema.py` & `aa_ledger-0.4.0/ledger/api/schema.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8a1/ledger/api/templatemanager.py` & `aa_ledger-0.4.0/ledger/api/templatemanager.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8a1/ledger/api/character/ledger.py` & `aa_ledger-0.4.0/ledger/api/character/ledger.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8a1/ledger/api/character/template.py` & `aa_ledger-0.4.0/ledger/api/character/template.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8a1/ledger/api/corporation/ledger.py` & `aa_ledger-0.4.0/ledger/api/corporation/ledger.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8a1/ledger/api/corporation/template.py` & `aa_ledger-0.4.0/ledger/api/corporation/template.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8a1/ledger/managers/charaudit_manager.py` & `aa_ledger-0.4.0/ledger/managers/charaudit_manager.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8a1/ledger/managers/corpaudit_manager.py` & `aa_ledger-0.4.0/ledger/managers/corpaudit_manager.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8a1/ledger/managers/general_manager.py` & `aa_ledger-0.4.0/ledger/managers/general_manager.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8a1/ledger/models/characteraudit.py` & `aa_ledger-0.4.0/ledger/models/characteraudit.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8a1/ledger/models/corporationaudit.py` & `aa_ledger-0.4.0/ledger/models/corporationaudit.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8a1/ledger/models/events.py` & `aa_ledger-0.4.0/ledger/models/events.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8a1/ledger/models/general.py` & `aa_ledger-0.4.0/ledger/models/general.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8a1/ledger/static/ledger/css/billboards_dark.css` & `aa_ledger-0.4.0/ledger/static/ledger/css/billboards_dark.css`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8a1/ledger/static/ledger/css/cards.css` & `aa_ledger-0.4.0/ledger/static/ledger/css/cards.css`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8a1/ledger/static/ledger/css/custom.css` & `aa_ledger-0.4.0/ledger/static/ledger/css/custom.css`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8a1/ledger/static/ledger/guides/ledger-1.png` & `aa_ledger-0.4.0/ledger/static/ledger/guides/ledger-1.png`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8a1/ledger/static/ledger/guides/ledger-2.png` & `aa_ledger-0.4.0/ledger/static/ledger/guides/ledger-2.png`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8a1/ledger/static/ledger/guides/ledger-3.png` & `aa_ledger-0.4.0/ledger/static/ledger/guides/ledger-3.png`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8a1/ledger/static/ledger/images/Spinner-1s-64px-dark.gif` & `aa_ledger-0.4.0/ledger/static/ledger/images/Spinner-1s-64px-dark.gif`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8a1/ledger/static/ledger/images/Spinner-1s-64px-light.gif` & `aa_ledger-0.4.0/ledger/static/ledger/images/Spinner-1s-64px-light.gif`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8a1/ledger/static/ledger/js/charledger.js` & `aa_ledger-0.4.0/ledger/static/ledger/js/charledger.js`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8a1/ledger/static/ledger/js/corpledger.js` & `aa_ledger-0.4.0/ledger/static/ledger/js/corpledger.js`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8a1/ledger/static/ledger/js/img.js` & `aa_ledger-0.4.0/ledger/static/ledger/js/img.js`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8a1/ledger/task_helpers/char_helpers.py` & `aa_ledger-0.4.0/ledger/task_helpers/char_helpers.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8a1/ledger/task_helpers/core_helpers.py` & `aa_ledger-0.4.0/ledger/task_helpers/core_helpers.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8a1/ledger/task_helpers/corp_helpers.py` & `aa_ledger-0.4.0/ledger/task_helpers/corp_helpers.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8a1/ledger/task_helpers/etag_helpers.py` & `aa_ledger-0.4.0/ledger/task_helpers/etag_helpers.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8a1/ledger/templates/ledger/base.html` & `aa_ledger-0.4.0/ledger/templates/ledger/base.html`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 {% block header_nav_brand %}
     Ledger
 {% endblock header_nav_brand %}
 
 {% block header_nav_collapse_left %}
 
-{% block vow_menu %}{% include 'ledger/ledger/menu.html' %}{% endblock %}
+{% block vow_menu %}{% include 'ledger/menu.html' with memberaudit=memberaudit %}{% endblock %}
 
 {% endblock header_nav_collapse_left %}
 
 {% block content %}
 
 {% include 'ledger/bundles/ledger-css.html' %}
 {% include 'bundles/datatables-css-bs5.html' %}
```

### Comparing `aa_ledger-0.3.8a1/ledger/templates/ledger/error.html` & `aa_ledger-0.4.0/ledger/templates/ledger/error.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8a1/ledger/templates/ledger/ledger/index.html` & `aa_ledger-0.4.0/ledger/templates/ledger/index.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {% extends 'ledger/base.html' %}
-{% load i18n %}
-{% load humanize %}
-{% block vow_menu %}{% include 'ledger/ledger/menu.html' %}{% endblock %}
+    {% load i18n %}
+    {% load humanize %}
 
 {% block vow_block %}
+{{ memberaudit }}
     <div class="panel panel-primary">
         <div class="container-fluid">
             <div id="container">
                 <br>
                 <div class="line-container">
                     <div class="line-text"><h4>Ledger Guide</h4></div>
                     <hr class="custom-line">
```

#### html2text {}

```diff
@@ -1,10 +1,9 @@
 {% extends 'ledger/base.html' %} {% load i18n %} {% load humanize %} {% block
-vow_menu %}{% include 'ledger/ledger/menu.html' %}{% endblock %} {% block
-vow_block %}
+vow_block %} {{ memberaudit }}
 
 ****** LLeeddggeerr GGuuiiddee ******
 ===============================================================================
 Character Ledger shows all Ratting / ESS Payout / Mining entrys per Month / Day
 
 You can switch between Months to show what you have already done and how much
 it was.
```

### Comparing `aa_ledger-0.3.8a1/ledger/templates/ledger/ledger/menu.html` & `aa_ledger-0.4.0/ledger/templates/ledger/menu.html`

 * *Files 9% similar despite different names*

```diff
@@ -9,24 +9,25 @@
 <li class="nav-item">
     <a class="nav-link" href="{% url 'ledger:ledger_char_index' %}">Character Ledger</a>
 </li>
 
 <li class="nav-item">
     <span class="nav-link">|</span>
 </li>
-
+{% if not memberaudit %}
 <li class="nav-item">
     <a class="nav-link" href="{% url 'ledger:ledger_add_char' %}">Add Char</a>
 </li>
 {% endif %}
+{% endif %}
 
 {% if perms.ledger.corp_audit_admin_access %}
 <li class="nav-item">
     <a class="nav-link" href="{% url 'ledger:ledger_add_corp' %}">Add Corporation</a>
 </li>
 {% endif %}
 
-{% if perms.ledger.char_audit_admin_access %}
+{% if perms.ledger.char_audit_admin_access and memberaudit%}
 <li class="nav-item">
     <a class="nav-link" href="{% url 'ledger:ledger_fetch_memberaudit' %}">Add All Memberaudit Chars</a>
 </li>
 {% endif %}
```

### Comparing `aa_ledger-0.3.8a1/ledger/templates/ledger/ledger/charledger/char_ledger.html` & `aa_ledger-0.4.0/ledger/templates/ledger/charledger/char_ledger.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% extends 'ledger/ledger/base.html' %}
+{% extends 'ledger/base.html' %}
 {% load i18n %}
 {% load humanize %}
 {% load static %}
 {% load ledger %}
 
 {% block page_title %}Character Ledger{% endblock %}
 {% block page_topic %}<h1 class="page-header text-center">{% translate "Character Ledger" %}</h1>{% endblock page_topic %}
@@ -20,16 +20,16 @@
                 <a id="currentYearLink" class="nav-link" href="#tab-all_month" data-bs-toggle="tab" role="tab" data-bs-target="#tab-all_month">
                     Year - {% now "Y" %}
                 </a>
             </li>
         </ul>
         <div class="tab-content rounded-bottom">
             <div class="tab-content">
-                {% include 'ledger/ledger/charledger/month.html' %}
-                {% include 'ledger/ledger/charledger/year.html' %}
+                {% include 'ledger/charledger/month.html' %}
+                {% include 'ledger/charledger/year.html' %}
             </div>
         </div>
     </div>
 </div>
 
 <!-- Tab Session -->
 {% include 'ledger/modals/modal_dialog.html' with name="ViewCharacter" %}
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-{% extends 'ledger/ledger/base.html' %} {% load i18n %} {% load humanize %} {%
-load static %} {% load ledger %} {% block page_title %}Character Ledger{%
-endblock %} {% block page_topic %}
+{% extends 'ledger/base.html' %} {% load i18n %} {% load humanize %} {% load
+static %} {% load ledger %} {% block page_title %}Character Ledger{% endblock
+%} {% block page_topic %}
 ************ {{%% ttrraannssllaattee ""CChhaarraacctteerr LLeeddggeerr"" %%}} ************
 {% endblock page_topic %} {% block vow_block %}
     * _M_o_n_t_h_ _-_ _{_%_ _n_o_w_ _"_F_"_ _%_}
     * _Y_e_a_r_ _-_ _{_%_ _n_o_w_ _"_Y_"_ _%_}
-{% include 'ledger/ledger/charledger/month.html' %} {% include 'ledger/ledger/
-charledger/year.html' %}
+{% include 'ledger/charledger/month.html' %} {% include 'ledger/charledger/
+year.html' %}
 {% include 'ledger/modals/modal_dialog.html' with name="ViewCharacter" %} {%
 endblock %} {% block extra_css %}
 {% endblock %} {% block extra_javascript %}
 {% include 'bundles/datatables-js-bs5.html' %}
 {% endblock extra_javascript %} {% block extra_script %} {% endblock
 extra_script %}
```

### Comparing `aa_ledger-0.3.8a1/ledger/templates/ledger/ledger/charledger/month.html` & `aa_ledger-0.4.0/ledger/templates/ledger/corpledger/year.html`

 * *Files 19% similar despite different names*

```diff
@@ -1,87 +1,57 @@
 {% load i18n %}
 {% load humanize %}
 
-<div role="tabpanel" class="tab-pane active" id="tab-current_month">
+<div role="tabpanel" class="tab-pane" id="tab-all_month">
     <div class="card-body bg-secondary table-responsive">
-        <select class="form-select" style="width: 130px; display: none;" id="monthDropdown">
-            <option value="1">January</option>
-            <option value="2">February</option>
-            <option value="3">March</option>
-            <option value="4">April</option>
-            <option value="5">May</option>
-            <option value="6">June</option>
-            <option value="7">July</option>
-            <option value="8">August</option>
-            <option value="9">September</option>
-            <option value="10">October</option>
-            <option value="11">November</option>
-            <option value="12">Dezember</option>
-        </select>
-        <br>
-
-        <table class="table table-striped table-hover table-width-fix" id="ratting" style="width: 100%;">
+        <table class="table table-striped table-hover table-width-fix" id="ratting_year" style="width: 100%;">
             <br>
             <thead>
                 <th class="col-main-character" style="width: 20%;">Main Character</th>
-                <th class="col-total-amount" style="width: 20%;">Ratting Amount</th>
-                <th class="col-total-ess" style="width: 20%;">ESS Payout</th>
-                <th class="col-total-mining" style="width: 20%;">Mining Amount</th>
-                <th class="col-total-others" style="width: 10%;">Misc. Amount</th>
+                <th class="col-total-amount" style="width: 20%;">Total Amount</th>
+                <th class="col-total-ess" style="width: 20%;">ESS Amount</th>
                 <th class="col-total-action" style="width: 1%;"></th>
             </thead>
 
             <tbody>
             </tbody>
 
-            <tfoot id="foot">
+            <tfoot id="foot-year">
                 <tr>
                     <th><strong>Geteilt</strong></th>
                     <th class="col-total-amount"></th>
                     <th class="col-total-ess"></th>
-                    <th class="col-total-mining"></th>
-                    <th class="col-total-others"></th>
+                    <th></th>
                 </tr>
                 <tr>
                     <th><strong>Gesamt</strong></th>
-                    <th></th>
-                    <th></th>
-                    <th></th>
                     <th class="col-total-gesamt"></th>
+                    <th></th>
                     <th class="col-total-button"></th>
                 </tr>
             </tfoot>
         </table>
     </div>
     <br>
     <div class="card card-default">
         <div class="rounded-top">
             <div class="row g-0">
-                <div class="col-md-6 g-2" id="rattingBarContainer">
+                <div class="col-md-6 g-2" id="ChartYearContainer">
                     <div class="card-header bg-primary">
-                        <h3 class="card-title">Ledger 30 Days</h3>
+                        <h3 class="card-title">Ratting Chart</h3>
                     </div>
                     <div class="card-body bg-secondary">
-                        <div id="rattingBar"></div>
+                        <div id="rattingChartYear"></div>
                     </div>
                 </div>
-                <div class="col-md-6 g-2" id="walletChartContainer">
+                <div class="col-md-6 g-2" id="rattingBarYearContainer">
                     <div class="card-header bg-primary">
-                        <h3 class="card-title">Wallet</h3>
+                        <h3 class="card-title">Ratting Year</h3>
                     </div>
                     <div class="card-body bg-secondary">
-                        <div id="walletChart"></div>
-                    </div>
-                </div>
-                <div class="col-md-6 g-2" id="workGaugeContainer">
-                    <div class="card-header bg-primary">
-                        <h3 class="card-title">Workflow</h3>
-                    </div>
-                    <div class="card-body bg-secondary">
-                        <div id="workGauge"></div>
+                        <div id="rattingBarYear"></div>
                     </div>
                 </div>
             </div>
         </div>
     </div>
-
 </div>
```

#### html2text {}

```diff
@@ -1,9 +1,6 @@
 {% load i18n %} {% load humanize %}
-[One of: January/February/March/April/May/June/July/August/September/October/
-November/Dezember]
 GGeetteeiilltt
 GGeessaammtt
 
-******** LLeeddggeerr 3300 DDaayyss ********
-******** WWaalllleett ********
-******** WWoorrkkffllooww ********
+******** RRaattttiinngg CChhaarrtt ********
+******** RRaattttiinngg YYeeaarr ********
```

### Comparing `aa_ledger-0.3.8a1/ledger/templates/ledger/ledger/charledger/year.html` & `aa_ledger-0.4.0/ledger/templates/ledger/charledger/year.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8a1/ledger/templates/ledger/ledger/corpledger/corp_ledger.html` & `aa_ledger-0.4.0/ledger/templates/ledger/corpledger/corp_ledger.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% extends 'ledger/ledger/base.html' %}
+{% extends 'ledger/base.html' %}
 {% load i18n %}
 {% load humanize %}
 {% load static %}
 {% load ledger %}
 
 {% block page_title %}Corporation Ledger{% endblock %}
 {% block page_topic %}<h1 class="page-header text-center">{% translate "Corporation Ledger" %}</h1>{% endblock page_topic %}
@@ -20,16 +20,16 @@
                 <a id="currentYearLink" class="nav-link" href="#tab-all_month" data-bs-toggle="tab" role="tab" data-bs-target="#tab-all_month">
                     Year - {% now "Y" %}
                 </a>
             </li>
         </ul>
         <div class="tab-content rounded-bottom">
             <div class="tab-content">
-                {% include 'ledger/ledger/corpledger/month.html' %}
-                {% include 'ledger/ledger/corpledger/year.html' %}
+                {% include 'ledger/corpledger/month.html' %}
+                {% include 'ledger/corpledger/year.html' %}
             </div>
         </div>
     </div>
 </div>
 
 <!-- Tab Session -->
 {% include 'ledger/modals/modal_dialog.html' with name="ViewCharacter" %}
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-{% extends 'ledger/ledger/base.html' %} {% load i18n %} {% load humanize %} {%
-load static %} {% load ledger %} {% block page_title %}Corporation Ledger{%
-endblock %} {% block page_topic %}
+{% extends 'ledger/base.html' %} {% load i18n %} {% load humanize %} {% load
+static %} {% load ledger %} {% block page_title %}Corporation Ledger{% endblock
+%} {% block page_topic %}
 ************ {{%% ttrraannssllaattee ""CCoorrppoorraattiioonn LLeeddggeerr"" %%}} ************
 {% endblock page_topic %} {% block vow_block %}
     * _M_o_n_t_h_ _-_ _{_%_ _n_o_w_ _"_F_"_ _%_}
     * _Y_e_a_r_ _-_ _{_%_ _n_o_w_ _"_Y_"_ _%_}
-{% include 'ledger/ledger/corpledger/month.html' %} {% include 'ledger/ledger/
-corpledger/year.html' %}
+{% include 'ledger/corpledger/month.html' %} {% include 'ledger/corpledger/
+year.html' %}
 {% include 'ledger/modals/modal_dialog.html' with name="ViewCharacter" %} {%
 endblock %} {% block extra_css %}
 {% endblock %} {% block extra_javascript %}
 {% include 'bundles/datatables-js-bs5.html' %}
 {% endblock extra_javascript %} {% block extra_script %} {% endblock
 extra_script %}
```

### Comparing `aa_ledger-0.3.8a1/ledger/templates/ledger/ledger/corpledger/month.html` & `aa_ledger-0.4.0/ledger/templates/ledger/corpledger/month.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 {% load i18n %}
 {% load humanize %}
 
 <div role="tabpanel" class="tab-pane active" id="tab-current_month">
     <div class="card-body bg-secondary table-responsive">
         <select class="form-select" style="width: 130px; display: none;" id="monthDropdown">
-            <option value="1">January</option>
-            <option value="2">February</option>
-            <option value="3">March</option>
-            <option value="4">April</option>
-            <option value="5">May</option>
-            <option value="6">June</option>
-            <option value="7">July</option>
-            <option value="8">August</option>
-            <option value="9">September</option>
-            <option value="10">October</option>
-            <option value="11">November</option>
-            <option value="12">Dezember</option>
+            <option value="1">{% trans "January" %}</option>
+            <option value="2">{% trans "February" %}</option>
+            <option value="3">{% trans "March" %}</option>
+            <option value="4">{% trans "April" %}</option>
+            <option value="5">{% trans "May" %}</option>
+            <option value="6">{% trans "June" %}</option>
+            <option value="7">{% trans "July" %}</option>
+            <option value="8">{% trans "August" %}</option>
+            <option value="9">{% trans "September" %}</option>
+            <option value="10">{% trans "October" %}</option>
+            <option value="11">{% trans "November" %}</option>
+            <option value="12">{% trans "December" %}</option>
         </select>
         <br>
         <table class="table table-striped table-hover table-width-fix" id="ratting" style="width: 100%;">
             <br>
             <thead>
                 <th class="col-main-character" style="width: 20%;">Main Character</th>
                 <th class="col-total-amount" style="width: 20%;">Total Amount</th>
```

#### html2text {}

```diff
@@ -1,8 +1,10 @@
 {% load i18n %} {% load humanize %}
-[One of: January/February/March/April/May/June/July/August/September/October/
-November/Dezember]
+[One of: {% trans "January" %}/{% trans "February" %}/{% trans "March" %}/{%
+trans "April" %}/{% trans "May" %}/{% trans "June" %}/{% trans "July" %}/{%
+trans "August" %}/{% trans "September" %}/{% trans "October" %}/{% trans
+"November" %}/{% trans "December" %}]
 GGeetteeiilltt
 GGeessaammtt
 
 ******** RRaattttiinngg CChhaarrtt ********
 ******** RRaattttiinngg 3300 DDaayyss ********
```

### Comparing `aa_ledger-0.3.8a1/ledger/templates/ledger/modals/modal-full.html` & `aa_ledger-0.4.0/ledger/templates/ledger/modals/modal-full.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8a1/ledger/templates/ledger/modals/modal-xl.html` & `aa_ledger-0.4.0/ledger/templates/ledger/modals/modal-xl.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8a1/ledger/templates/ledger/modals/modal.html` & `aa_ledger-0.4.0/ledger/templates/ledger/modals/modal.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8a1/ledger/templates/ledger/modals/modal_dialog.html` & `aa_ledger-0.4.0/ledger/templates/ledger/modals/modal_dialog.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8a1/ledger/templates/ledger/modals/pve/view_character_content.html` & `aa_ledger-0.4.0/ledger/templates/ledger/modals/pve/view_character_content.html`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 {% load i18n %}
 {% load static %}
 {% load humanize %}
+{% load evelinks %}
 {% load ledger %}
 <div class="modal-content">
     <button type="button" class="btn-close py-3 px-3" data-bs-dismiss="modal" aria-label="Close"><span aria-hidden="true"></button>
     <div class="modal-header">
-        <h4 class="modal-title" id="modalTitle"><img src="{{ character.main_id|portrait }}" class="img-circle" alt="{{ data.main_name }}"> {{character.main_name}} - {{character.date}}</h4>
+        <h4 class="modal-title" id="modalTitle"><img src="{{ character.main_id|character_portrait_url:32 }}" class="img-circle" alt="{{ data.main_name }}"> {{character.main_name}} - {{character.date}}</h4>
     </div>
     <div class="card-body">
         <div class="row description-row">
             <h4 id="character-title"></h4>
         </div>
         {% if character %}
         <div>
@@ -25,260 +26,260 @@
                 </li>
             </ul>
             <div class="border border-secondary rounded-bottom tab-content px-2">
                 <div class="tab-pane panel panel-default active" id="tab-summary">
                     <div class="card-body modal-tab">
                         <div class="row description-row">
                             <div class="col-sm-6">Ratting:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.bounty.total_amount|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.bounty.total_amount|floatformat:0|intcomma }}</span> ISK</div>
                         </div>
                         <div class="row description-row">
                             <div class="col-sm-6">ESS:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.ess.total_amount|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.ess.total_amount|floatformat:0|intcomma }}</span> ISK</div>
                         </div>
                         <div class="row description-row">
                             <div class="col-sm-6">Stolen ESS:</div>
-                            <div class='col-sm-6'><span style="color: red">{{ character.stolen.total_amount|format_currency }}</span> ISK</div>
+                            <div class='col-sm-6'><span style="color: red">{{ character.stolen.total_amount|floatformat:0|intcomma }}</span> ISK</div>
                         </div>
                         {% if character.mining %}
                         <hr>
                         <div class="row description-row">
                             <div class="col-sm-6">Mining:</div>
-                            <div class='col-sm-6'><span style="color: green">{{ character.mining.total_amount|format_currency }}</span> ISK</div>
+                            <div class='col-sm-6'><span style="color: green">{{ character.mining.total_amount|floatformat:0|intcomma }}</span> ISK</div>
                         </div>
                         {% endif %}
                         {% if character.transaction %}
                         <hr>
                         <div class="row description-row">
                             <div class="col-sm-6">Trading:</div>
-                            <div class='col-sm-6'><span style="color: green">{{ character.transaction.total_amount|format_currency }}</span> ISK</div>
+                            <div class='col-sm-6'><span style="color: green">{{ character.transaction.total_amount|floatformat:0|intcomma }}</span> ISK</div>
                         </div>
                         <div class="row description-row">
                             <div class="col-sm-6">Trading Cost:</div>
-                            <div class='col-sm-6'><span style="color: red">{{ character.market_cost.total_amount|format_currency }}</span> ISK</div>
+                            <div class='col-sm-6'><span style="color: red">{{ character.market_cost.total_amount|floatformat:0|intcomma }}</span> ISK</div>
                         </div>
                         {% endif %}
                         {% if character.contract %}
                         <hr>
                         <div class="row description-row">
                             <div class="col-sm-6">Contracts:</div>
-                            <div class='col-sm-6'><span style="color: green">{{ character.contract.total_amount|format_currency }}</span> ISK</div>
+                            <div class='col-sm-6'><span style="color: green">{{ character.contract.total_amount|floatformat:0|intcomma }}</span> ISK</div>
                         </div>
                         {% endif %}
                         {% if character.donation %}
                         <hr>
                         <div class="row description-row">
                             <div class="col-sm-6">Donations:<br>
                             <span style="color: #FFBF00"><!--<i class="fas fa-exclamation-triangle"></i> Excluded from summary <i class="fas fa-exclamation-triangle"></i>--></span>
                             </div>
                             <div class='col-sm-6'>
                                 <span style="color: green">
-                                    {{ character.donation.total_amount|format_currency }}
+                                    {{ character.donation.total_amount|floatformat:0|intcomma }}
                                 </span> ISK
                                     <br><span style="color: #3483eb"><!--<i class="fas fa-info-circle"></i> Exluded registered chars <i class="fas fa-info-circle"></i>--></span>
                             </div>
                         </div>
                         {% endif %}
                         {% if character.production_cost %}
                         <hr>
                         <div class="row description-row">
                             <div class="col-sm-6">Production Cost:</div>
-                            <div class='col-sm-6'><span style="color: red">{{ character.production_cost.total_amount|format_currency }}</span> ISK</div>
+                            <div class='col-sm-6'><span style="color: red">{{ character.production_cost.total_amount|floatformat:0|intcomma }}</span> ISK</div>
                         </div>
                         {% endif %}
                         <hr>
                         <div class="row description-row">
                             <div class="col-sm-6">Summary:</div>
-                            <div class='col-sm-6'><span style="color: green">{{ character.summary.total_amount|format_currency }}</span> ISK</div>
+                            <div class='col-sm-6'><span style="color: green">{{ character.summary.total_amount|floatformat:0|intcomma }}</span> ISK</div>
                         </div>
                     </div>
                 </div>
                 <!--##############################DAILY#######################-->
                 <div class="tab-pane panel panel-default" id="tab-daily">
                     <div class="card-body modal-tab">
                         {% if character.bounty.total_amount_day %}
                         <div class="row description-row">
                             <div class="col-sm-6">Current Day - Ratting:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.bounty.total_amount_day|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.bounty.total_amount_day|floatformat:0|intcomma }}</span> ISK</div>
                         </div>
                         {% endif %}
                         <div class="row description-row">
                             <div class="col-sm-6">Avg. Ratting per Day:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.bounty.average_day|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.bounty.average_day|floatformat:0|intcomma }}</span> ISK</div>
                         </div>
                         <hr>
 
                         {% if character.ess.total_amount_day %}
                         <div class="row description-row">
                             <div class="col-sm-6">Current Day - ESS:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.ess.total_amount_day|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.ess.total_amount_day|floatformat:0|intcomma }}</span> ISK</div>
                         </div>
                         <div class="row description-row">
                             <div class="col-sm-6">Current Day - Stolen ESS:</div>
-                            <div class='col-sm-4'><span style="color: red">{{ character.stolen.average_day|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: red">{{ character.stolen.average_day|floatformat:0|intcomma }}</span> ISK</div>
                         </div>
                         {% endif %}
                         <div class="row description-row">
                             <div class="col-sm-6">Avg. ESS per Day:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.ess.average_day|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.ess.average_day|floatformat:0|intcomma }}</span> ISK</div>
                         </div>
                         <div class="row description-row">
                             <div class="col-sm-6">Avg. Stolen per Day:</div>
-                            <div class='col-sm-4'><span style="color: red">{{ character.stolen.average_day|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: red">{{ character.stolen.average_day|floatformat:0|intcomma }}</span> ISK</div>
                         </div>
                         {% if character.mining %}
                         <hr>
                         {% if character.mining.total_amount_day %}
                         <div class="row description-row">
                             <div class="col-sm-6">Current Day - Mining:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.mining.total_amount_day|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.mining.total_amount_day|floatformat:0|intcomma }}</span> ISK</div>
                         </div>
                         {% endif %}
                         <div class="row description-row">
                             <div class="col-sm-6">Avg. Mining per Day:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.mining.average_day|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.mining.average_day|floatformat:0|intcomma }}</span> ISK</div>
                         </div>
                         {% endif %}
 
                         {% if character.transaction %}
                         <hr>
                         {% if character.transaction.total_amount_day %}
                         <div class="row description-row">
                             <div class="col-sm-6">Current Day - Trading:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.transaction.total_amount_day|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.transaction.total_amount_day|floatformat:0|intcomma }}</span> ISK</div>
                         </div>
                         <div class="row description-row">
                             <div class="col-sm-6">Current Day - Trading Cost:</div>
-                            <div class='col-sm-4'><span style="color: red">{{ character.market_cost.total_amount_day|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: red">{{ character.market_cost.total_amount_day|floatformat:0|intcomma }}</span> ISK</div>
                         </div>
                         {% endif %}
                         <div class="row description-row">
                             <div class="col-sm-6">Avg. Trading per Day:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.transaction.average_day|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.transaction.average_day|floatformat:0|intcomma }}</span> ISK</div>
                         </div>
                         <div class="row description-row">
                             <div class="col-sm-6">Avg. Trading Cost per Day:</div>
-                            <div class='col-sm-4'><span style="color: red">{{ character.market_cost.average_day|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: red">{{ character.market_cost.average_day|floatformat:0|intcomma }}</span> ISK</div>
                         </div>
                         {% endif %}
 
                         {% if character.contract %}
                         <hr>
                         {% if character.contract.total_amount_day %}
                         <div class="row description-row">
                             <div class="col-sm-6">Current Day - Contracts:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.contract.total_amount_day|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.contract.total_amount_day|floatformat:0|intcomma }}</span> ISK</div>
                         </div>
                         {% endif %}
                         <div class="row description-row">
                             <div class="col-sm-6">Avg. Contracts per Day:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.contract.average_day|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.contract.average_day|floatformat:0|intcomma }}</span> ISK</div>
                         </div>
                         {% endif %}
 
                         {% if character.donation %}
                         <hr>
                         {% if character.donation.total_amount_day %}
                         <div class="row description-row">
                             <div class="col-sm-6">Current Day - Donations:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.donation.total_amount_day|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.donation.total_amount_day|floatformat:0|intcomma }}</span> ISK</div>
                         </div>
                         {% endif %}
                         <div class="row description-row">
                             <div class="col-sm-6">Avg. Donations per Day:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.donation.average_day|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.donation.average_day|floatformat:0|intcomma }}</span> ISK</div>
                         </div>
                         {% endif %}
 
                         {% if character.production_cost %}
                         <hr>
                         {% if character.production_cost.total_amount_day %}
                         <div class="row description-row">
                             <div class="col-sm-6">Current Day - Production Cost:</div>
-                            <div class='col-sm-4'><span style="color: red">{{ character.production_cost.total_amount_day|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: red">{{ character.production_cost.total_amount_day|floatformat:0|intcomma }}</span> ISK</div>
                         </div>
                         {% endif %}
                         <div class="row description-row">
                             <div class="col-sm-6">Avg. Production Cost per Day:</div>
-                            <div class='col-sm-4'><span style="color: red">{{ character.production_cost.average_day|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: red">{{ character.production_cost.average_day|floatformat:0|intcomma }}</span> ISK</div>
                         </div>
                         {% endif %}
                         {% if character.date %}
                         <hr>
                         <div class="row description-row">
                             <div class="col-sm-6">Summary Day</div>
-                            <div class='col-sm-6'><span style="color: green">{{ character.summary.total_amount_day|format_currency }}</span> ISK</div>
+                            <div class='col-sm-6'><span style="color: green">{{ character.summary.total_amount_day|floatformat:0|intcomma }}</span> ISK</div>
                         </div>
                         {% endif %}
                     </div>
                 </div>
                 <!--############################## HOURLY #######################-->
                 <div class="tab-pane panel panel-default" id="tab-hourly">
                     <div class="card-body modal-tab">
                         <div class="row description-row">
                             <div class="col-sm-6">Avg. Ratting per Hour:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.bounty.average_hour|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.bounty.average_hour|floatformat:0|intcomma }}</span> ISK</div>
                         </div>
                         <hr>
                         <div class="row description-row">
                             <div class="col-sm-6">Avg. ESS per Hour:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.bounty.average_hour|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.bounty.average_hour|floatformat:0|intcomma }}</span> ISK</div>
                         </div>
                         <div class="row description-row">
                             <div class="col-sm-6">Avg. Stolen per Hour:</div>
-                            <div class='col-sm-4'><span style="color: red">{{ character.stolen.average_hour|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: red">{{ character.stolen.average_hour|floatformat:0|intcomma }}</span> ISK</div>
                         </div>
 
                         {% if character.mining %}
                         <div class="row description-row">
                             <div class="col-sm-6">Avg. Mining per Hour:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.mining.average_hour|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.mining.average_hour|floatformat:0|intcomma }}</span> ISK</div>
                         </div>
                         {% endif %}
 
                         {% if character.transaction %}
                         <hr>
                         <div class="row description-row">
                             <div class="col-sm-6">Avg. Trading per Hour:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.transaction.average_hour|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.transaction.average_hour|floatformat:0|intcomma }}</span> ISK</div>
                         </div>
                         <div class="row description-row">
                             <div class="col-sm-6">Avg. Trading Cost per Hour:</div>
-                            <div class='col-sm-4'><span style="color: red">{{ character.market_cost.average_hour|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: red">{{ character.market_cost.average_hour|floatformat:0|intcomma }}</span> ISK</div>
                         </div>
                         {% endif %}
 
                         {% if character.contract %}
                         <hr>
                         <div class="row description-row">
                             <div class="col-sm-6">Avg. Contracts per Hour:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.contract.average_hour|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.contract.average_hour|floatformat:0|intcomma }}</span> ISK</div>
                         </div>
                         {% endif %}
 
                         {% if character.donation %}
                         <hr>
                         <div class="row description-row">
                             <div class="col-sm-6">Avg. Donations per Hour:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.donation.average_hour|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.donation.average_hour|floatformat:0|intcomma }}</span> ISK</div>
                         </div>
                         {% endif %}
 
                         {% if character.production_cost %}
                         <hr>
                         <div class="row description-row">
                             <div class="col-sm-6">Avg. Production Cost per Hour:</div>
-                            <div class='col-sm-4'><span style="color: red">{{ character.production_cost.average_hour|format_currency }}</span> ISK</div>
+                            <div class='col-sm-4'><span style="color: red">{{ character.production_cost.average_hour|floatformat:0|intcomma }}</span> ISK</div>
                         </div>
                         {% endif %}
                         {% if character.date %}
                         <hr>
                         <div class="row description-row">
                             <div class="col-sm-6">Summary Hour</div>
-                            <div class='col-sm-6'><span style="color: green">{{ character.summary.total_amount_hour|format_currency }}</span> ISK</div>
+                            <div class='col-sm-6'><span style="color: green">{{ character.summary.total_amount_hour|floatformat:0|intcomma }}</span> ISK</div>
                         </div>
                         {% endif %}
                     </div>
                 </div>
             </div>
         </div>
         {% else %}
```

### Comparing `aa_ledger-0.3.8a1/ledger/view_helpers/core.py` & `aa_ledger-0.4.0/ledger/view_helpers/core.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8a1/ledger/views/pve.py` & `aa_ledger-0.4.0/ledger/views/pve.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 """PvE Views"""
 
 # Django
+from django.conf import settings
 from django.contrib.auth.decorators import login_required, permission_required
 from django.shortcuts import render
 
 # Voices of War
 from ledger.hooks import get_extension_logger
 
 logger = get_extension_logger(__name__)
 
 
 @login_required
 @permission_required("ledger.basic_access")
-def index_pve(request):
-    context = {"text": ""}
-    return render(request, "ledger/pve/index.html", context)
-
-
-@login_required
-@permission_required("ledger.basic_access")
 def ledger_index(request):
-    return render(request, "ledger/ledger/index.html")
+    context = {
+        "memberaudit": settings.LEDGER_MEMBERAUDIT_USE,
+    }
+    return render(request, "ledger/index.html", context=context)
 
 
 @login_required
 @permission_required("ledger.basic_access")
 def ratting_index(request):
-    return render(request, "ledger/ledger/corpledger/corp_ledger.html")
+    context = {
+        "memberaudit": settings.LEDGER_MEMBERAUDIT_USE,
+    }
+    return render(request, "ledger/corpledger/corp_ledger.html", context=context)
 
 
 @login_required
 @permission_required("ledger.basic_access")
 def ratting_char_index(request):
-    return render(request, "ledger/ledger/charledger/char_ledger.html")
+    context = {
+        "memberaudit": settings.LEDGER_MEMBERAUDIT_USE,
+    }
+    return render(request, "ledger/charledger/char_ledger.html", context=context)
```

### Comparing `aa_ledger-0.3.8a1/ledger/views/character/char_audit.py` & `aa_ledger-0.4.0/ledger/views/character/char_audit.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         character=EveCharacter.objects.get_character_by_id(token.character_id)
     )
     update_character.apply_async(
         args=[token.character_id], kwargs={"force_refresh": True}, priority=6
     )
     msg = "Char successfully added/updated to Ledger"
     messages.info(request, msg)
-    return render(request, "ledger/ledger/index.html")
+    return render(request, "ledger/index.html")
 
 
 @login_required
 @permission_required(["ledger.admin_access", "ledger.char_audit_admin_access"])
 def fetch_memberaudit(request):
     """Add All Chars from Memberaudit to CharacterAudit"""
     try:
@@ -79,8 +79,8 @@
         messages.error(request, msg)
 
     except Exception as e:  # pylint: disable=broad-exception-caught
         logger.error(e, exc_info=True)
         msg = "An error occurred: Please inform your Admin."
         messages.error(request, msg)
 
-    return render(request, "ledger/ledger/index.html")
+    return render(request, "ledger/index.html")
```

### Comparing `aa_ledger-0.3.8a1/ledger/views/corporation/corp_audit.py` & `aa_ledger-0.4.0/ledger/views/corporation/corp_audit.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,8 +29,8 @@
 
     CorporationAudit.objects.update_or_create(corporation=corp)
     update_corp.apply_async(
         args=[char.corporation_id], kwargs={"force_refresh": True}, priority=6
     )
     msg = f"{char.corporation_name} successfully added/updated to Ledger"
     messages.info(request, msg)
-    return render(request, "ledger/ledger/index.html")
+    return render(request, "ledger/index.html")
```

### Comparing `aa_ledger-0.3.8a1/ledger/views/corporation/corp_events.py` & `aa_ledger-0.4.0/ledger/views/corporation/corp_events.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8a1/ledger/views/corporation/corp_tax.py` & `aa_ledger-0.4.0/ledger/views/corporation/corp_tax.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8a1/LICENSE` & `aa_ledger-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8a1/README.md` & `aa_ledger-0.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -86,14 +86,16 @@
 
 ### Step 6 - (Optional) Setting up Compatibilies<a name="step6"></a>
 
 The Following Settings can be setting up in the `local.py`
 
 - LEDGER_APP_NAME:          `"YOURNAME"`   - Set the name of the APP
 
+- LEDGER_CORP_TAX:          `15`   - Set Tax Value for ESS Payout Calculation
+
 - LEDGER_LOGGER_USE:        `True / False` - Set to use own Logger File
 
 - LEDGER_MEMBERAUDIT_USE:   `True / False` - Set to use the Memberaudit Journal to Fetch Statistics
 
 - LEDGER_CORPSTATS_TWO:     `True / False` - Set to use Corp Stats Two APP to Fetch Members that are not registred
 
 If you set up LEDGER_LOGGER_USE to `True` you need to add the following code below:
```

### Comparing `aa_ledger-0.3.8a1/pyproject.toml` & `aa_ledger-0.4.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 build-backend = "hatchling.build"
 requires = [
     "hatchling",
 ]
 
 [project]
 name = "aa-ledger"
-description = "EVE Online - Character/Corporation Ledger"
+description = "Character/Corporation Ledger"
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [
     { name = "Geuthur", email = "devgeuthur@gmail.com" },
 ]
 requires-python = ">=3.8"
 classifiers = [
@@ -30,15 +30,15 @@
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
 ]
 dynamic = [
     "version",
 ]
 dependencies = [
-    "allianceauth>=4",
+    "allianceauth<5,>=4",
     "allianceauth-app-utils>=1.19",
     "dacite",
     "django-eveuniverse>=1.3",
     "django-ninja",
 ]
 optional-dependencies.tests-allianceauth-latest = [
     "coverage",
```

### Comparing `aa_ledger-0.3.8a1/PKG-INFO` & `aa_ledger-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.3
 Name: aa-ledger
-Version: 0.3.8a1
-Summary: EVE Online - Character/Corporation Ledger
+Version: 0.4.0
+Summary: Character/Corporation Ledger
 Project-URL: Changelog, https://github.com/Geuthur/aa-ledger/blob/master/CHANGELOG.md
 Project-URL: Homepage, https://github.com/Geuthur/aa-ledger
 Project-URL: Source, https://github.com/Geuthur/aa-ledger
 Project-URL: Tracker, https://github.com/Geuthur/aa-ledger/issues
 Author-email: Geuthur <devgeuthur@gmail.com>
 License: MIT License
         
@@ -42,15 +42,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Requires-Dist: allianceauth-app-utils>=1.19
-Requires-Dist: allianceauth>=4
+Requires-Dist: allianceauth<5,>=4
 Requires-Dist: dacite
 Requires-Dist: django-eveuniverse>=1.3
 Requires-Dist: django-ninja
 Provides-Extra: tests-allianceauth-latest
 Requires-Dist: coverage; extra == 'tests-allianceauth-latest'
 Requires-Dist: django-webtest; extra == 'tests-allianceauth-latest'
 Description-Content-Type: text/markdown
@@ -143,14 +143,16 @@
 
 ### Step 6 - (Optional) Setting up Compatibilies<a name="step6"></a>
 
 The Following Settings can be setting up in the `local.py`
 
 - LEDGER_APP_NAME:          `"YOURNAME"`   - Set the name of the APP
 
+- LEDGER_CORP_TAX:          `15`   - Set Tax Value for ESS Payout Calculation
+
 - LEDGER_LOGGER_USE:        `True / False` - Set to use own Logger File
 
 - LEDGER_MEMBERAUDIT_USE:   `True / False` - Set to use the Memberaudit Journal to Fetch Statistics
 
 - LEDGER_CORPSTATS_TWO:     `True / False` - Set to use Corp Stats Two APP to Fetch Members that are not registred
 
 If you set up LEDGER_LOGGER_USE to `True` you need to add the following code below:
```

