# Comparing `tmp/jinja2_embedded-0.1.3.tar.gz` & `tmp/jinja2_embedded-0.1.4.tar.gz`

## Comparing `jinja2_embedded-0.1.3.tar` & `jinja2_embedded-0.1.4.tar`

### file list

```diff
@@ -1,31 +1,35 @@
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.3/.python-version
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.3/py.typed
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.3/pyoxidizer.bzl
--rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.3/requirements-dev.lock
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.3/requirements.lock
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.3/.github/workflows/pre-commit.yml
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.3/.github/workflows/pyoxidizer.yml
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.3/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.3/.vscode/settings.json
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.3/src/jinja2_embedded/__init__.py
--rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.3/src/jinja2_embedded/loaders.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.3/tests/conftest.py
--rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.3/tests/test_loader.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.3/tests/test_module/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.3/tests/test_module/src/test_module/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.3/tests/test_module/src/test_module/templates/__init__.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.3/tests/test_module/src/test_module/templates/broken.html
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.3/tests/test_module/src/test_module/templates/syntaxerror.html
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.3/tests/test_module/src/test_module/templates/test.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.3/tests/test_module/src/test_module/templates/bar/__init__.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.3/tests/test_module/src/test_module/templates/bar/test.html.jinja2
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.3/tests/test_module/src/test_module/templates/foo/test.html
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.3/tests/test_module/src/test_module/templates/foo/bar/x.html
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.3/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.3/LICENSE
--rw-r--r--   0        0        0     5236 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.3/README.rst
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     6330 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.4/.python-version
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.4/py.typed
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.4/pyoxidizer.bzl
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.4/requirements-dev.lock
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.4/requirements.lock
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.4/.github/workflows/pre-commit.yml
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.4/.github/workflows/pyoxidizer.yml
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.4/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.4/.vscode/settings.json
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.4/src/jinja2_embedded/__init__.py
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.4/src/jinja2_embedded/loaders.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.4/tests/conftest.py
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.4/tests/test_loader.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.4/tests/test_module/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.4/tests/test_module/src/test_module/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.4/tests/test_module/src/test_module/templates/__init__.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.4/tests/test_module/src/test_module/templates/broken.html
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.4/tests/test_module/src/test_module/templates/syntaxerror.html
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.4/tests/test_module/src/test_module/templates/test.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.4/tests/test_module/src/test_module/templates/bar/__init__.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.4/tests/test_module/src/test_module/templates/bar/test.html.jinja2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.4/tests/test_module/src/test_module/templates/baz/__init__.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.4/tests/test_module/src/test_module/templates/baz/a/b.html
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.4/tests/test_module/src/test_module/templates/foo/test.html
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.4/tests/test_module/src/test_module/templates/foo/bar/x.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.4/tests/test_module/src/test_module/templates/foo/bar/baz/__init__.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.4/tests/test_module/src/test_module/templates/foo/bar/baz/a.html
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.4/LICENSE
+-rw-r--r--   0        0        0     5371 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.4/README.rst
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     6465 2020-02-02 00:00:00.000000 jinja2_embedded-0.1.4/PKG-INFO
```

### Comparing `jinja2_embedded-0.1.3/.pre-commit-config.yaml` & `jinja2_embedded-0.1.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `jinja2_embedded-0.1.3/pyoxidizer.bzl` & `jinja2_embedded-0.1.4/pyoxidizer.bzl`

 * *Files identical despite different names*

### Comparing `jinja2_embedded-0.1.3/requirements-dev.lock` & `jinja2_embedded-0.1.4/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `jinja2_embedded-0.1.3/requirements.lock` & `jinja2_embedded-0.1.4/requirements.lock`

 * *Files identical despite different names*

### Comparing `jinja2_embedded-0.1.3/.github/workflows/pyoxidizer.yml` & `jinja2_embedded-0.1.4/.github/workflows/pyoxidizer.yml`

 * *Files identical despite different names*

### Comparing `jinja2_embedded-0.1.3/.github/workflows/python-package.yml` & `jinja2_embedded-0.1.4/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `jinja2_embedded-0.1.3/.github/workflows/python-publish.yml` & `jinja2_embedded-0.1.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `jinja2_embedded-0.1.3/src/jinja2_embedded/loaders.py` & `jinja2_embedded-0.1.4/src/jinja2_embedded/loaders.py`

 * *Files 7% similar despite different names*

```diff
@@ -97,28 +97,40 @@
             with resource_reader.open_resource(path) as resource:
                 source = resource.read()
         except FileNotFoundError as e:
             if len(parts) < 2:
                 raise TemplateNotFound(template) from e
 
             try:
+                source = self._recursive_resolve(parts[:-1], parts[-1])
+            except FileNotFoundError as e:
+                raise TemplateNotFound(template) from e
+
+        return source.decode(self.encoding), path, lambda: True
+
+    def _recursive_resolve(self, parts: list[str], template: str):
+        for i in range(1, len(parts) + 1):
+            module = '.'.join([self.package, *parts[:i]])
+            name = '/'.join([*parts[i:], template])
+            try:
                 resource_reader = self._loader.get_resource_reader(  # type: ignore[attr-defined]
-                    '.'.join([self.package, *parts[:-1]])
+                    module
                 )
-            except ImportError as e:
-                raise TemplateNotFound(template) from e
+            except ImportError:
+                # dir is not a module (missing __init__.py)
+                continue
 
             if resource_reader is None:
-                raise TemplateNotFound(
-                    template,
-                    'Could not create ResourceReader.',
-                )
+                # dir is not a module (missing __init__.py)
+                continue
 
             try:
                 # check if we can find the file in a submodule
                 # submodule = directory with __init__.py
-                with resource_reader.open_resource(parts[-1]) as resource:
-                    source = resource.read()
-            except FileNotFoundError as ex:
-                raise TemplateNotFound(template) from ex
+                with resource_reader.open_resource(name) as resource:
+                    return resource.read()
+            except FileNotFoundError:
+                continue
 
-        return source.decode(self.encoding), path, lambda: True
+        raise FileNotFoundError(
+            f'Could not find template {"/".join(parts)}/{template}.'
+        )
```

### Comparing `jinja2_embedded-0.1.3/tests/test_loader.py` & `jinja2_embedded-0.1.4/tests/test_loader.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,25 +8,29 @@
 def test_embedded_package_loader(embedded_package_loader):
     env = Environment(loader=embedded_package_loader)
     tmpl = env.get_template('test.html')
     assert tmpl.render().strip() == 'BAR'
     pytest.raises(TemplateNotFound, env.get_template, 'missing.html')
     pytest.raises(TemplateNotFound, env.get_template, 'foo/missing.html')
     pytest.raises(TemplateNotFound, env.get_template, 'bar/missing.html')
+    pytest.raises(TemplateNotFound, env.get_template, 'baz/a/missing.html')
+    pytest.raises(TemplateNotFound, env.get_template, 'oof/bar/missing.html')
 
 
 def test_embedded_package_loader_raised():
     pytest.raises(ValueError, EmbeddedPackageLoader, 'invalid_module')
 
 
 @pytest.mark.parametrize(
     ('template', 'expect'),
     [
         ('foo/test.html', 'FOO'),
         ('foo/bar/x.html', 'YYY'),
+        ('foo/bar/baz/a.html', 'AAA'),
+        ('baz/a/b.html', 'BBB'),
         ('bar/test.html.jinja2', 'BAR'),
         ('test.html', 'BAR'),
     ],
 )
 def test_embedded_package_dir_source(
     embedded_package_loader: EmbeddedPackageLoader,
     template: str,
```

### Comparing `jinja2_embedded-0.1.3/.gitignore` & `jinja2_embedded-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `jinja2_embedded-0.1.3/LICENSE` & `jinja2_embedded-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jinja2_embedded-0.1.3/README.rst` & `jinja2_embedded-0.1.4/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -43,19 +43,23 @@
 
     from jinja2 import Environment, PackageLoader
     from jinja2_embedded import EmbeddedPackageLoader
 
     # before
     env = Environment(
         loader=PackageLoader('my_package', 'templates'),
+        autoescape=True,
+        ...
     )
 
     # after
     env = Environment(
         loader=EmbeddedPackageLoader('my_package.templates'),
+        autoescape=True, # default False, but FastAPI uses True as default
+        extensions=[],
     )
 
     # with FastAPI
     from fastapi.templating import Jinja2Templates
     templates = Jinja2Templates(env=env)
 
 Second, declare the `templates` directory as a module by adding a :code:`__init__.py` file:
```

### Comparing `jinja2_embedded-0.1.3/pyproject.toml` & `jinja2_embedded-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jinja2_embedded-0.1.3/PKG-INFO` & `jinja2_embedded-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jinja2-embedded
-Version: 0.1.3
+Version: 0.1.4
 Summary: Jinja2 template loader for embedded Python runtimes
 Project-URL: Source, https://github.com/GPla/jinja2-embedded
 Author-email: GPla <36087062+GPla@users.noreply.github.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: bundler,embedded,executable,jinja2,pyoxidizer,python
 Classifier: Environment :: Web Environment
@@ -70,19 +70,23 @@
 
     from jinja2 import Environment, PackageLoader
     from jinja2_embedded import EmbeddedPackageLoader
 
     # before
     env = Environment(
         loader=PackageLoader('my_package', 'templates'),
+        autoescape=True,
+        ...
     )
 
     # after
     env = Environment(
         loader=EmbeddedPackageLoader('my_package.templates'),
+        autoescape=True, # default False, but FastAPI uses True as default
+        extensions=[],
     )
 
     # with FastAPI
     from fastapi.templating import Jinja2Templates
     templates = Jinja2Templates(env=env)
 
 Second, declare the `templates` directory as a module by adding a :code:`__init__.py` file:
```

