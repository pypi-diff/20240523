# Comparing `tmp/keyboardsounds-5.7.5.tar.gz` & `tmp/keyboardsounds-5.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keyboardsounds-5.7.5.tar", last modified: Fri Apr 19 22:39:56 2024, max compression
+gzip compressed data, was "keyboardsounds-5.7.6.tar", last modified: Thu May 23 05:59:10 2024, max compression
```

## Comparing `keyboardsounds-5.7.5.tar` & `keyboardsounds-5.7.6.tar`

### file list

```diff
@@ -1,163 +1,163 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 22:39:56.802567 keyboardsounds-5.7.5/
--rw-rw-rw-   0        0        0     1095 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/LICENSE
--rw-rw-rw-   0        0        0    13713 2024-04-19 22:39:56.801569 keyboardsounds-5.7.5/PKG-INFO
--rw-rw-rw-   0        0        0    13023 2024-04-19 22:39:41.000000 keyboardsounds-5.7.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 22:39:56.687371 keyboardsounds-5.7.5/keyboardsounds/
--rw-rw-rw-   0        0        0     5020 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/app_detector.py
--rw-rw-rw-   0        0        0     6278 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/app_rules.py
--rw-rw-rw-   0        0        0    10174 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/audio_manager.py
--rw-rw-rw-   0        0        0     4601 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/daemon.py
--rw-rw-rw-   0        0        0    10220 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/daemon_manager.py
-drwxrwxrwx   0        0        0        0 2024-04-19 22:39:56.700430 keyboardsounds-5.7.5/keyboardsounds/external_api/
--rw-rw-rw-   0        0        0     1987 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/external_api/__connection_handler.py
--rw-rw-rw-   0        0        0     1826 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/external_api/__external_api.py
--rw-rw-rw-   0        0        0       68 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/external_api/__init__.py
--rw-rw-rw-   0        0        0    14375 2024-04-19 22:39:41.000000 keyboardsounds-5.7.5/keyboardsounds/main.py
--rw-rw-rw-   0        0        0      185 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/path_resolver.py
--rw-rw-rw-   0        0        0     6304 2024-04-19 22:39:41.000000 keyboardsounds-5.7.5/keyboardsounds/profile.py
--rw-rw-rw-   0        0        0    18692 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profile_builder.py
--rw-rw-rw-   0        0        0     8946 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profile_validation.py
-drwxrwxrwx   0        0        0        0 2024-04-19 22:39:56.677359 keyboardsounds-5.7.5/keyboardsounds/profiles/
-drwxrwxrwx   0        0        0        0 2024-04-19 22:39:56.714609 keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/
--rw-rw-rw-   0        0        0     1107 2024-04-19 22:33:46.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/LICENSE
--rw-rw-rw-   0        0        0     2506 2024-04-19 22:25:39.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/press_back.mp3
--rw-rw-rw-   0        0        0     2506 2024-04-19 22:25:39.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/press_enter.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-19 22:25:39.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/press_key1.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-19 22:25:39.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/press_key2.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-19 22:25:39.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/press_key3.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-19 22:25:39.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/press_key4.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-19 22:25:39.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/press_key5.mp3
--rw-rw-rw-   0        0        0     2506 2024-04-19 22:25:39.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/press_space.mp3
--rw-rw-rw-   0        0        0     1028 2024-04-19 22:33:46.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/profile.yaml
--rw-rw-rw-   0        0        0     2088 2024-04-19 22:25:39.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/release_back.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-19 22:25:39.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/release_enter.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-19 22:25:39.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/release_key.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-19 22:25:39.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/release_space.mp3
-drwxrwxrwx   0        0        0        0 2024-04-19 22:39:56.725121 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/
--rw-rw-rw-   0        0        0     1107 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/LICENSE
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/press_back.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/press_enter.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/press_key1.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/press_key2.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/press_key3.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/press_key4.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/press_key5.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/press_space.mp3
--rw-rw-rw-   0        0        0     1040 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/profile.yaml
--rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/release_back.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/release_enter.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/release_key.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/release_space.mp3
-drwxrwxrwx   0        0        0        0 2024-04-19 22:39:56.735386 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/
--rw-rw-rw-   0        0        0     1107 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/LICENSE
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/press_back.mp3
--rw-rw-rw-   0        0        0     2924 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/press_enter.mp3
--rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/press_key1.mp3
--rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/press_key2.mp3
--rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/press_key3.mp3
--rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/press_key4.mp3
--rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/press_key5.mp3
--rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/press_space.mp3
--rw-rw-rw-   0        0        0     1036 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/profile.yaml
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/release_back.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/release_enter.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/release_key.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/release_space.mp3
-drwxrwxrwx   0        0        0        0 2024-04-19 22:39:56.745417 keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/
--rw-rw-rw-   0        0        0     1107 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/LICENSE
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/press_back.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/press_enter.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/press_key1.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/press_key2.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/press_key3.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/press_key4.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/press_key5.mp3
--rw-rw-rw-   0        0        0     5850 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/press_space.mp3
--rw-rw-rw-   0        0        0     1026 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/profile.yaml
--rw-rw-rw-   0        0        0     1670 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/release_back.mp3
--rw-rw-rw-   0        0        0     1252 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/release_enter.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/release_key.mp3
--rw-rw-rw-   0        0        0     1252 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/release_space.mp3
-drwxrwxrwx   0        0        0        0 2024-04-19 22:39:56.747417 keyboardsounds-5.7.5/keyboardsounds/profiles/ios/
--rw-rw-rw-   0        0        0   740450 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/ios/ios-video-recording.mp4
--rw-rw-rw-   0        0        0      668 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/ios/profile.yaml
-drwxrwxrwx   0        0        0        0 2024-04-19 22:39:56.759982 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/
--rw-rw-rw-   0        0        0     1107 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/LICENSE
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/press_back.mp3
--rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/press_enter.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/press_key1.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/press_key2.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/press_key3.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/press_key4.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/press_key5.mp3
--rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/press_space.mp3
--rw-rw-rw-   0        0        0     1029 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/profile.yaml
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/release_back.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/release_enter.mp3
--rw-rw-rw-   0        0        0     1670 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/release_key.mp3
--rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/release_space.mp3
-drwxrwxrwx   0        0        0        0 2024-04-19 22:39:56.767486 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-blue/
--rw-rw-rw-   0        0        0     1107 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-blue/LICENSE
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-blue/press_key1.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-blue/press_key2.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-blue/press_key3.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-blue/press_key4.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-blue/press_key5.mp3
--rw-rw-rw-   0        0        0      530 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-blue/profile.yaml
--rw-rw-rw-   0        0        0     1670 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-blue/release.mp3
-drwxrwxrwx   0        0        0        0 2024-04-19 22:39:56.778540 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/
--rw-rw-rw-   0        0        0     1107 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/LICENSE
--rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/press_back.mp3
--rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/press_enter.mp3
--rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/press_key1.mp3
--rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/press_key2.mp3
--rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/press_key3.mp3
--rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/press_key4.mp3
--rw-rw-rw-   0        0        0     2506 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/press_key5.mp3
--rw-rw-rw-   0        0        0     1670 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/press_space.mp3
--rw-rw-rw-   0        0        0     1029 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/profile.yaml
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/release_back.mp3
--rw-rw-rw-   0        0        0     4596 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/release_enter.mp3
--rw-rw-rw-   0        0        0     2088 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/release_key.mp3
--rw-rw-rw-   0        0        0     1670 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/release_space.mp3
-drwxrwxrwx   0        0        0        0 2024-04-19 22:39:56.783539 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-speed-silver/
--rw-rw-rw-   0        0        0    28336 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-1.wav
--rw-rw-rw-   0        0        0    34328 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-2.wav
--rw-rw-rw-   0        0        0    31488 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-3.wav
--rw-rw-rw-   0        0        0    31176 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-4.wav
--rw-rw-rw-   0        0        0    32228 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-5.wav
--rw-rw-rw-   0        0        0    32016 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-6.wav
--rw-rw-rw-   0        0        0      514 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/mx-speed-silver/profile.yaml
-drwxrwxrwx   0        0        0        0 2024-04-19 22:39:56.795050 keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/
--rw-rw-rw-   0        0        0    28076 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/back.wav
--rw-rw-rw-   0        0        0    31916 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/caps.wav
--rw-rw-rw-   0        0        0    32812 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/ctrl.wav
--rw-rw-rw-   0        0        0    22316 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/ent.wav
--rw-rw-rw-   0        0        0    42540 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/key1.wav
--rw-rw-rw-   0        0        0    26316 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/key2.wav
--rw-rw-rw-   0        0        0    25516 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/key3.wav
--rw-rw-rw-   0        0        0    25612 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/key4.wav
--rw-rw-rw-   0        0        0    28300 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/key5.wav
--rw-rw-rw-   0        0        0    26860 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/key6.wav
--rw-rw-rw-   0        0        0      982 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/profile.yaml
--rw-rw-rw-   0        0        0    23596 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/shift.wav
--rw-rw-rw-   0        0        0    23212 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/space.wav
--rw-rw-rw-   0        0        0    38060 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/tab.wav
-drwxrwxrwx   0        0        0        0 2024-04-19 22:39:56.799571 keyboardsounds-5.7.5/keyboardsounds/profiles/typewriter/
--rw-rw-rw-   0        0        0    60204 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/typewriter/delete.wav
--rw-rw-rw-   0        0        0   146204 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/typewriter/enter.wav
--rw-rw-rw-   0        0        0    32664 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/typewriter/key.wav
--rw-rw-rw-   0        0        0    31588 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/typewriter/key2.wav
--rw-rw-rw-   0        0        0      610 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/typewriter/profile.yaml
--rw-rw-rw-   0        0        0    35788 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/profiles/typewriter/space.wav
--rw-rw-rw-   0        0        0       61 2024-04-16 05:39:56.000000 keyboardsounds-5.7.5/keyboardsounds/root.py
-drwxrwxrwx   0        0        0        0 2024-04-19 22:39:56.800571 keyboardsounds-5.7.5/keyboardsounds.egg-info/
--rw-rw-rw-   0        0        0    13713 2024-04-19 22:39:56.000000 keyboardsounds-5.7.5/keyboardsounds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6760 2024-04-19 22:39:56.000000 keyboardsounds-5.7.5/keyboardsounds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 22:39:56.000000 keyboardsounds-5.7.5/keyboardsounds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2024-04-19 22:39:56.000000 keyboardsounds-5.7.5/keyboardsounds.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       76 2024-04-19 22:39:56.000000 keyboardsounds-5.7.5/keyboardsounds.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-19 22:39:56.000000 keyboardsounds-5.7.5/keyboardsounds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      727 2024-04-19 22:39:41.000000 keyboardsounds-5.7.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-19 22:39:56.802567 keyboardsounds-5.7.5/setup.cfg
--rw-rw-rw-   0        0        0     1146 2024-04-19 22:39:41.000000 keyboardsounds-5.7.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 05:59:10.980775 keyboardsounds-5.7.6/
+-rw-rw-rw-   0        0        0     1074 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/LICENSE
+-rw-rw-rw-   0        0        0    13701 2024-05-23 05:59:10.979753 keyboardsounds-5.7.6/PKG-INFO
+-rw-rw-rw-   0        0        0    12617 2024-05-23 05:55:42.000000 keyboardsounds-5.7.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 05:59:10.779882 keyboardsounds-5.7.6/keyboardsounds/
+-rw-rw-rw-   0        0        0     5020 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/app_detector.py
+-rw-rw-rw-   0        0        0     6278 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/app_rules.py
+-rw-rw-rw-   0        0        0     9942 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/audio_manager.py
+-rw-rw-rw-   0        0        0     4435 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/daemon.py
+-rw-rw-rw-   0        0        0     9894 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/daemon_manager.py
+drwxrwxrwx   0        0        0        0 2024-05-23 05:59:10.806591 keyboardsounds-5.7.6/keyboardsounds/external_api/
+-rw-rw-rw-   0        0        0     1987 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/external_api/__connection_handler.py
+-rw-rw-rw-   0        0        0     1826 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/external_api/__external_api.py
+-rw-rw-rw-   0        0        0       68 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/external_api/__init__.py
+-rw-rw-rw-   0        0        0    13956 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/main.py
+-rw-rw-rw-   0        0        0      178 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/path_resolver.py
+-rw-rw-rw-   0        0        0     6133 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profile.py
+-rw-rw-rw-   0        0        0    18167 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profile_builder.py
+-rw-rw-rw-   0        0        0     8802 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profile_validation.py
+drwxrwxrwx   0        0        0        0 2024-05-23 05:59:10.759460 keyboardsounds-5.7.6/keyboardsounds/profiles/
+drwxrwxrwx   0        0        0        0 2024-05-23 05:59:10.824337 keyboardsounds-5.7.6/keyboardsounds/profiles/alpaca/
+-rw-rw-rw-   0        0        0     1099 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/alpaca/LICENSE
+-rw-rw-rw-   0        0        0     2506 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/alpaca/press_back.mp3
+-rw-rw-rw-   0        0        0     2506 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/alpaca/press_enter.mp3
+-rw-rw-rw-   0        0        0     2088 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/alpaca/press_key1.mp3
+-rw-rw-rw-   0        0        0     2088 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/alpaca/press_key2.mp3
+-rw-rw-rw-   0        0        0     2088 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/alpaca/press_key3.mp3
+-rw-rw-rw-   0        0        0     2088 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/alpaca/press_key4.mp3
+-rw-rw-rw-   0        0        0     2088 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/alpaca/press_key5.mp3
+-rw-rw-rw-   0        0        0     2506 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/alpaca/press_space.mp3
+-rw-rw-rw-   0        0        0      980 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/alpaca/profile.yaml
+-rw-rw-rw-   0        0        0     2088 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/alpaca/release_back.mp3
+-rw-rw-rw-   0        0        0     2088 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/alpaca/release_enter.mp3
+-rw-rw-rw-   0        0        0     2088 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/alpaca/release_key.mp3
+-rw-rw-rw-   0        0        0     2088 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/alpaca/release_space.mp3
+drwxrwxrwx   0        0        0        0 2024-05-23 05:59:10.843471 keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-black-ink/
+-rw-rw-rw-   0        0        0     1099 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-black-ink/LICENSE
+-rw-rw-rw-   0        0        0     2088 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-black-ink/press_back.mp3
+-rw-rw-rw-   0        0        0     2088 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-black-ink/press_enter.mp3
+-rw-rw-rw-   0        0        0     2088 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-black-ink/press_key1.mp3
+-rw-rw-rw-   0        0        0     2088 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-black-ink/press_key2.mp3
+-rw-rw-rw-   0        0        0     2088 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-black-ink/press_key3.mp3
+-rw-rw-rw-   0        0        0     2088 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-black-ink/press_key4.mp3
+-rw-rw-rw-   0        0        0     2088 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-black-ink/press_key5.mp3
+-rw-rw-rw-   0        0        0     2088 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-black-ink/press_space.mp3
+-rw-rw-rw-   0        0        0      992 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-black-ink/profile.yaml
+-rw-rw-rw-   0        0        0     2506 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-black-ink/release_back.mp3
+-rw-rw-rw-   0        0        0     2088 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-black-ink/release_enter.mp3
+-rw-rw-rw-   0        0        0     2088 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-black-ink/release_key.mp3
+-rw-rw-rw-   0        0        0     2088 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-black-ink/release_space.mp3
+drwxrwxrwx   0        0        0        0 2024-05-23 05:59:10.863843 keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-red-ink/
+-rw-rw-rw-   0        0        0     1099 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-red-ink/LICENSE
+-rw-rw-rw-   0        0        0     2088 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-red-ink/press_back.mp3
+-rw-rw-rw-   0        0        0     2924 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-red-ink/press_enter.mp3
+-rw-rw-rw-   0        0        0     2506 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-red-ink/press_key1.mp3
+-rw-rw-rw-   0        0        0     2506 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-red-ink/press_key2.mp3
+-rw-rw-rw-   0        0        0     2506 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-red-ink/press_key3.mp3
+-rw-rw-rw-   0        0        0     2506 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-red-ink/press_key4.mp3
+-rw-rw-rw-   0        0        0     2506 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-red-ink/press_key5.mp3
+-rw-rw-rw-   0        0        0     2506 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-red-ink/press_space.mp3
+-rw-rw-rw-   0        0        0      988 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-red-ink/profile.yaml
+-rw-rw-rw-   0        0        0     2088 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-red-ink/release_back.mp3
+-rw-rw-rw-   0        0        0     2088 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-red-ink/release_enter.mp3
+-rw-rw-rw-   0        0        0     2088 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-red-ink/release_key.mp3
+-rw-rw-rw-   0        0        0     2088 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-red-ink/release_space.mp3
+drwxrwxrwx   0        0        0        0 2024-05-23 05:59:10.881013 keyboardsounds-5.7.6/keyboardsounds/profiles/holy-panda/
+-rw-rw-rw-   0        0        0     1099 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/holy-panda/LICENSE
+-rw-rw-rw-   0        0        0     2088 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/holy-panda/press_back.mp3
+-rw-rw-rw-   0        0        0     2088 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/holy-panda/press_enter.mp3
+-rw-rw-rw-   0        0        0     2088 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/holy-panda/press_key1.mp3
+-rw-rw-rw-   0        0        0     2088 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/holy-panda/press_key2.mp3
+-rw-rw-rw-   0        0        0     2088 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/holy-panda/press_key3.mp3
+-rw-rw-rw-   0        0        0     2088 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/holy-panda/press_key4.mp3
+-rw-rw-rw-   0        0        0     2088 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/holy-panda/press_key5.mp3
+-rw-rw-rw-   0        0        0     5850 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/holy-panda/press_space.mp3
+-rw-rw-rw-   0        0        0      978 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/holy-panda/profile.yaml
+-rw-rw-rw-   0        0        0     1670 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/holy-panda/release_back.mp3
+-rw-rw-rw-   0        0        0     1252 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/holy-panda/release_enter.mp3
+-rw-rw-rw-   0        0        0     2088 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/holy-panda/release_key.mp3
+-rw-rw-rw-   0        0        0     1252 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/holy-panda/release_space.mp3
+drwxrwxrwx   0        0        0        0 2024-05-23 05:59:10.884197 keyboardsounds-5.7.6/keyboardsounds/profiles/ios/
+-rw-rw-rw-   0        0        0   740450 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/ios/ios-video-recording.mp4
+-rw-rw-rw-   0        0        0      638 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/ios/profile.yaml
+drwxrwxrwx   0        0        0        0 2024-05-23 05:59:10.910200 keyboardsounds-5.7.6/keyboardsounds/profiles/mx-black/
+-rw-rw-rw-   0        0        0     1099 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/mx-black/LICENSE
+-rw-rw-rw-   0        0        0     2088 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/mx-black/press_back.mp3
+-rw-rw-rw-   0        0        0     2506 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/mx-black/press_enter.mp3
+-rw-rw-rw-   0        0        0     2088 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/mx-black/press_key1.mp3
+-rw-rw-rw-   0        0        0     2088 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/mx-black/press_key2.mp3
+-rw-rw-rw-   0        0        0     2088 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/mx-black/press_key3.mp3
+-rw-rw-rw-   0        0        0     2088 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/mx-black/press_key4.mp3
+-rw-rw-rw-   0        0        0     2088 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/mx-black/press_key5.mp3
+-rw-rw-rw-   0        0        0     2506 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/mx-black/press_space.mp3
+-rw-rw-rw-   0        0        0      981 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/mx-black/profile.yaml
+-rw-rw-rw-   0        0        0     2088 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/mx-black/release_back.mp3
+-rw-rw-rw-   0        0        0     2088 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/mx-black/release_enter.mp3
+-rw-rw-rw-   0        0        0     1670 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/mx-black/release_key.mp3
+-rw-rw-rw-   0        0        0     2506 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/mx-black/release_space.mp3
+drwxrwxrwx   0        0        0        0 2024-05-23 05:59:10.923221 keyboardsounds-5.7.6/keyboardsounds/profiles/mx-blue/
+-rw-rw-rw-   0        0        0     1099 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/mx-blue/LICENSE
+-rw-rw-rw-   0        0        0     2088 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/mx-blue/press_key1.mp3
+-rw-rw-rw-   0        0        0     2088 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/mx-blue/press_key2.mp3
+-rw-rw-rw-   0        0        0     2088 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/mx-blue/press_key3.mp3
+-rw-rw-rw-   0        0        0     2088 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/mx-blue/press_key4.mp3
+-rw-rw-rw-   0        0        0     2088 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/mx-blue/press_key5.mp3
+-rw-rw-rw-   0        0        0      504 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/mx-blue/profile.yaml
+-rw-rw-rw-   0        0        0     1670 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/mx-blue/release.mp3
+drwxrwxrwx   0        0        0        0 2024-05-23 05:59:10.942455 keyboardsounds-5.7.6/keyboardsounds/profiles/mx-brown/
+-rw-rw-rw-   0        0        0     1099 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/mx-brown/LICENSE
+-rw-rw-rw-   0        0        0     2506 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/mx-brown/press_back.mp3
+-rw-rw-rw-   0        0        0     2506 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/mx-brown/press_enter.mp3
+-rw-rw-rw-   0        0        0     2506 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/mx-brown/press_key1.mp3
+-rw-rw-rw-   0        0        0     2506 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/mx-brown/press_key2.mp3
+-rw-rw-rw-   0        0        0     2506 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/mx-brown/press_key3.mp3
+-rw-rw-rw-   0        0        0     2506 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/mx-brown/press_key4.mp3
+-rw-rw-rw-   0        0        0     2506 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/mx-brown/press_key5.mp3
+-rw-rw-rw-   0        0        0     1670 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/mx-brown/press_space.mp3
+-rw-rw-rw-   0        0        0      981 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/mx-brown/profile.yaml
+-rw-rw-rw-   0        0        0     2088 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/mx-brown/release_back.mp3
+-rw-rw-rw-   0        0        0     4596 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/mx-brown/release_enter.mp3
+-rw-rw-rw-   0        0        0     2088 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/mx-brown/release_key.mp3
+-rw-rw-rw-   0        0        0     1670 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/mx-brown/release_space.mp3
+drwxrwxrwx   0        0        0        0 2024-05-23 05:59:10.950848 keyboardsounds-5.7.6/keyboardsounds/profiles/mx-speed-silver/
+-rw-rw-rw-   0        0        0    28336 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-1.wav
+-rw-rw-rw-   0        0        0    34328 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-2.wav
+-rw-rw-rw-   0        0        0    31488 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-3.wav
+-rw-rw-rw-   0        0        0    31176 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-4.wav
+-rw-rw-rw-   0        0        0    32228 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-5.wav
+-rw-rw-rw-   0        0        0    32016 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-6.wav
+-rw-rw-rw-   0        0        0      491 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/mx-speed-silver/profile.yaml
+drwxrwxrwx   0        0        0        0 2024-05-23 05:59:10.968057 keyboardsounds-5.7.6/keyboardsounds/profiles/telios-v2/
+-rw-rw-rw-   0        0        0    28076 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/telios-v2/back.wav
+-rw-rw-rw-   0        0        0    31916 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/telios-v2/caps.wav
+-rw-rw-rw-   0        0        0    32812 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/telios-v2/ctrl.wav
+-rw-rw-rw-   0        0        0    22316 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/telios-v2/ent.wav
+-rw-rw-rw-   0        0        0    42540 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/telios-v2/key1.wav
+-rw-rw-rw-   0        0        0    26316 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/telios-v2/key2.wav
+-rw-rw-rw-   0        0        0    25516 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/telios-v2/key3.wav
+-rw-rw-rw-   0        0        0    25612 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/telios-v2/key4.wav
+-rw-rw-rw-   0        0        0    28300 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/telios-v2/key5.wav
+-rw-rw-rw-   0        0        0    26860 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/telios-v2/key6.wav
+-rw-rw-rw-   0        0        0      932 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/telios-v2/profile.yaml
+-rw-rw-rw-   0        0        0    23596 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/telios-v2/shift.wav
+-rw-rw-rw-   0        0        0    23212 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/telios-v2/space.wav
+-rw-rw-rw-   0        0        0    38060 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/telios-v2/tab.wav
+drwxrwxrwx   0        0        0        0 2024-05-23 05:59:10.976539 keyboardsounds-5.7.6/keyboardsounds/profiles/typewriter/
+-rw-rw-rw-   0        0        0    60204 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/typewriter/delete.wav
+-rw-rw-rw-   0        0        0   146204 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/typewriter/enter.wav
+-rw-rw-rw-   0        0        0    32664 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/typewriter/key.wav
+-rw-rw-rw-   0        0        0    31588 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/typewriter/key2.wav
+-rw-rw-rw-   0        0        0      579 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/typewriter/profile.yaml
+-rw-rw-rw-   0        0        0    35788 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/profiles/typewriter/space.wav
+-rw-rw-rw-   0        0        0       60 2024-05-23 05:54:08.000000 keyboardsounds-5.7.6/keyboardsounds/root.py
+drwxrwxrwx   0        0        0        0 2024-05-23 05:59:10.978652 keyboardsounds-5.7.6/keyboardsounds.egg-info/
+-rw-rw-rw-   0        0        0    13701 2024-05-23 05:59:10.000000 keyboardsounds-5.7.6/keyboardsounds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6760 2024-05-23 05:59:10.000000 keyboardsounds-5.7.6/keyboardsounds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 05:59:10.000000 keyboardsounds-5.7.6/keyboardsounds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       91 2024-05-23 05:59:10.000000 keyboardsounds-5.7.6/keyboardsounds.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       78 2024-05-23 05:59:10.000000 keyboardsounds-5.7.6/keyboardsounds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-23 05:59:10.000000 keyboardsounds-5.7.6/keyboardsounds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      702 2024-05-23 05:56:00.000000 keyboardsounds-5.7.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-23 05:59:10.980775 keyboardsounds-5.7.6/setup.cfg
+-rw-rw-rw-   0        0        0     1109 2024-05-23 05:56:05.000000 keyboardsounds-5.7.6/setup.py
```

### Comparing `keyboardsounds-5.7.5/LICENSE` & `keyboardsounds-5.7.6/keyboardsounds/profiles/alpaca/LICENSE`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,9 @@
-MIT License
-
-Copyright (c) 2022 Nathan Fiscaletti
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+Audio samples from https://github.com/tplai/kbsim
+
+Copyright (c) Thomas Lai
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `keyboardsounds-5.7.5/PKG-INFO` & `keyboardsounds-5.7.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: keyboardsounds
-Version: 5.7.5
+Version: 5.7.6
 Summary: Adds the ability to play sounds while typing on any system.
 Author: Nathan Fiscaletti
 Author-email: Nathan Fiscaletti <nate.fiscaletti@gmail.com>
 Project-URL: Homepage, https://github.com/nathan-fiscaletti/keyboardsounds
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pygame==2.5.2
 Requires-Dist: pynput==1.7.6
 Requires-Dist: psutil==5.9.4
 Requires-Dist: imageio-ffmpeg==0.4.6
-Requires-Dist: pyyaml==6.0
+Requires-Dist: pyyaml==6.0.1
 
 # Keyboard Sounds
 
 [![Sponsor Me!](https://img.shields.io/badge/%F0%9F%92%B8-Sponsor%20Me!-blue)](https://github.com/sponsors/nathan-fiscaletti)
 [![PyPI version](https://badge.fury.io/py/keyboardsounds.svg)](https://badge.fury.io/py/keyboardsounds)
 [![GitHub license](https://img.shields.io/github/license/nathan-fiscaletti/keyboardsounds.svg)](https://github.com/nathan-fiscaletti/keyboardsounds/blob/master/LICENSE)
 [![Downloads](https://static.pepy.tech/badge/keyboardsounds)](https://pepy.tech/project/keyboardsounds)
@@ -35,15 +35,15 @@
 
 The desktop application still requires the Python package to be installed on your system.
 
 ![Desktop App Preview](https://github.com/nathan-fiscaletti/keyboardsounds-desktop/blob/main/preview.png?raw=true)
 
 ### Python Package
 
-**Python 3.7** or higher is required for this application to function. See [Download Python](https://www.python.org/downloads/) for more information on installing Python on your system.
+**Python** is required for this application to function. See [Download Python](https://www.python.org/downloads/) for more information on installing Python on your system.
 
 Once you have Python installed, you can install this application by running the following command.
 
 ```sh
 $ pip install keyboardsounds
 ```
```

### Comparing `keyboardsounds-5.7.5/README.md` & `keyboardsounds-5.7.6/keyboardsounds.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: keyboardsounds
+Version: 5.7.6
+Summary: Adds the ability to play sounds while typing on any system.
+Author: Nathan Fiscaletti
+Author-email: Nathan Fiscaletti <nate.fiscaletti@gmail.com>
+Project-URL: Homepage, https://github.com/nathan-fiscaletti/keyboardsounds
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pygame==2.5.2
+Requires-Dist: pynput==1.7.6
+Requires-Dist: psutil==5.9.4
+Requires-Dist: imageio-ffmpeg==0.4.6
+Requires-Dist: pyyaml==6.0.1
+
 # Keyboard Sounds
 
 [![Sponsor Me!](https://img.shields.io/badge/%F0%9F%92%B8-Sponsor%20Me!-blue)](https://github.com/sponsors/nathan-fiscaletti)
 [![PyPI version](https://badge.fury.io/py/keyboardsounds.svg)](https://badge.fury.io/py/keyboardsounds)
 [![GitHub license](https://img.shields.io/github/license/nathan-fiscaletti/keyboardsounds.svg)](https://github.com/nathan-fiscaletti/keyboardsounds/blob/master/LICENSE)
 [![Downloads](https://static.pepy.tech/badge/keyboardsounds)](https://pepy.tech/project/keyboardsounds)
 [![Downloads](https://static.pepy.tech/badge/keyboardsounds/month)](https://pepy.tech/project/keyboardsounds)
@@ -16,15 +35,15 @@
 
 The desktop application still requires the Python package to be installed on your system.
 
 ![Desktop App Preview](https://github.com/nathan-fiscaletti/keyboardsounds-desktop/blob/main/preview.png?raw=true)
 
 ### Python Package
 
-**Python 3.7** or higher is required for this application to function. See [Download Python](https://www.python.org/downloads/) for more information on installing Python on your system.
+**Python** is required for this application to function. See [Download Python](https://www.python.org/downloads/) for more information on installing Python on your system.
 
 Once you have Python installed, you can install this application by running the following command.
 
 ```sh
 $ pip install keyboardsounds
 ```
```

### Comparing `keyboardsounds-5.7.5/keyboardsounds/app_detector.py` & `keyboardsounds-5.7.6/keyboardsounds/app_detector.py`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/app_rules.py` & `keyboardsounds-5.7.6/keyboardsounds/app_rules.py`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/audio_manager.py` & `keyboardsounds-5.7.6/keyboardsounds/audio_manager.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,232 +1,232 @@
-import subprocess
-import wave
-import os
-import io
-import random
-
-from typing import Optional
-
-from imageio_ffmpeg import get_ffmpeg_exe
-from pynput.keyboard import Key, KeyCode
-
-from keyboardsounds.profile import Profile
-
-
-class AudioManager:
-    def __init__(self, profile: Profile) -> None:
-        """
-        Initializes the AudioManager with a given profile.
-
-        Parameters:
-        - profile (Profile): The profile object containing configuration
-                             settings such as audio sources and key mappings.
-
-        The constructor initializes the internal state, loads the sound clips
-        based on the provided profile, and sets up the audio manager.
-        """
-        self.sounds = {}
-        self.profile = profile
-        self.__prime_audio_clips()
-        self.__enabled = True
-
-    def set_profile(self, profile: Profile):
-        """
-        Sets a new profile for the AudioManager.
-
-        Parameters:
-        - profile (Profile): The new profile to be set for the AudioManager.
-
-        This method allows for changing the profile associated with the
-        AudioManager instance, updating the sound clips and key mappings
-        accordingly.
-        """
-        self.sounds = {}
-        self.profile = profile
-        self.__prime_audio_clips()
-
-    def __prime_audio_clips(self):
-        """
-        Primes audio clips based on the profile configuration.
-
-        This private method reads the profile configuration to determine the
-        type of audio sources (e.g., video files, individual audio files) and
-        prepares the audio clips accordingly. It might involve converting video
-        files to audio, extracting specific segments from audio files, and
-        organizing them for playback.
-
-        No parameters or return values as it modifies the internal state of the
-        AudioManager instance.
-        """
-        if self.profile.value("profile.type") == "video-extract":
-            ffmpeg_exe = get_ffmpeg_exe()
-            V_FILE = self.profile.get_file_path(self.profile.value("profile.video"))
-            A_FILE = f"{V_FILE}.wav"
-            subprocess.run(
-                [ffmpeg_exe, "-y", "-i", V_FILE, "-f", "wav", "-vn", A_FILE],
-                stdout=subprocess.DEVNULL,
-                stderr=subprocess.DEVNULL,
-            )
-            for source in self.profile.value("sources"):
-                self.__extract(source["id"], A_FILE, source["start"], source["end"])
-            os.unlink(A_FILE)
-        elif self.profile.value("profile.type") == "files":
-            for source in self.profile.value("sources"):
-                if isinstance(source["source"], dict):
-                    source_id = source["id"]
-                    press_loc = source["source"]["press"]
-                    press_path = self.profile.get_file_path(press_loc)
-                    release_loc = source["source"]["release"]
-                    release_path = self.profile.get_file_path(release_loc)
-                    press_id = f"{source_id}__press"
-                    release_id = f"{source_id}__release"
-
-                    self.__extract(press_id, press_path)
-                    self.__extract(release_id, release_path)
-
-                    press_snd = self.sounds[press_id].getbuffer().tobytes()
-                    release_snd = self.sounds[release_id].getbuffer().tobytes()
-
-                    self.sounds[source_id] = {
-                        "press": io.BytesIO(press_snd),
-                        "release": io.BytesIO(release_snd),
-                    }
-                    del self.sounds[press_id]
-                    del self.sounds[release_id]
-                elif type(source["source"]) == str:
-                    source_id = source["id"]
-                    path = self.profile.get_file_path(source["source"])
-                    self.__extract(source_id, path)
-
-    def __extract(self, id, input, start: float = 0.0, end: float = None):
-        """
-        Extracts and prepares an audio clip from the specified input source.
-
-        Parameters:
-        - id (str): An identifier for the audio clip.
-        - input (str): The file path of the input audio or video file.
-        - start (float, optional): The start time in seconds from which the
-                                   audio clip should be extracted.
-                                   Defaults to 0.0.
-        - end (float, optional):   The end time in seconds till which the audio
-                                   clip should be extracted. If None, the clip
-                                   is extracted till the end of the file.
-
-        This method handles both audio and video files, extracting the required
-        segment and storing it in memory for quick access. The extracted audio
-        clip is associated with the provided id.
-        """
-        if input.endswith(("mp3", "MP3")):
-            source = open(input, "rb")
-            data = source.read()
-            source.close()
-            self.sounds[id] = io.BytesIO(data)
-        else:
-            source = wave.open(input, "rb")
-            source.setpos(int(start * source.getframerate()))
-            end = end or source.getnframes() / source.getframerate()
-            frames = int((end - start) * source.getframerate())
-            self.sounds[id] = io.BytesIO()
-            dest = wave.open(self.sounds[id], "wb")
-            dest.setparams(source.getparams())
-            dest.writeframes(source.readframes(frames))
-            source.close()
-            self.sounds[id].seek(0)
-
-    def get_sound(self, key, action: str = "press") -> Optional[io.BytesIO]:
-        """
-        Retrieves the sound clip associated with a particular key and action.
-
-        Parameters:
-        - key:                    The key for which the sound needs to be
-                                  retrieved. Can be an instance of
-                                  pynput.keyboard.Key or KeyCode, or a
-                                  character.
-        - action (str, optional): The type of action, either 'press' or
-                                  'release'. Defaults to 'press'.
-
-        Returns:
-        - (Optional[io.BytesIO]): A BytesIO object containing the sound clip if
-                                  available and AudioManager is enabled;
-                                  otherwise, None.
-
-        This method looks up the sound clip based on the provided key and
-        action, taking into account any custom mappings defined in the profile.
-        If no specific sound is mapped for the key, a default or random sound
-        might be returned based on the profile configuration.
-        """
-        if not self.__enabled:
-            return None
-
-        if self.profile.value("keys") is not None:
-            if self.profile.value("keys.other") is not None:
-                for mapping in self.profile.value("keys.other"):
-                    k_val = key.name if isinstance(key, Key) else key.char
-                    if k_val in mapping["keys"]:
-                        return self.__get_sound(mapping["sound"], action)
-            if self.profile.value("keys.default") is not None:
-                default_key = self.profile.value("keys.default")
-                return self.__get_sound(default_key, action)
-        return self.__get_sound(key=None, action=action)
-
-    def set_enabled(self, enabled: bool) -> None:
-        """
-        Enables or disables the AudioManager.
-
-        Parameters:
-        - enabled (bool): A boolean flag to enable (True) or disable (False)
-                          the AudioManager.
-
-        When disabled, the AudioManager will not return any sound clips for key
-        events. This method allows for dynamic enabling/disabling of the
-        AudioManager at runtime.
-        """
-        self.__enabled = enabled
-
-    def __get_sound(self, key=None, action: str = "press") -> io.BytesIO:
-        """
-        A private method to retrieve a sound clip based on a key and action.
-
-        Parameters:
-        - key (optional):         The key for which to retrieve the sound. If
-                                  None, a random key's sound will be selected.
-        - action (str, optional): The type of action, either 'press' or
-                                  'release'. Defaults to 'press'.
-
-        Returns:
-        - (io.BytesIO): A BytesIO object containing the sound clip.
-
-        This method encapsulates the logic for determining the appropriate sound
-        clip based on the key and action, including handling default and random
-        sound selection.
-        """
-        if key is None:
-            key = list(self.sounds.keys())
-        if type(key) is list:
-            return self.__parse_sound(self.sounds[random.choice(key)], action)
-        return self.__parse_sound(self.sounds[key], action)
-
-    def __parse_sound(self, sound, action: str = "press") -> io.BytesIO:
-        """
-        Converts a sound clip into a BytesIO object suitable for playback.
-
-        Parameters:
-        - sound:                  The sound clip to be parsed. Can be a direct
-                                  audio clip or a dictionary containing 'press'
-                                  and 'release' clips.
-        - action (str, optional): The type of action, either 'press' or
-                                  'release'. Defaults to 'press'.
-
-        Returns:
-        - (io.BytesIO): A BytesIO object containing the sound clip ready for
-                        playback.
-
-        This method processes the sound clip, ensuring it is in the correct
-        format for playback. If the sound clip is a dictionary (containing
-        separate clips for key press and release), the appropriate clip is
-        selected based on the action.
-        """
-        if type(sound) is dict:
-            return io.BytesIO(sound[action].getbuffer().tobytes())
-        elif action == "press":
-            return io.BytesIO(sound.getbuffer().tobytes())
-        return None
+import subprocess
+import wave
+import os
+import io
+import random
+
+from typing import Optional
+
+from imageio_ffmpeg import get_ffmpeg_exe
+from pynput.keyboard import Key, KeyCode
+
+from keyboardsounds.profile import Profile
+
+
+class AudioManager:
+    def __init__(self, profile: Profile) -> None:
+        """
+        Initializes the AudioManager with a given profile.
+
+        Parameters:
+        - profile (Profile): The profile object containing configuration
+                             settings such as audio sources and key mappings.
+
+        The constructor initializes the internal state, loads the sound clips
+        based on the provided profile, and sets up the audio manager.
+        """
+        self.sounds = {}
+        self.profile = profile
+        self.__prime_audio_clips()
+        self.__enabled = True
+
+    def set_profile(self, profile: Profile):
+        """
+        Sets a new profile for the AudioManager.
+
+        Parameters:
+        - profile (Profile): The new profile to be set for the AudioManager.
+
+        This method allows for changing the profile associated with the
+        AudioManager instance, updating the sound clips and key mappings
+        accordingly.
+        """
+        self.sounds = {}
+        self.profile = profile
+        self.__prime_audio_clips()
+
+    def __prime_audio_clips(self):
+        """
+        Primes audio clips based on the profile configuration.
+
+        This private method reads the profile configuration to determine the
+        type of audio sources (e.g., video files, individual audio files) and
+        prepares the audio clips accordingly. It might involve converting video
+        files to audio, extracting specific segments from audio files, and
+        organizing them for playback.
+
+        No parameters or return values as it modifies the internal state of the
+        AudioManager instance.
+        """
+        if self.profile.value("profile.type") == "video-extract":
+            ffmpeg_exe = get_ffmpeg_exe()
+            V_FILE = self.profile.get_file_path(self.profile.value("profile.video"))
+            A_FILE = f"{V_FILE}.wav"
+            subprocess.run(
+                [ffmpeg_exe, "-y", "-i", V_FILE, "-f", "wav", "-vn", A_FILE],
+                stdout=subprocess.DEVNULL,
+                stderr=subprocess.DEVNULL,
+            )
+            for source in self.profile.value("sources"):
+                self.__extract(source["id"], A_FILE, source["start"], source["end"])
+            os.unlink(A_FILE)
+        elif self.profile.value("profile.type") == "files":
+            for source in self.profile.value("sources"):
+                if isinstance(source["source"], dict):
+                    source_id = source["id"]
+                    press_loc = source["source"]["press"]
+                    press_path = self.profile.get_file_path(press_loc)
+                    release_loc = source["source"]["release"]
+                    release_path = self.profile.get_file_path(release_loc)
+                    press_id = f"{source_id}__press"
+                    release_id = f"{source_id}__release"
+
+                    self.__extract(press_id, press_path)
+                    self.__extract(release_id, release_path)
+
+                    press_snd = self.sounds[press_id].getbuffer().tobytes()
+                    release_snd = self.sounds[release_id].getbuffer().tobytes()
+
+                    self.sounds[source_id] = {
+                        "press": io.BytesIO(press_snd),
+                        "release": io.BytesIO(release_snd),
+                    }
+                    del self.sounds[press_id]
+                    del self.sounds[release_id]
+                elif type(source["source"]) == str:
+                    source_id = source["id"]
+                    path = self.profile.get_file_path(source["source"])
+                    self.__extract(source_id, path)
+
+    def __extract(self, id, input, start: float = 0.0, end: float = None):
+        """
+        Extracts and prepares an audio clip from the specified input source.
+
+        Parameters:
+        - id (str): An identifier for the audio clip.
+        - input (str): The file path of the input audio or video file.
+        - start (float, optional): The start time in seconds from which the
+                                   audio clip should be extracted.
+                                   Defaults to 0.0.
+        - end (float, optional):   The end time in seconds till which the audio
+                                   clip should be extracted. If None, the clip
+                                   is extracted till the end of the file.
+
+        This method handles both audio and video files, extracting the required
+        segment and storing it in memory for quick access. The extracted audio
+        clip is associated with the provided id.
+        """
+        if input.endswith(("mp3", "MP3")):
+            source = open(input, "rb")
+            data = source.read()
+            source.close()
+            self.sounds[id] = io.BytesIO(data)
+        else:
+            source = wave.open(input, "rb")
+            source.setpos(int(start * source.getframerate()))
+            end = end or source.getnframes() / source.getframerate()
+            frames = int((end - start) * source.getframerate())
+            self.sounds[id] = io.BytesIO()
+            dest = wave.open(self.sounds[id], "wb")
+            dest.setparams(source.getparams())
+            dest.writeframes(source.readframes(frames))
+            source.close()
+            self.sounds[id].seek(0)
+
+    def get_sound(self, key, action: str = "press") -> Optional[io.BytesIO]:
+        """
+        Retrieves the sound clip associated with a particular key and action.
+
+        Parameters:
+        - key:                    The key for which the sound needs to be
+                                  retrieved. Can be an instance of
+                                  pynput.keyboard.Key or KeyCode, or a
+                                  character.
+        - action (str, optional): The type of action, either 'press' or
+                                  'release'. Defaults to 'press'.
+
+        Returns:
+        - (Optional[io.BytesIO]): A BytesIO object containing the sound clip if
+                                  available and AudioManager is enabled;
+                                  otherwise, None.
+
+        This method looks up the sound clip based on the provided key and
+        action, taking into account any custom mappings defined in the profile.
+        If no specific sound is mapped for the key, a default or random sound
+        might be returned based on the profile configuration.
+        """
+        if not self.__enabled:
+            return None
+
+        if self.profile.value("keys") is not None:
+            if self.profile.value("keys.other") is not None:
+                for mapping in self.profile.value("keys.other"):
+                    k_val = key.name if isinstance(key, Key) else key.char
+                    if k_val in mapping["keys"]:
+                        return self.__get_sound(mapping["sound"], action)
+            if self.profile.value("keys.default") is not None:
+                default_key = self.profile.value("keys.default")
+                return self.__get_sound(default_key, action)
+        return self.__get_sound(key=None, action=action)
+
+    def set_enabled(self, enabled: bool) -> None:
+        """
+        Enables or disables the AudioManager.
+
+        Parameters:
+        - enabled (bool): A boolean flag to enable (True) or disable (False)
+                          the AudioManager.
+
+        When disabled, the AudioManager will not return any sound clips for key
+        events. This method allows for dynamic enabling/disabling of the
+        AudioManager at runtime.
+        """
+        self.__enabled = enabled
+
+    def __get_sound(self, key=None, action: str = "press") -> io.BytesIO:
+        """
+        A private method to retrieve a sound clip based on a key and action.
+
+        Parameters:
+        - key (optional):         The key for which to retrieve the sound. If
+                                  None, a random key's sound will be selected.
+        - action (str, optional): The type of action, either 'press' or
+                                  'release'. Defaults to 'press'.
+
+        Returns:
+        - (io.BytesIO): A BytesIO object containing the sound clip.
+
+        This method encapsulates the logic for determining the appropriate sound
+        clip based on the key and action, including handling default and random
+        sound selection.
+        """
+        if key is None:
+            key = list(self.sounds.keys())
+        if type(key) is list:
+            return self.__parse_sound(self.sounds[random.choice(key)], action)
+        return self.__parse_sound(self.sounds[key], action)
+
+    def __parse_sound(self, sound, action: str = "press") -> io.BytesIO:
+        """
+        Converts a sound clip into a BytesIO object suitable for playback.
+
+        Parameters:
+        - sound:                  The sound clip to be parsed. Can be a direct
+                                  audio clip or a dictionary containing 'press'
+                                  and 'release' clips.
+        - action (str, optional): The type of action, either 'press' or
+                                  'release'. Defaults to 'press'.
+
+        Returns:
+        - (io.BytesIO): A BytesIO object containing the sound clip ready for
+                        playback.
+
+        This method processes the sound clip, ensuring it is in the correct
+        format for playback. If the sound clip is a dictionary (containing
+        separate clips for key press and release), the appropriate clip is
+        selected based on the action.
+        """
+        if type(sound) is dict:
+            return io.BytesIO(sound[action].getbuffer().tobytes())
+        elif action == "press":
+            return io.BytesIO(sound.getbuffer().tobytes())
+        return None
```

### Comparing `keyboardsounds-5.7.5/keyboardsounds/daemon.py` & `keyboardsounds-5.7.6/keyboardsounds/daemon.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,166 +1,166 @@
-from sys import platform
-
-import json
-import base64
-
-from pygame import mixer
-
-from pynput.keyboard import Listener
-
-from keyboardsounds.profile import Profile
-from keyboardsounds.audio_manager import AudioManager
-
-WIN32 = platform.lower().startswith("win")
-
-if WIN32:
-    from keyboardsounds import app_detector
-    from keyboardsounds import app_rules
-    from keyboardsounds.app_rules import Action
-
-__am: AudioManager = None
-__dm = None
-__volume = 100
-__down = []
-
-
-def on_command(command: dict) -> None:
-    global __volume
-
-    if "action" in command:
-        action = command["action"]
-        if action == "set_volume":
-            if "volume" in command:
-                __volume = command["volume"]
-                __dm.update_lock_file(__volume, __am.profile.name)
-                print(f"Volume set to {__volume}%")
-        elif action == "set_profile":
-            if "profile" in command:
-                profile = command["profile"]
-                try:
-                    __am.set_profile(Profile(profile))
-                    __dm.update_lock_file(__volume, profile)
-                    print(f"Profile set to {profile}")
-                except ValueError as err:
-                    print(f"Error: {err}")
-
-
-def __on_press(key):
-    """
-    Callback function for key press events.
-
-    When a key is pressed, this function is invoked to play the corresponding
-    key press sound. It prevents the same key press sound from being played
-    multiple times if the key is already pressed and held down.
-
-    Parameters:
-    - key: The key that was pressed.
-    """
-    global __am
-    global __volume
-    global __down
-
-    if key in __down:
-        return
-
-    sound = __am.get_sound(key, action="press")
-    if sound is not None:
-        clip = mixer.Sound(sound)
-        clip.set_volume(float(__volume) / float(100))
-        clip.play()
-
-    # Play the sound
-    __down.append(key)
-
-
-def __on_release(key):
-    """
-    Callback function for key release events.
-
-    When a key is released, this function is invoked to play the corresponding
-    key release sound.
-
-    Parameters:
-    - key: The key that was released.
-    """
-    global __down
-    global __am
-
-    sound = __am.get_sound(key, action="release")
-    if sound is not None:
-        clip = mixer.Sound(sound)
-        clip.set_volume(float(__volume) / float(100))
-        clip.play()
-
-    __down = [k for k in __down if k != key]
-
-
-if WIN32:
-
-    def __on_focused_application_changed(app_path: str):
-        """
-        Callback function for detecting focused application changes on Windows.
-
-        It adjusts the AudioManager's state based on the foreground application
-        by consulting the app rules.
-
-        Parameters:
-        - app_path: The file path of the application that has just gained focus.
-        """
-        rules = app_rules.get_rules()
-
-        global __am
-        if rules.has_exclusive_rule():
-            if app_path == rules.get_exclusive_rule().app_path:
-                __am.set_enabled(True)
-            else:
-                __am.set_enabled(False)
-            return
-
-        action = rules.get_action(app_path)
-        if action == Action.DISABLE:
-            __am.set_enabled(False)
-        elif action in [Action.ENABLE, Action.EXCLUSIVE]:
-            __am.set_enabled(True)
-
-
-def run(dm, volume: int, profile: str):
-    """
-    Initializes and runs the keyboard sound application.
-
-    This function initializes the AudioManager with a given profile and volume,
-    sets up the application detector if on Windows, and starts listening for
-    keyboard events.
-
-    Parameters:
-    - volume: The volume level for the sound playback.
-    - profile: The sound profile to use for the AudioManager.
-    """
-    global __am
-    global __volume
-    global __dm
-
-    __volume = volume
-    __am = AudioManager(Profile(profile))
-    __dm = dm
-
-    if WIN32:
-        app_detector.start_listening(__on_focused_application_changed)
-
-    mixer.init()
-    with Listener(on_press=__on_press, on_release=__on_release) as listener:
-        listener.join()
-
-
-def get_audio_manager() -> AudioManager:
-    """
-    Retrieves the AudioManager instance.
-
-    This function returns the AudioManager instance that is currently in use by
-    the application. It is used by the external API to access the AudioManager
-    for sound playback.
-
-    Returns:
-    - AudioManager: The AudioManager instance.
-    """
-    global __am
-    return __am
+from sys import platform
+
+import json
+import base64
+
+from pygame import mixer
+
+from pynput.keyboard import Listener
+
+from keyboardsounds.profile import Profile
+from keyboardsounds.audio_manager import AudioManager
+
+WIN32 = platform.lower().startswith("win")
+
+if WIN32:
+    from keyboardsounds import app_detector
+    from keyboardsounds import app_rules
+    from keyboardsounds.app_rules import Action
+
+__am: AudioManager = None
+__dm = None
+__volume = 100
+__down = []
+
+
+def on_command(command: dict) -> None:
+    global __volume
+
+    if "action" in command:
+        action = command["action"]
+        if action == "set_volume":
+            if "volume" in command:
+                __volume = command["volume"]
+                __dm.update_lock_file(__volume, __am.profile.name)
+                print(f"Volume set to {__volume}%")
+        elif action == "set_profile":
+            if "profile" in command:
+                profile = command["profile"]
+                try:
+                    __am.set_profile(Profile(profile))
+                    __dm.update_lock_file(__volume, profile)
+                    print(f"Profile set to {profile}")
+                except ValueError as err:
+                    print(f"Error: {err}")
+
+
+def __on_press(key):
+    """
+    Callback function for key press events.
+
+    When a key is pressed, this function is invoked to play the corresponding
+    key press sound. It prevents the same key press sound from being played
+    multiple times if the key is already pressed and held down.
+
+    Parameters:
+    - key: The key that was pressed.
+    """
+    global __am
+    global __volume
+    global __down
+
+    if key in __down:
+        return
+
+    sound = __am.get_sound(key, action="press")
+    if sound is not None:
+        clip = mixer.Sound(sound)
+        clip.set_volume(float(__volume) / float(100))
+        clip.play()
+
+    # Play the sound
+    __down.append(key)
+
+
+def __on_release(key):
+    """
+    Callback function for key release events.
+
+    When a key is released, this function is invoked to play the corresponding
+    key release sound.
+
+    Parameters:
+    - key: The key that was released.
+    """
+    global __down
+    global __am
+
+    sound = __am.get_sound(key, action="release")
+    if sound is not None:
+        clip = mixer.Sound(sound)
+        clip.set_volume(float(__volume) / float(100))
+        clip.play()
+
+    __down = [k for k in __down if k != key]
+
+
+if WIN32:
+
+    def __on_focused_application_changed(app_path: str):
+        """
+        Callback function for detecting focused application changes on Windows.
+
+        It adjusts the AudioManager's state based on the foreground application
+        by consulting the app rules.
+
+        Parameters:
+        - app_path: The file path of the application that has just gained focus.
+        """
+        rules = app_rules.get_rules()
+
+        global __am
+        if rules.has_exclusive_rule():
+            if app_path == rules.get_exclusive_rule().app_path:
+                __am.set_enabled(True)
+            else:
+                __am.set_enabled(False)
+            return
+
+        action = rules.get_action(app_path)
+        if action == Action.DISABLE:
+            __am.set_enabled(False)
+        elif action in [Action.ENABLE, Action.EXCLUSIVE]:
+            __am.set_enabled(True)
+
+
+def run(dm, volume: int, profile: str):
+    """
+    Initializes and runs the keyboard sound application.
+
+    This function initializes the AudioManager with a given profile and volume,
+    sets up the application detector if on Windows, and starts listening for
+    keyboard events.
+
+    Parameters:
+    - volume: The volume level for the sound playback.
+    - profile: The sound profile to use for the AudioManager.
+    """
+    global __am
+    global __volume
+    global __dm
+
+    __volume = volume
+    __am = AudioManager(Profile(profile))
+    __dm = dm
+
+    if WIN32:
+        app_detector.start_listening(__on_focused_application_changed)
+
+    mixer.init()
+    with Listener(on_press=__on_press, on_release=__on_release) as listener:
+        listener.join()
+
+
+def get_audio_manager() -> AudioManager:
+    """
+    Retrieves the AudioManager instance.
+
+    This function returns the AudioManager instance that is currently in use by
+    the application. It is used by the external API to access the AudioManager
+    for sound playback.
+
+    Returns:
+    - AudioManager: The AudioManager instance.
+    """
+    global __am
+    return __am
```

### Comparing `keyboardsounds-5.7.5/keyboardsounds/external_api/__connection_handler.py` & `keyboardsounds-5.7.6/keyboardsounds/external_api/__connection_handler.py`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/external_api/__external_api.py` & `keyboardsounds-5.7.6/keyboardsounds/external_api/__external_api.py`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/main.py` & `keyboardsounds-5.7.6/keyboardsounds/main.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,419 +1,419 @@
-import argparse
-import os
-import json
-
-from sys import platform
-
-LINUX = platform.lower().startswith("linux")
-WIN32 = platform.lower().startswith("win")
-
-os.environ["PYGAME_HIDE_SUPPORT_PROMPT"] = "1"
-import pygame
-
-from importlib.metadata import version
-
-from keyboardsounds.root import ROOT
-
-from keyboardsounds.daemon_manager import DaemonManager
-
-from keyboardsounds.profile import Profile
-from keyboardsounds.profile_builder import CliProfileBuilder
-
-from keyboardsounds.app_rules import Action, GlobalAction
-from keyboardsounds.app_rules import get_rules
-
-
-def main():
-    if LINUX:
-        if os.geteuid() != 0:
-            print(
-                "warning: it is recommended that you run this program "
-                + "as root on Linux systems."
-            )
-
-    LOCK_FILE = f"{ROOT}/.lock"
-
-    # Work around to get pygame to load mp3 files on windows
-    # see https://github.com/pygame/pygame/issues/2647
-    if os.name == "nt":
-        os.add_dll_directory(pygame.__path__[0])
-
-    dm = DaemonManager(LOCK_FILE)
-    if dm.capture_daemon_initialization():
-        return
-
-    version_number = version("keyboardsounds")
-
-    win_messages = []
-    if WIN32:
-        win_messages = (
-            f"  manage rules:{os.linesep * 2}"
-            f"    %(prog)s <ar|add-rule> -r <rule> -a <app>{os.linesep}"
-            f"    %(prog)s <rr|remove-rule> -a <app>{os.linesep}"
-            f"    %(prog)s <lr|list-rules> [-s]{os.linesep}"
-            f"    %(prog)s <sr|set-global-rule> -r <rule>{os.linesep}"
-            f"    %(prog)s <gr|get-global-rule> [-s]{os.linesep * 2}"
-        )
-
-    usage = (
-        (
-            f"usage: %(prog)s <action> [params]{os.linesep *2}"
-            f"  manage daemon:{os.linesep * 2}"
-            f"    %(prog)s start [-v <volume>] [-p <profile>]{os.linesep}"
-            f"    %(prog)s stop{os.linesep}"
-            f"    %(prog)s status [-s]{os.linesep * 2}"
-            f"  manage profiles:{os.linesep * 2}"
-            f"    %(prog)s <ap|add-profile> -z <zipfile>{os.linesep}"
-            f"    %(prog)s <rp|remove-profile> -n <profile>{os.linesep}"
-            f"    %(prog)s <lp|list-profiles> [-s] [--remote]{os.linesep}"
-            f"    %(prog)s <dp|download-profile> -n <profile>{os.linesep}"
-            f"    %(prog)s <bp|build-profile> -d <sound_dir> -o <zip_file>{os.linesep * 2}"
-        )
-        + win_messages
-        + (f"  other:{os.linesep * 2}" f"    %(prog)s [--version|-V]{os.linesep}")
-    )
-
-    parser = argparse.ArgumentParser(
-        prog=f"<keyboardsounds|kbs>",
-        usage=argparse.SUPPRESS,
-        description=f"Keyboard Sounds v{version_number}{os.linesep * 2}{usage}{os.linesep}",
-        formatter_class=argparse.RawDescriptionHelpFormatter,
-    )
-
-    parser.add_argument("action", help="The action to perform")
-
-    # Start Action
-    parser.add_argument(
-        "-v",
-        "--volume",
-        type=int,
-        default=100,
-        metavar="volume",
-        help="volume of the sound effects (0-100), default 100",
-    )
-    parser.add_argument(
-        "-p",
-        "--profile",
-        type=str,
-        default="ios",
-        metavar="profile",
-        help="sound profile to use, default 'ios'",
-    )
-
-    # Status Action
-    parser.add_argument(
-        "-s",
-        "--short",
-        action="store_true",
-        help="consolidate output to a single line of json for scripting",
-    )
-
-    # Profiles
-    parser.add_argument(
-        "-n",
-        "--name",
-        type=str,
-        default=None,
-        metavar="name",
-        help="name of the profile remove",
-    )
-    parser.add_argument(
-        "-z",
-        "--zip",
-        type=str,
-        default=None,
-        metavar="file",
-        help="path to the zip file containing the profile to add",
-    )
-    parser.add_argument(
-        "--remote",
-        action="store_true",
-        help="used with the list-profiles action to list remote profiles",
-    )
-    parser.add_argument("-V", "--version", action="version", version=version_number)
-
-    # Profile Builder
-    parser.add_argument(
-        "-d",
-        "--directory",
-        type=str,
-        default=None,
-        metavar="directory",
-        help="path to the directory containing the sounds to use for the profile",
-    )
-    parser.add_argument(
-        "-o",
-        "--output",
-        type=str,
-        default=None,
-        metavar="file",
-        help="path to the zip file to create",
-    )
-
-    # Rules
-    if WIN32:
-        parser.add_argument(
-            "-a",
-            "--app",
-            type=str,
-            default=None,
-            metavar="app",
-            help="absolute path to the application to add the rule for",
-        )
-        parser.add_argument(
-            "-r",
-            "--rule",
-            type=str,
-            default=None,
-            metavar="rule",
-            help="rule to apply. must be one of 'enable', 'disable', or 'exclusive'",
-        )
-
-    args = parser.parse_args()
-
-    if args.action == "start":
-        status = dm.status()
-        if status == "running":
-            print("Re-configuring running instance of Keyboard Sounds daemon...")
-        elif status == "stale" or status == "free":
-            print("Starting Keyboard Sounds daemon...")
-        if not dm.try_start(volume=args.volume, profile=args.profile):
-            print("Failed to start.")
-            return
-        print(f"Started Keyboard Sounds.")
-    elif args.action == "stop":
-        stopped = dm.try_stop()
-        print(
-            "Stopped Keyboard Sounds daemon."
-            if stopped
-            else "Failed to stop Keyboard Sounds daemon. Is it running?"
-        )
-    elif args.action == "status":
-        status = dm.status(full=not args.short, short=args.short)
-        print(f"{status}")
-    elif args.action == "add-profile" or args.action == "ap":
-        if args.zip is None:
-            print("Please specify a zip file for the profile to add.")
-            return
-        Profile.add_profile(args.zip)
-        return
-    elif args.action == "remove-profile" or args.action == "rp":
-        if args.name is None:
-            print("Please specify a name for the profile to remove.")
-            return
-        Profile.remove_profile(args.name)
-        return
-    elif args.action == "list-profiles" or args.action == "lp":
-        if args.remote:
-            profiles = Profile.list_remote_profiles()
-
-            if args.short:
-                print(json.dumps(profiles))
-                return
-            else:
-                print(f"{os.linesep} Fetching remote profiles...{os.linesep}")
-
-                names = [profile["name"] for profile in profiles]
-                names.append("Name")
-                authors = [profile["author"] for profile in profiles]
-                authors.append("Author")
-                name_len = len(max(names, key=len))
-                auth_len = len(max(authors, key=len))
-
-                print(f" Downloadable profiles{os.linesep}")
-                print(
-                    f" {'Name'.ljust(name_len)} | {'Author'.ljust(auth_len)} | Description"
-                )
-                print(f" {'-' * name_len} | {'-' * auth_len} | -----------")
-                for profile in profiles:
-                    print(
-                        f" {profile['name'].ljust(name_len)} | {profile['author'].ljust(auth_len)} | {profile['description']}"
-                    )
-                print(os.linesep)
-        else:
-            profiles = [profile.metadata() for profile in Profile.list()]
-
-            if args.short:
-                print(
-                    json.dumps(
-                        [
-                            {
-                                "name": profile["name"],
-                                "author": profile["author"],
-                                "description": profile["description"],
-                            }
-                            for profile in profiles
-                        ]
-                    )
-                )
-                return
-
-            names = [profile["name"] for profile in profiles]
-            names.append("Name")
-            authors = [profile["author"] for profile in profiles]
-            authors.append("Author")
-            name_len = len(max(names, key=len))
-            auth_len = len(max(authors, key=len))
-
-            print(f"{os.linesep} Available profiles{os.linesep}")
-            print(
-                f" {'Name'.ljust(name_len)} | {'Author'.ljust(auth_len)} | Description"
-            )
-            print(f" {'-' * name_len} | {'-' * auth_len} | -----------")
-            for profile in profiles:
-                print(
-                    f" {profile['name'].ljust(name_len)} | {profile['author'].ljust(auth_len)} | {profile['description']}"
-                )
-            print(os.linesep)
-            return
-    elif args.action == "build-profile" or args.action == "bp":
-        if args.directory is None:
-            print(
-                "Please specify a directory containing the sounds to use for the profile."
-            )
-            return
-        if args.output is None:
-            print("Please specify a zip file to create.")
-            return
-
-        builder = CliProfileBuilder(args.directory, args.output)
-        builder.start()
-    elif args.action == "download-profile" or args.action == "dp":
-        if args.name is None:
-            print("Please specify a name for the remote profile to download.")
-            return
-
-        existing = Profile.list()
-        for profile in existing:
-            if profile.metadata()["name"] == args.name:
-                print(f"Profile '{args.name}' already exists.")
-                return
-
-        try:
-            Profile.download_profile(args.name)
-        except Exception as e:
-            print(e)
-
-    # Rules are only available on windows
-    elif WIN32 and (args.action == "list-rules" or args.action == "lr"):
-        rules = get_rules()
-
-        if args.short:
-            print(
-                json.dumps(
-                    [
-                        {"app_path": rule.app_path, "action": rule.action.value}
-                        for rule in rules.rules
-                    ]
-                )
-            )
-            return
-
-        print(f"Keyboard Sounds v{version_number} - Application Rules{os.linesep}")
-
-        print(
-            f"Use 'keyboardsounds add-rule' to add a rule for a specific application."
-        )
-        print(
-            f"Use 'keyboardsounds remove-rule' to remove a rule for a specific application."
-        )
-        print(f"Use 'keyboardsounds set-global-rule' to set the global rule.")
-
-        print(f"{os.linesep}Configured Rules:{os.linesep}")
-
-        print(f" - Application : Global")
-        print(f"   Action      : {rules.global_action.value.upper()}")
-
-        for rule in rules.rules:
-            print("")
-            print(f" - Application : {rule.app_path}")
-            print(f"   Action      : {rule.action.value.upper()}")
-        print("")
-    elif WIN32 and (args.action == "add-rule" or args.action == "ar"):
-        if args.app is None:
-            print("Please specify an application to add the rule for.")
-            return
-        if args.rule is None:
-            print(
-                "Please specify a rule to apply. Must be one of 'enable', 'disable', or 'exclusive'."
-            )
-            return
-
-        args.rule = args.rule.lower()
-
-        rules = get_rules()
-        if args.rule.lower() not in [
-            Action.ENABLE.value,
-            Action.DISABLE.value,
-            Action.EXCLUSIVE.value,
-        ]:
-            print("Invalid rule. Must be one of 'enable', 'disable', or 'exclusive'.")
-            return
-        if args.rule.lower() == Action.EXCLUSIVE.value:
-            if rules.has_exclusive_rule():
-                print(
-                    "Exclusive rule already exists. Only one exclusive rule can be set."
-                )
-                return
-        rules.set_rule(args.app, Action(args.rule))
-        try:
-            rules.save()
-            print(f"Rule '{args.rule.upper()}' added for {args.app}.")
-        except Exception as e:
-            print(f"Failed to save rules: {e}")
-    elif WIN32 and (args.action == "remove-rule" or args.action == "rr"):
-        if args.app is None:
-            print("Please specify an application to remove the rule for.")
-            return
-
-        rules = get_rules()
-        if not rules.has_rule(args.app):
-            print(f"No rule exists for {args.app}.")
-            return
-
-        rules.remove_rule(args.app)
-        try:
-            rules.save()
-            print(f"Rule removed for {args.app}.")
-        except Exception as e:
-            print(f"Failed to save rules: {e}")
-    elif WIN32 and (args.action == "set-global-rule" or args.action == "sr"):
-        if args.rule is None:
-            print(
-                "Please specify a rule to apply. Must be one of 'enable' or 'disable'."
-            )
-            return
-
-        args.rule = args.rule.lower()
-
-        if args.rule not in [Action.ENABLE.value, Action.DISABLE.value]:
-            print("Invalid rule. Must be one of 'enable' or 'disable'.")
-            return
-
-        if args.rule == "exclusive":
-            print("Global rule cannot be set to 'exclusive'.")
-            return
-
-        rules = get_rules()
-        rules.set_global_action(GlobalAction(args.rule))
-
-        try:
-            rules.save()
-        except Exception as e:
-            print(f"Failed to save rules: {e}")
-            return
-
-        print(f"Global rule set to '{args.rule.upper()}'.")
-    elif WIN32 and (args.action == "get-global-rule" or args.action == "gr"):
-        rules = get_rules()
-        if args.short:
-            print(json.dumps({"global_action": rules.global_action.value}))
-            return
-        print(f"Global rule is set to '{rules.global_action.value.upper()}'.")
-
-    else:
-        parser.print_usage()
-
-
-if __name__ == "__main__":
-    main()
+import argparse
+import os
+import json
+
+from sys import platform
+
+LINUX = platform.lower().startswith("linux")
+WIN32 = platform.lower().startswith("win")
+
+os.environ["PYGAME_HIDE_SUPPORT_PROMPT"] = "1"
+import pygame
+
+from importlib.metadata import version
+
+from keyboardsounds.root import ROOT
+
+from keyboardsounds.daemon_manager import DaemonManager
+
+from keyboardsounds.profile import Profile
+from keyboardsounds.profile_builder import CliProfileBuilder
+
+from keyboardsounds.app_rules import Action, GlobalAction
+from keyboardsounds.app_rules import get_rules
+
+
+def main():
+    if LINUX:
+        if os.geteuid() != 0:
+            print(
+                "warning: it is recommended that you run this program "
+                + "as root on Linux systems."
+            )
+
+    LOCK_FILE = f"{ROOT}/.lock"
+
+    # Work around to get pygame to load mp3 files on windows
+    # see https://github.com/pygame/pygame/issues/2647
+    if os.name == "nt":
+        os.add_dll_directory(pygame.__path__[0])
+
+    dm = DaemonManager(LOCK_FILE)
+    if dm.capture_daemon_initialization():
+        return
+
+    version_number = version("keyboardsounds")
+
+    win_messages = []
+    if WIN32:
+        win_messages = (
+            f"  manage rules:{os.linesep * 2}"
+            f"    %(prog)s <ar|add-rule> -r <rule> -a <app>{os.linesep}"
+            f"    %(prog)s <rr|remove-rule> -a <app>{os.linesep}"
+            f"    %(prog)s <lr|list-rules> [-s]{os.linesep}"
+            f"    %(prog)s <sr|set-global-rule> -r <rule>{os.linesep}"
+            f"    %(prog)s <gr|get-global-rule> [-s]{os.linesep * 2}"
+        )
+
+    usage = (
+        (
+            f"usage: %(prog)s <action> [params]{os.linesep *2}"
+            f"  manage daemon:{os.linesep * 2}"
+            f"    %(prog)s start [-v <volume>] [-p <profile>]{os.linesep}"
+            f"    %(prog)s stop{os.linesep}"
+            f"    %(prog)s status [-s]{os.linesep * 2}"
+            f"  manage profiles:{os.linesep * 2}"
+            f"    %(prog)s <ap|add-profile> -z <zipfile>{os.linesep}"
+            f"    %(prog)s <rp|remove-profile> -n <profile>{os.linesep}"
+            f"    %(prog)s <lp|list-profiles> [-s] [--remote]{os.linesep}"
+            f"    %(prog)s <dp|download-profile> -n <profile>{os.linesep}"
+            f"    %(prog)s <bp|build-profile> -d <sound_dir> -o <zip_file>{os.linesep * 2}"
+        )
+        + win_messages
+        + (f"  other:{os.linesep * 2}" f"    %(prog)s [--version|-V]{os.linesep}")
+    )
+
+    parser = argparse.ArgumentParser(
+        prog=f"<keyboardsounds|kbs>",
+        usage=argparse.SUPPRESS,
+        description=f"Keyboard Sounds v{version_number}{os.linesep * 2}{usage}{os.linesep}",
+        formatter_class=argparse.RawDescriptionHelpFormatter,
+    )
+
+    parser.add_argument("action", help="The action to perform")
+
+    # Start Action
+    parser.add_argument(
+        "-v",
+        "--volume",
+        type=int,
+        default=100,
+        metavar="volume",
+        help="volume of the sound effects (0-100), default 100",
+    )
+    parser.add_argument(
+        "-p",
+        "--profile",
+        type=str,
+        default="ios",
+        metavar="profile",
+        help="sound profile to use, default 'ios'",
+    )
+
+    # Status Action
+    parser.add_argument(
+        "-s",
+        "--short",
+        action="store_true",
+        help="consolidate output to a single line of json for scripting",
+    )
+
+    # Profiles
+    parser.add_argument(
+        "-n",
+        "--name",
+        type=str,
+        default=None,
+        metavar="name",
+        help="name of the profile remove",
+    )
+    parser.add_argument(
+        "-z",
+        "--zip",
+        type=str,
+        default=None,
+        metavar="file",
+        help="path to the zip file containing the profile to add",
+    )
+    parser.add_argument(
+        "--remote",
+        action="store_true",
+        help="used with the list-profiles action to list remote profiles",
+    )
+    parser.add_argument("-V", "--version", action="version", version=version_number)
+
+    # Profile Builder
+    parser.add_argument(
+        "-d",
+        "--directory",
+        type=str,
+        default=None,
+        metavar="directory",
+        help="path to the directory containing the sounds to use for the profile",
+    )
+    parser.add_argument(
+        "-o",
+        "--output",
+        type=str,
+        default=None,
+        metavar="file",
+        help="path to the zip file to create",
+    )
+
+    # Rules
+    if WIN32:
+        parser.add_argument(
+            "-a",
+            "--app",
+            type=str,
+            default=None,
+            metavar="app",
+            help="absolute path to the application to add the rule for",
+        )
+        parser.add_argument(
+            "-r",
+            "--rule",
+            type=str,
+            default=None,
+            metavar="rule",
+            help="rule to apply. must be one of 'enable', 'disable', or 'exclusive'",
+        )
+
+    args = parser.parse_args()
+
+    if args.action == "start":
+        status = dm.status()
+        if status == "running":
+            print("Re-configuring running instance of Keyboard Sounds daemon...")
+        elif status == "stale" or status == "free":
+            print("Starting Keyboard Sounds daemon...")
+        if not dm.try_start(volume=args.volume, profile=args.profile):
+            print("Failed to start.")
+            return
+        print(f"Started Keyboard Sounds.")
+    elif args.action == "stop":
+        stopped = dm.try_stop()
+        print(
+            "Stopped Keyboard Sounds daemon."
+            if stopped
+            else "Failed to stop Keyboard Sounds daemon. Is it running?"
+        )
+    elif args.action == "status":
+        status = dm.status(full=not args.short, short=args.short)
+        print(f"{status}")
+    elif args.action == "add-profile" or args.action == "ap":
+        if args.zip is None:
+            print("Please specify a zip file for the profile to add.")
+            return
+        Profile.add_profile(args.zip)
+        return
+    elif args.action == "remove-profile" or args.action == "rp":
+        if args.name is None:
+            print("Please specify a name for the profile to remove.")
+            return
+        Profile.remove_profile(args.name)
+        return
+    elif args.action == "list-profiles" or args.action == "lp":
+        if args.remote:
+            profiles = Profile.list_remote_profiles()
+
+            if args.short:
+                print(json.dumps(profiles))
+                return
+            else:
+                print(f"{os.linesep} Fetching remote profiles...{os.linesep}")
+
+                names = [profile["name"] for profile in profiles]
+                names.append("Name")
+                authors = [profile["author"] for profile in profiles]
+                authors.append("Author")
+                name_len = len(max(names, key=len))
+                auth_len = len(max(authors, key=len))
+
+                print(f" Downloadable profiles{os.linesep}")
+                print(
+                    f" {'Name'.ljust(name_len)} | {'Author'.ljust(auth_len)} | Description"
+                )
+                print(f" {'-' * name_len} | {'-' * auth_len} | -----------")
+                for profile in profiles:
+                    print(
+                        f" {profile['name'].ljust(name_len)} | {profile['author'].ljust(auth_len)} | {profile['description']}"
+                    )
+                print(os.linesep)
+        else:
+            profiles = [profile.metadata() for profile in Profile.list()]
+
+            if args.short:
+                print(
+                    json.dumps(
+                        [
+                            {
+                                "name": profile["name"],
+                                "author": profile["author"],
+                                "description": profile["description"],
+                            }
+                            for profile in profiles
+                        ]
+                    )
+                )
+                return
+
+            names = [profile["name"] for profile in profiles]
+            names.append("Name")
+            authors = [profile["author"] for profile in profiles]
+            authors.append("Author")
+            name_len = len(max(names, key=len))
+            auth_len = len(max(authors, key=len))
+
+            print(f"{os.linesep} Available profiles{os.linesep}")
+            print(
+                f" {'Name'.ljust(name_len)} | {'Author'.ljust(auth_len)} | Description"
+            )
+            print(f" {'-' * name_len} | {'-' * auth_len} | -----------")
+            for profile in profiles:
+                print(
+                    f" {profile['name'].ljust(name_len)} | {profile['author'].ljust(auth_len)} | {profile['description']}"
+                )
+            print(os.linesep)
+            return
+    elif args.action == "build-profile" or args.action == "bp":
+        if args.directory is None:
+            print(
+                "Please specify a directory containing the sounds to use for the profile."
+            )
+            return
+        if args.output is None:
+            print("Please specify a zip file to create.")
+            return
+
+        builder = CliProfileBuilder(args.directory, args.output)
+        builder.start()
+    elif args.action == "download-profile" or args.action == "dp":
+        if args.name is None:
+            print("Please specify a name for the remote profile to download.")
+            return
+
+        existing = Profile.list()
+        for profile in existing:
+            if profile.metadata()["name"] == args.name:
+                print(f"Profile '{args.name}' already exists.")
+                return
+
+        try:
+            Profile.download_profile(args.name)
+        except Exception as e:
+            print(e)
+
+    # Rules are only available on windows
+    elif WIN32 and (args.action == "list-rules" or args.action == "lr"):
+        rules = get_rules()
+
+        if args.short:
+            print(
+                json.dumps(
+                    [
+                        {"app_path": rule.app_path, "action": rule.action.value}
+                        for rule in rules.rules
+                    ]
+                )
+            )
+            return
+
+        print(f"Keyboard Sounds v{version_number} - Application Rules{os.linesep}")
+
+        print(
+            f"Use 'keyboardsounds add-rule' to add a rule for a specific application."
+        )
+        print(
+            f"Use 'keyboardsounds remove-rule' to remove a rule for a specific application."
+        )
+        print(f"Use 'keyboardsounds set-global-rule' to set the global rule.")
+
+        print(f"{os.linesep}Configured Rules:{os.linesep}")
+
+        print(f" - Application : Global")
+        print(f"   Action      : {rules.global_action.value.upper()}")
+
+        for rule in rules.rules:
+            print("")
+            print(f" - Application : {rule.app_path}")
+            print(f"   Action      : {rule.action.value.upper()}")
+        print("")
+    elif WIN32 and (args.action == "add-rule" or args.action == "ar"):
+        if args.app is None:
+            print("Please specify an application to add the rule for.")
+            return
+        if args.rule is None:
+            print(
+                "Please specify a rule to apply. Must be one of 'enable', 'disable', or 'exclusive'."
+            )
+            return
+
+        args.rule = args.rule.lower()
+
+        rules = get_rules()
+        if args.rule.lower() not in [
+            Action.ENABLE.value,
+            Action.DISABLE.value,
+            Action.EXCLUSIVE.value,
+        ]:
+            print("Invalid rule. Must be one of 'enable', 'disable', or 'exclusive'.")
+            return
+        if args.rule.lower() == Action.EXCLUSIVE.value:
+            if rules.has_exclusive_rule():
+                print(
+                    "Exclusive rule already exists. Only one exclusive rule can be set."
+                )
+                return
+        rules.set_rule(args.app, Action(args.rule))
+        try:
+            rules.save()
+            print(f"Rule '{args.rule.upper()}' added for {args.app}.")
+        except Exception as e:
+            print(f"Failed to save rules: {e}")
+    elif WIN32 and (args.action == "remove-rule" or args.action == "rr"):
+        if args.app is None:
+            print("Please specify an application to remove the rule for.")
+            return
+
+        rules = get_rules()
+        if not rules.has_rule(args.app):
+            print(f"No rule exists for {args.app}.")
+            return
+
+        rules.remove_rule(args.app)
+        try:
+            rules.save()
+            print(f"Rule removed for {args.app}.")
+        except Exception as e:
+            print(f"Failed to save rules: {e}")
+    elif WIN32 and (args.action == "set-global-rule" or args.action == "sr"):
+        if args.rule is None:
+            print(
+                "Please specify a rule to apply. Must be one of 'enable' or 'disable'."
+            )
+            return
+
+        args.rule = args.rule.lower()
+
+        if args.rule not in [Action.ENABLE.value, Action.DISABLE.value]:
+            print("Invalid rule. Must be one of 'enable' or 'disable'.")
+            return
+
+        if args.rule == "exclusive":
+            print("Global rule cannot be set to 'exclusive'.")
+            return
+
+        rules = get_rules()
+        rules.set_global_action(GlobalAction(args.rule))
+
+        try:
+            rules.save()
+        except Exception as e:
+            print(f"Failed to save rules: {e}")
+            return
+
+        print(f"Global rule set to '{args.rule.upper()}'.")
+    elif WIN32 and (args.action == "get-global-rule" or args.action == "gr"):
+        rules = get_rules()
+        if args.short:
+            print(json.dumps({"global_action": rules.global_action.value}))
+            return
+        print(f"Global rule is set to '{rules.global_action.value.upper()}'.")
+
+    else:
+        parser.print_usage()
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profile.py` & `keyboardsounds-5.7.6/keyboardsounds/profile.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,171 +1,171 @@
-import os
-import yaml
-import zipfile
-import shutil
-import tempfile
-import requests
-
-from keyboardsounds.root import ROOT
-from keyboardsounds.path_resolver import PathResolver
-from keyboardsounds.profile_validation import validate_profile
-
-PROFILES_REMOTE_URL = "https://api.github.com/repos/nathan-fiscaletti/keyboardsounds/contents/keyboardsounds/profiles?ref=master"
-PROFILE_REMOTE_URL = "https://api.github.com/repos/nathan-fiscaletti/keyboardsounds/contents/keyboardsounds/profiles/{name}?ref=master"
-PROFILE_DETAIL_URL = "https://raw.githubusercontent.com/nathan-fiscaletti/keyboardsounds/master/keyboardsounds/profiles/{name}/profile.yaml"
-
-
-class Profile(PathResolver):
-    def __init__(self, name: str):
-        super().__init__(os.path.join(ROOT, "profiles", name))
-        self.name = name
-        self.__validate()
-
-    def __validate(self):
-        # Validate File Structure
-
-        if not os.path.isdir(self.root):
-            raise ValueError(f"Profile '{self.name}' does not exist")
-        if not os.path.isfile(self.get_file_path("profile.yaml")):
-            raise ValueError(
-                f"Profile '{self.name}' is corrupted. Missing profile.yaml."
-            )
-
-        with open(self.get_file_path("profile.yaml"), "r") as f:
-            data = yaml.safe_load(f)
-            self.__data = validate_profile(self, data)
-
-    def value(self, key: str):
-        value = self.__data
-        map = key.split(".")
-        for key in map:
-            if key not in value:
-                return None
-            value = value[key]
-        return value
-
-    def data(self):
-        return self.__data
-
-    def metadata(self):
-        name = self.__data["profile"]["name"]
-        author = (
-            self.__data["profile"]["author"]
-            if "author" in self.__data["profile"]
-            else None
-        )
-        description = (
-            self.__data["profile"]["description"]
-            if "description" in self.__data["profile"]
-            else None
-        )
-        return {"name": name, "author": author, "description": description}
-
-    @classmethod
-    def list(cls):
-        names = [
-            f.name for f in os.scandir(os.path.join(ROOT, "profiles")) if f.is_dir()
-        ]
-        return [Profile(name) for name in names]
-
-    @classmethod
-    def remove_profile(cls, name: str):
-        output_path = os.path.join(ROOT, "profiles", name)
-        if os.path.isdir(output_path):
-            shutil.rmtree(output_path)
-            print("Profile removed.")
-        else:
-            print("Profile does not exist.")
-
-    @classmethod
-    def list_remote_profiles(cls):
-        response = requests.get(PROFILES_REMOTE_URL)
-        if response.status_code != 200:
-            raise ValueError("Failed to fetch remote profiles.")
-        profile_names = [f["name"] for f in response.json() if f["type"] == "dir"]
-
-        result = []
-        # Retrieve `profile.yaml` for the profile
-        for profile_name in profile_names:
-            response = requests.get(PROFILE_DETAIL_URL.format(name=profile_name))
-            if response.status_code != 200:
-                raise ValueError(f"Failed to fetch remote profile '{profile_name}'.")
-            # parse the yaml file
-            profile_data = yaml.safe_load(response.text)
-            result.append(profile_data["profile"])
-        return result
-
-    @classmethod
-    def download_profile(cls, name: str):
-        print(f"Retrieving meta-data for profile '{name}'...")
-        response = requests.get(PROFILE_REMOTE_URL.format(name=name))
-        if response.status_code != 200:
-            raise ValueError(f"Failed to fetch remote profile '{name}'.")
-
-        print(f"Downloading profile '{name}'...")
-        # Get the profile data
-        profile_data = response.json()
-
-        # Create a temporary working directory
-        tmpdir = tempfile.mkdtemp()
-
-        # Download the profiles files into the directory
-        for file in profile_data:
-            if file["type"] == "file":
-                response = requests.get(file["download_url"])
-                with open(os.path.join(tmpdir, file["name"]), "wb") as f:
-                    f.write(response.content)
-
-        # Compress the contents of the directory into a zip file (stored in the temporary directory)
-        output_path = os.path.join(tmpdir, f"{name}.zip")
-        with zipfile.ZipFile(output_path, "w") as zip_ref:
-            for file in os.listdir(tmpdir):
-                file_path = os.path.join(tmpdir, file)
-                if file_path != output_path:
-                    zip_ref.write(file_path, file)
-
-        # Add the profile to the local profiles directory
-        err = None
-        try:
-            Profile.add_profile(output_path)
-        except ValueError as e:
-            err = e
-        finally:
-            # Clean up the temporary directory
-            shutil.rmtree(tmpdir)
-            if err:
-                raise err
-
-    @classmethod
-    def add_profile(cls, path: str):
-        input_path = os.path.abspath(path)
-        tmpdir = tempfile.mkdtemp()
-
-        with zipfile.ZipFile(input_path, "r") as zip_ref:
-            zip_ref.extractall(tmpdir)
-
-        profile_data = None
-        if os.path.isfile(os.path.join(tmpdir, "profile.yaml")):
-            with open(os.path.join(tmpdir, "profile.yaml"), "r") as f:
-                profile_data = yaml.safe_load(f)
-
-        if (
-            not profile_data
-            or "profile" not in profile_data
-            or "name" not in profile_data["profile"]
-        ):
-            shutil.rmtree(tmpdir)
-            raise ValueError("Profile is corrupted. Missing or invalid profile.yaml.")
-        name = profile_data["profile"]["name"]
-
-        print(f"Importing profile from '{input_path}'...")
-        output_path = os.path.join(ROOT, "profiles", name)
-
-        shutil.move(tmpdir, output_path)
-        try:
-            Profile(name)
-            print(f"Successfully imported profile '{name}'.")
-        except ValueError as e:
-            print(f"Profile '{name}' is invalid. Deleting...")
-            shutil.rmtree(output_path)
-            print(f"Error: {e}")
-            return
+import os
+import yaml
+import zipfile
+import shutil
+import tempfile
+import requests
+
+from keyboardsounds.root import ROOT
+from keyboardsounds.path_resolver import PathResolver
+from keyboardsounds.profile_validation import validate_profile
+
+PROFILES_REMOTE_URL = "https://api.github.com/repos/nathan-fiscaletti/keyboardsounds/contents/keyboardsounds/profiles?ref=master"
+PROFILE_REMOTE_URL = "https://api.github.com/repos/nathan-fiscaletti/keyboardsounds/contents/keyboardsounds/profiles/{name}?ref=master"
+PROFILE_DETAIL_URL = "https://raw.githubusercontent.com/nathan-fiscaletti/keyboardsounds/master/keyboardsounds/profiles/{name}/profile.yaml"
+
+
+class Profile(PathResolver):
+    def __init__(self, name: str):
+        super().__init__(os.path.join(ROOT, "profiles", name))
+        self.name = name
+        self.__validate()
+
+    def __validate(self):
+        # Validate File Structure
+
+        if not os.path.isdir(self.root):
+            raise ValueError(f"Profile '{self.name}' does not exist")
+        if not os.path.isfile(self.get_file_path("profile.yaml")):
+            raise ValueError(
+                f"Profile '{self.name}' is corrupted. Missing profile.yaml."
+            )
+
+        with open(self.get_file_path("profile.yaml"), "r") as f:
+            data = yaml.safe_load(f)
+            self.__data = validate_profile(self, data)
+
+    def value(self, key: str):
+        value = self.__data
+        map = key.split(".")
+        for key in map:
+            if key not in value:
+                return None
+            value = value[key]
+        return value
+
+    def data(self):
+        return self.__data
+
+    def metadata(self):
+        name = self.__data["profile"]["name"]
+        author = (
+            self.__data["profile"]["author"]
+            if "author" in self.__data["profile"]
+            else None
+        )
+        description = (
+            self.__data["profile"]["description"]
+            if "description" in self.__data["profile"]
+            else None
+        )
+        return {"name": name, "author": author, "description": description}
+
+    @classmethod
+    def list(cls):
+        names = [
+            f.name for f in os.scandir(os.path.join(ROOT, "profiles")) if f.is_dir()
+        ]
+        return [Profile(name) for name in names]
+
+    @classmethod
+    def remove_profile(cls, name: str):
+        output_path = os.path.join(ROOT, "profiles", name)
+        if os.path.isdir(output_path):
+            shutil.rmtree(output_path)
+            print("Profile removed.")
+        else:
+            print("Profile does not exist.")
+
+    @classmethod
+    def list_remote_profiles(cls):
+        response = requests.get(PROFILES_REMOTE_URL)
+        if response.status_code != 200:
+            raise ValueError("Failed to fetch remote profiles.")
+        profile_names = [f["name"] for f in response.json() if f["type"] == "dir"]
+
+        result = []
+        # Retrieve `profile.yaml` for the profile
+        for profile_name in profile_names:
+            response = requests.get(PROFILE_DETAIL_URL.format(name=profile_name))
+            if response.status_code != 200:
+                raise ValueError(f"Failed to fetch remote profile '{profile_name}'.")
+            # parse the yaml file
+            profile_data = yaml.safe_load(response.text)
+            result.append(profile_data["profile"])
+        return result
+
+    @classmethod
+    def download_profile(cls, name: str):
+        print(f"Retrieving meta-data for profile '{name}'...")
+        response = requests.get(PROFILE_REMOTE_URL.format(name=name))
+        if response.status_code != 200:
+            raise ValueError(f"Failed to fetch remote profile '{name}'.")
+
+        print(f"Downloading profile '{name}'...")
+        # Get the profile data
+        profile_data = response.json()
+
+        # Create a temporary working directory
+        tmpdir = tempfile.mkdtemp()
+
+        # Download the profiles files into the directory
+        for file in profile_data:
+            if file["type"] == "file":
+                response = requests.get(file["download_url"])
+                with open(os.path.join(tmpdir, file["name"]), "wb") as f:
+                    f.write(response.content)
+
+        # Compress the contents of the directory into a zip file (stored in the temporary directory)
+        output_path = os.path.join(tmpdir, f"{name}.zip")
+        with zipfile.ZipFile(output_path, "w") as zip_ref:
+            for file in os.listdir(tmpdir):
+                file_path = os.path.join(tmpdir, file)
+                if file_path != output_path:
+                    zip_ref.write(file_path, file)
+
+        # Add the profile to the local profiles directory
+        err = None
+        try:
+            Profile.add_profile(output_path)
+        except ValueError as e:
+            err = e
+        finally:
+            # Clean up the temporary directory
+            shutil.rmtree(tmpdir)
+            if err:
+                raise err
+
+    @classmethod
+    def add_profile(cls, path: str):
+        input_path = os.path.abspath(path)
+        tmpdir = tempfile.mkdtemp()
+
+        with zipfile.ZipFile(input_path, "r") as zip_ref:
+            zip_ref.extractall(tmpdir)
+
+        profile_data = None
+        if os.path.isfile(os.path.join(tmpdir, "profile.yaml")):
+            with open(os.path.join(tmpdir, "profile.yaml"), "r") as f:
+                profile_data = yaml.safe_load(f)
+
+        if (
+            not profile_data
+            or "profile" not in profile_data
+            or "name" not in profile_data["profile"]
+        ):
+            shutil.rmtree(tmpdir)
+            raise ValueError("Profile is corrupted. Missing or invalid profile.yaml.")
+        name = profile_data["profile"]["name"]
+
+        print(f"Importing profile from '{input_path}'...")
+        output_path = os.path.join(ROOT, "profiles", name)
+
+        shutil.move(tmpdir, output_path)
+        try:
+            Profile(name)
+            print(f"Successfully imported profile '{name}'.")
+        except ValueError as e:
+            print(f"Profile '{name}' is invalid. Deleting...")
+            shutil.rmtree(output_path)
+            print(f"Error: {e}")
+            return
```

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profile_builder.py` & `keyboardsounds-5.7.6/keyboardsounds/profile_builder.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,526 +1,526 @@
-import os
-import sys
-import tempfile
-import yaml
-import shutil
-
-from typing import List
-
-from enum import Enum
-from pynput.keyboard import Listener, Key
-
-from keyboardsounds.profile_validation import SUPPORTED_AUDIO_FORMATS
-from keyboardsounds.path_resolver import PathResolver
-
-class SourceEvent(Enum):
-    PRESS = "press"
-    RELEASE = "release"
-
-class AudioFile:
-    def __init__(self, resolver: PathResolver, value: str):
-        if not str(value).endswith(tuple(SUPPORTED_AUDIO_FORMATS)):
-            raise ValueError(f"Invalid audio file '{value}'.")
-        if not os.path.isfile(resolver.get_file_path(value)):
-            raise ValueError(f"Missing audio file '{value}'.")
-        self.value = value
-
-    def __str__(self) -> str:
-        return self.value
-
-class ProfileBuilder(PathResolver):
-    def __init__(self, path):
-        super().__init__(path)
-        self.__audio_files = []
-        self.__data = {}
-        self.__load_audio_files()
-        
-    def __load_audio_files(self):
-        for path, dirs, files in os.walk(self.root):
-            for file in files:
-                if file.endswith(tuple(SUPPORTED_AUDIO_FORMATS)):
-                    self.__audio_files.append(AudioFile(self, file))
-
-    def set_metadata(self, name: str, author: str, description: str):
-        self.__data["profile"] = {
-            "name": name,
-            "author": author,
-            "description": description
-        }
-        self.__data["sources"] = []
-
-    def get_metadata(self):
-        return self.__data["profile"] if "profile" in self.__data else {}
-
-    def preview_metadata(self):
-        return yaml.dump(self.get_metadata())
-
-    def get_audio_files(self) -> List[AudioFile]:
-        return self.__audio_files
-
-    def has_audio_file(self, audio_file) -> bool:
-        return audio_file in [str(audio_file) for audio_file in self.__audio_files]
-
-    def add_source(self, id: str, audio_file: AudioFile, event: SourceEvent = SourceEvent.PRESS):
-        if "sources" not in self.__data:
-            raise ValueError("You must set meta-data before adding sources.")
-
-        existing_source = {
-            "id": id,
-            "source": str(audio_file)
-        }
-
-        existing_sources = [source for source in self.__data["sources"] if source["id"] == id]
-        if len(existing_sources) > 0:
-            existing_source = existing_sources[0]
-
-        if type(existing_source["source"]) == str:
-            if event == SourceEvent.PRESS:
-                existing_source["source"] = str(audio_file)
-            elif event == SourceEvent.RELEASE:
-                existing_press = existing_source["source"]
-                existing_source["source"] = {
-                    SourceEvent.PRESS.value: existing_press,
-                    SourceEvent.RELEASE.value: str(audio_file)
-                }
-        elif type(existing_source["source"]) == dict:
-            if event == SourceEvent.PRESS:
-                existing_source["source"][SourceEvent.PRESS.value] = str(audio_file)
-            elif event == SourceEvent.RELEASE:
-                existing_source["source"][SourceEvent.RELEASE.value] = str(audio_file)
-
-        self.__data["sources"] = [source for source in self.__data["sources"] if source["id"] != id]
-        self.__data["sources"].append(existing_source)
-
-    def get_sources(self) -> List[dict]:
-        return self.__data["sources"] if "sources" in self.__data else []
-
-    def has_source(self, id) -> bool:
-        sources = self.get_sources()
-        return id in [source["id"] for source in sources]
-
-    def preview_sources(self) -> str:
-        return yaml.dump(self.__data["sources"])
-
-    def set_default_source(self, source: any):
-        if "keys" not in self.__data:
-            self.__data["keys"] = {}
-        self.__data["keys"]["default"] = source
-
-    def remove_default_source(self):
-        if "keys" in self.__data:
-            if "default" in self.__data["keys"]:
-                del self.__data["keys"]["default"]
-
-    def has_default_source(self) -> bool:
-        return "keys" in self.__data and "default" in self.__data["keys"]
-
-    def add_key_mapping(self, id: str, keys: List[str], source: any):
-        if "keys" not in self.__data:
-            self.__data["keys"] = {}
-        if "other" not in self.__data["keys"]:
-            self.__data["keys"]["other"] = []
-        other = list(self.__data["keys"]["other"])
-        other.append({
-            "id": id,
-            "sound": source,
-            "keys": keys
-        })
-        self.__data["keys"]["other"] = other
-
-    def has_key_mapping(self, id: str) -> bool:
-        if "keys" not in self.__data:
-            return False
-        if "other" not in self.__data["keys"]:
-            return False
-        return id in [mapping["id"] for mapping in self.__data["keys"]["other"]]
-
-    def remove_key_mapping(self, id: str):
-        if "keys" not in self.__data:
-            return
-        if "other" not in self.__data["keys"]:
-            return
-        self.__data["keys"]["other"] = [mapping for mapping in self.__data["keys"]["other"] if mapping["id"] != id]
-
-    def preview_keys_mappings(self) -> str:
-        return yaml.dump(self.__data["keys"] if "keys" in self.__data else {})
-
-    def preview(self) -> str:
-        return yaml.dump(self.__data)
-
-    def build(self, output: str):
-        intermediate_dir = tempfile.mkdtemp()
-        intermediate = PathResolver(intermediate_dir)
-
-        profile_file = intermediate.get_file_path("profile.yaml")
-        with open(profile_file, "w") as file:
-            yaml.dump(self.__data, file)
-        
-        used_files = []
-        for source in self.__data["sources"]:
-            if type(source["source"]) == str:
-                used_files.append(source["source"])
-            elif type(source["source"]) == dict:
-                if SourceEvent.PRESS.value in source["source"]:
-                    used_files.append(source["source"][SourceEvent.PRESS.value])
-                if SourceEvent.RELEASE.value in source["source"]:
-                    used_files.append(source["source"][SourceEvent.RELEASE.value])
-        used_files = list(set(used_files))
-
-        for file in used_files:
-            source = self.get_file_path(file)
-            destination = intermediate.get_file_path(file)
-            shutil.copy(source, destination)
-
-        shutil.make_archive(output, "zip", intermediate_dir)
-        shutil.rmtree(intermediate_dir)
-
-class KeyCollector:
-    def __init__(self):
-        self.__pressed = []
-        self.__keys = []
-
-    def __unique_keys(self):
-        unique = []
-        for key in self.__keys:
-            if key not in unique:
-                unique.append(key)
-        return unique
-
-    def __on_press(self, key):
-        key_name = key.name if type(key) == Key else key.char
-        if ('ctrl' in self.__pressed or 'ctrl_l' in self.__pressed or 'ctrl_r' in self.__pressed) and 'shift' in self.__pressed:
-            if key_name == 'delete':
-                self.__keys = []
-                return False
-            if key_name == 'enter':
-                return False
-        self.__pressed.append(key_name)
-
-    def __on_release(self, key):
-        key_name = key.name if type(key) == Key else key.char
-        if key_name in self.__pressed:
-            self.__pressed = [pressed for pressed in self.__pressed if pressed != key_name]
-            self.__keys.append(key_name)
-        self.__report_keys()
-
-    def __report_keys(self):
-        print("\rPressed Keys:", end=" ")
-        unique = self.__unique_keys()
-        if len(unique) > 0:
-            for key in unique:
-                print(key, end=" ")
-                sys.stdout.flush()
-        else:
-            print("None", end=" ")
-            sys.stdout.flush()
-
-    def get_keys(self):
-        self.__report_keys()
-        with Listener(on_press=self.__on_press, on_release=self.__on_release) as listener:
-            listener.join()
-        print(os.linesep, end="")
-        try:
-            import termios
-            termios.tcflush(sys.stdin, termios.TCIOFLUSH)
-        except ImportError:
-            import msvcrt
-            while msvcrt.kbhit():
-                msvcrt.getch()
-        return self.__unique_keys()
-
-class CliProfileBuilder:
-    def __init__(self, path: str, output: str):
-        if not output.endswith(".zip"):
-            print("Error: Output file must be a zip file.")
-            exit(1)
-
-        self.__builder = ProfileBuilder(path)
-        self.__output = output[:-4]
-        self.__cmd = None
-        self.__args = []
-
-    def start(self):
-        self.__collect_metadata()
-        self.__open_command_interface()
-
-    def __collect_metadata(self):
-        print(f"{os.linesep}Meta Data{os.linesep}")
-        name = input("Profile name: ")
-        author = input("Profile author: ")
-        description = input("Profile description: ")
-        self.__builder.set_metadata(name, author, description)
-
-    def __open_command_interface(self):
-        print(f"{os.linesep}Configure Profile (type 'help' for help){os.linesep}")
-        while True:
-            user_input = input("> ")
-            print("")
-            input_argv = user_input.split(" ")
-            self.__cmd = input_argv[0]
-            self.__args = input_argv[1:]
-
-            if not self.__process_command():
-                break
-
-    def __process_command(self):
-        if self.__cmd == "help":
-            return self.__print_help()
-        elif self.__cmd == "list":
-            return self.__list()
-        elif self.__cmd == "metadata":
-            return self.__metadata()
-        elif self.__cmd == "preview":
-            return self.__preview()
-        elif self.__cmd == "add":
-            return self.__add()
-        elif self.__cmd == "remove":
-            return self.__remove()
-        elif self.__cmd == "save":
-            return self.__save()
-        elif self.__cmd == "cancel":
-            return False
-
-    def __add(self) -> bool:
-        if len(self.__args) < 1:
-            return self.__print_help("Error: Missing arguments.")
-        
-        add_type = self.__args[0]
-        if add_type not in ["source", "keys", "default-key"]:
-            return self.__print_help("Error: Invalid type. Must be one of 'source', 'keys' or 'default-key'.")
-
-        if add_type == "keys":
-            return self.__add_keys()
-        if add_type == "default-key":
-            return self.__add_default_key()
-        return self.__add_source()
-
-    def __remove(self) -> bool:
-        if len(self.__args) < 1:
-            return self.__print_help("Error: Missing arguments.")
-        
-        remove_type = self.__args[0]
-        if remove_type not in ["source", "keys", "default-key"]:
-            return self.__print_help("Error: Invalid type. Must be one of 'source', 'keys' or 'default-key'.")
-
-        if remove_type == "keys":
-            return self.__remove_key_mapping()
-        if remove_type == "default-key":
-            return self.__remove_default_key()
-        return self.__remove_source()
-    
-    def __add_source(self) -> bool:
-        print("Add Source")
-        print("")
-        
-        id = None
-        while True:
-            id = input("Enter Source ID: ")
-            if id == "":
-                print("Error: No ID provided for new source.")
-                return True
-            if not self.__builder.has_source(id):
-                break
-            print("Error: Source ID already in use.")
-            
-        press = None
-        release = None
-
-        while True:
-            in_press = input("Press Sound (leave empty to cancel): ")
-            if in_press == "":
-                return True
-            if not self.__builder.has_audio_file(in_press):
-                print("Error: Invalid sound.")
-                continue
-            press = AudioFile(self.__builder, in_press)
-            break
-        
-        while True:
-            in_release = input("Release Sound (leave empty for none): ")
-            if in_release == "":
-                break
-            if not self.__builder.has_audio_file(in_release):
-                print("Error: Invalid sound.")
-                continue
-            release = AudioFile(self.__builder, in_release)
-            break
-
-        self.__builder.add_source(id, press, SourceEvent.PRESS)
-        if release is not None:
-            self.__builder.add_source(id, release, SourceEvent.RELEASE)
-
-        print("")
-        print("Source added.")
-        print("")
-        print(self.__builder.preview_sources())
-
-        return True
-
-    def __remove_source(self) -> bool:
-        id = input("Enter Source ID to Remove: ")
-        if id == "":
-            print("Error: No ID provided.")
-            return True
-        if not self.__builder.has_source(id):
-            print("Error: Source ID not found.")
-            return True
-        self.__builder.remove_source(id)
-        return True
-
-    def __add_default_key(self):
-        print("Add Default Key Mapping")
-        print("")
-        print("Enter a source ID to include in the default key mapping. Leave empty to finish.")
-        print("")
-        source_ids = []
-        source = input("Source ID: ")
-        while source != "":
-            if not self.__builder.has_source(source):
-                print("Error: Invalid source ID.")
-            else:
-                source_ids.append(source)
-            source = input("Source ID: ")
-        
-        if len(source_ids) < 1:
-            print("")
-            print("Error: No source IDs entered. Default key mapping not set.")
-            print("")
-            return True
-
-        if len(source_ids) == 1:
-            self.__builder.set_default_source(source_ids[0])
-        else:
-            self.__builder.set_default_source(source)
-
-        print("")
-        print("Default key mapping set.")
-        print("")
-        print(self.__builder.preview_keys_mappings())
-        return True
-
-    def __remove_default_key(self):
-        if self.__builder.has_default_source():
-            self.__builder.remove_default_source()
-            print("Default source removed.")
-        else:
-            print("Error: No default source set.")
-        return True
-
-    def __add_keys(self):
-        print("Add Key Mappings")
-        print("")
-        
-        id = None
-        while True:
-            id = input("Enter Key Mapping ID: ")
-            if id == "":
-                print("Error: No ID provided for new key mapping.")
-                return True
-            if not self.__builder.has_key_mapping(id):
-                break
-            print("Error: Key Mapping ID already in use.")
-
-        print("")
-        print(" - Press the keys you wish to map to a source.")
-        print(" - Press 'Control + Shift + DELETE' to cancel. Press 'Control + Shift + Enter' when finished.")
-        print("")
-
-        key_names = KeyCollector().get_keys()
-
-        if len(key_names) < 1:
-            print("")
-            print("Error: No key names entered. Key mapping not set.")
-            print("")
-            return True
-
-        print("")
-        print("Enter source IDs to map to the keys. Leave empty to finish.")
-        print("")
-
-        source_ids = []
-        source_id = input("Source ID: ")
-        while source_id != "":
-            if not self.__builder.has_source(source_id):
-                print("Error: Invalid source ID.")
-            else:
-                source_ids.append(source_id)
-            source_id = input("Source ID: ")
-        
-        if len(source_ids) < 1:
-            print("")
-            print("Error: No source IDs entered. Key mapping not set.")
-            print("")
-            return True
-
-        if len(source_ids) == 1:
-            self.__builder.add_key_mapping(id, key_names, source_ids[0])
-        else:
-            self.__builder.add_key_mapping(id, key_names, source_ids)
-
-        print("")
-        print("Key mapping set.")
-        print("")
-        print(self.__builder.preview_keys_mappings())
-        return True
-
-    def __remove_key_mapping(self):
-        id = input("Enter Key Mapping ID to Remove: ")
-        if id == "":
-            print("Error: No ID provided.")
-            return True
-        if not self.__builder.has_key_mapping(id):
-            print("Error: Key Mapping ID not found.")
-            return True
-        self.__builder.remove_key_mapping(id)
-        return True
-
-    def __list(self) -> bool:
-        if len(self.__args) < 1:
-            return self.__print_help("Error: Missing arguments.")
-        
-        list_type = self.__args[0]
-        if list_type not in ["sources", "keys", "sounds"]:
-            return self.__print_help("Error: Invalid type. Must be one of 'sources', 'keys' or 'sounds'.")
-        
-        if list_type == "sources":
-            print(self.__builder.preview_sources())
-        elif list_type == "keys":
-            print(self.__builder.preview_keys_mappings())
-        elif list_type == "sounds":
-            audio_files = self.__builder.get_audio_files()
-            print(yaml.dump([str(audio_file) for audio_file in audio_files]))
-        return True
-
-    def __metadata(self) -> bool:
-        print(self.__builder.preview_metadata())
-        return True
-
-    def __preview(self) -> bool:
-        print(self.__builder.preview())
-        return True
-
-    def __save(self) -> bool:
-        print("")
-        print(f"Compressing to ZIP file at '{self.__output}'...")
-        self.__builder.build(self.__output)
-        print("Done.")
-        return False
-
-    def __print_help(self, msg: str = None) -> bool:
-        if msg is not None:
-            print(msg)
-            print("")
-        print("Available Commands:")
-        print("")
-        print(" help - print this help")
-        print(" metadata - print profile metadata")
-        print(" list <sources|keys|sounds> - list sources, keys or sounds")
-        print(" preview - preview current profile configuration")
-        print(" cancel - quit profile builder without saving")
-        print(" add <source|keys> - add a new source or key mapping")
-        print(" remove <source|keys> - remove a source or key mapping")
-        print(" save - saves the profile to the output file")
-        print("")
-        return True
-            
+import os
+import sys
+import tempfile
+import yaml
+import shutil
+
+from typing import List
+
+from enum import Enum
+from pynput.keyboard import Listener, Key
+
+from keyboardsounds.profile_validation import SUPPORTED_AUDIO_FORMATS
+from keyboardsounds.path_resolver import PathResolver
+
+class SourceEvent(Enum):
+    PRESS = "press"
+    RELEASE = "release"
+
+class AudioFile:
+    def __init__(self, resolver: PathResolver, value: str):
+        if not str(value).endswith(tuple(SUPPORTED_AUDIO_FORMATS)):
+            raise ValueError(f"Invalid audio file '{value}'.")
+        if not os.path.isfile(resolver.get_file_path(value)):
+            raise ValueError(f"Missing audio file '{value}'.")
+        self.value = value
+
+    def __str__(self) -> str:
+        return self.value
+
+class ProfileBuilder(PathResolver):
+    def __init__(self, path):
+        super().__init__(path)
+        self.__audio_files = []
+        self.__data = {}
+        self.__load_audio_files()
+        
+    def __load_audio_files(self):
+        for path, dirs, files in os.walk(self.root):
+            for file in files:
+                if file.endswith(tuple(SUPPORTED_AUDIO_FORMATS)):
+                    self.__audio_files.append(AudioFile(self, file))
+
+    def set_metadata(self, name: str, author: str, description: str):
+        self.__data["profile"] = {
+            "name": name,
+            "author": author,
+            "description": description
+        }
+        self.__data["sources"] = []
+
+    def get_metadata(self):
+        return self.__data["profile"] if "profile" in self.__data else {}
+
+    def preview_metadata(self):
+        return yaml.dump(self.get_metadata())
+
+    def get_audio_files(self) -> List[AudioFile]:
+        return self.__audio_files
+
+    def has_audio_file(self, audio_file) -> bool:
+        return audio_file in [str(audio_file) for audio_file in self.__audio_files]
+
+    def add_source(self, id: str, audio_file: AudioFile, event: SourceEvent = SourceEvent.PRESS):
+        if "sources" not in self.__data:
+            raise ValueError("You must set meta-data before adding sources.")
+
+        existing_source = {
+            "id": id,
+            "source": str(audio_file)
+        }
+
+        existing_sources = [source for source in self.__data["sources"] if source["id"] == id]
+        if len(existing_sources) > 0:
+            existing_source = existing_sources[0]
+
+        if type(existing_source["source"]) == str:
+            if event == SourceEvent.PRESS:
+                existing_source["source"] = str(audio_file)
+            elif event == SourceEvent.RELEASE:
+                existing_press = existing_source["source"]
+                existing_source["source"] = {
+                    SourceEvent.PRESS.value: existing_press,
+                    SourceEvent.RELEASE.value: str(audio_file)
+                }
+        elif type(existing_source["source"]) == dict:
+            if event == SourceEvent.PRESS:
+                existing_source["source"][SourceEvent.PRESS.value] = str(audio_file)
+            elif event == SourceEvent.RELEASE:
+                existing_source["source"][SourceEvent.RELEASE.value] = str(audio_file)
+
+        self.__data["sources"] = [source for source in self.__data["sources"] if source["id"] != id]
+        self.__data["sources"].append(existing_source)
+
+    def get_sources(self) -> List[dict]:
+        return self.__data["sources"] if "sources" in self.__data else []
+
+    def has_source(self, id) -> bool:
+        sources = self.get_sources()
+        return id in [source["id"] for source in sources]
+
+    def preview_sources(self) -> str:
+        return yaml.dump(self.__data["sources"])
+
+    def set_default_source(self, source: any):
+        if "keys" not in self.__data:
+            self.__data["keys"] = {}
+        self.__data["keys"]["default"] = source
+
+    def remove_default_source(self):
+        if "keys" in self.__data:
+            if "default" in self.__data["keys"]:
+                del self.__data["keys"]["default"]
+
+    def has_default_source(self) -> bool:
+        return "keys" in self.__data and "default" in self.__data["keys"]
+
+    def add_key_mapping(self, id: str, keys: List[str], source: any):
+        if "keys" not in self.__data:
+            self.__data["keys"] = {}
+        if "other" not in self.__data["keys"]:
+            self.__data["keys"]["other"] = []
+        other = list(self.__data["keys"]["other"])
+        other.append({
+            "id": id,
+            "sound": source,
+            "keys": keys
+        })
+        self.__data["keys"]["other"] = other
+
+    def has_key_mapping(self, id: str) -> bool:
+        if "keys" not in self.__data:
+            return False
+        if "other" not in self.__data["keys"]:
+            return False
+        return id in [mapping["id"] for mapping in self.__data["keys"]["other"]]
+
+    def remove_key_mapping(self, id: str):
+        if "keys" not in self.__data:
+            return
+        if "other" not in self.__data["keys"]:
+            return
+        self.__data["keys"]["other"] = [mapping for mapping in self.__data["keys"]["other"] if mapping["id"] != id]
+
+    def preview_keys_mappings(self) -> str:
+        return yaml.dump(self.__data["keys"] if "keys" in self.__data else {})
+
+    def preview(self) -> str:
+        return yaml.dump(self.__data)
+
+    def build(self, output: str):
+        intermediate_dir = tempfile.mkdtemp()
+        intermediate = PathResolver(intermediate_dir)
+
+        profile_file = intermediate.get_file_path("profile.yaml")
+        with open(profile_file, "w") as file:
+            yaml.dump(self.__data, file)
+        
+        used_files = []
+        for source in self.__data["sources"]:
+            if type(source["source"]) == str:
+                used_files.append(source["source"])
+            elif type(source["source"]) == dict:
+                if SourceEvent.PRESS.value in source["source"]:
+                    used_files.append(source["source"][SourceEvent.PRESS.value])
+                if SourceEvent.RELEASE.value in source["source"]:
+                    used_files.append(source["source"][SourceEvent.RELEASE.value])
+        used_files = list(set(used_files))
+
+        for file in used_files:
+            source = self.get_file_path(file)
+            destination = intermediate.get_file_path(file)
+            shutil.copy(source, destination)
+
+        shutil.make_archive(output, "zip", intermediate_dir)
+        shutil.rmtree(intermediate_dir)
+
+class KeyCollector:
+    def __init__(self):
+        self.__pressed = []
+        self.__keys = []
+
+    def __unique_keys(self):
+        unique = []
+        for key in self.__keys:
+            if key not in unique:
+                unique.append(key)
+        return unique
+
+    def __on_press(self, key):
+        key_name = key.name if type(key) == Key else key.char
+        if ('ctrl' in self.__pressed or 'ctrl_l' in self.__pressed or 'ctrl_r' in self.__pressed) and 'shift' in self.__pressed:
+            if key_name == 'delete':
+                self.__keys = []
+                return False
+            if key_name == 'enter':
+                return False
+        self.__pressed.append(key_name)
+
+    def __on_release(self, key):
+        key_name = key.name if type(key) == Key else key.char
+        if key_name in self.__pressed:
+            self.__pressed = [pressed for pressed in self.__pressed if pressed != key_name]
+            self.__keys.append(key_name)
+        self.__report_keys()
+
+    def __report_keys(self):
+        print("\rPressed Keys:", end=" ")
+        unique = self.__unique_keys()
+        if len(unique) > 0:
+            for key in unique:
+                print(key, end=" ")
+                sys.stdout.flush()
+        else:
+            print("None", end=" ")
+            sys.stdout.flush()
+
+    def get_keys(self):
+        self.__report_keys()
+        with Listener(on_press=self.__on_press, on_release=self.__on_release) as listener:
+            listener.join()
+        print(os.linesep, end="")
+        try:
+            import termios
+            termios.tcflush(sys.stdin, termios.TCIOFLUSH)
+        except ImportError:
+            import msvcrt
+            while msvcrt.kbhit():
+                msvcrt.getch()
+        return self.__unique_keys()
+
+class CliProfileBuilder:
+    def __init__(self, path: str, output: str):
+        if not output.endswith(".zip"):
+            print("Error: Output file must be a zip file.")
+            exit(1)
+
+        self.__builder = ProfileBuilder(path)
+        self.__output = output[:-4]
+        self.__cmd = None
+        self.__args = []
+
+    def start(self):
+        self.__collect_metadata()
+        self.__open_command_interface()
+
+    def __collect_metadata(self):
+        print(f"{os.linesep}Meta Data{os.linesep}")
+        name = input("Profile name: ")
+        author = input("Profile author: ")
+        description = input("Profile description: ")
+        self.__builder.set_metadata(name, author, description)
+
+    def __open_command_interface(self):
+        print(f"{os.linesep}Configure Profile (type 'help' for help){os.linesep}")
+        while True:
+            user_input = input("> ")
+            print("")
+            input_argv = user_input.split(" ")
+            self.__cmd = input_argv[0]
+            self.__args = input_argv[1:]
+
+            if not self.__process_command():
+                break
+
+    def __process_command(self):
+        if self.__cmd == "help":
+            return self.__print_help()
+        elif self.__cmd == "list":
+            return self.__list()
+        elif self.__cmd == "metadata":
+            return self.__metadata()
+        elif self.__cmd == "preview":
+            return self.__preview()
+        elif self.__cmd == "add":
+            return self.__add()
+        elif self.__cmd == "remove":
+            return self.__remove()
+        elif self.__cmd == "save":
+            return self.__save()
+        elif self.__cmd == "cancel":
+            return False
+
+    def __add(self) -> bool:
+        if len(self.__args) < 1:
+            return self.__print_help("Error: Missing arguments.")
+        
+        add_type = self.__args[0]
+        if add_type not in ["source", "keys", "default-key"]:
+            return self.__print_help("Error: Invalid type. Must be one of 'source', 'keys' or 'default-key'.")
+
+        if add_type == "keys":
+            return self.__add_keys()
+        if add_type == "default-key":
+            return self.__add_default_key()
+        return self.__add_source()
+
+    def __remove(self) -> bool:
+        if len(self.__args) < 1:
+            return self.__print_help("Error: Missing arguments.")
+        
+        remove_type = self.__args[0]
+        if remove_type not in ["source", "keys", "default-key"]:
+            return self.__print_help("Error: Invalid type. Must be one of 'source', 'keys' or 'default-key'.")
+
+        if remove_type == "keys":
+            return self.__remove_key_mapping()
+        if remove_type == "default-key":
+            return self.__remove_default_key()
+        return self.__remove_source()
+    
+    def __add_source(self) -> bool:
+        print("Add Source")
+        print("")
+        
+        id = None
+        while True:
+            id = input("Enter Source ID: ")
+            if id == "":
+                print("Error: No ID provided for new source.")
+                return True
+            if not self.__builder.has_source(id):
+                break
+            print("Error: Source ID already in use.")
+            
+        press = None
+        release = None
+
+        while True:
+            in_press = input("Press Sound (leave empty to cancel): ")
+            if in_press == "":
+                return True
+            if not self.__builder.has_audio_file(in_press):
+                print("Error: Invalid sound.")
+                continue
+            press = AudioFile(self.__builder, in_press)
+            break
+        
+        while True:
+            in_release = input("Release Sound (leave empty for none): ")
+            if in_release == "":
+                break
+            if not self.__builder.has_audio_file(in_release):
+                print("Error: Invalid sound.")
+                continue
+            release = AudioFile(self.__builder, in_release)
+            break
+
+        self.__builder.add_source(id, press, SourceEvent.PRESS)
+        if release is not None:
+            self.__builder.add_source(id, release, SourceEvent.RELEASE)
+
+        print("")
+        print("Source added.")
+        print("")
+        print(self.__builder.preview_sources())
+
+        return True
+
+    def __remove_source(self) -> bool:
+        id = input("Enter Source ID to Remove: ")
+        if id == "":
+            print("Error: No ID provided.")
+            return True
+        if not self.__builder.has_source(id):
+            print("Error: Source ID not found.")
+            return True
+        self.__builder.remove_source(id)
+        return True
+
+    def __add_default_key(self):
+        print("Add Default Key Mapping")
+        print("")
+        print("Enter a source ID to include in the default key mapping. Leave empty to finish.")
+        print("")
+        source_ids = []
+        source = input("Source ID: ")
+        while source != "":
+            if not self.__builder.has_source(source):
+                print("Error: Invalid source ID.")
+            else:
+                source_ids.append(source)
+            source = input("Source ID: ")
+        
+        if len(source_ids) < 1:
+            print("")
+            print("Error: No source IDs entered. Default key mapping not set.")
+            print("")
+            return True
+
+        if len(source_ids) == 1:
+            self.__builder.set_default_source(source_ids[0])
+        else:
+            self.__builder.set_default_source(source)
+
+        print("")
+        print("Default key mapping set.")
+        print("")
+        print(self.__builder.preview_keys_mappings())
+        return True
+
+    def __remove_default_key(self):
+        if self.__builder.has_default_source():
+            self.__builder.remove_default_source()
+            print("Default source removed.")
+        else:
+            print("Error: No default source set.")
+        return True
+
+    def __add_keys(self):
+        print("Add Key Mappings")
+        print("")
+        
+        id = None
+        while True:
+            id = input("Enter Key Mapping ID: ")
+            if id == "":
+                print("Error: No ID provided for new key mapping.")
+                return True
+            if not self.__builder.has_key_mapping(id):
+                break
+            print("Error: Key Mapping ID already in use.")
+
+        print("")
+        print(" - Press the keys you wish to map to a source.")
+        print(" - Press 'Control + Shift + DELETE' to cancel. Press 'Control + Shift + Enter' when finished.")
+        print("")
+
+        key_names = KeyCollector().get_keys()
+
+        if len(key_names) < 1:
+            print("")
+            print("Error: No key names entered. Key mapping not set.")
+            print("")
+            return True
+
+        print("")
+        print("Enter source IDs to map to the keys. Leave empty to finish.")
+        print("")
+
+        source_ids = []
+        source_id = input("Source ID: ")
+        while source_id != "":
+            if not self.__builder.has_source(source_id):
+                print("Error: Invalid source ID.")
+            else:
+                source_ids.append(source_id)
+            source_id = input("Source ID: ")
+        
+        if len(source_ids) < 1:
+            print("")
+            print("Error: No source IDs entered. Key mapping not set.")
+            print("")
+            return True
+
+        if len(source_ids) == 1:
+            self.__builder.add_key_mapping(id, key_names, source_ids[0])
+        else:
+            self.__builder.add_key_mapping(id, key_names, source_ids)
+
+        print("")
+        print("Key mapping set.")
+        print("")
+        print(self.__builder.preview_keys_mappings())
+        return True
+
+    def __remove_key_mapping(self):
+        id = input("Enter Key Mapping ID to Remove: ")
+        if id == "":
+            print("Error: No ID provided.")
+            return True
+        if not self.__builder.has_key_mapping(id):
+            print("Error: Key Mapping ID not found.")
+            return True
+        self.__builder.remove_key_mapping(id)
+        return True
+
+    def __list(self) -> bool:
+        if len(self.__args) < 1:
+            return self.__print_help("Error: Missing arguments.")
+        
+        list_type = self.__args[0]
+        if list_type not in ["sources", "keys", "sounds"]:
+            return self.__print_help("Error: Invalid type. Must be one of 'sources', 'keys' or 'sounds'.")
+        
+        if list_type == "sources":
+            print(self.__builder.preview_sources())
+        elif list_type == "keys":
+            print(self.__builder.preview_keys_mappings())
+        elif list_type == "sounds":
+            audio_files = self.__builder.get_audio_files()
+            print(yaml.dump([str(audio_file) for audio_file in audio_files]))
+        return True
+
+    def __metadata(self) -> bool:
+        print(self.__builder.preview_metadata())
+        return True
+
+    def __preview(self) -> bool:
+        print(self.__builder.preview())
+        return True
+
+    def __save(self) -> bool:
+        print("")
+        print(f"Compressing to ZIP file at '{self.__output}'...")
+        self.__builder.build(self.__output)
+        print("Done.")
+        return False
+
+    def __print_help(self, msg: str = None) -> bool:
+        if msg is not None:
+            print(msg)
+            print("")
+        print("Available Commands:")
+        print("")
+        print(" help - print this help")
+        print(" metadata - print profile metadata")
+        print(" list <sources|keys|sounds> - list sources, keys or sounds")
+        print(" preview - preview current profile configuration")
+        print(" cancel - quit profile builder without saving")
+        print(" add <source|keys> - add a new source or key mapping")
+        print(" remove <source|keys> - remove a source or key mapping")
+        print(" save - saves the profile to the output file")
+        print("")
+        return True
+
```

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profile_validation.py` & `keyboardsounds-5.7.6/keyboardsounds/profile_validation.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,145 +1,145 @@
-import os
-
-from keyboardsounds.path_resolver import PathResolver
-
-VALID_PROFILE_TYPES = ["video-extract", "files"]
-SUPPORTED_AUDIO_FORMATS = [".wav", ".mp3", ".WAV", ".MP3"]
-SUPPORTED_VIDEO_FORMATS = [".mp4", ".MP4"]
-
-def validate_profile(path_resolver: PathResolver, data: dict):
-    # Validate Required Generic Keys
-
-    required_keys = ["profile", "sources"]
-    for required_key in required_keys:
-        if required_key not in data:
-            raise ValueError(f"Profile is corrupted. Missing '{required_key}' in profile.yaml.")
-
-    # Validate Profile Metadata
-    data = __validate_meta_data(path_resolver, data)
-    name = data["profile"]["name"]
-
-    # Validate Sources
-    __validate_sources(path_resolver, name, data)
-
-    # Validate Keys
-    __validate_keys(path_resolver, name, data)
-
-    return data
-
-def __validate_meta_data(path_resolver: PathResolver, data: dict) -> str:
-    if "name" not in data["profile"]:
-        raise ValueError(f"Profile is corrupted. Missing 'name' in profile.yaml.")
-    if type(data["profile"]["name"]) != str:
-        raise ValueError(f"Profile is corrupted. 'name' in profile.yaml must be a string.")
-    name = data["profile"]["name"]
-    if "type" in data["profile"]:
-        if data["profile"]["type"] not in VALID_PROFILE_TYPES:
-            raise ValueError(f"Profile '{name}' is corrupted. Invalid 'type' in profile.yaml.")
-    else:
-        data["profile"]["type"] = "files"
-    if "author" in data["profile"]:
-        if type(data["profile"]["author"]) != str:
-            raise ValueError(f"Profile '{name}' is corrupted. Invalid 'author' in profile.yaml.")
-    if "description" in data["profile"]:
-        if type(data["profile"]["description"]) != str:
-            raise ValueError(f"Profile '{name}' is corrupted. Invalid 'description' in profile.yaml.")
-
-    if data["profile"]["type"] == "video-extract":
-        if "video" not in data["profile"]:
-            raise ValueError(f"Profile '{name}' is corrupted. Missing 'video' in profile.yaml.")
-        if type(data["profile"]["video"]) != str:
-            raise ValueError(f"Profile '{name}' is corrupted. Invalid 'video' in profile.yaml.")
-        if not str(data["profile"]["video"]).endswith(tuple(SUPPORTED_VIDEO_FORMATS)):
-            raise ValueError(f"Profile '{name}' is corrupted. Invalid 'video' in profile.yaml.")
-        if not os.path.isfile(path_resolver.get_file_path(data["profile"]["video"])):
-            raise ValueError(f"Profile '{name}' is corrupted. Missing video file '{data['profile']['video']}' in profile folder.")
-    
-    return data
-
-def __validate_sources(path_resolver: PathResolver, name: str, data: dict):
-    if "sources" not in data:
-        raise ValueError(f"Profile '{name}' is corrupted. Missing 'sources' in profile.yaml.")
-    if type(data["sources"]) != list:
-        raise ValueError(f"Profile '{name}' is corrupted. Invalid 'sources' in profile.yaml.")
-    for source in data["sources"]:
-       __validate_source(path_resolver, name, data, source)
-
-def __validate_source(path_resolver: PathResolver, name: str, data: dict, source: any):
-    if type(source) != dict:
-        raise ValueError(f"Profile '{name}' is corrupted. Invalid 'sources' in profile.yaml.")
-    if "id" not in source:
-        raise ValueError(f"Profile '{name}' is corrupted. Missing 'id' one or more source in profile.yaml.")
-
-    if data["profile"]["type"] == "files":
-        if "source" not in source:
-            raise ValueError(f"Profile '{name}' is corrupted. Missing 'source' one or more source in profile.yaml.")
-        if type(source["source"]) not in [dict, str]:
-            raise ValueError(f"Profile '{name}' is corrupted. Invalid 'source' one or more source in profile.yaml.")
-        if type(source["source"]) == dict:
-            if not "press" in source["source"]:
-                raise ValueError(f"Profile '{name}' is corrupted. Missing 'press' in source object of one or more sources in profile.yaml.")
-            if type(source["source"]["press"]) != str:
-                raise ValueError(f"Profile '{name}' is corrupted. Invalid 'press' in source object of one or more sources in profile.yaml.")
-            if not str(source["source"]["press"]).endswith(tuple(SUPPORTED_AUDIO_FORMATS)):
-                raise ValueError(f"Profile '{name}' is corrupted. Invalid 'press' in source object of one or more sources in profile.yaml.")
-            if not os.path.isfile(path_resolver.get_file_path(source["source"]["press"])):
-                raise ValueError(f"Profile '{name}' is corrupted. Missing audio file '{source['source']['press']}' in profile folder.")
-            if "release" in source["source"]:
-                if type(source["source"]["release"]) != str:
-                    raise ValueError(f"Profile '{name}' is corrupted. Invalid 'release' in source object of one or more sources in profile.yaml.")
-                if not str(source["source"]["release"]).endswith(tuple(SUPPORTED_AUDIO_FORMATS)):
-                    raise ValueError(f"Profile '{name}' is corrupted. Invalid 'release' in source object of one or more sources in profile.yaml.")
-                if not os.path.isfile(path_resolver.get_file_path(source["source"]["release"])):
-                    raise ValueError(f"Profile '{name}' is corrupted. Missing audio file '{source['source']['release']}' in profile folder.")
-        elif type(source["source"]) == str:
-            if not str(source["source"]).endswith(tuple(SUPPORTED_AUDIO_FORMATS)):
-                raise ValueError(f"Profile '{name}' is corrupted. Invalid 'source' in one or more sources in profile.yaml.")
-            if not os.path.isfile(path_resolver.get_file_path(source["source"])):
-                raise ValueError(f"Profile '{name}' is corrupted. Missing audio file '{source['source']}' in profile folder.")
-    elif data["profile"]["type"] == "video-extract":
-        if "start" not in source:
-            raise ValueError(f"Profile '{name}' is corrupted. Missing 'start' one or more source in profile.yaml.")
-        if type(source["start"]) != float:
-            raise ValueError(f"Profile '{name}' is corrupted. Invalid 'start' one or more source in profile.yaml.")
-        if "end" not in source:
-            raise ValueError(f"Profile '{name}' is corrupted. Missing 'end' one or more source in profile.yaml.")
-        if type(source["end"]) != float:
-            raise ValueError(f"Profile '{name}' is corrupted. Invalid 'end' one or more source in profile.yaml.")
-
-def __validate_keys(path_resolver: PathResolver, name: str, data: dict):
-    if "keys" in data:
-        if type(data["keys"]) != dict:
-            raise ValueError(f"Profile '{name}' is corrupted. Invalid 'keys' in profile.yaml.")
-        if "default" in data["keys"]:
-            if type(data["keys"]["default"]) not in [str, list]:
-                raise ValueError(f"Profile '{name}' is corrupted. Invalid 'default' in keys in profile.yaml.")
-            if type(data["keys"]["default"]) == str:
-                __validate_source_ref(path_resolver, name, data, data["keys"]["default"])
-            elif type(data["keys"]["default"]) == list:
-                for source_ref in data["keys"]["default"]:
-                    __validate_source_ref(path_resolver, name, data, source_ref)
-        if "other" in data["keys"]:
-            if type(data["keys"]["other"]) != list:
-                raise ValueError(f"Profile '{name}' is corrupted. Invalid 'other' in keys in profile.yaml.")
-            for key in data["keys"]["other"]:
-                __validate_key(path_resolver, name, data, key)
-
-def __validate_key(path_resolver: PathResolver, name: str, data: dict, key: any):
-    if type(key) not in [str, list, dict]:
-        raise ValueError(f"Profile '{name}' is corrupted. Invalid 'default' in keys in profile.yaml.")
-    if "sound" not in key:
-        raise ValueError(f"Profile '{name}' is corrupted. Missing 'sound' in one or more keys in profile.yaml.")
-    if type(key["sound"]) not in [list, str]:
-        raise ValueError(f"Profile '{name}' is corrupted. Invalid 'sound' in one or more keys in profile.yaml.")
-    if type(key["sound"]) == list:
-        for source_ref in key["sound"]:
-            __validate_source_ref(path_resolver, name, data, source_ref)
-    else:
-        __validate_source_ref(path_resolver, name, data, key["sound"])
-    pass
-
-def __validate_source_ref(path_resolver: PathResolver, name: str, data: dict, source_ref: any):
-    if type(source_ref) != str:
-        raise ValueError(f"Profile '{name}' is corrupted. Invalid 'sound' in one or more keys in profile.yaml.")
-    if source_ref is None or source_ref not in [source["id"] if "id" in source else None for source in data["sources"]]:
+import os
+
+from keyboardsounds.path_resolver import PathResolver
+
+VALID_PROFILE_TYPES = ["video-extract", "files"]
+SUPPORTED_AUDIO_FORMATS = [".wav", ".mp3", ".WAV", ".MP3"]
+SUPPORTED_VIDEO_FORMATS = [".mp4", ".MP4"]
+
+def validate_profile(path_resolver: PathResolver, data: dict):
+    # Validate Required Generic Keys
+
+    required_keys = ["profile", "sources"]
+    for required_key in required_keys:
+        if required_key not in data:
+            raise ValueError(f"Profile is corrupted. Missing '{required_key}' in profile.yaml.")
+
+    # Validate Profile Metadata
+    data = __validate_meta_data(path_resolver, data)
+    name = data["profile"]["name"]
+
+    # Validate Sources
+    __validate_sources(path_resolver, name, data)
+
+    # Validate Keys
+    __validate_keys(path_resolver, name, data)
+
+    return data
+
+def __validate_meta_data(path_resolver: PathResolver, data: dict) -> str:
+    if "name" not in data["profile"]:
+        raise ValueError(f"Profile is corrupted. Missing 'name' in profile.yaml.")
+    if type(data["profile"]["name"]) != str:
+        raise ValueError(f"Profile is corrupted. 'name' in profile.yaml must be a string.")
+    name = data["profile"]["name"]
+    if "type" in data["profile"]:
+        if data["profile"]["type"] not in VALID_PROFILE_TYPES:
+            raise ValueError(f"Profile '{name}' is corrupted. Invalid 'type' in profile.yaml.")
+    else:
+        data["profile"]["type"] = "files"
+    if "author" in data["profile"]:
+        if type(data["profile"]["author"]) != str:
+            raise ValueError(f"Profile '{name}' is corrupted. Invalid 'author' in profile.yaml.")
+    if "description" in data["profile"]:
+        if type(data["profile"]["description"]) != str:
+            raise ValueError(f"Profile '{name}' is corrupted. Invalid 'description' in profile.yaml.")
+
+    if data["profile"]["type"] == "video-extract":
+        if "video" not in data["profile"]:
+            raise ValueError(f"Profile '{name}' is corrupted. Missing 'video' in profile.yaml.")
+        if type(data["profile"]["video"]) != str:
+            raise ValueError(f"Profile '{name}' is corrupted. Invalid 'video' in profile.yaml.")
+        if not str(data["profile"]["video"]).endswith(tuple(SUPPORTED_VIDEO_FORMATS)):
+            raise ValueError(f"Profile '{name}' is corrupted. Invalid 'video' in profile.yaml.")
+        if not os.path.isfile(path_resolver.get_file_path(data["profile"]["video"])):
+            raise ValueError(f"Profile '{name}' is corrupted. Missing video file '{data['profile']['video']}' in profile folder.")
+    
+    return data
+
+def __validate_sources(path_resolver: PathResolver, name: str, data: dict):
+    if "sources" not in data:
+        raise ValueError(f"Profile '{name}' is corrupted. Missing 'sources' in profile.yaml.")
+    if type(data["sources"]) != list:
+        raise ValueError(f"Profile '{name}' is corrupted. Invalid 'sources' in profile.yaml.")
+    for source in data["sources"]:
+       __validate_source(path_resolver, name, data, source)
+
+def __validate_source(path_resolver: PathResolver, name: str, data: dict, source: any):
+    if type(source) != dict:
+        raise ValueError(f"Profile '{name}' is corrupted. Invalid 'sources' in profile.yaml.")
+    if "id" not in source:
+        raise ValueError(f"Profile '{name}' is corrupted. Missing 'id' one or more source in profile.yaml.")
+
+    if data["profile"]["type"] == "files":
+        if "source" not in source:
+            raise ValueError(f"Profile '{name}' is corrupted. Missing 'source' one or more source in profile.yaml.")
+        if type(source["source"]) not in [dict, str]:
+            raise ValueError(f"Profile '{name}' is corrupted. Invalid 'source' one or more source in profile.yaml.")
+        if type(source["source"]) == dict:
+            if not "press" in source["source"]:
+                raise ValueError(f"Profile '{name}' is corrupted. Missing 'press' in source object of one or more sources in profile.yaml.")
+            if type(source["source"]["press"]) != str:
+                raise ValueError(f"Profile '{name}' is corrupted. Invalid 'press' in source object of one or more sources in profile.yaml.")
+            if not str(source["source"]["press"]).endswith(tuple(SUPPORTED_AUDIO_FORMATS)):
+                raise ValueError(f"Profile '{name}' is corrupted. Invalid 'press' in source object of one or more sources in profile.yaml.")
+            if not os.path.isfile(path_resolver.get_file_path(source["source"]["press"])):
+                raise ValueError(f"Profile '{name}' is corrupted. Missing audio file '{source['source']['press']}' in profile folder.")
+            if "release" in source["source"]:
+                if type(source["source"]["release"]) != str:
+                    raise ValueError(f"Profile '{name}' is corrupted. Invalid 'release' in source object of one or more sources in profile.yaml.")
+                if not str(source["source"]["release"]).endswith(tuple(SUPPORTED_AUDIO_FORMATS)):
+                    raise ValueError(f"Profile '{name}' is corrupted. Invalid 'release' in source object of one or more sources in profile.yaml.")
+                if not os.path.isfile(path_resolver.get_file_path(source["source"]["release"])):
+                    raise ValueError(f"Profile '{name}' is corrupted. Missing audio file '{source['source']['release']}' in profile folder.")
+        elif type(source["source"]) == str:
+            if not str(source["source"]).endswith(tuple(SUPPORTED_AUDIO_FORMATS)):
+                raise ValueError(f"Profile '{name}' is corrupted. Invalid 'source' in one or more sources in profile.yaml.")
+            if not os.path.isfile(path_resolver.get_file_path(source["source"])):
+                raise ValueError(f"Profile '{name}' is corrupted. Missing audio file '{source['source']}' in profile folder.")
+    elif data["profile"]["type"] == "video-extract":
+        if "start" not in source:
+            raise ValueError(f"Profile '{name}' is corrupted. Missing 'start' one or more source in profile.yaml.")
+        if type(source["start"]) != float:
+            raise ValueError(f"Profile '{name}' is corrupted. Invalid 'start' one or more source in profile.yaml.")
+        if "end" not in source:
+            raise ValueError(f"Profile '{name}' is corrupted. Missing 'end' one or more source in profile.yaml.")
+        if type(source["end"]) != float:
+            raise ValueError(f"Profile '{name}' is corrupted. Invalid 'end' one or more source in profile.yaml.")
+
+def __validate_keys(path_resolver: PathResolver, name: str, data: dict):
+    if "keys" in data:
+        if type(data["keys"]) != dict:
+            raise ValueError(f"Profile '{name}' is corrupted. Invalid 'keys' in profile.yaml.")
+        if "default" in data["keys"]:
+            if type(data["keys"]["default"]) not in [str, list]:
+                raise ValueError(f"Profile '{name}' is corrupted. Invalid 'default' in keys in profile.yaml.")
+            if type(data["keys"]["default"]) == str:
+                __validate_source_ref(path_resolver, name, data, data["keys"]["default"])
+            elif type(data["keys"]["default"]) == list:
+                for source_ref in data["keys"]["default"]:
+                    __validate_source_ref(path_resolver, name, data, source_ref)
+        if "other" in data["keys"]:
+            if type(data["keys"]["other"]) != list:
+                raise ValueError(f"Profile '{name}' is corrupted. Invalid 'other' in keys in profile.yaml.")
+            for key in data["keys"]["other"]:
+                __validate_key(path_resolver, name, data, key)
+
+def __validate_key(path_resolver: PathResolver, name: str, data: dict, key: any):
+    if type(key) not in [str, list, dict]:
+        raise ValueError(f"Profile '{name}' is corrupted. Invalid 'default' in keys in profile.yaml.")
+    if "sound" not in key:
+        raise ValueError(f"Profile '{name}' is corrupted. Missing 'sound' in one or more keys in profile.yaml.")
+    if type(key["sound"]) not in [list, str]:
+        raise ValueError(f"Profile '{name}' is corrupted. Invalid 'sound' in one or more keys in profile.yaml.")
+    if type(key["sound"]) == list:
+        for source_ref in key["sound"]:
+            __validate_source_ref(path_resolver, name, data, source_ref)
+    else:
+        __validate_source_ref(path_resolver, name, data, key["sound"])
+    pass
+
+def __validate_source_ref(path_resolver: PathResolver, name: str, data: dict, source_ref: any):
+    if type(source_ref) != str:
+        raise ValueError(f"Profile '{name}' is corrupted. Invalid 'sound' in one or more keys in profile.yaml.")
+    if source_ref is None or source_ref not in [source["id"] if "id" in source else None for source in data["sources"]]:
         raise ValueError(f"Profile '{name}' is corrupted. Invalid 'sound' in one or more keys in profile.yaml.")
```

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/LICENSE` & `keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-black-ink/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Audio samples from https://github.com/tplai/kbsim
-
-Copyright (c) Thomas Lai
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
+Audio samples from https://github.com/tplai/kbsim
+
+Copyright (c) Thomas Lai
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/press_back.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/alpaca/press_back.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/press_enter.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/alpaca/press_enter.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/press_key1.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/alpaca/press_key1.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/press_key2.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/alpaca/press_key2.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/press_key3.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/alpaca/press_key3.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/press_key4.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/alpaca/press_key4.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/press_key5.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/alpaca/press_key5.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/press_space.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/alpaca/press_space.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/profile.yaml` & `keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-black-ink/profile.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-profile:
-  name: alpaca
-  author: kbsim
-  description: Sample of an Alpaca Mechanical Keyboard
-
-sources:
-  - id: key1
-    source:
-      press: press_key1.mp3
-      release: release_key.mp3
-  - id: key2
-    source:
-      press: press_key2.mp3
-      release: release_key.mp3
-  - id: key3
-    source:
-      press: press_key3.mp3
-      release: release_key.mp3
-  - id: key4
-    source:
-      press: press_key4.mp3
-      release: release_key.mp3
-  - id: key5
-    source:
-      press: press_key5.mp3
-      release: release_key.mp3
-  - id: space
-    source:
-      press: press_space.mp3
-      release: release_space.mp3
-  - id: enter
-    source:
-      press: press_enter.mp3
-      release: release_enter.mp3
-  - id: back
-    source:
-      press: press_back.mp3
-      release: release_back.mp3
-
-keys:
-  default: [ key1, key2, key3, key4, key5 ]
-  other:
-    - sound: back
-      keys: [ backspace, delete ]
-    - sound: enter
-      keys: [ enter ]
-    - sound: space
-      keys: [ space ]
+profile:
+  name: gateron-black-ink
+  author: kbsim
+  description: Sample of Gateron Black Ink key switches
+
+sources:
+  - id: key1
+    source:
+      press: press_key1.mp3
+      release: release_key.mp3
+  - id: key2
+    source:
+      press: press_key2.mp3
+      release: release_key.mp3
+  - id: key3
+    source:
+      press: press_key3.mp3
+      release: release_key.mp3
+  - id: key4
+    source:
+      press: press_key4.mp3
+      release: release_key.mp3
+  - id: key5
+    source:
+      press: press_key5.mp3
+      release: release_key.mp3
+  - id: space
+    source:
+      press: press_space.mp3
+      release: release_space.mp3
+  - id: enter
+    source:
+      press: press_enter.mp3
+      release: release_enter.mp3
+  - id: back
+    source:
+      press: press_back.mp3
+      release: release_back.mp3
+
+keys:
+  default: [ key1, key2, key3, key4, key5 ]
+  other:
+    - sound: back
+      keys: [ backspace, delete ]
+    - sound: enter
+      keys: [ enter ]
+    - sound: space
+      keys: [ space ]
```

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/release_back.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/alpaca/release_back.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/release_enter.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/alpaca/release_enter.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/release_key.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/alpaca/release_key.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/alpaca/release_space.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/alpaca/release_space.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/LICENSE` & `keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-red-ink/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Audio samples from https://github.com/tplai/kbsim
-
-Copyright (c) Thomas Lai
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
+Audio samples from https://github.com/tplai/kbsim
+
+Copyright (c) Thomas Lai
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/press_back.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-black-ink/press_back.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/press_enter.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-black-ink/press_enter.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/press_key1.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-black-ink/press_key1.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/press_key2.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-black-ink/press_key2.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/press_key3.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-black-ink/press_key3.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/press_key4.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-black-ink/press_key4.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/press_key5.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-black-ink/press_key5.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/press_space.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-black-ink/press_space.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/release_back.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-black-ink/release_back.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/release_enter.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-black-ink/release_enter.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/release_key.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-black-ink/release_key.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-black-ink/release_space.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-black-ink/release_space.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/LICENSE` & `keyboardsounds-5.7.6/keyboardsounds/profiles/holy-panda/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Audio samples from https://github.com/tplai/kbsim
-
-Copyright (c) Thomas Lai
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
+Audio samples from https://github.com/tplai/kbsim
+
+Copyright (c) Thomas Lai
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/press_back.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-red-ink/press_back.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/press_enter.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-red-ink/press_enter.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/press_key1.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-red-ink/press_key1.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/press_key2.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-red-ink/press_key2.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/press_key3.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-red-ink/press_key3.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/press_key4.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-red-ink/press_key4.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/press_key5.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-red-ink/press_key5.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/press_space.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-red-ink/press_space.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/release_back.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-red-ink/release_back.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/release_enter.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-red-ink/release_enter.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/release_key.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-red-ink/release_key.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/gateron-red-ink/release_space.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/gateron-red-ink/release_space.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/LICENSE` & `keyboardsounds-5.7.6/keyboardsounds/profiles/mx-black/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Audio samples from https://github.com/tplai/kbsim
-
-Copyright (c) Thomas Lai
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
+Audio samples from https://github.com/tplai/kbsim
+
+Copyright (c) Thomas Lai
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/press_back.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/holy-panda/press_back.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/press_enter.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/holy-panda/press_enter.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/press_key1.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/holy-panda/press_key1.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/press_key2.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/holy-panda/press_key2.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/press_key3.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/holy-panda/press_key3.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/press_key4.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/holy-panda/press_key4.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/press_key5.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/holy-panda/press_key5.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/press_space.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/holy-panda/press_space.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/release_back.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/holy-panda/release_back.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/release_enter.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/holy-panda/release_enter.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/release_key.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/holy-panda/release_key.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/holy-panda/release_space.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/holy-panda/release_space.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/ios/ios-video-recording.mp4` & `keyboardsounds-5.7.6/keyboardsounds/profiles/ios/ios-video-recording.mp4`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/ios/profile.yaml` & `keyboardsounds-5.7.6/keyboardsounds/profiles/ios/profile.yaml`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-profile:
-  name: ios
-  author: Apple, Inc. (Sampled)
-  type: video-extract
-  video: ios-video-recording.mp4
-  description: Simulates the sounds made by an iPhone or iPad keyboard.
-
-sources:
-  - id: standard_key_sound
-    start: 3.377
-    end: 3.392
-  - id: alternative_key_sound
-    start: 5.050
-    end: 5.073
-  - id: back_key_sound
-    start: 6.723
-    end: 6.766
-
-keys:
-  default: standard_key_sound
-  other:
-    - sound: alternative_key_sound
-      keys: [
-        space, alt, ctrl,
-        shift, tab, enter,
-        insert, home, page_up,
-        page_down, delete, end
-      ]
-    - sound: back_key_sound
-      keys: [ backspace ]
+profile:
+  name: ios
+  author: Apple, Inc. (Sampled)
+  type: video-extract
+  video: ios-video-recording.mp4
+  description: Simulates the sounds made by an iPhone or iPad keyboard.
+
+sources:
+  - id: standard_key_sound
+    start: 3.377
+    end: 3.392
+  - id: alternative_key_sound
+    start: 5.050
+    end: 5.073
+  - id: back_key_sound
+    start: 6.723
+    end: 6.766
+
+keys:
+  default: standard_key_sound
+  other:
+    - sound: alternative_key_sound
+      keys: [
+        space, alt, ctrl,
+        shift, tab, enter,
+        insert, home, page_up,
+        page_down, delete, end
+      ]
+    - sound: back_key_sound
+      keys: [ backspace ]
```

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/LICENSE` & `keyboardsounds-5.7.6/keyboardsounds/profiles/mx-blue/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Audio samples from https://github.com/tplai/kbsim
-
-Copyright (c) Thomas Lai
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
+Audio samples from https://github.com/tplai/kbsim
+
+Copyright (c) Thomas Lai
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/press_back.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/mx-black/press_back.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/press_enter.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/mx-black/press_enter.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/press_key1.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/mx-black/press_key1.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/press_key2.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/mx-black/press_key2.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/press_key3.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/mx-black/press_key3.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/press_key4.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/mx-black/press_key4.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/press_key5.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/mx-black/press_key5.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/press_space.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/mx-black/press_space.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/release_back.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/mx-black/release_back.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/release_enter.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/mx-black/release_enter.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/release_key.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/mx-black/release_key.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-black/release_space.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/mx-black/release_space.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-blue/LICENSE` & `keyboardsounds-5.7.6/keyboardsounds/profiles/mx-brown/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Audio samples from https://github.com/tplai/kbsim
-
-Copyright (c) Thomas Lai
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
+Audio samples from https://github.com/tplai/kbsim
+
+Copyright (c) Thomas Lai
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-blue/press_key1.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/mx-blue/press_key1.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-blue/press_key2.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/mx-blue/press_key2.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-blue/press_key3.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/mx-blue/press_key3.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-blue/press_key4.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/mx-blue/press_key4.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-blue/press_key5.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/mx-blue/press_key5.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-blue/release.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/mx-blue/release.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/LICENSE` & `keyboardsounds-5.7.6/LICENSE`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,21 @@
-Audio samples from https://github.com/tplai/kbsim
-
-Copyright (c) Thomas Lai
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+MIT License
+
+Copyright (c) 2022 Nathan Fiscaletti
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/press_back.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/mx-brown/press_back.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/press_enter.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/mx-brown/press_enter.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/press_key1.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/mx-brown/press_key1.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/press_key2.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/mx-brown/press_key2.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/press_key3.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/mx-brown/press_key3.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/press_key4.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/mx-brown/press_key4.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/press_key5.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/mx-brown/press_key5.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/press_space.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/mx-brown/press_space.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/release_back.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/mx-brown/release_back.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/release_enter.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/mx-brown/release_enter.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/release_key.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/mx-brown/release_key.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-brown/release_space.mp3` & `keyboardsounds-5.7.6/keyboardsounds/profiles/mx-brown/release_space.mp3`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-1.wav` & `keyboardsounds-5.7.6/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-1.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-2.wav` & `keyboardsounds-5.7.6/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-2.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-3.wav` & `keyboardsounds-5.7.6/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-3.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-4.wav` & `keyboardsounds-5.7.6/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-4.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-5.wav` & `keyboardsounds-5.7.6/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-5.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-6.wav` & `keyboardsounds-5.7.6/keyboardsounds/profiles/mx-speed-silver/mx-speed-silver-6.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/back.wav` & `keyboardsounds-5.7.6/keyboardsounds/profiles/telios-v2/back.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/caps.wav` & `keyboardsounds-5.7.6/keyboardsounds/profiles/telios-v2/caps.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/ctrl.wav` & `keyboardsounds-5.7.6/keyboardsounds/profiles/telios-v2/ctrl.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/ent.wav` & `keyboardsounds-5.7.6/keyboardsounds/profiles/telios-v2/ent.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/key1.wav` & `keyboardsounds-5.7.6/keyboardsounds/profiles/telios-v2/key1.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/key2.wav` & `keyboardsounds-5.7.6/keyboardsounds/profiles/telios-v2/key2.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/key3.wav` & `keyboardsounds-5.7.6/keyboardsounds/profiles/telios-v2/key3.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/key4.wav` & `keyboardsounds-5.7.6/keyboardsounds/profiles/telios-v2/key4.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/key5.wav` & `keyboardsounds-5.7.6/keyboardsounds/profiles/telios-v2/key5.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/key6.wav` & `keyboardsounds-5.7.6/keyboardsounds/profiles/telios-v2/key6.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/profile.yaml` & `keyboardsounds-5.7.6/keyboardsounds/profiles/telios-v2/profile.yaml`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-profile:
-  name: telios-v2
-  author: Mechvibes Community
-  description: Sample audio of Telios V2 linear key switches
-
-sources:
-  - id: key1
-    source: key1.wav
-  - id: key2
-    source: key2.wav
-  - id: key3
-    source: key3.wav
-  - id: key4
-    source: key4.wav
-  - id: key5
-    source: key5.wav
-  - id: key6
-    source: key6.wav
-  - id: shift
-    source: shift.wav
-  - id: space
-    source: space.wav
-  - id: tab
-    source: tab.wav
-  - id: enter
-    source: ent.wav
-  - id: ctrl
-    source: ctrl.wav
-  - id: caps
-    source: caps.wav
-  - id: back
-    source: back.wav
-
-keys:
-  default: [ key1, key2, key3, key4, key5, key6 ]
-  other:
-    - sound: back
-      keys: [ backspace, delete ]
-    - sound: caps
-      keys: [ capslock ]
-    - sound: ctrl
-      keys: [ ctrl ]
-    - sound: enter
-      keys: [ enter ]
-    - sound: shift
-      keys: [ shift ]
-    - sound: space
-      keys: [ space ]
-    - sound: tab
-      keys: [ tab ]
+profile:
+  name: telios-v2
+  author: Mechvibes Community
+  description: Sample audio of Telios V2 linear key switches
+
+sources:
+  - id: key1
+    source: key1.wav
+  - id: key2
+    source: key2.wav
+  - id: key3
+    source: key3.wav
+  - id: key4
+    source: key4.wav
+  - id: key5
+    source: key5.wav
+  - id: key6
+    source: key6.wav
+  - id: shift
+    source: shift.wav
+  - id: space
+    source: space.wav
+  - id: tab
+    source: tab.wav
+  - id: enter
+    source: ent.wav
+  - id: ctrl
+    source: ctrl.wav
+  - id: caps
+    source: caps.wav
+  - id: back
+    source: back.wav
+
+keys:
+  default: [ key1, key2, key3, key4, key5, key6 ]
+  other:
+    - sound: back
+      keys: [ backspace, delete ]
+    - sound: caps
+      keys: [ capslock ]
+    - sound: ctrl
+      keys: [ ctrl ]
+    - sound: enter
+      keys: [ enter ]
+    - sound: shift
+      keys: [ shift ]
+    - sound: space
+      keys: [ space ]
+    - sound: tab
+      keys: [ tab ]
```

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/shift.wav` & `keyboardsounds-5.7.6/keyboardsounds/profiles/telios-v2/shift.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/space.wav` & `keyboardsounds-5.7.6/keyboardsounds/profiles/telios-v2/space.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/telios-v2/tab.wav` & `keyboardsounds-5.7.6/keyboardsounds/profiles/telios-v2/tab.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/typewriter/delete.wav` & `keyboardsounds-5.7.6/keyboardsounds/profiles/typewriter/delete.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/typewriter/enter.wav` & `keyboardsounds-5.7.6/keyboardsounds/profiles/typewriter/enter.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/typewriter/key.wav` & `keyboardsounds-5.7.6/keyboardsounds/profiles/typewriter/key.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/typewriter/key2.wav` & `keyboardsounds-5.7.6/keyboardsounds/profiles/typewriter/key2.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds/profiles/typewriter/space.wav` & `keyboardsounds-5.7.6/keyboardsounds/profiles/typewriter/space.wav`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/keyboardsounds.egg-info/PKG-INFO` & `keyboardsounds-5.7.6/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,411 +1,392 @@
-Metadata-Version: 2.1
-Name: keyboardsounds
-Version: 5.7.5
-Summary: Adds the ability to play sounds while typing on any system.
-Author: Nathan Fiscaletti
-Author-email: Nathan Fiscaletti <nate.fiscaletti@gmail.com>
-Project-URL: Homepage, https://github.com/nathan-fiscaletti/keyboardsounds
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pygame==2.5.2
-Requires-Dist: pynput==1.7.6
-Requires-Dist: psutil==5.9.4
-Requires-Dist: imageio-ffmpeg==0.4.6
-Requires-Dist: pyyaml==6.0
-
-# Keyboard Sounds
-
-[![Sponsor Me!](https://img.shields.io/badge/%F0%9F%92%B8-Sponsor%20Me!-blue)](https://github.com/sponsors/nathan-fiscaletti)
-[![PyPI version](https://badge.fury.io/py/keyboardsounds.svg)](https://badge.fury.io/py/keyboardsounds)
-[![GitHub license](https://img.shields.io/github/license/nathan-fiscaletti/keyboardsounds.svg)](https://github.com/nathan-fiscaletti/keyboardsounds/blob/master/LICENSE)
-[![Downloads](https://static.pepy.tech/badge/keyboardsounds)](https://pepy.tech/project/keyboardsounds)
-[![Downloads](https://static.pepy.tech/badge/keyboardsounds/month)](https://pepy.tech/project/keyboardsounds)
-
-This python package will add the ability to play sounds while typing anywhere on your system. You can also create [Custom Profiles](#custom-profiles) for customized audio when typing.
-
-## Installation
-
-### Desktop Application
-
-There is a work-in-progress desktop application available for Keyboard Sounds. You can find information on how to get it up and running on the [Keyboard Sounds Desktop repository](https://github.com/nathan-fiscaletti/keyboardsounds-desktop).
-
-The desktop application still requires the Python package to be installed on your system.
-
-![Desktop App Preview](https://github.com/nathan-fiscaletti/keyboardsounds-desktop/blob/main/preview.png?raw=true)
-
-### Python Package
-
-**Python 3.7** or higher is required for this application to function. See [Download Python](https://www.python.org/downloads/) for more information on installing Python on your system.
-
-Once you have Python installed, you can install this application by running the following command.
-
-```sh
-$ pip install keyboardsounds
-```
-
-## Platform Support
-
-|Windows|Linux|macOS|
-|---|---|---|
-|✅ Supported|✅ Supported|❓ Not Tested|
-
-## Default Sound Profiles
-
-By default, Keyboard Sounds comes with the following profiles pre-loaded.
-
-|Name              | Author                | Description                                             |
-|----------------- | --------------------- | ------------------------------------------------------- |
-|alpaca            | kbsim                 | Sample of an Alpaca Mechanical Keyboard                 |
-|gateron-black-ink | kbsim                 | Sample of Gateron Black Ink key switches                |
-|gateron-red-ink   | kbsim                 | Sample of Gateron Red Ink key switches                  |
-|holy-panda        | kbsim                 | Sample of Holy Panda key switches                       |
-|ios               | Apple, Inc. (Sampled) | Simulates the sounds made by an iPhone or iPad keyboard.|
-|mx-black          | kbsim                 | Sample of Cherry MX Black key switches                  |
-|mx-blue           | kbsim                 | Sample of Cherry MX Blue key switches                   |
-|mx-brown          | kbsim                 | Sample of Cherry MX Brown key switches                  |
-|mx-speed-silver   | Mechvibes Community   | Sample audio of MX Speed Silver key switches            |
-|telios-v2         | Mechvibes Community   | Sample audio of Telios V2 linear key switches           |
-|typewriter        | Mechvibes Community   | Sample audio of an antique typewriter                   |
-
-## Usage
-
-- [Managing the Daemon](#manage-the-daemon)
-- [Managing Application Rules](#managing-application-rules)
-- [Manage Profiles](#manage-profiles)
-- [Custom Profiles](#custom-profiles)
-
-```yaml
-Keyboard Sounds vX.X.X
-
-usage: <keyboardsounds|kbs> <action> [params]
-
-  manage daemon:
-
-    <keyboardsounds|kbs> start [-v <volume>] [-p <profile>]
-    <keyboardsounds|kbs> stop
-    <keyboardsounds|kbs> status [-s]
-
-  manage profiles:
-
-    <keyboardsounds|kbs> <ap|add-profile> -z <zipfile>
-    <keyboardsounds|kbs> <rp|remove-profile> -n <profile>
-    <keyboardsounds|kbs> <lp|list-profiles> [-s] [--remote]
-    <keyboardsounds|kbs> <dp|download-profile> -n <profile>
-    <keyboardsounds|kbs> <bp|build-profile> -d <sound_dir> -o <zip_file>
-
-  manage rules:
-
-    <keyboardsounds|kbs> <ar|add-rule> -r <rule> -a <app>
-    <keyboardsounds|kbs> <rr|remove-rule> -a <app>
-    <keyboardsounds|kbs> <lr|list-rules> [-s]
-    <keyboardsounds|kbs> <sr|set-global-rule> -r <rule>
-    <keyboardsounds|kbs> <gr|get-global-rule> [-s]
-
-  other:
-
-    <keyboardsounds|kbs> [--version|-V]
-
-
-positional arguments:
-  action                The action to perform
-
-options:
-  -h, --help            show this help message and exit
-  -v volume, --volume volume
-                        volume of the sound effects (0-100), default 100
-  -p profile, --profile profile
-                        sound profile to use, default 'ios'
-  -s, --short           consolidate output to a single line of json for scripting
-  -n name, --name name  name of the profile remove
-  -z file, --zip file   path to the zip file containing the profile to add
-  --remote              used with the list-profiles action to list remote profiles
-  -V, --version         show program's version number and exit
-  -d directory, --directory directory
-                        path to the directory containing the sounds to use for the profile
-  -o file, --output file
-                        path to the zip file to create
-  -a app, --app app     absolute path to the application to add the rule for
-  -r rule, --rule rule  rule to apply. must be one of 'enable', 'disable', or 'exclusive'
-```
-
-### Manage the Daemon
-
-**Start the daemon.**
-
-Can also be used to re-start the daemon with an adjusted configuration.
-
-```bash
-# Start with default volume of 100%
-$ kbs start
-```
-
-```bash
-# Start or reconfigure with a volume of 50%
-$ kbs start -v 50
-```
-
-```bash
-# Start or reconfigure with a specific profile
-$ kbs start -p typewriter
-```
-
-**Check the current status of the daemon.**
-
-```bash
-$ kbs status
-```
-
-**Stop the daemon if it is running.**
-
-```bash
-$ kbs stop
-```
-
-### Managing Application Rules
-
-Keyboard Sounds supports the ability to enable or disable the typing sound effects for specific applications. You can also set a global rule that will be used for all applications that do not have a specific rule set.
-
-**⚠️ Application Rules are only available on Windows.**
-
-#### Rule Types
-
-- `enable` - Enable sound effects for the application.
-- `disable` - Disable sound effects for the application.
-- `exclusive` - Only play sound effects for the application.
-
-> The global rule can only be set to `enable` or `disable`. By default, the global rule is set to `enable`.
-
-**Add a new rule for an application.**
-
-```bash
-$ kbs add-rule -r enable -a "C:\Program Files\MyApp\MyApp.exe" 
-```
-
-**Remove a rule for an application.**
-
-```bash
-$ kbs remove-rule -a "C:\Program Files\MyApp\MyApp.exe"
-```
-
-**Lists the currently loaded rules.**
-
-```bash
-$ kbs list-rules
-```
-
-**Set the global rule.**
-
-> The global rule is used as the fallback for any application that does not have a specific rule set. By default, it is set to `enable`.
-
-```bash
-$ kbs set-global-rule -r disable
-```
-
-**Get the current global rule.**
-
-```bash
-$ kbs get-global-rule
-```
-
-### Manage Profiles
-
-**List downloadable profiles.**
-
-```bash
-$ kbs list-profiles --remote
-```
-
-**Lists the currently installed profiles.**
-
-```bash
-$ kbs list-profiles
-```
-
-**Download a profile.**
-
-```bash
-$ kbs download-profile -n myprofile
-```
-
-**Add a new profile to the application.**
-
-```bash
-$ kbs add-profile -z ./my-profile.zip
-```
-
-**Removes a profile from the application.**
-
-```bash
-$ kbs remove-profile -n myprofile
-```
-
-## Custom Profiles
-
-This application supports custom profiles in which you can provide your own WAV or MP3 files to be used for the different keys pressed.
-
-### Creating a Profile
-
-1. Create a new directory containing the sounds you wish to use.
-2. Add a new file to the directory called `profile.yaml`.
-3. Follow the example format below to fill the file in.
-4. Combine the files into a ZIP file. The files must be at the root of the zip file.
-
-You can then load this profile into the application using the `add-profile` action.
-
-> Note: Alternately you can use the `build-profile` action for an environment with built in validation when creating a new profile.
-
-### Adding a profile to the official repository
-
-If you have created a profile that you think others would enjoy, you can submit it to the official repository. To do this, you will need to create a pull request.
-
-1. Fork the repository.
-2. Add your profile to the `profiles` directory.
-3. Create a pull request.
-
-### Example Profile
-
-```yaml
-# General information about your profile, this includes
-# name, author and description.
-#
-# You are only required to provide the "name" field.
-profile:
-  name: my-profile
-  author: Nathan Fiscaletti
-  description: Describe the sounds packaged in this profile
-
-# A list of all audio sources used by this profile each
-# containing an identifier and a source.
-#
-# The source can either be the name of an audio file
-# packaged with this profile OR a dictionary with two
-# keys, one 'press' and one 'release', who's
-# corresponding values are names of audio files
-# packaged with this profile.
-sources:
-  - id: key1
-    source: sound1.wav
-  - id: key2
-    source:
-      press: sound2.wav
-      release: sound3.wav
-
-# An optional mappings of audio sources to
-# particular keys on the keyboard.
-#
-# If you chose to omit the keys section, each time
-# a key is pressed on the keyboard a random sound
-# from the list of audio sources will be used.
-keys:
-  # The default value to use for any key not
-  # mapped elsewhere in the keys object.
-  #
-  # If you provide the keys object, you MUST
-  # provide a value for the default property.
-  #
-  # The value for this property can either be
-  # the ID of one of the sources you defined
-  # above, or an array of IDs.
-  default: [ key1, key2 ]
-
-  # A list of mappings of sources to keyboard keys.
-  other:
-      # The sound to play when one of the keys listed
-      # in the keys array is pressed.
-      #
-      # The value for this property can either be
-      # the ID of one of the sources you defined
-      # above, or an array of IDs.
-    - sound: key1
-      # An array of keys that you can press that this
-      # sound will be mapped to.
-      keys: [ backspace, delete ]
-
-```
-
-## Development
-
-This section is intended for developers who wish to contribute to this project. Follow the steps below to set up your development environment and start contributing.
-
-### Prerequisites
-
-- [Git](https://git-scm.com/downloads)
-- [Python](https://www.python.org/) (version 3.7 or higher)
-- [pip](https://pip.pypa.io/en/stable/installing/) (Python package installer)
-- [virtualenv](https://virtualenv.pypa.io/en/latest/installation.html) (optional, but recommended)
-
-### Setting Up the Development Environment
-
-1. **Clone the Repository**
-
-   Begin by cloning the repository to your local machine using Git:
-
-   ```bash
-   git clone https://github.com/nathan-fiscaletti/keyboardsounds.git
-   ```
-
-2. **Navigate to the Project Directory**
-
-   Change to the project directory:
-
-   ```bash
-   cd keyboardsounds
-   ```
-
-3. **Create a Virtual Environment (Optional)**
-
-   It's recommended to create a virtual environment to keep dependencies required by different projects separate. If you have `virtualenv` installed, create a virtual environment:
-
-   ```bash
-   virtualenv venv
-   ```
-
-   Activate the virtual environment:
-
-   - On Windows:
-     ```cmd
-     .\venv\Scripts\activate
-     ```
-   - On Unix or MacOS:
-     ```bash
-     source venv/bin/activate
-     ```
-
-4. **Install Dependencies**
-
-   Install the project dependencies using `pip`:
-
-   ```bash
-   pip install -r requirements.txt
-   ```
-
-### Running the Project Locally
-
-It is recommended that you install the package in editable mode to allow you to make changes to the code and see the changes reflected in the application.
-
-- To install the package in editable mode, use the following command:
-
-  ```bash
-  pip install -e .
-  ```
-
-  This command will install the package in editable mode, allowing you to make changes to the code and see the changes reflected in the application.
-
-### Contributing
-
-Contributions are what make the open-source community an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.
-
-#### Submitting Pull Requests
-
-1. Fork the repository and create your branch from `master`.
-2. If you've added code, ensure your code adheres to the project's coding conventions.
-4. Update documentation as necessary.
-5. Submit your pull request with a detailed description of your changes.
-
-### Getting Help
-
-Should you have any questions or encounter issues, feel free to open an issue on the repository, and I'll do my best to address it.
+# Keyboard Sounds
+
+[![Sponsor Me!](https://img.shields.io/badge/%F0%9F%92%B8-Sponsor%20Me!-blue)](https://github.com/sponsors/nathan-fiscaletti)
+[![PyPI version](https://badge.fury.io/py/keyboardsounds.svg)](https://badge.fury.io/py/keyboardsounds)
+[![GitHub license](https://img.shields.io/github/license/nathan-fiscaletti/keyboardsounds.svg)](https://github.com/nathan-fiscaletti/keyboardsounds/blob/master/LICENSE)
+[![Downloads](https://static.pepy.tech/badge/keyboardsounds)](https://pepy.tech/project/keyboardsounds)
+[![Downloads](https://static.pepy.tech/badge/keyboardsounds/month)](https://pepy.tech/project/keyboardsounds)
+
+This python package will add the ability to play sounds while typing anywhere on your system. You can also create [Custom Profiles](#custom-profiles) for customized audio when typing.
+
+## Installation
+
+### Desktop Application
+
+There is a work-in-progress desktop application available for Keyboard Sounds. You can find information on how to get it up and running on the [Keyboard Sounds Desktop repository](https://github.com/nathan-fiscaletti/keyboardsounds-desktop).
+
+The desktop application still requires the Python package to be installed on your system.
+
+![Desktop App Preview](https://github.com/nathan-fiscaletti/keyboardsounds-desktop/blob/main/preview.png?raw=true)
+
+### Python Package
+
+**Python** is required for this application to function. See [Download Python](https://www.python.org/downloads/) for more information on installing Python on your system.
+
+Once you have Python installed, you can install this application by running the following command.
+
+```sh
+$ pip install keyboardsounds
+```
+
+## Platform Support
+
+|Windows|Linux|macOS|
+|---|---|---|
+|✅ Supported|✅ Supported|❓ Not Tested|
+
+## Default Sound Profiles
+
+By default, Keyboard Sounds comes with the following profiles pre-loaded.
+
+|Name              | Author                | Description                                             |
+|----------------- | --------------------- | ------------------------------------------------------- |
+|alpaca            | kbsim                 | Sample of an Alpaca Mechanical Keyboard                 |
+|gateron-black-ink | kbsim                 | Sample of Gateron Black Ink key switches                |
+|gateron-red-ink   | kbsim                 | Sample of Gateron Red Ink key switches                  |
+|holy-panda        | kbsim                 | Sample of Holy Panda key switches                       |
+|ios               | Apple, Inc. (Sampled) | Simulates the sounds made by an iPhone or iPad keyboard.|
+|mx-black          | kbsim                 | Sample of Cherry MX Black key switches                  |
+|mx-blue           | kbsim                 | Sample of Cherry MX Blue key switches                   |
+|mx-brown          | kbsim                 | Sample of Cherry MX Brown key switches                  |
+|mx-speed-silver   | Mechvibes Community   | Sample audio of MX Speed Silver key switches            |
+|telios-v2         | Mechvibes Community   | Sample audio of Telios V2 linear key switches           |
+|typewriter        | Mechvibes Community   | Sample audio of an antique typewriter                   |
+
+## Usage
+
+- [Managing the Daemon](#manage-the-daemon)
+- [Managing Application Rules](#managing-application-rules)
+- [Manage Profiles](#manage-profiles)
+- [Custom Profiles](#custom-profiles)
+
+```yaml
+Keyboard Sounds vX.X.X
+
+usage: <keyboardsounds|kbs> <action> [params]
+
+  manage daemon:
+
+    <keyboardsounds|kbs> start [-v <volume>] [-p <profile>]
+    <keyboardsounds|kbs> stop
+    <keyboardsounds|kbs> status [-s]
+
+  manage profiles:
+
+    <keyboardsounds|kbs> <ap|add-profile> -z <zipfile>
+    <keyboardsounds|kbs> <rp|remove-profile> -n <profile>
+    <keyboardsounds|kbs> <lp|list-profiles> [-s] [--remote]
+    <keyboardsounds|kbs> <dp|download-profile> -n <profile>
+    <keyboardsounds|kbs> <bp|build-profile> -d <sound_dir> -o <zip_file>
+
+  manage rules:
+
+    <keyboardsounds|kbs> <ar|add-rule> -r <rule> -a <app>
+    <keyboardsounds|kbs> <rr|remove-rule> -a <app>
+    <keyboardsounds|kbs> <lr|list-rules> [-s]
+    <keyboardsounds|kbs> <sr|set-global-rule> -r <rule>
+    <keyboardsounds|kbs> <gr|get-global-rule> [-s]
+
+  other:
+
+    <keyboardsounds|kbs> [--version|-V]
+
+
+positional arguments:
+  action                The action to perform
+
+options:
+  -h, --help            show this help message and exit
+  -v volume, --volume volume
+                        volume of the sound effects (0-100), default 100
+  -p profile, --profile profile
+                        sound profile to use, default 'ios'
+  -s, --short           consolidate output to a single line of json for scripting
+  -n name, --name name  name of the profile remove
+  -z file, --zip file   path to the zip file containing the profile to add
+  --remote              used with the list-profiles action to list remote profiles
+  -V, --version         show program's version number and exit
+  -d directory, --directory directory
+                        path to the directory containing the sounds to use for the profile
+  -o file, --output file
+                        path to the zip file to create
+  -a app, --app app     absolute path to the application to add the rule for
+  -r rule, --rule rule  rule to apply. must be one of 'enable', 'disable', or 'exclusive'
+```
+
+### Manage the Daemon
+
+**Start the daemon.**
+
+Can also be used to re-start the daemon with an adjusted configuration.
+
+```bash
+# Start with default volume of 100%
+$ kbs start
+```
+
+```bash
+# Start or reconfigure with a volume of 50%
+$ kbs start -v 50
+```
+
+```bash
+# Start or reconfigure with a specific profile
+$ kbs start -p typewriter
+```
+
+**Check the current status of the daemon.**
+
+```bash
+$ kbs status
+```
+
+**Stop the daemon if it is running.**
+
+```bash
+$ kbs stop
+```
+
+### Managing Application Rules
+
+Keyboard Sounds supports the ability to enable or disable the typing sound effects for specific applications. You can also set a global rule that will be used for all applications that do not have a specific rule set.
+
+**⚠️ Application Rules are only available on Windows.**
+
+#### Rule Types
+
+- `enable` - Enable sound effects for the application.
+- `disable` - Disable sound effects for the application.
+- `exclusive` - Only play sound effects for the application.
+
+> The global rule can only be set to `enable` or `disable`. By default, the global rule is set to `enable`.
+
+**Add a new rule for an application.**
+
+```bash
+$ kbs add-rule -r enable -a "C:\Program Files\MyApp\MyApp.exe" 
+```
+
+**Remove a rule for an application.**
+
+```bash
+$ kbs remove-rule -a "C:\Program Files\MyApp\MyApp.exe"
+```
+
+**Lists the currently loaded rules.**
+
+```bash
+$ kbs list-rules
+```
+
+**Set the global rule.**
+
+> The global rule is used as the fallback for any application that does not have a specific rule set. By default, it is set to `enable`.
+
+```bash
+$ kbs set-global-rule -r disable
+```
+
+**Get the current global rule.**
+
+```bash
+$ kbs get-global-rule
+```
+
+### Manage Profiles
+
+**List downloadable profiles.**
+
+```bash
+$ kbs list-profiles --remote
+```
+
+**Lists the currently installed profiles.**
+
+```bash
+$ kbs list-profiles
+```
+
+**Download a profile.**
+
+```bash
+$ kbs download-profile -n myprofile
+```
+
+**Add a new profile to the application.**
+
+```bash
+$ kbs add-profile -z ./my-profile.zip
+```
+
+**Removes a profile from the application.**
+
+```bash
+$ kbs remove-profile -n myprofile
+```
+
+## Custom Profiles
+
+This application supports custom profiles in which you can provide your own WAV or MP3 files to be used for the different keys pressed.
+
+### Creating a Profile
+
+1. Create a new directory containing the sounds you wish to use.
+2. Add a new file to the directory called `profile.yaml`.
+3. Follow the example format below to fill the file in.
+4. Combine the files into a ZIP file. The files must be at the root of the zip file.
+
+You can then load this profile into the application using the `add-profile` action.
+
+> Note: Alternately you can use the `build-profile` action for an environment with built in validation when creating a new profile.
+
+### Adding a profile to the official repository
+
+If you have created a profile that you think others would enjoy, you can submit it to the official repository. To do this, you will need to create a pull request.
+
+1. Fork the repository.
+2. Add your profile to the `profiles` directory.
+3. Create a pull request.
+
+### Example Profile
+
+```yaml
+# General information about your profile, this includes
+# name, author and description.
+#
+# You are only required to provide the "name" field.
+profile:
+  name: my-profile
+  author: Nathan Fiscaletti
+  description: Describe the sounds packaged in this profile
+
+# A list of all audio sources used by this profile each
+# containing an identifier and a source.
+#
+# The source can either be the name of an audio file
+# packaged with this profile OR a dictionary with two
+# keys, one 'press' and one 'release', who's
+# corresponding values are names of audio files
+# packaged with this profile.
+sources:
+  - id: key1
+    source: sound1.wav
+  - id: key2
+    source:
+      press: sound2.wav
+      release: sound3.wav
+
+# An optional mappings of audio sources to
+# particular keys on the keyboard.
+#
+# If you chose to omit the keys section, each time
+# a key is pressed on the keyboard a random sound
+# from the list of audio sources will be used.
+keys:
+  # The default value to use for any key not
+  # mapped elsewhere in the keys object.
+  #
+  # If you provide the keys object, you MUST
+  # provide a value for the default property.
+  #
+  # The value for this property can either be
+  # the ID of one of the sources you defined
+  # above, or an array of IDs.
+  default: [ key1, key2 ]
+
+  # A list of mappings of sources to keyboard keys.
+  other:
+      # The sound to play when one of the keys listed
+      # in the keys array is pressed.
+      #
+      # The value for this property can either be
+      # the ID of one of the sources you defined
+      # above, or an array of IDs.
+    - sound: key1
+      # An array of keys that you can press that this
+      # sound will be mapped to.
+      keys: [ backspace, delete ]
+
+```
+
+## Development
+
+This section is intended for developers who wish to contribute to this project. Follow the steps below to set up your development environment and start contributing.
+
+### Prerequisites
+
+- [Git](https://git-scm.com/downloads)
+- [Python](https://www.python.org/) (version 3.7 or higher)
+- [pip](https://pip.pypa.io/en/stable/installing/) (Python package installer)
+- [virtualenv](https://virtualenv.pypa.io/en/latest/installation.html) (optional, but recommended)
+
+### Setting Up the Development Environment
+
+1. **Clone the Repository**
+
+   Begin by cloning the repository to your local machine using Git:
+
+   ```bash
+   git clone https://github.com/nathan-fiscaletti/keyboardsounds.git
+   ```
+
+2. **Navigate to the Project Directory**
+
+   Change to the project directory:
+
+   ```bash
+   cd keyboardsounds
+   ```
+
+3. **Create a Virtual Environment (Optional)**
+
+   It's recommended to create a virtual environment to keep dependencies required by different projects separate. If you have `virtualenv` installed, create a virtual environment:
+
+   ```bash
+   virtualenv venv
+   ```
+
+   Activate the virtual environment:
+
+   - On Windows:
+     ```cmd
+     .\venv\Scripts\activate
+     ```
+   - On Unix or MacOS:
+     ```bash
+     source venv/bin/activate
+     ```
+
+4. **Install Dependencies**
+
+   Install the project dependencies using `pip`:
+
+   ```bash
+   pip install -r requirements.txt
+   ```
+
+### Running the Project Locally
+
+It is recommended that you install the package in editable mode to allow you to make changes to the code and see the changes reflected in the application.
+
+- To install the package in editable mode, use the following command:
+
+  ```bash
+  pip install -e .
+  ```
+
+  This command will install the package in editable mode, allowing you to make changes to the code and see the changes reflected in the application.
+
+### Contributing
+
+Contributions are what make the open-source community an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.
+
+#### Submitting Pull Requests
+
+1. Fork the repository and create your branch from `master`.
+2. If you've added code, ensure your code adheres to the project's coding conventions.
+4. Update documentation as necessary.
+5. Submit your pull request with a detailed description of your changes.
+
+### Getting Help
+
+Should you have any questions or encounter issues, feel free to open an issue on the repository, and I'll do my best to address it.
```

### Comparing `keyboardsounds-5.7.5/keyboardsounds.egg-info/SOURCES.txt` & `keyboardsounds-5.7.6/keyboardsounds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `keyboardsounds-5.7.5/pyproject.toml` & `keyboardsounds-5.7.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-[project]
-name = "keyboardsounds"
-version = "5.7.5"
-authors = [
-  { name="Nathan Fiscaletti", email="nate.fiscaletti@gmail.com" },
-]
-description = "Adds the ability to play sounds while typing on any system."
-readme = "README.md"
-requires-python = ">=3.7"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-dependencies=[
-  "pygame==2.5.2",
-  "pynput==1.7.6",
-  "psutil==5.9.4",
-  "imageio-ffmpeg==0.4.6",
-  "pyyaml==6.0"
-]
-
-[project.urls]
-"Homepage" = "https://github.com/nathan-fiscaletti/keyboardsounds"
-
-[project.scripts]
-keyboardsounds = "keyboardsounds.main:main"
+[project]
+name = "keyboardsounds"
+version = "5.7.6"
+authors = [
+  { name="Nathan Fiscaletti", email="nate.fiscaletti@gmail.com" },
+]
+description = "Adds the ability to play sounds while typing on any system."
+readme = "README.md"
+requires-python = ">=3.7"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+dependencies=[
+  "pygame==2.5.2",
+  "pynput==1.7.6",
+  "psutil==5.9.4",
+  "imageio-ffmpeg==0.4.6",
+  "pyyaml==6.0.1"
+]
+
+[project.urls]
+"Homepage" = "https://github.com/nathan-fiscaletti/keyboardsounds"
+
+[project.scripts]
+keyboardsounds = "keyboardsounds.main:main"
 kbs = "keyboardsounds.main:main"
```

### Comparing `keyboardsounds-5.7.5/setup.py` & `keyboardsounds-5.7.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-from setuptools import setup
-
-setup(
-    name="keyboardsounds",
-    version="5.7.5",
-    description="Adds the ability to play sounds while typing on any system.",
-    author="Nathan Fiscaletti",
-    author_email="nate.fiscaletti@gmail.com",
-    packages=["keyboardsounds"],
-    install_requires=[
-        "pygame==2.5.2",
-        "pynput==1.7.6",
-        "psutil==5.9.4",
-        "imageio-ffmpeg==0.4.6",
-        "pyyaml==6.0",
-    ],
-    package_data={
-        "keyboardsounds": [
-            "profiles/alpaca/*",
-            "profiles/gateron-black-ink/*",
-            "profiles/gateron-red-ink/*",
-            "profiles/holy-panda/*",
-            "profiles/ios/*",
-            "profiles/mx-black/*",
-            "profiles/mx-blue/*",
-            "profiles/mx-brown/*",
-            "profiles/mx-speed-silver/*",
-            "profiles/telios-v2/*",
-            "profiles/typewriter/*",
-            "external_api/*",
-        ],
-    },
-    entry_points={
-        "console_scripts": [
-            "keyboardsounds = keyboardsounds.main:main",
-            "kbs = keyboardsounds.main:main",
-        ],
-    },
-)
+from setuptools import setup
+
+setup(
+    name="keyboardsounds",
+    version="5.7.6",
+    description="Adds the ability to play sounds while typing on any system.",
+    author="Nathan Fiscaletti",
+    author_email="nate.fiscaletti@gmail.com",
+    packages=["keyboardsounds"],
+    install_requires=[
+        "pygame==2.5.2",
+        "pynput==1.7.6",
+        "psutil==5.9.4",
+        "imageio-ffmpeg==0.4.6",
+        "pyyaml==6.0.1",
+    ],
+    package_data={
+        "keyboardsounds": [
+            "profiles/alpaca/*",
+            "profiles/gateron-black-ink/*",
+            "profiles/gateron-red-ink/*",
+            "profiles/holy-panda/*",
+            "profiles/ios/*",
+            "profiles/mx-black/*",
+            "profiles/mx-blue/*",
+            "profiles/mx-brown/*",
+            "profiles/mx-speed-silver/*",
+            "profiles/telios-v2/*",
+            "profiles/typewriter/*",
+            "external_api/*",
+        ],
+    },
+    entry_points={
+        "console_scripts": [
+            "keyboardsounds = keyboardsounds.main:main",
+            "kbs = keyboardsounds.main:main",
+        ],
+    },
+)
```

