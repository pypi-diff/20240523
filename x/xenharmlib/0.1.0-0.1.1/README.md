# Comparing `tmp/xenharmlib-0.1.0.tar.gz` & `tmp/xenharmlib-0.1.1.tar.gz`

## Comparing `xenharmlib-0.1.0.tar` & `xenharmlib-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 xenharmlib-0.1.0/xenharmlib/__init__.py
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 xenharmlib-0.1.0/xenharmlib/exc.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 xenharmlib-0.1.0/xenharmlib/play.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xenharmlib-0.1.0/xenharmlib/core/__init__.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 xenharmlib-0.1.0/xenharmlib/core/constants.py
--rw-r--r--   0        0        0     9963 2020-02-02 00:00:00.000000 xenharmlib-0.1.0/xenharmlib/core/frequencies.py
--rw-r--r--   0        0        0    36281 2020-02-02 00:00:00.000000 xenharmlib-0.1.0/xenharmlib/core/notation.py
--rw-r--r--   0        0        0    36149 2020-02-02 00:00:00.000000 xenharmlib-0.1.0/xenharmlib/core/note_scale.py
--rw-r--r--   0        0        0    24105 2020-02-02 00:00:00.000000 xenharmlib-0.1.0/xenharmlib/core/notes.py
--rw-r--r--   0        0        0    15451 2020-02-02 00:00:00.000000 xenharmlib-0.1.0/xenharmlib/core/pitch.py
--rw-r--r--   0        0        0    25098 2020-02-02 00:00:00.000000 xenharmlib-0.1.0/xenharmlib/core/pitch_scale.py
--rw-r--r--   0        0        0     5104 2020-02-02 00:00:00.000000 xenharmlib-0.1.0/xenharmlib/core/protocols.py
--rw-r--r--   0        0        0    21804 2020-02-02 00:00:00.000000 xenharmlib-0.1.0/xenharmlib/core/symbols.py
--rw-r--r--   0        0        0    17352 2020-02-02 00:00:00.000000 xenharmlib-0.1.0/xenharmlib/core/tunings.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 xenharmlib-0.1.0/xenharmlib/core/utils.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 xenharmlib-0.1.0/xenharmlib/export/__init__.py
--rw-r--r--   0        0        0     6479 2020-02-02 00:00:00.000000 xenharmlib-0.1.0/xenharmlib/export/audio.py
--rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 xenharmlib-0.1.0/xenharmlib/export/scl.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 xenharmlib-0.1.0/xenharmlib/notation/__init__.py
--rw-r--r--   0        0        0    22274 2020-02-02 00:00:00.000000 xenharmlib-0.1.0/xenharmlib/notation/updown.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 xenharmlib-0.1.0/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 xenharmlib-0.1.0/LICENCE
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 xenharmlib-0.1.0/README.md
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 xenharmlib-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 xenharmlib-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 xenharmlib-0.1.1/xenharmlib/__init__.py
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 xenharmlib-0.1.1/xenharmlib/exc.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 xenharmlib-0.1.1/xenharmlib/play.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xenharmlib-0.1.1/xenharmlib/core/__init__.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 xenharmlib-0.1.1/xenharmlib/core/constants.py
+-rw-r--r--   0        0        0    28282 2020-02-02 00:00:00.000000 xenharmlib-0.1.1/xenharmlib/core/frequencies.py
+-rw-r--r--   0        0        0    36281 2020-02-02 00:00:00.000000 xenharmlib-0.1.1/xenharmlib/core/notation.py
+-rw-r--r--   0        0        0    36149 2020-02-02 00:00:00.000000 xenharmlib-0.1.1/xenharmlib/core/note_scale.py
+-rw-r--r--   0        0        0    24105 2020-02-02 00:00:00.000000 xenharmlib-0.1.1/xenharmlib/core/notes.py
+-rw-r--r--   0        0        0    15451 2020-02-02 00:00:00.000000 xenharmlib-0.1.1/xenharmlib/core/pitch.py
+-rw-r--r--   0        0        0    25098 2020-02-02 00:00:00.000000 xenharmlib-0.1.1/xenharmlib/core/pitch_scale.py
+-rw-r--r--   0        0        0     5104 2020-02-02 00:00:00.000000 xenharmlib-0.1.1/xenharmlib/core/protocols.py
+-rw-r--r--   0        0        0    21804 2020-02-02 00:00:00.000000 xenharmlib-0.1.1/xenharmlib/core/symbols.py
+-rw-r--r--   0        0        0    17741 2020-02-02 00:00:00.000000 xenharmlib-0.1.1/xenharmlib/core/tunings.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 xenharmlib-0.1.1/xenharmlib/core/utils.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 xenharmlib-0.1.1/xenharmlib/export/__init__.py
+-rw-r--r--   0        0        0     6483 2020-02-02 00:00:00.000000 xenharmlib-0.1.1/xenharmlib/export/audio.py
+-rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 xenharmlib-0.1.1/xenharmlib/export/scl.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 xenharmlib-0.1.1/xenharmlib/notation/__init__.py
+-rw-r--r--   0        0        0    22274 2020-02-02 00:00:00.000000 xenharmlib-0.1.1/xenharmlib/notation/updown.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 xenharmlib-0.1.1/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 xenharmlib-0.1.1/LICENCE
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 xenharmlib-0.1.1/README.md
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 xenharmlib-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 xenharmlib-0.1.1/PKG-INFO
```

### Comparing `xenharmlib-0.1.0/xenharmlib/exc.py` & `xenharmlib-0.1.1/xenharmlib/exc.py`

 * *Files identical despite different names*

### Comparing `xenharmlib-0.1.0/xenharmlib/play.py` & `xenharmlib-0.1.1/xenharmlib/play.py`

 * *Files identical despite different names*

### Comparing `xenharmlib-0.1.0/xenharmlib/core/constants.py` & `xenharmlib-0.1.1/xenharmlib/core/constants.py`

 * *Files identical despite different names*

### Comparing `xenharmlib-0.1.0/xenharmlib/core/notation.py` & `xenharmlib-0.1.1/xenharmlib/core/notation.py`

 * *Files identical despite different names*

### Comparing `xenharmlib-0.1.0/xenharmlib/core/note_scale.py` & `xenharmlib-0.1.1/xenharmlib/core/note_scale.py`

 * *Files identical despite different names*

### Comparing `xenharmlib-0.1.0/xenharmlib/core/notes.py` & `xenharmlib-0.1.1/xenharmlib/core/notes.py`

 * *Files identical despite different names*

### Comparing `xenharmlib-0.1.0/xenharmlib/core/pitch.py` & `xenharmlib-0.1.1/xenharmlib/core/pitch.py`

 * *Files identical despite different names*

### Comparing `xenharmlib-0.1.0/xenharmlib/core/pitch_scale.py` & `xenharmlib-0.1.1/xenharmlib/core/pitch_scale.py`

 * *Files identical despite different names*

### Comparing `xenharmlib-0.1.0/xenharmlib/core/protocols.py` & `xenharmlib-0.1.1/xenharmlib/core/protocols.py`

 * *Files identical despite different names*

### Comparing `xenharmlib-0.1.0/xenharmlib/core/symbols.py` & `xenharmlib-0.1.1/xenharmlib/core/symbols.py`

 * *Files identical despite different names*

### Comparing `xenharmlib-0.1.0/xenharmlib/core/tunings.py` & `xenharmlib-0.1.1/xenharmlib/core/tunings.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,22 +20,24 @@
 In this module, you will find a collection of tuning classes, each with
 a certain set of assumptions built into them. Some tuning classes can
 be used as they are to create tuning objects, some are abstract classes
 that need a couple of methods implemented by a subclass.
 """
 
 from __future__ import annotations
+import os
 import sympy as sp
 from abc import ABC
 from abc import abstractmethod
 from fractions import Fraction
 from typing import TypeVar
 from typing import Generic
 from typing import List
 from typing import Optional
+from unittest import mock
 
 from .pitch import Pitch
 from .pitch import PitchInterval
 from .pitch_scale import PitchScale
 
 from .pitch import PeriodicPitch
 from .pitch import PeriodicPitchInterval
@@ -44,14 +46,15 @@
 from .pitch import EDPitch
 from .pitch import EDOPitch
 from .pitch import EDPitchInterval
 from .pitch import EDOPitchInterval
 from .pitch_scale import EDPitchScale
 from .pitch_scale import EDOPitchScale
 from .frequencies import Frequency
+from .frequencies import FrequencyRatio
 from ..exc import IncompatibleTunings
 
 PitchT = TypeVar('PitchT', bound=Pitch)
 IntervalT = TypeVar('IntervalT', bound=PitchInterval)
 ScaleT = TypeVar('ScaleT', bound=PitchScale)
 
 
@@ -333,31 +336,35 @@
 
             if p == 1:  # numbers are co-prime
                 generators.append(self.pitch(index))
 
         return generators
 
 
-Hz440C0 = Frequency(sp.Integer(55) / sp.Integer(2) ** sp.Rational(7, 4))
+# hack for RTD (see doc/conf.py for more info)
+if 'READTHEDOCS' in os.environ:
+    Hz440C0 = Frequency(55 / 2 ** Fraction(7, 4))
+else:
+    Hz440C0 = Frequency(sp.Integer(55) / sp.Integer(2) ** sp.Rational(7, 4))
 
 
 class EDTuning(PeriodicTuning[EDPitch, EDPitchInterval, EDPitchScale]):
     """
     EDTuning ("equal division tuning") takes a base interval
     given as a frequency ratio and divides this base interval
     into pitches equally spaced from one another.
 
     For example, the Bohlen-Pierce tuning can be created
     like this:
 
     >>> from xenharmlib import EDTuning
-    >>> from xenharmlib import Frequency
+    >>> from xenharmlib import FrequencyRatio
     >>> BP = EDTuning(
     ...     divisions=13,
-    ...     eq_ratio=Frequency(3)
+    ...     eq_ratio=FrequencyRatio(3)
     ... )
 
     :param divisions: The number of divisions of the base
         interval
     :param eq_ratio: The frequency factor defining the base
         interval (e.g. 2 for an octave, 3/2 for a fifth)
     :param pitch_cls: (Optional) The python class for the pitch
@@ -378,28 +385,34 @@
         lowest pitch (pitch index 0). Defaults to the frequency
         for C0 in EDO tunings for A4 = 440Hz (about 16.35 Hz)
     """
 
     def __init__(
         self,
         divisions,
-        eq_ratio: Frequency,
+        eq_ratio: FrequencyRatio,
         pitch_cls: type[EDPitch] = EDPitch,
         pitch_interval_cls: type[EDPitchInterval] = EDPitchInterval,
         pitch_scale_cls: type[EDPitchScale] = EDPitchScale,
         ref_frequency: Frequency = Hz440C0,
     ):
 
         super().__init__(
             period_length=divisions,
             pitch_cls=pitch_cls,
             pitch_interval_cls=pitch_interval_cls,
             pitch_scale_cls=pitch_scale_cls,
             ref_frequency=ref_frequency,
         )
+
+        if not isinstance(eq_ratio, FrequencyRatio):
+            raise TypeError(
+                'eq_ratio must be a FrequencyRatio'
+            )
+
         self.divisions = divisions
         self.eq_ratio = eq_ratio
 
     @property
     def name(self) -> str:
         expr = f'{self.eq_ratio.sp_expr}'
         return f'{self.divisions}ed{expr}'
@@ -415,15 +428,16 @@
 
         if pitch.tuning is not self:
             raise IncompatibleTunings('Given pitch has a different tuning')
 
         scale_size = len(self)
         index = pitch.pitch_index
         exp = sp.Rational(1, scale_size)
-        return Frequency(self.ref_frequency * (self.eq_ratio**exp) ** index)
+        ratio = (self.eq_ratio**exp)**index
+        return self.ref_frequency * ratio
 
 
 class EDOTuning(EDTuning):
     """
     EDOTuning ("equal division of the octave tuning") divides an
     octave into pitches equally spaced from each other.
 
@@ -454,15 +468,15 @@
         pitch_interval_cls: type[EDOPitchInterval] = EDOPitchInterval,
         pitch_scale_cls: type[EDOPitchScale] = EDOPitchScale,
         ref_frequency: Frequency = Hz440C0,
     ):
 
         super().__init__(
             divisions=divisions,
-            eq_ratio=Frequency(2),
+            eq_ratio=FrequencyRatio(2),
             pitch_cls=pitch_cls,
             pitch_interval_cls=pitch_interval_cls,
             pitch_scale_cls=pitch_scale_cls,
             ref_frequency=ref_frequency,
         )
 
     @property
@@ -472,15 +486,15 @@
     @property
     def best_fifth(self):
         """
         Returns the pitch that best approximates the pure fifth
         (frequency ratio 3/2) in this tuning.
         """
         return self.get_approx_pitch(
-            self.ref_frequency * Frequency(Fraction(3, 2))
+            self.ref_frequency * FrequencyRatio(3, 2)
         )
 
     @property
     def fifth(self):
         """
         Returns the pitch that represents the fifth of
         this tuning. In the default implementation, this
```

### Comparing `xenharmlib-0.1.0/xenharmlib/core/utils.py` & `xenharmlib-0.1.1/xenharmlib/core/utils.py`

 * *Files identical despite different names*

### Comparing `xenharmlib-0.1.0/xenharmlib/export/__init__.py` & `xenharmlib-0.1.1/xenharmlib/export/__init__.py`

 * *Files identical despite different names*

### Comparing `xenharmlib-0.1.0/xenharmlib/export/audio.py` & `xenharmlib-0.1.1/xenharmlib/export/audio.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     :param frequency: The frequency of the sine wave
     :param duration: The duration in seconds
     :param sample_rate: The sample rate of the raw audio
         (optional, default is 22050)
     """
 
-    frequency = float(frequency)
+    frequency = frequency.to_float()
     t = np.linspace(0, duration, math.ceil(sample_rate * duration))
     output = np.sin(2 * np.pi * frequency * t)
 
     # generate fade in/out array (to remove the clicking
     # noise on frequency change)
 
     fade_in_t = min(100, len(output) // 100)
```

### Comparing `xenharmlib-0.1.0/xenharmlib/export/scl.py` & `xenharmlib-0.1.1/xenharmlib/export/scl.py`

 * *Files identical despite different names*

### Comparing `xenharmlib-0.1.0/xenharmlib/notation/updown.py` & `xenharmlib-0.1.1/xenharmlib/notation/updown.py`

 * *Files identical despite different names*

### Comparing `xenharmlib-0.1.0/LICENCE` & `xenharmlib-0.1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `xenharmlib-0.1.0/README.md` & `xenharmlib-0.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 Xenharmlib is a music theory library for the exploration and research of
 microtonality, diatonic set theory, non-standard notations, and many
 more. The library implements a superset of Western classical music theory,
 so you can also use it to compose and analyze music in the boundaries of
 the common practice period or 20th century Western music.
 
+[Click here for the official documentation](https://xenharmlib.readthedocs.io/en/latest/)
+
 So far it supports the following:
 
 * Equal division tunings (e.g. Western, Modern Arabic, Bohlen-Pierce)
 * Analysis of intervals, scales, and their relations to one another
 * Group theoretical analysis (integer pitches, pitch classes, etc)
 * Up/Down Notation (a superset of Western accidental notation)
 * Building blocks for custom notations
```

### Comparing `xenharmlib-0.1.0/pyproject.toml` & `xenharmlib-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.sdist]
 include = ["xenharmlib"]
 
 [project]
 name = "xenharmlib"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Fabian Vallon", email="fabian.vallon@gmail.com" },
 ]
 description = "A library for microtonal music theory"
 keywords = [
     "music",
     "musicology",
@@ -36,9 +36,10 @@
   "numpy>=1.26.4",
   "scipy>=1.12.0",
   "sounddevice>=0.4.6",
   "sympy>=1.12",
 ]
 
 [project.urls]
+Documentation = "https://xenharmlib.readthedocs.io/en/latest/"
 Homepage = "https://gitlab.com/retooth/xenharmlib"
 Issues = "https://gitlab.com/retooth/xenharmlib/-/issues"
```

### Comparing `xenharmlib-0.1.0/PKG-INFO` & `xenharmlib-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.3
 Name: xenharmlib
-Version: 0.1.0
+Version: 0.1.1
 Summary: A library for microtonal music theory
+Project-URL: Documentation, https://xenharmlib.readthedocs.io/en/latest/
 Project-URL: Homepage, https://gitlab.com/retooth/xenharmlib
 Project-URL: Issues, https://gitlab.com/retooth/xenharmlib/-/issues
 Author-email: Fabian Vallon <fabian.vallon@gmail.com>
 License-File: LICENCE
 Keywords: diatonic set theory,microtonal,microtonality,music,music theory,musicology,xenharmonics
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -25,14 +26,16 @@
 
 Xenharmlib is a music theory library for the exploration and research of
 microtonality, diatonic set theory, non-standard notations, and many
 more. The library implements a superset of Western classical music theory,
 so you can also use it to compose and analyze music in the boundaries of
 the common practice period or 20th century Western music.
 
+[Click here for the official documentation](https://xenharmlib.readthedocs.io/en/latest/)
+
 So far it supports the following:
 
 * Equal division tunings (e.g. Western, Modern Arabic, Bohlen-Pierce)
 * Analysis of intervals, scales, and their relations to one another
 * Group theoretical analysis (integer pitches, pitch classes, etc)
 * Up/Down Notation (a superset of Western accidental notation)
 * Building blocks for custom notations
```

