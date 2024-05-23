# Comparing `tmp/cone.app-1.1a2.tar.gz` & `tmp/cone_app-1.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cone.app-1.1a2.tar", last modified: Mon Feb 12 10:05:31 2024, max compression
+gzip compressed data, was "cone_app-1.1rc1.tar", last modified: Thu May 23 13:45:55 2024, max compression
```

## Comparing `cone.app-1.1a2.tar` & `cone_app-1.1rc1.tar`

### file list

```diff
@@ -1,208 +1,208 @@
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-02-12 10:05:31.572425 cone.app-1.1a2/
--rw-r--r--   0 rnix      (1000) rnix      (1000)    32590 2024-02-12 10:05:31.000000 cone.app-1.1a2/CHANGES.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1378 2024-02-12 10:05:31.000000 cone.app-1.1a2/LICENSE.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)      138 2024-02-12 10:05:31.000000 cone.app-1.1a2/MANIFEST.in
--rw-r--r--   0 rnix      (1000) rnix      (1000)    36429 2024-02-12 10:05:31.572425 cone.app-1.1a2/PKG-INFO
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1179 2024-02-12 10:05:31.000000 cone.app-1.1a2/README.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2829 2024-02-12 10:05:31.000000 cone.app-1.1a2/TODO.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)       74 2024-02-12 10:05:31.572425 cone.app-1.1a2/setup.cfg
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2153 2024-02-12 10:05:31.000000 cone.app-1.1a2/setup.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-02-12 10:05:31.552425 cone.app-1.1a2/src/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-02-12 10:05:31.556425 cone.app-1.1a2/src/cone/
--rw-r--r--   0 rnix      (1000) rnix      (1000)       56 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/__init__.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-02-12 10:05:31.556425 cone.app-1.1a2/src/cone/app/
--rw-r--r--   0 rnix      (1000) rnix      (1000)    12270 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/__init__.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-02-12 10:05:31.556425 cone.app-1.1a2/src/cone/app/browser/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3025 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/__init__.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    17063 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/actions.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    12016 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/ajax.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    18877 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/authoring.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    15277 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/batch.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3889 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/content.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     8741 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/contents.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     5143 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/contextmenu.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     5563 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/copysupport.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3006 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/exception.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     6293 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/form.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    16540 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/layout.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3223 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/login.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2440 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/order.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    15050 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/referencebrowser.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    11679 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/resources.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     6175 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/settings.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     7325 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/sharing.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-02-12 10:05:31.552425 cone.app-1.1a2/src/cone/app/browser/static/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-02-12 10:05:31.552425 cone.app-1.1a2/src/cone/app/browser/static/bootstrap/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-02-12 10:05:31.560425 cone.app-1.1a2/src/cone/app/browser/static/bootstrap/css/
--rw-r--r--   0 rnix      (1000) rnix      (1000)    25682 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/static/bootstrap/css/bootstrap-theme.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)    48005 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/static/bootstrap/css/bootstrap-theme.css.map
--rw-r--r--   0 rnix      (1000) rnix      (1000)    23411 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/static/bootstrap/css/bootstrap-theme.min.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)    75600 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/static/bootstrap/css/bootstrap-theme.min.css.map
--rw-r--r--   0 rnix      (1000) rnix      (1000)   145933 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/static/bootstrap/css/bootstrap.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)   390887 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/static/bootstrap/css/bootstrap.css.map
--rw-r--r--   0 rnix      (1000) rnix      (1000)   121457 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/static/bootstrap/css/bootstrap.min.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)   540434 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/static/bootstrap/css/bootstrap.min.css.map
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-02-12 10:05:31.560425 cone.app-1.1a2/src/cone/app/browser/static/bootstrap/fonts/
--rw-r--r--   0 rnix      (1000) rnix      (1000)    20127 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/static/bootstrap/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 rnix      (1000) rnix      (1000)   108738 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/static/bootstrap/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 rnix      (1000) rnix      (1000)    45404 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/static/bootstrap/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 rnix      (1000) rnix      (1000)    23424 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/static/bootstrap/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 rnix      (1000) rnix      (1000)    18028 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/static/bootstrap/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-02-12 10:05:31.560425 cone.app-1.1a2/src/cone/app/browser/static/bootstrap/js/
--rw-r--r--   0 rnix      (1000) rnix      (1000)    75484 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/static/bootstrap/js/bootstrap.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)    39680 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/static/bootstrap/js/bootstrap.min.js
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-02-12 10:05:31.560425 cone.app-1.1a2/src/cone/app/browser/static/cone/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     5591 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/static/cone/cone.app.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4446 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/static/cone/cone.app.min.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)       67 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/static/cone/cone.app.print.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)    23862 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/static/cone/cone.app.protected.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)    11129 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/static/cone/cone.app.protected.min.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2128 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/static/cone/cone.app.public.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1111 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/static/cone/cone.app.public.min.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1406 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/static/cone/favicon.ico
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-02-12 10:05:31.560425 cone.app-1.1a2/src/cone/app/browser/static/ionicons/
--rw-r--r--   0 rnix      (1000) rnix      (1000)       31 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/static/ionicons/.gitignore
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-02-12 10:05:31.560425 cone.app-1.1a2/src/cone/app/browser/static/ionicons/css/
--rw-r--r--   0 rnix      (1000) rnix      (1000)    47987 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/static/ionicons/css/ionicons.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)    42998 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/static/ionicons/css/ionicons.min.css
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-02-12 10:05:31.560425 cone.app-1.1a2/src/cone/app/browser/static/ionicons/fonts/
--rw-r--r--   0 rnix      (1000) rnix      (1000)   101984 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/static/ionicons/fonts/ionicons.eot
--rw-r--r--   0 rnix      (1000) rnix      (1000)   286345 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/static/ionicons/fonts/ionicons.svg
--rw-r--r--   0 rnix      (1000) rnix      (1000)   164548 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/static/ionicons/fonts/ionicons.ttf
--rw-r--r--   0 rnix      (1000) rnix      (1000)    57276 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/static/ionicons/fonts/ionicons.woff
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-02-12 10:05:31.564425 cone.app-1.1a2/src/cone/app/browser/static/jquery/
--rw-r--r--   0 rnix      (1000) rnix      (1000)   288580 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/static/jquery/jquery-3.6.0.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)    89501 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/static/jquery/jquery-3.6.0.min.js
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-02-12 10:05:31.564425 cone.app-1.1a2/src/cone/app/browser/static/typeahead/
--rw-r--r--   0 rnix      (1000) rnix      (1000)    71417 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/static/typeahead/typeahead.bundle.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     6240 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/static/typeahead/typeahead.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)     7236 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/table.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-02-12 10:05:31.564425 cone.app-1.1a2/src/cone/app/browser/templates/
--rw-r--r--   0 rnix      (1000) rnix      (1000)      912 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/templates/action_dropdown.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      842 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/templates/add_dropdown.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4359 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/templates/batch.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      713 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/templates/batched_items.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1043 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/templates/batched_items_footer.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2568 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/templates/batched_items_header.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1577 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/templates/button_action.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      697 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/templates/byline.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      627 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/templates/content_form.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      548 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/templates/contextmenu.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      682 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/templates/contextmenu_dropdown.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)       23 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/templates/default_root.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      324 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/templates/footer.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      402 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/templates/insufficient_privileges.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      830 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/templates/language.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2280 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/templates/layout.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2603 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/templates/link_action.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      223 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/templates/listing.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      846 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/templates/livesearch.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      417 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/templates/logo.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      647 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/templates/main.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2476 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/templates/mainmenu.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      558 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/templates/navtree.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      976 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/templates/navtree_recue.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      363 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/templates/not_found.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1030 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/templates/pathbar.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      524 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/templates/personaltools.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      424 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/templates/referencebrowser.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      898 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/templates/referencebrowser_pathbar.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      253 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/templates/resources.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1133 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/templates/settings.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      315 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/templates/settings_form.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1332 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/templates/settings_sidebar.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      220 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/templates/sharing.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)     7517 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/templates/table.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      377 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/templates/unauthorized.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1435 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/templates/wf_dropdown.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4160 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/translation.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3617 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/utils.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2574 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/browser/workflow.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)      715 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/compat.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)      140 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/configure.zcml
--rw-r--r--   0 rnix      (1000) rnix      (1000)     6452 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/interfaces.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-02-12 10:05:31.564425 cone.app-1.1a2/src/cone/app/locale/
--rw-r--r--   0 rnix      (1000) rnix      (1000)    11022 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/locale/cone.app.pot
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-02-12 10:05:31.552425 cone.app-1.1a2/src/cone/app/locale/de/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-02-12 10:05:31.564425 cone.app-1.1a2/src/cone/app/locale/de/LC_MESSAGES/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     5714 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/locale/de/LC_MESSAGES/cone.app.mo
--rw-r--r--   0 rnix      (1000) rnix      (1000)    12832 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/locale/de/LC_MESSAGES/cone.app.po
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-02-12 10:05:31.552425 cone.app-1.1a2/src/cone/app/locale/en/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-02-12 10:05:31.564425 cone.app-1.1a2/src/cone/app/locale/en/LC_MESSAGES/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     5207 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/locale/en/LC_MESSAGES/cone.app.mo
--rw-r--r--   0 rnix      (1000) rnix      (1000)    12317 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/locale/en/LC_MESSAGES/cone.app.po
--rw-r--r--   0 rnix      (1000) rnix      (1000)    21797 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/model.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     8760 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/security.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-02-12 10:05:31.568425 cone.app-1.1a2/src/cone/app/testing/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     7002 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/testing/__init__.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-02-12 10:05:31.552425 cone.app-1.1a2/src/cone/app/testing/data/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-02-12 10:05:31.568425 cone.app-1.1a2/src/cone/app/testing/data/ugm/
--rw-r--r--   0 rnix      (1000) rnix      (1000)       11 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/testing/data/ugm/groups
--rw-r--r--   0 rnix      (1000) rnix      (1000)       81 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/testing/data/ugm/roles
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-02-12 10:05:31.552425 cone.app-1.1a2/src/cone/app/testing/data/ugm/userdata/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-02-12 10:05:31.568425 cone.app-1.1a2/src/cone/app/testing/data/ugm/userdata/groups/
--rw-r--r--   0 rnix      (1000) rnix      (1000)       50 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/testing/data/ugm/userdata/groups/group1
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-02-12 10:05:31.568425 cone.app-1.1a2/src/cone/app/testing/data/ugm/userdata/users/
--rw-r--r--   0 rnix      (1000) rnix      (1000)       40 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/testing/data/ugm/userdata/users/admin
--rw-r--r--   0 rnix      (1000) rnix      (1000)       42 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/testing/data/ugm/userdata/users/editor
--rw-r--r--   0 rnix      (1000) rnix      (1000)       44 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/testing/data/ugm/userdata/users/manager
--rw-r--r--   0 rnix      (1000) rnix      (1000)       42 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/testing/data/ugm/userdata/users/max
--rw-r--r--   0 rnix      (1000) rnix      (1000)       44 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/testing/data/ugm/userdata/users/sepp
--rw-r--r--   0 rnix      (1000) rnix      (1000)       42 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/testing/data/ugm/userdata/users/viewer
--rw-r--r--   0 rnix      (1000) rnix      (1000)      379 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/testing/data/ugm/users
--rw-r--r--   0 rnix      (1000) rnix      (1000)       36 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/testing/dummy_action.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      126 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/testing/dummy_batched_items.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      393 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/testing/dummy_form.yaml
--rw-r--r--   0 rnix      (1000) rnix      (1000)      234 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/testing/dummy_main.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      956 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/testing/dummy_workflow.zcml
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3222 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/testing/mock.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-02-12 10:05:31.568425 cone.app-1.1a2/src/cone/app/testing/static/
--rw-r--r--   0 rnix      (1000) rnix      (1000)       26 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/testing/static/print1.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)       26 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/testing/static/print2.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)       23 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/testing/static/script1.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)       23 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/testing/static/script2.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)       27 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/testing/static/style1.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)       27 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/testing/static/style2.css
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-02-12 10:05:31.572425 cone.app-1.1a2/src/cone/app/tests/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3616 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/tests/__init__.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     8027 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/tests/test_app.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2977 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/tests/test_browser.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    31055 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/tests/test_browser_actions.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    18113 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/tests/test_browser_ajax.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    50700 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/tests/test_browser_authoring.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    33391 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/tests/test_browser_batch.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4380 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/tests/test_browser_content.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    14673 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/tests/test_browser_contents.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     5391 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/tests/test_browser_contextmenu.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     8429 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/tests/test_browser_copysupport.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     5885 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/tests/test_browser_exception.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    17324 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/tests/test_browser_form.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    27684 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/tests/test_browser_layout.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2203 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/tests/test_browser_login.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2458 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/tests/test_browser_order.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    41731 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/tests/test_browser_referencebrowser.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    16029 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/tests/test_browser_resources.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    12875 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/tests/test_browser_settings.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    10985 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/tests/test_browser_sharing.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     7869 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/tests/test_browser_table.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    11245 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/tests/test_browser_translation.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4867 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/tests/test_browser_utils.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2080 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/tests/test_browser_workflow.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    35237 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/tests/test_model.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    20521 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/tests/test_security.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2708 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/tests/test_testing.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4879 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/tests/test_ugm.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4206 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/tests/test_utils.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4595 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/tests/test_workflow.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3186 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/ugm.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2091 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/utils.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4007 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone/app/workflow.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-02-12 10:05:31.572425 cone.app-1.1a2/src/cone.app.egg-info/
--rw-r--r--   0 rnix      (1000) rnix      (1000)    36429 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone.app.egg-info/PKG-INFO
--rw-r--r--   0 rnix      (1000) rnix      (1000)     7456 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone.app.egg-info/SOURCES.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone.app.egg-info/dependency_links.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      120 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone.app.egg-info/entry_points.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        5 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone.app.egg-info/namespace_packages.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone.app.egg-info/not-zip-safe
--rw-r--r--   0 rnix      (1000) rnix      (1000)      342 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone.app.egg-info/requires.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        5 2024-02-12 10:05:31.000000 cone.app-1.1a2/src/cone.app.egg-info/top_level.txt
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:45:55.777179 cone_app-1.1rc1/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    32910 2024-05-23 13:45:55.000000 cone_app-1.1rc1/CHANGES.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1378 2024-05-23 13:45:55.000000 cone_app-1.1rc1/LICENSE.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      138 2024-05-23 13:45:55.000000 cone_app-1.1rc1/MANIFEST.in
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    36750 2024-05-23 13:45:55.777179 cone_app-1.1rc1/PKG-INFO
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1179 2024-05-23 13:45:55.000000 cone_app-1.1rc1/README.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2829 2024-05-23 13:45:55.000000 cone_app-1.1rc1/TODO.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       74 2024-05-23 13:45:55.777179 cone_app-1.1rc1/setup.cfg
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2154 2024-05-23 13:45:55.000000 cone_app-1.1rc1/setup.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:45:55.757179 cone_app-1.1rc1/src/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:45:55.757179 cone_app-1.1rc1/src/cone/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       56 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/__init__.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:45:55.761179 cone_app-1.1rc1/src/cone/app/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    12495 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/__init__.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:45:55.761179 cone_app-1.1rc1/src/cone/app/browser/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3025 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/__init__.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    17063 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/actions.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    12016 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/ajax.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    18962 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/authoring.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    15277 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/batch.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3889 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/content.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     8741 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/contents.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     5143 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/contextmenu.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     5563 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/copysupport.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3006 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/exception.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     6293 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/form.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    16540 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/layout.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3223 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/login.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2440 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/order.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    15050 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/referencebrowser.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    11679 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/resources.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     6175 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/settings.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     7325 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/sharing.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:45:55.757179 cone_app-1.1rc1/src/cone/app/browser/static/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:45:55.757179 cone_app-1.1rc1/src/cone/app/browser/static/bootstrap/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:45:55.765179 cone_app-1.1rc1/src/cone/app/browser/static/bootstrap/css/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    25682 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/static/bootstrap/css/bootstrap-theme.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    48005 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/static/bootstrap/css/bootstrap-theme.css.map
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    23411 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/static/bootstrap/css/bootstrap-theme.min.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    75600 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/static/bootstrap/css/bootstrap-theme.min.css.map
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   145933 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/static/bootstrap/css/bootstrap.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   390887 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/static/bootstrap/css/bootstrap.css.map
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   121457 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/static/bootstrap/css/bootstrap.min.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   540434 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/static/bootstrap/css/bootstrap.min.css.map
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:45:55.765179 cone_app-1.1rc1/src/cone/app/browser/static/bootstrap/fonts/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    20127 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/static/bootstrap/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   108738 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/static/bootstrap/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    45404 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/static/bootstrap/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    23424 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/static/bootstrap/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    18028 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/static/bootstrap/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:45:55.765179 cone_app-1.1rc1/src/cone/app/browser/static/bootstrap/js/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    75484 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/static/bootstrap/js/bootstrap.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    39680 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/static/bootstrap/js/bootstrap.min.js
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:45:55.765179 cone_app-1.1rc1/src/cone/app/browser/static/cone/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     5591 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/static/cone/cone.app.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4446 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/static/cone/cone.app.min.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       67 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/static/cone/cone.app.print.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    23862 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/static/cone/cone.app.protected.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    11129 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/static/cone/cone.app.protected.min.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2128 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/static/cone/cone.app.public.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1111 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/static/cone/cone.app.public.min.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1406 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/static/cone/favicon.ico
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:45:55.765179 cone_app-1.1rc1/src/cone/app/browser/static/ionicons/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       31 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/static/ionicons/.gitignore
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:45:55.765179 cone_app-1.1rc1/src/cone/app/browser/static/ionicons/css/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    47987 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/static/ionicons/css/ionicons.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    42998 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/static/ionicons/css/ionicons.min.css
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:45:55.765179 cone_app-1.1rc1/src/cone/app/browser/static/ionicons/fonts/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   101984 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/static/ionicons/fonts/ionicons.eot
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   286345 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/static/ionicons/fonts/ionicons.svg
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   164548 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/static/ionicons/fonts/ionicons.ttf
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    57276 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/static/ionicons/fonts/ionicons.woff
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:45:55.765179 cone_app-1.1rc1/src/cone/app/browser/static/jquery/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   288580 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/static/jquery/jquery-3.6.0.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    89501 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/static/jquery/jquery-3.6.0.min.js
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:45:55.765179 cone_app-1.1rc1/src/cone/app/browser/static/typeahead/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    71417 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/static/typeahead/typeahead.bundle.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     6240 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/static/typeahead/typeahead.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     7236 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/table.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:45:55.769179 cone_app-1.1rc1/src/cone/app/browser/templates/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      912 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/templates/action_dropdown.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      842 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/templates/add_dropdown.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4359 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/templates/batch.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      713 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/templates/batched_items.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1043 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/templates/batched_items_footer.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2568 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/templates/batched_items_header.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1577 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/templates/button_action.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      697 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/templates/byline.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      627 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/templates/content_form.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      548 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/templates/contextmenu.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      682 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/templates/contextmenu_dropdown.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       23 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/templates/default_root.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      324 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/templates/footer.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      402 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/templates/insufficient_privileges.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      830 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/templates/language.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2280 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/templates/layout.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2603 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/templates/link_action.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      223 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/templates/listing.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      846 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/templates/livesearch.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      417 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/templates/logo.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      647 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/templates/main.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2476 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/templates/mainmenu.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      558 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/templates/navtree.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      976 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/templates/navtree_recue.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      363 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/templates/not_found.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1030 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/templates/pathbar.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      524 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/templates/personaltools.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      424 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/templates/referencebrowser.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      898 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/templates/referencebrowser_pathbar.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      253 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/templates/resources.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1133 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/templates/settings.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      315 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/templates/settings_form.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1332 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/templates/settings_sidebar.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      220 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/templates/sharing.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     7517 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/templates/table.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      377 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/templates/unauthorized.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1435 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/templates/wf_dropdown.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4160 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/translation.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3617 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/utils.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2574 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/browser/workflow.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      715 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/compat.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      140 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/configure.zcml
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     6452 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/interfaces.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:45:55.769179 cone_app-1.1rc1/src/cone/app/locale/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    11048 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/locale/cone.app.pot
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:45:55.757179 cone_app-1.1rc1/src/cone/app/locale/de/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:45:55.769179 cone_app-1.1rc1/src/cone/app/locale/de/LC_MESSAGES/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     5685 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/locale/de/LC_MESSAGES/cone.app.mo
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    12850 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/locale/de/LC_MESSAGES/cone.app.po
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:45:55.757179 cone_app-1.1rc1/src/cone/app/locale/en/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:45:55.769179 cone_app-1.1rc1/src/cone/app/locale/en/LC_MESSAGES/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     5179 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/locale/en/LC_MESSAGES/cone.app.mo
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    12336 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/locale/en/LC_MESSAGES/cone.app.po
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    22050 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/model.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     9249 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/security.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:45:55.769179 cone_app-1.1rc1/src/cone/app/testing/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     7332 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/testing/__init__.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:45:55.757179 cone_app-1.1rc1/src/cone/app/testing/data/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:45:55.773179 cone_app-1.1rc1/src/cone/app/testing/data/ugm/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       11 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/testing/data/ugm/groups
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       81 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/testing/data/ugm/roles
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:45:55.757179 cone_app-1.1rc1/src/cone/app/testing/data/ugm/userdata/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:45:55.773179 cone_app-1.1rc1/src/cone/app/testing/data/ugm/userdata/groups/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       50 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/testing/data/ugm/userdata/groups/group1
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:45:55.773179 cone_app-1.1rc1/src/cone/app/testing/data/ugm/userdata/users/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       40 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/testing/data/ugm/userdata/users/admin
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       42 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/testing/data/ugm/userdata/users/editor
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       44 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/testing/data/ugm/userdata/users/manager
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       42 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/testing/data/ugm/userdata/users/max
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       44 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/testing/data/ugm/userdata/users/sepp
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       42 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/testing/data/ugm/userdata/users/viewer
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      379 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/testing/data/ugm/users
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       36 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/testing/dummy_action.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      126 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/testing/dummy_batched_items.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      393 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/testing/dummy_form.yaml
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      234 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/testing/dummy_main.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      956 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/testing/dummy_workflow.zcml
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3252 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/testing/mock.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:45:55.773179 cone_app-1.1rc1/src/cone/app/testing/static/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       26 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/testing/static/print1.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       26 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/testing/static/print2.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       23 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/testing/static/script1.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       23 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/testing/static/script2.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       27 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/testing/static/style1.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       27 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/testing/static/style2.css
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:45:55.773179 cone_app-1.1rc1/src/cone/app/tests/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3616 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/tests/__init__.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     8392 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/tests/test_app.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2977 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/tests/test_browser.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    31055 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/tests/test_browser_actions.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    18113 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/tests/test_browser_ajax.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    51471 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/tests/test_browser_authoring.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    33391 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/tests/test_browser_batch.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4380 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/tests/test_browser_content.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    14673 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/tests/test_browser_contents.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     5391 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/tests/test_browser_contextmenu.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     8429 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/tests/test_browser_copysupport.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     5885 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/tests/test_browser_exception.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    17324 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/tests/test_browser_form.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    27684 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/tests/test_browser_layout.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2203 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/tests/test_browser_login.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2458 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/tests/test_browser_order.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    41731 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/tests/test_browser_referencebrowser.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    16029 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/tests/test_browser_resources.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    12875 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/tests/test_browser_settings.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    10985 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/tests/test_browser_sharing.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     7869 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/tests/test_browser_table.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    11245 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/tests/test_browser_translation.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4867 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/tests/test_browser_utils.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2080 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/tests/test_browser_workflow.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    35382 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/tests/test_model.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    21595 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/tests/test_security.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2708 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/tests/test_testing.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4879 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/tests/test_ugm.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4206 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/tests/test_utils.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4595 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/tests/test_workflow.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3186 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/ugm.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2091 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/utils.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4007 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone/app/workflow.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:45:55.777179 cone_app-1.1rc1/src/cone.app.egg-info/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    36750 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone.app.egg-info/PKG-INFO
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     7456 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone.app.egg-info/SOURCES.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone.app.egg-info/dependency_links.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      120 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone.app.egg-info/entry_points.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        5 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone.app.egg-info/namespace_packages.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone.app.egg-info/not-zip-safe
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      342 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone.app.egg-info/requires.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        5 2024-05-23 13:45:55.000000 cone_app-1.1rc1/src/cone.app.egg-info/top_level.txt
```

### Comparing `cone.app-1.1a2/CHANGES.rst` & `cone_app-1.1rc1/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,25 @@
 Changes
 =======
 
+1.1rc1 (2024-05-23)
+-------------------
+
+- ``node_info`` decorator stores name on node info instance.
+  [rnix]
+
+- ``node_info`` decorator accepts additional keyword arguments to add custom
+  properties.
+  [rnix]
+
+- Add ``node_available`` callback to check whether node is allowed to be
+  used in application.
+  [rnix]
+
+
 1.1a2 (2024-02-12)
 ------------------
 
 - Introduce ``cone.app.browser.form.``,
   ``cone.app.browser.form.FormTarget``,
   ``cone.app.browser.form.AddFormTarget``,
   ``cone.app.browser.form.EditFormTarget``,
```

### Comparing `cone.app-1.1a2/LICENSE.rst` & `cone_app-1.1rc1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/PKG-INFO` & `cone_app-1.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cone.app
-Version: 1.1a2
+Version: 1.1rc1
 Summary: Web application stub
 Home-page: http://github.com/conestack/cone.app
 Author: Cone Contributors
 Author-email: dev@conestack.org
 License: Simplified BSD
 Keywords: node pyramid cone web
 Classifier: Environment :: Web Environment
@@ -87,14 +87,29 @@
 - Peter Holzer
 - Johannes Raggam
 
 
 Changes
 =======
 
+1.1rc1 (2024-05-23)
+-------------------
+
+- ``node_info`` decorator stores name on node info instance.
+  [rnix]
+
+- ``node_info`` decorator accepts additional keyword arguments to add custom
+  properties.
+  [rnix]
+
+- Add ``node_available`` callback to check whether node is allowed to be
+  used in application.
+  [rnix]
+
+
 1.1a2 (2024-02-12)
 ------------------
 
 - Introduce ``cone.app.browser.form.``,
   ``cone.app.browser.form.FormTarget``,
   ``cone.app.browser.form.AddFormTarget``,
   ``cone.app.browser.form.EditFormTarget``,
```

### Comparing `cone.app-1.1a2/README.rst` & `cone_app-1.1rc1/README.rst`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/TODO.rst` & `cone_app-1.1rc1/TODO.rst`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/setup.py` & `cone_app-1.1rc1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 def read_file(name):
     with open(os.path.join(os.path.dirname(__file__), name)) as f:
         return f.read()
 
 
-version = '1.1a2'
+version = '1.1rc1'
 shortdesc = 'Web application stub'
 longdesc = '\n\n'.join([read_file(name) for name in [
     'README.rst',
     'CHANGES.rst',
     'LICENSE.rst'
 ]])
```

### Comparing `cone.app-1.1a2/src/cone/app/__init__.py` & `cone_app-1.1rc1/src/cone/app/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,14 +211,19 @@
     """Returns WSGI application.
     """
     # set authentication related application properties
     security.ADMIN_USER = settings.get('cone.admin_user')
     security.ADMIN_PASSWORD = settings.get('cone.admin_password')
     security.AUTHENTICATOR = settings.get('cone.authenticator')
 
+    # set node availability callback
+    node_available_callback = settings.pop('cone.root.node_available', None)
+    if node_available_callback:
+        security.node_available = import_from_string(node_available_callback)
+
     auth_secret = settings.pop('cone.auth_secret', 'secret')
     auth_cookie_name = settings.pop('cone.auth_cookie_name', 'auth_tkt')
     auth_secure = settings.pop('cone.auth_secure', False)
     auth_include_ip = settings.pop('cone.auth_include_ip', False)
     auth_timeout = settings.pop('cone.auth_timeout', None)
     auth_reissue_time = settings.pop('cone.auth_reissue_time', None)
     if auth_reissue_time is not None:
```

### Comparing `cone.app-1.1a2/src/cone/app/browser/__init__.py` & `cone_app-1.1rc1/src/cone/app/browser/__init__.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/actions.py` & `cone_app-1.1rc1/src/cone/app/browser/actions.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/ajax.py` & `cone_app-1.1rc1/src/cone/app/browser/ajax.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/authoring.py` & `cone_app-1.1rc1/src/cone/app/browser/authoring.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 from cone.app import compat
+from cone.app import security
 from cone.app.browser import render_main_template
 from cone.app.browser.actions import ActionContext
-from cone.app.browser.ajax import AjaxEvent
-from cone.app.browser.ajax import AjaxOverlay
-from cone.app.browser.ajax import AjaxPath
 from cone.app.browser.ajax import ajax_continue
 from cone.app.browser.ajax import ajax_form_fiddle
 from cone.app.browser.ajax import ajax_message
+from cone.app.browser.ajax import AjaxEvent
+from cone.app.browser.ajax import AjaxOverlay
+from cone.app.browser.ajax import AjaxPath
 from cone.app.browser.ajax import render_ajax_form
 from cone.app.browser.form import FormTarget
 from cone.app.browser.utils import make_query
 from cone.app.browser.utils import make_url
 from cone.app.model import AdapterNode
 from cone.app.model import BaseNode
-from cone.app.model import Properties
 from cone.app.model import get_node_info
+from cone.app.model import Properties
 from cone.app.utils import app_config
 from cone.app.utils import node_path
-from cone.tile import Tile
 from cone.tile import render_template
 from cone.tile import render_tile
+from cone.tile import Tile
 from cone.tile import tile
 from plumber import Behavior
 from plumber import default
 from plumber import override
 from plumber import plumb
-from pyramid.i18n import TranslationStringFactory
 from pyramid.i18n import get_localizer
+from pyramid.i18n import TranslationStringFactory
 from pyramid.view import view_config
 from webob.exc import HTTPFound
 from yafowil.base import factory
 import logging
 import warnings
 
 
@@ -330,15 +331,15 @@
     def items(self):
         ret = list()
         addables = self.model.nodeinfo.addables
         if not addables:
             return ret
         for addable in addables:
             info = get_node_info(addable)
-            if not info:
+            if not info or not security.node_available(self.model, addable):
                 continue
             ret.append(self.make_item(addable, info))
         return ret
 
 
 @view_config(name='add', permission='add')
 def add(model, request):
@@ -365,16 +366,16 @@
             factory = default_addmodel_factory
         addmodel = factory(self.model, nodeinfo)
         return render_tile(addmodel, self.request, self.form_tile_name)
 
     @property
     def info(self):
         factory = self.request.params.get('factory')
-        allowed = self.model.nodeinfo.addables
-        if not factory or not allowed or factory not in allowed:
+        addables = self.model.nodeinfo.addables
+        if not factory or not addables or factory not in addables:
             return None
         return get_node_info(factory)
 
 
 class AddFactoryProxy(Behavior):
     """Form behavior for add forms hooking the hidden field 'factory' to
     request parameters.
```

### Comparing `cone.app-1.1a2/src/cone/app/browser/batch.py` & `cone_app-1.1rc1/src/cone/app/browser/batch.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/content.py` & `cone_app-1.1rc1/src/cone/app/browser/content.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/contents.py` & `cone_app-1.1rc1/src/cone/app/browser/contents.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/contextmenu.py` & `cone_app-1.1rc1/src/cone/app/browser/contextmenu.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/copysupport.py` & `cone_app-1.1rc1/src/cone/app/browser/copysupport.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/exception.py` & `cone_app-1.1rc1/src/cone/app/browser/exception.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/form.py` & `cone_app-1.1rc1/src/cone/app/browser/form.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/layout.py` & `cone_app-1.1rc1/src/cone/app/browser/layout.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/login.py` & `cone_app-1.1rc1/src/cone/app/browser/login.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/order.py` & `cone_app-1.1rc1/src/cone/app/browser/order.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/referencebrowser.py` & `cone_app-1.1rc1/src/cone/app/browser/referencebrowser.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/resources.py` & `cone_app-1.1rc1/src/cone/app/browser/resources.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/settings.py` & `cone_app-1.1rc1/src/cone/app/browser/settings.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/sharing.py` & `cone_app-1.1rc1/src/cone/app/browser/sharing.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/static/bootstrap/css/bootstrap-theme.css` & `cone_app-1.1rc1/src/cone/app/browser/static/bootstrap/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/static/bootstrap/css/bootstrap-theme.css.map` & `cone_app-1.1rc1/src/cone/app/browser/static/bootstrap/css/bootstrap-theme.css.map`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/static/bootstrap/css/bootstrap-theme.min.css` & `cone_app-1.1rc1/src/cone/app/browser/static/bootstrap/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/static/bootstrap/css/bootstrap-theme.min.css.map` & `cone_app-1.1rc1/src/cone/app/browser/static/bootstrap/css/bootstrap-theme.min.css.map`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/static/bootstrap/css/bootstrap.css` & `cone_app-1.1rc1/src/cone/app/browser/static/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/static/bootstrap/css/bootstrap.css.map` & `cone_app-1.1rc1/src/cone/app/browser/static/bootstrap/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/static/bootstrap/css/bootstrap.min.css` & `cone_app-1.1rc1/src/cone/app/browser/static/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/static/bootstrap/css/bootstrap.min.css.map` & `cone_app-1.1rc1/src/cone/app/browser/static/bootstrap/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/static/bootstrap/fonts/glyphicons-halflings-regular.eot` & `cone_app-1.1rc1/src/cone/app/browser/static/bootstrap/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/static/bootstrap/fonts/glyphicons-halflings-regular.svg` & `cone_app-1.1rc1/src/cone/app/browser/static/bootstrap/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/static/bootstrap/fonts/glyphicons-halflings-regular.ttf` & `cone_app-1.1rc1/src/cone/app/browser/static/bootstrap/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/static/bootstrap/fonts/glyphicons-halflings-regular.woff` & `cone_app-1.1rc1/src/cone/app/browser/static/bootstrap/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/static/bootstrap/fonts/glyphicons-halflings-regular.woff2` & `cone_app-1.1rc1/src/cone/app/browser/static/bootstrap/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/static/bootstrap/js/bootstrap.js` & `cone_app-1.1rc1/src/cone/app/browser/static/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/static/bootstrap/js/bootstrap.min.js` & `cone_app-1.1rc1/src/cone/app/browser/static/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/static/cone/cone.app.css` & `cone_app-1.1rc1/src/cone/app/browser/static/cone/cone.app.css`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/static/cone/cone.app.min.css` & `cone_app-1.1rc1/src/cone/app/browser/static/cone/cone.app.min.css`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/static/cone/cone.app.protected.js` & `cone_app-1.1rc1/src/cone/app/browser/static/cone/cone.app.protected.js`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/static/cone/cone.app.protected.min.js` & `cone_app-1.1rc1/src/cone/app/browser/static/cone/cone.app.protected.min.js`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/static/cone/cone.app.public.js` & `cone_app-1.1rc1/src/cone/app/browser/static/cone/cone.app.public.js`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/static/cone/cone.app.public.min.js` & `cone_app-1.1rc1/src/cone/app/browser/static/cone/cone.app.public.min.js`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/static/cone/favicon.ico` & `cone_app-1.1rc1/src/cone/app/browser/static/cone/favicon.ico`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/static/ionicons/css/ionicons.css` & `cone_app-1.1rc1/src/cone/app/browser/static/ionicons/css/ionicons.css`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/static/ionicons/css/ionicons.min.css` & `cone_app-1.1rc1/src/cone/app/browser/static/ionicons/css/ionicons.min.css`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/static/ionicons/fonts/ionicons.eot` & `cone_app-1.1rc1/src/cone/app/browser/static/ionicons/fonts/ionicons.eot`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/static/ionicons/fonts/ionicons.svg` & `cone_app-1.1rc1/src/cone/app/browser/static/ionicons/fonts/ionicons.svg`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/static/ionicons/fonts/ionicons.ttf` & `cone_app-1.1rc1/src/cone/app/browser/static/ionicons/fonts/ionicons.ttf`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/static/ionicons/fonts/ionicons.woff` & `cone_app-1.1rc1/src/cone/app/browser/static/ionicons/fonts/ionicons.woff`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/static/jquery/jquery-3.6.0.js` & `cone_app-1.1rc1/src/cone/app/browser/static/jquery/jquery-3.6.0.js`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/static/jquery/jquery-3.6.0.min.js` & `cone_app-1.1rc1/src/cone/app/browser/static/jquery/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/static/typeahead/typeahead.bundle.js` & `cone_app-1.1rc1/src/cone/app/browser/static/typeahead/typeahead.bundle.js`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/static/typeahead/typeahead.css` & `cone_app-1.1rc1/src/cone/app/browser/static/typeahead/typeahead.css`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/table.py` & `cone_app-1.1rc1/src/cone/app/browser/table.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/templates/action_dropdown.pt` & `cone_app-1.1rc1/src/cone/app/browser/templates/action_dropdown.pt`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/templates/add_dropdown.pt` & `cone_app-1.1rc1/src/cone/app/browser/templates/add_dropdown.pt`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/templates/batch.pt` & `cone_app-1.1rc1/src/cone/app/browser/templates/batch.pt`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/templates/batched_items.pt` & `cone_app-1.1rc1/src/cone/app/browser/templates/batched_items.pt`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/templates/batched_items_footer.pt` & `cone_app-1.1rc1/src/cone/app/browser/templates/batched_items_footer.pt`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/templates/batched_items_header.pt` & `cone_app-1.1rc1/src/cone/app/browser/templates/batched_items_header.pt`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/templates/button_action.pt` & `cone_app-1.1rc1/src/cone/app/browser/templates/button_action.pt`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/templates/byline.pt` & `cone_app-1.1rc1/src/cone/app/browser/templates/byline.pt`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/templates/content_form.pt` & `cone_app-1.1rc1/src/cone/app/browser/templates/content_form.pt`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/templates/contextmenu.pt` & `cone_app-1.1rc1/src/cone/app/browser/templates/contextmenu.pt`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/templates/contextmenu_dropdown.pt` & `cone_app-1.1rc1/src/cone/app/browser/templates/contextmenu_dropdown.pt`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/templates/language.pt` & `cone_app-1.1rc1/src/cone/app/browser/templates/language.pt`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/templates/layout.pt` & `cone_app-1.1rc1/src/cone/app/browser/templates/layout.pt`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/templates/link_action.pt` & `cone_app-1.1rc1/src/cone/app/browser/templates/link_action.pt`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/templates/livesearch.pt` & `cone_app-1.1rc1/src/cone/app/browser/templates/livesearch.pt`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/templates/main.pt` & `cone_app-1.1rc1/src/cone/app/browser/templates/main.pt`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/templates/mainmenu.pt` & `cone_app-1.1rc1/src/cone/app/browser/templates/mainmenu.pt`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/templates/navtree.pt` & `cone_app-1.1rc1/src/cone/app/browser/templates/navtree.pt`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/templates/navtree_recue.pt` & `cone_app-1.1rc1/src/cone/app/browser/templates/navtree_recue.pt`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/templates/pathbar.pt` & `cone_app-1.1rc1/src/cone/app/browser/templates/pathbar.pt`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/templates/personaltools.pt` & `cone_app-1.1rc1/src/cone/app/browser/templates/personaltools.pt`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/templates/referencebrowser_pathbar.pt` & `cone_app-1.1rc1/src/cone/app/browser/templates/referencebrowser_pathbar.pt`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/templates/settings.pt` & `cone_app-1.1rc1/src/cone/app/browser/templates/settings.pt`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/templates/settings_sidebar.pt` & `cone_app-1.1rc1/src/cone/app/browser/templates/settings_sidebar.pt`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/templates/table.pt` & `cone_app-1.1rc1/src/cone/app/browser/templates/table.pt`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/templates/wf_dropdown.pt` & `cone_app-1.1rc1/src/cone/app/browser/templates/wf_dropdown.pt`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/translation.py` & `cone_app-1.1rc1/src/cone/app/browser/translation.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/utils.py` & `cone_app-1.1rc1/src/cone/app/browser/utils.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/browser/workflow.py` & `cone_app-1.1rc1/src/cone/app/browser/workflow.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/compat.py` & `cone_app-1.1rc1/src/cone/app/compat.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/interfaces.py` & `cone_app-1.1rc1/src/cone/app/interfaces.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/locale/cone.app.pot` & `cone_app-1.1rc1/src/cone/app/locale/cone.app.pot`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 #
 # SOME DESCRIPTIVE TITLE
 # This file is distributed under the same license as the PACKAGE package.
-# FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
+# FIRST AUTHOR <EMAIL@ADDRESS>, 2024.
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE 1.0\n"
-"POT-Creation-Date: 2022-11-29 17:34+0100\n"
+"POT-Creation-Date: 2024-05-23 15:41+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Lingua 4.15.0\n"
 
 #. Default: No Title
-#: ./src/cone/app/model.py:153
+#: ./src/cone/app/model.py:161
 msgid "no_title"
 msgstr ""
 
 #. Default: Settings
-#: ./src/cone/app/model.py:247 ./src/cone/app/browser/layout.py:132
+#: ./src/cone/app/model.py:255 ./src/cone/app/browser/settings.py:43
+#: ./src/cone/app/browser/templates/settings_sidebar.pt:13
+#: ./src/cone/app/browser/templates/settings.pt:12
 msgid "settings"
 msgstr ""
 
 #. Default: Viewer
 #: ./src/cone/app/security.py:27
 msgid "role_viewer"
 msgstr ""
@@ -43,87 +45,87 @@
 
 #. Default: Manager
 #: ./src/cone/app/security.py:30
 msgid "role_manager"
 msgstr ""
 
 #. Default: Actions
-#: ./src/cone/app/browser/contents.py:119
+#: ./src/cone/app/browser/contents.py:120
 #: ./src/cone/app/browser/contextmenu.py:141
 msgid "actions"
 msgstr ""
 
 #. Default: Title
-#: ./src/cone/app/browser/contents.py:125
+#: ./src/cone/app/browser/contents.py:126
 #: ./src/cone/app/browser/referencebrowser.py:222
 msgid "title"
 msgstr ""
 
 #. Default: Sort on title
-#: ./src/cone/app/browser/contents.py:127
+#: ./src/cone/app/browser/contents.py:128
 msgid "sort_on_title"
 msgstr ""
 
 #. Default: Creator
-#: ./src/cone/app/browser/contents.py:131
+#: ./src/cone/app/browser/contents.py:132
 msgid "creator"
 msgstr ""
 
 #. Default: Sort on creator
-#: ./src/cone/app/browser/contents.py:133
+#: ./src/cone/app/browser/contents.py:134
 msgid "sort_on_creator"
 msgstr ""
 
 #. Default: Created
-#: ./src/cone/app/browser/contents.py:137
+#: ./src/cone/app/browser/contents.py:138
 msgid "created"
 msgstr ""
 
 #. Default: Sort on created
-#: ./src/cone/app/browser/contents.py:139
+#: ./src/cone/app/browser/contents.py:140
 msgid "sort_on_created"
 msgstr ""
 
 #. Default: Modified
-#: ./src/cone/app/browser/contents.py:143
+#: ./src/cone/app/browser/contents.py:144
 msgid "modified"
 msgstr ""
 
 #. Default: Sort on modified
-#: ./src/cone/app/browser/contents.py:145
+#: ./src/cone/app/browser/contents.py:146
 msgid "sort_on_modified"
 msgstr ""
 
 #. Default: No username given
-#: ./src/cone/app/browser/login.py:63
+#: ./src/cone/app/browser/login.py:45
 msgid "no_username_given"
 msgstr ""
 
 #. Default: Username
-#: ./src/cone/app/browser/login.py:64
+#: ./src/cone/app/browser/login.py:46
 msgid "username"
 msgstr ""
 
 #. Default: No password given
-#: ./src/cone/app/browser/login.py:71
+#: ./src/cone/app/browser/login.py:53
 msgid "no_password_given"
 msgstr ""
 
 #. Default: Password
-#: ./src/cone/app/browser/login.py:72
+#: ./src/cone/app/browser/login.py:54
 msgid "password"
 msgstr ""
 
 #. Default: Login
-#: ./src/cone/app/browser/login.py:92
+#: ./src/cone/app/browser/login.py:74
 msgid "login"
 msgstr ""
 
 #. Default: Invalid Credentials
-#: ./src/cone/app/browser/login.py:107
+#: ./src/cone/app/browser/login.py:88
 msgid "invalid_credentials"
 msgstr ""
 
 #. Default: Principal
 #: ./src/cone/app/browser/sharing.py:53
 msgid "principal"
 msgstr ""
@@ -182,15 +184,15 @@
 
 #. Default: Pasting of ${count} items failed
 #: ./src/cone/app/browser/copysupport.py:135
 msgid "pasting_items_failed"
 msgstr ""
 
 #. Default: Unknown
-#: ./src/cone/app/browser/utils.py:81
+#: ./src/cone/app/browser/utils.py:82
 msgid "unknown"
 msgstr ""
 
 #. Default: Add reference
 #: ./src/cone/app/browser/referencebrowser.py:148
 msgid "add_reference"
 msgstr ""
@@ -206,161 +208,156 @@
 msgstr ""
 
 #. Default: Browse
 #: ./src/cone/app/browser/referencebrowser.py:342
 msgid "browse"
 msgstr ""
 
-#. Default: Error
-#: ./src/cone/app/browser/settings.py:29
-msgid "error"
-msgstr ""
-
 #. Default: One level up
-#: ./src/cone/app/browser/actions.py:231
+#: ./src/cone/app/browser/actions.py:268
 msgid "action_one_level_up"
 msgstr ""
 
 #. Default: View
-#: ./src/cone/app/browser/actions.py:266
+#: ./src/cone/app/browser/actions.py:303
 msgid "action_view"
 msgstr ""
 
 #. Default: Listing
-#: ./src/cone/app/browser/actions.py:312
+#: ./src/cone/app/browser/actions.py:349
 msgid "action_listing"
 msgstr ""
 
 #. Default: Sharing
-#: ./src/cone/app/browser/actions.py:334
+#: ./src/cone/app/browser/actions.py:371
 msgid "action_sharing"
 msgstr ""
 
 #. Default: Edit
-#: ./src/cone/app/browser/actions.py:378
+#: ./src/cone/app/browser/actions.py:415
 msgid "action_edit"
 msgstr ""
 
 #. Default: Do you really want to delete this Item?
-#: ./src/cone/app/browser/actions.py:399
+#: ./src/cone/app/browser/actions.py:436
 msgid "delete_item_confirm"
 msgstr ""
 
 #. Default: Delete
-#: ./src/cone/app/browser/actions.py:401
+#: ./src/cone/app/browser/actions.py:438
 msgid "action_delete"
 msgstr ""
 
 #. Default: Do you really want to delete selected Items?
-#: ./src/cone/app/browser/actions.py:420
+#: ./src/cone/app/browser/actions.py:457
 msgid "delete_items_confirm"
 msgstr ""
 
 #. Default: Delete selected children
-#: ./src/cone/app/browser/actions.py:422
+#: ./src/cone/app/browser/actions.py:459
 msgid "action_delete_selected_children"
 msgstr ""
 
 #. Default: Cut
-#: ./src/cone/app/browser/actions.py:440
+#: ./src/cone/app/browser/actions.py:477
 msgid "action_cut"
 msgstr ""
 
 #. Default: Copy
-#: ./src/cone/app/browser/actions.py:456
+#: ./src/cone/app/browser/actions.py:493
 msgid "action_copy"
 msgstr ""
 
 #. Default: Paste
-#: ./src/cone/app/browser/actions.py:472
+#: ./src/cone/app/browser/actions.py:509
 msgid "action_paste"
 msgstr ""
 
 #. Default: Move up
-#: ./src/cone/app/browser/actions.py:517
+#: ./src/cone/app/browser/actions.py:554
 msgid "move_up"
 msgstr ""
 
 #. Default: Move down
-#: ./src/cone/app/browser/actions.py:532
+#: ./src/cone/app/browser/actions.py:569
 msgid "move_down"
 msgstr ""
 
 #. Default: Logout
-#: ./src/cone/app/browser/layout.py:162
+#: ./src/cone/app/browser/layout.py:132
 msgid "logout"
 msgstr ""
 
 #. Default: Navigation
-#: ./src/cone/app/browser/layout.py:356
+#: ./src/cone/app/browser/layout.py:321
 msgid "navigation"
 msgstr ""
 
 #. Default: English
-#: ./src/cone/app/browser/layout.py:507
+#: ./src/cone/app/browser/layout.py:479
 msgid "lang_en"
 msgstr ""
 
 #. Default: German
-#: ./src/cone/app/browser/layout.py:508
+#: ./src/cone/app/browser/layout.py:480
 msgid "lang_de"
 msgstr ""
 
 #. Default: French
-#: ./src/cone/app/browser/layout.py:509
+#: ./src/cone/app/browser/layout.py:481
 msgid "lang_fr"
 msgstr ""
 
 #. Default: Italian
-#: ./src/cone/app/browser/layout.py:510
+#: ./src/cone/app/browser/layout.py:482
 msgid "lang_it"
 msgstr ""
 
 #. Default: Object "${title}" not movable
 #: ./src/cone/app/browser/order.py:35
 msgid "object_not_movable"
 msgstr ""
 
 #. Default: You are not permitted to move this object
 #: ./src/cone/app/browser/order.py:46
 msgid "object_moving_not_permitted"
 msgstr ""
 
 #. Default: Content Form Heading
-#: ./src/cone/app/browser/authoring.py:201
+#: ./src/cone/app/browser/authoring.py:216
 msgid "content_form_heading"
 msgstr ""
 
 #. Default: Unknown factory
-#: ./src/cone/app/browser/authoring.py:340
+#: ./src/cone/app/browser/authoring.py:363
 msgid "unknown_factory"
 msgstr ""
 
 #. Default: Add: ${title}
-#: ./src/cone/app/browser/authoring.py:381
+#: ./src/cone/app/browser/authoring.py:403
 msgid "add_form_heading"
 msgstr ""
 
 #. Default: Edit
-#: ./src/cone/app/browser/authoring.py:449
+#: ./src/cone/app/browser/authoring.py:479
 msgid "edit"
 msgstr ""
 
 #. Default: Edit: ${title}
-#: ./src/cone/app/browser/authoring.py:452
+#: ./src/cone/app/browser/authoring.py:482
 msgid "edit_form_heading"
 msgstr ""
 
 #. Default: Object "${title}" not deletable
-#: ./src/cone/app/browser/authoring.py:507
+#: ./src/cone/app/browser/authoring.py:546
 msgid "object_not_deletable"
 msgstr ""
 
 #. Default: Deleted: ${title}
-#: ./src/cone/app/browser/authoring.py:525
+#: ./src/cone/app/browser/authoring.py:564
 msgid "deleted_object"
 msgstr ""
 
 #. Default: You are here
 #: ./src/cone/app/browser/templates/pathbar.pt:13
 msgid "you_are_here"
 msgstr ""
```

### Comparing `cone.app-1.1a2/src/cone/app/locale/de/LC_MESSAGES/cone.app.mo` & `cone_app-1.1rc1/src/cone/app/locale/de/LC_MESSAGES/cone.app.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -110,17 +110,14 @@
 
 msgid "edit_form_heading"
 msgstr "Editieren: ${title}"
 
 msgid "entries"
 msgstr "Einträge"
 
-msgid "error"
-msgstr "Fehler"
-
 msgid "first"
 msgstr "Anfang"
 
 msgid "insufficient_privileges"
 msgstr "Unzureichende Berechtigung"
 
 msgid "insufficient_privileges_help"
```

### Comparing `cone.app-1.1a2/src/cone/app/locale/de/LC_MESSAGES/cone.app.po` & `cone_app-1.1rc1/src/cone/app/locale/de/LC_MESSAGES/cone.app.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,32 +3,34 @@
 # This file is distributed under the same license as the cone.app project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2012.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: cone.app 0.9.3dev\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2022-11-29 17:34+0100\n"
+"POT-Creation-Date: 2024-05-23 15:41+0200\n"
 "PO-Revision-Date: 2012-04-25 13:00+0200\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: de <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1)\n"
 "Generated-By: Babel 0.9.4\n"
 
 #. Default: No Title
-#: src/cone/app/model.py:153
+#: src/cone/app/model.py:161
 msgid "no_title"
 msgstr "Kein Titel"
 
 #. Default: Settings
-#: src/cone/app/model.py:247 src/cone/app/browser/layout.py:132
+#: src/cone/app/model.py:255 src/cone/app/browser/settings.py:43
+#: src/cone/app/browser/templates/settings_sidebar.pt:13
+#: src/cone/app/browser/templates/settings.pt:12
 msgid "settings"
 msgstr "Einstellungen"
 
 #. Default: Viewer
 #: src/cone/app/security.py:27
 msgid "role_viewer"
 msgstr "Betrachter"
@@ -45,86 +47,86 @@
 
 #. Default: Manager
 #: src/cone/app/security.py:30
 msgid "role_manager"
 msgstr "Superuser"
 
 #. Default: Actions
-#: src/cone/app/browser/contents.py:119 src/cone/app/browser/contextmenu.py:141
+#: src/cone/app/browser/contents.py:120 src/cone/app/browser/contextmenu.py:141
 msgid "actions"
 msgstr "Aktionen"
 
 #. Default: Title
-#: src/cone/app/browser/contents.py:125
+#: src/cone/app/browser/contents.py:126
 #: src/cone/app/browser/referencebrowser.py:222
 msgid "title"
 msgstr "Titel"
 
 #. Default: Sort on title
-#: src/cone/app/browser/contents.py:127
+#: src/cone/app/browser/contents.py:128
 msgid "sort_on_title"
 msgstr "Sortiere nach Titel"
 
 #. Default: Creator
-#: src/cone/app/browser/contents.py:131
+#: src/cone/app/browser/contents.py:132
 msgid "creator"
 msgstr "Ersteller"
 
 #. Default: Sort on creator
-#: src/cone/app/browser/contents.py:133
+#: src/cone/app/browser/contents.py:134
 msgid "sort_on_creator"
 msgstr "Sortiere nach Ersteller"
 
 #. Default: Created
-#: src/cone/app/browser/contents.py:137
+#: src/cone/app/browser/contents.py:138
 msgid "created"
 msgstr "Erstellt"
 
 #. Default: Sort on created
-#: src/cone/app/browser/contents.py:139
+#: src/cone/app/browser/contents.py:140
 msgid "sort_on_created"
 msgstr "Sortiere nach Erstellt"
 
 #. Default: Modified
-#: src/cone/app/browser/contents.py:143
+#: src/cone/app/browser/contents.py:144
 msgid "modified"
 msgstr "Geändert"
 
 #. Default: Sort on modified
-#: src/cone/app/browser/contents.py:145
+#: src/cone/app/browser/contents.py:146
 msgid "sort_on_modified"
 msgstr "Sortiere nach Geändert"
 
 #. Default: No username given
-#: src/cone/app/browser/login.py:63
+#: src/cone/app/browser/login.py:45
 msgid "no_username_given"
 msgstr "Kein Benutzername angegeben"
 
 #. Default: Username
-#: src/cone/app/browser/login.py:64
+#: src/cone/app/browser/login.py:46
 msgid "username"
 msgstr "Benutzername"
 
 #. Default: No password given
-#: src/cone/app/browser/login.py:71
+#: src/cone/app/browser/login.py:53
 msgid "no_password_given"
 msgstr "Kein Passwort angegeben"
 
 #. Default: Password
-#: src/cone/app/browser/login.py:72
+#: src/cone/app/browser/login.py:54
 msgid "password"
 msgstr "Passwort"
 
 #. Default: Login
-#: src/cone/app/browser/login.py:92
+#: src/cone/app/browser/login.py:74
 msgid "login"
 msgstr "Anmelden"
 
 #. Default: Invalid Credentials
-#: src/cone/app/browser/login.py:107
+#: src/cone/app/browser/login.py:88
 msgid "invalid_credentials"
 msgstr "Anmeldung fehlgeschlagen"
 
 #. Default: Principal
 #: src/cone/app/browser/sharing.py:53
 msgid "principal"
 msgstr "Benutzer/Gruppe"
@@ -183,15 +185,15 @@
 
 #. Default: Pasting of ${count} items failed
 #: src/cone/app/browser/copysupport.py:135
 msgid "pasting_items_failed"
 msgstr "${count} Objekte konnten nicht eingefügt werden"
 
 #. Default: Unknown
-#: src/cone/app/browser/utils.py:81
+#: src/cone/app/browser/utils.py:82
 msgid "unknown"
 msgstr "Unbekannt"
 
 #. Default: Add reference
 #: src/cone/app/browser/referencebrowser.py:148
 msgid "add_reference"
 msgstr "Referenz hinzufügen"
@@ -207,161 +209,156 @@
 msgstr "Aktionen"
 
 #. Default: Browse
 #: src/cone/app/browser/referencebrowser.py:342
 msgid "browse"
 msgstr "Durchsuchen"
 
-#. Default: Error
-#: src/cone/app/browser/settings.py:29
-msgid "error"
-msgstr "Fehler"
-
 #. Default: One level up
-#: src/cone/app/browser/actions.py:231
+#: src/cone/app/browser/actions.py:268
 msgid "action_one_level_up"
 msgstr "Eine Ebene höher"
 
 #. Default: View
-#: src/cone/app/browser/actions.py:266
+#: src/cone/app/browser/actions.py:303
 msgid "action_view"
 msgstr "Anzeigen"
 
 #. Default: Listing
-#: src/cone/app/browser/actions.py:312
+#: src/cone/app/browser/actions.py:349
 msgid "action_listing"
 msgstr "Liste"
 
 #. Default: Sharing
-#: src/cone/app/browser/actions.py:334
+#: src/cone/app/browser/actions.py:371
 msgid "action_sharing"
 msgstr "Freigabe"
 
 #. Default: Edit
-#: src/cone/app/browser/actions.py:378
+#: src/cone/app/browser/actions.py:415
 msgid "action_edit"
 msgstr "Editieren"
 
 #. Default: Do you really want to delete this Item?
-#: src/cone/app/browser/actions.py:399
+#: src/cone/app/browser/actions.py:436
 msgid "delete_item_confirm"
 msgstr "Wollen Sie dieses Objekt wirklich löschen?"
 
 #. Default: Delete
-#: src/cone/app/browser/actions.py:401
+#: src/cone/app/browser/actions.py:438
 msgid "action_delete"
 msgstr "Löschen"
 
 #. Default: Do you really want to delete selected Items?
-#: src/cone/app/browser/actions.py:420
+#: src/cone/app/browser/actions.py:457
 msgid "delete_items_confirm"
 msgstr "Wollen Sie die ausgewählten Objekte wirklich löschen?"
 
 #. Default: Delete selected children
-#: src/cone/app/browser/actions.py:422
+#: src/cone/app/browser/actions.py:459
 msgid "action_delete_selected_children"
 msgstr "Wollen Sie die ausgewählten Objekte wirklich löschen?"
 
 #. Default: Cut
-#: src/cone/app/browser/actions.py:440
+#: src/cone/app/browser/actions.py:477
 msgid "action_cut"
 msgstr "Ausschneiden"
 
 #. Default: Copy
-#: src/cone/app/browser/actions.py:456
+#: src/cone/app/browser/actions.py:493
 msgid "action_copy"
 msgstr "Kopieren"
 
 #. Default: Paste
-#: src/cone/app/browser/actions.py:472
+#: src/cone/app/browser/actions.py:509
 msgid "action_paste"
 msgstr "Einfügen"
 
 #. Default: Move up
-#: src/cone/app/browser/actions.py:517
+#: src/cone/app/browser/actions.py:554
 msgid "move_up"
 msgstr "Nach oben verschieben"
 
 #. Default: Move down
-#: src/cone/app/browser/actions.py:532
+#: src/cone/app/browser/actions.py:569
 msgid "move_down"
 msgstr "Nach unten verschieben"
 
 #. Default: Logout
-#: src/cone/app/browser/layout.py:162
+#: src/cone/app/browser/layout.py:132
 msgid "logout"
 msgstr "Abmelden"
 
 #. Default: Navigation
-#: src/cone/app/browser/layout.py:356
+#: src/cone/app/browser/layout.py:321
 msgid "navigation"
 msgstr "Navigation"
 
 #. Default: English
-#: src/cone/app/browser/layout.py:507
+#: src/cone/app/browser/layout.py:479
 msgid "lang_en"
 msgstr "Englisch"
 
 #. Default: German
-#: src/cone/app/browser/layout.py:508
+#: src/cone/app/browser/layout.py:480
 msgid "lang_de"
 msgstr "Deutsch"
 
 #. Default: French
-#: src/cone/app/browser/layout.py:509
+#: src/cone/app/browser/layout.py:481
 msgid "lang_fr"
 msgstr "Französisch"
 
 #. Default: Italian
-#: src/cone/app/browser/layout.py:510
+#: src/cone/app/browser/layout.py:482
 msgid "lang_it"
 msgstr "Italienisch"
 
 #. Default: Object "${title}" not movable
 #: src/cone/app/browser/order.py:35
 msgid "object_not_movable"
 msgstr "Objekt \"${title}\" kann nicht verschoben werden"
 
 #. Default: You are not permitted to move this object
 #: src/cone/app/browser/order.py:46
 msgid "object_moving_not_permitted"
 msgstr "Sie haben nicht die Berechtigung um dieses Objekt zu verschieben"
 
 #. Default: Content Form Heading
-#: src/cone/app/browser/authoring.py:201
+#: src/cone/app/browser/authoring.py:216
 msgid "content_form_heading"
 msgstr "Content Formular Überschrift"
 
 #. Default: Unknown factory
-#: src/cone/app/browser/authoring.py:340
+#: src/cone/app/browser/authoring.py:363
 msgid "unknown_factory"
 msgstr "Unbekannt"
 
 #. Default: Add: ${title}
-#: src/cone/app/browser/authoring.py:381
+#: src/cone/app/browser/authoring.py:403
 msgid "add_form_heading"
 msgstr "Hinzufügen: ${title}"
 
 #. Default: Edit
-#: src/cone/app/browser/authoring.py:449
+#: src/cone/app/browser/authoring.py:479
 msgid "edit"
 msgstr "Editieren"
 
 #. Default: Edit: ${title}
-#: src/cone/app/browser/authoring.py:452
+#: src/cone/app/browser/authoring.py:482
 msgid "edit_form_heading"
 msgstr "Editieren: ${title}"
 
 #. Default: Object "${title}" not deletable
-#: src/cone/app/browser/authoring.py:507
+#: src/cone/app/browser/authoring.py:546
 msgid "object_not_deletable"
 msgstr "Objekt \"${title}\" kann nicht gelöscht werden"
 
 #. Default: Deleted: ${title}
-#: src/cone/app/browser/authoring.py:525
+#: src/cone/app/browser/authoring.py:564
 msgid "deleted_object"
 msgstr "Gelöscht: ${title}"
 
 #. Default: You are here
 #: src/cone/app/browser/templates/pathbar.pt:13
 msgid "you_are_here"
 msgstr "Sie sind hier"
```

### Comparing `cone.app-1.1a2/src/cone/app/locale/en/LC_MESSAGES/cone.app.mo` & `cone_app-1.1rc1/src/cone/app/locale/en/LC_MESSAGES/cone.app.mo`

 * *Files 14% similar despite different names*

#### msgunfmt {}

```diff
@@ -110,17 +110,14 @@
 
 msgid "edit_form_heading"
 msgstr "Edit: ${title}"
 
 msgid "entries"
 msgstr "entries"
 
-msgid "error"
-msgstr "Error"
-
 msgid "first"
 msgstr "First"
 
 msgid "insufficient_privileges"
 msgstr "Insufficient privileges"
 
 msgid "insufficient_privileges_help"
```

### Comparing `cone.app-1.1a2/src/cone/app/locale/en/LC_MESSAGES/cone.app.po` & `cone_app-1.1rc1/src/cone/app/locale/en/LC_MESSAGES/cone.app.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,32 +3,34 @@
 # This file is distributed under the same license as the cone.app project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2012.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: cone.app 0.9.3dev\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2022-11-29 17:34+0100\n"
+"POT-Creation-Date: 2024-05-23 15:41+0200\n"
 "PO-Revision-Date: 2012-04-25 13:00+0200\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: en <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1)\n"
 "Generated-By: Babel 0.9.4\n"
 
 #. Default: No Title
-#: src/cone/app/model.py:153
+#: src/cone/app/model.py:161
 msgid "no_title"
 msgstr "No Title"
 
 #. Default: Settings
-#: src/cone/app/model.py:247 src/cone/app/browser/layout.py:132
+#: src/cone/app/model.py:255 src/cone/app/browser/settings.py:43
+#: src/cone/app/browser/templates/settings_sidebar.pt:13
+#: src/cone/app/browser/templates/settings.pt:12
 msgid "settings"
 msgstr "Settings"
 
 #. Default: Viewer
 #: src/cone/app/security.py:27
 msgid "role_viewer"
 msgstr "Viewer"
@@ -45,86 +47,86 @@
 
 #. Default: Manager
 #: src/cone/app/security.py:30
 msgid "role_manager"
 msgstr "Manager"
 
 #. Default: Actions
-#: src/cone/app/browser/contents.py:119 src/cone/app/browser/contextmenu.py:141
+#: src/cone/app/browser/contents.py:120 src/cone/app/browser/contextmenu.py:141
 msgid "actions"
 msgstr "Actions"
 
 #. Default: Title
-#: src/cone/app/browser/contents.py:125
+#: src/cone/app/browser/contents.py:126
 #: src/cone/app/browser/referencebrowser.py:222
 msgid "title"
 msgstr "Title"
 
 #. Default: Sort on title
-#: src/cone/app/browser/contents.py:127
+#: src/cone/app/browser/contents.py:128
 msgid "sort_on_title"
 msgstr "Sort on title"
 
 #. Default: Creator
-#: src/cone/app/browser/contents.py:131
+#: src/cone/app/browser/contents.py:132
 msgid "creator"
 msgstr "Creator"
 
 #. Default: Sort on creator
-#: src/cone/app/browser/contents.py:133
+#: src/cone/app/browser/contents.py:134
 msgid "sort_on_creator"
 msgstr "Sort on creator"
 
 #. Default: Created
-#: src/cone/app/browser/contents.py:137
+#: src/cone/app/browser/contents.py:138
 msgid "created"
 msgstr "Created"
 
 #. Default: Sort on created
-#: src/cone/app/browser/contents.py:139
+#: src/cone/app/browser/contents.py:140
 msgid "sort_on_created"
 msgstr "Sort on created"
 
 #. Default: Modified
-#: src/cone/app/browser/contents.py:143
+#: src/cone/app/browser/contents.py:144
 msgid "modified"
 msgstr "Modified"
 
 #. Default: Sort on modified
-#: src/cone/app/browser/contents.py:145
+#: src/cone/app/browser/contents.py:146
 msgid "sort_on_modified"
 msgstr "Sort on modified"
 
 #. Default: No username given
-#: src/cone/app/browser/login.py:63
+#: src/cone/app/browser/login.py:45
 msgid "no_username_given"
 msgstr "No username given"
 
 #. Default: Username
-#: src/cone/app/browser/login.py:64
+#: src/cone/app/browser/login.py:46
 msgid "username"
 msgstr "Username"
 
 #. Default: No password given
-#: src/cone/app/browser/login.py:71
+#: src/cone/app/browser/login.py:53
 msgid "no_password_given"
 msgstr "No password given"
 
 #. Default: Password
-#: src/cone/app/browser/login.py:72
+#: src/cone/app/browser/login.py:54
 msgid "password"
 msgstr "Password"
 
 #. Default: Login
-#: src/cone/app/browser/login.py:92
+#: src/cone/app/browser/login.py:74
 msgid "login"
 msgstr "Login"
 
 #. Default: Invalid Credentials
-#: src/cone/app/browser/login.py:107
+#: src/cone/app/browser/login.py:88
 msgid "invalid_credentials"
 msgstr "Invalid Credentials"
 
 #. Default: Principal
 #: src/cone/app/browser/sharing.py:53
 msgid "principal"
 msgstr "Principal"
@@ -183,15 +185,15 @@
 
 #. Default: Pasting of ${count} items failed
 #: src/cone/app/browser/copysupport.py:135
 msgid "pasting_items_failed"
 msgstr "Pasting of ${count} items failed"
 
 #. Default: Unknown
-#: src/cone/app/browser/utils.py:81
+#: src/cone/app/browser/utils.py:82
 msgid "unknown"
 msgstr "Unknown"
 
 #. Default: Add reference
 #: src/cone/app/browser/referencebrowser.py:148
 msgid "add_reference"
 msgstr "Add reference"
@@ -207,161 +209,156 @@
 msgstr "Actions"
 
 #. Default: Browse
 #: src/cone/app/browser/referencebrowser.py:342
 msgid "browse"
 msgstr "Browse"
 
-#. Default: Error
-#: src/cone/app/browser/settings.py:29
-msgid "error"
-msgstr "Error"
-
 #. Default: One level up
-#: src/cone/app/browser/actions.py:231
+#: src/cone/app/browser/actions.py:268
 msgid "action_one_level_up"
 msgstr "One level up"
 
 #. Default: View
-#: src/cone/app/browser/actions.py:266
+#: src/cone/app/browser/actions.py:303
 msgid "action_view"
 msgstr "View"
 
 #. Default: Listing
-#: src/cone/app/browser/actions.py:312
+#: src/cone/app/browser/actions.py:349
 msgid "action_listing"
 msgstr "Listing"
 
 #. Default: Sharing
-#: src/cone/app/browser/actions.py:334
+#: src/cone/app/browser/actions.py:371
 msgid "action_sharing"
 msgstr "Sharing"
 
 #. Default: Edit
-#: src/cone/app/browser/actions.py:378
+#: src/cone/app/browser/actions.py:415
 msgid "action_edit"
 msgstr "Edit"
 
 #. Default: Do you really want to delete this Item?
-#: src/cone/app/browser/actions.py:399
+#: src/cone/app/browser/actions.py:436
 msgid "delete_item_confirm"
 msgstr "Do you really want to delete this Item?"
 
 #. Default: Delete
-#: src/cone/app/browser/actions.py:401
+#: src/cone/app/browser/actions.py:438
 msgid "action_delete"
 msgstr "Delete"
 
 #. Default: Do you really want to delete selected Items?
-#: src/cone/app/browser/actions.py:420
+#: src/cone/app/browser/actions.py:457
 msgid "delete_items_confirm"
 msgstr "Do you really want to delete selected Items?"
 
 #. Default: Delete selected children
-#: src/cone/app/browser/actions.py:422
+#: src/cone/app/browser/actions.py:459
 msgid "action_delete_selected_children"
 msgstr "Delete selected children"
 
 #. Default: Cut
-#: src/cone/app/browser/actions.py:440
+#: src/cone/app/browser/actions.py:477
 msgid "action_cut"
 msgstr "Cut"
 
 #. Default: Copy
-#: src/cone/app/browser/actions.py:456
+#: src/cone/app/browser/actions.py:493
 msgid "action_copy"
 msgstr "Copy"
 
 #. Default: Paste
-#: src/cone/app/browser/actions.py:472
+#: src/cone/app/browser/actions.py:509
 msgid "action_paste"
 msgstr "Paste"
 
 #. Default: Move up
-#: src/cone/app/browser/actions.py:517
+#: src/cone/app/browser/actions.py:554
 msgid "move_up"
 msgstr "Move up"
 
 #. Default: Move down
-#: src/cone/app/browser/actions.py:532
+#: src/cone/app/browser/actions.py:569
 msgid "move_down"
 msgstr "Move down"
 
 #. Default: Logout
-#: src/cone/app/browser/layout.py:162
+#: src/cone/app/browser/layout.py:132
 msgid "logout"
 msgstr "Logout"
 
 #. Default: Navigation
-#: src/cone/app/browser/layout.py:356
+#: src/cone/app/browser/layout.py:321
 msgid "navigation"
 msgstr "Navigation"
 
 #. Default: English
-#: src/cone/app/browser/layout.py:507
+#: src/cone/app/browser/layout.py:479
 msgid "lang_en"
 msgstr "English"
 
 #. Default: German
-#: src/cone/app/browser/layout.py:508
+#: src/cone/app/browser/layout.py:480
 msgid "lang_de"
 msgstr "German"
 
 #. Default: French
-#: src/cone/app/browser/layout.py:509
+#: src/cone/app/browser/layout.py:481
 msgid "lang_fr"
 msgstr "French"
 
 #. Default: Italian
-#: src/cone/app/browser/layout.py:510
+#: src/cone/app/browser/layout.py:482
 msgid "lang_it"
 msgstr "Italian"
 
 #. Default: Object "${title}" not movable
 #: src/cone/app/browser/order.py:35
 msgid "object_not_movable"
 msgstr "Object \"${title}\" not movable"
 
 #. Default: You are not permitted to move this object
 #: src/cone/app/browser/order.py:46
 msgid "object_moving_not_permitted"
 msgstr "You are not permitted to move this object"
 
 #. Default: Content Form Heading
-#: src/cone/app/browser/authoring.py:201
+#: src/cone/app/browser/authoring.py:216
 msgid "content_form_heading"
 msgstr "Content Form Heading"
 
 #. Default: Unknown factory
-#: src/cone/app/browser/authoring.py:340
+#: src/cone/app/browser/authoring.py:363
 msgid "unknown_factory"
 msgstr "Unknown factory"
 
 #. Default: Add: ${title}
-#: src/cone/app/browser/authoring.py:381
+#: src/cone/app/browser/authoring.py:403
 msgid "add_form_heading"
 msgstr "Add: ${title}"
 
 #. Default: Edit
-#: src/cone/app/browser/authoring.py:449
+#: src/cone/app/browser/authoring.py:479
 msgid "edit"
 msgstr "Edit"
 
 #. Default: Edit: ${title}
-#: src/cone/app/browser/authoring.py:452
+#: src/cone/app/browser/authoring.py:482
 msgid "edit_form_heading"
 msgstr "Edit: ${title}"
 
 #. Default: Object "${title}" not deletable
-#: src/cone/app/browser/authoring.py:507
+#: src/cone/app/browser/authoring.py:546
 msgid "object_not_deletable"
 msgstr "Object \"${title}\" not deletable"
 
 #. Default: Deleted: ${title}
-#: src/cone/app/browser/authoring.py:525
+#: src/cone/app/browser/authoring.py:564
 msgid "deleted_object"
 msgstr "Deleted: ${title}"
 
 #. Default: You are here
 #: src/cone/app/browser/templates/pathbar.pt:13
 msgid "you_are_here"
 msgstr "You are here"
```

### Comparing `cone.app-1.1a2/src/cone/app/model.py` & `cone_app-1.1rc1/src/cone/app/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from cone.app import security
 from cone.app.compat import configparser
 from cone.app.compat import IS_PY2
 from cone.app.compat import ITER_TYPES
 from cone.app.interfaces import IAdapterNode
 from cone.app.interfaces import IApplicationEnvironment
 from cone.app.interfaces import IApplicationNode
 from cone.app.interfaces import ICopySupport
@@ -10,15 +11,14 @@
 from cone.app.interfaces import ILeafNode
 from cone.app.interfaces import IMetadata
 from cone.app.interfaces import INodeInfo
 from cone.app.interfaces import IProperties
 from cone.app.interfaces import ISettingsNode
 from cone.app.interfaces import ITranslation
 from cone.app.interfaces import IUUIDAsName
-from cone.app.security import acl_registry
 from cone.app.utils import app_config
 from cone.app.utils import DatetimeHelper
 from node import schema
 from node.behaviors import AsAttrAccess
 from node.behaviors import Attributes
 from node.behaviors import ChildFactory
 from node.behaviors import DefaultInit
@@ -89,35 +89,38 @@
 
 
 # B/C removed as of cone.app 1.1
 getNodeInfo = get_node_info
 
 
 class node_info(object):
-    """Node info decorator.
-    """
+    """Node info decorator."""
 
     def __init__(self, name, title=None, description=None,
-                 factory=None, icon=None, addables=[]):
+                 factory=None, icon=None, addables=[], **kw):
         self.name = name
         self.title = title
         self.description = description
         self.factory = factory
         self.icon = icon
         self.addables = addables
+        self.kw = kw
 
     def __call__(self, cls):
         cls.node_info_name = self.name
         info = NodeInfo()
+        info.name = self.name
         info.node = cls
         info.title = self.title
         info.description = self.description
         info.factory = self.factory
         info.addables = self.addables
         info.icon = self.icon
+        for name, value in self.kw.items():
+            setattr(info, name, value)
         register_node_info(cls.node_info_name, info)
         return cls
 
 
 @implementer(IApplicationEnvironment)
 class AppEnvironment(Behavior):
 
@@ -135,15 +138,17 @@
 @implementer(IApplicationNode)
 class AppNode(Behavior):
     node_info_name = default('')
 
     @default
     @property
     def __acl__(self):
-        return acl_registry.lookup(self.__class__, self.node_info_name)
+        if not security.node_available(self, self.node_info_name):
+            return [(Deny, Everyone, ALL_PERMISSIONS)]
+        return security.acl_registry.lookup(self.__class__, self.node_info_name)
 
     @default
     @instance_property
     def properties(self):
         props = Properties()
         props.in_navtree = False
         return props
```

### Comparing `cone.app-1.1a2/src/cone/app/security.py` & `cone_app-1.1rc1/src/cone/app/security.py`

 * *Files 6% similar despite different names*

```diff
@@ -187,14 +187,27 @@
     def lookup(self, obj=None, node_info_name='', default=DEFAULT_ACL):
         return self.get((obj, node_info_name), default)
 
 
 acl_registry = ACLRegistry()
 
 
+def default_node_available(model, node_info_name):
+    """Default callback for checking node availability in UI.
+
+    :param model: application node to gain access to the application model.
+    :param node_info_name: Node info name the node to check availability.
+    """
+    return True
+
+
+# callbak for application node availability
+node_available = default_node_available
+
+
 @implementer(IOwnerSupport)
 class OwnerSupport(Behavior):
     """Plumbing behavior providing ownership information.
     """
     owner_attribute_name = default('owner')
 
     @plumb
@@ -292,14 +305,16 @@
     """Plumbing behavior providing ACL from ``IACLAdapter``
     """
     default_acl = default(DEFAULT_ACL)
 
     @override
     @property
     def __acl__(self):
+        if not node_available(self, self.node_info_name):
+            return [(Deny, Everyone, ALL_PERMISSIONS)]
         request = get_current_request()
         acl_adapter = request.registry.queryAdapter(
             self,
             IACLAdapter,
             default=None
         )
         if acl_adapter:
```

### Comparing `cone.app-1.1a2/src/cone/app/testing/__init__.py` & `cone_app-1.1rc1/src/cone/app/testing/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,26 @@
         try:
             fn(*a, **kw)
         finally:
             resources._registry = resource_registry_orgin
     return wrapper
 
 
+def reset_node_available(fn):
+    """Decorator for tests modifying node_available callback
+    """
+    def wrapper(*a, **kw):
+        node_available_orgin = security_module.node_available
+        try:
+            fn(*a, **kw)
+        finally:
+            security_module.node_available = node_available_orgin
+    return wrapper
+
+
 class DummyRequest(BaseDummyRequest, AuthenticationAPIMixin):
     _accept = None
 
     @property
     def is_xhr(self):
         return self.headers.get('X-Requested-With') == 'XMLHttpRequest'
```

### Comparing `cone.app-1.1a2/src/cone/app/testing/dummy_workflow.zcml` & `cone_app-1.1rc1/src/cone/app/testing/dummy_workflow.zcml`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/testing/mock.py` & `cone_app-1.1rc1/src/cone/app/testing/mock.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,20 +15,23 @@
 from node.behaviors import OdictStorage
 from node.utils import instance_property
 from plumber import plumbing
 from pyramid.security import ALL_PERMISSIONS
 from pyramid.security import Allow
 from pyramid.security import Deny
 from pyramid.security import Everyone
-from pyramid.static import static_view
 from zope.component import adapter
 from zope.interface import implementer
 from zope.interface import Interface
 
 
+def testing_node_available(model, node_info_name):
+    return True
+
+
 @plumbing(WorkflowState, WorkflowACL)
 class WorkflowNode(BaseNode):
     workflow_name = u'dummy'
     workflow_tsf = None
 
     @property
     def properties(self):
```

### Comparing `cone.app-1.1a2/src/cone/app/tests/__init__.py` & `cone_app-1.1rc1/src/cone/app/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/tests/test_app.py` & `cone_app-1.1rc1/src/cone/app/tests/test_app.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from cone.app import ApplicationNodeTraverser
 from cone.app import DefaultLayoutConfig
 from cone.app import get_root
 from cone.app import layout_config
 from cone.app import main_hook
 from cone.app import make_remote_addr_middleware
+from cone.app import security
 from cone.app import testing
 from cone.app.interfaces import ILayoutConfig
 from cone.app.model import BaseNode
 from cone.app.model import LayoutConfig
 from node.base import BaseNode as NodeBaseNode
 from node.tests import NodeTestCase
 from pyramid.authentication import AuthTktAuthenticationPolicy
@@ -73,14 +74,15 @@
         with self.assertRaises(ValueError) as arc:
             cone.app.register_config('dummy', BaseNode)
         self.assertEqual(
             str(arc.exception),
             "Config with name 'dummy' already registered."
         )
 
+    @testing.reset_node_available
     def test_main(self):
         # main hook
         hooks = dict(called=0)
 
         def custom_main_hook(configurator, global_config, settings):
             hooks['called'] += 1
 
@@ -107,23 +109,30 @@
             'cone.admin_password': 'admin',
             'cone.auth_secret': '12345',
             'cone.auth_reissue_time': '300',
             'cone.auth_max_age': '600',
             'cone.main_template': 'package.browser:templates/main.pt',
             # ensure custom root node factory gets invoked
             'cone.root.node_factory': 'cone.app.default_root_node_factory',
+            # ensure custom node_available factory gets invoked
+            'cone.root.node_available': 'cone.app.testing.mock.testing_node_available',
             # ensure dummy main hooks called
             'cone.plugins': 'cone.app.tests'
         }
 
         # main
         router = cone.app.main({}, **settings)
         self.assertTrue(isinstance(router, Router))
         self.assertEqual(hooks['called'], 2)
 
+        # Check custom node_available
+        self.assertTrue(
+            security.node_available is testing.mock.testing_node_available
+        )
+
         # Remove custom main hook after testing
         cone.app.main_hooks.remove(custom_main_hook)
         cone.app.main_hooks.remove(decorated_main_hook)
 
         # Check main template was set properly
         self.assertEqual(
             cone.app.cfg.main_template,
```

### Comparing `cone.app-1.1a2/src/cone/app/tests/test_browser.py` & `cone_app-1.1rc1/src/cone/app/tests/test_browser.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/tests/test_browser_actions.py` & `cone_app-1.1rc1/src/cone/app/tests/test_browser_actions.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/tests/test_browser_ajax.py` & `cone_app-1.1rc1/src/cone/app/tests/test_browser_ajax.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/tests/test_browser_authoring.py` & `cone_app-1.1rc1/src/cone/app/tests/test_browser_authoring.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from cone.app import compat
+from cone.app import security
 from cone.app import testing
 from cone.app.browser.ajax import AjaxEvent
 from cone.app.browser.ajax import AjaxMessage
 from cone.app.browser.ajax import AjaxPath
 from cone.app.browser.authoring import _FormRenderingTile
 from cone.app.browser.authoring import add
 from cone.app.browser.authoring import AddFormHeading
@@ -841,14 +842,15 @@
             AjaxMessage
         ))
         self.checkOutput("""
         <class '...CallableNode'>: None
         """, node.treerepr())
 
     @testing.reset_node_info_registry
+    @testing.reset_node_available
     def test_add_items_dropdown(self):
         @node_info(
             name='mynode',
             addables=['mynode'])
         class MyNode(BaseNode):
             pass
 
@@ -893,14 +895,31 @@
         # Ajax targets for add form
         expected = 'ajax:target="http://example.com/somechild?factory=mynode"'
         self.assertTrue(rendered.find(expected) != -1)
 
         expected = 'ajax:target="http://example.com/somechild?factory=anothernode"'
         self.assertTrue(rendered.find(expected) != -1)
 
+        # now disable this other node type globally
+        def node_available(model, node_info_name):
+            if node_info_name == 'anothernode':
+                return False
+            return True
+        security.node_available = node_available
+
+        with self.layer.authenticated('manager'):
+            request = self.layer.new_request()
+            rendered = render_tile(root['somechild'], request, 'add_dropdown')
+
+        expected = 'ajax:target="http://example.com/somechild?factory=mynode"'
+        self.assertTrue(rendered.find(expected) != -1)
+
+        expected = 'ajax:target="http://example.com/somechild?factory=anothernode"'
+        self.assertFalse(rendered.find(expected) != -1)
+
         # Test node without addables, results in empty listing.
         # XXX: hide entire widget if no items
         @node_info(name='nochildaddingnode')
         class NoChildAddingNode(BaseNode):
             pass
 
         with self.layer.authenticated('manager'):
```

### Comparing `cone.app-1.1a2/src/cone/app/tests/test_browser_batch.py` & `cone_app-1.1rc1/src/cone/app/tests/test_browser_batch.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/tests/test_browser_content.py` & `cone_app-1.1rc1/src/cone/app/tests/test_browser_content.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/tests/test_browser_contents.py` & `cone_app-1.1rc1/src/cone/app/tests/test_browser_contents.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/tests/test_browser_contextmenu.py` & `cone_app-1.1rc1/src/cone/app/tests/test_browser_contextmenu.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/tests/test_browser_copysupport.py` & `cone_app-1.1rc1/src/cone/app/tests/test_browser_copysupport.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/tests/test_browser_exception.py` & `cone_app-1.1rc1/src/cone/app/tests/test_browser_exception.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/tests/test_browser_form.py` & `cone_app-1.1rc1/src/cone/app/tests/test_browser_form.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/tests/test_browser_layout.py` & `cone_app-1.1rc1/src/cone/app/tests/test_browser_layout.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/tests/test_browser_login.py` & `cone_app-1.1rc1/src/cone/app/tests/test_browser_login.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/tests/test_browser_order.py` & `cone_app-1.1rc1/src/cone/app/tests/test_browser_order.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/tests/test_browser_referencebrowser.py` & `cone_app-1.1rc1/src/cone/app/tests/test_browser_referencebrowser.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/tests/test_browser_resources.py` & `cone_app-1.1rc1/src/cone/app/tests/test_browser_resources.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/tests/test_browser_settings.py` & `cone_app-1.1rc1/src/cone/app/tests/test_browser_settings.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/tests/test_browser_sharing.py` & `cone_app-1.1rc1/src/cone/app/tests/test_browser_sharing.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/tests/test_browser_table.py` & `cone_app-1.1rc1/src/cone/app/tests/test_browser_table.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/tests/test_browser_translation.py` & `cone_app-1.1rc1/src/cone/app/tests/test_browser_translation.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/tests/test_browser_utils.py` & `cone_app-1.1rc1/src/cone/app/tests/test_browser_utils.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/tests/test_browser_workflow.py` & `cone_app-1.1rc1/src/cone/app/tests/test_browser_workflow.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/tests/test_model.py` & `cone_app-1.1rc1/src/cone/app/tests/test_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -351,25 +351,28 @@
     def test_node_info(self):
         @node_info(
             name='mynode',
             title='My Node',
             description='My Node Descriptrion',
             factory=None,
             icon='icon',
-            addables=['othernode'])
+            addables=['othernode'],
+            custom_prop='custom_value')
         class MyNode(BaseNode):
             pass
 
         info = get_node_info('mynode')
+        self.assertEqual(info.name, 'mynode')
         self.assertTrue(info.node is MyNode)
         self.assertEqual(info.title, 'My Node')
         self.assertEqual(info.description, 'My Node Descriptrion')
         self.assertEqual(info.factory, None)
         self.assertEqual(info.addables, ['othernode'])
         self.assertEqual(info.icon, 'icon')
+        self.assertEqual(info.custom_prop, 'custom_value')
         self.assertEqual(MyNode.node_info_name, 'mynode')
 
     def test_AppEnvironment(self):
         @plumbing(AppEnvironment)
         class AppEnvironmentNode(BaseNode):
             pass
```

### Comparing `cone.app-1.1a2/src/cone/app/tests/test_security.py` & `cone_app-1.1rc1/src/cone/app/tests/test_security.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 from cone.app import testing
 from cone.app.interfaces import IACLAdapter
 from cone.app.interfaces import IAdapterACL
 from cone.app.interfaces import IApplicationNode
 from cone.app.interfaces import IAuthenticator
 from cone.app.interfaces import IOwnerSupport
 from cone.app.interfaces import IPrincipalACL
+from cone.app.model import AppNode
 from cone.app.model import BaseNode
+from cone.app.model import node_info
 from cone.app.security import acl_registry
 from cone.app.security import AdapterACL
 from cone.app.security import authenticate
 from cone.app.security import authenticated_user
 from cone.app.security import DEFAULT_ACL
 from cone.app.security import groups_callback
 from cone.app.security import logger
@@ -26,14 +28,16 @@
 from plumber import default
 from plumber import plumbing
 from pyramid.authentication import AuthTktAuthenticationPolicy
 from pyramid.interfaces import IAuthenticationPolicy
 from pyramid.security import ACLAllowed
 from pyramid.security import ACLDenied
 from pyramid.security import ALL_PERMISSIONS
+from pyramid.security import Deny
+from pyramid.security import Everyone
 from pyramid.threadlocal import get_current_registry
 from zope.component import adapter
 from zope.component.globalregistry import BaseGlobalComponents
 from zope.interface import implementer
 import logging
 
 
@@ -438,14 +442,15 @@
         self.assertEqual(rule[1], 'system.Everyone')
         self.assertEqual(rule[2], ALL_PERMISSIONS)
         self.assertEqual(
             node.__acl__[-1],
             ('Deny', 'system.Everyone', ALL_PERMISSIONS)
         )
 
+    @testing.reset_node_available
     def test_AdapterACL(self):
         @plumbing(AdapterACL)
         class AdapterACLNode(BaseNode):
             pass
 
         node = AdapterACLNode()
         self.assertEqual(node.__acl__, security.DEFAULT_ACL)
@@ -471,14 +476,19 @@
             IACLAdapter,
             default=None
         )
         self.assertIsInstance(acl_adapter, ACLAdapter)
         self.assertEqual(acl_adapter.acl, acl)
         self.assertEqual(node.__acl__, acl)
 
+        def node_available(model, node_info_name):
+            return False
+        security.node_available = node_available
+        self.assertEqual(node.__acl__, [(Deny, Everyone, ALL_PERMISSIONS)])
+
         request.registry.unregisterAdapter(ACLAdapter)
 
     def test_authentication_logging(self):
         # If an authentication plugin raises an error when calling
         # ``authenticate``, an error message is logged
         class TestHandler(logging.StreamHandler):
             record = None
@@ -534,7 +544,32 @@
 
         with self.layer.authenticated('foo'):
             self.assertEqual(request.authenticated_userid, 'foo')
         self.assertEqual(request.authenticated_userid, None)
 
         security.AUTHENTICATOR = authenticator_origin
         registry.unregisterUtility(authenticator)
+
+    @testing.reset_node_info_registry
+    @testing.reset_node_available
+    def test_node_available(self):
+        def node_available(model, node_info_name):
+            if node_info_name == 'denied':
+                return False
+            return True
+        security.node_available = node_available
+
+        @node_info(name='allowed')
+        @plumbing(AppNode)
+        class AllowedNode:
+            ...
+
+        @node_info(name='denied')
+        @plumbing(AppNode)
+        class DeniedNode:
+            ...
+
+        self.assertEqual(AllowedNode().__acl__, DEFAULT_ACL)
+        self.assertEqual(
+            DeniedNode().__acl__,
+            [(Deny, Everyone, ALL_PERMISSIONS)]
+        )
```

### Comparing `cone.app-1.1a2/src/cone/app/tests/test_testing.py` & `cone_app-1.1rc1/src/cone/app/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/tests/test_ugm.py` & `cone_app-1.1rc1/src/cone/app/tests/test_ugm.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/tests/test_utils.py` & `cone_app-1.1rc1/src/cone/app/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/tests/test_workflow.py` & `cone_app-1.1rc1/src/cone/app/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/ugm.py` & `cone_app-1.1rc1/src/cone/app/ugm.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/utils.py` & `cone_app-1.1rc1/src/cone/app/utils.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone/app/workflow.py` & `cone_app-1.1rc1/src/cone/app/workflow.py`

 * *Files identical despite different names*

### Comparing `cone.app-1.1a2/src/cone.app.egg-info/PKG-INFO` & `cone_app-1.1rc1/src/cone.app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cone.app
-Version: 1.1a2
+Version: 1.1rc1
 Summary: Web application stub
 Home-page: http://github.com/conestack/cone.app
 Author: Cone Contributors
 Author-email: dev@conestack.org
 License: Simplified BSD
 Keywords: node pyramid cone web
 Classifier: Environment :: Web Environment
@@ -87,14 +87,29 @@
 - Peter Holzer
 - Johannes Raggam
 
 
 Changes
 =======
 
+1.1rc1 (2024-05-23)
+-------------------
+
+- ``node_info`` decorator stores name on node info instance.
+  [rnix]
+
+- ``node_info`` decorator accepts additional keyword arguments to add custom
+  properties.
+  [rnix]
+
+- Add ``node_available`` callback to check whether node is allowed to be
+  used in application.
+  [rnix]
+
+
 1.1a2 (2024-02-12)
 ------------------
 
 - Introduce ``cone.app.browser.form.``,
   ``cone.app.browser.form.FormTarget``,
   ``cone.app.browser.form.AddFormTarget``,
   ``cone.app.browser.form.EditFormTarget``,
```

### Comparing `cone.app-1.1a2/src/cone.app.egg-info/SOURCES.txt` & `cone_app-1.1rc1/src/cone.app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

