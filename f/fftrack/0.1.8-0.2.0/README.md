# Comparing `tmp/fftrack-0.1.8.tar.gz` & `tmp/fftrack-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fftrack-0.1.8.tar", last modified: Thu May  2 13:53:55 2024, max compression
+gzip compressed data, was "fftrack-0.2.0.tar", last modified: Thu May 23 17:00:07 2024, max compression
```

## Comparing `fftrack-0.1.8.tar` & `fftrack-0.2.0.tar`

### file list

```diff
@@ -1,37 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:53:55.686652 fftrack-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-05-02 13:53:55.686652 fftrack-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-02 13:53:51.000000 fftrack-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:53:55.678652 fftrack-0.1.8/fftrack/
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-02 13:53:51.000000 fftrack-0.1.8/fftrack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-02 13:53:51.000000 fftrack-0.1.8/fftrack/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:53:55.682652 fftrack-0.1.8/fftrack/audio/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:53:51.000000 fftrack-0.1.8/fftrack/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9346 2024-05-02 13:53:51.000000 fftrack-0.1.8/fftrack/audio/audio_compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     9160 2024-05-02 13:53:51.000000 fftrack-0.1.8/fftrack/audio/audio_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-05-02 13:53:51.000000 fftrack-0.1.8/fftrack/audio/audio_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-02 13:53:51.000000 fftrack-0.1.8/fftrack/audio/main_audio.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-02 13:53:51.000000 fftrack-0.1.8/fftrack/config.json
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-02 13:53:51.000000 fftrack-0.1.8/fftrack/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:53:55.682652 fftrack-0.1.8/fftrack/database/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-02 13:53:51.000000 fftrack-0.1.8/fftrack/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-05-02 13:53:51.000000 fftrack-0.1.8/fftrack/database/db_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-02 13:53:51.000000 fftrack-0.1.8/fftrack/database/main_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-02 13:53:51.000000 fftrack-0.1.8/fftrack/database/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-05-02 13:53:51.000000 fftrack-0.1.8/fftrack/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:53:55.682652 fftrack-0.1.8/fftrack/matching/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:53:51.000000 fftrack-0.1.8/fftrack/matching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6334 2024-05-02 13:53:51.000000 fftrack-0.1.8/fftrack/matching/main_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     9366 2024-05-02 13:53:51.000000 fftrack-0.1.8/fftrack/matching/matcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:53:55.682652 fftrack-0.1.8/fftrack/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:53:51.000000 fftrack-0.1.8/fftrack/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-05-02 13:53:51.000000 fftrack-0.1.8/fftrack/scripts/populate_database.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-02 13:53:51.000000 fftrack-0.1.8/fftrack/scripts/songs_to_download.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:53:55.682652 fftrack-0.1.8/fftrack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-05-02 13:53:55.000000 fftrack-0.1.8/fftrack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-02 13:53:55.000000 fftrack-0.1.8/fftrack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 13:53:55.000000 fftrack-0.1.8/fftrack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-02 13:53:55.000000 fftrack-0.1.8/fftrack.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-02 13:53:55.000000 fftrack-0.1.8/fftrack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-02 13:53:55.000000 fftrack-0.1.8/fftrack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 13:53:55.686652 fftrack-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-05-02 13:53:51.000000 fftrack-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:00:07.247636 fftrack-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-05-23 17:00:07.247636 fftrack-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-23 17:00:03.000000 fftrack-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:00:07.239636 fftrack-0.2.0/fftrack/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-23 17:00:03.000000 fftrack-0.2.0/fftrack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-23 17:00:03.000000 fftrack-0.2.0/fftrack/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:00:07.243636 fftrack-0.2.0/fftrack/audio/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-23 17:00:03.000000 fftrack-0.2.0/fftrack/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9288 2024-05-23 17:00:03.000000 fftrack-0.2.0/fftrack/audio/audio_compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17808 2024-05-23 17:00:03.000000 fftrack-0.2.0/fftrack/audio/audio_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-23 17:00:03.000000 fftrack-0.2.0/fftrack/audio/audio_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-23 17:00:03.000000 fftrack-0.2.0/fftrack/audio/main_audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-23 17:00:03.000000 fftrack-0.2.0/fftrack/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-23 17:00:03.000000 fftrack-0.2.0/fftrack/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:00:07.243636 fftrack-0.2.0/fftrack/database/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-23 17:00:03.000000 fftrack-0.2.0/fftrack/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-05-23 17:00:03.000000 fftrack-0.2.0/fftrack/database/db_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-23 17:00:03.000000 fftrack-0.2.0/fftrack/database/main_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-23 17:00:03.000000 fftrack-0.2.0/fftrack/database/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10746 2024-05-23 17:00:03.000000 fftrack-0.2.0/fftrack/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:00:07.243636 fftrack-0.2.0/fftrack/matching/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-23 17:00:03.000000 fftrack-0.2.0/fftrack/matching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-05-23 17:00:03.000000 fftrack-0.2.0/fftrack/matching/main_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13889 2024-05-23 17:00:03.000000 fftrack-0.2.0/fftrack/matching/matcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:00:07.243636 fftrack-0.2.0/fftrack/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 17:00:03.000000 fftrack-0.2.0/fftrack/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7063 2024-05-23 17:00:03.000000 fftrack-0.2.0/fftrack/scripts/populate_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-05-23 17:00:03.000000 fftrack-0.2.0/fftrack/scripts/songs_to_download.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:00:07.243636 fftrack-0.2.0/fftrack/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 17:00:03.000000 fftrack-0.2.0/fftrack/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-23 17:00:03.000000 fftrack-0.2.0/fftrack/ui/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 17:00:03.000000 fftrack-0.2.0/fftrack/ui/main_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:00:07.243636 fftrack-0.2.0/fftrack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-05-23 17:00:07.000000 fftrack-0.2.0/fftrack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-23 17:00:07.000000 fftrack-0.2.0/fftrack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 17:00:07.000000 fftrack-0.2.0/fftrack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-23 17:00:07.000000 fftrack-0.2.0/fftrack.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-23 17:00:07.000000 fftrack-0.2.0/fftrack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-23 17:00:07.000000 fftrack-0.2.0/fftrack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 17:00:07.247636 fftrack-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-05-23 17:00:03.000000 fftrack-0.2.0/setup.py
```

### Comparing `fftrack-0.1.8/PKG-INFO` & `fftrack-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fftrack
-Version: 0.1.8
+Version: 0.2.0
 Summary: FFTrack is a Python-based music recognition tool that allows users to identify songs from audio input.
 Author: schuldt-ogre <nschuldt@ogre.run>
 Description-Content-Type: text/markdown
 Requires-Dist: aniso8601>=9.0.1
 Requires-Dist: audioread>=3.0.1
 Requires-Dist: blinker>=1.7.0
 Requires-Dist: certifi>=2024.2.2
@@ -92,21 +92,18 @@
 - Simple database for storing song information
 
 ## Installation
 To install FFTrack, follow these steps:
 1. Clone the repository to your local machine:
 2. Install the package using the following command:
 ```
-pip install .
+pip install fftrack
 ```
-3. Install the required dependencies using the following command:
-```
-pip install -r requirements.txt
-```
-4. Verify the installation by running the following command:
+
+3. Verify the installation by running the following command:
 ```
 fftrack --help
 ```
 
 ## Usage
 ### Database Setup
 To create the database, run the following command in your terminal:
@@ -128,14 +125,16 @@
 
 ## Configuration
 To configure FFTrack, run the following command in your terminal (not available yet):
 ```
 fftrack config
 ```
 
+
+
 [//]: # (## Contributing)
 
 [//]: # (If you want to contribute to this project, please follow these steps:)
 
 
 ## License
```

### Comparing `fftrack-0.1.8/README.md` & `fftrack-0.2.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -11,21 +11,18 @@
 - Simple database for storing song information
 
 ## Installation
 To install FFTrack, follow these steps:
 1. Clone the repository to your local machine:
 2. Install the package using the following command:
 ```
-pip install .
+pip install fftrack
 ```
-3. Install the required dependencies using the following command:
-```
-pip install -r requirements.txt
-```
-4. Verify the installation by running the following command:
+
+3. Verify the installation by running the following command:
 ```
 fftrack --help
 ```
 
 ## Usage
 ### Database Setup
 To create the database, run the following command in your terminal:
@@ -47,14 +44,16 @@
 
 ## Configuration
 To configure FFTrack, run the following command in your terminal (not available yet):
 ```
 fftrack config
 ```
 
+
+
 [//]: # (## Contributing)
 
 [//]: # (If you want to contribute to this project, please follow these steps:)
 
 
 ## License
```

### Comparing `fftrack-0.1.8/fftrack/audio/audio_compare.py` & `fftrack-0.2.0/fftrack/audio/audio_compare.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,12 @@
 import argparse
-import hashlib
 import logging
 from collections import defaultdict, Counter
 
-import librosa
-import matplotlib.colors as colors
 import matplotlib.pyplot as plt
-import numpy as np
-from matplotlib.mlab import window_hanning, specgram
-from pydub import AudioSegment
-from scipy.ndimage import maximum_filter, binary_erosion, generate_binary_structure, iterate_structure
 
 from fftrack.audio.audio_processing import AudioProcessing
 from fftrack.database.db_manager import DatabaseManager
 from fftrack.database.models import create_database
 
 # Constants for fingerprinting
 DEFAULT_FS = 44100  # Sampling rate
@@ -27,38 +20,40 @@
 MIN_HASH_TIME_DELTA = 0  # Min time delta between peaks in a hash
 PEAK_SORT = True  # Whether to sort peaks for hashing
 
 # Constants for matching
 CONFIDENCE_THRESHOLD = 0.5  # Confidence threshold for a match
 
 # Flags for plotting and logging
-PLOT = False
+PLOT = True
 LOG_INFO = True
 
 # Configure logging
-logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
+logging.basicConfig(level=logging.INFO,
+                    format='%(asctime)s - %(levelname)s - %(message)s')
+
 
 def find_matches(sample_hashes, plot=False):
     results, hashes_no_dupl = [], defaultdict(int)
 
     for sample_hash, offset in sample_hashes:
         matching_fingerprints = dbm.get_fingerprint_by_hash(sample_hash)
         for song_id, db_offset in matching_fingerprints:
             # Ensure both offsets are integers
             db_offset = int(db_offset)
-            offset = int(offset)  # This should already be an integer, but just to be safe
+            # This should already be an integer, but just to be safe
+            offset = int(offset)
 
             offset_difference = db_offset - offset
             results.append((song_id, offset_difference))
             hashes_no_dupl[song_id] += 1
 
     return results, hashes_no_dupl
 
 
-
 def align_matches(matches):
     """
     Aligns matches to find the most probable song match.
 
     Params:
         matches (list): List of matches in the format [(song_id, offset_difference), ...].
 
@@ -112,26 +107,30 @@
 
     :param aligned_results: A dictionary of aligned match results for each song.
     :return: A tuple of the best matching song ID and its match details.
     """
     best_match = max(aligned_results.items(), key=lambda x: x[1]["count"])
     return best_match
 
+
 def parse_arguments():
     """Parse command line arguments for song file paths."""
-    parser = argparse.ArgumentParser(description='Compare two songs and determine if they are the same.')
+    parser = argparse.ArgumentParser(
+        description='Compare two songs and determine if they are the same.')
     parser.add_argument('song1', type=str, help='Path to the first song file.')
-    parser.add_argument('song2', type=str, help='Path to the second song file.')
+    parser.add_argument('song2', type=str,
+                        help='Path to the second song file.')
     return parser.parse_args()
 
 
 def main():
     audio_processor = AudioProcessing(plot=False)
     # Setup logging
-    logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
+    logging.basicConfig(level=logging.INFO,
+                        format='%(asctime)s - %(levelname)s - %(message)s')
 
     # Parse arguments
     args = parse_arguments()
 
     # Load and process the first song
     logging.info(f"Loading and processing {args.song1}")
     samples1, rate1 = audio_processor.load_audio_file(args.song1)
@@ -143,52 +142,54 @@
     samples2, rate2 = audio_processor.load_audio_file(args.song2)
     fingerprints2 = fingerprint(samples2)
 
     # Simulate adding the fingerprints of the first song to the database
     db_fingerprints = {"song1": fingerprints1}
 
     # Find matches between the second song and the database
-    matches, hashes_no_dupl = find_matches(fingerprints2, db_fingerprints, plot=PLOT)
+    matches, hashes_no_dupl = find_matches(
+        fingerprints2, db_fingerprints, plot=PLOT)
 
     # Align matches and find the best match
     aligned_results = align_matches(matches)
     best_match_sid, best_match_details = find_best_match(aligned_results)
 
     # Determine if the songs are the same based on the best match
     song_match = "same" if best_match_details['confidence'] > CONFIDENCE_THRESHOLD else "different"
 
     # Print the conclusion and relevant data
     logging.info(f"The songs are {song_match}.")
     logging.info(f"Song ID: {best_match_sid}")
-    logging.info(f"Offset in s: {audio_processor.offset_to_seconds(best_match_details['offset'])}")
+    logging.info(
+        f"Offset in s: {audio_processor.offset_to_seconds(best_match_details['offset'])}")
     logging.info(f"Confidence: {best_match_details['confidence']:.2f}")
 
 
 # if __name__ == "__main__":
 #     main()
 
 # Example usage with an audio file
 if __name__ == "__main__":
 
-    audio_processor = AudioProcessing(plot=False)  # Enable plotting for demonstration
-
+    # Enable plotting for demonstration
+    audio_processor = AudioProcessing(plot=True)
 
     # initialize database
     create_database()
 
     dbm = DatabaseManager()
 
-    print("Adding a new song...")
-    song_id_studio = dbm.add_song("Crazy Little Thing Called Love - Studio", "Queen",
-                                  "A Night at the Opera", "1975-10-31")
-    print(f"Added song with ID: {song_id_studio}")
-
-    song_id_live = dbm.add_song("Crazy Little Thing Called Love - Live", "Queen",
-                                "A Night at the Opera", "1975-10-31")
-    print(f"Added song with ID: {song_id_live}")
+    # print("Adding a new song...")
+    # song_id_studio = dbm.add_song("Crazy Little Thing Called Love - Studio", "Queen",
+    #                               "A Night at the Opera", "1975-10-31")
+    # print(f"Added song with ID: {song_id_studio}")
+    #
+    # song_id_live = dbm.add_song("Crazy Little Thing Called Love - Live", "Queen",
+    #                             "A Night at the Opera", "1975-10-31")
+    # print(f"Added song with ID: {song_id_live}")
 
     file_path1 = "/Users/nicolas/Developer/workspace/Uni/L2/S4/Projet/SONGS/crazy-little-thing.mp3"
     file_path2 = "/Users/nicolas/Developer/workspace/Uni/L2/S4/Projet/SONGS/crazy-little-thing-LIVE.mp3"
     file_path3 = "/Users/nicolas/Developer/workspace/Uni/L2/S4/Projet/SONGS/crazy-little-thing-cropped.mp3"
     # # # Load audio
     samples1, rate1 = audio_processor.load_audio_file(file_path1)
     print(f"Samples shape: {samples1.shape}, type: {type(samples1)}")
@@ -204,42 +205,46 @@
     samples3 = audio_processor.crop_samples(samples1, 3, 6)
 
     # fingerprints1 = fingerprint(samples1)
     # fingerprints2 = fingerprint(samples2)
     # fingerprints3 = fingerprint(samples3)
 
     # Generate fingerprints
-    fingerprints1 = audio_processor.generate_fingerprints_from_samples(samples1)
-    fingerprints2 = audio_processor.generate_fingerprints_from_samples(samples2)
-    fingerprints3 = audio_processor.generate_fingerprints_from_samples(samples3)
-
+    fingerprints1 = audio_processor.generate_fingerprints_from_samples(
+        samples1)
+    fingerprints2 = audio_processor.generate_fingerprints_from_samples_threads(
+        samples2)
+    fingerprints3 = audio_processor.generate_fingerprints_from_samples_threads(
+        samples3)
 
     if PLOT:
         plt.figure(figsize=(15, 7))
-        plt.bar(["Studio", "Cropped", "Live"], [len(fingerprints1), len(fingerprints3), len(fingerprints2)])
+        plt.bar(["Studio", "Cropped", "Live"], [
+                len(fingerprints1), len(fingerprints3), len(fingerprints2)])
         plt.title('Number of Fingerprints')
         plt.xlabel('Sample')
         plt.ylabel('Number of Fingerprints')
         plt.show()
 
-    # add fingerprints to database
-    for fingerprint in fingerprints1:
-        dbm.add_fingerprint(song_id_studio, fingerprint[0], fingerprint[1])
-
-    for fingerprint in fingerprints2:
-        dbm.add_fingerprint(song_id_live, fingerprint[0], fingerprint[1])
+    # # add fingerprints to database
+    # for fingerprint in fingerprints1:
+    #     dbm.add_fingerprint(song_id_studio, fingerprint[0], fingerprint[1])
+    #
+    # for fingerprint in fingerprints2:
+    #     dbm.add_fingerprint(song_id_live, fingerprint[0], fingerprint[1])
 
     # Find matches
     matches, hashes_no_dupl = find_matches(fingerprints3, plot=PLOT)
 
     # determine song with most matches, and also the offset
     aligned_results = align_matches(matches)
     best_match_sid, best_match_details = find_best_match(aligned_results)
 
     # Print results
     match_found = best_match_details["confidence"] > CONFIDENCE_THRESHOLD
     if match_found:
         print(f"Match found!: {best_match_sid}")
-        print(f"Offset: {best_match_details['offset']} ({audio_processor.offset_to_seconds(best_match_details['offset'])}s)")
+        print(
+            f"Offset: {best_match_details['offset']} ({audio_processor.offset_to_seconds(best_match_details['offset'])}s)")
         print(f"Confidence: {best_match_details['confidence']:.2f}")
     else:
         print("No match found.")
```

### Comparing `fftrack-0.1.8/fftrack/database/db_manager.py` & `fftrack-0.2.0/fftrack/database/db_manager.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from datetime import datetime
 
 from sqlalchemy.exc import SQLAlchemyError
 from sqlalchemy.orm import sessionmaker
+from sqlalchemy import and_
 
 from .models import engine, Song, Fingerprint
 
 # Create a Session class bound to the engine (for database interactions with
 # the models defined in models.py)
 Session = sessionmaker(bind=engine)
 
@@ -19,15 +20,14 @@
     def __init__(self, session=None):
         """
         Initializes DatabaseManager with a session.
         If no session is provided, a new session is created.
         """
         self.session = session if session else Session()
 
-
     def add_song(self, title, artist, album=None, release_date=None, youtube_link=None):
         """
         Adds a new song to the database.
 
         Parameters:
             title (str): The title of the song.
             artist (str): The artist of the song.
@@ -39,67 +39,164 @@
             song_id (int): The ID of the newly added song,
             or None if an error occurred.
         """
         try:
             # Convert release_date from string to date object if release_date
             # is not None
             if release_date:
-                release_date = datetime.strptime(release_date,
-                                                 "%Y-%m-%d").date()
+                try:
+                    release_date = datetime.strptime(
+                        release_date, "%Y-%m-%d").date()
+                except ValueError:
+                    release_date = None
 
             new_song = Song(title=title, artist=artist, album=album,
                             release_date=release_date, youtube_link=youtube_link)
             self.session.add(new_song)
             self.session.commit()
             return new_song.song_id
         except SQLAlchemyError as e:
             self.session.rollback()  # Roll back the transaction on error
             print(f"Error adding song to database: {e}")
             return None
 
-
     def get_song_by_id(self, song_id):
         """
         Gets a song by its ID.
 
         Parameters:
             song_id (int): The ID of the song to retrieve.
 
         Returns:
             Song: The Song object if found, None otherwise.
         """
         try:
-            song = self.session.query(Song).filter(Song.song_id == song_id).first()
+            song = self.session.query(Song).filter(
+                Song.song_id == song_id).first()
+            return song
+        except SQLAlchemyError as e:
+            print(f"Error retrieving song from database: {e}")
+            return None
+
+    def get_song_by_title_artist(self, title, artist):
+        """
+        Gets a song by its title, and its artist.
+
+        Parameters:
+            title (string): The title of the song to retrieve.
+            artist (string): The artist of the song to retrieve.
+
+        Returns:
+            Song: The Song object if found, None otherwise.
+        """
+        try:
+            song = self.session.query(Song).filter(
+                and_(Song.title == title, Song.artist == artist)).first()
             return song
         except SQLAlchemyError as e:
             print(f"Error retrieving song from database: {e}")
             return None
 
+    def get_all_songs(self):
+        """
+        Gets all songs from the database.
+
+        Returns:
+            list: A list of Song objects.
+        """
+        try:
+            songs = self.session.query(Song).all()
+            return songs
+        except SQLAlchemyError as e:
+            print(f"Error retrieving songs from database: {e}")
+            return []
+
+    def delete_song(self, song_id):
+        """
+        Deletes a song and its fingerprints from the database.
+
+        Parameters:
+            song_id (int): The ID of the song to delete.
+
+        Returns:
+            bool: True if the song was deleted successfully, False otherwise.
+        """
+        try:
+            song = self.session.query(Song).filter(
+                Song.song_id == song_id).first()
+
+            if song:
+                # delete fingerprints associated with the song
+                fingerprints = self.session.query(Fingerprint).filter(
+                    Fingerprint.song_id == song_id).all()
+                for fingerprint in fingerprints:
+                    self.session.delete(fingerprint)
+                self.session.commit()
+                self.session.delete(song)
+                self.session.commit()
+
+                return True
+
+            else:
+                return False
+
+        except SQLAlchemyError as e:
+            self.session.rollback()
+            print(f"Error deleting song from database: {e}")
+            return False
+
     def add_fingerprint(self, song_id, hex_fingerprint, offset):
         """
         Adds a new fingerprint to the database associated with a song.
 
         Parameters:
             song_id (int): The ID of the song the fingerprint belongs to.
             hex_fingerprint (str): The fingerprint data as a 20-character hexadecimal string.
             offset (int): The offset of the fingerprint within the song.
 
         Returns:
             bool: True if the fingerprint was added successfully, False otherwise.
         """
         try:
-            new_fingerprint = Fingerprint(song_id=song_id, hash=hex_fingerprint, offset=offset)
+            new_fingerprint = Fingerprint(
+                song_id=song_id, hash=hex_fingerprint, offset=offset)
             self.session.add(new_fingerprint)
             self.session.commit()
             return True
         except SQLAlchemyError as e:
             self.session.rollback()
             print(f"Error adding fingerprint to database: {e}")
             return False
 
+    def add_fingerprints_bulk(self, song_id, fingerprints):
+        """
+        Adds multiple fingerprints to the database associated with a song.
+
+        Parameters:
+            song_id (int): The ID of the song the fingerprints belong to.
+            fingerprints (list): A list of tuples, where each tuple contains (hex_fingerprint, offset).
+
+        Returns:
+            bool: True if all fingerprints were added successfully, False otherwise.
+        """
+
+        def prepare_fingerprints_for_bulk_insertion(song_id, fingerprints):
+            return [{'song_id': song_id, 'hash': hex_fingerprint, 'offset': offset} for hex_fingerprint, offset in
+                    fingerprints]
+
+        try:
+            fingerprint_data = prepare_fingerprints_for_bulk_insertion(song_id, fingerprints)
+            self.session.bulk_insert_mappings(Fingerprint, fingerprint_data)
+            self.session.commit()
+            return True
+        except SQLAlchemyError as e:
+            self.session.rollback()
+            print(f"Error adding fingerprints to database: {e}")
+            return False
+
     def get_fingerprint_by_hash(self, hex_fingerprint):
         """
         Fetches fingerprints by their hash, returning offsets and song IDs.
 
         Parameters:
             hex_fingerprint (str): The 20-character hexadecimal hash of the fingerprint to search for.
```

### Comparing `fftrack-0.1.8/fftrack/database/main_db.py` & `fftrack-0.2.0/fftrack/database/main_db.py`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.8/fftrack/matching/main_matching.py` & `fftrack-0.2.0/fftrack/matching/main_matching.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # demo for how to use the matcher
-from .matcher import Matcher
 from fftrack.database.db_manager import DatabaseManager
 from fftrack.database.models import create_database
+from .matcher import Matcher
 
 
 # Initialise database and add songs and their fingerprints to it for testing
 def database():
     # 1. Initialize the database
     print("Initializing the database...")
     create_database()
@@ -140,18 +140,18 @@
     else:
         print("Matcher initialisation failed.")
         return
 
     # 2. Find matches for the sample match
     print("Creating list of possible matches according to hashes...")
     possible_matches, matches_per_song = match.find_matches([('be3e08e64b5e1442168d', 77),
-            ('060e923715797a050c3b', 79),
-            ('8e6e5474fac838a5a78c', 45),
-            ('be3e08e64b5e1442168d', 43),
-            ('228f2e4fe7d02b97790d', 12)])
+                                                             ('060e923715797a050c3b', 79),
+                                                             ('8e6e5474fac838a5a78c', 45),
+                                                             ('be3e08e64b5e1442168d', 43),
+                                                             ('228f2e4fe7d02b97790d', 12)])
 
     if possible_matches:
         print("Possible matches successfully retracted.")
         print(f"Matches per song: {matches_per_song}")
         print(f"List of possible matches: {possible_matches}")
     else:
         print("Matching hashes failed.")
@@ -177,9 +177,10 @@
     else:
         print("Finding best match failed.")
         return
 
     # Clean up
     db_manager.close_session()
 
+
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `fftrack-0.1.8/fftrack/matching/matcher.py` & `fftrack-0.2.0/fftrack/matching/matcher.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,63 @@
 from fftrack.audio.audio_processing import AudioProcessing
 
 import logging
 from collections import defaultdict, Counter
 import matplotlib.pyplot as plt
 
+from fftrack import config as cfg
+
+# config
+config = cfg.load_config()
+
 # Flags for plotting and logging
-PLOT = False
-LOG_LEVEL = logging.INFO
+PLOT = config["plot"]
+level = config["log_level"]
+LOG_LEVEL = logging.getLevelName(level) if level else logging.INFO
 
 # Configure logging
 logging.basicConfig(level=LOG_LEVEL, format='%(asctime)s - %(levelname)s - %(message)s')
 
 # Constants for matching
-CONFIDENCE_THRESHOLD = 0.5  # Confidence threshold for a match
-TOP_N = 5 # Number of top matches to return
+TOP_N = config["matching"]["top_n"]  # Number of top matches to return
+TOP_LIST_BASED_ON = config["matching"]["top_list_based_on"]  # List is constructed by; 0: number of matches, 1: confidence level, 2: mix of the two
+MATCH_COUNT_BENCHMARK = config["matching"][
+    "match_count_benchmark"]  # Minimum number of fingerprint matches needed to count as a match
+# Choose the confidence calculator
+# 0: dividing with the length of offsets,
+# 1: dividing with the sum of all matches,
+# 2: counting score
+CONFIDENCE_CALCULATOR = config["matching"]["confidence_calculator"]
+CONFIDENCE_THRESHOLD = config["matching"]["confidence_threshold"]  # Confidence threshold for a match; for calculator 0 and 1: <1, for 2: >1
+CONFIDENCE_DIFFERENCE = config["matching"]["confidence_difference"]  # if a potential match has less matches but is more confident than the one above it, by confidence_diff
+COUNT_DIFFERENCE = config["matching"]["count_difference"]  # if a potential match is less confident, but has count_diff more matches than the one above it
 
 
 class Matcher:
     """
     Matches the fingerprint of the query with the fingerprints of the database.
     """
 
-    def __init__(self, database_manager, plot=PLOT, confidence_threshold=CONFIDENCE_THRESHOLD, top_n=TOP_N):
+    def __init__(self, database_manager, plot=PLOT, top_n=TOP_N, top_list=TOP_LIST_BASED_ON,
+                 confidence_threshold=CONFIDENCE_THRESHOLD, match_count_benchmark=MATCH_COUNT_BENCHMARK,
+                 confidence_calculator=CONFIDENCE_CALCULATOR, confidence_difference=CONFIDENCE_DIFFERENCE,
+                 count_difference=COUNT_DIFFERENCE):
         """
         Initialises the matcher with the database manager.
         """
         self.db_manager = database_manager
         self.audio_processor = AudioProcessing()
         self.plot = plot
-        self.confidence_threshold = confidence_threshold
         self.top_n = top_n
-
+        self.top_list = top_list
+        self.confidence_threshold = confidence_threshold
+        self.match_count_benchmark = match_count_benchmark
+        self.confidence_calculator = confidence_calculator
+        self.confidence_difference = confidence_difference
+        self.count_difference = count_difference
 
     def get_best_match(self, sample_fingerprint):
         """
         Matches the sample fingerprint with the database.
 
         Args:
             sample_fingerprint (list): List of hashes in the format [(hash, offset), ...].
@@ -43,60 +66,61 @@
             best_match (tuple): A tuple of the best matching song ID and its match details.
         """
 
         # Find matches between sample hashes and the database
         hash_matches, matches_per_song = self.find_matches(sample_fingerprint)
 
         # Align the matches to find the most probable song match
-        aligned_results = self.align_matches(hash_matches, matches_per_song)
+        try:
+            aligned_results = self.align_matches(hash_matches, matches_per_song)
 
-        # Find the best match based on the highest count (confidence)
-        if aligned_results:
+            # Find the best match based on the highest count (confidence)
             top_matches = self.find_top_n_matches(aligned_results, self.top_n)
             best_match = self.find_best_match(top_matches)
-
             return top_matches, best_match
-        else:
+
+        except TypeError:
             logging.info("No matches found, the song is not in the database.")
             return None, None
 
-
     def find_matches(self, sample_hashes):
         """
         Find matches between sample hashes and the database.
 
         Args:
             sample_hashes (list): List of hashes in the format [(hash, offset), ...].
         Returns:
-            tuple: tuple of the match results and the number of unique hashes for each song.
+            possible_matches (list): A list of tuples of the match results, in the form of (song_id, offset_difference)
+            matches_per_song (dict): A dictionary of the song IDs, and the number of matches each song has
         """
 
         logging.info(f"Matching {len(sample_hashes)} fingerprints with the database.")
 
         # Number of hash matches for each song (before aligning)
         matches_per_song = defaultdict(int)
         # List of all the possible matches
         possible_matches = []
 
         for hsh, sampled_offset in sample_hashes:
             # extracting the list of (song_id, offset) for the current hash
             matches_curr_hash = self.db_manager.get_fingerprint_by_hash(hsh)
 
             for sid, db_offset in matches_curr_hash:
-                # Counting hash matches per song, without regards to offset
-                matches_per_song[sid] += 1
-
                 offset_difference = db_offset - sampled_offset
 
                 # To filter the cases when db_offset > sampled_offset
                 if offset_difference >= 0:
                     possible_matches.append((sid, offset_difference))
+                    # Counting hash matches per song, without regards to offset
+                    matches_per_song[sid] += 1
 
-        return possible_matches, matches_per_song
-
+        if possible_matches and matches_per_song:
+            return possible_matches, matches_per_song
+        else:
+            return None, None
 
     def align_matches(self, matches, matches_per_song):
         """
         Aligns the time difference of matches to find the most probable song match.
 
         Args:
             matches (list): List of matches in the format [(song_id, offset_difference), ...].
@@ -116,99 +140,120 @@
         # Analyze offset differences to find the best match
         aligned_results = {}
         # Sum of all the matches to calculate confidence
         sum_matches = 0
 
         for sid, offsets in offset_by_song.items():
             # Find the most common offset and its count (only if it is over the benchmark)
-            # Testing benchmark: 0 matches for the same offset difference
-            offset_counts = Counter({freq: count for freq, count in Counter(offsets).items() if count >= 0})
+            offset_counts = Counter(
+                {freq: count for freq, count in Counter(offsets).items() if count >= self.match_count_benchmark})
 
             if offset_counts:
                 most_common_offset, count = offset_counts.most_common(1)[0]
                 sum_matches += count
 
                 aligned_results[sid] = {
                     "song_id": sid,
                     "offset": most_common_offset,
                     "count": count,
                     "confidence": count / len(offsets)
                 }
 
         # Calculate confidence in a different way than by number of offsets
-        aligned_results = self.confidence_by_matches(aligned_results, sum_matches)
-        #aligned_results = self.confidence_by_score(aligned_results, matches_per_song)
+        if self.confidence_calculator == 1:
+            aligned_results = self.confidence_by_matches(aligned_results, sum_matches)
+        elif self.confidence_calculator == 2:
+            aligned_results = self.confidence_by_score(aligned_results, matches_per_song)
 
         if self.plot:
-            # Plot the distribution of offset differences for each song
-            plt.figure(figsize=(15, 7))
-            for sid, offsets in offset_by_song.items():
-                plt.hist(offsets, bins=50, alpha=0.5, label=sid)
-            plt.title('Distribution of Offset Differences')
-            plt.xlabel('Offset Difference')
-            plt.ylabel('Count')
-            plt.legend()
-            plt.show()
+            self.plot_distribution(offset_by_song)
 
-        return aligned_results
+        if aligned_results:
+            return aligned_results
+        else:
+            return None
 
+    def plot_distribution(self, offset_by_song):
+        """
+        Plot the distribution of offset differences for each song
+        """
+        plt.figure(figsize=(15, 7))
+        for sid, offsets in offset_by_song.items():
+            plt.hist(offsets, bins=50, alpha=0.5, label=sid)
+        plt.title('Distribution of Offset Differences')
+        plt.xlabel('Offset Difference')
+        plt.ylabel('Count')
+        plt.legend()
+        plt.show()
 
     def confidence_by_score(self, aligned_results, matches_per_song):
         """
         Calculates how confident the algorithm is in the correctness of the match,
         which is the sum of hash and offset matches in each song.
 
         Args:
             aligned_results (dict): A dictionary of aligned match results for each song.
             matches_per_song (dict): Dictionary of songs and the number of their hash matches.
         Returns:
             aligned_result: Updated results.
         """
-
+        songs_under_benchmark = []
         for sid, info in aligned_results.items():
             most_common_offset = info["offset"]
             count = info["count"]
             matches_per_song[sid] += count
             info["confidence"] = matches_per_song[sid]
             confidence = info["confidence"]
 
-            logging.info(f"Song ID: {sid}, "
-                         f"Most Common Offset: {most_common_offset} "
-                         f"({self.audio_processor.offset_to_seconds(most_common_offset)}s, "
-                         f"Matches: {count}, "
-                         f"Confidence: {confidence:.2f}")
+            if confidence <= self.confidence_threshold:
+                songs_under_benchmark.append(sid)
 
-        return aligned_results
+            if sid not in songs_under_benchmark:
+                logging.info(f"Song ID: {sid}, "
+                             f"Most Common Offset: {most_common_offset} "
+                             f"({self.audio_processor.offset_to_seconds(most_common_offset)}s, "
+                             f"Matches: {count}, "
+                             f"Confidence: {confidence:.2f}")
 
+        for sid in songs_under_benchmark:
+            del aligned_results[sid]
+
+        return aligned_results
 
     def confidence_by_matches(self, aligned_results, sum_matches):
         """
         Calculates how confident the algorithm is in the correctness of the match.
 
         Args:
             aligned_results (dict): A dictionary of aligned match results for each song.
             sum_matches (int): Sum of all the aligned matches.
         Returns:
             confidence (float): Percentage of confidence in the match, which is the ratio of song matches to total matches.
         """
-
+        songs_under_benchmark = []
         for sid, info in aligned_results.items():
             most_common_offset = info["offset"]
             count = info["count"]
             info["confidence"] = count / sum_matches
             confidence = info["confidence"]
 
-            logging.info(f"Song ID: {sid}, "
-                         f"Most Common Offset: {most_common_offset} "
-                         f"({self.audio_processor.offset_to_seconds(most_common_offset)}s, "
-                         f"Matches: {count}, "
-                         f"Confidence: {confidence:.2f}")
+            if confidence <= self.confidence_threshold:
+                songs_under_benchmark.append(sid)
 
-        return aligned_results
+            if sid not in songs_under_benchmark:
+                logging.info(f"Song ID: {sid}, "
+                             f"Most Common Offset: {most_common_offset} "
+                             f"({self.audio_processor.offset_to_seconds(most_common_offset)}s, "
+                             f"Matches: {count}, "
+                             f"Confidence: {confidence:.2f}")
+
+        for sid in songs_under_benchmark:
+            del aligned_results[sid]
 
+        return aligned_results
 
     def find_top_n_matches(self, aligned_results, n):
         """
         Find the top matches (max top n) from aligned results based on the highest count.
 
         Args:
             aligned_results (dict): A dictionary of aligned match results for each song.
@@ -222,19 +267,57 @@
 
         if nb_song_matches >= n:
             top = n
         else:
             top = nb_song_matches
 
         # Sort and add top matches to a list
-        sorted_matches = sorted(aligned_results.items(), key=lambda x: x[1]['count'], reverse=True)
+        if self.top_list == 0:
+            sorted_matches = sorted(aligned_results.items(), key=lambda x: x[1]['count'], reverse=True)
+        elif self.top_list == 1:
+            sorted_matches = sorted(aligned_results.items(), key=lambda x: x[1]['confidence'], reverse=True)
+        else:
+            sorted_matches = self.sort_by_matches_and_confidence(aligned_results)
+
         top_matches = sorted_matches[:top]
 
         return top_matches
 
+    def sort_by_matches_and_confidence(self, aligned_results):
+        """
+        Sort aligned matches taking into account their number as well as their confidence.
+
+        Args:
+            aligned_results (dict): A dictionary of aligned match results for each song {sid: {sid, offset, count(nb of matches), confidence}}.
+        """
+        sort_by_count = sorted(aligned_results.items(), key=lambda x: x[1]['count'], reverse=True)
+
+        final_list = self.bubble_sort_matches(sort_by_count)
+
+        return final_list
+
+    def bubble_sort_matches(self, sorted_matches):
+        n = len(sorted_matches)
+
+        for i in range(n):
+            swapped = False
+
+            # Last i elements are already in place
+            for j in range(0, n - i - 1):
+                if sorted_matches[j][1]['confidence'] + self.confidence_difference < sorted_matches[j + 1][1]['confidence']\
+                        or (sorted_matches[j][1]['confidence'] < sorted_matches[j + 1][1]['confidence']
+                            and sorted_matches[j][1]['count'] == sorted_matches[j + 1][1]['count'])\
+                        or (sorted_matches[j][1]['confidence'] > sorted_matches[j + 1][1]['confidence']
+                            and sorted_matches[j][1]['count'] + self.count_difference < sorted_matches[j + 1][1]['count']):
+                    sorted_matches[j], sorted_matches[j + 1] = sorted_matches[j + 1], sorted_matches[j]
+                    swapped = True
+            if not swapped:
+                break
+
+        return sorted_matches
 
     def find_best_match(self, top_matches):
         """
         Returns the best match from the top matches.
 
         Args:
             top_matches (list): A list of tuples with the top matches.
```

### Comparing `fftrack-0.1.8/fftrack.egg-info/PKG-INFO` & `fftrack-0.2.0/fftrack.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fftrack
-Version: 0.1.8
+Version: 0.2.0
 Summary: FFTrack is a Python-based music recognition tool that allows users to identify songs from audio input.
 Author: schuldt-ogre <nschuldt@ogre.run>
 Description-Content-Type: text/markdown
 Requires-Dist: aniso8601>=9.0.1
 Requires-Dist: audioread>=3.0.1
 Requires-Dist: blinker>=1.7.0
 Requires-Dist: certifi>=2024.2.2
@@ -92,21 +92,18 @@
 - Simple database for storing song information
 
 ## Installation
 To install FFTrack, follow these steps:
 1. Clone the repository to your local machine:
 2. Install the package using the following command:
 ```
-pip install .
+pip install fftrack
 ```
-3. Install the required dependencies using the following command:
-```
-pip install -r requirements.txt
-```
-4. Verify the installation by running the following command:
+
+3. Verify the installation by running the following command:
 ```
 fftrack --help
 ```
 
 ## Usage
 ### Database Setup
 To create the database, run the following command in your terminal:
@@ -128,14 +125,16 @@
 
 ## Configuration
 To configure FFTrack, run the following command in your terminal (not available yet):
 ```
 fftrack config
 ```
 
+
+
 [//]: # (## Contributing)
 
 [//]: # (If you want to contribute to this project, please follow these steps:)
 
 
 ## License
```

### Comparing `fftrack-0.1.8/fftrack.egg-info/SOURCES.txt` & `fftrack-0.2.0/fftrack.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -21,8 +21,11 @@
 fftrack/database/main_db.py
 fftrack/database/models.py
 fftrack/matching/__init__.py
 fftrack/matching/main_matching.py
 fftrack/matching/matcher.py
 fftrack/scripts/__init__.py
 fftrack/scripts/populate_database.py
-fftrack/scripts/songs_to_download.csv
+fftrack/scripts/songs_to_download.csv
+fftrack/ui/__init__.py
+fftrack/ui/cli.py
+fftrack/ui/main_cli.py
```

### Comparing `fftrack-0.1.8/fftrack.egg-info/requires.txt` & `fftrack-0.2.0/fftrack.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `fftrack-0.1.8/setup.py` & `fftrack-0.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='fftrack',
-    version='0.1.8',
+    version='0.2.0',
     description='FFTrack is a Python-based music recognition tool that allows users to identify songs from audio input.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='schuldt-ogre <nschuldt@ogre.run>',
     packages=find_packages(),
     package_data={
         'fftrack': ['config.json', 'scripts/*.csv'],
```

