# Comparing `tmp/hyper-v-2.0.2.tar.gz` & `tmp/hyper_v-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyper-v-2.0.2.tar", last modified: Fri Nov 10 05:54:32 2023, max compression
+gzip compressed data, was "hyper_v-2.0.3.tar", last modified: Thu May 23 05:22:11 2024, max compression
```

## Comparing `hyper-v-2.0.2.tar` & `hyper_v-2.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2023-11-10 05:54:32.318599 hyper-v-2.0.2/
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     1681 2023-11-10 05:54:32.318599 hyper-v-2.0.2/PKG-INFO
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     1193 2023-01-19 14:36:04.000000 hyper-v-2.0.2/README.md
-drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2023-11-10 05:54:32.318599 hyper-v-2.0.2/hyper_v.egg-info/
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     1681 2023-11-10 05:54:32.000000 hyper-v-2.0.2/hyper_v.egg-info/PKG-INFO
--rw-rw-r--   0 viktor    (1000) viktor    (1000)      222 2023-11-10 05:54:32.000000 hyper-v-2.0.2/hyper_v.egg-info/SOURCES.txt
--rw-rw-r--   0 viktor    (1000) viktor    (1000)        1 2023-11-10 05:54:32.000000 hyper-v-2.0.2/hyper_v.egg-info/dependency_links.txt
--rw-rw-r--   0 viktor    (1000) viktor    (1000)       34 2023-11-10 05:54:32.000000 hyper-v-2.0.2/hyper_v.egg-info/requires.txt
--rw-rw-r--   0 viktor    (1000) viktor    (1000)        7 2023-11-10 05:54:32.000000 hyper-v-2.0.2/hyper_v.egg-info/top_level.txt
-drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2023-11-10 05:54:32.318599 hyper-v-2.0.2/hyperv/
--rw-rw-r--   0 viktor    (1000) viktor    (1000)       51 2023-03-10 13:25:12.000000 hyper-v-2.0.2/hyperv/__init__.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)    13584 2023-11-10 05:53:04.000000 hyper-v-2.0.2/hyperv/hyperv.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)     1087 2023-03-15 11:14:27.000000 hyper-v-2.0.2/hyperv/net.py
--rw-rw-r--   0 viktor    (1000) viktor    (1000)       38 2023-11-10 05:54:32.318599 hyper-v-2.0.2/setup.cfg
--rw-rw-r--   0 viktor    (1000) viktor    (1000)      841 2023-11-10 05:53:34.000000 hyper-v-2.0.2/setup.py
+drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2024-05-23 05:22:11.168002 hyper_v-2.0.3/
+-rw-r--r--   0 viktor    (1000) viktor    (1000)     1709 2024-05-23 05:22:11.168002 hyper_v-2.0.3/PKG-INFO
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     1193 2023-01-19 14:36:04.000000 hyper_v-2.0.3/README.md
+drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2024-05-23 05:22:11.164002 hyper_v-2.0.3/hyper_v.egg-info/
+-rw-r--r--   0 viktor    (1000) viktor    (1000)     1709 2024-05-23 05:22:11.000000 hyper_v-2.0.3/hyper_v.egg-info/PKG-INFO
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)      222 2024-05-23 05:22:11.000000 hyper_v-2.0.3/hyper_v.egg-info/SOURCES.txt
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)        1 2024-05-23 05:22:11.000000 hyper_v-2.0.3/hyper_v.egg-info/dependency_links.txt
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)       34 2024-05-23 05:22:11.000000 hyper_v-2.0.3/hyper_v.egg-info/requires.txt
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)        7 2024-05-23 05:22:11.000000 hyper_v-2.0.3/hyper_v.egg-info/top_level.txt
+drwxrwxr-x   0 viktor    (1000) viktor    (1000)        0 2024-05-23 05:22:11.164002 hyper_v-2.0.3/hyperv/
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)       51 2023-03-10 13:25:12.000000 hyper_v-2.0.3/hyperv/__init__.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)    14278 2024-05-23 05:18:13.000000 hyper_v-2.0.3/hyperv/hyperv.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)     1087 2023-03-15 11:14:27.000000 hyper_v-2.0.3/hyperv/net.py
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)       38 2024-05-23 05:22:11.168002 hyper_v-2.0.3/setup.cfg
+-rw-rw-r--   0 viktor    (1000) viktor    (1000)      841 2024-05-23 05:18:43.000000 hyper_v-2.0.3/setup.py
```

### Comparing `hyper-v-2.0.2/PKG-INFO` & `hyper_v-2.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: hyper-v
-Version: 2.0.2
+Version: 2.0.3
 Summary: Удаленное управление Hyper-V через winrm
 Home-page: https://github.com/viktor-gorinskiy/hyper-v
 Author: Viktor Gorinskiy
 Author-email: viktor@gorinskiy.ru
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Requires-Dist: pywinrm==0.4.3
+Requires-Dist: python-nmap==0.7.1
 
 # Hyper-V winrm python
 
 На данный момент можно создавать виртуальные машины только через заранее подготовленный шаблон виртуальноф машины.
 
 
 ## Installation
@@ -48,8 +48,7 @@
 * `host`    -   Hyper-V хост 
 * `user`    - Имя пользователя для доступа по winrm
 * `password`    - Пароль пользователя для доступа по winrm
 
 ## License
 
 [GPL-3.0](LICENSE)
-
```

### Comparing `hyper-v-2.0.2/README.md` & `hyper_v-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `hyper-v-2.0.2/hyper_v.egg-info/PKG-INFO` & `hyper_v-2.0.3/hyper_v.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: hyper-v
-Version: 2.0.2
+Version: 2.0.3
 Summary: Удаленное управление Hyper-V через winrm
 Home-page: https://github.com/viktor-gorinskiy/hyper-v
 Author: Viktor Gorinskiy
 Author-email: viktor@gorinskiy.ru
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Requires-Dist: pywinrm==0.4.3
+Requires-Dist: python-nmap==0.7.1
 
 # Hyper-V winrm python
 
 На данный момент можно создавать виртуальные машины только через заранее подготовленный шаблон виртуальноф машины.
 
 
 ## Installation
@@ -48,8 +48,7 @@
 * `host`    -   Hyper-V хост 
 * `user`    - Имя пользователя для доступа по winrm
 * `password`    - Пароль пользователя для доступа по winrm
 
 ## License
 
 [GPL-3.0](LICENSE)
-
```

### Comparing `hyper-v-2.0.2/hyperv/hyperv.py` & `hyper_v-2.0.3/hyperv/hyperv.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,14 +232,15 @@
     
     # Генерирует PS более/менее стандартные скрипты
     def gen_job(self, job, vms_list=[], **kwargs):
         params = ''
         if kwargs:
             if 'create_snapshot' in kwargs.keys(): params = f"-SnapshotName {kwargs['create_snapshot']}"
             if 'get_snapshot' in kwargs.keys(): params = f"| Get-VMSnapshot"
+            if 'get_json_snapshot' in kwargs.keys(): params = f"| Get-VMSnapshot | ConvertTo-Json"
             if 'current_snapshot' in kwargs.keys(): params = f"| select Name, ParentSnapshotName"
             if 'dellete_snapshots' in kwargs.keys(): params = f"| Remove-VMSnapshot -Name {kwargs['dellete_snapshots']}"
             if 'apply_snapshots' in kwargs.keys(): params = f"| Restore-VMSnapshot -Name  {kwargs['apply_snapshots']} -Confirm:$false"
             
             if 'force' in kwargs.keys():
                 params = '-Force'
 
@@ -279,15 +280,26 @@
         if not r:
             return False
         for line in r[0].splitlines():
             if line:
                 # r_result.setdefault(line.split()[0], []).append(line.split()[1:])
                 r_result.setdefault(line.split()[0], []).append(dict(zip(state_keys, (line.split()[1:]))))
         return r_result
-
+    
+    # Список снапшотов виртуалных машин 
+    def get_json_snapshot(self, vms=[]):
+        state_keys = ['name', 'type', 'creation_date', 'creation_time', 'parent_snapshot' ]
+        ps_script = self.gen_job(vms_list=vms, job='Get-VM', get_snapshot = True)
+        result = self.session.run_ps(ps_script)
+        logging.debug(f"result std_out: {result.std_out.decode('utf-8')}")
+        logging.debug(f"result status_code \n{result.status_code}")
+        if result.status_code == '1':
+            return False
+        return result.std_out.decode('utf-8')
+    
     # Получить текущие снапшоты виртуальных машин
     def snapshot_get_current(self, vms=[]):
         ps_script = self.gen_job(vms_list=vms, job='Get-VM', current_snapshot = True)
         result = self.session.run_ps(ps_script)
         logging.debug(f"result std_out: {result.std_out.decode('utf-8')}")
         logging.debug(f"result status_code \n{result.status_code}")
         if result.status_code == '1':
```

### Comparing `hyper-v-2.0.2/hyperv/net.py` & `hyper_v-2.0.3/hyperv/net.py`

 * *Files identical despite different names*

### Comparing `hyper-v-2.0.2/setup.py` & `hyper_v-2.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
       name="hyper-v",
       packages=setuptools.find_packages(),
-      version="2.0.2",
+      version="2.0.3",
       author="Viktor Gorinskiy",
       author_email="viktor@gorinskiy.ru",
       description="Удаленное управление Hyper-V через winrm",
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/viktor-gorinskiy/hyper-v",
 	install_requires=[
```

