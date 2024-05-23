# Comparing `tmp/decoutilities-0.3.3.tar.gz` & `tmp/decoutilities-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decoutilities-0.3.3.tar", last modified: Wed May 22 19:25:11 2024, max compression
+gzip compressed data, was "decoutilities-0.3.4.tar", last modified: Thu May 23 19:43:59 2024, max compression
```

## Comparing `decoutilities-0.3.3.tar` & `decoutilities-0.3.4.tar`

### file list

```diff
@@ -1,35 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 19:25:11.072588 decoutilities-0.3.3/
--rw-rw-rw-   0        0        0     1089 2024-05-08 22:21:06.000000 decoutilities-0.3.3/LICENSE
--rw-rw-rw-   0        0        0    19887 2024-05-22 19:25:11.071514 decoutilities-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0    19408 2024-05-22 19:24:49.000000 decoutilities-0.3.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 19:25:11.048856 decoutilities-0.3.3/decoutilities/
--rw-rw-rw-   0        0        0     4740 2024-05-08 22:21:06.000000 decoutilities-0.3.3/decoutilities/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 19:25:11.057283 decoutilities-0.3.3/decoutilities/components/
--rw-rw-rw-   0        0        0      129 2024-05-22 19:14:30.000000 decoutilities-0.3.3/decoutilities/components/__init__.py
--rw-rw-rw-   0        0        0     1611 2024-05-22 19:14:30.000000 decoutilities-0.3.3/decoutilities/components/checkmark.py
--rw-rw-rw-   0        0        0     7380 2024-05-22 19:14:30.000000 decoutilities-0.3.3/decoutilities/components/input.py
--rw-rw-rw-   0        0        0     1357 2024-05-22 19:14:30.000000 decoutilities-0.3.3/decoutilities/components/selector.py
-drwxrwxrwx   0        0        0        0 2024-05-22 19:25:11.060448 decoutilities-0.3.3/decoutilities/config/
--rw-rw-rw-   0        0        0      104 2024-05-08 22:21:06.000000 decoutilities-0.3.3/decoutilities/config/__init__.py
--rw-rw-rw-   0        0        0      994 2024-05-08 22:21:06.000000 decoutilities-0.3.3/decoutilities/config/config.py
--rw-rw-rw-   0        0        0     2736 2024-05-08 22:21:06.000000 decoutilities-0.3.3/decoutilities/config/configContainer.py
-drwxrwxrwx   0        0        0        0 2024-05-22 19:25:11.063593 decoutilities-0.3.3/decoutilities/data/
--rw-rw-rw-   0        0        0      104 2024-05-08 22:21:06.000000 decoutilities-0.3.3/decoutilities/data/__init__.py
--rw-rw-rw-   0        0        0     2154 2024-05-08 22:21:06.000000 decoutilities-0.3.3/decoutilities/data/dataEncryptor.py
--rw-rw-rw-   0        0        0     1671 2024-05-08 22:21:06.000000 decoutilities-0.3.3/decoutilities/data/keyManager.py
-drwxrwxrwx   0        0        0        0 2024-05-22 19:25:11.066238 decoutilities-0.3.3/decoutilities/inject/
--rw-rw-rw-   0        0        0       44 2024-05-08 22:21:06.000000 decoutilities-0.3.3/decoutilities/inject/__init__.py
--rw-rw-rw-   0        0        0      569 2024-05-18 20:23:23.000000 decoutilities-0.3.3/decoutilities/inject/injector.py
-drwxrwxrwx   0        0        0        0 2024-05-22 19:25:11.067309 decoutilities-0.3.3/decoutilities/logger/
--rw-rw-rw-   0        0        0     1221 2024-05-22 19:14:30.000000 decoutilities-0.3.3/decoutilities/logger/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 19:25:11.068368 decoutilities-0.3.3/decoutilities/queue/
--rw-rw-rw-   0        0        0     1043 2024-05-08 22:21:06.000000 decoutilities-0.3.3/decoutilities/queue/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 19:25:11.069419 decoutilities-0.3.3/decoutilities/textUtils/
--rw-rw-rw-   0        0        0     2832 2024-05-22 19:14:30.000000 decoutilities-0.3.3/decoutilities/textUtils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 19:25:11.070468 decoutilities-0.3.3/decoutilities.egg-info/
--rw-rw-rw-   0        0        0    19887 2024-05-22 19:25:11.000000 decoutilities-0.3.3/decoutilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      717 2024-05-22 19:25:11.000000 decoutilities-0.3.3/decoutilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 19:25:11.000000 decoutilities-0.3.3/decoutilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-22 19:25:11.000000 decoutilities-0.3.3/decoutilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 19:25:11.073654 decoutilities-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0      729 2024-05-22 19:24:05.000000 decoutilities-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:43:59.020094 decoutilities-0.3.4/
+-rw-rw-rw-   0        0        0     1089 2024-05-08 22:21:06.000000 decoutilities-0.3.4/LICENSE
+-rw-rw-rw-   0        0        0    20606 2024-05-23 19:43:59.019034 decoutilities-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0    20127 2024-05-23 19:43:02.000000 decoutilities-0.3.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 19:43:58.982616 decoutilities-0.3.4/decoutilities/
+-rw-rw-rw-   0        0        0     4740 2024-05-08 22:21:06.000000 decoutilities-0.3.4/decoutilities/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:43:58.994581 decoutilities-0.3.4/decoutilities/components/
+-rw-rw-rw-   0        0        0      129 2024-05-22 19:14:30.000000 decoutilities-0.3.4/decoutilities/components/__init__.py
+-rw-rw-rw-   0        0        0     1611 2024-05-22 19:14:30.000000 decoutilities-0.3.4/decoutilities/components/checkmark.py
+-rw-rw-rw-   0        0        0     7380 2024-05-22 19:14:30.000000 decoutilities-0.3.4/decoutilities/components/input.py
+-rw-rw-rw-   0        0        0     1357 2024-05-22 19:14:30.000000 decoutilities-0.3.4/decoutilities/components/selector.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:43:58.998799 decoutilities-0.3.4/decoutilities/config/
+-rw-rw-rw-   0        0        0      104 2024-05-08 22:21:06.000000 decoutilities-0.3.4/decoutilities/config/__init__.py
+-rw-rw-rw-   0        0        0      994 2024-05-08 22:21:06.000000 decoutilities-0.3.4/decoutilities/config/config.py
+-rw-rw-rw-   0        0        0     2736 2024-05-08 22:21:06.000000 decoutilities-0.3.4/decoutilities/config/configContainer.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:43:59.003735 decoutilities-0.3.4/decoutilities/data/
+-rw-rw-rw-   0        0        0      104 2024-05-08 22:21:06.000000 decoutilities-0.3.4/decoutilities/data/__init__.py
+-rw-rw-rw-   0        0        0     2154 2024-05-08 22:21:06.000000 decoutilities-0.3.4/decoutilities/data/dataEncryptor.py
+-rw-rw-rw-   0        0        0     1671 2024-05-08 22:21:06.000000 decoutilities-0.3.4/decoutilities/data/keyManager.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:43:59.006895 decoutilities-0.3.4/decoutilities/inject/
+-rw-rw-rw-   0        0        0       44 2024-05-08 22:21:06.000000 decoutilities-0.3.4/decoutilities/inject/__init__.py
+-rw-rw-rw-   0        0        0      569 2024-05-18 20:23:23.000000 decoutilities-0.3.4/decoutilities/inject/injector.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:43:59.007943 decoutilities-0.3.4/decoutilities/logger/
+-rw-rw-rw-   0        0        0     1490 2024-05-23 19:43:02.000000 decoutilities-0.3.4/decoutilities/logger/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:43:59.010058 decoutilities-0.3.4/decoutilities/queue/
+-rw-rw-rw-   0        0        0     1043 2024-05-08 22:21:06.000000 decoutilities-0.3.4/decoutilities/queue/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:43:59.014278 decoutilities-0.3.4/decoutilities/screenUtils/
+-rw-rw-rw-   0        0        0       68 2024-05-23 19:43:02.000000 decoutilities-0.3.4/decoutilities/screenUtils/__init__.py
+-rw-rw-rw-   0        0        0      473 2024-05-23 19:43:02.000000 decoutilities-0.3.4/decoutilities/screenUtils/screen.py
+-rw-rw-rw-   0        0        0     2180 2024-05-23 19:43:02.000000 decoutilities-0.3.4/decoutilities/screenUtils/titler.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:43:59.015352 decoutilities-0.3.4/decoutilities/textUtils/
+-rw-rw-rw-   0        0        0     3055 2024-05-23 19:43:02.000000 decoutilities-0.3.4/decoutilities/textUtils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:43:59.016925 decoutilities-0.3.4/decoutilities.egg-info/
+-rw-rw-rw-   0        0        0    20606 2024-05-23 19:43:58.000000 decoutilities-0.3.4/decoutilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      827 2024-05-23 19:43:58.000000 decoutilities-0.3.4/decoutilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 19:43:58.000000 decoutilities-0.3.4/decoutilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-23 19:43:58.000000 decoutilities-0.3.4/decoutilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 19:43:59.020094 decoutilities-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      729 2024-05-23 19:43:37.000000 decoutilities-0.3.4/setup.py
```

### Comparing `decoutilities-0.3.3/LICENSE` & `decoutilities-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `decoutilities-0.3.3/PKG-INFO` & `decoutilities-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decoutilities
-Version: 0.3.3
+Version: 0.3.4
 Summary: Enhance the readability of your code with decorators and simplify the creation of configuration files.
 Author: Hugo Torres
 Author-email: contact@redactado.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -574,14 +574,37 @@
 ```python
 email = Input('Email', '', 'REQUIRED|EMAIL', 'Enter your email')
 email.display()
 ```
 
 This will create an input that requires a valid email address.
 
+## Screen Utils
+
+### Screen
+
+Screen is a way to easily know the terminal's size. Altough for the moment it only has this feature, will have more as the development continues. As right now this feature is not long enough to have its own section on the README.md I will not explain it in detail, however you are free to check the source code if wondering to use it.
+
+Planned:
+- Screen division
+- Tab manager
+- Freeze screens
+
+### Titler
+
+This one, relays on the `Screen` feature, and allows to make simple titles.
+
+```python
+from decoutilities.screenUtils import Titler
+
+welcome = Titler('Welcome to my program!', '[ Press anything to continue ]')  # last argument is optional
+
+welcome.show()
+```
+
 ## Experimental Features
 
 All features marked as in `BETA` or being `EXPERIMENTAL` are untested, what means they were only tested below specific condititons and not with all case of uses.
 
 Please report any issues or contribute by making a PR (look for [CONTRIBUTING](CONTRIBUTING) section for details).
 
 ### REMEMBER:
```

### Comparing `decoutilities-0.3.3/README.md` & `decoutilities-0.3.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -561,14 +561,37 @@
 ```python
 email = Input('Email', '', 'REQUIRED|EMAIL', 'Enter your email')
 email.display()
 ```
 
 This will create an input that requires a valid email address.
 
+## Screen Utils
+
+### Screen
+
+Screen is a way to easily know the terminal's size. Altough for the moment it only has this feature, will have more as the development continues. As right now this feature is not long enough to have its own section on the README.md I will not explain it in detail, however you are free to check the source code if wondering to use it.
+
+Planned:
+- Screen division
+- Tab manager
+- Freeze screens
+
+### Titler
+
+This one, relays on the `Screen` feature, and allows to make simple titles.
+
+```python
+from decoutilities.screenUtils import Titler
+
+welcome = Titler('Welcome to my program!', '[ Press anything to continue ]')  # last argument is optional
+
+welcome.show()
+```
+
 ## Experimental Features
 
 All features marked as in `BETA` or being `EXPERIMENTAL` are untested, what means they were only tested below specific condititons and not with all case of uses.
 
 Please report any issues or contribute by making a PR (look for [CONTRIBUTING](CONTRIBUTING) section for details).
 
 ### REMEMBER:
```

### Comparing `decoutilities-0.3.3/decoutilities/__init__.py` & `decoutilities-0.3.4/decoutilities/__init__.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.3.3/decoutilities/components/checkmark.py` & `decoutilities-0.3.4/decoutilities/components/checkmark.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.3.3/decoutilities/components/input.py` & `decoutilities-0.3.4/decoutilities/components/input.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.3.3/decoutilities/components/selector.py` & `decoutilities-0.3.4/decoutilities/components/selector.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.3.3/decoutilities/config/config.py` & `decoutilities-0.3.4/decoutilities/config/config.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.3.3/decoutilities/config/configContainer.py` & `decoutilities-0.3.4/decoutilities/config/configContainer.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.3.3/decoutilities/data/dataEncryptor.py` & `decoutilities-0.3.4/decoutilities/data/dataEncryptor.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.3.3/decoutilities/data/keyManager.py` & `decoutilities-0.3.4/decoutilities/data/keyManager.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.3.3/decoutilities/inject/injector.py` & `decoutilities-0.3.4/decoutilities/inject/injector.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.3.3/decoutilities/logger/__init__.py` & `decoutilities-0.3.4/decoutilities/logger/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -33,8 +33,17 @@
         self.__log("SUCCESS", message)
 
     def debug(self, message):
         if self.debug:
             self.__log("DEBUG", message)
 
     def announce(self, message):
-        self.__log("ANNOUNCE", message)
+        self.__log("ANNOUNCE", message)
+
+    # @newEvent(name)
+    # Create a new event.
+    def newEvent(self, name):
+        def decorator(func):
+            def wrapper(*args, **kwargs):
+                self.__log(name, func(*args, **kwargs))
+            return wrapper
+        return decorator
```

### Comparing `decoutilities-0.3.3/decoutilities/queue/__init__.py` & `decoutilities-0.3.4/decoutilities/queue/__init__.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.3.3/decoutilities/textUtils/__init__.py` & `decoutilities-0.3.4/decoutilities/textUtils/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,16 +39,20 @@
                 return "\033[1m" + text + "\033[0m"
             case "underline":
                 return "\033[4m" + text + "\033[0m"
             case "italic":
                 return "\033[3m" + text + "\033[0m"
             case _:
                 return text
+
+    def hexColor(hexColor, text):
+        return "\033[38;2;0x" + hexColor + "m" + text + "\033[0m"
         
     def format(text):
+        import re
         aliases = {
             "{bold}": "\033[1m",
             "{underline}": "\033[4m",
             "{italic}": "\033[3m",
             "{red}": "\033[91m",
             "{green}": "\033[92m",
             "{yellow}": "\033[93m",
@@ -64,14 +68,17 @@
             "{black}": "\033[30m",
             "{reset}": "\033[0m"
         }
 
         for key, value in aliases.items():
             text = text.replace(key, value)
 
+        # Hex {#RRGGBB}
+        text = re.sub(r'{#([0-9A-Fa-f]{6})}', r'\033[38;2;0x\1m', text)
+
         return text + "\033[0m"  # reset at the end
 def format(text):
     return textUtils.format(text)
 def color(color, text):
     return textUtils.color(color, text)
 def decorate(decoration, text):
     return textUtils.decorate(decoration, text)
```

### Comparing `decoutilities-0.3.3/decoutilities.egg-info/PKG-INFO` & `decoutilities-0.3.4/decoutilities.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decoutilities
-Version: 0.3.3
+Version: 0.3.4
 Summary: Enhance the readability of your code with decorators and simplify the creation of configuration files.
 Author: Hugo Torres
 Author-email: contact@redactado.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -574,14 +574,37 @@
 ```python
 email = Input('Email', '', 'REQUIRED|EMAIL', 'Enter your email')
 email.display()
 ```
 
 This will create an input that requires a valid email address.
 
+## Screen Utils
+
+### Screen
+
+Screen is a way to easily know the terminal's size. Altough for the moment it only has this feature, will have more as the development continues. As right now this feature is not long enough to have its own section on the README.md I will not explain it in detail, however you are free to check the source code if wondering to use it.
+
+Planned:
+- Screen division
+- Tab manager
+- Freeze screens
+
+### Titler
+
+This one, relays on the `Screen` feature, and allows to make simple titles.
+
+```python
+from decoutilities.screenUtils import Titler
+
+welcome = Titler('Welcome to my program!', '[ Press anything to continue ]')  # last argument is optional
+
+welcome.show()
+```
+
 ## Experimental Features
 
 All features marked as in `BETA` or being `EXPERIMENTAL` are untested, what means they were only tested below specific condititons and not with all case of uses.
 
 Please report any issues or contribute by making a PR (look for [CONTRIBUTING](CONTRIBUTING) section for details).
 
 ### REMEMBER:
```

### Comparing `decoutilities-0.3.3/decoutilities.egg-info/SOURCES.txt` & `decoutilities-0.3.4/decoutilities.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -16,8 +16,11 @@
 decoutilities/data/__init__.py
 decoutilities/data/dataEncryptor.py
 decoutilities/data/keyManager.py
 decoutilities/inject/__init__.py
 decoutilities/inject/injector.py
 decoutilities/logger/__init__.py
 decoutilities/queue/__init__.py
+decoutilities/screenUtils/__init__.py
+decoutilities/screenUtils/screen.py
+decoutilities/screenUtils/titler.py
 decoutilities/textUtils/__init__.py
```

### Comparing `decoutilities-0.3.3/setup.py` & `decoutilities-0.3.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
 name='decoutilities',
-version='0.3.3',
+version='0.3.4',
 author='Hugo Torres',
 author_email='contact@redactado.es',
 description='Enhance the readability of your code with decorators and simplify the creation of configuration files.',
 packages=find_packages(include=['decoutilities', 'decoutilities.*']),
 classifiers=[
 'Programming Language :: Python :: 3',
 'License :: OSI Approved :: MIT License',
```

