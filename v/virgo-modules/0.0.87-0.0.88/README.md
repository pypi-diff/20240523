# Comparing `tmp/virgo_modules-0.0.87.tar.gz` & `tmp/virgo_modules-0.0.88.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virgo_modules-0.0.87.tar", last modified: Tue May 21 14:13:26 2024, max compression
+gzip compressed data, was "virgo_modules-0.0.88.tar", last modified: Thu May 23 16:45:38 2024, max compression
```

## Comparing `virgo_modules-0.0.87.tar` & `virgo_modules-0.0.88.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 14:13:26.835959 virgo_modules-0.0.87/
--rw-rw-rw-   0        0        0     1097 2024-01-28 08:59:04.000000 virgo_modules-0.0.87/LICENSE
--rw-rw-rw-   0        0        0     1411 2024-05-21 14:13:26.826506 virgo_modules-0.0.87/PKG-INFO
--rw-rw-rw-   0        0        0      354 2024-01-28 09:03:10.000000 virgo_modules-0.0.87/README.md
--rw-rw-rw-   0        0        0       42 2024-05-21 14:13:26.835959 virgo_modules-0.0.87/setup.cfg
--rw-rw-rw-   0        0        0     1230 2024-05-21 14:13:11.000000 virgo_modules-0.0.87/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:13:26.754350 virgo_modules-0.0.87/virgo_app/
-drwxrwxrwx   0        0        0        0 2024-05-21 14:13:26.774359 virgo_modules-0.0.87/virgo_app/virgo_modules/
--rw-rw-rw-   0        0        0        0 2024-01-25 18:20:42.000000 virgo_modules-0.0.87/virgo_app/virgo_modules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:13:26.822508 virgo_modules-0.0.87/virgo_app/virgo_modules/src/
--rw-rw-rw-   0        0        0        0 2024-01-25 17:59:03.000000 virgo_modules-0.0.87/virgo_app/virgo_modules/src/__init__.py
--rw-rw-rw-   0        0        0     2571 2024-04-05 07:01:35.000000 virgo_modules-0.0.87/virgo_app/virgo_modules/src/aws_utils.py
--rw-rw-rw-   0        0        0    13732 2024-05-16 12:03:48.000000 virgo_modules-0.0.87/virgo_app/virgo_modules/src/edge_utils.py
--rw-rw-rw-   0        0        0     1989 2023-12-10 12:51:06.000000 virgo_modules-0.0.87/virgo_app/virgo_modules/src/pull_artifacts.py
--rw-rw-rw-   0        0        0    72002 2024-05-21 14:13:11.000000 virgo_modules-0.0.87/virgo_app/virgo_modules/src/re_utils.py
--rw-rw-rw-   0        0        0   143298 2024-05-02 07:44:54.000000 virgo_modules-0.0.87/virgo_app/virgo_modules/src/ticketer_source.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:13:26.789400 virgo_modules-0.0.87/virgo_app/virgo_modules.egg-info/
--rw-rw-rw-   0        0        0     1411 2024-05-21 14:13:26.000000 virgo_modules-0.0.87/virgo_app/virgo_modules.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      552 2024-05-21 14:13:26.000000 virgo_modules-0.0.87/virgo_app/virgo_modules.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 14:13:26.000000 virgo_modules-0.0.87/virgo_app/virgo_modules.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      276 2024-05-21 14:13:26.000000 virgo_modules-0.0.87/virgo_app/virgo_modules.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-21 14:13:26.000000 virgo_modules-0.0.87/virgo_app/virgo_modules.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 16:45:38.887897 virgo_modules-0.0.88/
+-rw-rw-rw-   0        0        0     1097 2024-01-28 08:59:04.000000 virgo_modules-0.0.88/LICENSE
+-rw-rw-rw-   0        0        0     1411 2024-05-23 16:45:38.882897 virgo_modules-0.0.88/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2024-01-28 09:03:10.000000 virgo_modules-0.0.88/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-23 16:45:38.887897 virgo_modules-0.0.88/setup.cfg
+-rw-rw-rw-   0        0        0     1230 2024-05-23 16:27:32.000000 virgo_modules-0.0.88/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 16:45:38.800904 virgo_modules-0.0.88/virgo_app/
+drwxrwxrwx   0        0        0        0 2024-05-23 16:45:38.824897 virgo_modules-0.0.88/virgo_app/virgo_modules/
+-rw-rw-rw-   0        0        0        0 2024-01-25 18:20:42.000000 virgo_modules-0.0.88/virgo_app/virgo_modules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 16:45:38.878899 virgo_modules-0.0.88/virgo_app/virgo_modules/src/
+-rw-rw-rw-   0        0        0        0 2024-01-25 17:59:03.000000 virgo_modules-0.0.88/virgo_app/virgo_modules/src/__init__.py
+-rw-rw-rw-   0        0        0     2571 2024-04-05 07:01:35.000000 virgo_modules-0.0.88/virgo_app/virgo_modules/src/aws_utils.py
+-rw-rw-rw-   0        0        0    13732 2024-05-16 12:03:48.000000 virgo_modules-0.0.88/virgo_app/virgo_modules/src/edge_utils.py
+-rw-rw-rw-   0        0        0     1989 2023-12-10 12:51:06.000000 virgo_modules-0.0.88/virgo_app/virgo_modules/src/pull_artifacts.py
+-rw-rw-rw-   0        0        0    72244 2024-05-23 16:28:19.000000 virgo_modules-0.0.88/virgo_app/virgo_modules/src/re_utils.py
+-rw-rw-rw-   0        0        0   146629 2024-05-23 16:27:32.000000 virgo_modules-0.0.88/virgo_app/virgo_modules/src/ticketer_source.py
+drwxrwxrwx   0        0        0        0 2024-05-23 16:45:38.849900 virgo_modules-0.0.88/virgo_app/virgo_modules.egg-info/
+-rw-rw-rw-   0        0        0     1411 2024-05-23 16:45:38.000000 virgo_modules-0.0.88/virgo_app/virgo_modules.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      552 2024-05-23 16:45:38.000000 virgo_modules-0.0.88/virgo_app/virgo_modules.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 16:45:38.000000 virgo_modules-0.0.88/virgo_app/virgo_modules.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      276 2024-05-23 16:45:38.000000 virgo_modules-0.0.88/virgo_app/virgo_modules.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-23 16:45:38.000000 virgo_modules-0.0.88/virgo_app/virgo_modules.egg-info/top_level.txt
```

### Comparing `virgo_modules-0.0.87/LICENSE` & `virgo_modules-0.0.88/LICENSE`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.87/PKG-INFO` & `virgo_modules-0.0.88/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: virgo_modules
-Version: 0.0.87
+Version: 0.0.88
 Summary: data processing and statistical modeling using stock market data
 Home-page: https://github.com/miguelmayhem92/virgo_module
 Author: Miguel Mayhuire
 Author-email: miguelmayhem92@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `virgo_modules-0.0.87/setup.py` & `virgo_modules-0.0.88/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("virgo_app/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="virgo_modules",
-    version="0.0.87",
+    version="0.0.88",
     description="data processing and statistical modeling using stock market data",
     package_dir={"": "virgo_app"},
     packages=find_packages(where="virgo_app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/miguelmayhem92/virgo_module",
     author="Miguel Mayhuire",
```

### Comparing `virgo_modules-0.0.87/virgo_app/virgo_modules/src/aws_utils.py` & `virgo_modules-0.0.88/virgo_app/virgo_modules/src/aws_utils.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.87/virgo_app/virgo_modules/src/edge_utils.py` & `virgo_modules-0.0.88/virgo_app/virgo_modules/src/edge_utils.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.87/virgo_app/virgo_modules/src/pull_artifacts.py` & `virgo_modules-0.0.88/virgo_app/virgo_modules/src/pull_artifacts.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.87/virgo_app/virgo_modules/src/re_utils.py` & `virgo_modules-0.0.88/virgo_app/virgo_modules/src/re_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -696,15 +696,19 @@
         'volume_feature':'analysis_volume',  ## this may crash but deprecated
         'smooth_volume':'analysis_smooth_volume',
         'roc_feature':'roc_feature',
         'stoch_feature':'stoch_feature',
         'stochastic_feature':'stochastic_feature',
         'william_feature':'william_feature',
         'vortex_feature':'vortex_feature',
-        'pair_index_feature':'pair_index_feature' # this has a diff structure! 
+        'pair_index_feature':'pair_index_feature', # this has a diff structure!
+        'min_distance_pricefeature':'minmax_pricefeature', 
+        'min_relprice_pricefeature':'minmax_pricefeature', 
+        'max_distance_pricefeature':'minmax_pricefeature',
+        'max_relprice_pricefeature':'minmax_pricefeature',
     }
     exceptions = ['pair_feature','pair_index_feature']
     ### standar feature
     for feature in feature_map.keys():
         if (feature in ticket_settings['settings']) and (feature not in exceptions):
             parameters = ticket_settings['settings'][feature]
             method_to_use = feature_map.get(feature)
```

### Comparing `virgo_modules-0.0.87/virgo_app/virgo_modules/src/ticketer_source.py` & `virgo_modules-0.0.88/virgo_app/virgo_modules/src/ticketer_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -379,14 +379,16 @@
         perform stochastic oscilator RSI feature
     stochastic_feature(window=int, smooth=int, threshold=float, plot=boolean, save_features=boolean):
         perform stochastic oscilator feature
     william_feature(lbp=int, threshold=float, plot=boolean, save_features=boolean):
         perfom fast stochastic oscilator or william indicator
     vortex_feature(window=int, threshold=float, plot=boolean, save_features=boolean):
         perform vortex oscilator
+    minmax_pricefeature(type_func=str, window=int, distance=bolean, save_features=boolean)
+        get relative price/ distance feature with respect to the min/max price in a given window
     pair_index_feature(pair_symbol=str, feature_label=str, window=int, threshold=float, plot=boolean, save_features=boolean):
         perform additional asset ROC feature, then a new feature is created in the main dataframe
     produce_order_features(feature_name=str, save_features=boolean):
         perform a feature that captures high and low values in an index. this is usefull to know duration/persistence of a signal
     create_hmm_derived_features():
         create features derived from hmm states features. Features are the index of the state, the duration of the state, chain raturn
     cluster_hmm_analysis(n_clusters=int,features_hmm=list, test_data_size=int, seed=int, lag_returns_state=int, plot=boolean, save_features=boolean, model=obj):
@@ -1694,14 +1696,78 @@
 
         if save_features:
             self.log_features_standard(feature_name)
             self.settings_vortex_feature = {'window':window, 'threshold':threshold}
         if plot:
             self.signal_plotter(feature_name)
 
+    def minmax_pricefeature(self, type_func, window, distance = False, save_features = False):
+        """
+        perform relative price/distance with respect to the min/max price in a given time scope
+
+        Parameters
+        ----------
+        type_func (str): either min or max
+        window (int): window scope
+        distance (boolean): if true, get distance feature else relative feature
+        save_features (boolean): True to save feature configuration and feature names
+        
+        Returns
+        -------
+        None
+        """
+        if type_func == 'min':
+            self.df['Price_ref'] = self.df[['Open','High', 'Low','Close']].min(axis = 1)
+        elif type_func == 'max':
+            self.df['Price_ref'] = self.df[['Open','High', 'Low','Close']].max(axis = 1)
+
+        init_shape = self.df.shape[0]
+        df_date = self.df[['Date','Price_ref']].rename(columns = {'Date':'Date_ref'}).copy()
+        
+        self.df = self.df.rename(columns = {'Price_ref':'Price_to_use'})
+        
+        if type_func == 'min':
+            self.df[f'window_price'] = (self.df.sort_values("Date")["Price_to_use"].transform(lambda x: x.rolling(window, min_periods=1).min()))
+        elif type_func == 'max':
+            self.df[f'window_price'] = (self.df.sort_values("Date")["Price_to_use"].transform(lambda x: x.rolling(window, min_periods=1).max()))
+        
+        
+        self.df = self.df.merge(df_date, left_on = 'window_price', right_on = 'Price_ref', how = 'left')
+        self.df['date_span'] = self.df['Date'] - self.df['Date_ref']
+        
+        self.df['RN'] = self.df.sort_values(['date_span'], ascending=False).groupby(['Date']).cumcount() + 1
+        self.df = self.df[self.df['RN'] == 1]
+
+        if distance:
+            self.df[f'{type_func}_distance_to_price'] = pd.to_numeric(self.df['date_span'].dt.days, downcast='integer')
+
+        if not distance:
+            if type_func == 'min':
+                self.df[f'{type_func}_relprice'] = self.df['Price_to_use']/self.df['window_price']-1
+            
+            if type_func == 'max':
+                self.df[f'{type_func}_relprice'] = self.df['window_price']/self.df['Price_to_use']-1
+        
+        self.df = self.df.drop(columns = ['RN', 'date_span', 'Price_to_use', 'window_price', 'Date_ref','Price_ref'])
+        
+        end_shape = self.df.shape[0]
+
+        if init_shape != end_shape:
+            raise Exception("shapes are not the same")
+
+        if save_features:
+            if distance:
+                self.features.append(f'{type_func}_distance_to_price')
+                name_attr = f'{type_func}_distance'
+            if not distance:
+                self.features.append(f'{type_func}_relprice')
+                name_attr = f'{type_func}_relprice'
+                
+            setattr(self,f'settings_{name_attr}_pricefeature' , {'type_func': type_func, 'window': window, 'distance': distance})
+
     def pair_index_feature(self, pair_symbol, feature_label, window, threshold, plot = False, save_features = False):
         """
         perform additional asset ROC feature, then a new feature is created in the main dataframe
 
         Parameters
         ----------
         pair_symbol (str): symbol of the asset to extract the data
@@ -2293,15 +2359,17 @@
             self.settings['model_type'] = model_type
             self.settings['target'] = list(set(self.target))
             self.settings['targets'] = target_list
 
         ## for now this is hard coded
         feature_list = ['spread_ma','relative_spread_ma','pair_feature','count_features','bidirect_count_features','price_range','relative_price_range','rsi_feature',
                         'rsi_feature_v2', 'days_features','days_features_v2', 'volume_feature','smooth_volume', 'roc_feature', 'stoch_feature', 'stochastic_feature',
-                        'william_feature', 'vortex_feature', 'pair_index_feature','hmm']
+                        'william_feature', 'vortex_feature', 'pair_index_feature','hmm',
+                        'min_distance_pricefeature', 'min_relprice_pricefeature', 'max_distance_pricefeature','max_relprice_pricefeature'
+                        ]
 
         for feature in feature_list:
             try:
                 self.settings['settings'][feature] = getattr(self, f'settings_{feature}')
             except:
                 pass
         try:
```

### Comparing `virgo_modules-0.0.87/virgo_app/virgo_modules.egg-info/PKG-INFO` & `virgo_modules-0.0.88/virgo_app/virgo_modules.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: virgo-modules
-Version: 0.0.87
+Version: 0.0.88
 Summary: data processing and statistical modeling using stock market data
 Home-page: https://github.com/miguelmayhem92/virgo_module
 Author: Miguel Mayhuire
 Author-email: miguelmayhem92@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `virgo_modules-0.0.87/virgo_app/virgo_modules.egg-info/SOURCES.txt` & `virgo_modules-0.0.88/virgo_app/virgo_modules.egg-info/SOURCES.txt`

 * *Files identical despite different names*

