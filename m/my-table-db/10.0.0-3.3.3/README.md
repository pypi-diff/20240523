# Comparing `tmp/my_table_db-10.0.0.tar.gz` & `tmp/my_table_db-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_table_db-10.0.0.tar", last modified: Thu May 23 20:46:47 2024, max compression
+gzip compressed data, was "my_table_db-3.3.3.tar", last modified: Sat May 18 23:43:10 2024, max compression
```

## Comparing `my_table_db-10.0.0.tar` & `my_table_db-3.3.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 20:46:47.145108 my_table_db-10.0.0/
--rw-rw-rw-   0        0        0     1086 2024-05-18 20:21:49.000000 my_table_db-10.0.0/LICENSE
--rw-rw-rw-   0        0        0     5330 2024-05-23 20:46:47.145108 my_table_db-10.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     5091 2024-05-23 20:45:26.000000 my_table_db-10.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 20:46:47.144108 my_table_db-10.0.0/my_table_db.egg-info/
--rw-rw-rw-   0        0        0     5330 2024-05-23 20:46:47.000000 my_table_db-10.0.0/my_table_db.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      181 2024-05-23 20:46:47.000000 my_table_db-10.0.0/my_table_db.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 20:46:47.000000 my_table_db-10.0.0/my_table_db.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-23 20:46:47.000000 my_table_db-10.0.0/my_table_db.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6809 2024-05-23 20:46:29.000000 my_table_db-10.0.0/my_table_db.py
--rw-rw-rw-   0        0        0       42 2024-05-23 20:46:47.145108 my_table_db-10.0.0/setup.cfg
--rw-rw-rw-   0        0        0      382 2024-05-23 19:41:24.000000 my_table_db-10.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 23:43:10.387852 my_table_db-3.3.3/
+-rw-rw-rw-   0        0        0     1086 2024-05-18 20:21:49.000000 my_table_db-3.3.3/LICENSE
+-rw-rw-rw-   0        0        0     3904 2024-05-18 23:43:10.386842 my_table_db-3.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3666 2024-05-18 23:40:31.000000 my_table_db-3.3.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 23:43:10.385842 my_table_db-3.3.3/my_table_db.egg-info/
+-rw-rw-rw-   0        0        0     3904 2024-05-18 23:43:10.000000 my_table_db-3.3.3/my_table_db.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      181 2024-05-18 23:43:10.000000 my_table_db-3.3.3/my_table_db.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 23:43:10.000000 my_table_db-3.3.3/my_table_db.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-18 23:43:10.000000 my_table_db-3.3.3/my_table_db.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1906 2024-05-18 23:00:35.000000 my_table_db-3.3.3/my_table_db.py
+-rw-rw-rw-   0        0        0       42 2024-05-18 23:43:10.387852 my_table_db-3.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      381 2024-05-18 23:43:05.000000 my_table_db-3.3.3/setup.py
```

### Comparing `my_table_db-10.0.0/LICENSE` & `my_table_db-3.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `my_table_db-10.0.0/PKG-INFO` & `my_table_db-3.3.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: my_table_db
-Version: 10.0.0
+Version: 3.3.3
 Summary: A small library for conclusion table db
 Author: k0ng999
 Author-email: baydar_14@mail.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -33,68 +33,37 @@
 ***
 
 # Установка
 
 ` pip install my_table_db `
 
 ## Пример 1
-
-Содержимое таблицы
-```csv
-id  Name    Salary
-1   Alice   50000
-2   Bob     60000
-```
-Код с использованием my_table_db_full
+Пример использования функции my_table_db:
 
 ```python
-import psycopg2
-from my_table_db import my_table_db_full
-
-def fetch_data():
-    conn = None
-    try:
-        conn = con = psycopg2.connect(
-            dbname=...,
-            user=...,
-            password=...,
-            host=...,
-            port=...)
-        cur = conn.cursor()
-        cur.execute("SELECT * FROM employees")
-        
-        rows = cur.fetchall()   #Получаем все строки
-        colum_name = [desc[0] for desc in cur.description]  #Получаем все названия колонок
-        
-        my_table_db_full(rows, colum_name)  #Выводим на экран всю табличку
-        
-        cur.close()
-    except (Exception, psycopg2.DatabaseError) as error:
-        print(error)
-    finally:
-        if conn is not None:
-            conn.close()
-            print()
-            print("Database connection closed.")
+from my_table_db import my_table_db
 
+print(my_table_db('ID', 1, 'Name', 'Alice', 'Salary', 50000))
 
-fetch_data()
 ```
-
-#### Вывод
-
+### Вывод
 ```shell
-id:1 | Name:Alice | Salary:50000
-id:2 | Name:Bob   | Salary:60000
+ID:1         |        Name:Alice     |        Salary:50000
 
-Database connection closed.
 ```
 
 ## Пример 2
-Код с использованием my_table_db_full
+
+Содержимое таблицы
+```csv
+id  name    salary
+1   Alice   50000
+2   Bob     60000
+```
+Код с использованием my_table_db
 
 ```python
 import psycopg2
 from my_table_db import my_table_db
 
 def fetch_data():
     conn = None
@@ -103,50 +72,41 @@
             dbname=...,
             user=...,
             password=...,
             host=...,
             port=...)
         cur = conn.cursor()
         cur.execute("SELECT * FROM employees")
-        
-        rows = cur.fetchall()   #Получаем все строки
+        rows = cur.fetchall()
         for row in rows:
-            my_table_db(rows,'id',row[0],'Name',row[1],'Salary',row[2])  #Выводим на экран табличку 
-        
+            print(my_table_db('ID', row[0], 'Name', row[1], 'Salary', row[2]))
         cur.close()
     except (Exception, psycopg2.DatabaseError) as error:
         print(error)
     finally:
         if conn is not None:
             conn.close()
             print()
             print("Database connection closed.")
 
 
 fetch_data()
 ```
-```shell
-id:1 | Name:Alice | Salary:50000
-id:2 | Name:Bob   | Salary:60000
 
-Database connection closed.
-```
-### Преймущества 2 способа в том что мы можем вывести не всю табличку, а только то что хотим, а так же мы можем указать собственное имя столбца. Например мы могли написать 
-```python
-my_table_db(rows,'Имя',row[1],'Зарплата',row[2])
-```
-И в этом случае вывелось бы:
+#### Вывод
 
 ```shell
-Имя:Alice | Зарплата:50000
-Имя:Bob   | Зарплата:60000
+ID:1         |        Name:Alice     |        Salary:50000
+ID:2         |        Name:Bob       |        Salary:60000
+
+Database connection closed.
 ```
 
 ***
 
 # Заключение
-#### Библиотека my_table_db полезна для форматирования и отображения наборов пар имя-значение в структурированном и читаемом формате. Она может обрабатывать различное количество аргументов и гарантирует, что вывод останется выровненным и легко читаемым.
+#### Функция my_table_db полезна для форматирования и отображения наборов пар имя-значение в структурированном и читаемом формате. Она может обрабатывать различное количество аргументов и гарантирует, что вывод останется выровненным и легко читаемым.
 
 ***
 ### Автор
 
 Автор: k0ng999
```

### Comparing `my_table_db-10.0.0/README.md` & `my_table_db-3.3.3/my_table_db.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: my_table_db
+Version: 3.3.3
+Summary: A small library for conclusion table db
+Author: k0ng999
+Author-email: baydar_14@mail.ru
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Функция my_table_db
 
 Этот Python-скрипт определяет функцию my_table_db, которая форматирует набор именованных аргументов и их соответствующих значений в строку. Выходная строка структурирована с определенным форматом, где каждая пара имя-значение разделена символом | и дополнена до выравнивания в столбцах.
 
 ***
 
 
@@ -23,68 +33,37 @@
 ***
 
 # Установка
 
 ` pip install my_table_db `
 
 ## Пример 1
-
-Содержимое таблицы
-```csv
-id  Name    Salary
-1   Alice   50000
-2   Bob     60000
-```
-Код с использованием my_table_db_full
+Пример использования функции my_table_db:
 
 ```python
-import psycopg2
-from my_table_db import my_table_db_full
-
-def fetch_data():
-    conn = None
-    try:
-        conn = con = psycopg2.connect(
-            dbname=...,
-            user=...,
-            password=...,
-            host=...,
-            port=...)
-        cur = conn.cursor()
-        cur.execute("SELECT * FROM employees")
-        
-        rows = cur.fetchall()   #Получаем все строки
-        colum_name = [desc[0] for desc in cur.description]  #Получаем все названия колонок
-        
-        my_table_db_full(rows, colum_name)  #Выводим на экран всю табличку
-        
-        cur.close()
-    except (Exception, psycopg2.DatabaseError) as error:
-        print(error)
-    finally:
-        if conn is not None:
-            conn.close()
-            print()
-            print("Database connection closed.")
+from my_table_db import my_table_db
 
+print(my_table_db('ID', 1, 'Name', 'Alice', 'Salary', 50000))
 
-fetch_data()
 ```
-
-#### Вывод
-
+### Вывод
 ```shell
-id:1 | Name:Alice | Salary:50000
-id:2 | Name:Bob   | Salary:60000
+ID:1         |        Name:Alice     |        Salary:50000
 
-Database connection closed.
 ```
 
 ## Пример 2
-Код с использованием my_table_db_full
+
+Содержимое таблицы
+```csv
+id  name    salary
+1   Alice   50000
+2   Bob     60000
+```
+Код с использованием my_table_db
 
 ```python
 import psycopg2
 from my_table_db import my_table_db
 
 def fetch_data():
     conn = None
@@ -93,50 +72,41 @@
             dbname=...,
             user=...,
             password=...,
             host=...,
             port=...)
         cur = conn.cursor()
         cur.execute("SELECT * FROM employees")
-        
-        rows = cur.fetchall()   #Получаем все строки
+        rows = cur.fetchall()
         for row in rows:
-            my_table_db(rows,'id',row[0],'Name',row[1],'Salary',row[2])  #Выводим на экран табличку 
-        
+            print(my_table_db('ID', row[0], 'Name', row[1], 'Salary', row[2]))
         cur.close()
     except (Exception, psycopg2.DatabaseError) as error:
         print(error)
     finally:
         if conn is not None:
             conn.close()
             print()
             print("Database connection closed.")
 
 
 fetch_data()
 ```
-```shell
-id:1 | Name:Alice | Salary:50000
-id:2 | Name:Bob   | Salary:60000
 
-Database connection closed.
-```
-### Преймущества 2 способа в том что мы можем вывести не всю табличку, а только то что хотим, а так же мы можем указать собственное имя столбца. Например мы могли написать 
-```python
-my_table_db(rows,'Имя',row[1],'Зарплата',row[2])
-```
-И в этом случае вывелось бы:
+#### Вывод
 
 ```shell
-Имя:Alice | Зарплата:50000
-Имя:Bob   | Зарплата:60000
+ID:1         |        Name:Alice     |        Salary:50000
+ID:2         |        Name:Bob       |        Salary:60000
+
+Database connection closed.
 ```
 
 ***
 
 # Заключение
-#### Библиотека my_table_db полезна для форматирования и отображения наборов пар имя-значение в структурированном и читаемом формате. Она может обрабатывать различное количество аргументов и гарантирует, что вывод останется выровненным и легко читаемым.
+#### Функция my_table_db полезна для форматирования и отображения наборов пар имя-значение в структурированном и читаемом формате. Она может обрабатывать различное количество аргументов и гарантирует, что вывод останется выровненным и легко читаемым.
 
 ***
 ### Автор
 
 Автор: k0ng999
```

