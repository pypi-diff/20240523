# Comparing `tmp/TMDBTraktSyncer-1.6.4.tar.gz` & `tmp/tmdbtraktsyncer-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TMDBTraktSyncer-1.6.4.tar", last modified: Tue Nov 28 23:09:48 2023, max compression
+gzip compressed data, was "tmdbtraktsyncer-1.7.0.tar", last modified: Thu May 23 12:13:53 2024, max compression
```

## Comparing `TMDBTraktSyncer-1.6.4.tar` & `tmdbtraktsyncer-1.7.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-11-28 23:09:48.318930 TMDBTraktSyncer-1.6.4/
--rw-rw-rw-   0        0        0     1079 2023-05-21 01:51:26.000000 TMDBTraktSyncer-1.6.4/LICENSE
--rw-rw-rw-   0        0        0    11458 2023-11-28 23:09:48.316929 TMDBTraktSyncer-1.6.4/PKG-INFO
--rw-rw-rw-   0        0        0    10684 2023-09-30 06:54:24.000000 TMDBTraktSyncer-1.6.4/README.md
-drwxrwxrwx   0        0        0        0 2023-11-28 23:09:48.284929 TMDBTraktSyncer-1.6.4/TMDBTraktSyncer/
--rw-rw-rw-   0        0        0    18069 2023-07-31 05:41:54.000000 TMDBTraktSyncer-1.6.4/TMDBTraktSyncer/TMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-07-31 05:41:54.000000 TMDBTraktSyncer-1.6.4/TMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     6379 2023-11-09 08:07:17.000000 TMDBTraktSyncer-1.6.4/TMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0    10185 2023-11-09 06:21:42.000000 TMDBTraktSyncer-1.6.4/TMDBTraktSyncer/errorHandling.py
--rw-rw-rw-   0        0        0     1642 2023-11-28 22:57:57.000000 TMDBTraktSyncer-1.6.4/TMDBTraktSyncer/errorLogger.py
--rw-rw-rw-   0        0        0     4058 2023-11-08 13:56:56.000000 TMDBTraktSyncer-1.6.4/TMDBTraktSyncer/tmdbData.py
--rw-rw-rw-   0        0        0     7135 2023-10-13 00:03:27.000000 TMDBTraktSyncer-1.6.4/TMDBTraktSyncer/traktData.py
--rw-rw-rw-   0        0        0     9293 2023-11-09 06:27:14.000000 TMDBTraktSyncer-1.6.4/TMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-11-28 23:09:48.314930 TMDBTraktSyncer-1.6.4/TMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0    11458 2023-11-28 23:09:48.000000 TMDBTraktSyncer-1.6.4/TMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      512 2023-11-28 23:09:48.000000 TMDBTraktSyncer-1.6.4/TMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-28 23:09:48.000000 TMDBTraktSyncer-1.6.4/TMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-11-28 23:09:48.000000 TMDBTraktSyncer-1.6.4/TMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-11-28 23:09:48.000000 TMDBTraktSyncer-1.6.4/TMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-11-28 23:09:48.000000 TMDBTraktSyncer-1.6.4/TMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-11-28 23:09:48.318930 TMDBTraktSyncer-1.6.4/setup.cfg
--rw-rw-rw-   0        0        0     1341 2023-11-28 22:57:46.000000 TMDBTraktSyncer-1.6.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 12:13:53.680636 tmdbtraktsyncer-1.7.0/
+-rw-rw-rw-   0        0        0     1079 2023-05-21 01:51:26.000000 tmdbtraktsyncer-1.7.0/LICENSE
+-rw-rw-rw-   0        0        0    11457 2024-05-23 12:13:53.677636 tmdbtraktsyncer-1.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10683 2024-05-23 12:12:53.000000 tmdbtraktsyncer-1.7.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 12:13:53.645636 tmdbtraktsyncer-1.7.0/TMDBTraktSyncer/
+-rw-rw-rw-   0        0        0    18294 2024-05-23 11:44:31.000000 tmdbtraktsyncer-1.7.0/TMDBTraktSyncer/TMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-07-31 05:41:54.000000 tmdbtraktsyncer-1.7.0/TMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     6379 2023-11-09 08:07:17.000000 tmdbtraktsyncer-1.7.0/TMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0     1952 2024-05-23 11:39:00.000000 tmdbtraktsyncer-1.7.0/TMDBTraktSyncer/checkVersion.py
+-rw-rw-rw-   0        0        0    10185 2023-11-09 06:21:42.000000 tmdbtraktsyncer-1.7.0/TMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     1642 2023-11-28 22:57:57.000000 tmdbtraktsyncer-1.7.0/TMDBTraktSyncer/errorLogger.py
+-rw-rw-rw-   0        0        0     4058 2023-11-08 13:56:56.000000 tmdbtraktsyncer-1.7.0/TMDBTraktSyncer/tmdbData.py
+-rw-rw-rw-   0        0        0     7135 2023-10-13 00:03:27.000000 tmdbtraktsyncer-1.7.0/TMDBTraktSyncer/traktData.py
+-rw-rw-rw-   0        0        0     9367 2024-05-23 11:39:52.000000 tmdbtraktsyncer-1.7.0/TMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2024-05-23 12:13:53.676635 tmdbtraktsyncer-1.7.0/TMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0    11457 2024-05-23 12:13:53.000000 tmdbtraktsyncer-1.7.0/TMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      544 2024-05-23 12:13:53.000000 tmdbtraktsyncer-1.7.0/TMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 12:13:53.000000 tmdbtraktsyncer-1.7.0/TMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2024-05-23 12:13:53.000000 tmdbtraktsyncer-1.7.0/TMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2024-05-23 12:13:53.000000 tmdbtraktsyncer-1.7.0/TMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-23 12:13:53.000000 tmdbtraktsyncer-1.7.0/TMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 12:13:53.680636 tmdbtraktsyncer-1.7.0/setup.cfg
+-rw-rw-rw-   0        0        0     1341 2024-05-23 12:13:18.000000 tmdbtraktsyncer-1.7.0/setup.py
```

### Comparing `TMDBTraktSyncer-1.6.4/LICENSE` & `tmdbtraktsyncer-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.6.4/PKG-INFO` & `tmdbtraktsyncer-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TMDBTraktSyncer
-Version: 1.6.4
+Version: 1.7.0
 Summary: A python script that syncs user watchlist and ratings for Movies, TV Shows and Episodes both ways between Trakt and TMDB.
 Home-page: https://github.com/RileyXX/TMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,tmdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
@@ -80,16 +80,16 @@
 - Setup Automation for:
    - [Windows](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Windows)
    - [Linux](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Linux)
    - [macOS](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-macOS)
 - Python Script to Update all Packages with Pip (Windows, Linux, Mac, ChromeOS, etc.) [Link #1](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Python-Script-to-Update-all-Packages-with-Pip-\(Windows,-Linux,-Mac,-ChromeOS,-etc\))
 
 ## Troubleshooting, Known Issues, Workarounds & Future Outlook:
-* Add support for review/comment sync [Issue #1](https://github.com/RileyXX/TMDB-Trakt-Syncer/issues/1)
 * If any of your details change (passwords, logins, API keys, etc.), simply open `credentials.txt`, modify your details, save it and then run the script again. Alternatively, delete `credentials.txt` to reset the script and it will prompt you to enter your new details on the next run.
+* Add support for review/comment sync [Issue #1](https://github.com/RileyXX/TMDB-Trakt-Syncer/issues/1)
 
 ## Screenshot:
 ![Demo](https://i.imgur.com/5LI04O2.png)
 
 ## Sponsorships, Donations, and Custom Projects:
 If you find my scripts helpful, you can become a [sponsor](https://github.com/sponsors/RileyXX) and support my projects! If you need help with a project, open an issue, and I'll do my best to assist you. For other inquiries and custom projects, you can contact me on [Twitter](https://twitter.com/RileyxBell).
 
@@ -108,15 +108,15 @@
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 ## Other Recommended Projects:
 
 | Project Name | Description |
 |--------------|-------------|
 | [PlexTraktSync](https://github.com/Taxel/PlexTraktSync) | A script that syncs user watch history and ratings between Trakt and Plex (without needing a PlexPass or Trakt VIP subscription). |
-| [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer) | A script that syncs user watchlist, ratings, and comments both ways between Trakt and IMDB. |
+| [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer) | A script that syncs user watchlist, ratings, and reviews both ways between Trakt and IMDB. |
 | [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer) | A script that syncs user watchlist and ratings both ways between Trakt and TMDB. |
 | [PlexPreferNonForcedSubs](https://github.com/RileyXX/PlexPreferNonForcedSubs) | A script that sets all movies and shows in your local Plex library to English non-forced subtitles by default. |
 | [Casvt / AudioSubChanger](https://github.com/Casvt/Plex-scripts/blob/main/changing_settings/audio_sub_changer.py) | A script with advanced options for changing audio & subtitle tracks in Plex. |
 | [Casvt / PlexAutoDelete](https://github.com/Casvt/Plex-scripts/blob/main/changing_settings/plex_auto_delete.py) | A script for automatically deleting watched content from Plex. |
 | [universal-trakt-scrobbler](https://github.com/trakt-tools/universal-trakt-scrobbler) | An extension that automatically scrobbles TV shows and Movies from several streaming services to Trakt. |
 | [Netflix-to-Trakt-Import](https://github.com/jensb89/Netflix-to-Trakt-Import) | A tool to import your Netflix viewing history into Trakt. |
 | [trakt-tv-backup](https://darekkay.com/blog/trakt-tv-backup/) | A command-line tool for backing up your Trakt.tv data. |
```

### Comparing `TMDBTraktSyncer-1.6.4/README.md` & `tmdbtraktsyncer-1.7.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -63,16 +63,16 @@
 - Setup Automation for:
    - [Windows](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Windows)
    - [Linux](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Linux)
    - [macOS](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-macOS)
 - Python Script to Update all Packages with Pip (Windows, Linux, Mac, ChromeOS, etc.) [Link #1](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Python-Script-to-Update-all-Packages-with-Pip-\(Windows,-Linux,-Mac,-ChromeOS,-etc\))
 
 ## Troubleshooting, Known Issues, Workarounds & Future Outlook:
-* Add support for review/comment sync [Issue #1](https://github.com/RileyXX/TMDB-Trakt-Syncer/issues/1)
 * If any of your details change (passwords, logins, API keys, etc.), simply open `credentials.txt`, modify your details, save it and then run the script again. Alternatively, delete `credentials.txt` to reset the script and it will prompt you to enter your new details on the next run.
+* Add support for review/comment sync [Issue #1](https://github.com/RileyXX/TMDB-Trakt-Syncer/issues/1)
 
 ## Screenshot:
 ![Demo](https://i.imgur.com/5LI04O2.png)
 
 ## Sponsorships, Donations, and Custom Projects:
 If you find my scripts helpful, you can become a [sponsor](https://github.com/sponsors/RileyXX) and support my projects! If you need help with a project, open an issue, and I'll do my best to assist you. For other inquiries and custom projects, you can contact me on [Twitter](https://twitter.com/RileyxBell).
 
@@ -91,15 +91,15 @@
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 ## Other Recommended Projects:
 
 | Project Name | Description |
 |--------------|-------------|
 | [PlexTraktSync](https://github.com/Taxel/PlexTraktSync) | A script that syncs user watch history and ratings between Trakt and Plex (without needing a PlexPass or Trakt VIP subscription). |
-| [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer) | A script that syncs user watchlist, ratings, and comments both ways between Trakt and IMDB. |
+| [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer) | A script that syncs user watchlist, ratings, and reviews both ways between Trakt and IMDB. |
 | [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer) | A script that syncs user watchlist and ratings both ways between Trakt and TMDB. |
 | [PlexPreferNonForcedSubs](https://github.com/RileyXX/PlexPreferNonForcedSubs) | A script that sets all movies and shows in your local Plex library to English non-forced subtitles by default. |
 | [Casvt / AudioSubChanger](https://github.com/Casvt/Plex-scripts/blob/main/changing_settings/audio_sub_changer.py) | A script with advanced options for changing audio & subtitle tracks in Plex. |
 | [Casvt / PlexAutoDelete](https://github.com/Casvt/Plex-scripts/blob/main/changing_settings/plex_auto_delete.py) | A script for automatically deleting watched content from Plex. |
 | [universal-trakt-scrobbler](https://github.com/trakt-tools/universal-trakt-scrobbler) | An extension that automatically scrobbles TV shows and Movies from several streaming services to Trakt. |
 | [Netflix-to-Trakt-Import](https://github.com/jensb89/Netflix-to-Trakt-Import) | A tool to import your Netflix viewing history into Trakt. |
 | [trakt-tv-backup](https://darekkay.com/blog/trakt-tv-backup/) | A command-line tool for backing up your Trakt.tv data. |
```

### Comparing `TMDBTraktSyncer-1.6.4/TMDBTraktSyncer/TMDBTraktSyncer.py` & `tmdbtraktsyncer-1.7.0/TMDBTraktSyncer/TMDBTraktSyncer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-import json
-import requests
-import time
-try:
-    from TMDBTraktSyncer import verifyCredentials as VC
-    from TMDBTraktSyncer import traktData
-    from TMDBTraktSyncer import tmdbData
-    from TMDBTraktSyncer import errorHandling as EH
-    from TMDBTraktSyncer import errorLogger as EL
-except ImportError:
-    import verifyCredentials as VC
-    import traktData
-    import tmdbData
-    import errorHandling as EH
-    import errorLogger as EL
-
-
 def main():
+    print("Starting TMDBTraktSyncer....")
+    import json
+    import requests
+    import time
+    try:
+        from TMDBTraktSyncer import checkVersion
+        from TMDBTraktSyncer import verifyCredentials as VC
+        from TMDBTraktSyncer import traktData
+        from TMDBTraktSyncer import tmdbData
+        from TMDBTraktSyncer import errorHandling as EH
+        from TMDBTraktSyncer import errorLogger as EL
+    except ImportError:
+        import checkVersion
+        import verifyCredentials as VC
+        import traktData
+        import tmdbData
+        import errorHandling as EH
+        import errorLogger as EL
+
     try:
             
         trakt_watchlist, trakt_ratings, watched_content = traktData.getTraktData()
         tmdb_watchlist, tmdb_ratings = tmdbData.getTMDBRatings()
 
         #Get trakt and tmdb ratings and filter out trakt ratings with missing tmdb id
         trakt_ratings = [rating for rating in trakt_ratings if rating['TMDB_ID'] is not None]
@@ -345,14 +347,16 @@
                         print(f"   - {error_message}")
                         EL.logger.error(error_message)
 
                 
                 print('Removing Watched Items From TMDB Watchlist Complete')
             else:
                 print('No Watched Items To Remove From TMDB Watchlist')
+
+        print("TMDBTraktSyncer Complete")
         
     except Exception as e:
         error_message = "An error occurred while running the script."
         EH.report_error(error_message)
         EL.logger.error(error_message, exc_info=True)
 
 if __name__ == '__main__':
```

### Comparing `TMDBTraktSyncer-1.6.4/TMDBTraktSyncer/authTrakt.py` & `tmdbtraktsyncer-1.7.0/TMDBTraktSyncer/authTrakt.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.6.4/TMDBTraktSyncer/errorHandling.py` & `tmdbtraktsyncer-1.7.0/TMDBTraktSyncer/errorHandling.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.6.4/TMDBTraktSyncer/errorLogger.py` & `tmdbtraktsyncer-1.7.0/TMDBTraktSyncer/errorLogger.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.6.4/TMDBTraktSyncer/tmdbData.py` & `tmdbtraktsyncer-1.7.0/TMDBTraktSyncer/tmdbData.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.6.4/TMDBTraktSyncer/traktData.py` & `tmdbtraktsyncer-1.7.0/TMDBTraktSyncer/traktData.py`

 * *Files identical despite different names*

### Comparing `TMDBTraktSyncer-1.6.4/TMDBTraktSyncer/verifyCredentials.py` & `tmdbtraktsyncer-1.7.0/TMDBTraktSyncer/verifyCredentials.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     import authTrakt
     import errorLogger as EL
 
 def prompt_get_credentials():
     # Define the file path
     here = os.path.abspath(os.path.dirname(__file__))
     file_path = os.path.join(here, 'credentials.txt')
+    print(f"Your credentials and error log files are saved at:\n{here}")
 
     default_values = {
         "trakt_client_id": "empty",
         "trakt_client_secret": "empty",
         "trakt_access_token": "empty",
         "trakt_refresh_token": "empty",
         "tmdb_access_token": "empty",
```

### Comparing `TMDBTraktSyncer-1.6.4/TMDBTraktSyncer.egg-info/PKG-INFO` & `tmdbtraktsyncer-1.7.0/TMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TMDBTraktSyncer
-Version: 1.6.4
+Version: 1.7.0
 Summary: A python script that syncs user watchlist and ratings for Movies, TV Shows and Episodes both ways between Trakt and TMDB.
 Home-page: https://github.com/RileyXX/TMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,tmdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
@@ -80,16 +80,16 @@
 - Setup Automation for:
    - [Windows](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Windows)
    - [Linux](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Linux)
    - [macOS](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-macOS)
 - Python Script to Update all Packages with Pip (Windows, Linux, Mac, ChromeOS, etc.) [Link #1](https://github.com/RileyXX/TMDB-Trakt-Syncer/wiki/Python-Script-to-Update-all-Packages-with-Pip-\(Windows,-Linux,-Mac,-ChromeOS,-etc\))
 
 ## Troubleshooting, Known Issues, Workarounds & Future Outlook:
-* Add support for review/comment sync [Issue #1](https://github.com/RileyXX/TMDB-Trakt-Syncer/issues/1)
 * If any of your details change (passwords, logins, API keys, etc.), simply open `credentials.txt`, modify your details, save it and then run the script again. Alternatively, delete `credentials.txt` to reset the script and it will prompt you to enter your new details on the next run.
+* Add support for review/comment sync [Issue #1](https://github.com/RileyXX/TMDB-Trakt-Syncer/issues/1)
 
 ## Screenshot:
 ![Demo](https://i.imgur.com/5LI04O2.png)
 
 ## Sponsorships, Donations, and Custom Projects:
 If you find my scripts helpful, you can become a [sponsor](https://github.com/sponsors/RileyXX) and support my projects! If you need help with a project, open an issue, and I'll do my best to assist you. For other inquiries and custom projects, you can contact me on [Twitter](https://twitter.com/RileyxBell).
 
@@ -108,15 +108,15 @@
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 ## Other Recommended Projects:
 
 | Project Name | Description |
 |--------------|-------------|
 | [PlexTraktSync](https://github.com/Taxel/PlexTraktSync) | A script that syncs user watch history and ratings between Trakt and Plex (without needing a PlexPass or Trakt VIP subscription). |
-| [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer) | A script that syncs user watchlist, ratings, and comments both ways between Trakt and IMDB. |
+| [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer) | A script that syncs user watchlist, ratings, and reviews both ways between Trakt and IMDB. |
 | [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer) | A script that syncs user watchlist and ratings both ways between Trakt and TMDB. |
 | [PlexPreferNonForcedSubs](https://github.com/RileyXX/PlexPreferNonForcedSubs) | A script that sets all movies and shows in your local Plex library to English non-forced subtitles by default. |
 | [Casvt / AudioSubChanger](https://github.com/Casvt/Plex-scripts/blob/main/changing_settings/audio_sub_changer.py) | A script with advanced options for changing audio & subtitle tracks in Plex. |
 | [Casvt / PlexAutoDelete](https://github.com/Casvt/Plex-scripts/blob/main/changing_settings/plex_auto_delete.py) | A script for automatically deleting watched content from Plex. |
 | [universal-trakt-scrobbler](https://github.com/trakt-tools/universal-trakt-scrobbler) | An extension that automatically scrobbles TV shows and Movies from several streaming services to Trakt. |
 | [Netflix-to-Trakt-Import](https://github.com/jensb89/Netflix-to-Trakt-Import) | A tool to import your Netflix viewing history into Trakt. |
 | [trakt-tv-backup](https://darekkay.com/blog/trakt-tv-backup/) | A command-line tool for backing up your Trakt.tv data. |
```

### Comparing `TMDBTraktSyncer-1.6.4/TMDBTraktSyncer.egg-info/SOURCES.txt` & `tmdbtraktsyncer-1.7.0/TMDBTraktSyncer.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 setup.py
 TMDBTraktSyncer/TMDBTraktSyncer.py
 TMDBTraktSyncer/__init__.py
 TMDBTraktSyncer/authTrakt.py
+TMDBTraktSyncer/checkVersion.py
 TMDBTraktSyncer/errorHandling.py
 TMDBTraktSyncer/errorLogger.py
 TMDBTraktSyncer/tmdbData.py
 TMDBTraktSyncer/traktData.py
 TMDBTraktSyncer/verifyCredentials.py
 TMDBTraktSyncer.egg-info/PKG-INFO
 TMDBTraktSyncer.egg-info/SOURCES.txt
```

### Comparing `TMDBTraktSyncer-1.6.4/setup.py` & `tmdbtraktsyncer-1.7.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), 'r', encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.6.4'
+VERSION = '1.7.0'
 DESCRIPTION = 'A python script that syncs user watchlist and ratings for Movies, TV Shows and Episodes both ways between Trakt and TMDB.'
 
 # Setting up
 setup(
     name="TMDBTraktSyncer",
     version=VERSION,
     author="RileyXX",
```

