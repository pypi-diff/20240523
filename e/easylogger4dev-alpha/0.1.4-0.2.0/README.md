# Comparing `tmp/easylogger4dev_alpha-0.1.4.tar.gz` & `tmp/easylogger4dev_alpha-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easylogger4dev_alpha-0.1.4.tar", last modified: Mon Apr 29 06:03:57 2024, max compression
+gzip compressed data, was "easylogger4dev_alpha-0.2.0.tar", last modified: Thu May 23 03:00:43 2024, max compression
```

## Comparing `easylogger4dev_alpha-0.1.4.tar` & `easylogger4dev_alpha-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 06:03:57.410000 easylogger4dev_alpha-0.1.4/
--rw-rw-rw-   0        0        0     1091 2024-04-27 23:51:28.000000 easylogger4dev_alpha-0.1.4/LICENSE.txt
--rw-rw-rw-   0        0        0      306 2024-04-29 06:03:58.000000 easylogger4dev_alpha-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-25 06:19:42.000000 easylogger4dev_alpha-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 06:03:57.440000 easylogger4dev_alpha-0.1.4/easylogger4dev_alpha/
--rw-rw-rw-   0        0        0     8683 2024-04-29 06:01:54.000000 easylogger4dev_alpha-0.1.4/easylogger4dev_alpha/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 06:03:57.480000 easylogger4dev_alpha-0.1.4/easylogger4dev_alpha.egg-info/
--rw-rw-rw-   0        0        0      306 2024-04-29 06:03:58.000000 easylogger4dev_alpha-0.1.4/easylogger4dev_alpha.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      321 2024-04-29 06:03:58.000000 easylogger4dev_alpha-0.1.4/easylogger4dev_alpha.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 06:03:58.000000 easylogger4dev_alpha-0.1.4/easylogger4dev_alpha.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-29 06:03:58.000000 easylogger4dev_alpha-0.1.4/easylogger4dev_alpha.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2024-04-29 06:03:58.000000 easylogger4dev_alpha-0.1.4/easylogger4dev_alpha.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 06:03:58.000000 easylogger4dev_alpha-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      397 2024-04-29 06:02:00.000000 easylogger4dev_alpha-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 06:03:57.520000 easylogger4dev_alpha-0.1.4/tests/
--rw-rw-rw-   0        0        0        0 2024-04-25 06:18:48.000000 easylogger4dev_alpha-0.1.4/tests/__init__.py
--rw-rw-rw-   0        0        0     9271 2024-04-28 06:21:52.000000 easylogger4dev_alpha-0.1.4/tests/test_module.py
+drwxrwxrwx   0        0        0        0 2024-05-23 03:00:43.761895 easylogger4dev_alpha-0.2.0/
+-rw-rw-rw-   0        0        0     1091 2024-04-27 23:51:28.000000 easylogger4dev_alpha-0.2.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      306 2024-05-23 03:00:43.753689 easylogger4dev_alpha-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-25 06:19:42.000000 easylogger4dev_alpha-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 03:00:43.631712 easylogger4dev_alpha-0.2.0/easylogger4dev_alpha/
+-rw-rw-rw-   0        0        0     9269 2024-05-23 02:49:07.000000 easylogger4dev_alpha-0.2.0/easylogger4dev_alpha/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 03:00:43.687746 easylogger4dev_alpha-0.2.0/easylogger4dev_alpha.egg-info/
+-rw-rw-rw-   0        0        0      306 2024-05-23 03:00:43.000000 easylogger4dev_alpha-0.2.0/easylogger4dev_alpha.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      321 2024-05-23 03:00:43.000000 easylogger4dev_alpha-0.2.0/easylogger4dev_alpha.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 03:00:43.000000 easylogger4dev_alpha-0.2.0/easylogger4dev_alpha.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-23 03:00:43.000000 easylogger4dev_alpha-0.2.0/easylogger4dev_alpha.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2024-05-23 03:00:43.000000 easylogger4dev_alpha-0.2.0/easylogger4dev_alpha.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 03:00:43.761895 easylogger4dev_alpha-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      397 2024-05-23 02:24:44.000000 easylogger4dev_alpha-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 03:00:43.706666 easylogger4dev_alpha-0.2.0/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-25 06:18:47.000000 easylogger4dev_alpha-0.2.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     9271 2024-04-28 06:21:52.000000 easylogger4dev_alpha-0.2.0/tests/test_module.py
```

### Comparing `easylogger4dev_alpha-0.1.4/LICENSE.txt` & `easylogger4dev_alpha-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `easylogger4dev_alpha-0.1.4/easylogger4dev_alpha/__init__.py` & `easylogger4dev_alpha-0.2.0/tests/test_module.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 import pandas as pd
 
 """zh：当前包仅用于开发使用，功能尚不完善。所有的日志功能均通过修饰器进行实现"""
 
 
 def logger_ini():
     """初始化日志文件配置文件，使用日志模块前请先初始化，只需要初始化一次否则无法正常使用"""
-    log_front = "./log/"
-    directory_list = ["./log", log_front + r"jsons/",
-                      log_front + "txts/",
-                      log_front + "csvs/",
-                      log_front + "excels/"]
+    log_front = r".\log\\"
+    directory_list = [r".\log", log_front + r"jsons\\",
+                      log_front + r"txts\\",
+                      log_front + r"csvs\\",
+                      log_front + r"excels\\"]
     for directory in directory_list:
         if not os.path.exists(directory):
             os.makedirs(directory)
 
     current_time = time.localtime()
     formatted_time = time.strftime("%Y-%m-%d--%H-%M-%S", current_time)
     log_name = "log_" + formatted_time
-    with open('log/log_config.json', mode='w', encoding='utf-8') as config:
+    with open(r'log\log_config.json', mode='w', encoding='utf-8') as config:
         log_path_data = {"json_log_path": directory_list[1] + log_name + ".json",
                          "txt_log_path": directory_list[2] + log_name + ".txt",
                          "csv_log_path": directory_list[3] + log_name + ".csv",
                          "excel_log_path": directory_list[4] + log_name + ".xlsx"}
         json.dump(log_path_data, config, ensure_ascii=False, indent=4)
 
     with open(log_path_data['json_log_path'], mode='w', encoding='utf-8') as logging:
@@ -54,15 +54,15 @@
                  """
 
     def log_decorator(func):
         def wrapper(*args, **kwargs):
             start_time = time.time()
             result = func(*args, **kwargs)
             end_time = time.time()
-            with open('log/log_config.json', mode='r', encoding='utf') as config:
+            with open(r'log\log_config.json', mode='r', encoding='utf') as config:
                 log_path_data = json.load(config)
             file_path = log_path_data['json_log_path']
             log_dict = {"调用模块": module,
                         "调用函数": func.__name__,
                         "函数执行时间": f"{(end_time - start_time):.2f}秒",
                         "返回值": result
                         }
@@ -102,15 +102,15 @@
              """
 
     def log_decorator(func):
         def wrapper(*args, **kwargs):
             start_time = time.time()
             result = func(*args, **kwargs)
             end_time = time.time()
-            with open('log/log_config.json', mode='r', encoding='utf') as config:
+            with open(r'log\log_config.json', mode='r', encoding='utf') as config:
                 log_path_data = json.load(config)
             file_path = log_path_data['txt_log_path']
             if remarks is None:
                 logging_list = [
                     f"调用模块：{module} \n",
                     f"调用函数：{func.__name__} \n",
                     f"函数执行时间：{(end_time - start_time):.2f}秒 \n",
@@ -156,15 +156,15 @@
                  """
 
     def log_decorator(func):
         def wrapper(*args, **kwargs):
             start_time = time.time()
             result = func(*args, **kwargs)
             end_time = time.time()
-            with open('log/log_config.json', mode='r', encoding='utf') as config:
+            with open(r'log\log_config.json', mode='r', encoding='utf') as config:
                 log_path_data = json.load(config)
             file_path = log_path_data['csv_log_path']
             info_row = [module, func.__name__, f"{(end_time - start_time):.2f}秒", result, remarks]
             df = pd.read_csv(file_path)
             new_row = pd.DataFrame([info_row], columns=df.columns)
             df = pd.concat([df, new_row], ignore_index=True)
             df.to_csv(file_path, index=True)
@@ -204,9 +204,34 @@
             return result
 
         return wrapper
 
     return log_decorator
 
 
+@log4txt("log", remarks="这是一次测试", divisionline="^", numoflines=10)
+def test_func():
+    return "测试函数被执行"
+
+
+@log4json("log", remarks="这是一次测试")
+def test_func1():
+    return "测试函数被执行"
+
+
+@log4csv("log", remarks="这是一次测试")
+def test_func2():
+    return "测试函数被执行"
+
+
+@log4excel("log", remarks="这是一次测试")
+def test_func3():
+    return "测试函数被执行"
+
 
+if __name__ == "__main__":
+    logger_ini()
+    test_func()
+    test_func1()
+    test_func2()
+    test_func3()
```

### Comparing `easylogger4dev_alpha-0.1.4/tests/test_module.py` & `easylogger4dev_alpha-0.2.0/easylogger4dev_alpha/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 import time
 import json
 import os
 import pandas as pd
 
 """zh：当前包仅用于开发使用，功能尚不完善。所有的日志功能均通过修饰器进行实现"""
-
+is_log = True
 
 def logger_ini():
     """初始化日志文件配置文件，使用日志模块前请先初始化，只需要初始化一次否则无法正常使用"""
-    log_front = r".\log\\"
-    directory_list = [r".\log", log_front + r"jsons\\",
-                      log_front + r"txts\\",
-                      log_front + r"csvs\\",
-                      log_front + r"excels\\"]
-    for directory in directory_list:
-        if not os.path.exists(directory):
-            os.makedirs(directory)
-
-    current_time = time.localtime()
-    formatted_time = time.strftime("%Y-%m-%d--%H-%M-%S", current_time)
-    log_name = "log_" + formatted_time
-    with open(r'log\log_config.json', mode='w', encoding='utf-8') as config:
-        log_path_data = {"json_log_path": directory_list[1] + log_name + ".json",
-                         "txt_log_path": directory_list[2] + log_name + ".txt",
-                         "csv_log_path": directory_list[3] + log_name + ".csv",
-                         "excel_log_path": directory_list[4] + log_name + ".xlsx"}
-        json.dump(log_path_data, config, ensure_ascii=False, indent=4)
-
-    with open(log_path_data['json_log_path'], mode='w', encoding='utf-8') as logging:
-        ini_data = ["程序开始执行"]
-        json.dump(ini_data, logging, ensure_ascii=False, indent=4)
-    with open(log_path_data['txt_log_path'], mode='w', encoding='utf-8') as logging:
-        ini_data = "程序开始执行"
-        logging.write(ini_data)
-    columns = ['调用模块', '调用函数', '运行时间', '返回值', '备注']
-    df = pd.DataFrame(columns=columns)
-    df.to_csv(log_path_data["csv_log_path"], index=False)
-    df.to_excel(log_path_data["excel_log_path"], index=False)
+    if is_log == True:
+        log_front = "./log/"
+        directory_list = ["./log", log_front + r"jsons/",
+                          log_front + "txts/",
+                          log_front + "csvs/",
+                          log_front + "excels/"]
+        for directory in directory_list:
+            if not os.path.exists(directory):
+                os.makedirs(directory)
+
+        current_time = time.localtime()
+        formatted_time = time.strftime("%Y-%m-%d--%H-%M-%S", current_time)
+        log_name = "log_" + formatted_time
+        with open('log/log_config.json', mode='w', encoding='utf-8') as config:
+            log_path_data = {"json_log_path": directory_list[1] + log_name + ".json",
+                             "txt_log_path": directory_list[2] + log_name + ".txt",
+                             "csv_log_path": directory_list[3] + log_name + ".csv",
+                             "excel_log_path": directory_list[4] + log_name + ".xlsx"}
+            json.dump(log_path_data, config, ensure_ascii=False, indent=4)
+
+        with open(log_path_data['json_log_path'], mode='w', encoding='utf-8') as logging:
+            ini_data = ["程序开始执行"]
+            json.dump(ini_data, logging, ensure_ascii=False, indent=4)
+        with open(log_path_data['txt_log_path'], mode='w', encoding='utf-8') as logging:
+            ini_data = "程序开始执行"
+            logging.write(ini_data)
+        columns = ['调用模块', '调用函数', '运行时间', '返回值', '备注']
+        df = pd.DataFrame(columns=columns)
+        df.to_csv(log_path_data["csv_log_path"], index=False)
+        df.to_excel(log_path_data["excel_log_path"], index=False)
 
 
 def log4json(module,
              remarks=None):
     """
              一个用于记录日志的装饰器，接受日志目录和日志编写模式的参数输入，在日志中记录运行的函数和运行的时间，仅适用于返回单个值的函数
 
@@ -48,43 +49,44 @@
                  module(str):在面向对象编程中调用的模块的名称，方便开发进行调试时明确模块
                  remarks(str):备注，便于开发者在调试过程中插入备注
 
 
              Raises:
                  None: 此装饰器不抛出报错
                  """
+    if is_log == True:
+
+        def log_decorator(func):
+            def wrapper(*args, **kwargs):
+                start_time = time.time()
+                result = func(*args, **kwargs)
+                end_time = time.time()
+                with open('log/log_config.json', mode='r', encoding='utf') as config:
+                    log_path_data = json.load(config)
+                file_path = log_path_data['json_log_path']
+                log_dict = {"调用模块": module,
+                            "调用函数": func.__name__,
+                            "函数执行时间": f"{(end_time - start_time):.2f}秒",
+                            "返回值": result
+                            }
+                if remarks is not None:
+                    log_dict["备注"] = remarks
+                with open(file=file_path, mode='r', encoding='utf-8') as logging:
+                    log_data = json.load(logging)
 
-    def log_decorator(func):
-        def wrapper(*args, **kwargs):
-            start_time = time.time()
-            result = func(*args, **kwargs)
-            end_time = time.time()
-            with open(r'log\log_config.json', mode='r', encoding='utf') as config:
-                log_path_data = json.load(config)
-            file_path = log_path_data['json_log_path']
-            log_dict = {"调用模块": module,
-                        "调用函数": func.__name__,
-                        "函数执行时间": f"{(end_time - start_time):.2f}秒",
-                        "返回值": result
-                        }
-            if remarks is not None:
-                log_dict["备注"] = remarks
-            with open(file=file_path, mode='r', encoding='utf-8') as logging:
-                log_data = json.load(logging)
-
-            log_data.append(log_dict)
+                log_data.append(log_dict)
 
-            with open(file=file_path, mode='w', encoding='utf-8') as logging:
-                json.dump(log_data, logging, ensure_ascii=False, indent=4)
+                with open(file=file_path, mode='w', encoding='utf-8') as logging:
+                    json.dump(log_data, logging, ensure_ascii=False, indent=4)
 
-            return result
+                return result
 
-        return wrapper
+            return wrapper
 
-    return log_decorator
+        return log_decorator
 
 
 def log4txt(module,
             remarks=None,
             numoflines=72,
             divisionline='-'):
     """
@@ -96,142 +98,120 @@
              numoflines(int):个性化选择，在txt文件中分隔线中'-'的数量
              divisionline(str):个性化选择，在txt文件中自定义分割线的样式
 
 
          Raises:
              None: 此装饰器不抛出报错
              """
+    if is_log:
 
-    def log_decorator(func):
-        def wrapper(*args, **kwargs):
-            start_time = time.time()
-            result = func(*args, **kwargs)
-            end_time = time.time()
-            with open(r'log\log_config.json', mode='r', encoding='utf') as config:
-                log_path_data = json.load(config)
-            file_path = log_path_data['txt_log_path']
-            if remarks is None:
-                logging_list = [
-                    f"调用模块：{module} \n",
-                    f"调用函数：{func.__name__} \n",
-                    f"函数执行时间：{(end_time - start_time):.2f}秒 \n",
-                    f"返回值：{result} \n",
-                    "\n",
-                    divisionline * numoflines,
-                    "\n"
-                ]
-            else:
-                logging_list = [
-                    f"调用模块：{module} \n",
-                    f"调用函数：{func.__name__} \n",
-                    f"函数执行时间：{(end_time - start_time):.2f}秒 \n",
-                    f"返回值：{result} \n",
-                    f"备注：{remarks}\n"
-                    "\n",
-                    divisionline * numoflines,
-                    "\n"
-                ]
-
-            with open(file=file_path, mode='a', encoding='utf-8') as logging:
-                for log in logging_list:
-                    logging.write(log)
+        def log_decorator(func):
+            def wrapper(*args, **kwargs):
+                start_time = time.time()
+                result = func(*args, **kwargs)
+                end_time = time.time()
+                with open('log/log_config.json', mode='r', encoding='utf') as config:
+                    log_path_data = json.load(config)
+                file_path = log_path_data['txt_log_path']
+                if remarks is None:
+                    logging_list = [
+                        f"调用模块：{module} \n",
+                        f"调用函数：{func.__name__} \n",
+                        f"函数执行时间：{(end_time - start_time):.2f}秒 \n",
+                        f"返回值：{result} \n",
+                        "\n",
+                        divisionline * numoflines,
+                        "\n"
+                    ]
+                else:
+                    logging_list = [
+                        f"调用模块：{module} \n",
+                        f"调用函数：{func.__name__} \n",
+                        f"函数执行时间：{(end_time - start_time):.2f}秒 \n",
+                        f"返回值：{result} \n",
+                        f"备注：{remarks}\n"
+                        "\n",
+                        divisionline * numoflines,
+                        "\n"
+                    ]
+
+                with open(file=file_path, mode='a', encoding='utf-8') as logging:
+                    for log in logging_list:
+                        logging.write(log)
 
-                return result
+                    return result
 
-        return wrapper
+            return wrapper
 
-    return log_decorator
+        return log_decorator
 
 
 def log4csv(module, remarks=None):
     """
              一个用于记录日志的装饰器，接受日志目录和日志编写模式的参数输入，在日志中记录运行的函数和运行的时间，仅适用于返回单个值的函数
 
              Args:
                  module(str):在面向对象编程中调用的模块的名称，方便开发进行调试时明确模块
                  remarks(str):备注，便于开发者在调试过程中插入备注
 
 
              Raises:
                  None: 此装饰器不抛出报错
                  """
+    if is_log:
 
-    def log_decorator(func):
-        def wrapper(*args, **kwargs):
-            start_time = time.time()
-            result = func(*args, **kwargs)
-            end_time = time.time()
-            with open(r'log\log_config.json', mode='r', encoding='utf') as config:
-                log_path_data = json.load(config)
-            file_path = log_path_data['csv_log_path']
-            info_row = [module, func.__name__, f"{(end_time - start_time):.2f}秒", result, remarks]
-            df = pd.read_csv(file_path)
-            new_row = pd.DataFrame([info_row], columns=df.columns)
-            df = pd.concat([df, new_row], ignore_index=True)
-            df.to_csv(file_path, index=True)
-            return result
+        def log_decorator(func):
+            def wrapper(*args, **kwargs):
+                start_time = time.time()
+                result = func(*args, **kwargs)
+                end_time = time.time()
+                with open('log/log_config.json', mode='r', encoding='utf') as config:
+                    log_path_data = json.load(config)
+                file_path = log_path_data['csv_log_path']
+                info_row = [None,module, func.__name__, f"{(end_time - start_time):.2f}秒", result, remarks]
+                df = pd.read_csv(file_path)
+                new_row = pd.DataFrame([info_row], columns=df.columns)
+                df = pd.concat([df, new_row], ignore_index=True)
+                df.to_csv(file_path, index=True)
+                return result
 
-        return wrapper
+            return wrapper
 
-    return log_decorator
+        return log_decorator
 
 
 def log4excel(module, remarks=None):
     """
              一个用于记录日志的装饰器，接受日志目录和日志编写模式的参数输入，在日志中记录运行的函数和运行的时间，仅适用于返回单个值的函数
 
              Args:
                  module(str):在面向对象编程中调用的模块的名称，方便开发进行调试时明确模块
                  remarks(str):备注，便于开发者在调试过程中插入备注
 
 
              Raises:
                  None: 此装饰器不抛出报错
                  """
+    if is_log:
 
-    def log_decorator(func):
-        def wrapper(*args, **kwargs):
-            start_time = time.time()
-            result = func(*args, **kwargs)
-            end_time = time.time()
-            with open(r'log\log_config.json', mode='r', encoding='utf') as config:
-                log_path_data = json.load(config)
-            file_path = log_path_data['excel_log_path']
-            info_row = [module, func.__name__, f"{(end_time - start_time):.2f}秒", result, remarks]
-            df = pd.read_excel(file_path)
-            new_row = pd.DataFrame([info_row], columns=df.columns)
-            df = pd.concat([df, new_row], ignore_index=True)
-            df.to_excel(file_path, index=False)
-            return result
-
-        return wrapper
-
-    return log_decorator
-
-
-@log4txt("log", remarks="这是一次测试", divisionline="^", numoflines=10)
-def test_func():
-    return "测试函数被执行"
-
-
-@log4json("log", remarks="这是一次测试")
-def test_func1():
-    return "测试函数被执行"
-
+        def log_decorator(func):
+            def wrapper(*args, **kwargs):
+                start_time = time.time()
+                result = func(*args, **kwargs)
+                end_time = time.time()
+                with open('log/log_config.json', mode='r', encoding='utf') as config:
+                    log_path_data = json.load(config)
+                file_path = log_path_data['excel_log_path']
+                info_row = [None,module, func.__name__, f"{(end_time - start_time):.2f}秒", result, remarks]
+                df = pd.read_excel(file_path)
+                new_row = pd.DataFrame([info_row], columns=df.columns)
+                df = pd.concat([df, new_row], ignore_index=True)
+                df.to_excel(file_path, index=False)
+                return result
 
-@log4csv("log", remarks="这是一次测试")
-def test_func2():
-    return "测试函数被执行"
+            return wrapper
 
+        return log_decorator
 
-@log4excel("log", remarks="这是一次测试")
-def test_func3():
-    return "测试函数被执行"
 
 
-if __name__ == "__main__":
-    logger_ini()
-    test_func()
-    test_func1()
-    test_func2()
-    test_func3()
```

