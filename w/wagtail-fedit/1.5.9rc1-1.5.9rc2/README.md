# Comparing `tmp/wagtail_fedit-1.5.9rc1.tar.gz` & `tmp/wagtail_fedit-1.5.9rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.5.9rc1.tar", last modified: Mon May 20 19:49:27 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.5.9rc2.tar", last modified: Thu May 23 07:47:46 2024, max compression
```

## Comparing `wagtail_fedit-1.5.9rc1.tar` & `wagtail_fedit-1.5.9rc2.tar`

### file list

```diff
@@ -1,138 +1,145 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 19:49:27.065934 wagtail_fedit-1.5.9rc1/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.9rc1/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.9rc1/MANIFEST.in
--rw-rw-rw-   0        0        0     3093 2024-05-20 19:49:27.065934 wagtail_fedit-1.5.9rc1/PKG-INFO
--rw-rw-rw-   0        0        0     1892 2024-05-20 10:40:42.000000 wagtail_fedit-1.5.9rc1/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.9rc1/pyproject.toml
--rw-rw-rw-   0        0        0     1189 2024-05-20 19:49:27.066941 wagtail_fedit-1.5.9rc1/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.9rc1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-20 19:49:26.973551 wagtail_fedit-1.5.9rc1/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 19:49:26.985927 wagtail_fedit-1.5.9rc1/wagtail_fedit/adapters/
--rw-rw-rw-   0        0        0      455 2024-05-18 21:36:58.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/adapters/__init__.py
--rw-rw-rw-   0        0        0    15622 2024-05-19 22:05:36.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/adapters/base.py
--rw-rw-rw-   0        0        0    10801 2024-05-20 10:35:06.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/adapters/block.py
--rw-rw-rw-   0        0        0     8946 2024-05-19 22:04:41.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/adapters/field.py
--rw-rw-rw-   0        0        0     2305 2024-04-25 18:28:58.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/adapters/funcs.py
--rw-rw-rw-   0        0        0     2755 2024-04-25 18:28:49.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/adapters/misc.py
--rw-rw-rw-   0        0        0     5665 2024-05-19 22:05:27.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/adapters/models.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/apps.py
--rw-rw-rw-   0        0        0     1354 2024-04-25 09:55:56.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/errors.py
-drwxrwxrwx   0        0        0        0 2024-05-20 19:49:26.988931 wagtail_fedit-1.5.9rc1/wagtail_fedit/forms/
--rw-rw-rw-   0        0        0      215 2024-04-23 13:02:23.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/forms/__init__.py
--rw-rw-rw-   0        0        0     2881 2024-04-18 20:27:35.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/forms/blocks.py
--rw-rw-rw-   0        0        0     3269 2024-04-23 13:28:56.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/forms/fields.py
--rw-rw-rw-   0        0        0     5612 2024-05-18 18:03:06.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-05-20 19:49:26.948845 wagtail_fedit-1.5.9rc1/wagtail_fedit/locale/
-drwxrwxrwx   0        0        0        0 2024-05-20 19:49:26.948845 wagtail_fedit-1.5.9rc1/wagtail_fedit/locale/nl/
-drwxrwxrwx   0        0        0        0 2024-05-20 19:49:26.992200 wagtail_fedit-1.5.9rc1/wagtail_fedit/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0        0        0     9614 2024-05-19 22:55:13.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    16810 2024-05-19 22:55:04.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2024-05-20 19:49:26.993147 wagtail_fedit-1.5.9rc1/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 19:49:26.994154 wagtail_fedit-1.5.9rc1/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/models.py
--rw-rw-rw-   0        0        0     1451 2024-05-18 21:38:18.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/registry.py
--rw-rw-rw-   0        0        0     1626 2024-04-25 13:40:59.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/settings.py
-drwxrwxrwx   0        0        0        0 2024-05-20 19:49:26.949854 wagtail_fedit-1.5.9rc1/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-05-20 19:49:26.951380 wagtail_fedit-1.5.9rc1/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-05-20 19:49:26.996152 wagtail_fedit-1.5.9rc1/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0     5862 2024-05-18 21:44:47.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     4997 2024-05-18 21:47:34.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/static/wagtail_fedit/css/furniture.css
--rw-rw-rw-   0        0        0     1249 2024-05-18 12:55:22.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
-drwxrwxrwx   0        0        0        0 2024-05-20 19:49:26.997559 wagtail_fedit-1.5.9rc1/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    56782 2024-05-20 19:49:23.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/static/wagtail_fedit/js/edit.js
-drwxrwxrwx   0        0        0        0 2024-05-20 19:49:26.998565 wagtail_fedit-1.5.9rc1/wagtail_fedit/static/wagtail_fedit/js/licenses/
--rw-rw-rw-   0        0        0     1091 2024-04-23 15:39:19.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/static/wagtail_fedit/js/licenses/TIPPY.LICENSE
-drwxrwxrwx   0        0        0        0 2024-05-20 19:49:26.952057 wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-05-20 19:49:26.999565 wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/wagtail_fedit/
--rw-rw-rw-   0        0        0       56 2024-04-16 18:37:39.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/wagtail_fedit/_hook_output.html
-drwxrwxrwx   0        0        0        0 2024-05-20 19:49:27.001565 wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-05-20 19:49:27.006336 wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      929 2024-04-23 15:23:24.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html
--rw-rw-rw-   0        0        0      991 2024-04-23 15:27:54.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
--rw-rw-rw-   0        0        0      742 2024-05-19 21:41:44.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/wagtail_fedit/content/buttons/move_down.html
--rw-rw-rw-   0        0        0      738 2024-05-19 21:41:46.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/wagtail_fedit/content/buttons/move_up.html
--rw-rw-rw-   0        0        0      601 2024-05-17 08:51:23.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
--rw-rw-rw-   0        0        0      378 2024-05-18 11:23:40.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/wagtail_fedit/content/editable_dom_positioned_adapter.html
-drwxrwxrwx   0        0        0        0 2024-05-20 19:49:27.014545 wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
--rw-rw-rw-   0        0        0     3699 2024-04-20 21:55:10.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
--rw-rw-rw-   0        0        0      266 2024-04-21 21:15:09.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler.html
--rw-rw-rw-   0        0        0      265 2024-04-21 21:23:24.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler_form.html
--rw-rw-rw-   0        0        0      786 2024-05-18 21:59:44.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html
--rw-rw-rw-   0        0        0      455 2024-04-21 00:11:35.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form_errors.html
--rw-rw-rw-   0        0        0      345 2024-05-18 12:28:53.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
--rw-rw-rw-   0        0        0      397 2024-05-18 21:49:55.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe_dom_positioned.html
--rw-rw-rw-   0        0        0     5537 2024-05-18 12:20:21.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
--rw-rw-rw-   0        0        0      549 2024-05-18 15:36:09.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/wagtail_fedit/editor/field.html
-drwxrwxrwx   0        0        0        0 2024-05-20 19:49:27.019890 wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/wagtail_fedit/icons/
--rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
--rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
--rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
--rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
--rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
-drwxrwxrwx   0        0        0        0 2024-05-20 19:49:27.022889 wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
-drwxrwxrwx   0        0        0        0 2024-05-20 19:49:27.024059 wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
--rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
--rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
-drwxrwxrwx   0        0        0        0 2024-05-20 19:49:27.024059 wagtail_fedit-1.5.9rc1/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 19:49:27.029753 wagtail_fedit-1.5.9rc1/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    13210 2024-05-18 21:38:53.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0    10414 2024-05-18 21:38:48.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-05-20 19:49:27.030750 wagtail_fedit-1.5.9rc1/wagtail_fedit/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 19:49:27.033671 wagtail_fedit-1.5.9rc1/wagtail_fedit/test/core/
--rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/test/core/__init__.py
--rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/test/core/apps.py
--rw-rw-rw-   0        0        0      130 2024-04-15 20:12:38.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/test/core/context_processors.py
-drwxrwxrwx   0        0        0        0 2024-05-20 19:49:27.036947 wagtail_fedit-1.5.9rc1/wagtail_fedit/test/core/migrations/
--rw-rw-rw-   0        0        0    12115 2024-04-20 22:33:35.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/test/core/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      509 2024-04-21 18:41:55.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/test/core/migrations/0002_basicmodel_related_field.py
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/test/core/migrations/__init__.py
--rw-rw-rw-   0        0        0     6047 2024-04-23 13:09:46.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/test/core/models.py
-drwxrwxrwx   0        0        0        0 2024-05-20 19:49:27.047918 wagtail_fedit-1.5.9rc1/wagtail_fedit/test/core/tests/
--rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/test/core/tests/__init__.py
--rw-rw-rw-   0        0        0     8962 2024-04-25 13:24:28.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/test/core/tests/base.py
--rw-rw-rw-   0        0        0    32593 2024-05-20 12:32:25.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/test/core/tests/test_adapters.py
--rw-rw-rw-   0        0        0     4352 2024-05-19 20:28:32.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/test/core/tests/test_block_edit.py
--rw-rw-rw-   0        0        0     7376 2024-05-19 20:53:17.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/test/core/tests/test_blocks.py
--rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/test/core/tests/test_field_edit.py
--rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/test/core/tests/test_generic.py
--rw-rw-rw-   0        0        0     4865 2024-04-23 14:23:09.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/test/core/tests/test_model_edit.py
--rw-rw-rw-   0        0        0     1574 2024-04-20 20:49:12.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/test/core/tests/test_revision.py
--rw-rw-rw-   0        0        0     9545 2024-04-20 21:54:40.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/test/core/tests/test_submit.py
--rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/test/manage.py
-drwxrwxrwx   0        0        0        0 2024-05-20 19:49:27.052901 wagtail_fedit-1.5.9rc1/wagtail_fedit/test/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/test/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/test/testapp/asgi.py
--rw-rw-rw-   0        0        0     3660 2024-05-18 16:08:35.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/test/testapp/settings.py
--rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/test/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/test/testapp/wsgi.py
--rw-rw-rw-   0        0        0     2220 2024-04-23 14:21:34.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0     1131 2024-05-18 22:43:51.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0    18837 2024-05-19 22:26:15.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-20 19:49:27.057926 wagtail_fedit-1.5.9rc1/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      215 2024-04-23 17:24:50.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     9078 2024-05-19 20:23:42.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/views/adapters.py
--rw-rw-rw-   0        0        0    17734 2024-05-20 09:37:43.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0     2239 2024-04-25 09:52:47.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/views/mixins.py
-drwxrwxrwx   0        0        0        0 2024-05-20 19:49:27.062695 wagtail_fedit-1.5.9rc1/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      155 2024-05-18 18:02:59.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0     1907 2024-05-13 18:26:02.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/wagtail_hooks/action_menu.py
--rw-rw-rw-   0        0        0     2446 2024-05-07 21:59:49.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/wagtail_hooks/adapter_hooks.py
--rw-rw-rw-   0        0        0     1173 2024-05-18 21:36:35.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/wagtail_hooks/adapters.py
--rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/wagtail_hooks/icons.py
--rw-rw-rw-   0        0        0     4017 2024-05-19 22:47:30.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0     7637 2024-04-23 20:17:24.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-05-20 19:49:26.980613 wagtail_fedit-1.5.9rc1/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0     3093 2024-05-20 19:49:26.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4662 2024-05-20 19:49:26.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 19:49:26.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-05-20 19:49:26.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-20 19:49:26.000000 wagtail_fedit-1.5.9rc1/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 07:47:46.896395 wagtail_fedit-1.5.9rc2/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.9rc2/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.9rc2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3093 2024-05-23 07:47:46.897404 wagtail_fedit-1.5.9rc2/PKG-INFO
+-rw-rw-rw-   0        0        0     1892 2024-05-20 10:40:42.000000 wagtail_fedit-1.5.9rc2/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.9rc2/pyproject.toml
+-rw-rw-rw-   0        0        0     1189 2024-05-23 07:47:46.899031 wagtail_fedit-1.5.9rc2/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.9rc2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 07:47:46.715255 wagtail_fedit-1.5.9rc2/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 07:47:46.731959 wagtail_fedit-1.5.9rc2/wagtail_fedit/adapters/
+-rw-rw-rw-   0        0        0      455 2024-05-21 19:49:09.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/adapters/__init__.py
+-rw-rw-rw-   0        0        0    15762 2024-05-21 19:41:15.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/adapters/base.py
+drwxrwxrwx   0        0        0        0 2024-05-23 07:47:46.746976 wagtail_fedit-1.5.9rc2/wagtail_fedit/adapters/block/
+-rw-rw-rw-   0        0        0       76 2024-05-21 19:49:08.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/adapters/block/__init__.py
+-rw-rw-rw-   0        0        0     8345 2024-05-22 10:03:59.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/adapters/block/adapter.py
+-rw-rw-rw-   0        0        0     1800 2024-05-21 19:53:21.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/adapters/block/buttons.py
+-rw-rw-rw-   0        0        0     5509 2024-05-22 10:06:29.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/adapters/block/views.py
+-rw-rw-rw-   0        0        0     8946 2024-05-19 22:04:41.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/adapters/field.py
+-rw-rw-rw-   0        0        0     2305 2024-04-25 18:28:58.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/adapters/funcs.py
+-rw-rw-rw-   0        0        0     2755 2024-04-25 18:28:49.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/adapters/misc.py
+-rw-rw-rw-   0        0        0     5665 2024-05-19 22:05:27.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/adapters/models.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/apps.py
+-rw-rw-rw-   0        0        0     1354 2024-04-25 09:55:56.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/errors.py
+drwxrwxrwx   0        0        0        0 2024-05-23 07:47:46.753926 wagtail_fedit-1.5.9rc2/wagtail_fedit/forms/
+-rw-rw-rw-   0        0        0      215 2024-04-23 13:02:23.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/forms/__init__.py
+-rw-rw-rw-   0        0        0     2881 2024-04-18 20:27:35.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/forms/blocks.py
+-rw-rw-rw-   0        0        0     3269 2024-04-23 13:28:56.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/forms/fields.py
+-rw-rw-rw-   0        0        0     5612 2024-05-18 18:03:06.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-05-23 07:47:46.665280 wagtail_fedit-1.5.9rc2/wagtail_fedit/locale/
+drwxrwxrwx   0        0        0        0 2024-05-23 07:47:46.665280 wagtail_fedit-1.5.9rc2/wagtail_fedit/locale/nl/
+drwxrwxrwx   0        0        0        0 2024-05-23 07:47:46.757926 wagtail_fedit-1.5.9rc2/wagtail_fedit/locale/nl/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     9614 2024-05-19 22:55:13.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    16810 2024-05-19 22:55:04.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/locale/nl/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2024-05-23 07:47:46.759926 wagtail_fedit-1.5.9rc2/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 07:47:46.762098 wagtail_fedit-1.5.9rc2/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3170 2024-04-05 20:30:10.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/models.py
+-rw-rw-rw-   0        0        0     1451 2024-05-18 21:38:18.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/registry.py
+-rw-rw-rw-   0        0        0     1626 2024-04-25 13:40:59.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/settings.py
+drwxrwxrwx   0        0        0        0 2024-05-23 07:47:46.680641 wagtail_fedit-1.5.9rc2/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-05-23 07:47:46.681934 wagtail_fedit-1.5.9rc2/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-05-23 07:47:46.769582 wagtail_fedit-1.5.9rc2/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0     5957 2024-05-22 09:18:05.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     5091 2024-05-22 09:07:12.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+-rw-rw-rw-   0        0        0     1249 2024-05-18 12:55:22.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
+drwxrwxrwx   0        0        0        0 2024-05-23 07:47:46.771579 wagtail_fedit-1.5.9rc2/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    58202 2024-05-23 07:47:43.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/static/wagtail_fedit/js/edit.js
+drwxrwxrwx   0        0        0        0 2024-05-23 07:47:46.773103 wagtail_fedit-1.5.9rc2/wagtail_fedit/static/wagtail_fedit/js/licenses/
+-rw-rw-rw-   0        0        0     1091 2024-04-23 15:39:19.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/static/wagtail_fedit/js/licenses/TIPPY.LICENSE
+drwxrwxrwx   0        0        0        0 2024-05-23 07:47:46.681934 wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-05-23 07:47:46.773103 wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/
+-rw-rw-rw-   0        0        0       56 2024-04-16 18:37:39.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/_hook_output.html
+drwxrwxrwx   0        0        0        0 2024-05-23 07:47:46.781241 wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-05-23 07:47:46.782119 wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      708 2024-05-21 20:01:50.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/content/buttons/add_block.html
+-rw-rw-rw-   0        0        0      929 2024-04-23 15:23:24.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html
+-rw-rw-rw-   0        0        0      991 2024-04-23 15:27:54.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
+-rw-rw-rw-   0        0        0      742 2024-05-19 21:41:44.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/content/buttons/move_down.html
+-rw-rw-rw-   0        0        0      738 2024-05-19 21:41:46.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/content/buttons/move_up.html
+-rw-rw-rw-   0        0        0      601 2024-05-17 08:51:23.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
+-rw-rw-rw-   0        0        0      378 2024-05-18 11:23:40.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/content/editable_dom_positioned_adapter.html
+drwxrwxrwx   0        0        0        0 2024-05-23 07:47:46.815362 wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0     2259 2024-04-11 08:02:26.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
+-rw-rw-rw-   0        0        0     3699 2024-04-20 21:55:10.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
+-rw-rw-rw-   0        0        0      266 2024-04-21 21:15:09.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler.html
+-rw-rw-rw-   0        0        0      265 2024-04-21 21:23:24.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler_form.html
+-rw-rw-rw-   0        0        0      786 2024-05-18 21:59:44.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html
+-rw-rw-rw-   0        0        0      455 2024-04-21 00:11:35.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form_errors.html
+-rw-rw-rw-   0        0        0      345 2024-05-18 12:28:53.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
+-rw-rw-rw-   0        0        0      397 2024-05-18 21:49:55.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe_dom_positioned.html
+-rw-rw-rw-   0        0        0     5537 2024-05-18 12:20:21.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+-rw-rw-rw-   0        0        0       99 2024-05-21 20:50:08.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/editor/block_adapter_add_form.html
+-rw-rw-rw-   0        0        0      544 2024-05-22 09:02:31.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/editor/block_adapter_iframe.html
+-rw-rw-rw-   0        0        0      549 2024-05-18 15:36:09.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+drwxrwxrwx   0        0        0        0 2024-05-23 07:47:46.825399 wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/icons/
+-rw-rw-rw-   0        0        0      797 2024-04-11 08:36:19.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
+-rw-rw-rw-   0        0        0      584 2024-04-11 08:36:55.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
+-rw-rw-rw-   0        0        0      377 2024-04-11 08:23:07.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
+-rw-rw-rw-   0        0        0      725 2024-04-11 09:02:58.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
+-rw-rw-rw-   0        0        0     1323 2024-04-11 08:36:52.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
+drwxrwxrwx   0        0        0        0 2024-05-23 07:47:46.828409 wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+drwxrwxrwx   0        0        0        0 2024-05-23 07:47:46.830417 wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/
+-rw-rw-rw-   0        0        0      263 2024-04-11 08:24:35.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/action_button.html
+-rw-rw-rw-   0        0        0      967 2024-04-11 09:03:51.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html
+drwxrwxrwx   0        0        0        0 2024-05-23 07:47:46.832011 wagtail_fedit-1.5.9rc2/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 07:47:46.832011 wagtail_fedit-1.5.9rc2/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    13210 2024-05-18 21:38:53.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10414 2024-05-18 21:38:48.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-05-23 07:47:46.842102 wagtail_fedit-1.5.9rc2/wagtail_fedit/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 07:47:46.847809 wagtail_fedit-1.5.9rc2/wagtail_fedit/test/core/
+-rw-rw-rw-   0        0        0      151 2024-04-05 07:59:49.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/test/core/__init__.py
+-rw-rw-rw-   0        0        0      165 2024-04-05 08:41:40.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/test/core/apps.py
+-rw-rw-rw-   0        0        0      130 2024-04-15 20:12:38.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/test/core/context_processors.py
+drwxrwxrwx   0        0        0        0 2024-05-23 07:47:46.848625 wagtail_fedit-1.5.9rc2/wagtail_fedit/test/core/migrations/
+-rw-rw-rw-   0        0        0    12115 2024-04-20 22:33:35.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/test/core/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      509 2024-04-21 18:41:55.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/test/core/migrations/0002_basicmodel_related_field.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/test/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0     6047 2024-04-23 13:09:46.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/test/core/models.py
+drwxrwxrwx   0        0        0        0 2024-05-23 07:47:46.865462 wagtail_fedit-1.5.9rc2/wagtail_fedit/test/core/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-05 07:59:29.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/test/core/tests/__init__.py
+-rw-rw-rw-   0        0        0     8962 2024-04-25 13:24:28.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/test/core/tests/base.py
+-rw-rw-rw-   0        0        0    32593 2024-05-20 12:32:25.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/test/core/tests/test_adapters.py
+-rw-rw-rw-   0        0        0     4352 2024-05-19 20:28:32.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/test/core/tests/test_block_edit.py
+-rw-rw-rw-   0        0        0     7376 2024-05-19 20:53:17.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/test/core/tests/test_blocks.py
+-rw-rw-rw-   0        0        0     3642 2024-04-05 18:00:23.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/test/core/tests/test_field_edit.py
+-rw-rw-rw-   0        0        0     3709 2024-04-10 13:03:30.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/test/core/tests/test_generic.py
+-rw-rw-rw-   0        0        0     4865 2024-04-23 14:23:09.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/test/core/tests/test_model_edit.py
+-rw-rw-rw-   0        0        0     1574 2024-04-20 20:49:12.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/test/core/tests/test_revision.py
+-rw-rw-rw-   0        0        0     9545 2024-04-20 21:54:40.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/test/core/tests/test_submit.py
+-rw-rw-rw-   0        0        0      704 2024-04-05 17:55:36.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/test/manage.py
+drwxrwxrwx   0        0        0        0 2024-05-23 07:47:46.876816 wagtail_fedit-1.5.9rc2/wagtail_fedit/test/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/test/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/test/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3660 2024-05-18 16:08:35.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/test/testapp/settings.py
+-rw-rw-rw-   0        0        0      897 2024-04-05 08:04:53.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/test/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/test/testapp/wsgi.py
+-rw-rw-rw-   0        0        0     2220 2024-04-23 14:21:34.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0     1131 2024-05-18 22:43:51.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0    19872 2024-05-22 09:00:33.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-23 07:47:46.881889 wagtail_fedit-1.5.9rc2/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      215 2024-04-23 17:24:50.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     9286 2024-05-21 20:14:34.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/views/adapters.py
+-rw-rw-rw-   0        0        0    17734 2024-05-20 09:37:43.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0     2239 2024-04-25 09:52:47.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/views/mixins.py
+drwxrwxrwx   0        0        0        0 2024-05-23 07:47:46.894304 wagtail_fedit-1.5.9rc2/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      155 2024-05-18 18:02:59.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0     1907 2024-05-13 18:26:02.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/wagtail_hooks/action_menu.py
+-rw-rw-rw-   0        0        0     2446 2024-05-07 21:59:49.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/wagtail_hooks/adapter_hooks.py
+-rw-rw-rw-   0        0        0     1173 2024-05-18 21:36:35.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/wagtail_hooks/adapters.py
+-rw-rw-rw-   0        0        0      398 2024-04-11 09:03:10.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/wagtail_hooks/icons.py
+-rw-rw-rw-   0        0        0     4017 2024-05-19 22:47:30.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0     7637 2024-04-23 20:17:24.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-05-23 07:47:46.715255 wagtail_fedit-1.5.9rc2/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0     3093 2024-05-23 07:47:46.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5002 2024-05-23 07:47:46.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 07:47:46.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-05-23 07:47:46.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-23 07:47:46.000000 wagtail_fedit-1.5.9rc2/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.5.9rc1/LICENSE` & `wagtail_fedit-1.5.9rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/PKG-INFO` & `wagtail_fedit-1.5.9rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.5.9rc1
+Version: 1.5.9rc2
 Summary: Frontend editing for your Wagtail site
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-2.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `wagtail_fedit-1.5.9rc1/README.md` & `wagtail_fedit-1.5.9rc2/README.md`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/setup.cfg` & `wagtail_fedit-1.5.9rc2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 352e  ..version = 1.5.
-00000030: 3972 6331 0d0a 6465 7363 7269 7074 696f  9rc1..descriptio
+00000030: 3972 6332 0d0a 6465 7363 7269 7074 696f  9rc2..descriptio
 00000040: 6e20 3d20 4672 6f6e 7465 6e64 2065 6469  n = Frontend edi
 00000050: 7469 6e67 2066 6f72 2079 6f75 7220 5761  ting for your Wa
 00000060: 6774 6169 6c20 7369 7465 0d0a 6c6f 6e67  gtail site..long
 00000070: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 00000080: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
 00000090: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 000000a0: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type =
```

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/adapters/base.py` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/adapters/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,14 +176,18 @@
 
 
 class BaseAdapter(FeditIFrameMixin, metaclass=AdapterMeta):
     # Type hints for keyword arguments set by metaclass.
     required_kwargs: tuple[str]
     absolute_tokens: tuple[str]
     _defaults:       dict[str, Any]
+    
+    # Set by utils.wrap_adapter
+    # Automatically sets the encoded context string on the adapter.
+    shared_context_string: str
 
     # How the adapter is identified on inside of the templatetag.
     identifier              = None
 
     # If the templatetag required the first argument to be model.field or just model
     field_required          = True
```

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/adapters/block.py` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/adapters/block/adapter.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,138 +1,58 @@
 from django.db import models
 from django.urls import (
-    path, reverse,
-)
-from django.http import (
-    HttpResponseBadRequest,
-    HttpResponseForbidden,
-    JsonResponse,
+    path,
 )
 from django.utils import translation
 from django.utils.translation import gettext_lazy as _
 from django.utils.functional import cached_property
 from django.http import HttpRequest
 
 from wagtail.log_actions import log
 from wagtail.blocks import (
     StreamValue,
 )
 from wagtail.models import (
     RevisionMixin,
-    Revision,
 )
 
-from .base import (
+from ..base import (
     URLMixin,
     BlockFieldReplacementAdapter,
     DomPositionedMixin,
     AdapterError,
     Keyword,
     VARIABLES,
 )
-from ..views import (
+from ...views import (
     BaseAdapterView,
 )
-from ..forms import (
+from ...forms import (
     blocks as block_forms,
 )
-from .. import utils
+from ... import utils
 from wagtail.admin.admin_url_finder import (
     AdminURLFinder,
 )
-from ..toolbar import (
+from ...toolbar import (
     FeditAdapterComponent,
     FeditAdapterAdminLinkButton,
 )
 
+from .buttons import (
+    MoveUpButton,
+    MoveDownButton,
+    AddableButton,
+)
 
-class BaseMoveButton(FeditAdapterComponent):
-    permissions = [
-        "wagtailadmin.access_admin",
-    ]
-    direction: str
-
-    def get_context_data(self):
-        return super().get_context_data() | {
-            "direction": self.direction,
-            "change_url": utils.shared_context_url(self.adapter.shared_context_string, reverse(
-                "wagtail_fedit:block-move",
-                kwargs=utils.get_reverse_kwargs(self.adapter)
-            ), action=self.direction),
-        }
-
-
-class MoveUpButton(BaseMoveButton):
-    template_name = "wagtail_fedit/content/buttons/move_up.html"
-    direction = "up"
-
-class MoveDownButton(BaseMoveButton):
-    template_name = "wagtail_fedit/content/buttons/move_down.html"
-    direction = "down"
-
-class BlockMoveAdapterView(BaseAdapterView):
-    adapter: "BlockAdapter"
-    
-
-    def post(self, request, *args, **kwargs):
-        if not isinstance(self.adapter, BlockAdapter):
-            return JsonResponse({
-                "error": "Invalid adapter type"
-            })
-
-        if not self.adapter.kwargs["movable"]:
-            return JsonResponse({
-                "error": "Block is not movable"
-            })
-        
-        action = self.request.GET.get("action")
-        idx = self.adapter.block_index
-        parent = self.adapter.parent
-        if action.lower() == "up":
-            if idx > 0 and idx < len(parent):
-                parent[idx], parent[idx - 1] = parent[idx - 1], parent[idx]
-            else:
-                return JsonResponse({"error": "Cannot move block up"})
-
-        elif action.lower() == "down":
-            if idx < len(parent) - 1 and idx >= 0:
-                parent[idx], parent[idx + 1] = parent[idx + 1], parent[idx]
-            else:
-                return JsonResponse({"error": "Cannot move block down"})
-        else:
-            return JsonResponse({"error": "Invalid action"})
-        
-        if isinstance(self.adapter.object, RevisionMixin):
-            self.adapter.object.save_revision(
-                user=self.request.user,
-            )
-        else:
-            self.adapter.object.save()
-
-        with translation.override(None):
-            log(
-                instance=self.adapter.object,
-                action="wagtail_fedit.move_block",
-                user=self.request.user,
-                data={
-                    "model_id": self.adapter.object.pk,
-                    "model_name": self.adapter.object._meta.model_name,
-                    "app_label": self.adapter.object._meta.app_label,
-                    "field_name": self.adapter.meta_field.verbose_name,
-                    "block_label": self.adapter.block.block.label,
-                    "block_id": self.adapter.kwargs["block_id"],
-                    "direction": action,
-                },
-                content_changed=True,
-            )
-
-        return JsonResponse({
-            "success": True,
-        })
 
+from .views import (
+    BlockMoveAdapterView,
+    BlockAddAdapterView,
+)
 
 
 class BlockAdapter(URLMixin, BlockFieldReplacementAdapter):
     """
     An adapter for editing Wagtail blocks.
     This will render the block and replace it on the frontend
     on successful form submission.
@@ -152,16 +72,20 @@
         ),
         Keyword("admin",
             absolute=True,
             help_text="if passed; the adapter will add a quick- link to the Wagtail Admin for this block."
         ),
         Keyword("movable",
             absolute=True,
-            help_text="if passed; the adapter will add move buttons to the toolbar."
-        )
+            help_text="if passed; the adapter will add 'move' buttons to the toolbar."
+        ),
+        Keyword("addable",
+            absolute=True,
+            help_text="if passed; the adapter will add an 'add' button to the toolbar."
+        ),
     )
 
     def __init__(self, object: models.Model, field_name: str, request: HttpRequest, **kwargs):
         super().__init__(object, field_name, request, **kwargs)
 
         self.block = self.kwargs.pop("block", None)
         self.parent = None
@@ -181,14 +105,17 @@
             self.streamfield: StreamValue = getattr(self.object, self.field_name)
             result = utils.find_block(block_id, self.streamfield)
             if not result:
                 raise AdapterError("Block not found; did you provide the correct block ID?")
             
             self.block, _, self.parent, self.block_index = result
 
+            if self.block_index == -1:
+                raise AdapterError("Block not found; did you provide the correct block ID?")
+
     @cached_property
     def tooltip(self) -> str:
         return self.get_header_title()
 
     def get_admin_url(self) -> str:
         finder = AdminURLFinder(self.request.user)
         url = finder.get_edit_url(self.object)
@@ -198,33 +125,39 @@
     @classmethod
     def get_admin_urls(self) -> list:
         return [
             path(
                 BaseAdapterView.prefix_url_path("block-move"),
                 BlockMoveAdapterView.as_view(),
                 name="block-move"
-            )
+            ),
+            path(
+                BaseAdapterView.prefix_url_path("block-add"),
+                BlockAddAdapterView.as_view(),
+                name="block-add"
+            ),
         ]
 
     def get_toolbar_buttons(self) -> list[FeditAdapterComponent]:
         buttons = super().get_toolbar_buttons()
 
         if self.kwargs["admin"]:
             buttons.append(FeditAdapterAdminLinkButton(
                 self.request, self,
             ))
 
-        if self.kwargs["movable"]:
-            buttons.append(MoveDownButton(
-                self.request, self,
-            ))
-
-            buttons.append(MoveUpButton(
-                self.request, self,
-            ))
+        buttons.append(AddableButton(
+            self.request, self,
+        ))
+        buttons.append(MoveDownButton(
+            self.request, self,
+        ))
+        buttons.append(MoveUpButton(
+            self.request, self,
+        ))
 
         return buttons
 
     def get_header_title(self):
 
         model_string = getattr(self.object, "get_admin_display_title", None)
         if model_string:
```

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/adapters/field.py` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/adapters/field.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/adapters/funcs.py` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/adapters/funcs.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/adapters/misc.py` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/adapters/misc.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/adapters/models.py` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/adapters/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/errors.py` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/errors.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/forms/blocks.py` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/forms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/forms/fields.py` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/forms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/hooks.py` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/locale/nl/LC_MESSAGES/django.po` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/models.py` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/registry.py` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/registry.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/settings.py` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,17 @@
     z-index: 300;
 }
 .wagtail-fedit-adapter-wrapper:not(.wagtail-fedit-block):has(.wagtail-fedit-adapter-wrapper) > .wagtail-fedit-buttons {
     right: 30px;
 }
 .wagtail-fedit-buttons {
     display: flex;
-    gap: 0.5em;
+    flex-wrap: wrap;
+    max-height: 100%;
+    gap: 0.15em;
     border-radius: 0.5em;
     position: absolute;
     right: 0;
     z-index: 1;
 }
 
 .wagtail-fedit-adapter-wrapper.wagtail-fedit-inline {
@@ -177,16 +179,16 @@
 @media (max-width: 768px) {
     .wagtail-fedit-modal-wrapper .wagtail-fedit-modal {
         margin: 0;
         max-width: 100%;
         max-height: 100%;
     }
 }
-.wagtail-fedit-modal-wrapper iframe,
-.wagtail-fedit-adapter-wrapper iframe {
+.wagtail-fedit-modal-wrapper #wagtail-fedit-iframe,
+.wagtail-fedit-adapter-wrapper #wagtail-fedit-iframe {
     width: 100%;
     height: 100%;
     border: none;
     z-index: 300;
     position: relative;
     flex: 1;
 }
@@ -205,14 +207,15 @@
     border-radius: 0 0 0 0.5em;
     border: 1px solid rgb(172, 27, 27);
     border-right-width: 0;
     border-top-width: 0;
     background-color: rgb(255, 255, 255);
     color: rgb(172, 27, 27);
     cursor: pointer;
+    z-index: 400;
 }
 .wagtail-fedit-modal-wrapper .wagtail-fedit-close-button:hover {
     background-color: rgb(172, 27, 27);
     color: rgb(235, 235, 235);
 }
 
 .wagtail-fedit-banner-modal {
```

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files 2% similar despite different names*

```diff
@@ -173,13 +173,17 @@
     height: 1.5rem;
     justify-content: center;
     margin: 0;
     outline-offset: -3px;
     padding: 0;
     width: 1.5rem;
 }
+.c-sf-add-button .icon {
+    width: 1.25rem !important;
+    height: 1.25rem !important;
+}
 /* .content-wrapper.content-wrapper:has(.nice-padding > .fedit-full)  .buttons { */
     /* justify-content: flex-start; */
 /* } */
 /* .content-wrapper.content-wrapper .nice-padding:has(> .fedit-full) { */
     /* padding: 0; */
 /* } */
```

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/static/wagtail_fedit/js/edit.js` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/static/wagtail_fedit/js/edit.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -194,206 +194,211 @@
             a: t
         }), t
     }, n.d = (e, t) => {
         for (var i in t) n.o(t, i) && !n.o(e, i) && Object.defineProperty(e, i, {
             enumerable: !0,
             get: t[i]
         })
-    }, n.o = (e, t) => Object.prototype.hasOwnProperty.call(e, t), n.nc = void 0, (() => {
+    }, n.o = (e, t) => Object.prototype.hasOwnProperty.call(e, t), n.nc = void 0;
+    var i = {};
+    (() => {
         function e(e) {
             if (null == e) return window;
             if ("[object Window]" !== e.toString()) {
                 var t = e.ownerDocument;
                 return t && t.defaultView || window
             }
             return e
         }
 
         function t(t) {
             return t instanceof e(t).Element || t instanceof Element
         }
 
-        function i(t) {
+        function r(t) {
             return t instanceof e(t).HTMLElement || t instanceof HTMLElement
         }
 
-        function r(t) {
+        function o(t) {
             return "undefined" != typeof ShadowRoot && (t instanceof e(t).ShadowRoot || t instanceof ShadowRoot)
         }
-        var o = Math.max,
-            a = Math.min,
-            s = Math.round;
+        n.d(i, {
+            DU: () => Dt
+        });
+        var a = Math.max,
+            s = Math.min,
+            c = Math.round;
 
-        function c() {
+        function l() {
             var e = navigator.userAgentData;
             return null != e && e.brands && Array.isArray(e.brands) ? e.brands.map((function(e) {
                 return e.brand + "/" + e.version
             })).join(" ") : navigator.userAgent
         }
 
-        function l() {
-            return !/^((?!chrome|android).)*safari/i.test(c())
+        function d() {
+            return !/^((?!chrome|android).)*safari/i.test(l())
         }
 
-        function d(n, r, o) {
-            void 0 === r && (r = !1), void 0 === o && (o = !1);
+        function p(n, i, o) {
+            void 0 === i && (i = !1), void 0 === o && (o = !1);
             var a = n.getBoundingClientRect(),
-                c = 1,
-                d = 1;
-            r && i(n) && (c = n.offsetWidth > 0 && s(a.width) / n.offsetWidth || 1, d = n.offsetHeight > 0 && s(a.height) / n.offsetHeight || 1);
+                s = 1,
+                l = 1;
+            i && r(n) && (s = n.offsetWidth > 0 && c(a.width) / n.offsetWidth || 1, l = n.offsetHeight > 0 && c(a.height) / n.offsetHeight || 1);
             var p = (t(n) ? e(n) : window).visualViewport,
-                u = !l() && o,
-                f = (a.left + (u && p ? p.offsetLeft : 0)) / c,
-                h = (a.top + (u && p ? p.offsetTop : 0)) / d,
-                m = a.width / c,
-                v = a.height / d;
+                u = !d() && o,
+                f = (a.left + (u && p ? p.offsetLeft : 0)) / s,
+                h = (a.top + (u && p ? p.offsetTop : 0)) / l,
+                m = a.width / s,
+                v = a.height / l;
             return {
                 width: m,
                 height: v,
                 top: h,
                 right: f + m,
                 bottom: h + v,
                 left: f,
                 x: f,
                 y: h
             }
         }
 
-        function p(t) {
+        function u(t) {
             var n = e(t);
             return {
                 scrollLeft: n.pageXOffset,
                 scrollTop: n.pageYOffset
             }
         }
 
-        function u(e) {
+        function f(e) {
             return e ? (e.nodeName || "").toLowerCase() : null
         }
 
-        function f(e) {
+        function h(e) {
             return ((t(e) ? e.ownerDocument : e.document) || window.document).documentElement
         }
 
-        function h(e) {
-            return d(f(e)).left + p(e).scrollLeft
+        function m(e) {
+            return p(h(e)).left + u(e).scrollLeft
         }
 
-        function m(t) {
+        function v(t) {
             return e(t).getComputedStyle(t)
         }
 
-        function v(e) {
-            var t = m(e),
+        function g(e) {
+            var t = v(e),
                 n = t.overflow,
                 i = t.overflowX,
                 r = t.overflowY;
             return /auto|scroll|overlay|hidden/.test(n + r + i)
         }
 
-        function g(t, n, r) {
-            void 0 === r && (r = !1);
-            var o, a, c = i(n),
-                l = i(n) && function(e) {
+        function w(t, n, i) {
+            void 0 === i && (i = !1);
+            var o, a, s = r(n),
+                l = r(n) && function(e) {
                     var t = e.getBoundingClientRect(),
-                        n = s(t.width) / e.offsetWidth || 1,
-                        i = s(t.height) / e.offsetHeight || 1;
+                        n = c(t.width) / e.offsetWidth || 1,
+                        i = c(t.height) / e.offsetHeight || 1;
                     return 1 !== n || 1 !== i
                 }(n),
-                m = f(n),
-                g = d(t, l, r),
+                d = h(n),
+                v = p(t, l, i),
                 w = {
                     scrollLeft: 0,
                     scrollTop: 0
                 },
                 y = {
                     x: 0,
                     y: 0
                 };
-            return (c || !c && !r) && (("body" !== u(n) || v(m)) && (w = (o = n) !== e(o) && i(o) ? {
+            return (s || !s && !i) && (("body" !== f(n) || g(d)) && (w = (o = n) !== e(o) && r(o) ? {
                 scrollLeft: (a = o).scrollLeft,
                 scrollTop: a.scrollTop
-            } : p(o)), i(n) ? ((y = d(n, !0)).x += n.clientLeft, y.y += n.clientTop) : m && (y.x = h(m))), {
-                x: g.left + w.scrollLeft - y.x,
-                y: g.top + w.scrollTop - y.y,
-                width: g.width,
-                height: g.height
+            } : u(o)), r(n) ? ((y = p(n, !0)).x += n.clientLeft, y.y += n.clientTop) : d && (y.x = m(d))), {
+                x: v.left + w.scrollLeft - y.x,
+                y: v.top + w.scrollTop - y.y,
+                width: v.width,
+                height: v.height
             }
         }
 
-        function w(e) {
-            var t = d(e),
+        function y(e) {
+            var t = p(e),
                 n = e.offsetWidth,
                 i = e.offsetHeight;
             return Math.abs(t.width - n) <= 1 && (n = t.width), Math.abs(t.height - i) <= 1 && (i = t.height), {
                 x: e.offsetLeft,
                 y: e.offsetTop,
                 width: n,
                 height: i
             }
         }
 
-        function y(e) {
-            return "html" === u(e) ? e : e.assignedSlot || e.parentNode || (r(e) ? e.host : null) || f(e)
+        function b(e) {
+            return "html" === f(e) ? e : e.assignedSlot || e.parentNode || (o(e) ? e.host : null) || h(e)
         }
 
-        function b(e) {
-            return ["html", "body", "#document"].indexOf(u(e)) >= 0 ? e.ownerDocument.body : i(e) && v(e) ? e : b(y(e))
+        function E(e) {
+            return ["html", "body", "#document"].indexOf(f(e)) >= 0 ? e.ownerDocument.body : r(e) && g(e) ? e : E(b(e))
         }
 
-        function E(t, n) {
+        function x(t, n) {
             var i;
             void 0 === n && (n = []);
-            var r = b(t),
+            var r = E(t),
                 o = r === (null == (i = t.ownerDocument) ? void 0 : i.body),
                 a = e(r),
-                s = o ? [a].concat(a.visualViewport || [], v(r) ? r : []) : r,
+                s = o ? [a].concat(a.visualViewport || [], g(r) ? r : []) : r,
                 c = n.concat(s);
-            return o ? c : c.concat(E(y(s)))
+            return o ? c : c.concat(x(b(s)))
         }
 
-        function x(e) {
-            return ["table", "td", "th"].indexOf(u(e)) >= 0
+        function O(e) {
+            return ["table", "td", "th"].indexOf(f(e)) >= 0
         }
 
-        function O(e) {
-            return i(e) && "fixed" !== m(e).position ? e.offsetParent : null
+        function L(e) {
+            return r(e) && "fixed" !== v(e).position ? e.offsetParent : null
         }
 
-        function L(t) {
-            for (var n = e(t), o = O(t); o && x(o) && "static" === m(o).position;) o = O(o);
-            return o && ("html" === u(o) || "body" === u(o) && "static" === m(o).position) ? n : o || function(e) {
-                var t = /firefox/i.test(c());
-                if (/Trident/i.test(c()) && i(e) && "fixed" === m(e).position) return null;
-                var n = y(e);
-                for (r(n) && (n = n.host); i(n) && ["html", "body"].indexOf(u(n)) < 0;) {
-                    var o = m(n);
-                    if ("none" !== o.transform || "none" !== o.perspective || "paint" === o.contain || -1 !== ["transform", "perspective"].indexOf(o.willChange) || t && "filter" === o.willChange || t && o.filter && "none" !== o.filter) return n;
+        function T(t) {
+            for (var n = e(t), i = L(t); i && O(i) && "static" === v(i).position;) i = L(i);
+            return i && ("html" === f(i) || "body" === f(i) && "static" === v(i).position) ? n : i || function(e) {
+                var t = /firefox/i.test(l());
+                if (/Trident/i.test(l()) && r(e) && "fixed" === v(e).position) return null;
+                var n = b(e);
+                for (o(n) && (n = n.host); r(n) && ["html", "body"].indexOf(f(n)) < 0;) {
+                    var i = v(n);
+                    if ("none" !== i.transform || "none" !== i.perspective || "paint" === i.contain || -1 !== ["transform", "perspective"].indexOf(i.willChange) || t && "filter" === i.willChange || t && i.filter && "none" !== i.filter) return n;
                     n = n.parentNode
                 }
                 return null
             }(t) || n
         }
-        var T = "top",
-            A = "bottom",
-            S = "right",
-            C = "left",
-            D = "auto",
-            M = [T, A, S, C],
-            I = "start",
-            k = "end",
-            R = "viewport",
+        var A = "top",
+            S = "bottom",
+            C = "right",
+            D = "left",
+            M = "auto",
+            I = [A, S, C, D],
+            k = "start",
+            R = "end",
+            P = "viewport",
             j = "popper",
-            P = M.reduce((function(e, t) {
-                return e.concat([t + "-" + I, t + "-" + k])
+            H = I.reduce((function(e, t) {
+                return e.concat([t + "-" + k, t + "-" + R])
             }), []),
-            H = [].concat(M, [D]).reduce((function(e, t) {
-                return e.concat([t, t + "-" + I, t + "-" + k])
+            N = [].concat(I, [M]).reduce((function(e, t) {
+                return e.concat([t, t + "-" + k, t + "-" + R])
             }), []),
-            N = ["beforeRead", "read", "afterRead", "beforeMain", "main", "afterMain", "beforeWrite", "write", "afterWrite"];
+            F = ["beforeRead", "read", "afterRead", "beforeMain", "main", "afterMain", "beforeWrite", "write", "afterWrite"];
 
         function W(e) {
             var t = new Map,
                 n = new Set,
                 i = [];
 
             function r(e) {
@@ -412,15 +417,15 @@
         }
         var B = {
             placement: "bottom",
             modifiers: [],
             strategy: "absolute"
         };
 
-        function F() {
+        function _() {
             for (var e = arguments.length, t = new Array(e), n = 0; n < e; n++) t[n] = arguments[n];
             return !t.some((function(e) {
                 return !(e && "function" == typeof e.getBoundingClientRect)
             }))
         }
 
         function q(e) {
@@ -447,20 +452,20 @@
                     l = [],
                     d = !1,
                     p = {
                         state: c,
                         setOptions: function(i) {
                             var o = "function" == typeof i ? i(c.options) : i;
                             u(), c.options = Object.assign({}, a, c.options, o), c.scrollParents = {
-                                reference: t(e) ? E(e) : e.contextElement ? E(e.contextElement) : [],
-                                popper: E(n)
+                                reference: t(e) ? x(e) : e.contextElement ? x(e.contextElement) : [],
+                                popper: x(n)
                             };
                             var s, d, f = function(e) {
                                 var t = W(e);
-                                return N.reduce((function(e, n) {
+                                return F.reduce((function(e, n) {
                                     return e.concat(t.filter((function(e) {
                                         return e.phase === n
                                     })))
                                 }), [])
                             }((s = [].concat(r, c.options.modifiers), d = s.reduce((function(e, t) {
                                 var n = e[t.name];
                                 return e[t.name] = n ? Object.assign({}, n, t, {
@@ -489,18 +494,18 @@
                             })), p.update()
                         },
                         forceUpdate: function() {
                             if (!d) {
                                 var e = c.elements,
                                     t = e.reference,
                                     n = e.popper;
-                                if (F(t, n)) {
+                                if (_(t, n)) {
                                     c.rects = {
-                                        reference: g(t, L(n), "fixed" === c.options.strategy),
-                                        popper: w(n)
+                                        reference: w(t, T(n), "fixed" === c.options.strategy),
+                                        popper: y(n)
                                     }, c.reset = !1, c.placement = c.options.placement, c.orderedModifiers.forEach((function(e) {
                                         return c.modifiersData[e.name] = Object.assign({}, e.data)
                                     }));
                                     for (var i = 0; i < c.orderedModifiers.length; i++)
                                         if (!0 !== c.reset) {
                                             var r = c.orderedModifiers[i],
                                                 o = r.fn,
@@ -528,30 +533,30 @@
                                 }))
                             }))), s
                         }),
                         destroy: function() {
                             u(), d = !0
                         }
                     };
-                if (!F(e, n)) return p;
+                if (!_(e, n)) return p;
 
                 function u() {
                     l.forEach((function(e) {
                         return e()
                     })), l = []
                 }
                 return p.setOptions(i).then((function(e) {
                     !d && i.onFirstUpdate && i.onFirstUpdate(e)
                 })), p
             }
         }
-        var _ = {
+        var V = {
             passive: !0
         };
-        const V = {
+        const $ = {
             name: "eventListeners",
             enabled: !0,
             phase: "write",
             fn: function() {},
             effect: function(t) {
                 var n = t.state,
                     i = t.instance,
@@ -559,199 +564,199 @@
                     o = r.scroll,
                     a = void 0 === o || o,
                     s = r.resize,
                     c = void 0 === s || s,
                     l = e(n.elements.popper),
                     d = [].concat(n.scrollParents.reference, n.scrollParents.popper);
                 return a && d.forEach((function(e) {
-                        e.addEventListener("scroll", i.update, _)
-                    })), c && l.addEventListener("resize", i.update, _),
+                        e.addEventListener("scroll", i.update, V)
+                    })), c && l.addEventListener("resize", i.update, V),
                     function() {
                         a && d.forEach((function(e) {
-                            e.removeEventListener("scroll", i.update, _)
-                        })), c && l.removeEventListener("resize", i.update, _)
+                            e.removeEventListener("scroll", i.update, V)
+                        })), c && l.removeEventListener("resize", i.update, V)
                     }
             },
             data: {}
         };
 
-        function $(e) {
+        function U(e) {
             return e.split("-")[0]
         }
 
-        function U(e) {
+        function z(e) {
             return e.split("-")[1]
         }
 
-        function z(e) {
+        function X(e) {
             return ["top", "bottom"].indexOf(e) >= 0 ? "x" : "y"
         }
 
-        function X(e) {
+        function Y(e) {
             var t, n = e.reference,
                 i = e.element,
                 r = e.placement,
-                o = r ? $(r) : null,
-                a = r ? U(r) : null,
+                o = r ? U(r) : null,
+                a = r ? z(r) : null,
                 s = n.x + n.width / 2 - i.width / 2,
                 c = n.y + n.height / 2 - i.height / 2;
             switch (o) {
-                case T:
+                case A:
                     t = {
                         x: s,
                         y: n.y - i.height
                     };
                     break;
-                case A:
+                case S:
                     t = {
                         x: s,
                         y: n.y + n.height
                     };
                     break;
-                case S:
+                case C:
                     t = {
                         x: n.x + n.width,
                         y: c
                     };
                     break;
-                case C:
+                case D:
                     t = {
                         x: n.x - i.width,
                         y: c
                     };
                     break;
                 default:
                     t = {
                         x: n.x,
                         y: n.y
                     }
             }
-            var l = o ? z(o) : null;
+            var l = o ? X(o) : null;
             if (null != l) {
                 var d = "y" === l ? "height" : "width";
                 switch (a) {
-                    case I:
+                    case k:
                         t[l] = t[l] - (n[d] / 2 - i[d] / 2);
                         break;
-                    case k:
+                    case R:
                         t[l] = t[l] + (n[d] / 2 - i[d] / 2)
                 }
             }
             return t
         }
-        var Y = {
+        var J = {
             top: "auto",
             right: "auto",
             bottom: "auto",
             left: "auto"
         };
 
-        function J(t) {
+        function G(t) {
             var n, i = t.popper,
                 r = t.popperRect,
                 o = t.placement,
                 a = t.variation,
-                c = t.offsets,
+                s = t.offsets,
                 l = t.position,
                 d = t.gpuAcceleration,
                 p = t.adaptive,
                 u = t.roundOffsets,
-                h = t.isFixed,
-                v = c.x,
-                g = void 0 === v ? 0 : v,
-                w = c.y,
+                f = t.isFixed,
+                m = s.x,
+                g = void 0 === m ? 0 : m,
+                w = s.y,
                 y = void 0 === w ? 0 : w,
                 b = "function" == typeof u ? u({
                     x: g,
                     y
                 }) : {
                     x: g,
                     y
                 };
             g = b.x, y = b.y;
-            var E = c.hasOwnProperty("x"),
-                x = c.hasOwnProperty("y"),
-                O = C,
-                D = T,
+            var E = s.hasOwnProperty("x"),
+                x = s.hasOwnProperty("y"),
+                O = D,
+                L = A,
                 M = window;
             if (p) {
-                var I = L(i),
-                    R = "clientHeight",
-                    j = "clientWidth";
-                I === e(i) && "static" !== m(I = f(i)).position && "absolute" === l && (R = "scrollHeight", j = "scrollWidth"), (o === T || (o === C || o === S) && a === k) && (D = A, y -= (h && I === M && M.visualViewport ? M.visualViewport.height : I[R]) - r.height, y *= d ? 1 : -1), o !== C && (o !== T && o !== A || a !== k) || (O = S, g -= (h && I === M && M.visualViewport ? M.visualViewport.width : I[j]) - r.width, g *= d ? 1 : -1)
+                var I = T(i),
+                    k = "clientHeight",
+                    P = "clientWidth";
+                I === e(i) && "static" !== v(I = h(i)).position && "absolute" === l && (k = "scrollHeight", P = "scrollWidth"), (o === A || (o === D || o === C) && a === R) && (L = S, y -= (f && I === M && M.visualViewport ? M.visualViewport.height : I[k]) - r.height, y *= d ? 1 : -1), o !== D && (o !== A && o !== S || a !== R) || (O = C, g -= (f && I === M && M.visualViewport ? M.visualViewport.width : I[P]) - r.width, g *= d ? 1 : -1)
             }
-            var P, H = Object.assign({
+            var j, H = Object.assign({
                     position: l
-                }, p && Y),
+                }, p && J),
                 N = !0 === u ? function(e, t) {
                     var n = e.x,
                         i = e.y,
                         r = t.devicePixelRatio || 1;
                     return {
-                        x: s(n * r) / r || 0,
-                        y: s(i * r) / r || 0
+                        x: c(n * r) / r || 0,
+                        y: c(i * r) / r || 0
                     }
                 }({
                     x: g,
                     y
                 }, e(i)) : {
                     x: g,
                     y
                 };
-            return g = N.x, y = N.y, d ? Object.assign({}, H, ((P = {})[D] = x ? "0" : "", P[O] = E ? "0" : "", P.transform = (M.devicePixelRatio || 1) <= 1 ? "translate(" + g + "px, " + y + "px)" : "translate3d(" + g + "px, " + y + "px, 0)", P)) : Object.assign({}, H, ((n = {})[D] = x ? y + "px" : "", n[O] = E ? g + "px" : "", n.transform = "", n))
+            return g = N.x, y = N.y, d ? Object.assign({}, H, ((j = {})[L] = x ? "0" : "", j[O] = E ? "0" : "", j.transform = (M.devicePixelRatio || 1) <= 1 ? "translate(" + g + "px, " + y + "px)" : "translate3d(" + g + "px, " + y + "px, 0)", j)) : Object.assign({}, H, ((n = {})[L] = x ? y + "px" : "", n[O] = E ? g + "px" : "", n.transform = "", n))
         }
-        const G = {
+        const K = {
                 name: "computeStyles",
                 enabled: !0,
                 phase: "beforeWrite",
                 fn: function(e) {
                     var t = e.state,
                         n = e.options,
                         i = n.gpuAcceleration,
                         r = void 0 === i || i,
                         o = n.adaptive,
                         a = void 0 === o || o,
                         s = n.roundOffsets,
                         c = void 0 === s || s,
                         l = {
-                            placement: $(t.placement),
-                            variation: U(t.placement),
+                            placement: U(t.placement),
+                            variation: z(t.placement),
                             popper: t.elements.popper,
                             popperRect: t.rects.popper,
                             gpuAcceleration: r,
                             isFixed: "fixed" === t.options.strategy
                         };
-                    null != t.modifiersData.popperOffsets && (t.styles.popper = Object.assign({}, t.styles.popper, J(Object.assign({}, l, {
+                    null != t.modifiersData.popperOffsets && (t.styles.popper = Object.assign({}, t.styles.popper, G(Object.assign({}, l, {
                         offsets: t.modifiersData.popperOffsets,
                         position: t.options.strategy,
                         adaptive: a,
                         roundOffsets: c
-                    })))), null != t.modifiersData.arrow && (t.styles.arrow = Object.assign({}, t.styles.arrow, J(Object.assign({}, l, {
+                    })))), null != t.modifiersData.arrow && (t.styles.arrow = Object.assign({}, t.styles.arrow, G(Object.assign({}, l, {
                         offsets: t.modifiersData.arrow,
                         position: "absolute",
                         adaptive: !1,
                         roundOffsets: c
                     })))), t.attributes.popper = Object.assign({}, t.attributes.popper, {
                         "data-popper-placement": t.placement
                     })
                 },
                 data: {}
             },
-            K = {
+            Q = {
                 name: "applyStyles",
                 enabled: !0,
                 phase: "write",
                 fn: function(e) {
                     var t = e.state;
                     Object.keys(t.elements).forEach((function(e) {
                         var n = t.styles[e] || {},
-                            r = t.attributes[e] || {},
+                            i = t.attributes[e] || {},
                             o = t.elements[e];
-                        i(o) && u(o) && (Object.assign(o.style, n), Object.keys(r).forEach((function(e) {
-                            var t = r[e];
+                        r(o) && f(o) && (Object.assign(o.style, n), Object.keys(i).forEach((function(e) {
+                            var t = i[e];
                             !1 === t ? o.removeAttribute(e) : o.setAttribute(e, !0 === t ? "" : t)
                         })))
                     }))
                 },
                 effect: function(e) {
                     var t = e.state,
                         n = {
@@ -765,656 +770,656 @@
                                 position: "absolute"
                             },
                             reference: {}
                         };
                     return Object.assign(t.elements.popper.style, n.popper), t.styles = n, t.elements.arrow && Object.assign(t.elements.arrow.style, n.arrow),
                         function() {
                             Object.keys(t.elements).forEach((function(e) {
-                                var r = t.elements[e],
+                                var i = t.elements[e],
                                     o = t.attributes[e] || {},
                                     a = Object.keys(t.styles.hasOwnProperty(e) ? t.styles[e] : n[e]).reduce((function(e, t) {
                                         return e[t] = "", e
                                     }), {});
-                                i(r) && u(r) && (Object.assign(r.style, a), Object.keys(o).forEach((function(e) {
-                                    r.removeAttribute(e)
+                                r(i) && f(i) && (Object.assign(i.style, a), Object.keys(o).forEach((function(e) {
+                                    i.removeAttribute(e)
                                 })))
                             }))
                         }
                 },
                 requires: ["computeStyles"]
             },
-            Q = {
+            Z = {
                 name: "offset",
                 enabled: !0,
                 phase: "main",
                 requires: ["popperOffsets"],
                 fn: function(e) {
                     var t = e.state,
                         n = e.options,
                         i = e.name,
                         r = n.offset,
                         o = void 0 === r ? [0, 0] : r,
-                        a = H.reduce((function(e, n) {
+                        a = N.reduce((function(e, n) {
                             return e[n] = function(e, t, n) {
-                                var i = $(e),
-                                    r = [C, T].indexOf(i) >= 0 ? -1 : 1,
+                                var i = U(e),
+                                    r = [D, A].indexOf(i) >= 0 ? -1 : 1,
                                     o = "function" == typeof n ? n(Object.assign({}, t, {
                                         placement: e
                                     })) : n,
                                     a = o[0],
                                     s = o[1];
-                                return a = a || 0, s = (s || 0) * r, [C, S].indexOf(i) >= 0 ? {
+                                return a = a || 0, s = (s || 0) * r, [D, C].indexOf(i) >= 0 ? {
                                     x: s,
                                     y: a
                                 } : {
                                     x: a,
                                     y: s
                                 }
                             }(n, t.rects, o), e
                         }), {}),
                         s = a[t.placement],
                         c = s.x,
                         l = s.y;
                     null != t.modifiersData.popperOffsets && (t.modifiersData.popperOffsets.x += c, t.modifiersData.popperOffsets.y += l), t.modifiersData[i] = a
                 }
             };
-        var Z = {
+        var ee = {
             left: "right",
             right: "left",
             bottom: "top",
             top: "bottom"
         };
 
-        function ee(e) {
+        function te(e) {
             return e.replace(/left|right|bottom|top/g, (function(e) {
-                return Z[e]
+                return ee[e]
             }))
         }
-        var te = {
+        var ne = {
             start: "end",
             end: "start"
         };
 
-        function ne(e) {
+        function ie(e) {
             return e.replace(/start|end/g, (function(e) {
-                return te[e]
+                return ne[e]
             }))
         }
 
-        function ie(e, t) {
+        function re(e, t) {
             var n = t.getRootNode && t.getRootNode();
             if (e.contains(t)) return !0;
-            if (n && r(n)) {
+            if (n && o(n)) {
                 var i = t;
                 do {
                     if (i && e.isSameNode(i)) return !0;
                     i = i.parentNode || i.host
                 } while (i)
             }
             return !1
         }
 
-        function re(e) {
+        function oe(e) {
             return Object.assign({}, e, {
                 left: e.x,
                 top: e.y,
                 right: e.x + e.width,
                 bottom: e.y + e.height
             })
         }
 
-        function oe(n, i, r) {
-            return i === R ? re(function(t, n) {
+        function ae(n, i, r) {
+            return i === P ? oe(function(t, n) {
                 var i = e(t),
-                    r = f(t),
+                    r = h(t),
                     o = i.visualViewport,
                     a = r.clientWidth,
                     s = r.clientHeight,
                     c = 0,
-                    d = 0;
+                    l = 0;
                 if (o) {
                     a = o.width, s = o.height;
-                    var p = l();
-                    (p || !p && "fixed" === n) && (c = o.offsetLeft, d = o.offsetTop)
+                    var p = d();
+                    (p || !p && "fixed" === n) && (c = o.offsetLeft, l = o.offsetTop)
                 }
                 return {
                     width: a,
                     height: s,
-                    x: c + h(t),
-                    y: d
+                    x: c + m(t),
+                    y: l
                 }
             }(n, r)) : t(i) ? function(e, t) {
-                var n = d(e, !1, "fixed" === t);
+                var n = p(e, !1, "fixed" === t);
                 return n.top = n.top + e.clientTop, n.left = n.left + e.clientLeft, n.bottom = n.top + e.clientHeight, n.right = n.left + e.clientWidth, n.width = e.clientWidth, n.height = e.clientHeight, n.x = n.left, n.y = n.top, n
-            }(i, r) : re(function(e) {
-                var t, n = f(e),
-                    i = p(e),
+            }(i, r) : oe(function(e) {
+                var t, n = h(e),
+                    i = u(e),
                     r = null == (t = e.ownerDocument) ? void 0 : t.body,
-                    a = o(n.scrollWidth, n.clientWidth, r ? r.scrollWidth : 0, r ? r.clientWidth : 0),
-                    s = o(n.scrollHeight, n.clientHeight, r ? r.scrollHeight : 0, r ? r.clientHeight : 0),
-                    c = -i.scrollLeft + h(e),
+                    o = a(n.scrollWidth, n.clientWidth, r ? r.scrollWidth : 0, r ? r.clientWidth : 0),
+                    s = a(n.scrollHeight, n.clientHeight, r ? r.scrollHeight : 0, r ? r.clientHeight : 0),
+                    c = -i.scrollLeft + m(e),
                     l = -i.scrollTop;
-                return "rtl" === m(r || n).direction && (c += o(n.clientWidth, r ? r.clientWidth : 0) - a), {
-                    width: a,
+                return "rtl" === v(r || n).direction && (c += a(n.clientWidth, r ? r.clientWidth : 0) - o), {
+                    width: o,
                     height: s,
                     x: c,
                     y: l
                 }
-            }(f(n)))
+            }(h(n)))
         }
 
-        function ae(e) {
+        function se(e) {
             return Object.assign({}, {
                 top: 0,
                 right: 0,
                 bottom: 0,
                 left: 0
             }, e)
         }
 
-        function se(e, t) {
+        function ce(e, t) {
             return t.reduce((function(t, n) {
                 return t[n] = e, t
             }), {})
         }
 
-        function ce(e, n) {
+        function le(e, n) {
             void 0 === n && (n = {});
-            var r = n,
-                s = r.placement,
-                c = void 0 === s ? e.placement : s,
-                l = r.strategy,
-                p = void 0 === l ? e.strategy : l,
-                h = r.boundary,
-                v = void 0 === h ? "clippingParents" : h,
-                g = r.rootBoundary,
-                w = void 0 === g ? R : g,
-                b = r.elementContext,
-                x = void 0 === b ? j : b,
-                O = r.altBoundary,
-                C = void 0 !== O && O,
-                D = r.padding,
-                I = void 0 === D ? 0 : D,
-                k = ae("number" != typeof I ? I : se(I, M)),
-                P = x === j ? "reference" : j,
+            var i = n,
+                o = i.placement,
+                c = void 0 === o ? e.placement : o,
+                l = i.strategy,
+                d = void 0 === l ? e.strategy : l,
+                u = i.boundary,
+                m = void 0 === u ? "clippingParents" : u,
+                g = i.rootBoundary,
+                w = void 0 === g ? P : g,
+                y = i.elementContext,
+                E = void 0 === y ? j : y,
+                O = i.altBoundary,
+                L = void 0 !== O && O,
+                D = i.padding,
+                M = void 0 === D ? 0 : D,
+                k = se("number" != typeof M ? M : ce(M, I)),
+                R = E === j ? "reference" : j,
                 H = e.rects.popper,
-                N = e.elements[C ? P : x],
-                W = function(e, n, r, s) {
+                N = e.elements[L ? R : E],
+                F = function(e, n, i, o) {
                     var c = "clippingParents" === n ? function(e) {
-                            var n = E(y(e)),
-                                r = ["absolute", "fixed"].indexOf(m(e).position) >= 0 && i(e) ? L(e) : e;
-                            return t(r) ? n.filter((function(e) {
-                                return t(e) && ie(e, r) && "body" !== u(e)
+                            var n = x(b(e)),
+                                i = ["absolute", "fixed"].indexOf(v(e).position) >= 0 && r(e) ? T(e) : e;
+                            return t(i) ? n.filter((function(e) {
+                                return t(e) && re(e, i) && "body" !== f(e)
                             })) : []
                         }(e) : [].concat(n),
-                        l = [].concat(c, [r]),
+                        l = [].concat(c, [i]),
                         d = l[0],
                         p = l.reduce((function(t, n) {
-                            var i = oe(e, n, s);
-                            return t.top = o(i.top, t.top), t.right = a(i.right, t.right), t.bottom = a(i.bottom, t.bottom), t.left = o(i.left, t.left), t
-                        }), oe(e, d, s));
+                            var i = ae(e, n, o);
+                            return t.top = a(i.top, t.top), t.right = s(i.right, t.right), t.bottom = s(i.bottom, t.bottom), t.left = a(i.left, t.left), t
+                        }), ae(e, d, o));
                     return p.width = p.right - p.left, p.height = p.bottom - p.top, p.x = p.left, p.y = p.top, p
-                }(t(N) ? N : N.contextElement || f(e.elements.popper), v, w, p),
-                B = d(e.elements.reference),
-                F = X({
-                    reference: B,
+                }(t(N) ? N : N.contextElement || h(e.elements.popper), m, w, d),
+                W = p(e.elements.reference),
+                B = Y({
+                    reference: W,
                     element: H,
                     strategy: "absolute",
                     placement: c
                 }),
-                q = re(Object.assign({}, H, F)),
-                _ = x === j ? q : B,
+                _ = oe(Object.assign({}, H, B)),
+                q = E === j ? _ : W,
                 V = {
-                    top: W.top - _.top + k.top,
-                    bottom: _.bottom - W.bottom + k.bottom,
-                    left: W.left - _.left + k.left,
-                    right: _.right - W.right + k.right
+                    top: F.top - q.top + k.top,
+                    bottom: q.bottom - F.bottom + k.bottom,
+                    left: F.left - q.left + k.left,
+                    right: q.right - F.right + k.right
                 },
                 $ = e.modifiersData.offset;
-            if (x === j && $) {
+            if (E === j && $) {
                 var U = $[c];
                 Object.keys(V).forEach((function(e) {
-                    var t = [S, A].indexOf(e) >= 0 ? 1 : -1,
-                        n = [T, A].indexOf(e) >= 0 ? "y" : "x";
+                    var t = [C, S].indexOf(e) >= 0 ? 1 : -1,
+                        n = [A, S].indexOf(e) >= 0 ? "y" : "x";
                     V[e] += U[n] * t
                 }))
             }
             return V
         }
-        const le = {
+        const de = {
             name: "flip",
             enabled: !0,
             phase: "main",
             fn: function(e) {
                 var t = e.state,
                     n = e.options,
                     i = e.name;
                 if (!t.modifiersData[i]._skip) {
-                    for (var r = n.mainAxis, o = void 0 === r || r, a = n.altAxis, s = void 0 === a || a, c = n.fallbackPlacements, l = n.padding, d = n.boundary, p = n.rootBoundary, u = n.altBoundary, f = n.flipVariations, h = void 0 === f || f, m = n.allowedAutoPlacements, v = t.options.placement, g = $(v), w = c || (g !== v && h ? function(e) {
-                            if ($(e) === D) return [];
-                            var t = ee(e);
-                            return [ne(e), t, ne(t)]
-                        }(v) : [ee(v)]), y = [v].concat(w).reduce((function(e, n) {
-                            return e.concat($(n) === D ? function(e, t) {
+                    for (var r = n.mainAxis, o = void 0 === r || r, a = n.altAxis, s = void 0 === a || a, c = n.fallbackPlacements, l = n.padding, d = n.boundary, p = n.rootBoundary, u = n.altBoundary, f = n.flipVariations, h = void 0 === f || f, m = n.allowedAutoPlacements, v = t.options.placement, g = U(v), w = c || (g !== v && h ? function(e) {
+                            if (U(e) === M) return [];
+                            var t = te(e);
+                            return [ie(e), t, ie(t)]
+                        }(v) : [te(v)]), y = [v].concat(w).reduce((function(e, n) {
+                            return e.concat(U(n) === M ? function(e, t) {
                                 void 0 === t && (t = {});
                                 var n = t,
                                     i = n.placement,
                                     r = n.boundary,
                                     o = n.rootBoundary,
                                     a = n.padding,
                                     s = n.flipVariations,
                                     c = n.allowedAutoPlacements,
-                                    l = void 0 === c ? H : c,
-                                    d = U(i),
-                                    p = d ? s ? P : P.filter((function(e) {
-                                        return U(e) === d
-                                    })) : M,
+                                    l = void 0 === c ? N : c,
+                                    d = z(i),
+                                    p = d ? s ? H : H.filter((function(e) {
+                                        return z(e) === d
+                                    })) : I,
                                     u = p.filter((function(e) {
                                         return l.indexOf(e) >= 0
                                     }));
                                 0 === u.length && (u = p);
                                 var f = u.reduce((function(t, n) {
-                                    return t[n] = ce(e, {
+                                    return t[n] = le(e, {
                                         placement: n,
                                         boundary: r,
                                         rootBoundary: o,
                                         padding: a
-                                    })[$(n)], t
+                                    })[U(n)], t
                                 }), {});
                                 return Object.keys(f).sort((function(e, t) {
                                     return f[e] - f[t]
                                 }))
                             }(t, {
                                 placement: n,
                                 boundary: d,
                                 rootBoundary: p,
                                 padding: l,
                                 flipVariations: h,
                                 allowedAutoPlacements: m
                             }) : n)
-                        }), []), b = t.rects.reference, E = t.rects.popper, x = new Map, O = !0, L = y[0], k = 0; k < y.length; k++) {
-                        var R = y[k],
-                            j = $(R),
-                            N = U(R) === I,
-                            W = [T, A].indexOf(j) >= 0,
-                            B = W ? "width" : "height",
-                            F = ce(t, {
+                        }), []), b = t.rects.reference, E = t.rects.popper, x = new Map, O = !0, L = y[0], T = 0; T < y.length; T++) {
+                        var R = y[T],
+                            P = U(R),
+                            j = z(R) === k,
+                            F = [A, S].indexOf(P) >= 0,
+                            W = F ? "width" : "height",
+                            B = le(t, {
                                 placement: R,
                                 boundary: d,
                                 rootBoundary: p,
                                 altBoundary: u,
                                 padding: l
                             }),
-                            q = W ? N ? S : C : N ? A : T;
-                        b[B] > E[B] && (q = ee(q));
-                        var _ = ee(q),
+                            _ = F ? j ? C : D : j ? S : A;
+                        b[W] > E[W] && (_ = te(_));
+                        var q = te(_),
                             V = [];
-                        if (o && V.push(F[j] <= 0), s && V.push(F[q] <= 0, F[_] <= 0), V.every((function(e) {
+                        if (o && V.push(B[P] <= 0), s && V.push(B[_] <= 0, B[q] <= 0), V.every((function(e) {
                                 return e
                             }))) {
                             L = R, O = !1;
                             break
                         }
                         x.set(R, V)
                     }
                     if (O)
-                        for (var z = function(e) {
+                        for (var $ = function(e) {
                                 var t = y.find((function(t) {
                                     var n = x.get(t);
                                     if (n) return n.slice(0, e).every((function(e) {
                                         return e
                                     }))
                                 }));
                                 if (t) return L = t, "break"
-                            }, X = h ? 3 : 1; X > 0 && "break" !== z(X); X--);
+                            }, X = h ? 3 : 1; X > 0 && "break" !== $(X); X--);
                     t.placement !== L && (t.modifiersData[i]._skip = !0, t.placement = L, t.reset = !0)
                 }
             },
             requiresIfExists: ["offset"],
             data: {
                 _skip: !1
             }
         };
 
-        function de(e, t, n) {
-            return o(e, a(t, n))
+        function pe(e, t, n) {
+            return a(e, s(t, n))
         }
-        const pe = {
+        const ue = {
                 name: "preventOverflow",
                 enabled: !0,
                 phase: "main",
                 fn: function(e) {
                     var t = e.state,
                         n = e.options,
                         i = e.name,
                         r = n.mainAxis,
-                        s = void 0 === r || r,
+                        o = void 0 === r || r,
                         c = n.altAxis,
                         l = void 0 !== c && c,
                         d = n.boundary,
                         p = n.rootBoundary,
                         u = n.altBoundary,
                         f = n.padding,
                         h = n.tether,
                         m = void 0 === h || h,
                         v = n.tetherOffset,
                         g = void 0 === v ? 0 : v,
-                        y = ce(t, {
+                        w = le(t, {
                             boundary: d,
                             rootBoundary: p,
                             padding: f,
                             altBoundary: u
                         }),
-                        b = $(t.placement),
-                        E = U(t.placement),
+                        b = U(t.placement),
+                        E = z(t.placement),
                         x = !E,
-                        O = z(b),
-                        D = "x" === O ? "y" : "x",
+                        O = X(b),
+                        L = "x" === O ? "y" : "x",
                         M = t.modifiersData.popperOffsets,
-                        k = t.rects.reference,
+                        I = t.rects.reference,
                         R = t.rects.popper,
-                        j = "function" == typeof g ? g(Object.assign({}, t.rects, {
+                        P = "function" == typeof g ? g(Object.assign({}, t.rects, {
                             placement: t.placement
                         })) : g,
-                        P = "number" == typeof j ? {
-                            mainAxis: j,
-                            altAxis: j
+                        j = "number" == typeof P ? {
+                            mainAxis: P,
+                            altAxis: P
                         } : Object.assign({
                             mainAxis: 0,
                             altAxis: 0
-                        }, j),
+                        }, P),
                         H = t.modifiersData.offset ? t.modifiersData.offset[t.placement] : null,
                         N = {
                             x: 0,
                             y: 0
                         };
                     if (M) {
-                        if (s) {
-                            var W, B = "y" === O ? T : C,
-                                F = "y" === O ? A : S,
-                                q = "y" === O ? "height" : "width",
-                                _ = M[O],
-                                V = _ + y[B],
-                                X = _ - y[F],
-                                Y = m ? -R[q] / 2 : 0,
-                                J = E === I ? k[q] : R[q],
-                                G = E === I ? -R[q] : -k[q],
+                        if (o) {
+                            var F, W = "y" === O ? A : D,
+                                B = "y" === O ? S : C,
+                                _ = "y" === O ? "height" : "width",
+                                q = M[O],
+                                V = q + w[W],
+                                $ = q - w[B],
+                                Y = m ? -R[_] / 2 : 0,
+                                J = E === k ? I[_] : R[_],
+                                G = E === k ? -R[_] : -I[_],
                                 K = t.elements.arrow,
-                                Q = m && K ? w(K) : {
+                                Q = m && K ? y(K) : {
                                     width: 0,
                                     height: 0
                                 },
                                 Z = t.modifiersData["arrow#persistent"] ? t.modifiersData["arrow#persistent"].padding : {
                                     top: 0,
                                     right: 0,
                                     bottom: 0,
                                     left: 0
                                 },
-                                ee = Z[B],
-                                te = Z[F],
-                                ne = de(0, k[q], Q[q]),
-                                ie = x ? k[q] / 2 - Y - ne - ee - P.mainAxis : J - ne - ee - P.mainAxis,
-                                re = x ? -k[q] / 2 + Y + ne + te + P.mainAxis : G + ne + te + P.mainAxis,
-                                oe = t.elements.arrow && L(t.elements.arrow),
+                                ee = Z[W],
+                                te = Z[B],
+                                ne = pe(0, I[_], Q[_]),
+                                ie = x ? I[_] / 2 - Y - ne - ee - j.mainAxis : J - ne - ee - j.mainAxis,
+                                re = x ? -I[_] / 2 + Y + ne + te + j.mainAxis : G + ne + te + j.mainAxis,
+                                oe = t.elements.arrow && T(t.elements.arrow),
                                 ae = oe ? "y" === O ? oe.clientTop || 0 : oe.clientLeft || 0 : 0,
-                                se = null != (W = null == H ? void 0 : H[O]) ? W : 0,
-                                le = _ + re - se,
-                                pe = de(m ? a(V, _ + ie - se - ae) : V, _, m ? o(X, le) : X);
-                            M[O] = pe, N[O] = pe - _
+                                se = null != (F = null == H ? void 0 : H[O]) ? F : 0,
+                                ce = q + re - se,
+                                de = pe(m ? s(V, q + ie - se - ae) : V, q, m ? a($, ce) : $);
+                            M[O] = de, N[O] = de - q
                         }
                         if (l) {
-                            var ue, fe = "x" === O ? T : C,
-                                he = "x" === O ? A : S,
-                                me = M[D],
-                                ve = "y" === D ? "height" : "width",
-                                ge = me + y[fe],
-                                we = me - y[he],
-                                ye = -1 !== [T, C].indexOf(b),
-                                be = null != (ue = null == H ? void 0 : H[D]) ? ue : 0,
-                                Ee = ye ? ge : me - k[ve] - R[ve] - be + P.altAxis,
-                                xe = ye ? me + k[ve] + R[ve] - be - P.altAxis : we,
+                            var ue, fe = "x" === O ? A : D,
+                                he = "x" === O ? S : C,
+                                me = M[L],
+                                ve = "y" === L ? "height" : "width",
+                                ge = me + w[fe],
+                                we = me - w[he],
+                                ye = -1 !== [A, D].indexOf(b),
+                                be = null != (ue = null == H ? void 0 : H[L]) ? ue : 0,
+                                Ee = ye ? ge : me - I[ve] - R[ve] - be + j.altAxis,
+                                xe = ye ? me + I[ve] + R[ve] - be - j.altAxis : we,
                                 Oe = m && ye ? function(e, t, n) {
-                                    var i = de(e, t, n);
+                                    var i = pe(e, t, n);
                                     return i > n ? n : i
-                                }(Ee, me, xe) : de(m ? Ee : ge, me, m ? xe : we);
-                            M[D] = Oe, N[D] = Oe - me
+                                }(Ee, me, xe) : pe(m ? Ee : ge, me, m ? xe : we);
+                            M[L] = Oe, N[L] = Oe - me
                         }
                         t.modifiersData[i] = N
                     }
                 },
                 requiresIfExists: ["offset"]
             },
-            ue = {
+            fe = {
                 name: "arrow",
                 enabled: !0,
                 phase: "main",
                 fn: function(e) {
                     var t, n = e.state,
                         i = e.name,
                         r = e.options,
                         o = n.elements.arrow,
                         a = n.modifiersData.popperOffsets,
-                        s = $(n.placement),
-                        c = z(s),
-                        l = [C, S].indexOf(s) >= 0 ? "height" : "width";
+                        s = U(n.placement),
+                        c = X(s),
+                        l = [D, C].indexOf(s) >= 0 ? "height" : "width";
                     if (o && a) {
                         var d = function(e, t) {
-                                return ae("number" != typeof(e = "function" == typeof e ? e(Object.assign({}, t.rects, {
+                                return se("number" != typeof(e = "function" == typeof e ? e(Object.assign({}, t.rects, {
                                     placement: t.placement
-                                })) : e) ? e : se(e, M))
+                                })) : e) ? e : ce(e, I))
                             }(r.padding, n),
-                            p = w(o),
-                            u = "y" === c ? T : C,
-                            f = "y" === c ? A : S,
+                            p = y(o),
+                            u = "y" === c ? A : D,
+                            f = "y" === c ? S : C,
                             h = n.rects.reference[l] + n.rects.reference[c] - a[c] - n.rects.popper[l],
                             m = a[c] - n.rects.reference[c],
-                            v = L(o),
+                            v = T(o),
                             g = v ? "y" === c ? v.clientHeight || 0 : v.clientWidth || 0 : 0,
-                            y = h / 2 - m / 2,
+                            w = h / 2 - m / 2,
                             b = d[u],
                             E = g - p[l] - d[f],
-                            x = g / 2 - p[l] / 2 + y,
-                            O = de(b, x, E),
-                            D = c;
-                        n.modifiersData[i] = ((t = {})[D] = O, t.centerOffset = O - x, t)
+                            x = g / 2 - p[l] / 2 + w,
+                            O = pe(b, x, E),
+                            L = c;
+                        n.modifiersData[i] = ((t = {})[L] = O, t.centerOffset = O - x, t)
                     }
                 },
                 effect: function(e) {
                     var t = e.state,
                         n = e.options.element,
                         i = void 0 === n ? "[data-popper-arrow]" : n;
-                    null != i && ("string" != typeof i || (i = t.elements.popper.querySelector(i))) && ie(t.elements.popper, i) && (t.elements.arrow = i)
+                    null != i && ("string" != typeof i || (i = t.elements.popper.querySelector(i))) && re(t.elements.popper, i) && (t.elements.arrow = i)
                 },
                 requires: ["popperOffsets"],
                 requiresIfExists: ["preventOverflow"]
             };
 
-        function fe(e, t, n) {
+        function he(e, t, n) {
             return void 0 === n && (n = {
                 x: 0,
                 y: 0
             }), {
                 top: e.top - t.height - n.y,
                 right: e.right - t.width + n.x,
                 bottom: e.bottom - t.height + n.y,
                 left: e.left - t.width - n.x
             }
         }
 
-        function he(e) {
-            return [T, S, A, C].some((function(t) {
+        function me(e) {
+            return [A, C, S, D].some((function(t) {
                 return e[t] >= 0
             }))
         }
-        var me = q({
-                defaultModifiers: [V, {
+        var ve = q({
+                defaultModifiers: [$, {
                     name: "popperOffsets",
                     enabled: !0,
                     phase: "read",
                     fn: function(e) {
                         var t = e.state,
                             n = e.name;
-                        t.modifiersData[n] = X({
+                        t.modifiersData[n] = Y({
                             reference: t.rects.reference,
                             element: t.rects.popper,
                             strategy: "absolute",
                             placement: t.placement
                         })
                     },
                     data: {}
-                }, G, K, Q, le, pe, ue, {
+                }, K, Q, Z, de, ue, fe, {
                     name: "hide",
                     enabled: !0,
                     phase: "main",
                     requiresIfExists: ["preventOverflow"],
                     fn: function(e) {
                         var t = e.state,
                             n = e.name,
                             i = t.rects.reference,
                             r = t.rects.popper,
                             o = t.modifiersData.preventOverflow,
-                            a = ce(t, {
+                            a = le(t, {
                                 elementContext: "reference"
                             }),
-                            s = ce(t, {
+                            s = le(t, {
                                 altBoundary: !0
                             }),
-                            c = fe(a, i),
-                            l = fe(s, r, o),
-                            d = he(c),
-                            p = he(l);
+                            c = he(a, i),
+                            l = he(s, r, o),
+                            d = me(c),
+                            p = me(l);
                         t.modifiersData[n] = {
                             referenceClippingOffsets: c,
                             popperEscapeOffsets: l,
                             isReferenceHidden: d,
                             hasPopperEscaped: p
                         }, t.attributes.popper = Object.assign({}, t.attributes.popper, {
                             "data-popper-reference-hidden": d,
                             "data-popper-escaped": p
                         })
                     }
                 }]
             }),
-            ve = "tippy-content",
-            ge = "tippy-backdrop",
-            we = "tippy-arrow",
-            ye = "tippy-svg-arrow",
-            be = {
+            ge = "tippy-content",
+            we = "tippy-backdrop",
+            ye = "tippy-arrow",
+            be = "tippy-svg-arrow",
+            Ee = {
                 passive: !0,
                 capture: !0
             },
-            Ee = function() {
+            xe = function() {
                 return document.body
             };
 
-        function xe(e, t, n) {
+        function Oe(e, t, n) {
             if (Array.isArray(e)) {
                 var i = e[t];
                 return null == i ? Array.isArray(n) ? n[t] : n : i
             }
             return e
         }
 
-        function Oe(e, t) {
+        function Le(e, t) {
             var n = {}.toString.call(e);
             return 0 === n.indexOf("[object") && n.indexOf(t + "]") > -1
         }
 
-        function Le(e, t) {
+        function Te(e, t) {
             return "function" == typeof e ? e.apply(void 0, t) : e
         }
 
-        function Te(e, t) {
+        function Ae(e, t) {
             return 0 === t ? e : function(i) {
                 clearTimeout(n), n = setTimeout((function() {
                     e(i)
                 }), t)
             };
             var n
         }
 
-        function Ae(e) {
+        function Se(e) {
             return [].concat(e)
         }
 
-        function Se(e, t) {
+        function Ce(e, t) {
             -1 === e.indexOf(t) && e.push(t)
         }
 
-        function Ce(e) {
+        function De(e) {
             return [].slice.call(e)
         }
 
-        function De(e) {
+        function Me(e) {
             return Object.keys(e).reduce((function(t, n) {
                 return void 0 !== e[n] && (t[n] = e[n]), t
             }), {})
         }
 
-        function Me() {
+        function Ie() {
             return document.createElement("div")
         }
 
-        function Ie(e) {
+        function ke(e) {
             return ["Element", "Fragment"].some((function(t) {
-                return Oe(e, t)
+                return Le(e, t)
             }))
         }
 
-        function ke(e, t) {
+        function Re(e, t) {
             e.forEach((function(e) {
                 e && (e.style.transitionDuration = t + "ms")
             }))
         }
 
-        function Re(e, t) {
+        function Pe(e, t) {
             e.forEach((function(e) {
                 e && e.setAttribute("data-state", t)
             }))
         }
 
         function je(e, t, n) {
             var i = t + "EventListener";
             ["transitionend", "webkitTransitionEnd"].forEach((function(t) {
                 e[i](t, n)
             }))
         }
 
-        function Pe(e, t) {
+        function He(e, t) {
             for (var n = t; n;) {
                 var i;
                 if (e.contains(n)) return !0;
                 n = null == n.getRootNode || null == (i = n.getRootNode()) ? void 0 : i.host
             }
             return !1
         }
-        var He = {
+        var Ne = {
                 isTouch: !1
             },
-            Ne = 0;
+            Fe = 0;
 
         function We() {
-            He.isTouch || (He.isTouch = !0, window.performance && document.addEventListener("mousemove", Be))
+            Ne.isTouch || (Ne.isTouch = !0, window.performance && document.addEventListener("mousemove", Be))
         }
 
         function Be() {
             var e = performance.now();
-            e - Ne < 20 && (He.isTouch = !1, document.removeEventListener("mousemove", Be)), Ne = e
+            e - Fe < 20 && (Ne.isTouch = !1, document.removeEventListener("mousemove", Be)), Fe = e
         }
 
-        function Fe() {
+        function _e() {
             var e, t = document.activeElement;
             if ((e = t) && e._tippy && e._tippy.reference === e) {
                 var n = t._tippy;
                 t.blur && !n.state.isVisible && t.blur()
             }
         }
         var qe = !("undefined" == typeof window || "undefined" == typeof document || !window.msCrypto),
-            _e = Object.assign({
-                appendTo: Ee,
+            Ve = Object.assign({
+                appendTo: xe,
                 aria: {
                     content: "auto",
                     expanded: "auto"
                 },
                 delay: 0,
                 duration: [300, 250],
                 getReferenceClientRect: null,
@@ -1457,121 +1462,121 @@
                 content: "",
                 inertia: !1,
                 maxWidth: 350,
                 role: "tooltip",
                 theme: "",
                 zIndex: 9999
             }),
-            Ve = Object.keys(_e);
+            $e = Object.keys(Ve);
 
-        function $e(e) {
+        function Ue(e) {
             var t = (e.plugins || []).reduce((function(t, n) {
                 var i, r = n.name,
                     o = n.defaultValue;
-                return r && (t[r] = void 0 !== e[r] ? e[r] : null != (i = _e[r]) ? i : o), t
+                return r && (t[r] = void 0 !== e[r] ? e[r] : null != (i = Ve[r]) ? i : o), t
             }), {});
             return Object.assign({}, e, t)
         }
 
-        function Ue(e, t) {
+        function ze(e, t) {
             var n = Object.assign({}, t, {
-                content: Le(t.content, [e])
+                content: Te(t.content, [e])
             }, t.ignoreAttributes ? {} : function(e, t) {
-                return (t ? Object.keys($e(Object.assign({}, _e, {
+                return (t ? Object.keys(Ue(Object.assign({}, Ve, {
                     plugins: t
-                }))) : Ve).reduce((function(t, n) {
+                }))) : $e).reduce((function(t, n) {
                     var i = (e.getAttribute("data-tippy-" + n) || "").trim();
                     if (!i) return t;
                     if ("content" === n) t[n] = i;
                     else try {
                         t[n] = JSON.parse(i)
                     } catch (e) {
                         t[n] = i
                     }
                     return t
                 }), {})
             }(e, t.plugins));
-            return n.aria = Object.assign({}, _e.aria, n.aria), n.aria = {
+            return n.aria = Object.assign({}, Ve.aria, n.aria), n.aria = {
                 expanded: "auto" === n.aria.expanded ? t.interactive : n.aria.expanded,
                 content: "auto" === n.aria.content ? t.interactive ? null : "describedby" : n.aria.content
             }, n
         }
-        var ze = function() {
+        var Xe = function() {
             return "innerHTML"
         };
 
-        function Xe(e, t) {
-            e[ze()] = t
+        function Ye(e, t) {
+            e[Xe()] = t
         }
 
-        function Ye(e) {
-            var t = Me();
-            return !0 === e ? t.className = we : (t.className = ye, Ie(e) ? t.appendChild(e) : Xe(t, e)), t
+        function Je(e) {
+            var t = Ie();
+            return !0 === e ? t.className = ye : (t.className = be, ke(e) ? t.appendChild(e) : Ye(t, e)), t
         }
 
-        function Je(e, t) {
-            Ie(t.content) ? (Xe(e, ""), e.appendChild(t.content)) : "function" != typeof t.content && (t.allowHTML ? Xe(e, t.content) : e.textContent = t.content)
+        function Ge(e, t) {
+            ke(t.content) ? (Ye(e, ""), e.appendChild(t.content)) : "function" != typeof t.content && (t.allowHTML ? Ye(e, t.content) : e.textContent = t.content)
         }
 
-        function Ge(e) {
+        function Ke(e) {
             var t = e.firstElementChild,
-                n = Ce(t.children);
+                n = De(t.children);
             return {
                 box: t,
                 content: n.find((function(e) {
-                    return e.classList.contains(ve)
+                    return e.classList.contains(ge)
                 })),
                 arrow: n.find((function(e) {
-                    return e.classList.contains(we) || e.classList.contains(ye)
+                    return e.classList.contains(ye) || e.classList.contains(be)
                 })),
                 backdrop: n.find((function(e) {
-                    return e.classList.contains(ge)
+                    return e.classList.contains(we)
                 }))
             }
         }
 
-        function Ke(e) {
-            var t = Me(),
-                n = Me();
+        function Qe(e) {
+            var t = Ie(),
+                n = Ie();
             n.className = "tippy-box", n.setAttribute("data-state", "hidden"), n.setAttribute("tabindex", "-1");
-            var i = Me();
+            var i = Ie();
 
             function r(n, i) {
-                var r = Ge(t),
+                var r = Ke(t),
                     o = r.box,
                     a = r.content,
                     s = r.arrow;
-                i.theme ? o.setAttribute("data-theme", i.theme) : o.removeAttribute("data-theme"), "string" == typeof i.animation ? o.setAttribute("data-animation", i.animation) : o.removeAttribute("data-animation"), i.inertia ? o.setAttribute("data-inertia", "") : o.removeAttribute("data-inertia"), o.style.maxWidth = "number" == typeof i.maxWidth ? i.maxWidth + "px" : i.maxWidth, i.role ? o.setAttribute("role", i.role) : o.removeAttribute("role"), n.content === i.content && n.allowHTML === i.allowHTML || Je(a, e.props), i.arrow ? s ? n.arrow !== i.arrow && (o.removeChild(s), o.appendChild(Ye(i.arrow))) : o.appendChild(Ye(i.arrow)) : s && o.removeChild(s)
+                i.theme ? o.setAttribute("data-theme", i.theme) : o.removeAttribute("data-theme"), "string" == typeof i.animation ? o.setAttribute("data-animation", i.animation) : o.removeAttribute("data-animation"), i.inertia ? o.setAttribute("data-inertia", "") : o.removeAttribute("data-inertia"), o.style.maxWidth = "number" == typeof i.maxWidth ? i.maxWidth + "px" : i.maxWidth, i.role ? o.setAttribute("role", i.role) : o.removeAttribute("role"), n.content === i.content && n.allowHTML === i.allowHTML || Ge(a, e.props), i.arrow ? s ? n.arrow !== i.arrow && (o.removeChild(s), o.appendChild(Je(i.arrow))) : o.appendChild(Je(i.arrow)) : s && o.removeChild(s)
             }
-            return i.className = ve, i.setAttribute("data-state", "hidden"), Je(i, e.props), t.appendChild(n), n.appendChild(i), r(e.props, e.props), {
+            return i.className = ge, i.setAttribute("data-state", "hidden"), Ge(i, e.props), t.appendChild(n), n.appendChild(i), r(e.props, e.props), {
                 popper: t,
                 onUpdate: r
             }
         }
-        Ke.$$tippy = !0;
-        var Qe = 1,
-            Ze = [],
-            et = [];
+        Qe.$$tippy = !0;
+        var Ze = 1,
+            et = [],
+            tt = [];
 
-        function tt(e, t) {
-            var n, i, r, o, a, s, c, l, d = Ue(e, Object.assign({}, _e, $e(De(t)))),
+        function nt(e, t) {
+            var n, i, r, o, a, s, c, l, d = ze(e, Object.assign({}, Ve, Ue(Me(t)))),
                 p = !1,
                 u = !1,
                 f = !1,
                 h = !1,
                 m = [],
-                v = Te(X, d.interactiveDebounce),
-                g = Qe++,
+                v = Ae(X, d.interactiveDebounce),
+                g = Ze++,
                 w = (l = d.plugins).filter((function(e, t) {
                     return l.indexOf(e) === t
                 })),
                 y = {
                     id: g,
                     reference: e,
-                    popper: Me(),
+                    popper: Ie(),
                     popperInstance: null,
                     props: d,
                     state: {
                         isEnabled: !0,
                         isVisible: !1,
                         isDestroyed: !1,
                         isMounted: !1,
@@ -1581,91 +1586,91 @@
                     clearDelayTimeouts: function() {
                         clearTimeout(n), clearTimeout(i), cancelAnimationFrame(r)
                     },
                     setProps: function(t) {
                         if (!y.state.isDestroyed) {
                             R("onBeforeUpdate", [y, t]), U();
                             var n = y.props,
-                                i = Ue(e, Object.assign({}, n, De(t), {
+                                i = ze(e, Object.assign({}, n, Me(t), {
                                     ignoreAttributes: !0
                                 }));
-                            y.props = i, $(), n.interactiveDebounce !== i.interactiveDebounce && (H(), v = Te(X, i.interactiveDebounce)), n.triggerTarget && !i.triggerTarget ? Ae(n.triggerTarget).forEach((function(e) {
+                            y.props = i, $(), n.interactiveDebounce !== i.interactiveDebounce && (H(), v = Ae(X, i.interactiveDebounce)), n.triggerTarget && !i.triggerTarget ? Se(n.triggerTarget).forEach((function(e) {
                                 e.removeAttribute("aria-expanded")
-                            })) : i.triggerTarget && e.removeAttribute("aria-expanded"), P(), k(), x && x(n, i), y.popperInstance && (K(), Z().forEach((function(e) {
+                            })) : i.triggerTarget && e.removeAttribute("aria-expanded"), j(), k(), x && x(n, i), y.popperInstance && (K(), Z().forEach((function(e) {
                                 requestAnimationFrame(e._tippy.popperInstance.forceUpdate)
                             }))), R("onAfterUpdate", [y, t])
                         }
                     },
                     setContent: function(e) {
                         y.setProps({
                             content: e
                         })
                     },
                     show: function() {
                         var e = y.state.isVisible,
                             t = y.state.isDestroyed,
                             n = !y.state.isEnabled,
-                            i = He.isTouch && !y.props.touch,
-                            r = xe(y.props.duration, 0, _e.duration);
+                            i = Ne.isTouch && !y.props.touch,
+                            r = Oe(y.props.duration, 0, Ve.duration);
                         if (!(e || t || n || i || C().hasAttribute("disabled") || (R("onShow", [y], !1), !1 === y.props.onShow(y)))) {
-                            if (y.state.isVisible = !0, S() && (E.style.visibility = "visible"), k(), F(), y.state.isMounted || (E.style.transition = "none"), S()) {
+                            if (y.state.isVisible = !0, S() && (E.style.visibility = "visible"), k(), B(), y.state.isMounted || (E.style.transition = "none"), S()) {
                                 var o = M();
-                                ke([o.box, o.content], 0)
+                                Re([o.box, o.content], 0)
                             }
                             var a, c, l;
                             s = function() {
                                 var e;
                                 if (y.state.isVisible && !h) {
                                     if (h = !0, E.offsetHeight, E.style.transition = y.props.moveTransition, S() && y.props.animation) {
                                         var t = M(),
                                             n = t.box,
                                             i = t.content;
-                                        ke([n, i], r), Re([n, i], "visible")
+                                        Re([n, i], r), Pe([n, i], "visible")
                                     }
-                                    j(), P(), Se(et, y), null == (e = y.popperInstance) || e.forceUpdate(), R("onMount", [y]), y.props.animation && S() && function(e, t) {
-                                        _(e, (function() {
+                                    P(), j(), Ce(tt, y), null == (e = y.popperInstance) || e.forceUpdate(), R("onMount", [y]), y.props.animation && S() && function(e, t) {
+                                        q(e, (function() {
                                             y.state.isShown = !0, R("onShown", [y])
                                         }))
                                     }(r)
                                 }
-                            }, c = y.props.appendTo, l = C(), (a = y.props.interactive && c === Ee || "parent" === c ? l.parentNode : Le(c, [l])).contains(E) || a.appendChild(E), y.state.isMounted = !0, K()
+                            }, c = y.props.appendTo, l = C(), (a = y.props.interactive && c === xe || "parent" === c ? l.parentNode : Te(c, [l])).contains(E) || a.appendChild(E), y.state.isMounted = !0, K()
                         }
                     },
                     hide: function() {
                         var e = !y.state.isVisible,
                             t = y.state.isDestroyed,
                             n = !y.state.isEnabled,
-                            i = xe(y.props.duration, 1, _e.duration);
+                            i = Oe(y.props.duration, 1, Ve.duration);
                         if (!(e || t || n) && (R("onHide", [y], !1), !1 !== y.props.onHide(y))) {
-                            if (y.state.isVisible = !1, y.state.isShown = !1, h = !1, p = !1, S() && (E.style.visibility = "hidden"), H(), q(), k(!0), S()) {
+                            if (y.state.isVisible = !1, y.state.isShown = !1, h = !1, p = !1, S() && (E.style.visibility = "hidden"), H(), _(), k(!0), S()) {
                                 var r = M(),
                                     o = r.box,
                                     a = r.content;
-                                y.props.animation && (ke([o, a], i), Re([o, a], "hidden"))
+                                y.props.animation && (Re([o, a], i), Pe([o, a], "hidden"))
                             }
-                            j(), P(), y.props.animation ? S() && function(e, t) {
-                                _(e, (function() {
+                            P(), j(), y.props.animation ? S() && function(e, t) {
+                                q(e, (function() {
                                     !y.state.isVisible && E.parentNode && E.parentNode.contains(E) && t()
                                 }))
                             }(i, y.unmount) : y.unmount()
                         }
                     },
                     hideWithInteractivity: function(e) {
-                        D().addEventListener("mousemove", v), Se(Ze, v), v(e)
+                        D().addEventListener("mousemove", v), Ce(et, v), v(e)
                     },
                     enable: function() {
                         y.state.isEnabled = !0
                     },
                     disable: function() {
                         y.hide(), y.state.isEnabled = !1
                     },
                     unmount: function() {
                         y.state.isVisible && y.hide(), y.state.isMounted && (Q(), Z().forEach((function(e) {
                             e._tippy.unmount()
-                        })), E.parentNode && E.parentNode.removeChild(E), et = et.filter((function(e) {
+                        })), E.parentNode && E.parentNode.removeChild(E), tt = tt.filter((function(e) {
                             return e !== y
                         })), y.state.isMounted = !1, R("onHidden", [y]))
                     },
                     destroy: function() {
                         y.state.isDestroyed || (y.clearDelayTimeouts(), y.unmount(), U(), delete e._tippy, y.state.isDestroyed = !0, R("onDestroy", [y]))
                     }
                 };
@@ -1674,15 +1679,15 @@
                 E = b.popper,
                 x = b.onUpdate;
             E.setAttribute("data-tippy-root", ""), E.id = "tippy-" + y.id, y.popper = E, e._tippy = y, E._tippy = y;
             var O = w.map((function(e) {
                     return e.fn(y)
                 })),
                 L = e.hasAttribute("aria-expanded");
-            return $(), P(), k(), R("onCreate", [y]), d.showOnCreate && ee(), E.addEventListener("mouseenter", (function() {
+            return $(), j(), k(), R("onCreate", [y]), d.showOnCreate && ee(), E.addEventListener("mouseenter", (function() {
                 y.props.interactive && y.state.isVisible && y.clearDelayTimeouts()
             })), E.addEventListener("mouseleave", (function() {
                 y.props.interactive && y.props.trigger.indexOf("mouseenter") >= 0 && D().addEventListener("mousemove", v)
             })), y;
 
             function T() {
                 var e = y.props.touch;
@@ -1700,111 +1705,111 @@
 
             function C() {
                 return c || e
             }
 
             function D() {
                 var e, t, n = C().parentNode;
-                return n ? null != (t = Ae(n)[0]) && null != (e = t.ownerDocument) && e.body ? t.ownerDocument : document : document
+                return n ? null != (t = Se(n)[0]) && null != (e = t.ownerDocument) && e.body ? t.ownerDocument : document : document
             }
 
             function M() {
-                return Ge(E)
+                return Ke(E)
             }
 
             function I(e) {
-                return y.state.isMounted && !y.state.isVisible || He.isTouch || o && "focus" === o.type ? 0 : xe(y.props.delay, e ? 0 : 1, _e.delay)
+                return y.state.isMounted && !y.state.isVisible || Ne.isTouch || o && "focus" === o.type ? 0 : Oe(y.props.delay, e ? 0 : 1, Ve.delay)
             }
 
             function k(e) {
                 void 0 === e && (e = !1), E.style.pointerEvents = y.props.interactive && !e ? "" : "none", E.style.zIndex = "" + y.props.zIndex
             }
 
             function R(e, t, n) {
                 var i;
                 void 0 === n && (n = !0), O.forEach((function(n) {
                     n[e] && n[e].apply(n, t)
                 })), n && (i = y.props)[e].apply(i, t)
             }
 
-            function j() {
+            function P() {
                 var t = y.props.aria;
                 if (t.content) {
                     var n = "aria-" + t.content,
                         i = E.id;
-                    Ae(y.props.triggerTarget || e).forEach((function(e) {
+                    Se(y.props.triggerTarget || e).forEach((function(e) {
                         var t = e.getAttribute(n);
                         if (y.state.isVisible) e.setAttribute(n, t ? t + " " + i : i);
                         else {
                             var r = t && t.replace(i, "").trim();
                             r ? e.setAttribute(n, r) : e.removeAttribute(n)
                         }
                     }))
                 }
             }
 
-            function P() {
-                !L && y.props.aria.expanded && Ae(y.props.triggerTarget || e).forEach((function(e) {
+            function j() {
+                !L && y.props.aria.expanded && Se(y.props.triggerTarget || e).forEach((function(e) {
                     y.props.interactive ? e.setAttribute("aria-expanded", y.state.isVisible && e === C() ? "true" : "false") : e.removeAttribute("aria-expanded")
                 }))
             }
 
             function H() {
-                D().removeEventListener("mousemove", v), Ze = Ze.filter((function(e) {
+                D().removeEventListener("mousemove", v), et = et.filter((function(e) {
                     return e !== v
                 }))
             }
 
             function N(t) {
-                if (!He.isTouch || !f && "mousedown" !== t.type) {
+                if (!Ne.isTouch || !f && "mousedown" !== t.type) {
                     var n = t.composedPath && t.composedPath()[0] || t.target;
-                    if (!y.props.interactive || !Pe(E, n)) {
-                        if (Ae(y.props.triggerTarget || e).some((function(e) {
-                                return Pe(e, n)
+                    if (!y.props.interactive || !He(E, n)) {
+                        if (Se(y.props.triggerTarget || e).some((function(e) {
+                                return He(e, n)
                             }))) {
-                            if (He.isTouch) return;
+                            if (Ne.isTouch) return;
                             if (y.state.isVisible && y.props.trigger.indexOf("click") >= 0) return
                         } else R("onClickOutside", [y, t]);
                         !0 === y.props.hideOnClick && (y.clearDelayTimeouts(), y.hide(), u = !0, setTimeout((function() {
                             u = !1
-                        })), y.state.isMounted || q())
+                        })), y.state.isMounted || _())
                     }
                 }
             }
 
-            function W() {
+            function F() {
                 f = !0
             }
 
-            function B() {
+            function W() {
                 f = !1
             }
 
-            function F() {
+            function B() {
                 var e = D();
-                e.addEventListener("mousedown", N, !0), e.addEventListener("touchend", N, be), e.addEventListener("touchstart", B, be), e.addEventListener("touchmove", W, be)
+                e.addEventListener("mousedown", N, !0), e.addEventListener("touchend", N, Ee), e.addEventListener("touchstart", W, Ee), e.addEventListener("touchmove", F, Ee)
             }
 
-            function q() {
+            function _() {
                 var e = D();
-                e.removeEventListener("mousedown", N, !0), e.removeEventListener("touchend", N, be), e.removeEventListener("touchstart", B, be), e.removeEventListener("touchmove", W, be)
+                e.removeEventListener("mousedown", N, !0), e.removeEventListener("touchend", N, Ee), e.removeEventListener("touchstart", W, Ee), e.removeEventListener("touchmove", F, Ee)
             }
 
-            function _(e, t) {
+            function q(e, t) {
                 var n = M().box;
 
                 function i(e) {
                     e.target === n && (je(n, "remove", i), t())
                 }
                 if (0 === e) return t();
                 je(n, "remove", a), je(n, "add", i), a = i
             }
 
             function V(t, n, i) {
-                void 0 === i && (i = !1), Ae(y.props.triggerTarget || e).forEach((function(e) {
+                void 0 === i && (i = !1), Se(y.props.triggerTarget || e).forEach((function(e) {
                     e.addEventListener(t, n, i), m.push({
                         node: e,
                         eventType: t,
                         handler: n,
                         options: i
                     })
                 }))
@@ -1840,15 +1845,15 @@
                 })), m = []
             }
 
             function z(e) {
                 var t, n = !1;
                 if (y.state.isEnabled && !G(e) && !u) {
                     var i = "focus" === (null == (t = o) ? void 0 : t.type);
-                    o = e, c = e.currentTarget, P(), !y.state.isVisible && Oe(e, "MouseEvent") && Ze.forEach((function(t) {
+                    o = e, c = e.currentTarget, j(), !y.state.isVisible && Le(e, "MouseEvent") && et.forEach((function(t) {
                         return t(e)
                     })), "click" === e.type && (y.props.trigger.indexOf("mouseenter") < 0 || p) && !1 !== y.props.hideOnClick && y.state.isVisible ? n = !0 : ee(e), "click" === e.type && (p = !n), n && !i && te(e)
                 }
             }
 
             function X(e) {
                 var t = e.target,
@@ -1891,26 +1896,26 @@
             }
 
             function J(e) {
                 y.props.trigger.indexOf("focusin") < 0 && e.target !== C() || y.props.interactive && e.relatedTarget && E.contains(e.relatedTarget) || te(e)
             }
 
             function G(e) {
-                return !!He.isTouch && A() !== e.type.indexOf("touch") >= 0
+                return !!Ne.isTouch && A() !== e.type.indexOf("touch") >= 0
             }
 
             function K() {
                 Q();
                 var t = y.props,
                     n = t.popperOptions,
                     i = t.placement,
                     r = t.offset,
                     o = t.getReferenceClientRect,
                     a = t.moveTransition,
-                    c = S() ? Ge(E).arrow : null,
+                    c = S() ? Ke(E).arrow : null,
                     l = o ? {
                         getBoundingClientRect: o,
                         contextElement: o.contextElement || C()
                     } : e,
                     d = [{
                         name: "offset",
                         options: {
@@ -1953,74 +1958,74 @@
                     }];
                 S() && c && d.push({
                     name: "arrow",
                     options: {
                         element: c,
                         padding: 3
                     }
-                }), d.push.apply(d, (null == n ? void 0 : n.modifiers) || []), y.popperInstance = me(l, E, Object.assign({}, n, {
+                }), d.push.apply(d, (null == n ? void 0 : n.modifiers) || []), y.popperInstance = ve(l, E, Object.assign({}, n, {
                     placement: i,
                     onFirstUpdate: s,
                     modifiers: d
                 }))
             }
 
             function Q() {
                 y.popperInstance && (y.popperInstance.destroy(), y.popperInstance = null)
             }
 
             function Z() {
-                return Ce(E.querySelectorAll("[data-tippy-root]"))
+                return De(E.querySelectorAll("[data-tippy-root]"))
             }
 
             function ee(e) {
-                y.clearDelayTimeouts(), e && R("onTrigger", [y, e]), F();
+                y.clearDelayTimeouts(), e && R("onTrigger", [y, e]), B();
                 var t = I(!0),
                     i = T(),
                     r = i[0],
                     o = i[1];
-                He.isTouch && "hold" === r && o && (t = o), t ? n = setTimeout((function() {
+                Ne.isTouch && "hold" === r && o && (t = o), t ? n = setTimeout((function() {
                     y.show()
                 }), t) : y.show()
             }
 
             function te(e) {
                 if (y.clearDelayTimeouts(), R("onUntrigger", [y, e]), y.state.isVisible) {
                     if (!(y.props.trigger.indexOf("mouseenter") >= 0 && y.props.trigger.indexOf("click") >= 0 && ["mouseleave", "mousemove"].indexOf(e.type) >= 0 && p)) {
                         var t = I(!1);
                         t ? i = setTimeout((function() {
                             y.state.isVisible && y.hide()
                         }), t) : r = requestAnimationFrame((function() {
                             y.hide()
                         }))
                     }
-                } else q()
+                } else _()
             }
         }
 
-        function nt(e, t) {
+        function it(e, t) {
             void 0 === t && (t = {});
-            var n = _e.plugins.concat(t.plugins || []);
-            document.addEventListener("touchstart", We, be), window.addEventListener("blur", Fe);
+            var n = Ve.plugins.concat(t.plugins || []);
+            document.addEventListener("touchstart", We, Ee), window.addEventListener("blur", _e);
             var i, r = Object.assign({}, t, {
                     plugins: n
                 }),
-                o = (i = e, Ie(i) ? [i] : function(e) {
-                    return Oe(e, "NodeList")
-                }(i) ? Ce(i) : Array.isArray(i) ? i : Ce(document.querySelectorAll(i))).reduce((function(e, t) {
-                    var n = t && tt(t, r);
+                o = (i = e, ke(i) ? [i] : function(e) {
+                    return Le(e, "NodeList")
+                }(i) ? De(i) : Array.isArray(i) ? i : De(document.querySelectorAll(i))).reduce((function(e, t) {
+                    var n = t && nt(t, r);
                     return n && e.push(n), e
                 }), []);
-            return Ie(e) ? o[0] : o
+            return ke(e) ? o[0] : o
         }
-        nt.defaultProps = _e, nt.setDefaultProps = function(e) {
+        it.defaultProps = Ve, it.setDefaultProps = function(e) {
             Object.keys(e).forEach((function(t) {
-                _e[t] = e[t]
+                Ve[t] = e[t]
             }))
-        }, nt.currentInput = He, Object.assign({}, K, {
+        }, it.currentInput = Ne, Object.assign({}, Q, {
             effect: function(e) {
                 var t = e.state,
                     n = {
                         popper: {
                             position: t.options.strategy,
                             left: "0",
                             top: "0",
@@ -2029,90 +2034,90 @@
                         arrow: {
                             position: "absolute"
                         },
                         reference: {}
                     };
                 Object.assign(t.elements.popper.style, n.popper), t.styles = n, t.elements.arrow && Object.assign(t.elements.arrow.style, n.arrow)
             }
-        }), nt.setDefaultProps({
-            render: Ke
+        }), it.setDefaultProps({
+            render: Qe
         });
-        const it = nt;
-        var rt = n(72),
-            ot = n.n(rt),
-            at = n(825),
-            st = n.n(at),
-            ct = n(659),
-            lt = n.n(ct),
-            dt = n(56),
-            pt = n.n(dt),
-            ut = n(540),
-            ft = n.n(ut),
-            ht = n(113),
-            mt = n.n(ht),
-            vt = n(2),
-            gt = {};
-        gt.styleTagTransform = mt(), gt.setAttributes = pt(), gt.insert = lt().bind(null, "head"), gt.domAPI = st(), gt.insertStyleElement = ft(), ot()(vt.A, gt), vt.A && vt.A.locals && vt.A.locals;
-        class wt {
+        const rt = it;
+        var ot = n(72),
+            at = n.n(ot),
+            st = n(825),
+            ct = n.n(st),
+            lt = n(659),
+            dt = n.n(lt),
+            pt = n(56),
+            ut = n.n(pt),
+            ft = n(540),
+            ht = n.n(ft),
+            mt = n(113),
+            vt = n.n(mt),
+            gt = n(2),
+            wt = {};
+        wt.styleTagTransform = vt(), wt.setAttributes = ut(), wt.insert = dt().bind(null, "head"), wt.domAPI = ct(), wt.insertStyleElement = ht(), at()(gt.A, wt), gt.A && gt.A.locals && gt.A.locals;
+        class yt {
             constructor(e) {
                 this.element = e, this.tooltipConfig = this.makeConfig(), this.init()
             }
             init() {
-                it(this.element, this.tooltipConfig)
+                rt(this.element, this.tooltipConfig)
             }
             makeConfig() {
                 const e = {
                     content: this.element.getAttribute("title")
                 };
                 for (let t = 0; t < this.element.attributes.length; t++) {
                     const n = this.element.attributes[t];
                     n.name.startsWith("data-tooltip-") && (e[n.name.replace("data-tooltip-", "")] = n.value)
                 }
                 return this.tooltipConfig = e, e
             }
         }
 
-        function yt(e) {
+        function bt(e) {
             const t = e.dataset.feditConstructor;
             if (t) return window.wagtailFedit.editors[t];
             throw new Error("No editor class found for element")
         }
 
-        function bt(e = document) {
+        function Et(e = document) {
             let t;
             t = e instanceof HTMLElement && e.classList.contains("wagtail-fedit-adapter-wrapper") && !e.classList.contains("wagtail-fedit-initialized") ? [e] : e.querySelectorAll(".wagtail-fedit-adapter-wrapper");
             for (let n = 0; n < t.length; n++) {
                 const i = t[n];
                 if (!i.classList.contains("wagtail-fedit-initialized")) {
                     i.classList.add("wagtail-fedit-initialized");
-                    const e = yt(i);
+                    const e = bt(i);
                     e ? new e(i) : console.error("No editor class found for element", i)
                 }
                 const r = e.querySelectorAll("[data-tooltip='true']");
                 for (let e = 0; e < r.length; e++) {
                     const t = r[e];
-                    "true" == t.dataset.tooltip && (new wt(t), delete t.dataset.tooltip)
+                    "true" == t.dataset.tooltip && (new yt(t), delete t.dataset.tooltip)
                 }
             }
         }
 
-        function Et() {
+        function xt() {
             let e = window.location.href,
                 t = window.scrollY,
                 n = window.scrollX,
                 i = new URL(e);
             i.searchParams.set("scrollY", `${t}`), i.searchParams.set("scrollX", `${n}`), window.location.href = i.toString()
         }
 
-        function xt(e) {
+        function Ot(e) {
             if (!e) return;
             const t = new URL(e.href);
             window.scrollY > 100 && t.searchParams.set("scrollY", `${window.scrollY}`), window.scrollX > 100 && t.searchParams.set("scrollX", `${window.scrollX}`), e.href = t.toString()
         }
-        class Ot {
+        class Lt {
             constructor(e) {
                 this.editor = e
             }
             openEditor() {
                 this.editor.openEditor()
             }
             closeEditor() {
@@ -2152,18 +2157,18 @@
                                 if (r.substring(0, 10) === e + "=") {
                                     t = decodeURIComponent(r.substring(10));
                                     break
                                 }
                             }
                         }
                         return t
-                    }("csrftoken")), fetch(e, {
+                    }("csrftoken")), n instanceof FormData || (n = JSON.stringify(n)), fetch(e, {
                         method: t,
                         headers: i,
-                        body: JSON.stringify(n)
+                        body: n
                     }).then((e => e.json()))
                 }, new((o = void 0) || (o = Promise))((function(e, t) {
                     function n(e) {
                         try {
                             c(a.next(e))
                         } catch (e) {
                             t(e)
@@ -2191,30 +2196,30 @@
             refetch() {
                 return this.editor.refetch()
             }
             execRelated(e) {
                 for (const t of this.editor.relatedWrappers) e(t.editorAPI)
             }
         }
-        const Lt = "wagtail-fedit-modal",
-            Tt = `\n<div class="${Lt}-wrapper">\n    <div class="${Lt}" id="${Lt}-__ID__-modal">\n    </div>\n</div>`;
-        class At {
+        const Tt = "wagtail-fedit-modal",
+            At = `\n<div class="${Tt}-wrapper">\n    <div class="${Tt}" id="${Tt}-__ID__-modal">\n    </div>\n</div>`;
+        class St {
             constructor(e) {
-                this.options = e, this.modalHtml = Tt.replace("__ID__", this.options.modalId)
+                this.options = e, this.modalHtml = At.replace("__ID__", this.options.modalId)
             }
             static get modalWrapper() {
-                var e = document.querySelector(`#${Lt}-wrapper`);
-                return e || ((e = document.createElement("div")).id = `${Lt}-wrapper`, e.classList.add(`${Lt}-wrapper`), document.body.appendChild(e), e)
+                var e = document.querySelector(`#${Tt}-wrapper`);
+                return e || ((e = document.createElement("div")).id = `${Tt}-wrapper`, e.classList.add(`${Tt}-wrapper`), document.body.appendChild(e), e)
             }
             get wrapper() {
                 return this.constructor.modalWrapper
             }
             get modal() {
-                var e = this.wrapper.querySelector(`.${Lt}`);
-                e && e.id !== `${Lt}-${this.options.modalId}-modal` && (e.remove(), e = null), e || (e = this.buildModal());
+                var e = this.wrapper.querySelector(`.${Tt}`);
+                e && e.id !== `${Tt}-${this.options.modalId}-modal` && (e.remove(), e = null), e || (e = this.buildModal());
                 var t = e;
                 return t.modal = this, t
             }
             get innerHTML() {
                 return this.modal.innerHTML
             }
             set innerHTML(e) {
@@ -2227,16 +2232,16 @@
                 return this.modal.classList
             }
             get children() {
                 return this.modal.children
             }
             buildModal() {
                 var e = this.wrapper,
-                    t = e.querySelector(`.${Lt}`);
-                return t || (e.innerHTML = this.modalHtml, t = e.querySelector(`.${Lt}`)), t.modal || (t.modal = this), t
+                    t = e.querySelector(`.${Tt}`);
+                return t || (e.innerHTML = this.modalHtml, t = e.querySelector(`.${Tt}`)), t.modal || (t.modal = this), t
             }
             addClass(e) {
                 this.modal.classList.add(e)
             }
             removeClass(e) {
                 this.modal.classList.remove(e)
             }
@@ -2266,50 +2271,34 @@
             addEventListener(e, t) {
                 this.modal.addEventListener(e, t)
             }
             removeEventListener(e, t) {
                 this.modal.removeEventListener(e, t)
             }
         }
-        class St {
+        class Ct {
             constructor(e) {
-                this.executeOnloadImmediately = !1;
-                const {
-                    id: t,
-                    className: n,
-                    srcdoc: i = null,
-                    url: r = null,
-                    onLoad: o = (() => {}),
-                    onError: a = (() => {}),
-                    onCancel: s = (() => {}),
-                    onResize: c = (() => {}),
-                    executeOnloadImmediately: l = !1
-                } = e;
-                this.url = r, this.srcdoc = i, this.iframe = null, this.id = t, this.className = n, this.onResize = c, this.executeOnloadImmediately = l, this.onLoad = o, this.onError = a, this.onCancel = s, this.render()
+                this.executeOnloadImmediately = !1, this.url = e.url, this.srcdoc = e.srcdoc, this.iframe = null, this.id = e.id, this.className = e.className, this.onResize = e.onResize, this.executeOnloadImmediately = e.executeOnloadImmediately, this.onLoad = e.onLoad, this.onError = e.onError, this.onCancel = e.onCancel, this.render()
             }
             get element() {
                 return this.iframe || (this.iframe = this._renderFrame(this.url, this.srcdoc, this.onLoad)), this.iframe
             }
             get document() {
                 return this.window ? this.window.document : null
             }
             get window() {
-                return this.element.contentWindow
+                var e;
+                return null === (e = this.element) || void 0 === e ? void 0 : e.contentWindow
             }
             get mainElement() {
                 var e;
                 return null === (e = this.document) || void 0 === e ? void 0 : e.querySelector("#main")
             }
-            get formElement() {
-                var e;
-                return null === (e = this.document) || void 0 === e ? void 0 : e.querySelector("#wagtail-fedit-form")
-            }
-            get formWrapper() {
-                var e;
-                return null === (e = this.document) || void 0 === e ? void 0 : e.querySelector(".wagtail-fedit-form-wrapper")
+            get scrollableElement() {
+                return this.document.body
             }
             destroy() {
                 this.iframe.remove(), this.resizeInterval && (clearInterval(this.resizeInterval), delete this.resizeInterval)
             }
             update(e, t) {
                 this.srcdoc = t, this.url = e, this._renderFrame(this.url, this.srcdoc, (({
                     newFrame: e
@@ -2321,42 +2310,59 @@
             }
             render() {
                 return this.iframe || (this.iframe = this._renderFrame(this.url, this.srcdoc, this.onLoad)), this.iframe
             }
             _renderFrame(e, t, n, i = (() => {})) {
                 const r = document.createElement("iframe");
                 return t ? r.srcdoc = t : r.src = e, r.id = this.id, r.className = this.className, r.onload = () => {
-                    if (!this.formElement) return void i();
-                    let e = this.formElement,
+                    if (!this.scrollableElement) return void i();
+                    let e = this.scrollableElement,
                         t = e.scrollHeight;
                     this.onResize && this.onResize(0, t), this.resizeInterval && clearInterval(this.resizeInterval), this.onResize && (this.resizeInterval = setInterval((() => {
                         if (e) try {
                             t !== e.scrollHeight && (this.onResize(t, e.scrollHeight), t = e.scrollHeight)
                         } catch (e) {
                             clearInterval(this.resizeInterval), console.error(e), i()
                         } else clearInterval(this.resizeInterval)
-                    }), 25));
-                    const o = this.document.querySelector(".wagtail-fedit-cancel-button");
-                    o && o.addEventListener("click", (() => {
-                        clearInterval(this.resizeInterval), this.onCancel()
-                    })), "complete" === this.document.readyState || this.executeOnloadImmediately ? n({
+                    }), 25)), this._onLoad(r), n && (this.executeOnloadImmediately || "complete" === this.document.readyState ? n({
                         newFrame: r
                     }) : r.contentWindow.addEventListener("DOMContentLoaded", (() => {
                         n({
                             newFrame: r
                         })
-                    }))
+                    })))
                 }, r.onerror = () => {
                     i()
                 }, r
             }
+            _onLoad(e) {}
         }
-        class Ct extends EventTarget {
+        class Dt extends Ct {
+            get scrollableElement() {
+                return this.document.querySelector(".wagtail-fedit-form-wrapper")
+            }
+            get formElement() {
+                var e;
+                return null === (e = this.document) || void 0 === e ? void 0 : e.querySelector("#wagtail-fedit-form")
+            }
+            get formWrapper() {
+                var e;
+                return null === (e = this.document) || void 0 === e ? void 0 : e.querySelector(".wagtail-fedit-form-wrapper")
+            }
+            _onLoad(e) {
+                super._onLoad(e);
+                const t = this.document.querySelector(".wagtail-fedit-cancel-button");
+                t && t.addEventListener("click", (() => {
+                    clearInterval(this.resizeInterval), this.onCancel && this.onCancel()
+                }))
+            }
+        }
+        class Mt extends EventTarget {
             constructor(e) {
-                super(), this.api = new Ot(this), this.initialTitle = document.title, this.wrapperElement = e, this.sharedContext = null, this.editBtn = null, this.iframe = null, this.init(), window.location.hash === `#${this.wrapperElement.id}` && (this.openEditor(), this.focus())
+                super(), this.api = new Lt(this), this.initialTitle = document.title, this.wrapperElement = e, this.sharedContext = null, this.editBtn = null, this.iframe = null, this.init(), window.location.hash === `#${this.wrapperElement.id}` && (this.openEditor(), this.focus())
             }
             get editUrl() {
                 return this.wrapperElement.dataset.editUrl
             }
             get refetchUrl() {
                 return this.wrapperElement.dataset.refetchUrl
             }
@@ -2394,37 +2400,48 @@
                         }
                         c((r = r.apply(t, n || [])).next())
                     }));
                     var t, n, i, r
                 }))
             }
             initNewEditors() {
-                bt(this.wrapperElement)
+                Et(this.wrapperElement)
             }
             focus() {
                 this.wrapperElement.focus()
             }
             refetch() {
                 return new Promise(((e, t) => {
                     fetch(this.refetchUrl).then((e => e.json())).then((t => {
                         t.success ? (this.onResponse(t), e(t)) : console.error("Errors rendering response, failed to refetch", t)
                     })).catch((e => {
                         console.error("Failed to refetch", e), t(e)
                     }))
                 }))
             }
+            refetchParent(e) {
+                let t = document.body,
+                    n = this.wrapperElement.parentElement;
+                for (; n && n !== t;) {
+                    if (n.classList.contains("wagtail-fedit-initialized")) return void n.editorAPI.refetch().then((() => {
+                        Et(n)
+                    }));
+                    n = n.parentElement
+                }
+                e && e()
+            }
             onResponse(e) {
                 throw new Error("onResponse not implemented, cannot call super")
             }
             get frameOptions() {
                 return {}
             }
             openIframe(e, t) {
                 if (this.iframe) return e.appendChild(this.iframe.element), void t(this.iframe);
-                this.iframe = new St(Object.assign(Object.assign({
+                this.iframe = new Dt(Object.assign(Object.assign({
                     url: this.editUrl,
                     id: "wagtail-fedit-iframe",
                     className: null,
                     executeOnloadImmediately: !0
                 }, this.frameOptions), {
                     onLoad: () => {
                         const t = e => {
@@ -2476,19 +2493,18 @@
                     },
                     onCancel: () => {
                         this.closeEditor()
                     }
                 })), e.appendChild(this.iframe.element), t(this.iframe)
             }
             openEditor() {
-                this.modal || (this.modal = new At({
-                    modalId: this.wrapperElement.id
+                this.modal || (this.modal = new St({
+                    modalId: `${this.wrapperElement.id}-modal`
                 })), this.opened = !0, this.openIframe(this.modal, (e => {
-                    const t = document.createElement("button");
-                    t.innerHTML = "&times;", t.classList.add("wagtail-fedit-close-button"), t.addEventListener("click", this.closeEditor.bind(this)), this.modal.appendChild(t), this.executeEvent(window.wagtailFedit.EVENTS.EDITOR_OPEN, {
+                    this.modal.appendChild(It(this.closeEditor.bind(this))), this.executeEvent(window.wagtailFedit.EVENTS.EDITOR_OPEN, {
                         iframe: this.iframe,
                         modal: this.modal
                     }), this.modal.openModal()
                 }))
             }
             closeEditor() {
                 this.opened = !1, window.history.pushState(null, this.initialTitle, window.location.href.split("#")[0]), document.title = this.initialTitle, this.executeEvent(window.wagtailFedit.EVENTS.EDITOR_CLOSE), this.modal.closeModal()
@@ -2499,15 +2515,20 @@
                 }), t.editor = this, t.api = this.api, e.startsWith(`${window.wagtailFedit.NAMESPACE}:`) || (e = `${window.wagtailFedit.NAMESPACE}:${e}`);
                 const n = new CustomEvent(e, {
                     detail: t
                 });
                 super.dispatchEvent(n), this.wrapperElement.dispatchEvent(n), document.dispatchEvent(n)
             }
         }
-        class Dt {
+
+        function It(e) {
+            const t = document.createElement("button");
+            return t.innerHTML = "&times;", t.classList.add("wagtail-fedit-close-button"), t.addEventListener("click", e), t
+        }
+        class kt {
             constructor(e) {
                 this.publishButton = e, this.publishButtonsWrapper = e.parentElement.querySelector(".wagtail-fedit-form-buttons"), this.publishButtonsWrapper.querySelectorAll(".wagtail-fedit-userbar-button"), this.init()
             }
             init() {
                 this.publishButton.addEventListener("click", (e => {
                     this.publishButtonsWrapper.classList.contains("open") ? this.publishButtonsWrapper.animate([{
                         opacity: 1,
@@ -2531,30 +2552,30 @@
                         easing: "ease-in-out"
                     }).onfinish = () => {
                         this.publishButtonsWrapper.classList.add("open")
                     })
                 }))
             }
         }
-        class Mt extends Ct {
+        class Rt extends Mt {
             static get funcMap() {
                 return window
             }
             onResponse(e) {
                 const t = e.func.name,
                     n = e.func.target;
                 if (!t || !n) return void console.error("Invalid response", e);
                 const i = document.querySelector(n);
                 if (!i) return void console.error("Target element not found", n);
                 const r = this.constructor.funcMap[t];
                 if (r) return r(i, e);
                 console.error("Function not found", t)
             }
         }
-        class It extends Ct {
+        class Pt extends Mt {
             onResponse(e) {
                 return this.api.updateHtml((t => {
                     this.wrapperElement.animate([{
                         opacity: 1
                     }, {
                         opacity: 0
                     }], {
@@ -2575,35 +2596,71 @@
                             n.style.opacity = "1"
                         }
                     }
                 }))
             }
         }
 
-        function kt(e) {
+        function jt(e) {
             return class extends e {
                 constructor(...e) {
                     super(...e);
                     let t = this.wrapperElement.querySelectorAll("[data-direction]");
                     for (let e = 0; e < t.length; e++) {
                         let n = t[e],
                             i = n.dataset.url;
                         n.addEventListener("click", (e => {
                             e.preventDefault(), this.api.fetch(i, "POST", {}).then((e => {
-                                e.success ? Et() : e.error ? alert("Failed to move block: " + e.error) : alert("Failed to move block")
+                                e.success ? this.refetchParent(xt) : e.error ? alert("Failed to move block: " + e.error) : alert("Failed to move block")
                             })).catch((e => {
                                 console.error("Failed to move block", e), alert("Failed to move block")
                             }))
                         }))
                     }
                 }
             }
         }
-        class Rt extends(kt(It)) {}
-        class jt extends It {
+
+        function Ht(e) {
+            return class extends e {
+                constructor(...e) {
+                    super(...e);
+                    let t = this.wrapperElement.querySelector("[data-add]");
+                    if (!t) return void console.error('"Add" button not found, cannot further initialize AddableMixin');
+                    const n = t.dataset.url,
+                        i = new St({
+                            modalId: `${this.wrapperElement.id}-modal`
+                        });
+                    t.addEventListener("click", (e => {
+                        e.preventDefault(), i.openModal();
+                        const t = new Dt({
+                            id: "wagtail-fedit-iframe",
+                            className: null,
+                            url: n,
+                            onLoad: ({
+                                newFrame: e
+                            }) => {
+                                t.formElement.onsubmit = e => {
+                                    e.preventDefault();
+                                    const r = new FormData(t.formElement);
+                                    this.api.fetch(n, "POST", r).then((e => {
+                                        e.success ? (i.closeModal(), this.refetchParent(xt)) : e.error ? alert("Failed to add block: " + e.error) : alert("Failed to add block")
+                                    })).catch((e => {
+                                        console.error("Failed to add block", e), alert("Failed to add block")
+                                    }))
+                                }
+                            }
+                        });
+                        t.destroy(), i.appendChild(t.element), i.appendChild(It(i.closeModal.bind(i)))
+                    }))
+                }
+            }
+        }
+        class Nt extends(Ht(jt(Pt))) {}
+        class Ft extends Pt {
             get buttonsElement() {
                 return this.wrapperElement.querySelector(".wagtail-fedit-buttons")
             }
             get formElement() {
                 return this.wrapperElement.querySelector(".wagtail-fedit-adapter-form")
             }
             get contentElement() {
@@ -2621,22 +2678,22 @@
                     this.contentElement.style.display = "none"
                 }))
             }
             closeEditor() {
                 this.opened = !1, window.history.pushState(null, this.initialTitle, window.location.href.split("#")[0]), document.title = this.initialTitle, this.contentElement.style.display = "block", this.iframe.destroy(), this.executeEvent(window.wagtailFedit.EVENTS.EDITOR_CLOSE), delete this.iframe
             }
         }
-        class Pt extends(kt(jt)) {}
+        class Wt extends(Ht(jt(Ft))) {}
 
-        function Ht() {
-            bt(), new MutationObserver((e => {
+        function Bt() {
+            Et(), new MutationObserver((e => {
                 for (const t of e)
                     for (let e = 0; e < t.addedNodes.length; e++) {
                         const n = t.addedNodes[e];
-                        1 === n.nodeType && bt(n)
+                        1 === n.nodeType && Et(n)
                     }
             })).observe(document.body, {
                 childList: !0,
                 subtree: !0
             });
             const e = new URL(window.location.href),
                 t = e.searchParams.get("scrollY") || 0,
@@ -2647,40 +2704,40 @@
                 const e = i.shadowRoot.querySelector("#wagtail-fedit-editor-button"),
                     t = i.shadowRoot.querySelector("#wagtail-fedit-live-button"),
                     n = i.shadowRoot.querySelector("#wagtail-fedit-publish-menu");
                 if (e || t) {
                     let n;
                     window.addEventListener("scroll", (() => {
                         n && clearTimeout(n), n = setTimeout((() => {
-                            xt(e), xt(t);
+                            Ot(e), Ot(t);
                             const n = new URL(window.location.href);
                             n.searchParams.set("scrollY", `${window.scrollY}`), n.searchParams.set("scrollX", `${window.scrollX}`), window.history.replaceState(null, "", n.toString())
                         }), 50)
                     }))
                 }
-                n && new Dt(n)
+                n && new kt(n)
             }
         }
         window.wagtailFedit = {
             NAMESPACE: "wagtail-fedit",
             EVENTS: {
                 SUBMIT: "wagtail-fedit:submit",
                 CHANGE: "wagtail-fedit:change",
                 EDITOR_OPEN: "wagtail-fedit:editorOpen",
                 EDITOR_LOAD: "wagtail-fedit:editorLoad",
                 EDITOR_CLOSE: "wagtail-fedit:editorClose",
                 SUBMIT_ERROR: "wagtail-fedit:submitError"
             },
             editors: {
-                "wagtail_fedit.editors.BaseFuncEditor": Mt,
-                "wagtail_fedit.editors.FieldEditor": It,
-                "wagtail_fedit.editors.BlockEditor": Rt,
-                "wagtail_fedit.editors.DomPositionedFieldEditor": jt,
-                "wagtail_fedit.editors.DomPositionedBlockEditor": Pt,
-                "wagtail_fedit.editors.WagtailFeditFuncEditor": class extends Mt {
+                "wagtail_fedit.editors.BaseFuncEditor": Rt,
+                "wagtail_fedit.editors.FieldEditor": Pt,
+                "wagtail_fedit.editors.BlockEditor": Nt,
+                "wagtail_fedit.editors.DomPositionedFieldEditor": Ft,
+                "wagtail_fedit.editors.DomPositionedBlockEditor": Wt,
+                "wagtail_fedit.editors.WagtailFeditFuncEditor": class extends Rt {
                     static get funcMap() {
                         return window.wagtailFedit.funcs
                     }
                 }
             },
             funcs: {
                 "wagtail_fedit.funcs.backgroundImageFunc": function(e, t) {
@@ -2691,10 +2748,10 @@
             },
             register: function(e, t) {
                 this.editors[e] = t
             },
             registerFunc: function(e, t) {
                 this.funcs[e] = t
             }
-        }, "loading" === document.readyState ? document.addEventListener("DOMContentLoaded", Ht) : Ht()
+        }, "loading" === document.readyState ? document.addEventListener("DOMContentLoaded", Bt) : Bt()
     })()
 })();
```

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/static/wagtail_fedit/js/licenses/TIPPY.LICENSE` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/static/wagtail_fedit/js/licenses/TIPPY.LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/wagtail_fedit/content/buttons/move_down.html` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/content/buttons/move_down.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/wagtail_fedit/content/buttons/move_up.html` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/content/buttons/move_up.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/wagtail_fedit/editor/field.html` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/editor/field.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/templates/wagtail_fedit/userbar/publish/item_fedit_publishing.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/templatetags/fedit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/test/core/migrations/0001_initial.py` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/test/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/test/core/models.py` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/test/core/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/test/core/tests/base.py` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/test/core/tests/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/test/core/tests/test_adapters.py` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/test/core/tests/test_adapters.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/test/core/tests/test_block_edit.py` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/test/core/tests/test_block_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/test/core/tests/test_blocks.py` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/test/core/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/test/core/tests/test_field_edit.py` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/test/core/tests/test_field_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/test/core/tests/test_generic.py` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/test/core/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/test/core/tests/test_model_edit.py` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/test/core/tests/test_model_edit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/test/core/tests/test_revision.py` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/test/core/tests/test_revision.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/test/core/tests/test_submit.py` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/test/core/tests/test_submit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/test/manage.py` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/test/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/test/testapp/settings.py` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/test/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/test/testapp/urls.py` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/test/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/toolbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/urls.py` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/utils.py` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 from django.conf import settings
 from django.urls import reverse
 
 from wagtail.models import (
     DraftStateMixin,
     WorkflowMixin,
     LockableMixin,
-    PreviewableMixin
+    PreviewableMixin,
+    RevisionMixin,
 )
 from wagtail.admin.admin_url_finder import AdminURLFinder
 from wagtail.blocks.stream_block import StreamValue
 from wagtail.blocks.list_block import ListValue
 from wagtail import (
     hooks,
     blocks,
@@ -192,39 +193,40 @@
         contentpath = []
 
     # Check and cast field to iterable if necessary, but do not append non-StreamValue names to contentpath here.
     if not isinstance(field, StreamValue) and not hasattr(field, "__iter__"):
         field = [field]
 
     # Adjust for ListValue to get the iterable bound_blocks.
+    parent_block = field
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
 
         elif isinstance(block.value, (StreamValue, StreamValue.StreamChild, ListValue)):
             found, found_path, parent, block_index = find_block(block_id, block.value, contentpath + [block_name])
             if found:
                 return found, found_path, parent, block_index
 
     # Return None and the current path if no block is found at this level.
-    return None, contentpath, field, -1
+    return None, contentpath, parent_block, -1
 
 
 
 _renderer_map = {}
 _field_renderer_map = {}
 _looked_for_renderers = False
 
@@ -467,14 +469,41 @@
             user
         )
     else:
         lock = None
         locked_for_user = False
 
     return _lock_info(lock, locked_for_user)
+    
+def insert_many(parent: Union[StreamValue, ListValue], idx, blocks):
+    if len(parent) == 0 or idx == len(parent) - 1:
+        parent.extend(blocks)
+    elif idx < len(parent) - 1:
+        if isinstance(parent, StreamValue):
+            for i, block in enumerate(blocks):
+                parent.insert(idx + i + 1, block)
+                parent._raw_data[idx + i + 1] = block.get_prep_value()
+        elif isinstance(parent, ListValue):
+            for i, block in enumerate(blocks):
+                parent.insert(idx + i + 1, block)
+    else:
+        raise IndexError("Cannot add block, index out of range ({} > {})".format(idx, len(parent) - 1))
+
+def save_revision(instance: models.Model, user: Any) -> models.Model:
+    """
+    Save a revision for a model instance.
+    """
+    if isinstance(instance, RevisionMixin):
+        instance.save_revision(
+            user=user,
+        )
+    else:
+        instance.save()
+    return instance
+
 
 def _flatten_context(context: dict) -> dict:
     if hasattr(context, "flatten"):
         return context.flatten()
     return context
 
 def base_adapter_context(adapter: "BaseAdapter", context: Union[Context, dict]) -> dict:
```

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/views/adapters.py` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/views/adapters.py`

 * *Files 5% similar despite different names*

```diff
@@ -145,23 +145,30 @@
 
         setattr(
             self.request,
             FEDIT_PREVIEW_VAR,
             True,
         )
 
+        could_respond = self.before_dispatch()
+        if isinstance(could_respond, HttpResponse):
+            return could_respond
+
         return super().dispatch(
             request,
             adapter_id=adapter_id,
             field_name=field_name,
             app_label=app_label,
             model_name=model_name,
             model_id=model_id,
         )
     
+    def before_dispatch(self) -> HttpResponse | None:
+        pass
+
     @classmethod
     def prefix_url_path(cls, name: str, *suffix: str) -> str:
         suffix_url = ""
         
         if suffix:
             suffix_url = f"{'/'.join(suffix)}"
```

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/views/editable.py` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/views/editable.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/views/mixins.py` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/views/mixins.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/wagtail_hooks/action_menu.py` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/wagtail_hooks/action_menu.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/wagtail_hooks/adapter_hooks.py` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/wagtail_hooks/adapter_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/wagtail_hooks/adapters.py` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/wagtail_hooks/adapters.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.5.9rc2/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit.egg-info/PKG-INFO` & `wagtail_fedit-1.5.9rc2/wagtail_fedit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-fedit
-Version: 1.5.9rc1
+Version: 1.5.9rc2
 Summary: Frontend editing for your Wagtail site
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-2.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `wagtail_fedit-1.5.9rc1/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.5.9rc2/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,19 +17,22 @@
 wagtail_fedit.egg-info/PKG-INFO
 wagtail_fedit.egg-info/SOURCES.txt
 wagtail_fedit.egg-info/dependency_links.txt
 wagtail_fedit.egg-info/requires.txt
 wagtail_fedit.egg-info/top_level.txt
 wagtail_fedit/adapters/__init__.py
 wagtail_fedit/adapters/base.py
-wagtail_fedit/adapters/block.py
 wagtail_fedit/adapters/field.py
 wagtail_fedit/adapters/funcs.py
 wagtail_fedit/adapters/misc.py
 wagtail_fedit/adapters/models.py
+wagtail_fedit/adapters/block/__init__.py
+wagtail_fedit/adapters/block/adapter.py
+wagtail_fedit/adapters/block/buttons.py
+wagtail_fedit/adapters/block/views.py
 wagtail_fedit/forms/__init__.py
 wagtail_fedit/forms/blocks.py
 wagtail_fedit/forms/fields.py
 wagtail_fedit/locale/nl/LC_MESSAGES/django.mo
 wagtail_fedit/locale/nl/LC_MESSAGES/django.po
 wagtail_fedit/migrations/__init__.py
 wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
@@ -37,27 +40,30 @@
 wagtail_fedit/static/wagtail_fedit/css/furniture.css
 wagtail_fedit/static/wagtail_fedit/css/userbar-menu.css
 wagtail_fedit/static/wagtail_fedit/js/edit.js
 wagtail_fedit/static/wagtail_fedit/js/licenses/TIPPY.LICENSE
 wagtail_fedit/templates/wagtail_fedit/_hook_output.html
 wagtail_fedit/templates/wagtail_fedit/content/editable_adapter.html
 wagtail_fedit/templates/wagtail_fedit/content/editable_dom_positioned_adapter.html
+wagtail_fedit/templates/wagtail_fedit/content/buttons/add_block.html
 wagtail_fedit/templates/wagtail_fedit/content/buttons/admin_link.html
 wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_adapter.html
 wagtail_fedit/templates/wagtail_fedit/content/buttons/move_down.html
 wagtail_fedit/templates/wagtail_fedit/content/buttons/move_up.html
 wagtail_fedit/templates/wagtail_fedit/editor/action_confirm.html
 wagtail_fedit/templates/wagtail_fedit/editor/action_publish_confirm.html
 wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler.html
 wagtail_fedit/templates/wagtail_fedit/editor/adapter_edit_handler_form.html
 wagtail_fedit/templates/wagtail_fedit/editor/adapter_form.html
 wagtail_fedit/templates/wagtail_fedit/editor/adapter_form_errors.html
 wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe.html
 wagtail_fedit/templates/wagtail_fedit/editor/adapter_iframe_dom_positioned.html
 wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+wagtail_fedit/templates/wagtail_fedit/editor/block_adapter_add_form.html
+wagtail_fedit/templates/wagtail_fedit/editor/block_adapter_iframe.html
 wagtail_fedit/templates/wagtail_fedit/editor/field.html
 wagtail_fedit/templates/wagtail_fedit/icons/fedit-check-list.svg
 wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-closed.svg
 wagtail_fedit/templates/wagtail_fedit/icons/fedit-eye-open.svg
 wagtail_fedit/templates/wagtail_fedit/icons/fedit-save.svg
 wagtail_fedit/templates/wagtail_fedit/icons/fedit-stop-sign.svg
 wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
```

