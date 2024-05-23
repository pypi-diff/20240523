# Comparing `tmp/spender-0.2.4.tar.gz` & `tmp/spender-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spender-0.2.4.tar", last modified: Tue Nov  7 16:06:22 2023, max compression
+gzip compressed data, was "spender-0.2.5.tar", last modified: Thu May 23 21:46:20 2024, max compression
```

## Comparing `spender-0.2.4.tar` & `spender-0.2.5.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 pmelchior   (501) staff       (20)        0 2023-11-07 16:06:22.313184 spender-0.2.4/
--rw-r--r--   0 pmelchior   (501) staff       (20)     1082 2022-08-08 22:13:56.000000 spender-0.2.4/LICENSE
--rw-r--r--   0 pmelchior   (501) staff       (20)     5203 2023-11-07 16:06:22.312998 spender-0.2.4/PKG-INFO
--rw-r--r--   0 pmelchior   (501) staff       (20)     4513 2023-10-30 13:32:40.000000 spender-0.2.4/README.md
--rw-r--r--   0 pmelchior   (501) staff       (20)       38 2023-11-07 16:06:22.313236 spender-0.2.4/setup.cfg
--rw-r--r--   0 pmelchior   (501) staff       (20)     1051 2023-11-07 16:03:26.000000 spender-0.2.4/setup.py
-drwxr-xr-x   0 pmelchior   (501) staff       (20)        0 2023-11-07 16:06:22.310789 spender-0.2.4/spender/
--rw-r--r--   0 pmelchior   (501) staff       (20)     3590 2023-11-07 15:49:33.000000 spender-0.2.4/spender/__init__.py
-drwxr-xr-x   0 pmelchior   (501) staff       (20)        0 2023-11-07 16:06:22.312399 spender-0.2.4/spender/data/
--rw-r--r--   0 pmelchior   (501) staff       (20)        0 2022-08-08 22:13:56.000000 spender-0.2.4/spender/data/__init__.py
--rw-r--r--   0 pmelchior   (501) staff       (20)    23704 2023-10-30 11:27:49.000000 spender-0.2.4/spender/data/desi.py
--rwxr-xr-x   0 pmelchior   (501) staff       (20)     1082 2023-05-17 22:05:49.000000 spender-0.2.4/spender/data/emission_lines.py
--rw-r--r--   0 pmelchior   (501) staff       (20)    19391 2023-05-17 22:05:49.000000 spender-0.2.4/spender/data/sdss.py
--rwxr-xr-x   0 pmelchior   (501) staff       (20)     4382 2023-11-07 15:31:14.000000 spender-0.2.4/spender/flow.py
--rw-r--r--   0 pmelchior   (501) staff       (20)     3933 2023-05-17 22:05:49.000000 spender-0.2.4/spender/instrument.py
--rw-r--r--   0 pmelchior   (501) staff       (20)    19985 2023-10-30 13:32:40.000000 spender-0.2.4/spender/model.py
--rw-r--r--   0 pmelchior   (501) staff       (20)     3654 2023-10-30 13:32:40.000000 spender-0.2.4/spender/util.py
-drwxr-xr-x   0 pmelchior   (501) staff       (20)        0 2023-11-07 16:06:22.311517 spender-0.2.4/spender.egg-info/
--rw-r--r--   0 pmelchior   (501) staff       (20)     5203 2023-11-07 16:06:22.000000 spender-0.2.4/spender.egg-info/PKG-INFO
--rw-r--r--   0 pmelchior   (501) staff       (20)      369 2023-11-07 16:06:22.000000 spender-0.2.4/spender.egg-info/SOURCES.txt
--rw-r--r--   0 pmelchior   (501) staff       (20)        1 2023-11-07 16:06:22.000000 spender-0.2.4/spender.egg-info/dependency_links.txt
--rw-r--r--   0 pmelchior   (501) staff       (20)       68 2023-11-07 16:06:22.000000 spender-0.2.4/spender.egg-info/requires.txt
--rw-r--r--   0 pmelchior   (501) staff       (20)        8 2023-11-07 16:06:22.000000 spender-0.2.4/spender.egg-info/top_level.txt
+drwxr-xr-x   0 pmelchior   (501) staff       (20)        0 2024-05-23 21:46:20.835485 spender-0.2.5/
+-rw-r--r--   0 pmelchior   (501) staff       (20)     1087 2024-05-23 21:38:54.000000 spender-0.2.5/LICENSE
+-rw-r--r--   0 pmelchior   (501) staff       (20)     5096 2024-05-23 21:46:20.835360 spender-0.2.5/PKG-INFO
+-rw-r--r--   0 pmelchior   (501) staff       (20)     4406 2024-05-23 21:38:04.000000 spender-0.2.5/README.md
+-rw-r--r--   0 pmelchior   (501) staff       (20)       38 2024-05-23 21:46:20.835525 spender-0.2.5/setup.cfg
+-rw-r--r--   0 pmelchior   (501) staff       (20)     1013 2024-05-23 21:44:04.000000 spender-0.2.5/setup.py
+drwxr-xr-x   0 pmelchior   (501) staff       (20)        0 2024-05-23 21:46:20.832999 spender-0.2.5/spender/
+-rw-r--r--   0 pmelchior   (501) staff       (20)     3607 2024-05-23 21:32:20.000000 spender-0.2.5/spender/__init__.py
+drwxr-xr-x   0 pmelchior   (501) staff       (20)        0 2024-05-23 21:46:20.834746 spender-0.2.5/spender/data/
+-rw-r--r--   0 pmelchior   (501) staff       (20)        0 2022-08-08 22:13:56.000000 spender-0.2.5/spender/data/__init__.py
+-rw-r--r--   0 pmelchior   (501) staff       (20)    23704 2023-10-30 11:27:49.000000 spender-0.2.5/spender/data/desi.py
+-rwxr-xr-x   0 pmelchior   (501) staff       (20)     1082 2023-05-17 22:05:49.000000 spender-0.2.5/spender/data/emission_lines.py
+-rw-r--r--   0 pmelchior   (501) staff       (20)    19391 2023-05-17 22:05:49.000000 spender-0.2.5/spender/data/sdss.py
+-rwxr-xr-x   0 pmelchior   (501) staff       (20)     4382 2023-11-07 15:31:14.000000 spender-0.2.5/spender/flow.py
+-rw-r--r--   0 pmelchior   (501) staff       (20)     1074 2024-05-23 21:29:57.000000 spender-0.2.5/spender/hub.py
+-rw-r--r--   0 pmelchior   (501) staff       (20)     3933 2023-05-17 22:05:49.000000 spender-0.2.5/spender/instrument.py
+-rw-r--r--   0 pmelchior   (501) staff       (20)    19985 2023-10-30 13:32:40.000000 spender-0.2.5/spender/model.py
+-rw-r--r--   0 pmelchior   (501) staff       (20)     3654 2023-10-30 13:32:40.000000 spender-0.2.5/spender/util.py
+drwxr-xr-x   0 pmelchior   (501) staff       (20)        0 2024-05-23 21:46:20.833695 spender-0.2.5/spender.egg-info/
+-rw-r--r--   0 pmelchior   (501) staff       (20)     5096 2024-05-23 21:46:20.000000 spender-0.2.5/spender.egg-info/PKG-INFO
+-rw-r--r--   0 pmelchior   (501) staff       (20)      384 2024-05-23 21:46:20.000000 spender-0.2.5/spender.egg-info/SOURCES.txt
+-rw-r--r--   0 pmelchior   (501) staff       (20)        1 2024-05-23 21:46:20.000000 spender-0.2.5/spender.egg-info/dependency_links.txt
+-rw-r--r--   0 pmelchior   (501) staff       (20)       75 2024-05-23 21:46:20.000000 spender-0.2.5/spender.egg-info/requires.txt
+-rw-r--r--   0 pmelchior   (501) staff       (20)        8 2024-05-23 21:46:20.000000 spender-0.2.5/spender.egg-info/top_level.txt
```

### Comparing `spender-0.2.4/LICENSE` & `spender-0.2.5/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Peter Melchior, Yan Liang
+Copyright (c) 2022-2024 Peter Melchior, Yan Liang
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `spender-0.2.4/PKG-INFO` & `spender-0.2.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spender
-Version: 0.2.4
+Version: 0.2.5
 Summary: Spectrum encoder and decoder
 Home-page: https://github.com/pmelchior/spender
 Author: Peter Melchior
 Author-email: peter.m.melchior@gmail.com
 License: MIT
 Keywords: spectroscopy,autoencoder
 Classifier: Development Status :: 4 - Beta
@@ -29,70 +29,71 @@
 From a data-driven side, galaxy spectra have two fundamental degrees of freedom: their instrinsic spectral properties (or type, if you believe in such a thing) and their redshift. The latter makes them awkward to ingest because it stretches everything, which means spectral features don't appear at the same places. This is why most analyses of the intrinsic properties are done by transforming the observed spectrum to restframe.
 
 We decided to do the opposite. We build a custom architecture, which describes the restframe spectrum by an autoencoder and transforms the restframe model to the observed redshift. While we're at it we also match the spectral resolution and line spread function of the instrument:
 ![sketch](https://github.com/pmelchior/spender/assets/1463403/8e861c0b-358c-4b92-8862-e31325acae1b)
 
 Doing so clearly separates the responsibilities in the architecture. Spender establishes a restframe that has higher resolution and larger wavelength range than the spectra from which it is trained. The model can be trained from spectra at different redshifts or even from different instruments without the need to standardize the observations. Spender also has an explicit, differentiable redshift dependence, which can be coupled with a redshift estimator for a fully data-driven spectrum analysis pipeline.
 
-## Installation (optional: for development)
+## Installation
 
-The easiest way is `pip install spender`. When installing from the code repo, run `pip install -e .`.
+The easiest way is `pip install spender`. When installing from a downloaded code repo, run `pip install -e .`.
 
 For the time being, you will have to install one dependency manually: `torchinterp1d` is available [here](https://github.com/aliutkus/torchinterp1d).
 
-## Pretrained models (requires no spender install)
+## Pretrained models
 
-We make the best-fitting models discussed in the paper available through the Astro Data Lab Hub. Here's a workflow:
+We make the best-fitting models discussed in the paper available through the Astro Data Lab Hub. Here's the workflow:
 
 ```python
-import torch.hub
-github = "pmelchior/spender"
+import os
+import spender
 
-# get the spender code and show list of pretrained models
-torch.hub.list(github)
+# show list of pretrained models
+spender.hub.list()
 
 # print out details for SDSS model from paper II
-print(torch.hub.help(github, 'sdss_II'))
+print(spender.hub.help('sdss_II'))
 
 # load instrument and spectrum model from the hub
-sdss, model = torch.hub.load(github, 'sdss_II')
+sdss, model = spender.hub.load('sdss_II')
 
 # if your machine does not have GPUs, specify the device
 from accelerate import Accelerator
 accelerator = Accelerator(mixed_precision='fp16')
-sdss, model = torch.hub.load(github, 'sdss_II', map_location=accelerator.device)
+sdss, model = spender.hub.load('sdss_II', map_location=accelerator.device)
 ```
  
 ## Outliers Catalogs
 
 catalog of latent-space probabilities for
 * [SDSS-I main galaxy sample](https://hub.pmelchior.net/spender.sdss.paperII.logP.txt.bz2); see Liang et al. (2023a) for details
 * [DESI EDR BGS sample](https://hub.pmelchior.net/spender.desi-edr.full-bgs-objects-logP.txt.bz2); see Liang et al. (2023b) for details
 
 ## Use
 
 Documentation and tutorials are forthcoming. In the meantime, check out `train/diagnostics.ipynb` for a worked through example that generates the figures from the paper.
 
 In short, you can run spender like this:
 ```python
+import os
+import spender
 import torch
 from accelerate import Accelerator
 
 # hardware optimization
 accelerator = Accelerator(mixed_precision='fp16')
 
 # get code, instrument, and pretrained spectrum model from the hub
-github = "pmelchior/spender"
-sdss, model = torch.hub.load(github, 'sdss_II',  map_location=accelerator.device)
+code_dir = os.path.dirname(spender.__file__)
+sdss, model = torch.hub.load(code_dir, 'sdss_II',  map_location=accelerator.device)
 
 # get some SDSS spectra from the ids, store locally in data_path
-from spender.data.sdss import SDSS
 data_path = "./DATA"
 ids = ((412, 52254, 308), (412, 52250, 129))
-spec, w, z, norm, zerr = SDSS.make_batch(data_path, ids)
+spec, w, z, norm, zerr = sdss.make_batch(data_path, ids)
 
 # run spender end-to-end
 with torch.no_grad():
   spec_reco = model(spec, instrument=sdss, z=z)
 
 # for more fine-grained control, run spender's internal _forward method
 # which return the latents s, the model for the restframe, and the observed spectrum
```

### Comparing `spender-0.2.4/README.md` & `spender-0.2.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -9,70 +9,71 @@
 From a data-driven side, galaxy spectra have two fundamental degrees of freedom: their instrinsic spectral properties (or type, if you believe in such a thing) and their redshift. The latter makes them awkward to ingest because it stretches everything, which means spectral features don't appear at the same places. This is why most analyses of the intrinsic properties are done by transforming the observed spectrum to restframe.
 
 We decided to do the opposite. We build a custom architecture, which describes the restframe spectrum by an autoencoder and transforms the restframe model to the observed redshift. While we're at it we also match the spectral resolution and line spread function of the instrument:
 ![sketch](https://github.com/pmelchior/spender/assets/1463403/8e861c0b-358c-4b92-8862-e31325acae1b)
 
 Doing so clearly separates the responsibilities in the architecture. Spender establishes a restframe that has higher resolution and larger wavelength range than the spectra from which it is trained. The model can be trained from spectra at different redshifts or even from different instruments without the need to standardize the observations. Spender also has an explicit, differentiable redshift dependence, which can be coupled with a redshift estimator for a fully data-driven spectrum analysis pipeline.
 
-## Installation (optional: for development)
+## Installation
 
-The easiest way is `pip install spender`. When installing from the code repo, run `pip install -e .`.
+The easiest way is `pip install spender`. When installing from a downloaded code repo, run `pip install -e .`.
 
 For the time being, you will have to install one dependency manually: `torchinterp1d` is available [here](https://github.com/aliutkus/torchinterp1d).
 
-## Pretrained models (requires no spender install)
+## Pretrained models
 
-We make the best-fitting models discussed in the paper available through the Astro Data Lab Hub. Here's a workflow:
+We make the best-fitting models discussed in the paper available through the Astro Data Lab Hub. Here's the workflow:
 
 ```python
-import torch.hub
-github = "pmelchior/spender"
+import os
+import spender
 
-# get the spender code and show list of pretrained models
-torch.hub.list(github)
+# show list of pretrained models
+spender.hub.list()
 
 # print out details for SDSS model from paper II
-print(torch.hub.help(github, 'sdss_II'))
+print(spender.hub.help('sdss_II'))
 
 # load instrument and spectrum model from the hub
-sdss, model = torch.hub.load(github, 'sdss_II')
+sdss, model = spender.hub.load('sdss_II')
 
 # if your machine does not have GPUs, specify the device
 from accelerate import Accelerator
 accelerator = Accelerator(mixed_precision='fp16')
-sdss, model = torch.hub.load(github, 'sdss_II', map_location=accelerator.device)
+sdss, model = spender.hub.load('sdss_II', map_location=accelerator.device)
 ```
  
 ## Outliers Catalogs
 
 catalog of latent-space probabilities for
 * [SDSS-I main galaxy sample](https://hub.pmelchior.net/spender.sdss.paperII.logP.txt.bz2); see Liang et al. (2023a) for details
 * [DESI EDR BGS sample](https://hub.pmelchior.net/spender.desi-edr.full-bgs-objects-logP.txt.bz2); see Liang et al. (2023b) for details
 
 ## Use
 
 Documentation and tutorials are forthcoming. In the meantime, check out `train/diagnostics.ipynb` for a worked through example that generates the figures from the paper.
 
 In short, you can run spender like this:
 ```python
+import os
+import spender
 import torch
 from accelerate import Accelerator
 
 # hardware optimization
 accelerator = Accelerator(mixed_precision='fp16')
 
 # get code, instrument, and pretrained spectrum model from the hub
-github = "pmelchior/spender"
-sdss, model = torch.hub.load(github, 'sdss_II',  map_location=accelerator.device)
+code_dir = os.path.dirname(spender.__file__)
+sdss, model = torch.hub.load(code_dir, 'sdss_II',  map_location=accelerator.device)
 
 # get some SDSS spectra from the ids, store locally in data_path
-from spender.data.sdss import SDSS
 data_path = "./DATA"
 ids = ((412, 52254, 308), (412, 52250, 129))
-spec, w, z, norm, zerr = SDSS.make_batch(data_path, ids)
+spec, w, z, norm, zerr = sdss.make_batch(data_path, ids)
 
 # run spender end-to-end
 with torch.no_grad():
   spec_reco = model(spec, instrument=sdss, z=z)
 
 # for more fine-grained control, run spender's internal _forward method
 # which return the latents s, the model for the restframe, and the observed spectrum
```

### Comparing `spender-0.2.4/setup.py` & `spender-0.2.5/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,27 +3,26 @@
 long_description = open('README.md').read()
 
 setup(
     name="spender",
     description="Spectrum encoder and decoder",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version="0.2.4",
+    version="0.2.5",
     license="MIT",
     author="Peter Melchior",
     author_email="peter.m.melchior@gmail.com",
     url="https://github.com/pmelchior/spender",
     packages=["spender", "spender.data"],
-    package_data={"skymapper.data": ['*.txt']},
     classifiers=[
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: MIT License",
         "Intended Audience :: Developers",
         "Intended Audience :: Education",
         "Intended Audience :: Science/Research",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Topic :: Scientific/Engineering :: Astronomy"
     ],
     keywords = ['spectroscopy','autoencoder'],
-    install_requires=["torch", "numpy", "accelerate", "torchinterp1d", "astropy", "humanize", "psutil", "GPUtil"]
+    install_requires=["torch", "numpy", "accelerate", "torchinterp1d", "astropy", "humanize", "psutil", "GPUtil", "nflows"]
 )
```

### Comparing `spender-0.2.4/spender/__init__.py` & `spender-0.2.5/spender/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import torch
 import torch.hub
-
+from . import hub
 from .flow import NeuralDensityEstimator
 from .instrument import LSF, Instrument
 from .model import (MLP, SpectrumAutoencoder, SpectrumDecoder, SpectrumEncoder,
                     SpeculatorActivation)
 
 
 def load_model(filename, instrument, **kwargs):
```

### Comparing `spender-0.2.4/spender/data/desi.py` & `spender-0.2.5/spender/data/desi.py`

 * *Files identical despite different names*

### Comparing `spender-0.2.4/spender/data/emission_lines.py` & `spender-0.2.5/spender/data/emission_lines.py`

 * *Files identical despite different names*

### Comparing `spender-0.2.4/spender/data/sdss.py` & `spender-0.2.5/spender/data/sdss.py`

 * *Files identical despite different names*

### Comparing `spender-0.2.4/spender/flow.py` & `spender-0.2.5/spender/flow.py`

 * *Files identical despite different names*

### Comparing `spender-0.2.4/spender/instrument.py` & `spender-0.2.5/spender/instrument.py`

 * *Files identical despite different names*

### Comparing `spender-0.2.4/spender/model.py` & `spender-0.2.5/spender/model.py`

 * *Files identical despite different names*

### Comparing `spender-0.2.4/spender/util.py` & `spender-0.2.5/spender/util.py`

 * *Files identical despite different names*

### Comparing `spender-0.2.4/spender.egg-info/PKG-INFO` & `spender-0.2.5/spender.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spender
-Version: 0.2.4
+Version: 0.2.5
 Summary: Spectrum encoder and decoder
 Home-page: https://github.com/pmelchior/spender
 Author: Peter Melchior
 Author-email: peter.m.melchior@gmail.com
 License: MIT
 Keywords: spectroscopy,autoencoder
 Classifier: Development Status :: 4 - Beta
@@ -29,70 +29,71 @@
 From a data-driven side, galaxy spectra have two fundamental degrees of freedom: their instrinsic spectral properties (or type, if you believe in such a thing) and their redshift. The latter makes them awkward to ingest because it stretches everything, which means spectral features don't appear at the same places. This is why most analyses of the intrinsic properties are done by transforming the observed spectrum to restframe.
 
 We decided to do the opposite. We build a custom architecture, which describes the restframe spectrum by an autoencoder and transforms the restframe model to the observed redshift. While we're at it we also match the spectral resolution and line spread function of the instrument:
 ![sketch](https://github.com/pmelchior/spender/assets/1463403/8e861c0b-358c-4b92-8862-e31325acae1b)
 
 Doing so clearly separates the responsibilities in the architecture. Spender establishes a restframe that has higher resolution and larger wavelength range than the spectra from which it is trained. The model can be trained from spectra at different redshifts or even from different instruments without the need to standardize the observations. Spender also has an explicit, differentiable redshift dependence, which can be coupled with a redshift estimator for a fully data-driven spectrum analysis pipeline.
 
-## Installation (optional: for development)
+## Installation
 
-The easiest way is `pip install spender`. When installing from the code repo, run `pip install -e .`.
+The easiest way is `pip install spender`. When installing from a downloaded code repo, run `pip install -e .`.
 
 For the time being, you will have to install one dependency manually: `torchinterp1d` is available [here](https://github.com/aliutkus/torchinterp1d).
 
-## Pretrained models (requires no spender install)
+## Pretrained models
 
-We make the best-fitting models discussed in the paper available through the Astro Data Lab Hub. Here's a workflow:
+We make the best-fitting models discussed in the paper available through the Astro Data Lab Hub. Here's the workflow:
 
 ```python
-import torch.hub
-github = "pmelchior/spender"
+import os
+import spender
 
-# get the spender code and show list of pretrained models
-torch.hub.list(github)
+# show list of pretrained models
+spender.hub.list()
 
 # print out details for SDSS model from paper II
-print(torch.hub.help(github, 'sdss_II'))
+print(spender.hub.help('sdss_II'))
 
 # load instrument and spectrum model from the hub
-sdss, model = torch.hub.load(github, 'sdss_II')
+sdss, model = spender.hub.load('sdss_II')
 
 # if your machine does not have GPUs, specify the device
 from accelerate import Accelerator
 accelerator = Accelerator(mixed_precision='fp16')
-sdss, model = torch.hub.load(github, 'sdss_II', map_location=accelerator.device)
+sdss, model = spender.hub.load('sdss_II', map_location=accelerator.device)
 ```
  
 ## Outliers Catalogs
 
 catalog of latent-space probabilities for
 * [SDSS-I main galaxy sample](https://hub.pmelchior.net/spender.sdss.paperII.logP.txt.bz2); see Liang et al. (2023a) for details
 * [DESI EDR BGS sample](https://hub.pmelchior.net/spender.desi-edr.full-bgs-objects-logP.txt.bz2); see Liang et al. (2023b) for details
 
 ## Use
 
 Documentation and tutorials are forthcoming. In the meantime, check out `train/diagnostics.ipynb` for a worked through example that generates the figures from the paper.
 
 In short, you can run spender like this:
 ```python
+import os
+import spender
 import torch
 from accelerate import Accelerator
 
 # hardware optimization
 accelerator = Accelerator(mixed_precision='fp16')
 
 # get code, instrument, and pretrained spectrum model from the hub
-github = "pmelchior/spender"
-sdss, model = torch.hub.load(github, 'sdss_II',  map_location=accelerator.device)
+code_dir = os.path.dirname(spender.__file__)
+sdss, model = torch.hub.load(code_dir, 'sdss_II',  map_location=accelerator.device)
 
 # get some SDSS spectra from the ids, store locally in data_path
-from spender.data.sdss import SDSS
 data_path = "./DATA"
 ids = ((412, 52254, 308), (412, 52250, 129))
-spec, w, z, norm, zerr = SDSS.make_batch(data_path, ids)
+spec, w, z, norm, zerr = sdss.make_batch(data_path, ids)
 
 # run spender end-to-end
 with torch.no_grad():
   spec_reco = model(spec, instrument=sdss, z=z)
 
 # for more fine-grained control, run spender's internal _forward method
 # which return the latents s, the model for the restframe, and the observed spectrum
```

