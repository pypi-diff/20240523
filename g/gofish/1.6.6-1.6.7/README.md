# Comparing `tmp/gofish-1.6.6.tar.gz` & `tmp/gofish-1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gofish-1.6.6.tar", last modified: Fri Apr 12 12:53:17 2024, max compression
+gzip compressed data, was "gofish-1.6.7.tar", last modified: Thu May 23 19:41:20 2024, max compression
```

## Comparing `gofish-1.6.6.tar` & `gofish-1.6.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 richardteague   (501) staff       (20)        0 2024-04-12 12:53:17.141147 gofish-1.6.6/
--rw-r--r--   0 richardteague   (501) staff       (20)    35149 2023-03-27 18:30:37.000000 gofish-1.6.6/LICENSE.md
--rw-r--r--   0 richardteague   (501) staff       (20)      392 2024-04-12 12:53:17.141023 gofish-1.6.6/PKG-INFO
--rw-r--r--   0 richardteague   (501) staff       (20)     2778 2023-03-27 18:30:37.000000 gofish-1.6.6/README.md
-drwxr-xr-x   0 richardteague   (501) staff       (20)        0 2024-04-12 12:53:17.140312 gofish-1.6.6/gofish/
--rw-r--r--   0 richardteague   (501) staff       (20)      104 2023-03-27 18:30:38.000000 gofish-1.6.6/gofish/__init__.py
--rw-r--r--   0 richardteague   (501) staff       (20)    45466 2023-04-09 23:58:51.000000 gofish-1.6.6/gofish/annulus.py
--rw-r--r--   0 richardteague   (501) staff       (20)   193338 2024-04-12 12:52:54.000000 gofish-1.6.6/gofish/gofish.py
-drwxr-xr-x   0 richardteague   (501) staff       (20)        0 2024-04-12 12:53:17.140903 gofish-1.6.6/gofish.egg-info/
--rw-r--r--   0 richardteague   (501) staff       (20)      392 2024-04-12 12:53:17.000000 gofish-1.6.6/gofish.egg-info/PKG-INFO
--rw-r--r--   0 richardteague   (501) staff       (20)      232 2024-04-12 12:53:17.000000 gofish-1.6.6/gofish.egg-info/SOURCES.txt
--rw-r--r--   0 richardteague   (501) staff       (20)        1 2024-04-12 12:53:17.000000 gofish-1.6.6/gofish.egg-info/dependency_links.txt
--rw-r--r--   0 richardteague   (501) staff       (20)       38 2024-04-12 12:53:17.000000 gofish-1.6.6/gofish.egg-info/requires.txt
--rw-r--r--   0 richardteague   (501) staff       (20)        7 2024-04-12 12:53:17.000000 gofish-1.6.6/gofish.egg-info/top_level.txt
--rw-r--r--   0 richardteague   (501) staff       (20)       38 2024-04-12 12:53:17.141192 gofish-1.6.6/setup.cfg
--rw-r--r--   0 richardteague   (501) staff       (20)      593 2024-04-12 12:53:06.000000 gofish-1.6.6/setup.py
+drwxr-xr-x   0 richardteague   (501) staff       (20)        0 2024-05-23 19:41:20.112329 gofish-1.6.7/
+-rw-r--r--   0 richardteague   (501) staff       (20)    35149 2023-03-27 18:30:37.000000 gofish-1.6.7/LICENSE.md
+-rw-r--r--   0 richardteague   (501) staff       (20)      392 2024-05-23 19:41:20.112218 gofish-1.6.7/PKG-INFO
+-rw-r--r--   0 richardteague   (501) staff       (20)     2778 2023-03-27 18:30:37.000000 gofish-1.6.7/README.md
+drwxr-xr-x   0 richardteague   (501) staff       (20)        0 2024-05-23 19:41:20.111496 gofish-1.6.7/gofish/
+-rw-r--r--   0 richardteague   (501) staff       (20)      102 2024-05-23 18:53:31.000000 gofish-1.6.7/gofish/__init__.py
+-rw-r--r--   0 richardteague   (501) staff       (20)    48508 2024-05-23 19:30:15.000000 gofish-1.6.7/gofish/annulus.py
+-rw-r--r--   0 richardteague   (501) staff       (20)   193338 2024-05-23 19:38:32.000000 gofish-1.6.7/gofish/gofish.py
+drwxr-xr-x   0 richardteague   (501) staff       (20)        0 2024-05-23 19:41:20.112084 gofish-1.6.7/gofish.egg-info/
+-rw-r--r--   0 richardteague   (501) staff       (20)      392 2024-05-23 19:41:20.000000 gofish-1.6.7/gofish.egg-info/PKG-INFO
+-rw-r--r--   0 richardteague   (501) staff       (20)      232 2024-05-23 19:41:20.000000 gofish-1.6.7/gofish.egg-info/SOURCES.txt
+-rw-r--r--   0 richardteague   (501) staff       (20)        1 2024-05-23 19:41:20.000000 gofish-1.6.7/gofish.egg-info/dependency_links.txt
+-rw-r--r--   0 richardteague   (501) staff       (20)       38 2024-05-23 19:41:20.000000 gofish-1.6.7/gofish.egg-info/requires.txt
+-rw-r--r--   0 richardteague   (501) staff       (20)        7 2024-05-23 19:41:20.000000 gofish-1.6.7/gofish.egg-info/top_level.txt
+-rw-r--r--   0 richardteague   (501) staff       (20)       38 2024-05-23 19:41:20.112362 gofish-1.6.7/setup.cfg
+-rw-r--r--   0 richardteague   (501) staff       (20)      593 2024-05-23 18:53:26.000000 gofish-1.6.7/setup.py
```

### Comparing `gofish-1.6.6/LICENSE.md` & `gofish-1.6.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gofish-1.6.6/README.md` & `gofish-1.6.7/README.md`

 * *Files identical despite different names*

### Comparing `gofish-1.6.6/gofish/annulus.py` & `gofish-1.6.7/gofish/annulus.py`

 * *Files 3% similar despite different names*

```diff
@@ -733,15 +733,15 @@
     def _deprojected_spectra(self, vrot, vrad=0.0):
         """Returns all deprojected points as an ensemble."""
         vlos = self.calc_vlos(vrot=vrot, vrad=vrad)
         return np.array([np.interp(self.velax, self.velax - dv, spectra)
                          for dv, spectra in zip(vlos, self.spectra)])
 
     def deprojected_spectrum(self, vrot, vrad=0.0, resample=False,
-                             scatter=False):
+                             scatter=False, empirical_uncertainty=True):
         """
         Returns ``(x, y[, dy])`` of the collapsed and deprojected spectrum
         using the provided velocities to deproject the data. Different methods
         to resample the data can be applied.
 
             ``reasmple=False`` - returns the unbinned, shifted pixels.
 
@@ -761,24 +761,32 @@
 
         Args:
             vrot (float): Rotational velocity in [m/s].
             vrad (optional[float]): Radial velocity in [m/s].
             resample (optional): Type of resampling to be applied.
             scatter (optional[bool]): If the spectrum is resampled, whether to
                 return the scatter in each velocity bin.
+            empirical_uncertainty (optional[bool]): If ``True`` (default),
+                calculate the uncertainty by an iterative sigma clip. If
+                ``False`` then return the standard error on the mean (i.e., 
+                divide the bin standard deviation by the square root of the bin
+                count). This generally results in an underestimated noise.
 
         Returns:
             A deprojected spectrum, resampled using the provided method.
 
         """
         vlos = self.calc_vlos(vrot=vrot, vrad=vrad)
         vpnts = self.velax[None, :] - vlos[:, None]
         vpnts, spnts = self._order_spectra(vpnts=vpnts.flatten())
-        return self._resample_spectra(vpnts, spnts, resample=resample,
-                                      scatter=scatter)
+        return self._resample_spectra(vpnts=vpnts,
+                                      spnts=spnts,
+                                      resample=resample,
+                                      scatter=scatter,
+                                      empirical_uncertainty=empirical_uncertainty)
 
     def _line_centroids(self, method='max', spectra=None, velax=None):
         """
         Return the velocities of the peak pixels.
 
         Args:
             method (str): Method used to determine the line centroid. Must be
@@ -821,15 +829,16 @@
         """Return velocity order spectra."""
         spnts = self.spectra_flat if spnts is None else spnts
         if len(spnts) != len(vpnts):
             raise ValueError("Wrong size in 'vpnts' and 'spnts'.")
         idxs = np.argsort(vpnts)
         return vpnts[idxs], spnts[idxs]
 
-    def _resample_spectra(self, vpnts, spnts, resample=False, scatter=False):
+    def _resample_spectra(self, vpnts, spnts, resample=False, scatter=False,
+                          empirical_uncertainty=True, method='binning'):
         """
         Resample the spectra to a given velocity axis. The scatter is estimated
         as the standard deviation of the bin (note that this is not rescaled by
         the square root of the number of samples).
 
         Args:
             vpnts (ndarray): Array of the velocity values.
@@ -837,25 +846,41 @@
             resample (bool/int/float): Describes the resampling method. If
                 False, no resample is done and the vpnts and spnts are returned
                 as is. If an integer (where True = 1), this samples vpnts on a
                 velocity grid at a sampling rate 'resample' times that of the
                 originally supplied velocity axis. If a float, this will
                 describe the spectral resolution of the sampled grid.
             scatter (bool): If True, return the standard deviation in each bin.
-
+            empirical_uncertainty (optional[bool]): If ``True`` (default),
+                calculate the uncertainty by an iterative sigma clip. If
+                ``False`` then return the standard error on the mean (i.e., 
+                divide the bin standard deviation by the square root of the bin
+                count). This generally results in an underestimated noise.
+            method (optional[str]): Method to resample the spectra. Either
+                `'binning'` or `'smoothing'`. Still TODO!!
+            
         Returns:
             x (ndarray): Velocity bin centers.
             y (ndarray): Mean of the bin.
             dy (ndarray/None): Standard error on the mean of the bin.
         """
+
+        if method != 'binning':
+            raise NotImplementedError("Hold your horses!")
+
+        # If no resampling is requested, just return the raw points.
+
         if isinstance(resample, bool):
             if not resample:
                 if not scatter:
                     return vpnts, spnts
                 return vpnts, spnts, np.zeros(vpnts.size)
+            
+        # Otherwise, we decide what sampling we want.
+
         if isinstance(resample, (int, bool)):
             bins = int(self.velax.size * int(resample) + 1)
             bins = np.linspace(self.velax[0], self.velax[-1], bins)
         elif isinstance(resample, float):
             bins = np.arange(self.velax[0], self.velax[-1], resample)
             bins += 0.5 * (vpnts.max() - bins[-1])
         elif isinstance(resample, np.ndarray):
@@ -867,17 +892,54 @@
             raise TypeError("Resample must be a boolean, int, float or array.")
         idxs = np.isfinite(spnts)
         vpnts, spnts = vpnts[idxs], spnts[idxs]
         y = binned_statistic(vpnts, spnts, statistic='mean', bins=bins)[0]
         x = np.average([bins[1:], bins[:-1]], axis=0)
         if not scatter:
             return x, y
-        dy = binned_statistic(vpnts, spnts, statistic='std', bins=bins)[0]
+        if empirical_uncertainty:
+            dy = annulus.estimate_uncertainty(y) * np.ones(y.size)
+        else:
+            N = binned_statistic(vpnts, spnts, statistic='count', bins=bins)[0]
+            dy = binned_statistic(vpnts, spnts, statistic='std', bins=bins)[0]
+            dy /= np.sqrt(N)
         return x, y, dy
 
+    @staticmethod
+    def estimate_uncertainty(a, nsigma=3.0, niter=20):
+        """
+        Estimate the noise by iteratively sigma-clipping. For each iteraction
+        the ``a`` array is masked above ``abs(a) > nsigma * std`` and the
+        standard deviation, ``std`` calculated. This is repeated until either
+        convergence or for ``niter`` iteractions. In some cases, usually with
+        low ``nsigma`` values, the ``std`` will approach zero and all ``a``
+        values are masked, resulting in an NaN. In this case, the function will
+        return the last finite value.
+
+        Args:
+            a (array): Array of data from which to estimate the uncertainty.
+            nsigma (Optional[float]): Factor of the standard devitation above
+                which to mask ``a`` values.
+            niter (Optional[int]): Number of iterations to halt after if
+                convergence is not reached.
+
+        Returns:
+            std (float): Standard deviation of the sigma-clipped data.
+        """
+        if niter < 1:
+            raise ValueError("Must have at least one iteration.")
+        nonzero = a != 0.0
+        std = np.nanmax(a)
+        for _ in range(niter):
+            std_new = np.nanstd(a[(abs(a) <= nsigma * std) & nonzero])
+            if std_new == std or np.isnan(std_new) or std_new == 0.0:
+                return std
+            std = std_new
+        return std
+
     def _get_masked_spectrum(self, x, y):
         """Return the masked spectrum for fitting."""
         mask = np.logical_and(x >= self.velax_mask[0], x <= self.velax_mask[1])
         return x[mask], y[mask]
 
     def guess_parameters(self, method='quadratic', fit=True):
         """
```

### Comparing `gofish-1.6.6/gofish/gofish.py` & `gofish-1.6.7/gofish/gofish.py`

 * *Files 0% similar despite different names*

```diff
@@ -1067,15 +1067,15 @@
         maskC = np.where(maskA * maskB[None, :, :], 1, 0)
         masked_data = self.data.copy() * maskC * self.beams_per_pix
 
         # Integrate the emission. Uncertainty is sqrt(Nbeams) * RMS.
 
         flux = np.array([c.sum() for c in masked_data])
         flux_error = np.sqrt([c.sum() for c in maskC])
-        flux_error *= self.beams_per_pix**1.5 * self.rms
+        flux_error *= self.beams_per_pix**0.5 * self.rms
 
         return self.velax, flux, flux_error
 
     def radial_spectra(self, rvals=None, rbins=None, dr=None, x0=0.0, y0=0.0,
         inc=0.0, PA=0.0, z0=None, psi=None, r_cavity=None, r_taper=None,
         q_taper=None, z_func=None, mstar=1.0, dist=100., resample=1,
         beam_spacing=False, r_min=None, r_max=None, PA_min=None, PA_max=None,
```

### Comparing `gofish-1.6.6/setup.py` & `gofish-1.6.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="gofish",
-    version="1.6.6",
+    version="1.6.7",
     author="Richard Teague",
     author_email="rteague@mit.edu",
     description="Fishing for molecular line emission in protoplanetary disks.",
     url="https://github.com/richteague/gofish",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
```

