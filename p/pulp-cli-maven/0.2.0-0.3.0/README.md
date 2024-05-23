# Comparing `tmp/pulp-cli-maven-0.2.0.tar.gz` & `tmp/pulp-cli-maven-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulp-cli-maven-0.2.0.tar", last modified: Fri Mar 17 10:03:31 2023, max compression
+gzip compressed data, was "pulp-cli-maven-0.3.0.tar", last modified: Thu May 23 10:00:16 2024, max compression
```

## Comparing `pulp-cli-maven-0.2.0.tar` & `pulp-cli-maven-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:03:31.615516 pulp-cli-maven-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-03-17 10:03:31.615516 pulp-cli-maven-0.2.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:03:31.615516 pulp-cli-maven-0.2.0/pulp_cli_maven.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-03-17 10:03:31.000000 pulp-cli-maven-0.2.0/pulp_cli_maven.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-17 10:03:31.000000 pulp-cli-maven-0.2.0/pulp_cli_maven.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 10:03:31.000000 pulp-cli-maven-0.2.0/pulp_cli_maven.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-17 10:03:31.000000 pulp-cli-maven-0.2.0/pulp_cli_maven.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-17 10:03:31.000000 pulp-cli-maven-0.2.0/pulp_cli_maven.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-17 10:03:31.000000 pulp-cli-maven-0.2.0/pulp_cli_maven.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:03:31.615516 pulp-cli-maven-0.2.0/pulpcore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:03:31.615516 pulp-cli-maven-0.2.0/pulpcore/cli/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 10:03:31.615516 pulp-cli-maven-0.2.0/pulpcore/cli/maven/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-03-17 10:03:13.000000 pulp-cli-maven-0.2.0/pulpcore/cli/maven/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-03-17 10:03:13.000000 pulp-cli-maven-0.2.0/pulpcore/cli/maven/distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-03-17 10:03:13.000000 pulp-cli-maven-0.2.0/pulpcore/cli/maven/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-03-17 10:03:13.000000 pulp-cli-maven-0.2.0/pulpcore/cli/maven/repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-03-17 10:03:13.000000 pulp-cli-maven-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-17 10:03:31.615516 pulp-cli-maven-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-03-17 10:03:13.000000 pulp-cli-maven-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:00:16.032311 pulp-cli-maven-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-23 10:00:16.028311 pulp-cli-maven-0.3.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:00:16.028311 pulp-cli-maven-0.3.0/pulp_cli_maven.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-23 10:00:16.000000 pulp-cli-maven-0.3.0/pulp_cli_maven.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-23 10:00:16.000000 pulp-cli-maven-0.3.0/pulp_cli_maven.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 10:00:16.000000 pulp-cli-maven-0.3.0/pulp_cli_maven.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 10:00:16.000000 pulp-cli-maven-0.3.0/pulp_cli_maven.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-23 10:00:16.000000 pulp-cli-maven-0.3.0/pulp_cli_maven.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-23 10:00:16.000000 pulp-cli-maven-0.3.0/pulp_cli_maven.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:00:16.028311 pulp-cli-maven-0.3.0/pulpcore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:00:16.028311 pulp-cli-maven-0.3.0/pulpcore/cli/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:00:16.028311 pulp-cli-maven-0.3.0/pulpcore/cli/maven/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-23 10:00:06.000000 pulp-cli-maven-0.3.0/pulpcore/cli/maven/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-05-23 10:00:06.000000 pulp-cli-maven-0.3.0/pulpcore/cli/maven/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-23 10:00:06.000000 pulp-cli-maven-0.3.0/pulpcore/cli/maven/remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-05-23 10:00:06.000000 pulp-cli-maven-0.3.0/pulpcore/cli/maven/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-05-23 10:00:06.000000 pulp-cli-maven-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 10:00:16.032311 pulp-cli-maven-0.3.0/setup.cfg
```

### Comparing `pulp-cli-maven-0.2.0/pulpcore/cli/maven/__init__.py` & `pulp-cli-maven-0.3.0/pulpcore/cli/maven/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from pulpcore.cli.maven.distribution import distribution
 from pulpcore.cli.maven.remote import remote
 from pulpcore.cli.maven.repository import repository
 
 translation = get_translation(__name__)
 _ = translation.gettext
 
-__version__ = "0.2.0"
+__version__ = "0.3.0"
 
 
 @pulp_group(name="maven")
 def maven_group() -> None:
     pass
```

### Comparing `pulp-cli-maven-0.2.0/pulpcore/cli/maven/distribution.py` & `pulp-cli-maven-0.3.0/pulpcore/cli/maven/distribution.py`

 * *Files identical despite different names*

### Comparing `pulp-cli-maven-0.2.0/pulpcore/cli/maven/remote.py` & `pulp-cli-maven-0.3.0/pulpcore/cli/maven/remote.py`

 * *Files identical despite different names*

### Comparing `pulp-cli-maven-0.2.0/pulpcore/cli/maven/repository.py` & `pulp-cli-maven-0.3.0/pulpcore/cli/maven/repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from typing import Any, Dict
+import typing as t
 
 import click
-from pulp_glue.common.context import EntityFieldDefinition, PulpRemoteContext
+from pulp_glue.common.context import EntityFieldDefinition, PulpRemoteContext, PulpRepositoryContext
 from pulp_glue.common.i18n import get_translation
 from pulp_glue.maven.context import PulpMavenArtifactContentContext, PulpMavenRepositoryContext
 from pulpcore.cli.common.generic import (
     PulpCLIContext,
     create_command,
     destroy_command,
     href_option,
@@ -89,23 +89,25 @@
 @repository.command()
 @name_option
 @href_option
 @repository_lookup_option
 @remote_option
 @pass_repository_context
 def add_cached_content(
-    repository_ctx: PulpMavenRepositoryContext,
+    repository_ctx: PulpRepositoryContext,
     remote: EntityFieldDefinition,
 ) -> None:
     """
     Add cached Maven content to the repository. The remote is used to identify which
     content created by pulpcore-content to add to the repository. If a remote is not
     specified, the remote associated with the repository will be used.
     """
-    body: Dict[str, Any] = {}
+    assert isinstance(repository_ctx, PulpMavenRepositoryContext)
+
+    body: t.Dict[str, t.Any] = {}
     repository = repository_ctx.entity
 
     if remote:
         body["remote"] = remote
     elif repository["remote"] is None:
         raise click.ClickException(
             _(
```

