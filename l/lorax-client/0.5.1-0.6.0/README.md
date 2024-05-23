# Comparing `tmp/lorax_client-0.5.1.tar.gz` & `tmp/lorax_client-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lorax_client-0.5.1.tar", max compression
+gzip compressed data, was "lorax_client-0.6.0.tar", max compression
```

## Comparing `lorax_client-0.5.1.tar` & `lorax_client-0.6.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     6812 2024-05-14 20:26:08.448869 lorax_client-0.5.1/README.md
--rw-r--r--   0        0        0      691 2024-05-16 15:26:04.081010 lorax_client-0.5.1/lorax/__init__.py
--rw-r--r--   0        0        0    26903 2024-05-16 15:25:49.514648 lorax_client-0.5.1/lorax/client.py
--rw-r--r--   0        0        0     2892 2024-05-14 20:26:08.449138 lorax_client-0.5.1/lorax/errors.py
--rw-r--r--   0        0        0    11459 2024-05-14 20:26:08.449197 lorax_client-0.5.1/lorax/types.py
--rw-r--r--   0        0        0      780 2024-05-16 15:26:22.915896 lorax_client-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     7742 1970-01-01 00:00:00.000000 lorax_client-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     6812 2024-05-14 20:26:08.448869 lorax_client-0.6.0/README.md
+-rw-r--r--   0        0        0      691 2024-05-23 16:39:27.127713 lorax_client-0.6.0/lorax/__init__.py
+-rw-r--r--   0        0        0    26903 2024-05-16 15:44:53.935014 lorax_client-0.6.0/lorax/client.py
+-rw-r--r--   0        0        0     2892 2024-05-14 20:26:08.449138 lorax_client-0.6.0/lorax/errors.py
+-rw-r--r--   0        0        0    11459 2024-05-14 20:26:08.449197 lorax_client-0.6.0/lorax/types.py
+-rw-r--r--   0        0        0      780 2024-05-23 16:39:38.173868 lorax_client-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     7692 1970-01-01 00:00:00.000000 lorax_client-0.6.0/PKG-INFO
```

### Comparing `lorax_client-0.5.1/README.md` & `lorax_client-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `lorax_client-0.5.1/lorax/__init__.py` & `lorax_client-0.6.0/lorax/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,10 +8,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.5.1"
+__version__ = "0.6.0"
 
 from lorax.client import Client, AsyncClient, MergedAdapters
```

### Comparing `lorax_client-0.5.1/lorax/client.py` & `lorax_client-0.6.0/lorax/client.py`

 * *Files identical despite different names*

### Comparing `lorax_client-0.5.1/lorax/errors.py` & `lorax_client-0.6.0/lorax/errors.py`

 * *Files identical despite different names*

### Comparing `lorax_client-0.5.1/lorax/types.py` & `lorax_client-0.6.0/lorax/types.py`

 * *Files identical despite different names*

### Comparing `lorax_client-0.5.1/pyproject.toml` & `lorax_client-0.6.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "lorax-client"
 packages = [
     {include = "lorax"}
 ]
-version = "0.5.1"
+version = "0.6.0"
 description = "LoRAX Python Client"
 license = "Apache-2.0"
 authors = ["Travis Addair <travis@predibase.com>", "Olivier Dehaene <olivier@huggingface.co>"]
 maintainers = ["Travis Addair <travis@predibase.com>"]
 readme = "README.md"
 homepage = "https://github.com/predibase/lorax"
 repository = "https://github.com/predibase/lorax"
 
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 pydantic = "> 2, < 3"
-aiohttp = "^3.8"
+aiohttp = "^3.9"
 huggingface-hub = ">= 0.12, < 1.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 pytest-asyncio = "^0.17.2"
 pytest-cov = "^3.0.0"
```

### Comparing `lorax_client-0.5.1/PKG-INFO` & `lorax_client-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: lorax-client
-Version: 0.5.1
+Version: 0.6.0
 Summary: LoRAX Python Client
 Home-page: https://github.com/predibase/lorax
 License: Apache-2.0
 Author: Travis Addair
 Author-email: travis@predibase.com
 Maintainer: Travis Addair
 Maintainer-email: travis@predibase.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: aiohttp (>=3.8,<4.0)
+Requires-Dist: aiohttp (>=3.9,<4.0)
 Requires-Dist: huggingface-hub (>=0.12,<1.0)
 Requires-Dist: pydantic (>2,<3)
 Project-URL: Repository, https://github.com/predibase/lorax
 Description-Content-Type: text/markdown
 
 # LoRAX Python Client
```

