# Comparing `tmp/jyhelper-1.2.3.tar.gz` & `tmp/jyhelper-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jyhelper-1.2.3.tar", last modified: Thu May 16 09:07:58 2024, max compression
+gzip compressed data, was "jyhelper-1.2.4.tar", last modified: Thu May 23 02:48:26 2024, max compression
```

## Comparing `jyhelper-1.2.3.tar` & `jyhelper-1.2.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 09:07:58.837970 jyhelper-1.2.3/
--rw-rw-rw-   0        0        0     1130 2024-05-16 09:07:58.835993 jyhelper-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0      820 2023-11-17 09:46:48.000000 jyhelper-1.2.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 09:07:58.808683 jyhelper-1.2.3/jyhelper/
--rw-rw-rw-   0        0        0      385 2023-11-17 06:00:40.000000 jyhelper-1.2.3/jyhelper/__init__.py
--rw-rw-rw-   0        0        0     4455 2024-01-30 07:23:11.000000 jyhelper-1.2.3/jyhelper/common.py
--rw-rw-rw-   0        0        0    15783 2023-12-28 09:52:26.000000 jyhelper-1.2.3/jyhelper/db.py
--rw-rw-rw-   0        0        0     5284 2024-01-05 03:38:54.000000 jyhelper-1.2.3/jyhelper/feishuRobot.py
--rw-rw-rw-   0        0        0     1888 2024-05-16 08:55:22.000000 jyhelper-1.2.3/jyhelper/file.py
--rw-rw-rw-   0        0        0     4651 2024-04-30 03:17:37.000000 jyhelper-1.2.3/jyhelper/timeHelper.py
-drwxrwxrwx   0        0        0        0 2024-05-16 09:07:58.832531 jyhelper-1.2.3/jyhelper.egg-info/
--rw-rw-rw-   0        0        0     1130 2024-05-16 09:07:58.000000 jyhelper-1.2.3/jyhelper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2024-05-16 09:07:58.000000 jyhelper-1.2.3/jyhelper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 09:07:58.000000 jyhelper-1.2.3/jyhelper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-16 09:07:58.000000 jyhelper-1.2.3/jyhelper.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-16 09:07:58.000000 jyhelper-1.2.3/jyhelper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 09:07:58.837970 jyhelper-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0      718 2024-05-16 09:05:44.000000 jyhelper-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 02:48:26.827283 jyhelper-1.2.4/
+-rw-rw-rw-   0        0        0     1130 2024-05-23 02:48:26.826283 jyhelper-1.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0      820 2023-11-17 09:46:48.000000 jyhelper-1.2.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 02:48:26.800707 jyhelper-1.2.4/jyhelper/
+-rw-rw-rw-   0        0        0      385 2023-11-17 06:00:40.000000 jyhelper-1.2.4/jyhelper/__init__.py
+-rw-rw-rw-   0        0        0     4455 2024-01-30 07:23:11.000000 jyhelper-1.2.4/jyhelper/common.py
+-rw-rw-rw-   0        0        0    15771 2024-05-23 02:43:07.000000 jyhelper-1.2.4/jyhelper/db.py
+-rw-rw-rw-   0        0        0     5284 2024-01-05 03:38:54.000000 jyhelper-1.2.4/jyhelper/feishuRobot.py
+-rw-rw-rw-   0        0        0     1888 2024-05-21 03:10:31.000000 jyhelper-1.2.4/jyhelper/file.py
+-rw-rw-rw-   0        0        0     4651 2024-04-30 03:17:37.000000 jyhelper-1.2.4/jyhelper/timeHelper.py
+drwxrwxrwx   0        0        0        0 2024-05-23 02:48:26.824055 jyhelper-1.2.4/jyhelper.egg-info/
+-rw-rw-rw-   0        0        0     1130 2024-05-23 02:48:26.000000 jyhelper-1.2.4/jyhelper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2024-05-23 02:48:26.000000 jyhelper-1.2.4/jyhelper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 02:48:26.000000 jyhelper-1.2.4/jyhelper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-23 02:48:26.000000 jyhelper-1.2.4/jyhelper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-23 02:48:26.000000 jyhelper-1.2.4/jyhelper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 02:48:26.827283 jyhelper-1.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      718 2024-05-23 02:47:35.000000 jyhelper-1.2.4/setup.py
```

### Comparing `jyhelper-1.2.3/PKG-INFO` & `jyhelper-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jyhelper
-Version: 1.2.3
+Version: 1.2.4
 Summary: 各种实用、常用的小函数、类
 Home-page: https://pypi.org/project/jyhelper/
 Author: JY
 Author-email: your-email@example.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.0
```

### Comparing `jyhelper-1.2.3/README.md` & `jyhelper-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `jyhelper-1.2.3/jyhelper/common.py` & `jyhelper-1.2.4/jyhelper/common.py`

 * *Files identical despite different names*

### Comparing `jyhelper-1.2.3/jyhelper/db.py` & `jyhelper-1.2.4/jyhelper/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -355,20 +355,19 @@
         try:
             with self.__conn.cursor() as cursor:
                 cursor.execute(sql)
                 for oneItem in cursor:
                     yield oneItem
         except Exception as e:
             print(self.getDate(), self.__host, '第%s次执行SQL失败...' % str(except_time + 1), sql, e)
-            # common.debug(self.__host + '---- ' + sql + ' ----' + str(e))
-            if except_time == 0:
-                except_time = 1
-                print(self.getDate(), self.__host, '第%s次执行SQL尝试...' % str(except_time + 1), sql)
-                reda = self.__execute_ss(sql, except_time)
-                return reda if bool(reda) else []
+            # if except_time == 0:
+            #     except_time = 1
+            #     print(self.getDate(), self.__host, '第%s次执行SQL尝试...' % str(except_time + 1), sql)
+            #     reda = self.__execute_ss(sql, except_time)
+            #     return reda if bool(reda) else []
         finally:
             self.__closeConn()
             self.__clearWhere()
 
     # 关闭连接
     def __closeConn(self):
         if self.__conn is not None:
@@ -408,13 +407,14 @@
 
 
 if __name__ == '__main__':
     config = {
         'host': 'localhost',
         'port': 3306,
         'user': 'root',
-        'password': '',
+        'password': 'root',
         'db': 'laravel'
     }
 
-    data = db(config).table('ax_video').where('id=177 or id=178').count()
-    print(data)
+    data = db(config).setSSCursor().table('ax_video').where('id=177 or id=178 or id=179').select()
+    for row in data:
+        print(row)
```

### Comparing `jyhelper-1.2.3/jyhelper/feishuRobot.py` & `jyhelper-1.2.4/jyhelper/feishuRobot.py`

 * *Files identical despite different names*

### Comparing `jyhelper-1.2.3/jyhelper/file.py` & `jyhelper-1.2.4/jyhelper/file.py`

 * *Files identical despite different names*

### Comparing `jyhelper-1.2.3/jyhelper/timeHelper.py` & `jyhelper-1.2.4/jyhelper/timeHelper.py`

 * *Files identical despite different names*

### Comparing `jyhelper-1.2.3/jyhelper.egg-info/PKG-INFO` & `jyhelper-1.2.4/jyhelper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jyhelper
-Version: 1.2.3
+Version: 1.2.4
 Summary: 各种实用、常用的小函数、类
 Home-page: https://pypi.org/project/jyhelper/
 Author: JY
 Author-email: your-email@example.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.0
```

### Comparing `jyhelper-1.2.3/setup.py` & `jyhelper-1.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # @Time : 2023/11/08 18:38 
 # @Author : JY
 
 from setuptools import setup
 
 setup(
     name='jyhelper',
-    version='1.2.3',
+    version='1.2.4',
     packages=['jyhelper'],
     install_requires=[
         'pymysql',
         'requests'
     ],
     description='各种实用、常用的小函数、类',
     long_description=open('README.md',encoding='utf-8').read(),  # 详细描述，通常从 README.md 中读取
```

