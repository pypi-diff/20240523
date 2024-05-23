# Comparing `tmp/django-friendly-tag-loader-1.3.1.tar.gz` & `tmp/django_friendly_tag_loader-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-friendly-tag-loader-1.3.1.tar", last modified: Wed Aug 15 04:05:01 2018, max compression
+gzip compressed data, was "django_friendly_tag_loader-1.3.2.tar", last modified: Thu May 23 02:37:06 2024, max compression
```

## Comparing `django-friendly-tag-loader-1.3.1.tar` & `django_friendly_tag_loader-1.3.2.tar`

### file list

```diff
@@ -1,33 +1,32 @@
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2018-08-15 04:05:01.000000 django-friendly-tag-loader-1.3.1/
--rw-r--r--   0 adam       (501) staff       (20)     6158 2018-06-27 02:41:28.000000 django-friendly-tag-loader-1.3.1/bootstrap.py
--rw-r--r--   0 adam       (501) staff       (20)     1282 2018-06-27 02:41:28.000000 django-friendly-tag-loader-1.3.1/buildout.cfg
--rw-r--r--   0 adam       (501) staff       (20)      561 2018-08-15 04:02:08.000000 django-friendly-tag-loader-1.3.1/CHANGES.rst
--rw-r--r--   0 adam       (501) staff       (20)     1070 2018-06-27 02:41:28.000000 django-friendly-tag-loader-1.3.1/LICENSE
--rw-r--r--   0 adam       (501) staff       (20)     1729 2018-06-27 02:41:28.000000 django-friendly-tag-loader-1.3.1/Makefile
--rw-r--r--   0 adam       (501) staff       (20)      112 2018-06-27 02:41:28.000000 django-friendly-tag-loader-1.3.1/MANIFEST.in
--rw-r--r--   0 adam       (501) staff       (20)     4106 2018-08-15 04:05:01.000000 django-friendly-tag-loader-1.3.1/PKG-INFO
--rw-r--r--   0 adam       (501) staff       (20)     1844 2018-06-27 02:41:28.000000 django-friendly-tag-loader-1.3.1/README.rst
--rw-r--r--   0 adam       (501) staff       (20)       88 2018-08-15 04:05:01.000000 django-friendly-tag-loader-1.3.1/setup.cfg
--rw-r--r--   0 adam       (501) staff       (20)     1331 2018-08-15 04:02:25.000000 django-friendly-tag-loader-1.3.1/setup.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2018-08-15 04:05:01.000000 django-friendly-tag-loader-1.3.1/src/
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2018-08-15 04:05:01.000000 django-friendly-tag-loader-1.3.1/src/django_friendly_tag_loader.egg-info/
--rw-rw-r--   0 adam       (501) staff       (20)        1 2018-08-15 04:05:01.000000 django-friendly-tag-loader-1.3.1/src/django_friendly_tag_loader.egg-info/dependency_links.txt
--rw-rw-r--   0 adam       (501) staff       (20)        1 2018-08-14 05:02:31.000000 django-friendly-tag-loader-1.3.1/src/django_friendly_tag_loader.egg-info/not-zip-safe
--rw-rw-r--   0 adam       (501) staff       (20)     4106 2018-08-15 04:05:01.000000 django-friendly-tag-loader-1.3.1/src/django_friendly_tag_loader.egg-info/PKG-INFO
--rw-rw-r--   0 adam       (501) staff       (20)      699 2018-08-15 04:05:01.000000 django-friendly-tag-loader-1.3.1/src/django_friendly_tag_loader.egg-info/SOURCES.txt
--rw-rw-r--   0 adam       (501) staff       (20)       18 2018-08-15 04:05:01.000000 django-friendly-tag-loader-1.3.1/src/django_friendly_tag_loader.egg-info/top_level.txt
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2018-08-15 04:05:01.000000 django-friendly-tag-loader-1.3.1/src/friendlytagloader/
--rw-r--r--   0 adam       (501) staff       (20)        0 2018-06-27 02:41:28.000000 django-friendly-tag-loader-1.3.1/src/friendlytagloader/__init__.py
--rw-r--r--   0 adam       (501) staff       (20)        0 2018-06-27 02:41:28.000000 django-friendly-tag-loader-1.3.1/src/friendlytagloader/models.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2018-08-15 04:05:01.000000 django-friendly-tag-loader-1.3.1/src/friendlytagloader/templatetags/
--rw-r--r--   0 adam       (501) staff       (20)        0 2018-06-27 02:41:28.000000 django-friendly-tag-loader-1.3.1/src/friendlytagloader/templatetags/__init__.py
--rw-r--r--   0 adam       (501) staff       (20)     4978 2018-08-15 04:01:44.000000 django-friendly-tag-loader-1.3.1/src/friendlytagloader/templatetags/friendly_loader.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2018-08-15 04:05:01.000000 django-friendly-tag-loader-1.3.1/tests/
--rw-r--r--   0 adam       (501) staff       (20)        0 2018-06-27 02:41:28.000000 django-friendly-tag-loader-1.3.1/tests/__init__.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2018-08-15 04:05:01.000000 django-friendly-tag-loader-1.3.1/tests/testproject/
--rw-r--r--   0 adam       (501) staff       (20)        0 2018-06-27 02:41:28.000000 django-friendly-tag-loader-1.3.1/tests/testproject/__init__.py
--rw-r--r--   0 adam       (501) staff       (20)        0 2018-06-27 02:41:28.000000 django-friendly-tag-loader-1.3.1/tests/testproject/models.py
--rw-r--r--   0 adam       (501) staff       (20)     1290 2018-06-27 02:41:28.000000 django-friendly-tag-loader-1.3.1/tests/testproject/settings.py
--rw-r--r--   0 adam       (501) staff       (20)     7235 2018-06-27 02:41:28.000000 django-friendly-tag-loader-1.3.1/tests/testproject/tests.py
--rw-r--r--   0 adam       (501) staff       (20)      149 2018-06-27 02:41:28.000000 django-friendly-tag-loader-1.3.1/tests/testproject/urls.py
--rw-r--r--   0 adam       (501) staff       (20)      999 2018-08-15 04:01:44.000000 django-friendly-tag-loader-1.3.1/tox.ini
+drwxr-xr-x   0 taylors    (501) staff       (20)        0 2024-05-23 02:37:06.959088 django_friendly_tag_loader-1.3.2/
+-rw-r--r--   0 taylors    (501) staff       (20)      644 2024-05-23 02:21:23.000000 django_friendly_tag_loader-1.3.2/CHANGES.rst
+-rw-r--r--   0 taylors    (501) staff       (20)     1070 2024-05-21 02:32:21.000000 django_friendly_tag_loader-1.3.2/LICENSE
+-rw-r--r--   0 taylors    (501) staff       (20)      112 2024-05-23 02:14:39.000000 django_friendly_tag_loader-1.3.2/MANIFEST.in
+-rw-r--r--   0 taylors    (501) staff       (20)     1729 2024-05-21 02:32:21.000000 django_friendly_tag_loader-1.3.2/Makefile
+-rw-r--r--   0 taylors    (501) staff       (20)     3358 2024-05-23 02:37:06.958373 django_friendly_tag_loader-1.3.2/PKG-INFO
+-rw-r--r--   0 taylors    (501) staff       (20)     1844 2024-05-21 02:32:21.000000 django_friendly_tag_loader-1.3.2/README.rst
+-rw-r--r--   0 taylors    (501) staff       (20)     6158 2024-05-21 02:32:21.000000 django_friendly_tag_loader-1.3.2/bootstrap.py
+-rw-r--r--   0 taylors    (501) staff       (20)     1282 2024-05-21 02:32:21.000000 django_friendly_tag_loader-1.3.2/buildout.cfg
+-rw-r--r--   0 taylors    (501) staff       (20)     1516 2024-05-23 02:21:33.000000 django_friendly_tag_loader-1.3.2/pyproject.toml
+-rw-r--r--   0 taylors    (501) staff       (20)       38 2024-05-23 02:37:06.959262 django_friendly_tag_loader-1.3.2/setup.cfg
+drwxr-xr-x   0 taylors    (501) staff       (20)        0 2024-05-23 02:37:06.939288 django_friendly_tag_loader-1.3.2/src/
+drwxr-xr-x   0 taylors    (501) staff       (20)        0 2024-05-23 02:37:06.957618 django_friendly_tag_loader-1.3.2/src/django_friendly_tag_loader.egg-info/
+-rw-r--r--   0 taylors    (501) staff       (20)     3358 2024-05-23 02:37:06.000000 django_friendly_tag_loader-1.3.2/src/django_friendly_tag_loader.egg-info/PKG-INFO
+-rw-r--r--   0 taylors    (501) staff       (20)      642 2024-05-23 02:37:06.000000 django_friendly_tag_loader-1.3.2/src/django_friendly_tag_loader.egg-info/SOURCES.txt
+-rw-r--r--   0 taylors    (501) staff       (20)        1 2024-05-23 02:37:06.000000 django_friendly_tag_loader-1.3.2/src/django_friendly_tag_loader.egg-info/dependency_links.txt
+-rw-r--r--   0 taylors    (501) staff       (20)       18 2024-05-23 02:37:06.000000 django_friendly_tag_loader-1.3.2/src/django_friendly_tag_loader.egg-info/top_level.txt
+drwxr-xr-x   0 taylors    (501) staff       (20)        0 2024-05-23 02:37:06.948697 django_friendly_tag_loader-1.3.2/src/friendlytagloader/
+-rw-r--r--   0 taylors    (501) staff       (20)        0 2024-05-23 01:29:32.000000 django_friendly_tag_loader-1.3.2/src/friendlytagloader/__init__.py
+-rw-r--r--   0 taylors    (501) staff       (20)        0 2024-05-21 02:32:21.000000 django_friendly_tag_loader-1.3.2/src/friendlytagloader/models.py
+drwxr-xr-x   0 taylors    (501) staff       (20)        0 2024-05-23 02:37:06.949363 django_friendly_tag_loader-1.3.2/src/friendlytagloader/templatetags/
+-rw-r--r--   0 taylors    (501) staff       (20)        0 2024-05-21 02:32:21.000000 django_friendly_tag_loader-1.3.2/src/friendlytagloader/templatetags/__init__.py
+-rw-r--r--   0 taylors    (501) staff       (20)     4972 2024-05-21 22:25:58.000000 django_friendly_tag_loader-1.3.2/src/friendlytagloader/templatetags/friendly_loader.py
+drwxr-xr-x   0 taylors    (501) staff       (20)        0 2024-05-23 02:37:06.950012 django_friendly_tag_loader-1.3.2/tests/
+-rw-r--r--   0 taylors    (501) staff       (20)        0 2024-05-21 02:32:21.000000 django_friendly_tag_loader-1.3.2/tests/__init__.py
+drwxr-xr-x   0 taylors    (501) staff       (20)        0 2024-05-23 02:37:06.956739 django_friendly_tag_loader-1.3.2/tests/testproject/
+-rw-r--r--   0 taylors    (501) staff       (20)        0 2024-05-21 02:32:21.000000 django_friendly_tag_loader-1.3.2/tests/testproject/__init__.py
+-rw-r--r--   0 taylors    (501) staff       (20)        0 2024-05-21 02:32:21.000000 django_friendly_tag_loader-1.3.2/tests/testproject/models.py
+-rw-r--r--   0 taylors    (501) staff       (20)     1296 2024-05-21 02:32:21.000000 django_friendly_tag_loader-1.3.2/tests/testproject/settings.py
+-rw-r--r--   0 taylors    (501) staff       (20)     7354 2024-05-23 01:27:30.000000 django_friendly_tag_loader-1.3.2/tests/testproject/tests.py
+-rw-r--r--   0 taylors    (501) staff       (20)      247 2024-05-21 02:32:21.000000 django_friendly_tag_loader-1.3.2/tests/testproject/urls.py
+-rw-r--r--   0 taylors    (501) staff       (20)     1266 2024-05-23 02:30:07.000000 django_friendly_tag_loader-1.3.2/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-friendly-tag-loader-1.3.1/bootstrap.py` & `django_friendly_tag_loader-1.3.2/bootstrap.py`

 * *Files identical despite different names*

### Comparing `django-friendly-tag-loader-1.3.1/buildout.cfg` & `django_friendly_tag_loader-1.3.2/buildout.cfg`

 * *Files identical despite different names*

### Comparing `django-friendly-tag-loader-1.3.1/CHANGES.rst` & `django_friendly_tag_loader-1.3.2/CHANGES.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changes
 =======
 
+1.3.2 (2024-05-22)
+------------------
+
+- Added support for Django 4.1 through 5.0
+
 1.3.1 (2018-08-14)
 ------------------
 
 - Added support for Django 2.1
 
 1.3 (2018-06-21)
 ----------------
```

### Comparing `django-friendly-tag-loader-1.3.1/LICENSE` & `django_friendly_tag_loader-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-friendly-tag-loader-1.3.1/Makefile` & `django_friendly_tag_loader-1.3.2/Makefile`

 * *Files identical despite different names*

### Comparing `django-friendly-tag-loader-1.3.1/PKG-INFO` & `django_friendly_tag_loader-1.3.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,126 +1,95 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-friendly-tag-loader
-Version: 1.3.1
+Version: 1.3.2
 Summary: Want to optionally use a template tag library? Use this!
-Home-page: https://github.com/ataylor32/django-friendly-tag-loader
-Author: Jaap Roes
-Author-email: jaap.roes@gmail.com
+Author-email: Jaap Roes <jaap.roes@gmail.com>, Adam Taylor <ataylor32@gmail.com>
 License: MIT
-Description: ==========================
-        django-friendly-tag-loader
-        ==========================
-        
-        Use templatetag libraries in Django templates to optionally support features.
-        
-        This app provides three template tags ``{% friendly_load %}``,
-        ``{% if_has_tag %}`` and ``{% ifnot_has_tag %}``.
-        
-        Used together you can built templates that have optional support for certain
-        template tags. You can use them if they are available and do something else if
-        they are not.
-        
-        Installation
-        ============
-        
-        Add ``friendlytagloader`` to ``INSTALLED_APPS``
-        
-        Usage
-        =====
-        
-        ``{% load friendly_loader %}`` in your template
-        
-        Load some optional taglib ``{% friendly_load comments %}``
-        
-        Or load a specific tag ``{% friendly_load cycle from future %}``
-        
-        Conditionally use its tag::
-        
-          {% if_has_tag render_comment_list %}
-              {% render_comment_list for obj %}
-          {% else %}
-              Comment support is not available
-          {% endif_has_tag %}
-        
-        ``{% friendly_load %}`` takes multiple arguments, so loading multiple optional
-        template tag libraries at once is supported::
-        
-          {% friendly_load comments webdesign website_tags %}
-        
-        ``{% if_has_tag %}`` and ``{% ifnot_has_tag %}`` can also handle multiple
-        arguments.
-        
-        In the case of ``if_has_tag`` this means that all given tags should be
-        available, so this will render nothing even though ``now`` is a built-in tag::
-        
-          {% if_has_tag now nonexisting_tag %}
-            {% now 'Y' %}
-          {% endif_has_tag %}
-        
-        The ``ifnot_has_tag`` condition will trigger if any of the given tags is
-        unavailable. For example this will render the message since, even though
-        ``now`` is a built-in tag, ``nonexisting_tag`` is not available::
-        
-          {% ifnot_has_tag now nonexisting_tag %}
-            Some tags are unavailable.
-          {% endifnot_has_tag %}
-        
-        Credits
-        =======
-        
-        Original Author: `Jaap Roes <https://github.com/jaap3>`_
-        
-        Current Maintainer: `Adam Taylor <https://github.com/ataylor32>`_
-        
-        Changes
-        =======
-        
-        1.3.1 (2018-08-14)
-        ------------------
-        
-        - Added support for Django 2.1
-        
-        1.3 (2018-06-21)
-        ----------------
-        
-        - Dropped support for Django < 1.11
-        - Added support for Django 1.11 and 2.0
-        
-        
-        1.2.1 (2015-07-01)
-        ------------------
-        
-        - Django 1.8 support
-        
-        
-        1.2 (2014-09-29)
-        ----------------
-        
-        - Dropped support for Django < 1.4
-        - Verified Django support up to 1.7
-        - Added Python 3 support
-        - Support ``friendly_load tag from taglib`` syntax
-        
-        
-        1.1 (2012-06-01)
-        ----------------
-        
-        - Django 1.4 compatible
-        
-        
-        1.0 (2011-10-21)
-        ----------------
-        
-        - Initial release
-Platform: UNKNOWN
+Project-URL: Homepage, https://github.com/ataylor32/django-friendly-tag-loader
+Project-URL: Repository, https://github.com/ataylor32/django-friendly-tag-loader.git
+Project-URL: Issues, https://github.com/ataylor32/django-friendly-tag-loader/issues
+Project-URL: Changelog, https://github.com/ataylor32/django-friendly-tag-loader/blob/master/CHANGES.rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+==========================
+django-friendly-tag-loader
+==========================
+
+Use templatetag libraries in Django templates to optionally support features.
+
+This app provides three template tags ``{% friendly_load %}``,
+``{% if_has_tag %}`` and ``{% ifnot_has_tag %}``.
+
+Used together you can built templates that have optional support for certain
+template tags. You can use them if they are available and do something else if
+they are not.
+
+Installation
+============
+
+Add ``friendlytagloader`` to ``INSTALLED_APPS``
+
+Usage
+=====
+
+``{% load friendly_loader %}`` in your template
+
+Load some optional taglib ``{% friendly_load comments %}``
+
+Or load a specific tag ``{% friendly_load cycle from future %}``
+
+Conditionally use its tag::
+
+  {% if_has_tag render_comment_list %}
+      {% render_comment_list for obj %}
+  {% else %}
+      Comment support is not available
+  {% endif_has_tag %}
+
+``{% friendly_load %}`` takes multiple arguments, so loading multiple optional
+template tag libraries at once is supported::
+
+  {% friendly_load comments webdesign website_tags %}
+
+``{% if_has_tag %}`` and ``{% ifnot_has_tag %}`` can also handle multiple
+arguments.
+
+In the case of ``if_has_tag`` this means that all given tags should be
+available, so this will render nothing even though ``now`` is a built-in tag::
+
+  {% if_has_tag now nonexisting_tag %}
+    {% now 'Y' %}
+  {% endif_has_tag %}
+
+The ``ifnot_has_tag`` condition will trigger if any of the given tags is
+unavailable. For example this will render the message since, even though
+``now`` is a built-in tag, ``nonexisting_tag`` is not available::
+
+  {% ifnot_has_tag now nonexisting_tag %}
+    Some tags are unavailable.
+  {% endifnot_has_tag %}
+
+Credits
+=======
+
+Original Author: `Jaap Roes <https://github.com/jaap3>`_
+
+Current Maintainer: `Adam Taylor <https://github.com/ataylor32>`_
```

### Comparing `django-friendly-tag-loader-1.3.1/README.rst` & `django_friendly_tag_loader-1.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `django-friendly-tag-loader-1.3.1/src/django_friendly_tag_loader.egg-info/PKG-INFO` & `django_friendly_tag_loader-1.3.2/src/django_friendly_tag_loader.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,126 +1,95 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-friendly-tag-loader
-Version: 1.3.1
+Version: 1.3.2
 Summary: Want to optionally use a template tag library? Use this!
-Home-page: https://github.com/ataylor32/django-friendly-tag-loader
-Author: Jaap Roes
-Author-email: jaap.roes@gmail.com
+Author-email: Jaap Roes <jaap.roes@gmail.com>, Adam Taylor <ataylor32@gmail.com>
 License: MIT
-Description: ==========================
-        django-friendly-tag-loader
-        ==========================
-        
-        Use templatetag libraries in Django templates to optionally support features.
-        
-        This app provides three template tags ``{% friendly_load %}``,
-        ``{% if_has_tag %}`` and ``{% ifnot_has_tag %}``.
-        
-        Used together you can built templates that have optional support for certain
-        template tags. You can use them if they are available and do something else if
-        they are not.
-        
-        Installation
-        ============
-        
-        Add ``friendlytagloader`` to ``INSTALLED_APPS``
-        
-        Usage
-        =====
-        
-        ``{% load friendly_loader %}`` in your template
-        
-        Load some optional taglib ``{% friendly_load comments %}``
-        
-        Or load a specific tag ``{% friendly_load cycle from future %}``
-        
-        Conditionally use its tag::
-        
-          {% if_has_tag render_comment_list %}
-              {% render_comment_list for obj %}
-          {% else %}
-              Comment support is not available
-          {% endif_has_tag %}
-        
-        ``{% friendly_load %}`` takes multiple arguments, so loading multiple optional
-        template tag libraries at once is supported::
-        
-          {% friendly_load comments webdesign website_tags %}
-        
-        ``{% if_has_tag %}`` and ``{% ifnot_has_tag %}`` can also handle multiple
-        arguments.
-        
-        In the case of ``if_has_tag`` this means that all given tags should be
-        available, so this will render nothing even though ``now`` is a built-in tag::
-        
-          {% if_has_tag now nonexisting_tag %}
-            {% now 'Y' %}
-          {% endif_has_tag %}
-        
-        The ``ifnot_has_tag`` condition will trigger if any of the given tags is
-        unavailable. For example this will render the message since, even though
-        ``now`` is a built-in tag, ``nonexisting_tag`` is not available::
-        
-          {% ifnot_has_tag now nonexisting_tag %}
-            Some tags are unavailable.
-          {% endifnot_has_tag %}
-        
-        Credits
-        =======
-        
-        Original Author: `Jaap Roes <https://github.com/jaap3>`_
-        
-        Current Maintainer: `Adam Taylor <https://github.com/ataylor32>`_
-        
-        Changes
-        =======
-        
-        1.3.1 (2018-08-14)
-        ------------------
-        
-        - Added support for Django 2.1
-        
-        1.3 (2018-06-21)
-        ----------------
-        
-        - Dropped support for Django < 1.11
-        - Added support for Django 1.11 and 2.0
-        
-        
-        1.2.1 (2015-07-01)
-        ------------------
-        
-        - Django 1.8 support
-        
-        
-        1.2 (2014-09-29)
-        ----------------
-        
-        - Dropped support for Django < 1.4
-        - Verified Django support up to 1.7
-        - Added Python 3 support
-        - Support ``friendly_load tag from taglib`` syntax
-        
-        
-        1.1 (2012-06-01)
-        ----------------
-        
-        - Django 1.4 compatible
-        
-        
-        1.0 (2011-10-21)
-        ----------------
-        
-        - Initial release
-Platform: UNKNOWN
+Project-URL: Homepage, https://github.com/ataylor32/django-friendly-tag-loader
+Project-URL: Repository, https://github.com/ataylor32/django-friendly-tag-loader.git
+Project-URL: Issues, https://github.com/ataylor32/django-friendly-tag-loader/issues
+Project-URL: Changelog, https://github.com/ataylor32/django-friendly-tag-loader/blob/master/CHANGES.rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+==========================
+django-friendly-tag-loader
+==========================
+
+Use templatetag libraries in Django templates to optionally support features.
+
+This app provides three template tags ``{% friendly_load %}``,
+``{% if_has_tag %}`` and ``{% ifnot_has_tag %}``.
+
+Used together you can built templates that have optional support for certain
+template tags. You can use them if they are available and do something else if
+they are not.
+
+Installation
+============
+
+Add ``friendlytagloader`` to ``INSTALLED_APPS``
+
+Usage
+=====
+
+``{% load friendly_loader %}`` in your template
+
+Load some optional taglib ``{% friendly_load comments %}``
+
+Or load a specific tag ``{% friendly_load cycle from future %}``
+
+Conditionally use its tag::
+
+  {% if_has_tag render_comment_list %}
+      {% render_comment_list for obj %}
+  {% else %}
+      Comment support is not available
+  {% endif_has_tag %}
+
+``{% friendly_load %}`` takes multiple arguments, so loading multiple optional
+template tag libraries at once is supported::
+
+  {% friendly_load comments webdesign website_tags %}
+
+``{% if_has_tag %}`` and ``{% ifnot_has_tag %}`` can also handle multiple
+arguments.
+
+In the case of ``if_has_tag`` this means that all given tags should be
+available, so this will render nothing even though ``now`` is a built-in tag::
+
+  {% if_has_tag now nonexisting_tag %}
+    {% now 'Y' %}
+  {% endif_has_tag %}
+
+The ``ifnot_has_tag`` condition will trigger if any of the given tags is
+unavailable. For example this will render the message since, even though
+``now`` is a built-in tag, ``nonexisting_tag`` is not available::
+
+  {% ifnot_has_tag now nonexisting_tag %}
+    Some tags are unavailable.
+  {% endifnot_has_tag %}
+
+Credits
+=======
+
+Original Author: `Jaap Roes <https://github.com/jaap3>`_
+
+Current Maintainer: `Adam Taylor <https://github.com/ataylor32>`_
```

### Comparing `django-friendly-tag-loader-1.3.1/src/django_friendly_tag_loader.egg-info/SOURCES.txt` & `django_friendly_tag_loader-1.3.2/src/django_friendly_tag_loader.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 CHANGES.rst
 LICENSE
 MANIFEST.in
 Makefile
 README.rst
 bootstrap.py
 buildout.cfg
-setup.cfg
-setup.py
+pyproject.toml
 tox.ini
 src/django_friendly_tag_loader.egg-info/PKG-INFO
 src/django_friendly_tag_loader.egg-info/SOURCES.txt
 src/django_friendly_tag_loader.egg-info/dependency_links.txt
-src/django_friendly_tag_loader.egg-info/not-zip-safe
 src/django_friendly_tag_loader.egg-info/top_level.txt
 src/friendlytagloader/__init__.py
 src/friendlytagloader/models.py
 src/friendlytagloader/templatetags/__init__.py
 src/friendlytagloader/templatetags/friendly_loader.py
 tests/__init__.py
 tests/testproject/__init__.py
```

### Comparing `django-friendly-tag-loader-1.3.1/src/friendlytagloader/templatetags/friendly_loader.py` & `django_friendly_tag_loader-1.3.2/src/friendlytagloader/templatetags/friendly_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from django.template import Library, TemplateSyntaxError
+from django.template import Library, NodeList, TemplateSyntaxError
 
 try:
     from django.template.base import TokenType
 except ImportError:
     # Django < 2.1
     from django.template.base import TOKEN_BLOCK
 else:
     TOKEN_BLOCK = TokenType.BLOCK
 
-from django.template.defaulttags import (CommentNode, IfNode, LoadNode,
-                                         find_library, load_from_library)
+from django.template.defaulttags import (IfNode, LoadNode, find_library,
+                                         load_from_library)
 from django.template.smartif import Literal
 
 register = Library()
 
 
 @register.tag
 def friendly_load(parser, token):
@@ -85,15 +85,15 @@
     """
     bits = list(token.split_contents())
     if len(bits) < 2:
         raise TemplateSyntaxError("%r takes at least one arguments" % bits[0])
     end_tag = 'end%s' % bits[0]
     has_tag = all([tag in parser.tags for tag in bits[1:]])
     has_tag = (not negate and has_tag) or (negate and not has_tag)
-    nodelist_true = nodelist_false = CommentNode()
+    nodelist_true = nodelist_false = NodeList()
     if has_tag:
         nodelist_true = parser.parse(('else', end_tag))
         token = parser.next_token()
         if token.contents == 'else':
             parser.skip_past(end_tag)
     else:
         while parser.tokens:
```

### Comparing `django-friendly-tag-loader-1.3.1/tests/testproject/settings.py` & `django_friendly_tag_loader-1.3.2/tests/testproject/settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from os.path import dirname, join
 
+import dj_database_url
+
 DEBUG = True
 
 MIDDLEWARE = (
     'django.contrib.sessions.middleware.SessionMiddleware',
     'django.middleware.common.CommonMiddleware',
     'django.middleware.csrf.CsrfViewMiddleware',
     'django.contrib.auth.middleware.AuthenticationMiddleware',
     'django.contrib.messages.middleware.MessageMiddleware',
     'django.middleware.clickjacking.XFrameOptionsMiddleware',
 )
 
 DATABASES = {
-    "default": {
-        "ENGINE": 'django.db.backends.sqlite3',
-        "NAME": join(dirname(__file__), 'db', 'friendlytagloader.db')
-    }
+    'default': dj_database_url.config(
+        default='postgres://developer:developer@localhost:5432/django_test',
+    ),
 }
 
 INSTALLED_APPS = (
     'testproject',
     'friendlytagloader',
     'django.contrib.sites',
     'django.contrib.flatpages',
```

### Comparing `django-friendly-tag-loader-1.3.1/tests/testproject/tests.py` & `django_friendly_tag_loader-1.3.2/tests/testproject/tests.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,20 @@
 from django.template.engine import Engine
 from django.test import TestCase
 
 engine = Engine.get_default()
 
 
 def _render_template(template):
-    return Template(template).render(Context({})).strip()
+    return Template(
+        '{% extends "base.html" %}' +
+        '{% block content %}' +
+        template +
+        '{% endblock content %}'
+    ).render(Context({})).strip()
 
 
 class FriendlyLoadingTest(TestCase):
 
     def test_cannot_load_missing_taglib_using_standard_load(self):
         template = '{% load error_tags %}'
         self.assertRaises(TemplateSyntaxError, Template, template)
```

