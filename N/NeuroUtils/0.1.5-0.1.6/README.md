# Comparing `tmp/NeuroUtils-0.1.5-py3-none-any.whl.zip` & `tmp/NeuroUtils-0.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 17257 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat    25630 b- defN 24-May-12 15:47 NeuroUtils/Architectures.py
--rw-rw-rw-  2.0 fat    23771 b- defN 24-May-12 16:36 NeuroUtils/Core.py
--rw-rw-rw-  2.0 fat    24791 b- defN 24-May-12 10:29 NeuroUtils/ML_assets.py
+Zip file size: 22486 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat    28003 b- defN 24-May-18 10:08 NeuroUtils/Architectures.py
+-rw-rw-rw-  2.0 fat    52929 b- defN 24-May-23 20:16 NeuroUtils/Core.py
+-rw-rw-rw-  2.0 fat    27786 b- defN 24-May-23 10:35 NeuroUtils/ML_assets.py
 -rw-rw-rw-  2.0 fat       50 b- defN 24-May-10 18:38 NeuroUtils/__init__.py
--rw-rw-rw-  2.0 fat      571 b- defN 24-May-12 16:43 NeuroUtils-0.1.5.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     2078 b- defN 24-May-12 16:43 NeuroUtils-0.1.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-12 16:43 NeuroUtils-0.1.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 24-May-12 16:43 NeuroUtils-0.1.5.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      723 b- defN 24-May-12 16:43 NeuroUtils-0.1.5.dist-info/RECORD
-9 files, 77717 bytes uncompressed, 16015 bytes compressed:  79.4%
+-rw-rw-rw-  2.0 fat      571 b- defN 24-May-23 21:08 NeuroUtils-0.1.6.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     2078 b- defN 24-May-23 21:08 NeuroUtils-0.1.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-23 21:08 NeuroUtils-0.1.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 24-May-23 21:08 NeuroUtils-0.1.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      723 b- defN 24-May-23 21:08 NeuroUtils-0.1.6.dist-info/RECORD
+9 files, 112243 bytes uncompressed, 21244 bytes compressed:  81.1%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: NeuroUtils/ML_assets.py
 Comment: 
 
 Filename: NeuroUtils/__init__.py
 Comment: 
 
-Filename: NeuroUtils-0.1.5.dist-info/LICENSE.txt
+Filename: NeuroUtils-0.1.6.dist-info/LICENSE.txt
 Comment: 
 
-Filename: NeuroUtils-0.1.5.dist-info/METADATA
+Filename: NeuroUtils-0.1.6.dist-info/METADATA
 Comment: 
 
-Filename: NeuroUtils-0.1.5.dist-info/WHEEL
+Filename: NeuroUtils-0.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: NeuroUtils-0.1.5.dist-info/top_level.txt
+Filename: NeuroUtils-0.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: NeuroUtils-0.1.5.dist-info/RECORD
+Filename: NeuroUtils-0.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## NeuroUtils/Architectures.py

```diff
@@ -659,8 +659,72 @@
         x = Dense_batch_swish(x, channels = 64, dropout = 0.3)
     
     
     
         outputs = tf.keras.layers.Dense(n_classes, activation='softmax')(x)
     
         model = tf.keras.Model(inputs=[inputs], outputs=[outputs])
-        return model    
+        return model    
+    
+    
+    
+    
+    
+class Gan():
+    
+    @staticmethod
+    def Test_generator_28(latent_dim):
+        inputs = tf.keras.layers.Input((latent_dim))
+        # foundation for 7x7 image
+        n_nodes = 128 * 7 * 7
+        x = tf.keras.layers.Dense(n_nodes)(inputs)
+        x = tf.keras.layers.LeakyReLU(alpha=0.2)(x)
+        x = tf.keras.layers.Reshape((7, 7, 128))(x)
+        # upsample to 14x14
+        x = tf.keras.layers.Conv2DTranspose(256, (4,4), strides=(2,2), padding='same')(x)
+        x = tf.keras.layers.LeakyReLU(alpha=0.2)(x)
+        
+        x = tf.keras.layers.Conv2D(256, (4,4), strides=(1,1), padding='same')(x)
+        x = tf.keras.layers.LeakyReLU(alpha=0.2)(x)
+        # upsample to 28x28
+        x = tf.keras.layers.Conv2DTranspose(256, (4,4), strides=(2,2), padding='same')(x)
+        x = tf.keras.layers.LeakyReLU(alpha=0.2)(x)
+        
+        x = tf.keras.layers.Conv2D(128, (4,4), strides=(1,1), padding='same')(x)
+        x = tf.keras.layers.LeakyReLU(alpha=0.2)(x)
+        
+        outputs = tf.keras.layers.Conv2D(1, (7,7), activation='tanh', padding='same')(x)
+
+        model = tf.keras.Model(inputs=[inputs], outputs=[outputs])
+        
+        return model
+    
+    
+    def Test_discriminator_28(in_shape=(28,28,1)):
+        inputs = tf.keras.layers.Input(in_shape)
+        
+        x = tf.keras.layers.Conv2D(128, (3,3), strides=(2, 2), padding='same')(inputs)
+        x = tf.keras.layers.LeakyReLU(alpha=0.2)(x)
+        x = tf.keras.layers.Dropout(0.4)(x)
+        
+        x = tf.keras.layers.Conv2D(128, (3,3), strides=(1, 1), padding='same')(x)
+        x = tf.keras.layers.LeakyReLU(alpha=0.2)(x)
+        x = tf.keras.layers.Dropout(0.4)(x)
+        
+        x = tf.keras.layers.Conv2D(256, (3,3), strides=(2, 2), padding='same')(x)
+        x = tf.keras.layers.LeakyReLU(alpha=0.2)(x)
+        x = tf.keras.layers.Dropout(0.4)(x)
+        
+        x = tf.keras.layers.Conv2D(256, (3,3), strides=(1, 1), padding='same')(x)
+        x = tf.keras.layers.LeakyReLU(alpha=0.2)(x)
+        x = tf.keras.layers.Dropout(0.4)(x)
+        
+        x = tf.keras.layers.GlobalAveragePooling2D()(x)
+        
+        outputs = tf.keras.layers.Dense(1, activation='sigmoid')(x)
+        
+        model = tf.keras.Model(inputs=[inputs], outputs=[outputs])
+        
+        return model
+
+
+
```

## NeuroUtils/Core.py

```diff
@@ -8,21 +8,38 @@
 
 import tensorflow as tf
 import matplotlib.pyplot as plt
 import numpy as np
 from timeit import default_timer as timer   
 import pandas as pd
 from sklearn.model_selection import train_test_split
-
-
+from tqdm import tqdm
+from contextlib import redirect_stdout
+from ipywidgets import interact, IntSlider
+from IPython.display import display
+from matplotlib.widgets import Slider
+import math
 
 class Utils:
     
     def Initialize_data(DataBase_directory, Data_directory, img_H, img_W, grayscale, Load_from_CSV):
-    
+        """
+        Initializes -> Loading data from main DataBase folder and load it by classes in 
+        data directory
+
+        Args:
+            DataBase_directory (str):   Main DataBase directory
+            Data_directory (str):       Local project resized/grayscaled DataBase directory
+            img_H / img_W (int):        Image height and width in local DataBase
+            grayscale (bool):           Grayscale or RGB 
+            Load_from_CSV (bool):       Load data from CSV file instead of jpg/png...
+
+        Returns:
+            Database in project folder
+        """    
         
         if not os.path.isdir(Data_directory):
             os.makedirs(Data_directory)
             print("Creating data storage directory...\n")
             
         if len(os.listdir(Data_directory)) == 0:
             print("There is no Dataset Initialized, initializing Dataset...")
@@ -32,20 +49,21 @@
                 ml.DataSets.Create_Img_Classification_DataSet(DataBase_directory, img_H, img_W, Save_directory=Data_directory , grayscale = grayscale)
         else:
             print("Found initialized Dataset")
             database_list = os.listdir(DataBase_directory)
             data_list = os.listdir(Data_directory)
             if Load_from_CSV:
                 data_list = [element.replace(".csv" , "") for element in data_list] 
-                database_list = ['sample_submission', 'x_test','x_train', 'y_test','y_train']
+                database_list = ['x_test','x_train', 'y_test','y_train']
                 
-            data_list_clean = [element.replace(".npy" , "") for element in data_list] 
+            data_list_clean = [element.replace(".npy" , "") for element in data_list]
+            
             
             
-            if database_list != data_list_clean:
+            if all(elem in data_list for elem in database_list):
                 print("Dataset is lacking some of the classes, initializing Dataset again")
                 if Load_from_CSV:
                     ml.DataSets.Create_Img_Classification_DataSet_CSV(DataBase_directory, img_H, img_W, Save_directory=Data_directory)
                 else:
                     ml.DataSets.Create_Img_Classification_DataSet(DataBase_directory, img_H, img_W, Save_directory=Data_directory , grayscale = grayscale)
             else:
                 print("Dataset is initialized correctly!")
@@ -93,18 +111,18 @@
         if Kaggle_set:
             x_train , x_val , y_train , y_val = train_test_split(x,y,test_size = 0.2 ,stratify = y, shuffle = True)
         else:
             x_train , x_val , y_train , y_val = train_test_split(x,y,test_size = 0.3 ,stratify = y, shuffle = True)
             x_val , x_test , y_val , y_test = train_test_split(x_val,y_val,test_size = 0.66 ,stratify = y_val, shuffle = True)
         
         print("Augmentation of images...")
-        if (not (flipRotate and randBright and gaussian and denoise and contour)) and dataset_multiplier >1:
+        if (not (flipRotate or randBright or gaussian or denoise or contour)) and dataset_multiplier >1:
             print("\nNo augmentation specified, dataset will be just multiplied",dataset_multiplier, "times")
             
-        if not (flipRotate and randBright and gaussian and denoise and contour) and dataset_multiplier <1:
+        if (not (flipRotate or randBright or gaussian or denoise or contour)) and dataset_multiplier <=1:
             print("\nNo augmentation, skipping...")
         x_train,y_train = ml.DataSets.Augment_classification_dataset(x_train, y_train, dataset_multiplier, flipRotate, randBright, gaussian, denoise, contour )            
             
         
         
         
         if not Kaggle_set:
@@ -160,29 +178,62 @@
         if show_architecture:
             model.summary()
         
         #########################################################################
         #########################################################################
         return model
     
+    def Initialize_Gan_model(generator_arch, discriminator_arch, latent_dim, show_architecture):    
+        g_arch = f"{generator_arch}"
+        d_arch = f"{discriminator_arch}"
+        generator_class = getattr(arch.Gan, g_arch, None)
+        discriminator_class = getattr(arch.Gan, d_arch, None)
+        
+        if (generator_class and discriminator_class) is not None:
+            gan_generator = generator_class(latent_dim)
+            gan_discriminator = discriminator_class()
+            print("Found generator named: ",g_arch,"\nFound discriminator named: ",d_arch)
+        else:
+            if generator_class is None:
+                print("Could not find generator class named: ",g_arch)
+                return
+            if discriminator_class is None:
+                print("Could not find discriminator class named: ",d_arch)
+                return
+                
+        gan_discriminator.compile(loss='binary_crossentropy', optimizer=tf.keras.optimizers.Adam(0.0002, 0.5), metrics=['accuracy'])
+
+        # make weights in the discriminator not trainable
+        gan_discriminator.trainable = False
+        # connect them
+        gan_model = tf.keras.Sequential()
+        # add generator
+        gan_model.add(gan_generator)
+        # add the discriminator
+        gan_model.add(gan_discriminator)
+        gan_model.compile(loss='binary_crossentropy', optimizer=tf.keras.optimizers.Adam(0.0002, 0.5))
+        
+        return gan_model, gan_generator, gan_discriminator
+            
+
         
     def Initialize_weights_and_training(x_train, y_train, model, model_directory, model_architecture, train, epochs, patience, batch_size,min_delta, x_val=None, y_val=None, device = "CPU:0"):    
         #!!! Model training
         #########################################################################
         #########################################################################
         #Check if directory of trained model is present, if not, create one 
         if not os.path.isdir(model_directory):
             os.makedirs(model_directory)
             print("Creating model directory storage directory...\n")
             
         model_name = str(model_architecture + "_bs"+str(batch_size)+".keras")
         model_weights_directory = os.path.join(model_directory , model_name)
         model_history_directory = os.path.join(model_directory , "Model_history.csv")
         
-        model , train , starting_epoch = ml.General.Load_model_check_training_progress(model, train, model_weights_directory, model_history_directory)
+        model , train , starting_epoch = ml.General.Load_model_check_training_progress(model, train, epochs, model_weights_directory, model_history_directory)
         
     
              
         if train:
             #Create callback function to save best performing model
             
             if starting_epoch == 0:
@@ -228,14 +279,16 @@
          
             
          
         #########################################################################
         #########################################################################
         return model
     
+    
+
        
     def Initialize_Results(model,model_directory, dictionary,evaluate, x_train = None ,y_train = None ,x_val = None , y_val = None , x_test = None , y_test = None):    
         #!!! Model results
         #########################################################################
         #########################################################################
         
         #Plot model training history
@@ -326,15 +379,16 @@
             #High level constants
             #Form
             self.FORM = "Grayscale" if self.GRAYSCALE else "RGB"
             #Channels
             self.CHANNELS = 3 if self.FORM == "RGB" else 1
             self.CHANNELS = self.CHANNELS+1 if self.CONTOUR else self.CHANNELS
     
-            self.PARAM_MARK = "__" + "_".join(["1" if x else "0" for x in [self.FLIPROTATE, self.RANDBRIGHT, self.GAUSSIAN, self.DENOISE, self.CONTOUR]])
+            cr = 0 if self.REDUCED_SET_SIZE is None else self.REDUCED_SET_SIZE
+            self.PARAM_MARK = "_m"+str(self.DATASET_MULTIPLIER)+"_cr"+str(cr)+"_"+ "_".join(["1" if x else "0" for x in [self.FLIPROTATE, self.RANDBRIGHT, self.GAUSSIAN, self.DENOISE, self.CONTOUR]])
     
                     
             self.DATA_DIRECTORY = os.path.join(self.PROJECT_DIRECTORY , "DataSet" , str(str(self.IMG_H)+"x"+str(self.IMG_W)+"_"+self.FORM))
             self.DATAPROCESSED_DIRECTORY = os.path.join(self.PROJECT_DIRECTORY , "DataSet_Processed" , str(str(self.IMG_H)+"x"+str(self.IMG_W)+"_"+self.FORM),self.PARAM_MARK)
             self.MODEL_DIRECTORY =  os.path.join(self.PROJECT_DIRECTORY , "Models_saved" , str(self.MODEL_ARCHITECTURE) , self.FORM , str(str(self.IMG_H)+"x"+str(self.IMG_W)) , str("bs"+str(self.BATCH_SIZE) + self.PARAM_MARK)  )
             
             
@@ -445,12 +499,503 @@
             
         def Generate_sample_submission(self, filepath = None):
             if filepath is None:
                 sample_submission = pd.read_csv(os.path.join(self.DATA_DIRECTORY , "sample_submission.csv")) 
 
             #img_id = sample_submission.columns[0]
             label = sample_submission.columns[1]
-
-            label_array = np.argmax(self.MODEL.predict(self.X_TEST), axis = 1)
+            try:
+                label_array = np.argmax(self.MODEL.predict(self.X_TEST), axis = 1)
+            except:
+                label_array = self.Y_TEST
             sample_submission[label] = label_array
             return sample_submission
     
+
+
+
+
+    
+    class Gan_Project:
+        def  __init__(self,config):
+            #Low level constants
+            self.PROJECT_DIRECTORY = os.path.dirname(os.path.abspath(sys.argv[0]))
+            #Initial
+            self.DATABASE_DIRECTORY = config.Initial_params["DataBase_directory"]
+            self.KAGGLE_SET = config.Initial_params["Kaggle_set"]
+            self.CSV_LOAD = config.Initial_params["Load_from_CSV"]
+            self.IMG_H = config.Initial_params["img_H"]
+            self.IMG_W = config.Initial_params["img_W"]
+            self.GRAYSCALE= config.Initial_params["grayscale"]
+            self.DATA_TYPE = config.Initial_params["DataType"]
+            
+            #Augment
+            self.REDUCED_SET_SIZE = config.Augment_params["reduced_set_size"]
+            self.DATASET_MULTIPLIER = config.Augment_params["dataset_multiplier"]
+            self.FLIPROTATE = config.Augment_params["flipRotate"]
+            self.RANDBRIGHT = config.Augment_params["randBright"]
+            self.GAUSSIAN = config.Augment_params["gaussian_noise"]
+            self.DENOISE = config.Augment_params["denoise"]
+            self.CONTOUR = config.Augment_params["contour"]
+            
+            #Model
+            self.GENERATOR_ARCHITECTURE = config.Model_parameters["generator_architecture"]
+            self.DISCRIMINATOR_ARCHITECTURE = config.Model_parameters["discriminator_architecture"]
+            self.SHOW_ARCHITECTURE = config.Model_parameters["show_architecture"]
+            self.DEVICE = config.Model_parameters["device"]
+            self.TRAIN = config.Model_parameters["train"]
+            self.EPOCHS = config.Model_parameters["epochs"]
+            #self.PATIENCE = config.Model_parameters["patience"]
+            self.LATENT_DIM = config.Model_parameters["latent_dim"]
+            self.BATCH_SIZE = config.Model_parameters["batch_size"]
+            self.SAMPLE_INTERVAL = config.Model_parameters["sample_interval"]
+            self.SAMPLE_NUMBER = config.Model_parameters["sample_number"]
+            #self.MIN_DELTA = config.Model_parameters["min_delta"]
+            self.EVALUATE = config.Model_parameters["evaluate"]
+            
+            #High level constants
+            #Form
+            self.FORM = "Grayscale" if self.GRAYSCALE else "RGB"
+            #Channels
+            self.CHANNELS = 3 if self.FORM == "RGB" else 1
+            self.CHANNELS = self.CHANNELS+1 if self.CONTOUR else self.CHANNELS
+            
+            cr = 0 if self.REDUCED_SET_SIZE is None else self.REDUCED_SET_SIZE
+            self.PARAM_MARK = "_m"+str(self.DATASET_MULTIPLIER)+"_cr"+str(cr)+"_"+ "_".join(["1" if x else "0" for x in [self.FLIPROTATE, self.RANDBRIGHT, self.GAUSSIAN, self.DENOISE, self.CONTOUR]])
+    
+                    
+            self.DATA_DIRECTORY = os.path.join(self.PROJECT_DIRECTORY , "DataSet" , str(str(self.IMG_H)+"x"+str(self.IMG_W)+"_"+self.FORM))
+            self.DATAPROCESSED_DIRECTORY = os.path.join(self.PROJECT_DIRECTORY , "DataSet_Processed" , str(str(self.IMG_H)+"x"+str(self.IMG_W)+"_"+self.FORM),self.PARAM_MARK)
+            
+            self.MODEL_ARCHITECTURE = ''.join([self.GENERATOR_ARCHITECTURE , "__" , self.DISCRIMINATOR_ARCHITECTURE])
+            self.MODEL_DIRECTORY =  os.path.join(self.PROJECT_DIRECTORY , "Models_saved" , self.MODEL_ARCHITECTURE , self.FORM , str(str(self.IMG_H)+"x"+str(self.IMG_W)) , str("bs"+str(self.BATCH_SIZE) + self.PARAM_MARK)  )
+            self.MODEL_NAME = str(self.MODEL_ARCHITECTURE + "_bs"+str(self.BATCH_SIZE)+".keras")
+            
+            self.MODEL_WEIGHTS_DIRECTORY = os.path.join(self.MODEL_DIRECTORY , self.MODEL_NAME)
+            self.MODEL_HISTORY_DIRECTORY = os.path.join(self.MODEL_DIRECTORY , "Model_history.csv")
+        ########################################################    
+            
+        def __str__(self):
+            return f"This is class representing the project, main parameters are:\n\nOriginalDatabase: {self.DATABASE_DIRECTORY}\nGenerator Used: {self.GENERATOR_ARCHITECTURE}\nDiscriminator Used: {self.DISCRIMINATOR_ARCHITECTURE}"
+            
+        ########################################################
+    
+        def Initialize_data(self): 
+            """Initializing dataset from main database folder with photos to project folder in numpy format. Photos are 
+            Resized and cropped without loosing much aspect ratio, r parameter decides above what proportions of edges 
+            image will be cropped to square instead of squeezed""" 
+            
+            Utils.Initialize_data(DataBase_directory = self.DATABASE_DIRECTORY, 
+                                  Data_directory = self.DATA_DIRECTORY, 
+                                  img_H = self.IMG_H, 
+                                  img_W = self.IMG_W, 
+                                  grayscale = self.GRAYSCALE, 
+                                  Load_from_CSV = self.CSV_LOAD
+                                  )
+            
+        ########################################################
+        
+        def Load_and_merge_data(self):
+            """Loading dataset to memory from data directory in project folder, sets can be reduced to equal size
+            to eliminate disproportions if they are not same size at the main database
+            In this module dictionary with names of classes is created as well, names are based on names of datsets
+            Datasets names are based on the folder names in main database folder"""
+            if not self.KAGGLE_SET:
+                self.X_TRAIN, self.Y_TRAIN, self.DICTIONARY = ml.DataSets.Load_And_Merge_DataSet(self.DATA_DIRECTORY , self.REDUCED_SET_SIZE )
+                self.N_CLASSES = len(self.DICTIONARY)
+                
+            else:
+                #To add searching for key words such as test, x, train etc. as for now just name csvs like train, test
+                self.X_TRAIN = np.load(os.path.join(self.DATA_DIRECTORY , "x_train.npy"))
+                self.Y_TRAIN = np.load(os.path.join(self.DATA_DIRECTORY , "y_train.npy"))
+                
+                self.X_TEST = np.load(os.path.join(self.DATA_DIRECTORY , "x_test.npy"))
+                try:
+                    self.Y_TEST = np.load(os.path.join(self.DATA_DIRECTORY , "y_test.npy"))
+                except:
+                    self.Y_TEST = np.load(os.path.join(self.DATA_DIRECTORY , "y_test.npy"),allow_pickle = True)
+                
+        ########################################################
+            
+        def Process_data(self):
+
+            if self.KAGGLE_SET:
+                self.X_TRAIN , self.Y_TRAIN, self.X_VAL , self.Y_VAL = Utils.Process_Data(x = self.X_TRAIN,
+                                                                                          y = self.Y_TRAIN,
+                                                                                          dataset_multiplier = self.DATASET_MULTIPLIER,
+                                                                                          DataProcessed_directory = self.DATAPROCESSED_DIRECTORY,
+                                                                                          Kaggle_set = self.KAGGLE_SET,
+                                                                                          flipRotate = self.FLIPROTATE,
+                                                                                          randBright = self.RANDBRIGHT,
+                                                                                          gaussian = self.GAUSSIAN,
+                                                                                          denoise = self.DENOISE,
+                                                                                          contour = self.CONTOUR
+                                                                                          )
+
+            else:
+                self.X_TRAIN , self.Y_TRAIN, self.X_VAL , self.Y_VAL , self.X_TEST , self.Y_TEST = Utils.Process_Data(x = self.X_TRAIN,
+                                                                                                                      y = self.Y_TRAIN,
+                                                                                                                      dataset_multiplier = self.DATASET_MULTIPLIER,
+                                                                                                                      DataProcessed_directory = self.DATAPROCESSED_DIRECTORY,
+                                                                                                                      Kaggle_set = self.KAGGLE_SET,
+                                                                                                                      flipRotate = self.FLIPROTATE,
+                                                                                                                      randBright = self.RANDBRIGHT,
+                                                                                                                      gaussian = self.GAUSSIAN,
+                                                                                                                      denoise = self.DENOISE,
+                                                                                                                      contour = self.CONTOUR
+                                                                                                                      )
+            
+            try:
+                self.X_TRAIN = np.array((self.X_TRAIN/255-0.5)*2 , dtype = self.DATA_TYPE)
+                self.Y_TRAIN = np.array(self.Y_TRAIN , dtype = self.DATA_TYPE)
+                
+                self.X_VAL = np.array((self.X_VAL/255-0.5)*2 , dtype = self.DATA_TYPE)
+                self.Y_VAL = np.array(self.Y_VAL , dtype = self.DATA_TYPE)
+                
+                self.X_TEST = np.array((self.X_TEST/255-0.5)*2 , dtype = self.DATA_TYPE)
+                self.Y_TEST = np.array(self.Y_TEST , dtype = self.DATA_TYPE)
+            except Exception as e:
+                print("Could not standarize data:",e)
+                
+            
+        ########################################################
+        
+            
+        def Initialize_model_from_library(self):
+            self.MODEL,self.GENERATOR,self.DISCRIMINATOR = Utils.Initialize_Gan_model(generator_arch = self.GENERATOR_ARCHITECTURE,
+                                                                                      discriminator_arch = self.DISCRIMINATOR_ARCHITECTURE,
+                                                                                      latent_dim = self.LATENT_DIM,
+                                                                                      show_architecture = self.SHOW_ARCHITECTURE
+                                                                                      )
+            
+            
+ 
+        def Callback(self,current_epoch, constant_noise):
+            #1    
+            #Saving npy images   
+            if current_epoch % self.SAMPLE_INTERVAL == 0:
+                if not os.path.isdir(os.path.join(self.MODEL_DIRECTORY , "Images")):
+                    os.makedirs(os.path.join(self.MODEL_DIRECTORY , "Images"))
+                    print("\nCreating model directory storage directory...")
+                    
+                print('\nSaving',self.SAMPLE_NUMBER,'samples from',current_epoch,'epoch')
+                filename = os.path.join(self.MODEL_DIRECTORY, 'Images', 'Epoch_%03d.npy' %current_epoch )
+                checkpoint_samples = self.GENERATOR.predict(constant_noise)
+                if len(checkpoint_samples.shape) == 4:
+                    checkpoint_samples = np.squeeze(checkpoint_samples, axis = -1)
+                # create 'fake' class labels (0)
+                if len(checkpoint_samples) < self.SAMPLE_NUMBER:
+                    for i in range(self.SAMPLE_NUMBER // len(checkpoint_samples) +1):
+                        value = math.log(i+1.6)
+                        temp = self.GENERATOR.predict(constant_noise*value)
+                        if len(temp.shape) == 4:
+                            temp = np.squeeze(temp, axis = -1)
+                        checkpoint_samples = np.vstack((checkpoint_samples , temp ))
+                        
+                checkpoint_samples = (checkpoint_samples[0:self.SAMPLE_NUMBER]+1)/2  
+                checkpoint_samples = np.array(checkpoint_samples*255 , dtype = np.uint8)
+                np.save(filename, checkpoint_samples)   
+                   
+            """
+            #2
+            #Saving model
+            if val_acc> max_vall_acc:
+                if val_acc-max_vall_acc>=delta:
+                    save_model
+                else:
+                    counter+=1
+            if counter==patience:
+                stop_training
+            """
+            #3
+            #Saving history
+            if self.csv_append:
+                model_history = pd.read_csv(self.MODEL_HISTORY_DIRECTORY)
+                
+                next_index = len(model_history)  
+                model_history.loc[next_index, 'epoch'] = current_epoch
+                
+                model_history.to_csv(self.MODEL_HISTORY_DIRECTORY, index = False)
+            else:
+                c = ["epoch"]
+                model_history = pd.DataFrame(columns = c)
+                
+                next_index = len(model_history)  
+                model_history.loc[next_index, 'epoch'] = int(current_epoch)
+                model_history.to_csv(self.MODEL_HISTORY_DIRECTORY, index = False)
+                
+                self.csv_append = True
+                
+            self.MODEL.save(self.MODEL_WEIGHTS_DIRECTORY)   
+                
+                
+            ########################################################
+    
+        def Initialize_weights_and_training_gan(self, precompiled_model=None, precompiled_generator = None, precompiled_discriminator = None):
+            #5
+            ########################################################
+            if precompiled_model and precompiled_generator and precompiled_discriminator:
+                # Use the provided precompiled model
+                self.MODEL = precompiled_model
+                self.GENERATOR = precompiled_generator
+                self.DISCRIMINATOR = precompiled_discriminator
+            else:
+                # Use the initialized model from Initialize_model function
+                assert hasattr(self, 'MODEL'), "Model not initialized. Call Initialize_model_from_library first or use custom compiled model, f.e, from keras or your own."
+            
+
+            #Check if directory of trained model is present, if not, create one 
+            if not os.path.isdir(self.MODEL_DIRECTORY):
+                os.makedirs(self.MODEL_DIRECTORY)
+                print("Creating model directory storage directory...\n")
+
+            
+            self.MODEL , train , starting_epoch = ml.General.Load_model_check_training_progress(model = self.MODEL,
+                                                                                                train = self.TRAIN,
+                                                                                                epochs_to_train = self.EPOCHS,
+                                                                                                model_weights_directory = self.MODEL_WEIGHTS_DIRECTORY,
+                                                                                                model_history_directory = self.MODEL_HISTORY_DIRECTORY
+                                                                                                )
+            try:
+                starting_epoch = int(starting_epoch)
+            except:
+                pass
+                #No starting epoch, or its NONE
+                 
+            if train:
+                #Create callback function to save best performing model
+                
+                if starting_epoch == 0:
+                    self.csv_append = False
+                else:
+                    self.csv_append = True
+                
+                self.CONSTANT_NOISE = np.random.normal(0, 1, (self.SAMPLE_NUMBER, self.LATENT_DIM))
+                
+                #Deleting images if training from scratch
+                if os.path.isdir(os.path.join(self.MODEL_DIRECTORY , "Images")) and not self.csv_append:
+                    print("Deleting remaining images from folder 'Images'... ")
+                    ml.General.delete_files_in_folder(os.path.join(self.MODEL_DIRECTORY , "Images"))
+                
+                timer_start = timer()
+                #To add stable noise over continued training, now its only during one session
+                with tf.device(self.DEVICE):
+                    for epoch in range(starting_epoch+1 , self.EPOCHS+1):
+                        print("\nEpoch:",epoch)
+                        steps_per_epoch = len(self.X_TRAIN) // self.BATCH_SIZE
+                        for step in tqdm(range(steps_per_epoch)):
+                            with redirect_stdout(open(os.devnull, 'w')):
+                                #1
+                                #Taking batch of real samples from dataset
+                                x_real, y_real = ml.General.generate_real_samples(self.X_TRAIN, self.BATCH_SIZE//2)
+                                
+                                #2
+                                #Generating batch of fake samples from generator
+                                x_fake , y_fake = ml.General.generate_fake_samples(self.GENERATOR, self.LATENT_DIM, self.BATCH_SIZE//2)
+                                
+                                #3
+                                #Preparing combined real-fake set for discriminator to train
+                                x = np.vstack((x_real,x_fake))
+                                y = np.vstack((y_real, y_fake))
+                                
+                                #4
+                                #Training discriminator
+                                discriminator_loss = self.DISCRIMINATOR.train_on_batch(x,y)
+                                
+                                #5
+                                #Update generator via discriminator error
+                                noise = np.random.normal(0, 1, (self.BATCH_SIZE, self.LATENT_DIM))
+                                ones = np.ones((self.BATCH_SIZE, 1))
+                                generator_loss = self.MODEL.train_on_batch(noise, ones)
+                                
+                                
+                        # Print the progress
+                        sys.stdout.write(f"\n[D loss: {discriminator_loss[0]:.3f} | D acc: {discriminator_loss[1]:.3f}] [G loss: {generator_loss:.3f}]")    
+                       
+                        # Save generated images every sample_interval
+                        #gan_callback()
+                        self.Callback(current_epoch = epoch,
+                                      constant_noise = self.CONSTANT_NOISE
+                                      )
+                            
+                        #To make in callbacks some kind of stable random noise to have nice animation of training
+                    
+                    
+                    print("Time took to train model: ",round(timer()-timer_start),2)    
+                    
+                
+                #Save the best achieved model
+                print("Loading model which was performing best during training...\n")
+                self.MODEL.load_weights(self.MODEL_WEIGHTS_DIRECTORY)   
+
+
+
+                                
+
+        def Initialize_history(self,plot_size = 3):
+            if plot_size**2>self.SAMPLE_NUMBER:
+                print("Not enough samples, consider reducing plot size")
+                return
+            #1
+            #Loading most actual model to initialize results
+            try:
+                print("Trying to load most actual model...")
+                self.MODEL.load_weights(self.MODEL_WEIGHTS_DIRECTORY)  
+            except:
+                print("Could not load most actual model, working with current one loaded")
+            
+            #2
+            #Creating 
+            history_array = []
+            path = os.path.join(self.MODEL_DIRECTORY , "Images")
+            img_list = os.listdir(path)
+            
+            for filename in img_list:
+                sample = np.load(os.path.join(path,filename))
+                history_array.append(sample)
+                
+            history_array = np.array(history_array)
+            
+            if len(history_array) == 0:
+                print("There is no data, try to train model a little first")
+            
+            plt.subplots_adjust(bottom=0.25)
+            
+            def update_plot(val):
+                epoch = int(val)
+                plt.suptitle(f"Epoch {epoch}")
+                for i in range(plot_size**2):
+                    plt.axis("off")
+                    plt.subplot(plot_size,plot_size,i+1)
+                    if epoch < len(history_array):
+                        if self.GRAYSCALE:
+                            plt.imshow(history_array[epoch][i], cmap="gray")
+                        else:
+                            plt.imshow(history_array[epoch][i])
+                    else:
+                        plt.text(0,0,"No data")  # Display blank image if epoch exceeds available data
+                plt.draw()
+                    
+            ax_slider = plt.axes([0.25, 0.1, 0.65, 0.03], facecolor='lightgoldenrodyellow')
+            slider = Slider(ax_slider, 'Epoch', 0, len(history_array)-1, valinit=0, valstep=1)
+            
+            # Update the plot when the slider value changes
+            slider.on_changed(update_plot)
+            
+            # Initialize the first plot
+            update_plot(0)
+            
+            plt.show()
+                
+            
+            return history_array , slider
+            
+        
+        def Initialize_results(self,plot_size = 4):
+            #1
+            #Loading most actual model to initialize results
+            try:
+                print("Trying to load most actual model...")
+                self.MODEL.load_weights(self.MODEL_WEIGHTS_DIRECTORY)  
+            except:
+                print("Could not load most actual model, working with current one loaded")
+            
+            Gen_imgs , _ = ml.General.generate_fake_samples(gan_generator = self.GENERATOR,
+                                                    latent_dim = self.LATENT_DIM,
+                                                    n_samples = plot_size**2
+                                                    )
+            Gen_imgs = (Gen_imgs+1)/2
+            
+            plt.figure()
+            plt.suptitle("Results of generator")
+            for i in range(plot_size**2):
+                plt.subplot(plot_size,plot_size,i+1)
+                plt.axis("off")
+                if self.GRAYSCALE:
+                    plt.imshow(Gen_imgs[i] , cmap = 'gray')
+                else:
+                    plt.imshow(Gen_imgs[i])
+                    
+            
+        def Initialize_results_interpolation(self,n_variations = 10, steps_to_variation = 50):
+            gen_img_list = []
+            n_vectors = n_variations
+            steps = steps_to_variation
+            #Interpolated latent vectors for smooth transition effect
+            latent_vectors = [np.random.randn(self.LATENT_DIM) for _ in range(n_vectors)]
+            interpolated_latent_vectors = []
+            for i in range(len(latent_vectors)-1):
+                for alpha in np.linspace(0, 1, steps, endpoint=False):
+                    interpolated_vector = latent_vectors[i] * (1 - alpha) + latent_vectors[i + 1] * alpha
+                    interpolated_latent_vectors.append(interpolated_vector)
+            # Add the last vector to complete the sequence
+
+            for vector in tqdm(interpolated_latent_vectors,desc = "Creating interpolation plot..."):
+                r_vector = np.reshape(vector , (1,len(vector)))
+                
+                gen_img = self.GENERATOR.predict(r_vector , verbose = 0)
+                if len(gen_img.shape) >= 4 and not self.GRAYSCALE:
+                    gen_img = np.reshape(gen_img,(self.IMG_H,self.IMG_W,3))
+                    
+                if len(gen_img.shape) >= 3 and self.GRAYSCALE:
+                    gen_img = np.reshape(gen_img,(self.IMG_H,self.IMG_W))
+                
+                gen_img = (gen_img+1)/2
+                gen_img_list.append(gen_img)
+                ##########
+
+
+                
+                
+            gen_img_list = np.array(gen_img_list)
+            
+            #Plot
+            
+            def update_interpol(i):
+                ax.clear()  # Clear the previous image
+                if self.GRAYSCALE:
+                    ax.imshow(gen_img_list[i], cmap="gray")
+                else:
+                    ax.imshow(gen_img_list[i])
+                    
+                # Optionally, update the title
+                ax.axis("off")
+                plt.draw()
+            
+            # Create the figure and the axis
+            fig, ax = plt.subplots()
+            plt.subplots_adjust(left=0.25, bottom=0.25)
+            
+            # Create the slider
+            ax_slider = plt.axes([0.25, 0.1, 0.65, 0.03], facecolor='lightgoldenrodyellow')
+            inter_slider = Slider(ax_slider, 'Interpolation', 0, len(gen_img_list) - 1, valinit=0, valstep=1)
+            
+            # Update the plot when the slider value changes
+            inter_slider.on_changed(update_interpol)
+            
+            # Initialize the first plot
+            update_interpol(0)
+            
+            plt.show()
+            
+            return gen_img_list , inter_slider
+            
+            
+            
+                        
+                    
+            
+            
+            
+            
+            
+            
+            
+            
+            
+            
+            
+            
+            
+            
+
+
```

## NeuroUtils/ML_assets.py

```diff
@@ -214,16 +214,22 @@
             
     def Load_And_Merge_DataSet(Data_directory , samples_per_class = None):
 
         Classes_list  = os.listdir(Data_directory)
         n_classes = len(Classes_list)
         ClassSet=np.zeros((0,n_classes) , dtype = np.uint8)
         Dictionary = []
-        
-        temporary_sheet = np.load(os.path.join(Data_directory , Classes_list[0]) , mmap_mode='r')
+        try:
+            temporary_sheet = np.load(os.path.join(Data_directory , Classes_list[0]) , mmap_mode='r')
+        except:
+            try:
+                temporary_sheet = np.load(os.path.join(Data_directory , Classes_list[0]) , mmap_mode='r',allow_pickle = True)
+            except:
+                print("Unsuported file in folde, pergaps some sample submission? If you already have dataset set to x_train,x_val, skip this function and go to Process_data")
+                return
         h = temporary_sheet.shape[1]
         w = temporary_sheet.shape[2]
         channels = temporary_sheet.shape[3]
         del temporary_sheet
 
         if channels == 3 :
             x = np.zeros((0,h,w,3) , dtype = np.uint8)
@@ -457,29 +463,37 @@
         if contour:
             image = ImageProcessing.contour_mod(image)
             
         return image        
 
 class General:
     
-    def Load_model_check_training_progress(model , train , model_weights_directory, model_history_directory):
+    def Load_model_check_training_progress(model , train , epochs_to_train, model_weights_directory, model_history_directory):
         starting_epoch = None
         if train:
             try:
                 Model_history = pd.read_csv(model_history_directory)
                 starting_epoch = Model_history["epoch"].iloc[-1]
-                best_val_acc = Model_history["val_accuracy"].idxmax()
-                
-                best_val_loss = round(Model_history["val_loss"][best_val_acc],3)
-                best_val_acc = round(Model_history["val_accuracy"][best_val_acc],3)
+                try:
+                    best_val_acc = Model_history["val_accuracy"].idxmax()
+                    
+                    best_val_loss = round(Model_history["val_loss"][best_val_acc],3)
+                    best_val_acc = round(Model_history["val_accuracy"][best_val_acc],3)
+                except:
+                    print("Could not load model scores...")
         
                 print("Found existing model trained for ",starting_epoch," epochs")
-                print("Best model score aqcuired in ",starting_epoch," epoch\nVal_acc: ",best_val_acc,"\nVal_loss: ",best_val_loss,)
-                
-                print("Do you want to continue training? \nType 'y' for yes and 'n' for no \n")
+                try:
+                    print("Best model score aqcuired in ",starting_epoch," epoch\nVal_acc: ",best_val_acc,"\nVal_loss: ",best_val_loss,)
+                except:
+                    print("No score available")
+                if starting_epoch == epochs_to_train:
+                    print("\nTraining of this model is completed, do you want to load this model? \nType 'y' for yes and 'n' for no \n")
+                else:
+                    print("\nDo you want to continue training? \nType 'y' for yes and 'n' for no \n")
                 user_input = input()
         
                 while True:
                     if user_input.lower() =="y":
                         print("Continuing model training")
                         print("Loading trained weights to model...")
                         model.load_weights(model_weights_directory)
@@ -640,9 +654,69 @@
        
     def Stratification_test(labels):
         print("Dataset stratification test: \n")
         for i in range(labels.shape[1]):
             print("Class",i,"share: ")
             print("Training Set: ", round(sum(labels[:,i])/len(labels),2) )
 
- 
-        
+
+    #Generating real samples from dataset
+    def generate_real_samples(dataset, n_samples):
+        """
+        Taking n random samples from real dataset
+
+        Args:
+            dataset (array):   Dataset to take real samples from
+            n_samples (int)    Amount of samples to take from dataset
+
+
+        Returns:
+            x (array): array of real samples from dataset
+            y (array): array of ones (labels of real samples)
+        """  
+        #Generate random indexes
+        idx = np.random.randint(0, len(dataset), n_samples)
+        #Get random images from dataset
+        x = dataset[idx]
+        #generating labels for real class
+        y = np.ones((n_samples, 1))
+        return x, y   
+
+        
+    #Generating fake samples using noise and generator
+    def generate_fake_samples(gan_generator, latent_dim, n_samples):
+        """
+        Generating n samples using generator
+    
+        Args:
+            gan_generator (compiled model):     Trained generator model
+            latent_dim (array):                 number of parameters to create random noise, it serves as input to the generator
+            n_samples (int):                    Amount of samples to generate
+    
+    
+        Returns:
+            x (array): array of generated samples
+            y (array): array of zeros (labels of fake samples)
+        """ 
+        #generate noise as input for generator
+        noise = np.random.normal(0, 1, (n_samples, latent_dim))
+        # predict outputs
+        x = gan_generator.predict(noise)
+        if len(x.shape) == 4:
+            x = np.squeeze(x, axis = -1)
+        # create 'fake' class labels (0)
+        y = np.zeros((n_samples, 1))
+        return x, y
+    
+
+    def delete_files_in_folder(folder_path):
+        # Iterate over all files in the folder
+        for filename in os.listdir(folder_path):
+            file_path = os.path.join(folder_path, filename)
+            # Check if the path is a file (not a subdirectory)
+            if os.path.isfile(file_path):
+                # Delete the file
+                os.remove(file_path)
+    
+    
+    
+
```

## Comparing `NeuroUtils-0.1.5.dist-info/LICENSE.txt` & `NeuroUtils-0.1.6.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `NeuroUtils-0.1.5.dist-info/METADATA` & `NeuroUtils-0.1.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeuroUtils
-Version: 0.1.5
+Version: 0.1.6
 Summary: Library for neural network projects organisation
 Author-email: Sebastian Borukało <Ciapserr@gmail.com>
 Project-URL: Homepage, https://github.com/Ciapser/NeuroUtils
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 2 - Pre-Alpha
```

