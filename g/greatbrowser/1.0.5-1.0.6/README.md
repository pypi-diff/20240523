# Comparing `tmp/greatbrowser-1.0.5.tar.gz` & `tmp/greatbrowser-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "greatbrowser-1.0.5.tar", last modified: Tue May 21 20:06:56 2024, max compression
+gzip compressed data, was "greatbrowser-1.0.6.tar", last modified: Thu May 23 07:22:42 2024, max compression
```

## Comparing `greatbrowser-1.0.5.tar` & `greatbrowser-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:06:56.988410 greatbrowser-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-21 20:06:45.000000 greatbrowser-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-21 20:06:56.988410 greatbrowser-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-21 20:06:45.000000 greatbrowser-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:06:56.988410 greatbrowser-1.0.5/greatbrowser/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-21 20:06:45.000000 greatbrowser-1.0.5/greatbrowser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17115 2024-05-21 20:06:45.000000 greatbrowser-1.0.5/greatbrowser/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13482 2024-05-21 20:06:45.000000 greatbrowser-1.0.5/greatbrowser/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:06:56.988410 greatbrowser-1.0.5/greatbrowser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-21 20:06:56.000000 greatbrowser-1.0.5/greatbrowser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-21 20:06:56.000000 greatbrowser-1.0.5/greatbrowser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 20:06:56.000000 greatbrowser-1.0.5/greatbrowser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-21 20:06:56.000000 greatbrowser-1.0.5/greatbrowser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 20:06:56.000000 greatbrowser-1.0.5/greatbrowser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 20:06:56.988410 greatbrowser-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-21 20:06:45.000000 greatbrowser-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:22:42.729900 greatbrowser-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-23 07:22:33.000000 greatbrowser-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-05-23 07:22:42.729900 greatbrowser-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-23 07:22:33.000000 greatbrowser-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:22:42.729900 greatbrowser-1.0.6/greatbrowser/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-23 07:22:33.000000 greatbrowser-1.0.6/greatbrowser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17726 2024-05-23 07:22:33.000000 greatbrowser-1.0.6/greatbrowser/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15334 2024-05-23 07:22:33.000000 greatbrowser-1.0.6/greatbrowser/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:22:42.729900 greatbrowser-1.0.6/greatbrowser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-05-23 07:22:42.000000 greatbrowser-1.0.6/greatbrowser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-23 07:22:42.000000 greatbrowser-1.0.6/greatbrowser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 07:22:42.000000 greatbrowser-1.0.6/greatbrowser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-23 07:22:42.000000 greatbrowser-1.0.6/greatbrowser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-23 07:22:42.000000 greatbrowser-1.0.6/greatbrowser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 07:22:42.729900 greatbrowser-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-23 07:22:33.000000 greatbrowser-1.0.6/setup.py
```

### Comparing `greatbrowser-1.0.5/LICENSE` & `greatbrowser-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `greatbrowser-1.0.5/PKG-INFO` & `greatbrowser-1.0.6/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,8 @@
-Metadata-Version: 2.1
-Name: greatbrowser
-Version: 1.0.5
-Summary: Automate Stanford's GREAT browser
-Author: Sam Anderson
-Author-email: sanderson01@wesleyan.edu
-Project-URL: Source, https://github.com/SamAndTheSun/greatbrowser
-Project-URL: Bug Reports, https://github.com/SamAndTheSun/greatbrowser/issues
-Keywords: python,genomics,genetics,greatbrowser,great,automated,analysis
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: Unix
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# greatbrowser v1.0.5
+# greatbrowser v1.0.6
 A selenium implementation in python for Stanford's GREAT browser, allowing for quick and easy genomic analysis.
 
 This repository can be installed as a module
 
 ```
 pip install greatbrowser
 ```
@@ -40,9 +23,13 @@
 while others are encapsulated within the "global_settings" dictionary parameter as key options. More specific information is available in the great_analysis() docstring. 
 Because the project uses switch statements, its requires python >= 3.10 to run. Analysis is limited to <200,000 regions.
 
 This repository is ideal for individuals attempting to conduct many different analyses using GREAT across many different probe sets. 
 It is fully functional with regards to its ability to modify table output settings, 
 but is not ideal if one desires to perform highly custom visual modifications to specifically the raw barplot or hierarchy plots generated by GREAT. 
 
+Due to the nature of GREAT browser, sometimes errors may occur if too many requests are sent quick in succession. To parse this, use headless=0 and observe
+the results. HTTP Error 500 is the most common indicator that too many requests have been sent in a short interval. This can be resolved by either
+spacing out requests or resuming analysis at a later date. This repo does not automatically space requests.
+
 This repository is not affiliated with the official GREAT browser and was developed solely for the sake of convenience.
```

### Comparing `greatbrowser-1.0.5/greatbrowser/functions.py` & `greatbrowser-1.0.6/greatbrowser/functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,21 +21,22 @@
 import numpy as np
 from PIL import Image
 import io
 
 import urllib3
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
-def format_for_great(bed_data: pd.DataFrame | pl.DataFrame | list | np.ndarray | str, df_chr, df_start, df_end, df_index,
+def format_for_great(bed_data: pd.DataFrame | pl.DataFrame | list | np.ndarray | str, get, df_chr, df_start, df_end, df_index,
                      df_score, df_strand, df_thickStart, df_thickEnd, df_rgb):
     '''
     formats the inputted data so that it is processed properly by GREAT
 
         param bed_data: the data to be assessed. The data is converted into a dataframe with the columns "chr", "start", "end", and "name"
             If there are enough columns, score, strand, thickStart, thickEnd, and rgb are also made into columns
+        param get: determines what information is generated by the function. for more information call great_get_options()
         param df_chr: the name of the column in bed_data representing chromosome
         param df_start: the name of the column in bed_data representing start point
         param df_end: the name of the column in bed_data representing end point
         param df_index: the name of the column in bed_data representing name, or index
         param df_score: the name of the column in bed_data representing score
         param df_strand: the name of the column in bed_data representing start point
         param df_thickStart: the name of the column in bed_data representing thickStart
@@ -51,16 +52,21 @@
 
     #convert list to np array
     if isinstance(bed_data, list):
         bed_data = np.array(bed_data)
 
     #load file as df
     elif isinstance(bed_data, str):
-        try: bed_data = pd.read_excel(bed_data)
-        except: bed_data = pd.read_csv(bed_data)
+        try: bed_data = pd.read_excel(bed_data); print('exc')
+        except: 
+            bed_source = bed_data
+            bed_data = pd.read_csv(bed_data, sep='\t')
+        #if csv, not tsv/BED
+        if bed_data.shape[1] == 1:
+            bed_data = pd.read_csv(bed_source, sep=',')
 
     #format df
     if isinstance(bed_data, pd.DataFrame) or isinstance(bed_data, pl.DataFrame):
 
         bed_data[df_start] = bed_data[df_start].astype(int)
         bed_data[df_end] = bed_data[df_end].astype(int)
 
@@ -84,17 +90,18 @@
         if potential_cols[0] not in df_dict: raise Exception(f'KeyError: "{df_chr}" not found in columns')
         if potential_cols[1] not in df_dict: raise Exception(f'KeyError: "{df_start}" not found in columns')
         if potential_cols[2] not in df_dict: raise Exception(f'KeyError: "{df_end}" not found in columns')
 
     else:
         print('Invalid file type detected. Must be either pandas dataframe, polars dataframe, list, numpy array, or path (str)')
 
-    #add _ to all indices to differentiate them from genes in parsing
-    bed_data[df_index] = bed_data[df_index].astype(str)   
-    bed_data[df_index] = bed_data[df_index] + '_'
+    if get == 'genes':
+        #add _ to all indices to differentiate them from genes in parsing
+        bed_data[df_index] = bed_data[df_index].astype(str)   
+        bed_data[df_index] = bed_data[df_index] + '_'
 
     return bed_data
 
 def get_genes(driver):
     '''
     get the gene table for a given region set
         param driver: the driver focused on the webpage of interest
@@ -114,31 +121,37 @@
         except IndexError: pass
 
     #Find the relevant gene table
     try:
         soup = BeautifulSoup(driver.page_source, 'lxml')
         tables = soup.find_all('table', class_='gSubTable')
     except WebDriverException:
-        raise Exception('Error: Loading exceeded 1 minute. Potential reasons: dataset too large for GREAT or connection problems. To get gene associations for large datasets, split the dataset first. Use headless=False to troubleshoot')
+        raise Exception('Error: Cannot locate table. Potential reasons: dataset too large for GREAT or connection problems. To get gene associations for large datasets, split the dataset first. Use headless=False to troubleshoot')
 
-    #Find all gene names and positions
-    gene_tags = tables[0].find_all('td')
+    try:
+        #Find all gene names and positions
+        gene_tags = tables[0].find_all('td')
+    except IndexError:
+        raise Exception('Error: Too many requests sent in quick succession. Please delay submitting requests to GREAT')
 
     #prepare to create list of genes from table
     gene_by_ids = []
-    gene_list = []
 
     #Extract gene names / positions by id
     for tag in gene_tags:
         if '_' in tag.text: #differentiate between indices and values
-            gene_by_ids.append(gene_list)
+            try: gene_by_ids.append(gene_list)
+            except UnboundLocalError: pass
             gene_list = []
         else:
             gene_list.append(tag.text)
     
+    gene_by_ids.append(gene_list)
+    gene_by_ids = [x[0] for x in gene_by_ids]
+
     return gene_by_ids
 
 def get_genes_pivot(driver):
     '''
     get the region table for a given gene set
         param driver: the driver focused on the webpage of interest
 
@@ -156,15 +169,15 @@
     driver.switch_to.window(driver.window_handles[1]) #focus driver on newly opened tab
 
     #Find the relevant gene table
     try:
         soup = BeautifulSoup(driver.page_source, 'lxml')
         tables = soup.find_all('table', class_='gSubTable')
     except WebDriverException:
-        raise Exception('Error: Loading exceeded 1 minute. Potential reasons: dataset too large for GREAT or connection problems. To get gene associations for large datasets, split the dataset first. Use headless=False to troubleshoot')
+        raise Exception('Error: Cannot locate table. Potential reasons: dataset too large for GREAT or connection problems. To get gene associations for large datasets, split the dataset first. Use headless=False to troubleshoot')
 
     #Find all gene names and positions
     gene_tags = tables[1].find_all('td')
     genes = gene_tags[::2]
     ids = gene_tags[1::2]
 
     for g, i in zip(genes, ids):
@@ -259,15 +272,15 @@
 
     while True: #account for serverside issues
 
         #get data from tables
         try:
             soup = BeautifulSoup(driver.page_source, 'lxml')
             tables = soup.find_all('table', class_='gSubTable')
-        except WebDriverException: raise Exception('Error: Loading exceeded 1 minute. Potential reasons: dataset too large for GREAT or connection problems. To get gene associations for large datasets, split the dataset first. Use headless=False to troubleshoot')
+        except WebDriverException: raise Exception('Error: Cannot locate table. Potential reasons: dataset too large for GREAT or connection problems. To get gene associations for large datasets, split the dataset first. Use headless=False to troubleshoot')
         soup = BeautifulSoup(driver.page_source, 'lxml')
 
         #Find the relevant table
         tables = soup.find_all('table')
         table = tables[specifier]
 
         # Iterate through each row of the table
@@ -419,13 +432,13 @@
             pass
 
     #get png
     img = driver.find_element(By.TAG_NAME, 'img')
     src = img.get_attribute('src')
     response = requests.get(src, verify=False)
     
-    #write pdf as file
-    with open(file_name, 'wb') as f:
+    #write png as file
+    with open(f'{file_name}', 'wb') as f:
         f.write(response.content)
 
     print(f"PNG image downloaded successfully as '{file_name}'")
     return
```

### Comparing `greatbrowser-1.0.5/greatbrowser/main.py` & `greatbrowser-1.0.6/greatbrowser/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.chrome.service import Service
 
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.support.ui import WebDriverWait
 
 from selenium.webdriver.common.by import By
-from selenium.common.exceptions import TimeoutException, WebDriverException
+from selenium.common.exceptions import TimeoutException, WebDriverException, UnexpectedAlertPresentException
 
 import os
 import pandas as pd
 pd.options.mode.chained_assignment = None
 
 import polars as pl
 import numpy as np
@@ -51,153 +51,176 @@
         param plot: whether or not to plot tables for certain get options, detailed in great_get_options(). options include: "bar", "hierarchy"
         param file_name: what to name any pngs downloaded via get options, detailed in great_get_options(). do not include the extension
         param global_controls: dictionary controlling certain attributes of the data analysis. see great_global_controls() for more information
  
         return: varies depending on 'get' parameters. call great_get_options() for more information
     '''
 
-    #format genetic data if not already formatted
-    if not is_formatted:
-        test_regions = format_for_great(test_regions, df_chr, df_start, df_end, df_index, df_score, df_strand, df_thickStart, df_thickEnd, df_rgb)
-        if not isinstance(background_regions, bool): 
-            background_regions = format_for_great(background_regions, df_chr, df_start, df_end, df_index, df_score, df_strand, df_thickStart, df_thickEnd, df_rgb)
-    elif isinstance(test_regions, str): #load formatted file
-        test_regions = pd.read_excel(test_regions)
-        if not isinstance(background_regions, bool):
-            background_regions = pd.read_excel(background_regions)
+    try:
     
-    #establish settings
-    options = Options()
-    options.add_argument('--ignore-ssl-errors=yes') #ignore insecure warning
-    options.add_argument('--ignore-certificate-errors')
-    options.add_argument('--disable-dev-shm-usage')
-    options.add_argument('--disable-blink-features=AutomationControlled')
-    options.add_argument("--disable-extensions")
-
-    if headless:
-        options.add_argument('--headless') #makes it so that the browser doesn't open
-
-    #split the dataset if too large
-    if test_regions.shape[0] > 200000:
-        print('Error: Datasets with over 200,000 locations are not currently supported')
-        return
-
-    #establish driver
-    driver = webdriver.Chrome(service=Service(ChromeDriverManager().install()),
-                            options=options)
-    driver.get('https://great.stanford.edu/great/public/html/')
-
-    cookies = driver.get_cookies()
-    #get cookies for requests, helps to deal with 403 denied error
-    for cookie in cookies:
-        driver.add_cookie(cookie)
-    driver.execute_script("Object.defineProperty(navigator, 'webdriver', {get: () => undefined})")
-    
-    #set assembly to desired choice
-    set_assembly = driver.find_element(By.ID, assembly)
-    set_assembly.click()
-
-    #select 'BED data'
-    use_input = driver.find_element(By.ID, 'fgChoiceData')
-    use_input.click()
-
-    #put BED data into text box
-    test_regions_string = test_regions.to_csv(index=False, header=None, sep='\t')
-    driver.execute_script('arguments[0].value = arguments[1];', driver.find_element(By.NAME, 'fgData'), test_regions_string)
-
-    #add background region data if applicable
-    if isinstance(background_regions, bool): pass
-    else:
-
-        #select button to input
-        bg_input = driver.find_element(By.XPATH, '/html/body/div[2]/div[4]/div/form/fieldset/div[3]/div/ul/li[3]/label/input')
-        bg_input.click()
-
-        #put background data into text box
-        background_regions_string = background_regions.to_csv(index=False, header=None, sep='\t')
-        driver.execute_script('arguments[0].value = arguments[1];', 
-                                driver.find_element(By.XPATH, '/html/body/div[2]/div[4]/div/form/fieldset/div[3]/div/ul/li[3]/textarea'), 
-                                background_regions_string)
+        #format genetic data if not already formatted
+        if not is_formatted:
+            test_regions = format_for_great(test_regions, get, df_chr, df_start, df_end, df_index, df_score, df_strand, df_thickStart, df_thickEnd, df_rgb)
+            if not isinstance(background_regions, bool): 
+                background_regions = format_for_great(background_regions, get, df_chr, df_start, df_end, df_index, df_score, df_strand, df_thickStart, df_thickEnd, df_rgb)
+        elif isinstance(test_regions, str): #load formatted file
+            try: test_regions = pd.read_excel(test_regions)
+            except: test_regions = pd.read_csv(test_regions, sep='\t')
+            if not isinstance(background_regions, bool):
+                try: background_regions = pd.read_excel(background_regions)
+                except: background_regions = pd.read_csv(background_regions, sep='\t')\
         
-    #show genomic region options
-    show_criteria = driver.find_element(By.ID, 'assoc_btn')
-    show_criteria.click()
-
-    #select gene association criteria
-    if assoc_criteria == 'basal':
-        pass
-    else:
-        #select criteria
-        if assoc_criteria == 'two_closest':
-            select_criteria = driver.find_element(By.ID, 'twoClosestRule')
-            select_criteria.click()
-        elif assoc_criteria == 'one_closest':
-            select_criteria = driver.find_element(By.ID, 'oneClosestRule')
-            select_criteria.click()
-        else:
-            raise Exception('Invalid criteria given. Valid options include "basal", "two_nearest", and "one_nearest"')
-
-    #change curated regulatory domain option
-    if cur_reg:
-        pass
-    else:
-        cur_reg_dom = driver.find_element(By.ID, 'adv_includeCuratedRegDoms')
-        cur_reg_dom.click()
-
-    #submit data
-    submit = driver.find_element(By.ID, 'submit_button')
-    submit.click()
-
-    #wait for the table
-    try: newelem = WebDriverWait(driver, 60).until(EC.presence_of_element_located((By.ID, 'job_description_container')))
-    except TimeoutException:
-        error_msg = driver.find_element(By.XPATH, '/html/body/div[2]/div[2]/blockquote ')
-        print(error_msg.text)
-        raise Exception('Error: Loading exceeded 1 minute. Potential reasons: invalid input (generally or for assembly) or connection problems. Use headless=False to troubleshoot.')
-    
-    #expand the table
-    driver.execute_script("document.getElementById('job_description_container').style.display = 'block';")
+        #establish settings
+        options = Options()
+        options.add_argument('--ignore-ssl-errors=yes') #ignore insecure warning
+        options.add_argument('--ignore-certificate-errors')
+        options.add_argument('--disable-dev-shm-usage')
+        options.add_argument('--disable-blink-features=AutomationControlled')
+        options.add_argument("--disable-extensions")
+
+        if headless:
+            options.add_argument('--headless') #makes it so that the browser doesn't open
+
+        #split the dataset if too large, or raise an error
+        gene_list = []
+        n = 1
+        if test_regions.shape[0] >= 200000:
+            if get == 'genes': n = -(test_regions.shape[0] // -200000)
+            else: raise Exception('Error: Datasets with >= 200,000 regions are only supported for "get = genes"')
+            
+        m = 0
+        while m < n:
+
+            #split dataset if necessary
+            working_data = test_regions[(m)*200000:(m+1)*200000]
+
+            #establish driver
+            driver = webdriver.Chrome(service=Service(ChromeDriverManager().install()),
+                                    options=options)
+            driver.get('https://great.stanford.edu/great/public/html/')
+
+            cookies = driver.get_cookies()
+            #get cookies for requests, helps to deal with 403 denied error
+            for cookie in cookies:
+                driver.add_cookie(cookie)
+            driver.execute_script("Object.defineProperty(navigator, 'webdriver', {get: () => undefined})")
+            
+            #set assembly to desired choice
+            set_assembly = driver.find_element(By.ID, assembly)
+            set_assembly.click()
+
+            #select 'BED data'
+            use_input = driver.find_element(By.ID, 'fgChoiceData')
+            use_input.click()
+
+            #put BED data into text box
+            working_string = working_data.to_csv(index=False, header=None, sep='\t')
+            driver.execute_script('arguments[0].value = arguments[1];', driver.find_element(By.NAME, 'fgData'), working_string)
+
+            #add background region data if applicable
+            if isinstance(background_regions, bool): pass
+            else:
+
+                #select button to input
+                bg_input = driver.find_element(By.XPATH, '/html/body/div[2]/div[4]/div/form/fieldset/div[3]/div/ul/li[3]/label/input')
+                bg_input.click()
+
+                #put background data into text box
+                background_regions_string = background_regions.to_csv(index=False, header=None, sep='\t')
+                driver.execute_script('arguments[0].value = arguments[1];', 
+                                        driver.find_element(By.XPATH, '/html/body/div[2]/div[4]/div/form/fieldset/div[3]/div/ul/li[3]/textarea'), 
+                                        background_regions_string)
+                
+            #show genomic region options
+            show_criteria = driver.find_element(By.ID, 'assoc_btn')
+            show_criteria.click()
+
+            #select gene association criteria
+            if assoc_criteria == 'basal':
+                pass
+            else:
+                #select criteria
+                if assoc_criteria == 'two_closest':
+                    select_criteria = driver.find_element(By.ID, 'twoClosestRule')
+                    select_criteria.click()
+                elif assoc_criteria == 'one_closest':
+                    select_criteria = driver.find_element(By.ID, 'oneClosestRule')
+                    select_criteria.click()
+                else:
+                    raise Exception('Invalid criteria given. Valid options include "basal", "two_nearest", and "one_nearest"')
+
+            #change curated regulatory domain option
+            if cur_reg:
+                pass
+            else:
+                cur_reg_dom = driver.find_element(By.ID, 'adv_includeCuratedRegDoms')
+                cur_reg_dom.click()
+
+            #submit data
+            submit = driver.find_element(By.ID, 'submit_button')
+            submit.click()
+
+            #wait for the table
+            try: newelem = WebDriverWait(driver, 20).until(EC.presence_of_element_located((By.ID, 'job_description_container')))
+            except TimeoutException:
+                error_msg = driver.find_element(By.XPATH, '/html/body/div[2]/div[2]/blockquote ')
+                print(error_msg.text)
+                raise Exception('Error: Loading exceeded 20 seconds. Potential reasons: invalid input (generally or for assembly) or connection problems. Use headless=False to troubleshoot.')
+            
+            #expand the table
+            driver.execute_script("document.getElementById('job_description_container').style.display = 'block';")
+
+            #modify global controls
+            if isinstance(global_controls, dict):
+                adjust_global_controls(driver, global_controls)
+
+            #get desired data
+            output = False #default output
+            n_table = False #default table
+            match get:
+                case 'genes':
+                    gene_list.extend(get_genes(driver))
+                    if (n == 1) or (m == (n-1)): #if last iteration
+                        test_regions[df_index] = test_regions[df_index].str.slice(0, -1) #remove added '_' in index
+                        output = test_regions
+                        output['associated_genes'] = gene_list
+                    else:
+                        pass
+                case 'ucsc_browser': get_ucsc_browser(driver) 
+                case 'genes_pivot': output = get_genes_pivot(driver)
+                case 'n_genes_region': get_n_genes_region(driver, 0, file_name, get)
+                case 'n_genes_TSS': get_n_genes_region(driver, 1, file_name, get)
+                case 'n_genes_abs_TSS': get_n_genes_region(driver, 2, file_name, get)
+                case 'ensembl_genes': n_table = 0; output = get_table(driver, n_table)
+                case 'go_process': n_table = 1; output = get_table(driver, n_table)
+                case 'go_component': n_table = 2; output = get_table(driver, n_table)
+                case 'go_function': n_table = 3; output = get_table(driver, n_table)
+                case 'human_phenotype': n_table = 4; output = get_table(driver, n_table)
+                case 'mouse_phenotype_KO': n_table = 5; output = get_table(driver, n_table)
+                case 'mouse_phenotype': n_table = 6; output = get_table(driver, n_table)
+
+            if n > 1: #if doing multiple iterations
+                pass 
+            elif not isinstance(output, pd.DataFrame): #if an output does not exist, quit the driver and return
+                driver.quit()
+                return
+            elif not isinstance(n_table, pd.DataFrame) == False: #if a table is not defined, quit the driver and return the output
+                pass
+            elif not isinstance(plot, str): #if a table is defined, and visualization is not active, quit the driver and return the output
+                pass
+            else:
+                plot_table(driver, plot, n_table, get, file_name)
 
-    #modify global controls
-    if isinstance(global_controls, dict):
-        adjust_global_controls(driver, global_controls)
-
-    #get desired data
-    output = False #default output
-    n_table = False #default table
-    match get:
-        case 'genes':
-            test_regions[df_index] = test_regions[df_index].str.slice(0, -1) #remove added '_'
-            output = test_regions
-            output['associated_genes'] = get_genes(driver)
-        case 'ucsc_browser': get_ucsc_browser(driver) 
-        case 'genes_pivot': output = get_genes_pivot(driver)
-        case 'n_genes_region': get_n_genes_region(driver, 0, file_name, get)
-        case 'n_genes_TSS': get_n_genes_region(driver, 1, file_name, get)
-        case 'n_genes_abs_TSS': get_n_genes_region(driver, 2, file_name, get)
-        case 'ensembl_genes': n_table = 0; output = get_table(driver, n_table)
-        case 'go_process': n_table = 1; output = get_table(driver, n_table)
-        case 'go_component': n_table = 2; output = get_table(driver, n_table)
-        case 'go_function': n_table = 3; output = get_table(driver, n_table)
-        case 'human_phenotype': n_table = 4; output = get_table(driver, n_table)
-        case 'mouse_phenotype_KO': n_table = 5; output = get_table(driver, n_table)
-        case 'mouse_phenotype': n_table = 6; output = get_table(driver, n_table)
+            m+=1
 
-    if not isinstance(output, pd.DataFrame): #if an output does not exist, quit the driver and return
         driver.quit()
-        return
-    elif not isinstance(n_table, pd.DataFrame) == False: #if a table is not defined, quit the driver and return the output
-        pass
-    elif not isinstance(plot, str): #if a table is defined, and visualization is not active, quit the driver and return the output
-        pass
-    else:
-        plot_table(driver, plot, n_table, get, file_name)
+        return output
 
-    driver.quit()
-    return output
+    except UnexpectedAlertPresentException:
+        raise Exception('Error: Too many requests sent in quick succession. Please delay submitting requests to GREAT')
 
 def great_get_options():
     '''
     gives information regarding potential "get" parameter options.\
         for more in-depth information about each particular output, see https://great-help.atlassian.net/wiki/spaces/GREAT/overview'
     return: none
     '''
```

### Comparing `greatbrowser-1.0.5/greatbrowser.egg-info/PKG-INFO` & `greatbrowser-1.0.6/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: greatbrowser
-Version: 1.0.5
+Version: 1.0.6
 Summary: Automate Stanford's GREAT browser
 Author: Sam Anderson
 Author-email: sanderson01@wesleyan.edu
 Project-URL: Source, https://github.com/SamAndTheSun/greatbrowser
 Project-URL: Bug Reports, https://github.com/SamAndTheSun/greatbrowser/issues
 Keywords: python,genomics,genetics,greatbrowser,great,automated,analysis
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# greatbrowser v1.0.5
+# greatbrowser v1.0.6
 A selenium implementation in python for Stanford's GREAT browser, allowing for quick and easy genomic analysis.
 
 This repository can be installed as a module
 
 ```
 pip install greatbrowser
 ```
@@ -40,9 +40,13 @@
 while others are encapsulated within the "global_settings" dictionary parameter as key options. More specific information is available in the great_analysis() docstring. 
 Because the project uses switch statements, its requires python >= 3.10 to run. Analysis is limited to <200,000 regions.
 
 This repository is ideal for individuals attempting to conduct many different analyses using GREAT across many different probe sets. 
 It is fully functional with regards to its ability to modify table output settings, 
 but is not ideal if one desires to perform highly custom visual modifications to specifically the raw barplot or hierarchy plots generated by GREAT. 
 
+Due to the nature of GREAT browser, sometimes errors may occur if too many requests are sent quick in succession. To parse this, use headless=0 and observe
+the results. HTTP Error 500 is the most common indicator that too many requests have been sent in a short interval. This can be resolved by either
+spacing out requests or resuming analysis at a later date. This repo does not automatically space requests.
+
 This repository is not affiliated with the official GREAT browser and was developed solely for the sake of convenience.
```

### Comparing `greatbrowser-1.0.5/setup.py` & `greatbrowser-1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.5'
+VERSION = '1.0.6'
 DESCRIPTION = "Automate Stanford's GREAT browser"
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
```

