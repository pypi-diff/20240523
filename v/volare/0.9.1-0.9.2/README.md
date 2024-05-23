# Comparing `tmp/volare-0.9.1.tar.gz` & `tmp/volare-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/volare-0.9.1.tar", last modified: Thu Jul 20 23:05:07 2023, max compression
+gzip compressed data, was "dist/volare-0.9.2.tar", last modified: Mon Jul 24 11:26:07 2023, max compression
```

## Comparing `volare-0.9.1.tar` & `volare-0.9.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 23:05:07.000000 volare-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-20 23:05:07.000000 volare-0.9.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 23:05:07.000000 volare-0.9.1/volare/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 23:05:07.000000 volare-0.9.1/volare/build/
--rw-r--r--   0 runner    (1001) docker     (122)     7450 2023-07-20 23:04:52.000000 volare-0.9.1/volare/build/git_multi_clone.py
--rw-r--r--   0 runner    (1001) docker     (122)     6730 2023-07-20 23:04:52.000000 volare-0.9.1/volare/build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3559 2023-07-20 23:04:52.000000 volare-0.9.1/volare/build/magic.py
--rw-r--r--   0 runner    (1001) docker     (122)    14117 2023-07-20 23:04:52.000000 volare-0.9.1/volare/build/sky130.py
--rw-r--r--   0 runner    (1001) docker     (122)     9206 2023-07-20 23:04:52.000000 volare-0.9.1/volare/build/gf180mcu.py
--rw-r--r--   0 runner    (1001) docker     (122)     4897 2023-07-20 23:04:52.000000 volare-0.9.1/volare/build/asap7.py
--rw-r--r--   0 runner    (1001) docker     (122)     2236 2023-07-20 23:04:52.000000 volare-0.9.1/volare/families.py
--rw-r--r--   0 runner    (1001) docker     (122)      783 2023-07-20 23:04:52.000000 volare-0.9.1/volare/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      671 2023-07-20 23:04:52.000000 volare-0.9.1/volare/__version__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 23:04:52.000000 volare-0.9.1/volare/py.typed
--rwxr-xr-x   0 runner    (1001) docker     (122)     8810 2023-07-20 23:04:52.000000 volare-0.9.1/volare/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3654 2023-07-20 23:04:52.000000 volare-0.9.1/volare/click_common.py
--rw-r--r--   0 runner    (1001) docker     (122)    10607 2023-07-20 23:04:52.000000 volare-0.9.1/volare/common.py
--rw-r--r--   0 runner    (1001) docker     (122)     8838 2023-07-20 23:04:52.000000 volare-0.9.1/volare/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 23:05:07.000000 volare-0.9.1/volare.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 23:05:07.000000 volare-0.9.1/volare.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      491 2023-07-20 23:05:07.000000 volare-0.9.1/volare.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-07-20 23:05:07.000000 volare-0.9.1/volare.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-07-20 23:05:07.000000 volare-0.9.1/volare.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     8665 2023-07-20 23:05:07.000000 volare-0.9.1/volare.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       96 2023-07-20 23:05:07.000000 volare-0.9.1/volare.egg-info/requires.txt
--rwxr-xr-x   0 runner    (1001) docker     (122)      931 2023-07-20 23:04:52.000000 volare-0.9.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)     8665 2023-07-20 23:05:07.000000 volare-0.9.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 11:26:07.000000 volare-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-24 11:26:07.000000 volare-0.9.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 11:26:07.000000 volare-0.9.2/volare/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 11:26:07.000000 volare-0.9.2/volare/build/
+-rw-r--r--   0 runner    (1001) docker     (122)     7450 2023-07-24 11:25:48.000000 volare-0.9.2/volare/build/git_multi_clone.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6730 2023-07-24 11:25:48.000000 volare-0.9.2/volare/build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3559 2023-07-24 11:25:48.000000 volare-0.9.2/volare/build/magic.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14117 2023-07-24 11:25:48.000000 volare-0.9.2/volare/build/sky130.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9206 2023-07-24 11:25:48.000000 volare-0.9.2/volare/build/gf180mcu.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4897 2023-07-24 11:25:48.000000 volare-0.9.2/volare/build/asap7.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2236 2023-07-24 11:25:48.000000 volare-0.9.2/volare/families.py
+-rw-r--r--   0 runner    (1001) docker     (122)      783 2023-07-24 11:25:48.000000 volare-0.9.2/volare/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      671 2023-07-24 11:25:48.000000 volare-0.9.2/volare/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-24 11:25:48.000000 volare-0.9.2/volare/py.typed
+-rwxr-xr-x   0 runner    (1001) docker     (122)     8880 2023-07-24 11:25:48.000000 volare-0.9.2/volare/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3654 2023-07-24 11:25:48.000000 volare-0.9.2/volare/click_common.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10607 2023-07-24 11:25:48.000000 volare-0.9.2/volare/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8838 2023-07-24 11:25:48.000000 volare-0.9.2/volare/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 11:26:07.000000 volare-0.9.2/volare.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-24 11:26:07.000000 volare-0.9.2/volare.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      491 2023-07-24 11:26:07.000000 volare-0.9.2/volare.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-07-24 11:26:07.000000 volare-0.9.2/volare.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-07-24 11:26:07.000000 volare-0.9.2/volare.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     8665 2023-07-24 11:26:07.000000 volare-0.9.2/volare.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       96 2023-07-24 11:26:07.000000 volare-0.9.2/volare.egg-info/requires.txt
+-rwxr-xr-x   0 runner    (1001) docker     (122)      931 2023-07-24 11:25:48.000000 volare-0.9.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8665 2023-07-24 11:26:07.000000 volare-0.9.2/PKG-INFO
```

### Comparing `volare-0.9.1/volare/build/git_multi_clone.py` & `volare-0.9.2/volare/build/git_multi_clone.py`

 * *Files identical despite different names*

### Comparing `volare-0.9.1/volare/build/__init__.py` & `volare-0.9.2/volare/build/__init__.py`

 * *Files identical despite different names*

### Comparing `volare-0.9.1/volare/build/magic.py` & `volare-0.9.2/volare/build/magic.py`

 * *Files identical despite different names*

### Comparing `volare-0.9.1/volare/build/sky130.py` & `volare-0.9.2/volare/build/sky130.py`

 * *Files identical despite different names*

### Comparing `volare-0.9.1/volare/build/gf180mcu.py` & `volare-0.9.2/volare/build/gf180mcu.py`

 * *Files identical despite different names*

### Comparing `volare-0.9.1/volare/build/asap7.py` & `volare-0.9.2/volare/build/asap7.py`

 * *Files identical despite different names*

### Comparing `volare-0.9.1/volare/families.py` & `volare-0.9.2/volare/families.py`

 * *Files identical despite different names*

### Comparing `volare-0.9.1/volare/__init__.py` & `volare-0.9.2/volare/__init__.py`

 * *Files identical despite different names*

### Comparing `volare-0.9.1/volare/__version__.py` & `volare-0.9.2/volare/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,11 +7,11 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-__version__ = "0.9.1"
+__version__ = "0.9.2"
 
 if __name__ == "__main__":
     print(__version__, end="")
```

### Comparing `volare-0.9.1/volare/__main__.py` & `volare-0.9.2/volare/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,14 +231,15 @@
     pre,
     clear_build_artifacts,
     tool_metadata_file_path,
     also_push,
     version,
     use_repo_at,
     build_magic,
+    push_libraries,
 ):
     """
     Attempts to activate a given PDK version. If the version is not found locally or remotely,
     it will instead attempt to build said version.
 
     Parameters: <version>
     """
@@ -262,14 +263,15 @@
                 "build_magic": build_magic,
             },
             push_kwargs={
                 "owner": owner,
                 "repository": repository,
                 "token": token,
                 "pre": pre,
+                "push_libraries": push_libraries,
             },
             include_libraries=include_libraries,
             output=console,
         )
     except Exception as e:
         console.print(f"[red]{e}")
         exit(-1)
```

### Comparing `volare-0.9.1/volare/click_common.py` & `volare-0.9.2/volare/click_common.py`

 * *Files identical despite different names*

### Comparing `volare-0.9.1/volare/common.py` & `volare-0.9.2/volare/common.py`

 * *Files identical despite different names*

### Comparing `volare-0.9.1/volare/manage.py` & `volare-0.9.2/volare/manage.py`

 * *Files identical despite different names*

### Comparing `volare-0.9.1/volare.egg-info/PKG-INFO` & `volare-0.9.2/volare.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volare
-Version: 0.9.1
+Version: 0.9.2
 Summary: An open_pdks PDK builder/version manager
 Home-page: UNKNOWN
 Author: Efabless Corporation
 Author-email: donn@efabless.com
 License: UNKNOWN
 Description: <h1 align="center">⛰️ Volare</h1>
         <p align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: volare Version: 0.9.1 Summary: An open_pdks PDK
+Metadata-Version: 2.1 Name: volare Version: 0.9.2 Summary: An open_pdks PDK
 builder/version manager Home-page: UNKNOWN Author: Efabless Corporation Author-
 email: donn@efabless.com License: UNKNOWN Description:
                           ************ ?â??°?ï?¸? VVoollaarree ************
 _[_L_i_c_e_n_s_e_:_ _A_p_a_c_h_e_ _2_._0_][CI Status]_[_I_n_v_i_t_e_ _t_o_ _t_h_e_ _S_k_y_w_a_t_e_r_ _P_D_K_ _S_l_a_c_k_]_[_C_o_d_e_ _S_t_y_l_e_:
                                     _B_l_a_c_k_]
 Volare is a version manager (and builder) for builds of _G_o_o_g_l_e_ _o_p_e_n_-_s_o_u_r_c_e_ _P_D_K_s
                                using _o_p_e_n___p_d_k_s.
```

### Comparing `volare-0.9.1/setup.py` & `volare-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `volare-0.9.1/PKG-INFO` & `volare-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volare
-Version: 0.9.1
+Version: 0.9.2
 Summary: An open_pdks PDK builder/version manager
 Home-page: UNKNOWN
 Author: Efabless Corporation
 Author-email: donn@efabless.com
 License: UNKNOWN
 Description: <h1 align="center">⛰️ Volare</h1>
         <p align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: volare Version: 0.9.1 Summary: An open_pdks PDK
+Metadata-Version: 2.1 Name: volare Version: 0.9.2 Summary: An open_pdks PDK
 builder/version manager Home-page: UNKNOWN Author: Efabless Corporation Author-
 email: donn@efabless.com License: UNKNOWN Description:
                           ************ ?â??°?ï?¸? VVoollaarree ************
 _[_L_i_c_e_n_s_e_:_ _A_p_a_c_h_e_ _2_._0_][CI Status]_[_I_n_v_i_t_e_ _t_o_ _t_h_e_ _S_k_y_w_a_t_e_r_ _P_D_K_ _S_l_a_c_k_]_[_C_o_d_e_ _S_t_y_l_e_:
                                     _B_l_a_c_k_]
 Volare is a version manager (and builder) for builds of _G_o_o_g_l_e_ _o_p_e_n_-_s_o_u_r_c_e_ _P_D_K_s
                                using _o_p_e_n___p_d_k_s.
```

