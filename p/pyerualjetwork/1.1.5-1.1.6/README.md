# Comparing `tmp/pyerualjetwork-1.1.5.tar.gz` & `tmp/pyerualjetwork-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyerualjetwork-1.1.5.tar", last modified: Thu May 23 00:30:56 2024, max compression
+gzip compressed data, was "pyerualjetwork-1.1.6.tar", last modified: Thu May 23 00:46:13 2024, max compression
```

## Comparing `pyerualjetwork-1.1.5.tar` & `pyerualjetwork-1.1.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 00:30:56.736061 pyerualjetwork-1.1.5/
--rw-rw-rw-   0        0        0      276 2024-05-23 00:30:56.736061 pyerualjetwork-1.1.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-23 00:30:56.725529 pyerualjetwork-1.1.5/plan/
--rw-rw-rw-   0        0        0      315 2024-05-23 00:30:11.000000 pyerualjetwork-1.1.5/plan/__init__.py
--rw-rw-rw-   0        0        0    40243 2024-05-22 22:36:00.000000 pyerualjetwork-1.1.5/plan/plan.py
-drwxrwxrwx   0        0        0        0 2024-05-23 00:30:56.736061 pyerualjetwork-1.1.5/pyerualjetwork.egg-info/
--rw-rw-rw-   0        0        0      276 2024-05-23 00:30:56.000000 pyerualjetwork-1.1.5/pyerualjetwork.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-05-23 00:30:56.000000 pyerualjetwork-1.1.5/pyerualjetwork.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 00:30:56.000000 pyerualjetwork-1.1.5/pyerualjetwork.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-23 00:30:56.000000 pyerualjetwork-1.1.5/pyerualjetwork.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 00:30:56.736061 pyerualjetwork-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0      452 2024-05-23 00:30:49.000000 pyerualjetwork-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 00:46:13.330536 pyerualjetwork-1.1.6/
+-rw-rw-rw-   0        0        0      276 2024-05-23 00:46:13.330536 pyerualjetwork-1.1.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-23 00:46:13.314911 pyerualjetwork-1.1.6/plan/
+-rw-rw-rw-   0        0        0      315 2024-05-23 00:45:27.000000 pyerualjetwork-1.1.6/plan/__init__.py
+-rw-rw-rw-   0        0        0    40246 2024-05-23 00:44:58.000000 pyerualjetwork-1.1.6/plan/plan.py
+drwxrwxrwx   0        0        0        0 2024-05-23 00:46:13.330536 pyerualjetwork-1.1.6/pyerualjetwork.egg-info/
+-rw-rw-rw-   0        0        0      276 2024-05-23 00:46:12.000000 pyerualjetwork-1.1.6/pyerualjetwork.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-05-23 00:46:13.000000 pyerualjetwork-1.1.6/pyerualjetwork.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 00:46:12.000000 pyerualjetwork-1.1.6/pyerualjetwork.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-23 00:46:12.000000 pyerualjetwork-1.1.6/pyerualjetwork.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 00:46:13.330536 pyerualjetwork-1.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      452 2024-05-23 00:46:02.000000 pyerualjetwork-1.1.6/setup.py
```

### Comparing `pyerualjetwork-1.1.5/plan/plan.py` & `pyerualjetwork-1.1.6/plan/plan.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import numpy as np
 import time
 from colorama import Fore,Style
 from typing import List, Union
 import math
 # BUILD -----
-def TrainDPNN(
+def TrainPLAN(
     Inputs: List[Union[int, float]], 
     Labels: List[Union[int, float, str]], # At least two.. and one hot encoded
     ClassCount: int,
     Layers: List[str],
     Neurons: List[Union[int, float]],
     ThresholdSigns: List[str],
     ThresholdValues: List[Union[int, float]],
     Normalizations: List[str],
     Activations: List[str]
 ) -> str:
         
-    infoDPNN = """
-    Creates and configures a DPNN model.
+    infoPLAN = """
+    Creates and configures a PLAN model.
     
     Args:
         Inputs (list[num]): List of input data.
         Labels (list[num]): List of labels. (one hot encoded)
         ClassCount (int): Number of classes.
         Layers (list[str]): List of layer names. (options: 'fex' (Feature Extraction), 'cat' (Catalyser))
         Neurons (list[num]): List of neuron counts for each layer.
@@ -33,107 +33,107 @@
     Returns:
         list([num]): (Weight matrices list, TrainPredictions list.).
         error handled ?: Process status ('e')
 """
         
     LastNeuron = Neurons[-1:][0]
     if LastNeuron != ClassCount:
-            print(Fore.RED + "ERROR108: Last layer of neuron count must be equal class count. from: TrainDPNN",infoDPNN)
+            print(Fore.RED + "ERROR108: Last layer of neuron count must be equal class count. from: TrainPLAN",infoPLAN)
             return 'e'
     
     if len(Normalizations) != len(ThresholdValues):
         
-            print(Fore.RED + "ERROR307: Normalization list length must be equal to length of ThresholdSigns List,ThresholdValues List,Layers List,Neurons List. from: TrainDPNN",infoDPNN)
+            print(Fore.RED + "ERROR307: Normalization list length must be equal to length of ThresholdSigns List,ThresholdValues List,Layers List,Neurons List. from: TrainPLAN",infoPLAN)
             return 'e'
     
     if len(Inputs) != len(Labels):
-        print(Fore.RED + "ERROR301: Inputs list and Labels list must be same length.",infoDPNN)
+        print(Fore.RED + "ERROR301: Inputs list and Labels list must be same length.",infoPLAN)
         return 'e'
     
     for i, Value in enumerate(ThresholdValues):
         
         if Normalizations[i] != 'y' and Normalizations[i] != 'n':
-                print(Fore.RED + "ERROR105: Normalization list must be 'y' or 'n'.",infoDPNN)
+                print(Fore.RED + "ERROR105: Normalization list must be 'y' or 'n'.",infoPLAN)
                 return 'e'
             
         if ThresholdSigns[i] == 'none':
-            print(Fore.MAGENTA + "WARNING102: We are advise to do not put 'none' Threshold sign. But some cases improves performance of the model from: TrainDPNN",infoDPNN  + Style.RESET_ALL)
+            print(Fore.MAGENTA + "WARNING102: We are advise to do not put 'none' Threshold sign. But some cases improves performance of the model from: TrainPLAN",infoPLAN  + Style.RESET_ALL)
             time.sleep(3)
             
         if isinstance(Value, str):
-            print(Fore.RED + "ERROR201: Threshold values must be numeric. from: TrainDPNN")
+            print(Fore.RED + "ERROR201: Threshold values must be numeric. from: TrainPLAN")
             return 'e'
         
         if isinstance(Neurons[i], str):
             print(Fore.RED + "ERROR202: Neurons list must be numeric.")
             return 'e'
     
     if len(ThresholdSigns) != len(ThresholdValues):
-        print(Fore.RED + "ERROR302: Threshold signs list and Threshold Values list must be same length. from: TrainDPNN",infoDPNN)
+        print(Fore.RED + "ERROR302: Threshold signs list and Threshold Values list must be same length. from: TrainPLAN",infoPLAN)
         return 'e'
     
     if len(Layers) != len(Neurons):
-        print(Fore.RED + "ERROR303: Layers list and Neurons list must same length. from: TrainDPNN",infoDPNN)
+        print(Fore.RED + "ERROR303: Layers list and Neurons list must same length. from: TrainPLAN",infoPLAN)
         return 'e'
     
     if len(ThresholdValues) != len(Layers) or len(ThresholdSigns) != len(Layers):
-        print(Fore.RED + "ERROR306: Threshold Values and Threshold Signs lists length must be same Layers list length. from: TrainDPNN",infoDPNN)
+        print(Fore.RED + "ERROR306: Threshold Values and Threshold Signs lists length must be same Layers list length. from: TrainPLAN",infoPLAN)
         return 'e'
     
     
     for Activation in Activations:
         if Activation != 'softmax' and Activation != 'sigmoid' and Activation != 'relu' and Activation != 'none':
-            print(Fore.RED + "ERROR108: Activations list must be 'sigmoid' or 'softmax' or 'relu' or 'none' from: TrainDPNN",infoDPNN)
+            print(Fore.RED + "ERROR108: Activations list must be 'sigmoid' or 'softmax' or 'relu' or 'none' from: TrainPLAN",infoPLAN)
             return 'e'
     
 
     for index, Neuron in enumerate(Neurons):
         if Neuron < 1:
-            print(Fore.RED + "ERROR101: Neurons list must be positive non zero integer. from: TrainDPNN",infoDPNN)
+            print(Fore.RED + "ERROR101: Neurons list must be positive non zero integer. from: TrainPLAN",infoPLAN)
             return 'e'
         
         if index + 1 != len(Neurons) and Neuron % 2 != 0:
-            print(Fore.MAGENTA + "WARNING101: We strongly advise to do Neuron counts be should even numbers. from: TrainDPNN",infoDPNN)
+            print(Fore.MAGENTA + "WARNING101: We strongly advise to do Neuron counts be should even numbers. from: TrainPLAN",infoPLAN)
             time.sleep(3)
             
         if Neuron < ClassCount:
-            print(Fore.RED + "ERROR102: Neuron count must be greater than class count(For DPNN). from: TrainDPNN")
+            print(Fore.RED + "ERROR102: Neuron count must be greater than class count(For PLAN). from: TrainPLAN")
             return 'e'
         
         if Layers[index] != 'fex' and Layers[index] != 'cat':
-            print(Fore.RED + "ERROR107: Layers list must be 'fex'(Feature Extraction Layer) or 'cat' (Catalyser Layer). from: TrainDPNN",infoDPNN)
+            print(Fore.RED + "ERROR107: Layers list must be 'fex'(Feature Extraction Layer) or 'cat' (Catalyser Layer). from: TrainPLAN",infoPLAN)
             return 'e'
     
     if len(ThresholdSigns) != len(ThresholdValues):
-        print(Fore.RED + "ERROR305: Threshold signs list and Threshold values list must be same length. from: TrainDPNN",infoDPNN)
+        print(Fore.RED + "ERROR305: Threshold signs list and Threshold values list must be same length. from: TrainPLAN",infoPLAN)
         return 'e'
     
     
     for i, Sign in enumerate(ThresholdSigns):
         if Sign != '>' and Sign != '<' and Sign != '==' and Sign != '!=' and Sign != 'none':
-            print(Fore.RED + "ERROR104: Threshold signs must be '>' or '<' or '==' or '!='. or 'none' from: TrainDPNN",infoDPNN)
+            print(Fore.RED + "ERROR104: Threshold signs must be '>' or '<' or '==' or '!='. or 'none' from: TrainPLAN",infoPLAN)
             return 'e'
         
         if Layers[i] == 'fex' and Sign == 'none':
-            print(Fore.RED + "ERROR109: at layer type 'fex', pairing with 'none' Threshold is not acceptlable. if you want to 'none' put '==' and make threshold value '0'. from: TrainDPNN ",infoDPNN)
+            print(Fore.RED + "ERROR109: at layer type 'fex', pairing with 'none' Threshold is not acceptlable. if you want to 'none' put '==' and make threshold value '0'. from: TrainPLAN ",infoPLAN)
             return 'e'
         
     UniqueLabels = set()
     for sublist in Labels:
       
         UniqueLabels.add(tuple(sublist))
     
     
     UniqueLabels = list(UniqueLabels)
     
     Labels = [tuple(sublist) for sublist in Labels]
     
     
     if len(UniqueLabels) != ClassCount:
-        print(Fore.RED + "ERROR106: Label variety length must be same Class Count. from: TrainDPNN",infoDPNN)
+        print(Fore.RED + "ERROR106: Label variety length must be same Class Count. from: TrainPLAN",infoPLAN)
         return 'e'
     
     Inputs[0] = np.array(Inputs[0])
     Inputs[0] = Inputs[0].ravel()
     InputSize = len(Inputs[0])
     
     W = WeightIdentification(len(Layers) - 1,ClassCount,Neurons,InputSize)
@@ -146,15 +146,15 @@
     StartTime = time.time()
     for index, inp in enumerate(Inputs):
         UniStartTime = time.time()
         inp = np.array(inp)
         inp = inp.ravel()
         
         if InputSize != len(inp):
-            print(Fore.RED +"ERROR304: All input matrices or vectors in inputs list, must be same size. from: TrainDPNN",infoDPNN + Style.RESET_ALL)
+            print(Fore.RED +"ERROR304: All input matrices or vectors in inputs list, must be same size. from: TrainPLAN",infoPLAN + Style.RESET_ALL)
             return 'e'
         
         
         for Ulindex, Ul in enumerate(UniqueLabels):
             
             if Ul == Labels[index]:
                 for Windex, w in enumerate(W):
@@ -547,15 +547,15 @@
         list[num]: Transformed data after applying ReLU function.
     """
 
     
     return np.maximum(0, x)
 
 
-def TestDPNN(
+def TestPLAN(
     TestInputs,         # list[list[num]]: Test input data.
     TestLabels,         # list[num]: Test labels.
     Layers,             # list[str]: List of layer names.
     ThresholdSigns,     # list[str]: List of threshold signs for each layer.
     ThresholdValues,    # list[num]: List of threshold values for each layer.
     Normalizations,    # str: Whether normalization will be performed ("y" or "n").
     Activation,         # str: Activation function list for the neural network.
@@ -657,20 +657,20 @@
             print(Fore.MAGENTA + '\nTotal Test Accuracy: ' ,Acc, '\n' + Style.RESET_ALL)
         
         elif Acc <= 0.6:
             print(Fore.RED+ '\nTotal Test Accuracy: ' ,Acc, '\n' + Style.RESET_ALL)   
     
     except:
         
-        print(Fore.RED + "ERROR: Testing model parameters like 'Layers' 'ThresholdCounts' must be same as trained model. Check parameters. Are you sure weights are loaded ? from: TestDPNN" + infoTestModel + Style.RESET_ALL)
+        print(Fore.RED + "ERROR: Testing model parameters like 'Layers' 'ThresholdCounts' must be same as trained model. Check parameters. Are you sure weights are loaded ? from: TestPLAN" + infoTestModel + Style.RESET_ALL)
         return 'e'
    
     return TestPredictions,Acc
 
-def SaveDPNN(ModelName,
+def SavePLAN(ModelName,
              ModelType,
              Layers,
              ClassCount,
              ThresholdSigns,
              ThresholdValues,
              Normalizations,
              Activations,
@@ -678,61 +678,61 @@
              LogType,
              WeightsType,
              WeightFormat,
              SavePath,
              W
  ):
     
-    infoSaveDPNN = """
+    infoSavePLAN = """
     Function to save a deep learning model.
 
     Arguments:
     ModelName (str): Name of the model.
-    ModelType (str): Type of the model.(options: DPNN)
+    ModelType (str): Type of the model.(options: PLAN)
     Layers (list): List containing 'fex' and 'cat' layers.
     ClassCount (int): Number of classes.
     ThresholdSigns (list): List containing threshold signs.
     ThresholdValues (list): List containing threshold values.
     DoNormalization (str): is that normalized data ? 'y' or 'n'.
     Activations (list): List containing activation functions for each layer.
     TestAcc (float): Test accuracy of the model.
     LogType (str): Type of log to save (options: 'csv', 'txt', 'hdf5').
     WeightsType (str): Type of weights to save (options: 'txt', 'npy', 'mat').
     WeightFormat (str): Format of the weights (options: 'd', 'f', 'raw').
-    SavePath (str): Path where the model will be saved. For example: C:/Users/beydili/Desktop/denemeDPNN/
+    SavePath (str): Path where the model will be saved. For example: C:/Users/beydili/Desktop/denemePLAN/
     W: Weights of the model.
     
     Returns:
     str: Message indicating if the model was saved successfully or encountered an error.
     """
     
     # Operations to be performed by the function will be written here
     pass
 
     if LogType != 'csv' and  LogType != 'txt' and LogType != 'hdf5':
-        print(Fore.RED + "ERROR109: Save Log Type (File Extension) must be 'csv' or 'txt' or 'hdf5' from: SaveDPNN" + infoSaveDPNN + Style.RESET_ALL)
+        print(Fore.RED + "ERROR109: Save Log Type (File Extension) must be 'csv' or 'txt' or 'hdf5' from: SavePLAN" + infoSavePLAN + Style.RESET_ALL)
         return 'e'
     
     if WeightsType != 'txt' and  WeightsType != 'npy' and WeightsType != 'mat':
-        print(Fore.RED + "ERROR110: Save Weight type (File Extension) Type must be 'txt' or 'npy' or 'mat' from: SaveDPNN" + infoSaveDPNN + Style.RESET_ALL)
+        print(Fore.RED + "ERROR110: Save Weight type (File Extension) Type must be 'txt' or 'npy' or 'mat' from: SavePLAN" + infoSavePLAN + Style.RESET_ALL)
         return 'e'
     
     if WeightFormat != 'd' and  WeightFormat != 'f' and WeightFormat != 'raw':
-        print(Fore.RED + "ERROR111: Weight Format Type must be 'd' or 'f' or 'raw' from: SaveDPNN" + infoSaveDPNN + Style.RESET_ALL)
+        print(Fore.RED + "ERROR111: Weight Format Type must be 'd' or 'f' or 'raw' from: SavePLAN" + infoSavePLAN + Style.RESET_ALL)
         return 'e'
     
     NeuronCount = 0
     SynapseCount = 0
     try:
         for w in W:
             NeuronCount += np.shape(w)[0]
             SynapseCount += np.shape(w)[0] * np.shape(w)[1]
     except:
         
-        print(Fore.RED + "ERROR: Weight matrices has a problem from: SaveDPNN" + infoSaveDPNN + Style.RESET_ALL)
+        print(Fore.RED + "ERROR: Weight matrices has a problem from: SavePLAN" + infoSavePLAN + Style.RESET_ALL)
         return 'e'
     import pandas as pd
     from datetime import datetime
     from scipy import io
     
     data = {'MODEL NAME': ModelName,
             'MODEL TYPE': ModelType,
@@ -765,15 +765,15 @@
             
         elif LogType == 'hdf5':
             
             df.to_hdf(SavePath + ModelName + '.h5', key='data', mode='w')
             
     except:
         
-        print(Fore.RED + "ERROR: Model log not saved. Check the log parameters from: SaveDPNN" + infoSaveDPNN + Style.RESET_ALL)
+        print(Fore.RED + "ERROR: Model log not saved. Check the log parameters from: SavePLAN" + infoSavePLAN + Style.RESET_ALL)
         return 'e'
     try:
         
         if WeightsType == 'txt' and WeightFormat == 'd':
             
             for i, w in enumerate(W):
                 np.savetxt(SavePath + ModelName +  str(i+1) + 'w.txt' ,  w, fmt='%d')
@@ -827,31 +827,31 @@
             
             for i, w in enumerate(W):
                 w = {'w': w}
                 io.savemat(SavePath + ModelName + str(i+1) + 'w.mat', w)
             
     except:
         
-        print(Fore.RED + "ERROR: Model Weights not saved. Check the Weight parameters. SaveFilePath expl: 'C:/Users/hasancanbeydili/Desktop/denemeDPNN/' from: SaveDPNN" + infoSaveDPNN + Style.RESET_ALL)
+        print(Fore.RED + "ERROR: Model Weights not saved. Check the Weight parameters. SaveFilePath expl: 'C:/Users/hasancanbeydili/Desktop/denemePLAN/' from: SavePLAN" + infoSavePLAN + Style.RESET_ALL)
         return 'e'
     print(df)
     message = (
         Fore.GREEN + "Model Saved Successfully\n" +
         Fore.MAGENTA + "Don't forget, if you want to load model: model log file and weight files must be in the same directory." + 
         Style.RESET_ALL
         )
     
     return print(message)
 
 
-def LoadDPNN(ModelName,
+def LoadPLAN(ModelName,
              LoadPath,
              LogType,
 ):
-   infoLoadDPNN = """
+   infoLoadPLAN = """
    Function to load a deep learning model.
 
    Arguments:
    ModelName (str): Name of the model.
    LoadPath (str): Path where the model is saved.
    LogType (str): Type of log to load (options: 'csv', 'txt', 'hdf5').
 
@@ -873,15 +873,15 @@
        if LogType == 'txt':
            df = pd.read_csv(LoadPath + ModelName + '.' + LogType, delimiter='\t')
         
     
        if LogType == 'hdf5':
            df = pd.read_hdf(LoadPath + ModelName + '.' + LogType)
    except:
-       print(Fore.RED + "ERROR: Model Path error. Accaptable form: 'C:/Users/hasancanbeydili/Desktop/denemeDPNN/' from: LoadDPNN" + infoLoadDPNN + Style.RESET_ALL)
+       print(Fore.RED + "ERROR: Model Path error. Accaptable form: 'C:/Users/hasancanbeydili/Desktop/denemePLAN/' from: LoadPLAN" + infoLoadPLAN + Style.RESET_ALL)
 
    ModelName = str(df['MODEL NAME'].iloc[0])
    Layers = df['LAYERS'].tolist()
    LayerCount = int(df['LAYER COUNT'].iloc[0])
    ClassCount = int(df['CLASS COUNT'].iloc[0])
    ThresholdSigns = df['THRESHOLD SIGNS'].tolist()
    ThresholdValues = df['THRESHOLD VALUES'].tolist()
@@ -903,32 +903,32 @@
    elif WeightType == 'npy':
        for i in range(LayerCount):    
            W[i] = np.load(LoadPath + ModelName + str(i+1) + 'w.npy')
    elif WeightType == 'mat':
        for i in range(LayerCount):  
            W[i] = sio.loadmat(LoadPath + ModelName + str(i+1) + 'w.mat')
    else:
-        raise ValueError(Fore.RED + "Incorrect weight type value. Value must be 'txt', 'npy' or 'mat' from: LoadDPNN."  + infoLoadDPNN + Style.RESET_ALL)
+        raise ValueError(Fore.RED + "Incorrect weight type value. Value must be 'txt', 'npy' or 'mat' from: LoadPLAN."  + infoLoadPLAN + Style.RESET_ALL)
    print(Fore.GREEN + "Model loaded succesfully" + Style.RESET_ALL)     
    return W,Layers,ThresholdSigns,ThresholdValues,Normalization,Activations,df
 
-def PredictFromDiscDPNN(Input,ModelName,ModelPath,LogType):
-    infoPredictFromDİscDPNN = """
-    Function to make a prediction using a divided pruning deep learning neural network (DPNN).
+def PredictFromDiscPLAN(Input,ModelName,ModelPath,LogType):
+    infoPredictFromDİscPLAN = """
+    Function to make a prediction using a divided pruning deep learning neural network (PLAN).
 
     Arguments:
     Input (list or ndarray): Input data for the model (single vector or single matrix).
     ModelName (str): Name of the model.
     ModelPath (str): Path where the model is saved.
     LogType (str): Type of log to load (options: 'csv', 'txt', 'hdf5').
 
     Returns:
     ndarray: Output from the model.
     """
-    W,Layers,ThresholdSigns,ThresholdValues,Normalization,Activations = LoadDPNN(ModelName,ModelPath,
+    W,Layers,ThresholdSigns,ThresholdValues,Normalization,Activations = LoadPLAN(ModelName,ModelPath,
                                                                                   LogType)[0:6]
     Wc = [0] * len(W)
     for i, w in enumerate(W):
         Wc[i] = np.copy(w)
     try:
         NeuralLayer = Input
         NeuralLayer = np.array(NeuralLayer)
@@ -949,24 +949,24 @@
                                           ThresholdValues[index])
             if Layers[index] == 'cat':
                 NeuralLayer,useless = Cat(NeuralLayer, W[index],
                                           ThresholdSigns[index],
                                           ThresholdValues[index],
                                           0)
     except:
-       print(Fore.RED + "ERROR: The input was probably entered incorrectly. from: PredictFromDiscDPNN"  + infoPredictFromDİscDPNN + Style.RESET_ALL)
+       print(Fore.RED + "ERROR: The input was probably entered incorrectly. from: PredictFromDiscPLAN"  + infoPredictFromDİscPLAN + Style.RESET_ALL)
        return 'e'
     for i, w in enumerate(Wc):
         W[i] = np.copy(w)
     return NeuralLayer
 
 
-def PredictFromRamDPNN(Input,Layers,ThresholdSigns,ThresholdValues,Normalizations,Activations,W):
-    infoPredictFromRamDPNN = """
-    Function to make a prediction using a divided pruning learning neural network (DPNN)
+def PredictFromRamPLAN(Input,Layers,ThresholdSigns,ThresholdValues,Normalizations,Activations,W):
+    infoPredictFromRamPLAN = """
+    Function to make a prediction using a pruning learning artificial neural network (PLAN)
     from weights and parameters stored in memory.
 
     Arguments:
     Input (list or ndarray): Input data for the model (single vector or single matrix).
     Layers (list): Number and types of layers.
     ThresholdSigns (list): Threshold signs.
     ThresholdValues (list): Threshold values.
@@ -1000,15 +1000,15 @@
                                           ThresholdSigns[index],
                                           ThresholdValues[index])
             if Layers[index] == 'cat':
                 NeuralLayer,useless = Cat(NeuralLayer, W[index],
                                           ThresholdSigns[index],
                                           ThresholdValues[index],0)
     except:
-        print(Fore.RED + "ERROR: Unexpected input or wrong model parameters from: PredictFromRamDPNN."  + infoPredictFromRamDPNN + Style.RESET_ALL)
+        print(Fore.RED + "ERROR: Unexpected input or wrong model parameters from: PredictFromRamPLAN."  + infoPredictFromRamPLAN + Style.RESET_ALL)
         return 'e'
     for i, w in enumerate(Wc):
         W[i] = np.copy(w)
     return NeuralLayer
     
 
 def AutoBalancer(TrainInputs, TrainLabels, ClassCount):
```

