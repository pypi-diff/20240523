# Comparing `tmp/VanityMnem-0.0.1.tar.gz` & `tmp/VanityMnem-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VanityMnem-0.0.1.tar", last modified: Tue Sep  6 10:02:48 2022, max compression
+gzip compressed data, was "VanityMnem-0.0.2.tar", last modified: Thu May 23 19:46:19 2024, max compression
```

## Comparing `VanityMnem-0.0.1.tar` & `VanityMnem-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2022-09-06 10:02:48.669222 VanityMnem-0.0.1/
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     1072 2022-05-13 13:04:11.000000 VanityMnem-0.0.1/LICENSE
--rw-rw-r--   0 valerio   (1000) valerio   (1000)       16 2022-08-30 13:45:00.000000 VanityMnem-0.0.1/MANIFEST.in
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     9859 2022-09-06 10:02:48.669222 VanityMnem-0.0.1/PKG-INFO
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     9450 2022-05-13 13:04:11.000000 VanityMnem-0.0.1/README.md
-drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2022-09-06 10:02:48.669222 VanityMnem-0.0.1/VanityMnem.egg-info/
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     9859 2022-09-06 10:02:48.000000 VanityMnem-0.0.1/VanityMnem.egg-info/PKG-INFO
--rw-rw-r--   0 valerio   (1000) valerio   (1000)      258 2022-09-06 10:02:48.000000 VanityMnem-0.0.1/VanityMnem.egg-info/SOURCES.txt
--rw-rw-r--   0 valerio   (1000) valerio   (1000)        1 2022-09-06 10:02:48.000000 VanityMnem-0.0.1/VanityMnem.egg-info/dependency_links.txt
--rw-rw-r--   0 valerio   (1000) valerio   (1000)       47 2022-09-06 10:02:48.000000 VanityMnem-0.0.1/VanityMnem.egg-info/entry_points.txt
--rw-rw-r--   0 valerio   (1000) valerio   (1000)       50 2022-09-06 10:02:48.000000 VanityMnem-0.0.1/VanityMnem.egg-info/requires.txt
--rw-rw-r--   0 valerio   (1000) valerio   (1000)       11 2022-09-06 10:02:48.000000 VanityMnem-0.0.1/VanityMnem.egg-info/top_level.txt
--rw-rw-r--   0 valerio   (1000) valerio   (1000)       38 2022-09-06 10:02:48.669222 VanityMnem-0.0.1/setup.cfg
--rw-rw-r--   0 valerio   (1000) valerio   (1000)      928 2022-09-06 10:02:04.000000 VanityMnem-0.0.1/setup.py
--rwxrwxr-x   0 valerio   (1000) valerio   (1000)    10136 2022-08-30 21:22:08.000000 VanityMnem-0.0.1/vanitymnem.py
+drwxr-xr-x   0 valerio   (1000) valerio   (1000)        0 2024-05-23 19:46:19.403638 VanityMnem-0.0.2/
+-rw-r--r--   0 valerio   (1000) valerio   (1000)     1072 2024-05-19 19:07:27.000000 VanityMnem-0.0.2/LICENSE
+-rw-r--r--   0 valerio   (1000) valerio   (1000)       16 2024-05-19 19:07:27.000000 VanityMnem-0.0.2/MANIFEST.in
+-rw-r--r--   0 valerio   (1000) valerio   (1000)     7356 2024-05-23 19:46:19.403638 VanityMnem-0.0.2/PKG-INFO
+-rw-r--r--   0 valerio   (1000) valerio   (1000)     6947 2024-05-19 19:07:27.000000 VanityMnem-0.0.2/README.md
+drwxr-xr-x   0 valerio   (1000) valerio   (1000)        0 2024-05-23 19:46:19.403638 VanityMnem-0.0.2/VanityMnem.egg-info/
+-rw-r--r--   0 valerio   (1000) valerio   (1000)     7356 2024-05-23 19:46:19.000000 VanityMnem-0.0.2/VanityMnem.egg-info/PKG-INFO
+-rw-r--r--   0 valerio   (1000) valerio   (1000)      258 2024-05-23 19:46:19.000000 VanityMnem-0.0.2/VanityMnem.egg-info/SOURCES.txt
+-rw-r--r--   0 valerio   (1000) valerio   (1000)        1 2024-05-23 19:46:19.000000 VanityMnem-0.0.2/VanityMnem.egg-info/dependency_links.txt
+-rw-r--r--   0 valerio   (1000) valerio   (1000)       47 2024-05-23 19:46:19.000000 VanityMnem-0.0.2/VanityMnem.egg-info/entry_points.txt
+-rw-r--r--   0 valerio   (1000) valerio   (1000)       50 2024-05-23 19:46:19.000000 VanityMnem-0.0.2/VanityMnem.egg-info/requires.txt
+-rw-r--r--   0 valerio   (1000) valerio   (1000)       11 2024-05-23 19:46:19.000000 VanityMnem-0.0.2/VanityMnem.egg-info/top_level.txt
+-rw-r--r--   0 valerio   (1000) valerio   (1000)       38 2024-05-23 19:46:19.403638 VanityMnem-0.0.2/setup.cfg
+-rw-r--r--   0 valerio   (1000) valerio   (1000)      928 2024-05-23 19:44:55.000000 VanityMnem-0.0.2/setup.py
+-rwxr-xr-x   0 valerio   (1000) valerio   (1000)    10136 2024-05-19 19:07:27.000000 VanityMnem-0.0.2/vanitymnem.py
```

### Comparing `VanityMnem-0.0.1/LICENSE` & `VanityMnem-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `VanityMnem-0.0.1/PKG-INFO` & `VanityMnem-0.0.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,177 +1,119 @@
-Metadata-Version: 2.1
-Name: VanityMnem
-Version: 0.0.1
-Summary: create your vanity mnemonics
-Home-page: https://github.com/valerio-vaccaro/vanitymnem
-Author: Valerio Vaccaro
-Author-email: valerio.vaccaro@gmail.com
-License: MIT
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Vanitymnem
 ```
 '##::::'##::::'###::::'##::: ##:'####:'########:'##:::'##:'##::::'##:'##::: ##:'########:'##::::'##:
  ##:::: ##:::'## ##::: ###:: ##:. ##::... ##..::. ##:'##:: ###::'###: ###:: ##: ##.....:: ###::'###:
  ##:::: ##::'##:. ##:: ####: ##:: ##::::: ##:::::. ####::: ####'####: ####: ##: ##::::::: ####'####:
  ##:::: ##:'##:::. ##: ## ## ##:: ##::::: ##::::::. ##:::: ## ### ##: ## ## ##: ######::: ## ### ##:
 . ##:: ##:: #########: ##. ####:: ##::::: ##::::::: ##:::: ##. #: ##: ##. ####: ##...:::: ##. #: ##:
 :. ## ##::: ##.... ##: ##:. ###:: ##::::: ##::::::: ##:::: ##:.:: ##: ##:. ###: ##::::::: ##:.:: ##:
 ::. ###:::: ##:::: ##: ##::. ##:'####:::: ##::::::: ##:::: ##:::: ##: ##::. ##: ########: ##:::: ##:
 :::...:::::..:::::..::..::::..::....:::::..::::::::..:::::..:::::..::..::::..::........::..:::::..::
-                  VanityMnem - create your vanity mnemonics - 2020 Valerio Vaccaro
-                           https://github.com/valerio-vaccaro/vanitymnem
+                  VanityMnem - create your vanity mnemonics - 2020-2022 Valerio Vaccaro
+                         https://github.com/valerio-vaccaro/vanitymnem
 ```
 
 Create a valid Bitcoin mnemonic with a vanity address in a specific derivation.
 
 Hey this is a PoC! I take no responsibility if you lose your bitcoins using this
 program! Be careful and use testnet!
 
 ## Install
-You will need python3 and virtualenv plus **only one** external library
-(libwally).
-
-Create a virtual environment and load it.
+You can install using pip.
 
 ```
-virtualenv -p python3 venv3
-. venv3/bin/activate
+pip install vanitymnem
 ```
 
-Install dependencies.
-
-```
-pip install -r requirements.txt
-```
-
-You are ready!
-
 ## Usage
 
-Just call the script `vanitymnem.py` with
+Just call the program  `vanitymnem` with
 
 ```
-usage: vanitymnem.py [-h] [-v] [-n NETWORK] [-p PATTERN] [-d DERIVATION]
-                     [-c CHILDREN] (--hardened | --no-hardened) [-a ADDRESS]
+vanitymnem -h
+usage: vanitymnem [-h] [-v] [-n NETWORK] [-p PATTERN] [-P PASSPHRASE] [-t TWELVE] [-c CHILDREN] [-a ADDRESS]
 
-Create a valid Bitcoin mnemonic with a vanity address in a specific
-derivation.
+Create a valid Bitcoin mnemonic with a vanity address in a specific derivation.
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   -v, --verbose         Be more verbose. Can be used multiple times.
   -n NETWORK, --network NETWORK
                         main, test (default=test)
   -p PATTERN, --pattern PATTERN
                         Regex for pattern
-  -d DERIVATION, --derivation DERIVATION
-                        Base derivation (default=m/44'/0'/0')
+  -P PASSPHRASE, --passphrase PASSPHRASE
+                        Passphrase
+  -t TWELVE, --twelve TWELVE
+                        Twelve words (if false a twentyfour words mnemonic will be returned)
   -c CHILDREN, --children CHILDREN
-                        Check in children derivations from 0 to this value
-                        (default=100).
-  --hardened            Add for have hardened child.
-  --no-hardened         Add for have not hardened child.
+                        Check in children derivations from 0 to this value (default=100).
   -a ADDRESS, --address ADDRESS
-                        native_segwit, nested_segwit or legacy
-                        (default=native_segwit).
-```
-
-### Examples
-
-Generate a mnemonic with a derivation with beef (with upper or lower case chars)
-in a mainnet legacy address (check on first 1000 derivations hardened).
+                        native_segwit, nested_segwit or legacy (default=native_segwit).
 
+MIT License - Copyright (c) 2020 Valerio Vaccaro
 ```
-python vanitymnem.py -p "^.*[bB][eE][eE][fF]" -n main -c 1000  --hardened -a legacy -v
 
-'##::::'##::::'###::::'##::: ##:'####:'########:'##:::'##:'##::::'##:'##::: ##:'########:'##::::'##:
- ##:::: ##:::'## ##::: ###:: ##:. ##::... ##..::. ##:'##:: ###::'###: ###:: ##: ##.....:: ###::'###:
- ##:::: ##::'##:. ##:: ####: ##:: ##::::: ##:::::. ####::: ####'####: ####: ##: ##::::::: ####'####:
- ##:::: ##:'##:::. ##: ## ## ##:: ##::::: ##::::::. ##:::: ## ### ##: ## ## ##: ######::: ## ### ##:
-. ##:: ##:: #########: ##. ####:: ##::::: ##::::::: ##:::: ##. #: ##: ##. ####: ##...:::: ##. #: ##:
-:. ## ##::: ##.... ##: ##:. ###:: ##::::: ##::::::: ##:::: ##:.:: ##: ##:. ###: ##::::::: ##:.:: ##:
-::. ###:::: ##:::: ##: ##::. ##:'####:::: ##::::::: ##:::: ##:::: ##: ##::. ##: ########: ##:::: ##:
-:::...:::::..:::::..::..::::..::....:::::..::::::::..:::::..:::::..::..::::..::........::..:::::..::
-                  VanityMnem - create your vanity mnemonics - 2020 Valerio Vaccaro
-                           https://github.com/valerio-vaccaro/vanitymnem
-::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
-  Processed 12 mnemonics in 2 seconds (6 mnemonics per second).
-::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
-Tested mnemonics:      12
-::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
-Seed:                  7bcce0a77871e3a4a77ad5b264ab95311d40de669b1b7547318ad78b88e5d5446638accf0ddf39e513d63dc4da64c0f434106767c65b3ab55170024e287f8fd1
-Mnemonic:              bronze hint primary cause gesture basic feel glove regular layer unveil acid magnet glance disease sell wood excite crash lawsuit rebuild awesome stock price
-Master key:            xprv9s21ZrQH143K4bQ5Uy3zPXVqm7wzrHLCCPZawCx498NW9wU9EaZsoZuZbHyxWBdqNUovrZz69cfiV2r9BbYyE2JpNYK4k8TMPBU1pF6c7sa
-Derivation:            m/44'/0'/0'/790'
-Legacy address:        1JeKLTEJD32ufTZ7ypZsEcPfBeEFppYShu
-::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
-```
+### Examples
 
-The same in testnet but not hardened.
+Generate a mnemonic with a derivation with beef (with upper or lower case chars) in a mainnet legacy address (check on first 1000 derivations).
 
 ```
-vanitymnem % python vanitymnem.py -p "^.*[bB][eE][eE][fF]" -n test -c 1000  --no-hardened -a legacy -v
+vanitymnem -p "^.*[bB][eE][eE][fF]" -n main -c 1000  -a legacy -v
 
 '##::::'##::::'###::::'##::: ##:'####:'########:'##:::'##:'##::::'##:'##::: ##:'########:'##::::'##:
  ##:::: ##:::'## ##::: ###:: ##:. ##::... ##..::. ##:'##:: ###::'###: ###:: ##: ##.....:: ###::'###:
  ##:::: ##::'##:. ##:: ####: ##:: ##::::: ##:::::. ####::: ####'####: ####: ##: ##::::::: ####'####:
  ##:::: ##:'##:::. ##: ## ## ##:: ##::::: ##::::::. ##:::: ## ### ##: ## ## ##: ######::: ## ### ##:
 . ##:: ##:: #########: ##. ####:: ##::::: ##::::::: ##:::: ##. #: ##: ##. ####: ##...:::: ##. #: ##:
 :. ## ##::: ##.... ##: ##:. ###:: ##::::: ##::::::: ##:::: ##:.:: ##: ##:. ###: ##::::::: ##:.:: ##:
 ::. ###:::: ##:::: ##: ##::. ##:'####:::: ##::::::: ##:::: ##:::: ##: ##::. ##: ########: ##:::: ##:
 :::...:::::..:::::..::..::::..::....:::::..::::::::..:::::..:::::..::..::::..::........::..:::::..::
-                  VanityMnem - create your vanity mnemonics - 2020 Valerio Vaccaro
-                           https://github.com/valerio-vaccaro/vanitymnem
+                  VanityMnem - create your vanity mnemonics - 2020-2022 Valerio Vaccaro
+                         https://github.com/valerio-vaccaro/vanitymnem
 ::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
-  Processed 16 mnemonics in 3 seconds (6 mnemonics per second).
+  Processed 37 mnemonics in 6 seconds (6 mnemonics per second).
 ::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
-Tested mnemonics:      16
+Tested mnemonics:      37
 ::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
-Seed:                  57422164b2f36dbcffce4038875c91b3e46184ee979716613152f8208fd612b4f0eed07249c9289f740e55c246a7b01c9c563315dcd2181f0f07064f6d3eba9d
-Mnemonic:              culture check elder resemble pony minimum woman people volume february youth weather credit yellow farm coyote virus cream biology category online vivid bus dawn
-Master key:            tprv8ZgxMBicQKsPdV57khs5criFS2bHqVs1SwkvjXzBHWLH6NDSBuZ74uCQrfUPj7QtcXSw2amPm4a7fQcdPp8ZAYUsNLVWHp1ZJfDSvh97hky
-Derivation:            m/44'/0'/0'/253
-Legacy address:        mwFQ7VtuKDBrcLqpaoW2xu2BEefQNtuWAt
+Seed:                  4942f7915d0ca896b0794c3e5db05394f13b6f764d8e3462a8a00a50d26504b28a8da5e5b786e20f9d7fd319b819584bf4fd1fd659a0e30823605f124791643d
+Mnemonic:              punch useful able actor gun coast arrow owner wear fold same scrub outside crisp cause dice inch bar employ lucky artefact soldier buddy whip
+Passphrase:            
+Master key:            xprv9s21ZrQH143K3mYSRVTtrmyNDM7bhTwrhv4Kr8T3j2Z25bmLcdzCGUuuiK2iudotFQsCVFotwtH7eAki9qez9uZZ5Rzc3gPB8fZm6m4G1SC
+Derivation:            m/44'/0'/0'/0/66
+Legacy address:        16HTutTekFFo3UJbuaBeEFcZ6cWokefLss
 ::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
 ```
 
-Generate a mnemonic with a derivation compatible with regex `^.*[vV][aA][lL][eE]`
-in a mainnet legacy address (check on first 100 derivations hardened).
+Generate a 12 words mnemonic with a derivation compatible with regex `^.*[vV][aA][lL][eE]` in mainnet address (check on first 100 derivations hardened) with passphrase test
 
 ```
-python vanitymnem.py -d "m/0'/0'/0'" -v -n main --hardened -a legacy
+vanitymnem -t true -P test -n main -v
 
 '##::::'##::::'###::::'##::: ##:'####:'########:'##:::'##:'##::::'##:'##::: ##:'########:'##::::'##:
  ##:::: ##:::'## ##::: ###:: ##:. ##::... ##..::. ##:'##:: ###::'###: ###:: ##: ##.....:: ###::'###:
  ##:::: ##::'##:. ##:: ####: ##:: ##::::: ##:::::. ####::: ####'####: ####: ##: ##::::::: ####'####:
  ##:::: ##:'##:::. ##: ## ## ##:: ##::::: ##::::::. ##:::: ## ### ##: ## ## ##: ######::: ## ### ##:
 . ##:: ##:: #########: ##. ####:: ##::::: ##::::::: ##:::: ##. #: ##: ##. ####: ##...:::: ##. #: ##:
 :. ## ##::: ##.... ##: ##:. ###:: ##::::: ##::::::: ##:::: ##:.:: ##: ##:. ###: ##::::::: ##:.:: ##:
 ::. ###:::: ##:::: ##: ##::. ##:'####:::: ##::::::: ##:::: ##:::: ##: ##::. ##: ########: ##:::: ##:
 :::...:::::..:::::..::..::::..::....:::::..::::::::..:::::..:::::..::..::::..::........::..:::::..::
-                  VanityMnem - create your vanity mnemonics - 2020 Valerio Vaccaro
-                           https://github.com/valerio-vaccaro/vanitymnem
-
+                  VanityMnem - create your vanity mnemonics - 2020-2022 Valerio Vaccaro
+                         https://github.com/valerio-vaccaro/vanitymnem
 ::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
-  Processed 315 mnemonics in 7 seconds (45 mnemonics per second).
+  Processed 101 mnemonics in 2 seconds (50 mnemonics per second).
 ::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
-Tested mnemonics:      315
+Tested mnemonics:      101
 ::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
-Seed:                  d439433f959aecaad201c18d875b978303279f5aa5b0e910a9e7825326166a013535bd99db212efbae34fbb163ae1a9a2733b1e6c836dd5d6a76aabc76d
-5e8d9
-Mnemonic:              ticket snow winner twin flip where mutual wolf great mother wild useless upset crime toilet consider rose medal notice divi
-de census canoe better include
-Master key:            xprv9s21ZrQH143K2mYECXTUUGtJfpXMbXWwf44xRAXwo6XXVcBJpaZqCZhZG9kxkuAQrSnRMwufhY2AkyGG6ihqHtbqZtvh5jh7g99GBTp1C7s
-Derivation:            m/0'/0'/0'/96'
-Legacy address:        19vbqAd4fwao3RqFvALEdS4nTgfW4ZXiuG
+Seed:                  e1493a1c19f4ec4a0b2f9647b66697a880b44b1c0b209f7bdff02c99e6093908d1dc7faded67ff1d115abfc27e769aa6e4e549481bc0733900cce2af3edcc8c8
+Mnemonic:              hammer throw trick invest circle walk that drink practice admit legal switch
+Passphrase:            test
+Master key:            xprv9s21ZrQH143K2urfneTLs7YSCpg8NkNNuqjCwMKU3g87ggpE6dxLmDNHnjXey4bQKoqZTL2q4Ttu8afUzyXUS8XziUSndNdwKx85ZnZzQXv
+Derivation:            m/84'/0'/0'/0/35
+Native segwit address: bc1qk5srrutmvaletm2l0wt9309d6r3tcuqzgy60st
 ::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
 ```
 
 If you run this example your mnemonics will be different.
 
 ## Check
```

### Comparing `VanityMnem-0.0.1/README.md` & `VanityMnem-0.0.2/vanitymnem.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,164 +1,194 @@
-# Vanitymnem
-```
-'##::::'##::::'###::::'##::: ##:'####:'########:'##:::'##:'##::::'##:'##::: ##:'########:'##::::'##:
- ##:::: ##:::'## ##::: ###:: ##:. ##::... ##..::. ##:'##:: ###::'###: ###:: ##: ##.....:: ###::'###:
- ##:::: ##::'##:. ##:: ####: ##:: ##::::: ##:::::. ####::: ####'####: ####: ##: ##::::::: ####'####:
- ##:::: ##:'##:::. ##: ## ## ##:: ##::::: ##::::::. ##:::: ## ### ##: ## ## ##: ######::: ## ### ##:
-. ##:: ##:: #########: ##. ####:: ##::::: ##::::::: ##:::: ##. #: ##: ##. ####: ##...:::: ##. #: ##:
-:. ## ##::: ##.... ##: ##:. ###:: ##::::: ##::::::: ##:::: ##:.:: ##: ##:. ###: ##::::::: ##:.:: ##:
-::. ###:::: ##:::: ##: ##::. ##:'####:::: ##::::::: ##:::: ##:::: ##: ##::. ##: ########: ##:::: ##:
-:::...:::::..:::::..::..::::..::....:::::..::::::::..:::::..:::::..::..::::..::........::..:::::..::
-                  VanityMnem - create your vanity mnemonics - 2020 Valerio Vaccaro
-                           https://github.com/valerio-vaccaro/vanitymnem
-```
-
-Create a valid Bitcoin mnemonic with a vanity address in a specific derivation.
-
-Hey this is a PoC! I take no responsibility if you lose your bitcoins using this
-program! Be careful and use testnet!
-
-## Install
-You will need python3 and virtualenv plus **only one** external library
-(libwally).
-
-Create a virtual environment and load it.
-
-```
-virtualenv -p python3 venv3
-. venv3/bin/activate
-```
-
-Install dependencies.
-
-```
-pip install -r requirements.txt
-```
-
-You are ready!
-
-## Usage
-
-Just call the script `vanitymnem.py` with
-
-```
-usage: vanitymnem.py [-h] [-v] [-n NETWORK] [-p PATTERN] [-d DERIVATION]
-                     [-c CHILDREN] (--hardened | --no-hardened) [-a ADDRESS]
-
-Create a valid Bitcoin mnemonic with a vanity address in a specific
-derivation.
-
-optional arguments:
-  -h, --help            show this help message and exit
-  -v, --verbose         Be more verbose. Can be used multiple times.
-  -n NETWORK, --network NETWORK
-                        main, test (default=test)
-  -p PATTERN, --pattern PATTERN
-                        Regex for pattern
-  -d DERIVATION, --derivation DERIVATION
-                        Base derivation (default=m/44'/0'/0')
-  -c CHILDREN, --children CHILDREN
-                        Check in children derivations from 0 to this value
-                        (default=100).
-  --hardened            Add for have hardened child.
-  --no-hardened         Add for have not hardened child.
-  -a ADDRESS, --address ADDRESS
-                        native_segwit, nested_segwit or legacy
-                        (default=native_segwit).
-```
-
-### Examples
-
-Generate a mnemonic with a derivation with beef (with upper or lower case chars)
-in a mainnet legacy address (check on first 1000 derivations hardened).
-
-```
-python vanitymnem.py -p "^.*[bB][eE][eE][fF]" -n main -c 1000  --hardened -a legacy -v
-
-'##::::'##::::'###::::'##::: ##:'####:'########:'##:::'##:'##::::'##:'##::: ##:'########:'##::::'##:
- ##:::: ##:::'## ##::: ###:: ##:. ##::... ##..::. ##:'##:: ###::'###: ###:: ##: ##.....:: ###::'###:
- ##:::: ##::'##:. ##:: ####: ##:: ##::::: ##:::::. ####::: ####'####: ####: ##: ##::::::: ####'####:
- ##:::: ##:'##:::. ##: ## ## ##:: ##::::: ##::::::. ##:::: ## ### ##: ## ## ##: ######::: ## ### ##:
-. ##:: ##:: #########: ##. ####:: ##::::: ##::::::: ##:::: ##. #: ##: ##. ####: ##...:::: ##. #: ##:
-:. ## ##::: ##.... ##: ##:. ###:: ##::::: ##::::::: ##:::: ##:.:: ##: ##:. ###: ##::::::: ##:.:: ##:
-::. ###:::: ##:::: ##: ##::. ##:'####:::: ##::::::: ##:::: ##:::: ##: ##::. ##: ########: ##:::: ##:
-:::...:::::..:::::..::..::::..::....:::::..::::::::..:::::..:::::..::..::::..::........::..:::::..::
-                  VanityMnem - create your vanity mnemonics - 2020 Valerio Vaccaro
-                           https://github.com/valerio-vaccaro/vanitymnem
-::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
-  Processed 12 mnemonics in 2 seconds (6 mnemonics per second).
-::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
-Tested mnemonics:      12
-::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
-Seed:                  7bcce0a77871e3a4a77ad5b264ab95311d40de669b1b7547318ad78b88e5d5446638accf0ddf39e513d63dc4da64c0f434106767c65b3ab55170024e287f8fd1
-Mnemonic:              bronze hint primary cause gesture basic feel glove regular layer unveil acid magnet glance disease sell wood excite crash lawsuit rebuild awesome stock price
-Master key:            xprv9s21ZrQH143K4bQ5Uy3zPXVqm7wzrHLCCPZawCx498NW9wU9EaZsoZuZbHyxWBdqNUovrZz69cfiV2r9BbYyE2JpNYK4k8TMPBU1pF6c7sa
-Derivation:            m/44'/0'/0'/790'
-Legacy address:        1JeKLTEJD32ufTZ7ypZsEcPfBeEFppYShu
-::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
-```
+# '##::::'##::::'###::::'##::: ##:'####:'########:'##:::'##:'##::::'##:'##::: ##:'########:'##::::'##:
+#  ##:::: ##:::'## ##::: ###:: ##:. ##::... ##..::. ##:'##:: ###::'###: ###:: ##: ##.....:: ###::'###:
+#  ##:::: ##::'##:. ##:: ####: ##:: ##::::: ##:::::. ####::: ####'####: ####: ##: ##::::::: ####'####:
+#  ##:::: ##:'##:::. ##: ## ## ##:: ##::::: ##::::::. ##:::: ## ### ##: ## ## ##: ######::: ## ### ##:
+# . ##:: ##:: #########: ##. ####:: ##::::: ##::::::: ##:::: ##. #: ##: ##. ####: ##...:::: ##. #: ##:
+# :. ## ##::: ##.... ##: ##:. ###:: ##::::: ##::::::: ##:::: ##:.:: ##: ##:. ###: ##::::::: ##:.:: ##:
+# ::. ###:::: ##:::: ##: ##::. ##:'####:::: ##::::::: ##:::: ##:::: ##: ##::. ##: ########: ##:::: ##:
+# :::...:::::..:::::..::..::::..::....:::::..::::::::..:::::..:::::..::..::::..::........::..:::::..::
+#                 VanityMnem - create your vanity mnemonics - 2020-2022 Valerio Vaccaro
+#                            https://github.com/valerio-vaccaro/vanitymnem
+
+import argparse
+import os
+import wallycore as wally
+import re
+import time
 
-The same in testnet but not hardened.
-
-```
-vanitymnem % python vanitymnem.py -p "^.*[bB][eE][eE][fF]" -n test -c 1000  --no-hardened -a legacy -v
+from colorama import init
+from termcolor import colored
 
+banner = """
 '##::::'##::::'###::::'##::: ##:'####:'########:'##:::'##:'##::::'##:'##::: ##:'########:'##::::'##:
  ##:::: ##:::'## ##::: ###:: ##:. ##::... ##..::. ##:'##:: ###::'###: ###:: ##: ##.....:: ###::'###:
  ##:::: ##::'##:. ##:: ####: ##:: ##::::: ##:::::. ####::: ####'####: ####: ##: ##::::::: ####'####:
  ##:::: ##:'##:::. ##: ## ## ##:: ##::::: ##::::::. ##:::: ## ### ##: ## ## ##: ######::: ## ### ##:
 . ##:: ##:: #########: ##. ####:: ##::::: ##::::::: ##:::: ##. #: ##: ##. ####: ##...:::: ##. #: ##:
 :. ## ##::: ##.... ##: ##:. ###:: ##::::: ##::::::: ##:::: ##:.:: ##: ##:. ###: ##::::::: ##:.:: ##:
 ::. ###:::: ##:::: ##: ##::. ##:'####:::: ##::::::: ##:::: ##:::: ##: ##::. ##: ########: ##:::: ##:
 :::...:::::..:::::..::..::::..::....:::::..::::::::..:::::..:::::..::..::::..::........::..:::::..::
-                  VanityMnem - create your vanity mnemonics - 2020 Valerio Vaccaro
-                           https://github.com/valerio-vaccaro/vanitymnem
-::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
-  Processed 16 mnemonics in 3 seconds (6 mnemonics per second).
-::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
-Tested mnemonics:      16
-::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
-Seed:                  57422164b2f36dbcffce4038875c91b3e46184ee979716613152f8208fd612b4f0eed07249c9289f740e55c246a7b01c9c563315dcd2181f0f07064f6d3eba9d
-Mnemonic:              culture check elder resemble pony minimum woman people volume february youth weather credit yellow farm coyote virus cream biology category online vivid bus dawn
-Master key:            tprv8ZgxMBicQKsPdV57khs5criFS2bHqVs1SwkvjXzBHWLH6NDSBuZ74uCQrfUPj7QtcXSw2amPm4a7fQcdPp8ZAYUsNLVWHp1ZJfDSvh97hky
-Derivation:            m/44'/0'/0'/253
-Legacy address:        mwFQ7VtuKDBrcLqpaoW2xu2BEefQNtuWAt
-::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
-```
-
-Generate a mnemonic with a derivation compatible with regex `^.*[vV][aA][lL][eE]`
-in a mainnet legacy address (check on first 100 derivations hardened).
-
-```
-python vanitymnem.py -d "m/0'/0'/0'" -v -n main --hardened -a legacy
-
-'##::::'##::::'###::::'##::: ##:'####:'########:'##:::'##:'##::::'##:'##::: ##:'########:'##::::'##:
- ##:::: ##:::'## ##::: ###:: ##:. ##::... ##..::. ##:'##:: ###::'###: ###:: ##: ##.....:: ###::'###:
- ##:::: ##::'##:. ##:: ####: ##:: ##::::: ##:::::. ####::: ####'####: ####: ##: ##::::::: ####'####:
- ##:::: ##:'##:::. ##: ## ## ##:: ##::::: ##::::::. ##:::: ## ### ##: ## ## ##: ######::: ## ### ##:
-. ##:: ##:: #########: ##. ####:: ##::::: ##::::::: ##:::: ##. #: ##: ##. ####: ##...:::: ##. #: ##:
-:. ## ##::: ##.... ##: ##:. ###:: ##::::: ##::::::: ##:::: ##:.:: ##: ##:. ###: ##::::::: ##:.:: ##:
-::. ###:::: ##:::: ##: ##::. ##:'####:::: ##::::::: ##:::: ##:::: ##: ##::. ##: ########: ##:::: ##:
-:::...:::::..:::::..::..::::..::....:::::..::::::::..:::::..:::::..::..::::..::........::..:::::..::
-                  VanityMnem - create your vanity mnemonics - 2020 Valerio Vaccaro
-                           https://github.com/valerio-vaccaro/vanitymnem
-
-::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
-  Processed 315 mnemonics in 7 seconds (45 mnemonics per second).
-::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
-Tested mnemonics:      315
-::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
-Seed:                  d439433f959aecaad201c18d875b978303279f5aa5b0e910a9e7825326166a013535bd99db212efbae34fbb163ae1a9a2733b1e6c836dd5d6a76aabc76d
-5e8d9
-Mnemonic:              ticket snow winner twin flip where mutual wolf great mother wild useless upset crime toilet consider rose medal notice divi
-de census canoe better include
-Master key:            xprv9s21ZrQH143K2mYECXTUUGtJfpXMbXWwf44xRAXwo6XXVcBJpaZqCZhZG9kxkuAQrSnRMwufhY2AkyGG6ihqHtbqZtvh5jh7g99GBTp1C7s
-Derivation:            m/0'/0'/0'/96'
-Legacy address:        19vbqAd4fwao3RqFvALEdS4nTgfW4ZXiuG
-::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::
-```
-
-If you run this example your mnemonics will be different.
+                  VanityMnem - create your vanity mnemonics - 2020-2022 Valerio Vaccaro
+                         https://github.com/valerio-vaccaro/vanitymnem"""
 
-## Check
+def str2bool(v):
+    if isinstance(v, bool):
+       return v
+    if v.lower() in ('yes', 'true', 't', 'y', '1'):
+        return True
+    elif v.lower() in ('no', 'false', 'f', 'n', '0'):
+        return False
+    else:
+        raise argparse.ArgumentTypeError('Boolean value expected.')
+
+def main():
+    init()
+    parser = argparse.ArgumentParser(description='Create a valid Bitcoin mnemonic with a vanity address in a specific derivation.', epilog='MIT License - Copyright (c) 2020 Valerio Vaccaro')
+    parser.add_argument('-v', '--verbose', action='count', default=0, help='Be more verbose. Can be used multiple times.')
+    parser.add_argument('-n', '--network', help=' main, test (default=test)', default='test')
+    parser.add_argument('-p', '--pattern', help='Regex for pattern', default='^.*[vV][aA][lL][eE]')
+    parser.add_argument('-P', '--passphrase', help='Passphrase', default='')
+    parser.add_argument('-t', '--twelve', help='Twelve words (if false a twentyfour words mnemonic will be returned)', type=bool, default=False)
+    parser.add_argument('-c', '--children', help='Check in children derivations from 0 to this value (default=100).', type=int, default=100)
+    parser.add_argument('-a', '--address', help='native_segwit, nested_segwit or legacy (default=native_segwit).', default='native_segwit')
+    args = parser.parse_args()
+    print(colored(banner, 'green'))
+
+    # check net
+    if args.network == 'main':
+        master_key_flags = wally.BIP32_VER_MAIN_PRIVATE
+        native_segwit_address_flags = 'bc'
+        nested_segwit_address_flags = wally.WALLY_ADDRESS_VERSION_P2SH_MAINNET
+        legacy_address_flags = wally.WALLY_ADDRESS_VERSION_P2PKH_MAINNET
+    elif args.network == 'test':
+        master_key_flags = wally.BIP32_VER_TEST_PRIVATE
+        native_segwit_address_flags = 'bc'
+        nested_segwit_address_flags = wally.WALLY_ADDRESS_VERSION_P2SH_TESTNET
+        legacy_address_flags = wally.WALLY_ADDRESS_VERSION_P2PKH_TESTNET
+    else:
+        print(colored('Wrong network type, choose between main or test.', 'red'))
+        exit(1)
+
+    # check address
+    if args.address == 'native_segwit':
+        derivation = "m/84'/0'/0'"
+    elif args.address == 'nested_segwit':
+        derivation = "m/49'/0'/0'"
+    elif args.address == 'legacy':
+        derivation = "m/44'/0'/0'"
+    else:
+        print(colored('Wrong address type, choose between native_segwit or nested_segwit or legacy.', 'red'))
+        exit(1)
+    
+    # check external addresses, not change ones
+    derivation = derivation + '/0'
+
+    path = []
+    for c in derivation.split('/'):
+        der = c.split("'")
+        if (der[0] == 'm'):
+            continue
+        if len(der) == 2:
+            path = path + [0x80000000 + int(der[0])]
+        else:
+            path = path + [int(der[0])]
+
+    pattern = re.compile(args.pattern)
+    i = 0
+    start = time.time()
+
+    while(True):
+        i = i + 1
+
+        # get entropy
+        if args.twelve:
+            entropy = os.urandom(16)
+        else:
+            entropy = os.urandom(32)
+
+        # calculate mnemonic
+        mnemonic = wally.bip39_mnemonic_from_bytes(None, entropy)
+
+        # calculate the seed
+        seed = bytearray(64)
+        wally.bip39_mnemonic_to_seed(mnemonic, args.passphrase, seed)
+
+        # calculate master key
+        master_key = wally.bip32_key_from_seed(seed, master_key_flags, wally.BIP32_FLAG_SKIP_HASH)
+        if args.verbose > 1:
+            print(colored('::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::', 'yellow'))
+            print(colored('Seed:                  {}'.format(seed.hex()), 'red'))
+            print(colored('Mnemonic:              {}'.format(mnemonic), 'red'))
+            print(colored('Passphrase:            {}'.format(args.passphrase), 'red'))
+            print(colored('Master key:            {}'.format(wally.bip32_key_to_base58(master_key, 0)), 'yellow'))
+            print(colored('::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::', 'yellow'))
+
+        # derive a children
+        found = False
+        for x in range(0, args.children + 1):
+            child = x
+            derived = wally.bip32_key_from_parent_path(master_key, path + [child],  wally.BIP32_FLAG_KEY_PRIVATE);
+
+            if args.verbose > 1:
+                print(colored('Derivation:            {}/{}'.format(derivation, x), 'yellow'))
+
+            if args.address == 'native_segwit':
+                # calculate native segwit address
+                native_segwit = wally.bip32_key_to_addr_segwit(derived, native_segwit_address_flags, 0);
+                if args.verbose > 1:
+                    print(colored('Native segwit address: {}'.format(native_segwit), 'yellow'))
+                if pattern.match(native_segwit):
+                    found = True
+            if args.address == 'nested_segwit':
+                # calculate nested segwit address - base_58
+                nested_segwit = wally.bip32_key_to_address(derived, wally.WALLY_ADDRESS_TYPE_P2SH_P2WPKH, nested_segwit_address_flags);
+                if args.verbose > 1:
+                    print(colored('Nested segwit addres:  {}'.format(nested_segwit), 'yellow'))
+                if pattern.match(nested_segwit):
+                    found = True
+
+            if args.address == 'legacy':
+                # calculate legacy address - base_58
+                legacy_address = wally.bip32_key_to_address(derived, wally.WALLY_ADDRESS_TYPE_P2PKH, legacy_address_flags);
+                if args.verbose > 1:
+                    print(colored('Legacy address:        {}'.format(legacy_address), 'yellow'))
+                if pattern.match(legacy_address):
+                    found = True
+
+            if args.verbose > 1:
+                print(colored('::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::', 'yellow'))
+
+            if found:
+                break
+
+        if found:
+            break
+
+        if i%1000 == 0:
+            if args.verbose > 0:
+                end = time.time()
+                print(colored('::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::', 'yellow'))
+                print('  Processed {} mnemonics in {} seconds ({} mnemonics per second).'.format(i, round(end-start), round(i/(end-start))))
+
+    end = time.time()
+    if args.verbose > 0:
+        print(colored('::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::', 'yellow'))
+        print(colored('  Processed {} mnemonics in {} seconds ({} mnemonics per second).'.format(i, round(end-start), round(i/(end-start))), 'yellow'))
+        print(colored('::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::', 'yellow'))
+        print(colored('Tested mnemonics:      {}'.format(i), 'yellow'))
+
+    print(colored('::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::', 'yellow'))
+    print(colored('Seed:                  {}'.format(seed.hex()), 'red'))
+    print(colored('Mnemonic:              {}'.format(mnemonic), 'red'))
+    print(colored('Passphrase:            {}'.format(args.passphrase), 'red'))
+    print(colored('Master key:            {}'.format(wally.bip32_key_to_base58(master_key, 0)), 'yellow'))
+    print(colored('Derivation:            {}/{}'.format(derivation, x), 'yellow'))
+    if args.address == 'native_segwit':
+        print(colored('Native segwit address: {}'.format(native_segwit), 'yellow'))
+    if args.address == 'nested_segwit':
+        print(colored('Nested segwit addres:  {}'.format(nested_segwit), 'yellow'))
+    if args.address == 'legacy':
+        print(colored('Legacy address:        {}'.format(legacy_address), 'yellow'))
+    print(colored('::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::', 'yellow'))
 
-You can check generate address using [iancoleman bip39 tool](https://iancoleman.io/bip39/).
+if __name__== "__main__" :
+    main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `VanityMnem-0.0.1/setup.py` & `VanityMnem-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.read()
 
 setup(
     name = 'VanityMnem',
-    version = '0.0.1',
+    version = '0.0.2',
     author = 'Valerio Vaccaro',
     author_email = 'valerio.vaccaro@gmail.com',
     license = 'MIT',
     description = 'create your vanity mnemonics',
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = 'https://github.com/valerio-vaccaro/vanitymnem',
```

