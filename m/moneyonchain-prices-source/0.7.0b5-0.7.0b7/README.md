# Comparing `tmp/moneyonchain_prices_source-0.7.0b5.tar.gz` & `tmp/moneyonchain_prices_source-0.7.0b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moneyonchain_prices_source-0.7.0b5.tar", last modified: Thu May 16 19:26:54 2024, max compression
+gzip compressed data, was "moneyonchain_prices_source-0.7.0b7.tar", last modified: Thu May 23 15:12:54 2024, max compression
```

## Comparing `moneyonchain_prices_source-0.7.0b5.tar` & `moneyonchain_prices_source-0.7.0b7.tar`

### file list

```diff
@@ -1,128 +1,129 @@
-drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2024-05-16 19:26:54.100992 moneyonchain_prices_source-0.7.0b5/
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4743 2024-05-16 19:26:54.100992 moneyonchain_prices_source-0.7.0b5/PKG-INFO
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     2942 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b5/README.md
-drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2024-05-16 19:26:54.045157 moneyonchain_prices_source-0.7.0b5/moc_prices_source/
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     6610 2024-04-30 17:56:23.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/__init__.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      486 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/cli.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    10728 2024-05-14 15:09:31.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/cli_check.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      625 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/coins.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     3247 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/computed_pairs.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     3892 2024-05-10 19:44:58.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/conf.py
-drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2024-05-16 19:26:54.053133 moneyonchain_prices_source-0.7.0b5/moc_prices_source/data/
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      174 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/data/database_default.json
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       17 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/data/redis_default.json
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      221 2024-05-14 13:03:36.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/data/remote_weighing_default.json
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     2427 2024-05-16 19:16:20.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/data/weighing.json
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     5715 2024-01-11 13:54:48.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/database.py
-drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2024-05-16 19:26:54.093015 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     3806 2024-04-30 20:09:02.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/__init__.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      766 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/bnb_usdt_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      720 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_ars_argenbtc.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      791 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_ars_belo_app.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      816 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_ars_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      770 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_ars_bitso.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      788 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_ars_buda.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      762 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_ars_buenbit.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      521 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_ars_coinbase.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      756 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_ars_cryptomkt.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      836 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_ars_decrypto.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      805 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_ars_lemoncash.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      805 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_ars_ripio.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      772 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_ars_ripio_exch.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      643 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_ars_rofex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      718 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_ars_satoshitango.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      770 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_cop_bitso.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      788 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_cop_buda.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      763 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_cop_buenbit.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      521 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_cop_coinbase.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      756 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_cop_cryptomkt.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      523 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_usd_bitfinex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      693 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_usd_bitgo.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      535 2024-04-30 16:19:10.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_usd_bitstamp.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_usd_bittrex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      503 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_usd_blockchain.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      518 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_usd_cex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      526 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_usd_coinbase.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      505 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_usd_gemini.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      513 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_usd_itbit.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      582 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_usd_kraken.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      559 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_usd_kucoin.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      524 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_usd_okcoin.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      859 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_usdt_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      525 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_usdt_bitfinex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_usdt_coinbase.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      581 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_usdt_kraken.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     5459 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/coins.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    13974 2024-04-30 19:24:19.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/engine_base.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      856 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/eth_btc_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      523 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/eth_btc_bitfinex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      535 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/eth_btc_bitstamp.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      505 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/eth_btc_gemini.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      580 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/eth_btc_kraken.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1616 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/gas_btc_rsk.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1484 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/moc_btc_sovryn.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      856 2023-05-12 17:54:43.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/rif_btc_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      584 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/rif_btc_bitfinex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      666 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/rif_btc_coinbene.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      636 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/rif_btc_coingecko.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      639 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/rif_btc_kucoin.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      627 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/rif_btc_mexc.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1822 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/rif_btc_mp1p_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      627 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/rif_btc_mxc.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1484 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/rif_btc_sovryn.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      859 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/rif_usdt_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      598 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/rif_usdt_ma2_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      598 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/rif_usdt_ma3_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1814 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/rif_usdt_ma_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1828 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/rif_usdt_mp1p_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      822 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_ars_ambito.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      829 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_ars_ccl_ambito.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      640 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_ars_ccl_coinmonitor.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      696 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_ars_ccl_criptoya.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1359 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_ars_ccl_cronista.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1301 2024-04-29 14:09:15.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_ars_ccl_dolarhoy.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1125 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_ars_ccl_dolarsi.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1255 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_ars_ccl_infobae.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1441 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_ars_ccl_infodolar.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      858 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_ars_ccl_lanacion.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      653 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_ars_ccl_rofex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      632 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_ars_coinmonitor.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      728 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_ars_criptoya.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1339 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_ars_cronista.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1283 2024-04-29 14:09:23.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_ars_dolarhoy.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1108 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_ars_dolarsi.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1250 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_ars_infobae.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1414 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_ars_infodolar.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      855 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_ars_lanacion.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      537 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_cop_banrep.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1494 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_cop_dolarhoy.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      921 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_mxn_bitso.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1069 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_mxn_citibanamex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1224 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_mxn_coinmonitor.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1181 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_mxn_currencymeuk.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1193 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_mxn_eldolar_info.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1235 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_mxn_eleconomista.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1344 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_mxn_infodolar.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1078 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_mxn_intercam.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1125 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_mxn_themoneyconverter.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      806 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_mxn_wise.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1223 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_mxn_xrates.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usdt_usd_bitstamp.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usdt_usd_coinbase.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      584 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usdt_usd_kraken.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      718 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/my_logging.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     6605 2024-05-10 20:45:29.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/server.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     6008 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/to_db.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)        8 2024-05-16 19:24:55.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/version.txt
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     8091 2024-05-14 15:15:23.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source/weighing.py
--rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)      117 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source_api
--rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)      118 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source_check
--rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)      128 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.7.0b5/moc_prices_source_to_db
-drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2024-05-16 19:26:54.100992 moneyonchain_prices_source-0.7.0b5/moneyonchain_prices_source.egg-info/
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4743 2024-05-16 19:26:53.000000 moneyonchain_prices_source-0.7.0b5/moneyonchain_prices_source.egg-info/PKG-INFO
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     5230 2024-05-16 19:26:53.000000 moneyonchain_prices_source-0.7.0b5/moneyonchain_prices_source.egg-info/SOURCES.txt
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)        1 2024-05-16 19:26:53.000000 moneyonchain_prices_source-0.7.0b5/moneyonchain_prices_source.egg-info/dependency_links.txt
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      146 2024-05-16 19:26:53.000000 moneyonchain_prices_source-0.7.0b5/moneyonchain_prices_source.egg-info/requires.txt
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       18 2024-05-16 19:26:53.000000 moneyonchain_prices_source-0.7.0b5/moneyonchain_prices_source.egg-info/top_level.txt
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       38 2024-05-16 19:26:54.100992 moneyonchain_prices_source-0.7.0b5/setup.cfg
--rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)     1863 2024-04-29 14:33:12.000000 moneyonchain_prices_source-0.7.0b5/setup.py
+drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2024-05-23 15:12:54.817398 moneyonchain_prices_source-0.7.0b7/
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4743 2024-05-23 15:12:54.817398 moneyonchain_prices_source-0.7.0b7/PKG-INFO
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     2942 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b7/README.md
+drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2024-05-23 15:12:54.729397 moneyonchain_prices_source-0.7.0b7/moc_prices_source/
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     7229 2024-05-23 12:32:30.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/__init__.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      486 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/cli.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    11492 2024-05-23 14:44:06.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/cli_check.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      628 2024-05-17 19:12:34.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/coins.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     3272 2024-05-22 20:08:39.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/computed_pairs.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     3892 2024-05-10 19:44:58.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/conf.py
+drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2024-05-23 15:12:54.729397 moneyonchain_prices_source-0.7.0b7/moc_prices_source/data/
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      174 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/data/database_default.json
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       17 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/data/redis_default.json
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      221 2024-05-14 13:03:36.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/data/remote_weighing_default.json
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     2428 2024-05-22 20:08:59.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/data/weighing.json
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     5865 2024-05-20 15:22:32.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/database.py
+drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2024-05-23 15:12:54.813398 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     3806 2024-04-30 20:09:02.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/__init__.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      766 2024-05-20 12:30:23.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/bnb_usdt_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      720 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_argenbtc.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      791 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_belo_app.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      869 2024-05-20 12:30:52.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      770 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_bitso.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      788 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_buda.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      762 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_buenbit.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      635 2024-05-20 12:27:49.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_coinbase.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      756 2024-05-21 15:01:04.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_cryptomkt.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      836 2024-05-21 13:16:41.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_decrypto.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      919 2024-05-20 12:32:50.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_lemoncash.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      805 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_ripio.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      772 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_ripio_exch.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      643 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_rofex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      718 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_satoshitango.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      770 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_cop_bitso.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      788 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_cop_buda.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      763 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_cop_buenbit.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      521 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_cop_coinbase.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      756 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_cop_cryptomkt.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      523 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usd_bitfinex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      693 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usd_bitgo.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      535 2024-04-30 16:19:10.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usd_bitstamp.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usd_bittrex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      503 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usd_blockchain.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      518 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usd_cex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      526 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usd_coinbase.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      505 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usd_gemini.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      513 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usd_itbit.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      582 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usd_kraken.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      559 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usd_kucoin.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      524 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usd_okcoin.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1823 2024-05-22 12:26:22.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usd_onchain.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      859 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usdt_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      525 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usdt_bitfinex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usdt_coinbase.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      581 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usdt_kraken.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     5726 2024-05-22 20:08:10.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/coins.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    13974 2024-04-30 19:24:19.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/engine_base.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      856 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/eth_btc_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      523 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/eth_btc_bitfinex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      535 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/eth_btc_bitstamp.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      505 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/eth_btc_gemini.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      580 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/eth_btc_kraken.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1616 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/gas_btc_rsk.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1484 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/moc_btc_sovryn.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      856 2023-05-12 17:54:43.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_btc_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      584 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_btc_bitfinex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      666 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_btc_coinbene.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      636 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_btc_coingecko.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      639 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_btc_kucoin.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      627 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_btc_mexc.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1822 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_btc_mp1p_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      627 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_btc_mxc.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1484 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_btc_sovryn.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      859 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_usdt_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      598 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_usdt_ma2_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      598 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_usdt_ma3_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1814 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_usdt_ma_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1828 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_usdt_mp1p_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      822 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_ambito.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      829 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_ccl_ambito.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      640 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_ccl_coinmonitor.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      696 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_ccl_criptoya.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1359 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_ccl_cronista.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1301 2024-04-29 14:09:15.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_ccl_dolarhoy.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1125 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_ccl_dolarsi.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1255 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_ccl_infobae.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1441 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_ccl_infodolar.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      858 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_ccl_lanacion.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      653 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_ccl_rofex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      632 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_coinmonitor.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      728 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_criptoya.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1339 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_cronista.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1283 2024-04-29 14:09:23.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_dolarhoy.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1108 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_dolarsi.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1250 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_infobae.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1414 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_infodolar.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      855 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_lanacion.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      537 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_cop_banrep.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1494 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_cop_dolarhoy.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      921 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_mxn_bitso.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1069 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_mxn_citibanamex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1224 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_mxn_coinmonitor.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1181 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_mxn_currencymeuk.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1193 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_mxn_eldolar_info.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1235 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_mxn_eleconomista.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1344 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_mxn_infodolar.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1078 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_mxn_intercam.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1125 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_mxn_themoneyconverter.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      806 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_mxn_wise.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1223 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_mxn_xrates.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usdt_usd_bitstamp.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usdt_usd_coinbase.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      584 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usdt_usd_kraken.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      718 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/my_logging.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     6943 2024-05-21 16:17:41.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/server.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     8576 2024-05-23 14:47:40.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/to_db.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)        8 2024-05-23 15:09:55.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/version.txt
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     8315 2024-05-23 15:02:25.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/weighing.py
+-rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)      117 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source_api
+-rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)      118 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source_check
+-rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)      128 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source_to_db
+drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2024-05-23 15:12:54.817398 moneyonchain_prices_source-0.7.0b7/moneyonchain_prices_source.egg-info/
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4743 2024-05-23 15:12:53.000000 moneyonchain_prices_source-0.7.0b7/moneyonchain_prices_source.egg-info/PKG-INFO
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     5275 2024-05-23 15:12:54.000000 moneyonchain_prices_source-0.7.0b7/moneyonchain_prices_source.egg-info/SOURCES.txt
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)        1 2024-05-23 15:12:53.000000 moneyonchain_prices_source-0.7.0b7/moneyonchain_prices_source.egg-info/dependency_links.txt
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      146 2024-05-23 15:12:53.000000 moneyonchain_prices_source-0.7.0b7/moneyonchain_prices_source.egg-info/requires.txt
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       18 2024-05-23 15:12:53.000000 moneyonchain_prices_source-0.7.0b7/moneyonchain_prices_source.egg-info/top_level.txt
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       38 2024-05-23 15:12:54.817398 moneyonchain_prices_source-0.7.0b7/setup.cfg
+-rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)     1863 2024-04-29 14:33:12.000000 moneyonchain_prices_source-0.7.0b7/setup.py
```

### Comparing `moneyonchain_prices_source-0.7.0b5/PKG-INFO` & `moneyonchain_prices_source-0.7.0b7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moneyonchain_prices_source
-Version: 0.7.0b5
+Version: 0.7.0b7
 Summary: Prices source for MoC projects
 Home-page: UNKNOWN
 Author: Juan S. Bokser
 Author-email: juan.bokser@moneyonchain.com
 License: UNKNOWN
 Description: # **MoC prices source**
         
@@ -32,15 +32,15 @@
         >>> get_price(BTC_USD)
         Decimal('29395.82')
         >>> 
         ```
         
         And that's it!
         
-        More [usage examples](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b5/docs/examples.md) can be seen [here](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b5/docs/examples.md)
+        More [usage examples](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b7/docs/examples.md) can be seen [here](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b7/docs/examples.md)
         
         
         
         ## How the included CLI tool looks like
         
         Here you can see how the output of the `moc_prices_source_check` command looks like
         
@@ -61,21 +61,21 @@
         
         Response time 1.1s
         
         user@host:~$ 
         ```
         
         This command has many options. you can run `moc_prices_source_check --help` to get help on how to run them.
-        More information about this CLI tool can be seen [here](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b5/docs/cli.md).
+        More information about this CLI tool can be seen [here](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b7/docs/cli.md).
         
         
         
         ## References
         
-        * [Source code in Github](https://github.com/money-on-chain/moc_prices_source/tree/v0.7.0b5)
+        * [Source code in Github](https://github.com/money-on-chain/moc_prices_source/tree/v0.7.0b7)
         * [Package from Python package index (PyPI)](https://pypi.org/project/moneyonchain-prices-source)
         
         
         
         ## Requirements
         
         * Python 3.6+ support
@@ -98,15 +98,15 @@
         $ moc_prices_source_check --version
         ```
         
         To verify that it has been installed correctly
         
         ### From source
         
-        Download from [Github](https://github.com/money-on-chain/moc_prices_source/tree/v0.7.0b5)
+        Download from [Github](https://github.com/money-on-chain/moc_prices_source/tree/v0.7.0b7)
         
         Standing inside the folder, run:
         
         ```shell
         $ pip3 install -r requirements.txt 
         ```
         
@@ -124,15 +124,15 @@
         
         To verify that it has been installed correctly
         
         
         
         ## Supported coinpairs and symbols
         
-        [Here](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b5/docs/supported_coinpairs.md) you can find an [summary of supported coinpairs and symbols](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b5/docs/supported_coinpairs.md)
+        [Here](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b7/docs/supported_coinpairs.md) you can find an [summary of supported coinpairs and symbols](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b7/docs/supported_coinpairs.md)
         
         
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
```

### Comparing `moneyonchain_prices_source-0.7.0b5/README.md` & `moneyonchain_prices_source-0.7.0b7/README.md`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/__init__.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 base_dir = dirname(abspath(__file__))
 
 with open(base_dir + "/version.txt", "r") as file_:
     version = file_.read().split()[0]
 __version__ = version
 
 bkpath   = sys.path[:]
-sys.path.append(dirname(base_dir))
+sys.path.insert(0, dirname(base_dir))
 
 from moc_prices_source.engines        import get_coinpair_list, get_engines_names, get_prices, session_storage
 from moc_prices_source.computed_pairs import computed_pairs
 from moc_prices_source.weighing       import weighing, weighted_median, median, mean
 from moc_prices_source.coins          import *
 
 sys.path = bkpath
@@ -87,44 +87,58 @@
             coinpair_prices[value['coinpair']]['sum_weighing'] += value['weighing']
 
     for d in coinpair_prices.values():
         sum_weighing = d['sum_weighing']
         for v in d['data']:
             weighing = v['weighing']
             if not weighing:
-                percentual_weighing = 0
+                percentual_weighing = Decimal('0.0')
             elif not sum_weighing:
-                percentual_weighing = 0
+                percentual_weighing = Decimal('0.0')
             else:
                 percentual_weighing = weighing / sum_weighing
             v['percentual_weighing'] = percentual_weighing
 
-    for d in coinpair_prices.values():
+    for k, d in coinpair_prices.items():
         if not 'weighings' in d:
             d['weighings'] = []
         if not 'prices' in d:
             d['prices'] = []
         for v in d['data']:
             d['weighings'].append(v['percentual_weighing'])
             d['prices'].append(v['price'])
         del d['data']
         del d['sum_weighing']
+
+        ok_sources_count = len(list(filter(bool, d['weighings'])))
+        min_ok_sources_count = k.min_ok_sources_count
+
+        d['ok_sources_count'] = ok_sources_count
+        d['min_ok_sources_count'] = min_ok_sources_count
+        d['ok'] = True
+        d['error'] = ''
+
+        if ok_sources_count < min_ok_sources_count:
+            d['ok'] = False
+            d['error'] = f"Not enough price sources ({ok_sources_count} < {min_ok_sources_count})"
+
         d['median_price'] = median(d['prices'])
         d['mean_price'] = mean(d['prices'])
         if any (d['weighings']):
             d['weighted_median_price'] = weighted_median(d['prices'], d['weighings'])
         else:
             d['weighted_median_price'] = None
 
     if requested:
         for r in [r for r in requested if (
             (r in computed_pairs) and (not r in coinpair_prices)) ]:
             requirements = computed_pairs[r]['requirements']
             if set(requirements).issubset(set(coinpair_prices.keys())):
                 coinpair_prices[r] = {}
+                coinpair_prices[r]['ok'] = all([ coinpair_prices[q]['ok'] for q in requirements ])
                 coinpair_prices[r]['requirements'] = requirements
                 formula = computed_pairs[r]['formula']
                 for k in ['median_price', 'mean_price', 'weighted_median_price']:
                     args = [ coinpair_prices[q][k] for q in requirements ]
                     try:
                         coinpair_prices[r][k] = formula(*args)
                     except:
@@ -133,18 +147,18 @@
     detail['values'] = coinpair_prices
 
     out = {}
 
     for key, value in coinpair_prices.items():
         if requested:
             if key in requested:
-                if value['weighted_median_price']:
+                if value['weighted_median_price'] and value['ok']:
                     out[key] = value['weighted_median_price']
         else:
-            if value['weighted_median_price']:
+            if value['weighted_median_price'] and value['ok']:
                 out[key] = value['weighted_median_price']
 
     if requested and len(requested)==1:
         if requested[0] in out:
             out = out[requested[0]]
         else:
             out = None
```

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/cli_check.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/cli_check.py`

 * *Files 4% similar despite different names*

```diff
@@ -114,30 +114,34 @@
 
     title = "Coinpairs"
     str_source = {
         'direct': 'Weighted',
         'computed': 'Computed'
     }
     table = [[str(pair), pair.from_.symbol+'/'+pair.to_.symbol, pair.variant,
-              str_source[data['type']]] for pair, data in summary_data.items()]
+             str_source[data['type']]] for pair, data in summary_data.items()]
     table.sort()
     headers=['Name', 'Coinpair', 'Variant', 'Method']
     print()
     show_title(title)
     print()
     show_table(table, headers)
     print()
     table = [
         ['Weighted', 'Weighted median of values ​​obtained from multiple sources'],
         ['Computed', 'Compute made with previously obtained coinpairs']
     ]
     headers=['Method', 'Description']
     show_table(table, headers)
     print()
-    
+    table = [[str(pair), pair.description] for pair, data in summary_data.items()]
+    table.sort()
+    headers=['Name', 'Comment/Description']
+    show_table(table, headers)
+    print()    
 
 
     title="Formulas used in the computed coinpairs"
     table=[[str(pair), '=', data['formula_desc']] for pair, data in
            summary_data.items() if data['type']=='computed']
     table.sort()
     print()
@@ -190,23 +194,26 @@
         help='Show the default weighing and exit.')
 @option('-c', '--computed', 'show_computed_pairs', is_flag=True,
         help='Show the computed pairs formula and exit.')
 @option('-s', '--summary', 'show_summary', is_flag=True,
         help='Show the summary and exit.')
 @option('-m', '--markdown', 'md_summary', is_flag=True,
         help='Set markdown for the summary format.')
+@option('-z', '--ignore-zero-weighing', 'ignore_zero_weighing', is_flag=True,
+        help='Ignore sources with zero weighing.')
 @cli.argument('coinpairs_filter', required=False)
 def cli_check(
         show_version=False,
         show_json=False,
         show_weighing=False,
         show_computed_pairs=False,
         coinpairs_filter=None,
         show_summary=False,
-        md_summary=False
+        md_summary=False,
+        ignore_zero_weighing=False
     ):
     """\b
 Description:
     CLI-type tool that shows the data obtained by
     the `moc_price_source` library.   
     Useful for troubleshooting.
 \n\b
@@ -253,15 +260,19 @@
     
     if show_summary:
         summary(coinpairs, md_summary)
         return
 
     data = {}
 
-    get_price(coinpairs, detail=data, serializable=show_json)
+    get_price(
+        coinpairs,
+        ignore_zero_weighing=ignore_zero_weighing,
+        detail=data,
+        serializable=show_json)
 
     if show_json:
         print(json.dumps(data, indent=4, sort_keys=True))
         return
 
     def format_time(t):
         return '{}s'.format(round(t.seconds + t.microseconds/1000000, 2))
@@ -314,29 +325,36 @@
         else:
             row.append('ƒ')
         row.append(coinpair)
         row.append(d['median_price'])
         row.append(d['mean_price'])
         row.append(d['weighted_median_price'])
         if 'prices' in d:
-            row.append(len(d['prices']))
+            if 'ok_sources_count' in d:
+                row.append(f"{d['ok_sources_count']} of {len(d['prices'])}")
+            else:
+                row.append(len(d['prices']))
         else:
             row.append('N/A')
+        row.append('✓' if d['ok'] else '✕')
         table.append(row)
     if table:
         table.sort(key=lambda x: str(x[1]))
         print()
         print(tabulate(table, headers=[
-            '', 'Coin pair', 'Mediam', 'Mean', 'Weighted median', 'Sources'
+            '', 'Coin pair', 'Mediam', 'Mean', 'Weighted median', 'Sources', 'Ok'
         ]))
 
     errors = []
     for p in prices:
         if not p["ok"] and p['weighing']:
-            errors.append((p["name"], p["error"]))
+            errors.append((f"Source {p['name']}", p["error"]))
+    for k, v in values.items():
+        if 'error' in v and v["error"]:
+            errors.append((f"Coinpair {k}", v["error"]))    
 
     if errors:
         print()
         print("Errors detail")
         print("------ ------")
         for e in errors:
             print()
```

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/coins.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/coins.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 from os.path  import dirname, abspath
 
 bkpath   = sys.path[:]
 base_dir = dirname(abspath(__file__))
-sys.path.append(dirname(base_dir))
+sys.path.insert(0, dirname(base_dir))
 
 from moc_prices_source.engines.coins import *
 
 sys.path = bkpath
 
 
 if __name__ == '__main__':
```

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/computed_pairs.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/computed_pairs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import sys
 from os.path import dirname, abspath
 from inspect import getsource
-from types   import LambdaType
+from types import LambdaType
+from decimal import Decimal
 
 base_dir = dirname(abspath(__file__))
 
 bkpath   = sys.path[:]
 sys.path.insert(0, dirname(base_dir), )
 
 from moc_prices_source.engines.coins import \
@@ -61,15 +62,15 @@
     USD_ARS_CCB: {
         'requirements': [BTC_ARS, BTC_USD],
         'formula': lambda btc_ars, btc_usd: btc_ars / btc_usd
     },
     USD_COP_CCB: {
         'requirements': [BTC_COP, BTC_USD],
         'formula': lambda btc_cop, btc_usd: btc_cop / btc_usd
-    },
+    }
 }
 
 for pair, data in computed_pairs.items():
     formula = data['formula']
     if isinstance(formula, LambdaType):
         formula_desc = ':'.join(getsource(formula).split('lambda')[-1].strip(
             ).split(':')[1:]).strip()
```

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/conf.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/conf.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/data/weighing.json` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/data/weighing.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -1,21 +1,21 @@
 {
     "btc_ars_argenbtc": 0.142,
-    "btc_ars_buenbit": 0.142,
-    "btc_ars_decrypto": 0.142,
     "btc_ars_belo_app": 0.142,
-    "btc_ars_bitso": 0,
-    "btc_ars_cryptomkt": 0.142,
-    "btc_ars_satoshitango": 0,
     "btc_ars_binance": 0.142,
+    "btc_ars_buenbit": 0.142,
+    "btc_ars_cryptomkt": 0.142,
+    "btc_ars_decrypto": 0.142,
     "btc_ars_lemoncash": 0.142,
+    "btc_ars_bitso": 0,
+    "btc_ars_buda": 0,
     "btc_ars_coinbase": 0,
     "btc_ars_ripio": 0,
-    "btc_ars_buda": 0,
     "btc_ars_ripio_exch": 0,
+    "btc_ars_satoshitango": 0,
     "btc_usd_coinbase": 0.25,
     "btc_usd_bitstamp": 0.22,
     "btc_usd_bitfinex": 0.18,
     "btc_usd_kraken": 0.18,
     "btc_usd_gemini": 0.17,
     "rif_btc_binance": 1,
     "rif_btc_sovryn": 0,
```

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/database.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,29 @@
-import datetime, json, sys
-from sys             import stderr
-from influxdb        import InfluxDBClient
-from os.path         import dirname, abspath
+import datetime, sys
+from influxdb import InfluxDBClient
+from os.path import dirname, abspath
 
 bkpath   = sys.path[:]
 base_dir = dirname(abspath(__file__))
-sys.path.append(dirname(base_dir))
+sys.path.insert(0, dirname(base_dir))
 
 from moc_prices_source.conf import get
 
 sys.path = bkpath
 
 
+to_gmt = int(round(float((datetime.datetime.utcnow() -
+                          datetime.datetime.now()).seconds)/3600))
+if to_gmt==24:
+    to_gmt=0
+
+
 db_conf = None
-envs    = {}
+envs = {}
+config_file = None
 
 
 def call_back(options):
 
     selected_profile = options['selected_profile']
 
     return {
@@ -53,15 +59,15 @@
         self.client.switch_database(self.name)
 
 
     @staticmethod
     def _validate_time(time_):
         if time_ is None:
             time_ = datetime.datetime.utcnow()
-        return time_
+        return time_ + datetime.timedelta(hours=to_gmt)
 
 
     def write(self, measurement, fields, tags={}, time_ = None):
 
         time_ = self._validate_time(time_)
 
         item = {}
```

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/__init__.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/bnb_usdt_binance.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/bnb_usdt_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_ars_argenbtc.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_argenbtc.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_ars_belo_app.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_belo_app.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_ars_binance.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_binance.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 class Engine(BaseWithFailover):
 
     _name         = BaseWithFailover._name_from_file(__file__)
     _description  = "Binance"
     _uri          = base_uri.format("api.binance.com")
     _uri_failover = base_uri.format("moc-proxy-api-binance.moneyonchain.com")
     _coinpair     = BTC_ARS
-    _max_time_without_price_change = 0 # zero means infinity
+
+    _max_age                       = 3600 # 1hs.
+    _max_time_without_price_change = 0    # zero means infinity
 
     def _map(self, data):
         return {
             'price':  data['lastPrice'],
             'volume': data['volume']}
```

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_ars_bitso.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_bitso.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_ars_buda.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_buda.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_ars_buenbit.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_buenbit.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_ars_coinbase.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usd_coinbase.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from engine_base import Base, BTC_ARS
+from engine_base import Base, BTC_USD
 
 
 class Engine(Base):
 
     _name        = Base._name_from_file(__file__)
     _description = "Coinbase"
-    _uri         = "https://api.coinbase.com/v2/prices/BTC-ARS/spot"
-    _coinpair    = BTC_ARS
+    _uri         = "https://api.coinbase.com/v2/prices/spot?currency=USD"
+    _coinpair    = BTC_USD
 
     def _map(self, data):
         return {
             'price':  data['data']['amount']
             }
```

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_ars_cryptomkt.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_cryptomkt.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_ars_decrypto.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_decrypto.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_ars_lemoncash.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usdt_kraken.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,21 @@
-from engine_base import Base, BTC_ARS
-from decimal import Decimal
+from engine_base import Base, BTC_USDT
 
 
 class Engine(Base):
 
     _name        = Base._name_from_file(__file__)
-    _description = "Lemoncash"
-    _uri         = "https://api.lemoncash.com.ar/api/v1/exchange-rates-quotations-external"
-    _coinpair    = BTC_ARS
+    _description = "Kraken"
+    _uri         = "https://api.kraken.com/0/public/Ticker?pair=XBTUSDT"
+    _coinpair    = BTC_USDT
 
     def _map(self, data):
-        value = {}
-        for i in data['results']:
-            if i['instrument']=='BTC-ARS':
-                value['price'] = (Decimal(i['purchase_price']['amount']) \
-                                  + Decimal(i['sale_price']['amount'])) / Decimal('2')
-                break       
-        return value
+        return {
+            'price':  data['result']['XBTUSDT']['c'][0],
+            'volume': data['result']['XBTUSDT']['v'][1] }
 
 
 if __name__ == '__main__':
     print("File: {}, Ok!".format(repr(__file__)))
     engine = Engine()
     engine()
     print(engine)
```

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_ars_ripio.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_ripio.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_ars_ripio_exch.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_ripio_exch.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_ars_rofex.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_rofex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_ars_satoshitango.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_satoshitango.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_cop_bitso.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_cop_bitso.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_cop_buda.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_cop_buda.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_cop_buenbit.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_cop_buenbit.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_cop_coinbase.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_cop_coinbase.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_cop_cryptomkt.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_cop_cryptomkt.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_usd_bitfinex.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usd_bitfinex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_usd_bitgo.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usd_bitgo.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_usd_bitstamp.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usd_bitstamp.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_usd_bittrex.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usd_bittrex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_usd_cex.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usd_cex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_usd_coinbase.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usdt_coinbase.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from engine_base import Base, BTC_USD
+from engine_base import Base, BTC_USDT
 
 
 class Engine(Base):
 
     _name        = Base._name_from_file(__file__)
     _description = "Coinbase"
-    _uri         = "https://api.coinbase.com/v2/prices/spot?currency=USD"
-    _coinpair    = BTC_USD
+    _uri         = "https://api.coinbase.com/v2/exchange-rates?currency=BTC"
+    _coinpair    = BTC_USDT
 
     def _map(self, data):
         return {
-            'price':  data['data']['amount']
+            'price':  data['data']['rates']['USDT']
             }
 
 
 if __name__ == '__main__':
     print("File: {}, Ok!".format(repr(__file__)))
     engine = Engine()
     engine()
```

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_usd_itbit.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usd_itbit.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_usd_kraken.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usd_kraken.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_usd_kucoin.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usd_kucoin.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_usd_okcoin.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usd_okcoin.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_usdt_binance.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usdt_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_usdt_bitfinex.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usdt_bitfinex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_usdt_coinbase.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usdt_usd_coinbase.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from engine_base import Base, BTC_USDT
+from engine_base import Base, USDT_USD
 
 
 class Engine(Base):
 
     _name        = Base._name_from_file(__file__)
     _description = "Coinbase"
-    _uri         = "https://api.coinbase.com/v2/exchange-rates?currency=BTC"
-    _coinpair    = BTC_USDT
+    _uri         = "https://api.coinbase.com/v2/exchange-rates?currency=USDT"
+    _coinpair    = USDT_USD
 
     def _map(self, data):
         return {
-            'price':  data['data']['rates']['USDT']
+            'price':  data['data']['rates']['USD']
             }
 
 
 if __name__ == '__main__':
     print("File: {}, Ok!".format(repr(__file__)))
     engine = Engine()
     engine()
```

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/btc_usdt_kraken.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usdt_usd_kraken.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from engine_base import Base, BTC_USDT
+from engine_base import Base, USDT_USD
 
 
 class Engine(Base):
 
     _name        = Base._name_from_file(__file__)
     _description = "Kraken"
-    _uri         = "https://api.kraken.com/0/public/Ticker?pair=XBTUSDT"
-    _coinpair    = BTC_USDT
+    _uri         = "https://api.kraken.com/0/public/Ticker?pair=USDTZUSD"
+    _coinpair    = USDT_USD
 
     def _map(self, data):
         return {
-            'price':  data['result']['XBTUSDT']['c'][0],
-            'volume': data['result']['XBTUSDT']['v'][1] }
+            'price':  data['result']['USDTZUSD']['c'][0],
+            'volume': data['result']['USDTZUSD']['v'][1] }
 
 
 if __name__ == '__main__':
     print("File: {}, Ok!".format(repr(__file__)))
     engine = Engine()
     engine()
     print(engine)
```

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/coins.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/coins.py`

 * *Files 26% similar despite different names*

```diff
@@ -44,25 +44,25 @@
     def __lt__(self, other):
         return str(self).lower()<str(other).strip().lower()
 
     def __hash__(self):
         return hash(str(self))
 
 
-BTC  = Coin('Bitcoin',        'btc',  '₿')
-USD  = Coin('Dollar',         'usd',  '$')
-RIF  = Coin('RIF Token',      'rif')
-MOC  = Coin('MOC Token',      'moc')
-ETH  = Coin('Ether',          'eth',  '⟠')
-USDT = Coin('Tether',         'usdt', '₮')
-BNB  = Coin('Binance Coin',   'bnb',  'Ƀ')
-ARS  = Coin('Peso Argentino', 'ars',  '$')
-MXN  = Coin('Peso Mexicano',  'mxn',  '$')
-COP  = Coin('Peso Colombiano','cop',  '$')
-GAS  = Coin('Gas',            'gas')
+BTC  = Coin('Bitcoin', 'btc', '₿')
+USD  = Coin('Dollar', 'usd', '$')
+RIF  = Coin('RIF Token', 'rif')
+MOC  = Coin('MOC Token', 'moc')
+ETH  = Coin('Ether', 'eth', '⟠')
+USDT = Coin('Tether', 'usdt', '₮')
+BNB  = Coin('Binance Coin', 'bnb', 'Ƀ')
+ARS  = Coin('Peso Argentino', 'ars', '$')
+MXN  = Coin('Peso Mexicano', 'mxn', '$')
+COP  = Coin('Peso Colombiano','cop', '$')
+GAS  = Coin('Gas', 'gas')
 
 
 Coins = [ c for c in locals().values() if isinstance(c, Coin) ]
 
 
 
 def get_coin(value):
@@ -72,20 +72,32 @@
     except KeyError:
         return dict([ (str(c).strip().lower(), c) for c in Coins])[value]
         
 
 
 class CoinPair(object):
 
-    def __init__(self, from_: Coin, to_: Coin, variant=None):
-        self._from    = from_
-        self._to      = to_
+    def __init__(self,
+                 from_: Coin, to_: Coin, variant=None, description=None,
+                 min_ok_sources_count = 0):
+        self._from = from_
+        self._to = to_
         self._variant = str(variant) if variant else None
+        self._description = str(description) if description else None
+        self._min_ok_sources_count = int(min_ok_sources_count) if min_ok_sources_count else 0
 
     @property
+    def min_ok_sources_count(self):
+        return self._min_ok_sources_count
+    
+    @property
+    def description(self):
+        return self._description
+    
+    @property
     def variant(self):
         return self._variant
 
     @property
     def from_(self):
         return self._from
 
@@ -119,45 +131,46 @@
     def __lt__(self, other):
         return str(self).lower()<str(other).strip().lower()
 
     def __hash__(self):
         return hash(str(self))
 
 
-BTC_USD         = CoinPair(BTC,  USD)
-BTC_ARS         = CoinPair(BTC,  ARS)
-BTC_COP         = CoinPair(BTC,  COP)
-RIF_BTC         = CoinPair(RIF,  BTC)
-RIF_BTC_MP1P    = CoinPair(RIF,  BTC, "mp1%") # To move the price 1 percent
-RIF_USD         = CoinPair(RIF,  USD) # Leave this as legacy
-RIF_USD_B       = CoinPair(RIF,  USD, "B") # Passing through Bitcoin
-RIF_USD_T       = CoinPair(RIF,  USD, "T") # Passing through Tether
-RIF_USD_TB      = CoinPair(RIF,  USD, "TB") # Passing through Tether & Bitcoin
-RIF_USD_WMTB    = CoinPair(RIF,  USD, "WMTB") # Passing through Tether & Bitcoin usinng weighted_median
-RIF_USDT        = CoinPair(RIF,  USDT)
-RIF_USDT_MA     = CoinPair(RIF,  USDT, "MA") # Using the magic average algorithm with orderbook depth
-RIF_USDT_MA2    = CoinPair(RIF,  USDT, "MA2")
-RIF_USDT_MA3    = CoinPair(RIF,  USDT, "MA3")
-RIF_USDT_MP1P   = CoinPair(RIF,  USDT, "mp1%") # To move the price 1 percent
-MOC_BTC         = CoinPair(MOC,  BTC)
-MOC_USD         = CoinPair(MOC,  USD)
-ETH_BTC         = CoinPair(ETH,  BTC)
-ETH_USD         = CoinPair(ETH,  USD)
-BTC_USDT        = CoinPair(BTC,  USDT)
-USDT_USD        = CoinPair(USDT, USD)
-USDT_USD_B      = CoinPair(USDT, USD, "B") # Passing through Bitcoin
-BNB_USDT        = CoinPair(BNB,  USDT)
-BNB_USD         = CoinPair(BNB,  USD)
-USD_ARS         = CoinPair(USD,  ARS)
-USD_ARS_CCL     = CoinPair(USD,  ARS, "CCL")
-USD_ARS_CCB     = CoinPair(USD,  ARS, "CCB")
-USD_MXN         = CoinPair(USD,  MXN)
-USD_COP         = CoinPair(USD,  COP)
-USD_COP_CCB     = CoinPair(USD,  COP, "CCB")
-GAS_BTC         = CoinPair(GAS,  BTC)
+BTC_USD = CoinPair(BTC, USD)
+BTC_USD_OCH = CoinPair(BTC, USD, "och", "Obtained from the blockchain")
+BTC_ARS = CoinPair(BTC, ARS, min_ok_sources_count=3)
+BTC_COP = CoinPair(BTC, COP, min_ok_sources_count=2)
+RIF_BTC = CoinPair(RIF, BTC)
+RIF_BTC_MP1P = CoinPair(RIF, BTC, "mp1%", "To move the price 1 percent")
+RIF_USD = CoinPair(RIF, USD, description="Leave this as legacy")
+RIF_USD_B = CoinPair(RIF, USD, "B", "Passing through Bitcoin")
+RIF_USD_T = CoinPair(RIF, USD, "T", "Passing through Tether")
+RIF_USD_TB = CoinPair(RIF, USD, "TB", "Passing through Tether & Bitcoin")
+RIF_USD_WMTB = CoinPair(RIF, USD, "WMTB", "Passing through Tether & Bitcoin usinng weighted_median")
+RIF_USDT = CoinPair(RIF, USDT)
+RIF_USDT_MA = CoinPair(RIF, USDT, "MA", "Using the magic average algorithm with orderbook depth")
+RIF_USDT_MA2 = CoinPair(RIF, USDT, "MA2")
+RIF_USDT_MA3 = CoinPair(RIF, USDT, "MA3")
+RIF_USDT_MP1P = CoinPair(RIF, USDT, "mp1%", "To move the price 1 percent")
+MOC_BTC = CoinPair(MOC, BTC)
+MOC_USD = CoinPair(MOC, USD)
+ETH_BTC = CoinPair(ETH, BTC)
+ETH_USD = CoinPair(ETH, USD)
+BTC_USDT = CoinPair(BTC, USDT)
+USDT_USD = CoinPair(USDT, USD)
+USDT_USD_B = CoinPair(USDT, USD, "B", "Passing through Bitcoin")
+BNB_USDT = CoinPair(BNB, USDT)
+BNB_USD = CoinPair(BNB, USD)
+USD_ARS = CoinPair(USD, ARS)
+USD_ARS_CCL = CoinPair(USD, ARS, "CCL")
+USD_ARS_CCB = CoinPair(USD, ARS, "CCB")
+USD_MXN = CoinPair(USD, MXN)
+USD_COP = CoinPair(USD, COP)
+USD_COP_CCB = CoinPair(USD, COP, "CCB")
+GAS_BTC = CoinPair(GAS, BTC)
 
 
 CoinPairs = [ c for c in locals().values() if isinstance(c, CoinPair) ]
 
 
 
 def get_coin_pair(value):
```

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/engine_base.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/engine_base.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/eth_btc_binance.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/eth_btc_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/eth_btc_bitfinex.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/eth_btc_bitfinex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/eth_btc_bitstamp.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/eth_btc_bitstamp.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/eth_btc_kraken.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/eth_btc_kraken.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/gas_btc_rsk.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/gas_btc_rsk.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/moc_btc_sovryn.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/moc_btc_sovryn.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/rif_btc_binance.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_btc_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/rif_btc_bitfinex.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_btc_bitfinex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/rif_btc_coinbene.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_btc_coinbene.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/rif_btc_coingecko.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_btc_coingecko.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/rif_btc_kucoin.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_btc_kucoin.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/rif_btc_mexc.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_btc_mexc.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/rif_btc_mp1p_binance.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_btc_mp1p_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/rif_btc_mxc.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_btc_mxc.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/rif_btc_sovryn.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_btc_sovryn.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/rif_usdt_binance.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_usdt_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/rif_usdt_ma2_binance.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_usdt_ma2_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/rif_usdt_ma3_binance.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_usdt_ma3_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/rif_usdt_ma_binance.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_usdt_ma_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/rif_usdt_mp1p_binance.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_usdt_mp1p_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_ars_ambito.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_ambito.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_ars_ccl_ambito.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_ccl_ambito.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_ars_ccl_coinmonitor.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_ccl_coinmonitor.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_ars_ccl_criptoya.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_ccl_criptoya.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_ars_ccl_cronista.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_ccl_cronista.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_ars_ccl_dolarhoy.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_ccl_dolarhoy.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_ars_ccl_dolarsi.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_ccl_dolarsi.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_ars_ccl_infobae.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_ccl_infobae.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_ars_ccl_infodolar.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_ccl_infodolar.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_ars_ccl_lanacion.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_ccl_lanacion.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_ars_ccl_rofex.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_ccl_rofex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_ars_coinmonitor.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_coinmonitor.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_ars_criptoya.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_criptoya.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_ars_cronista.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_cronista.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_ars_dolarhoy.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_dolarhoy.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_ars_dolarsi.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_dolarsi.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_ars_infobae.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_infobae.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_ars_infodolar.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_infodolar.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_ars_lanacion.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_lanacion.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_cop_banrep.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_cop_banrep.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_cop_dolarhoy.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_cop_dolarhoy.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_mxn_bitso.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_mxn_bitso.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_mxn_citibanamex.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_mxn_citibanamex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_mxn_coinmonitor.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_mxn_coinmonitor.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_mxn_currencymeuk.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_mxn_currencymeuk.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_mxn_eldolar_info.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_mxn_eldolar_info.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_mxn_eleconomista.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_mxn_eleconomista.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_mxn_infodolar.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_mxn_infodolar.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_mxn_intercam.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_mxn_intercam.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_mxn_themoneyconverter.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_mxn_themoneyconverter.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_mxn_wise.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_mxn_wise.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usd_mxn_xrates.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_mxn_xrates.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usdt_usd_bitstamp.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usdt_usd_bitstamp.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/engines/usdt_usd_coinbase.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_coinbase.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,23 @@
-from engine_base import Base, USDT_USD
+from engine_base import Base, BTC_ARS
 
 
 class Engine(Base):
 
     _name        = Base._name_from_file(__file__)
     _description = "Coinbase"
-    _uri         = "https://api.coinbase.com/v2/exchange-rates?currency=USDT"
-    _coinpair    = USDT_USD
+    _uri         = "https://api.coinbase.com/v2/prices/BTC-ARS/spot"
+    _coinpair    = BTC_ARS
+
+    _max_age                       = 3600 # 1hs.
+    _max_time_without_price_change = 0    # zero means infinity
 
     def _map(self, data):
         return {
-            'price':  data['data']['rates']['USD']
+            'price':  data['data']['amount']
             }
 
 
 if __name__ == '__main__':
     print("File: {}, Ok!".format(repr(__file__)))
     engine = Engine()
     engine()
```

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/my_logging.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/my_logging.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/server.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/server.py`

 * *Files 13% similar despite different names*

```diff
@@ -184,24 +184,32 @@
             value = float(value)
 
         sources_count = {}
         sources_count_ok = {}
         for p in detail.get('prices', []):
             sub_coinpair = p.get('coinpair', 'unknown')
             sources_count[sub_coinpair] = sources_count.get(sub_coinpair, 0) + 1
-            if  p.get('ok'):
+            if p.get('ok'):
                 sources_count_ok[sub_coinpair] = sources_count_ok.get(sub_coinpair, 0) + 1
             else:
                 source = p.get('description', 'unknown')
                 error = p.get('error', 'unknown')
                 if coinpair==sub_coinpair:
                     app.logger.warning(f"{coinpair} --> {source} {error}")
                 else:
                     app.logger.warning(f"{sub_coinpair} for {coinpair} --> {source} {error}")
 
+        for sub_coinpair, p in detail.get('values', {}).items():
+            error = p.get('error')
+            if error:
+                if coinpair==sub_coinpair:
+                    app.logger.warning(f"{coinpair} --> {error}")
+                else:
+                    app.logger.warning(f"{sub_coinpair} for {coinpair} --> {error}")
+
         if sources_count:
             sources_count_str = ', '.join([ f"{k}: {sources_count_ok[k]} of {v}" for (k, v) in sources_count.items()])
             if len(sources_count)>1:
                 app.logger.info(f"Sources count for {coinpair}: {sources_count_str}")
             else:
                 app.logger.info(f"Sources count for {sources_count_str}")
```

### Comparing `moneyonchain_prices_source-0.7.0b5/moc_prices_source/weighing.py` & `moneyonchain_prices_source-0.7.0b7/moc_prices_source/weighing.py`

 * *Files 6% similar despite different names*

```diff
@@ -197,15 +197,20 @@
 
 
 weighing = Weighing()
 
 
 
 def weighted_median(values, weights):
-    
+
+    if not all(weights):
+        non_zero = [(v, w) for (v, w) in zip(values, weights) if w]
+        values = [v for (v, w) in non_zero]
+        weights = [w for (v, w) in non_zero]
+   
     count = len(values)
     
     if 1==count:
         return values[0]
     
     idx = weighted_median_idx(values, weights)
 
@@ -224,24 +229,35 @@
     if isinstance(b, Decimal) and not isinstance(q, Decimal):
         q = Decimal(q)      
     
     return (a * p) + (b * q)
 
 
 def weighted_median_idx(values, weights):
-    ''' compute the weighted median of values list. The weighted median is computed as follows:
+    '''
+    Compute the weighted median of values list.
+    The weighted median is computed as follows:
+
     1- sort both lists (values and weights) based on values.
-    2- select the 0.5 point from the weights and return the corresponding values as results
-    e.g. values = [1, 3, 0] and weights=[0.1, 0.3, 0.6] assuming weights are probabilities.
-    sorted values = [0, 1, 3] and corresponding sorted weights = [0.6,     0.1, 0.3] the 0.5 point on
-    weight corresponds to the first item which is 0. so the weighted     median is 0.'''
+    
+    2- select the 0.5 point from the weights and return the corresponding
+       values as results.
+    
+    e.g. values = [1, 3, 0] and weights=[0.1, 0.3, 0.6] assuming weights
+    are probabilities.
+    
+    sorted values = [0, 1, 3] and corresponding sorted weights = [0.6, 0.1,
+    0.3] the 0.5 point on weight corresponds to the first item which is 0.
+    so the weighted median is 0.
+    '''
 
     # convert the weights into probabilities
     sum_weights = sum(weights)
     weights = [w / sum_weights for w in weights]
+    
     # sort values and weights based on values
     sorted_tuples = sorted(zip(values, weights, range(len(values))))
 
     # select the median point
     cumulative_probability = 0
     for i in range(len(sorted_tuples)):
         cumulative_probability += sorted_tuples[i][1]
```

### Comparing `moneyonchain_prices_source-0.7.0b5/moneyonchain_prices_source.egg-info/PKG-INFO` & `moneyonchain_prices_source-0.7.0b7/moneyonchain_prices_source.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moneyonchain-prices-source
-Version: 0.7.0b5
+Version: 0.7.0b7
 Summary: Prices source for MoC projects
 Home-page: UNKNOWN
 Author: Juan S. Bokser
 Author-email: juan.bokser@moneyonchain.com
 License: UNKNOWN
 Description: # **MoC prices source**
         
@@ -32,15 +32,15 @@
         >>> get_price(BTC_USD)
         Decimal('29395.82')
         >>> 
         ```
         
         And that's it!
         
-        More [usage examples](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b5/docs/examples.md) can be seen [here](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b5/docs/examples.md)
+        More [usage examples](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b7/docs/examples.md) can be seen [here](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b7/docs/examples.md)
         
         
         
         ## How the included CLI tool looks like
         
         Here you can see how the output of the `moc_prices_source_check` command looks like
         
@@ -61,21 +61,21 @@
         
         Response time 1.1s
         
         user@host:~$ 
         ```
         
         This command has many options. you can run `moc_prices_source_check --help` to get help on how to run them.
-        More information about this CLI tool can be seen [here](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b5/docs/cli.md).
+        More information about this CLI tool can be seen [here](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b7/docs/cli.md).
         
         
         
         ## References
         
-        * [Source code in Github](https://github.com/money-on-chain/moc_prices_source/tree/v0.7.0b5)
+        * [Source code in Github](https://github.com/money-on-chain/moc_prices_source/tree/v0.7.0b7)
         * [Package from Python package index (PyPI)](https://pypi.org/project/moneyonchain-prices-source)
         
         
         
         ## Requirements
         
         * Python 3.6+ support
@@ -98,15 +98,15 @@
         $ moc_prices_source_check --version
         ```
         
         To verify that it has been installed correctly
         
         ### From source
         
-        Download from [Github](https://github.com/money-on-chain/moc_prices_source/tree/v0.7.0b5)
+        Download from [Github](https://github.com/money-on-chain/moc_prices_source/tree/v0.7.0b7)
         
         Standing inside the folder, run:
         
         ```shell
         $ pip3 install -r requirements.txt 
         ```
         
@@ -124,15 +124,15 @@
         
         To verify that it has been installed correctly
         
         
         
         ## Supported coinpairs and symbols
         
-        [Here](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b5/docs/supported_coinpairs.md) you can find an [summary of supported coinpairs and symbols](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b5/docs/supported_coinpairs.md)
+        [Here](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b7/docs/supported_coinpairs.md) you can find an [summary of supported coinpairs and symbols](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b7/docs/supported_coinpairs.md)
         
         
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
```

### Comparing `moneyonchain_prices_source-0.7.0b5/moneyonchain_prices_source.egg-info/SOURCES.txt` & `moneyonchain_prices_source-0.7.0b7/moneyonchain_prices_source.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 moc_prices_source/engines/btc_usd_cex.py
 moc_prices_source/engines/btc_usd_coinbase.py
 moc_prices_source/engines/btc_usd_gemini.py
 moc_prices_source/engines/btc_usd_itbit.py
 moc_prices_source/engines/btc_usd_kraken.py
 moc_prices_source/engines/btc_usd_kucoin.py
 moc_prices_source/engines/btc_usd_okcoin.py
+moc_prices_source/engines/btc_usd_onchain.py
 moc_prices_source/engines/btc_usdt_binance.py
 moc_prices_source/engines/btc_usdt_bitfinex.py
 moc_prices_source/engines/btc_usdt_coinbase.py
 moc_prices_source/engines/btc_usdt_kraken.py
 moc_prices_source/engines/coins.py
 moc_prices_source/engines/engine_base.py
 moc_prices_source/engines/eth_btc_binance.py
```

### Comparing `moneyonchain_prices_source-0.7.0b5/setup.py` & `moneyonchain_prices_source-0.7.0b7/setup.py`

 * *Files identical despite different names*

