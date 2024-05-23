# Comparing `tmp/wagtail_translatableforms-0.1.2.tar.gz` & `tmp/wagtail_translatableforms-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_translatableforms-0.1.2.tar", max compression
+gzip compressed data, was "wagtail_translatableforms-0.1.3.tar", max compression
```

## Comparing `wagtail_translatableforms-0.1.2.tar` & `wagtail_translatableforms-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1069 2024-05-21 15:01:21.958783 wagtail_translatableforms-0.1.2/LICENSE
--rw-r--r--   0        0        0    10792 2024-05-23 07:15:10.620068 wagtail_translatableforms-0.1.2/README.md
--rw-r--r--   0        0        0      567 2024-05-23 07:16:09.733059 wagtail_translatableforms-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      977 2024-05-22 11:16:42.552643 wagtail_translatableforms-0.1.2/wagtail_translatableforms/__init__.py
--rw-r--r--   0        0        0     4656 2024-05-22 14:05:58.582858 wagtail_translatableforms-0.1.2/wagtail_translatableforms/apps.py
--rw-r--r--   0        0        0     1467 2024-05-22 11:16:42.556643 wagtail_translatableforms-0.1.2/wagtail_translatableforms/blocks.py
--rw-r--r--   0        0        0     8600 2024-05-22 11:16:42.556643 wagtail_translatableforms-0.1.2/wagtail_translatableforms/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-05-22 11:16:42.556643 wagtail_translatableforms-0.1.2/wagtail_translatableforms/migrations/__init__.py
--rw-r--r--   0        0        0     5689 2024-05-22 11:16:42.560643 wagtail_translatableforms-0.1.2/wagtail_translatableforms/models.py
--rw-r--r--   0        0        0     1777 2024-05-22 11:32:03.624558 wagtail_translatableforms-0.1.2/wagtail_translatableforms/serializers.py
--rw-r--r--   0        0        0     1046 2024-05-22 11:16:42.564643 wagtail_translatableforms-0.1.2/wagtail_translatableforms/templates/customforms/confirm_delete.html
--rw-r--r--   0        0        0     4945 2024-05-22 11:16:42.564643 wagtail_translatableforms-0.1.2/wagtail_translatableforms/templates/customforms/index.html
--rw-r--r--   0        0        0     4124 2024-05-22 11:16:42.564643 wagtail_translatableforms-0.1.2/wagtail_translatableforms/templates/customforms/index_submissions.html
--rw-r--r--   0        0        0     1047 2024-05-22 11:16:42.564643 wagtail_translatableforms-0.1.2/wagtail_translatableforms/templates/customforms/result_list.html
--rw-r--r--   0        0        0        0 2024-05-22 11:16:42.564643 wagtail_translatableforms-0.1.2/wagtail_translatableforms/templatetags/__init__.py
--rw-r--r--   0        0        0     4593 2024-05-22 11:16:42.568643 wagtail_translatableforms-0.1.2/wagtail_translatableforms/templatetags/custom_tags.py
--rw-r--r--   0        0        0      405 2024-05-22 11:16:42.568643 wagtail_translatableforms-0.1.2/wagtail_translatableforms/urls.py
--rw-r--r--   0        0        0     1155 2024-05-22 11:16:42.568643 wagtail_translatableforms-0.1.2/wagtail_translatableforms/utils.py
--rw-r--r--   0        0        0     4137 2024-05-22 11:16:42.568643 wagtail_translatableforms-0.1.2/wagtail_translatableforms/views.py
--rw-r--r--   0        0        0    11597 1970-01-01 00:00:00.000000 wagtail_translatableforms-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-21 15:01:21.958783 wagtail_translatableforms-0.1.3/LICENSE
+-rw-r--r--   0        0        0    11000 2024-05-23 07:19:51.032650 wagtail_translatableforms-0.1.3/README.md
+-rw-r--r--   0        0        0      567 2024-05-23 07:20:26.005159 wagtail_translatableforms-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      977 2024-05-22 11:16:42.552643 wagtail_translatableforms-0.1.3/wagtail_translatableforms/__init__.py
+-rw-r--r--   0        0        0     4656 2024-05-22 14:05:58.582858 wagtail_translatableforms-0.1.3/wagtail_translatableforms/apps.py
+-rw-r--r--   0        0        0     1467 2024-05-22 11:16:42.556643 wagtail_translatableforms-0.1.3/wagtail_translatableforms/blocks.py
+-rw-r--r--   0        0        0     8600 2024-05-22 11:16:42.556643 wagtail_translatableforms-0.1.3/wagtail_translatableforms/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-05-22 11:16:42.556643 wagtail_translatableforms-0.1.3/wagtail_translatableforms/migrations/__init__.py
+-rw-r--r--   0        0        0     5689 2024-05-22 11:16:42.560643 wagtail_translatableforms-0.1.3/wagtail_translatableforms/models.py
+-rw-r--r--   0        0        0     1777 2024-05-22 11:32:03.624558 wagtail_translatableforms-0.1.3/wagtail_translatableforms/serializers.py
+-rw-r--r--   0        0        0     1046 2024-05-22 11:16:42.564643 wagtail_translatableforms-0.1.3/wagtail_translatableforms/templates/customforms/confirm_delete.html
+-rw-r--r--   0        0        0     4945 2024-05-22 11:16:42.564643 wagtail_translatableforms-0.1.3/wagtail_translatableforms/templates/customforms/index.html
+-rw-r--r--   0        0        0     4124 2024-05-22 11:16:42.564643 wagtail_translatableforms-0.1.3/wagtail_translatableforms/templates/customforms/index_submissions.html
+-rw-r--r--   0        0        0     1047 2024-05-22 11:16:42.564643 wagtail_translatableforms-0.1.3/wagtail_translatableforms/templates/customforms/result_list.html
+-rw-r--r--   0        0        0        0 2024-05-22 11:16:42.564643 wagtail_translatableforms-0.1.3/wagtail_translatableforms/templatetags/__init__.py
+-rw-r--r--   0        0        0     4593 2024-05-22 11:16:42.568643 wagtail_translatableforms-0.1.3/wagtail_translatableforms/templatetags/custom_tags.py
+-rw-r--r--   0        0        0      405 2024-05-22 11:16:42.568643 wagtail_translatableforms-0.1.3/wagtail_translatableforms/urls.py
+-rw-r--r--   0        0        0     1155 2024-05-22 11:16:42.568643 wagtail_translatableforms-0.1.3/wagtail_translatableforms/utils.py
+-rw-r--r--   0        0        0     4137 2024-05-22 11:16:42.568643 wagtail_translatableforms-0.1.3/wagtail_translatableforms/views.py
+-rw-r--r--   0        0        0    11805 1970-01-01 00:00:00.000000 wagtail_translatableforms-0.1.3/PKG-INFO
```

### Comparing `wagtail_translatableforms-0.1.2/LICENSE` & `wagtail_translatableforms-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.2/README.md` & `wagtail_translatableforms-0.1.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 * WAGTAIL_TRANSLATABLEFORM_FORM_MODEL = 'app.Model' (pass variable only in case of subclassing 'AbstractTranslatableForm');
 * WAGTAIL_TRANSLATABLEFORM_SHOW_IP = True/False (add client IP in forms submissions representation, get IP from request.headers["X-Real-Ip"]. Pass Django Request object to 'process_form_submission' in your code. Default to False).
 
 ## License
 This project is licensed under the [MIT License](https://github.com/BenderEg/wagtail-translatableforms/blob/main/LICENSE).
 
 
-We use Wagtail Localize, below is a quote from their license agreement:
+We use [Wagtail Localize](https://pypi.org/project/wagtail-localize/), below is a quote from their license agreement:
 
 ```
 Copyright (c) 2018-present Torchbox Ltd and individual contributors.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification,
 are permitted provided that the following conditions are met:
@@ -118,15 +118,15 @@
 BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
 DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY
 OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED
 OF THE POSSIBILITY OF SUCH DAMAGE.
 ```
 
-We use drf-spectacular, below is a quote from their license agreement:
+We use [drf-spectacular](https://github.com/tfranzel/drf-spectacular/), below is a quote from their license agreement:
 
 ```
 Copyright © 2011-present, Encode OSS Ltd.
 Copyright © 2019-2021, T. Franzel <tfranzel@gmail.com>, Cashlink Technologies GmbH.
 Copyright © 2021-present, T. Franzel <tfranzel@gmail.com>.
 
 All rights reserved.
@@ -153,15 +153,15 @@
 DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 ```
 
-We use Django, below is a quote from their license agreement:
+We use [Django](https://www.djangoproject.com/), below is a quote from their license agreement:
 
 ```
 Copyright (c) Django Software Foundation and individual contributors.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification,
 are permitted provided that the following conditions are met:
@@ -185,15 +185,15 @@
 (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
 ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 ```
 
-We use Wagtail, below is a quote from their license agreement:
+We use [Wagtail CMS](https://wagtail.org/), below is a quote from their license agreement:
 
 ```
 Copyright (c) 2014-present Torchbox Ltd and individual contributors.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification,
 are permitted provided that the following conditions are met:
@@ -217,15 +217,15 @@
 (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
 ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 ```
 
-We use Django-Rest-Framework, below is a quote from their license agreement:
+We use [Django-Rest-Framework](https://github.com/encode/django-rest-framework/), below is a quote from their license agreement:
 
 ```
 Copyright © 2011-present, Encode OSS Ltd. All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
     Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
```

### Comparing `wagtail_translatableforms-0.1.2/pyproject.toml` & `wagtail_translatableforms-0.1.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "wagtail_translatableforms"
-version = "0.1.2"
+version = "0.1.3"
 description = "Add translatableforms to wagtail projects"
 authors = ["Egor Nikitin <eanikitin90@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/BenderEg/wagtail-translatableforms"
 license = "MIT"
 
 [tool.poetry.dependencies]
```

### Comparing `wagtail_translatableforms-0.1.2/wagtail_translatableforms/__init__.py` & `wagtail_translatableforms-0.1.3/wagtail_translatableforms/__init__.py`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.2/wagtail_translatableforms/apps.py` & `wagtail_translatableforms-0.1.3/wagtail_translatableforms/apps.py`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.2/wagtail_translatableforms/blocks.py` & `wagtail_translatableforms-0.1.3/wagtail_translatableforms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.2/wagtail_translatableforms/migrations/0001_initial.py` & `wagtail_translatableforms-0.1.3/wagtail_translatableforms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.2/wagtail_translatableforms/models.py` & `wagtail_translatableforms-0.1.3/wagtail_translatableforms/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.2/wagtail_translatableforms/serializers.py` & `wagtail_translatableforms-0.1.3/wagtail_translatableforms/serializers.py`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.2/wagtail_translatableforms/templates/customforms/confirm_delete.html` & `wagtail_translatableforms-0.1.3/wagtail_translatableforms/templates/customforms/confirm_delete.html`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.2/wagtail_translatableforms/templates/customforms/index.html` & `wagtail_translatableforms-0.1.3/wagtail_translatableforms/templates/customforms/index.html`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.2/wagtail_translatableforms/templates/customforms/index_submissions.html` & `wagtail_translatableforms-0.1.3/wagtail_translatableforms/templates/customforms/index_submissions.html`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.2/wagtail_translatableforms/templates/customforms/result_list.html` & `wagtail_translatableforms-0.1.3/wagtail_translatableforms/templates/customforms/result_list.html`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.2/wagtail_translatableforms/templatetags/custom_tags.py` & `wagtail_translatableforms-0.1.3/wagtail_translatableforms/templatetags/custom_tags.py`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.2/wagtail_translatableforms/utils.py` & `wagtail_translatableforms-0.1.3/wagtail_translatableforms/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.2/wagtail_translatableforms/views.py` & `wagtail_translatableforms-0.1.3/wagtail_translatableforms/views.py`

 * *Files identical despite different names*

### Comparing `wagtail_translatableforms-0.1.2/PKG-INFO` & `wagtail_translatableforms-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_translatableforms
-Version: 0.1.2
+Version: 0.1.3
 Summary: Add translatableforms to wagtail projects
 Home-page: https://github.com/BenderEg/wagtail-translatableforms
 License: MIT
 Author: Egor Nikitin
 Author-email: eanikitin90@gmail.com
 Requires-Python: >=3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -107,15 +107,15 @@
 * WAGTAIL_TRANSLATABLEFORM_FORM_MODEL = 'app.Model' (pass variable only in case of subclassing 'AbstractTranslatableForm');
 * WAGTAIL_TRANSLATABLEFORM_SHOW_IP = True/False (add client IP in forms submissions representation, get IP from request.headers["X-Real-Ip"]. Pass Django Request object to 'process_form_submission' in your code. Default to False).
 
 ## License
 This project is licensed under the [MIT License](https://github.com/BenderEg/wagtail-translatableforms/blob/main/LICENSE).
 
 
-We use Wagtail Localize, below is a quote from their license agreement:
+We use [Wagtail Localize](https://pypi.org/project/wagtail-localize/), below is a quote from their license agreement:
 
 ```
 Copyright (c) 2018-present Torchbox Ltd and individual contributors.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification,
 are permitted provided that the following conditions are met:
@@ -139,15 +139,15 @@
 BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
 DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY
 OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED
 OF THE POSSIBILITY OF SUCH DAMAGE.
 ```
 
-We use drf-spectacular, below is a quote from their license agreement:
+We use [drf-spectacular](https://github.com/tfranzel/drf-spectacular/), below is a quote from their license agreement:
 
 ```
 Copyright © 2011-present, Encode OSS Ltd.
 Copyright © 2019-2021, T. Franzel <tfranzel@gmail.com>, Cashlink Technologies GmbH.
 Copyright © 2021-present, T. Franzel <tfranzel@gmail.com>.
 
 All rights reserved.
@@ -174,15 +174,15 @@
 DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 ```
 
-We use Django, below is a quote from their license agreement:
+We use [Django](https://www.djangoproject.com/), below is a quote from their license agreement:
 
 ```
 Copyright (c) Django Software Foundation and individual contributors.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification,
 are permitted provided that the following conditions are met:
@@ -206,15 +206,15 @@
 (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
 ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 ```
 
-We use Wagtail, below is a quote from their license agreement:
+We use [Wagtail CMS](https://wagtail.org/), below is a quote from their license agreement:
 
 ```
 Copyright (c) 2014-present Torchbox Ltd and individual contributors.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification,
 are permitted provided that the following conditions are met:
@@ -238,15 +238,15 @@
 (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
 ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 ```
 
-We use Django-Rest-Framework, below is a quote from their license agreement:
+We use [Django-Rest-Framework](https://github.com/encode/django-rest-framework/), below is a quote from their license agreement:
 
 ```
 Copyright © 2011-present, Encode OSS Ltd. All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
     Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
```

