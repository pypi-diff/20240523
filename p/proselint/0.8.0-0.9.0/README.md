# Comparing `tmp/proselint-0.8.0.tar.gz` & `tmp/proselint-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/proselint-0.8.0.tar", last modified: Thu Feb 23 06:09:45 2017, max compression
+gzip compressed data, was "dist/proselint-0.9.0.tar", last modified: Fri Jul 20 21:22:44 2018, max compression
```

## Comparing `proselint-0.8.0.tar` & `proselint-0.9.0.tar`

### file list

```diff
@@ -1,268 +1,269 @@
-drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2017-02-23 06:09:45.000000 proselint-0.8.0/
--rw-r--r--   0 jordansuchow   (501) staff       (20)    40817 2017-02-23 05:27:18.000000 proselint-0.8.0/CHANGELOG.md
--rw-r--r--   0 jordansuchow   (501) staff       (20)     1524 2016-03-21 09:16:14.000000 proselint-0.8.0/LICENSE.md
--rw-r--r--   0 jordansuchow   (501) staff       (20)       41 2017-02-21 04:08:15.000000 proselint-0.8.0/MANIFEST.in
--rw-r--r--   0 jordansuchow   (501) staff       (20)      301 2017-02-23 06:09:45.000000 proselint-0.8.0/PKG-INFO
-drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2017-02-23 06:09:45.000000 proselint-0.8.0/proselint/
--rw-r--r--   0 jordansuchow   (501) staff       (20)     3880 2017-02-21 04:08:15.000000 proselint-0.8.0/proselint/.proselintrc
--rw-r--r--   0 jordansuchow   (501) staff       (20)      108 2016-07-17 03:14:33.000000 proselint-0.8.0/proselint/__init__.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      142 2016-09-05 15:55:22.000000 proselint-0.8.0/proselint/__main__.py
-drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2017-02-23 06:09:45.000000 proselint-0.8.0/proselint/checks/
--rw-r--r--   0 jordansuchow   (501) staff       (20)       65 2016-03-21 09:16:14.000000 proselint-0.8.0/proselint/checks/__init__.py
-drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2017-02-23 06:09:45.000000 proselint-0.8.0/proselint/checks/airlinese/
--rw-r--r--   0 jordansuchow   (501) staff       (20)       17 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/airlinese/__init__.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      584 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/airlinese/misc.py
-drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2017-02-23 06:09:45.000000 proselint-0.8.0/proselint/checks/annotations/
--rw-r--r--   0 jordansuchow   (501) staff       (20)       19 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/annotations/__init__.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      660 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/annotations/misc.py
-drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2017-02-23 06:09:45.000000 proselint-0.8.0/proselint/checks/archaism/
--rw-r--r--   0 jordansuchow   (501) staff       (20)       16 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/archaism/__init__.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     1847 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/archaism/misc.py
-drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2017-02-23 06:09:45.000000 proselint-0.8.0/proselint/checks/cliches/
--rw-r--r--   0 jordansuchow   (501) staff       (20)       21 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/cliches/__init__.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      550 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/cliches/hell.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)    25363 2017-02-21 04:08:15.000000 proselint-0.8.0/proselint/checks/cliches/misc.py
-drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2017-02-23 06:09:45.000000 proselint-0.8.0/proselint/checks/consistency/
--rw-r--r--   0 jordansuchow   (501) staff       (20)       34 2016-03-21 09:16:14.000000 proselint-0.8.0/proselint/checks/consistency/__init__.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      664 2016-04-01 08:30:13.000000 proselint-0.8.0/proselint/checks/consistency/spacing.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     1474 2016-07-25 02:49:19.000000 proselint-0.8.0/proselint/checks/consistency/spelling.py
-drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2017-02-23 06:09:45.000000 proselint-0.8.0/proselint/checks/corporate_speak/
--rw-r--r--   0 jordansuchow   (501) staff       (20)       24 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/corporate_speak/__init__.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     1292 2016-08-10 22:10:05.000000 proselint-0.8.0/proselint/checks/corporate_speak/misc.py
-drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2017-02-23 06:09:45.000000 proselint-0.8.0/proselint/checks/cursing/
--rw-r--r--   0 jordansuchow   (501) staff       (20)       15 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/cursing/__init__.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      710 2016-08-25 05:46:19.000000 proselint-0.8.0/proselint/checks/cursing/filth.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)    24214 2016-08-25 05:46:19.000000 proselint-0.8.0/proselint/checks/cursing/nfl.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      574 2016-08-25 05:46:19.000000 proselint-0.8.0/proselint/checks/cursing/nword.py
-drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2017-02-23 06:09:45.000000 proselint-0.8.0/proselint/checks/dates_times/
--rw-r--r--   0 jordansuchow   (501) staff       (20)       23 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/dates_times/__init__.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     1463 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/dates_times/am_pm.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     1696 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/dates_times/dates.py
-drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2017-02-23 06:09:45.000000 proselint-0.8.0/proselint/checks/hedging/
--rw-r--r--   0 jordansuchow   (501) staff       (20)       15 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/hedging/__init__.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      560 2016-08-25 14:50:15.000000 proselint-0.8.0/proselint/checks/hedging/misc.py
-drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2017-02-23 06:09:45.000000 proselint-0.8.0/proselint/checks/hyperbole/
--rw-r--r--   0 jordansuchow   (501) staff       (20)       17 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/hyperbole/__init__.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      505 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/hyperbole/misc.py
-drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2017-02-23 06:09:45.000000 proselint-0.8.0/proselint/checks/jargon/
--rw-r--r--   0 jordansuchow   (501) staff       (20)       14 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/jargon/__init__.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      691 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/jargon/misc.py
-drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2017-02-23 06:09:45.000000 proselint-0.8.0/proselint/checks/lexical_illusions/
--rw-r--r--   0 jordansuchow   (501) staff       (20)       25 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/lexical_illusions/__init__.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      677 2016-08-04 09:17:49.000000 proselint-0.8.0/proselint/checks/lexical_illusions/misc.py
-drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2017-02-23 06:09:45.000000 proselint-0.8.0/proselint/checks/lgbtq/
--rw-r--r--   0 jordansuchow   (501) staff       (20)       13 2016-07-19 22:45:15.000000 proselint-0.8.0/proselint/checks/lgbtq/__init__.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     1107 2016-07-19 22:45:15.000000 proselint-0.8.0/proselint/checks/lgbtq/offensive_terms.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     1277 2016-07-19 22:45:15.000000 proselint-0.8.0/proselint/checks/lgbtq/terms.py
-drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2017-02-23 06:09:45.000000 proselint-0.8.0/proselint/checks/links/
--rw-r--r--   0 jordansuchow   (501) staff       (20)       20 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/links/__init__.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     1657 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/links/broken.py
-drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2017-02-23 06:09:45.000000 proselint-0.8.0/proselint/checks/malapropisms/
--rw-r--r--   0 jordansuchow   (501) staff       (20)       21 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/malapropisms/__init__.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      599 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/malapropisms/misc.py
-drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2017-02-23 06:09:45.000000 proselint-0.8.0/proselint/checks/misc/
--rw-r--r--   0 jordansuchow   (501) staff       (20)       54 2016-03-21 09:16:14.000000 proselint-0.8.0/proselint/checks/misc/__init__.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      558 2016-08-25 14:50:15.000000 proselint-0.8.0/proselint/checks/misc/apologizing.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      588 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/misc/back_formations.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      588 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/misc/bureaucratese.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      524 2017-02-21 04:08:15.000000 proselint-0.8.0/proselint/checks/misc/but.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     2541 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/misc/capitalization.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      791 2016-04-01 08:30:13.000000 proselint-0.8.0/proselint/checks/misc/chatspeak.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     1282 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/misc/commercialese.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     3486 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/misc/composition.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      522 2016-04-01 08:30:13.000000 proselint-0.8.0/proselint/checks/misc/currency.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      648 2017-02-21 04:08:15.000000 proselint-0.8.0/proselint/checks/misc/debased.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      839 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/misc/false_plurals.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      956 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/misc/greylist.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     1378 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/misc/illogic.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      724 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/misc/inferior_superior.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      787 2017-02-21 04:08:15.000000 proselint-0.8.0/proselint/checks/misc/institution_name.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      783 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/misc/latin.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      718 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/misc/many_a.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      587 2016-08-25 14:50:15.000000 proselint-0.8.0/proselint/checks/misc/metaconcepts.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      705 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/misc/metadiscourse.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      638 2016-08-25 14:50:15.000000 proselint-0.8.0/proselint/checks/misc/narcissism.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     1086 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/misc/not_guilty.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     6975 2017-02-21 04:08:15.000000 proselint-0.8.0/proselint/checks/misc/phrasal_adjectives.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     7587 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/misc/preferred_forms.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      624 2017-02-21 04:08:15.000000 proselint-0.8.0/proselint/checks/misc/pretension.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      553 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/misc/professions.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      530 2017-02-21 04:08:15.000000 proselint-0.8.0/proselint/checks/misc/punctuation.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      578 2016-08-25 14:50:15.000000 proselint-0.8.0/proselint/checks/misc/scare_quotes.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     1495 2017-02-21 04:08:15.000000 proselint-0.8.0/proselint/checks/misc/suddenly.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     1089 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/misc/tense_present.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     2019 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/misc/usage.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     1843 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/misc/waxed.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      460 2016-04-01 09:36:45.000000 proselint-0.8.0/proselint/checks/misc/whence.py
-drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2017-02-23 06:09:45.000000 proselint-0.8.0/proselint/checks/mixed_metaphors/
--rw-r--r--   0 jordansuchow   (501) staff       (20)       23 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/mixed_metaphors/__init__.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     1385 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/mixed_metaphors/misc.py
-drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2017-02-23 06:09:45.000000 proselint-0.8.0/proselint/checks/mondegreens/
--rw-r--r--   0 jordansuchow   (501) staff       (20)       19 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/mondegreens/__init__.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     1089 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/mondegreens/misc.py
-drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2017-02-23 06:09:45.000000 proselint-0.8.0/proselint/checks/needless_variants/
--rw-r--r--   0 jordansuchow   (501) staff       (20)       25 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/needless_variants/__init__.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)    17582 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/needless_variants/misc.py
-drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2017-02-23 06:09:45.000000 proselint-0.8.0/proselint/checks/nonwords/
--rw-r--r--   0 jordansuchow   (501) staff       (20)       16 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/nonwords/__init__.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     2440 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/nonwords/misc.py
-drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2017-02-23 06:09:45.000000 proselint-0.8.0/proselint/checks/oxymorons/
--rw-r--r--   0 jordansuchow   (501) staff       (20)       17 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/oxymorons/__init__.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     1094 2017-02-21 04:08:15.000000 proselint-0.8.0/proselint/checks/oxymorons/misc.py
-drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2017-02-23 06:09:45.000000 proselint-0.8.0/proselint/checks/psychology/
--rw-r--r--   0 jordansuchow   (501) staff       (20)       25 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/psychology/__init__.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     1412 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/psychology/misc.py
-drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2017-02-23 06:09:45.000000 proselint-0.8.0/proselint/checks/redundancy/
--rw-r--r--   0 jordansuchow   (501) staff       (20)       18 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/redundancy/__init__.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)    25077 2016-07-01 10:09:58.000000 proselint-0.8.0/proselint/checks/redundancy/misc.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     1331 2016-09-05 15:55:22.000000 proselint-0.8.0/proselint/checks/redundancy/ras_syndrome.py
-drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2017-02-23 06:09:45.000000 proselint-0.8.0/proselint/checks/security/
--rw-r--r--   0 jordansuchow   (501) staff       (20)       16 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/security/__init__.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      651 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/security/credit_card.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      742 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/security/password.py
-drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2017-02-23 06:09:45.000000 proselint-0.8.0/proselint/checks/sexism/
--rw-r--r--   0 jordansuchow   (501) staff       (20)       14 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/sexism/__init__.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     2567 2017-02-21 04:08:15.000000 proselint-0.8.0/proselint/checks/sexism/misc.py
-drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2017-02-23 06:09:45.000000 proselint-0.8.0/proselint/checks/skunked_terms/
--rw-r--r--   0 jordansuchow   (501) staff       (20)       27 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/skunked_terms/__init__.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      766 2016-09-05 15:55:22.000000 proselint-0.8.0/proselint/checks/skunked_terms/misc.py
-drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2017-02-23 06:09:45.000000 proselint-0.8.0/proselint/checks/spelling/
--rw-r--r--   0 jordansuchow   (501) staff       (20)       16 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/spelling/__init__.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     3696 2016-09-05 15:55:22.000000 proselint-0.8.0/proselint/checks/spelling/able_atable.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     7367 2016-09-05 15:55:22.000000 proselint-0.8.0/proselint/checks/spelling/able_ible.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     1452 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/spelling/athletes.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     2233 2016-09-05 15:55:22.000000 proselint-0.8.0/proselint/checks/spelling/em_im_en_in.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     1516 2016-09-05 15:55:22.000000 proselint-0.8.0/proselint/checks/spelling/er_or.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      529 2016-09-05 15:55:22.000000 proselint-0.8.0/proselint/checks/spelling/in_un.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     6346 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/spelling/misc.py
-drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2017-02-23 06:09:45.000000 proselint-0.8.0/proselint/checks/terms/
--rw-r--r--   0 jordansuchow   (501) staff       (20)       13 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/terms/__init__.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     2440 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/terms/animal_adjectives.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     3331 2016-09-05 15:55:22.000000 proselint-0.8.0/proselint/checks/terms/denizen_labels.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      680 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/terms/eponymous_adjectives.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     2635 2016-07-28 07:15:30.000000 proselint-0.8.0/proselint/checks/terms/venery.py
-drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2017-02-23 06:09:45.000000 proselint-0.8.0/proselint/checks/typography/
--rw-r--r--   0 jordansuchow   (501) staff       (20)       28 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/typography/__init__.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     4722 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/typography/diacritical_marks.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     1130 2016-08-03 23:39:20.000000 proselint-0.8.0/proselint/checks/typography/exclamation.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     2848 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/typography/symbols.py
-drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2017-02-23 06:09:45.000000 proselint-0.8.0/proselint/checks/uncomparables/
--rw-r--r--   0 jordansuchow   (501) staff       (20)       33 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/uncomparables/__init__.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     4239 2016-07-28 07:15:29.000000 proselint-0.8.0/proselint/checks/uncomparables/misc.py
-drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2017-02-23 06:09:45.000000 proselint-0.8.0/proselint/checks/weasel_words/
--rw-r--r--   0 jordansuchow   (501) staff       (20)       20 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/checks/weasel_words/__init__.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      411 2017-02-21 19:36:46.000000 proselint-0.8.0/proselint/checks/weasel_words/misc.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      733 2016-09-05 15:55:22.000000 proselint-0.8.0/proselint/checks/weasel_words/very.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     5168 2017-02-23 04:32:23.000000 proselint-0.8.0/proselint/command_line.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     6095 2016-06-27 17:14:40.000000 proselint-0.8.0/proselint/demo.md
--rw-r--r--   0 jordansuchow   (501) staff       (20)     2681 2016-06-28 08:41:28.000000 proselint-0.8.0/proselint/score.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)    12299 2017-02-21 03:59:11.000000 proselint-0.8.0/proselint/tools.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)       55 2017-02-23 05:27:18.000000 proselint-0.8.0/proselint/version.py
-drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2017-02-23 06:09:45.000000 proselint-0.8.0/proselint.egg-info/
--rw-r--r--   0 jordansuchow   (501) staff       (20)        1 2017-02-23 06:09:44.000000 proselint-0.8.0/proselint.egg-info/dependency_links.txt
--rw-r--r--   0 jordansuchow   (501) staff       (20)       64 2017-02-23 06:09:44.000000 proselint-0.8.0/proselint.egg-info/entry_points.txt
--rw-r--r--   0 jordansuchow   (501) staff       (20)        1 2016-04-06 00:20:12.000000 proselint-0.8.0/proselint.egg-info/not-zip-safe
--rw-r--r--   0 jordansuchow   (501) staff       (20)       47 2016-08-25 14:51:36.000000 proselint-0.8.0/proselint.egg-info/pbr.json
--rw-r--r--   0 jordansuchow   (501) staff       (20)      301 2017-02-23 06:09:44.000000 proselint-0.8.0/proselint.egg-info/PKG-INFO
--rw-r--r--   0 jordansuchow   (501) staff       (20)       17 2017-02-23 06:09:44.000000 proselint-0.8.0/proselint.egg-info/requires.txt
--rw-r--r--   0 jordansuchow   (501) staff       (20)     7607 2017-02-23 06:09:45.000000 proselint-0.8.0/proselint.egg-info/SOURCES.txt
--rw-r--r--   0 jordansuchow   (501) staff       (20)       16 2017-02-23 06:09:44.000000 proselint-0.8.0/proselint.egg-info/top_level.txt
--rw-r--r--   0 jordansuchow   (501) staff       (20)    11173 2017-02-21 04:33:36.000000 proselint-0.8.0/README.md
--rw-r--r--   0 jordansuchow   (501) staff       (20)      270 2017-02-23 06:09:45.000000 proselint-0.8.0/setup.cfg
--rw-r--r--   0 jordansuchow   (501) staff       (20)      747 2016-09-05 03:17:28.000000 proselint-0.8.0/setup.py
-drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2017-02-23 06:09:45.000000 proselint-0.8.0/tests/
--rw-r--r--   0 jordansuchow   (501) staff       (20)       27 2016-03-21 09:16:14.000000 proselint-0.8.0/tests/__init__.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      485 2016-06-28 08:41:28.000000 proselint-0.8.0/tests/_test_version.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     1781 2016-06-28 08:41:28.000000 proselint-0.8.0/tests/check.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      612 2016-08-10 22:10:05.000000 proselint-0.8.0/tests/test_annotations.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      620 2016-08-10 22:10:05.000000 proselint-0.8.0/tests/test_archaism.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     1625 2016-06-28 08:41:28.000000 proselint-0.8.0/tests/test_butterick_symbols.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     5334 2017-02-23 04:32:23.000000 proselint-0.8.0/tests/test_clear_cache.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     1798 2016-06-28 08:41:28.000000 proselint-0.8.0/tests/test_cliches.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      926 2016-07-17 03:14:33.000000 proselint-0.8.0/tests/test_consistency_check.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      676 2016-08-10 22:10:05.000000 proselint-0.8.0/tests/test_consistency_spacing.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      739 2016-08-10 22:10:05.000000 proselint-0.8.0/tests/test_consistency_spelling.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      637 2016-08-10 22:10:05.000000 proselint-0.8.0/tests/test_corporate_speak.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      540 2016-08-25 05:46:19.000000 proselint-0.8.0/tests/test_cursing_filth.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      536 2016-08-25 05:46:19.000000 proselint-0.8.0/tests/test_cursing_nfl.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      527 2016-08-25 05:46:19.000000 proselint-0.8.0/tests/test_cursing_nword.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     2047 2016-08-25 05:46:19.000000 proselint-0.8.0/tests/test_dates_times_am_pm.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     2662 2016-08-25 05:46:19.000000 proselint-0.8.0/tests/test_dates_times_dates.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      108 2016-07-17 03:14:33.000000 proselint-0.8.0/tests/test_demo.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      747 2016-06-28 08:41:28.000000 proselint-0.8.0/tests/test_dfw_uncomparables.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     1900 2016-06-28 08:41:28.000000 proselint-0.8.0/tests/test_existence_check.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      569 2016-06-28 08:41:28.000000 proselint-0.8.0/tests/test_exit_codes.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     1088 2016-06-28 08:41:28.000000 proselint-0.8.0/tests/test_garner_dates.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      551 2016-08-25 05:46:19.000000 proselint-0.8.0/tests/test_hedging.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      537 2016-08-25 05:46:19.000000 proselint-0.8.0/tests/test_hyperbole.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     1182 2016-07-17 03:14:33.000000 proselint-0.8.0/tests/test_illegal_chars.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      540 2016-08-25 05:46:19.000000 proselint-0.8.0/tests/test_jargon.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      866 2016-08-03 23:39:20.000000 proselint-0.8.0/tests/test_leonard.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      580 2016-08-25 05:46:19.000000 proselint-0.8.0/tests/test_lexical_illusions.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      611 2016-07-19 22:45:15.000000 proselint-0.8.0/tests/test_lgbtq_offensive_terms.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      914 2016-07-19 22:45:15.000000 proselint-0.8.0/tests/test_lgbtq_terms.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      571 2016-08-29 16:53:46.000000 proselint-0.8.0/tests/test_malaproprisms.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      552 2017-02-21 04:08:15.000000 proselint-0.8.0/tests/test_misc_apologizing.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      571 2017-02-21 04:08:15.000000 proselint-0.8.0/tests/test_misc_back_formations.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      592 2017-02-21 04:08:15.000000 proselint-0.8.0/tests/test_misc_bureaucratese.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      534 2017-02-21 04:08:15.000000 proselint-0.8.0/tests/test_misc_but.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     1077 2017-02-21 04:08:15.000000 proselint-0.8.0/tests/test_misc_capitalization.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      539 2017-02-21 04:08:15.000000 proselint-0.8.0/tests/test_misc_chatspeak.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      568 2017-02-21 04:08:15.000000 proselint-0.8.0/tests/test_misc_commercialese.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      552 2017-02-21 04:08:15.000000 proselint-0.8.0/tests/test_misc_composition.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      536 2017-02-21 04:08:15.000000 proselint-0.8.0/tests/test_misc_currency.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      543 2017-02-21 04:08:15.000000 proselint-0.8.0/tests/test_misc_debased.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      807 2017-02-21 04:08:15.000000 proselint-0.8.0/tests/test_misc_false_plurals.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      549 2017-02-21 04:08:15.000000 proselint-0.8.0/tests/test_misc_greylist.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     1199 2017-02-21 04:08:15.000000 proselint-0.8.0/tests/test_misc_illogic.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      607 2017-02-21 04:08:15.000000 proselint-0.8.0/tests/test_misc_inferior_superior.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      537 2017-02-21 04:08:15.000000 proselint-0.8.0/tests/test_misc_latin.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      562 2017-02-21 04:08:15.000000 proselint-0.8.0/tests/test_misc_many_a.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      437 2017-02-21 04:08:15.000000 proselint-0.8.0/tests/test_misc_metaconcepts.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      575 2017-02-21 04:08:15.000000 proselint-0.8.0/tests/test_misc_metadiscourse.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      637 2017-02-21 04:08:15.000000 proselint-0.8.0/tests/test_misc_narcissism.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      581 2017-02-21 04:08:15.000000 proselint-0.8.0/tests/test_misc_not_guilty.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      939 2017-02-21 04:08:15.000000 proselint-0.8.0/tests/test_misc_phrasal_adjectives.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      567 2017-02-21 04:08:15.000000 proselint-0.8.0/tests/test_misc_preferred_forms.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      563 2017-02-21 04:08:15.000000 proselint-0.8.0/tests/test_misc_pretension.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      560 2017-02-21 04:08:15.000000 proselint-0.8.0/tests/test_misc_professions.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      545 2017-02-21 04:08:15.000000 proselint-0.8.0/tests/test_misc_punctuation.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      565 2017-02-21 04:08:15.000000 proselint-0.8.0/tests/test_misc_scare_quotes.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      544 2017-02-21 04:08:15.000000 proselint-0.8.0/tests/test_misc_suddenly.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      566 2017-02-21 04:08:15.000000 proselint-0.8.0/tests/test_misc_tense_present.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      409 2017-02-21 04:08:15.000000 proselint-0.8.0/tests/test_misc_usage.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      537 2017-02-21 04:08:15.000000 proselint-0.8.0/tests/test_misc_waxed.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      537 2017-02-21 04:08:15.000000 proselint-0.8.0/tests/test_misc_whence.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      905 2016-08-29 16:53:46.000000 proselint-0.8.0/tests/test_mixed_metaphors.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      615 2016-08-29 16:53:46.000000 proselint-0.8.0/tests/test_mondegreens.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      583 2016-08-29 16:53:46.000000 proselint-0.8.0/tests/test_needless_variants.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      547 2016-08-29 16:53:46.000000 proselint-0.8.0/tests/test_nonwords.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      548 2016-08-29 16:53:46.000000 proselint-0.8.0/tests/test_oxymorons.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     1227 2016-07-17 01:41:11.000000 proselint-0.8.0/tests/test_preferred_forms_check.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     1324 2016-08-29 16:53:46.000000 proselint-0.8.0/tests/test_psychology.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     1445 2016-09-05 15:55:22.000000 proselint-0.8.0/tests/test_redundancy_misc.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      585 2016-09-05 15:55:22.000000 proselint-0.8.0/tests/test_redundancy_ras_syndrome.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      661 2016-09-05 15:55:22.000000 proselint-0.8.0/tests/test_security_credit_card.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      618 2016-09-05 15:55:22.000000 proselint-0.8.0/tests/test_security_password.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      570 2016-09-05 15:55:22.000000 proselint-0.8.0/tests/test_sexism.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      597 2016-09-05 15:55:22.000000 proselint-0.8.0/tests/test_skunked_terms.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      582 2016-09-05 15:55:22.000000 proselint-0.8.0/tests/test_spelling_able_atable.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      563 2016-09-05 15:55:22.000000 proselint-0.8.0/tests/test_spelling_able_ible.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      562 2016-09-05 15:55:22.000000 proselint-0.8.0/tests/test_spelling_athletes.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      572 2016-09-05 15:55:22.000000 proselint-0.8.0/tests/test_spelling_em_im_en_in.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      546 2016-09-05 15:55:22.000000 proselint-0.8.0/tests/test_spelling_er_or.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      544 2016-09-05 15:55:22.000000 proselint-0.8.0/tests/test_spelling_in_un.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      533 2016-09-05 15:55:22.000000 proselint-0.8.0/tests/test_spelling_misc.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      707 2016-03-21 09:16:14.000000 proselint-0.8.0/tests/test_strunk_white_eos.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      587 2016-09-05 15:55:22.000000 proselint-0.8.0/tests/test_terms_animal_adjectives.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      577 2016-09-05 15:55:22.000000 proselint-0.8.0/tests/test_terms_denizen_labels.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      601 2016-09-05 15:55:22.000000 proselint-0.8.0/tests/test_terms_eponymous_adjectives.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      544 2016-09-05 15:55:22.000000 proselint-0.8.0/tests/test_terms_venery.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     1043 2016-07-13 12:11:22.000000 proselint-0.8.0/tests/test_tools.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      709 2016-03-21 09:16:14.000000 proselint-0.8.0/tests/test_topic_detector.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      610 2016-09-05 15:55:22.000000 proselint-0.8.0/tests/test_typography_diacritical_marks.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     1069 2016-09-05 15:55:22.000000 proselint-0.8.0/tests/test_typography_exclamation.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)     1625 2016-09-05 15:55:22.000000 proselint-0.8.0/tests/test_typography_symbols.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      561 2016-09-05 15:55:22.000000 proselint-0.8.0/tests/test_uncomparables.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      590 2016-09-05 15:55:22.000000 proselint-0.8.0/tests/test_weasel_words_misc.py
--rw-r--r--   0 jordansuchow   (501) staff       (20)      562 2016-09-05 15:55:22.000000 proselint-0.8.0/tests/test_weasel_words_very.py
+drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2018-07-20 21:22:44.000000 proselint-0.9.0/
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      621 2018-07-20 21:22:44.000000 proselint-0.9.0/PKG-INFO
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     1524 2016-03-21 09:16:14.000000 proselint-0.9.0/LICENSE.md
+drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2018-07-20 21:22:43.000000 proselint-0.9.0/proselint.egg-info/
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      621 2018-07-20 21:22:43.000000 proselint-0.9.0/proselint.egg-info/PKG-INFO
+-rw-r--r--   0 jordansuchow   (501) staff       (20)        1 2016-04-06 00:20:12.000000 proselint-0.9.0/proselint.egg-info/not-zip-safe
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     7631 2018-07-20 21:22:43.000000 proselint-0.9.0/proselint.egg-info/SOURCES.txt
+-rw-r--r--   0 jordansuchow   (501) staff       (20)       64 2018-07-20 21:22:43.000000 proselint-0.9.0/proselint.egg-info/entry_points.txt
+-rw-r--r--   0 jordansuchow   (501) staff       (20)       47 2016-08-25 14:50:26.000000 proselint-0.9.0/proselint.egg-info/pbr.json
+-rw-r--r--   0 jordansuchow   (501) staff       (20)       17 2018-07-20 21:22:43.000000 proselint-0.9.0/proselint.egg-info/requires.txt
+-rw-r--r--   0 jordansuchow   (501) staff       (20)       10 2018-07-20 21:22:43.000000 proselint-0.9.0/proselint.egg-info/top_level.txt
+-rw-r--r--   0 jordansuchow   (501) staff       (20)        1 2018-07-20 21:22:43.000000 proselint-0.9.0/proselint.egg-info/dependency_links.txt
+-rw-r--r--   0 jordansuchow   (501) staff       (20)    41086 2018-07-20 20:59:53.000000 proselint-0.9.0/CHANGELOG.md
+drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2018-07-20 21:22:43.000000 proselint-0.9.0/proselint/
+-rw-r--r--   0 jordansuchow   (501) staff       (20)       55 2018-07-20 20:59:53.000000 proselint-0.9.0/proselint/version.py
+drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2018-07-20 21:22:43.000000 proselint-0.9.0/proselint/checks/
+drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2018-07-20 21:22:44.000000 proselint-0.9.0/proselint/checks/misc/
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     6975 2017-11-08 05:36:15.000000 proselint-0.9.0/proselint/checks/misc/phrasal_adjectives.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      578 2017-11-08 05:36:15.000000 proselint-0.9.0/proselint/checks/misc/scare_quotes.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      791 2016-04-01 08:30:13.000000 proselint-0.9.0/proselint/checks/misc/chatspeak.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      724 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/misc/inferior_superior.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      705 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/misc/metadiscourse.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     7587 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/misc/preferred_forms.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     1282 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/misc/commercialese.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      718 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/misc/many_a.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      587 2017-11-08 05:36:15.000000 proselint-0.9.0/proselint/checks/misc/metaconcepts.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      530 2017-11-08 05:36:15.000000 proselint-0.9.0/proselint/checks/misc/punctuation.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      787 2017-11-08 05:36:15.000000 proselint-0.9.0/proselint/checks/misc/institution_name.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      524 2017-11-08 05:36:15.000000 proselint-0.9.0/proselint/checks/misc/but.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)       54 2015-10-20 01:41:01.000000 proselint-0.9.0/proselint/checks/misc/__init__.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     1378 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/misc/illogic.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     1086 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/misc/not_guilty.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     1843 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/misc/waxed.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      783 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/misc/latin.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      588 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/misc/bureaucratese.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      624 2017-11-08 05:36:15.000000 proselint-0.9.0/proselint/checks/misc/pretension.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      588 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/misc/back_formations.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      558 2017-11-08 05:36:15.000000 proselint-0.9.0/proselint/checks/misc/apologizing.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     1495 2017-11-08 05:36:15.000000 proselint-0.9.0/proselint/checks/misc/suddenly.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      553 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/misc/professions.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     3486 2017-11-08 05:36:15.000000 proselint-0.9.0/proselint/checks/misc/composition.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     1089 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/misc/tense_present.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      839 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/misc/false_plurals.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      956 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/misc/greylist.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      522 2016-04-01 08:30:13.000000 proselint-0.9.0/proselint/checks/misc/currency.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      460 2016-04-01 09:36:45.000000 proselint-0.9.0/proselint/checks/misc/whence.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      638 2017-11-08 05:36:15.000000 proselint-0.9.0/proselint/checks/misc/narcissism.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     2019 2017-11-08 05:36:15.000000 proselint-0.9.0/proselint/checks/misc/usage.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      648 2017-11-08 05:36:15.000000 proselint-0.9.0/proselint/checks/misc/debased.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     2541 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/misc/capitalization.py
+drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2018-07-20 21:22:44.000000 proselint-0.9.0/proselint/checks/oxymorons/
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     1094 2017-11-08 05:36:15.000000 proselint-0.9.0/proselint/checks/oxymorons/misc.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)       17 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/oxymorons/__init__.py
+drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2018-07-20 21:22:43.000000 proselint-0.9.0/proselint/checks/cursing/
+-rw-r--r--   0 jordansuchow   (501) staff       (20)    24214 2017-11-08 05:36:15.000000 proselint-0.9.0/proselint/checks/cursing/nfl.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)       15 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/cursing/__init__.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      574 2017-11-08 05:36:15.000000 proselint-0.9.0/proselint/checks/cursing/nword.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      710 2017-11-08 05:36:15.000000 proselint-0.9.0/proselint/checks/cursing/filth.py
+drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2018-07-20 21:22:44.000000 proselint-0.9.0/proselint/checks/weasel_words/
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      411 2017-02-21 19:36:46.000000 proselint-0.9.0/proselint/checks/weasel_words/misc.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)       20 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/weasel_words/__init__.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      733 2017-11-08 05:36:15.000000 proselint-0.9.0/proselint/checks/weasel_words/very.py
+drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2018-07-20 21:22:44.000000 proselint-0.9.0/proselint/checks/jargon/
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      691 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/jargon/misc.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)       14 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/jargon/__init__.py
+drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2018-07-20 21:22:44.000000 proselint-0.9.0/proselint/checks/mondegreens/
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     1089 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/mondegreens/misc.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)       19 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/mondegreens/__init__.py
+drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2018-07-20 21:22:44.000000 proselint-0.9.0/proselint/checks/nonwords/
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     2440 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/nonwords/misc.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)       16 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/nonwords/__init__.py
+drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2018-07-20 21:22:43.000000 proselint-0.9.0/proselint/checks/corporate_speak/
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     1292 2017-11-08 05:36:15.000000 proselint-0.9.0/proselint/checks/corporate_speak/misc.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)       24 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/corporate_speak/__init__.py
+drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2018-07-20 21:22:44.000000 proselint-0.9.0/proselint/checks/hyperbole/
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      505 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/hyperbole/misc.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)       17 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/hyperbole/__init__.py
+drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2018-07-20 21:22:44.000000 proselint-0.9.0/proselint/checks/security/
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      651 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/security/credit_card.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)       16 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/security/__init__.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      742 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/security/password.py
+drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2018-07-20 21:22:43.000000 proselint-0.9.0/proselint/checks/archaism/
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     1847 2017-11-08 05:36:15.000000 proselint-0.9.0/proselint/checks/archaism/misc.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)       16 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/archaism/__init__.py
+drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2018-07-20 21:22:44.000000 proselint-0.9.0/proselint/checks/uncomparables/
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     4239 2017-11-08 05:36:15.000000 proselint-0.9.0/proselint/checks/uncomparables/misc.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)       33 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/uncomparables/__init__.py
+drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2018-07-20 21:22:44.000000 proselint-0.9.0/proselint/checks/psychology/
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     1412 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/psychology/misc.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)       25 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/psychology/__init__.py
+drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2018-07-20 21:22:44.000000 proselint-0.9.0/proselint/checks/terms/
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      680 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/terms/eponymous_adjectives.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     2440 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/terms/animal_adjectives.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)       13 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/terms/__init__.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     2635 2017-11-08 05:36:15.000000 proselint-0.9.0/proselint/checks/terms/venery.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     3331 2017-11-08 05:36:15.000000 proselint-0.9.0/proselint/checks/terms/denizen_labels.py
+drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2018-07-20 21:22:44.000000 proselint-0.9.0/proselint/checks/needless_variants/
+-rw-r--r--   0 jordansuchow   (501) staff       (20)    17582 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/needless_variants/misc.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)       25 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/needless_variants/__init__.py
+drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2018-07-20 21:22:44.000000 proselint-0.9.0/proselint/checks/redundancy/
+-rw-r--r--   0 jordansuchow   (501) staff       (20)    25077 2017-11-08 05:36:15.000000 proselint-0.9.0/proselint/checks/redundancy/misc.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)       18 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/redundancy/__init__.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     1331 2017-11-08 05:36:15.000000 proselint-0.9.0/proselint/checks/redundancy/ras_syndrome.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)       65 2015-10-20 01:41:01.000000 proselint-0.9.0/proselint/checks/__init__.py
+drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2018-07-20 21:22:43.000000 proselint-0.9.0/proselint/checks/cliches/
+-rw-r--r--   0 jordansuchow   (501) staff       (20)    25363 2017-11-08 05:36:15.000000 proselint-0.9.0/proselint/checks/cliches/misc.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)       21 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/cliches/__init__.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      550 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/cliches/hell.py
+drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2018-07-20 21:22:44.000000 proselint-0.9.0/proselint/checks/malapropisms/
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      599 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/malapropisms/misc.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)       21 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/malapropisms/__init__.py
+drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2018-07-20 21:22:43.000000 proselint-0.9.0/proselint/checks/hedging/
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      560 2017-11-08 05:36:15.000000 proselint-0.9.0/proselint/checks/hedging/misc.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)       15 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/hedging/__init__.py
+drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2018-07-20 21:22:43.000000 proselint-0.9.0/proselint/checks/consistency/
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     1474 2017-11-08 05:36:15.000000 proselint-0.9.0/proselint/checks/consistency/spelling.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      664 2016-04-01 08:30:13.000000 proselint-0.9.0/proselint/checks/consistency/spacing.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)       34 2015-10-20 01:41:01.000000 proselint-0.9.0/proselint/checks/consistency/__init__.py
+drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2018-07-20 21:22:43.000000 proselint-0.9.0/proselint/checks/annotations/
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      660 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/annotations/misc.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)       19 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/annotations/__init__.py
+drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2018-07-20 21:22:44.000000 proselint-0.9.0/proselint/checks/lgbtq/
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     1277 2017-11-08 05:36:15.000000 proselint-0.9.0/proselint/checks/lgbtq/terms.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     1107 2017-11-08 05:36:15.000000 proselint-0.9.0/proselint/checks/lgbtq/offensive_terms.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)       13 2017-11-08 05:36:15.000000 proselint-0.9.0/proselint/checks/lgbtq/__init__.py
+drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2018-07-20 21:22:44.000000 proselint-0.9.0/proselint/checks/sexism/
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     2567 2017-11-08 05:36:15.000000 proselint-0.9.0/proselint/checks/sexism/misc.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)       14 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/sexism/__init__.py
+drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2018-07-20 21:22:44.000000 proselint-0.9.0/proselint/checks/links/
+-rw-r--r--   0 jordansuchow   (501) staff       (20)       20 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/links/__init__.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     1664 2017-11-08 05:36:15.000000 proselint-0.9.0/proselint/checks/links/broken.py
+drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2018-07-20 21:22:44.000000 proselint-0.9.0/proselint/checks/typography/
+-rw-r--r--   0 jordansuchow   (501) staff       (20)       28 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/typography/__init__.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     4722 2017-11-08 05:36:15.000000 proselint-0.9.0/proselint/checks/typography/diacritical_marks.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     2848 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/typography/symbols.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     1130 2017-11-08 05:36:15.000000 proselint-0.9.0/proselint/checks/typography/exclamation.py
+drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2018-07-20 21:22:44.000000 proselint-0.9.0/proselint/checks/skunked_terms/
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      766 2017-11-08 05:36:15.000000 proselint-0.9.0/proselint/checks/skunked_terms/misc.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)       27 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/skunked_terms/__init__.py
+drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2018-07-20 21:22:43.000000 proselint-0.9.0/proselint/checks/airlinese/
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      584 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/airlinese/misc.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)       17 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/airlinese/__init__.py
+drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2018-07-20 21:22:44.000000 proselint-0.9.0/proselint/checks/mixed_metaphors/
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     1385 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/mixed_metaphors/misc.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)       23 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/mixed_metaphors/__init__.py
+drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2018-07-20 21:22:43.000000 proselint-0.9.0/proselint/checks/dates_times/
+-rw-r--r--   0 jordansuchow   (501) staff       (20)       23 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/dates_times/__init__.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     1463 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/dates_times/am_pm.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     1696 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/dates_times/dates.py
+drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2018-07-20 21:22:44.000000 proselint-0.9.0/proselint/checks/spelling/
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     6346 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/spelling/misc.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     7367 2017-11-08 05:36:15.000000 proselint-0.9.0/proselint/checks/spelling/able_ible.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     1452 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/spelling/athletes.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     3696 2017-11-08 05:36:15.000000 proselint-0.9.0/proselint/checks/spelling/able_atable.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     2233 2017-11-08 05:36:15.000000 proselint-0.9.0/proselint/checks/spelling/em_im_en_in.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)       16 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/spelling/__init__.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      529 2017-11-08 05:36:15.000000 proselint-0.9.0/proselint/checks/spelling/in_un.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     1516 2017-11-08 05:36:15.000000 proselint-0.9.0/proselint/checks/spelling/er_or.py
+drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2018-07-20 21:22:44.000000 proselint-0.9.0/proselint/checks/lexical_illusions/
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      677 2017-11-08 05:36:15.000000 proselint-0.9.0/proselint/checks/lexical_illusions/misc.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)       25 2016-06-28 08:41:28.000000 proselint-0.9.0/proselint/checks/lexical_illusions/__init__.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     4926 2018-03-23 05:12:46.000000 proselint-0.9.0/proselint/command_line.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)    13357 2018-03-23 05:12:46.000000 proselint-0.9.0/proselint/tools.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      108 2017-11-08 05:36:15.000000 proselint-0.9.0/proselint/__init__.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     6095 2017-02-25 03:55:31.000000 proselint-0.9.0/proselint/demo.md
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     3892 2018-03-23 05:12:46.000000 proselint-0.9.0/proselint/.proselintrc
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      142 2017-11-08 05:36:15.000000 proselint-0.9.0/proselint/__main__.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     2659 2017-11-08 05:36:15.000000 proselint-0.9.0/proselint/score.py
+drwxr-xr-x   0 jordansuchow   (501) staff       (20)        0 2018-07-20 21:22:44.000000 proselint-0.9.0/tests/
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     1445 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_redundancy_misc.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     2662 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_dates_times_dates.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      551 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_hedging.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      562 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_misc_many_a.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     1069 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_typography_exclamation.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      437 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_misc_metaconcepts.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      537 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_hyperbole.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      563 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_spelling_able_ible.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      539 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_misc_chatspeak.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      866 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_leonard.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      676 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_consistency_spacing.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      611 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_lgbtq_offensive_terms.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      572 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_spelling_em_im_en_in.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      562 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_spelling_athletes.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      747 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_dfw_uncomparables.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      560 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_misc_professions.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     1781 2016-06-28 08:41:28.000000 proselint-0.9.0/tests/check.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      552 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_misc_apologizing.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      709 2015-10-20 01:41:01.000000 proselint-0.9.0/tests/test_topic_detector.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      536 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_misc_currency.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      549 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_misc_greylist.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      562 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_weasel_words_very.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      565 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_misc_scare_quotes.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      540 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_jargon.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      536 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_cursing_nfl.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      537 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_misc_latin.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      905 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_mixed_metaphors.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      582 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_spelling_able_atable.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      537 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_misc_waxed.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     2047 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_dates_times_am_pm.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     4539 2018-03-23 05:12:46.000000 proselint-0.9.0/tests/test_clear_cache.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      566 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_misc_tense_present.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      807 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_misc_false_plurals.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      552 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_misc_composition.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      597 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_skunked_terms.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      637 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_misc_narcissism.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      544 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_misc_suddenly.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      707 2015-10-20 01:41:01.000000 proselint-0.9.0/tests/test_strunk_white_eos.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      926 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_consistency_check.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      546 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_spelling_er_or.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)       65 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/illegal-chars.txt
+-rw-r--r--   0 jordansuchow   (501) staff       (20)       27 2015-10-20 01:41:01.000000 proselint-0.9.0/tests/__init__.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     1077 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_misc_capitalization.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      571 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_misc_back_formations.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      601 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_terms_eponymous_adjectives.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     1182 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_illegal_chars.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      620 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_archaism.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      543 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_misc_debased.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      637 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_corporate_speak.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      569 2016-06-28 08:41:28.000000 proselint-0.9.0/tests/test_exit_codes.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      537 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_misc_whence.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      547 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_nonwords.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      580 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_lexical_illusions.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      548 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_oxymorons.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      533 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_spelling_misc.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      612 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_annotations.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     1625 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_typography_symbols.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      661 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_security_credit_card.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      618 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_security_password.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      914 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_lgbtq_terms.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      575 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_misc_metadiscourse.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      540 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_cursing_filth.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     1900 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_existence_check.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     1324 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_psychology.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      583 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_needless_variants.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      587 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_terms_animal_adjectives.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      485 2016-06-28 08:41:28.000000 proselint-0.9.0/tests/_test_version.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     1227 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_preferred_forms_check.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      571 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_malaproprisms.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     1625 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_butterick_symbols.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      563 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_misc_pretension.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      610 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_typography_diacritical_marks.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      581 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_misc_not_guilty.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      545 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_misc_punctuation.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      585 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_redundancy_ras_syndrome.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      568 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_misc_commercialese.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      567 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_misc_preferred_forms.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      409 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_misc_usage.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     1798 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_cliches.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     1043 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_tools.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      534 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_misc_but.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      607 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_misc_inferior_superior.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      108 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_demo.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      577 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_terms_denizen_labels.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      939 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_misc_phrasal_adjectives.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      544 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_spelling_in_un.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      561 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_uncomparables.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      592 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_misc_bureaucratese.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      544 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_terms_venery.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     1088 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_garner_dates.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      527 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_cursing_nword.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      570 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_sexism.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      590 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_weasel_words_misc.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     1199 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_misc_illogic.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      739 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_consistency_spelling.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      615 2017-11-08 05:36:15.000000 proselint-0.9.0/tests/test_mondegreens.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)       65 2017-11-08 05:36:15.000000 proselint-0.9.0/MANIFEST.in
+-rw-r--r--   0 jordansuchow   (501) staff       (20)    11800 2018-07-20 19:43:01.000000 proselint-0.9.0/README.md
+-rw-r--r--   0 jordansuchow   (501) staff       (20)     1147 2017-11-08 05:36:15.000000 proselint-0.9.0/setup.py
+-rw-r--r--   0 jordansuchow   (501) staff       (20)      249 2018-07-20 21:22:44.000000 proselint-0.9.0/setup.cfg
```

### Comparing `proselint-0.8.0/CHANGELOG.md` & `proselint-0.9.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Change Log
 
+## [0.9.0](https://github.com/amperser/proselint/tree/0.9.0) (2018-07-20)
+[Full Changelog](https://github.com/amperser/proselint/compare/0.8.0...0.9.0)
+
+- Add new plugins to README
+- Update dependencies
+- Comply with XDG spec ([xu-cheng](https://github.com/xu-cheng))
+
 ## [0.8.0](https://github.com/amperser/proselint/tree/0.8.0) (2017-02-22)
 [Full Changelog](https://github.com/amperser/proselint/compare/0.7.0...0.8.0)
 
 - Fix a cache-clearing issue ([m-charlton](https://github.com/m-charlton))
 - Tons of improvements to tests ([joshmgrant](https://github.com/joshmgrant))
 - New LGBTQ-terms module
 - Misc. bug fixes and improvements
```

### Comparing `proselint-0.8.0/LICENSE.md` & `proselint-0.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/.proselintrc` & `proselint-0.9.0/proselint/.proselintrc`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 2% similar despite different names*

```diff
@@ -98,146 +98,147 @@
 00000610: 5f70 6c75 7261 6c73 2220 2020 2020 2020  _plurals"       
 00000620: 2020 2020 203a 2074 7275 652c 0a20 2020       : true,.   
 00000630: 2020 2020 2022 6d69 7363 2e69 6c6c 6f67       "misc.illog
 00000640: 6963 2220 2020 2020 2020 2020 2020 2020  ic"             
 00000650: 2020 2020 203a 2074 7275 652c 0a20 2020       : true,.   
 00000660: 2020 2020 2022 6d69 7363 2e69 6e66 6572       "misc.infer
 00000670: 696f 725f 7375 7065 7269 6f72 2220 2020  ior_superior"   
-00000680: 2020 2020 203a 2074 7275 652c 0a09 0922       : true,..."
-00000690: 6d69 7363 2e69 6e73 7469 7475 7469 6f6e  misc.institution
-000006a0: 5f6e 616d 6522 0909 093a 2074 7275 652c  _name"...: true,
-000006b0: 0a20 2020 2020 2020 2022 6d69 7363 2e6c  .        "misc.l
-000006c0: 6174 696e 2220 2020 2020 2020 2020 2020  atin"           
-000006d0: 2020 2020 2020 2020 203a 2074 7275 652c           : true,
-000006e0: 0a20 2020 2020 2020 2022 6d69 7363 2e6d  .        "misc.m
-000006f0: 616e 795f 6122 2020 2020 2020 2020 2020  any_a"          
-00000700: 2020 2020 2020 2020 203a 2074 7275 652c           : true,
-00000710: 0a20 2020 2020 2020 2022 6d69 7363 2e6d  .        "misc.m
-00000720: 6574 6163 6f6e 6365 7074 7322 2020 2020  etaconcepts"    
-00000730: 2020 2020 2020 2020 203a 2074 7275 652c           : true,
-00000740: 0a20 2020 2020 2020 2022 6d69 7363 2e6d  .        "misc.m
-00000750: 6574 6164 6973 636f 7572 7365 2220 2020  etadiscourse"   
-00000760: 2020 2020 2020 2020 203a 2074 7275 652c           : true,
-00000770: 0a20 2020 2020 2020 2022 6d69 7363 2e6e  .        "misc.n
-00000780: 6172 6369 7373 6973 6d22 2020 2020 2020  arcissism"      
-00000790: 2020 2020 2020 2020 203a 2074 7275 652c           : true,
-000007a0: 0a20 2020 2020 2020 2022 6d69 7363 2e6e  .        "misc.n
-000007b0: 6f74 5f67 7569 6c74 7922 2020 2020 2020  ot_guilty"      
-000007c0: 2020 2020 2020 2020 203a 2074 7275 652c           : true,
-000007d0: 0a20 2020 2020 2020 2022 6d69 7363 2e70  .        "misc.p
-000007e0: 6872 6173 616c 5f61 646a 6563 7469 7665  hrasal_adjective
-000007f0: 7322 2020 2020 2020 203a 2074 7275 652c  s"       : true,
-00000800: 0a20 2020 2020 2020 2022 6d69 7363 2e70  .        "misc.p
-00000810: 7265 6665 7272 6564 5f66 6f72 6d73 2220  referred_forms" 
-00000820: 2020 2020 2020 2020 203a 2074 7275 652c           : true,
-00000830: 0a20 2020 2020 2020 2022 6d69 7363 2e70  .        "misc.p
-00000840: 7265 7465 6e73 696f 6e22 2020 2020 2020  retension"      
-00000850: 2020 2020 2020 2020 203a 2074 7275 652c           : true,
-00000860: 0a20 2020 2020 2020 2022 6d69 7363 2e70  .        "misc.p
-00000870: 726f 6665 7373 696f 6e73 2220 2020 2020  rofessions"     
-00000880: 2020 2020 2020 2020 203a 2074 7275 652c           : true,
-00000890: 0a20 2020 2020 2020 2022 6d69 7363 2e70  .        "misc.p
-000008a0: 756e 6374 7561 7469 6f6e 2220 2020 2020  unctuation"     
-000008b0: 2020 2020 2020 2020 203a 2074 7275 652c           : true,
-000008c0: 0a20 2020 2020 2020 2022 6d69 7363 2e73  .        "misc.s
-000008d0: 6361 7265 5f71 756f 7465 7322 2020 2020  care_quotes"    
-000008e0: 2020 2020 2020 2020 203a 2074 7275 652c           : true,
-000008f0: 0a20 2020 2020 2020 2022 6d69 7363 2e73  .        "misc.s
-00000900: 7564 6465 6e6c 7922 2020 2020 2020 2020  uddenly"        
-00000910: 2020 2020 2020 2020 203a 2074 7275 652c           : true,
-00000920: 0a20 2020 2020 2020 2022 6d69 7363 2e74  .        "misc.t
-00000930: 656e 7365 5f70 7265 7365 6e74 2220 2020  ense_present"   
-00000940: 2020 2020 2020 2020 203a 2074 7275 652c           : true,
-00000950: 0a20 2020 2020 2020 2022 6d69 7363 2e77  .        "misc.w
-00000960: 6178 6564 2220 2020 2020 2020 2020 2020  axed"           
-00000970: 2020 2020 2020 2020 203a 2074 7275 652c           : true,
-00000980: 0a20 2020 2020 2020 2022 6d69 7363 2e77  .        "misc.w
-00000990: 6865 6e63 6522 2020 2020 2020 2020 2020  hence"          
-000009a0: 2020 2020 2020 2020 203a 2074 7275 652c           : true,
-000009b0: 0a20 2020 2020 2020 2022 6d69 7865 645f  .        "mixed_
-000009c0: 6d65 7461 7068 6f72 732e 6d69 7363 2220  metaphors.misc" 
-000009d0: 2020 2020 2020 2020 203a 2074 7275 652c           : true,
-000009e0: 0a20 2020 2020 2020 2022 6d6f 6e64 6567  .        "mondeg
-000009f0: 7265 656e 732e 6d69 7363 2220 2020 2020  reens.misc"     
-00000a00: 2020 2020 2020 2020 203a 2074 7275 652c           : true,
-00000a10: 0a20 2020 2020 2020 2022 6e65 6564 6c65  .        "needle
-00000a20: 7373 5f76 6172 6961 6e74 732e 6d69 7363  ss_variants.misc
-00000a30: 2220 2020 2020 2020 203a 2074 7275 652c  "        : true,
-00000a40: 0a20 2020 2020 2020 2022 6e6f 6e77 6f72  .        "nonwor
-00000a50: 6473 2e6d 6973 6322 2020 2020 2020 2020  ds.misc"        
-00000a60: 2020 2020 2020 2020 203a 2074 7275 652c           : true,
-00000a70: 0a20 2020 2020 2020 2022 6f78 796d 6f72  .        "oxymor
-00000a80: 6f6e 732e 6d69 7363 2220 2020 2020 2020  ons.misc"       
-00000a90: 2020 2020 2020 2020 203a 2074 7275 652c           : true,
-00000aa0: 0a20 2020 2020 2020 2022 7073 7963 686f  .        "psycho
-00000ab0: 6c6f 6779 2e6d 6973 6322 2020 2020 2020  logy.misc"      
-00000ac0: 2020 2020 2020 2020 203a 2074 7275 652c           : true,
-00000ad0: 0a20 2020 2020 2020 2022 7265 6475 6e64  .        "redund
-00000ae0: 616e 6379 2e6d 6973 6322 2020 2020 2020  ancy.misc"      
-00000af0: 2020 2020 2020 2020 203a 2074 7275 652c           : true,
-00000b00: 0a20 2020 2020 2020 2022 7265 6475 6e64  .        "redund
-00000b10: 616e 6379 2e72 6173 5f73 796e 6472 6f6d  ancy.ras_syndrom
-00000b20: 6522 2020 2020 2020 203a 2074 7275 652c  e"       : true,
-00000b30: 0a20 2020 2020 2020 2022 736b 756e 6b65  .        "skunke
-00000b40: 645f 7465 726d 732e 6d69 7363 2220 2020  d_terms.misc"   
-00000b50: 2020 2020 2020 2020 203a 2074 7275 652c           : true,
-00000b60: 0a20 2020 2020 2020 2022 7370 656c 6c69  .        "spelli
-00000b70: 6e67 2e61 626c 655f 6174 6162 6c65 2220  ng.able_atable" 
-00000b80: 2020 2020 2020 2020 203a 2074 7275 652c           : true,
-00000b90: 0a20 2020 2020 2020 2022 7370 656c 6c69  .        "spelli
-00000ba0: 6e67 2e61 626c 655f 6962 6c65 2220 2020  ng.able_ible"   
-00000bb0: 2020 2020 2020 2020 203a 2074 7275 652c           : true,
-00000bc0: 0a20 2020 2020 2020 2022 7370 656c 6c69  .        "spelli
-00000bd0: 6e67 2e61 7468 6c65 7465 7322 2020 2020  ng.athletes"    
-00000be0: 2020 2020 2020 2020 203a 2074 7275 652c           : true,
-00000bf0: 0a20 2020 2020 2020 2022 7370 656c 6c69  .        "spelli
-00000c00: 6e67 2e65 6d5f 696d 5f65 6e5f 696e 2220  ng.em_im_en_in" 
-00000c10: 2020 2020 2020 2020 203a 2074 7275 652c           : true,
-00000c20: 0a20 2020 2020 2020 2022 7370 656c 6c69  .        "spelli
-00000c30: 6e67 2e65 725f 6f72 2220 2020 2020 2020  ng.er_or"       
-00000c40: 2020 2020 2020 2020 203a 2074 7275 652c           : true,
-00000c50: 0a20 2020 2020 2020 2022 7370 656c 6c69  .        "spelli
-00000c60: 6e67 2e69 6e5f 756e 2220 2020 2020 2020  ng.in_un"       
-00000c70: 2020 2020 2020 2020 203a 2074 7275 652c           : true,
-00000c80: 0a20 2020 2020 2020 2022 7370 656c 6c69  .        "spelli
-00000c90: 6e67 2e6d 6973 6322 2020 2020 2020 2020  ng.misc"        
-00000ca0: 2020 2020 2020 2020 203a 2074 7275 652c           : true,
-00000cb0: 0a20 2020 2020 2020 2022 7365 6375 7269  .        "securi
-00000cc0: 7479 2e63 7265 6469 745f 6361 7264 2220  ty.credit_card" 
-00000cd0: 2020 2020 2020 2020 203a 2074 7275 652c           : true,
-00000ce0: 0a20 2020 2020 2020 2022 7365 6375 7269  .        "securi
-00000cf0: 7479 2e70 6173 7377 6f72 6422 2020 2020  ty.password"    
-00000d00: 2020 2020 2020 2020 203a 2074 7275 652c           : true,
-00000d10: 0a20 2020 2020 2020 2022 7365 7869 736d  .        "sexism
-00000d20: 2e6d 6973 6322 2020 2020 2020 2020 2020  .misc"          
-00000d30: 2020 2020 2020 2020 203a 2074 7275 652c           : true,
-00000d40: 0a20 2020 2020 2020 2022 7465 726d 732e  .        "terms.
-00000d50: 616e 696d 616c 5f61 646a 6563 7469 7665  animal_adjective
-00000d60: 7322 2020 2020 2020 203a 2074 7275 652c  s"       : true,
-00000d70: 0a20 2020 2020 2020 2022 7465 726d 732e  .        "terms.
-00000d80: 6465 6e69 7a65 6e5f 6c61 6265 6c73 2220  denizen_labels" 
-00000d90: 2020 2020 2020 2020 203a 2074 7275 652c           : true,
-00000da0: 0a20 2020 2020 2020 2022 7465 726d 732e  .        "terms.
-00000db0: 6570 6f6e 796d 6f75 735f 6164 6a65 6374  eponymous_adject
-00000dc0: 6976 6573 2220 2020 203a 2074 7275 652c  ives"    : true,
-00000dd0: 0a20 2020 2020 2020 2022 7465 726d 732e  .        "terms.
-00000de0: 7665 6e65 7279 2220 2020 2020 2020 2020  venery"         
-00000df0: 2020 2020 2020 2020 203a 2074 7275 652c           : true,
-00000e00: 0a20 2020 2020 2020 2022 7479 706f 6772  .        "typogr
-00000e10: 6170 6879 2e64 6961 6372 6974 6963 616c  aphy.diacritical
-00000e20: 5f6d 6172 6b73 2220 203a 2074 7275 652c  _marks"  : true,
-00000e30: 0a20 2020 2020 2020 2022 7479 706f 6772  .        "typogr
-00000e40: 6170 6879 2e65 7863 6c61 6d61 7469 6f6e  aphy.exclamation
-00000e50: 2220 2020 2020 2020 203a 2074 7275 652c  "        : true,
-00000e60: 0a20 2020 2020 2020 2022 7479 706f 6772  .        "typogr
-00000e70: 6170 6879 2e73 796d 626f 6c73 2220 2020  aphy.symbols"   
-00000e80: 2020 2020 2020 2020 203a 2074 7275 652c           : true,
-00000e90: 0a20 2020 2020 2020 2022 756e 636f 6d70  .        "uncomp
-00000ea0: 6172 6162 6c65 732e 6d69 7363 2220 2020  arables.misc"   
-00000eb0: 2020 2020 2020 2020 203a 2074 7275 652c           : true,
-00000ec0: 0a20 2020 2020 2020 2022 7765 6173 656c  .        "weasel
-00000ed0: 5f77 6f72 6473 2e6d 6973 6322 2020 2020  _words.misc"    
-00000ee0: 2020 2020 2020 2020 203a 2074 7275 652c           : true,
-00000ef0: 0a20 2020 2020 2020 2022 7765 6173 656c  .        "weasel
-00000f00: 5f77 6f72 6473 2e76 6572 7922 2020 2020  _words.very"    
-00000f10: 2020 2020 2020 2020 203a 2074 7275 650a           : true.
-00000f20: 2020 2020 7d0a 7d0a                          }.}.
+00000680: 2020 2020 203a 2074 7275 652c 0a20 2020       : true,.   
+00000690: 2020 2020 2022 6d69 7363 2e69 6e73 7469       "misc.insti
+000006a0: 7475 7469 6f6e 5f6e 616d 6522 0920 2020  tution_name".   
+000006b0: 2020 2020 203a 2074 7275 652c 0a20 2020       : true,.   
+000006c0: 2020 2020 2022 6d69 7363 2e6c 6174 696e       "misc.latin
+000006d0: 2220 2020 2020 2020 2020 2020 2020 2020  "               
+000006e0: 2020 2020 203a 2074 7275 652c 0a20 2020       : true,.   
+000006f0: 2020 2020 2022 6d69 7363 2e6d 616e 795f       "misc.many_
+00000700: 6122 2020 2020 2020 2020 2020 2020 2020  a"              
+00000710: 2020 2020 203a 2074 7275 652c 0a20 2020       : true,.   
+00000720: 2020 2020 2022 6d69 7363 2e6d 6574 6163       "misc.metac
+00000730: 6f6e 6365 7074 7322 2020 2020 2020 2020  oncepts"        
+00000740: 2020 2020 203a 2074 7275 652c 0a20 2020       : true,.   
+00000750: 2020 2020 2022 6d69 7363 2e6d 6574 6164       "misc.metad
+00000760: 6973 636f 7572 7365 2220 2020 2020 2020  iscourse"       
+00000770: 2020 2020 203a 2074 7275 652c 0a20 2020       : true,.   
+00000780: 2020 2020 2022 6d69 7363 2e6e 6172 6369       "misc.narci
+00000790: 7373 6973 6d22 2020 2020 2020 2020 2020  ssism"          
+000007a0: 2020 2020 203a 2074 7275 652c 0a20 2020       : true,.   
+000007b0: 2020 2020 2022 6d69 7363 2e6e 6f74 5f67       "misc.not_g
+000007c0: 7569 6c74 7922 2020 2020 2020 2020 2020  uilty"          
+000007d0: 2020 2020 203a 2074 7275 652c 0a20 2020       : true,.   
+000007e0: 2020 2020 2022 6d69 7363 2e70 6872 6173       "misc.phras
+000007f0: 616c 5f61 646a 6563 7469 7665 7322 2020  al_adjectives"  
+00000800: 2020 2020 203a 2074 7275 652c 0a20 2020       : true,.   
+00000810: 2020 2020 2022 6d69 7363 2e70 7265 6665       "misc.prefe
+00000820: 7272 6564 5f66 6f72 6d73 2220 2020 2020  rred_forms"     
+00000830: 2020 2020 203a 2074 7275 652c 0a20 2020       : true,.   
+00000840: 2020 2020 2022 6d69 7363 2e70 7265 7465       "misc.prete
+00000850: 6e73 696f 6e22 2020 2020 2020 2020 2020  nsion"          
+00000860: 2020 2020 203a 2074 7275 652c 0a20 2020       : true,.   
+00000870: 2020 2020 2022 6d69 7363 2e70 726f 6665       "misc.profe
+00000880: 7373 696f 6e73 2220 2020 2020 2020 2020  ssions"         
+00000890: 2020 2020 203a 2074 7275 652c 0a20 2020       : true,.   
+000008a0: 2020 2020 2022 6d69 7363 2e70 756e 6374       "misc.punct
+000008b0: 7561 7469 6f6e 2220 2020 2020 2020 2020  uation"         
+000008c0: 2020 2020 203a 2074 7275 652c 0a20 2020       : true,.   
+000008d0: 2020 2020 2022 6d69 7363 2e73 6361 7265       "misc.scare
+000008e0: 5f71 756f 7465 7322 2020 2020 2020 2020  _quotes"        
+000008f0: 2020 2020 203a 2074 7275 652c 0a20 2020       : true,.   
+00000900: 2020 2020 2022 6d69 7363 2e73 7564 6465       "misc.sudde
+00000910: 6e6c 7922 2020 2020 2020 2020 2020 2020  nly"            
+00000920: 2020 2020 203a 2074 7275 652c 0a20 2020       : true,.   
+00000930: 2020 2020 2022 6d69 7363 2e74 656e 7365       "misc.tense
+00000940: 5f70 7265 7365 6e74 2220 2020 2020 2020  _present"       
+00000950: 2020 2020 203a 2074 7275 652c 0a20 2020       : true,.   
+00000960: 2020 2020 2022 6d69 7363 2e77 6178 6564       "misc.waxed
+00000970: 2220 2020 2020 2020 2020 2020 2020 2020  "               
+00000980: 2020 2020 203a 2074 7275 652c 0a20 2020       : true,.   
+00000990: 2020 2020 2022 6d69 7363 2e77 6865 6e63       "misc.whenc
+000009a0: 6522 2020 2020 2020 2020 2020 2020 2020  e"              
+000009b0: 2020 2020 203a 2074 7275 652c 0a20 2020       : true,.   
+000009c0: 2020 2020 2022 6d69 7865 645f 6d65 7461       "mixed_meta
+000009d0: 7068 6f72 732e 6d69 7363 2220 2020 2020  phors.misc"     
+000009e0: 2020 2020 203a 2074 7275 652c 0a20 2020       : true,.   
+000009f0: 2020 2020 2022 6d6f 6e64 6567 7265 656e       "mondegreen
+00000a00: 732e 6d69 7363 2220 2020 2020 2020 2020  s.misc"         
+00000a10: 2020 2020 203a 2074 7275 652c 0a20 2020       : true,.   
+00000a20: 2020 2020 2022 6e65 6564 6c65 7373 5f76       "needless_v
+00000a30: 6172 6961 6e74 732e 6d69 7363 2220 2020  ariants.misc"   
+00000a40: 2020 2020 203a 2074 7275 652c 0a20 2020       : true,.   
+00000a50: 2020 2020 2022 6e6f 6e77 6f72 6473 2e6d       "nonwords.m
+00000a60: 6973 6322 2020 2020 2020 2020 2020 2020  isc"            
+00000a70: 2020 2020 203a 2074 7275 652c 0a20 2020       : true,.   
+00000a80: 2020 2020 2022 6f78 796d 6f72 6f6e 732e       "oxymorons.
+00000a90: 6d69 7363 2220 2020 2020 2020 2020 2020  misc"           
+00000aa0: 2020 2020 203a 2074 7275 652c 0a20 2020       : true,.   
+00000ab0: 2020 2020 2022 7073 7963 686f 6c6f 6779       "psychology
+00000ac0: 2e6d 6973 6322 2020 2020 2020 2020 2020  .misc"          
+00000ad0: 2020 2020 203a 2074 7275 652c 0a20 2020       : true,.   
+00000ae0: 2020 2020 2022 7265 6475 6e64 616e 6379       "redundancy
+00000af0: 2e6d 6973 6322 2020 2020 2020 2020 2020  .misc"          
+00000b00: 2020 2020 203a 2074 7275 652c 0a20 2020       : true,.   
+00000b10: 2020 2020 2022 7265 6475 6e64 616e 6379       "redundancy
+00000b20: 2e72 6173 5f73 796e 6472 6f6d 6522 2020  .ras_syndrome"  
+00000b30: 2020 2020 203a 2074 7275 652c 0a20 2020       : true,.   
+00000b40: 2020 2020 2022 736b 756e 6b65 645f 7465       "skunked_te
+00000b50: 726d 732e 6d69 7363 2220 2020 2020 2020  rms.misc"       
+00000b60: 2020 2020 203a 2074 7275 652c 0a20 2020       : true,.   
+00000b70: 2020 2020 2022 7370 656c 6c69 6e67 2e61       "spelling.a
+00000b80: 626c 655f 6174 6162 6c65 2220 2020 2020  ble_atable"     
+00000b90: 2020 2020 203a 2074 7275 652c 0a20 2020       : true,.   
+00000ba0: 2020 2020 2022 7370 656c 6c69 6e67 2e61       "spelling.a
+00000bb0: 626c 655f 6962 6c65 2220 2020 2020 2020  ble_ible"       
+00000bc0: 2020 2020 203a 2074 7275 652c 0a20 2020       : true,.   
+00000bd0: 2020 2020 2022 7370 656c 6c69 6e67 2e61       "spelling.a
+00000be0: 7468 6c65 7465 7322 2020 2020 2020 2020  thletes"        
+00000bf0: 2020 2020 203a 2074 7275 652c 0a20 2020       : true,.   
+00000c00: 2020 2020 2022 7370 656c 6c69 6e67 2e65       "spelling.e
+00000c10: 6d5f 696d 5f65 6e5f 696e 2220 2020 2020  m_im_en_in"     
+00000c20: 2020 2020 203a 2074 7275 652c 0a20 2020       : true,.   
+00000c30: 2020 2020 2022 7370 656c 6c69 6e67 2e65       "spelling.e
+00000c40: 725f 6f72 2220 2020 2020 2020 2020 2020  r_or"           
+00000c50: 2020 2020 203a 2074 7275 652c 0a20 2020       : true,.   
+00000c60: 2020 2020 2022 7370 656c 6c69 6e67 2e69       "spelling.i
+00000c70: 6e5f 756e 2220 2020 2020 2020 2020 2020  n_un"           
+00000c80: 2020 2020 203a 2074 7275 652c 0a20 2020       : true,.   
+00000c90: 2020 2020 2022 7370 656c 6c69 6e67 2e6d       "spelling.m
+00000ca0: 6973 6322 2020 2020 2020 2020 2020 2020  isc"            
+00000cb0: 2020 2020 203a 2074 7275 652c 0a20 2020       : true,.   
+00000cc0: 2020 2020 2022 7365 6375 7269 7479 2e63       "security.c
+00000cd0: 7265 6469 745f 6361 7264 2220 2020 2020  redit_card"     
+00000ce0: 2020 2020 203a 2074 7275 652c 0a20 2020       : true,.   
+00000cf0: 2020 2020 2022 7365 6375 7269 7479 2e70       "security.p
+00000d00: 6173 7377 6f72 6422 2020 2020 2020 2020  assword"        
+00000d10: 2020 2020 203a 2074 7275 652c 0a20 2020       : true,.   
+00000d20: 2020 2020 2022 7365 7869 736d 2e6d 6973       "sexism.mis
+00000d30: 6322 2020 2020 2020 2020 2020 2020 2020  c"              
+00000d40: 2020 2020 203a 2074 7275 652c 0a20 2020       : true,.   
+00000d50: 2020 2020 2022 7465 726d 732e 616e 696d       "terms.anim
+00000d60: 616c 5f61 646a 6563 7469 7665 7322 2020  al_adjectives"  
+00000d70: 2020 2020 203a 2074 7275 652c 0a20 2020       : true,.   
+00000d80: 2020 2020 2022 7465 726d 732e 6465 6e69       "terms.deni
+00000d90: 7a65 6e5f 6c61 6265 6c73 2220 2020 2020  zen_labels"     
+00000da0: 2020 2020 203a 2074 7275 652c 0a20 2020       : true,.   
+00000db0: 2020 2020 2022 7465 726d 732e 6570 6f6e       "terms.epon
+00000dc0: 796d 6f75 735f 6164 6a65 6374 6976 6573  ymous_adjectives
+00000dd0: 2220 2020 203a 2074 7275 652c 0a20 2020  "    : true,.   
+00000de0: 2020 2020 2022 7465 726d 732e 7665 6e65       "terms.vene
+00000df0: 7279 2220 2020 2020 2020 2020 2020 2020  ry"             
+00000e00: 2020 2020 203a 2074 7275 652c 0a20 2020       : true,.   
+00000e10: 2020 2020 2022 7479 706f 6772 6170 6879       "typography
+00000e20: 2e64 6961 6372 6974 6963 616c 5f6d 6172  .diacritical_mar
+00000e30: 6b73 2220 203a 2074 7275 652c 0a20 2020  ks"  : true,.   
+00000e40: 2020 2020 2022 7479 706f 6772 6170 6879       "typography
+00000e50: 2e65 7863 6c61 6d61 7469 6f6e 2220 2020  .exclamation"   
+00000e60: 2020 2020 203a 2074 7275 652c 0a20 2020       : true,.   
+00000e70: 2020 2020 2022 7479 706f 6772 6170 6879       "typography
+00000e80: 2e73 796d 626f 6c73 2220 2020 2020 2020  .symbols"       
+00000e90: 2020 2020 203a 2074 7275 652c 0a20 2020       : true,.   
+00000ea0: 2020 2020 2022 756e 636f 6d70 6172 6162       "uncomparab
+00000eb0: 6c65 732e 6d69 7363 2220 2020 2020 2020  les.misc"       
+00000ec0: 2020 2020 203a 2074 7275 652c 0a20 2020       : true,.   
+00000ed0: 2020 2020 2022 7765 6173 656c 5f77 6f72       "weasel_wor
+00000ee0: 6473 2e6d 6973 6322 2020 2020 2020 2020  ds.misc"        
+00000ef0: 2020 2020 203a 2074 7275 652c 0a20 2020       : true,.   
+00000f00: 2020 2020 2022 7765 6173 656c 5f77 6f72       "weasel_wor
+00000f10: 6473 2e76 6572 7922 2020 2020 2020 2020  ds.very"        
+00000f20: 2020 2020 203a 2074 7275 650a 2020 2020       : true.    
+00000f30: 7d0a 7d0a                                }.}.
```

### Comparing `proselint-0.8.0/proselint/checks/airlinese/misc.py` & `proselint-0.9.0/proselint/checks/airlinese/misc.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/annotations/misc.py` & `proselint-0.9.0/proselint/checks/annotations/misc.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/archaism/misc.py` & `proselint-0.9.0/proselint/checks/archaism/misc.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/cliches/hell.py` & `proselint-0.9.0/proselint/checks/cliches/hell.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/cliches/misc.py` & `proselint-0.9.0/proselint/checks/cliches/misc.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/consistency/spacing.py` & `proselint-0.9.0/proselint/checks/consistency/spacing.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/consistency/spelling.py` & `proselint-0.9.0/proselint/checks/consistency/spelling.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/corporate_speak/misc.py` & `proselint-0.9.0/proselint/checks/corporate_speak/misc.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/cursing/filth.py` & `proselint-0.9.0/proselint/checks/cursing/filth.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/cursing/nfl.py` & `proselint-0.9.0/proselint/checks/cursing/nfl.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/cursing/nword.py` & `proselint-0.9.0/proselint/checks/cursing/nword.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/dates_times/am_pm.py` & `proselint-0.9.0/proselint/checks/dates_times/am_pm.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/dates_times/dates.py` & `proselint-0.9.0/proselint/checks/dates_times/dates.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/hedging/misc.py` & `proselint-0.9.0/proselint/checks/hedging/misc.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/jargon/misc.py` & `proselint-0.9.0/proselint/checks/jargon/misc.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/lexical_illusions/misc.py` & `proselint-0.9.0/proselint/checks/lexical_illusions/misc.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/lgbtq/offensive_terms.py` & `proselint-0.9.0/proselint/checks/lgbtq/offensive_terms.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/lgbtq/terms.py` & `proselint-0.9.0/proselint/checks/lgbtq/terms.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/links/broken.py` & `proselint-0.9.0/proselint/checks/links/broken.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     msg = u"Broken link: {}"
 
     regex = re.compile(
         r"""(?i)\b((?:https?://|www\d{0,3}[.]
         |[a-z0-9.\-]+[.][a-z]{2,4}/)(?:[^\s()<>]+|\(([^\s()<>]+
         |(\([^\s()<>]+\)))*\))+(?:\(([^\s()<>]+|(\([^\s()<>]+\)))*\)
         |[^\s`!()\[\]{};:\'".,<>?\xab\xbb\u201c\u201d\u2018\u2019\u21a9]))""",
-        re.U)
+        re.U | re.X)
 
     errors = []
     for m in re.finditer(regex, text):
         url = m.group(0).strip()
 
         if "http://" not in url and "https://" not in url:
             url = "http://" + url
```

### Comparing `proselint-0.8.0/proselint/checks/malapropisms/misc.py` & `proselint-0.9.0/proselint/checks/malapropisms/misc.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/misc/apologizing.py` & `proselint-0.9.0/proselint/checks/misc/apologizing.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/misc/back_formations.py` & `proselint-0.9.0/proselint/checks/misc/back_formations.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/misc/bureaucratese.py` & `proselint-0.9.0/proselint/checks/misc/bureaucratese.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/misc/but.py` & `proselint-0.9.0/proselint/checks/misc/but.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/misc/capitalization.py` & `proselint-0.9.0/proselint/checks/misc/capitalization.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/misc/chatspeak.py` & `proselint-0.9.0/proselint/checks/misc/chatspeak.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/misc/commercialese.py` & `proselint-0.9.0/proselint/checks/misc/commercialese.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/misc/composition.py` & `proselint-0.9.0/proselint/checks/misc/composition.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/misc/currency.py` & `proselint-0.9.0/proselint/checks/misc/currency.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/misc/debased.py` & `proselint-0.9.0/proselint/checks/misc/debased.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/misc/false_plurals.py` & `proselint-0.9.0/proselint/checks/misc/false_plurals.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/misc/greylist.py` & `proselint-0.9.0/proselint/checks/misc/greylist.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/misc/illogic.py` & `proselint-0.9.0/proselint/checks/misc/illogic.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/misc/inferior_superior.py` & `proselint-0.9.0/proselint/checks/misc/inferior_superior.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/misc/institution_name.py` & `proselint-0.9.0/proselint/checks/misc/institution_name.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/misc/latin.py` & `proselint-0.9.0/proselint/checks/misc/latin.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/misc/many_a.py` & `proselint-0.9.0/proselint/checks/misc/many_a.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/misc/metaconcepts.py` & `proselint-0.9.0/proselint/checks/misc/metaconcepts.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/misc/metadiscourse.py` & `proselint-0.9.0/proselint/checks/misc/metadiscourse.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/misc/narcissism.py` & `proselint-0.9.0/proselint/checks/misc/narcissism.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/misc/not_guilty.py` & `proselint-0.9.0/proselint/checks/misc/not_guilty.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/misc/phrasal_adjectives.py` & `proselint-0.9.0/proselint/checks/misc/phrasal_adjectives.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/misc/preferred_forms.py` & `proselint-0.9.0/proselint/checks/misc/preferred_forms.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/misc/pretension.py` & `proselint-0.9.0/proselint/checks/misc/pretension.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/misc/professions.py` & `proselint-0.9.0/proselint/checks/misc/professions.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/misc/punctuation.py` & `proselint-0.9.0/proselint/checks/misc/punctuation.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/misc/scare_quotes.py` & `proselint-0.9.0/proselint/checks/misc/scare_quotes.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/misc/suddenly.py` & `proselint-0.9.0/proselint/checks/misc/suddenly.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/misc/tense_present.py` & `proselint-0.9.0/proselint/checks/misc/tense_present.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/misc/usage.py` & `proselint-0.9.0/proselint/checks/misc/usage.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/misc/waxed.py` & `proselint-0.9.0/proselint/checks/misc/waxed.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/mixed_metaphors/misc.py` & `proselint-0.9.0/proselint/checks/mixed_metaphors/misc.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/mondegreens/misc.py` & `proselint-0.9.0/proselint/checks/mondegreens/misc.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/needless_variants/misc.py` & `proselint-0.9.0/proselint/checks/needless_variants/misc.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/nonwords/misc.py` & `proselint-0.9.0/proselint/checks/nonwords/misc.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/oxymorons/misc.py` & `proselint-0.9.0/proselint/checks/oxymorons/misc.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/psychology/misc.py` & `proselint-0.9.0/proselint/checks/psychology/misc.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/redundancy/misc.py` & `proselint-0.9.0/proselint/checks/redundancy/misc.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/redundancy/ras_syndrome.py` & `proselint-0.9.0/proselint/checks/redundancy/ras_syndrome.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/security/credit_card.py` & `proselint-0.9.0/proselint/checks/security/credit_card.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/security/password.py` & `proselint-0.9.0/proselint/checks/security/password.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/sexism/misc.py` & `proselint-0.9.0/proselint/checks/sexism/misc.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/skunked_terms/misc.py` & `proselint-0.9.0/proselint/checks/skunked_terms/misc.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/spelling/able_atable.py` & `proselint-0.9.0/proselint/checks/spelling/able_atable.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/spelling/able_ible.py` & `proselint-0.9.0/proselint/checks/spelling/able_ible.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/spelling/athletes.py` & `proselint-0.9.0/proselint/checks/spelling/athletes.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/spelling/em_im_en_in.py` & `proselint-0.9.0/proselint/checks/spelling/em_im_en_in.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/spelling/er_or.py` & `proselint-0.9.0/proselint/checks/spelling/er_or.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/spelling/in_un.py` & `proselint-0.9.0/proselint/checks/spelling/in_un.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/spelling/misc.py` & `proselint-0.9.0/proselint/checks/spelling/misc.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/terms/animal_adjectives.py` & `proselint-0.9.0/proselint/checks/terms/animal_adjectives.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/terms/denizen_labels.py` & `proselint-0.9.0/proselint/checks/terms/denizen_labels.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/terms/eponymous_adjectives.py` & `proselint-0.9.0/proselint/checks/terms/eponymous_adjectives.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/terms/venery.py` & `proselint-0.9.0/proselint/checks/terms/venery.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/typography/diacritical_marks.py` & `proselint-0.9.0/proselint/checks/typography/diacritical_marks.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/typography/exclamation.py` & `proselint-0.9.0/proselint/checks/typography/exclamation.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/typography/symbols.py` & `proselint-0.9.0/proselint/checks/typography/symbols.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/uncomparables/misc.py` & `proselint-0.9.0/proselint/checks/uncomparables/misc.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/checks/weasel_words/very.py` & `proselint-0.9.0/proselint/checks/weasel_words/very.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/command_line.py` & `proselint-0.9.0/proselint/command_line.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 """Command line utility for proselint."""
 from __future__ import print_function
 from __future__ import absolute_import
 from builtins import str
 
@@ -46,15 +45,14 @@
 def clear_cache():
     """Delete the contents of the cache."""
     click.echo("Deleting the cache...")
 
     # see issue #624
     _delete_compiled_python_files()
     _delete_cache()
-    _create_home_cache()
 
 
 def _delete_compiled_python_files():
     """Remove files with a 'pyc' extension."""
     for path, _, files in os.walk(os.getcwd()):
         for fname in [f for f in files if os.path.splitext(f)[1] == ".pyc"]:
             try:
@@ -68,22 +66,14 @@
     proselint_cache = os.path.join("proselint", "cache")
     try:
         shutil.rmtree(proselint_cache)
     except OSError:
         pass
 
 
-def _create_home_cache():
-    """Create a cache in the users 'HOME' directory."""
-    try:
-        os.makedirs(os.path.join(os.path.expanduser("~"), ".proselint"))
-    except OSError:
-        pass
-
-
 def print_errors(filename, errors, output_json=False, compact=False):
     """Print the errors, resulting from lint, for filename."""
     if output_json:
         click.echo(errors_to_json(errors))
 
     else:
         for error in errors:
```

### Comparing `proselint-0.8.0/proselint/demo.md` & `proselint-0.9.0/proselint/demo.md`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/proselint/score.py` & `proselint-0.9.0/proselint/score.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 """Compute the lintscore on the corpus."""
 
 from __future__ import print_function
 from builtins import input
 from builtins import int
```

### Comparing `proselint-0.8.0/proselint/tools.py` & `proselint-0.9.0/proselint/tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 """General-purpose tools shared across linting checks."""
 
 from __future__ import print_function
 from __future__ import unicode_literals
 import sys
@@ -44,14 +43,32 @@
     @functools.wraps(f)
     def wrapped(*args, **kwargs):
         f(*args, **kwargs)
         close_cache_shelves()
     return wrapped
 
 
+def _get_xdg_path(variable_name, default_path):
+    path = os.environ.get(variable_name)
+    if path is None or path == '':
+        return default_path
+    else:
+        return path
+
+
+def _get_xdg_config_home():
+    return _get_xdg_path('XDG_CONFIG_HOME',
+                         os.path.join(os.path.expanduser('~'), '.config'))
+
+
+def _get_xdg_cache_home():
+    return _get_xdg_path('XDG_CACHE_HOME',
+                         os.path.join(os.path.expanduser('~'), '.cache'))
+
+
 def _get_cache(cachepath):
     if cachepath in _cache_shelves:
         return _cache_shelves[cachepath]
 
     try:
         cache = shelve.open(cachepath, protocol=2)
     except dbm.error:
@@ -78,19 +95,24 @@
     _cache_shelves[cachepath] = cache
     return cache
 
 
 def memoize(f):
     """Cache results of computations on disk."""
     # Determine the location of the cache.
-    cache_dirname = os.path.join(os.path.expanduser("~"), ".proselint")
+    cache_dirname = os.path.join(_get_xdg_cache_home(), 'proselint')
+    legacy_cache_dirname = os.path.join(os.path.expanduser("~"), ".proselint")
 
-    # Create the cache if it does not already exist.
     if not os.path.isdir(cache_dirname):
-        os.mkdir(cache_dirname)
+        # Migrate the cache from the legacy path to XDG complaint location.
+        if os.path.isdir(legacy_cache_dirname):
+            os.rename(legacy_cache_dirname, cache_dirname)
+        # Create the cache if it does not already exist.
+        else:
+            os.makedirs(cache_dirname)
 
     cache_filename = f.__module__ + "." + f.__name__
     cachepath = os.path.join(cache_dirname, cache_filename)
 
     @functools.wraps(f)
     def wrapped(*args, **kwargs):
 
@@ -154,19 +176,29 @@
         try:
             options = json.load(open(filename))
             break
         except IOError:
             pass
 
     try:
-        user_options = json.load(open(os.path.expanduser('~/.proselintrc')))
+        user_options = json.load(
+            open(os.path.join(_get_xdg_config_home(), 'proselint', 'config')))
         has_overrides = True
     except IOError:
         pass
 
+    # Read user configuration from the legacy path.
+    if not has_overrides:
+        try:
+            user_options = json.load(
+                open(os.path.join(os.path.expanduser('~'), '.proselintrc')))
+            has_overrides = True
+        except IOError:
+            pass
+
     if has_overrides:
         if 'max_errors' in user_options:
             options['max_errors'] = user_options['max_errors']
         if 'checks' in user_options:
             for (key, value) in user_options['checks'].items():
                 try:
                     options['checks'][key] = value
```

### Comparing `proselint-0.8.0/proselint.egg-info/SOURCES.txt` & `proselint-0.9.0/proselint.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -133,14 +133,15 @@
 proselint/checks/uncomparables/misc.py
 proselint/checks/weasel_words/__init__.py
 proselint/checks/weasel_words/misc.py
 proselint/checks/weasel_words/very.py
 tests/__init__.py
 tests/_test_version.py
 tests/check.py
+tests/illegal-chars.txt
 tests/test_annotations.py
 tests/test_archaism.py
 tests/test_butterick_symbols.py
 tests/test_clear_cache.py
 tests/test_cliches.py
 tests/test_consistency_check.py
 tests/test_consistency_spacing.py
```

### Comparing `proselint-0.8.0/README.md` & `proselint-0.9.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -13,33 +13,53 @@
 
 `proselint` places the world’s greatest writers and editors by your side, where they whisper suggestions on how to improve your prose. You’ll be guided by advice inspired by Bryan Garner, David Foster Wallace, Chuck Palahniuk, Steve Pinker, Mary Norris, Mark Twain, Elmore Leonard, George Orwell, Matthew Butterick, William Strunk, E.B. White, Philip Corbett, Ernest Gowers, and the editorial staff of the world’s finest literary magazines and newspapers, among others. Our goal is to aggregate knowledge about best practices in writing and to make that knowledge immediately accessible to all authors in the form of a linter for prose.
 
 `proselint` is a command-line utility that can be integrated into existing tools.
 
 ### Installation
 
-To get this up and running, install it using pip:
+To get this up and running, install it using [pip](https://packaging.python.org/installing/#use-pip-for-installing):
 
 ```
 pip install proselint
 ```
 
+#### Fedora
+
+```
+sudo dnf install proselint
+```
+
+#### Debian
+
+```
+sudo apt install python3-proselint
+```
+
+#### Ubuntu
+
+```
+sudo add-apt-repository universe
+sudo apt install python3-proselint
+```
+
 ### Plugins for other software
 
 `proselint` is available on:
 
 - [x] A [demo editor](http://proselint.com/write)
 - [x] [Sublime Text](https://github.com/amperser/proselint/tree/master/plugins/sublime/SublimeLinter-contrib-proselint)
 - [x] [Atom Editor](https://github.com/smockle/linter-proselint) (thanks to [Clay Miller](https://github.com/smockle)).
-- [x] [Emacs via Flycheck](https://github.com/amperser/proselint/tree/master/plugins/flycheck) (thanks to [Aaron Jacobs](https://github.com/atheriel))
-- [x] [Vim](https://github.com/vim-syntastic/syntastic) (thanks to @lcd047 & @Carreau)
+- [x] [Emacs via Flycheck](http://www.flycheck.org/).
+- [x] Vim via [ALE](https://github.com/w0rp/ale) or [Syntastic](https://github.com/vim-syntastic/syntastic) (thanks to @lcd047, @Carreau, and [Daniel M. Capella](https://github.com/polyzen))
 - [x] [Phabricator's `arc` CLI](https://github.com/google/arc-proselint) (thanks to [Jeff Verkoeyen](https://github.com/jverkoey))
 - [x] [Danger](https://github.com/dbgrandi/danger-prose) (thanks to [David Grandinetti](https://github.com/dbgrandi) and [Orta Therox](https://github.com/orta))
 - [x] [Visual Studio Code](https://github.com/ppeszko/vscode-proselint) (thanks to [Patryk Peszko](https://github.com/ppeszko))
-- [x] [coala](https://github.com/coala-analyzer/bear-docs/blob/master/docs/ProseLintBear.rst) (thanks to the [coala Development Group](https://github.com/coala-analyzer))  
+- [x] [coala](https://github.com/coala-analyzer/bear-docs/blob/master/docs/ProseLintBear.rst) (thanks to the [coala Development Group](https://github.com/coala-analyzer))
+- [x] [IntelliJ](https://github.com/kropp/intellij-proselint) (by [Victor Kropp](https://github.com/kropp))
 
 ### Usage
 
 Suppose you had a document `text.md` with the following text:
 
 ```
 John is very unique.
@@ -118,15 +138,16 @@
 
 ```python
 [('weasel_words.very', "Substitute 'damn' every time you're inclined to write 'very;' your editor will delete it and the writing will be just as it should be.", 0, 17, 17, 22, 5, 'warning', None), ('uncomparables.misc', "Comparison of an uncomparable: 'very unique.' is not comparable.", 0, 17, 17, 29, 12, 'warning', None)]
 ```
 
 ### Checks
 
-You can disable any of the checks by modifying `~/.proselintrc`:
+You can disable any of the checks by modifying `$XDG_CONFIG_HOME/proselint/config`. If `$XDG_CONFIG_HOME` is not set or empty, `~/.config/proselint/config` will be used.
+Additionally for compatible reason, the legacy configuration `~/.proselintrc` will be used if `$XDG_CONFIG_HOME/proselint/config` does not exist.
 
 ```json
 {
   "checks": {
     "typography.diacritical_marks": false
   }
 }
@@ -224,14 +245,14 @@
 ### Running Automated Tests
 
 Automated tests are included in the `proselint/tests` directory. To run these tests locally, use the test runner [nose](http://nose.readthedocs.io/en/latest/) and run the following commands:
 ```bash
 cd tests/
 nosetests
 ```
-and watch the output. Nose is compatible with Python versions 2.7, 3.3, 3.4 and 3.5.
+and watch the output. Nose is compatible with Python versions 2.7, 3.4, 3.5 and 3.6.
 
 All automated tests in `tests/` are run as part of each submitted pull request, including newly added tests.
 
 ### License
 
 The project is licensed under the BSD license.
```

### Comparing `proselint-0.8.0/tests/check.py` & `proselint-0.9.0/tests/check.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/tests/test_annotations.py` & `proselint-0.9.0/tests/test_annotations.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class TestCheck(Check):
     """The test class for annotations.misc."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
         """Basic smoke test for annotations.misc."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
         assert self.passes("""Add it to the to do list.""")
         assert not self.passes("""Add it to the TODO list.""")
```

### Comparing `proselint-0.8.0/tests/test_archaism.py` & `proselint-0.9.0/tests/test_misc_apologizing.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-"""Tests for archaism.misc check."""
+"""Tests for misc.apologizing check."""
 from __future__ import absolute_import
 
 from .check import Check
 
-from proselint.checks.archaism import misc as chk
+from proselint.checks.misc import apologizing as chk
 
 
 class TestCheck(Check):
-    """The test class for archaism.misc."""
+    """The test class for misc.apologizing."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
-        """Basic smoke test for archaism.misc."""
+        """Basic smoke test for misc.apologizing."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
-        assert self.passes("""I want to sleep, and maybe dream.""")
-        assert not self.passes("""I want to sleep, perchance to dream.""")
+        assert not self.passes("""More research is needed.""")
```

### Comparing `proselint-0.8.0/tests/test_butterick_symbols.py` & `proselint-0.9.0/tests/test_typography_symbols.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class TestCheck(Check):
     """The test class for typography.symbols."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_ellipsis(self):
         """Find ... in a string."""
         assert chk.check_ellipsis("""The long and winding road...""")
 
     def test_copyright(self):
```

### Comparing `proselint-0.8.0/tests/test_clear_cache.py` & `proselint-0.9.0/tests/test_clear_cache.py`

 * *Files 9% similar despite different names*

```diff
@@ -136,31 +136,7 @@
         """Ignore if unable to delete."""
         cl._delete_cache()
 
     @mock.patch('shutil.rmtree', side_effect=OSError)
     def test_on_oserror(self, mock_rmtree):
         """Ignore if general OSError."""
         cl._delete_cache()
-
-
-class Test_create_home_cache(unittest.TestCase):
-    """proselint.command_line._create_home_cache()."""
-
-    def setUp(self):
-        """Init common data."""
-        self.cache_path = os.path.join(os.path.expanduser("~"), ".proselint")
-
-    @mock.patch('os.makedirs')
-    def test_makedir(self, mock_makedir):
-        """correct directory is used."""
-        cl._create_home_cache()
-        mock_makedir.assert_called_with(self.cache_path)
-
-    @mock.patch('os.makedirs', side_effect=OSError)
-    def test_on_oserror(self, mock_rmtree):
-        """Ignore if general OSError."""
-        cl._create_home_cache()
-
-    @mock.patch('os.makedirs', side_effect=PermissionError)
-    def test__no_permission(self, mock_rmtree):
-        """Ignore if unable to delete."""
-        cl._create_home_cache()
```

### Comparing `proselint-0.8.0/tests/test_cliches.py` & `proselint-0.9.0/tests/test_cliches.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class TestCheck(Check):
     """The test class for cliches.misc."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def setUp(self):
         """Create test sentences."""
         self.l_garner = """Worse than a fate worse than death."""
         self.l_write_good = """He's a chip off the old block."""
         self.l_gnu_diction = """It's a matter of concern."""
```

### Comparing `proselint-0.8.0/tests/test_consistency_check.py` & `proselint-0.9.0/tests/test_consistency_check.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class TestCheck(Check):
     """The test class for tools.consistency_check."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def setUp(self):
         """Create some test fixtures."""
         self.l = [['colour', 'color']]
         self.err = 'error message'
         self.msg = 'inconsistent form of {} vs {}'
```

### Comparing `proselint-0.8.0/tests/test_consistency_spacing.py` & `proselint-0.9.0/tests/test_consistency_spacing.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class TestCheck(Check):
     """The test class for consistency.spacing."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
         """Basic smoke test for consistency.spacing."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
         assert self.passes(
             """This is good. Only one space each time. Every time.""")
```

### Comparing `proselint-0.8.0/tests/test_consistency_spelling.py` & `proselint-0.9.0/tests/test_consistency_spelling.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class TestCheck(Check):
     """The test class for consistency.spelling."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
         """Basic smoke test for consistency.spelling."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
         assert self.passes("""The centre for the arts is the art centre.""")
         assert self.passes("""The center for the arts is the art center.""")
```

### Comparing `proselint-0.8.0/tests/test_corporate_speak.py` & `proselint-0.9.0/tests/test_corporate_speak.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class TestCheck(Check):
     """The test class for corporate_speak.misc."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
         """Basic smoke test for corporate_speak.misc."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
         assert self.passes("""We will discuss it later.""")
         assert not self.passes("""We will circle back around to it.""")
```

### Comparing `proselint-0.8.0/tests/test_cursing_filth.py` & `proselint-0.9.0/tests/test_cursing_filth.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,14 @@
 class TestCheck(Check):
     """The test class for cursing.filth."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
         """Basic smoke test for cursing.filth."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
         assert not self.passes("""Bad shit in this phrase.""")
```

### Comparing `proselint-0.8.0/tests/test_cursing_nfl.py` & `proselint-0.9.0/tests/test_cursing_nfl.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,14 @@
 class TestCheck(Check):
     """The test class for cursing.nfl."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
         """Basic smoke test for cursing.nfl."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
         assert not self.passes("""The QB is named ball licker.""")
```

### Comparing `proselint-0.8.0/tests/test_cursing_nword.py` & `proselint-0.9.0/tests/test_cursing_nword.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,14 @@
 class TestCheck(Check):
     """The test class for cursing.nword."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
         """Basic smoke test for cursing.nword."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
         assert not self.passes("""The n-word.""")
```

### Comparing `proselint-0.8.0/tests/test_dates_times_am_pm.py` & `proselint-0.9.0/tests/test_dates_times_am_pm.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class TestCheck(Check):
     """The test class for dates_times.am_pm."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke_check_lowercase_periods(self):
         """Basic smoke test.
 
         This is for the function
         dates_times.am_pm.check_lowercase_periods.
```

### Comparing `proselint-0.8.0/tests/test_dates_times_dates.py` & `proselint-0.9.0/tests/test_dates_times_dates.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class TestCheck(Check):
     """The test class for dates_times.dates."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke_check_decade_apostrophes_short(self):
         """Basic smoke test.
 
         This for the function
         dates_times.dates.check_decade_apostrophes_short.
```

### Comparing `proselint-0.8.0/tests/test_dfw_uncomparables.py` & `proselint-0.9.0/tests/test_dfw_uncomparables.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 class TestCheck(Check):
     """The test class for dfw.uncomparables."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_sample_phrases(self):
         """Find 'very unique'."""
         assert not self.passes("""This sentence is very unique.""")
 
     def test_linebreaks(self):
```

### Comparing `proselint-0.8.0/tests/test_existence_check.py` & `proselint-0.9.0/tests/test_existence_check.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class TestCheck(Check):
     """The test class for tools.existence_check."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def setUp(self):
         """setUp method creating some test fixtures."""
         self.l = ['abc']
         self.err = 'error message'
         self.msg = 'it exists'
```

### Comparing `proselint-0.8.0/tests/test_exit_codes.py` & `proselint-0.9.0/tests/test_exit_codes.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/tests/test_garner_dates.py` & `proselint-0.9.0/tests/test_garner_dates.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/tests/test_hedging.py` & `proselint-0.9.0/tests/test_misc_pretension.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-"""Tests for hedging.misc check."""
+"""Tests for misc.pretension check."""
 from __future__ import absolute_import
 
 from .check import Check
 
-from proselint.checks.hedging import misc as chk
+from proselint.checks.misc import pretension as chk
 
 
 class TestCheck(Check):
-    """The test class for hedging.misc."""
+    """The test class for misc.pretension."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
-        """Basic smoke test for hedging.misc."""
+        """Basic smoke test for misc.pretension."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
-        assert not self.passes("""I would argue that this is a good test.""")
+        assert not self.passes("""We need to reconceptualize the project.""")
```

### Comparing `proselint-0.8.0/tests/test_hyperbole.py` & `proselint-0.9.0/tests/test_hyperbole.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,14 @@
 class TestCheck(Check):
     """The test class for hyperbole.misc."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
         """Basic smoke test for hyperbole.misc."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
         assert not self.passes("""So exaggerated!!!""")
```

### Comparing `proselint-0.8.0/tests/test_illegal_chars.py` & `proselint-0.9.0/tests/test_illegal_chars.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/tests/test_jargon.py` & `proselint-0.9.0/tests/test_misc_currency.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-"""Tests for jargon.misc check."""
+"""Tests for misc.currency check."""
 from __future__ import absolute_import
 
 from .check import Check
 
-from proselint.checks.jargon import misc as chk
+from proselint.checks.misc import currency as chk
 
 
 class TestCheck(Check):
-    """The test class for jargon.misc."""
+    """The test class for misc.currency."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
-        """Basic smoke test for jargon.misc."""
+        """Basic smoke test for misc.currency."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
-        assert not self.passes("""I agree it's in the affirmative.""")
+        assert not self.passes("""It cost $10 dollars.""")
```

### Comparing `proselint-0.8.0/tests/test_leonard.py` & `proselint-0.9.0/tests/test_leonard.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/tests/test_lexical_illusions.py` & `proselint-0.9.0/tests/test_lexical_illusions.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,14 +9,14 @@
 class TestCheck(Check):
     """The test class for lexical_illusions.misc."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
         """Basic smoke test for lexical_illusions.misc."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
         assert not self.passes("""Paris in the the springtime.""")
```

### Comparing `proselint-0.8.0/tests/test_lgbtq_offensive_terms.py` & `proselint-0.9.0/tests/test_lgbtq_offensive_terms.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class TestCheck(Check):
     """The test class for lgbtq.offensive_terms."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
         """Basic smoke test for lgbtq.offensive_terms."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
         assert self.passes("""I once met a gay man.""")
         assert not self.passes("""I once met a fag.""")
```

### Comparing `proselint-0.8.0/tests/test_lgbtq_terms.py` & `proselint-0.9.0/tests/test_lgbtq_terms.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class TestCheck(Check):
     """The test class for lgbtq.terms."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
         """Basic smoke test for lgbtq.terms."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
         assert self.passes("""They were a gay couple.""")
         assert not self.passes("""He was a homosexual man.""")
```

### Comparing `proselint-0.8.0/tests/test_malaproprisms.py` & `proselint-0.9.0/tests/test_malaproprisms.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,14 @@
 class TestCheck(Check):
     """The test class for malaproprisms.misc."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
         """Basic smoke test for malaproprisms.misc."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
         assert not self.passes("""Found in the Infinitesimal Universe.""")
```

### Comparing `proselint-0.8.0/tests/test_misc_apologizing.py` & `proselint-0.9.0/tests/test_security_password.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-"""Tests for misc.apologizing check."""
+"""Tests for security.password check."""
 from __future__ import absolute_import
 
 from .check import Check
 
-from proselint.checks.misc import apologizing as chk
+from proselint.checks.security import password as chk
 
 
 class TestCheck(Check):
-    """The test class for misc.apologizing."""
+    """The test class for security.password."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
-        """Basic smoke test for misc.apologizing."""
+        """Basic smoke test for security.password."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
-        assert not self.passes("""More research is needed.""")
+        assert not self.passes("""The password is 123456.""")
+        assert not self.passes("""My password is PASSWORD.""")
```

### Comparing `proselint-0.8.0/tests/test_misc_back_formations.py` & `proselint-0.9.0/tests/test_misc_back_formations.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,14 @@
 class TestCheck(Check):
     """The test class for misc.back_formations."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
         """Basic smoke test for misc.back_formations."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
         assert not self.passes("""It is an improprietous use.""")
```

### Comparing `proselint-0.8.0/tests/test_misc_bureaucratese.py` & `proselint-0.9.0/tests/test_misc_bureaucratese.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class TestCheck(Check):
     """The test class for misc.bureaucratese."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
         """Basic smoke test for misc.bureaucratese."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
         assert not self.passes(
             """I hope the report meets with your approval.""")
```

### Comparing `proselint-0.8.0/tests/test_misc_but.py` & `proselint-0.9.0/tests/test_misc_chatspeak.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-"""Tests for misc.but check."""
+"""Tests for misc.chatspeak check."""
 from __future__ import absolute_import
 
 from .check import Check
 
-from proselint.checks.misc import but as chk
+from proselint.checks.misc import chatspeak as chk
 
 
 class TestCheck(Check):
-    """The test class for misc.but."""
+    """The test class for misc.chatspeak."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
-        """Basic smoke test for misc.but."""
+        """Basic smoke test for misc.chatspeak."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
-        assert not self.passes("""But I never start with the word "but".""")
+        assert not self.passes("""BRB getting coffee.""")
```

### Comparing `proselint-0.8.0/tests/test_misc_capitalization.py` & `proselint-0.9.0/tests/test_misc_capitalization.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class TestCheck(Check):
     """The test class for misc.capitalization."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
         """Basic smoke test for misc.capitalization.check."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
         assert not self.passes("""It goes back to the stone age.""")
```

### Comparing `proselint-0.8.0/tests/test_misc_chatspeak.py` & `proselint-0.9.0/tests/test_misc_waxed.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-"""Tests for misc.chatspeak check."""
+"""Tests for misc.waxed check."""
 from __future__ import absolute_import
 
 from .check import Check
 
-from proselint.checks.misc import chatspeak as chk
+from proselint.checks.misc import waxed as chk
 
 
 class TestCheck(Check):
-    """The test class for misc.chatspeak."""
+    """The test class for misc.waxed."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
-        """Basic smoke test for misc.chatspeak."""
+        """Basic smoke test for misc.waxed."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
-        assert not self.passes("""BRB getting coffee.""")
+        assert not self.passes("""They really could wax poetically.""")
```

### Comparing `proselint-0.8.0/tests/test_misc_commercialese.py` & `proselint-0.9.0/tests/test_skunked_terms.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-"""Tests for misc.commercialese check."""
+"""Tests for skunked_terms.misc check."""
 from __future__ import absolute_import
 
 from .check import Check
 
-from proselint.checks.misc import commercialese as chk
+from proselint.checks.skunked_terms import misc as chk
 
 
 class TestCheck(Check):
-    """The test class for misc.commercialese."""
+    """The test class for skunked_terms.misc."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
-        """Basic smoke test for misc.commercialese."""
+        """Basic smoke test for skunked_terms.misc."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
-        assert not self.passes("""We regret to inform you of this.""")
+        assert not self.passes(
+            """I gave an impassionate defence of the situation.""")
```

### Comparing `proselint-0.8.0/tests/test_misc_composition.py` & `proselint-0.9.0/tests/test_misc_composition.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,14 @@
 class TestCheck(Check):
     """The test class for misc.composition."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
         """Basic smoke test for misc.composition."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
         assert not self.passes("""His story is not honest.""")
```

### Comparing `proselint-0.8.0/tests/test_misc_currency.py` & `proselint-0.9.0/tests/test_misc_but.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-"""Tests for misc.currency check."""
+"""Tests for misc.but check."""
 from __future__ import absolute_import
 
 from .check import Check
 
-from proselint.checks.misc import currency as chk
+from proselint.checks.misc import but as chk
 
 
 class TestCheck(Check):
-    """The test class for misc.currency."""
+    """The test class for misc.but."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
-        """Basic smoke test for misc.currency."""
+        """Basic smoke test for misc.but."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
-        assert not self.passes("""It cost $10 dollars.""")
+        assert not self.passes("""But I never start with the word "but".""")
```

### Comparing `proselint-0.8.0/tests/test_misc_debased.py` & `proselint-0.9.0/tests/test_misc_debased.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,14 @@
 class TestCheck(Check):
     """The test class for misc.debased."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
         """Basic smoke test for misc.debased."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
         assert not self.passes("""This leaves much to be desired.""")
```

### Comparing `proselint-0.8.0/tests/test_misc_false_plurals.py` & `proselint-0.9.0/tests/test_misc_false_plurals.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class TestCheck(Check):
     """The test class for misc.false_plurals."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
         """Basic smoke test for misc.false_plurals."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
         assert not self.passes("""There were several phenomenons.""")
```

### Comparing `proselint-0.8.0/tests/test_misc_greylist.py` & `proselint-0.9.0/tests/test_hedging.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-"""Tests for misc.greylist check."""
+"""Tests for hedging.misc check."""
 from __future__ import absolute_import
 
 from .check import Check
 
-from proselint.checks.misc import greylist as chk
+from proselint.checks.hedging import misc as chk
 
 
 class TestCheck(Check):
-    """The test class for misc.greylist."""
+    """The test class for hedging.misc."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
-        """Basic smoke test for misc.greylist."""
+        """Basic smoke test for hedging.misc."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
-        assert not self.passes("""She should utilize her knowledge.""")
+        assert not self.passes("""I would argue that this is a good test.""")
```

### Comparing `proselint-0.8.0/tests/test_misc_illogic.py` & `proselint-0.9.0/tests/test_misc_illogic.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class TestCheck(Check):
     """The test class for misc.illogic."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
         """Basic smoke test for misc.illogic."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
         assert not self.passes("""We should preplan the trip.""")
```

### Comparing `proselint-0.8.0/tests/test_misc_inferior_superior.py` & `proselint-0.9.0/tests/test_misc_inferior_superior.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class TestCheck(Check):
     """The test class for misc.inferior_superior."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
         """Basic smoke test for misc.inferior_superior."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
         assert not self.passes(
             """It was more inferior than the alternative.""")
```

### Comparing `proselint-0.8.0/tests/test_misc_latin.py` & `proselint-0.9.0/tests/test_misc_latin.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,14 @@
 class TestCheck(Check):
     """The test class for misc.latin."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
         """Basic smoke test for misc.latin."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
         assert not self.passes("""And ceteris paribus, it was good.""")
```

### Comparing `proselint-0.8.0/tests/test_misc_many_a.py` & `proselint-0.9.0/tests/test_misc_many_a.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class TestCheck(Check):
     """The test class for misc.many_a."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
         """Basic smoke test for misc.many_a."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
         assert not self.passes(
             """There were many a day I thought about it.""")
```

### Comparing `proselint-0.8.0/tests/test_misc_metadiscourse.py` & `proselint-0.9.0/tests/test_misc_metadiscourse.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,14 +9,14 @@
 class TestCheck(Check):
     """The test class for misc.metadiscourse."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
         """Basic smoke test for misc.metadiscourse."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
         assert not self.passes("""It's based on the rest of this article.""")
```

### Comparing `proselint-0.8.0/tests/test_misc_narcissism.py` & `proselint-0.9.0/tests/test_misc_greylist.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-"""Tests for misc.narcissism check."""
+"""Tests for misc.greylist check."""
 from __future__ import absolute_import
 
 from .check import Check
 
-from proselint.checks.misc import narcissism as chk
+from proselint.checks.misc import greylist as chk
 
 
 class TestCheck(Check):
-    """The test class for misc.narcissism."""
+    """The test class for misc.greylist."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
-        """Basic smoke test for misc.narcissism."""
+        """Basic smoke test for misc.greylist."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
-        assert not self.passes(
-            """In recent years, an increasing number of scientists have studied
-             the problem in detail.""")
+        assert not self.passes("""She should utilize her knowledge.""")
```

### Comparing `proselint-0.8.0/tests/test_misc_not_guilty.py` & `proselint-0.9.0/tests/test_misc_not_guilty.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class TestCheck(Check):
     """The test class for misc.not_guilty."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
         """Basic smoke test for misc.not_guilty."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
         assert not self.passes(
             """She is not guilty beyond a reasonable doubt.""")
```

### Comparing `proselint-0.8.0/tests/test_misc_phrasal_adjectives.py` & `proselint-0.9.0/tests/test_misc_phrasal_adjectives.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class TestCheck(Check):
     """The test class for misc.phrasal_adjectives."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
         """Basic smoke test for misc.phrasal_adjectives."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
         assert not self.passes("""There were across the board discounts.""")
```

### Comparing `proselint-0.8.0/tests/test_misc_preferred_forms.py` & `proselint-0.9.0/tests/test_misc_preferred_forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,14 @@
 class TestCheck(Check):
     """The test class for misc.preferred_forms."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
         """Basic smoke test for misc.preferred_forms."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
         assert not self.passes("""It was almost haloween.""")
```

### Comparing `proselint-0.8.0/tests/test_misc_pretension.py` & `proselint-0.9.0/tests/test_sexism.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-"""Tests for misc.pretension check."""
+"""Tests for sexism.misc check."""
 from __future__ import absolute_import
 
 from .check import Check
 
-from proselint.checks.misc import pretension as chk
+from proselint.checks.sexism import misc as chk
 
 
 class TestCheck(Check):
-    """The test class for misc.pretension."""
+    """The test class for sexism.misc."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
-        """Basic smoke test for misc.pretension."""
+        """Basic smoke test for sexism.misc."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
-        assert not self.passes("""We need to reconceptualize the project.""")
+        assert not self.passes(
+            """The legal team had two lawyers and a lady lawyer.""")
```

### Comparing `proselint-0.8.0/tests/test_misc_professions.py` & `proselint-0.9.0/tests/test_terms_venery.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-"""Tests for misc.professions check."""
+"""Tests for terms.venery check."""
 from __future__ import absolute_import
 
 from .check import Check
 
-from proselint.checks.misc import professions as chk
+from proselint.checks.terms import venery as chk
 
 
 class TestCheck(Check):
-    """The test class for misc.professions."""
+    """The test class for terms.venery."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
-        """Basic smoke test for misc.professions."""
+        """Basic smoke test for terms.venery."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
-        assert not self.passes("""I really need a shoe repair guy.""")
+        assert not self.passes("""There was a group of alligators.""")
```

### Comparing `proselint-0.8.0/tests/test_misc_punctuation.py` & `proselint-0.9.0/tests/test_misc_punctuation.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,14 +9,14 @@
 class TestCheck(Check):
     """The test class for misc.punctuation."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
         """Basic smoke test for misc.punctuation."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
         assert not self.passes("""See Smith et. al.""")
```

### Comparing `proselint-0.8.0/tests/test_misc_scare_quotes.py` & `proselint-0.9.0/tests/test_misc_scare_quotes.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,14 @@
 class TestCheck(Check):
     """The test class for misc.scare_quotes."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
         """Basic smoke test for misc.scare_quotes."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
         assert not self.passes("""What was the 'take-home message'?""")
```

### Comparing `proselint-0.8.0/tests/test_misc_tense_present.py` & `proselint-0.9.0/tests/test_misc_tense_present.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,14 @@
 class TestCheck(Check):
     """The test class for misc.tense_present."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
         """Basic smoke test for misc.tense_present."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
         assert not self.passes("""I did it on accident honestly.""")
```

### Comparing `proselint-0.8.0/tests/test_misc_waxed.py` & `proselint-0.9.0/tests/test_misc_whence.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-"""Tests for misc.waxed check."""
+"""Tests for misc.whence check."""
 from __future__ import absolute_import
 
 from .check import Check
 
-from proselint.checks.misc import waxed as chk
+from proselint.checks.misc import whence as chk
 
 
 class TestCheck(Check):
-    """The test class for misc.waxed."""
+    """The test class for misc.whence."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
-        """Basic smoke test for misc.waxed."""
+        """Basic smoke test for misc.whence."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
-        assert not self.passes("""They really could wax poetically.""")
+        assert not self.passes("""Go back from whence you came!""")
```

### Comparing `proselint-0.8.0/tests/test_misc_whence.py` & `proselint-0.9.0/tests/test_spelling_misc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-"""Tests for misc.whence check."""
+"""Tests for spelling.misc check."""
 from __future__ import absolute_import
 
 from .check import Check
 
-from proselint.checks.misc import whence as chk
+from proselint.checks.spelling import misc as chk
 
 
 class TestCheck(Check):
-    """The test class for misc.whence."""
+    """The test class for spelling.misc."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
-        """Basic smoke test for misc.whence."""
+        """Basic smoke test for spelling.misc."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
-        assert not self.passes("""Go back from whence you came!""")
+        assert not self.passes("""I like this alot.""")
```

### Comparing `proselint-0.8.0/tests/test_mixed_metaphors.py` & `proselint-0.9.0/tests/test_mixed_metaphors.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class TestCheck(Check):
     """The test class for mixed_metaphors.misc."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke_bottleneck(self):
         """Basic smoke test for check_bottleneck."""
         assert chk.check_bottleneck(
             """Smoke phrase with nothing flagged.""") == []
         assert chk.check_bottleneck(
```

### Comparing `proselint-0.8.0/tests/test_mondegreens.py` & `proselint-0.9.0/tests/test_mondegreens.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class TestCheck(Check):
     """The test class for mondegreens.misc."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
         """Basic smoke test for mondegreens.misc."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
         assert self.passes("""... and laid him on the green.""")
         assert not self.passes("""..and Lady Mondegreen.""")
```

### Comparing `proselint-0.8.0/tests/test_needless_variants.py` & `proselint-0.9.0/tests/test_spelling_em_im_en_in.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-"""Tests for needless_variants.misc check."""
+"""Tests for spelling.em_im_en_in check."""
 from __future__ import absolute_import
 
 from .check import Check
 
-from proselint.checks.needless_variants import misc as chk
+from proselint.checks.spelling import em_im_en_in as chk
 
 
 class TestCheck(Check):
-    """The test class for needless_variants.misc."""
+    """The test class for spelling.em_im_en_in."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
-        """Basic smoke test for needless_variants.misc."""
+        """Basic smoke test for spelling.em_im_en_in."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
-        assert not self.passes("""It was an extensible telescope.""")
+        assert not self.passes("""We shall imbark on a voyage.""")
```

### Comparing `proselint-0.8.0/tests/test_nonwords.py` & `proselint-0.9.0/tests/test_nonwords.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,14 @@
 class TestCheck(Check):
     """The test class for nonwords.misc."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
         """Basic smoke test for nonwords.misc."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
         assert not self.passes("""The test was good irregardless.""")
```

### Comparing `proselint-0.8.0/tests/test_oxymorons.py` & `proselint-0.9.0/tests/test_oxymorons.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,14 @@
 class TestCheck(Check):
     """The test class for oxymorons.misc."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
         """Basic smoke test for oxymorons.misc."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
         assert not self.passes("""He needed an exact estimate.""")
```

### Comparing `proselint-0.8.0/tests/test_preferred_forms_check.py` & `proselint-0.9.0/tests/test_preferred_forms_check.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class TestCheck(Check):
     """The test class for tools.preferred_forms_check."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def setUp(self):
         """Create some test fixtures."""
         self.l = [['use', ['utilize']]]
         self.l_caps = [["Stone Age",  ["stone age"]]]
         self.err = 'error message'
```

### Comparing `proselint-0.8.0/tests/test_psychology.py` & `proselint-0.9.0/tests/test_psychology.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class TestCheck(Check):
     """The test class for psychology.misc."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke_lie_detector_test(self):
         """Basic smoke test for psychology.misc.check_lie_detector_test."""
         assert chk.check_lie_detector_test(
             """Smoke phrase with nothing flagged.""") == []
         assert chk.check_lie_detector_test(
```

### Comparing `proselint-0.8.0/tests/test_redundancy_misc.py` & `proselint-0.9.0/tests/test_redundancy_misc.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class TestCheck(Check):
     """The test class for redundancy.misc."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke_check(self):
         """Basic smoke test for redundancy.misc.check."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
         assert not self.passes("""The table was rectangular in shape.""")
```

### Comparing `proselint-0.8.0/tests/test_redundancy_ras_syndrome.py` & `proselint-0.9.0/tests/test_redundancy_ras_syndrome.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,14 @@
 class TestCheck(Check):
     """The test class for redundancy.ras_syndrome."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
         """Basic smoke test for redundancy.ras_syndrome."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
         assert not self.passes("""Please enter your PIN number.""")
```

### Comparing `proselint-0.8.0/tests/test_security_credit_card.py` & `proselint-0.9.0/tests/test_security_credit_card.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class TestCheck(Check):
     """The test class for security.credit_card."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
         """Basic smoke test for security.credit_card.
 
         This makes use of a test MasterCard number.
         """
```

### Comparing `proselint-0.8.0/tests/test_security_password.py` & `proselint-0.9.0/tests/test_jargon.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-"""Tests for security.password check."""
+"""Tests for jargon.misc check."""
 from __future__ import absolute_import
 
 from .check import Check
 
-from proselint.checks.security import password as chk
+from proselint.checks.jargon import misc as chk
 
 
 class TestCheck(Check):
-    """The test class for security.password."""
+    """The test class for jargon.misc."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
-        """Basic smoke test for security.password."""
+        """Basic smoke test for jargon.misc."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
-        assert not self.passes("""The password is 123456.""")
-        assert not self.passes("""My password is PASSWORD.""")
+        assert not self.passes("""I agree it's in the affirmative.""")
```

### Comparing `proselint-0.8.0/tests/test_skunked_terms.py` & `proselint-0.9.0/tests/test_spelling_athletes.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-"""Tests for skunked_terms.misc check."""
+"""Tests for spelling.athletes check."""
 from __future__ import absolute_import
 
 from .check import Check
 
-from proselint.checks.skunked_terms import misc as chk
+from proselint.checks.spelling import athletes as chk
 
 
 class TestCheck(Check):
-    """The test class for skunked_terms.misc."""
+    """The test class for spelling.athletes."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
-        """Basic smoke test for skunked_terms.misc."""
+        """Basic smoke test for spelling.athletes."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
-        assert not self.passes(
-            """I gave an impassionate defence of the situation.""")
+        assert not self.passes("""One of the greats: Cal Ripkin.""")
```

### Comparing `proselint-0.8.0/tests/test_spelling_able_atable.py` & `proselint-0.9.0/tests/test_spelling_able_ible.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-"""Tests for spelling.able_atable check."""
+"""Tests for spelling.able_ible check."""
 from __future__ import absolute_import
 
 from .check import Check
 
-from proselint.checks.spelling import able_atable as chk
+from proselint.checks.spelling import able_ible as chk
 
 
 class TestCheck(Check):
-    """The test class for spelling.able_atable."""
+    """The test class for spelling.able_ible."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
-        """Basic smoke test for spelling.able_atable."""
+        """Basic smoke test for spelling.able_ible."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
-        assert not self.passes("""There was a demonstratable difference.""")
+        assert not self.passes("""It was a sensable decision.""")
```

### Comparing `proselint-0.8.0/tests/test_spelling_athletes.py` & `proselint-0.9.0/tests/test_spelling_able_atable.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-"""Tests for spelling.athletes check."""
+"""Tests for spelling.able_atable check."""
 from __future__ import absolute_import
 
 from .check import Check
 
-from proselint.checks.spelling import athletes as chk
+from proselint.checks.spelling import able_atable as chk
 
 
 class TestCheck(Check):
-    """The test class for spelling.athletes."""
+    """The test class for spelling.able_atable."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
-        """Basic smoke test for spelling.athletes."""
+        """Basic smoke test for spelling.able_atable."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
-        assert not self.passes("""One of the greats: Cal Ripkin.""")
+        assert not self.passes("""There was a demonstratable difference.""")
```

### Comparing `proselint-0.8.0/tests/test_spelling_er_or.py` & `proselint-0.9.0/tests/test_spelling_er_or.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,14 @@
 class TestCheck(Check):
     """The test class for spelling.er_or."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
         """Basic smoke test for spelling.er_or."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
         assert not self.passes("""She met with the invester.""")
```

### Comparing `proselint-0.8.0/tests/test_spelling_in_un.py` & `proselint-0.9.0/tests/test_uncomparables.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-"""Tests for spelling.in_un check."""
+"""Tests for uncomparables.misc check."""
 from __future__ import absolute_import
 
 from .check import Check
 
-from proselint.checks.spelling import in_un as chk
+from proselint.checks.uncomparables import misc as chk
 
 
 class TestCheck(Check):
-    """The test class for spelling.in_un."""
+    """The test class for uncomparables.misc."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
-        """Basic smoke test for spelling.in_un."""
+        """Basic smoke test for uncomparables.misc."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
-        assert not self.passes("""The plan was unfeasible.""")
+        assert not self.passes("""The item was more unique.""")
```

### Comparing `proselint-0.8.0/tests/test_strunk_white_eos.py` & `proselint-0.9.0/tests/test_strunk_white_eos.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/tests/test_terms_animal_adjectives.py` & `proselint-0.9.0/tests/test_terms_animal_adjectives.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,14 @@
 class TestCheck(Check):
     """The test class for terms.animal_adjectives."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
         """Basic smoke test for terms.animal_adjectives."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
         assert not self.passes("""It was some bird-like creature.""")
```

### Comparing `proselint-0.8.0/tests/test_terms_denizen_labels.py` & `proselint-0.9.0/tests/test_terms_denizen_labels.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,14 @@
 class TestCheck(Check):
     """The test class for terms.denizen_labels."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
         """Basic smoke test for terms.denizen_labels."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
         assert not self.passes("""He was definitely a Hong Kongite.""")
```

### Comparing `proselint-0.8.0/tests/test_terms_eponymous_adjectives.py` & `proselint-0.9.0/tests/test_terms_eponymous_adjectives.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,14 @@
 class TestCheck(Check):
     """The test class for terms.eponymous_adjectives."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
         """Basic smoke test for terms.eponymous_adjectives."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
         assert not self.passes("""The writing wasn't Shakespearian.""")
```

### Comparing `proselint-0.8.0/tests/test_tools.py` & `proselint-0.9.0/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/tests/test_topic_detector.py` & `proselint-0.9.0/tests/test_topic_detector.py`

 * *Files identical despite different names*

### Comparing `proselint-0.8.0/tests/test_typography_diacritical_marks.py` & `proselint-0.9.0/tests/test_typography_diacritical_marks.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,14 +9,14 @@
 class TestCheck(Check):
     """The test class for typography.diacritical_marks."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
         """Basic smoke test for typography.diacritical_marks."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
         assert not self.passes("""He saw the performance by Beyonce.""")
```

### Comparing `proselint-0.8.0/tests/test_typography_exclamation.py` & `proselint-0.9.0/tests/test_typography_exclamation.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class TestCheck(Check):
     """The test class for typography.exclamation."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke_repeated_exclamations(self):
         """Basic smoke test.
 
         Test for typography.exclamation.check_repeated_exclamations.
         """
```

### Comparing `proselint-0.8.0/tests/test_typography_symbols.py` & `proselint-0.9.0/tests/test_butterick_symbols.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class TestCheck(Check):
     """The test class for typography.symbols."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_ellipsis(self):
         """Find ... in a string."""
         assert chk.check_ellipsis("""The long and winding road...""")
 
     def test_copyright(self):
```

### Comparing `proselint-0.8.0/tests/test_uncomparables.py` & `proselint-0.9.0/tests/test_weasel_words_misc.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-"""Tests for uncomparables.misc check."""
+"""Tests for weasel_words.misc check."""
 from __future__ import absolute_import
 
 from .check import Check
 
-from proselint.checks.uncomparables import misc as chk
+from proselint.checks.weasel_words import misc as chk
+from nose import SkipTest
 
 
 class TestCheck(Check):
-    """The test class for uncomparables.misc."""
+    """The test class for weasel_words.misc."""
+
+    raise SkipTest
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
-        """Basic smoke test for uncomparables.misc."""
+        """Basic smoke test for weasel_words.misc."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
-        assert not self.passes("""The item was more unique.""")
+        # FIXME add test when check is implemented
```

### Comparing `proselint-0.8.0/tests/test_weasel_words_misc.py` & `proselint-0.9.0/tests/test_weasel_words_very.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,22 @@
-"""Tests for weasel_words.misc check."""
+"""Tests for weasel_words.very check."""
 from __future__ import absolute_import
 
 from .check import Check
 
-from proselint.checks.weasel_words import misc as chk
-from nose import SkipTest
+from proselint.checks.weasel_words import very as chk
 
 
 class TestCheck(Check):
-    """The test class for weasel_words.misc."""
-
-    raise SkipTest
+    """The test class for weasel_words.very."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
-        """Basic smoke test for weasel_words.misc."""
+        """Basic smoke test for weasel_words.very."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
-        # FIXME add test when check is implemented
+        assert not self.passes("""The book was very interesting.""")
```

### Comparing `proselint-0.8.0/tests/test_weasel_words_very.py` & `proselint-0.9.0/tests/test_misc_professions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-"""Tests for weasel_words.very check."""
+"""Tests for misc.professions check."""
 from __future__ import absolute_import
 
 from .check import Check
 
-from proselint.checks.weasel_words import very as chk
+from proselint.checks.misc import professions as chk
 
 
 class TestCheck(Check):
-    """The test class for weasel_words.very."""
+    """The test class for misc.professions."""
 
     __test__ = True
 
     @property
     def this_check(self):
-        """Bolierplate."""
+        """Boilerplate."""
         return chk
 
     def test_smoke(self):
-        """Basic smoke test for weasel_words.very."""
+        """Basic smoke test for misc.professions."""
         assert self.passes("""Smoke phrase with nothing flagged.""")
-        assert not self.passes("""The book was very interesting.""")
+        assert not self.passes("""I really need a shoe repair guy.""")
```

