# Comparing `tmp/pwsAI-0.1.1.tar.gz` & `tmp/pwsai-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwsAI-0.1.1.tar", last modified: Fri Dec  8 06:06:27 2023, max compression
+gzip compressed data, was "C:\Users\nai5790\OneDrive - Northwestern University\Documents\personalCoding\git_repos\PWS_AI_git\dist\.tmp-2_pga1xc\pwsai-0.1.", last modified: Wed May 22 09:59:25 2024, max compression
```

## Comparing `pwsAI-0.1.1.tar` & `pwsai-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-12-08 06:06:27.943352 pwsAI-0.1.1/
--rw-rw-rw-   0        0        0     1747 2023-12-08 06:06:27.940059 pwsAI-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1118 2023-12-08 03:27:41.000000 pwsAI-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-12-08 06:06:27.944419 pwsAI-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1500 2023-12-08 06:05:45.000000 pwsAI-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-12-08 06:06:27.593390 pwsAI-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-12-08 06:06:27.831126 pwsAI-0.1.1/src/pwsAI/
--rw-rw-rw-   0        0        0     3018 2023-12-08 03:58:34.000000 pwsAI-0.1.1/src/pwsAI/NIS_Naming_Script.py
--rw-rw-rw-   0        0        0        0 2023-12-08 05:41:23.000000 pwsAI-0.1.1/src/pwsAI/__init__.py
--rw-rw-rw-   0        0        0     6872 2023-12-08 06:05:32.000000 pwsAI-0.1.1/src/pwsAI/__main__.py
-drwxrwxrwx   0        0        0        0 2023-12-08 06:06:27.908734 pwsAI-0.1.1/src/pwsAI/_resources/
--rw-rw-rw-   0        0        0  7852496 2023-12-08 03:27:41.000000 pwsAI-0.1.1/src/pwsAI/_resources/PWS_with_augmentation_weights_minmax_norm_ali_roi_updated_522_images_bf_rms_sw_patch512_100_epoches.hdf5
--rw-rw-rw-   0        0        0    13708 2023-12-08 05:46:09.000000 pwsAI-0.1.1/src/pwsAI/autoSegCube.py
--rw-rw-rw-   0        0        0     2902 2023-12-08 03:27:41.000000 pwsAI-0.1.1/src/pwsAI/convertNuc.py
--rw-rw-rw-   0        0        0     1847 2023-12-08 03:27:41.000000 pwsAI-0.1.1/src/pwsAI/convertRMS.py
--rw-rw-rw-   0        0        0     3318 2023-12-08 03:27:41.000000 pwsAI-0.1.1/src/pwsAI/regular_unet.py
--rw-rw-rw-   0        0        0      922 2023-12-08 03:27:41.000000 pwsAI-0.1.1/src/pwsAI/selectFolder.py
--rw-rw-rw-   0        0        0      389 2023-12-08 03:27:41.000000 pwsAI-0.1.1/src/pwsAI/t.py
-drwxrwxrwx   0        0        0        0 2023-12-08 06:06:27.937530 pwsAI-0.1.1/src/pwsAI.egg-info/
--rw-rw-rw-   0        0        0     1747 2023-12-08 06:06:27.000000 pwsAI-0.1.1/src/pwsAI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      559 2023-12-08 06:06:27.000000 pwsAI-0.1.1/src/pwsAI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-08 06:06:27.000000 pwsAI-0.1.1/src/pwsAI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-12-08 06:06:27.000000 pwsAI-0.1.1/src/pwsAI.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      125 2023-12-08 06:06:27.000000 pwsAI-0.1.1/src/pwsAI.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-12-08 06:06:27.000000 pwsAI-0.1.1/src/pwsAI.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 09:59:25.140446 pwsai-0.1.2/
+-rw-rw-rw-   0        0        0     2521 2024-05-22 09:59:25.131957 pwsai-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1844 2024-05-21 17:34:52.000000 pwsai-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-22 09:59:25.140446 pwsai-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1560 2024-05-22 09:59:09.000000 pwsai-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 09:59:25.086261 pwsai-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-22 09:59:25.112929 pwsai-0.1.2/src/pwsAI/
+-rw-rw-rw-   0        0        0     3018 2024-05-21 17:34:52.000000 pwsai-0.1.2/src/pwsAI/NIS_Naming_Script.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 17:34:52.000000 pwsai-0.1.2/src/pwsAI/__init__.py
+-rw-rw-rw-   0        0        0     7058 2024-05-22 09:52:07.000000 pwsai-0.1.2/src/pwsAI/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 09:59:25.123960 pwsai-0.1.2/src/pwsAI/_resources/
+-rw-rw-rw-   0        0        0  7852496 2024-05-21 17:34:52.000000 pwsai-0.1.2/src/pwsAI/_resources/PWS_with_augmentation_weights_minmax_norm_ali_roi_updated_522_images_bf_rms_sw_patch512_100_epoches.hdf5
+-rw-rw-rw-   0        0        0    13708 2024-05-22 09:41:01.000000 pwsai-0.1.2/src/pwsAI/autoSegCube.py
+-rw-rw-rw-   0        0        0     3785 2024-05-22 09:52:24.000000 pwsai-0.1.2/src/pwsAI/convertNuc.py
+-rw-rw-rw-   0        0        0     1914 2024-05-22 09:40:58.000000 pwsai-0.1.2/src/pwsAI/convertRMS.py
+-rw-rw-rw-   0        0        0     3318 2024-05-21 17:34:52.000000 pwsai-0.1.2/src/pwsAI/regular_unet.py
+-rw-rw-rw-   0        0        0      922 2024-05-21 17:34:52.000000 pwsai-0.1.2/src/pwsAI/selectFolder.py
+-rw-rw-rw-   0        0        0      389 2024-05-21 17:34:52.000000 pwsai-0.1.2/src/pwsAI/t.py
+drwxrwxrwx   0        0        0        0 2024-05-22 09:59:25.131957 pwsai-0.1.2/src/pwsAI.egg-info/
+-rw-rw-rw-   0        0        0     2521 2024-05-22 09:59:25.000000 pwsai-0.1.2/src/pwsAI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      559 2024-05-22 09:59:25.000000 pwsai-0.1.2/src/pwsAI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 09:59:25.000000 pwsai-0.1.2/src/pwsAI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-05-22 09:59:25.000000 pwsai-0.1.2/src/pwsAI.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      157 2024-05-22 09:59:25.000000 pwsai-0.1.2/src/pwsAI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-22 09:59:25.000000 pwsai-0.1.2/src/pwsAI.egg-info/top_level.txt
```

### Comparing `pwsAI-0.1.1/setup.py` & `pwsai-0.1.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,35 +7,36 @@
 import pathlib
 from setuptools import setup, find_packages
 
 HERE = pathlib.Path(__file__).parent  # The directory containing this file
 README = (HERE / "README.md").read_text()  # The text of the README file
 
 setup(name='pwsAI',
-      version='0.1.1',
+      version='0.1.2',
       description='A GUI for AI segmentation of cell imagery.',
       long_description=README,
       long_description_content_type="text/markdown",
       author='Nico Acosta',
       author_email='nicolasacosta2026@u.northwestern.edu',
       url='https://github.com/nanthony21/pws_AI',
-      python_requires='>=3.6',
+      python_requires='>=3.7',
       install_requires=['numpy',
                         'matplotlib',
-                        'PySimpleGUI',
+                        'PySimpleGUI==4.50.0',
                         'pwspy',
                         'pillow',
                         'scikit-image',
                         'scikit-learn',
                         'tifffile',
                         'opencv-python',
                         'patchify',
                         'h5py',
                         'rasterio',
-                        'tensorflow'
+                        'tensorflow==2.6.2',
+                        'protobuf<=3.19.6'
                         ],
       package_dir={'': 'src'},
       package_data={'pwsAI': ['_resources/*']},
       packages=find_packages('src'),
 	  entry_points={'gui_scripts': [
           'PwsAIGui = pwsAI.__main__:main'
       ]}
```

### Comparing `pwsAI-0.1.1/src/pwsAI/NIS_Naming_Script.py` & `pwsai-0.1.2/src/pwsAI/NIS_Naming_Script.py`

 * *Files identical despite different names*

### Comparing `pwsAI-0.1.1/src/pwsAI/__main__.py` & `pwsai-0.1.2/src/pwsAI/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,15 @@
  
 This script imports the naming function that in naming.py
 '''
 import PySimpleGUI as sg
 from pwsAI.selectFolder import select_folder
 from pwsAI.convertRMS import convertrms
 from pwsAI.autoSegCube import autoSeg
+import pwsAI.convertNuc as convertNuc
 import numpy as np
 from matplotlib import pyplot as plt
 
 
 ######################################################
 #################### GUI CODE ########################
 ######################################################
@@ -41,14 +42,15 @@
 
     leftPanel_layout = [[sg.Button('Select Parent Folder!', key='-sf-')]]
 
     rightPanel_layout = [
         [sg.Frame(title='Output', size=(400, 320), layout=[
             [sg.Text("File Path Below, Check before converting the data\nto RMS to input into the AI")],
             [sg.HSeparator()], [sg.Text("", key='-fpath-')],
+            [sg.Text("Analysis Name \n(e.g p0):"),sg.InputText(key='-a_name-')],
             [sg.Button('Get RMS Images', key='-cv_rms-')], [sg.Text("STATUS:\n", key='-rmsGen-')],
             [sg.Text("Threshold Value"), sg.InputText(key='thresh')],
             [sg.Button('Generate Auto ROIs', key='-auto-')], [sg.Text("STATUS:\n", key='-autotxt-')],
             [sg.Button('Push ROI to PWSPY', key='-push-')], [sg.Text("STATUS:\n", key='-pushtext-')]
         ]
                   )]
     ]
@@ -92,18 +94,20 @@
         elif event == '-sf-':
             fpath = select_folder()
             # only print the last two entries of the selected folder path
             tpath = fpath.split('/')
             displayPath = tpath[-3] + '/' + tpath[-2] + '/' + tpath[-1]
             window['-fpath-'].update(f'PATH SELECTED\n{displayPath}')
             print('Select Folder Function')
+
         # conver the iamge to rms
         elif event == '-cv_rms-':
             print('Convert RMS Function')
-            fileList = convertrms(fpath)
+            a_name = values['-a_name-']
+            fileList = convertrms(fpath,a_name)
             window['-rmsGen-'].update('STATUS:\nRMS images generated!')
         # auto roi run in each cell folder, save cube
 
         elif event == '-auto-':
             # run the code wihtin each file path in fileList, however only plot if its in
             # cell num1 because dont want to be annoying
 
@@ -139,15 +143,15 @@
                         else:
                             ax.imshow(data[i])
                             ax.set_title(titles[i])
                     plt.show()
 
             window['-autotxt-'].update('STATUS:\nROIs generated!')
 
-        # gets tricky because of different environment
+        # if installed package correclty this should throw no errors 
         elif event == '-push-':
             print('Push to PWSPY')
             convertNuc.runCvtNuc(fileList)
             window['-pushtext-'].update('STATUS:\nROIs now in PWSPY!')
 
         print('Values', values)
```

### Comparing `pwsAI-0.1.1/src/pwsAI/_resources/PWS_with_augmentation_weights_minmax_norm_ali_roi_updated_522_images_bf_rms_sw_patch512_100_epoches.hdf5` & `pwsai-0.1.2/src/pwsAI/_resources/PWS_with_augmentation_weights_minmax_norm_ali_roi_updated_522_images_bf_rms_sw_patch512_100_epoches.hdf5`

 * *Files identical despite different names*

### Comparing `pwsAI-0.1.1/src/pwsAI/autoSegCube.py` & `pwsai-0.1.2/src/pwsAI/autoSegCube.py`

 * *Files 0% similar despite different names*

```diff
@@ -307,15 +307,15 @@
         blobMask = cv.bitwise_and(colorCopy, colorCopy, mask=binaryMask)
         binaryImage = reconstructed_image - blobMask
         reconstructed_image= binaryImage
         blobMask = blobMask.astype('uint16')
         nucleus_cube.append(blobMask) # create the image cube. This cube can be used to integrate it with PWS software
 
     # ****************** Save the segmented nuclei as tif cube ****************
-    imsave(os.path.join(fpath,f'reconstructed_nuclie_cube_Cell{num}.tif'), nucleus_cube)
+    imsave(os.path.join(fpath,f'reconstructed_nuclei_cube_Cell{num}.tif'), nucleus_cube)
 
 
     return data,titles
 
 
 if __name__ =='__main__':
     # run the code here by giving it the number, the fpath and the thresh
```

### Comparing `pwsAI-0.1.1/src/pwsAI/convertNuc.py` & `pwsai-0.1.2/src/pwsAI/convertNuc.py`

 * *Files 13% similar despite different names*

```diff
@@ -45,19 +45,37 @@
     acq.saveRoi(f'{roiName}',roiNumber,roi)
     print(f"uploaded {roiName} {roiNumber}")
     return 
 
 def runCvtNuc(fileList):
     # get list of all cells from path input
     print(fileList)
+    # now with file List --> run code iteratively through each path
+    for i in range(len(fileList)):
+        cellPath = fileList[i] 
+        # set variables to load in cell folders 
+        num = i+1
+        filename = os.path.join(cellPath,f'reconstructed_nuclei_cube_Cell{num}.tif')
+        # push mask to the pwpsy in each folder 
+        # read images using tif.imread
+        maskCube = tif.imread(filename)
+        # iterate through each mask, convert to rasterio boolean, save to specific acquisiton with specific name 
+        roiName = f"AUTO"
+        for i in range(len(maskCube)):
+            roiNumber = i
+            mask = maskCube[i,:,:].astype(rasterio.bool_)
+            # run importMask with these parameters to save ROI 
+            importMask(mask,cellPath,roiName,roiNumber)
+        print('DONE')
+    
     return
 
 
 if __name__ =='__main__':
-    # hardcoding path rnow because gui saves the 
+    # hardcoding path rnow because gui saves it this is just test dont actually run this 
     genPath = r'''C:\Users\nai5790\OneDrive - Northwestern University\Sunil - PWS Project\PWS Nuclei segmentation AI code\Test\guiTestData'''
     fileList=[]
 
     for file in os.listdir(genPath):
         if  not len(file) == 7 and file[4] != '9':
             if file == ".DS_Store":
                 # removing DS.STORE
```

### Comparing `pwsAI-0.1.1/src/pwsAI/convertRMS.py` & `pwsai-0.1.2/src/pwsAI/convertRMS.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,29 +15,30 @@
 from tkinter import Tk
 from tkinter.filedialog import askdirectory 
 import h5py
 import tifffile as tif
 import numpy as np
 import cv2 as cv
 
-def convertrms(dataPath):
+def convertrms(dataPath,a_name):
     # generate the paths for each of the cell folders, save it in a list 
     fileList = [] 
     for file in os.listdir(dataPath):
         if file.startswith('C'):
             if  not len(file) == 7 and file[4] != '9':
                 if file == ".DS_Store":
                     # removing DS.STORE 
                     os.remove(os.path.join(dataPath,file))
                 else: 
                     fileList.append(os.path.join(dataPath,file))
                 # set cell path 
                 cellPath = os.path.join(dataPath,file)
                 # once you have cell path, open up the analyiss folder and get the rms 
-                fullFileName = os.path.join(cellPath,'PWS/analyses/analysisResults_AD.h5')
+                analysisFileName = f'PWS/analyses/analysisResults_{a_name}.h5'
+                fullFileName = os.path.join(cellPath,analysisFileName)
                 f = h5py.File(fullFileName,'r')
                 rmsArray = f['rms']
                 #print(np.min(rmsArray),np.max(rmsArray))
                 # normalize cv to 0-255 and save it as 8 bit to input intp the model!
                 rmsArrayNorm = cv.normalize(np.array(rmsArray),None,0,255,cv.NORM_MINMAX).astype(np.uint8)
                 tif.imsave(os.path.join(cellPath,f'rms_{file}.tif'),rmsArrayNorm)
```

### Comparing `pwsAI-0.1.1/src/pwsAI/regular_unet.py` & `pwsai-0.1.2/src/pwsAI/regular_unet.py`

 * *Files identical despite different names*

### Comparing `pwsAI-0.1.1/src/pwsAI/selectFolder.py` & `pwsai-0.1.2/src/pwsAI/selectFolder.py`

 * *Files identical despite different names*

### Comparing `pwsAI-0.1.1/src/pwsAI.egg-info/SOURCES.txt` & `pwsai-0.1.2/src/pwsAI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

