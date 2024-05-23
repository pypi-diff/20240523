# Comparing `tmp/moneyonchain_prices_source-0.7.0b7.tar.gz` & `tmp/moneyonchain_prices_source-0.7.0b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moneyonchain_prices_source-0.7.0b7.tar", last modified: Thu May 23 15:12:54 2024, max compression
+gzip compressed data, was "moneyonchain_prices_source-0.7.0b8.tar", last modified: Thu May 23 16:53:39 2024, max compression
```

## Comparing `moneyonchain_prices_source-0.7.0b7.tar` & `moneyonchain_prices_source-0.7.0b8.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2024-05-23 15:12:54.817398 moneyonchain_prices_source-0.7.0b7/
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4743 2024-05-23 15:12:54.817398 moneyonchain_prices_source-0.7.0b7/PKG-INFO
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     2942 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b7/README.md
-drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2024-05-23 15:12:54.729397 moneyonchain_prices_source-0.7.0b7/moc_prices_source/
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     7229 2024-05-23 12:32:30.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/__init__.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      486 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/cli.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    11492 2024-05-23 14:44:06.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/cli_check.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      628 2024-05-17 19:12:34.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/coins.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     3272 2024-05-22 20:08:39.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/computed_pairs.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     3892 2024-05-10 19:44:58.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/conf.py
-drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2024-05-23 15:12:54.729397 moneyonchain_prices_source-0.7.0b7/moc_prices_source/data/
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      174 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/data/database_default.json
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       17 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/data/redis_default.json
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      221 2024-05-14 13:03:36.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/data/remote_weighing_default.json
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     2428 2024-05-22 20:08:59.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/data/weighing.json
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     5865 2024-05-20 15:22:32.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/database.py
-drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2024-05-23 15:12:54.813398 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     3806 2024-04-30 20:09:02.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/__init__.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      766 2024-05-20 12:30:23.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/bnb_usdt_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      720 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_argenbtc.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      791 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_belo_app.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      869 2024-05-20 12:30:52.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      770 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_bitso.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      788 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_buda.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      762 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_buenbit.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      635 2024-05-20 12:27:49.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_coinbase.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      756 2024-05-21 15:01:04.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_cryptomkt.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      836 2024-05-21 13:16:41.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_decrypto.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      919 2024-05-20 12:32:50.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_lemoncash.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      805 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_ripio.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      772 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_ripio_exch.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      643 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_rofex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      718 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_satoshitango.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      770 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_cop_bitso.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      788 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_cop_buda.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      763 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_cop_buenbit.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      521 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_cop_coinbase.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      756 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_cop_cryptomkt.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      523 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usd_bitfinex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      693 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usd_bitgo.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      535 2024-04-30 16:19:10.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usd_bitstamp.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usd_bittrex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      503 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usd_blockchain.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      518 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usd_cex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      526 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usd_coinbase.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      505 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usd_gemini.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      513 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usd_itbit.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      582 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usd_kraken.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      559 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usd_kucoin.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      524 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usd_okcoin.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1823 2024-05-22 12:26:22.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usd_onchain.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      859 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usdt_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      525 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usdt_bitfinex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usdt_coinbase.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      581 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usdt_kraken.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     5726 2024-05-22 20:08:10.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/coins.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    13974 2024-04-30 19:24:19.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/engine_base.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      856 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/eth_btc_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      523 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/eth_btc_bitfinex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      535 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/eth_btc_bitstamp.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      505 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/eth_btc_gemini.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      580 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/eth_btc_kraken.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1616 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/gas_btc_rsk.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1484 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/moc_btc_sovryn.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      856 2023-05-12 17:54:43.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_btc_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      584 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_btc_bitfinex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      666 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_btc_coinbene.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      636 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_btc_coingecko.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      639 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_btc_kucoin.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      627 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_btc_mexc.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1822 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_btc_mp1p_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      627 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_btc_mxc.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1484 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_btc_sovryn.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      859 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_usdt_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      598 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_usdt_ma2_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      598 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_usdt_ma3_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1814 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_usdt_ma_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1828 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_usdt_mp1p_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      822 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_ambito.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      829 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_ccl_ambito.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      640 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_ccl_coinmonitor.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      696 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_ccl_criptoya.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1359 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_ccl_cronista.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1301 2024-04-29 14:09:15.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_ccl_dolarhoy.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1125 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_ccl_dolarsi.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1255 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_ccl_infobae.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1441 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_ccl_infodolar.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      858 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_ccl_lanacion.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      653 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_ccl_rofex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      632 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_coinmonitor.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      728 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_criptoya.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1339 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_cronista.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1283 2024-04-29 14:09:23.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_dolarhoy.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1108 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_dolarsi.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1250 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_infobae.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1414 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_infodolar.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      855 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_lanacion.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      537 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_cop_banrep.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1494 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_cop_dolarhoy.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      921 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_mxn_bitso.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1069 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_mxn_citibanamex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1224 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_mxn_coinmonitor.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1181 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_mxn_currencymeuk.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1193 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_mxn_eldolar_info.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1235 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_mxn_eleconomista.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1344 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_mxn_infodolar.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1078 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_mxn_intercam.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1125 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_mxn_themoneyconverter.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      806 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_mxn_wise.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1223 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_mxn_xrates.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usdt_usd_bitstamp.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usdt_usd_coinbase.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      584 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usdt_usd_kraken.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      718 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/my_logging.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     6943 2024-05-21 16:17:41.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/server.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     8576 2024-05-23 14:47:40.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/to_db.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)        8 2024-05-23 15:09:55.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/version.txt
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     8315 2024-05-23 15:02:25.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source/weighing.py
--rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)      117 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source_api
--rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)      118 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source_check
--rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)      128 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.7.0b7/moc_prices_source_to_db
-drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2024-05-23 15:12:54.817398 moneyonchain_prices_source-0.7.0b7/moneyonchain_prices_source.egg-info/
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4743 2024-05-23 15:12:53.000000 moneyonchain_prices_source-0.7.0b7/moneyonchain_prices_source.egg-info/PKG-INFO
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     5275 2024-05-23 15:12:54.000000 moneyonchain_prices_source-0.7.0b7/moneyonchain_prices_source.egg-info/SOURCES.txt
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)        1 2024-05-23 15:12:53.000000 moneyonchain_prices_source-0.7.0b7/moneyonchain_prices_source.egg-info/dependency_links.txt
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      146 2024-05-23 15:12:53.000000 moneyonchain_prices_source-0.7.0b7/moneyonchain_prices_source.egg-info/requires.txt
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       18 2024-05-23 15:12:53.000000 moneyonchain_prices_source-0.7.0b7/moneyonchain_prices_source.egg-info/top_level.txt
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       38 2024-05-23 15:12:54.817398 moneyonchain_prices_source-0.7.0b7/setup.cfg
--rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)     1863 2024-04-29 14:33:12.000000 moneyonchain_prices_source-0.7.0b7/setup.py
+drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2024-05-23 16:53:39.654860 moneyonchain_prices_source-0.7.0b8/
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4743 2024-05-23 16:53:39.654860 moneyonchain_prices_source-0.7.0b8/PKG-INFO
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     2942 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b8/README.md
+drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2024-05-23 16:53:39.630860 moneyonchain_prices_source-0.7.0b8/moc_prices_source/
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     7312 2024-05-23 16:41:54.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/__init__.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      486 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/cli.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    11513 2024-05-23 16:46:00.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/cli_check.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      628 2024-05-17 19:12:34.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/coins.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     3272 2024-05-22 20:08:39.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/computed_pairs.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     3892 2024-05-10 19:44:58.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/conf.py
+drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2024-05-23 16:53:39.630860 moneyonchain_prices_source-0.7.0b8/moc_prices_source/data/
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      174 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/data/database_default.json
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       17 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/data/redis_default.json
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      221 2024-05-14 13:03:36.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/data/remote_weighing_default.json
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     2428 2024-05-22 20:08:59.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/data/weighing.json
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     5865 2024-05-20 15:22:32.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/database.py
+drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2024-05-23 16:53:39.654860 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     3806 2024-04-30 20:09:02.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/__init__.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      766 2024-05-20 12:30:23.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/bnb_usdt_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      720 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_ars_argenbtc.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      791 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_ars_belo_app.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      869 2024-05-20 12:30:52.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_ars_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      770 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_ars_bitso.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      788 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_ars_buda.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      762 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_ars_buenbit.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      635 2024-05-20 12:27:49.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_ars_coinbase.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      756 2024-05-21 15:01:04.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_ars_cryptomkt.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      836 2024-05-21 13:16:41.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_ars_decrypto.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      919 2024-05-20 12:32:50.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_ars_lemoncash.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      805 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_ars_ripio.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      772 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_ars_ripio_exch.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      643 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_ars_rofex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      718 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_ars_satoshitango.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      770 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_cop_bitso.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      788 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_cop_buda.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      763 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_cop_buenbit.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      521 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_cop_coinbase.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      756 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_cop_cryptomkt.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      523 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_usd_bitfinex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      693 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_usd_bitgo.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      535 2024-04-30 16:19:10.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_usd_bitstamp.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_usd_bittrex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      503 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_usd_blockchain.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      518 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_usd_cex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      526 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_usd_coinbase.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      505 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_usd_gemini.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      513 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_usd_itbit.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      582 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_usd_kraken.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      559 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_usd_kucoin.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      524 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_usd_okcoin.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1823 2024-05-22 12:26:22.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_usd_onchain.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      859 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_usdt_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      525 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_usdt_bitfinex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_usdt_coinbase.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      581 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_usdt_kraken.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     5726 2024-05-22 20:08:10.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/coins.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    13974 2024-04-30 19:24:19.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/engine_base.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      856 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/eth_btc_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      523 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/eth_btc_bitfinex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      535 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/eth_btc_bitstamp.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      505 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/eth_btc_gemini.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      580 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/eth_btc_kraken.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1616 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/gas_btc_rsk.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1484 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/moc_btc_sovryn.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      856 2023-05-12 17:54:43.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/rif_btc_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      584 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/rif_btc_bitfinex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      666 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/rif_btc_coinbene.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      636 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/rif_btc_coingecko.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      639 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/rif_btc_kucoin.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      627 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/rif_btc_mexc.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1822 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/rif_btc_mp1p_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      627 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/rif_btc_mxc.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1484 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/rif_btc_sovryn.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      859 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/rif_usdt_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      598 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/rif_usdt_ma2_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      598 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/rif_usdt_ma3_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1814 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/rif_usdt_ma_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1828 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/rif_usdt_mp1p_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      822 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_ars_ambito.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      829 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_ars_ccl_ambito.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      640 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_ars_ccl_coinmonitor.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      696 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_ars_ccl_criptoya.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1359 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_ars_ccl_cronista.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1301 2024-04-29 14:09:15.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_ars_ccl_dolarhoy.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1125 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_ars_ccl_dolarsi.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1255 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_ars_ccl_infobae.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1441 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_ars_ccl_infodolar.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      858 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_ars_ccl_lanacion.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      653 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_ars_ccl_rofex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      632 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_ars_coinmonitor.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      728 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_ars_criptoya.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1339 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_ars_cronista.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1283 2024-04-29 14:09:23.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_ars_dolarhoy.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1108 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_ars_dolarsi.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1250 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_ars_infobae.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1414 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_ars_infodolar.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      855 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_ars_lanacion.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      537 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_cop_banrep.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1494 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_cop_dolarhoy.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      921 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_mxn_bitso.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1069 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_mxn_citibanamex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1224 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_mxn_coinmonitor.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1181 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_mxn_currencymeuk.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1193 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_mxn_eldolar_info.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1235 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_mxn_eleconomista.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1344 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_mxn_infodolar.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1078 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_mxn_intercam.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1125 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_mxn_themoneyconverter.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      806 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_mxn_wise.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1223 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_mxn_xrates.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usdt_usd_bitstamp.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usdt_usd_coinbase.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      584 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usdt_usd_kraken.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      718 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/my_logging.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     6943 2024-05-21 16:17:41.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/server.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     8576 2024-05-23 14:47:40.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/to_db.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)        8 2024-05-23 16:49:39.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/version.txt
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     8315 2024-05-23 15:02:25.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source/weighing.py
+-rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)      117 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source_api
+-rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)      118 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source_check
+-rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)      128 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.7.0b8/moc_prices_source_to_db
+drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2024-05-23 16:53:39.654860 moneyonchain_prices_source-0.7.0b8/moneyonchain_prices_source.egg-info/
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4743 2024-05-23 16:53:38.000000 moneyonchain_prices_source-0.7.0b8/moneyonchain_prices_source.egg-info/PKG-INFO
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     5275 2024-05-23 16:53:39.000000 moneyonchain_prices_source-0.7.0b8/moneyonchain_prices_source.egg-info/SOURCES.txt
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)        1 2024-05-23 16:53:38.000000 moneyonchain_prices_source-0.7.0b8/moneyonchain_prices_source.egg-info/dependency_links.txt
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      146 2024-05-23 16:53:38.000000 moneyonchain_prices_source-0.7.0b8/moneyonchain_prices_source.egg-info/requires.txt
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       18 2024-05-23 16:53:38.000000 moneyonchain_prices_source-0.7.0b8/moneyonchain_prices_source.egg-info/top_level.txt
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       38 2024-05-23 16:53:39.658860 moneyonchain_prices_source-0.7.0b8/setup.cfg
+-rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)     1863 2024-04-29 14:33:12.000000 moneyonchain_prices_source-0.7.0b8/setup.py
```

### Comparing `moneyonchain_prices_source-0.7.0b7/PKG-INFO` & `moneyonchain_prices_source-0.7.0b8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moneyonchain_prices_source
-Version: 0.7.0b7
+Version: 0.7.0b8
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
         
-        More [usage examples](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b7/docs/examples.md) can be seen [here](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b7/docs/examples.md)
+        More [usage examples](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b8/docs/examples.md) can be seen [here](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b8/docs/examples.md)
         
         
         
         ## How the included CLI tool looks like
         
         Here you can see how the output of the `moc_prices_source_check` command looks like
         
@@ -61,21 +61,21 @@
         
         Response time 1.1s
         
         user@host:~$ 
         ```
         
         This command has many options. you can run `moc_prices_source_check --help` to get help on how to run them.
-        More information about this CLI tool can be seen [here](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b7/docs/cli.md).
+        More information about this CLI tool can be seen [here](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b8/docs/cli.md).
         
         
         
         ## References
         
-        * [Source code in Github](https://github.com/money-on-chain/moc_prices_source/tree/v0.7.0b7)
+        * [Source code in Github](https://github.com/money-on-chain/moc_prices_source/tree/v0.7.0b8)
         * [Package from Python package index (PyPI)](https://pypi.org/project/moneyonchain-prices-source)
         
         
         
         ## Requirements
         
         * Python 3.6+ support
@@ -98,15 +98,15 @@
         $ moc_prices_source_check --version
         ```
         
         To verify that it has been installed correctly
         
         ### From source
         
-        Download from [Github](https://github.com/money-on-chain/moc_prices_source/tree/v0.7.0b7)
+        Download from [Github](https://github.com/money-on-chain/moc_prices_source/tree/v0.7.0b8)
         
         Standing inside the folder, run:
         
         ```shell
         $ pip3 install -r requirements.txt 
         ```
         
@@ -124,15 +124,15 @@
         
         To verify that it has been installed correctly
         
         
         
         ## Supported coinpairs and symbols
         
-        [Here](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b7/docs/supported_coinpairs.md) you can find an [summary of supported coinpairs and symbols](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b7/docs/supported_coinpairs.md)
+        [Here](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b8/docs/supported_coinpairs.md) you can find an [summary of supported coinpairs and symbols](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b8/docs/supported_coinpairs.md)
         
         
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
```

### Comparing `moneyonchain_prices_source-0.7.0b7/README.md` & `moneyonchain_prices_source-0.7.0b8/README.md`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/__init__.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 def get_price(
     coinpairs            = None,
     engines_names        = None,
     detail               = {},
     weighing             = weighing,
     serializable         = False,
-    ignore_zero_weighing = False):
+    ignore_zero_weighing = True):
 
     start_time = datetime.datetime.now()
 
     requested = coinpairs
 
     if coinpairs:
 
@@ -108,29 +108,31 @@
             d['prices'].append(v['price'])
         del d['data']
         del d['sum_weighing']
 
         ok_sources_count = len(list(filter(bool, d['weighings'])))
         min_ok_sources_count = k.min_ok_sources_count
 
+        d['median_price'] = median(d['prices'])
+        d['mean_price'] = mean(d['prices'])
+        if any (d['weighings']):
+            d['weighted_median_price'] = weighted_median(d['prices'], d['weighings'])
+        else:
+            d['weighted_median_price'] = None
+
         d['ok_sources_count'] = ok_sources_count
         d['min_ok_sources_count'] = min_ok_sources_count
         d['ok'] = True
         d['error'] = ''
+        d['ok_value'] = d['weighted_median_price']
 
         if ok_sources_count < min_ok_sources_count:
             d['ok'] = False
             d['error'] = f"Not enough price sources ({ok_sources_count} < {min_ok_sources_count})"
-
-        d['median_price'] = median(d['prices'])
-        d['mean_price'] = mean(d['prices'])
-        if any (d['weighings']):
-            d['weighted_median_price'] = weighted_median(d['prices'], d['weighings'])
-        else:
-            d['weighted_median_price'] = None
+            d['ok_value'] = None
 
     if requested:
         for r in [r for r in requested if (
             (r in computed_pairs) and (not r in coinpair_prices)) ]:
             requirements = computed_pairs[r]['requirements']
             if set(requirements).issubset(set(coinpair_prices.keys())):
                 coinpair_prices[r] = {}
```

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/cli_check.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/cli_check.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,26 +194,26 @@
         help='Show the default weighing and exit.')
 @option('-c', '--computed', 'show_computed_pairs', is_flag=True,
         help='Show the computed pairs formula and exit.')
 @option('-s', '--summary', 'show_summary', is_flag=True,
         help='Show the summary and exit.')
 @option('-m', '--markdown', 'md_summary', is_flag=True,
         help='Set markdown for the summary format.')
-@option('-z', '--ignore-zero-weighing', 'ignore_zero_weighing', is_flag=True,
-        help='Ignore sources with zero weighing.')
+@option('-n', '--not-ignore-zero-weighing', 'not_ignore_zero_weighing',
+        is_flag=True, help='Ignore sources with zero weighing.')
 @cli.argument('coinpairs_filter', required=False)
 def cli_check(
         show_version=False,
         show_json=False,
         show_weighing=False,
         show_computed_pairs=False,
         coinpairs_filter=None,
         show_summary=False,
         md_summary=False,
-        ignore_zero_weighing=False
+        not_ignore_zero_weighing=False
     ):
     """\b
 Description:
     CLI-type tool that shows the data obtained by
     the `moc_price_source` library.   
     Useful for troubleshooting.
 \n\b
@@ -262,15 +262,15 @@
         summary(coinpairs, md_summary)
         return
 
     data = {}
 
     get_price(
         coinpairs,
-        ignore_zero_weighing=ignore_zero_weighing,
+        ignore_zero_weighing=not(not_ignore_zero_weighing),
         detail=data,
         serializable=show_json)
 
     if show_json:
         print(json.dumps(data, indent=4, sort_keys=True))
         return
```

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/coins.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/coins.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/computed_pairs.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/computed_pairs.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/conf.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/conf.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/data/weighing.json` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/data/weighing.json`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/database.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/database.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/__init__.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/bnb_usdt_binance.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/bnb_usdt_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_argenbtc.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_ars_argenbtc.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_belo_app.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_ars_belo_app.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_binance.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_ars_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_bitso.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_ars_bitso.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_buda.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_ars_buda.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_buenbit.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_ars_buenbit.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_coinbase.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_ars_coinbase.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_cryptomkt.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_ars_cryptomkt.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_decrypto.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_ars_decrypto.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_lemoncash.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_ars_lemoncash.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_ripio.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_ars_ripio.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_ripio_exch.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_ars_ripio_exch.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_rofex.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_ars_rofex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_ars_satoshitango.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_ars_satoshitango.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_cop_bitso.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_cop_bitso.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_cop_buda.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_cop_buda.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_cop_buenbit.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_cop_buenbit.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_cop_coinbase.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_cop_coinbase.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_cop_cryptomkt.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_cop_cryptomkt.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usd_bitfinex.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_usd_bitfinex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usd_bitgo.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_usd_bitgo.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usd_bitstamp.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_usd_bitstamp.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usd_bittrex.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_usd_bittrex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usd_cex.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_usd_cex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usd_coinbase.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_usd_coinbase.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usd_itbit.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_usd_itbit.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usd_kraken.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_usd_kraken.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usd_kucoin.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_usd_kucoin.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usd_okcoin.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_usd_okcoin.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usd_onchain.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_usd_onchain.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usdt_binance.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_usdt_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usdt_bitfinex.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_usdt_bitfinex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usdt_coinbase.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_usdt_coinbase.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/btc_usdt_kraken.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/btc_usdt_kraken.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/coins.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/coins.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/engine_base.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/engine_base.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/eth_btc_binance.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/eth_btc_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/eth_btc_bitfinex.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/eth_btc_bitfinex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/eth_btc_bitstamp.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/eth_btc_bitstamp.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/eth_btc_kraken.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/eth_btc_kraken.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/gas_btc_rsk.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/gas_btc_rsk.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/moc_btc_sovryn.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/moc_btc_sovryn.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_btc_binance.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/rif_btc_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_btc_bitfinex.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/rif_btc_bitfinex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_btc_coinbene.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/rif_btc_coinbene.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_btc_coingecko.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/rif_btc_coingecko.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_btc_kucoin.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/rif_btc_kucoin.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_btc_mexc.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/rif_btc_mexc.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_btc_mp1p_binance.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/rif_btc_mp1p_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_btc_mxc.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/rif_btc_mxc.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_btc_sovryn.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/rif_btc_sovryn.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_usdt_binance.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/rif_usdt_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_usdt_ma2_binance.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/rif_usdt_ma2_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_usdt_ma3_binance.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/rif_usdt_ma3_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_usdt_ma_binance.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/rif_usdt_ma_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/rif_usdt_mp1p_binance.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/rif_usdt_mp1p_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_ambito.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_ars_ambito.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_ccl_ambito.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_ars_ccl_ambito.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_ccl_coinmonitor.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_ars_ccl_coinmonitor.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_ccl_criptoya.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_ars_ccl_criptoya.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_ccl_cronista.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_ars_ccl_cronista.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_ccl_dolarhoy.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_ars_ccl_dolarhoy.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_ccl_dolarsi.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_ars_ccl_dolarsi.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_ccl_infobae.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_ars_ccl_infobae.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_ccl_infodolar.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_ars_ccl_infodolar.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_ccl_lanacion.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_ars_ccl_lanacion.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_ccl_rofex.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_ars_ccl_rofex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_coinmonitor.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_ars_coinmonitor.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_criptoya.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_ars_criptoya.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_cronista.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_ars_cronista.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_dolarhoy.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_ars_dolarhoy.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_dolarsi.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_ars_dolarsi.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_infobae.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_ars_infobae.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_infodolar.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_ars_infodolar.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_ars_lanacion.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_ars_lanacion.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_cop_banrep.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_cop_banrep.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_cop_dolarhoy.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_cop_dolarhoy.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_mxn_bitso.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_mxn_bitso.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_mxn_citibanamex.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_mxn_citibanamex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_mxn_coinmonitor.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_mxn_coinmonitor.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_mxn_currencymeuk.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_mxn_currencymeuk.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_mxn_eldolar_info.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_mxn_eldolar_info.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_mxn_eleconomista.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_mxn_eleconomista.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_mxn_infodolar.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_mxn_infodolar.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_mxn_intercam.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_mxn_intercam.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_mxn_themoneyconverter.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_mxn_themoneyconverter.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_mxn_wise.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_mxn_wise.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usd_mxn_xrates.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usd_mxn_xrates.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usdt_usd_bitstamp.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usdt_usd_bitstamp.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usdt_usd_coinbase.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usdt_usd_coinbase.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/engines/usdt_usd_kraken.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/engines/usdt_usd_kraken.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/my_logging.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/my_logging.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/server.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/server.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/to_db.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/to_db.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moc_prices_source/weighing.py` & `moneyonchain_prices_source-0.7.0b8/moc_prices_source/weighing.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/moneyonchain_prices_source.egg-info/PKG-INFO` & `moneyonchain_prices_source-0.7.0b8/moneyonchain_prices_source.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moneyonchain-prices-source
-Version: 0.7.0b7
+Version: 0.7.0b8
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
         
-        More [usage examples](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b7/docs/examples.md) can be seen [here](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b7/docs/examples.md)
+        More [usage examples](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b8/docs/examples.md) can be seen [here](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b8/docs/examples.md)
         
         
         
         ## How the included CLI tool looks like
         
         Here you can see how the output of the `moc_prices_source_check` command looks like
         
@@ -61,21 +61,21 @@
         
         Response time 1.1s
         
         user@host:~$ 
         ```
         
         This command has many options. you can run `moc_prices_source_check --help` to get help on how to run them.
-        More information about this CLI tool can be seen [here](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b7/docs/cli.md).
+        More information about this CLI tool can be seen [here](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b8/docs/cli.md).
         
         
         
         ## References
         
-        * [Source code in Github](https://github.com/money-on-chain/moc_prices_source/tree/v0.7.0b7)
+        * [Source code in Github](https://github.com/money-on-chain/moc_prices_source/tree/v0.7.0b8)
         * [Package from Python package index (PyPI)](https://pypi.org/project/moneyonchain-prices-source)
         
         
         
         ## Requirements
         
         * Python 3.6+ support
@@ -98,15 +98,15 @@
         $ moc_prices_source_check --version
         ```
         
         To verify that it has been installed correctly
         
         ### From source
         
-        Download from [Github](https://github.com/money-on-chain/moc_prices_source/tree/v0.7.0b7)
+        Download from [Github](https://github.com/money-on-chain/moc_prices_source/tree/v0.7.0b8)
         
         Standing inside the folder, run:
         
         ```shell
         $ pip3 install -r requirements.txt 
         ```
         
@@ -124,15 +124,15 @@
         
         To verify that it has been installed correctly
         
         
         
         ## Supported coinpairs and symbols
         
-        [Here](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b7/docs/supported_coinpairs.md) you can find an [summary of supported coinpairs and symbols](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b7/docs/supported_coinpairs.md)
+        [Here](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b8/docs/supported_coinpairs.md) you can find an [summary of supported coinpairs and symbols](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b8/docs/supported_coinpairs.md)
         
         
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
```

### Comparing `moneyonchain_prices_source-0.7.0b7/moneyonchain_prices_source.egg-info/SOURCES.txt` & `moneyonchain_prices_source-0.7.0b8/moneyonchain_prices_source.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b7/setup.py` & `moneyonchain_prices_source-0.7.0b8/setup.py`

 * *Files identical despite different names*

