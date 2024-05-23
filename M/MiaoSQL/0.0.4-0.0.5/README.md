# Comparing `tmp/MiaoSQL-0.0.4.tar.gz` & `tmp/MiaoSQL-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MiaoSQL-0.0.4.tar", last modified: Fri May 10 14:33:58 2024, max compression
+gzip compressed data, was "MiaoSQL-0.0.5.tar", last modified: Thu May 23 14:48:04 2024, max compression
```

## Comparing `MiaoSQL-0.0.4.tar` & `MiaoSQL-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 14:33:58.743469 MiaoSQL-0.0.4/
-drwxrwxrwx   0        0        0        0 2024-05-10 14:33:58.738852 MiaoSQL-0.0.4/MiaoSQL/
--rw-rw-rw-   0        0        0       37 2024-05-10 05:25:21.000000 MiaoSQL-0.0.4/MiaoSQL/Exception.py
--rw-rw-rw-   0        0        0        0 2024-03-18 14:02:58.000000 MiaoSQL-0.0.4/MiaoSQL/__init__.py
--rw-rw-rw-   0        0        0     9706 2024-05-10 14:05:37.000000 MiaoSQL-0.0.4/MiaoSQL/miaosql.py
-drwxrwxrwx   0        0        0        0 2024-05-10 14:33:58.741854 MiaoSQL-0.0.4/MiaoSQL.egg-info/
--rw-rw-rw-   0        0        0      300 2024-05-10 14:33:58.000000 MiaoSQL-0.0.4/MiaoSQL.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2024-05-10 14:33:58.000000 MiaoSQL-0.0.4/MiaoSQL.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 14:33:58.000000 MiaoSQL-0.0.4/MiaoSQL.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-10 14:33:58.000000 MiaoSQL-0.0.4/MiaoSQL.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      300 2024-05-10 14:33:58.741854 MiaoSQL-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-10 14:33:58.743469 MiaoSQL-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      420 2024-05-10 14:33:44.000000 MiaoSQL-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:48:04.528861 MiaoSQL-0.0.5/
+drwxrwxrwx   0        0        0        0 2024-05-23 14:48:04.524587 MiaoSQL-0.0.5/MiaoSQL/
+-rw-rw-rw-   0        0        0       37 2024-05-10 05:25:21.000000 MiaoSQL-0.0.5/MiaoSQL/Exception.py
+-rw-rw-rw-   0        0        0        0 2024-03-18 14:02:58.000000 MiaoSQL-0.0.5/MiaoSQL/__init__.py
+-rw-rw-rw-   0        0        0     9609 2024-05-23 14:44:00.000000 MiaoSQL-0.0.5/MiaoSQL/miaosql.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:48:04.527842 MiaoSQL-0.0.5/MiaoSQL.egg-info/
+-rw-rw-rw-   0        0        0      300 2024-05-23 14:48:04.000000 MiaoSQL-0.0.5/MiaoSQL.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2024-05-23 14:48:04.000000 MiaoSQL-0.0.5/MiaoSQL.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 14:48:04.000000 MiaoSQL-0.0.5/MiaoSQL.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-23 14:48:04.000000 MiaoSQL-0.0.5/MiaoSQL.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      300 2024-05-23 14:48:04.527842 MiaoSQL-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-23 14:48:04.528861 MiaoSQL-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      420 2024-05-23 14:48:02.000000 MiaoSQL-0.0.5/setup.py
```

### Comparing `MiaoSQL-0.0.4/MiaoSQL/miaosql.py` & `MiaoSQL-0.0.5/MiaoSQL/miaosql.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,14 @@
             以某一列排序输出
 
         Returns
         -------
         _type_
             查询结构对象
         """
-        assert len(cols) == len(vals), f"列[{len(cols)}]与值[{len(vals)}]的数目不相同"
 
         qur = (
             f"SELECT {'*' if not out_cols else ', '.join('`' + out_col + '`' for out_col in out_cols)} FROM `{table}` "
             f"WHERE {condition if condition else 1} "
             f"{'' if not order else 'ORDER BY `' + order + '`'}"
         )
         print(qur)
```

