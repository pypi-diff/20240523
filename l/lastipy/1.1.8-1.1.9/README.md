# Comparing `tmp/lastipy-1.1.8.tar.gz` & `tmp/lastipy-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lastipy-1.1.8.tar", last modified: Tue May 11 14:31:29 2021, max compression
+gzip compressed data, was "dist/lastipy-1.1.9.tar", last modified: Wed May 12 15:13:11 2021, max compression
```

## Comparing `lastipy-1.1.8.tar` & `lastipy-1.1.9.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 jenkins    (118) jenkins    (123)        0 2021-05-11 14:31:29.088643 lastipy-1.1.8/
--rw-r--r--   0 jenkins    (118) jenkins    (123)      281 2021-05-11 14:31:29.088643 lastipy-1.1.8/PKG-INFO
--rw-r--r--   0 jenkins    (118) jenkins    (123)     2044 2021-05-11 14:31:12.000000 lastipy-1.1.8/README.md
-drwxr-xr-x   0 jenkins    (118) jenkins    (123)        0 2021-05-11 14:31:29.084643 lastipy-1.1.8/lastipy/
--rw-r--r--   0 jenkins    (118) jenkins    (123)        0 2021-05-11 14:31:12.000000 lastipy-1.1.8/lastipy/__init__.py
--rw-r--r--   0 jenkins    (118) jenkins    (123)       65 2021-05-11 14:31:12.000000 lastipy-1.1.8/lastipy/definitions.py
-drwxr-xr-x   0 jenkins    (118) jenkins    (123)        0 2021-05-11 14:31:29.084643 lastipy-1.1.8/lastipy/lastfm/
--rw-r--r--   0 jenkins    (118) jenkins    (123)        0 2021-05-11 14:31:12.000000 lastipy-1.1.8/lastipy/lastfm/__init__.py
--rw-r--r--   0 jenkins    (118) jenkins    (123)     1639 2021-05-11 14:31:12.000000 lastipy-1.1.8/lastipy/lastfm/lastfm_recommendations.py
-drwxr-xr-x   0 jenkins    (118) jenkins    (123)        0 2021-05-11 14:31:29.084643 lastipy-1.1.8/lastipy/lastfm/library/
--rw-r--r--   0 jenkins    (118) jenkins    (123)        0 2021-05-11 14:31:12.000000 lastipy-1.1.8/lastipy/lastfm/library/__init__.py
--rw-r--r--   0 jenkins    (118) jenkins    (123)     2137 2021-05-11 14:31:12.000000 lastipy-1.1.8/lastipy/lastfm/library/paginated_endpoint.py
--rw-r--r--   0 jenkins    (118) jenkins    (123)      194 2021-05-11 14:31:12.000000 lastipy-1.1.8/lastipy/lastfm/library/period.py
--rw-r--r--   0 jenkins    (118) jenkins    (123)     1286 2021-05-11 14:31:12.000000 lastipy-1.1.8/lastipy/lastfm/library/recent_artists.py
--rw-r--r--   0 jenkins    (118) jenkins    (123)      923 2021-05-11 14:31:12.000000 lastipy-1.1.8/lastipy/lastfm/library/recent_tracks.py
--rw-r--r--   0 jenkins    (118) jenkins    (123)      500 2021-05-11 14:31:12.000000 lastipy-1.1.8/lastipy/lastfm/library/scrobbled_artist.py
--rw-r--r--   0 jenkins    (118) jenkins    (123)      659 2021-05-11 14:31:12.000000 lastipy-1.1.8/lastipy/lastfm/library/top_track.py
--rw-r--r--   0 jenkins    (118) jenkins    (123)     1291 2021-05-11 14:31:12.000000 lastipy-1.1.8/lastipy/lastfm/library/top_tracks.py
--rw-r--r--   0 jenkins    (118) jenkins    (123)     1518 2021-05-11 14:31:12.000000 lastipy-1.1.8/lastipy/lastfm/library/track_info.py
--rw-r--r--   0 jenkins    (118) jenkins    (123)      290 2021-05-11 14:31:12.000000 lastipy-1.1.8/lastipy/lastfm/parse_lastfm_tracks.py
-drwxr-xr-x   0 jenkins    (118) jenkins    (123)        0 2021-05-11 14:31:29.084643 lastipy-1.1.8/lastipy/recommendations/
--rw-r--r--   0 jenkins    (118) jenkins    (123)        0 2021-05-11 14:31:12.000000 lastipy-1.1.8/lastipy/recommendations/__init__.py
--rw-r--r--   0 jenkins    (118) jenkins    (123)     2708 2021-05-11 14:31:12.000000 lastipy-1.1.8/lastipy/recommendations/rating_calculator.py
--rw-r--r--   0 jenkins    (118) jenkins    (123)     3930 2021-05-11 14:31:12.000000 lastipy-1.1.8/lastipy/recommendations/recommendations.py
--rw-r--r--   0 jenkins    (118) jenkins    (123)      853 2021-05-11 14:31:12.000000 lastipy-1.1.8/lastipy/recommendations/recommended_track.py
-drwxr-xr-x   0 jenkins    (118) jenkins    (123)        0 2021-05-11 14:31:29.088643 lastipy-1.1.8/lastipy/spotify/
--rw-r--r--   0 jenkins    (118) jenkins    (123)        0 2021-05-11 14:31:12.000000 lastipy-1.1.8/lastipy/spotify/__init__.py
--rw-r--r--   0 jenkins    (118) jenkins    (123)      862 2021-05-11 14:31:12.000000 lastipy-1.1.8/lastipy/spotify/album.py
--rw-r--r--   0 jenkins    (118) jenkins    (123)     2485 2021-05-11 14:31:12.000000 lastipy-1.1.8/lastipy/spotify/library.py
--rw-r--r--   0 jenkins    (118) jenkins    (123)     6622 2021-05-11 14:31:12.000000 lastipy-1.1.8/lastipy/spotify/new_releases.py
--rw-r--r--   0 jenkins    (118) jenkins    (123)      851 2021-05-11 14:31:12.000000 lastipy-1.1.8/lastipy/spotify/parse_spotify_tracks.py
--rw-r--r--   0 jenkins    (118) jenkins    (123)     5476 2021-05-11 14:31:12.000000 lastipy-1.1.8/lastipy/spotify/playlist.py
--rw-r--r--   0 jenkins    (118) jenkins    (123)      659 2021-05-11 14:31:12.000000 lastipy-1.1.8/lastipy/spotify/playlist_track.py
--rw-r--r--   0 jenkins    (118) jenkins    (123)      777 2021-05-11 14:31:12.000000 lastipy-1.1.8/lastipy/spotify/search.py
--rw-r--r--   0 jenkins    (118) jenkins    (123)     1052 2021-05-11 14:31:12.000000 lastipy-1.1.8/lastipy/spotify/spotify_recommendations.py
--rw-r--r--   0 jenkins    (118) jenkins    (123)     1972 2021-05-11 14:31:12.000000 lastipy-1.1.8/lastipy/spotify/token.py
--rw-r--r--   0 jenkins    (118) jenkins    (123)      806 2021-05-11 14:31:12.000000 lastipy-1.1.8/lastipy/track.py
-drwxr-xr-x   0 jenkins    (118) jenkins    (123)        0 2021-05-11 14:31:29.088643 lastipy-1.1.8/lastipy/util/
--rw-r--r--   0 jenkins    (118) jenkins    (123)        0 2021-05-11 14:31:12.000000 lastipy-1.1.8/lastipy/util/__init__.py
--rw-r--r--   0 jenkins    (118) jenkins    (123)      517 2021-05-11 14:31:12.000000 lastipy-1.1.8/lastipy/util/parse_api_keys.py
--rw-r--r--   0 jenkins    (118) jenkins    (123)      896 2021-05-11 14:31:12.000000 lastipy-1.1.8/lastipy/util/setup_logging.py
-drwxr-xr-x   0 jenkins    (118) jenkins    (123)        0 2021-05-11 14:31:29.084643 lastipy-1.1.8/lastipy.egg-info/
--rw-r--r--   0 jenkins    (118) jenkins    (123)      281 2021-05-11 14:31:29.000000 lastipy-1.1.8/lastipy.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (118) jenkins    (123)     2073 2021-05-11 14:31:29.000000 lastipy-1.1.8/lastipy.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (118) jenkins    (123)        1 2021-05-11 14:31:29.000000 lastipy-1.1.8/lastipy.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (118) jenkins    (123)      241 2021-05-11 14:31:29.000000 lastipy-1.1.8/lastipy.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (118) jenkins    (123)       54 2021-05-11 14:31:29.000000 lastipy-1.1.8/lastipy.egg-info/requires.txt
--rw-r--r--   0 jenkins    (118) jenkins    (123)       21 2021-05-11 14:31:29.000000 lastipy-1.1.8/lastipy.egg-info/top_level.txt
-drwxr-xr-x   0 jenkins    (118) jenkins    (123)        0 2021-05-11 14:31:29.088643 lastipy-1.1.8/scripts/
--rw-r--r--   0 jenkins    (118) jenkins    (123)        0 2021-05-11 14:31:12.000000 lastipy-1.1.8/scripts/__init__.py
--rw-r--r--   0 jenkins    (118) jenkins    (123)     6048 2021-05-11 14:31:12.000000 lastipy-1.1.8/scripts/organize_favorites.py
--rw-r--r--   0 jenkins    (118) jenkins    (123)     5706 2021-05-11 14:31:12.000000 lastipy-1.1.8/scripts/recommendations_playlist.py
--rw-r--r--   0 jenkins    (118) jenkins    (123)     3352 2021-05-11 14:31:12.000000 lastipy-1.1.8/scripts/save_new_releases.py
--rw-r--r--   0 jenkins    (118) jenkins    (123)       38 2021-05-11 14:31:29.088643 lastipy-1.1.8/setup.cfg
--rw-r--r--   0 jenkins    (118) jenkins    (123)      734 2021-05-11 14:31:21.000000 lastipy-1.1.8/setup.py
-drwxr-xr-x   0 jenkins    (118) jenkins    (123)        0 2021-05-11 14:31:29.088643 lastipy-1.1.8/test/
--rw-r--r--   0 jenkins    (118) jenkins    (123)        0 2021-05-11 14:31:12.000000 lastipy-1.1.8/test/__init__.py
-drwxr-xr-x   0 jenkins    (118) jenkins    (123)        0 2021-05-11 14:31:29.088643 lastipy-1.1.8/test/lastfm/
--rw-r--r--   0 jenkins    (118) jenkins    (123)       53 2021-05-11 14:31:12.000000 lastipy-1.1.8/test/lastfm/__init__.py
-drwxr-xr-x   0 jenkins    (118) jenkins    (123)        0 2021-05-11 14:31:29.088643 lastipy-1.1.8/test/lastfm/library/
--rw-r--r--   0 jenkins    (118) jenkins    (123)        0 2021-05-11 14:31:12.000000 lastipy-1.1.8/test/lastfm/library/__init__.py
--rw-r--r--   0 jenkins    (118) jenkins    (123)     2272 2021-05-11 14:31:12.000000 lastipy-1.1.8/test/lastfm/library/test_fetch_playcount.py
--rw-r--r--   0 jenkins    (118) jenkins    (123)     6917 2021-05-11 14:31:12.000000 lastipy-1.1.8/test/lastfm/library/test_paginated_endpoint.py
--rw-r--r--   0 jenkins    (118) jenkins    (123)     1862 2021-05-11 14:31:12.000000 lastipy-1.1.8/test/lastfm/library/test_recent_artists.py
--rw-r--r--   0 jenkins    (118) jenkins    (123)     2067 2021-05-11 14:31:12.000000 lastipy-1.1.8/test/lastfm/library/test_recent_tracks.py
--rw-r--r--   0 jenkins    (118) jenkins    (123)     2651 2021-05-11 14:31:12.000000 lastipy-1.1.8/test/lastfm/library/test_top_tracks.py
--rw-r--r--   0 jenkins    (118) jenkins    (123)     1524 2021-05-11 14:31:12.000000 lastipy-1.1.8/test/lastfm/test_lastfm_recommendations.py
--rw-r--r--   0 jenkins    (118) jenkins    (123)      918 2021-05-11 14:31:12.000000 lastipy-1.1.8/test/lastfm/test_parse_lastfm_tracks.py
-drwxr-xr-x   0 jenkins    (118) jenkins    (123)        0 2021-05-11 14:31:29.088643 lastipy-1.1.8/test/recommendations/
--rw-r--r--   0 jenkins    (118) jenkins    (123)        0 2021-05-11 14:31:12.000000 lastipy-1.1.8/test/recommendations/__init__.py
--rw-r--r--   0 jenkins    (118) jenkins    (123)     4470 2021-05-11 14:31:12.000000 lastipy-1.1.8/test/recommendations/test_generate_recommendations.py
--rw-r--r--   0 jenkins    (118) jenkins    (123)     7445 2021-05-11 14:31:12.000000 lastipy-1.1.8/test/recommendations/test_rating_calculator.py
-drwxr-xr-x   0 jenkins    (118) jenkins    (123)        0 2021-05-11 14:31:29.088643 lastipy-1.1.8/test/spotify/
--rw-r--r--   0 jenkins    (118) jenkins    (123)        0 2021-05-11 14:31:12.000000 lastipy-1.1.8/test/spotify/__init__.py
--rw-r--r--   0 jenkins    (118) jenkins    (123)     1640 2021-05-11 14:31:12.000000 lastipy-1.1.8/test/spotify/test_add_albums_to_library.py
--rw-r--r--   0 jenkins    (118) jenkins    (123)     1602 2021-05-11 14:31:12.000000 lastipy-1.1.8/test/spotify/test_add_tracks_to_library.py
--rw-r--r--   0 jenkins    (118) jenkins    (123)     2657 2021-05-11 14:31:12.000000 lastipy-1.1.8/test/spotify/test_get_saved_tracks.py
--rw-r--r--   0 jenkins    (118) jenkins    (123)     1274 2021-05-11 14:31:12.000000 lastipy-1.1.8/test/test_requests.py
+drwxr-xr-x   0 jenkins    (118) jenkins    (123)        0 2021-05-12 15:13:11.685904 lastipy-1.1.9/
+-rw-r--r--   0 jenkins    (118) jenkins    (123)      281 2021-05-12 15:13:11.685904 lastipy-1.1.9/PKG-INFO
+-rw-r--r--   0 jenkins    (118) jenkins    (123)     2044 2021-05-12 15:12:54.000000 lastipy-1.1.9/README.md
+drwxr-xr-x   0 jenkins    (118) jenkins    (123)        0 2021-05-12 15:13:11.681904 lastipy-1.1.9/lastipy/
+-rw-r--r--   0 jenkins    (118) jenkins    (123)        0 2021-05-12 15:12:54.000000 lastipy-1.1.9/lastipy/__init__.py
+-rw-r--r--   0 jenkins    (118) jenkins    (123)       65 2021-05-12 15:12:54.000000 lastipy-1.1.9/lastipy/definitions.py
+drwxr-xr-x   0 jenkins    (118) jenkins    (123)        0 2021-05-12 15:13:11.685904 lastipy-1.1.9/lastipy/lastfm/
+-rw-r--r--   0 jenkins    (118) jenkins    (123)        0 2021-05-12 15:12:54.000000 lastipy-1.1.9/lastipy/lastfm/__init__.py
+-rw-r--r--   0 jenkins    (118) jenkins    (123)     1639 2021-05-12 15:12:54.000000 lastipy-1.1.9/lastipy/lastfm/lastfm_recommendations.py
+drwxr-xr-x   0 jenkins    (118) jenkins    (123)        0 2021-05-12 15:13:11.685904 lastipy-1.1.9/lastipy/lastfm/library/
+-rw-r--r--   0 jenkins    (118) jenkins    (123)        0 2021-05-12 15:12:54.000000 lastipy-1.1.9/lastipy/lastfm/library/__init__.py
+-rw-r--r--   0 jenkins    (118) jenkins    (123)     2137 2021-05-12 15:12:54.000000 lastipy-1.1.9/lastipy/lastfm/library/paginated_endpoint.py
+-rw-r--r--   0 jenkins    (118) jenkins    (123)      194 2021-05-12 15:12:54.000000 lastipy-1.1.9/lastipy/lastfm/library/period.py
+-rw-r--r--   0 jenkins    (118) jenkins    (123)     1286 2021-05-12 15:12:54.000000 lastipy-1.1.9/lastipy/lastfm/library/recent_artists.py
+-rw-r--r--   0 jenkins    (118) jenkins    (123)      923 2021-05-12 15:12:54.000000 lastipy-1.1.9/lastipy/lastfm/library/recent_tracks.py
+-rw-r--r--   0 jenkins    (118) jenkins    (123)      500 2021-05-12 15:12:54.000000 lastipy-1.1.9/lastipy/lastfm/library/scrobbled_artist.py
+-rw-r--r--   0 jenkins    (118) jenkins    (123)      659 2021-05-12 15:12:54.000000 lastipy-1.1.9/lastipy/lastfm/library/top_track.py
+-rw-r--r--   0 jenkins    (118) jenkins    (123)     1291 2021-05-12 15:12:54.000000 lastipy-1.1.9/lastipy/lastfm/library/top_tracks.py
+-rw-r--r--   0 jenkins    (118) jenkins    (123)     1518 2021-05-12 15:12:54.000000 lastipy-1.1.9/lastipy/lastfm/library/track_info.py
+-rw-r--r--   0 jenkins    (118) jenkins    (123)      290 2021-05-12 15:12:54.000000 lastipy-1.1.9/lastipy/lastfm/parse_lastfm_tracks.py
+drwxr-xr-x   0 jenkins    (118) jenkins    (123)        0 2021-05-12 15:13:11.685904 lastipy-1.1.9/lastipy/recommendations/
+-rw-r--r--   0 jenkins    (118) jenkins    (123)        0 2021-05-12 15:12:54.000000 lastipy-1.1.9/lastipy/recommendations/__init__.py
+-rw-r--r--   0 jenkins    (118) jenkins    (123)     2708 2021-05-12 15:12:54.000000 lastipy-1.1.9/lastipy/recommendations/rating_calculator.py
+-rw-r--r--   0 jenkins    (118) jenkins    (123)     3930 2021-05-12 15:12:54.000000 lastipy-1.1.9/lastipy/recommendations/recommendations.py
+-rw-r--r--   0 jenkins    (118) jenkins    (123)      853 2021-05-12 15:12:54.000000 lastipy-1.1.9/lastipy/recommendations/recommended_track.py
+drwxr-xr-x   0 jenkins    (118) jenkins    (123)        0 2021-05-12 15:13:11.685904 lastipy-1.1.9/lastipy/spotify/
+-rw-r--r--   0 jenkins    (118) jenkins    (123)        0 2021-05-12 15:12:54.000000 lastipy-1.1.9/lastipy/spotify/__init__.py
+-rw-r--r--   0 jenkins    (118) jenkins    (123)      862 2021-05-12 15:12:54.000000 lastipy-1.1.9/lastipy/spotify/album.py
+-rw-r--r--   0 jenkins    (118) jenkins    (123)     2485 2021-05-12 15:12:54.000000 lastipy-1.1.9/lastipy/spotify/library.py
+-rw-r--r--   0 jenkins    (118) jenkins    (123)     6090 2021-05-12 15:12:54.000000 lastipy-1.1.9/lastipy/spotify/new_releases.py
+-rw-r--r--   0 jenkins    (118) jenkins    (123)      851 2021-05-12 15:12:54.000000 lastipy-1.1.9/lastipy/spotify/parse_spotify_tracks.py
+-rw-r--r--   0 jenkins    (118) jenkins    (123)     5476 2021-05-12 15:12:54.000000 lastipy-1.1.9/lastipy/spotify/playlist.py
+-rw-r--r--   0 jenkins    (118) jenkins    (123)      659 2021-05-12 15:12:54.000000 lastipy-1.1.9/lastipy/spotify/playlist_track.py
+-rw-r--r--   0 jenkins    (118) jenkins    (123)      777 2021-05-12 15:12:54.000000 lastipy-1.1.9/lastipy/spotify/search.py
+-rw-r--r--   0 jenkins    (118) jenkins    (123)     1052 2021-05-12 15:12:54.000000 lastipy-1.1.9/lastipy/spotify/spotify_recommendations.py
+-rw-r--r--   0 jenkins    (118) jenkins    (123)     1972 2021-05-12 15:12:54.000000 lastipy-1.1.9/lastipy/spotify/token.py
+-rw-r--r--   0 jenkins    (118) jenkins    (123)      806 2021-05-12 15:12:54.000000 lastipy-1.1.9/lastipy/track.py
+drwxr-xr-x   0 jenkins    (118) jenkins    (123)        0 2021-05-12 15:13:11.685904 lastipy-1.1.9/lastipy/util/
+-rw-r--r--   0 jenkins    (118) jenkins    (123)        0 2021-05-12 15:12:54.000000 lastipy-1.1.9/lastipy/util/__init__.py
+-rw-r--r--   0 jenkins    (118) jenkins    (123)      517 2021-05-12 15:12:54.000000 lastipy-1.1.9/lastipy/util/parse_api_keys.py
+-rw-r--r--   0 jenkins    (118) jenkins    (123)      896 2021-05-12 15:12:54.000000 lastipy-1.1.9/lastipy/util/setup_logging.py
+drwxr-xr-x   0 jenkins    (118) jenkins    (123)        0 2021-05-12 15:13:11.685904 lastipy-1.1.9/lastipy.egg-info/
+-rw-r--r--   0 jenkins    (118) jenkins    (123)      281 2021-05-12 15:13:11.000000 lastipy-1.1.9/lastipy.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (118) jenkins    (123)     2073 2021-05-12 15:13:11.000000 lastipy-1.1.9/lastipy.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (118) jenkins    (123)        1 2021-05-12 15:13:11.000000 lastipy-1.1.9/lastipy.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (118) jenkins    (123)      241 2021-05-12 15:13:11.000000 lastipy-1.1.9/lastipy.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (118) jenkins    (123)       54 2021-05-12 15:13:11.000000 lastipy-1.1.9/lastipy.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (118) jenkins    (123)       21 2021-05-12 15:13:11.000000 lastipy-1.1.9/lastipy.egg-info/top_level.txt
+drwxr-xr-x   0 jenkins    (118) jenkins    (123)        0 2021-05-12 15:13:11.685904 lastipy-1.1.9/scripts/
+-rw-r--r--   0 jenkins    (118) jenkins    (123)        0 2021-05-12 15:12:54.000000 lastipy-1.1.9/scripts/__init__.py
+-rw-r--r--   0 jenkins    (118) jenkins    (123)     5816 2021-05-12 15:12:54.000000 lastipy-1.1.9/scripts/organize_favorites.py
+-rw-r--r--   0 jenkins    (118) jenkins    (123)     5706 2021-05-12 15:12:54.000000 lastipy-1.1.9/scripts/recommendations_playlist.py
+-rw-r--r--   0 jenkins    (118) jenkins    (123)     3189 2021-05-12 15:12:54.000000 lastipy-1.1.9/scripts/save_new_releases.py
+-rw-r--r--   0 jenkins    (118) jenkins    (123)       38 2021-05-12 15:13:11.685904 lastipy-1.1.9/setup.cfg
+-rw-r--r--   0 jenkins    (118) jenkins    (123)      734 2021-05-12 15:13:03.000000 lastipy-1.1.9/setup.py
+drwxr-xr-x   0 jenkins    (118) jenkins    (123)        0 2021-05-12 15:13:11.685904 lastipy-1.1.9/test/
+-rw-r--r--   0 jenkins    (118) jenkins    (123)        0 2021-05-12 15:12:54.000000 lastipy-1.1.9/test/__init__.py
+drwxr-xr-x   0 jenkins    (118) jenkins    (123)        0 2021-05-12 15:13:11.685904 lastipy-1.1.9/test/lastfm/
+-rw-r--r--   0 jenkins    (118) jenkins    (123)       53 2021-05-12 15:12:54.000000 lastipy-1.1.9/test/lastfm/__init__.py
+drwxr-xr-x   0 jenkins    (118) jenkins    (123)        0 2021-05-12 15:13:11.685904 lastipy-1.1.9/test/lastfm/library/
+-rw-r--r--   0 jenkins    (118) jenkins    (123)        0 2021-05-12 15:12:54.000000 lastipy-1.1.9/test/lastfm/library/__init__.py
+-rw-r--r--   0 jenkins    (118) jenkins    (123)     2272 2021-05-12 15:12:54.000000 lastipy-1.1.9/test/lastfm/library/test_fetch_playcount.py
+-rw-r--r--   0 jenkins    (118) jenkins    (123)     6917 2021-05-12 15:12:54.000000 lastipy-1.1.9/test/lastfm/library/test_paginated_endpoint.py
+-rw-r--r--   0 jenkins    (118) jenkins    (123)     1862 2021-05-12 15:12:54.000000 lastipy-1.1.9/test/lastfm/library/test_recent_artists.py
+-rw-r--r--   0 jenkins    (118) jenkins    (123)     2067 2021-05-12 15:12:54.000000 lastipy-1.1.9/test/lastfm/library/test_recent_tracks.py
+-rw-r--r--   0 jenkins    (118) jenkins    (123)     2651 2021-05-12 15:12:54.000000 lastipy-1.1.9/test/lastfm/library/test_top_tracks.py
+-rw-r--r--   0 jenkins    (118) jenkins    (123)     1524 2021-05-12 15:12:54.000000 lastipy-1.1.9/test/lastfm/test_lastfm_recommendations.py
+-rw-r--r--   0 jenkins    (118) jenkins    (123)      918 2021-05-12 15:12:54.000000 lastipy-1.1.9/test/lastfm/test_parse_lastfm_tracks.py
+drwxr-xr-x   0 jenkins    (118) jenkins    (123)        0 2021-05-12 15:13:11.685904 lastipy-1.1.9/test/recommendations/
+-rw-r--r--   0 jenkins    (118) jenkins    (123)        0 2021-05-12 15:12:54.000000 lastipy-1.1.9/test/recommendations/__init__.py
+-rw-r--r--   0 jenkins    (118) jenkins    (123)     4470 2021-05-12 15:12:54.000000 lastipy-1.1.9/test/recommendations/test_generate_recommendations.py
+-rw-r--r--   0 jenkins    (118) jenkins    (123)     7445 2021-05-12 15:12:54.000000 lastipy-1.1.9/test/recommendations/test_rating_calculator.py
+drwxr-xr-x   0 jenkins    (118) jenkins    (123)        0 2021-05-12 15:13:11.685904 lastipy-1.1.9/test/spotify/
+-rw-r--r--   0 jenkins    (118) jenkins    (123)        0 2021-05-12 15:12:54.000000 lastipy-1.1.9/test/spotify/__init__.py
+-rw-r--r--   0 jenkins    (118) jenkins    (123)     1640 2021-05-12 15:12:54.000000 lastipy-1.1.9/test/spotify/test_add_albums_to_library.py
+-rw-r--r--   0 jenkins    (118) jenkins    (123)     1602 2021-05-12 15:12:54.000000 lastipy-1.1.9/test/spotify/test_add_tracks_to_library.py
+-rw-r--r--   0 jenkins    (118) jenkins    (123)     2657 2021-05-12 15:12:54.000000 lastipy-1.1.9/test/spotify/test_get_saved_tracks.py
+-rw-r--r--   0 jenkins    (118) jenkins    (123)     1274 2021-05-12 15:12:54.000000 lastipy-1.1.9/test/test_requests.py
```

### Comparing `lastipy-1.1.8/README.md` & `lastipy-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `lastipy-1.1.8/lastipy/lastfm/lastfm_recommendations.py` & `lastipy-1.1.9/lastipy/lastfm/lastfm_recommendations.py`

 * *Files identical despite different names*

### Comparing `lastipy-1.1.8/lastipy/lastfm/library/paginated_endpoint.py` & `lastipy-1.1.9/lastipy/lastfm/library/paginated_endpoint.py`

 * *Files identical despite different names*

### Comparing `lastipy-1.1.8/lastipy/lastfm/library/recent_artists.py` & `lastipy-1.1.9/lastipy/lastfm/library/recent_artists.py`

 * *Files identical despite different names*

### Comparing `lastipy-1.1.8/lastipy/lastfm/library/recent_tracks.py` & `lastipy-1.1.9/lastipy/lastfm/library/recent_tracks.py`

 * *Files identical despite different names*

### Comparing `lastipy-1.1.8/lastipy/lastfm/library/top_track.py` & `lastipy-1.1.9/lastipy/lastfm/library/top_track.py`

 * *Files identical despite different names*

### Comparing `lastipy-1.1.8/lastipy/lastfm/library/top_tracks.py` & `lastipy-1.1.9/lastipy/lastfm/library/top_tracks.py`

 * *Files identical despite different names*

### Comparing `lastipy-1.1.8/lastipy/lastfm/library/track_info.py` & `lastipy-1.1.9/lastipy/lastfm/library/track_info.py`

 * *Files identical despite different names*

### Comparing `lastipy-1.1.8/lastipy/recommendations/rating_calculator.py` & `lastipy-1.1.9/lastipy/recommendations/rating_calculator.py`

 * *Files identical despite different names*

### Comparing `lastipy-1.1.8/lastipy/recommendations/recommendations.py` & `lastipy-1.1.9/lastipy/recommendations/recommendations.py`

 * *Files identical despite different names*

### Comparing `lastipy-1.1.8/lastipy/recommendations/recommended_track.py` & `lastipy-1.1.9/lastipy/recommendations/recommended_track.py`

 * *Files identical despite different names*

### Comparing `lastipy-1.1.8/lastipy/spotify/album.py` & `lastipy-1.1.9/lastipy/spotify/album.py`

 * *Files identical despite different names*

### Comparing `lastipy-1.1.8/lastipy/spotify/library.py` & `lastipy-1.1.9/lastipy/spotify/library.py`

 * *Files identical despite different names*

### Comparing `lastipy-1.1.8/lastipy/spotify/new_releases.py` & `lastipy-1.1.9/lastipy/spotify/new_releases.py`

 * *Files 7% similar despite different names*

```diff
@@ -93,36 +93,24 @@
         else:
             logging.warn(
                 "Album release date precision is not 'day' so ignoring (album: " + str(album) + ")")
     return new_albums
 
 
 def _fetch_artist_albums(spotify, album_types, artist_id):
-    # TODO definitely need to extract something here...
     albums = []
-    if album.ALBUM_ALBUM_TYPE in album_types:
+    for album_type in album_types:
         curr_response = spotify.artist_albums(
-            artist_id, album_type='album', limit=50)
-        albums = _convert_albums(curr_response, 'album')
+            artist_id, album_type=album_type, limit=50)
+        albums = _convert_albums(curr_response, album_type)
         while len(curr_response['items']) > 0:
             curr_response = spotify.artist_albums(
-                artist_id, album_type='album', limit=50, offset=len(albums))
-            albums += _convert_albums(curr_response, 'album')
-
-    singles = []
-    if album.SINGLE_ALBUM_TYPE in album_types:
-        curr_response = spotify.artist_albums(
-            artist_id, album_type='single', limit=50)
-        singles = _convert_albums(curr_response, 'single')
-        while len(curr_response['items']) > 0:
-            curr_response = spotify.artist_albums(
-                artist_id, album_type='single', limit=50, offset=len(singles))
-            singles += _convert_albums(curr_response, 'single')
-
-    return albums + singles
+                artist_id, album_type=album_type, limit=50, offset=len(albums))
+            albums += _convert_albums(curr_response, album_type)
+    return albums
 
 
 def _convert_albums(json_album_response, album_type):
     return [album.SpotifyAlbum(album_type=album_type, spotify_id=item['id'], release_date_precision=item['release_date_precision'], release_date=item['release_date']) for item in json_album_response['items']]
 
 
 def _fetch_album_tracks(spotify, album):
```

### Comparing `lastipy-1.1.8/lastipy/spotify/parse_spotify_tracks.py` & `lastipy-1.1.9/lastipy/spotify/parse_spotify_tracks.py`

 * *Files identical despite different names*

### Comparing `lastipy-1.1.8/lastipy/spotify/playlist.py` & `lastipy-1.1.9/lastipy/spotify/playlist.py`

 * *Files identical despite different names*

### Comparing `lastipy-1.1.8/lastipy/spotify/playlist_track.py` & `lastipy-1.1.9/lastipy/spotify/playlist_track.py`

 * *Files identical despite different names*

### Comparing `lastipy-1.1.8/lastipy/spotify/search.py` & `lastipy-1.1.9/lastipy/spotify/search.py`

 * *Files identical despite different names*

### Comparing `lastipy-1.1.8/lastipy/spotify/spotify_recommendations.py` & `lastipy-1.1.9/lastipy/spotify/spotify_recommendations.py`

 * *Files identical despite different names*

### Comparing `lastipy-1.1.8/lastipy/spotify/token.py` & `lastipy-1.1.9/lastipy/spotify/token.py`

 * *Files identical despite different names*

### Comparing `lastipy-1.1.8/lastipy/track.py` & `lastipy-1.1.9/lastipy/track.py`

 * *Files identical despite different names*

### Comparing `lastipy-1.1.8/lastipy/util/parse_api_keys.py` & `lastipy-1.1.9/lastipy/util/parse_api_keys.py`

 * *Files identical despite different names*

### Comparing `lastipy-1.1.8/lastipy/util/setup_logging.py` & `lastipy-1.1.9/lastipy/util/setup_logging.py`

 * *Files identical despite different names*

### Comparing `lastipy-1.1.8/lastipy.egg-info/SOURCES.txt` & `lastipy-1.1.9/lastipy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lastipy-1.1.8/scripts/organize_favorites.py` & `lastipy-1.1.9/scripts/organize_favorites.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,17 +4,14 @@
 from spotipy import Spotify
 from lastipy.spotify import token
 from configparser import ConfigParser
 import argparse
 import os
 from lastipy import definitions
 from lastipy.lastfm.library.top_tracks import fetch_top_tracks
-from lastipy.lastfm.recommendations.similar_tracks import fetch_similar_tracks
-from lastipy.lastfm.recommendations.recommendations import generate_recommendations
-from lastipy.lastfm.library.recent_tracks import fetch_recent_tracks
 from lastipy.lastfm.library.recent_artists import fetch_recent_artists
 from lastipy.lastfm.library import period
 from lastipy.track import Track
 from numpy.random import choice
 from spotipy import Spotify
 from lastipy.spotify import token
 from lastipy.util.setup_logging import setup_logging
```

### Comparing `lastipy-1.1.8/scripts/recommendations_playlist.py` & `lastipy-1.1.9/scripts/recommendations_playlist.py`

 * *Files identical despite different names*

### Comparing `lastipy-1.1.8/scripts/save_new_releases.py` & `lastipy-1.1.9/scripts/save_new_releases.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 #!/usr/bin/env python3.7
 
 from configparser import ConfigParser
 import argparse
 import os
 from lastipy import definitions
 from lastipy.lastfm.library.top_tracks import fetch_top_tracks
-from lastipy.lastfm.recommendations.similar_tracks import fetch_similar_tracks
-from lastipy.lastfm.recommendations.recommendations import generate_recommendations
 from lastipy.lastfm.library.recent_tracks import fetch_recent_tracks
 from lastipy.lastfm.library.recent_artists import fetch_recent_artists
 from lastipy.lastfm.library import period
 from lastipy.spotify import playlist, search, library
 from lastipy.track import Track
 from numpy.random import choice
 from spotipy import Spotify
```

### Comparing `lastipy-1.1.8/setup.py` & `lastipy-1.1.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 setup(name='lastipy',
-      version='1.1.8',
+      version='1.1.9',
       description='Python library that combines Last.fm and Spotify',
       url='http://github.com/evanjamesjackson/lastipy',
       author='Evan Jackson',
       author_email='evanjamesjackson@gmail.com',
       packages=find_packages(),
       entry_points={'console_scripts': [
           'recommendations_playlist = scripts.recommendations_playlist:build_recommendations_playlist',
```

### Comparing `lastipy-1.1.8/test/lastfm/library/test_fetch_playcount.py` & `lastipy-1.1.9/test/lastfm/library/test_fetch_playcount.py`

 * *Files identical despite different names*

### Comparing `lastipy-1.1.8/test/lastfm/library/test_paginated_endpoint.py` & `lastipy-1.1.9/test/lastfm/library/test_paginated_endpoint.py`

 * *Files identical despite different names*

### Comparing `lastipy-1.1.8/test/lastfm/library/test_recent_artists.py` & `lastipy-1.1.9/test/lastfm/library/test_recent_artists.py`

 * *Files identical despite different names*

### Comparing `lastipy-1.1.8/test/lastfm/library/test_recent_tracks.py` & `lastipy-1.1.9/test/lastfm/library/test_recent_tracks.py`

 * *Files identical despite different names*

### Comparing `lastipy-1.1.8/test/lastfm/library/test_top_tracks.py` & `lastipy-1.1.9/test/lastfm/library/test_top_tracks.py`

 * *Files identical despite different names*

### Comparing `lastipy-1.1.8/test/lastfm/test_lastfm_recommendations.py` & `lastipy-1.1.9/test/lastfm/test_lastfm_recommendations.py`

 * *Files identical despite different names*

### Comparing `lastipy-1.1.8/test/lastfm/test_parse_lastfm_tracks.py` & `lastipy-1.1.9/test/lastfm/test_parse_lastfm_tracks.py`

 * *Files identical despite different names*

### Comparing `lastipy-1.1.8/test/recommendations/test_generate_recommendations.py` & `lastipy-1.1.9/test/recommendations/test_generate_recommendations.py`

 * *Files identical despite different names*

### Comparing `lastipy-1.1.8/test/recommendations/test_rating_calculator.py` & `lastipy-1.1.9/test/recommendations/test_rating_calculator.py`

 * *Files identical despite different names*

### Comparing `lastipy-1.1.8/test/spotify/test_add_albums_to_library.py` & `lastipy-1.1.9/test/spotify/test_add_albums_to_library.py`

 * *Files identical despite different names*

### Comparing `lastipy-1.1.8/test/spotify/test_add_tracks_to_library.py` & `lastipy-1.1.9/test/spotify/test_add_tracks_to_library.py`

 * *Files identical despite different names*

### Comparing `lastipy-1.1.8/test/spotify/test_get_saved_tracks.py` & `lastipy-1.1.9/test/spotify/test_get_saved_tracks.py`

 * *Files identical despite different names*

### Comparing `lastipy-1.1.8/test/test_requests.py` & `lastipy-1.1.9/test/test_requests.py`

 * *Files identical despite different names*

