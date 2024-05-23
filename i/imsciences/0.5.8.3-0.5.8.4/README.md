# Comparing `tmp/imsciences-0.5.8.3.tar.gz` & `tmp/imsciences-0.5.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imsciences-0.5.8.3.tar", last modified: Mon May 20 13:56:16 2024, max compression
+gzip compressed data, was "imsciences-0.5.8.4.tar", last modified: Thu May 23 11:52:55 2024, max compression
```

## Comparing `imsciences-0.5.8.3.tar` & `imsciences-0.5.8.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 13:56:16.460247 imsciences-0.5.8.3/
--rw-rw-rw-   0        0        0     9976 2024-05-20 13:56:16.453184 imsciences-0.5.8.3/PKG-INFO
--rw-rw-rw-   0        0        0     9471 2024-05-17 09:27:28.000000 imsciences-0.5.8.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 13:56:16.391641 imsciences-0.5.8.3/imsciences/
--rw-rw-rw-   0        0        0       78 2024-05-20 13:24:02.000000 imsciences-0.5.8.3/imsciences/__init__.py
--rw-rw-rw-   0        0        0   103177 2024-05-20 13:55:59.000000 imsciences-0.5.8.3/imsciences/datafunctions.py
-drwxrwxrwx   0        0        0        0 2024-05-20 13:56:16.449660 imsciences-0.5.8.3/imsciences.egg-info/
--rw-rw-rw-   0        0        0     9976 2024-05-20 13:56:16.000000 imsciences-0.5.8.3/imsciences.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2024-05-20 13:56:16.000000 imsciences-0.5.8.3/imsciences.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 13:56:16.000000 imsciences-0.5.8.3/imsciences.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-20 13:56:16.000000 imsciences-0.5.8.3/imsciences.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-20 13:56:16.000000 imsciences-0.5.8.3/imsciences.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 13:56:16.461503 imsciences-0.5.8.3/setup.cfg
--rw-rw-rw-   0        0        0     1093 2024-05-20 13:56:12.000000 imsciences-0.5.8.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 11:52:55.351038 imsciences-0.5.8.4/
+-rw-rw-rw-   0        0        0     9976 2024-05-23 11:52:55.346582 imsciences-0.5.8.4/PKG-INFO
+-rw-rw-rw-   0        0        0     9471 2024-05-17 09:27:28.000000 imsciences-0.5.8.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 11:52:55.318144 imsciences-0.5.8.4/imsciences/
+-rw-rw-rw-   0        0        0       78 2024-05-20 13:24:02.000000 imsciences-0.5.8.4/imsciences/__init__.py
+-rw-rw-rw-   0        0        0   103132 2024-05-23 11:51:45.000000 imsciences-0.5.8.4/imsciences/datafunctions.py
+drwxrwxrwx   0        0        0        0 2024-05-23 11:52:55.343069 imsciences-0.5.8.4/imsciences.egg-info/
+-rw-rw-rw-   0        0        0     9976 2024-05-23 11:52:55.000000 imsciences-0.5.8.4/imsciences.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2024-05-23 11:52:55.000000 imsciences-0.5.8.4/imsciences.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 11:52:55.000000 imsciences-0.5.8.4/imsciences.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-23 11:52:55.000000 imsciences-0.5.8.4/imsciences.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-23 11:52:55.000000 imsciences-0.5.8.4/imsciences.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 11:52:55.351038 imsciences-0.5.8.4/setup.cfg
+-rw-rw-rw-   0        0        0     1093 2024-05-23 11:52:15.000000 imsciences-0.5.8.4/setup.py
```

### Comparing `imsciences-0.5.8.3/PKG-INFO` & `imsciences-0.5.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imsciences
-Version: 0.5.8.3
+Version: 0.5.8.4
 Summary: IMS Data Processing Package
 Author: IMS
 Author-email: cam@im-sciences.com
 Keywords: python,data processing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `imsciences-0.5.8.3/README.md` & `imsciences-0.5.8.4/README.md`

 * *Files identical despite different names*

### Comparing `imsciences-0.5.8.3/imsciences/datafunctions.py` & `imsciences-0.5.8.4/imsciences/datafunctions.py`

 * *Files 1% similar despite different names*

```diff
@@ -427,15 +427,15 @@
         start_day = day_mapping.get(start_day_str.lower())
         if start_day is None:
             raise ValueError(f"Invalid day input: '{start_day_str}'. Please use one of 'mon', 'tue', 'wed', 'thu', 'fri', 'sat', 'sun'.")
 
         # Function to convert week number to start date of the week
         def week_to_startdate(week_str, start_day):
             year, week = map(int, week_str.split('-W'))
-            first_day_of_year = datetime.datetime(year, 1, 1)
+            first_day_of_year = datetime(year, 1, 1)
             day_of_week = first_day_of_year.isocalendar()[2]
             days_to_add = (7 - day_of_week + 1) if day_of_week > 4 else (1 - day_of_week)
             start_of_iso_week = first_day_of_year + datetime.timedelta(days=days_to_add)
 
             # Adjust start day
             days_to_shift = (start_day - 1) % 7
             start_of_week = start_of_iso_week + datetime.timedelta(days=days_to_shift)
@@ -861,15 +861,15 @@
         combined_FY_and_H (str, optional): String used to specify is a combined half year and FY column is desired. Defaults to "No".
 
         Returns:
         pandas.DataFrame: DataFrame with a new column 'FY' containing the FY as well as, if desired, a half year column and a combined FY half year column.
         """
         
         try:
-            start_date = datetime.datetime.strptime(start_date, '%Y-%m-%d')
+            start_date = datetime.strptime(start_date, '%Y-%m-%d')
         except ValueError:
             print("Error: Date must be of format yyyy-mm-dd")
             return df
         
         df["OBS"] = pd.to_datetime(df[index_col])
         df["OBS as string"] = df["OBS"].dt.strftime("%Y-%m-%d")
 
@@ -1417,15 +1417,15 @@
         # Define a function to get quarterly data
         def get_quarter(p_date: datetime.date) -> int:
             return (p_date.month - 1) // 3 + 1
 
         # Define a function to get the last day of the quarter
         def get_last_day_of_the_quarter(p_date: datetime.date):
             quarter = get_quarter(p_date)
-            return datetime.datetime(p_date.year + 3 * quarter // 12, 3 * quarter % 12 + 1, 1) + datetime.timedelta(days=-1)
+            return datetime(p_date.year + 3 * quarter // 12, 3 * quarter % 12 + 1, 1) + datetime.timedelta(days=-1)
         
         # For the monthly data
         data_M, subjects_M, measures_M = cif.createDataFrameFromOECD(countries = countries_list, dsname = 'MEI',subject = ['LCEAMN01',
                                                                                                                     'LCEAPR',
                                                                                                                     'CSCICP03',
                                                                                                                     'CPALTT01',
                                                                                                                     'LRHUTTTT',
@@ -1744,15 +1744,15 @@
                 df_Q.reset_index(inplace=True)
 
                 daily_records = []
                 for _, row in df_Q.iterrows():
                     year = row["Date"].year
                     month = row["Date"].month
                     day = row["Date"].day
-                    last_date = get_last_day_of_the_quarter(datetime.datetime(year,month,day).date())
+                    last_date = get_last_day_of_the_quarter(datetime(year,month,day).date())
                     all_days = pd.date_range(row["Date"],last_date,freq="D")
 
                     # Create a new record for each day of the quarter
                     for day in all_days:
                         daily_row = row.copy()
                         daily_row["Date"] = row["Date"].replace(day=day.day,month=day.month)
                         daily_records.append(daily_row)
@@ -1795,15 +1795,15 @@
     ###############################################################  Seasonality  ##########################################################################
 
     def pull_combined_dummies(self, week_commencing):
         # Week commencing dictionary
         day_dict = {"mon": 0, "tue": 1, "wed": 2, "thur": 3, "fri": 4, "sat": 5, "sun": 6}
         
         # Create daily date range dataframe
-        date_range = pd.date_range(datetime.datetime(2015, 1, 1), datetime.date.today(), freq="d")
+        date_range = pd.date_range(datetime(2015, 1, 1), datetime.date.today(), freq="d")
         df_daily = pd.DataFrame(date_range, columns=["Date"])
 
         # Create weekly date range dataframe
         df_daily['week_start'] = df_daily["Date"].apply(lambda x: x - pd.Timedelta(days=(x.weekday() - day_dict[week_commencing]) % 7))
         df_weekly_start = df_daily[['week_start']].drop_duplicates().reset_index(drop=True)
         df_weekly_start.rename(columns={'week_start': "Date"}, inplace=True)
```

### Comparing `imsciences-0.5.8.3/imsciences.egg-info/PKG-INFO` & `imsciences-0.5.8.4/imsciences.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imsciences
-Version: 0.5.8.3
+Version: 0.5.8.4
 Summary: IMS Data Processing Package
 Author: IMS
 Author-email: cam@im-sciences.com
 Keywords: python,data processing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `imsciences-0.5.8.3/setup.py` & `imsciences-0.5.8.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Function to read the contents of the README file
 def read_md(file_name):
     if os.path.isfile(file_name):
         with open(file_name, 'r', encoding='utf-8') as f:
             return f.read()
     return ''
 
-VERSION = '0.5.8.3'
+VERSION = '0.5.8.4'
 DESCRIPTION = 'IMS Data Processing Package'
 LONG_DESCRIPTION = read_md('README.md')  # Reading from README.md
 
 # Setting up
 setup(
     name="imsciences",
     version=VERSION,
```

