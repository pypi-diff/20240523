# Comparing `tmp/bbg_fetch-1.0.7.tar.gz` & `tmp/bbg_fetch-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbg_fetch-1.0.7.tar", max compression
+gzip compressed data, was "bbg_fetch-1.0.8.tar", max compression
```

## Comparing `bbg_fetch-1.0.7.tar` & `bbg_fetch-1.0.8.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     9762 2024-05-23 05:22:10.636661 bbg_fetch-1.0.7/bbg_fetch.py
--rw-r--r--   0        0        0     1491 2024-05-23 05:22:35.015670 bbg_fetch-1.0.7/pyproject.toml
--rw-r--r--   0        0        0      437 2024-04-02 20:04:59.604378 bbg_fetch-1.0.7/README.md
--rw-r--r--   0        0        0     1904 1970-01-01 00:00:00.000000 bbg_fetch-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     9852 2024-05-23 05:39:55.258978 bbg_fetch-1.0.8/bbg_fetch.py
+-rw-r--r--   0        0        0     1491 2024-05-23 05:40:16.352258 bbg_fetch-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0      437 2024-04-02 20:04:59.604378 bbg_fetch-1.0.8/README.md
+-rw-r--r--   0        0        0     1904 1970-01-01 00:00:00.000000 bbg_fetch-1.0.8/PKG-INFO
```

### Comparing `bbg_fetch-1.0.7/bbg_fetch.py` & `bbg_fetch-1.0.8/bbg_fetch.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,15 +164,16 @@
                                                     'last_tradeable_dt'),
                                  add_gen_number: bool = True
                                  ) -> pd.DataFrame:
     contracts = blp.bds(ticker, "FUT_CHAIN")
     tickers = contracts['security_description']
     df = blp.bdp(tickers=tickers, flds=flds)
     tradable_tickers = tickers[np.in1d(tickers, df.index, assume_unique=True)]
-    df = df.loc[tradable_tickers, flds]
+    good_columns = pd.Index(flds)[np.in1d(flds, df.columns, assume_unique=True)]
+    df = df.loc[tradable_tickers, good_columns]
     if add_gen_number:
         df['gen_number'] = [n+1 for n in range(len(df.index))]
     return df
 
 
 class UnitTests(Enum):
     FUNDAMENTALS = 1
```

### Comparing `bbg_fetch-1.0.7/pyproject.toml` & `bbg_fetch-1.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b74 6f6f 6c2e 706f 6574 7279 5d0d 0a6e  [tool.poetry]..n
 00000010: 616d 6520 3d20 2262 6267 5f66 6574 6368  ame = "bbg_fetch
 00000020: 220d 0a76 6572 7369 6f6e 203d 2022 312e  "..version = "1.
-00000030: 302e 3722 0d0a 6465 7363 7269 7074 696f  0.7"..descriptio
+00000030: 302e 3822 0d0a 6465 7363 7269 7074 696f  0.8"..descriptio
 00000040: 6e20 3d20 2242 6c6f 6f6d 6265 7267 2066  n = "Bloomberg f
 00000050: 6574 6368 696e 6720 616e 616c 7974 6963  etching analytic
 00000060: 7320 7772 6170 7069 6e67 2078 6262 6720  s wrapping xbbg 
 00000070: 7061 636b 6167 6522 0d0a 6c69 6365 6e73  package"..licens
 00000080: 6520 3d20 224c 4943 454e 5345 2e74 7874  e = "LICENSE.txt
 00000090: 220d 0a61 7574 686f 7273 203d 205b 2241  "..authors = ["A
 000000a0: 7274 7572 2053 6570 7020 3c61 7274 7572  rtur Sepp <artur
```

### Comparing `bbg_fetch-1.0.7/PKG-INFO` & `bbg_fetch-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbg_fetch
-Version: 1.0.7
+Version: 1.0.8
 Summary: Bloomberg fetching analytics wrapping xbbg package
 Home-page: https://github.com/ArturSepp/BloombergFetch
 License: LICENSE.txt
 Keywords: quantitative,investing,portfolio optimization,systematic strategies,volatility
 Author: Artur Sepp
 Author-email: artursepp@gmail.com
 Maintainer: Artur Sepp
```

