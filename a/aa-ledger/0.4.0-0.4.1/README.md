# Comparing `tmp/aa_ledger-0.4.0.tar.gz` & `tmp/aa_ledger-0.4.1.tar.gz`

## Comparing `aa_ledger-0.4.0.tar` & `aa_ledger-0.4.1.tar`

### file list

```diff
@@ -1,80 +1,80 @@
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/__init__.py
--rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/admin.py
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/app_settings.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/apps.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/auth_hooks.py
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/decorators.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/errors.py
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/hooks.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/providers.py
--rw-r--r--   0        0        0     4956 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/tasks.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/urls.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/api/__init__.py
--rw-r--r--   0        0        0     7470 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/api/helpers.py
--rw-r--r--   0        0        0    22614 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/api/ledgermanager.py
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/api/schema.py
--rw-r--r--   0        0        0    16190 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/api/templatemanager.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/api/character/__init__.py
--rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/api/character/ledger.py
--rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/api/character/template.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/api/corporation/__init__.py
--rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/api/corporation/ledger.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/api/corporation/template.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/locate/__init__.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/locate/de.po
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/managers/charaudit_manager.py
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/managers/corpaudit_manager.py
--rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/managers/general_manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/migrations/__init__.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/models/__init__.py
--rw-r--r--   0        0        0     5771 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/models/characteraudit.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/models/corporationaudit.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/models/events.py
--rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/models/general.py
--rw-r--r--   0        0        0     5416 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/static/ledger/css/billboards_dark.css
--rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/static/ledger/css/cards.css
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/static/ledger/css/custom.css
--rw-r--r--   0        0        0   236145 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/static/ledger/guides/ledger-1.png
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/static/ledger/guides/ledger-2.png
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/static/ledger/guides/ledger-3.png
--rw-r--r--   0        0        0    43262 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/static/ledger/images/Spinner-1s-64px-dark.gif
--rw-r--r--   0        0        0    43381 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/static/ledger/images/Spinner-1s-64px-light.gif
--rw-r--r--   0        0        0    22096 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/static/ledger/js/charledger.js
--rw-r--r--   0        0        0    18853 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/static/ledger/js/corpledger.js
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/static/ledger/js/img.js
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/task_helpers/__init__.py
--rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/task_helpers/char_helpers.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/task_helpers/core_helpers.py
--rw-r--r--   0        0        0     8398 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/task_helpers/corp_helpers.py
--rw-r--r--   0        0        0     8434 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/task_helpers/etag_helpers.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/templates/ledger/base.html
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/templates/ledger/error.html
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/templates/ledger/index.html
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/templates/ledger/menu.html
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/templates/ledger/bundles/ledger-css.html
--rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/templates/ledger/charledger/char_ledger.html
--rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/templates/ledger/charledger/month.html
--rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/templates/ledger/charledger/year.html
--rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/templates/ledger/corpledger/corp_ledger.html
--rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/templates/ledger/corpledger/month.html
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/templates/ledger/corpledger/year.html
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/templates/ledger/modals/modal-full.html
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/templates/ledger/modals/modal-xl.html
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/templates/ledger/modals/modal.html
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/templates/ledger/modals/modal_dialog.html
--rw-r--r--   0        0        0    17987 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/templates/ledger/modals/pve/view_character_content.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/templatetags/__init__.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/templatetags/ledger.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/view_helpers/__init__.py
--rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/view_helpers/core.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/views/__init__.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/views/pve.py
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/views/character/char_audit.py
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/views/corporation/corp_audit.py
--rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/views/corporation/corp_events.py
--rw-r--r--   0        0        0     8919 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/ledger/views/corporation/corp_tax.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/LICENSE
--rw-r--r--   0        0        0     5602 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/README.md
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     8381 2020-02-02 00:00:00.000000 aa_ledger-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/__init__.py
+-rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/admin.py
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/app_settings.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/apps.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/auth_hooks.py
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/decorators.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/errors.py
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/hooks.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/providers.py
+-rw-r--r--   0        0        0     4956 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/tasks.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/urls.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/api/__init__.py
+-rw-r--r--   0        0        0     7394 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/api/helpers.py
+-rw-r--r--   0        0        0    23759 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/api/ledgermanager.py
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/api/schema.py
+-rw-r--r--   0        0        0    16151 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/api/templatemanager.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/api/character/__init__.py
+-rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/api/character/ledger.py
+-rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/api/character/template.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/api/corporation/__init__.py
+-rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/api/corporation/ledger.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/api/corporation/template.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/locate/__init__.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/locate/de.po
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/managers/charaudit_manager.py
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/managers/corpaudit_manager.py
+-rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/managers/general_manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/migrations/__init__.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/models/__init__.py
+-rw-r--r--   0        0        0     5771 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/models/characteraudit.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/models/corporationaudit.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/models/events.py
+-rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/models/general.py
+-rw-r--r--   0        0        0     5416 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/static/ledger/css/billboards_dark.css
+-rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/static/ledger/css/cards.css
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/static/ledger/css/custom.css
+-rw-r--r--   0        0        0   236145 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/static/ledger/guides/ledger-1.png
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/static/ledger/guides/ledger-2.png
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/static/ledger/guides/ledger-3.png
+-rw-r--r--   0        0        0    43262 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/static/ledger/images/Spinner-1s-64px-dark.gif
+-rw-r--r--   0        0        0    43381 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/static/ledger/images/Spinner-1s-64px-light.gif
+-rw-r--r--   0        0        0    22096 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/static/ledger/js/charledger.js
+-rw-r--r--   0        0        0    18853 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/static/ledger/js/corpledger.js
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/static/ledger/js/img.js
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/task_helpers/__init__.py
+-rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/task_helpers/char_helpers.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/task_helpers/core_helpers.py
+-rw-r--r--   0        0        0     8398 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/task_helpers/corp_helpers.py
+-rw-r--r--   0        0        0     8434 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/task_helpers/etag_helpers.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/templates/ledger/base.html
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/templates/ledger/error.html
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/templates/ledger/index.html
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/templates/ledger/menu.html
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/templates/ledger/bundles/ledger-css.html
+-rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/templates/ledger/charledger/char_ledger.html
+-rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/templates/ledger/charledger/month.html
+-rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/templates/ledger/charledger/year.html
+-rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/templates/ledger/corpledger/corp_ledger.html
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/templates/ledger/corpledger/month.html
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/templates/ledger/corpledger/year.html
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/templates/ledger/modals/modal-full.html
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/templates/ledger/modals/modal-xl.html
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/templates/ledger/modals/modal.html
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/templates/ledger/modals/modal_dialog.html
+-rw-r--r--   0        0        0    20050 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/templates/ledger/modals/pve/view_character_content.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/templatetags/__init__.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/templatetags/ledger.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/view_helpers/__init__.py
+-rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/view_helpers/core.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/views/__init__.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/views/pve.py
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/views/character/char_audit.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/views/corporation/corp_audit.py
+-rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/views/corporation/corp_events.py
+-rw-r--r--   0        0        0     8919 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/views/corporation/corp_tax.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/LICENSE
+-rw-r--r--   0        0        0     5633 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/README.md
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     8412 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/PKG-INFO
```

### Comparing `aa_ledger-0.4.0/ledger/admin.py` & `aa_ledger-0.4.1/ledger/admin.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/app_settings.py` & `aa_ledger-0.4.1/ledger/app_settings.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/auth_hooks.py` & `aa_ledger-0.4.1/ledger/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/decorators.py` & `aa_ledger-0.4.1/ledger/decorators.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/hooks.py` & `aa_ledger-0.4.1/ledger/hooks.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/tasks.py` & `aa_ledger-0.4.1/ledger/tasks.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/urls.py` & `aa_ledger-0.4.1/ledger/urls.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/api/__init__.py` & `aa_ledger-0.4.1/ledger/api/__init__.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/api/helpers.py` & `aa_ledger-0.4.1/ledger/api/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,29 +49,27 @@
                 CharacterMiningLedgerEntry as CharacterMiningLedger,
             )
             from memberaudit.models import CharacterWalletJournalEntry
 
             return (
                 CharacterMiningLedger,
                 CharacterWalletJournalEntry,
-                "character__eve_character",
             )
         except Exception as exc:
             logger.error("Memberaudit is enabled but not installed")
             raise LedgerImportError("Memberaudit is enabled but not installed") from exc
 
     from ledger.models.characteraudit import (
         CharacterMiningLedger,
         CharacterWalletJournalEntry,
     )
 
     return (
         CharacterMiningLedger,
         CharacterWalletJournalEntry,
-        "character__character",
     )
 
 
 def get_main_character(request, character_id):
     perms = True
 
     main_char = EveCharacter.objects.select_related(
```

### Comparing `aa_ledger-0.4.0/ledger/api/ledgermanager.py` & `aa_ledger-0.4.1/ledger/api/ledgermanager.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from ledger.api.helpers import get_models_and_string
 from ledger.hooks import get_extension_logger
 from ledger.models.corporationaudit import CorporationWalletJournalEntry
 from ledger.view_helpers.core import events_filter
 
 logger = get_extension_logger(__name__)
 
-CharacterMiningLedger, CharacterWalletJournalEntry, SR_CHAR = get_models_and_string()
+CharacterMiningLedger, CharacterWalletJournalEntry = get_models_and_string()
 
 
 class LedgerDataCore:
     """LedgerDataCore class to store the core data."""
 
     def __init__(self):
         self.total_bounty = 0
@@ -53,24 +53,14 @@
     def __init__(
         self, character_journal=None, corporation_journal=None, mining_journal=None
     ):
         self.char_journal = character_journal
         self.corp_journal = corporation_journal
         self.mining_journal = mining_journal
 
-    def to_values(self, journal):
-        logger.debug(type(journal))
-        return journal.values(
-            "amount", "ref_type", "first_party_id", "second_party_id", "date"
-        )
-
-    def to_values_mining(self, journal):
-        logger.debug(type(journal))
-        return journal.values("total", "date")
-
 
 class LedgerDate:
     """LedgerDate class to store the date data."""
 
     def __init__(self, year, month):
         self.year = year
         self.month = month
@@ -279,32 +269,30 @@
         chars = [char.character_id for char in self.chars]
 
         entries_filter = Q(second_party_id__in=chars) | Q(first_party_id__in=chars)
 
         # Filter the entries for the current day/month
         character_journal = CharacterWalletJournalEntry.objects.filter(
             filters, filter_date
-        ).select_related("first_party", "second_party", SR_CHAR)
+        ).select_related("first_party", "second_party")
 
         corporation_journal = CorporationWalletJournalEntry.objects.filter(
             entries_filter, filter_date
         ).select_related(
             "division",
             "division__corporation",
             "division__corporation__corporation",
             "first_party",
             "second_party",
         )
 
         # Exclude Events to avoid wrong stats
         corporation_journal = events_filter(corporation_journal)
         mining_journal = (
-            CharacterMiningLedger.objects.filter(filters, filter_date).select_related(
-                SR_CHAR
-            )
+            CharacterMiningLedger.objects.filter(filters, filter_date)
         ).annotate_pricing()
 
         self.process_character_chars(
             corporation_journal, character_journal, mining_journal
         )
 
         # Use Only Corporation Ledger
@@ -387,95 +375,134 @@
             "rattingbar": [],
             "workflowgauge": [],
         }
         self.date_billboard = ["x"]
 
     def aggregate_corp(self, journal, range_):
         """Aggregate the journal entries for the corporation."""
+        total_bounty = 0
+        total_ess_payout = 0
         for entry in journal:
             if entry["date"].year == self.date.year:
                 if (self.date.month == 0 and entry["date"].month == range_) or (
                     self.date.month != 0 and entry["date"].day == range_
                 ):
                     if self.is_corp:
                         if entry["ref_type"] == "bounty_prizes":
-                            self.data.total_bounty += entry["amount"]
+                            total_bounty += entry["amount"]
                     if entry["ref_type"] == "ess_escrow_transfer":
-                        self.data.total_ess_payout += entry["amount"]
+                        if self.is_corp:
+                            total_ess_payout += entry["amount"]
+                        else:
+                            total_ess_payout += (
+                                entry["amount"] / app_settings.LEDGER_CORP_TAX
+                            ) * (100 - app_settings.LEDGER_CORP_TAX)
+        return total_bounty, total_ess_payout
 
     def aggregate_char(self, journal, range_):
         """Aggregate the journal entries for the character."""
+        total_bounty = 0
+        total_miscellaneous = 0
+        total_isk = 0
+        total_cost = 0
+        total_market = 0
+        total_production_cost = 0
+
         for entry in journal:
             if entry["date"].year == self.date.year:
                 if (self.date.month == 0 and entry["date"].month == range_) or (
                     self.date.month != 0 and entry["date"].day == range_
                 ):
                     # Bounty Filter
                     if entry["ref_type"] == "bounty_prizes":
-                        self.data.total_bounty += entry["amount"]
+                        total_bounty += entry["amount"]
                     # Misc Filter
                     # TODO Add player_donation to the Billboard
                     if (
                         entry["ref_type"]
                         in [
                             "market_transaction",
                             "contract_price_payment_corp",
                             "contract_reward",
                             "contract_price",
                         ]
                         and entry["amount"] > 0
                     ):
-                        self.data.total_miscellaneous += entry["amount"]
+                        total_miscellaneous += entry["amount"]
                     # Total ISK
                     if entry["amount"] > 0:
-                        self.data.total_isk += entry["amount"]
+                        total_isk += entry["amount"]
                     else:
-                        self.data.total_cost += entry["amount"]
+                        total_cost += entry["amount"]
                     # Total Market
                     if entry["ref_type"] in [
                         "market_escrow",
                         "transaction_tax",
                         "market_provider_tax",
                         "brokers_fee",
                     ]:
-                        self.data.total_market += entry["amount"]
+                        total_market += entry["amount"]
                     # Production Cost
                     if entry["ref_type"] in ["industry_job_tax", "manufacturing"]:
-                        self.data.total_production_cost += entry["amount"]
+                        total_production_cost += entry["amount"]
+        return (
+            total_bounty,
+            total_miscellaneous,
+            total_isk,
+            total_cost,
+            total_market,
+            total_production_cost,
+        )
 
     def aggregate_mining(self, journal, range_):
         """Aggregate the journal entries for the mining."""
+        total_mining = 0
         for entry in journal:
             if entry["date"].year == self.date.year:
                 if (self.date.month == 0 and entry["date"].month == range_) or (
                     self.date.month != 0 and entry["date"].day == range_
                 ):
-                    self.data.total_mining += entry["total"]
+                    total_mining += entry["total"]
+        return total_mining
 
     # pylint: disable=too-many-branches
     def process_day(
         self, range_, corp_journal=None, char_journal=None, mining_journal=None
     ):
         """Process the day for the journal entries."""
         date = datetime.now()
 
-        # Reset the values
-        self.data.reset_values()
-
         if self.date.monthly:
             date = date.replace(day=1)
 
-        logger.debug(self.date.month)
-
         if corp_journal:
-            self.aggregate_corp(corp_journal, range_)
+            total_bounty, total_ess = self.aggregate_corp(corp_journal, range_)
+            self.data.total_bounty = total_bounty
+            self.data.total_ess_payout = total_ess
         if char_journal:
-            self.aggregate_char(char_journal, range_)
+            (
+                total_bounty,
+                total_miscellaneous,
+                total_isk,
+                total_cost,
+                total_market,
+                total_production_cost,
+            ) = self.aggregate_char(char_journal, range_)
+
+            self.data.total_bounty = total_bounty
+            self.data.total_miscellaneous = total_miscellaneous
+            # Wallet Charts
+            self.data.total_isk += total_isk
+            self.data.total_cost += total_cost
+            self.data.total_market += total_market
+            self.data.total_production_cost += total_production_cost
+
         if mining_journal:
-            self.aggregate_mining(mining_journal, range_)
+            total_mining = self.aggregate_mining(mining_journal, range_)
+            self.data.total_mining = total_mining
 
         # Add the totals to the respective lists
         self.sum.sum_amount.append(int(self.data.total_bounty))
         self.sum.sum_amount_ess.append(int(self.data.total_ess_payout))
         if not self.is_corp:
             self.sum.sum_amount_misc.append(int(self.data.total_miscellaneous))
             self.sum.sum_amount_mining.append(int(self.data.total_mining))
@@ -549,21 +576,26 @@
         misc_cost = abs(
             self.data.total_cost
             - self.data.total_production_cost
             - self.data.total_market
         )
         wallet_chart_data = [
             # Earns
-            ["Earns", int(self.data.total_isk)],
+            ["Income", int(self.data.total_isk)],
             # ["Ratting", int(total_sum_ratting)],  ["Mining", int(total_sum_mining)], ["Misc.", int(total_sum_misc)],
             # Costs
             ["Market Cost", int(abs(self.data.total_market))],
             ["Production Cost", int(abs(self.data.total_production_cost))],
-            ["Misc. Costs", int(misc_cost)],
+            ["Misc. Cost", int(misc_cost)],
         ]
+        logger.error(self.data.total_cost)
+        logger.error(self.data.total_production_cost)
+        logger.error(self.data.total_market)
+        logger.error(wallet_chart_data)
+
         self.billboard_dict["walletcharts"] = (
             wallet_chart_data
             if any(item[1] != 0 for item in wallet_chart_data)
             else None
         )
 
     # Generate Charts Billboard for Corporation Wallets
```

### Comparing `aa_ledger-0.4.0/ledger/api/schema.py` & `aa_ledger-0.4.1/ledger/api/schema.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/api/templatemanager.py` & `aa_ledger-0.4.1/ledger/api/templatemanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,30 +10,34 @@
     get_main_character,
     get_models_and_string,
 )
 from ledger.hooks import get_extension_logger
 from ledger.models.corporationaudit import CorporationWalletJournalEntry
 from ledger.view_helpers.core import calculate_days_year, events_filter
 
-CharacterMiningLedger, CharacterWalletJournalEntry, SR_CHAR = get_models_and_string()
+CharacterMiningLedger, CharacterWalletJournalEntry = get_models_and_string()
 
 logger = get_extension_logger(__name__)
 
 
 class TemplateFilterCore:
     """TemplateFilter class to store the filter data."""
 
     def __init__(self, char_id):
         self.char_id = char_id
         self.filter = Q(second_party_id__in=self.char_id) | Q(
             first_party_id__in=self.char_id
         )
         self.filter_bounty = self.filter & Q(ref_type="bounty_prizes")
         self.filter_ess = self.filter & Q(ref_type="ess_escrow_transfer")
-        self.filter_mining = Q(character__eve_character__character_id__in=self.char_id)
+        self.filter_mining = (
+            Q(character__character_id=char_id)
+            if app_settings.LEDGER_MEMBERAUDIT_USE
+            else Q(character__character__character_id__in=char_id)
+        )
 
 
 class TemplateFilterCost(TemplateFilterCore):
     """TemplateFilter class to store the filter data."""
 
     def __init__(self, char_id):
         super().__init__(char_id)
@@ -200,32 +204,28 @@
             filter_date &= Q(date__month=self.data.month)
 
         chars = [char.character_id for char in self.chars]
 
         entries_filter = Q(second_party_id__in=chars) | Q(first_party_id__in=chars)
 
         # Filter the entries for the current day/month
-        character_journal = (
-            CharacterWalletJournalEntry.objects.filter(filters, filter_date)
-            .select_related("first_party", "second_party", SR_CHAR)
-            .order_by("-date")
-        )
+        character_journal = CharacterWalletJournalEntry.objects.filter(
+            filters, filter_date
+        ).select_related("first_party", "second_party")
 
         corporation_journal = (
             CorporationWalletJournalEntry.objects.filter(entries_filter, filter_date)
             .select_related("first_party", "second_party")
             .order_by("-date")
         )
 
         # Exclude Events to avoid wrong stats
         corporation_journal = events_filter(corporation_journal)
         mining_journal = (
             CharacterMiningLedger.objects.filter(filters, filter_date)
-            .select_related(SR_CHAR)
-            .order_by("-date")
         ).annotate_pricing()
 
         self._process_characters(character_journal, corporation_journal, mining_journal)
         logger.debug(self.template_dict)
         return self.template_dict
 
     def corporation_template(self):
@@ -343,14 +343,16 @@
                         date__hour=self.data.current_date.hour,
                     ),
                 ),
                 0,
                 output_field=DecimalField(),
             ),
         )
+        if self.data.month == 0:
+            result["total_amount_day"] = 0
         return result
 
     # Update Core Dict
     def _update_template_dict(self, char):
         main_name = char.character_name if not self.show_year else "Summary"
         main_id = char.character_id if not self.show_year else 0
         date = (
@@ -382,22 +384,20 @@
             {
                 key: {
                     sub_key: value
                     for sub_key, value in {
                         "total_amount": round(amounts[key]["total_amount"], 2),
                         "total_amount_day": (
                             round(amounts[key]["total_amount_day"], 2)
-                            if amounts[key]["total_amount_day"] is not None
-                            else None
                         ),
                         "total_amount_hour": (
                             round(amounts[key]["total_amount_hour"], 2)
                             if key != "mining"
-                            and amounts[key]["total_amount_hour"] is not None
-                            else None
+                            # Bad Fix but it works..
+                            else round(amounts[key]["total_amount_day"], 2)
                         ),
                         "average_day": round(
                             amounts[key]["total_amount"] / current_day, 2
                         ),
                         "average_hour": round(
                             (amounts[key]["total_amount"] / current_day) / 24, 2
                         ),
```

### Comparing `aa_ledger-0.4.0/ledger/api/character/ledger.py` & `aa_ledger-0.4.1/ledger/api/character/ledger.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/api/character/template.py` & `aa_ledger-0.4.1/ledger/api/character/template.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/api/corporation/ledger.py` & `aa_ledger-0.4.1/ledger/api/corporation/ledger.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/api/corporation/template.py` & `aa_ledger-0.4.1/ledger/api/corporation/template.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/locate/de.po` & `aa_ledger-0.4.1/ledger/locate/de.po`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/managers/charaudit_manager.py` & `aa_ledger-0.4.1/ledger/managers/charaudit_manager.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/managers/corpaudit_manager.py` & `aa_ledger-0.4.1/ledger/managers/corpaudit_manager.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/managers/general_manager.py` & `aa_ledger-0.4.1/ledger/managers/general_manager.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/models/characteraudit.py` & `aa_ledger-0.4.1/ledger/models/characteraudit.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/models/corporationaudit.py` & `aa_ledger-0.4.1/ledger/models/corporationaudit.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/models/events.py` & `aa_ledger-0.4.1/ledger/models/events.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/models/general.py` & `aa_ledger-0.4.1/ledger/models/general.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/static/ledger/css/billboards_dark.css` & `aa_ledger-0.4.1/ledger/static/ledger/css/billboards_dark.css`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/static/ledger/css/cards.css` & `aa_ledger-0.4.1/ledger/static/ledger/css/cards.css`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/static/ledger/css/custom.css` & `aa_ledger-0.4.1/ledger/static/ledger/css/custom.css`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/static/ledger/guides/ledger-1.png` & `aa_ledger-0.4.1/ledger/static/ledger/guides/ledger-1.png`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/static/ledger/guides/ledger-2.png` & `aa_ledger-0.4.1/ledger/static/ledger/guides/ledger-2.png`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/static/ledger/guides/ledger-3.png` & `aa_ledger-0.4.1/ledger/static/ledger/guides/ledger-3.png`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/static/ledger/images/Spinner-1s-64px-dark.gif` & `aa_ledger-0.4.1/ledger/static/ledger/images/Spinner-1s-64px-dark.gif`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/static/ledger/images/Spinner-1s-64px-light.gif` & `aa_ledger-0.4.1/ledger/static/ledger/images/Spinner-1s-64px-light.gif`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/static/ledger/js/charledger.js` & `aa_ledger-0.4.1/ledger/static/ledger/js/charledger.js`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/static/ledger/js/corpledger.js` & `aa_ledger-0.4.1/ledger/static/ledger/js/corpledger.js`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/static/ledger/js/img.js` & `aa_ledger-0.4.1/ledger/static/ledger/js/img.js`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/task_helpers/char_helpers.py` & `aa_ledger-0.4.1/ledger/task_helpers/char_helpers.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/task_helpers/core_helpers.py` & `aa_ledger-0.4.1/ledger/task_helpers/core_helpers.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/task_helpers/corp_helpers.py` & `aa_ledger-0.4.1/ledger/task_helpers/corp_helpers.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/task_helpers/etag_helpers.py` & `aa_ledger-0.4.1/ledger/task_helpers/etag_helpers.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/templates/ledger/base.html` & `aa_ledger-0.4.1/ledger/templates/ledger/base.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/templates/ledger/error.html` & `aa_ledger-0.4.1/ledger/templates/ledger/error.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/templates/ledger/index.html` & `aa_ledger-0.4.1/ledger/templates/ledger/index.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/templates/ledger/menu.html` & `aa_ledger-0.4.1/ledger/templates/ledger/menu.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/templates/ledger/charledger/char_ledger.html` & `aa_ledger-0.4.1/ledger/templates/ledger/charledger/char_ledger.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/templates/ledger/charledger/month.html` & `aa_ledger-0.4.1/ledger/templates/ledger/charledger/month.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/templates/ledger/charledger/year.html` & `aa_ledger-0.4.1/ledger/templates/ledger/charledger/year.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/templates/ledger/corpledger/corp_ledger.html` & `aa_ledger-0.4.1/ledger/templates/ledger/corpledger/corp_ledger.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/templates/ledger/corpledger/month.html` & `aa_ledger-0.4.1/ledger/templates/ledger/corpledger/month.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/templates/ledger/corpledger/year.html` & `aa_ledger-0.4.1/ledger/templates/ledger/corpledger/year.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/templates/ledger/modals/modal-full.html` & `aa_ledger-0.4.1/ledger/templates/ledger/modals/modal-full.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/templates/ledger/modals/modal-xl.html` & `aa_ledger-0.4.1/ledger/templates/ledger/modals/modal-xl.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/templates/ledger/modals/modal.html` & `aa_ledger-0.4.1/ledger/templates/ledger/modals/modal.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/templates/ledger/modals/modal_dialog.html` & `aa_ledger-0.4.1/ledger/templates/ledger/modals/modal_dialog.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/templates/ledger/modals/pve/view_character_content.html` & `aa_ledger-0.4.1/ledger/templates/ledger/modals/pve/view_character_content.html`

 * *Files 6% similar despite different names*

```diff
@@ -24,263 +24,302 @@
                 <li>
                     <button class="nav-link" href="#tab-hourly" data-bs-toggle="tab">Hourly</button>
                 </li>
             </ul>
             <div class="border border-secondary rounded-bottom tab-content px-2">
                 <div class="tab-pane panel panel-default active" id="tab-summary">
                     <div class="card-body modal-tab">
-                        <div class="row description-row">
-                            <div class="col-sm-6">Ratting:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.bounty.total_amount|floatformat:0|intcomma }}</span> ISK</div>
-                        </div>
-                        <div class="row description-row">
-                            <div class="col-sm-6">ESS:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.ess.total_amount|floatformat:0|intcomma }}</span> ISK</div>
-                        </div>
-                        <div class="row description-row">
-                            <div class="col-sm-6">Stolen ESS:</div>
-                            <div class='col-sm-6'><span style="color: red">{{ character.stolen.total_amount|floatformat:0|intcomma }}</span> ISK</div>
-                        </div>
+                        {% if character.bounty %}
+                            <div class="row description-row">
+                                <div class="col-sm-6">Ratting:</div>
+                                <div class='col-sm-4'><span style="color: green">{{ character.bounty.total_amount|floatformat:0|intcomma }}</span> ISK</div>
+                            </div>
+                        {% endif %}
+
+                        {% if character.ess %}
+                            <div class="row description-row">
+                                <div class="col-sm-6">ESS:</div>
+                                <div class='col-sm-4'><span style="color: green">{{ character.ess.total_amount|floatformat:0|intcomma }}</span> ISK</div>
+                            </div>
+                        {% endif %}
+
+                        {% if character.stolen %}
+                            <div class="row description-row">
+                                <div class="col-sm-6">Stolen ESS:</div>
+                                <div class='col-sm-6'><span style="color: red">{{ character.stolen.total_amount|floatformat:0|intcomma }}</span> ISK</div>
+                            </div>
+                        {% endif %}
+
                         {% if character.mining %}
-                        <hr>
-                        <div class="row description-row">
-                            <div class="col-sm-6">Mining:</div>
-                            <div class='col-sm-6'><span style="color: green">{{ character.mining.total_amount|floatformat:0|intcomma }}</span> ISK</div>
-                        </div>
+                            <hr>
+                            <div class="row description-row">
+                                <div class="col-sm-6">Mining:</div>
+                                <div class='col-sm-6'><span style="color: green">{{ character.mining.total_amount|floatformat:0|intcomma }}</span> ISK</div>
+                            </div>
                         {% endif %}
+
                         {% if character.transaction %}
-                        <hr>
-                        <div class="row description-row">
-                            <div class="col-sm-6">Trading:</div>
-                            <div class='col-sm-6'><span style="color: green">{{ character.transaction.total_amount|floatformat:0|intcomma }}</span> ISK</div>
-                        </div>
-                        <div class="row description-row">
-                            <div class="col-sm-6">Trading Cost:</div>
-                            <div class='col-sm-6'><span style="color: red">{{ character.market_cost.total_amount|floatformat:0|intcomma }}</span> ISK</div>
-                        </div>
+                            <hr>
+                            <div class="row description-row">
+                                <div class="col-sm-6">Trading:</div>
+                                <div class='col-sm-6'><span style="color: green">{{ character.transaction.total_amount|floatformat:0|intcomma }}</span> ISK</div>
+                            </div>
+                            <div class="row description-row">
+                                <div class="col-sm-6">Trading Cost:</div>
+                                <div class='col-sm-6'><span style="color: red">{{ character.market_cost.total_amount|floatformat:0|intcomma }}</span> ISK</div>
+                            </div>
                         {% endif %}
+
                         {% if character.contract %}
-                        <hr>
-                        <div class="row description-row">
-                            <div class="col-sm-6">Contracts:</div>
-                            <div class='col-sm-6'><span style="color: green">{{ character.contract.total_amount|floatformat:0|intcomma }}</span> ISK</div>
-                        </div>
+                            <hr>
+                            <div class="row description-row">
+                                <div class="col-sm-6">Contracts:</div>
+                                <div class='col-sm-6'><span style="color: green">{{ character.contract.total_amount|floatformat:0|intcomma }}</span> ISK</div>
+                            </div>
                         {% endif %}
+
                         {% if character.donation %}
-                        <hr>
-                        <div class="row description-row">
-                            <div class="col-sm-6">Donations:<br>
-                            <span style="color: #FFBF00"><!--<i class="fas fa-exclamation-triangle"></i> Excluded from summary <i class="fas fa-exclamation-triangle"></i>--></span>
-                            </div>
-                            <div class='col-sm-6'>
-                                <span style="color: green">
-                                    {{ character.donation.total_amount|floatformat:0|intcomma }}
-                                </span> ISK
-                                    <br><span style="color: #3483eb"><!--<i class="fas fa-info-circle"></i> Exluded registered chars <i class="fas fa-info-circle"></i>--></span>
+                            <hr>
+                            <div class="row description-row">
+                                <div class="col-sm-6">Donations:<br>
+                                <span style="color: #FFBF00"><!--<i class="fas fa-exclamation-triangle"></i> Excluded from summary <i class="fas fa-exclamation-triangle"></i>--></span>
+                                </div>
+                                <div class='col-sm-6'>
+                                    <span style="color: green">
+                                        {{ character.donation.total_amount|floatformat:0|intcomma }}
+                                    </span> ISK
+                                        <br><span style="color: #3483eb"><!--<i class="fas fa-info-circle"></i> Exluded registered chars <i class="fas fa-info-circle"></i>--></span>
+                                </div>
                             </div>
-                        </div>
                         {% endif %}
+
                         {% if character.production_cost %}
-                        <hr>
-                        <div class="row description-row">
-                            <div class="col-sm-6">Production Cost:</div>
-                            <div class='col-sm-6'><span style="color: red">{{ character.production_cost.total_amount|floatformat:0|intcomma }}</span> ISK</div>
-                        </div>
+                            <hr>
+                            <div class="row description-row">
+                                <div class="col-sm-6">Production Cost:</div>
+                                <div class='col-sm-6'><span style="color: red">{{ character.production_cost.total_amount|floatformat:0|intcomma }}</span> ISK</div>
+                            </div>
                         {% endif %}
                         <hr>
                         <div class="row description-row">
                             <div class="col-sm-6">Summary:</div>
                             <div class='col-sm-6'><span style="color: green">{{ character.summary.total_amount|floatformat:0|intcomma }}</span> ISK</div>
                         </div>
                     </div>
                 </div>
                 <!--##############################DAILY#######################-->
                 <div class="tab-pane panel panel-default" id="tab-daily">
                     <div class="card-body modal-tab">
-                        {% if character.bounty.total_amount_day %}
-                        <div class="row description-row">
-                            <div class="col-sm-6">Current Day - Ratting:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.bounty.total_amount_day|floatformat:0|intcomma }}</span> ISK</div>
-                        </div>
+                        {% if character.bounty %}
+                            {% if character.bounty.total_amount_day %}
+                                <div class="row description-row">
+                                    <div class="col-sm-6">Current Day - Ratting:</div>
+                                    <div class='col-sm-4'><span style="color: green">{{ character.bounty.total_amount_day|floatformat:0|intcomma }}</span> ISK</div>
+                                </div>
+                            {% endif %}
+                            <div class="row description-row">
+                                <div class="col-sm-6">Avg. Ratting per Day:</div>
+                                <div class='col-sm-4'><span style="color: green">{{ character.bounty.average_day|floatformat:0|intcomma }}</span> ISK</div>
+                            </div>
                         {% endif %}
-                        <div class="row description-row">
-                            <div class="col-sm-6">Avg. Ratting per Day:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.bounty.average_day|floatformat:0|intcomma }}</span> ISK</div>
-                        </div>
-                        <hr>
 
-                        {% if character.ess.total_amount_day %}
-                        <div class="row description-row">
-                            <div class="col-sm-6">Current Day - ESS:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.ess.total_amount_day|floatformat:0|intcomma }}</span> ISK</div>
-                        </div>
-                        <div class="row description-row">
-                            <div class="col-sm-6">Current Day - Stolen ESS:</div>
-                            <div class='col-sm-4'><span style="color: red">{{ character.stolen.average_day|floatformat:0|intcomma }}</span> ISK</div>
-                        </div>
+                        {% if character.ess %}
+                            {% if character.ess.total_amount_day %}
+                                <div class="row description-row">
+                                    <div class="col-sm-6">Current Day - ESS:</div>
+                                    <div class='col-sm-4'><span style="color: green">{{ character.ess.total_amount_day|floatformat:0|intcomma }}</span> ISK</div>
+                                </div>
+                            {% endif %}
+                            <div class="row description-row">
+                                <div class="col-sm-6">Avg. ESS per Day:</div>
+                                <div class='col-sm-4'><span style="color: green">{{ character.ess.average_day|floatformat:0|intcomma }}</span> ISK</div>
+                            </div>
                         {% endif %}
-                        <div class="row description-row">
-                            <div class="col-sm-6">Avg. ESS per Day:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.ess.average_day|floatformat:0|intcomma }}</span> ISK</div>
-                        </div>
-                        <div class="row description-row">
-                            <div class="col-sm-6">Avg. Stolen per Day:</div>
-                            <div class='col-sm-4'><span style="color: red">{{ character.stolen.average_day|floatformat:0|intcomma }}</span> ISK</div>
-                        </div>
-                        {% if character.mining %}
-                        <hr>
-                        {% if character.mining.total_amount_day %}
-                        <div class="row description-row">
-                            <div class="col-sm-6">Current Day - Mining:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.mining.total_amount_day|floatformat:0|intcomma }}</span> ISK</div>
-                        </div>
+
+                        {% if character.stolen %}
+                            {% if character.stolen.average_day %}
+                                <div class="row description-row">
+                                    <div class="col-sm-6">Current Day - Stolen ESS:</div>
+                                    <div class='col-sm-4'><span style="color: red">{{ character.stolen.average_day|floatformat:0|intcomma }}</span> ISK</div>
+                                </div>
+                            {% endif %}
+                            <div class="row description-row">
+                                <div class="col-sm-6">Avg. Stolen per Day:</div>
+                                <div class='col-sm-4'><span style="color: red">{{ character.stolen.average_day|floatformat:0|intcomma }}</span> ISK</div>
+                            </div>
                         {% endif %}
-                        <div class="row description-row">
-                            <div class="col-sm-6">Avg. Mining per Day:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.mining.average_day|floatformat:0|intcomma }}</span> ISK</div>
-                        </div>
+
+                        {% if character.mining %}
+                            <hr>
+                            {% if character.mining.total_amount_day %}
+                                <div class="row description-row">
+                                    <div class="col-sm-6">Current Day - Mining:</div>
+                                    <div class='col-sm-4'><span style="color: green">{{ character.mining.total_amount_day|floatformat:0|intcomma }}</span> ISK</div>
+                                </div>
+                            {% endif %}
+                            <div class="row description-row">
+                                <div class="col-sm-6">Avg. Mining per Day:</div>
+                                <div class='col-sm-4'><span style="color: green">{{ character.mining.average_day|floatformat:0|intcomma }}</span> ISK</div>
+                            </div>
                         {% endif %}
 
                         {% if character.transaction %}
-                        <hr>
-                        {% if character.transaction.total_amount_day %}
-                        <div class="row description-row">
-                            <div class="col-sm-6">Current Day - Trading:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.transaction.total_amount_day|floatformat:0|intcomma }}</span> ISK</div>
-                        </div>
-                        <div class="row description-row">
-                            <div class="col-sm-6">Current Day - Trading Cost:</div>
-                            <div class='col-sm-4'><span style="color: red">{{ character.market_cost.total_amount_day|floatformat:0|intcomma }}</span> ISK</div>
-                        </div>
+                            <hr>
+                            {% if character.transaction.total_amount_day %}
+                                <div class="row description-row">
+                                    <div class="col-sm-6">Current Day - Trading:</div>
+                                    <div class='col-sm-4'><span style="color: green">{{ character.transaction.total_amount_day|floatformat:0|intcomma }}</span> ISK</div>
+                                </div>
+                            {% endif %}
+                            <div class="row description-row">
+                                <div class="col-sm-6">Avg. Trading per Day:</div>
+                                <div class='col-sm-4'><span style="color: green">{{ character.transaction.average_day|floatformat:0|intcomma }}</span> ISK</div>
+                            </div>
                         {% endif %}
-                        <div class="row description-row">
-                            <div class="col-sm-6">Avg. Trading per Day:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.transaction.average_day|floatformat:0|intcomma }}</span> ISK</div>
-                        </div>
-                        <div class="row description-row">
-                            <div class="col-sm-6">Avg. Trading Cost per Day:</div>
-                            <div class='col-sm-4'><span style="color: red">{{ character.market_cost.average_day|floatformat:0|intcomma }}</span> ISK</div>
-                        </div>
+
+                        {% if character.market_cost %}
+                            {% if character.market_cost.total_amount_day %}
+                                <div class="row description-row">
+                                    <div class="col-sm-6">Current Day - Trading Cost:</div>
+                                    <div class='col-sm-4'><span style="color: red">{{ character.market_cost.total_amount_day|floatformat:0|intcomma }}</span> ISK</div>
+                                </div>
+                            {% endif %}
+                            <div class="row description-row">
+                                <div class="col-sm-6">Avg. Trading Cost per Day:</div>
+                                <div class='col-sm-4'><span style="color: red">{{ character.market_cost.average_day|floatformat:0|intcomma }}</span> ISK</div>
+                            </div>
                         {% endif %}
 
                         {% if character.contract %}
-                        <hr>
-                        {% if character.contract.total_amount_day %}
-                        <div class="row description-row">
-                            <div class="col-sm-6">Current Day - Contracts:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.contract.total_amount_day|floatformat:0|intcomma }}</span> ISK</div>
-                        </div>
-                        {% endif %}
-                        <div class="row description-row">
-                            <div class="col-sm-6">Avg. Contracts per Day:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.contract.average_day|floatformat:0|intcomma }}</span> ISK</div>
-                        </div>
+                            <hr>
+                            {% if character.contract.total_amount_day %}
+                                <div class="row description-row">
+                                    <div class="col-sm-6">Current Day - Contracts:</div>
+                                    <div class='col-sm-4'><span style="color: green">{{ character.contract.total_amount_day|floatformat:0|intcomma }}</span> ISK</div>
+                                </div>
+                            {% endif %}
+                                <div class="row description-row">
+                                    <div class="col-sm-6">Avg. Contracts per Day:</div>
+                                    <div class='col-sm-4'><span style="color: green">{{ character.contract.average_day|floatformat:0|intcomma }}</span> ISK</div>
+                                </div>
                         {% endif %}
 
                         {% if character.donation %}
-                        <hr>
-                        {% if character.donation.total_amount_day %}
-                        <div class="row description-row">
-                            <div class="col-sm-6">Current Day - Donations:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.donation.total_amount_day|floatformat:0|intcomma }}</span> ISK</div>
-                        </div>
-                        {% endif %}
-                        <div class="row description-row">
-                            <div class="col-sm-6">Avg. Donations per Day:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.donation.average_day|floatformat:0|intcomma }}</span> ISK</div>
-                        </div>
+                            <hr>
+                            {% if character.donation.total_amount_day %}
+                                <div class="row description-row">
+                                    <div class="col-sm-6">Current Day - Donations:</div>
+                                    <div class='col-sm-4'><span style="color: green">{{ character.donation.total_amount_day|floatformat:0|intcomma }}</span> ISK</div>
+                                </div>
+                            {% endif %}
+                            <div class="row description-row">
+                                <div class="col-sm-6">Avg. Donations per Day:</div>
+                                <div class='col-sm-4'><span style="color: green">{{ character.donation.average_day|floatformat:0|intcomma }}</span> ISK</div>
+                            </div>
                         {% endif %}
 
                         {% if character.production_cost %}
                         <hr>
-                        {% if character.production_cost.total_amount_day %}
-                        <div class="row description-row">
-                            <div class="col-sm-6">Current Day - Production Cost:</div>
-                            <div class='col-sm-4'><span style="color: red">{{ character.production_cost.total_amount_day|floatformat:0|intcomma }}</span> ISK</div>
-                        </div>
-                        {% endif %}
-                        <div class="row description-row">
-                            <div class="col-sm-6">Avg. Production Cost per Day:</div>
-                            <div class='col-sm-4'><span style="color: red">{{ character.production_cost.average_day|floatformat:0|intcomma }}</span> ISK</div>
-                        </div>
+                            {% if character.production_cost.total_amount_day %}
+                                <div class="row description-row">
+                                    <div class="col-sm-6">Current Day - Production Cost:</div>
+                                    <div class='col-sm-4'><span style="color: red">{{ character.production_cost.total_amount_day|floatformat:0|intcomma }}</span> ISK</div>
+                                </div>
+                            {% endif %}
+                                <div class="row description-row">
+                                    <div class="col-sm-6">Avg. Production Cost per Day:</div>
+                                    <div class='col-sm-4'><span style="color: red">{{ character.production_cost.average_day|floatformat:0|intcomma }}</span> ISK</div>
+                                </div>
                         {% endif %}
+
                         {% if character.date %}
-                        <hr>
-                        <div class="row description-row">
-                            <div class="col-sm-6">Summary Day</div>
-                            <div class='col-sm-6'><span style="color: green">{{ character.summary.total_amount_day|floatformat:0|intcomma }}</span> ISK</div>
-                        </div>
+                            <hr>
+                            <div class="row description-row">
+                                <div class="col-sm-6">Summary Day</div>
+                                <div class='col-sm-6'><span style="color: green">{{ character.summary.total_amount_day|floatformat:0|intcomma }}</span> ISK</div>
+                            </div>
                         {% endif %}
                     </div>
                 </div>
                 <!--############################## HOURLY #######################-->
                 <div class="tab-pane panel panel-default" id="tab-hourly">
                     <div class="card-body modal-tab">
-                        <div class="row description-row">
-                            <div class="col-sm-6">Avg. Ratting per Hour:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.bounty.average_hour|floatformat:0|intcomma }}</span> ISK</div>
-                        </div>
-                        <hr>
-                        <div class="row description-row">
-                            <div class="col-sm-6">Avg. ESS per Hour:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.bounty.average_hour|floatformat:0|intcomma }}</span> ISK</div>
-                        </div>
-                        <div class="row description-row">
-                            <div class="col-sm-6">Avg. Stolen per Hour:</div>
-                            <div class='col-sm-4'><span style="color: red">{{ character.stolen.average_hour|floatformat:0|intcomma }}</span> ISK</div>
-                        </div>
+                        {% if character.bounty %}
+                            <div class="row description-row">
+                                <div class="col-sm-6">Avg. Ratting per Hour:</div>
+                                <div class='col-sm-4'><span style="color: green">{{ character.bounty.average_hour|floatformat:0|intcomma }}</span> ISK</div>
+                            </div>
+                        {% endif %}
+
+                        {% if character.ess %}
+                            <div class="row description-row">
+                                <div class="col-sm-6">Avg. ESS per Hour:</div>
+                                <div class='col-sm-4'><span style="color: green">{{ character.ess.average_hour|floatformat:0|intcomma }}</span> ISK</div>
+                            </div>
+                        {% endif %}
+
+                        {% if character.stolen %}
+                            <div class="row description-row">
+                                <div class="col-sm-6">Avg. Stolen per Hour:</div>
+                                <div class='col-sm-4'><span style="color: red">{{ character.stolen.average_hour|floatformat:0|intcomma }}</span> ISK</div>
+                            </div>
+                        {% endif %}
 
                         {% if character.mining %}
+                        <hr>
                         <div class="row description-row">
                             <div class="col-sm-6">Avg. Mining per Hour:</div>
                             <div class='col-sm-4'><span style="color: green">{{ character.mining.average_hour|floatformat:0|intcomma }}</span> ISK</div>
                         </div>
                         {% endif %}
 
                         {% if character.transaction %}
-                        <hr>
-                        <div class="row description-row">
-                            <div class="col-sm-6">Avg. Trading per Hour:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.transaction.average_hour|floatformat:0|intcomma }}</span> ISK</div>
-                        </div>
-                        <div class="row description-row">
-                            <div class="col-sm-6">Avg. Trading Cost per Hour:</div>
-                            <div class='col-sm-4'><span style="color: red">{{ character.market_cost.average_hour|floatformat:0|intcomma }}</span> ISK</div>
-                        </div>
+                            <hr>
+                            <div class="row description-row">
+                                <div class="col-sm-6">Avg. Trading per Hour:</div>
+                                <div class='col-sm-4'><span style="color: green">{{ character.transaction.average_hour|floatformat:0|intcomma }}</span> ISK</div>
+                            </div>
+                        {% endif %}
+
+                        {% if character.market_cost %}
+                            <div class="row description-row">
+                                <div class="col-sm-6">Avg. Trading Cost per Hour:</div>
+                                <div class='col-sm-4'><span style="color: red">{{ character.market_cost.average_hour|floatformat:0|intcomma }}</span> ISK</div>
+                            </div>
                         {% endif %}
 
                         {% if character.contract %}
-                        <hr>
-                        <div class="row description-row">
-                            <div class="col-sm-6">Avg. Contracts per Hour:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.contract.average_hour|floatformat:0|intcomma }}</span> ISK</div>
-                        </div>
+                            <hr>
+                            <div class="row description-row">
+                                <div class="col-sm-6">Avg. Contracts per Hour:</div>
+                                <div class='col-sm-4'><span style="color: green">{{ character.contract.average_hour|floatformat:0|intcomma }}</span> ISK</div>
+                            </div>
                         {% endif %}
 
                         {% if character.donation %}
-                        <hr>
-                        <div class="row description-row">
-                            <div class="col-sm-6">Avg. Donations per Hour:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.donation.average_hour|floatformat:0|intcomma }}</span> ISK</div>
-                        </div>
+                            <hr>
+                            <div class="row description-row">
+                                <div class="col-sm-6">Avg. Donations per Hour:</div>
+                                <div class='col-sm-4'><span style="color: green">{{ character.donation.average_hour|floatformat:0|intcomma }}</span> ISK</div>
+                            </div>
                         {% endif %}
 
                         {% if character.production_cost %}
-                        <hr>
-                        <div class="row description-row">
-                            <div class="col-sm-6">Avg. Production Cost per Hour:</div>
-                            <div class='col-sm-4'><span style="color: red">{{ character.production_cost.average_hour|floatformat:0|intcomma }}</span> ISK</div>
-                        </div>
+                            <hr>
+                            <div class="row description-row">
+                                <div class="col-sm-6">Avg. Production Cost per Hour:</div>
+                                <div class='col-sm-4'><span style="color: red">{{ character.production_cost.average_hour|floatformat:0|intcomma }}</span> ISK</div>
+                            </div>
                         {% endif %}
                         {% if character.date %}
-                        <hr>
-                        <div class="row description-row">
-                            <div class="col-sm-6">Summary Hour</div>
-                            <div class='col-sm-6'><span style="color: green">{{ character.summary.total_amount_hour|floatformat:0|intcomma }}</span> ISK</div>
-                        </div>
+                            <hr>
+                            <div class="row description-row">
+                                <div class="col-sm-6">Summary Hour</div>
+                                <div class='col-sm-6'><span style="color: green">{{ character.summary.total_amount_hour|floatformat:0|intcomma }}</span> ISK</div>
+                            </div>
                         {% endif %}
                     </div>
                 </div>
             </div>
         </div>
         {% else %}
         No ratting data found...
```

### Comparing `aa_ledger-0.4.0/ledger/view_helpers/core.py` & `aa_ledger-0.4.1/ledger/view_helpers/core.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/views/pve.py` & `aa_ledger-0.4.1/ledger/views/pve.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 """PvE Views"""
 
 # Django
-from django.conf import settings
 from django.contrib.auth.decorators import login_required, permission_required
 from django.shortcuts import render
 
 # Voices of War
+from ledger.app_settings import LEDGER_MEMBERAUDIT_USE
 from ledger.hooks import get_extension_logger
 
 logger = get_extension_logger(__name__)
 
 
 @login_required
 @permission_required("ledger.basic_access")
 def ledger_index(request):
     context = {
-        "memberaudit": settings.LEDGER_MEMBERAUDIT_USE,
+        "memberaudit": LEDGER_MEMBERAUDIT_USE,
     }
     return render(request, "ledger/index.html", context=context)
 
 
 @login_required
 @permission_required("ledger.basic_access")
 def ratting_index(request):
     context = {
-        "memberaudit": settings.LEDGER_MEMBERAUDIT_USE,
+        "memberaudit": LEDGER_MEMBERAUDIT_USE,
     }
     return render(request, "ledger/corpledger/corp_ledger.html", context=context)
 
 
 @login_required
 @permission_required("ledger.basic_access")
 def ratting_char_index(request):
     context = {
-        "memberaudit": settings.LEDGER_MEMBERAUDIT_USE,
+        "memberaudit": LEDGER_MEMBERAUDIT_USE,
     }
     return render(request, "ledger/charledger/char_ledger.html", context=context)
```

### Comparing `aa_ledger-0.4.0/ledger/views/character/char_audit.py` & `aa_ledger-0.4.1/ledger/views/character/char_audit.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/views/corporation/corp_audit.py` & `aa_ledger-0.4.1/ledger/views/corporation/corp_audit.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/views/corporation/corp_events.py` & `aa_ledger-0.4.1/ledger/views/corporation/corp_events.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/ledger/views/corporation/corp_tax.py` & `aa_ledger-0.4.1/ledger/views/corporation/corp_tax.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/LICENSE` & `aa_ledger-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/README.md` & `aa_ledger-0.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 - [AA Ledger](#aa-ledger)
   - [Features](#features)
   - [Upcoming](#upcoming)
   - [Installation](#features)
     - [Step 1 - Install the Package](#step1)
     - [Step 2 - Configure Alliance Auth](#step2)
-    - [Step 3 - Add the Scheduled Tasks](#step3)
+    - [Step 3 - Add the Scheduled Tasks and Settings](#step3)
     - [Step 4 - Migration to AA](#step4)
     - [Step 5 - Setting up Permissions](#step5)
     - [Step 6 - (Optional) Setting up Compatibilies](#step6)
   - [Highlights](#highlights)
 
 ## Features<a name="features"></a>
 
@@ -84,23 +84,23 @@
 | `char_audit_admin_access` | Can Manage Character Audit Module      | Can Manage Character Audit Module, Like Add Memeberaudit Chars, View Character Journals |
 | `corp_audit_admin_access` | Can Manage Corporation Audit Module    | Can Manage Corporation Audit Module, Like Add Corp, View Corporation Journals           |
 
 ### Step 6 - (Optional) Setting up Compatibilies<a name="step6"></a>
 
 The Following Settings can be setting up in the `local.py`
 
-- LEDGER_APP_NAME:          `"YOURNAME"`   - Set the name of the APP
+- LEDGER_APP_NAME:          `"YOURNAME"`     - Set the name of the APP
 
-- LEDGER_CORP_TAX:          `15`   - Set Tax Value for ESS Payout Calculation
+- LEDGER_CORP_TAX:          `15`             - Set Tax Value for ESS Payout Calculation
 
-- LEDGER_LOGGER_USE:        `True / False` - Set to use own Logger File
+- LEDGER_MEMBERAUDIT_USE:   `True / False`   - Set to use the Memberaudit Journal to Fetch Statistics
 
-- LEDGER_MEMBERAUDIT_USE:   `True / False` - Set to use the Memberaudit Journal to Fetch Statistics
+- LEDGER_LOGGER_USE:        `True / False`   - Set to use own Logger File
 
-- LEDGER_CORPSTATS_TWO:     `True / False` - Set to use Corp Stats Two APP to Fetch Members that are not registred
+- LEDGER_CORPSTATS_TWO:     `True / False`   - Set to use Corp Stats Two APP to Fetch Members that are not registred
 
 If you set up LEDGER_LOGGER_USE to `True` you need to add the following code below:
 
 ```python
 LOGGING_LEDGER = {
     "handlers": {
         "ledger_file": {
```

### Comparing `aa_ledger-0.4.0/pyproject.toml` & `aa_ledger-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.0/PKG-INFO` & `aa_ledger-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: aa-ledger
-Version: 0.4.0
+Version: 0.4.1
 Summary: Character/Corporation Ledger
 Project-URL: Changelog, https://github.com/Geuthur/aa-ledger/blob/master/CHANGELOG.md
 Project-URL: Homepage, https://github.com/Geuthur/aa-ledger
 Project-URL: Source, https://github.com/Geuthur/aa-ledger
 Project-URL: Tracker, https://github.com/Geuthur/aa-ledger/issues
 Author-email: Geuthur <devgeuthur@gmail.com>
 License: MIT License
@@ -63,15 +63,15 @@
 
 - [AA Ledger](#aa-ledger)
   - [Features](#features)
   - [Upcoming](#upcoming)
   - [Installation](#features)
     - [Step 1 - Install the Package](#step1)
     - [Step 2 - Configure Alliance Auth](#step2)
-    - [Step 3 - Add the Scheduled Tasks](#step3)
+    - [Step 3 - Add the Scheduled Tasks and Settings](#step3)
     - [Step 4 - Migration to AA](#step4)
     - [Step 5 - Setting up Permissions](#step5)
     - [Step 6 - (Optional) Setting up Compatibilies](#step6)
   - [Highlights](#highlights)
 
 ## Features<a name="features"></a>
 
@@ -141,23 +141,23 @@
 | `char_audit_admin_access` | Can Manage Character Audit Module      | Can Manage Character Audit Module, Like Add Memeberaudit Chars, View Character Journals |
 | `corp_audit_admin_access` | Can Manage Corporation Audit Module    | Can Manage Corporation Audit Module, Like Add Corp, View Corporation Journals           |
 
 ### Step 6 - (Optional) Setting up Compatibilies<a name="step6"></a>
 
 The Following Settings can be setting up in the `local.py`
 
-- LEDGER_APP_NAME:          `"YOURNAME"`   - Set the name of the APP
+- LEDGER_APP_NAME:          `"YOURNAME"`     - Set the name of the APP
 
-- LEDGER_CORP_TAX:          `15`   - Set Tax Value for ESS Payout Calculation
+- LEDGER_CORP_TAX:          `15`             - Set Tax Value for ESS Payout Calculation
 
-- LEDGER_LOGGER_USE:        `True / False` - Set to use own Logger File
+- LEDGER_MEMBERAUDIT_USE:   `True / False`   - Set to use the Memberaudit Journal to Fetch Statistics
 
-- LEDGER_MEMBERAUDIT_USE:   `True / False` - Set to use the Memberaudit Journal to Fetch Statistics
+- LEDGER_LOGGER_USE:        `True / False`   - Set to use own Logger File
 
-- LEDGER_CORPSTATS_TWO:     `True / False` - Set to use Corp Stats Two APP to Fetch Members that are not registred
+- LEDGER_CORPSTATS_TWO:     `True / False`   - Set to use Corp Stats Two APP to Fetch Members that are not registred
 
 If you set up LEDGER_LOGGER_USE to `True` you need to add the following code below:
 
 ```python
 LOGGING_LEDGER = {
     "handlers": {
         "ledger_file": {
```

