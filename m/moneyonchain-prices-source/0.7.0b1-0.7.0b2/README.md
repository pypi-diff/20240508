# Comparing `tmp/moneyonchain_prices_source-0.7.0b1.tar.gz` & `tmp/moneyonchain_prices_source-0.7.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moneyonchain_prices_source-0.7.0b1.tar", last modified: Tue Apr 30 20:12:38 2024, max compression
+gzip compressed data, was "moneyonchain_prices_source-0.7.0b2.tar", last modified: Wed May  8 15:11:13 2024, max compression
```

## Comparing `moneyonchain_prices_source-0.7.0b1.tar` & `moneyonchain_prices_source-0.7.0b2.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2024-04-30 20:12:38.535833 moneyonchain_prices_source-0.7.0b1/
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4743 2024-04-30 20:12:38.535833 moneyonchain_prices_source-0.7.0b1/PKG-INFO
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     2942 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b1/README.md
-drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2024-04-30 20:12:38.511832 moneyonchain_prices_source-0.7.0b1/moc_prices_source/
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     6610 2024-04-30 17:56:23.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/__init__.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      486 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/cli.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    10644 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/cli_check.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      625 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/coins.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     3247 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/computed_pairs.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     3892 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/conf.py
-drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2024-04-30 20:12:38.511832 moneyonchain_prices_source-0.7.0b1/moc_prices_source/data/
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      174 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/data/database_default.json
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       17 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/data/redis_default.json
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     2419 2024-04-29 14:18:02.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/data/weighing.json
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     5715 2024-01-11 13:54:48.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/database.py
-drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2024-04-30 20:12:38.535833 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     3806 2024-04-30 20:09:02.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/__init__.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      766 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/bnb_usdt_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      720 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_ars_argenbtc.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      791 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_ars_belo_app.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      816 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_ars_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      770 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_ars_bitso.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      788 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_ars_buda.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      762 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_ars_buenbit.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      521 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_ars_coinbase.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      756 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_ars_cryptomkt.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      836 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_ars_decrypto.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      805 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_ars_lemoncash.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      805 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_ars_ripio.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      772 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_ars_ripio_exch.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      643 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_ars_rofex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      718 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_ars_satoshitango.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      770 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_cop_bitso.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      788 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_cop_buda.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      763 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_cop_buenbit.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      521 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_cop_coinbase.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      756 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_cop_cryptomkt.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      523 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_usd_bitfinex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      693 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_usd_bitgo.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      535 2024-04-30 16:19:10.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_usd_bitstamp.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_usd_bittrex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      503 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_usd_blockchain.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      518 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_usd_cex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      526 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_usd_coinbase.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      505 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_usd_gemini.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      513 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_usd_itbit.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      582 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_usd_kraken.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      559 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_usd_kucoin.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      524 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_usd_okcoin.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      859 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_usdt_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      525 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_usdt_bitfinex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_usdt_coinbase.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      581 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_usdt_kraken.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     5459 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/coins.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    13974 2024-04-30 19:24:19.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/engine_base.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      856 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/eth_btc_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      523 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/eth_btc_bitfinex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      535 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/eth_btc_bitstamp.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      505 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/eth_btc_gemini.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      580 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/eth_btc_kraken.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1616 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/gas_btc_rsk.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1484 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/moc_btc_sovryn.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      856 2023-05-12 17:54:43.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/rif_btc_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      584 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/rif_btc_bitfinex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      666 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/rif_btc_coinbene.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      636 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/rif_btc_coingecko.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      639 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/rif_btc_kucoin.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      627 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/rif_btc_mexc.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1822 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/rif_btc_mp1p_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      627 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/rif_btc_mxc.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1484 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/rif_btc_sovryn.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      859 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/rif_usdt_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      598 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/rif_usdt_ma2_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      598 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/rif_usdt_ma3_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1814 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/rif_usdt_ma_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1828 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/rif_usdt_mp1p_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      822 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_ars_ambito.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      829 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_ars_ccl_ambito.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      640 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_ars_ccl_coinmonitor.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      696 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_ars_ccl_criptoya.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1359 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_ars_ccl_cronista.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1301 2024-04-29 14:09:15.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_ars_ccl_dolarhoy.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1125 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_ars_ccl_dolarsi.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1255 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_ars_ccl_infobae.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1441 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_ars_ccl_infodolar.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      858 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_ars_ccl_lanacion.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      653 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_ars_ccl_rofex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      632 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_ars_coinmonitor.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      728 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_ars_criptoya.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1339 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_ars_cronista.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1283 2024-04-29 14:09:23.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_ars_dolarhoy.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1108 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_ars_dolarsi.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1250 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_ars_infobae.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1414 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_ars_infodolar.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      855 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_ars_lanacion.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      537 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_cop_banrep.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1494 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_cop_dolarhoy.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      921 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_mxn_bitso.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1069 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_mxn_citibanamex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1224 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_mxn_coinmonitor.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1181 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_mxn_currencymeuk.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1193 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_mxn_eldolar_info.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1235 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_mxn_eleconomista.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1344 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_mxn_infodolar.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1078 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_mxn_intercam.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1125 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_mxn_themoneyconverter.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      806 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_mxn_wise.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1223 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_mxn_xrates.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usdt_usd_bitstamp.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usdt_usd_coinbase.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      584 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usdt_usd_kraken.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      718 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/my_logging.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     5441 2024-04-30 16:07:24.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/server.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     6008 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/to_db.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)        8 2024-04-30 19:34:22.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/version.txt
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     5014 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source/weighing.py
--rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)      117 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source_api
--rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)      118 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source_check
--rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)      128 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.7.0b1/moc_prices_source_to_db
-drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2024-04-30 20:12:38.535833 moneyonchain_prices_source-0.7.0b1/moneyonchain_prices_source.egg-info/
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4743 2024-04-30 20:12:37.000000 moneyonchain_prices_source-0.7.0b1/moneyonchain_prices_source.egg-info/PKG-INFO
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     5178 2024-04-30 20:12:38.000000 moneyonchain_prices_source-0.7.0b1/moneyonchain_prices_source.egg-info/SOURCES.txt
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)        1 2024-04-30 20:12:37.000000 moneyonchain_prices_source-0.7.0b1/moneyonchain_prices_source.egg-info/dependency_links.txt
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      146 2024-04-30 20:12:37.000000 moneyonchain_prices_source-0.7.0b1/moneyonchain_prices_source.egg-info/requires.txt
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       18 2024-04-30 20:12:37.000000 moneyonchain_prices_source-0.7.0b1/moneyonchain_prices_source.egg-info/top_level.txt
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       38 2024-04-30 20:12:38.535833 moneyonchain_prices_source-0.7.0b1/setup.cfg
--rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)     1863 2024-04-29 14:33:12.000000 moneyonchain_prices_source-0.7.0b1/setup.py
+drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2024-05-08 15:11:13.972430 moneyonchain_prices_source-0.7.0b2/
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4743 2024-05-08 15:11:13.972430 moneyonchain_prices_source-0.7.0b2/PKG-INFO
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     2942 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b2/README.md
+drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2024-05-08 15:11:13.888435 moneyonchain_prices_source-0.7.0b2/moc_prices_source/
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     6610 2024-04-30 17:56:23.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/__init__.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      486 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/cli.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    10644 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/cli_check.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      625 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/coins.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     3247 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/computed_pairs.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     3892 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/conf.py
+drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2024-05-08 15:11:13.904434 moneyonchain_prices_source-0.7.0b2/moc_prices_source/data/
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      174 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/data/database_default.json
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       17 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/data/redis_default.json
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     2419 2024-04-29 14:18:02.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/data/weighing.json
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     5715 2024-01-11 13:54:48.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/database.py
+drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2024-05-08 15:11:13.972430 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     3806 2024-04-30 20:09:02.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/__init__.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      766 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/bnb_usdt_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      720 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_ars_argenbtc.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      791 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_ars_belo_app.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      816 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_ars_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      770 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_ars_bitso.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      788 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_ars_buda.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      762 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_ars_buenbit.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      521 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_ars_coinbase.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      756 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_ars_cryptomkt.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      836 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_ars_decrypto.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      805 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_ars_lemoncash.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      805 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_ars_ripio.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      772 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_ars_ripio_exch.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      643 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_ars_rofex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      718 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_ars_satoshitango.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      770 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_cop_bitso.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      788 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_cop_buda.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      763 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_cop_buenbit.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      521 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_cop_coinbase.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      756 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_cop_cryptomkt.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      523 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_usd_bitfinex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      693 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_usd_bitgo.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      535 2024-04-30 16:19:10.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_usd_bitstamp.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_usd_bittrex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      503 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_usd_blockchain.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      518 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_usd_cex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      526 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_usd_coinbase.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      505 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_usd_gemini.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      513 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_usd_itbit.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      582 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_usd_kraken.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      559 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_usd_kucoin.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      524 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_usd_okcoin.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      859 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_usdt_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      525 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_usdt_bitfinex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_usdt_coinbase.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      581 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_usdt_kraken.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     5459 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/coins.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    13974 2024-04-30 19:24:19.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/engine_base.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      856 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/eth_btc_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      523 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/eth_btc_bitfinex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      535 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/eth_btc_bitstamp.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      505 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/eth_btc_gemini.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      580 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/eth_btc_kraken.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1616 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/gas_btc_rsk.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1484 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/moc_btc_sovryn.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      856 2023-05-12 17:54:43.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/rif_btc_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      584 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/rif_btc_bitfinex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      666 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/rif_btc_coinbene.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      636 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/rif_btc_coingecko.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      639 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/rif_btc_kucoin.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      627 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/rif_btc_mexc.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1822 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/rif_btc_mp1p_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      627 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/rif_btc_mxc.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1484 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/rif_btc_sovryn.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      859 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/rif_usdt_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      598 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/rif_usdt_ma2_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      598 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/rif_usdt_ma3_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1814 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/rif_usdt_ma_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1828 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/rif_usdt_mp1p_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      822 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_ars_ambito.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      829 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_ars_ccl_ambito.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      640 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_ars_ccl_coinmonitor.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      696 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_ars_ccl_criptoya.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1359 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_ars_ccl_cronista.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1301 2024-04-29 14:09:15.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_ars_ccl_dolarhoy.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1125 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_ars_ccl_dolarsi.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1255 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_ars_ccl_infobae.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1441 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_ars_ccl_infodolar.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      858 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_ars_ccl_lanacion.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      653 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_ars_ccl_rofex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      632 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_ars_coinmonitor.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      728 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_ars_criptoya.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1339 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_ars_cronista.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1283 2024-04-29 14:09:23.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_ars_dolarhoy.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1108 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_ars_dolarsi.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1250 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_ars_infobae.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1414 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_ars_infodolar.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      855 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_ars_lanacion.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      537 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_cop_banrep.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1494 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_cop_dolarhoy.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      921 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_mxn_bitso.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1069 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_mxn_citibanamex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1224 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_mxn_coinmonitor.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1181 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_mxn_currencymeuk.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1193 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_mxn_eldolar_info.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1235 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_mxn_eleconomista.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1344 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_mxn_infodolar.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1078 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_mxn_intercam.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1125 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_mxn_themoneyconverter.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      806 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_mxn_wise.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1223 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_mxn_xrates.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usdt_usd_bitstamp.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usdt_usd_coinbase.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      584 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usdt_usd_kraken.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      718 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/my_logging.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     5783 2024-05-08 15:02:48.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/server.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     6008 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/to_db.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)        8 2024-05-08 14:11:45.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/version.txt
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     5014 2024-04-25 21:01:28.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source/weighing.py
+-rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)      117 2024-04-29 13:56:07.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source_api
+-rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)      118 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source_check
+-rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)      128 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.7.0b2/moc_prices_source_to_db
+drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2024-05-08 15:11:13.972430 moneyonchain_prices_source-0.7.0b2/moneyonchain_prices_source.egg-info/
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4743 2024-05-08 15:11:12.000000 moneyonchain_prices_source-0.7.0b2/moneyonchain_prices_source.egg-info/PKG-INFO
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     5178 2024-05-08 15:11:13.000000 moneyonchain_prices_source-0.7.0b2/moneyonchain_prices_source.egg-info/SOURCES.txt
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)        1 2024-05-08 15:11:12.000000 moneyonchain_prices_source-0.7.0b2/moneyonchain_prices_source.egg-info/dependency_links.txt
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      146 2024-05-08 15:11:12.000000 moneyonchain_prices_source-0.7.0b2/moneyonchain_prices_source.egg-info/requires.txt
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       18 2024-05-08 15:11:12.000000 moneyonchain_prices_source-0.7.0b2/moneyonchain_prices_source.egg-info/top_level.txt
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       38 2024-05-08 15:11:13.972430 moneyonchain_prices_source-0.7.0b2/setup.cfg
+-rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)     1863 2024-04-29 14:33:12.000000 moneyonchain_prices_source-0.7.0b2/setup.py
```

### Comparing `moneyonchain_prices_source-0.7.0b1/PKG-INFO` & `moneyonchain_prices_source-0.7.0b2/moneyonchain_prices_source.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: moneyonchain_prices_source
-Version: 0.7.0b1
+Name: moneyonchain-prices-source
+Version: 0.7.0b2
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
         
-        More [usage examples](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b1/docs/examples.md) can be seen [here](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b1/docs/examples.md)
+        More [usage examples](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b2/docs/examples.md) can be seen [here](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b2/docs/examples.md)
         
         
         
         ## How the included CLI tool looks like
         
         Here you can see how the output of the `moc_prices_source_check` command looks like
         
@@ -61,21 +61,21 @@
         
         Response time 1.1s
         
         user@host:~$ 
         ```
         
         This command has many options. you can run `moc_prices_source_check --help` to get help on how to run them.
-        More information about this CLI tool can be seen [here](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b1/docs/cli.md).
+        More information about this CLI tool can be seen [here](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b2/docs/cli.md).
         
         
         
         ## References
         
-        * [Source code in Github](https://github.com/money-on-chain/moc_prices_source/tree/v0.7.0b1)
+        * [Source code in Github](https://github.com/money-on-chain/moc_prices_source/tree/v0.7.0b2)
         * [Package from Python package index (PyPI)](https://pypi.org/project/moneyonchain-prices-source)
         
         
         
         ## Requirements
         
         * Python 3.6+ support
@@ -98,15 +98,15 @@
         $ moc_prices_source_check --version
         ```
         
         To verify that it has been installed correctly
         
         ### From source
         
-        Download from [Github](https://github.com/money-on-chain/moc_prices_source/tree/v0.7.0b1)
+        Download from [Github](https://github.com/money-on-chain/moc_prices_source/tree/v0.7.0b2)
         
         Standing inside the folder, run:
         
         ```shell
         $ pip3 install -r requirements.txt 
         ```
         
@@ -124,15 +124,15 @@
         
         To verify that it has been installed correctly
         
         
         
         ## Supported coinpairs and symbols
         
-        [Here](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b1/docs/supported_coinpairs.md) you can find an [summary of supported coinpairs and symbols](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b1/docs/supported_coinpairs.md)
+        [Here](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b2/docs/supported_coinpairs.md) you can find an [summary of supported coinpairs and symbols](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b2/docs/supported_coinpairs.md)
         
         
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
```

### Comparing `moneyonchain_prices_source-0.7.0b1/README.md` & `moneyonchain_prices_source-0.7.0b2/README.md`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/__init__.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/__init__.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/cli_check.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/cli_check.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/coins.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/coins.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/computed_pairs.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/computed_pairs.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/conf.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/conf.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/data/weighing.json` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/data/weighing.json`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/database.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/database.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/__init__.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/bnb_usdt_binance.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/bnb_usdt_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_ars_argenbtc.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_ars_argenbtc.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_ars_belo_app.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_ars_belo_app.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_ars_binance.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_ars_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_ars_bitso.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_ars_bitso.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_ars_buda.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_ars_buda.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_ars_buenbit.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_ars_buenbit.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_ars_coinbase.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_ars_coinbase.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_ars_cryptomkt.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_ars_cryptomkt.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_ars_decrypto.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_ars_decrypto.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_ars_lemoncash.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_ars_lemoncash.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_ars_ripio.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_ars_ripio.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_ars_ripio_exch.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_ars_ripio_exch.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_ars_rofex.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_ars_rofex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_ars_satoshitango.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_ars_satoshitango.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_cop_bitso.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_cop_bitso.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_cop_buda.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_cop_buda.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_cop_buenbit.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_cop_buenbit.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_cop_coinbase.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_cop_coinbase.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_cop_cryptomkt.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_cop_cryptomkt.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_usd_bitfinex.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_usd_bitfinex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_usd_bitgo.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_usd_bitgo.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_usd_bitstamp.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_usd_bitstamp.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_usd_bittrex.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_usd_bittrex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_usd_cex.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_usd_cex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_usd_coinbase.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_usd_coinbase.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_usd_itbit.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_usd_itbit.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_usd_kraken.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_usd_kraken.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_usd_kucoin.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_usd_kucoin.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_usd_okcoin.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_usd_okcoin.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_usdt_binance.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_usdt_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_usdt_bitfinex.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_usdt_bitfinex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_usdt_coinbase.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_usdt_coinbase.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/btc_usdt_kraken.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/btc_usdt_kraken.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/coins.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/coins.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/engine_base.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/engine_base.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/eth_btc_binance.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/eth_btc_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/eth_btc_bitfinex.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/eth_btc_bitfinex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/eth_btc_bitstamp.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/eth_btc_bitstamp.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/eth_btc_kraken.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/eth_btc_kraken.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/gas_btc_rsk.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/gas_btc_rsk.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/moc_btc_sovryn.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/moc_btc_sovryn.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/rif_btc_binance.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/rif_btc_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/rif_btc_bitfinex.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/rif_btc_bitfinex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/rif_btc_coinbene.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/rif_btc_coinbene.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/rif_btc_coingecko.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/rif_btc_coingecko.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/rif_btc_kucoin.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/rif_btc_kucoin.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/rif_btc_mexc.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/rif_btc_mexc.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/rif_btc_mp1p_binance.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/rif_btc_mp1p_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/rif_btc_mxc.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/rif_btc_mxc.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/rif_btc_sovryn.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/rif_btc_sovryn.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/rif_usdt_binance.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/rif_usdt_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/rif_usdt_ma2_binance.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/rif_usdt_ma2_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/rif_usdt_ma3_binance.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/rif_usdt_ma3_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/rif_usdt_ma_binance.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/rif_usdt_ma_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/rif_usdt_mp1p_binance.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/rif_usdt_mp1p_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_ars_ambito.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_ars_ambito.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_ars_ccl_ambito.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_ars_ccl_ambito.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_ars_ccl_coinmonitor.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_ars_ccl_coinmonitor.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_ars_ccl_criptoya.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_ars_ccl_criptoya.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_ars_ccl_cronista.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_ars_ccl_cronista.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_ars_ccl_dolarhoy.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_ars_ccl_dolarhoy.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_ars_ccl_dolarsi.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_ars_ccl_dolarsi.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_ars_ccl_infobae.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_ars_ccl_infobae.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_ars_ccl_infodolar.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_ars_ccl_infodolar.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_ars_ccl_lanacion.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_ars_ccl_lanacion.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_ars_ccl_rofex.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_ars_ccl_rofex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_ars_coinmonitor.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_ars_coinmonitor.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_ars_criptoya.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_ars_criptoya.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_ars_cronista.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_ars_cronista.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_ars_dolarhoy.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_ars_dolarhoy.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_ars_dolarsi.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_ars_dolarsi.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_ars_infobae.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_ars_infobae.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_ars_infodolar.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_ars_infodolar.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_ars_lanacion.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_ars_lanacion.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_cop_banrep.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_cop_banrep.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_cop_dolarhoy.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_cop_dolarhoy.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_mxn_bitso.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_mxn_bitso.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_mxn_citibanamex.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_mxn_citibanamex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_mxn_coinmonitor.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_mxn_coinmonitor.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_mxn_currencymeuk.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_mxn_currencymeuk.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_mxn_eldolar_info.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_mxn_eldolar_info.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_mxn_eleconomista.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_mxn_eleconomista.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_mxn_infodolar.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_mxn_infodolar.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_mxn_intercam.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_mxn_intercam.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_mxn_themoneyconverter.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_mxn_themoneyconverter.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_mxn_wise.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_mxn_wise.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usd_mxn_xrates.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usd_mxn_xrates.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usdt_usd_bitstamp.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usdt_usd_bitstamp.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usdt_usd_coinbase.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usdt_usd_coinbase.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/engines/usdt_usd_kraken.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/engines/usdt_usd_kraken.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/my_logging.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/my_logging.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/server.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/server.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,29 +47,35 @@
 
 cache = Cache(config={'CACHE_TYPE': 'SimpleCache'})
 cache.init_app(app)
 
 
 class HashMethod():
 
-    def __init__(self, *options) -> None:
+    def __init__(self, *options, info=lambda x: None, pre="") -> None:
+        self._pre = pre
+        self.info = info
         self.options = list(map(lambda x: str(x).strip().lower(), list(options)))
         self.out = []
 
     def __call__(self, x) -> None:
         self.out = []
         for key, value in eval(x):
             key=str(key).strip().lower()
             if key in self.options:
                 value=str(value).strip().lower()
                 self.out.append((key, value))
         return self
 
     def hexdigest(self):
-        return repr(self.out) if self.out else ""
+        hash_ = repr(self.out) if self.out else ""
+        if self._pre:
+            hash_ = f"{self._pre}{hash_}"
+        self.info(f"hash = {repr(hash_)}")
+        return hash_
 
 
 api = Api(
     app,
     prefix='/api',
     doc='/api/doc',
     version=f"v{version}",
@@ -142,15 +148,23 @@
 @coinpairs_ns.route('/get_value')
 @coinpairs_ns.response(200, 'Success!')
 @coinpairs_ns.response(*bad_coinpair_choice)
 @coinpairs_ns.response(*coinpair_value_not_found)
 class CoinPairValue(Resource):
 
     @coinpairs_ns.expect(coinpair_value_get)
-    @cache.cached(timeout=5, query_string=True, hash_method=HashMethod('format', 'simple_format'))
+    @cache.cached(
+        timeout=5,
+        query_string=True,
+        hash_method=HashMethod(
+            'coinpair',
+            pre="get_coinpair_value",
+            #info=lambda x: app.logger.info(f"Cache: {x}")
+        )
+    )
     def get(self):
         """Get the price of a specific coinpair"""
 
         args = coinpair_value_get.parse_args()
         coinpair = args['coinpair']
 
         if coinpair not in all_coinpairs:
```

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/to_db.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/to_db.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moc_prices_source/weighing.py` & `moneyonchain_prices_source-0.7.0b2/moc_prices_source/weighing.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/moneyonchain_prices_source.egg-info/PKG-INFO` & `moneyonchain_prices_source-0.7.0b2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: moneyonchain-prices-source
-Version: 0.7.0b1
+Name: moneyonchain_prices_source
+Version: 0.7.0b2
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
         
-        More [usage examples](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b1/docs/examples.md) can be seen [here](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b1/docs/examples.md)
+        More [usage examples](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b2/docs/examples.md) can be seen [here](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b2/docs/examples.md)
         
         
         
         ## How the included CLI tool looks like
         
         Here you can see how the output of the `moc_prices_source_check` command looks like
         
@@ -61,21 +61,21 @@
         
         Response time 1.1s
         
         user@host:~$ 
         ```
         
         This command has many options. you can run `moc_prices_source_check --help` to get help on how to run them.
-        More information about this CLI tool can be seen [here](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b1/docs/cli.md).
+        More information about this CLI tool can be seen [here](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b2/docs/cli.md).
         
         
         
         ## References
         
-        * [Source code in Github](https://github.com/money-on-chain/moc_prices_source/tree/v0.7.0b1)
+        * [Source code in Github](https://github.com/money-on-chain/moc_prices_source/tree/v0.7.0b2)
         * [Package from Python package index (PyPI)](https://pypi.org/project/moneyonchain-prices-source)
         
         
         
         ## Requirements
         
         * Python 3.6+ support
@@ -98,15 +98,15 @@
         $ moc_prices_source_check --version
         ```
         
         To verify that it has been installed correctly
         
         ### From source
         
-        Download from [Github](https://github.com/money-on-chain/moc_prices_source/tree/v0.7.0b1)
+        Download from [Github](https://github.com/money-on-chain/moc_prices_source/tree/v0.7.0b2)
         
         Standing inside the folder, run:
         
         ```shell
         $ pip3 install -r requirements.txt 
         ```
         
@@ -124,15 +124,15 @@
         
         To verify that it has been installed correctly
         
         
         
         ## Supported coinpairs and symbols
         
-        [Here](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b1/docs/supported_coinpairs.md) you can find an [summary of supported coinpairs and symbols](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b1/docs/supported_coinpairs.md)
+        [Here](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b2/docs/supported_coinpairs.md) you can find an [summary of supported coinpairs and symbols](https://github.com/money-on-chain/moc_prices_source/blob/v0.7.0b2/docs/supported_coinpairs.md)
         
         
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
```

### Comparing `moneyonchain_prices_source-0.7.0b1/moneyonchain_prices_source.egg-info/SOURCES.txt` & `moneyonchain_prices_source-0.7.0b2/moneyonchain_prices_source.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.7.0b1/setup.py` & `moneyonchain_prices_source-0.7.0b2/setup.py`

 * *Files identical despite different names*

