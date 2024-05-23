# Comparing `tmp/wagtail_fedit-1.5.9rc3.tar.gz` & `tmp/wagtail_fedit-1.5.9rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.5.9rc3.tar", last modified: Thu May 23 08:27:01 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.5.9rc4.tar", last modified: Thu May 23 09:08:04 2024, max compression
```

## Comparing `wagtail_fedit-1.5.9rc3.tar` & `wagtail_fedit-1.5.9rc4.tar`

### file list

```diff
@@ -1,145 +1,145 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 08:27:01.986267 wagtail_fedit-1.5.9rc3/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.9rc3/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.9rc3/MANIFEST.in
--rw-rw-rw-   0        0        0     3126 2024-05-23 08:27:01.986874 wagtail_fedit-1.5.9rc3/PKG-INFO
--rw-rw-rw-   0        0        0     1925 2024-05-23 07:48:54.000000 wagtail_fedit-1.5.9rc3/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.9rc3/pyproject.toml
--rw-rw-rw-   0        0        0     1189 2024-05-23 08:27:01.989889 wagtail_fedit-1.5.9rc3/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.9rc3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-23 08:27:01.791650 wagtail_fedit-1.5.9rc3/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 08:27:01.812751 wagtail_fedit-1.5.9rc3/wagtail_fedit/adapters/
--rw-rw-rw-   0        0        0      455 2024-05-21 19:49:09.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/adapters/__init__.py
--rw-rw-rw-   0        0        0    15762 2024-05-21 19:41:15.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/adapters/base.py
-drwxrwxrwx   0        0        0        0 2024-05-23 08:27:01.820109 wagtail_fedit-1.5.9rc3/wagtail_fedit/adapters/block/
--rw-rw-rw-   0        0        0       76 2024-05-21 19:49:08.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/adapters/block/__init__.py
--rw-rw-rw-   0        0        0     8345 2024-05-22 10:03:59.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/adapters/block/adapter.py
--rw-rw-rw-   0        0        0     1800 2024-05-21 19:53:21.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/adapters/block/buttons.py
--rw-rw-rw-   0        0        0     5509 2024-05-22 10:06:29.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/adapters/block/views.py
--rw-rw-rw-   0        0        0     8946 2024-05-19 22:04:41.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/adapters/field.py
--rw-rw-rw-   0        0        0     2305 2024-04-25 18:28:58.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/adapters/funcs.py
--rw-rw-rw-   0        0        0     2755 2024-04-25 18:28:49.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/adapters/misc.py
--rw-rw-rw-   0        0        0     5665 2024-05-19 22:05:27.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/adapters/models.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/apps.py
--rw-rw-rw-   0        0        0     1354 2024-04-25 09:55:56.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/errors.py
-drwxrwxrwx   0        0        0        0 2024-05-23 08:27:01.826616 wagtail_fedit-1.5.9rc3/wagtail_fedit/forms/
--rw-rw-rw-   0        0        0      215 2024-04-23 13:02:23.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/forms/__init__.py
--rw-rw-rw-   0        0        0     2881 2024-04-18 20:27:35.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/forms/blocks.py
--rw-rw-rw-   0        0        0     3269 2024-04-23 13:28:56.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/forms/fields.py
--rw-rw-rw-   0        0        0     5612 2024-05-18 18:03:06.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-05-23 08:27:01.747312 wagtail_fedit-1.5.9rc3/wagtail_fedit/locale/
-drwxrwxrwx   0        0        0        0 2024-05-23 08:27:01.747312 wagtail_fedit-1.5.9rc3/wagtail_fedit/locale/nl/
-drwxrwxrwx   0        0        0        0 2024-05-23 08:27:01.829616 wagtail_fedit-1.5.9rc3/wagtail_fedit/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0        0        0     9614 2024-05-19 22:55:13.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    16810 2024-05-19 22:55:04.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2024-05-23 08:27:01.832142 wagtail_fedit-1.5.9rc3/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 08:27:01.833614 wagtail_fedit-1.5.9rc3/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/models.py
--rw-rw-rw-   0        0        0     1451 2024-05-18 21:38:18.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/registry.py
--rw-rw-rw-   0        0        0     1626 2024-04-25 13:40:59.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/settings.py
-drwxrwxrwx   0        0        0        0 2024-05-23 08:27:01.750769 wagtail_fedit-1.5.9rc3/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-05-23 08:27:01.752418 wagtail_fedit-1.5.9rc3/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-05-23 08:27:01.839599 wagtail_fedit-1.5.9rc3/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0     5957 2024-05-22 09:18:05.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     5091 2024-05-22 09:07:12.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/static/wagtail_fedit/css/furniture.css
--rw-rw-rw-   0        0        0     1249 2024-05-18 12:55:22.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
-drwxrwxrwx   0        0        0        0 2024-05-23 08:27:01.840803 wagtail_fedit-1.5.9rc3/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    58202 2024-05-23 07:47:43.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/static/wagtail_fedit/js/edit.js
-drwxrwxrwx   0        0        0        0 2024-05-23 08:27:01.843280 wagtail_fedit-1.5.9rc3/wagtail_fedit/static/wagtail_fedit/js/licenses/
--rw-rw-rw-   0        0        0     1091 2024-04-23 15:39:19.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/static/wagtail_fedit/js/licenses/TIPPY.LICENSE
-drwxrwxrwx   0        0        0        0 2024-05-23 08:27:01.754335 wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-05-23 08:27:01.845517 wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/
--rw-rw-rw-   0        0        0       56 2024-04-16 18:37:39.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/_hook_output.html
-drwxrwxrwx   0        0        0        0 2024-05-23 08:27:01.848942 wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-05-23 08:27:01.857772 wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      708 2024-05-21 20:01:50.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/content/buttons/add_block.html
--rw-rw-rw-   0        0        0      929 2024-04-23 15:23:24.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html
--rw-rw-rw-   0        0        0      991 2024-04-23 15:27:54.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
--rw-rw-rw-   0        0        0      742 2024-05-19 21:41:44.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/content/buttons/move_down.html
--rw-rw-rw-   0        0        0      738 2024-05-19 21:41:46.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/content/buttons/move_up.html
--rw-rw-rw-   0        0        0      601 2024-05-17 08:51:23.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
--rw-rw-rw-   0        0        0      378 2024-05-18 11:23:40.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/content/editable_dom_positioned_adapter.html
-drwxrwxrwx   0        0        0        0 2024-05-23 08:27:01.881086 wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
--rw-rw-rw-   0        0        0     3699 2024-04-20 21:55:10.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
--rw-rw-rw-   0        0        0      266 2024-04-21 21:15:09.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler.html
--rw-rw-rw-   0        0        0      265 2024-04-21 21:23:24.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler_form.html
--rw-rw-rw-   0        0        0      786 2024-05-18 21:59:44.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html
--rw-rw-rw-   0        0        0      455 2024-04-21 00:11:35.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form_errors.html
--rw-rw-rw-   0        0        0      345 2024-05-18 12:28:53.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
--rw-rw-rw-   0        0        0      397 2024-05-18 21:49:55.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe_dom_positioned.html
--rw-rw-rw-   0        0        0     5537 2024-05-18 12:20:21.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
--rw-rw-rw-   0        0        0       99 2024-05-21 20:50:08.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/editor/block_adapter_add_form.html
--rw-rw-rw-   0        0        0      544 2024-05-22 09:02:31.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/editor/block_adapter_iframe.html
--rw-rw-rw-   0        0        0      549 2024-05-18 15:36:09.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/editor/field.html
-drwxrwxrwx   0        0        0        0 2024-05-23 08:27:01.891250 wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/icons/
--rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
--rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
--rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
--rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
--rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
-drwxrwxrwx   0        0        0        0 2024-05-23 08:27:01.894819 wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
-drwxrwxrwx   0        0        0        0 2024-05-23 08:27:01.898818 wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
--rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
--rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
-drwxrwxrwx   0        0        0        0 2024-05-23 08:27:01.901145 wagtail_fedit-1.5.9rc3/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 08:27:01.903347 wagtail_fedit-1.5.9rc3/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    13210 2024-05-18 21:38:53.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0    10414 2024-05-18 21:38:48.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-05-23 08:27:01.903347 wagtail_fedit-1.5.9rc3/wagtail_fedit/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 08:27:01.919592 wagtail_fedit-1.5.9rc3/wagtail_fedit/test/core/
--rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/test/core/__init__.py
--rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/test/core/apps.py
--rw-rw-rw-   0        0        0      130 2024-04-15 20:12:38.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/test/core/context_processors.py
-drwxrwxrwx   0        0        0        0 2024-05-23 08:27:01.919852 wagtail_fedit-1.5.9rc3/wagtail_fedit/test/core/migrations/
--rw-rw-rw-   0        0        0    12115 2024-04-20 22:33:35.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/test/core/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      509 2024-04-21 18:41:55.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/test/core/migrations/0002_basicmodel_related_field.py
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/test/core/migrations/__init__.py
--rw-rw-rw-   0        0        0     6047 2024-04-23 13:09:46.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/test/core/models.py
-drwxrwxrwx   0        0        0        0 2024-05-23 08:27:01.948076 wagtail_fedit-1.5.9rc3/wagtail_fedit/test/core/tests/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/test/core/tests/__init__.py
--rw-rw-rw-   0        0        0     8962 2024-04-25 13:24:28.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/test/core/tests/base.py
--rw-rw-rw-   0        0        0    32620 2024-05-23 08:19:46.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/test/core/tests/test_adapters.py
--rw-rw-rw-   0        0        0     4352 2024-05-19 20:28:32.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/test/core/tests/test_block_edit.py
--rw-rw-rw-   0        0        0     7376 2024-05-23 08:22:32.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/test/core/tests/test_blocks.py
--rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/test/core/tests/test_field_edit.py
--rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/test/core/tests/test_generic.py
--rw-rw-rw-   0        0        0     4865 2024-04-23 14:23:09.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/test/core/tests/test_model_edit.py
--rw-rw-rw-   0        0        0     1574 2024-04-20 20:49:12.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/test/core/tests/test_revision.py
--rw-rw-rw-   0        0        0     9545 2024-04-20 21:54:40.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/test/core/tests/test_submit.py
--rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/test/manage.py
-drwxrwxrwx   0        0        0        0 2024-05-23 08:27:01.960077 wagtail_fedit-1.5.9rc3/wagtail_fedit/test/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/test/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/test/testapp/asgi.py
--rw-rw-rw-   0        0        0     3660 2024-05-18 16:08:35.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/test/testapp/settings.py
--rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/test/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/test/testapp/wsgi.py
--rw-rw-rw-   0        0        0     2220 2024-04-23 14:21:34.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0     1131 2024-05-18 22:43:51.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0    20178 2024-05-23 08:20:53.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-23 08:27:01.962210 wagtail_fedit-1.5.9rc3/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      215 2024-04-23 17:24:50.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     9286 2024-05-21 20:14:34.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/views/adapters.py
--rw-rw-rw-   0        0        0    17734 2024-05-20 09:37:43.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0     2239 2024-04-25 09:52:47.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/views/mixins.py
-drwxrwxrwx   0        0        0        0 2024-05-23 08:27:01.983561 wagtail_fedit-1.5.9rc3/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      155 2024-05-18 18:02:59.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0     1907 2024-05-13 18:26:02.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/wagtail_hooks/action_menu.py
--rw-rw-rw-   0        0        0     2446 2024-05-07 21:59:49.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/wagtail_hooks/adapter_hooks.py
--rw-rw-rw-   0        0        0     1173 2024-05-18 21:36:35.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/wagtail_hooks/adapters.py
--rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/wagtail_hooks/icons.py
--rw-rw-rw-   0        0        0     4017 2024-05-19 22:47:30.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0     7637 2024-04-23 20:17:24.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-05-23 08:27:01.802990 wagtail_fedit-1.5.9rc3/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0     3126 2024-05-23 08:27:01.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5002 2024-05-23 08:27:01.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 08:27:01.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-05-23 08:27:01.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-23 08:27:01.000000 wagtail_fedit-1.5.9rc3/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 09:08:04.936195 wagtail_fedit-1.5.9rc4/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.9rc4/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.9rc4/MANIFEST.in
+-rw-rw-rw-   0        0        0     3126 2024-05-23 09:08:04.936195 wagtail_fedit-1.5.9rc4/PKG-INFO
+-rw-rw-rw-   0        0        0     1925 2024-05-23 07:48:54.000000 wagtail_fedit-1.5.9rc4/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.9rc4/pyproject.toml
+-rw-rw-rw-   0        0        0     1189 2024-05-23 09:08:04.942202 wagtail_fedit-1.5.9rc4/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.9rc4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 09:08:04.466476 wagtail_fedit-1.5.9rc4/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 09:08:04.518825 wagtail_fedit-1.5.9rc4/wagtail_fedit/adapters/
+-rw-rw-rw-   0        0        0      455 2024-05-21 19:49:09.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/adapters/__init__.py
+-rw-rw-rw-   0        0        0    15762 2024-05-21 19:41:15.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/adapters/base.py
+drwxrwxrwx   0        0        0        0 2024-05-23 09:08:04.534258 wagtail_fedit-1.5.9rc4/wagtail_fedit/adapters/block/
+-rw-rw-rw-   0        0        0       76 2024-05-21 19:49:08.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/adapters/block/__init__.py
+-rw-rw-rw-   0        0        0     8345 2024-05-22 10:03:59.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/adapters/block/adapter.py
+-rw-rw-rw-   0        0        0     1800 2024-05-21 19:53:21.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/adapters/block/buttons.py
+-rw-rw-rw-   0        0        0     6235 2024-05-23 09:05:04.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/adapters/block/views.py
+-rw-rw-rw-   0        0        0     8946 2024-05-19 22:04:41.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/adapters/field.py
+-rw-rw-rw-   0        0        0     2305 2024-04-25 18:28:58.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/adapters/funcs.py
+-rw-rw-rw-   0        0        0     2755 2024-04-25 18:28:49.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/adapters/misc.py
+-rw-rw-rw-   0        0        0     5665 2024-05-19 22:05:27.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/adapters/models.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/apps.py
+-rw-rw-rw-   0        0        0     1354 2024-04-25 09:55:56.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/errors.py
+drwxrwxrwx   0        0        0        0 2024-05-23 09:08:04.546017 wagtail_fedit-1.5.9rc4/wagtail_fedit/forms/
+-rw-rw-rw-   0        0        0      215 2024-04-23 13:02:23.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/forms/__init__.py
+-rw-rw-rw-   0        0        0     2881 2024-04-18 20:27:35.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/forms/blocks.py
+-rw-rw-rw-   0        0        0     3269 2024-04-23 13:28:56.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/forms/fields.py
+-rw-rw-rw-   0        0        0     5612 2024-05-18 18:03:06.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-05-23 09:08:04.366791 wagtail_fedit-1.5.9rc4/wagtail_fedit/locale/
+drwxrwxrwx   0        0        0        0 2024-05-23 09:08:04.367787 wagtail_fedit-1.5.9rc4/wagtail_fedit/locale/nl/
+drwxrwxrwx   0        0        0        0 2024-05-23 09:08:04.551814 wagtail_fedit-1.5.9rc4/wagtail_fedit/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     9614 2024-05-19 22:55:13.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    16810 2024-05-19 22:55:04.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-05-23 09:08:04.559584 wagtail_fedit-1.5.9rc4/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 09:08:04.562582 wagtail_fedit-1.5.9rc4/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/models.py
+-rw-rw-rw-   0        0        0     1451 2024-05-18 21:38:18.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/registry.py
+-rw-rw-rw-   0        0        0     1626 2024-04-25 13:40:59.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/settings.py
+drwxrwxrwx   0        0        0        0 2024-05-23 09:08:04.372784 wagtail_fedit-1.5.9rc4/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-05-23 09:08:04.374328 wagtail_fedit-1.5.9rc4/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-05-23 09:08:04.582621 wagtail_fedit-1.5.9rc4/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0     5957 2024-05-22 09:18:05.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     5091 2024-05-22 09:07:12.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+-rw-rw-rw-   0        0        0     1249 2024-05-18 12:55:22.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
+drwxrwxrwx   0        0        0        0 2024-05-23 09:08:04.592969 wagtail_fedit-1.5.9rc4/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    58202 2024-05-23 07:47:43.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/static/wagtail_fedit/js/edit.js
+drwxrwxrwx   0        0        0        0 2024-05-23 09:08:04.597389 wagtail_fedit-1.5.9rc4/wagtail_fedit/static/wagtail_fedit/js/licenses/
+-rw-rw-rw-   0        0        0     1091 2024-04-23 15:39:19.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/static/wagtail_fedit/js/licenses/TIPPY.LICENSE
+drwxrwxrwx   0        0        0        0 2024-05-23 09:08:04.378347 wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-05-23 09:08:04.606543 wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/
+-rw-rw-rw-   0        0        0       56 2024-04-16 18:37:39.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/_hook_output.html
+drwxrwxrwx   0        0        0        0 2024-05-23 09:08:04.613561 wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-05-23 09:08:04.637621 wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      708 2024-05-21 20:01:50.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/content/buttons/add_block.html
+-rw-rw-rw-   0        0        0      929 2024-04-23 15:23:24.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html
+-rw-rw-rw-   0        0        0      991 2024-04-23 15:27:54.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
+-rw-rw-rw-   0        0        0      742 2024-05-19 21:41:44.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/content/buttons/move_down.html
+-rw-rw-rw-   0        0        0      738 2024-05-19 21:41:46.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/content/buttons/move_up.html
+-rw-rw-rw-   0        0        0      601 2024-05-17 08:51:23.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
+-rw-rw-rw-   0        0        0      378 2024-05-18 11:23:40.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/content/editable_dom_positioned_adapter.html
+drwxrwxrwx   0        0        0        0 2024-05-23 09:08:04.694026 wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
+-rw-rw-rw-   0        0        0     3699 2024-04-20 21:55:10.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
+-rw-rw-rw-   0        0        0      266 2024-04-21 21:15:09.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler.html
+-rw-rw-rw-   0        0        0      265 2024-04-21 21:23:24.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler_form.html
+-rw-rw-rw-   0        0        0      786 2024-05-18 21:59:44.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html
+-rw-rw-rw-   0        0        0      455 2024-04-21 00:11:35.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form_errors.html
+-rw-rw-rw-   0        0        0      345 2024-05-18 12:28:53.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
+-rw-rw-rw-   0        0        0      397 2024-05-18 21:49:55.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe_dom_positioned.html
+-rw-rw-rw-   0        0        0     5537 2024-05-18 12:20:21.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+-rw-rw-rw-   0        0        0       99 2024-05-21 20:50:08.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/editor/block_adapter_add_form.html
+-rw-rw-rw-   0        0        0      544 2024-05-22 09:02:31.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/editor/block_adapter_iframe.html
+-rw-rw-rw-   0        0        0      549 2024-05-18 15:36:09.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+drwxrwxrwx   0        0        0        0 2024-05-23 09:08:04.713447 wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/icons/
+-rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
+-rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
+-rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
+-rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
+-rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
+drwxrwxrwx   0        0        0        0 2024-05-23 09:08:04.721450 wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+drwxrwxrwx   0        0        0        0 2024-05-23 09:08:04.726095 wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
+-rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
+-rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
+drwxrwxrwx   0        0        0        0 2024-05-23 09:08:04.726095 wagtail_fedit-1.5.9rc4/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 09:08:04.745784 wagtail_fedit-1.5.9rc4/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    13210 2024-05-18 21:38:53.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10414 2024-05-18 21:38:48.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-05-23 09:08:04.752782 wagtail_fedit-1.5.9rc4/wagtail_fedit/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 09:08:04.770918 wagtail_fedit-1.5.9rc4/wagtail_fedit/test/core/
+-rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/test/core/__init__.py
+-rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/test/core/apps.py
+-rw-rw-rw-   0        0        0      130 2024-04-15 20:12:38.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/test/core/context_processors.py
+drwxrwxrwx   0        0        0        0 2024-05-23 09:08:04.783677 wagtail_fedit-1.5.9rc4/wagtail_fedit/test/core/migrations/
+-rw-rw-rw-   0        0        0    12115 2024-04-20 22:33:35.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/test/core/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      509 2024-04-21 18:41:55.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/test/core/migrations/0002_basicmodel_related_field.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/test/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0     6047 2024-04-23 13:09:46.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/test/core/models.py
+drwxrwxrwx   0        0        0        0 2024-05-23 09:08:04.849185 wagtail_fedit-1.5.9rc4/wagtail_fedit/test/core/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/test/core/tests/__init__.py
+-rw-rw-rw-   0        0        0     8962 2024-04-25 13:24:28.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/test/core/tests/base.py
+-rw-rw-rw-   0        0        0    35284 2024-05-23 09:05:27.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/test/core/tests/test_adapters.py
+-rw-rw-rw-   0        0        0     4352 2024-05-19 20:28:32.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/test/core/tests/test_block_edit.py
+-rw-rw-rw-   0        0        0     7467 2024-05-23 09:06:26.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/test/core/tests/test_blocks.py
+-rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/test/core/tests/test_field_edit.py
+-rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/test/core/tests/test_generic.py
+-rw-rw-rw-   0        0        0     4865 2024-04-23 14:23:09.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/test/core/tests/test_model_edit.py
+-rw-rw-rw-   0        0        0     1574 2024-04-20 20:49:12.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/test/core/tests/test_revision.py
+-rw-rw-rw-   0        0        0     9545 2024-04-20 21:54:40.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/test/core/tests/test_submit.py
+-rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/test/manage.py
+drwxrwxrwx   0        0        0        0 2024-05-23 09:08:04.868630 wagtail_fedit-1.5.9rc4/wagtail_fedit/test/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/test/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/test/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3660 2024-05-18 16:08:35.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/test/testapp/settings.py
+-rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/test/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/test/testapp/wsgi.py
+-rw-rw-rw-   0        0        0     2220 2024-04-23 14:21:34.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0     1131 2024-05-18 22:43:51.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0    20217 2024-05-23 08:37:50.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-23 09:08:04.879475 wagtail_fedit-1.5.9rc4/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      215 2024-04-23 17:24:50.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     9286 2024-05-21 20:14:34.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/views/adapters.py
+-rw-rw-rw-   0        0        0    17734 2024-05-20 09:37:43.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0     2239 2024-04-25 09:52:47.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/views/mixins.py
+drwxrwxrwx   0        0        0        0 2024-05-23 09:08:04.933197 wagtail_fedit-1.5.9rc4/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      155 2024-05-18 18:02:59.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0     1907 2024-05-13 18:26:02.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/wagtail_hooks/action_menu.py
+-rw-rw-rw-   0        0        0     2446 2024-05-07 21:59:49.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/wagtail_hooks/adapter_hooks.py
+-rw-rw-rw-   0        0        0     1173 2024-05-18 21:36:35.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/wagtail_hooks/adapters.py
+-rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/wagtail_hooks/icons.py
+-rw-rw-rw-   0        0        0     4017 2024-05-19 22:47:30.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0     7637 2024-04-23 20:17:24.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-05-23 09:08:04.488978 wagtail_fedit-1.5.9rc4/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0     3126 2024-05-23 09:08:04.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5002 2024-05-23 09:08:04.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 09:08:04.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-05-23 09:08:04.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-23 09:08:04.000000 wagtail_fedit-1.5.9rc4/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.5.9rc3/LICENSE` & `wagtail_fedit-1.5.9rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/PKG-INFO` & `wagtail_fedit-1.5.9rc4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.5.9rc3
+Version: 1.5.9rc4
 Summary: Frontend editing for your Wagtail site
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-2.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `wagtail_fedit-1.5.9rc3/README.md` & `wagtail_fedit-1.5.9rc4/README.md`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/setup.cfg` & `wagtail_fedit-1.5.9rc4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 352e  ..version = 1.5.
-00000030: 3972 6333 0d0a 6465 7363 7269 7074 696f  9rc3..descriptio
+00000030: 3972 6334 0d0a 6465 7363 7269 7074 696f  9rc4..descriptio
 00000040: 6e20 3d20 4672 6f6e 7465 6e64 2065 6469  n = Frontend edi
 00000050: 7469 6e67 2066 6f72 2079 6f75 7220 5761  ting for your Wa
 00000060: 6774 6169 6c20 7369 7465 0d0a 6c6f 6e67  gtail site..long
 00000070: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 00000080: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
 00000090: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 000000a0: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type =
```

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/adapters/base.py` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/adapters/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/adapters/block/adapter.py` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/adapters/block/adapter.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/adapters/block/buttons.py` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/adapters/block/buttons.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/adapters/block/views.py` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/adapters/block/views.py`

 * *Files 16% similar despite different names*

```diff
@@ -54,22 +54,29 @@
             })
         
         action = self.request.GET.get("action")
         idx = self.adapter.block_index
         parent = self.adapter.parent
         if action.lower() == "up":
             if idx > 0 and idx < len(parent):
-                parent[idx], parent[idx - 1] = parent[idx - 1], parent[idx]
+                if isinstance(parent, StreamValue):
+                    parent._raw_data[idx], parent._raw_data[idx - 1] = parent._raw_data[idx - 1], parent._raw_data[idx]
+                    parent[idx], parent[idx - 1] = parent[idx - 1], parent[idx]
+                elif isinstance(parent, ListValue):
+                    parent.bound_blocks[idx], parent.bound_blocks[idx - 1] = parent.bound_blocks[idx - 1], parent.bound_blocks[idx]
             else:
                 return JsonResponse({"error": "Cannot move block up"})
 
         elif action.lower() == "down":
             if idx < len(parent) - 1 and idx >= 0:
-                parent[idx], parent[idx + 1] = parent[idx + 1], parent[idx]
-
+                if isinstance(parent, StreamValue):
+                    parent._raw_data[idx], parent._raw_data[idx + 1] = parent._raw_data[idx + 1], parent._raw_data[idx]
+                    parent[idx], parent[idx + 1] = parent[idx + 1], parent[idx]
+                elif isinstance(parent, ListValue):
+                    parent.bound_blocks[idx], parent.bound_blocks[idx + 1] = parent.bound_blocks[idx + 1], parent.bound_blocks[idx]
                 # if isinstance(parent, StreamValue):
                     # parent._raw_data[idx], parent._raw_data[idx + 1] = parent._raw_data[idx + 1], parent._raw_data[idx]
             else:
                 return JsonResponse({"error": "Cannot move block down"})
         else:
             return JsonResponse({"error": "Invalid action"})
```

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/adapters/field.py` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/adapters/field.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/adapters/funcs.py` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/adapters/funcs.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/adapters/misc.py` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/adapters/misc.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/adapters/models.py` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/adapters/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/errors.py` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/errors.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/forms/blocks.py` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/forms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/forms/fields.py` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/forms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/hooks.py` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/locale/nl/LC_MESSAGES/django.po` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/models.py` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/registry.py` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/registry.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/settings.py` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/static/wagtail_fedit/js/edit.js` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/static/wagtail_fedit/js/edit.js`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/static/wagtail_fedit/js/licenses/TIPPY.LICENSE` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/static/wagtail_fedit/js/licenses/TIPPY.LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/content/buttons/add_block.html` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/content/buttons/add_block.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/content/buttons/move_down.html` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/content/buttons/move_down.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/content/buttons/move_up.html` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/content/buttons/move_up.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/editor/block_adapter_iframe.html` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/editor/block_adapter_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/editor/field.html` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/editor/field.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/templatetags/fedit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/test/core/migrations/0001_initial.py` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/test/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/test/core/models.py` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/test/core/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/test/core/tests/base.py` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/test/core/tests/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/test/core/tests/test_adapters.py` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/test/core/tests/test_adapters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from django.db.models.base import Model as Model
 from django.http import HttpRequest
 from django.urls import reverse
 from django.template import (
     Context, Template,
     TemplateSyntaxError,
 )
+from wagtail.blocks import (
+    BlockWidget,
+)
 from wagtail_fedit.adapters import (
     Keyword,
     BaseAdapter,
     BlockAdapter,
     FieldAdapter,
     ModelAdapter,
 )
@@ -26,14 +29,17 @@
     shared_context_url,
     get_reverse_kwargs,
     find_block,
 )
 from wagtail_fedit.templatetags.fedit import (
     wrap_adapter,
 )
+from ..models import (
+    MenuItemBlock,
+)
 from .base import (
     BaseFEditTest,
 )
 
 import json
 
 adapters = {}
@@ -708,15 +714,15 @@
 
         block = find_block(second_streamfield_listvalue_item, streamfield)
         block_value, _, parent, idx = block
         if idx != 1:
             self.fail(f"Expected 1, got {idx}")
 
         self.assertEqual(
-            parent[idx].value["link"]["text"],
+            parent.bound_blocks[idx].value["link"]["text"],
             "Test Item 2",
         )
 
         request = self.request_factory.get(
             self.get_editable_url(
                 self.basic_model.pk, self.basic_model._meta.app_label, self.basic_model._meta.model_name,
             )
@@ -759,20 +765,20 @@
         block = find_block(second_streamfield_listvalue_item, streamfield)
         block_value, _, parent, idx = block
 
         if idx != 0:
             self.fail(f"Expected 0, got {idx}")
             
         self.assertDictEqual(
-            parent[idx].value,
+            parent.bound_blocks[idx].value,
             block_value.value,
         )
 
         self.assertEqual(
-            parent[idx].value["link"]["text"],
+            parent.bound_blocks[idx].value["link"]["text"],
             "Test Item 2",
         )
 
 
     def test_move_block_down(self):
         id = get_adapter_id()
         streamfield = self.basic_model.content
@@ -781,15 +787,15 @@
 
         block = find_block(first_streamfield_listvalue_item, streamfield)
         block_value, _, parent, idx = block
         if idx != 0:
             self.fail(f"Expected 0, got {idx}")
 
         self.assertEqual(
-            parent[idx].value["link"]["text"],
+            parent.bound_blocks[idx].value["link"]["text"],
             "Test Item 1",
         )
 
         request = self.request_factory.get(
             self.get_editable_url(
                 self.basic_model.pk, self.basic_model._meta.app_label, self.basic_model._meta.model_name,
             )
@@ -823,33 +829,108 @@
         self.assertDictEqual(
             json.loads(response.content.decode("utf-8")),
             {
                 "success": True,
             }
         )
 
-        self.basic_model.refresh_from_db()
-
+        self.basic_model = self.basic_model.__class__.objects.get(pk=self.basic_model.pk)
         streamfield = self.basic_model.content
         block = find_block(first_streamfield_listvalue_item, streamfield)
         block_value, _, parent, idx = block
 
         if idx != 1:
             self.fail(f"Expected 1, got {idx}")
             
         self.assertDictEqual(
-            parent[idx].value,
+            parent.bound_blocks[idx].value,
             block_value.value,
         )
 
         self.assertEqual(
-            parent[idx].value["link"]["text"],
+            parent.bound_blocks[idx].value["link"]["text"],
             "Test Item 1",
         )
 
+    def test_add_block(self):
+        id = get_adapter_id()
+        streamfield = self.basic_model.content
+
+        first_streamfield_listvalue_item = "c757f54d-0df5-4b35-8a06-4174f180ec41"
+
+        block = find_block(first_streamfield_listvalue_item, streamfield)
+        block_value, _, parent, idx = block
+        if idx != 0:
+            self.fail(f"Expected 0, got {idx}")
+
+        self.assertEqual(
+            parent.bound_blocks[idx].value["link"]["text"],
+            "Test Item 1",
+        )
+
+        request = self.request_factory.get(
+            self.get_editable_url(
+                self.basic_model.pk, self.basic_model._meta.app_label, self.basic_model._meta.model_name,
+            )
+        )
+        adapter = TestBlockAdapter(
+            self.basic_model,
+            "content",
+            request,
+            id=id,
+            block=block_value,
+            block_id=first_streamfield_listvalue_item,
+            movable=True,
+            addable=True,
+        )
+
+        url = shared_context_url(
+            adapter.encode_shared_context(),
+            reverse(
+                "wagtail_fedit:block-add",
+                kwargs=get_reverse_kwargs(adapter)
+            ),
+        )
+
+        block_value = {
+            "wagtail-fedit-block-add-count": 1,
+            "wagtail-fedit-block-add-0-deleted": "",
+            "wagtail-fedit-block-add-0-order": 0,
+            "wagtail-fedit-block-add-0-type": "item",
+            "wagtail-fedit-block-add-0-value-link-text": "Test Item Addition",
+        }
+
+        self.client.force_login(self.admin_user)
+
+        response = self.client.post(url, block_value)
+        if response.status_code != 200:
+            self.fail(f"Expected 200, got {response.status_code} ({response.content})")
+
+        self.assertDictEqual(
+            json.loads(response.content.decode("utf-8")),
+            {
+                "success": True,
+            }
+        )
+
+        self.basic_model.refresh_from_db()
+
+        streamfield = self.basic_model.content
+        block = find_block(first_streamfield_listvalue_item, streamfield)
+        block_value, _, parent, idx = block
+
+        if idx != 0:
+            self.fail(f"Expected 1, got {idx}")
+
+        link_text = parent.bound_blocks[idx + 1].value["link"]["text"]
+
+        self.assertEqual(
+            link_text,
+            "Test Item Addition",
+        )
 
     def test_render_from_context(self):
         id = get_adapter_id()
         streamfield = self.basic_model.content
         block = find_block(self.BLOCK_ID, streamfield)
         request = self.request_factory.get(
             self.get_editable_url(
```

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/test/core/tests/test_block_edit.py` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/test/core/tests/test_block_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/test/core/tests/test_blocks.py` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/test/core/tests/test_blocks.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,41 +74,41 @@
 
     def test_find_block_parent(self):
         block, contentpath, parent, idx = utils.find_block("d543a6bf-34dc-4365-a3fa-d302561930ae", self.stream_value)
         self.assertEqual(parent, self.stream_value)
 
         block, contentpath, parent, idx = utils.find_block("a98a19c6-2ead-4e69-9ea2-3158c7e82976", self.stream_value)
         self.assertEqual(idx, 2)
-        self.assertEqual(parent[idx].value["link"]["text"], "Test Item 3")
+        self.assertEqual(parent.bound_blocks[idx].value["link"]["text"], "Test Item 3")
     
     def test_move_block_down(self):
         block, contentpath, parent, idx = utils.find_block("a98a19c6-2ead-4e69-9ea2-3158c7e82976", self.stream_value)
         self.assertEqual(idx, 2)
-        self.assertEqual(parent[idx].value["link"]["text"], "Test Item 3")
+        self.assertEqual(parent.bound_blocks[idx].value["link"]["text"], "Test Item 3")
 
         if idx < len(parent) - 1:
             parent[idx], parent[idx + 1] = parent[idx + 1], parent[idx]
         else:
             self.fail("Block is already at the bottom")
 
-        self.assertEqual(parent[idx].value["link"]["text"], "Test Item 4")
-        self.assertEqual(parent[idx + 1].value["link"]["text"], "Test Item 3")
+        self.assertEqual(parent.bound_blocks[idx].value["link"]["text"], "Test Item 4")
+        self.assertEqual(parent.bound_blocks[idx + 1].value["link"]["text"], "Test Item 3")
 
     def test_move_block_up(self):
         block, contentpath, parent, idx = utils.find_block("a98a19c6-2ead-4e69-9ea2-3158c7e82976", self.stream_value)
         self.assertEqual(idx, 2)
-        self.assertEqual(parent[idx].value["link"]["text"], "Test Item 3")
+        self.assertEqual(parent.bound_blocks[idx].value["link"]["text"], "Test Item 3")
 
         if idx > 0:
             parent[idx], parent[idx - 1] = parent[idx - 1], parent[idx]
         else:
             self.fail("Block is already at the top")
 
-        self.assertEqual(parent[idx].value["link"]["text"], "Test Item 2")
-        self.assertEqual(parent[idx - 1].value["link"]["text"], "Test Item 3")
+        self.assertEqual(parent.bound_blocks[idx].value["link"]["text"], "Test Item 2")
+        self.assertEqual(parent.bound_blocks[idx - 1].value["link"]["text"], "Test Item 3")
 
     def test_get_form_class(self):
         block = utils.find_block("d543a6bf-34dc-4365-a3fa-d302561930ae", self.stream_value)[0]
         form_class = block_forms.get_block_form_class(block.block)
         self.assertIsNotNone(form_class)
 
         VALID_DATA = {
```

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/test/core/tests/test_field_edit.py` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/test/core/tests/test_field_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/test/core/tests/test_generic.py` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/test/core/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/test/core/tests/test_model_edit.py` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/test/core/tests/test_model_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/test/core/tests/test_revision.py` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/test/core/tests/test_revision.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/test/core/tests/test_submit.py` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/test/core/tests/test_submit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/test/manage.py` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/test/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/test/testapp/settings.py` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/test/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/test/testapp/urls.py` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/test/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/toolbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/urls.py` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/utils.py` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,29 +194,31 @@
     - contentpath is a list of block names leading to the block
     - parent_block is the parent block of the block with the given ID
     - block_index is the index of the block within the parent block's value list
     """
     if contentpath is None:
         contentpath = []
 
-    # Check and cast field to iterable if necessary, but do not append non-StreamValue names to contentpath here.
+    parent_block = field
+
+    # Check and cast field to iterable if necessary, but do not append non-StreamValue names to contentpath here.    
     if not isinstance(field, (StreamValue, ListValue)) and not hasattr(field, "__iter__"):
         field = [field]
 
     # Adjust for ListValue to get the iterable bound_blocks.
     if isinstance(field, ListValue):
         field = field.bound_blocks
 
     for idx, block in enumerate(field):
         # Determine the block's name only if needed to avoid premature addition to contentpath.
         block_name = get_block_path(block)
         
         if getattr(block, "id", None) == block_id:
             # Append the block name here as it directly leads to the target.
-            return block, contentpath + [block_name], field, idx
+            return block, contentpath + [block_name], parent_block, idx
         
         # Prepare to check children without altering the current path yet.
         if isinstance(block.value, blocks.StructValue):
             for value in block.value.bound_blocks.values():
                 found, found_path, parent, block_index = find_block(block_id, value, contentpath + [block_name])
                 if found:
                     return found, found_path, parent, block_index
```

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/views/adapters.py` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/views/adapters.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/views/editable.py` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/views/editable.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/views/mixins.py` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/views/mixins.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/wagtail_hooks/action_menu.py` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/wagtail_hooks/action_menu.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/wagtail_hooks/adapter_hooks.py` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/wagtail_hooks/adapter_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/wagtail_hooks/adapters.py` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/wagtail_hooks/adapters.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.5.9rc4/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit.egg-info/PKG-INFO` & `wagtail_fedit-1.5.9rc4/wagtail_fedit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-fedit
-Version: 1.5.9rc3
+Version: 1.5.9rc4
 Summary: Frontend editing for your Wagtail site
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-2.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `wagtail_fedit-1.5.9rc3/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.5.9rc4/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

