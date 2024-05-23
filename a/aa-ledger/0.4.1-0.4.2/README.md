# Comparing `tmp/aa_ledger-0.4.1.tar.gz` & `tmp/aa_ledger-0.4.2.tar.gz`

## Comparing `aa_ledger-0.4.1.tar` & `aa_ledger-0.4.2.tar`

### file list

```diff
@@ -1,80 +1,80 @@
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/__init__.py
--rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/admin.py
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/app_settings.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/apps.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/auth_hooks.py
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/decorators.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/errors.py
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/hooks.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/providers.py
--rw-r--r--   0        0        0     4956 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/tasks.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/urls.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/api/__init__.py
--rw-r--r--   0        0        0     7394 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/api/helpers.py
--rw-r--r--   0        0        0    23759 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/api/ledgermanager.py
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/api/schema.py
--rw-r--r--   0        0        0    16151 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/api/templatemanager.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/api/character/__init__.py
--rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/api/character/ledger.py
--rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/api/character/template.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/api/corporation/__init__.py
--rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/api/corporation/ledger.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/api/corporation/template.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/locate/__init__.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/locate/de.po
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/managers/charaudit_manager.py
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/managers/corpaudit_manager.py
--rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/managers/general_manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/migrations/__init__.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/models/__init__.py
--rw-r--r--   0        0        0     5771 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/models/characteraudit.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/models/corporationaudit.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/models/events.py
--rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/models/general.py
--rw-r--r--   0        0        0     5416 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/static/ledger/css/billboards_dark.css
--rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/static/ledger/css/cards.css
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/static/ledger/css/custom.css
--rw-r--r--   0        0        0   236145 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/static/ledger/guides/ledger-1.png
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/static/ledger/guides/ledger-2.png
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/static/ledger/guides/ledger-3.png
--rw-r--r--   0        0        0    43262 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/static/ledger/images/Spinner-1s-64px-dark.gif
--rw-r--r--   0        0        0    43381 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/static/ledger/images/Spinner-1s-64px-light.gif
--rw-r--r--   0        0        0    22096 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/static/ledger/js/charledger.js
--rw-r--r--   0        0        0    18853 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/static/ledger/js/corpledger.js
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/static/ledger/js/img.js
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/task_helpers/__init__.py
--rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/task_helpers/char_helpers.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/task_helpers/core_helpers.py
--rw-r--r--   0        0        0     8398 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/task_helpers/corp_helpers.py
--rw-r--r--   0        0        0     8434 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/task_helpers/etag_helpers.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/templates/ledger/base.html
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/templates/ledger/error.html
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/templates/ledger/index.html
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/templates/ledger/menu.html
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/templates/ledger/bundles/ledger-css.html
--rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/templates/ledger/charledger/char_ledger.html
--rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/templates/ledger/charledger/month.html
--rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/templates/ledger/charledger/year.html
--rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/templates/ledger/corpledger/corp_ledger.html
--rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/templates/ledger/corpledger/month.html
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/templates/ledger/corpledger/year.html
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/templates/ledger/modals/modal-full.html
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/templates/ledger/modals/modal-xl.html
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/templates/ledger/modals/modal.html
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/templates/ledger/modals/modal_dialog.html
--rw-r--r--   0        0        0    20050 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/templates/ledger/modals/pve/view_character_content.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/templatetags/__init__.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/templatetags/ledger.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/view_helpers/__init__.py
--rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/view_helpers/core.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/views/__init__.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/views/pve.py
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/views/character/char_audit.py
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/views/corporation/corp_audit.py
--rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/views/corporation/corp_events.py
--rw-r--r--   0        0        0     8919 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/ledger/views/corporation/corp_tax.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/LICENSE
--rw-r--r--   0        0        0     5633 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/README.md
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     8412 2020-02-02 00:00:00.000000 aa_ledger-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/__init__.py
+-rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/admin.py
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/app_settings.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/apps.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/auth_hooks.py
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/decorators.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/errors.py
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/hooks.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/providers.py
+-rw-r--r--   0        0        0     4956 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/tasks.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/urls.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/api/__init__.py
+-rw-r--r--   0        0        0     7394 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/api/helpers.py
+-rw-r--r--   0        0        0    23577 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/api/ledgermanager.py
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/api/schema.py
+-rw-r--r--   0        0        0    16118 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/api/templatemanager.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/api/character/__init__.py
+-rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/api/character/ledger.py
+-rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/api/character/template.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/api/corporation/__init__.py
+-rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/api/corporation/ledger.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/api/corporation/template.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/locate/__init__.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/locate/de.po
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/managers/charaudit_manager.py
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/managers/corpaudit_manager.py
+-rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/managers/general_manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/migrations/__init__.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/models/__init__.py
+-rw-r--r--   0        0        0     5771 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/models/characteraudit.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/models/corporationaudit.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/models/events.py
+-rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/models/general.py
+-rw-r--r--   0        0        0     5416 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/static/ledger/css/billboards_dark.css
+-rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/static/ledger/css/cards.css
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/static/ledger/css/custom.css
+-rw-r--r--   0        0        0   236145 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/static/ledger/guides/ledger-1.png
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/static/ledger/guides/ledger-2.png
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/static/ledger/guides/ledger-3.png
+-rw-r--r--   0        0        0    43262 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/static/ledger/images/Spinner-1s-64px-dark.gif
+-rw-r--r--   0        0        0    43381 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/static/ledger/images/Spinner-1s-64px-light.gif
+-rw-r--r--   0        0        0    22096 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/static/ledger/js/charledger.js
+-rw-r--r--   0        0        0    18853 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/static/ledger/js/corpledger.js
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/static/ledger/js/img.js
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/task_helpers/__init__.py
+-rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/task_helpers/char_helpers.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/task_helpers/core_helpers.py
+-rw-r--r--   0        0        0     8398 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/task_helpers/corp_helpers.py
+-rw-r--r--   0        0        0     8434 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/task_helpers/etag_helpers.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/templates/ledger/base.html
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/templates/ledger/error.html
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/templates/ledger/index.html
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/templates/ledger/menu.html
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/templates/ledger/bundles/ledger-css.html
+-rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/templates/ledger/charledger/char_ledger.html
+-rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/templates/ledger/charledger/month.html
+-rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/templates/ledger/charledger/year.html
+-rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/templates/ledger/corpledger/corp_ledger.html
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/templates/ledger/corpledger/month.html
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/templates/ledger/corpledger/year.html
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/templates/ledger/modals/modal-full.html
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/templates/ledger/modals/modal-xl.html
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/templates/ledger/modals/modal.html
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/templates/ledger/modals/modal_dialog.html
+-rw-r--r--   0        0        0    20050 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/templates/ledger/modals/pve/view_character_content.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/templatetags/__init__.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/templatetags/ledger.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/view_helpers/__init__.py
+-rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/view_helpers/core.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/views/__init__.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/views/pve.py
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/views/character/char_audit.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/views/corporation/corp_audit.py
+-rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/views/corporation/corp_events.py
+-rw-r--r--   0        0        0     8919 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/ledger/views/corporation/corp_tax.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/LICENSE
+-rw-r--r--   0        0        0     5633 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/README.md
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     8412 2020-02-02 00:00:00.000000 aa_ledger-0.4.2/PKG-INFO
```

### Comparing `aa_ledger-0.4.1/ledger/admin.py` & `aa_ledger-0.4.2/ledger/admin.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/app_settings.py` & `aa_ledger-0.4.2/ledger/app_settings.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/auth_hooks.py` & `aa_ledger-0.4.2/ledger/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/decorators.py` & `aa_ledger-0.4.2/ledger/decorators.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/hooks.py` & `aa_ledger-0.4.2/ledger/hooks.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/tasks.py` & `aa_ledger-0.4.2/ledger/tasks.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/urls.py` & `aa_ledger-0.4.2/ledger/urls.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/api/__init__.py` & `aa_ledger-0.4.2/ledger/api/__init__.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/api/helpers.py` & `aa_ledger-0.4.2/ledger/api/helpers.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/api/ledgermanager.py` & `aa_ledger-0.4.2/ledger/api/ledgermanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -583,18 +583,14 @@
             ["Income", int(self.data.total_isk)],
             # ["Ratting", int(total_sum_ratting)],  ["Mining", int(total_sum_mining)], ["Misc.", int(total_sum_misc)],
             # Costs
             ["Market Cost", int(abs(self.data.total_market))],
             ["Production Cost", int(abs(self.data.total_production_cost))],
             ["Misc. Cost", int(misc_cost)],
         ]
-        logger.error(self.data.total_cost)
-        logger.error(self.data.total_production_cost)
-        logger.error(self.data.total_market)
-        logger.error(wallet_chart_data)
 
         self.billboard_dict["walletcharts"] = (
             wallet_chart_data
             if any(item[1] != 0 for item in wallet_chart_data)
             else None
         )
```

### Comparing `aa_ledger-0.4.1/ledger/api/schema.py` & `aa_ledger-0.4.2/ledger/api/schema.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/api/templatemanager.py` & `aa_ledger-0.4.2/ledger/api/templatemanager.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         self.char_id = char_id
         self.filter = Q(second_party_id__in=self.char_id) | Q(
             first_party_id__in=self.char_id
         )
         self.filter_bounty = self.filter & Q(ref_type="bounty_prizes")
         self.filter_ess = self.filter & Q(ref_type="ess_escrow_transfer")
         self.filter_mining = (
-            Q(character__character_id=char_id)
+            Q(character__eve_character_id__in=char_id)
             if app_settings.LEDGER_MEMBERAUDIT_USE
             else Q(character__character__character_id__in=char_id)
         )
 
 
 class TemplateFilterCost(TemplateFilterCore):
     """TemplateFilter class to store the filter data."""
@@ -221,15 +221,14 @@
         # Exclude Events to avoid wrong stats
         corporation_journal = events_filter(corporation_journal)
         mining_journal = (
             CharacterMiningLedger.objects.filter(filters, filter_date)
         ).annotate_pricing()
 
         self._process_characters(character_journal, corporation_journal, mining_journal)
-        logger.debug(self.template_dict)
         return self.template_dict
 
     def corporation_template(self):
         """
         Create the corporation template.
         return: dict
         """
```

### Comparing `aa_ledger-0.4.1/ledger/api/character/ledger.py` & `aa_ledger-0.4.2/ledger/api/character/ledger.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/api/character/template.py` & `aa_ledger-0.4.2/ledger/api/character/template.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/api/corporation/ledger.py` & `aa_ledger-0.4.2/ledger/api/corporation/ledger.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/api/corporation/template.py` & `aa_ledger-0.4.2/ledger/api/corporation/template.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/locate/de.po` & `aa_ledger-0.4.2/ledger/locate/de.po`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/managers/charaudit_manager.py` & `aa_ledger-0.4.2/ledger/managers/charaudit_manager.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/managers/corpaudit_manager.py` & `aa_ledger-0.4.2/ledger/managers/corpaudit_manager.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/managers/general_manager.py` & `aa_ledger-0.4.2/ledger/managers/general_manager.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/models/characteraudit.py` & `aa_ledger-0.4.2/ledger/models/characteraudit.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/models/corporationaudit.py` & `aa_ledger-0.4.2/ledger/models/corporationaudit.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/models/events.py` & `aa_ledger-0.4.2/ledger/models/events.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/models/general.py` & `aa_ledger-0.4.2/ledger/models/general.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/static/ledger/css/billboards_dark.css` & `aa_ledger-0.4.2/ledger/static/ledger/css/billboards_dark.css`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/static/ledger/css/cards.css` & `aa_ledger-0.4.2/ledger/static/ledger/css/cards.css`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/static/ledger/css/custom.css` & `aa_ledger-0.4.2/ledger/static/ledger/css/custom.css`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/static/ledger/guides/ledger-1.png` & `aa_ledger-0.4.2/ledger/static/ledger/guides/ledger-1.png`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/static/ledger/guides/ledger-2.png` & `aa_ledger-0.4.2/ledger/static/ledger/guides/ledger-2.png`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/static/ledger/guides/ledger-3.png` & `aa_ledger-0.4.2/ledger/static/ledger/guides/ledger-3.png`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/static/ledger/images/Spinner-1s-64px-dark.gif` & `aa_ledger-0.4.2/ledger/static/ledger/images/Spinner-1s-64px-dark.gif`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/static/ledger/images/Spinner-1s-64px-light.gif` & `aa_ledger-0.4.2/ledger/static/ledger/images/Spinner-1s-64px-light.gif`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/static/ledger/js/charledger.js` & `aa_ledger-0.4.2/ledger/static/ledger/js/charledger.js`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/static/ledger/js/corpledger.js` & `aa_ledger-0.4.2/ledger/static/ledger/js/corpledger.js`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/static/ledger/js/img.js` & `aa_ledger-0.4.2/ledger/static/ledger/js/img.js`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/task_helpers/char_helpers.py` & `aa_ledger-0.4.2/ledger/task_helpers/char_helpers.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/task_helpers/core_helpers.py` & `aa_ledger-0.4.2/ledger/task_helpers/core_helpers.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/task_helpers/corp_helpers.py` & `aa_ledger-0.4.2/ledger/task_helpers/corp_helpers.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/task_helpers/etag_helpers.py` & `aa_ledger-0.4.2/ledger/task_helpers/etag_helpers.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/templates/ledger/base.html` & `aa_ledger-0.4.2/ledger/templates/ledger/base.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/templates/ledger/error.html` & `aa_ledger-0.4.2/ledger/templates/ledger/error.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/templates/ledger/index.html` & `aa_ledger-0.4.2/ledger/templates/ledger/index.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/templates/ledger/menu.html` & `aa_ledger-0.4.2/ledger/templates/ledger/menu.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/templates/ledger/charledger/char_ledger.html` & `aa_ledger-0.4.2/ledger/templates/ledger/charledger/char_ledger.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/templates/ledger/charledger/month.html` & `aa_ledger-0.4.2/ledger/templates/ledger/charledger/month.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/templates/ledger/charledger/year.html` & `aa_ledger-0.4.2/ledger/templates/ledger/charledger/year.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/templates/ledger/corpledger/corp_ledger.html` & `aa_ledger-0.4.2/ledger/templates/ledger/corpledger/corp_ledger.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/templates/ledger/corpledger/month.html` & `aa_ledger-0.4.2/ledger/templates/ledger/corpledger/month.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/templates/ledger/corpledger/year.html` & `aa_ledger-0.4.2/ledger/templates/ledger/corpledger/year.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/templates/ledger/modals/modal-full.html` & `aa_ledger-0.4.2/ledger/templates/ledger/modals/modal-full.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/templates/ledger/modals/modal-xl.html` & `aa_ledger-0.4.2/ledger/templates/ledger/modals/modal-xl.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/templates/ledger/modals/modal.html` & `aa_ledger-0.4.2/ledger/templates/ledger/modals/modal.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/templates/ledger/modals/modal_dialog.html` & `aa_ledger-0.4.2/ledger/templates/ledger/modals/modal_dialog.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/templates/ledger/modals/pve/view_character_content.html` & `aa_ledger-0.4.2/ledger/templates/ledger/modals/pve/view_character_content.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/view_helpers/core.py` & `aa_ledger-0.4.2/ledger/view_helpers/core.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/views/pve.py` & `aa_ledger-0.4.2/ledger/views/pve.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/views/character/char_audit.py` & `aa_ledger-0.4.2/ledger/views/character/char_audit.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/views/corporation/corp_audit.py` & `aa_ledger-0.4.2/ledger/views/corporation/corp_audit.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/views/corporation/corp_events.py` & `aa_ledger-0.4.2/ledger/views/corporation/corp_events.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/ledger/views/corporation/corp_tax.py` & `aa_ledger-0.4.2/ledger/views/corporation/corp_tax.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/LICENSE` & `aa_ledger-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/README.md` & `aa_ledger-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/pyproject.toml` & `aa_ledger-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.4.1/PKG-INFO` & `aa_ledger-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: aa-ledger
-Version: 0.4.1
+Version: 0.4.2
 Summary: Character/Corporation Ledger
 Project-URL: Changelog, https://github.com/Geuthur/aa-ledger/blob/master/CHANGELOG.md
 Project-URL: Homepage, https://github.com/Geuthur/aa-ledger
 Project-URL: Source, https://github.com/Geuthur/aa-ledger
 Project-URL: Tracker, https://github.com/Geuthur/aa-ledger/issues
 Author-email: Geuthur <devgeuthur@gmail.com>
 License: MIT License
```

