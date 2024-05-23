# Comparing `tmp/enhancedwebdriver-0.1.6.tar.gz` & `tmp/enhancedwebdriver-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enhancedwebdriver-0.1.6.tar", last modified: Sat Apr 27 13:53:07 2024, max compression
+gzip compressed data, was "enhancedwebdriver-0.1.7.tar", last modified: Thu May 23 19:50:47 2024, max compression
```

## Comparing `enhancedwebdriver-0.1.6.tar` & `enhancedwebdriver-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-04-27 13:53:07.633942 enhancedwebdriver-0.1.6/
--rw-rw-r--   0 tesla     (1000) tesla     (1000)     1070 2024-04-12 20:08:24.000000 enhancedwebdriver-0.1.6/LICENSE
--rw-r--r--   0 tesla     (1000) tesla     (1000)     1106 2024-04-27 13:53:07.633942 enhancedwebdriver-0.1.6/PKG-INFO
--rw-rw-r--   0 tesla     (1000) tesla     (1000)      465 2024-04-13 15:12:35.000000 enhancedwebdriver-0.1.6/README.md
--rw-rw-r--   0 tesla     (1000) tesla     (1000)      106 2024-04-12 19:44:41.000000 enhancedwebdriver-0.1.6/pyproject.toml
--rw-rw-r--   0 tesla     (1000) tesla     (1000)      743 2024-04-27 13:53:07.633942 enhancedwebdriver-0.1.6/setup.cfg
-drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-04-27 13:53:07.625942 enhancedwebdriver-0.1.6/src/
-drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-04-27 13:53:07.629942 enhancedwebdriver-0.1.6/src/EnhancedWebdriver.egg-info/
--rw-r--r--   0 tesla     (1000) tesla     (1000)     1106 2024-04-27 13:53:07.000000 enhancedwebdriver-0.1.6/src/EnhancedWebdriver.egg-info/PKG-INFO
--rw-rw-r--   0 tesla     (1000) tesla     (1000)      345 2024-04-27 13:53:07.000000 enhancedwebdriver-0.1.6/src/EnhancedWebdriver.egg-info/SOURCES.txt
--rw-rw-r--   0 tesla     (1000) tesla     (1000)        1 2024-04-27 13:53:07.000000 enhancedwebdriver-0.1.6/src/EnhancedWebdriver.egg-info/dependency_links.txt
--rw-rw-r--   0 tesla     (1000) tesla     (1000)       64 2024-04-27 13:53:07.000000 enhancedwebdriver-0.1.6/src/EnhancedWebdriver.egg-info/requires.txt
--rw-rw-r--   0 tesla     (1000) tesla     (1000)       19 2024-04-27 13:53:07.000000 enhancedwebdriver-0.1.6/src/EnhancedWebdriver.egg-info/top_level.txt
-drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-04-27 13:53:07.629942 enhancedwebdriver-0.1.6/src/enhanced_webdriver/
--rw-rw-r--   0 tesla     (1000) tesla     (1000)    10376 2024-04-27 13:10:00.000000 enhancedwebdriver-0.1.6/src/enhanced_webdriver/EnhancedWebdriver.py
--rw-rw-r--   0 tesla     (1000) tesla     (1000)       82 2024-04-12 20:08:24.000000 enhancedwebdriver-0.1.6/src/enhanced_webdriver/__init__.py
+drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-05-23 19:50:47.355465 enhancedwebdriver-0.1.7/
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)     1070 2024-04-12 20:08:24.000000 enhancedwebdriver-0.1.7/LICENSE
+-rw-r--r--   0 tesla     (1000) tesla     (1000)     1106 2024-05-23 19:50:47.355465 enhancedwebdriver-0.1.7/PKG-INFO
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)      465 2024-04-13 15:12:35.000000 enhancedwebdriver-0.1.7/README.md
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)      106 2024-04-12 19:44:41.000000 enhancedwebdriver-0.1.7/pyproject.toml
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)      743 2024-05-23 19:50:47.359465 enhancedwebdriver-0.1.7/setup.cfg
+drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-05-23 19:50:47.347464 enhancedwebdriver-0.1.7/src/
+drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-05-23 19:50:47.355465 enhancedwebdriver-0.1.7/src/EnhancedWebdriver.egg-info/
+-rw-r--r--   0 tesla     (1000) tesla     (1000)     1106 2024-05-23 19:50:47.000000 enhancedwebdriver-0.1.7/src/EnhancedWebdriver.egg-info/PKG-INFO
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)      345 2024-05-23 19:50:47.000000 enhancedwebdriver-0.1.7/src/EnhancedWebdriver.egg-info/SOURCES.txt
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)        1 2024-05-23 19:50:47.000000 enhancedwebdriver-0.1.7/src/EnhancedWebdriver.egg-info/dependency_links.txt
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)       64 2024-05-23 19:50:47.000000 enhancedwebdriver-0.1.7/src/EnhancedWebdriver.egg-info/requires.txt
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)       19 2024-05-23 19:50:47.000000 enhancedwebdriver-0.1.7/src/EnhancedWebdriver.egg-info/top_level.txt
+drwxrwxr-x   0 tesla     (1000) tesla     (1000)        0 2024-05-23 19:50:47.355465 enhancedwebdriver-0.1.7/src/enhanced_webdriver/
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)    11134 2024-05-23 19:50:31.000000 enhancedwebdriver-0.1.7/src/enhanced_webdriver/EnhancedWebdriver.py
+-rw-rw-r--   0 tesla     (1000) tesla     (1000)       82 2024-04-12 20:08:24.000000 enhancedwebdriver-0.1.7/src/enhanced_webdriver/__init__.py
```

### Comparing `enhancedwebdriver-0.1.6/LICENSE` & `enhancedwebdriver-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `enhancedwebdriver-0.1.6/PKG-INFO` & `enhancedwebdriver-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EnhancedWebdriver
-Version: 0.1.6
+Version: 0.1.7
 Summary: Extension of webdriver with less boilerplate
 Home-page: https://github.com/Tesla2000/EnhancedWebdriver
 Author: Tesla2000
 Author-email: fratajczak124@gmail.com
 Project-URL: Homepage, https://github.com/Tesla2000/EnhancedWebdriver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `enhancedwebdriver-0.1.6/setup.cfg` & `enhancedwebdriver-0.1.7/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = EnhancedWebdriver
-version = 0.1.6
+version = 0.1.7
 author = Tesla2000
 author_email = fratajczak124@gmail.com
 description = Extension of webdriver with less boilerplate
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Tesla2000/EnhancedWebdriver
 project_urls =
```

### Comparing `enhancedwebdriver-0.1.6/src/EnhancedWebdriver.egg-info/PKG-INFO` & `enhancedwebdriver-0.1.7/src/EnhancedWebdriver.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EnhancedWebdriver
-Version: 0.1.6
+Version: 0.1.7
 Summary: Extension of webdriver with less boilerplate
 Home-page: https://github.com/Tesla2000/EnhancedWebdriver
 Author: Tesla2000
 Author-email: fratajczak124@gmail.com
 Project-URL: Homepage, https://github.com/Tesla2000/EnhancedWebdriver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `enhancedwebdriver-0.1.6/src/enhanced_webdriver/EnhancedWebdriver.py` & `enhancedwebdriver-0.1.7/src/enhanced_webdriver/EnhancedWebdriver.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+import typing
 from time import sleep
 from typing import Optional
+from contextlib import suppress
 
 import chromedriver_autoinstaller
 from retry import retry
 from selenium import webdriver
 from selenium.common.exceptions import (
     StaleElementReferenceException,
     NoSuchElementException,
@@ -14,15 +16,17 @@
 from selenium.webdriver import ActionChains
 from selenium.webdriver.chrome.service import Service
 from selenium.webdriver.common.by import By
 from selenium.webdriver.remote.webdriver import WebDriver
 from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.support import expected_conditions
 from selenium.webdriver.support.wait import WebDriverWait
-from undetected_chromedriver import ChromeOptions
+
+if typing.TYPE_CHECKING:
+    from undetected_chromedriver import ChromeOptions
 
 
 class EnhancedWebdriver(WebDriver):
     """Webdriver with added functions that can decrease boilerplates.
 
     :class:`EnhancedWebDriver` extends :class:`WebDriver` with additional features.
 
@@ -36,15 +40,15 @@
         )
 
     @classmethod
     def create(
         cls,
         web_driver: Optional[WebDriver] = None,
         undetected: bool = False,
-        options: ChromeOptions = None,
+        options: "ChromeOptions" = None,
         service: Service = None,
         keep_alive: bool = True,
     ) -> "EnhancedWebdriver":
         """
         Create an instance of EnhancedWebDriver.
 
         :param web_driver: An optional instance of WebDriver.[WebDriver], optional
@@ -88,168 +92,184 @@
 
         """
         self.quit()
 
     @retry(tries=5, delay=1)
     def get_text_of_element(self, value: str, by: By = By.XPATH, seconds=1) -> str:
         """
-        Get the visible (i.e., not hidden by CSS) innerText of this element.
+        Get the visible (i.e., not hidden by CSS) innerText of this elements.
 
-        :param value: Locator value of the element.
+        :param value: Locator value of the elements.
         :param by: Locator strategy, defaults to By.XPATH.
-        :param seconds: Maximum time to wait for the element, defaults to 1.
-        :return: The innerText of the element.
+        :param seconds: Maximum time to wait for the elements, defaults to 1.
+        :return: The innerText of the elements.
 
         """
-        elem = self._wait(value, seconds, by)
+        elem = self.get_element(value, seconds, by)
         return elem.text or elem.get_attribute("textContent")
 
     @retry(tries=5, delay=1)
     def is_element_present(
         self, value: str, seconds: float = 1, by: By = By.XPATH
     ) -> bool:
         """
-        Check if an element is present in the DOM.
+        Check if an elements is present in the DOM.
 
-        :param value: Locator value of the element.
-        :param seconds: Maximum time to wait for the element, defaults to 1.
+        :param value: Locator value of the elements.
+        :param seconds: Maximum time to wait for the elements, defaults to 1.
         :param by: Locator strategy, defaults to By.XPATH.
-        :return: True if element is present, False otherwise.
+        :return: True if elements is present, False otherwise.
 
         """
         try:
-            self._wait(value, seconds, by)
+            self.get_element(value, seconds, by)
             return True
         except NoSuchElementException:
             return False
 
     @retry(tries=5, delay=1)
     def is_element_selected(
         self, value: str, seconds: float = 1, by: By = By.XPATH
     ) -> bool:
         """
-        Determine if the element is selected or not.
+        Determine if the elements is selected or not.
+
+        :param value: Locator value of the elements.
+        :param seconds: Maximum time to wait for the elements, defaults to 1.
+        :param by: Locator strategy, defaults to By.XPATH.
+        :return: True if the elements is selected, False otherwise.
+
+        """
+        return self.get_element(value, seconds, by).is_selected()
+
+    def is_element_displayed(
+        self, value: str, seconds: float = 1, by: By = By.XPATH
+    ) -> bool:
+        """
+        Determine if the elements is selected or not.
 
-        :param value: Locator value of the element.
-        :param seconds: Maximum time to wait for the element, defaults to 1.
+        :param value: Locator value of the elements.
+        :param seconds: Maximum time to wait for the elements, defaults to 1.
         :param by: Locator strategy, defaults to By.XPATH.
-        :return: True if the element is selected, False otherwise.
+        :return: True if the elements is selected, False otherwise.
 
         """
-        return self._wait(value, seconds, by).is_selected()
+        with suppress(NoSuchElementException):
+            return self.get_all_elements(value, by).is_displayed()
+        return False
 
     @retry(tries=5, delay=1)
     def get_attribute(self, value: str, dtype: str, by: By = By.XPATH, seconds=10):
         """
-        Get the value of the specified attribute of the element.
+        Get the value of the specified attribute of the elements.
 
-        :param value: Locator value of the element.
+        :param value: Locator value of the elements.
         :param dtype: Name of the attribute to retrieve.
         :param by: Locator strategy, defaults to By.XPATH.
-        :param seconds: Maximum time to wait for the element, defaults to 10.
+        :param seconds: Maximum time to wait for the elements, defaults to 10.
         :return: The value of the attribute.
 
         """
-        return self._wait(value, seconds, by).get_attribute(dtype)
+        return self.get_element(value, seconds, by).get_attribute(dtype)
 
     @retry(tries=5, delay=1)
     def get_all_elements(self, element, by: By = By.XPATH):
         """
         Find all elements within the current context using the given mechanism.
 
-        :param element: Locator value of the element.
+        :param element: Locator value of the elements.
         :param by: Locator strategy, defaults to By.XPATH.
         :return: A list of all WebElements matching the criteria.
 
         """
         return self.find_elements(by=by, value=element)
 
     @retry(tries=5, delay=1)
     def write(
         self, value: str, keys: str, sleep_function=None, by: By = By.XPATH, time=10
     ) -> bool:
         """
-        Simulate typing into the element.
+        Simulate typing into the elements.
 
-        :param value: Locator value of the element.
+        :param value: Locator value of the elements.
         :param keys: The text to be typed.
         :param sleep_function: Function to execute after typing.
         :param by: Locator strategy, defaults to By.XPATH.
-        :param time: Maximum time to wait for the element, defaults to 10.
+        :param time: Maximum time to wait for the elements, defaults to 10.
         :return: True if typing was successful, False otherwise.
 
         """
         try:
-            element = self._wait(value, time, by)
+            element = self.get_element(value, time, by)
             element.clear()
             element.send_keys(str(keys))
             if sleep_function:
                 sleep_function()
         except WebDriverException:
             return False
         return True
 
     @retry(tries=5, delay=1)
     def click(self, value: str, sleep_function=None, by: By = By.XPATH, seconds=1):
         """
-        Click on an element.
+        Click on an elements.
 
-        :param value: Locator value of the element.
+        :param value: Locator value of the elements.
         :param sleep_function: Function to execute after clicking.
         :param by: Locator strategy, defaults to By.XPATH.
-        :param seconds: Maximum time to wait for the element, defaults to 1.
+        :param seconds: Maximum time to wait for the elements, defaults to 1.
         :return: True if click was successful,
 
         """
         try:
-            element = self._wait(value, seconds, by)
+            element = self.get_element(value, seconds, by)
             WebDriverWait(self, seconds).until(
                 expected_conditions.element_to_be_clickable(element)
             ).click()
 
             if sleep_function:
                 sleep_function()
         except ElementClickInterceptedException:
             sleep(0.01)
             WebDriverWait(self, seconds).until(
                 expected_conditions.element_to_be_clickable(
-                    self._wait(value, seconds, by)
+                    self.get_element(value, seconds, by)
                 )
             ).click()
         except (
             NoSuchElementException,
             TimeoutException,
             StaleElementReferenceException,
         ) as _:
             return False
         return True
 
     @retry(tries=5, delay=1)
     def wait_and_click_js(self, value: str, time=1, by: By = By.XPATH):
         """
-        Wait for an element to be present in the DOM and click using JavaScript.
+        Wait for an elements to be present in the DOM and click using JavaScript.
 
-        :param value: Locator value of the element.
-        :param time: Maximum time to wait for the element, defaults to 1.
+        :param value: Locator value of the elements.
+        :param time: Maximum time to wait for the elements, defaults to 1.
         :param by: Locator strategy, defaults to By.XPATH.
 
         """
-        element = self._wait(value, time, by)
+        element = self.get_element(value, time, by)
         self.execute_script("arguments[0].click();", element)
 
     @retry(tries=5, delay=1)
     def get_canvas(self, canvas_path: str = "//canvas"):
         """
         Get a screenshot of the canvas.
 
-        :param canvas_path: Locator value of the canvas element, defaults to "//canvas".
+        :param canvas_path: Locator value of the canvas elements, defaults to "//canvas".
         :return: Screenshot of the canvas.
 
         """
-        canvas = self._wait(canvas_path)
+        canvas = self.get_element(canvas_path)
         return canvas.screenshot_as_png
 
     @retry(tries=5, delay=1)
     def click_on_canvas(
         self,
         offset_x: int,
         offset_y: int,
@@ -257,19 +277,19 @@
         right_click: bool = False,
     ):
         """
         Click on a specific location on the canvas.
 
         :param offset_x: X-coordinate offset.
         :param offset_y: Y-coordinate offset.
-        :param canvas_path: Locator value of the canvas element, defaults to "//canvas".
+        :param canvas_path: Locator value of the canvas elements, defaults to "//canvas".
         :param right_click: Whether to perform a right click, defaults to False.
 
         """
-        canvas = self._wait(canvas_path)
+        canvas = self.get_element(canvas_path)
         if right_click:
             ActionChains(self).move_to_element(canvas).move_by_offset(
                 offset_x, offset_y
             ).context_click().release().perform()
         else:
             ActionChains(self).move_to_element(canvas).move_by_offset(
                 offset_x, offset_y
@@ -282,21 +302,21 @@
 
     def scroll_up(self):
         """Scroll up the webpage."""
         self.execute_script("window.scrollTo(0,-250)")
         sleep(0.5)
 
     @retry(tries=5, delay=1)
-    def _wait(self, value: str, seconds: float = 1, by: By = By.XPATH) -> WebElement:
+    def get_element(self, value: str, seconds: float = 1, by: By = By.XPATH) -> WebElement:
         """
-        Wait for an element to be present in the DOM and return it.
+        Wait for an elements to be present in the DOM and return it.
 
-        :param value: Locator value of the element.
-        :param seconds: Maximum time to wait for the element, defaults to 1.
+        :param value: Locator value of the elements.
+        :param seconds: Maximum time to wait for the elements, defaults to 1.
         :param by: Locator strategy, defaults to By.XPATH.
-        :return: The located element.
+        :return: The located elements.
 
         """
         self.implicitly_wait(seconds)
         element = self.find_element(by, value)
         sleep(0.5)
         return element
```

