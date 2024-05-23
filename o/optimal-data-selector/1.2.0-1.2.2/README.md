# Comparing `tmp/optimal_data_selector-1.2.0.tar.gz` & `tmp/optimal_data_selector-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimal_data_selector-1.2.0.tar", last modified: Wed Nov 29 16:00:52 2023, max compression
+gzip compressed data, was "optimal_data_selector-1.2.2.tar", last modified: Thu May 23 15:49:22 2024, max compression
```

## Comparing `optimal_data_selector-1.2.0.tar` & `optimal_data_selector-1.2.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-11-29 16:00:52.402605 optimal_data_selector-1.2.0/
--rw-rw-rw-   0        0        0        0 2023-10-03 04:14:42.000000 optimal_data_selector-1.2.0/LICENSE
--rw-rw-rw-   0        0        0     2573 2023-11-29 16:00:52.400603 optimal_data_selector-1.2.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-11-29 16:00:52.243699 optimal_data_selector-1.2.0/optimal_data_selector/
--rw-rw-rw-   0        0        0        0 2023-10-03 04:14:46.000000 optimal_data_selector-1.2.0/optimal_data_selector/__init__.py
--rw-rw-rw-   0        0        0       14 2023-10-14 09:12:26.000000 optimal_data_selector-1.2.0/optimal_data_selector/__version__.py
--rw-rw-rw-   0        0        0    12045 2023-11-07 12:23:36.000000 optimal_data_selector-1.2.0/optimal_data_selector/image.py
--rw-rw-rw-   0        0        0    24354 2023-10-15 17:00:41.000000 optimal_data_selector-1.2.0/optimal_data_selector/optimal.py
--rw-rw-rw-   0        0        0        0 2023-10-03 04:14:46.000000 optimal_data_selector-1.2.0/optimal_data_selector/optimal_2.py
--rw-rw-rw-   0        0        0     5633 2023-10-03 04:14:46.000000 optimal_data_selector-1.2.0/optimal_data_selector/sequential.py
--rw-rw-rw-   0        0        0    40624 2023-11-29 15:49:32.000000 optimal_data_selector-1.2.0/optimal_data_selector/text.py
--rw-rw-rw-   0        0        0     5060 2023-10-03 04:14:47.000000 optimal_data_selector-1.2.0/optimal_data_selector/word.py
-drwxrwxrwx   0        0        0        0 2023-11-29 16:00:52.397605 optimal_data_selector-1.2.0/optimal_data_selector.egg-info/
--rw-rw-rw-   0        0        0     2573 2023-11-29 16:00:50.000000 optimal_data_selector-1.2.0/optimal_data_selector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      462 2023-11-29 16:00:50.000000 optimal_data_selector-1.2.0/optimal_data_selector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-29 16:00:50.000000 optimal_data_selector-1.2.0/optimal_data_selector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-11-29 16:00:50.000000 optimal_data_selector-1.2.0/optimal_data_selector.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-11-29 16:00:52.403603 optimal_data_selector-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     2916 2023-11-29 15:48:24.000000 optimal_data_selector-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 15:49:22.180430 optimal_data_selector-1.2.2/
+-rw-rw-rw-   0        0        0        0 2023-10-03 04:14:42.000000 optimal_data_selector-1.2.2/LICENSE
+-rw-rw-rw-   0        0        0     2726 2024-05-23 15:49:22.167429 optimal_data_selector-1.2.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-23 15:49:22.126456 optimal_data_selector-1.2.2/optimal_data_selector/
+-rw-rw-rw-   0        0        0        0 2023-10-03 04:14:46.000000 optimal_data_selector-1.2.2/optimal_data_selector/__init__.py
+-rw-rw-rw-   0        0        0       14 2023-12-31 08:24:39.000000 optimal_data_selector-1.2.2/optimal_data_selector/__version__.py
+-rw-rw-rw-   0        0        0     5199 2023-12-25 11:00:47.000000 optimal_data_selector-1.2.2/optimal_data_selector/files.py
+-rw-rw-rw-   0        0        0    12045 2023-11-07 12:23:36.000000 optimal_data_selector-1.2.2/optimal_data_selector/image.py
+-rw-rw-rw-   0        0        0    28488 2023-12-31 08:34:40.000000 optimal_data_selector-1.2.2/optimal_data_selector/optimal.py
+-rw-rw-rw-   0        0        0        0 2023-10-03 04:14:46.000000 optimal_data_selector-1.2.2/optimal_data_selector/optimal_2.py
+-rw-rw-rw-   0        0        0     5633 2023-10-03 04:14:46.000000 optimal_data_selector-1.2.2/optimal_data_selector/sequential.py
+-rw-rw-rw-   0        0        0    40624 2023-11-29 15:49:32.000000 optimal_data_selector-1.2.2/optimal_data_selector/text.py
+-rw-rw-rw-   0        0        0     5060 2023-10-03 04:14:47.000000 optimal_data_selector-1.2.2/optimal_data_selector/word.py
+drwxrwxrwx   0        0        0        0 2024-05-23 15:49:22.165432 optimal_data_selector-1.2.2/optimal_data_selector.egg-info/
+-rw-rw-rw-   0        0        0     2726 2024-05-23 15:49:21.000000 optimal_data_selector-1.2.2/optimal_data_selector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      493 2024-05-23 15:49:21.000000 optimal_data_selector-1.2.2/optimal_data_selector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 15:49:21.000000 optimal_data_selector-1.2.2/optimal_data_selector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-05-23 15:49:21.000000 optimal_data_selector-1.2.2/optimal_data_selector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 15:49:22.181424 optimal_data_selector-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     3071 2024-05-23 15:49:09.000000 optimal_data_selector-1.2.2/setup.py
```

### Comparing `optimal_data_selector-1.2.0/PKG-INFO` & `optimal_data_selector-1.2.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: optimal_data_selector
-Version: 1.2.0
-Summary: ('A Package for to optimize models, use for nlp short word treatment, choosing optimal data for ML models, use for Image Scraping , use in timeseries problem to split the data into train and test', 'Deal with emojis and emoticons in nlp,word tokenize,token, get the list of Punctuation marks and English Pronouns too, can be used to read text files')
+Version: 1.2.2
+Summary: ('A Package for optimize models, transfer or copy files from one directory to other, use for nlp short word treatment, choosing optimal data for ML models, use for Image Scraping , use in timeseries problem to split the data into train and test', 'Deal with emojis and emoticons in nlp,word tokenize,token, get the list of Punctuation marks and English Pronouns too, can be used to read text files')
 Author: Rohan Majumder
 Author-email: majumderrohan2001@gmail.com
-Keywords: get best data combination,read text files,text files,lock data combination,save data,English,Pronouns,Punctuations,English pronouns,Model training,optimise accuracy,lock data combination,gives best result,best data for ML models,works on text data also,short word treatment,Image Scraping,download images,Web Image Scraping,timeseries,splitting timeseries data into train and test,deal with emojis and emoticons,emoji,emojis,emoticon,emoticons,word tokenize,NLP,short words,short words treatment,get best accuracy,performence enhancing,best data,more accurate model building,word to token,tokenizer
+Keywords: transfer or copy files from one directory to other,get best data combination,read text files,text files,lock data combination,save data,English,Pronouns,Punctuations,English pronouns,Model training,optimise accuracy,lock data combination,gives best result,best data for ML models,works on text data also,short word treatment,Image Scraping,download images,Web Image Scraping,timeseries,splitting timeseries data into train and test,deal with emojis and emoticons,emoji,emojis,emoticon,emoticons,word tokenize,NLP,short words,short words treatment,get best accuracy,performence enhancing,best data,more accurate model building,word to token,tokenizer
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.1
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
@@ -24,8 +24,8 @@
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: iOS
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-A package to increase the accuracy of ML models, gives you the best data for model training, works on text data also, short word treatment for NLP problems, can be used for Image Scraping also, use it to split the timeseries data into training and testing, deal with emojis and emoticons,word tokenizer,tokenize words,can be use to remove stop words too,Punctuations and get English Pronouns list too, use to read text files
+A package to increase the accuracy of ML models, transfer or copy files from one directory to other,  gives you the best data for model training, works on text data also, short word treatment for NLP problems, can be used for Image Scraping also, use it to split the timeseries data into training and testing, deal with emojis and emoticons,word tokenizer,tokenize words,can be use to remove stop words too,Punctuations and get English Pronouns list too, use to read text files
```

### Comparing `optimal_data_selector-1.2.0/optimal_data_selector/image.py` & `optimal_data_selector-1.2.2/optimal_data_selector/image.py`

 * *Files identical despite different names*

### Comparing `optimal_data_selector-1.2.0/optimal_data_selector/optimal.py` & `optimal_data_selector-1.2.2/optimal_data_selector/optimal.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,57 @@
-def OptimalDataSelector(predictor=None,target=None,combination=10,random_state=0,train_size=0.7,bs_problem='class',time_forecast=True,scaling=None,acc_forecast=True,boost=None,randomness=True,load_path=None,active_checkpoint=False):
+def OptimalDataSelector3(predictor=None,target=None,combination=10,random_state=0,train_size=0.7,bs_problem='class',time_forecast=True,scaling=None,acc_forecast=True,boost=None,randomness=True,load_path=None,active_checkpoint=False):
     '''Find the best data combination for models by maximizing accuracy on different sizes of data.
 
     Parameters:
-        predictor     : array-like
+       * predictor     : array-like
             The independent variables used for prediction.
 
-        target        : array-like
+       * target        : array-like
             The target variable to be predicted.
 
-        combination   : int, optional
+       * combination   : int, optional
             The number of combinations of data to consider. Default is 10.
 
-        random_state  : int, optional
+       * random_state  : int, optional
             The seed value for random number generation. Default is 0.
 
-        train_size    : float, optional
+       * train_size    : float, optional
             The proportion of data used for training. Default is 0.7.
 
-        bs_problem    : str, optional --> ['reg','class']
+       * bs_problem    : str, optional --> ['reg','class']
             The type of problem to solve. Options are 'class' for classification problems and 'reg' for regression problems.
             Default is 'class'.
 
-        time_forecast : bool, optional --> [True,False]
+       * time_forecast : bool, optional --> [True,False]
             Flag indicating whether to print the computation time. Default is True.
 
-        scaling       : str, optional --> ['normal','st_normal']
+       * scaling       : str, optional --> ['normal','st_normal']
             it takes the data and scale the value based on the option you have choosed, options are ['normal','st_normal'].Default is None
-
-        boost         : str, optional --> [None,'prim','max']
+       
+       * acc_forecast  : bool, optional --> [True,False]
+            Flag indicating whether to print the probable accuracy or not. Default is True.
+       
+       * boost         : str, optional --> [None,'prim','max']
             Flag indicating whether to use boosting performance or reduce the time complexcity [None,'prim','max'].
              When None, the function will try to find fully stabel data combination this case the function gives
              Completely zero weightage to  time saving , When 'prim', the function will look towards balanced data as well as
              less time this case function will give 50:50 weightage to both , When 'max', In this case time saving
              will be the first priority . Default is None.
 
-        randomness    : bool, True --> [True,False]
+       * randomness    : bool, True --> [True,False]
             it takes the mixture to the data combo from data, turn it into False to have sequential data,
             Default value is True
 
-        load_path     : str,  optional
+       * load_path     : str,  optional
             This parameter recalls a previously saved combination of data and splits it in the same way as before.
             By using this parameter, you can lock in a specific combination and reuse it endlessly.
             [Simply pass the file path with its extension,
             and the function will recall the same data structure that you saved]. The default value is None.
 
-        active_checkpoint        : bool, True --> [True,False]
+       * active_checkpoint        : bool, True --> [True,False]
             Set it to False, and the function will run without asking to save the data structure.
             When set to True, the function will ask you to save the data structure and it will mark every single
             combination. The default value is False.
 
     Returns:
         x_train : array-like
             The training data for the independent variables.
@@ -104,14 +107,17 @@
     from sklearn.svm import SVC
     from sklearn.tree import DecisionTreeClassifier,DecisionTreeRegressor
     from sklearn.naive_bayes import GaussianNB,MultinomialNB
     import scipy
     import time
     import warnings
     warnings.filterwarnings('ignore')
+    import os
+    
+    ext='.csv'
     dd=0
     save=0
     tr_s=0
     dd1=0
     train_len=0
     XXX=0
     YYY=0
@@ -163,27 +169,35 @@
               if acc_forecast == True:
                   print('Accuracy can be ~ '+str(max(acc)))
               if time_forecast == True:
                   print('Computation time = '+str((end0-start0)/60),' mints')
               if active_checkpoint == True:
                 main_per = input("Do you wanna save this combination ?[yes/no] : ")
                 if main_per == 'yes':
-                  print('Dont forget to write extension[.csv]')
-                  com_name = input("Enter file name : ")
-                  #x_train2=pd.DataFrame(x_train1)
-                  #x_test2=pd.DataFrame(x_test1)
-                  #y_train2=pd.DataFrame(y_train1)
-                  #y_test2=pd.DataFrame(y_test1)
-                  t_data=pd.concat([x_train1,x_test1],axis=0)
-                  t_data.index = range(0,len(t_data))
-                  tss_data=pd.concat([y_train1,y_test1],axis=0)
-                  tss_data.index=t_data.index
-                  saved_data=pd.concat([t_data,tss_data],axis=1)
+                  print('Give a name of the file ')
+                  while True:
+                      com_name1 = input("Enter file name [Without extension] : ")
+                      com_name = com_name1+ext
+                      if os.path.exists(com_name):
+                            print("The name you entered for this file already exists. Please enter a different name.")
+                            print()
+                      else:
+                            #x_train2=pd.DataFrame(x_train1)
+                            #x_test2=pd.DataFrame(x_test1)
+                            #y_train2=pd.DataFrame(y_train1)
+                            #y_test2=pd.DataFrame(y_test1)
+                            t_data=pd.concat([x_train1,x_test1],axis=0)
+                            t_data.index = range(0,len(t_data))
+                            tss_data=pd.concat([y_train1,y_test1],axis=0)
+                            tss_data.index=t_data.index
+                            saved_data=pd.concat([t_data,tss_data],axis=1)
+                            saved_data.to_csv(com_name)
 
-                  print("File ",com_name," has been saved to your 'PWD'")
+                            print("File ",com_name," has been saved to your 'PWD'")
+                            break
 
               return x_train1,x_test1,y_train1,y_test1
 
           elif bs_problem =='reg':
                 start01 = time.time()
                 for i in range(random_state,random_state+combination):
                     x_train1,x_test1,y_train1,y_test1=train_test_split(X,Y,train_size=train_size,random_state=i,shuffle=randomness)
@@ -201,27 +215,35 @@
                 if acc_forecast == True:
                     print('Accuracy can be ~ '+str(max(acc)))
                 if time_forecast == True:
                     print('Computation time = '+str((end01-start01)/60),' mints')
                 if active_checkpoint == True:
                   main_per = input("Do you wanna save this combination ?[yes/no] : ")
                   if main_per == 'yes':
-                    print('Dont forget to write extension[.csv]')
-                    com_name = input("Enter file name : ")
-                    #x_train2=pd.DataFrame(x_train1)
-                    #x_test2=pd.DataFrame(x_test1)
-                    #y_train2=pd.DataFrame(y_train1)
-                    #y_test2=pd.DataFrame(y_test1)
-                    t_data=pd.concat([x_train1,x_test1],axis=0)
-                    t_data.index = range(0,len(t_data))
-                    tss_data=pd.concat([y_train1,y_test1],axis=0)
-                    tss_data.index=t_data.index
-                    saved_data=pd.concat([t_data,tss_data],axis=1)
+                    print('Give a name of the file')
+                    while True:
+                        com_name1 = input("Enter file name [Without extension] : ")
+                        com_name= com_name1+ext
+                        if os.path.exists(com_name):
+                            print("The name you entered for this file already exists. Please enter a different name.")
+                            print()
+                        else:
+                            #x_train2=pd.DataFrame(x_train1)
+                            #x_test2=pd.DataFrame(x_test1)
+                            #y_train2=pd.DataFrame(y_train1)
+                            #y_test2=pd.DataFrame(y_test1)
+                            t_data=pd.concat([x_train1,x_test1],axis=0)
+                            t_data.index = range(0,len(t_data))
+                            tss_data=pd.concat([y_train1,y_test1],axis=0)
+                            tss_data.index=t_data.index
+                            saved_data=pd.concat([t_data,tss_data],axis=1)
+                            saved_data.to_csv(com_name)
 
-                    print("File ",com_name," has been saved to your 'PWD'")
+                            print("File ",com_name," has been saved to your 'PWD'")
+                            break
 
                 return x_train1,x_test1,y_train1,y_test1
 
       elif bs_problem == 'class' and boost == None and type(predictor) != scipy.sparse._csr.csr_matrix:
           start = time.time()
           for i in range(random_state,random_state+combination):
               x_train1,x_test1,y_train1,y_test1=train_test_split(X,Y,train_size=train_size,random_state=i,shuffle=randomness)
@@ -249,28 +271,35 @@
           if acc_forecast == True:
               print('Accuracy can be ~ '+str(max(i4)))
           if time_forecast == True:
               print('Computation time = '+str((end-start)/60),' mints')
           if active_checkpoint == True:
             main_per = input("Do you wanna save this combination ?[yes/no] : ")
             if main_per == 'yes':
-              print('Dont forget to write extension[.csv]')
-              com_name = input("Enter file name : ")
-              #x_train2=pd.DataFrame(x_train1)
-              #x_test2=pd.DataFrame(x_test1)
-              #y_train2=pd.DataFrame(y_train1)
-              #y_test2=pd.DataFrame(y_test1)
-              t_data=pd.concat([x_train1,x_test1],axis=0)
-              t_data.index = range(0,len(t_data))
-              tss_data=pd.concat([y_train1,y_test1],axis=0)
-              tss_data.index=t_data.index
-              saved_data=pd.concat([t_data,tss_data],axis=1)
-
-              saved_data.to_csv(com_name)
-              print("File ",com_name," has been saved to your 'PWD'")
+              print('Give a name of the file')
+              while True:
+                  com_name1 = input("Enter file name [Without extension] : ")
+                  com_name= com_name1+ext
+                  if os.path.exists(com_name):
+                        print("The name you entered for this file already exists. Please enter a different name.")
+                        print()
+                  else:
+                        #x_train2=pd.DataFrame(x_train1)
+                        #x_test2=pd.DataFrame(x_test1)
+                        #y_train2=pd.DataFrame(y_train1)
+                        #y_test2=pd.DataFrame(y_test1)
+                        t_data=pd.concat([x_train1,x_test1],axis=0)
+                        t_data.index = range(0,len(t_data))
+                        tss_data=pd.concat([y_train1,y_test1],axis=0)
+                        tss_data.index=t_data.index
+                        saved_data=pd.concat([t_data,tss_data],axis=1)
+
+                        saved_data.to_csv(com_name)
+                        print("File ",com_name," has been saved to your 'PWD'")
+                        break 
 
           return x_train1,x_test1,y_train1,y_test1
       elif bs_problem == 'class' and boost == None and type(predictor) == scipy.sparse._csr.csr_matrix:
 
           start22 = time.time()
           for i in range(random_state,random_state+combination):
               x_train1,x_test1,y_train1,y_test1=train_test_split(X,Y,train_size=train_size,random_state=i,shuffle=randomness)
@@ -298,27 +327,34 @@
           if acc_forecast == True:
               print('Accuracy can be ~ '+str(max(i4)))
           if time_forecast == True:
               print('Computation time = '+str((end22-start22)/60),' mints')
           if active_checkpoint == True:
             main_per = input("Do you wanna save this combination ?[yes/no] : ")
             if main_per == 'yes':
-              print('Dont forget to write extension[.csv]')
-              com_name = input("Enter file name : ")
-              #x_train2=pd.DataFrame(x_train1)
-              #x_test2=pd.DataFrame(x_test1)
-              #y_train2=pd.DataFrame(y_train1)
-              #y_test2=pd.DataFrame(y_test1)
-              t_data=pd.concat([x_train1,x_test1],axis=0)
-              t_data.index = range(0,len(t_data))
-              tss_data=pd.concat([y_train1,y_test1],axis=0)
-              tss_data.index=t_data.index
-              saved_data=pd.concat([t_data,tss_data],axis=1)
-
-              print("File ",com_name," has been saved to your 'PWD'")
+              print('Give a name of the file ')
+              while True:
+                  com_name1 = input("Enter file name [Without extension] : ")
+                  com_name = com_name1+ext
+                  if os.path.exists(com_name):
+                        print("The name you entered for this file already exists. Please enter a different name.")
+                        print()
+                  else:
+                        #x_train2=pd.DataFrame(x_train1)
+                        #x_test2=pd.DataFrame(x_test1)
+                        #y_train2=pd.DataFrame(y_train1)
+                        #y_test2=pd.DataFrame(y_test1)
+                        t_data=pd.concat([x_train1,x_test1],axis=0)
+                        t_data.index = range(0,len(t_data))
+                        tss_data=pd.concat([y_train1,y_test1],axis=0)
+                        tss_data.index=t_data.index
+                        saved_data=pd.concat([t_data,tss_data],axis=1)
+                        saved_data.to_csv(com_name)
+                        print("File ",com_name," has been saved to your 'PWD'")
+                        break
 
           return x_train1,x_test1,y_train1,y_test1
 
       elif bs_problem == 'reg' and boost == None and type(predictor) != scipy.sparse._csr.csr_matrix :
           start1=time.time()
           for i in range(random_state,random_state+combination):
               x_train1,x_test1,y_train1,y_test1=train_test_split(X,Y,train_size=train_size,random_state=i,shuffle=randomness)
@@ -345,27 +381,34 @@
           if acc_forecast == True:
               print('Accuracy can be ~ '+str(max(i4)))
           if time_forecast == True:
               print('Computation time = '+str((end1-start1)/60),' mints')
           if active_checkpoint == True:
             main_per = input("Do you wanna save this combination ?[yes/no] : ")
             if main_per == 'yes':
-              print('Dont forget to write extension[.csv]')
-              com_name = input("Enter file name : ")
-              #x_train2=pd.DataFrame(x_train1)
-              #x_test2=pd.DataFrame(x_test1)
-              #y_train2=pd.DataFrame(y_train1)
-              #y_test2=pd.DataFrame(y_test1)
-              t_data=pd.concat([x_train1,x_test1],axis=0)
-              t_data.index = range(0,len(t_data))
-              tss_data=pd.concat([y_train1,y_test1],axis=0)
-              tss_data.index=t_data.index
-              saved_data=pd.concat([t_data,tss_data],axis=1)
-
-              print("File ",com_name," has been saved to your 'PWD'")
+              print('Give a name of the file')
+              while True:
+                  com_name1 = input("Enter file name [Without extension] : ")
+                  com_name = com_name1+ext
+                  if os.path.exists(com_name):
+                        print("The name you entered for this file already exists. Please enter a different name.")
+                        print()
+                  else:
+                        #x_train2=pd.DataFrame(x_train1)
+                        #x_test2=pd.DataFrame(x_test1)
+                        #y_train2=pd.DataFrame(y_train1)
+                        #y_test2=pd.DataFrame(y_test1)
+                        t_data=pd.concat([x_train1,x_test1],axis=0)
+                        t_data.index = range(0,len(t_data))
+                        tss_data=pd.concat([y_train1,y_test1],axis=0)
+                        tss_data.index=t_data.index
+                        saved_data=pd.concat([t_data,tss_data],axis=1)
+                        saved_data.to_csv(com_name)
+                        print("File ",com_name," has been saved to your 'PWD'")
+                        break
 
           return x_train1,x_test1,y_train1,y_test1
 
       elif bs_problem == 'class' and boost == 'prim' and type(predictor) == scipy.sparse._csr.csr_matrix:
           start9 = time.time()
           for i in range(random_state,random_state+combination):
               x_train1,x_test1,y_train1,y_test1=train_test_split(X,Y,train_size=train_size,random_state=i,shuffle=randomness)
@@ -391,27 +434,34 @@
           if acc_forecast == True:
               print('Accuracy can be ~ '+str(max(i4)))
           if time_forecast == True:
               print('Computation time = '+str((end9-start9)/60),' mints')
           if active_checkpoint == True:
             main_per = input("Do you wanna save this combination ?[yes/no] : ")
             if main_per == 'yes':
-              print('Dont forget to write extension[.csv]')
-              com_name = input("Enter file name : ")
-              #x_train2=pd.DataFrame(x_train1)
-              #x_test2=pd.DataFrame(x_test1)
-              #y_train2=pd.DataFrame(y_train1)
-              #y_test2=pd.DataFrame(y_test1)
-              t_data=pd.concat([x_train1,x_test1],axis=0)
-              t_data.index = range(0,len(t_data))
-              tss_data=pd.concat([y_train1,y_test1],axis=0)
-              tss_data.index=t_data.index
-              saved_data=pd.concat([t_data,tss_data],axis=1)
-
-              print("File ",com_name," has been saved to your 'PWD'")
+              print('Give a name of the file')
+              while True:
+                  com_name1 = input("Enter file name [Without extension] : ")
+                  com_name = com_name1+ext
+                  if os.path.exists(com_name):
+                        print("The name you entered for this file already exists. Please enter a different name.")
+                        print()
+                  else:      
+                        #x_train2=pd.DataFrame(x_train1)
+                        #x_test2=pd.DataFrame(x_test1)
+                        #y_train2=pd.DataFrame(y_train1)
+                        #y_test2=pd.DataFrame(y_test1)
+                        t_data=pd.concat([x_train1,x_test1],axis=0)
+                        t_data.index = range(0,len(t_data))
+                        tss_data=pd.concat([y_train1,y_test1],axis=0)
+                        tss_data.index=t_data.index
+                        saved_data=pd.concat([t_data,tss_data],axis=1)
+                        saved_data.to_csv(com_name)
+                        print("File ",com_name," has been saved to your 'PWD'")
+                        break
 
           return x_train1,x_test1,y_train1,y_test1
 
       elif bs_problem == 'class' and boost == 'prim' and type(predictor) != scipy.sparse._csr.csr_matrix:
           start10 = time.time()
           for i in range(random_state,random_state+combination):
               x_train1,x_test1,y_train1,y_test1=train_test_split(X,Y,train_size=train_size,random_state=i,shuffle=randomness)
@@ -437,27 +487,34 @@
           if acc_forecast == True:
               print('Accuracy can be ~ '+str(max(i4)))
           if time_forecast == True:
               print('Computation time = '+str((end10-start10)/60),' mints')
           if active_checkpoint == True:
             main_per = input("Do you wanna save this combination ?[yes/no] : ")
             if main_per == 'yes':
-              print('Dont forget to write extension[.csv]')
-              com_name = input("Enter file name : ")
-              #x_train2=pd.DataFrame(x_train1)
-              #x_test2=pd.DataFrame(x_test1)
-              #y_train2=pd.DataFrame(y_train1)
-              #y_test2=pd.DataFrame(y_test1)
-              t_data=pd.concat([x_train1,x_test1],axis=0)
-              t_data.index = range(0,len(t_data))
-              tss_data=pd.concat([y_train1,y_test1],axis=0)
-              tss_data.index=t_data.index
-              saved_data=pd.concat([t_data,tss_data],axis=1)
-
-              print("File ",com_name," has been saved to your 'PWD'")
+              print('Give a name of the file')
+              while True:
+                  com_name1 = input("Enter file name [Without extension] : ")
+                  com_name = com_name1+ext
+                  if os.path.exists(com_name):
+                        print("The name you entered for this file already exists. Please enter a different name.")
+                        print()
+                  else:
+                        #x_train2=pd.DataFrame(x_train1)
+                        #x_test2=pd.DataFrame(x_test1)
+                        #y_train2=pd.DataFrame(y_train1)
+                        #y_test2=pd.DataFrame(y_test1)
+                        t_data=pd.concat([x_train1,x_test1],axis=0)
+                        t_data.index = range(0,len(t_data))
+                        tss_data=pd.concat([y_train1,y_test1],axis=0)
+                        tss_data.index=t_data.index
+                        saved_data=pd.concat([t_data,tss_data],axis=1)
+                        saved_data.to_csv(com_name)
+                        print("File ",com_name," has been saved to your 'PWD'")
+                        break
 
           return x_train1,x_test1,y_train1,y_test1
 
       elif bs_problem == 'reg' and boost == 'prim' and type(predictor) != scipy.sparse._csr.csr_matrix:
           start10 = time.time()
           for i in range(random_state,random_state+combination):
               x_train1,x_test1,y_train1,y_test1=train_test_split(X,Y,train_size=train_size,random_state=i,shuffle=randomness)
@@ -483,27 +540,34 @@
           if acc_forecast == True:
               print('Accuracy can be ~ '+str(max(i4)))
           if time_forecast == True:
               print('Computation time = '+str((end10-start10)/60),' mints')
           if active_checkpoint == True:
             main_per = input("Do you wanna save this combination ?[yes/no] : ")
             if main_per == 'yes':
-              print('Dont forget to write extension[.csv]')
-              com_name = input("Enter file name : ")
-              #x_train2=pd.DataFrame(x_train1)
-              #x_test2=pd.DataFrame(x_test1)
-              #y_train2=pd.DataFrame(y_train1)
-              #y_test2=pd.DataFrame(y_test1)
-              t_data=pd.concat([x_train1,x_test1],axis=0)
-              t_data.index = range(0,len(t_data))
-              tss_data=pd.concat([y_train1,y_test1],axis=0)
-              tss_data.index=t_data.index
-              saved_data=pd.concat([t_data,tss_data],axis=1)
-
-              print("File ",com_name," has been saved to your 'PWD'")
+              print('Give a name of the file')
+              while True:
+                  com_name1= input("Enter file name [Without extension] : ")
+                  com_name = com_name1+ext
+                  if os.path.exists(com_name):
+                        print("The name you entered for this file already exists. Please enter a different name.")
+                        print()
+                  else:
+                        #x_train2=pd.DataFrame(x_train1)
+                        #x_test2=pd.DataFrame(x_test1)
+                        #y_train2=pd.DataFrame(y_train1)
+                        #y_test2=pd.DataFrame(y_test1)
+                        t_data=pd.concat([x_train1,x_test1],axis=0)
+                        t_data.index = range(0,len(t_data))
+                        tss_data=pd.concat([y_train1,y_test1],axis=0)
+                        tss_data.index=t_data.index
+                        saved_data=pd.concat([t_data,tss_data],axis=1)
+                        saved_data.to_csv(com_name)
+                        print("File ",com_name," has been saved to your 'PWD'")
+                        break
           return x_train1,x_test1,y_train1,y_test1
 
     elif load_path != None:
       try:
         dd=pd.read_csv(load_path)
       except:
         raise FileNotFoundError("This file not found")
```

### Comparing `optimal_data_selector-1.2.0/optimal_data_selector/sequential.py` & `optimal_data_selector-1.2.2/optimal_data_selector/sequential.py`

 * *Files identical despite different names*

### Comparing `optimal_data_selector-1.2.0/optimal_data_selector/text.py` & `optimal_data_selector-1.2.2/optimal_data_selector/text.py`

 * *Files identical despite different names*

### Comparing `optimal_data_selector-1.2.0/optimal_data_selector/word.py` & `optimal_data_selector-1.2.2/optimal_data_selector/word.py`

 * *Files identical despite different names*

### Comparing `optimal_data_selector-1.2.0/optimal_data_selector.egg-info/PKG-INFO` & `optimal_data_selector-1.2.2/optimal_data_selector.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
-Name: optimal-data-selector
-Version: 1.2.0
-Summary: ('A Package for to optimize models, use for nlp short word treatment, choosing optimal data for ML models, use for Image Scraping , use in timeseries problem to split the data into train and test', 'Deal with emojis and emoticons in nlp,word tokenize,token, get the list of Punctuation marks and English Pronouns too, can be used to read text files')
+Name: optimal_data_selector
+Version: 1.2.2
+Summary: ('A Package for optimize models, transfer or copy files from one directory to other, use for nlp short word treatment, choosing optimal data for ML models, use for Image Scraping , use in timeseries problem to split the data into train and test', 'Deal with emojis and emoticons in nlp,word tokenize,token, get the list of Punctuation marks and English Pronouns too, can be used to read text files')
 Author: Rohan Majumder
 Author-email: majumderrohan2001@gmail.com
-Keywords: get best data combination,read text files,text files,lock data combination,save data,English,Pronouns,Punctuations,English pronouns,Model training,optimise accuracy,lock data combination,gives best result,best data for ML models,works on text data also,short word treatment,Image Scraping,download images,Web Image Scraping,timeseries,splitting timeseries data into train and test,deal with emojis and emoticons,emoji,emojis,emoticon,emoticons,word tokenize,NLP,short words,short words treatment,get best accuracy,performence enhancing,best data,more accurate model building,word to token,tokenizer
+Keywords: transfer or copy files from one directory to other,get best data combination,read text files,text files,lock data combination,save data,English,Pronouns,Punctuations,English pronouns,Model training,optimise accuracy,lock data combination,gives best result,best data for ML models,works on text data also,short word treatment,Image Scraping,download images,Web Image Scraping,timeseries,splitting timeseries data into train and test,deal with emojis and emoticons,emoji,emojis,emoticon,emoticons,word tokenize,NLP,short words,short words treatment,get best accuracy,performence enhancing,best data,more accurate model building,word to token,tokenizer
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.1
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
@@ -24,8 +24,8 @@
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: iOS
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-A package to increase the accuracy of ML models, gives you the best data for model training, works on text data also, short word treatment for NLP problems, can be used for Image Scraping also, use it to split the timeseries data into training and testing, deal with emojis and emoticons,word tokenizer,tokenize words,can be use to remove stop words too,Punctuations and get English Pronouns list too, use to read text files
+A package to increase the accuracy of ML models, transfer or copy files from one directory to other,  gives you the best data for model training, works on text data also, short word treatment for NLP problems, can be used for Image Scraping also, use it to split the timeseries data into training and testing, deal with emojis and emoticons,word tokenizer,tokenize words,can be use to remove stop words too,Punctuations and get English Pronouns list too, use to read text files
```

### Comparing `optimal_data_selector-1.2.0/setup.py` & `optimal_data_selector-1.2.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '1.2.0'
-DESCRIPTION = 'A Package for to optimize models, use for nlp short word treatment, choosing optimal data for ML models, use for Image Scraping , use in timeseries problem to split the data into train and test','Deal with emojis and emoticons in nlp,word tokenize,token, get the list of Punctuation marks and English Pronouns too, can be used to read text files'
-LONG_DESCRIPTION = 'A package to increase the accuracy of ML models, gives you the best data for model training, works on text data also, short word treatment for NLP problems, can be used for Image Scraping also, use it to split the timeseries data into training and testing, deal with emojis and emoticons,word tokenizer,tokenize words,can be use to remove stop words too,Punctuations and get English Pronouns list too, use to read text files'
+VERSION = '1.2.2'
+DESCRIPTION = 'A Package for optimize models, transfer or copy files from one directory to other, use for nlp short word treatment, choosing optimal data for ML models, use for Image Scraping , use in timeseries problem to split the data into train and test','Deal with emojis and emoticons in nlp,word tokenize,token, get the list of Punctuation marks and English Pronouns too, can be used to read text files'
+LONG_DESCRIPTION = 'A package to increase the accuracy of ML models, transfer or copy files from one directory to other,  gives you the best data for model training, works on text data also, short word treatment for NLP problems, can be used for Image Scraping also, use it to split the timeseries data into training and testing, deal with emojis and emoticons,word tokenizer,tokenize words,can be use to remove stop words too,Punctuations and get English Pronouns list too, use to read text files'
 
 # Setting up
 setup(
     name="optimal_data_selector",
     version=VERSION,
     author="Rohan Majumder",
     author_email="majumderrohan2001@gmail.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=[],
-    keywords=['get best data combination','read text files','text files','lock data combination','save data','English','Pronouns','Punctuations','English pronouns','Model training', 'optimise accuracy', 'lock data combination', 'gives best result', 'best data for ML models', 'works on text data also','short word treatment','Image Scraping','download images','Web Image Scraping','timeseries','splitting timeseries data into train and test','deal with emojis and emoticons','emoji','emojis','emoticon','emoticons','word tokenize','NLP','short words','short words treatment','get best accuracy','performence enhancing','best data','more accurate model building','word to token','tokenizer'],
+    keywords=['transfer or copy files from one directory to other','get best data combination','read text files','text files','lock data combination','save data','English','Pronouns','Punctuations','English pronouns','Model training', 'optimise accuracy', 'lock data combination', 'gives best result', 'best data for ML models', 'works on text data also','short word treatment','Image Scraping','download images','Web Image Scraping','timeseries','splitting timeseries data into train and test','deal with emojis and emoticons','emoji','emojis','emoticon','emoticons','word tokenize','NLP','short words','short words treatment','get best accuracy','performence enhancing','best data','more accurate model building','word to token','tokenizer'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         'Programming Language :: Python :: 3.1',
         'Programming Language :: Python :: 3.2',
         'Programming Language :: Python :: 3.3',
```

