# Comparing `tmp/trsolucoes-7.1.0.tar.gz` & `tmp/trsolucoes-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trsolucoes-7.1.0.tar", last modified: Thu May 23 13:04:34 2024, max compression
+gzip compressed data, was "trsolucoes-8.0.0.tar", last modified: Thu May 23 13:08:28 2024, max compression
```

## Comparing `trsolucoes-7.1.0.tar` & `trsolucoes-8.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 13:04:34.628853 trsolucoes-7.1.0/
--rw-rw-rw-   0        0        0     1088 2024-05-19 21:10:17.000000 trsolucoes-7.1.0/LICENCE
--rw-rw-rw-   0        0        0     2508 2024-05-23 13:04:34.628853 trsolucoes-7.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2182 2024-05-19 21:25:05.000000 trsolucoes-7.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 13:04:34.624868 trsolucoes-7.1.0/selenium_helper/
--rw-rw-rw-   0        0        0       58 2024-05-23 12:55:47.000000 trsolucoes-7.1.0/selenium_helper/__init__.py
--rw-rw-rw-   0        0        0    13601 2024-05-23 13:04:06.000000 trsolucoes-7.1.0/selenium_helper/selenium_helper.py
--rw-rw-rw-   0        0        0       42 2024-05-23 13:04:34.628853 trsolucoes-7.1.0/setup.cfg
--rw-rw-rw-   0        0        0      543 2024-05-23 13:04:25.000000 trsolucoes-7.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-23 13:04:34.627857 trsolucoes-7.1.0/trsolucoes.egg-info/
--rw-rw-rw-   0        0        0     2508 2024-05-23 13:04:34.000000 trsolucoes-7.1.0/trsolucoes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2024-05-23 13:04:34.000000 trsolucoes-7.1.0/trsolucoes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 13:04:34.000000 trsolucoes-7.1.0/trsolucoes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-23 13:04:34.000000 trsolucoes-7.1.0/trsolucoes.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 13:08:28.501736 trsolucoes-8.0.0/
+-rw-rw-rw-   0        0        0     1088 2024-05-19 21:10:17.000000 trsolucoes-8.0.0/LICENCE
+-rw-rw-rw-   0        0        0     2508 2024-05-23 13:08:28.501736 trsolucoes-8.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2182 2024-05-19 21:25:05.000000 trsolucoes-8.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 13:08:28.497750 trsolucoes-8.0.0/selenium_helper/
+-rw-rw-rw-   0        0        0       43 2024-05-23 13:08:07.000000 trsolucoes-8.0.0/selenium_helper/__init__.py
+-rw-rw-rw-   0        0        0    13509 2024-05-23 13:08:00.000000 trsolucoes-8.0.0/selenium_helper/selenium_helper.py
+-rw-rw-rw-   0        0        0       42 2024-05-23 13:08:28.501736 trsolucoes-8.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      543 2024-05-23 13:08:15.000000 trsolucoes-8.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 13:08:28.500740 trsolucoes-8.0.0/trsolucoes.egg-info/
+-rw-rw-rw-   0        0        0     2508 2024-05-23 13:08:28.000000 trsolucoes-8.0.0/trsolucoes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2024-05-23 13:08:28.000000 trsolucoes-8.0.0/trsolucoes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 13:08:28.000000 trsolucoes-8.0.0/trsolucoes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-23 13:08:28.000000 trsolucoes-8.0.0/trsolucoes.egg-info/top_level.txt
```

### Comparing `trsolucoes-7.1.0/LICENCE` & `trsolucoes-8.0.0/LICENCE`

 * *Files identical despite different names*

### Comparing `trsolucoes-7.1.0/PKG-INFO` & `trsolucoes-8.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trsolucoes
-Version: 7.1.0
+Version: 8.0.0
 Summary: Um repositório não oficial de funções de auxilio para Selenium
 Author: Tainan Ramos
 Author-email: tainan@trsolucoes.com.br
 License: MIT License
 Keywords: trsolucoes
 Requires: selenium
 Description-Content-Type: text/markdown
```

### Comparing `trsolucoes-7.1.0/README.md` & `trsolucoes-8.0.0/README.md`

 * *Files identical despite different names*

### Comparing `trsolucoes-7.1.0/selenium_helper/selenium_helper.py` & `trsolucoes-8.0.0/selenium_helper/selenium_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         Returns:
             * bool | WebElement: Retorna o elemento WebElement se return_element for True e o elemento for encontrado. Caso contrário, retorna um booleano indicando se o elemento foi encontrado (True) ou não (False).
         """
         sleep(delay_before)
         checked: bool = False
         element: WebElement
         try:
-            element = self.find_element(locator, tag_filter, timeout, max_result)
+            element = _find_element(self.driver, locator, tag_filter, timeout, max_result)
             if(element):
                 checked = True
             else:
                 checked = False
         except:
             checked = False
         sleep(delay_after)
@@ -73,15 +73,15 @@
             * delay_after (float, opcional): Tempo em segundos para esperar após enviar o texto para o elemento. Default é 0.3 segundos.
             * clear_form (bool, opcional): Se True, limpa o campo de texto antes de enviar o novo texto. Default é True.
             * click_before (bool, opcional): Se True, clica no elemento antes de enviar o texto. Default é False.
             * max_result (bool, opcional): Se True, aplica o filtro tag_filter ao resultado para retornar o elemento mais relevante. Default é False.
         """
         sleep(delay_before)
         element: WebElement
-        element = self.find_element(locator, tag_filter, timeout, max_result)
+        element = _find_element(self.driver, locator, tag_filter, timeout, max_result)
         if(click_before):
             self.wait_and_click(self.driver, locator, tag_filter)
         if(clear_form):
             element.clear()
         element.send_keys(text)
         sleep(delay_after)
 
@@ -96,15 +96,15 @@
             * timeout (int, opcional): Tempo máximo de espera pelo elemento em segundos. Default é 30 segundos.
             * delay_before (float, opcional): Tempo em segundos para esperar antes de iniciar a busca pelo elemento. Default é 0.3 segundos.
             * delay_after (float, opcional): Tempo em segundos para esperar após clicar no elemento. Default é 0.3 segundos.
             * max_result (bool, opcional): Se True, aplica o filtro tag_filter ao resultado para retornar o elemento mais relevante. Default é False.
         """
         sleep(delay_before)
         element: WebElement
-        element = self.find_element(locator, tag_filter, timeout, max_result)
+        element = _find_element(self.driver, locator, tag_filter, timeout, max_result)
         element.click()
         sleep(delay_after)
 
     def wait_and_select(self, locator: tuple[By, str], text: str, tag_filter: list[tuple[str, str]] = None, timeout: int = 30, delay_before: float = 0.3, delay_after: float = 0.3, max_result: bool = False) -> None:
         """
         Aguarda a presença de um elemento na página e seleciona uma opção por texto visível em um elemento <select>.
 
@@ -116,15 +116,15 @@
             * timeout (int, opcional): Tempo máximo de espera pelo elemento em segundos. Default é 30 segundos.
             * delay_before (float, opcional): Tempo em segundos para esperar antes de iniciar a busca pelo elemento. Default é 0.3 segundos.
             * delay_after (float, opcional): Tempo em segundos para esperar após selecionar a opção. Default é 0.3 segundos.
             * max_result (bool, opcional): Se True, aplica o filtro tag_filter ao resultado para retornar o elemento mais relevante. Default é False.
         """
         sleep(delay_before)
         element: WebElement
-        element = self.find_element(locator, tag_filter, timeout, max_result)
+        element = _find_element(self.driver, locator, tag_filter, timeout, max_result)
         select_object = Select(element)
         select_object.select_by_visible_text(text)
         sleep(delay_after)
 
     def wait_and_click_in_text(self, locator: tuple[By, str], text: str, delay_before: float = 0.3, delay_after: float = 0.3) -> None:
         """
         Aguarda um breve período e clica em um elemento cujo texto corresponde ao texto fornecido.
@@ -156,48 +156,48 @@
             * timeout (int, opcional): Tempo máximo de espera pelo elemento em segundos. Default é 30 segundos.
             * delay_before (float, opcional): Tempo em segundos para esperar antes de iniciar a busca pelo elemento. Default é 0.3 segundos.
             * delay_after (float, opcional): Tempo em segundos para esperar após passar o cursor sobre o elemento. Default é 0.3 segundos.
             * max_result (bool, opcional): Se True, aplica o filtro tag_filter ao resultado para retornar o elemento mais relevante. Default é False.
         """
         sleep(delay_before)
         element: WebElement
-        element = self.find_element(locator, tag_filter, timeout, max_result)
+        element = _find_element(self.driver, locator, tag_filter, timeout, max_result)
         actions = ActionChains(self.driver)
         actions.move_to_element(element).perform()
         sleep(delay_after)
 
-    def find_element(self, locator: tuple[By, str], tag_filter: list[tuple[str, str]], timeout: int, max_result: bool) -> WebElement:
-            """
-            Encontra um elemento na página e espera até que o elemento seja clicável.
-
-            Args:
-                * driver (WebDriver): Instância do WebDriver usada para interagir com o navegador.
-                * locator (tuple[By, str]): Localizador do elemento na forma (By, value), onde By é a estratégia de localização e value é o seletor.
-                * tag_filter (list[tuple[str, str]]): Lista de filtros de tags na forma [(atributo, valor)] para refinar a busca do elemento. Usado apenas quando a estratégia de localização é By.TAG_NAME.
-                * timeout (int): Tempo máximo de espera pelo elemento em segundos.
-                * max_result (bool): Se True, continua buscando até encontrar o elemento mais relevante baseado no filtro. Se False, retorna o primeiro elemento correspondente.
-
-            Returns:
-                * WebElement: O elemento WebElement encontrado que atende aos critérios, ou None se nenhum elemento for encontrado ou se ocorrer uma exceção.
-            """
-            element: WebElement = None
-            try:
-                if(tag_filter):
-                    WebDriverWait(self.driver, timeout).until(EC.presence_of_element_located(locator))
-                    elements = self.driver.find_elements(locator[0], locator[1])
-                    for el in elements:
-                        for filter in tag_filter:
-                            if (el.get_attribute(filter[0]) == filter[1]):
-                                element = el    
-                            else:
-                                element = None
-                                break
-                        if(element):
-                            if(max_result):
-                                continue
-                            else:
-                                break
-                else:
-                    element = WebDriverWait(self.driver, timeout).until(EC.presence_of_element_located(locator))
-            except:
-                element = None
-            return element
+def _find_element(driver: WebDriver, locator: tuple[By, str], tag_filter: list[tuple[str, str]], timeout: int, max_result: bool) -> WebElement:
+        """
+        Encontra um elemento na página e espera até que o elemento seja clicável.
+
+        Args:
+            * driver (WebDriver): Instância do WebDriver usada para interagir com o navegador.
+            * locator (tuple[By, str]): Localizador do elemento na forma (By, value), onde By é a estratégia de localização e value é o seletor.
+            * tag_filter (list[tuple[str, str]]): Lista de filtros de tags na forma [(atributo, valor)] para refinar a busca do elemento. Usado apenas quando a estratégia de localização é By.TAG_NAME.
+            * timeout (int): Tempo máximo de espera pelo elemento em segundos.
+            * max_result (bool): Se True, continua buscando até encontrar o elemento mais relevante baseado no filtro. Se False, retorna o primeiro elemento correspondente.
+
+        Returns:
+            * WebElement: O elemento WebElement encontrado que atende aos critérios, ou None se nenhum elemento for encontrado ou se ocorrer uma exceção.
+        """
+        element: WebElement = None
+        try:
+            if(tag_filter):
+                WebDriverWait(driver, timeout).until(EC.presence_of_element_located(locator))
+                elements = driver.find_elements(locator[0], locator[1])
+                for el in elements:
+                    for filter in tag_filter:
+                        if (el.get_attribute(filter[0]) == filter[1]):
+                            element = el    
+                        else:
+                            element = None
+                            break
+                    if(element):
+                        if(max_result):
+                            continue
+                        else:
+                            break
+            else:
+                element = WebDriverWait(driver, timeout).until(EC.presence_of_element_located(locator))
+        except:
+            element = None
+        return element
```

### Comparing `trsolucoes-7.1.0/setup.py` & `trsolucoes-8.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="UTF-8") as arq:
     readme = arq.read()
 
 setup(name="trsolucoes",
-      version="7.1.0",
+      version="8.0.0",
       license="MIT License",
       author="Tainan Ramos",
       long_description=readme,
       long_description_content_type="text/markdown",
       author_email="tainan@trsolucoes.com.br",
       keywords="trsolucoes",
       description="Um repositório não oficial de funções de auxilio para Selenium",
```

### Comparing `trsolucoes-7.1.0/trsolucoes.egg-info/PKG-INFO` & `trsolucoes-8.0.0/trsolucoes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trsolucoes
-Version: 7.1.0
+Version: 8.0.0
 Summary: Um repositório não oficial de funções de auxilio para Selenium
 Author: Tainan Ramos
 Author-email: tainan@trsolucoes.com.br
 License: MIT License
 Keywords: trsolucoes
 Requires: selenium
 Description-Content-Type: text/markdown
```

