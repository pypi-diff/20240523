# Comparing `tmp/cleaner_panda-0.1.8.tar.gz` & `tmp/cleaner_panda-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleaner_panda-0.1.8.tar", last modified: Thu May 23 17:25:46 2024, max compression
+gzip compressed data, was "cleaner_panda-0.1.9.tar", last modified: Thu May 23 17:46:08 2024, max compression
```

## Comparing `cleaner_panda-0.1.8.tar` & `cleaner_panda-0.1.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 17:25:46.326488 cleaner_panda-0.1.8/
--rw-rw-rw-   0        0        0    35802 2024-05-09 22:17:47.000000 cleaner_panda-0.1.8/LICENSE
--rw-rw-rw-   0        0        0     3013 2024-05-23 17:25:46.326488 cleaner_panda-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     2236 2024-05-23 14:31:35.000000 cleaner_panda-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 17:25:46.313374 cleaner_panda-0.1.8/cleaner_panda/
--rw-rw-rw-   0        0        0      508 2024-05-23 13:46:42.000000 cleaner_panda-0.1.8/cleaner_panda/__init__.py
--rw-rw-rw-   0        0        0     1371 2024-05-23 17:22:09.000000 cleaner_panda-0.1.8/cleaner_panda/categorical_encoder.py
--rw-rw-rw-   0        0        0      652 2024-05-21 14:18:40.000000 cleaner_panda-0.1.8/cleaner_panda/data_type_converter.py
--rw-rw-rw-   0        0        0     3440 2024-05-21 14:18:40.000000 cleaner_panda-0.1.8/cleaner_panda/date_time_handler.py
--rw-rw-rw-   0        0        0     3805 2024-05-23 14:42:39.000000 cleaner_panda-0.1.8/cleaner_panda/missing_value_handler.py
--rw-rw-rw-   0        0        0     2767 2024-05-23 17:20:51.000000 cleaner_panda-0.1.8/cleaner_panda/outlier_handler.py
--rw-rw-rw-   0        0        0     1817 2024-05-23 17:21:02.000000 cleaner_panda-0.1.8/cleaner_panda/scaler.py
--rw-rw-rw-   0        0        0     3464 2024-05-23 17:21:02.000000 cleaner_panda-0.1.8/cleaner_panda/text_cleaner.py
-drwxrwxrwx   0        0        0        0 2024-05-23 17:25:46.325485 cleaner_panda-0.1.8/cleaner_panda.egg-info/
--rw-rw-rw-   0        0        0     3013 2024-05-23 17:25:46.000000 cleaner_panda-0.1.8/cleaner_panda.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      713 2024-05-23 17:25:46.000000 cleaner_panda-0.1.8/cleaner_panda.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 17:25:46.000000 cleaner_panda-0.1.8/cleaner_panda.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2024-05-23 17:25:46.000000 cleaner_panda-0.1.8/cleaner_panda.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-23 17:25:46.000000 cleaner_panda-0.1.8/cleaner_panda.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-23 17:25:46.327491 cleaner_panda-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1024 2024-05-23 17:25:41.000000 cleaner_panda-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-23 17:25:46.324482 cleaner_panda-0.1.8/tests/
--rw-rw-rw-   0        0        0        0 2024-05-18 10:16:31.000000 cleaner_panda-0.1.8/tests/__init__.py
--rw-rw-rw-   0        0        0     1896 2024-05-23 13:46:42.000000 cleaner_panda-0.1.8/tests/test_categorical_encoder.py
--rw-rw-rw-   0        0        0     1343 2024-05-21 14:22:32.000000 cleaner_panda-0.1.8/tests/test_data_type_converter.py
--rw-rw-rw-   0        0        0     3973 2024-05-21 18:53:13.000000 cleaner_panda-0.1.8/tests/test_date_time_handler.py
--rw-rw-rw-   0        0        0     3853 2024-05-21 14:27:08.000000 cleaner_panda-0.1.8/tests/test_missing_value_handler.py
--rw-rw-rw-   0        0        0     2743 2024-05-21 18:53:13.000000 cleaner_panda-0.1.8/tests/test_outlier_handler.py
--rw-rw-rw-   0        0        0     3701 2024-05-21 18:53:13.000000 cleaner_panda-0.1.8/tests/test_scaler.py
--rw-rw-rw-   0        0        0     4451 2024-05-21 18:53:13.000000 cleaner_panda-0.1.8/tests/test_text_cleaner.py
+drwxrwxrwx   0        0        0        0 2024-05-23 17:46:08.762207 cleaner_panda-0.1.9/
+-rw-rw-rw-   0        0        0    35802 2024-05-09 22:17:47.000000 cleaner_panda-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0     3013 2024-05-23 17:46:08.761206 cleaner_panda-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2236 2024-05-23 14:31:35.000000 cleaner_panda-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 17:46:08.746668 cleaner_panda-0.1.9/cleaner_panda/
+-rw-rw-rw-   0        0        0      508 2024-05-23 13:46:42.000000 cleaner_panda-0.1.9/cleaner_panda/__init__.py
+-rw-rw-rw-   0        0        0     1401 2024-05-23 17:44:49.000000 cleaner_panda-0.1.9/cleaner_panda/categorical_encoder.py
+-rw-rw-rw-   0        0        0      652 2024-05-21 14:18:40.000000 cleaner_panda-0.1.9/cleaner_panda/data_type_converter.py
+-rw-rw-rw-   0        0        0     3440 2024-05-21 14:18:40.000000 cleaner_panda-0.1.9/cleaner_panda/date_time_handler.py
+-rw-rw-rw-   0        0        0     3805 2024-05-23 14:42:39.000000 cleaner_panda-0.1.9/cleaner_panda/missing_value_handler.py
+-rw-rw-rw-   0        0        0     2790 2024-05-23 17:44:05.000000 cleaner_panda-0.1.9/cleaner_panda/outlier_handler.py
+-rw-rw-rw-   0        0        0     1957 2024-05-23 17:38:51.000000 cleaner_panda-0.1.9/cleaner_panda/scaler.py
+-rw-rw-rw-   0        0        0     3550 2024-05-23 17:40:39.000000 cleaner_panda-0.1.9/cleaner_panda/text_cleaner.py
+drwxrwxrwx   0        0        0        0 2024-05-23 17:46:08.760206 cleaner_panda-0.1.9/cleaner_panda.egg-info/
+-rw-rw-rw-   0        0        0     3013 2024-05-23 17:46:08.000000 cleaner_panda-0.1.9/cleaner_panda.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      713 2024-05-23 17:46:08.000000 cleaner_panda-0.1.9/cleaner_panda.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 17:46:08.000000 cleaner_panda-0.1.9/cleaner_panda.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2024-05-23 17:46:08.000000 cleaner_panda-0.1.9/cleaner_panda.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-23 17:46:08.000000 cleaner_panda-0.1.9/cleaner_panda.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-23 17:46:08.763207 cleaner_panda-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1024 2024-05-23 17:45:10.000000 cleaner_panda-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 17:46:08.759205 cleaner_panda-0.1.9/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-18 10:16:31.000000 cleaner_panda-0.1.9/tests/__init__.py
+-rw-rw-rw-   0        0        0     1896 2024-05-23 13:46:42.000000 cleaner_panda-0.1.9/tests/test_categorical_encoder.py
+-rw-rw-rw-   0        0        0     1343 2024-05-21 14:22:32.000000 cleaner_panda-0.1.9/tests/test_data_type_converter.py
+-rw-rw-rw-   0        0        0     3973 2024-05-21 18:53:13.000000 cleaner_panda-0.1.9/tests/test_date_time_handler.py
+-rw-rw-rw-   0        0        0     3853 2024-05-21 14:27:08.000000 cleaner_panda-0.1.9/tests/test_missing_value_handler.py
+-rw-rw-rw-   0        0        0     2743 2024-05-21 18:53:13.000000 cleaner_panda-0.1.9/tests/test_outlier_handler.py
+-rw-rw-rw-   0        0        0     3701 2024-05-21 18:53:13.000000 cleaner_panda-0.1.9/tests/test_scaler.py
+-rw-rw-rw-   0        0        0     4451 2024-05-21 18:53:13.000000 cleaner_panda-0.1.9/tests/test_text_cleaner.py
```

### Comparing `cleaner_panda-0.1.8/LICENSE` & `cleaner_panda-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.8/PKG-INFO` & `cleaner_panda-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: cleaner_panda
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package for handling various data preprocessing tasks
 Home-page: https://github.com/EmirhanSyl/cleaner-panda
-Download-URL: https://github.com/EmirhanSyl/cleaner-panda/archive/refs/tags/v0.1.8.tar.gz
+Download-URL: https://github.com/EmirhanSyl/cleaner-panda/archive/refs/tags/v0.1.9.tar.gz
 Author: asimtarik & emirs
 Author-email: support@cleanpanda.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `cleaner_panda-0.1.8/README.md` & `cleaner_panda-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.8/cleaner_panda/categorical_encoder.py` & `cleaner_panda-0.1.9/cleaner_panda/categorical_encoder.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,37 +3,37 @@
 import category_encoders as ce
 
 class CategoricalEncoder:
     def __init__(self) -> None:
         pass
 
     # Label encoding
-    def label_encoding(dataframe, column):
+    def label_encoding(self, dataframe, column):
         encoder = LabelEncoder()
         dataframe[column] = encoder.fit_transform(dataframe[column])
         return dataframe
 
     # One-hot encoding
-    def one_hot_encoding(dataframe, column):
+    def one_hot_encoding(self, dataframe, column):
         one_hot_encoded = pd.get_dummies(dataframe[column], prefix=column)
         dataframe = dataframe.drop(column, axis=1)
         dataframe = dataframe.join(one_hot_encoded)
         return dataframe
 
     # Ordinal encoding
-    def ordinal_encoding(dataframe, column):
+    def ordinal_encoding(self, dataframe, column):
         encoder = OrdinalEncoder()
         dataframe[column] = encoder.fit_transform(dataframe[[column]])
         return dataframe
 
     # Binary encoding
-    def binary_encoding(dataframe, column):
+    def binary_encoding(self, dataframe, column):
         encoder = ce.BinaryEncoder(cols=[column])
         dataframe = encoder.fit_transform(dataframe)
         return dataframe
 
     # Target encoding
-    def target_encoding(dataframe, column, target):
+    def target_encoding(self, dataframe, column, target):
         encoder = ce.TargetEncoder(cols=[column])
         encoded_data = encoder.fit_transform(dataframe[column], dataframe[target])
         dataframe[column] = encoded_data
         return dataframe
```

### Comparing `cleaner_panda-0.1.8/cleaner_panda/data_type_converter.py` & `cleaner_panda-0.1.9/cleaner_panda/data_type_converter.py`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.8/cleaner_panda/date_time_handler.py` & `cleaner_panda-0.1.9/cleaner_panda/date_time_handler.py`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.8/cleaner_panda/missing_value_handler.py` & `cleaner_panda-0.1.9/cleaner_panda/missing_value_handler.py`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.8/cleaner_panda/outlier_handler.py` & `cleaner_panda-0.1.9/cleaner_panda/outlier_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,22 +34,22 @@
         else:
             dataframe.loc[(dataframe[column] < lower_bound) | (dataframe[column] > upper_bound), column] = replacement
         
         return dataframe
     
 
     # Identify outliers using Z-score method
-    def identify_outliers_zscore(data, threshold=3):
+    def identify_outliers_zscore(self, data, threshold=3):
         z_scores = np.abs(stats.zscore(data))
         outliers = z_scores > threshold
         return outliers
 
     # Handle outliers using Z-score method
-    def handle_outliers_zscore(data, threshold=3, replacement=None):
-        outliers = identify_outliers_zscore(data, threshold)
+    def handle_outliers_zscore(self, data, threshold=3, replacement=None):
+        outliers = self.identify_outliers_zscore(data, threshold)
         if replacement is None:
             # Remove outliers
             data_cleaned = data[~outliers]
         else:
             if replacement == 'median':
                 replacement_value = data.median()
             elif replacement == 'mean':
@@ -60,11 +60,11 @@
             # Replace outliers with replacement value
             data_cleaned = data.copy()
             data_cleaned[outliers] = replacement_value
 
         return data_cleaned
 
     # Winsorize data
-    def winsorize_data(data, limits=(0.05, 0.05)):
+    def winsorize_data(self, data, limits=(0.05, 0.05)):
         from scipy.stats.mstats import winsorize
         winsorized_data = winsorize(data, limits=limits)
         return pd.Series(winsorized_data)
```

### Comparing `cleaner_panda-0.1.8/cleaner_panda/scaler.py` & `cleaner_panda-0.1.9/cleaner_panda/scaler.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,48 +3,48 @@
 import numpy as np
 
 class Scaler:
     def __init__(self) -> None:
         pass
 
     # Standardize the data
-    def standardize_data(dataframe):
+    def standardize_data(self, dataframe: pd.DataFrame):
         scaler = StandardScaler()
         scaled_data = scaler.fit_transform(dataframe)
         return pd.DataFrame(scaled_data, columns=dataframe.columns)
 
     # Normalize the data
-    def normalize_data(dataframe):
+    def normalize_data(self, dataframe: pd.DataFrame):
         scaler = MinMaxScaler()
         scaled_data = scaler.fit_transform(dataframe)
         return pd.DataFrame(scaled_data, columns=dataframe.columns)
 
     # Robust scaling
-    def robust_scale_data(dataframe):
+    def robust_scale_data(self, dataframe: pd.DataFrame):
         scaler = RobustScaler()
         scaled_data = scaler.fit_transform(dataframe)
         return pd.DataFrame(scaled_data, columns=dataframe.columns)
 
     # Normalize vectors
-    def normalize_vectors(dataframe):
+    def normalize_vectors(self, dataframe: pd.DataFrame):
         norm = np.linalg.norm(dataframe, axis=1)
         normalized_data = dataframe.div(norm, axis=0)
         return pd.DataFrame(normalized_data, columns=dataframe.columns)
 
     # Log transform data
-    def log_transform_data(dataframe):
+    def log_transform_data(self, dataframe: pd.DataFrame):
         log_data = np.log1p(dataframe)
         return pd.DataFrame(log_data, columns=dataframe.columns)
 
     # MaxAbsScaler
-    def maxabs_scale_data(dataframe):
+    def maxabs_scale_data(self, dataframe: pd.DataFrame):
         scaler = MaxAbsScaler()
         scaled_data = scaler.fit_transform(dataframe)
         return pd.DataFrame(scaled_data, columns=dataframe.columns)
 
     # PowerTransformer
-    def power_transform_data(dataframe, method='yeo-johnson'):
+    def power_transform_data(self, dataframe: pd.DataFrame, method='yeo-johnson'):
         transformer = PowerTransformer(method=method)
         transformed_data = transformer.fit_transform(dataframe)
         return pd.DataFrame(transformed_data, columns=dataframe.columns)
```

### Comparing `cleaner_panda-0.1.8/cleaner_panda/text_cleaner.py` & `cleaner_panda-0.1.9/cleaner_panda/text_cleaner.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,81 +7,81 @@
 from contractions import contractions_dict
 
 nltk.download('stopwords')
 nltk.download('wordnet')
 
 class TextCleaner:
     def __init__(self) -> None:
+        self.lemmatizer = WordNetLemmatizer()
         pass
 
-    lemmatizer = WordNetLemmatizer()
 
     # Remove common words (stopwords)
-    def remove_common_words(dataframe, column):
+    def remove_common_words(self, dataframe, column):
         stop_words = set(stopwords.words('english'))
         dataframe[column] = dataframe[column].apply(lambda x: ' '.join([word for word in x.split() if word.lower() not in stop_words]))
         return dataframe
 
     # Convert text to lowercase
-    def convert_to_lowercase(dataframe, column):
+    def convert_to_lowercase(self, dataframe, column):
         dataframe[column] = dataframe[column].str.lower()
         return dataframe
 
     # Remove punctuation
-    def remove_punctuation(dataframe, column):
+    def remove_punctuation(self, dataframe, column):
         dataframe[column] = dataframe[column].str.replace(r'[^\w\s]', '', regex=True)
         return dataframe
 
     # Lemmatization
-    def lemmatization(dataframe, column):
-        dataframe[column] = dataframe[column].apply(lambda x: ' '.join([lemmatizer.lemmatize(word) for word in x.split()]))
+    def lemmatization(self, dataframe, column):
+        dataframe[column] = dataframe[column].apply(lambda x: ' '.join([self.lemmatizer.lemmatize(word) for word in x.split()]))
         return dataframe
 
     # Expand contractions
-    def expand_contractions(dataframe, column):
+    def expand_contractions(self, dataframe, column):
         contraction_re = re.compile('(%s)' % '|'.join(contractions_dict.keys()))
         def expand_text(text):
             def replace(match):
                 return contractions_dict[match.group(0)]
             return contraction_re.sub(replace, text)
         dataframe[column] = dataframe[column].apply(lambda x: expand_text(x))
         return dataframe
 
     # Remove special characters
-    def remove_special_characters(dataframe, column, remove=['.']):
+    def remove_special_characters(self, dataframe, column, remove=['.']):
         remove_re = '[' + re.escape(''.join(remove)) + ']'
         dataframe[column] = dataframe[column].str.replace(remove_re, '', regex=True)
         return dataframe
 
     # Remove numerical data
-    def remove_numerical(dataframe, column):
+    def remove_numerical(self, dataframe, column):
         dataframe[column] = dataframe[column].str.replace(r'\d+', '', regex=True)
         return dataframe
 
     # Filter out specific words
-    def filter_words(dataframe, column, remove=['fuck']):
+    def filter_words(self, dataframe, column, remove=['fuck']):
         remove_set = set(remove)
         dataframe[column] = dataframe[column].apply(lambda x: ' '.join([word for word in x.split() if word.lower() not in remove_set]))
         return dataframe
 
     # Remove stopwords
-    def remove_stopwords(dataframe, column):
+    def remove_stopwords(self, dataframe, column):
         stop_words = set(stopwords.words('english'))
         dataframe[column] = dataframe[column].apply(lambda x: ' '.join([word for word in x.split() if word.lower() not in stop_words]))
         return dataframe
 
     # Stem words
-    def stem_words(dataframe, column):
+    def stem_words(self, dataframe, column):
         stemmer = PorterStemmer()
         dataframe[column] = dataframe[column].apply(lambda x: ' '.join([stemmer.stem(word) for word in x.split()]))
         return dataframe
 
     # Remove HTML tags
-    def remove_html_tags(dataframe, column):
+    def remove_html_tags(self, dataframe, column):
         dataframe[column] = dataframe[column].apply(lambda x: BeautifulSoup(x, 'html.parser').get_text())
         return dataframe
 
     # Replace URLs with a placeholder
-    def replace_urls(dataframe, column, placeholder='[URL]'):
+    def replace_urls(self, dataframe, column, placeholder='[URL]'):
         url_pattern = re.compile(r'http\S+|www.\S+')
         dataframe[column] = dataframe[column].apply(lambda x: url_pattern.sub(placeholder, x))
         return dataframe
```

### Comparing `cleaner_panda-0.1.8/cleaner_panda.egg-info/PKG-INFO` & `cleaner_panda-0.1.9/cleaner_panda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: cleaner_panda
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package for handling various data preprocessing tasks
 Home-page: https://github.com/EmirhanSyl/cleaner-panda
-Download-URL: https://github.com/EmirhanSyl/cleaner-panda/archive/refs/tags/v0.1.8.tar.gz
+Download-URL: https://github.com/EmirhanSyl/cleaner-panda/archive/refs/tags/v0.1.9.tar.gz
 Author: asimtarik & emirs
 Author-email: support@cleanpanda.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `cleaner_panda-0.1.8/cleaner_panda.egg-info/SOURCES.txt` & `cleaner_panda-0.1.9/cleaner_panda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.8/setup.py` & `cleaner_panda-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 from setuptools import setup, find_packages
 
 setup(
     name='cleaner_panda',
-    version='0.1.8',
+    version='0.1.9',
     description='A package for handling various data preprocessing tasks',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='asimtarik & emirs',
     author_email='support@cleanpanda.com',
     url='https://github.com/EmirhanSyl/cleaner-panda',
-    download_url='https://github.com/EmirhanSyl/cleaner-panda/archive/refs/tags/v0.1.8.tar.gz',
+    download_url='https://github.com/EmirhanSyl/cleaner-panda/archive/refs/tags/v0.1.9.tar.gz',
     packages=find_packages(),
     install_requires=[
         'pandas',
         'numpy',
         'scikit-learn',
         'nltk',
         'category_encoders',
```

### Comparing `cleaner_panda-0.1.8/tests/test_categorical_encoder.py` & `cleaner_panda-0.1.9/tests/test_categorical_encoder.py`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.8/tests/test_data_type_converter.py` & `cleaner_panda-0.1.9/tests/test_data_type_converter.py`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.8/tests/test_date_time_handler.py` & `cleaner_panda-0.1.9/tests/test_date_time_handler.py`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.8/tests/test_missing_value_handler.py` & `cleaner_panda-0.1.9/tests/test_missing_value_handler.py`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.8/tests/test_outlier_handler.py` & `cleaner_panda-0.1.9/tests/test_outlier_handler.py`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.8/tests/test_scaler.py` & `cleaner_panda-0.1.9/tests/test_scaler.py`

 * *Files identical despite different names*

### Comparing `cleaner_panda-0.1.8/tests/test_text_cleaner.py` & `cleaner_panda-0.1.9/tests/test_text_cleaner.py`

 * *Files identical despite different names*

