# Comparing `tmp/real_estate_realtor_com_imp_local-0.0.8.tar.gz` & `tmp/real_estate_realtor_com_imp_local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "real_estate_realtor_com_imp_local-0.0.8.tar", last modified: Wed May 15 00:44:09 2024, max compression
+gzip compressed data, was "real_estate_realtor_com_imp_local-0.0.9.tar", last modified: Wed May 15 02:48:02 2024, max compression
```

## Comparing `real_estate_realtor_com_imp_local-0.0.8.tar` & `real_estate_realtor_com_imp_local-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:44:09.362881 real_estate_realtor_com_imp_local-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-15 00:44:09.358881 real_estate_realtor_com_imp_local-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-15 00:43:37.000000 real_estate_realtor_com_imp_local-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-15 00:43:37.000000 real_estate_realtor_com_imp_local-0.0.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:44:09.358881 real_estate_realtor_com_imp_local-0.0.8/real_estate_realtor_com_imp_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:44:09.358881 real_estate_realtor_com_imp_local-0.0.8/real_estate_realtor_com_imp_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 00:43:37.000000 real_estate_realtor_com_imp_local-0.0.8/real_estate_realtor_com_imp_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12225 2024-05-15 00:43:37.000000 real_estate_realtor_com_imp_local-0.0.8/real_estate_realtor_com_imp_local/src/realtor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:44:09.358881 real_estate_realtor_com_imp_local-0.0.8/real_estate_realtor_com_imp_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-15 00:44:09.000000 real_estate_realtor_com_imp_local-0.0.8/real_estate_realtor_com_imp_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-15 00:44:09.000000 real_estate_realtor_com_imp_local-0.0.8/real_estate_realtor_com_imp_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 00:44:09.000000 real_estate_realtor_com_imp_local-0.0.8/real_estate_realtor_com_imp_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-15 00:44:09.000000 real_estate_realtor_com_imp_local-0.0.8/real_estate_realtor_com_imp_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-15 00:44:09.000000 real_estate_realtor_com_imp_local-0.0.8/real_estate_realtor_com_imp_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 00:44:09.362881 real_estate_realtor_com_imp_local-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-15 00:43:37.000000 real_estate_realtor_com_imp_local-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 02:48:02.739539 real_estate_realtor_com_imp_local-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-15 02:48:02.739539 real_estate_realtor_com_imp_local-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-15 02:47:39.000000 real_estate_realtor_com_imp_local-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-15 02:47:39.000000 real_estate_realtor_com_imp_local-0.0.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 02:48:02.739539 real_estate_realtor_com_imp_local-0.0.9/real_estate_realtor_com_imp_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 02:48:02.739539 real_estate_realtor_com_imp_local-0.0.9/real_estate_realtor_com_imp_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 02:47:39.000000 real_estate_realtor_com_imp_local-0.0.9/real_estate_realtor_com_imp_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12308 2024-05-15 02:47:39.000000 real_estate_realtor_com_imp_local-0.0.9/real_estate_realtor_com_imp_local/src/realtor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 02:48:02.739539 real_estate_realtor_com_imp_local-0.0.9/real_estate_realtor_com_imp_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-15 02:48:02.000000 real_estate_realtor_com_imp_local-0.0.9/real_estate_realtor_com_imp_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-15 02:48:02.000000 real_estate_realtor_com_imp_local-0.0.9/real_estate_realtor_com_imp_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 02:48:02.000000 real_estate_realtor_com_imp_local-0.0.9/real_estate_realtor_com_imp_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-15 02:48:02.000000 real_estate_realtor_com_imp_local-0.0.9/real_estate_realtor_com_imp_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-15 02:48:02.000000 real_estate_realtor_com_imp_local-0.0.9/real_estate_realtor_com_imp_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 02:48:02.739539 real_estate_realtor_com_imp_local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-15 02:47:39.000000 real_estate_realtor_com_imp_local-0.0.9/setup.py
```

### Comparing `real_estate_realtor_com_imp_local-0.0.8/PKG-INFO` & `real_estate_realtor_com_imp_local-0.0.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: real-estate-realtor-com-imp-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Real estate python package
 Home-page: https://github.com/circles-zone/real-estate-realtor-com-imp-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `real_estate_realtor_com_imp_local-0.0.8/README.md` & `real_estate_realtor_com_imp_local-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `real_estate_realtor_com_imp_local-0.0.8/pyproject.toml` & `real_estate_realtor_com_imp_local-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `real_estate_realtor_com_imp_local-0.0.8/real_estate_realtor_com_imp_local/src/realtor.py` & `real_estate_realtor_com_imp_local-0.0.9/real_estate_realtor_com_imp_local/src/realtor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import os
 import json
 import re
 
 import mysql.connector
 from database_mysql_local.generic_crud import GenericCRUD
+
 # from data_source_local.data_source_enum import DataSource
 # from entity_type_local.entities_type import EntitiesType
 # from entity_type_local.entity_enum import EntityTypeId
 from importer_local.ImportersLocal import ImportersLocal
 from location_local.country import Country
 from logger_local.LoggerComponentEnum import LoggerComponentEnum
-from logger_local.LoggerLocal import Logger
+from logger_local.MetaLogger import MetaLogger
 from selenium import webdriver
 from selenium.webdriver.support.wait import WebDriverWait
 from selenium.common.exceptions import NoSuchElementException
 from selenium.webdriver.common.by import By
 from python_sdk_remote.utilities import our_get_env
 
 # TODO: move to const
@@ -23,90 +24,97 @@
 LISTINGS_LIMIT_PER_PAGE = 6  # TODO: Why?
 REALTOR_COM_USER_EXTERNAL_ID = 1
 REAL_ESTATE_ENTITY_ID = 1
 REAL_ESTATE_ENTITY_TYPE_ID = 79
 REAL_ESTATE_DATA_SOURCE_ID = 15
 
 REAL_ESTATE_REALTOR_COM_SELENIUM_IMP_COMPONENT_ID = 146
-REAL_ESTATE_REALTOR_COM_SELENIUM_IMP_COMPONENT_NAME = 'real-estate-realtor_com-selenium-imp-local-python-package'
-GET_LISTING_LINKS_FROM_LOCATION_FUNCTION_NAME = 'real-estate-realtor_com-selenium-imp-local-python-package/realtor.py get_listing_links_from_location()'
+REAL_ESTATE_REALTOR_COM_SELENIUM_IMP_COMPONENT_NAME = "real-estate-realtor_com-selenium-imp-local-python-package"
+GET_LISTING_LINKS_FROM_LOCATION_FUNCTION_NAME = (
+    "real-estate-realtor_com-selenium-imp-local-python-package/realtor.py get_listing_links_from_location()"
+)
 
 logger_code_init = {
-    'component_id': REAL_ESTATE_REALTOR_COM_SELENIUM_IMP_COMPONENT_ID,
-    'component_name': REAL_ESTATE_REALTOR_COM_SELENIUM_IMP_COMPONENT_NAME,
-    'component_category': LoggerComponentEnum.ComponentCategory.Code.value,
-    'developer_email': 'tal@circlez.ai'
+    "component_id": REAL_ESTATE_REALTOR_COM_SELENIUM_IMP_COMPONENT_ID,
+    "component_name": REAL_ESTATE_REALTOR_COM_SELENIUM_IMP_COMPONENT_NAME,
+    "component_category": LoggerComponentEnum.ComponentCategory.Code.value,
+    "developer_email": "tal@circlez.ai",
 }
-# TODO: meta logger
-logger = Logger.create_logger(object=logger_code_init)
 
 importers_local = ImportersLocal()
 
 
-class Realtor(GenericCRUD):
+class Realtor(GenericCRUD, metaclass=MetaLogger, object=logger_code_init):
     def __init__(self, is_test_data: bool = False) -> None:
-        super().__init__(default_schema_name='marketplace_goods_real_estate',
-                         default_table_name='real_estate_listing_table',
-                         default_view_table_name='real_estate_listing_view',
-                         default_column_name='real_estate_listing_id',
-                         is_test_data=is_test_data)
+        super().__init__(
+            default_schema_name="marketplace_goods_real_estate",
+            default_table_name="real_estate_listing_table",
+            default_view_table_name="real_estate_listing_view",
+            default_column_name="real_estate_listing_id",
+            is_test_data=is_test_data,
+        )
         self.country = Country()
 
         # create a new ChromeDriver instance
         options = webdriver.ChromeOptions()
-        if not our_get_env('DISABLE_HEADLESS_MODE', raise_if_not_found=False):
+        if not our_get_env("DISABLE_HEADLESS_MODE", raise_if_not_found=False):
             options.add_argument("--headless")
         self.driver = webdriver.Chrome(options=options)
 
     def get_listing_links_from_location(self, location: str) -> list[str]:
 
         location_base_url = self.get_link_from_location(location)
-        listings = [self.extract_listings_from_listings_page(f"{location_base_url}/p{page_num}")
-                    for page_num in range(1, PAGE_LIMIT + 1)]
+        listings = [
+            self.extract_listings_from_listings_page(f"{location_base_url}/p{page_num}")
+            for page_num in range(1, PAGE_LIMIT + 1)
+        ]
         listings = [item for sublist in listings for item in sublist]
         return listings
 
-
     def extract_listings_from_listings_page(self, url: str) -> list[str]:
         self.driver.get(url)
         WebDriverWait(self.driver, 5).until(
-            lambda driver: self.driver.find_element(By.CLASS_NAME, "listing-split-view-wrapper"))
+            lambda driver: self.driver.find_element(By.CLASS_NAME, "listing-split-view-wrapper")
+        )
         ul_elements = self.driver.find_elements(By.CLASS_NAME, "listing-split-view-wrapper")
-        links = [elem.find_element(By.TAG_NAME, "a").get_attribute('href')
-                 for elem in ul_elements]
+        links = [elem.find_element(By.TAG_NAME, "a").get_attribute("href") for elem in ul_elements]
         # ul_next_page_elements = driver.find_elements(By.CLASS_NAME, "pagination-box")
         # li_next_page_element = ul_next_page_elements.find_element(By.TAG_NAME,"a").get_attribute('href')
         return links[:LISTINGS_LIMIT_PER_PAGE]
 
-
     def insert_to_table(self, curr_location_listings: list[dict], location: str) -> None:
         country_name = self.country.get_country_name(location)
         # TODO replace with a call to location Class location-local-python-package
         query = """
         SELECT location_id
         FROM `location`.`location_table` AS location
                  JOIN `location`.`country_table` AS country ON country.country_id = location.country_id
         WHERE nicename = %s
         LIMIT 1"""
         self.cursor.execute(query, (country_name,))
         location_id = self.cursor.fetchone()[0]
         # TODO use data_source and entity_id packages const / enum
-        importers_local.insert(data_source_id=REAL_ESTATE_DATA_SOURCE_ID, location_id=location_id,
-                               entity_type_id=REAL_ESTATE_ENTITY_TYPE_ID, url=BASE_URL, entity_id=REAL_ESTATE_ENTITY_ID,
-                               user_external_id=REALTOR_COM_USER_EXTERNAL_ID)
+        importers_local.insert(
+            data_source_id=REAL_ESTATE_DATA_SOURCE_ID,
+            location_id=location_id,
+            entity_type_id=REAL_ESTATE_ENTITY_TYPE_ID,
+            url=BASE_URL,
+            entity_id=REAL_ESTATE_ENTITY_ID,
+            user_external_id=REALTOR_COM_USER_EXTERNAL_ID,
+        )
 
         try:
             # remove all rows with agent_office_phone missing values
             # curr_location_listings = curr_location_listings.dropna(subset=['agent_office_phone'])
             self.insert_many_dicts(data_dicts=curr_location_listings)
         except Exception as exception:
             if mysql.connector.errors.IntegrityError:
-                logger.error("Duplicate key has detected", object=exception)
+                self.logger.error("Duplicate key has detected", object=exception)
             else:
-                logger.exception(object=exception)
+                self.logger.exception(object=exception)
                 raise exception
 
         # TODO
         # # Specify the table name
         # table_name = 'listings'
         # # Insert the row into the table
         # line.to_sql(name=table_name, con=engine, if_exists='replace', index=False)
@@ -115,137 +123,139 @@
         #     conn.execute(text("SELECT * FROM users")
 
         # new_row = {'real_estate_listing_id': real_estate_listing_id_int, 'agent_name': agent_name, 'agent_office_phone': phone_int,
         #            'price': price_int, 'property_type': property_type, 'land_size': land_int,
         #            'building_size': building_size_int, 'num_of_bedrooms': num_bedrooms,
         #            'num_of_bathrooms': num_bathrooms}
 
-
     def wrapper_extract_data(self, links: list[str]) -> list[dict]:
-        data = [self.extract_data(link) for link in links]            
+        data = [self.extract_data(link) for link in links]
         return data
 
-
     def extract_data(self, link: str) -> dict:
         # TODO: break to multiple functions
         agent_office_phone = None
         price = None
         property_type = None
         land_size = None
         building_size = None
         num_of_bedrooms = None
         num_of_bathrooms = None
         real_estate_listing_id = None
         agent_name = None
 
         self.driver.get(link)
-        WebDriverWait(self.driver, 5).until(
-            lambda driver: self.driver.find_element(By.CLASS_NAME, "listing-id"))
+        WebDriverWait(self.driver, 5).until(lambda driver: self.driver.find_element(By.CLASS_NAME, "listing-id"))
         title = self.driver.title
         url = self.driver.current_url
         try:
-            address = re.search(r'(\w+(?:-\w+)? (?:\w+,? )+\d+)', title)
+            address = re.search(r"(\w+(?:-\w+)? (?:\w+,? )+\d+)", title)
             if address:
                 address = address.group(0)
-                logger.info(object={'address': address})
+                self.logger.info(object={"address": address})
         except NoSuchElementException:
-            logger.warning("No address id found", object={"title": title, "url": url})
+            self.logger.warning("No address id found", object={"title": title, "url": url})
         try:
             listing_id_element = self.driver.find_element(By.CLASS_NAME, "listing-id")
             real_estate_listing_id = int(listing_id_element.text)
         except NoSuchElementException:
-            logger.warning("No listing id found", object={"title": title, "url": url})
+            self.logger.warning("No listing id found", object={"title": title, "url": url})
         try:
             agent_name_element = self.driver.find_element(By.CLASS_NAME, "agent-name")
             agent_name = agent_name_element.text
             # print(agent_name)
         except NoSuchElementException:
-            logger.warning("No agent name found", object={"title": title, "url": url})
+            self.logger.warning("No agent name found", object={"title": title, "url": url})
         try:
             agent_office_phone_element = self.driver.find_element(By.CLASS_NAME, "agent-officephone")
-            agent_office_phone = agent_office_phone_element.get_attribute('href')
-            agent_office_phone = int(''.join(re.findall(r'\d+', agent_office_phone)))
-            logger.info(object={'agent_office_phone': agent_office_phone})
+            agent_office_phone = agent_office_phone_element.get_attribute("href")
+            agent_office_phone = int("".join(re.findall(r"\d+", agent_office_phone)))
+            self.logger.info(object={"agent_office_phone": agent_office_phone})
         except NoSuchElementException:
-            logger.warning("No agent office phone found", object={"title": title, "url": url})
+            self.logger.warning("No agent office phone found", object={"title": title, "url": url})
         try:
             price_element = self.driver.find_element(By.CLASS_NAME, "property-price")
-            price = int(''.join(re.findall(r'\d+', price_element.text)))
-            logger.info(object={'price': price})
+            price = int("".join(re.findall(r"\d+", price_element.text)))
+            self.logger.info(object={"price": price})
         except NoSuchElementException:
-            logger.warning("No property price found", object={"title": title, "url": url})
+            self.logger.warning("No property price found", object={"title": title, "url": url})
         try:
-            property_type_element = self.driver.find_element(
-                by='css selector', value=".propertyTypes .basicInfoValue")
+            property_type_element = self.driver.find_element(by="css selector", value=".propertyTypes .basicInfoValue")
             property_type = property_type_element.text
         except NoSuchElementException:
-            logger.warning("No property type found", object={"title": title, "url": url})
+            self.logger.warning("No property type found", object={"title": title, "url": url})
         try:  # TODO: use selenium.By
-            land_size_element = self.driver.find_element(
-                by='css selector', value=".landSize .basicInfoValue span")
-            building_size_until_point = re.search(r'\d[\d,.]*(?=\.)', land_size_element.text).group(0)
-            land_size = int(''.join(re.findall(r'\d+', building_size_until_point)))
-            logger.info(object={'land_size': land_size})
-        except NoSuchElementException:
-            logger.warning("No land size found", object={"title": title, "url": url})
-        try:
-            building_size_element = self.driver.find_element(by='xpath',
-                                                        value="//div[text()='Building Size']/following-sibling::div/span")
-            building_size_until_point = re.search(r'\d[\d,.]*(?=\.)', building_size_element.text).group(0)
-            building_size = int(''.join(re.findall(r'\d+', building_size_until_point)))
-            logger.info(object={'building_size': building_size})
+            land_size_element = self.driver.find_element(by="css selector", value=".landSize .basicInfoValue span")
+            building_size_until_point = re.search(r"\d[\d,.]*(?=\.)", land_size_element.text).group(0)
+            land_size = int("".join(re.findall(r"\d+", building_size_until_point)))
+            self.logger.info(object={"land_size": land_size})
         except NoSuchElementException:
-            logger.warning("No building size found", object={"title": title, "url": url})
+            self.logger.warning("No land size found", object={"title": title, "url": url})
         try:
-            rooms_element = self.driver.find_element(
-                by='css selector', value=".rooms .basicInfoValue")
+            building_size_element = self.driver.find_element(
+                by="xpath",
+                value="//div[text()='Building Size']/following-sibling::div/span",
+            )
+            building_size_until_point = re.search(r"\d[\d,.]*(?=\.)", building_size_element.text).group(0)
+            building_size = int("".join(re.findall(r"\d+", building_size_until_point)))
+            self.logger.info(object={"building_size": building_size})
+        except NoSuchElementException:
+            self.logger.warning("No building size found", object={"title": title, "url": url})
+        try:
+            rooms_element = self.driver.find_element(by="css selector", value=".rooms .basicInfoValue")
             rooms = rooms_element.text
-            rooms_list = rooms.split(',')
+            rooms_list = rooms.split(",")
             num_of_bedrooms = num_of_bathrooms = 0
             for room in rooms_list:
-                room_type = re.findall(r'[a-z]+', room)[0]
-                if room_type.startswith('bath'):
-                    num_of_bathrooms = int(re.findall(r'\d+', room)[0])
-                elif room_type.startswith('bed'):
-                    num_of_bedrooms = int(re.findall(r'\d+', room)[0])
+                room_type = re.findall(r"[a-z]+", room)[0]
+                if room_type.startswith("bath"):
+                    num_of_bathrooms = int(re.findall(r"\d+", room)[0])
+                elif room_type.startswith("bed"):
+                    num_of_bedrooms = int(re.findall(r"\d+", room)[0])
                 else:
-                    logger.error("you didn't prepared well")
+                    self.logger.error("you didn't prepared well")
                     raise Exception("you didn't prepared well")
         except NoSuchElementException:
-            logger.warning("No rooms found", object={"title": title, "url": url})
-        logger.info(
-            f"{real_estate_listing_id = }\n{agent_name = }\n{agent_office_phone = }\n{price = }\n{property_type = }\n{land_size = }\n{building_size = }\n The listing includes:{num_of_bedrooms = },{num_of_bathrooms = }")
-        new_row = {'real_estate_listing_id': real_estate_listing_id, 'agent_name': agent_name,
-                   'agent_office_phone': agent_office_phone, 'price': price, 'property_type': property_type,
-                   'land_size': land_size, 'building_size': building_size, 'num_of_bedrooms': num_of_bedrooms,
-                   'num_of_bathrooms': num_of_bathrooms}
+            self.logger.warning("No rooms found", object={"title": title, "url": url})
+        self.logger.info(
+            f"{real_estate_listing_id = }\n{agent_name = }\n{agent_office_phone = }\n{price = }\n"
+            f"{property_type = }\n{land_size = }\n{building_size = }\n"
+            f"The listing includes:{num_of_bedrooms = },{num_of_bathrooms = }"
+        )
+        new_row = {
+            "real_estate_listing_id": real_estate_listing_id,
+            "agent_name": agent_name,
+            "agent_office_phone": agent_office_phone,
+            "price": price,
+            "property_type": property_type,
+            "land_size": land_size,
+            "building_size": building_size,
+            "num_of_bedrooms": num_of_bedrooms,
+            "num_of_bathrooms": num_of_bathrooms,
+        }
         return new_row
 
-
     @staticmethod
     def read_locations_from_json():
-        suffix = 'locations.json'
+        suffix = "locations.json"
         locations_file = os.path.join(os.path.dirname(__file__), suffix)
         with open(locations_file) as f:
             locations = json.load(f)
         return locations["locations"]
 
-
     @staticmethod
     def get_link_from_location(location: str) -> str:
         link = BASE_URL + location
         return link
 
-
     def main_function(self, locations: list[str] = None) -> None:
         # read locations from JSON configuration file
         if not locations:
             locations = self.read_locations_from_json()
         for location in locations:
             # Get the links of all the listings
             listing_links = self.get_listing_links_from_location(location)
             curr_location_listings = self.wrapper_extract_data(listing_links)
             self.insert_to_table(curr_location_listings, location)
 
-
     def __del__(self):
-        self.driver.quit()
+        self.driver.quit()
```

### Comparing `real_estate_realtor_com_imp_local-0.0.8/real_estate_realtor_com_imp_local.egg-info/PKG-INFO` & `real_estate_realtor_com_imp_local-0.0.9/real_estate_realtor_com_imp_local.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: real-estate-realtor-com-imp-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Real estate python package
 Home-page: https://github.com/circles-zone/real-estate-realtor-com-imp-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `real_estate_realtor_com_imp_local-0.0.8/setup.py` & `real_estate_realtor_com_imp_local-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 PACKAGE_NAME = "real-estate-realtor-com-imp-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  
-    version='0.0.8', # https://pypi.org/project/real-estate-realtor-com-imp-local/
+    version='0.0.9', # https://pypi.org/project/real-estate-realtor-com-imp-local/
     author="Circles",
     author_email="info@circles.life",
     description="PyPI Package for Real estate python package",
     long_description="This is a package for sharing common realtor functions used in different repositories",
     long_description_content_type="text/markdown",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
```

