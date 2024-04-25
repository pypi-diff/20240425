# Comparing `tmp/ccxt-4.3.7.tar.gz` & `tmp/ccxt-4.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ccxt-4.3.7.tar", last modified: Wed Apr 24 16:50:04 2024, max compression
+gzip compressed data, was "dist/ccxt-4.3.8.tar", last modified: Thu Apr 25 18:16:36 2024, max compression
```

## Comparing `ccxt-4.3.7.tar` & `ccxt-4.3.8.tar`

### file list

```diff
@@ -1,572 +1,572 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-24 16:50:04.688356 ccxt-4.3.7/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1068 2024-04-24 16:45:27.000000 ccxt-4.3.7/LICENSE.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      101 2024-04-24 15:13:10.000000 ccxt-4.3.7/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)   115320 2024-04-24 16:50:04.692356 ccxt-4.3.7/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)   102253 2024-04-24 15:13:10.000000 ccxt-4.3.7/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-24 16:50:04.064311 ccxt-4.3.7/ccxt/
--rw-rw-r--   0 travis    (2000) travis    (2000)    15655 2024-04-24 16:45:23.000000 ccxt-4.3.7/ccxt/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-24 16:50:04.204321 ccxt-4.3.7/ccxt/abstract/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/abstract/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1448 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/ace.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10382 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/alpaca.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11394 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/ascendex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15601 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/bequant.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4895 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/bigone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    92016 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/binance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    92016 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/binancecoinm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    98736 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/binanceus.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    92016 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/binanceusdm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16041 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/bingx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2830 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/bit2c.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2735 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/bitbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5820 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/bitbay.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4082 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/bitbns.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15601 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/bitcoincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7605 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/bitfinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19194 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/bitfinex2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3576 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/bitflyer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    89841 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/bitget.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3443 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/bithumb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14031 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/bitmart.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10774 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/bitmex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3295 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/bitopro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3859 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/bitpanda.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9379 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/bitrue.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4025 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/bitso.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27930 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/bitstamp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3478 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/bitteam.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2357 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/bitvavo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2024 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/bl3p.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2638 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/blockchaincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3978 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/blofin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1380 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/btcalpha.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      849 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/btcbox.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3690 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/btcmarkets.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1777 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/btcturk.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    48599 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/bybit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3311 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/cex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15507 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/coinbase.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4770 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/coinbaseinternational.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7162 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/coinbasepro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3417 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/coincheck.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34678 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/coinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6538 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/coinlist.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6842 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/coinmate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3864 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/coinmetro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8291 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/coinone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8007 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/coinsph.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2707 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/coinspot.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18475 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/cryptocom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7563 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/currencycom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5107 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/delta.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15499 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/deribit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11452 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/digifinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6177 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/exmo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15601 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/fmfwio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41994 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/gate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41994 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/gateio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6915 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/gemini.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15601 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/hitbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15601 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/hitbtc3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2906 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/hollaex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    99311 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/htx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    99311 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/huobi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14331 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/huobijp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      240 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/hyperliquid.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2129 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/idex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4165 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/independentreserve.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2488 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/indodax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5877 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/kraken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3537 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/krakenfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25491 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/kucoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27937 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/kucoinfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24579 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/kuna.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7168 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/latoken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8675 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/lbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3373 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/luno.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2960 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/lykke.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2357 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/mercado.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25902 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/mexc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11878 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/ndax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3093 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/novadax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1721 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/oceanex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9414 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/okcoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    45891 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/okx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3859 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/onetrading.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2054 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/p2b.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2843 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/paymium.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15203 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/phemex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8073 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/poloniex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5219 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/poloniexfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1969 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/probit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5875 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/timex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4094 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/tokocrypto.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1372 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/tradeogre.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3576 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/upbit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19631 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/wavesexchange.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2782 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/wazirx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10977 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/whitebit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10368 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/woo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1339 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/yobit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3935 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/zaif.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5820 2024-04-24 15:15:11.000000 ccxt-4.3.7/ccxt/abstract/zonda.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41650 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/ace.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    47182 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/alpaca.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   151398 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/ascendex.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-24 16:50:04.396335 ccxt-4.3.7/ccxt/async_support/
--rw-rw-r--   0 travis    (2000) travis    (2000)    15408 2024-04-24 16:45:23.000000 ccxt-4.3.7/ccxt/async_support/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41874 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/ace.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    47394 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/alpaca.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   152186 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/ascendex.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-24 16:50:04.408336 ccxt-4.3.7/ccxt/async_support/base/
--rw-rw-r--   0 travis    (2000) travis    (2000)       67 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/base/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   107190 2024-04-24 16:45:23.000000 ccxt-4.3.7/ccxt/async_support/base/exchange.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1847 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/base/throttler.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-24 16:50:04.416336 ccxt-4.3.7/ccxt/async_support/base/ws/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1791 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/base/ws/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5751 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/base/ws/aiohttp_client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8100 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/base/ws/cache.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7289 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/base/ws/client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3864 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/base/ws/fast_client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1499 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/base/ws/functions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2067 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/base/ws/future.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2894 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/base/ws/order_book.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6478 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/base/ws/order_book_side.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1188 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/bequant.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    92644 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/bigone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   614233 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/binance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1683 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/binancecoinm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9177 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/binanceus.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2518 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/binanceusdm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   185217 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/bingx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37113 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/bit2c.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42099 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/bitbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      492 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/bitbay.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    48385 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/bitbns.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      516 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/bitcoincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    71973 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/bitfinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   158868 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/bitfinex2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41699 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/bitflyer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   423781 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/bitget.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    45758 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/bithumb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   200028 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/bitmart.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   126994 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/bitmex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    68920 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/bitopro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      485 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/bitpanda.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   136836 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/bitrue.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    71265 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/bitso.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    92765 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/bitstamp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   102352 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/bitteam.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    92005 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/bitvavo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20605 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/bl3p.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    49185 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/blockchaincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    99698 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/blofin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36973 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/btcalpha.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23680 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/btcbox.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    51828 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/btcmarkets.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36869 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/btcturk.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   411940 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/bybit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    70274 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/cex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   207970 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/coinbase.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    87777 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/coinbaseinternational.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    79171 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/coinbasepro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35864 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/coincheck.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   250239 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/coinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   103683 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/coinlist.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    46206 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/coinmate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    80729 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/coinmetro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    47132 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/coinone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    91060 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/coinsph.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23760 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/coinspot.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   130350 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/cryptocom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    87181 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/currencycom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   151059 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/delta.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   161229 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/deribit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   168860 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/digifinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   115075 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/exmo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1183 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/flowbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1250 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/fmfwio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   321438 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/gate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      459 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/gateio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    81132 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/gemini.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   153964 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/hitbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      469 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/hitbtc3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    76332 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/hollaex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   422776 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/htx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      452 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/huobi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    88462 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/huobijp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   100190 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/hyperliquid.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    73435 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/idex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    32429 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/independentreserve.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    52237 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/indodax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   125943 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/kraken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   117245 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/krakenfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   218785 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/kucoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   119225 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/kucoinfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    96401 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/kuna.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    79527 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/latoken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   115881 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/lbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    46126 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/luno.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    51378 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/lykke.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35575 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/mercado.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   241987 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/mexc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   109086 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/ndax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    64667 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/novadax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    38180 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/oceanex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   151634 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/okcoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   372435 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/okx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    88559 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/onetrading.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    54455 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/p2b.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24391 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/paymium.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   219623 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/phemex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   102501 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/poloniex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    78194 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/poloniexfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    76750 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/probit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    71643 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/timex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   123369 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/tokocrypto.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24094 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/tradeogre.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    82087 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/upbit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   114100 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/wavesexchange.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    51638 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/wazirx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   108793 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/whitebit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   139434 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/woo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    53500 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/yobit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    28139 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/zaif.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    80871 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/async_support/zonda.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-24 16:50:04.416336 ccxt-4.3.7/ccxt/base/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1320 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/base/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6634 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/base/decimal_to_precision.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4107 2024-04-24 15:28:33.000000 ccxt-4.3.7/ccxt/base/errors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   274740 2024-04-24 16:45:23.000000 ccxt-4.3.7/ccxt/base/exchange.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8565 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/base/precise.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7992 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/base/types.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1174 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/bequant.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    92190 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/bigone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   611565 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/binance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1645 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/binancecoinm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9163 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/binanceus.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2480 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/binanceusdm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   184181 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/bingx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36901 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/bit2c.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41839 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/bitbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      478 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/bitbay.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    48131 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/bitbns.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      502 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/bitcoincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    71533 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/bitfinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   158134 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/bitfinex2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41391 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/bitflyer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   422157 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/bitget.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    45528 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/bithumb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   199108 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/bitmart.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   126416 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/bitmex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    68516 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/bitopro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      471 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/bitpanda.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   136178 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/bitrue.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    70879 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/bitso.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    92265 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/bitstamp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   102020 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/bitteam.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    91571 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/bitvavo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20477 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/bl3p.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    48793 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/blockchaincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    99114 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/blofin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36695 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/btcalpha.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23486 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/btcbox.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    51478 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/btcmarkets.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36651 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/btcturk.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   410160 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/bybit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    69924 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/cex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   206918 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/coinbase.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    87223 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/coinbaseinternational.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    78665 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/coinbasepro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35658 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/coincheck.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   248951 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/coinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   103195 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/coinlist.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    45940 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/coinmate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    80409 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/coinmetro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    46890 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/coinone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    90626 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/coinsph.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23608 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/coinspot.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   129778 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/cryptocom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    86759 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/currencycom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   150451 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/delta.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   160453 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/deribit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   167890 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/digifinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   114443 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/exmo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1169 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/flowbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1236 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/fmfwio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   319760 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/gate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      445 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/gateio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    80619 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/gemini.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   152918 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/hitbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      455 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/hitbtc3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    75898 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/hollaex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   420420 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/htx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      438 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/huobi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    87962 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/huobijp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    99670 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/hyperliquid.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    72959 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/idex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    32169 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/independentreserve.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    51929 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/indodax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   125341 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/kraken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   116757 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/krakenfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   217713 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/kucoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   118623 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/kucoinfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    95985 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/kuna.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    79051 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/latoken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   115169 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/lbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    45788 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/luno.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    51064 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/lykke.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35333 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/mercado.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   240809 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/mexc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   108562 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/ndax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    64299 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/novadax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37860 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/oceanex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   151110 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/okcoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   370860 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/okx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    88107 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/onetrading.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    54213 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/p2b.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24203 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/paymium.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   218811 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/phemex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   101953 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/poloniex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    77808 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/poloniexfutures.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-24 16:50:04.528344 ccxt-4.3.7/ccxt/pro/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6998 2024-04-24 16:45:23.000000 ccxt-4.3.7/ccxt/pro/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27167 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/alpaca.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35432 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/ascendex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1351 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/bequant.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   152488 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/binance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      976 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/binancecoinm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2321 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/binanceus.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1357 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/binanceusdm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42110 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/bingx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1181 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/bitcoincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24826 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/bitfinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42744 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/bitfinex2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    71843 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/bitget.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16799 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/bithumb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    62382 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/bitmart.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    68956 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/bitmex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18724 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/bitopro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      415 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/bitpanda.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16448 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/bitrue.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20886 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/bitstamp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    56143 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/bitvavo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29560 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/blockchaincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    75022 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/bybit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    58380 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/cex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25807 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/coinbase.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25428 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/coinbaseinternational.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    38945 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/coinbasepro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7789 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/coincheck.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    45042 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/coinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15652 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/coinone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42643 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/cryptocom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22355 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/currencycom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41035 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/deribit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24527 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/exmo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    52489 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/gate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      391 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/gateio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36641 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/gemini.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    56285 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/hitbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21957 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/hollaex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    95779 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/htx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      385 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/huobi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23174 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/huobijp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20791 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/hyperliquid.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    28282 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/idex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11063 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/independentreserve.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    60658 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/kraken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    63917 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/krakenfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    50705 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/kucoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    46006 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/kucoinfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35105 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/lbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12348 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/luno.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42551 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/mexc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22643 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/ndax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    30385 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/okcoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    68821 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/okx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    54634 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/onetrading.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17877 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/p2b.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    61032 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/phemex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    51236 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/poloniex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41652 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/poloniexfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22822 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/probit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9654 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/upbit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    30043 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/wazirx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35021 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/whitebit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36988 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/pro/woo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    76358 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/probit.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-24 16:50:04.532345 ccxt-4.3.7/ccxt/static_dependencies/
--rw-rw-r--   0 travis    (2000) travis    (2000)       84 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-24 16:50:04.544346 ccxt-4.3.7/ccxt/static_dependencies/ecdsa/
--rw-rw-r--   0 travis    (2000) travis    (2000)      594 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ecdsa/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18461 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ecdsa/_version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1886 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ecdsa/curves.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6942 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ecdsa/der.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11336 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ecdsa/ecdsa.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5517 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ecdsa/ellipticcurve.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14201 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ecdsa/keys.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13468 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ecdsa/numbertheory.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2572 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ecdsa/rfc6979.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10037 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ecdsa/util.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-24 16:50:04.544346 ccxt-4.3.7/ccxt/static_dependencies/ethereum/
--rw-rw-r--   0 travis    (2000) travis    (2000)      171 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-24 16:50:04.560347 ccxt-4.3.7/ccxt/static_dependencies/ethereum/abi/
--rw-rw-r--   0 travis    (2000) travis    (2000)      276 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/abi/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      490 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/abi/abi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4861 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/abi/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6871 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/abi/codec.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       51 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/abi/constants.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16828 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/abi/decoding.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20162 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/abi/encoding.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2941 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/abi/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12358 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/abi/grammar.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      387 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/abi/packed.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/abi/py.typed
--rw-rw-r--   0 travis    (2000) travis    (2000)    19329 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/abi/registry.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-24 16:50:04.564347 ccxt-4.3.7/ccxt/static_dependencies/ethereum/abi/tools/
--rw-rw-r--   0 travis    (2000) travis    (2000)       65 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/abi/tools/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5742 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/abi/tools/_strategies.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-24 16:50:04.568347 ccxt-4.3.7/ccxt/static_dependencies/ethereum/abi/utils/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/abi/utils/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2097 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/abi/utils/numeric.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      426 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/abi/utils/padding.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      436 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/abi/utils/string.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-24 16:50:04.572347 ccxt-4.3.7/ccxt/static_dependencies/ethereum/account/
--rw-rw-r--   0 travis    (2000) travis    (2000)       48 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/account/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-24 16:50:04.572347 ccxt-4.3.7/ccxt/static_dependencies/ethereum/account/encode_typed_data/
--rw-rw-r--   0 travis    (2000) travis    (2000)       80 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/account/encode_typed_data/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7126 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/account/encode_typed_data/encoding_and_hashing.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      982 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/account/encode_typed_data/helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10588 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/account/messages.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/account/py.typed
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-24 16:50:04.576348 ccxt-4.3.7/ccxt/static_dependencies/ethereum/hexbytes/
--rw-rw-r--   0 travis    (2000) travis    (2000)       60 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/hexbytes/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1687 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/hexbytes/_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1768 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/hexbytes/main.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/hexbytes/py.typed
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-24 16:50:04.584349 ccxt-4.3.7/ccxt/static_dependencies/ethereum/typing/
--rw-rw-r--   0 travis    (2000) travis    (2000)      913 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/typing/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       85 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/typing/abi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      191 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/typing/bls.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       71 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/typing/discovery.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      117 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/typing/encoding.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      458 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/typing/enums.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      173 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/typing/ethpm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      546 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/typing/evm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20845 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/typing/networks.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/typing/py.typed
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-24 16:50:04.604350 ccxt-4.3.7/ccxt/static_dependencies/ethereum/utils/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2162 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/utils/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2123 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/utils/abi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4364 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/utils/address.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4342 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/utils/applicators.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5498 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/utils/conversions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3021 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/utils/currency.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-24 16:50:04.604350 ccxt-4.3.7/ccxt/static_dependencies/ethereum/utils/curried/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6398 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/utils/curried/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      499 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/utils/debug.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3997 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/utils/decorators.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      199 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/utils/encoding.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      110 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/utils/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2100 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/utils/functional.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1826 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/utils/hexadecimal.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4137 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/utils/humanize.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5155 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/utils/logging.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      842 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/utils/module_loading.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1190 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/utils/numeric.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/utils/py.typed
--rw-rw-r--   0 travis    (2000) travis    (2000)     1001 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/utils/toolz.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1074 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/utils/types.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-24 16:50:04.620351 ccxt-4.3.7/ccxt/static_dependencies/ethereum/utils/typing/
--rw-rw-r--   0 travis    (2000) travis    (2000)      325 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/utils/typing/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      189 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/utils/typing/misc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1757 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/ethereum/utils/units.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-24 16:50:04.624351 ccxt-4.3.7/ccxt/static_dependencies/keccak/
--rw-rw-r--   0 travis    (2000) travis    (2000)       45 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/keccak/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6934 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/keccak/keccak.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-24 16:50:04.628352 ccxt-4.3.7/ccxt/static_dependencies/msgpack/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1077 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/msgpack/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1081 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/msgpack/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5629 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/msgpack/ext.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    33175 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/msgpack/fallback.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-24 16:50:04.636352 ccxt-4.3.7/ccxt/static_dependencies/parsimonious/
--rw-rw-r--   0 travis    (2000) travis    (2000)      385 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/parsimonious/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3603 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/parsimonious/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16864 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/parsimonious/expressions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19190 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/parsimonious/grammar.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13084 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/parsimonious/nodes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1087 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/parsimonious/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-24 16:50:04.644353 ccxt-4.3.7/ccxt/static_dependencies/toolz/
--rw-rw-r--   0 travis    (2000) travis    (2000)      374 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/toolz/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20555 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/toolz/_signatures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18447 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/toolz/_version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      997 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/toolz/compatibility.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-24 16:50:04.644353 ccxt-4.3.7/ccxt/static_dependencies/toolz/curried/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2226 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/toolz/curried/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      344 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/toolz/curried/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      525 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/toolz/curried/operator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8955 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/toolz/dicttoolz.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29821 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/toolz/functoolz.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27612 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/toolz/itertoolz.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1256 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/toolz/recipes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      139 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/static_dependencies/toolz/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-24 16:50:04.648353 ccxt-4.3.7/ccxt/test/
--rw-rw-r--   0 travis    (2000) travis    (2000)      141 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/test/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-24 16:50:04.684356 ccxt-4.3.7/ccxt/test/base/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1889 2024-04-24 15:28:38.000000 ccxt-4.3.7/ccxt/test/base/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      978 2024-04-24 15:30:02.000000 ccxt-4.3.7/ccxt/test/base/test_account.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2931 2024-04-24 15:30:02.000000 ccxt-4.3.7/ccxt/test/base/test_balance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1808 2024-04-24 15:30:02.000000 ccxt-4.3.7/ccxt/test/base/test_borrow_interest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1500 2024-04-24 15:30:02.000000 ccxt-4.3.7/ccxt/test/base/test_borrow_rate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1177 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/test/base/test_calculate_fee.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7702 2024-04-24 15:28:35.000000 ccxt-4.3.7/ccxt/test/base/test_crypto.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4472 2024-04-24 15:30:02.000000 ccxt-4.3.7/ccxt/test/base/test_currency.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5235 2024-04-24 15:28:34.000000 ccxt-4.3.7/ccxt/test/base/test_datetime.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20934 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/test/base/test_decimal_to_precision.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1402 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/test/base/test_deep_extend.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2452 2024-04-24 15:30:02.000000 ccxt-4.3.7/ccxt/test/base/test_deposit_withdrawal.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3592 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/test/base/test_exchange_datetime_functions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1351 2024-04-24 15:30:02.000000 ccxt-4.3.7/ccxt/test/base/test_funding_rate_history.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1332 2024-04-24 15:30:02.000000 ccxt-4.3.7/ccxt/test/base/test_last_price.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2283 2024-04-24 15:30:02.000000 ccxt-4.3.7/ccxt/test/base/test_ledger_entry.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2154 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/test/base/test_ledger_item.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1656 2024-04-24 15:30:02.000000 ccxt-4.3.7/ccxt/test/base/test_leverage_tier.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      869 2024-04-24 15:30:02.000000 ccxt-4.3.7/ccxt/test/base/test_margin_mode.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1730 2024-04-24 15:30:02.000000 ccxt-4.3.7/ccxt/test/base/test_margin_modification.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11632 2024-04-24 15:30:02.000000 ccxt-4.3.7/ccxt/test/base/test_market.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22083 2024-04-24 15:28:34.000000 ccxt-4.3.7/ccxt/test/base/test_number.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2036 2024-04-24 15:30:02.000000 ccxt-4.3.7/ccxt/test/base/test_ohlcv.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1547 2024-04-24 15:30:02.000000 ccxt-4.3.7/ccxt/test/base/test_open_interest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3964 2024-04-24 15:30:02.000000 ccxt-4.3.7/ccxt/test/base/test_order.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3949 2024-04-24 15:30:02.000000 ccxt-4.3.7/ccxt/test/base/test_order_book.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3884 2024-04-24 15:30:02.000000 ccxt-4.3.7/ccxt/test/base/test_position.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19998 2024-04-24 15:30:02.000000 ccxt-4.3.7/ccxt/test/base/test_shared_methods.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      722 2024-04-24 15:30:02.000000 ccxt-4.3.7/ccxt/test/base/test_status.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3123 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/test/base/test_throttle.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5810 2024-04-24 15:30:02.000000 ccxt-4.3.7/ccxt/test/base/test_ticker.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2336 2024-04-24 15:30:03.000000 ccxt-4.3.7/ccxt/test/base/test_trade.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1066 2024-04-24 15:30:03.000000 ccxt-4.3.7/ccxt/test/base/test_trading_fee.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1434 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/test/base/test_transaction.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    78755 2024-04-24 15:28:38.000000 ccxt-4.3.7/ccxt/test/test_async.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    77736 2024-04-24 15:28:38.000000 ccxt-4.3.7/ccxt/test/test_sync.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    71281 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/timex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   123007 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/tokocrypto.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23900 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/tradeogre.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    81605 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/upbit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   113550 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/wavesexchange.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    51336 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/wazirx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   108191 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/whitebit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   138544 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/woo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    53216 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/yobit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27957 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/zaif.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    80557 2024-04-24 15:13:10.000000 ccxt-4.3.7/ccxt/zonda.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-24 16:50:04.064311 ccxt-4.3.7/ccxt.egg-info/
--rw-r--r--   0 travis    (2000) travis    (2000)   115320 2024-04-24 16:50:03.000000 ccxt-4.3.7/ccxt.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    15741 2024-04-24 16:50:03.000000 ccxt-4.3.7/ccxt.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-24 16:50:03.000000 ccxt-4.3.7/ccxt.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      218 2024-04-24 16:50:03.000000 ccxt-4.3.7/ccxt.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        5 2024-04-24 16:50:03.000000 ccxt-4.3.7/ccxt.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    12555 2024-04-24 16:45:26.000000 ccxt-4.3.7/package.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      205 2024-04-24 16:50:04.700357 ccxt-4.3.7/setup.cfg
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3071 2024-04-24 15:13:10.000000 ccxt-4.3.7/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.711214 ccxt-4.3.8/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1068 2024-04-25 18:11:51.000000 ccxt-4.3.8/LICENSE.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      101 2024-04-25 16:48:28.000000 ccxt-4.3.8/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)   115320 2024-04-25 18:16:36.719215 ccxt-4.3.8/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)   102253 2024-04-25 16:48:28.000000 ccxt-4.3.8/README.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.063167 ccxt-4.3.8/ccxt/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15655 2024-04-25 18:11:47.000000 ccxt-4.3.8/ccxt/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.179175 ccxt-4.3.8/ccxt/abstract/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/abstract/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1448 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/ace.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10382 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/alpaca.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11394 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/ascendex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15601 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/bequant.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4895 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/bigone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    92016 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/binance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    92016 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/binancecoinm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    98736 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/binanceus.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    92016 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/binanceusdm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16041 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/bingx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2830 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/bit2c.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2735 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/bitbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5820 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/bitbay.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4082 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/bitbns.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15601 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/bitcoincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7605 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/bitfinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19194 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/bitfinex2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3576 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/bitflyer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    89841 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/bitget.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3443 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/bithumb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14031 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/bitmart.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10774 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/bitmex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3295 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/bitopro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3859 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/bitpanda.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9379 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/bitrue.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4025 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/bitso.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27930 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/bitstamp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3478 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/bitteam.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2357 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/bitvavo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2024 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/bl3p.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2638 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/blockchaincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3978 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/blofin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1380 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/btcalpha.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      849 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/btcbox.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3690 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/btcmarkets.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1777 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/btcturk.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48599 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/bybit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3311 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/cex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15507 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/coinbase.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4770 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/coinbaseinternational.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7162 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/coinbasepro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3417 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/coincheck.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34678 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/coinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6538 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/coinlist.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6842 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/coinmate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3864 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/coinmetro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8291 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/coinone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8007 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/coinsph.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2707 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/coinspot.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18475 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/cryptocom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7563 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/currencycom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5107 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/delta.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15499 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/deribit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11452 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/digifinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6177 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/exmo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15601 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/fmfwio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41994 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/gate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41994 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/gateio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6915 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/gemini.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15601 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/hitbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15601 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/hitbtc3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2906 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/hollaex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    99311 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/htx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    99311 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/huobi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14331 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/huobijp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      240 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/hyperliquid.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2129 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/idex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4165 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/independentreserve.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2488 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/indodax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5877 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/kraken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3537 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/krakenfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25491 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/kucoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27937 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/kucoinfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24579 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/kuna.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7168 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/latoken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8675 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/lbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3373 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/luno.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2960 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/lykke.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2357 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/mercado.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25902 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/mexc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11878 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/ndax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3093 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/novadax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1721 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/oceanex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9414 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/okcoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45891 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/okx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3859 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/onetrading.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2054 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/p2b.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2843 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/paymium.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15203 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/phemex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8073 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/poloniex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5219 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/poloniexfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1969 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/probit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5875 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/timex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4094 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/tokocrypto.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1372 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/tradeogre.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3576 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/upbit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19631 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/wavesexchange.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2782 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/wazirx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10977 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/whitebit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10368 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/woo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1339 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/yobit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3935 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/zaif.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5820 2024-04-25 16:50:23.000000 ccxt-4.3.8/ccxt/abstract/zonda.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41650 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/ace.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    47182 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/alpaca.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   151398 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/ascendex.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.439194 ccxt-4.3.8/ccxt/async_support/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15408 2024-04-25 18:11:47.000000 ccxt-4.3.8/ccxt/async_support/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41874 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/ace.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    47394 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/alpaca.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   152186 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/ascendex.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.443194 ccxt-4.3.8/ccxt/async_support/base/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       67 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/base/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   107190 2024-04-25 18:11:47.000000 ccxt-4.3.8/ccxt/async_support/base/exchange.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1847 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/base/throttler.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.455195 ccxt-4.3.8/ccxt/async_support/base/ws/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1791 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/base/ws/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5751 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/base/ws/aiohttp_client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8100 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/base/ws/cache.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7289 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/base/ws/client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3864 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/base/ws/fast_client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1499 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/base/ws/functions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2067 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/base/ws/future.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2894 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/base/ws/order_book.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6478 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/base/ws/order_book_side.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1188 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/bequant.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    92644 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/bigone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   614239 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/binance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1683 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/binancecoinm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9177 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/binanceus.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2518 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/binanceusdm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   185234 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/bingx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37113 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/bit2c.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42099 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/bitbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      492 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/bitbay.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48385 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/bitbns.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      516 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/bitcoincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    71973 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/bitfinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   158868 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/bitfinex2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41699 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/bitflyer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   423787 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/bitget.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45758 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/bithumb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   200028 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/bitmart.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   126994 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/bitmex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    68920 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/bitopro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      485 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/bitpanda.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   136836 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/bitrue.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    71265 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/bitso.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    92765 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/bitstamp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   102352 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/bitteam.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    92005 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/bitvavo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20605 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/bl3p.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    49185 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/blockchaincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    99698 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/blofin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36973 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/btcalpha.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23680 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/btcbox.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51828 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/btcmarkets.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36869 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/btcturk.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   411940 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/bybit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    70274 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/cex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   207970 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/coinbase.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    87777 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/coinbaseinternational.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    79171 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/coinbasepro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35864 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/coincheck.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   247930 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/coinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   103683 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/coinlist.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    46206 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/coinmate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    80729 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/coinmetro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    47132 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/coinone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    91060 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/coinsph.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23760 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/coinspot.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   130350 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/cryptocom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    87181 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/currencycom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   151059 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/delta.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   161229 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/deribit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   168860 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/digifinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   115075 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/exmo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1183 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/flowbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1250 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/fmfwio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   321438 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/gate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      459 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/gateio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    81132 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/gemini.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   153964 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/hitbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      469 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/hitbtc3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    76332 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/hollaex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   422776 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/htx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      452 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/huobi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    88462 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/huobijp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   100190 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/hyperliquid.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    73435 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/idex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    32429 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/independentreserve.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    52237 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/indodax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   125943 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/kraken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   117245 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/krakenfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   218785 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/kucoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   119225 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/kucoinfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    96401 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/kuna.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    79527 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/latoken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   115881 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/lbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    46126 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/luno.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51378 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/lykke.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35575 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/mercado.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   241987 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/mexc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   109086 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/ndax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    64667 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/novadax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    38180 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/oceanex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   151634 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/okcoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   372441 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/okx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    88559 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/onetrading.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    54455 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/p2b.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24391 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/paymium.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   219623 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/phemex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   102501 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/poloniex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    78194 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/poloniexfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    76750 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/probit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    71643 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/timex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   123369 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/tokocrypto.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24094 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/tradeogre.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    82087 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/upbit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   114100 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/wavesexchange.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51638 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/wazirx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   108793 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/whitebit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   139440 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/woo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    53500 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/yobit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28139 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/zaif.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    80871 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/async_support/zonda.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.463196 ccxt-4.3.8/ccxt/base/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1320 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/base/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6634 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/base/decimal_to_precision.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4107 2024-04-25 17:02:53.000000 ccxt-4.3.8/ccxt/base/errors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   275089 2024-04-25 18:11:47.000000 ccxt-4.3.8/ccxt/base/exchange.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8565 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/base/precise.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7992 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/base/types.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1174 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/bequant.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    92190 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/bigone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   611571 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/binance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1645 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/binancecoinm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9163 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/binanceus.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2480 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/binanceusdm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   184198 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/bingx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36901 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/bit2c.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41839 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/bitbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      478 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/bitbay.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48131 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/bitbns.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      502 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/bitcoincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    71533 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/bitfinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   158134 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/bitfinex2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41391 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/bitflyer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   422163 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/bitget.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45528 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/bithumb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   199108 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/bitmart.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   126416 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/bitmex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    68516 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/bitopro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      471 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/bitpanda.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   136178 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/bitrue.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    70879 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/bitso.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    92265 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/bitstamp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   102020 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/bitteam.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    91571 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/bitvavo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20477 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/bl3p.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48793 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/blockchaincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    99114 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/blofin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36695 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/btcalpha.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23486 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/btcbox.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51478 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/btcmarkets.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36651 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/btcturk.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   410160 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/bybit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    69924 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/cex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   206918 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/coinbase.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    87223 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/coinbaseinternational.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    78665 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/coinbasepro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35658 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/coincheck.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   246642 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/coinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   103195 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/coinlist.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45940 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/coinmate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    80409 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/coinmetro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    46890 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/coinone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    90626 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/coinsph.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23608 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/coinspot.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   129778 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/cryptocom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    86759 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/currencycom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   150451 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/delta.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   160453 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/deribit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   167890 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/digifinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   114443 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/exmo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1169 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/flowbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1236 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/fmfwio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   319760 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/gate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      445 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/gateio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    80619 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/gemini.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   152918 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/hitbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      455 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/hitbtc3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    75898 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/hollaex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   420420 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/htx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      438 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/huobi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    87962 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/huobijp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    99670 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/hyperliquid.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    72959 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/idex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    32169 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/independentreserve.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51929 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/indodax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   125341 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/kraken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   116757 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/krakenfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   217713 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/kucoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   118623 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/kucoinfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    95985 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/kuna.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    79051 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/latoken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   115169 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/lbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45788 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/luno.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51064 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/lykke.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35333 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/mercado.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   240809 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/mexc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   108562 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/ndax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    64299 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/novadax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37860 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/oceanex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   151110 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/okcoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   370866 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/okx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    88107 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/onetrading.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    54213 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/p2b.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24203 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/paymium.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   218811 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/phemex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   101953 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/poloniex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    77808 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/poloniexfutures.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.567204 ccxt-4.3.8/ccxt/pro/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6998 2024-04-25 18:11:47.000000 ccxt-4.3.8/ccxt/pro/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27167 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/alpaca.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35432 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/ascendex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1351 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/bequant.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   152488 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/binance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      976 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/binancecoinm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2321 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/binanceus.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1357 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/binanceusdm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42110 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/bingx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1181 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/bitcoincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24826 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/bitfinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42744 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/bitfinex2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    71843 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/bitget.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16799 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/bithumb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    62382 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/bitmart.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    68956 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/bitmex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18724 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/bitopro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      415 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/bitpanda.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16448 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/bitrue.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20886 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/bitstamp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    56143 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/bitvavo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29560 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/blockchaincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    75022 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/bybit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    58380 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/cex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25807 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/coinbase.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25428 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/coinbaseinternational.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    38945 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/coinbasepro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7789 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/coincheck.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45042 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/coinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15652 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/coinone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42643 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/cryptocom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22355 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/currencycom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41035 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/deribit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24527 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/exmo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    52489 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/gate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      391 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/gateio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36641 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/gemini.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    56285 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/hitbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21957 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/hollaex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    95779 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/htx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      385 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/huobi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23174 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/huobijp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20791 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/hyperliquid.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28282 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/idex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11063 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/independentreserve.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    60658 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/kraken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    63917 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/krakenfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    50705 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/kucoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    46006 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/kucoinfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35105 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/lbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12348 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/luno.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42551 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/mexc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22643 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/ndax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30385 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/okcoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    68821 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/okx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    54634 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/onetrading.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17877 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/p2b.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    61032 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/phemex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51236 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/poloniex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41652 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/poloniexfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22822 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/probit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9654 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/upbit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30043 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/wazirx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35021 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/whitebit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36988 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/pro/woo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    76358 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/probit.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.571204 ccxt-4.3.8/ccxt/static_dependencies/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       84 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.579204 ccxt-4.3.8/ccxt/static_dependencies/ecdsa/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      594 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ecdsa/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18461 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ecdsa/_version.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1886 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ecdsa/curves.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6942 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ecdsa/der.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11336 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ecdsa/ecdsa.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5517 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ecdsa/ellipticcurve.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14201 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ecdsa/keys.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13468 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ecdsa/numbertheory.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2572 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ecdsa/rfc6979.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10037 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ecdsa/util.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.579204 ccxt-4.3.8/ccxt/static_dependencies/ethereum/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      171 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.587205 ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      276 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      490 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/abi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4861 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6871 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/codec.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       51 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/constants.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16828 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/decoding.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20162 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/encoding.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2941 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12358 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/grammar.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      387 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/packed.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/py.typed
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19329 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/registry.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.591205 ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/tools/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       65 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/tools/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5742 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/tools/_strategies.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.591205 ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/utils/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/utils/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2097 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/utils/numeric.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      426 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/utils/padding.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      436 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/utils/string.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.595206 ccxt-4.3.8/ccxt/static_dependencies/ethereum/account/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       48 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/account/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.595206 ccxt-4.3.8/ccxt/static_dependencies/ethereum/account/encode_typed_data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       80 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/account/encode_typed_data/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7126 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/account/encode_typed_data/encoding_and_hashing.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      982 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/account/encode_typed_data/helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10588 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/account/messages.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/account/py.typed
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.599206 ccxt-4.3.8/ccxt/static_dependencies/ethereum/hexbytes/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       60 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/hexbytes/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1687 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/hexbytes/_utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1768 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/hexbytes/main.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/hexbytes/py.typed
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.611207 ccxt-4.3.8/ccxt/static_dependencies/ethereum/typing/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      913 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/typing/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       85 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/typing/abi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      191 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/typing/bls.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       71 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/typing/discovery.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      117 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/typing/encoding.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      458 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/typing/enums.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      173 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/typing/ethpm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      546 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/typing/evm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20845 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/typing/networks.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/typing/py.typed
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.651210 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2162 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2123 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/abi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4364 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/address.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4342 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/applicators.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5498 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/conversions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3021 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/currency.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.651210 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/curried/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6398 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/curried/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      499 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/debug.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3997 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/decorators.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      199 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/encoding.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      110 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2100 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/functional.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1826 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/hexadecimal.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4137 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/humanize.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5155 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/logging.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      842 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/module_loading.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1190 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/numeric.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/py.typed
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1001 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/toolz.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1074 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/types.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.655210 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/typing/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      325 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/typing/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      189 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/typing/misc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1757 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/units.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.659210 ccxt-4.3.8/ccxt/static_dependencies/keccak/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       45 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/keccak/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6934 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/keccak/keccak.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.659210 ccxt-4.3.8/ccxt/static_dependencies/msgpack/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1077 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/msgpack/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1081 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/msgpack/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5629 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/msgpack/ext.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    33175 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/msgpack/fallback.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.667211 ccxt-4.3.8/ccxt/static_dependencies/parsimonious/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      385 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/parsimonious/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3603 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/parsimonious/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16864 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/parsimonious/expressions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19190 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/parsimonious/grammar.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13084 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/parsimonious/nodes.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1087 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/parsimonious/utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.671211 ccxt-4.3.8/ccxt/static_dependencies/toolz/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      374 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/toolz/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20555 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/toolz/_signatures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18447 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/toolz/_version.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      997 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/toolz/compatibility.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.675212 ccxt-4.3.8/ccxt/static_dependencies/toolz/curried/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2226 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/toolz/curried/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      344 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/toolz/curried/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      525 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/toolz/curried/operator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8955 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/toolz/dicttoolz.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29821 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/toolz/functoolz.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27612 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/toolz/itertoolz.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1256 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/toolz/recipes.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      139 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/static_dependencies/toolz/utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.679212 ccxt-4.3.8/ccxt/test/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      141 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/test/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.711214 ccxt-4.3.8/ccxt/test/base/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1889 2024-04-25 17:02:58.000000 ccxt-4.3.8/ccxt/test/base/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      978 2024-04-25 17:04:23.000000 ccxt-4.3.8/ccxt/test/base/test_account.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2931 2024-04-25 17:04:23.000000 ccxt-4.3.8/ccxt/test/base/test_balance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1808 2024-04-25 17:04:23.000000 ccxt-4.3.8/ccxt/test/base/test_borrow_interest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1500 2024-04-25 17:04:23.000000 ccxt-4.3.8/ccxt/test/base/test_borrow_rate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1177 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/test/base/test_calculate_fee.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7702 2024-04-25 17:02:55.000000 ccxt-4.3.8/ccxt/test/base/test_crypto.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4472 2024-04-25 17:04:23.000000 ccxt-4.3.8/ccxt/test/base/test_currency.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5235 2024-04-25 17:02:54.000000 ccxt-4.3.8/ccxt/test/base/test_datetime.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20934 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/test/base/test_decimal_to_precision.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1402 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/test/base/test_deep_extend.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2452 2024-04-25 17:04:23.000000 ccxt-4.3.8/ccxt/test/base/test_deposit_withdrawal.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3592 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/test/base/test_exchange_datetime_functions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1351 2024-04-25 17:04:23.000000 ccxt-4.3.8/ccxt/test/base/test_funding_rate_history.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1332 2024-04-25 17:04:23.000000 ccxt-4.3.8/ccxt/test/base/test_last_price.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2283 2024-04-25 17:04:23.000000 ccxt-4.3.8/ccxt/test/base/test_ledger_entry.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2154 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/test/base/test_ledger_item.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1656 2024-04-25 17:04:23.000000 ccxt-4.3.8/ccxt/test/base/test_leverage_tier.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      869 2024-04-25 17:04:23.000000 ccxt-4.3.8/ccxt/test/base/test_margin_mode.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1730 2024-04-25 17:04:23.000000 ccxt-4.3.8/ccxt/test/base/test_margin_modification.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11632 2024-04-25 17:04:23.000000 ccxt-4.3.8/ccxt/test/base/test_market.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22083 2024-04-25 17:02:54.000000 ccxt-4.3.8/ccxt/test/base/test_number.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2036 2024-04-25 17:04:23.000000 ccxt-4.3.8/ccxt/test/base/test_ohlcv.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1547 2024-04-25 17:04:23.000000 ccxt-4.3.8/ccxt/test/base/test_open_interest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3964 2024-04-25 17:04:23.000000 ccxt-4.3.8/ccxt/test/base/test_order.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3949 2024-04-25 17:04:23.000000 ccxt-4.3.8/ccxt/test/base/test_order_book.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3884 2024-04-25 17:04:23.000000 ccxt-4.3.8/ccxt/test/base/test_position.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19998 2024-04-25 17:04:23.000000 ccxt-4.3.8/ccxt/test/base/test_shared_methods.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      722 2024-04-25 17:04:23.000000 ccxt-4.3.8/ccxt/test/base/test_status.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3123 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/test/base/test_throttle.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5810 2024-04-25 17:04:23.000000 ccxt-4.3.8/ccxt/test/base/test_ticker.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2336 2024-04-25 17:04:23.000000 ccxt-4.3.8/ccxt/test/base/test_trade.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1066 2024-04-25 17:04:23.000000 ccxt-4.3.8/ccxt/test/base/test_trading_fee.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1434 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/test/base/test_transaction.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    78755 2024-04-25 17:02:58.000000 ccxt-4.3.8/ccxt/test/test_async.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    77736 2024-04-25 17:02:58.000000 ccxt-4.3.8/ccxt/test/test_sync.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    71281 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/timex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   123007 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/tokocrypto.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23900 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/tradeogre.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    81605 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/upbit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   113550 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/wavesexchange.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51336 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/wazirx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   108191 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/whitebit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   138550 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/woo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    53216 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/yobit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27957 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/zaif.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    80557 2024-04-25 16:48:28.000000 ccxt-4.3.8/ccxt/zonda.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-25 18:16:36.063167 ccxt-4.3.8/ccxt.egg-info/
+-rw-r--r--   0 travis    (2000) travis    (2000)   115320 2024-04-25 18:16:35.000000 ccxt-4.3.8/ccxt.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15741 2024-04-25 18:16:35.000000 ccxt-4.3.8/ccxt.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-25 18:16:35.000000 ccxt-4.3.8/ccxt.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      218 2024-04-25 18:16:35.000000 ccxt-4.3.8/ccxt.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        5 2024-04-25 18:16:35.000000 ccxt-4.3.8/ccxt.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12555 2024-04-25 18:11:50.000000 ccxt-4.3.8/package.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      205 2024-04-25 18:16:36.719215 ccxt-4.3.8/setup.cfg
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     3071 2024-04-25 16:48:28.000000 ccxt-4.3.8/setup.py
```

### Comparing `ccxt-4.3.7/LICENSE.txt` & `ccxt-4.3.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/PKG-INFO` & `ccxt-4.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccxt
-Version: 4.3.7
+Version: 4.3.8
 Summary: A JavaScript / TypeScript / Python / C# / PHP cryptocurrency trading library with support for 100+ exchanges
 Home-page: https://ccxt.com
 Author: Igor Kroitor
 Author-email: igor.kroitor@gmail.com
 License: MIT
 Project-URL: Homepage, https://ccxt.com
 Project-URL: Documentation, https://github.com/ccxt/ccxt/wiki
@@ -222,21 +222,21 @@
         console.log(version, Object.keys(exchanges));
         ```
         
         ### JavaScript (for use with the `<script>` tag):
         
         All-in-one browser bundle (dependencies included), served from a CDN of your choice:
         
-        * jsDelivr: https://cdn.jsdelivr.net/npm/ccxt@4.3.7/dist/ccxt.browser.js
-        * unpkg: https://unpkg.com/ccxt@4.3.7/dist/ccxt.browser.js
+        * jsDelivr: https://cdn.jsdelivr.net/npm/ccxt@4.3.8/dist/ccxt.browser.js
+        * unpkg: https://unpkg.com/ccxt@4.3.8/dist/ccxt.browser.js
         
         CDNs are not updated in real-time and may have delays. Defaulting to the most recent version without specifying the version number is not recommended. Please, keep in mind that we are not responsible for the correct operation of those CDN servers.
         
         ```HTML
-        <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/ccxt@4.3.7/dist/ccxt.browser.js"></script>
+        <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/ccxt@4.3.8/dist/ccxt.browser.js"></script>
         ```
         
         Creates a global `ccxt` object:
         
         ```JavaScript
         console.log (ccxt.exchanges) // print all available exchanges
         ```
```

### Comparing `ccxt-4.3.7/README.rst` & `ccxt-4.3.8/README.rst`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/__init__.py` & `ccxt-4.3.8/ccxt/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 # ----------------------------------------------------------------------------
 
-__version__ = '4.3.7'
+__version__ = '4.3.8'
 
 # ----------------------------------------------------------------------------
 
 from ccxt.base.exchange import Exchange                     # noqa: F401
 from ccxt.base.precise import Precise                       # noqa: F401
 
 from ccxt.base.decimal_to_precision import decimal_to_precision  # noqa: F401
```

### Comparing `ccxt-4.3.7/ccxt/abstract/ace.py` & `ccxt-4.3.8/ccxt/abstract/ace.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/alpaca.py` & `ccxt-4.3.8/ccxt/abstract/alpaca.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/ascendex.py` & `ccxt-4.3.8/ccxt/abstract/ascendex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/bequant.py` & `ccxt-4.3.8/ccxt/abstract/bequant.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/bigone.py` & `ccxt-4.3.8/ccxt/abstract/bigone.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/binance.py` & `ccxt-4.3.8/ccxt/abstract/binance.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/binancecoinm.py` & `ccxt-4.3.8/ccxt/abstract/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/binanceus.py` & `ccxt-4.3.8/ccxt/abstract/binanceus.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/binanceusdm.py` & `ccxt-4.3.8/ccxt/abstract/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/bingx.py` & `ccxt-4.3.8/ccxt/abstract/bingx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/bit2c.py` & `ccxt-4.3.8/ccxt/abstract/bit2c.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/bitbank.py` & `ccxt-4.3.8/ccxt/abstract/bitbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/bitbay.py` & `ccxt-4.3.8/ccxt/abstract/bitbay.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/bitbns.py` & `ccxt-4.3.8/ccxt/abstract/bitbns.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/bitcoincom.py` & `ccxt-4.3.8/ccxt/abstract/bitcoincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/bitfinex.py` & `ccxt-4.3.8/ccxt/abstract/bitfinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/bitfinex2.py` & `ccxt-4.3.8/ccxt/abstract/bitfinex2.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/bitflyer.py` & `ccxt-4.3.8/ccxt/abstract/bitflyer.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/bitget.py` & `ccxt-4.3.8/ccxt/abstract/bitget.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/bithumb.py` & `ccxt-4.3.8/ccxt/abstract/bithumb.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/bitmart.py` & `ccxt-4.3.8/ccxt/abstract/bitmart.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/bitmex.py` & `ccxt-4.3.8/ccxt/abstract/bitmex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/bitopro.py` & `ccxt-4.3.8/ccxt/abstract/bitopro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/bitpanda.py` & `ccxt-4.3.8/ccxt/abstract/bitpanda.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/bitrue.py` & `ccxt-4.3.8/ccxt/abstract/bitrue.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/bitso.py` & `ccxt-4.3.8/ccxt/abstract/bitso.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/bitstamp.py` & `ccxt-4.3.8/ccxt/abstract/bitstamp.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/bitteam.py` & `ccxt-4.3.8/ccxt/abstract/bitteam.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/bitvavo.py` & `ccxt-4.3.8/ccxt/abstract/bitvavo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/bl3p.py` & `ccxt-4.3.8/ccxt/abstract/bl3p.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/blockchaincom.py` & `ccxt-4.3.8/ccxt/abstract/blockchaincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/blofin.py` & `ccxt-4.3.8/ccxt/abstract/blofin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/btcalpha.py` & `ccxt-4.3.8/ccxt/abstract/btcalpha.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/btcbox.py` & `ccxt-4.3.8/ccxt/abstract/btcbox.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/btcmarkets.py` & `ccxt-4.3.8/ccxt/abstract/btcmarkets.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/btcturk.py` & `ccxt-4.3.8/ccxt/abstract/btcturk.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/bybit.py` & `ccxt-4.3.8/ccxt/abstract/bybit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/cex.py` & `ccxt-4.3.8/ccxt/abstract/cex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/coinbase.py` & `ccxt-4.3.8/ccxt/abstract/coinbase.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/coinbaseinternational.py` & `ccxt-4.3.8/ccxt/abstract/coinbaseinternational.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/coinbasepro.py` & `ccxt-4.3.8/ccxt/abstract/coinbasepro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/coincheck.py` & `ccxt-4.3.8/ccxt/abstract/coincheck.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/coinex.py` & `ccxt-4.3.8/ccxt/abstract/coinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/coinlist.py` & `ccxt-4.3.8/ccxt/abstract/coinlist.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/coinmate.py` & `ccxt-4.3.8/ccxt/abstract/coinmate.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/coinmetro.py` & `ccxt-4.3.8/ccxt/abstract/coinmetro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/coinone.py` & `ccxt-4.3.8/ccxt/abstract/coinone.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/coinsph.py` & `ccxt-4.3.8/ccxt/abstract/coinsph.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/coinspot.py` & `ccxt-4.3.8/ccxt/abstract/coinspot.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/cryptocom.py` & `ccxt-4.3.8/ccxt/abstract/cryptocom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/currencycom.py` & `ccxt-4.3.8/ccxt/abstract/currencycom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/delta.py` & `ccxt-4.3.8/ccxt/abstract/delta.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/deribit.py` & `ccxt-4.3.8/ccxt/abstract/deribit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/digifinex.py` & `ccxt-4.3.8/ccxt/abstract/digifinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/exmo.py` & `ccxt-4.3.8/ccxt/abstract/exmo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/fmfwio.py` & `ccxt-4.3.8/ccxt/abstract/fmfwio.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/gate.py` & `ccxt-4.3.8/ccxt/abstract/gate.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/gateio.py` & `ccxt-4.3.8/ccxt/abstract/gateio.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/gemini.py` & `ccxt-4.3.8/ccxt/abstract/gemini.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/hitbtc.py` & `ccxt-4.3.8/ccxt/abstract/hitbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/hitbtc3.py` & `ccxt-4.3.8/ccxt/abstract/hitbtc3.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/hollaex.py` & `ccxt-4.3.8/ccxt/abstract/hollaex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/htx.py` & `ccxt-4.3.8/ccxt/abstract/htx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/huobi.py` & `ccxt-4.3.8/ccxt/abstract/huobi.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/huobijp.py` & `ccxt-4.3.8/ccxt/abstract/huobijp.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/idex.py` & `ccxt-4.3.8/ccxt/abstract/idex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/independentreserve.py` & `ccxt-4.3.8/ccxt/abstract/independentreserve.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/indodax.py` & `ccxt-4.3.8/ccxt/abstract/indodax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/kraken.py` & `ccxt-4.3.8/ccxt/abstract/kraken.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/krakenfutures.py` & `ccxt-4.3.8/ccxt/abstract/krakenfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/kucoin.py` & `ccxt-4.3.8/ccxt/abstract/kucoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/kucoinfutures.py` & `ccxt-4.3.8/ccxt/abstract/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/kuna.py` & `ccxt-4.3.8/ccxt/abstract/kuna.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/latoken.py` & `ccxt-4.3.8/ccxt/abstract/latoken.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/lbank.py` & `ccxt-4.3.8/ccxt/abstract/lbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/luno.py` & `ccxt-4.3.8/ccxt/abstract/luno.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/lykke.py` & `ccxt-4.3.8/ccxt/abstract/lykke.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/mercado.py` & `ccxt-4.3.8/ccxt/abstract/mercado.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/mexc.py` & `ccxt-4.3.8/ccxt/abstract/mexc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/ndax.py` & `ccxt-4.3.8/ccxt/abstract/ndax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/novadax.py` & `ccxt-4.3.8/ccxt/abstract/novadax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/oceanex.py` & `ccxt-4.3.8/ccxt/abstract/oceanex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/okcoin.py` & `ccxt-4.3.8/ccxt/abstract/okcoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/okx.py` & `ccxt-4.3.8/ccxt/abstract/okx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/onetrading.py` & `ccxt-4.3.8/ccxt/abstract/onetrading.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/p2b.py` & `ccxt-4.3.8/ccxt/abstract/p2b.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/paymium.py` & `ccxt-4.3.8/ccxt/abstract/paymium.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/phemex.py` & `ccxt-4.3.8/ccxt/abstract/phemex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/poloniex.py` & `ccxt-4.3.8/ccxt/abstract/poloniex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/poloniexfutures.py` & `ccxt-4.3.8/ccxt/abstract/poloniexfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/probit.py` & `ccxt-4.3.8/ccxt/abstract/probit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/timex.py` & `ccxt-4.3.8/ccxt/abstract/timex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/tokocrypto.py` & `ccxt-4.3.8/ccxt/abstract/tokocrypto.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/tradeogre.py` & `ccxt-4.3.8/ccxt/abstract/tradeogre.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/upbit.py` & `ccxt-4.3.8/ccxt/abstract/upbit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/wavesexchange.py` & `ccxt-4.3.8/ccxt/abstract/wavesexchange.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/wazirx.py` & `ccxt-4.3.8/ccxt/abstract/wazirx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/whitebit.py` & `ccxt-4.3.8/ccxt/abstract/whitebit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/woo.py` & `ccxt-4.3.8/ccxt/abstract/woo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/yobit.py` & `ccxt-4.3.8/ccxt/abstract/yobit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/zaif.py` & `ccxt-4.3.8/ccxt/abstract/zaif.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/abstract/zonda.py` & `ccxt-4.3.8/ccxt/abstract/zonda.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/ace.py` & `ccxt-4.3.8/ccxt/ace.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/alpaca.py` & `ccxt-4.3.8/ccxt/alpaca.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/ascendex.py` & `ccxt-4.3.8/ccxt/ascendex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/__init__.py` & `ccxt-4.3.8/ccxt/async_support/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """CCXT: CryptoCurrency eXchange Trading Library (Async)"""
 
 # -----------------------------------------------------------------------------
 
-__version__ = '4.3.7'
+__version__ = '4.3.8'
 
 # -----------------------------------------------------------------------------
 
 from ccxt.async_support.base.exchange import Exchange                   # noqa: F401
 
 from ccxt.base.decimal_to_precision import decimal_to_precision  # noqa: F401
 from ccxt.base.decimal_to_precision import TRUNCATE              # noqa: F401
```

### Comparing `ccxt-4.3.7/ccxt/async_support/ace.py` & `ccxt-4.3.8/ccxt/async_support/ace.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/alpaca.py` & `ccxt-4.3.8/ccxt/async_support/alpaca.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/ascendex.py` & `ccxt-4.3.8/ccxt/async_support/ascendex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/base/exchange.py` & `ccxt-4.3.8/ccxt/async_support/base/exchange.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 # -----------------------------------------------------------------------------
 
-__version__ = '4.3.7'
+__version__ = '4.3.8'
 
 # -----------------------------------------------------------------------------
 
 import asyncio
 import concurrent.futures
 import socket
 import certifi
```

### Comparing `ccxt-4.3.7/ccxt/async_support/base/throttler.py` & `ccxt-4.3.8/ccxt/async_support/base/throttler.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/base/ws/__init__.py` & `ccxt-4.3.8/ccxt/async_support/base/ws/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/base/ws/aiohttp_client.py` & `ccxt-4.3.8/ccxt/async_support/base/ws/aiohttp_client.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/base/ws/cache.py` & `ccxt-4.3.8/ccxt/async_support/base/ws/cache.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/base/ws/client.py` & `ccxt-4.3.8/ccxt/async_support/base/ws/client.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/base/ws/fast_client.py` & `ccxt-4.3.8/ccxt/async_support/base/ws/fast_client.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/base/ws/functions.py` & `ccxt-4.3.8/ccxt/async_support/base/ws/functions.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/base/ws/future.py` & `ccxt-4.3.8/ccxt/async_support/base/ws/future.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/base/ws/order_book.py` & `ccxt-4.3.8/ccxt/async_support/base/ws/order_book.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/base/ws/order_book_side.py` & `ccxt-4.3.8/ccxt/async_support/base/ws/order_book_side.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/bequant.py` & `ccxt-4.3.8/ccxt/async_support/bequant.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/bigone.py` & `ccxt-4.3.8/ccxt/async_support/bigone.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/binance.py` & `ccxt-4.3.8/ccxt/async_support/binance.py`

 * *Files 0% similar despite different names*

```diff
@@ -38182,209 +38182,209 @@
 00095250: 2020 2020 2020 2023 0a20 2020 2020 2020         #.       
 00095260: 2072 6f77 7320 3d20 7365 6c66 2e73 6166   rows = self.saf
 00095270: 655f 6c69 7374 2872 6573 706f 6e73 652c  e_list(response,
 00095280: 2072 6573 706f 6e73 6551 7565 7279 2c20   responseQuery, 
 00095290: 5b5d 290a 2020 2020 2020 2020 7265 7475  []).        retu
 000952a0: 726e 2073 656c 662e 7061 7273 655f 636f  rn self.parse_co
 000952b0: 6e76 6572 7369 6f6e 7328 726f 7773 2c20  nversions(rows, 
-000952c0: 6672 6f6d 4375 7272 656e 6379 4b65 792c  fromCurrencyKey,
-000952d0: 2074 6f43 7572 7265 6e63 794b 6579 2c20   toCurrencyKey, 
-000952e0: 7369 6e63 652c 206c 696d 6974 290a 0a20  since, limit).. 
-000952f0: 2020 2064 6566 2070 6172 7365 5f63 6f6e     def parse_con
-00095300: 7665 7273 696f 6e28 7365 6c66 2c20 636f  version(self, co
-00095310: 6e76 6572 7369 6f6e 2c20 6672 6f6d 4375  nversion, fromCu
-00095320: 7272 656e 6379 3a20 4375 7272 656e 6379  rrency: Currency
-00095330: 203d 204e 6f6e 652c 2074 6f43 7572 7265   = None, toCurre
-00095340: 6e63 793a 2043 7572 7265 6e63 7920 3d20  ncy: Currency = 
-00095350: 4e6f 6e65 2920 2d3e 2043 6f6e 7665 7273  None) -> Convers
-00095360: 696f 6e3a 0a20 2020 2020 2020 2023 0a20  ion:.        #. 
-00095370: 2020 2020 2020 2023 2066 6574 6368 436f         # fetchCo
-00095380: 6e76 6572 7451 756f 7465 0a20 2020 2020  nvertQuote.     
-00095390: 2020 2023 0a20 2020 2020 2020 2023 2020     #.        #  
-000953a0: 2020 207b 0a20 2020 2020 2020 2023 2020     {.        #  
-000953b0: 2020 2020 2020 2022 7175 6f74 6549 6422         "quoteId"
-000953c0: 3a22 3132 3431 3535 3732 3536 3422 2c0a  :"12415572564",.
-000953d0: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-000953e0: 2020 2272 6174 696f 223a 2233 3831 3633    "ratio":"38163
-000953f0: 2e37 222c 0a20 2020 2020 2020 2023 2020  .7",.        #  
-00095400: 2020 2020 2020 2022 696e 7665 7273 6552         "inverseR
-00095410: 6174 696f 223a 2230 2e30 3030 3032 3632  atio":"0.0000262
-00095420: 222c 0a20 2020 2020 2020 2023 2020 2020  ",.        #    
-00095430: 2020 2020 2022 7661 6c69 6454 696d 6573       "validTimes
-00095440: 7461 6d70 223a 3136 3233 3331 3934 3631  tamp":1623319461
-00095450: 3637 302c 0a20 2020 2020 2020 2023 2020  670,.        #  
-00095460: 2020 2020 2020 2022 746f 416d 6f75 6e74         "toAmount
-00095470: 223a 2233 3831 362e 3337 222c 0a20 2020  ":"3816.37",.   
-00095480: 2020 2020 2023 2020 2020 2020 2020 2022       #         "
-00095490: 6672 6f6d 416d 6f75 6e74 223a 2230 2e31  fromAmount":"0.1
-000954a0: 220a 2020 2020 2020 2020 2320 2020 2020  ".        #     
-000954b0: 7d0a 2020 2020 2020 2020 230a 2020 2020  }.        #.    
-000954c0: 2020 2020 2320 6372 6561 7465 436f 6e76      # createConv
-000954d0: 6572 7454 7261 6465 0a20 2020 2020 2020  ertTrade.       
-000954e0: 2023 0a20 2020 2020 2020 2023 2020 2020   #.        #    
-000954f0: 207b 0a20 2020 2020 2020 2023 2020 2020   {.        #    
-00095500: 2020 2020 2022 6f72 6465 7249 6422 3a22       "orderId":"
-00095510: 3933 3332 3536 3237 3834 3236 3237 3434  9332562784262744
-00095520: 3236 222c 0a20 2020 2020 2020 2023 2020  26",.        #  
-00095530: 2020 2020 2020 2022 6372 6561 7465 5469         "createTi
-00095540: 6d65 223a 3136 3233 3338 3133 3330 3437  me":162338133047
-00095550: 322c 0a20 2020 2020 2020 2023 2020 2020  2,.        #    
-00095560: 2020 2020 2022 6f72 6465 7253 7461 7475       "orderStatu
-00095570: 7322 3a22 5052 4f43 4553 5322 0a20 2020  s":"PROCESS".   
-00095580: 2020 2020 2023 2020 2020 207d 0a20 2020       #     }.   
-00095590: 2020 2020 2023 0a20 2020 2020 2020 2023       #.        #
-000955a0: 2063 7265 6174 6543 6f6e 7665 7274 5472   createConvertTr
-000955b0: 6164 6520 4255 5344 0a20 2020 2020 2020  ade BUSD.       
-000955c0: 2023 0a20 2020 2020 2020 2023 2020 2020   #.        #    
-000955d0: 207b 0a20 2020 2020 2020 2023 2020 2020   {.        #    
-000955e0: 2020 2020 2022 7472 616e 4964 223a 2031       "tranId": 1
-000955f0: 3138 3236 3334 3037 3131 392c 0a20 2020  18263407119,.   
-00095600: 2020 2020 2023 2020 2020 2020 2020 2022       #         "
-00095610: 7374 6174 7573 223a 2022 5322 0a20 2020  status": "S".   
-00095620: 2020 2020 2023 2020 2020 207d 0a20 2020       #     }.   
-00095630: 2020 2020 2023 0a20 2020 2020 2020 2023       #.        #
-00095640: 2066 6574 6368 436f 6e76 6572 7454 7261   fetchConvertTra
-00095650: 6465 2c20 6665 7463 6843 6f6e 7665 7274  de, fetchConvert
-00095660: 5472 6164 6548 6973 746f 7279 2042 5553  TradeHistory BUS
-00095670: 440a 2020 2020 2020 2020 230a 2020 2020  D.        #.    
-00095680: 2020 2020 2320 2020 2020 7b0a 2020 2020      #     {.    
-00095690: 2020 2020 2320 2020 2020 2020 2020 2274      #         "t
-000956a0: 7261 6e49 6422 3a20 3131 3832 3633 3631  ranId": 11826361
-000956b0: 3539 3931 2c0a 2020 2020 2020 2020 2320  5991,.        # 
-000956c0: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
-000956d0: 3234 342c 0a20 2020 2020 2020 2023 2020  244,.        #  
-000956e0: 2020 2020 2020 2022 7469 6d65 223a 2031         "time": 1
-000956f0: 3636 3434 3432 3037 3830 3030 2c0a 2020  664442078000,.  
-00095700: 2020 2020 2020 2320 2020 2020 2020 2020        #         
-00095710: 2264 6564 7563 7465 6441 7373 6574 223a  "deductedAsset":
-00095720: 2022 4255 5344 222c 0a20 2020 2020 2020   "BUSD",.       
-00095730: 2023 2020 2020 2020 2020 2022 6465 6475   #         "dedu
-00095740: 6374 6564 416d 6f75 6e74 223a 2022 3122  ctedAmount": "1"
-00095750: 2c0a 2020 2020 2020 2020 2320 2020 2020  ,.        #     
-00095760: 2020 2020 2274 6172 6765 7441 7373 6574      "targetAsset
-00095770: 223a 2022 5553 4443 222c 0a20 2020 2020  ": "USDC",.     
-00095780: 2020 2023 2020 2020 2020 2020 2022 7461     #         "ta
-00095790: 7267 6574 416d 6f75 6e74 223a 2022 3122  rgetAmount": "1"
-000957a0: 2c0a 2020 2020 2020 2020 2320 2020 2020  ,.        #     
-000957b0: 2020 2020 2273 7461 7475 7322 3a20 2253      "status": "S
-000957c0: 222c 0a20 2020 2020 2020 2023 2020 2020  ",.        #    
-000957d0: 2020 2020 2022 6163 636f 756e 7454 7970       "accountTyp
-000957e0: 6522 3a20 224d 4149 4e22 0a20 2020 2020  e": "MAIN".     
-000957f0: 2020 2023 2020 2020 207d 0a20 2020 2020     #     }.     
-00095800: 2020 2023 0a20 2020 2020 2020 2023 2066     #.        # f
-00095810: 6574 6368 436f 6e76 6572 7454 7261 6465  etchConvertTrade
-00095820: 0a20 2020 2020 2020 2023 0a20 2020 2020  .        #.     
-00095830: 2020 2023 2020 2020 207b 0a20 2020 2020     #     {.     
-00095840: 2020 2023 2020 2020 2020 2020 2022 6f72     #         "or
-00095850: 6465 7249 6422 3a39 3333 3235 3632 3738  derId":933256278
-00095860: 3432 3632 3734 3432 362c 0a20 2020 2020  426274426,.     
-00095870: 2020 2023 2020 2020 2020 2020 2022 6f72     #         "or
-00095880: 6465 7253 7461 7475 7322 3a22 5355 4343  derStatus":"SUCC
-00095890: 4553 5322 2c0a 2020 2020 2020 2020 2320  ESS",.        # 
-000958a0: 2020 2020 2020 2020 2266 726f 6d41 7373          "fromAss
-000958b0: 6574 223a 2242 5443 222c 0a20 2020 2020  et":"BTC",.     
-000958c0: 2020 2023 2020 2020 2020 2020 2022 6672     #         "fr
-000958d0: 6f6d 416d 6f75 6e74 223a 2230 2e30 3030  omAmount":"0.000
-000958e0: 3534 3431 3422 2c0a 2020 2020 2020 2020  54414",.        
-000958f0: 2320 2020 2020 2020 2020 2274 6f41 7373  #         "toAss
-00095900: 6574 223a 2255 5344 5422 2c0a 2020 2020  et":"USDT",.    
-00095910: 2020 2020 2320 2020 2020 2020 2020 2274      #         "t
-00095920: 6f41 6d6f 756e 7422 3a22 3230 222c 0a20  oAmount":"20",. 
-00095930: 2020 2020 2020 2023 2020 2020 2020 2020         #        
-00095940: 2022 7261 7469 6f22 3a22 3336 3735 3522   "ratio":"36755"
-00095950: 2c0a 2020 2020 2020 2020 2320 2020 2020  ,.        #     
-00095960: 2020 2020 2269 6e76 6572 7365 5261 7469      "inverseRati
-00095970: 6f22 3a22 302e 3030 3030 3237 3231 222c  o":"0.00002721",
-00095980: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
-00095990: 2020 2022 6372 6561 7465 5469 6d65 223a     "createTime":
-000959a0: 3136 3233 3338 3133 3330 3437 320a 2020  1623381330472.  
-000959b0: 2020 2020 2020 2320 2020 2020 7d0a 2020        #     }.  
-000959c0: 2020 2020 2020 230a 2020 2020 2020 2020        #.        
-000959d0: 2320 6665 7463 6843 6f6e 7665 7274 5472  # fetchConvertTr
-000959e0: 6164 6548 6973 746f 7279 0a20 2020 2020  adeHistory.     
-000959f0: 2020 2023 0a20 2020 2020 2020 2023 2020     #.        #  
-00095a00: 2020 207b 0a20 2020 2020 2020 2023 2020     {.        #  
-00095a10: 2020 2020 2020 2022 7175 6f74 6549 6422         "quoteId"
-00095a20: 3a20 2266 3362 3931 6335 3235 6232 3634  : "f3b91c525b264
-00095a30: 3463 3762 6331 6531 6364 3331 6236 6531  4c7bc1e1cd31b6e1
-00095a40: 6161 3622 2c0a 2020 2020 2020 2020 2320  aa6",.        # 
-00095a50: 2020 2020 2020 2020 226f 7264 6572 4964          "orderId
-00095a60: 223a 2039 3430 3730 3834 3037 3436 3230  ": 9407084074620
-00095a70: 3837 3139 352c 0a20 2020 2020 2020 2023  87195,.        #
-00095a80: 2020 2020 2020 2020 2022 6f72 6465 7253           "orderS
-00095a90: 7461 7475 7322 3a20 2253 5543 4345 5353  tatus": "SUCCESS
-00095aa0: 222c 0a20 2020 2020 2020 2023 2020 2020  ",.        #    
-00095ab0: 2020 2020 2022 6672 6f6d 4173 7365 7422       "fromAsset"
-00095ac0: 3a20 2255 5344 5422 2c0a 2020 2020 2020  : "USDT",.      
-00095ad0: 2020 2320 2020 2020 2020 2020 2266 726f    #         "fro
-00095ae0: 6d41 6d6f 756e 7422 3a20 2232 3022 2c0a  mAmount": "20",.
-00095af0: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-00095b00: 2020 2274 6f41 7373 6574 223a 2022 424e    "toAsset": "BN
-00095b10: 4222 2c0a 2020 2020 2020 2020 2320 2020  B",.        #   
-00095b20: 2020 2020 2020 2274 6f41 6d6f 756e 7422        "toAmount"
-00095b30: 3a20 2230 2e30 3631 3534 3033 3622 2c0a  : "0.06154036",.
-00095b40: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-00095b50: 2020 2272 6174 696f 223a 2022 302e 3030    "ratio": "0.00
-00095b60: 3330 3737 3032 222c 0a20 2020 2020 2020  307702",.       
-00095b70: 2023 2020 2020 2020 2020 2022 696e 7665   #         "inve
-00095b80: 7273 6552 6174 696f 223a 2022 3332 342e  rseRatio": "324.
-00095b90: 3939 222c 0a20 2020 2020 2020 2023 2020  99",.        #  
-00095ba0: 2020 2020 2020 2022 6372 6561 7465 5469         "createTi
-00095bb0: 6d65 223a 2031 3632 3432 3438 3837 3231  me": 16242488721
-00095bc0: 3834 0a20 2020 2020 2020 2023 2020 2020  84.        #    
-00095bd0: 207d 0a20 2020 2020 2020 2023 0a20 2020   }.        #.   
-00095be0: 2020 2020 2074 696d 6573 7461 6d70 203d       timestamp =
-00095bf0: 2073 656c 662e 7361 6665 5f69 6e74 6567   self.safe_integ
-00095c00: 6572 5f6e 2863 6f6e 7665 7273 696f 6e2c  er_n(conversion,
-00095c10: 205b 2774 696d 6527 2c20 2776 616c 6964   ['time', 'valid
-00095c20: 5469 6d65 7374 616d 7027 2c20 2763 7265  Timestamp', 'cre
-00095c30: 6174 6554 696d 6527 5d29 0a20 2020 2020  ateTime']).     
-00095c40: 2020 2066 726f 6d43 7572 203d 2073 656c     fromCur = sel
-00095c50: 662e 7361 6665 5f73 7472 696e 675f 3228  f.safe_string_2(
-00095c60: 636f 6e76 6572 7369 6f6e 2c20 2764 6564  conversion, 'ded
-00095c70: 7563 7465 6441 7373 6574 272c 2027 6672  uctedAsset', 'fr
-00095c80: 6f6d 4173 7365 7427 290a 2020 2020 2020  omAsset').      
-00095c90: 2020 6672 6f6d 436f 6465 203d 2073 656c    fromCode = sel
-00095ca0: 662e 7361 6665 5f63 7572 7265 6e63 795f  f.safe_currency_
-00095cb0: 636f 6465 2866 726f 6d43 7572 2c20 6672  code(fromCur, fr
-00095cc0: 6f6d 4375 7272 656e 6379 290a 2020 2020  omCurrency).    
-00095cd0: 2020 2020 746f 203d 2073 656c 662e 7361      to = self.sa
-00095ce0: 6665 5f73 7472 696e 675f 3228 636f 6e76  fe_string_2(conv
-00095cf0: 6572 7369 6f6e 2c20 2774 6172 6765 7441  ersion, 'targetA
-00095d00: 7373 6574 272c 2027 746f 4173 7365 7427  sset', 'toAsset'
-00095d10: 290a 2020 2020 2020 2020 746f 436f 6465  ).        toCode
-00095d20: 203d 2073 656c 662e 7361 6665 5f63 7572   = self.safe_cur
-00095d30: 7265 6e63 795f 636f 6465 2874 6f2c 2074  rency_code(to, t
-00095d40: 6f43 7572 7265 6e63 7929 0a20 2020 2020  oCurrency).     
-00095d50: 2020 2072 6574 7572 6e20 7b0a 2020 2020     return {.    
-00095d60: 2020 2020 2020 2020 2769 6e66 6f27 3a20          'info': 
-00095d70: 636f 6e76 6572 7369 6f6e 2c0a 2020 2020  conversion,.    
-00095d80: 2020 2020 2020 2020 2774 696d 6573 7461          'timesta
-00095d90: 6d70 273a 2074 696d 6573 7461 6d70 2c0a  mp': timestamp,.
-00095da0: 2020 2020 2020 2020 2020 2020 2764 6174              'dat
-00095db0: 6574 696d 6527 3a20 7365 6c66 2e69 736f  etime': self.iso
-00095dc0: 3836 3031 2874 696d 6573 7461 6d70 292c  8601(timestamp),
-00095dd0: 0a20 2020 2020 2020 2020 2020 2027 6964  .            'id
-00095de0: 273a 2073 656c 662e 7361 6665 5f73 7472  ': self.safe_str
-00095df0: 696e 675f 6e28 636f 6e76 6572 7369 6f6e  ing_n(conversion
-00095e00: 2c20 5b27 7472 616e 4964 272c 2027 6f72  , ['tranId', 'or
-00095e10: 6465 7249 6427 2c20 2771 756f 7465 4964  derId', 'quoteId
-00095e20: 275d 292c 0a20 2020 2020 2020 2020 2020  ']),.           
-00095e30: 2027 6672 6f6d 4375 7272 656e 6379 273a   'fromCurrency':
-00095e40: 2066 726f 6d43 6f64 652c 0a20 2020 2020   fromCode,.     
-00095e50: 2020 2020 2020 2027 6672 6f6d 416d 6f75         'fromAmou
-00095e60: 6e74 273a 2073 656c 662e 7361 6665 5f6e  nt': self.safe_n
-00095e70: 756d 6265 725f 3228 636f 6e76 6572 7369  umber_2(conversi
-00095e80: 6f6e 2c20 2764 6564 7563 7465 6441 6d6f  on, 'deductedAmo
-00095e90: 756e 7427 2c20 2766 726f 6d41 6d6f 756e  unt', 'fromAmoun
-00095ea0: 7427 292c 0a20 2020 2020 2020 2020 2020  t'),.           
-00095eb0: 2027 746f 4375 7272 656e 6379 273a 2074   'toCurrency': t
-00095ec0: 6f43 6f64 652c 0a20 2020 2020 2020 2020  oCode,.         
-00095ed0: 2020 2027 746f 416d 6f75 6e74 273a 2073     'toAmount': s
-00095ee0: 656c 662e 7361 6665 5f6e 756d 6265 725f  elf.safe_number_
-00095ef0: 3228 636f 6e76 6572 7369 6f6e 2c20 2774  2(conversion, 't
-00095f00: 6172 6765 7441 6d6f 756e 7427 2c20 2774  argetAmount', 't
-00095f10: 6f41 6d6f 756e 7427 292c 0a20 2020 2020  oAmount'),.     
-00095f20: 2020 2020 2020 2027 7072 6963 6527 3a20         'price': 
-00095f30: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-00095f40: 2020 2766 6565 273a 204e 6f6e 652c 0a20    'fee': None,. 
-00095f50: 2020 2020 2020 207d 0a                          }.
+000952c0: 636f 6465 2c20 6672 6f6d 4375 7272 656e  code, fromCurren
+000952d0: 6379 4b65 792c 2074 6f43 7572 7265 6e63  cyKey, toCurrenc
+000952e0: 794b 6579 2c20 7369 6e63 652c 206c 696d  yKey, since, lim
+000952f0: 6974 290a 0a20 2020 2064 6566 2070 6172  it)..    def par
+00095300: 7365 5f63 6f6e 7665 7273 696f 6e28 7365  se_conversion(se
+00095310: 6c66 2c20 636f 6e76 6572 7369 6f6e 2c20  lf, conversion, 
+00095320: 6672 6f6d 4375 7272 656e 6379 3a20 4375  fromCurrency: Cu
+00095330: 7272 656e 6379 203d 204e 6f6e 652c 2074  rrency = None, t
+00095340: 6f43 7572 7265 6e63 793a 2043 7572 7265  oCurrency: Curre
+00095350: 6e63 7920 3d20 4e6f 6e65 2920 2d3e 2043  ncy = None) -> C
+00095360: 6f6e 7665 7273 696f 6e3a 0a20 2020 2020  onversion:.     
+00095370: 2020 2023 0a20 2020 2020 2020 2023 2066     #.        # f
+00095380: 6574 6368 436f 6e76 6572 7451 756f 7465  etchConvertQuote
+00095390: 0a20 2020 2020 2020 2023 0a20 2020 2020  .        #.     
+000953a0: 2020 2023 2020 2020 207b 0a20 2020 2020     #     {.     
+000953b0: 2020 2023 2020 2020 2020 2020 2022 7175     #         "qu
+000953c0: 6f74 6549 6422 3a22 3132 3431 3535 3732  oteId":"12415572
+000953d0: 3536 3422 2c0a 2020 2020 2020 2020 2320  564",.        # 
+000953e0: 2020 2020 2020 2020 2272 6174 696f 223a          "ratio":
+000953f0: 2233 3831 3633 2e37 222c 0a20 2020 2020  "38163.7",.     
+00095400: 2020 2023 2020 2020 2020 2020 2022 696e     #         "in
+00095410: 7665 7273 6552 6174 696f 223a 2230 2e30  verseRatio":"0.0
+00095420: 3030 3032 3632 222c 0a20 2020 2020 2020  000262",.       
+00095430: 2023 2020 2020 2020 2020 2022 7661 6c69   #         "vali
+00095440: 6454 696d 6573 7461 6d70 223a 3136 3233  dTimestamp":1623
+00095450: 3331 3934 3631 3637 302c 0a20 2020 2020  319461670,.     
+00095460: 2020 2023 2020 2020 2020 2020 2022 746f     #         "to
+00095470: 416d 6f75 6e74 223a 2233 3831 362e 3337  Amount":"3816.37
+00095480: 222c 0a20 2020 2020 2020 2023 2020 2020  ",.        #    
+00095490: 2020 2020 2022 6672 6f6d 416d 6f75 6e74       "fromAmount
+000954a0: 223a 2230 2e31 220a 2020 2020 2020 2020  ":"0.1".        
+000954b0: 2320 2020 2020 7d0a 2020 2020 2020 2020  #     }.        
+000954c0: 230a 2020 2020 2020 2020 2320 6372 6561  #.        # crea
+000954d0: 7465 436f 6e76 6572 7454 7261 6465 0a20  teConvertTrade. 
+000954e0: 2020 2020 2020 2023 0a20 2020 2020 2020         #.       
+000954f0: 2023 2020 2020 207b 0a20 2020 2020 2020   #     {.       
+00095500: 2023 2020 2020 2020 2020 2022 6f72 6465   #         "orde
+00095510: 7249 6422 3a22 3933 3332 3536 3237 3834  rId":"9332562784
+00095520: 3236 3237 3434 3236 222c 0a20 2020 2020  26274426",.     
+00095530: 2020 2023 2020 2020 2020 2020 2022 6372     #         "cr
+00095540: 6561 7465 5469 6d65 223a 3136 3233 3338  eateTime":162338
+00095550: 3133 3330 3437 322c 0a20 2020 2020 2020  1330472,.       
+00095560: 2023 2020 2020 2020 2020 2022 6f72 6465   #         "orde
+00095570: 7253 7461 7475 7322 3a22 5052 4f43 4553  rStatus":"PROCES
+00095580: 5322 0a20 2020 2020 2020 2023 2020 2020  S".        #    
+00095590: 207d 0a20 2020 2020 2020 2023 0a20 2020   }.        #.   
+000955a0: 2020 2020 2023 2063 7265 6174 6543 6f6e       # createCon
+000955b0: 7665 7274 5472 6164 6520 4255 5344 0a20  vertTrade BUSD. 
+000955c0: 2020 2020 2020 2023 0a20 2020 2020 2020         #.       
+000955d0: 2023 2020 2020 207b 0a20 2020 2020 2020   #     {.       
+000955e0: 2023 2020 2020 2020 2020 2022 7472 616e   #         "tran
+000955f0: 4964 223a 2031 3138 3236 3334 3037 3131  Id": 11826340711
+00095600: 392c 0a20 2020 2020 2020 2023 2020 2020  9,.        #    
+00095610: 2020 2020 2022 7374 6174 7573 223a 2022       "status": "
+00095620: 5322 0a20 2020 2020 2020 2023 2020 2020  S".        #    
+00095630: 207d 0a20 2020 2020 2020 2023 0a20 2020   }.        #.   
+00095640: 2020 2020 2023 2066 6574 6368 436f 6e76       # fetchConv
+00095650: 6572 7454 7261 6465 2c20 6665 7463 6843  ertTrade, fetchC
+00095660: 6f6e 7665 7274 5472 6164 6548 6973 746f  onvertTradeHisto
+00095670: 7279 2042 5553 440a 2020 2020 2020 2020  ry BUSD.        
+00095680: 230a 2020 2020 2020 2020 2320 2020 2020  #.        #     
+00095690: 7b0a 2020 2020 2020 2020 2320 2020 2020  {.        #     
+000956a0: 2020 2020 2274 7261 6e49 6422 3a20 3131      "tranId": 11
+000956b0: 3832 3633 3631 3539 3931 2c0a 2020 2020  8263615991,.    
+000956c0: 2020 2020 2320 2020 2020 2020 2020 2274      #         "t
+000956d0: 7970 6522 3a20 3234 342c 0a20 2020 2020  ype": 244,.     
+000956e0: 2020 2023 2020 2020 2020 2020 2022 7469     #         "ti
+000956f0: 6d65 223a 2031 3636 3434 3432 3037 3830  me": 16644420780
+00095700: 3030 2c0a 2020 2020 2020 2020 2320 2020  00,.        #   
+00095710: 2020 2020 2020 2264 6564 7563 7465 6441        "deductedA
+00095720: 7373 6574 223a 2022 4255 5344 222c 0a20  sset": "BUSD",. 
+00095730: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+00095740: 2022 6465 6475 6374 6564 416d 6f75 6e74   "deductedAmount
+00095750: 223a 2022 3122 2c0a 2020 2020 2020 2020  ": "1",.        
+00095760: 2320 2020 2020 2020 2020 2274 6172 6765  #         "targe
+00095770: 7441 7373 6574 223a 2022 5553 4443 222c  tAsset": "USDC",
+00095780: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+00095790: 2020 2022 7461 7267 6574 416d 6f75 6e74     "targetAmount
+000957a0: 223a 2022 3122 2c0a 2020 2020 2020 2020  ": "1",.        
+000957b0: 2320 2020 2020 2020 2020 2273 7461 7475  #         "statu
+000957c0: 7322 3a20 2253 222c 0a20 2020 2020 2020  s": "S",.       
+000957d0: 2023 2020 2020 2020 2020 2022 6163 636f   #         "acco
+000957e0: 756e 7454 7970 6522 3a20 224d 4149 4e22  untType": "MAIN"
+000957f0: 0a20 2020 2020 2020 2023 2020 2020 207d  .        #     }
+00095800: 0a20 2020 2020 2020 2023 0a20 2020 2020  .        #.     
+00095810: 2020 2023 2066 6574 6368 436f 6e76 6572     # fetchConver
+00095820: 7454 7261 6465 0a20 2020 2020 2020 2023  tTrade.        #
+00095830: 0a20 2020 2020 2020 2023 2020 2020 207b  .        #     {
+00095840: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+00095850: 2020 2022 6f72 6465 7249 6422 3a39 3333     "orderId":933
+00095860: 3235 3632 3738 3432 3632 3734 3432 362c  256278426274426,
+00095870: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+00095880: 2020 2022 6f72 6465 7253 7461 7475 7322     "orderStatus"
+00095890: 3a22 5355 4343 4553 5322 2c0a 2020 2020  :"SUCCESS",.    
+000958a0: 2020 2020 2320 2020 2020 2020 2020 2266      #         "f
+000958b0: 726f 6d41 7373 6574 223a 2242 5443 222c  romAsset":"BTC",
+000958c0: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+000958d0: 2020 2022 6672 6f6d 416d 6f75 6e74 223a     "fromAmount":
+000958e0: 2230 2e30 3030 3534 3431 3422 2c0a 2020  "0.00054414",.  
+000958f0: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+00095900: 2274 6f41 7373 6574 223a 2255 5344 5422  "toAsset":"USDT"
+00095910: 2c0a 2020 2020 2020 2020 2320 2020 2020  ,.        #     
+00095920: 2020 2020 2274 6f41 6d6f 756e 7422 3a22      "toAmount":"
+00095930: 3230 222c 0a20 2020 2020 2020 2023 2020  20",.        #  
+00095940: 2020 2020 2020 2022 7261 7469 6f22 3a22         "ratio":"
+00095950: 3336 3735 3522 2c0a 2020 2020 2020 2020  36755",.        
+00095960: 2320 2020 2020 2020 2020 2269 6e76 6572  #         "inver
+00095970: 7365 5261 7469 6f22 3a22 302e 3030 3030  seRatio":"0.0000
+00095980: 3237 3231 222c 0a20 2020 2020 2020 2023  2721",.        #
+00095990: 2020 2020 2020 2020 2022 6372 6561 7465           "create
+000959a0: 5469 6d65 223a 3136 3233 3338 3133 3330  Time":1623381330
+000959b0: 3437 320a 2020 2020 2020 2020 2320 2020  472.        #   
+000959c0: 2020 7d0a 2020 2020 2020 2020 230a 2020    }.        #.  
+000959d0: 2020 2020 2020 2320 6665 7463 6843 6f6e        # fetchCon
+000959e0: 7665 7274 5472 6164 6548 6973 746f 7279  vertTradeHistory
+000959f0: 0a20 2020 2020 2020 2023 0a20 2020 2020  .        #.     
+00095a00: 2020 2023 2020 2020 207b 0a20 2020 2020     #     {.     
+00095a10: 2020 2023 2020 2020 2020 2020 2022 7175     #         "qu
+00095a20: 6f74 6549 6422 3a20 2266 3362 3931 6335  oteId": "f3b91c5
+00095a30: 3235 6232 3634 3463 3762 6331 6531 6364  25b2644c7bc1e1cd
+00095a40: 3331 6236 6531 6161 3622 2c0a 2020 2020  31b6e1aa6",.    
+00095a50: 2020 2020 2320 2020 2020 2020 2020 226f      #         "o
+00095a60: 7264 6572 4964 223a 2039 3430 3730 3834  rderId": 9407084
+00095a70: 3037 3436 3230 3837 3139 352c 0a20 2020  07462087195,.   
+00095a80: 2020 2020 2023 2020 2020 2020 2020 2022       #         "
+00095a90: 6f72 6465 7253 7461 7475 7322 3a20 2253  orderStatus": "S
+00095aa0: 5543 4345 5353 222c 0a20 2020 2020 2020  UCCESS",.       
+00095ab0: 2023 2020 2020 2020 2020 2022 6672 6f6d   #         "from
+00095ac0: 4173 7365 7422 3a20 2255 5344 5422 2c0a  Asset": "USDT",.
+00095ad0: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+00095ae0: 2020 2266 726f 6d41 6d6f 756e 7422 3a20    "fromAmount": 
+00095af0: 2232 3022 2c0a 2020 2020 2020 2020 2320  "20",.        # 
+00095b00: 2020 2020 2020 2020 2274 6f41 7373 6574          "toAsset
+00095b10: 223a 2022 424e 4222 2c0a 2020 2020 2020  ": "BNB",.      
+00095b20: 2020 2320 2020 2020 2020 2020 2274 6f41    #         "toA
+00095b30: 6d6f 756e 7422 3a20 2230 2e30 3631 3534  mount": "0.06154
+00095b40: 3033 3622 2c0a 2020 2020 2020 2020 2320  036",.        # 
+00095b50: 2020 2020 2020 2020 2272 6174 696f 223a          "ratio":
+00095b60: 2022 302e 3030 3330 3737 3032 222c 0a20   "0.00307702",. 
+00095b70: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+00095b80: 2022 696e 7665 7273 6552 6174 696f 223a   "inverseRatio":
+00095b90: 2022 3332 342e 3939 222c 0a20 2020 2020   "324.99",.     
+00095ba0: 2020 2023 2020 2020 2020 2020 2022 6372     #         "cr
+00095bb0: 6561 7465 5469 6d65 223a 2031 3632 3432  eateTime": 16242
+00095bc0: 3438 3837 3231 3834 0a20 2020 2020 2020  48872184.       
+00095bd0: 2023 2020 2020 207d 0a20 2020 2020 2020   #     }.       
+00095be0: 2023 0a20 2020 2020 2020 2074 696d 6573   #.        times
+00095bf0: 7461 6d70 203d 2073 656c 662e 7361 6665  tamp = self.safe
+00095c00: 5f69 6e74 6567 6572 5f6e 2863 6f6e 7665  _integer_n(conve
+00095c10: 7273 696f 6e2c 205b 2774 696d 6527 2c20  rsion, ['time', 
+00095c20: 2776 616c 6964 5469 6d65 7374 616d 7027  'validTimestamp'
+00095c30: 2c20 2763 7265 6174 6554 696d 6527 5d29  , 'createTime'])
+00095c40: 0a20 2020 2020 2020 2066 726f 6d43 7572  .        fromCur
+00095c50: 203d 2073 656c 662e 7361 6665 5f73 7472   = self.safe_str
+00095c60: 696e 675f 3228 636f 6e76 6572 7369 6f6e  ing_2(conversion
+00095c70: 2c20 2764 6564 7563 7465 6441 7373 6574  , 'deductedAsset
+00095c80: 272c 2027 6672 6f6d 4173 7365 7427 290a  ', 'fromAsset').
+00095c90: 2020 2020 2020 2020 6672 6f6d 436f 6465          fromCode
+00095ca0: 203d 2073 656c 662e 7361 6665 5f63 7572   = self.safe_cur
+00095cb0: 7265 6e63 795f 636f 6465 2866 726f 6d43  rency_code(fromC
+00095cc0: 7572 2c20 6672 6f6d 4375 7272 656e 6379  ur, fromCurrency
+00095cd0: 290a 2020 2020 2020 2020 746f 203d 2073  ).        to = s
+00095ce0: 656c 662e 7361 6665 5f73 7472 696e 675f  elf.safe_string_
+00095cf0: 3228 636f 6e76 6572 7369 6f6e 2c20 2774  2(conversion, 't
+00095d00: 6172 6765 7441 7373 6574 272c 2027 746f  argetAsset', 'to
+00095d10: 4173 7365 7427 290a 2020 2020 2020 2020  Asset').        
+00095d20: 746f 436f 6465 203d 2073 656c 662e 7361  toCode = self.sa
+00095d30: 6665 5f63 7572 7265 6e63 795f 636f 6465  fe_currency_code
+00095d40: 2874 6f2c 2074 6f43 7572 7265 6e63 7929  (to, toCurrency)
+00095d50: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00095d60: 7b0a 2020 2020 2020 2020 2020 2020 2769  {.            'i
+00095d70: 6e66 6f27 3a20 636f 6e76 6572 7369 6f6e  nfo': conversion
+00095d80: 2c0a 2020 2020 2020 2020 2020 2020 2774  ,.            't
+00095d90: 696d 6573 7461 6d70 273a 2074 696d 6573  imestamp': times
+00095da0: 7461 6d70 2c0a 2020 2020 2020 2020 2020  tamp,.          
+00095db0: 2020 2764 6174 6574 696d 6527 3a20 7365    'datetime': se
+00095dc0: 6c66 2e69 736f 3836 3031 2874 696d 6573  lf.iso8601(times
+00095dd0: 7461 6d70 292c 0a20 2020 2020 2020 2020  tamp),.         
+00095de0: 2020 2027 6964 273a 2073 656c 662e 7361     'id': self.sa
+00095df0: 6665 5f73 7472 696e 675f 6e28 636f 6e76  fe_string_n(conv
+00095e00: 6572 7369 6f6e 2c20 5b27 7472 616e 4964  ersion, ['tranId
+00095e10: 272c 2027 6f72 6465 7249 6427 2c20 2771  ', 'orderId', 'q
+00095e20: 756f 7465 4964 275d 292c 0a20 2020 2020  uoteId']),.     
+00095e30: 2020 2020 2020 2027 6672 6f6d 4375 7272         'fromCurr
+00095e40: 656e 6379 273a 2066 726f 6d43 6f64 652c  ency': fromCode,
+00095e50: 0a20 2020 2020 2020 2020 2020 2027 6672  .            'fr
+00095e60: 6f6d 416d 6f75 6e74 273a 2073 656c 662e  omAmount': self.
+00095e70: 7361 6665 5f6e 756d 6265 725f 3228 636f  safe_number_2(co
+00095e80: 6e76 6572 7369 6f6e 2c20 2764 6564 7563  nversion, 'deduc
+00095e90: 7465 6441 6d6f 756e 7427 2c20 2766 726f  tedAmount', 'fro
+00095ea0: 6d41 6d6f 756e 7427 292c 0a20 2020 2020  mAmount'),.     
+00095eb0: 2020 2020 2020 2027 746f 4375 7272 656e         'toCurren
+00095ec0: 6379 273a 2074 6f43 6f64 652c 0a20 2020  cy': toCode,.   
+00095ed0: 2020 2020 2020 2020 2027 746f 416d 6f75           'toAmou
+00095ee0: 6e74 273a 2073 656c 662e 7361 6665 5f6e  nt': self.safe_n
+00095ef0: 756d 6265 725f 3228 636f 6e76 6572 7369  umber_2(conversi
+00095f00: 6f6e 2c20 2774 6172 6765 7441 6d6f 756e  on, 'targetAmoun
+00095f10: 7427 2c20 2774 6f41 6d6f 756e 7427 292c  t', 'toAmount'),
+00095f20: 0a20 2020 2020 2020 2020 2020 2027 7072  .            'pr
+00095f30: 6963 6527 3a20 4e6f 6e65 2c0a 2020 2020  ice': None,.    
+00095f40: 2020 2020 2020 2020 2766 6565 273a 204e          'fee': N
+00095f50: 6f6e 652c 0a20 2020 2020 2020 207d 0a    one,.        }.
```

### Comparing `ccxt-4.3.7/ccxt/async_support/binancecoinm.py` & `ccxt-4.3.8/ccxt/async_support/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/binanceus.py` & `ccxt-4.3.8/ccxt/async_support/binanceus.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/binanceusdm.py` & `ccxt-4.3.8/ccxt/async_support/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/bingx.py` & `ccxt-4.3.8/ccxt/async_support/bingx.py`

 * *Files 0% similar despite different names*

```diff
@@ -2314,15 +2314,15 @@
             #  takeProfit: '{"stopPrice":150,"workingType":"MARK_PRICE","type":"TAKE_PROFIT_MARKET","quantity":1}',
             if isinstance(takeProfit, str):
                 takeProfit = self.parse_json(takeProfit)
             takeProfitPrice = self.safe_number(takeProfit, 'stopPrice')
         return self.safe_order({
             'info': info,
             'id': self.safe_string_2(order, 'orderId', 'i'),
-            'clientOrderId': self.safe_string_n(order, ['clientOrderID', 'origClientOrderId', 'c']),
+            'clientOrderId': self.safe_string_n(order, ['clientOrderID', 'clientOrderId', 'origClientOrderId', 'c']),
             'symbol': self.safe_symbol(marketId, market, '-', marketType),
             'timestamp': timestamp,
             'datetime': self.iso8601(timestamp),
             'lastTradeTimestamp': lastTradeTimestamp,
             'lastUpdateTimestamp': self.safe_integer(order, 'updateTime'),
             'type': self.parse_order_type(self.safe_string_lower_2(order, 'type', 'o')),
             'timeInForce': self.safe_string(order, 'timeInForce'),
```

### Comparing `ccxt-4.3.7/ccxt/async_support/bit2c.py` & `ccxt-4.3.8/ccxt/async_support/bit2c.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/bitbank.py` & `ccxt-4.3.8/ccxt/async_support/bitbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/bitbns.py` & `ccxt-4.3.8/ccxt/async_support/bitbns.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/bitcoincom.py` & `ccxt-4.3.8/ccxt/async_support/bitcoincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/bitfinex.py` & `ccxt-4.3.8/ccxt/async_support/bitfinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/bitfinex2.py` & `ccxt-4.3.8/ccxt/async_support/bitfinex2.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/bitflyer.py` & `ccxt-4.3.8/ccxt/async_support/bitflyer.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/bitget.py` & `ccxt-4.3.8/ccxt/async_support/bitget.py`

 * *Files 0% similar despite different names*

```diff
@@ -8059,15 +8059,15 @@
         #             ],
         #             "endId": "1159296505255219205"
         #         }
         #     }
         #
         data = self.safe_dict(response, 'data', {})
         dataList = self.safe_list(data, 'dataList', [])
-        return self.parse_conversions(dataList, 'fromCoin', 'toCoin', since, limit)
+        return self.parse_conversions(dataList, code, 'fromCoin', 'toCoin', since, limit)
 
     def parse_conversion(self, conversion, fromCurrency: Currency = None, toCurrency: Currency = None) -> Conversion:
         #
         # fetchConvertQuote
         #
         #     {
         #         "fromCoin": "USDT",
```

### Comparing `ccxt-4.3.7/ccxt/async_support/bithumb.py` & `ccxt-4.3.8/ccxt/async_support/bithumb.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/bitmart.py` & `ccxt-4.3.8/ccxt/async_support/bitmart.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/bitmex.py` & `ccxt-4.3.8/ccxt/async_support/bitmex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/bitopro.py` & `ccxt-4.3.8/ccxt/async_support/bitopro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/bitrue.py` & `ccxt-4.3.8/ccxt/async_support/bitrue.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/bitso.py` & `ccxt-4.3.8/ccxt/async_support/bitso.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/bitstamp.py` & `ccxt-4.3.8/ccxt/async_support/bitstamp.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/bitteam.py` & `ccxt-4.3.8/ccxt/async_support/bitteam.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/bitvavo.py` & `ccxt-4.3.8/ccxt/async_support/bitvavo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/bl3p.py` & `ccxt-4.3.8/ccxt/async_support/bl3p.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/blockchaincom.py` & `ccxt-4.3.8/ccxt/async_support/blockchaincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/blofin.py` & `ccxt-4.3.8/ccxt/async_support/blofin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/btcalpha.py` & `ccxt-4.3.8/ccxt/async_support/btcalpha.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/btcbox.py` & `ccxt-4.3.8/ccxt/async_support/btcbox.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/btcmarkets.py` & `ccxt-4.3.8/ccxt/async_support/btcmarkets.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/btcturk.py` & `ccxt-4.3.8/ccxt/async_support/btcturk.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/bybit.py` & `ccxt-4.3.8/ccxt/async_support/bybit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/cex.py` & `ccxt-4.3.8/ccxt/async_support/cex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/coinbase.py` & `ccxt-4.3.8/ccxt/async_support/coinbase.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/coinbaseinternational.py` & `ccxt-4.3.8/ccxt/async_support/coinbaseinternational.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/coinbasepro.py` & `ccxt-4.3.8/ccxt/async_support/coinbasepro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/coincheck.py` & `ccxt-4.3.8/ccxt/async_support/coincheck.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/coinex.py` & `ccxt-4.3.8/ccxt/async_support/coinex.py`

 * *Files 2% similar despite different names*

```diff
@@ -1484,204 +1484,159 @@
         #     }
         #
         data = self.safe_list(response, 'data', [])
         return self.parse_ohlcvs(data, market, timeframe, since, limit)
 
     async def fetch_margin_balance(self, params={}):
         await self.load_markets()
-        symbol = self.safe_string(params, 'symbol')
-        marketId = self.safe_string(params, 'market')
-        market: Market = None
-        if symbol is not None:
-            market = self.market(symbol)
-            marketId = market['id']
-        elif marketId is None:
-            raise ArgumentsRequired(self.id + ' fetchMarginBalance() fetching a margin account requires a market parameter or a symbol parameter')
-        params = self.omit(params, ['symbol', 'market'])
-        request = {
-            'market': marketId,
-        }
-        response = await self.v1PrivateGetMarginAccount(self.extend(request, params))
+        response = await self.v2PrivateGetAssetsMarginBalance(params)
         #
-        #      {
-        #          "code":    0,
-        #           "data": {
-        #              "account_id":    126,
-        #              "leverage":    3,
-        #              "market_type":   "AAVEUSDT",
-        #              "sell_asset_type":   "AAVE",
-        #              "buy_asset_type":   "USDT",
-        #              "balance": {
-        #                  "sell_type": "0.3",     # borrowed
-        #                  "buy_type": "30"
-        #                  },
-        #              "frozen": {
-        #                  "sell_type": "0",
-        #                  "buy_type": "0"
-        #                  },
-        #              "loan": {
-        #                  "sell_type": "0.3",  # loan
-        #                  "buy_type": "0"
-        #                  },
-        #              "interest": {
-        #                  "sell_type": "0.0000125",
-        #                  "buy_type": "0"
-        #                  },
-        #              "can_transfer": {
-        #                  "sell_type": "0.02500646",
-        #                  "buy_type": "4.28635738"
-        #                  },
-        #              "warn_rate":   "",
-        #              "liquidation_price":   ""
-        #              },
-        #          "message": "Success"
-        #      }
+        #     {
+        #         "data": [
+        #             {
+        #                 "margin_account": "BTCUSDT",
+        #                 "base_ccy": "BTC",
+        #                 "quote_ccy": "USDT",
+        #                 "available": {
+        #                     "base_ccy": "0.00000026",
+        #                     "quote_ccy": "0"
+        #                 },
+        #                 "frozen": {
+        #                     "base_ccy": "0",
+        #                     "quote_ccy": "0"
+        #                 },
+        #                 "repaid": {
+        #                     "base_ccy": "0",
+        #                     "quote_ccy": "0"
+        #                 },
+        #                 "interest": {
+        #                     "base_ccy": "0",
+        #                     "quote_ccy": "0"
+        #                 },
+        #                 "rik_rate": "",
+        #                 "liq_price": ""
+        #             },
+        #         ],
+        #         "code": 0,
+        #         "message": "OK"
+        #     }
         #
         result = {'info': response}
-        data = self.safe_value(response, 'data', {})
-        free = self.safe_value(data, 'can_transfer', {})
-        total = self.safe_value(data, 'balance', {})
-        loan = self.safe_value(data, 'loan', {})
-        interest = self.safe_value(data, 'interest', {})
-        #
-        sellAccount = self.account()
-        sellCurrencyId = self.safe_string(data, 'sell_asset_type')
-        sellCurrencyCode = self.safe_currency_code(sellCurrencyId)
-        sellAccount['free'] = self.safe_string(free, 'sell_type')
-        sellAccount['total'] = self.safe_string(total, 'sell_type')
-        sellDebt = self.safe_string(loan, 'sell_type')
-        sellInterest = self.safe_string(interest, 'sell_type')
-        sellAccount['debt'] = Precise.string_add(sellDebt, sellInterest)
-        result[sellCurrencyCode] = sellAccount
-        #
-        buyAccount = self.account()
-        buyCurrencyId = self.safe_string(data, 'buy_asset_type')
-        buyCurrencyCode = self.safe_currency_code(buyCurrencyId)
-        buyAccount['free'] = self.safe_string(free, 'buy_type')
-        buyAccount['total'] = self.safe_string(total, 'buy_type')
-        buyDebt = self.safe_string(loan, 'buy_type')
-        buyInterest = self.safe_string(interest, 'buy_type')
-        buyAccount['debt'] = Precise.string_add(buyDebt, buyInterest)
-        result[buyCurrencyCode] = buyAccount
-        #
+        balances = self.safe_list(response, 'data', [])
+        for i in range(0, len(balances)):
+            entry = balances[i]
+            free = self.safe_dict(entry, 'available', {})
+            used = self.safe_dict(entry, 'frozen', {})
+            loan = self.safe_dict(entry, 'repaid', {})
+            interest = self.safe_dict(entry, 'interest', {})
+            baseAccount = self.account()
+            baseCurrencyId = self.safe_string(entry, 'base_ccy')
+            baseCurrencyCode = self.safe_currency_code(baseCurrencyId)
+            baseAccount['free'] = self.safe_string(free, 'base_ccy')
+            baseAccount['used'] = self.safe_string(used, 'base_ccy')
+            baseDebt = self.safe_string(loan, 'base_ccy')
+            baseInterest = self.safe_string(interest, 'base_ccy')
+            baseAccount['debt'] = Precise.string_add(baseDebt, baseInterest)
+            result[baseCurrencyCode] = baseAccount
         return self.safe_balance(result)
 
     async def fetch_spot_balance(self, params={}):
         await self.load_markets()
-        response = await self.v1PrivateGetBalanceInfo(params)
+        response = await self.v2PrivateGetAssetsSpotBalance(params)
         #
         #     {
-        #       "code": 0,
-        #       "data": {
-        #         "BCH": {                    # BCH account
-        #           "available": "13.60109",   # Available BCH
-        #           "frozen": "0.00000"        # Frozen BCH
-        #         },
-        #         "BTC": {                    # BTC account
-        #           "available": "32590.16",   # Available BTC
-        #           "frozen": "7000.00"        # Frozen BTC
-        #         },
-        #         "ETH": {                    # ETH account
-        #           "available": "5.06000",    # Available ETH
-        #           "frozen": "0.00000"        # Frozen ETH
-        #         }
-        #       },
-        #       "message": "Ok"
+        #         "code": 0,
+        #         "data": [
+        #             {
+        #                 "available": "0.00000046",
+        #                 "ccy": "USDT",
+        #                 "frozen": "0"
+        #             }
+        #         ],
+        #         "message": "OK"
         #     }
         #
         result = {'info': response}
-        balances = self.safe_value(response, 'data', {})
-        currencyIds = list(balances.keys())
-        for i in range(0, len(currencyIds)):
-            currencyId = currencyIds[i]
+        balances = self.safe_list(response, 'data', [])
+        for i in range(0, len(balances)):
+            entry = balances[i]
+            currencyId = self.safe_string(entry, 'ccy')
             code = self.safe_currency_code(currencyId)
-            balance = self.safe_value(balances, currencyId, {})
             account = self.account()
-            account['free'] = self.safe_string(balance, 'available')
-            account['used'] = self.safe_string(balance, 'frozen')
+            account['free'] = self.safe_string(entry, 'available')
+            account['used'] = self.safe_string(entry, 'frozen')
             result[code] = account
         return self.safe_balance(result)
 
     async def fetch_swap_balance(self, params={}):
         await self.load_markets()
-        response = await self.v1PerpetualPrivateGetAssetQuery(params)
+        response = await self.v2PrivateGetAssetsFuturesBalance(params)
         #
         #     {
         #         "code": 0,
-        #         "data": {
-        #             "USDT": {
-        #                 "available": "37.24817690383456000000",
-        #                 "balance_total": "37.24817690383456000000",
-        #                 "frozen": "0.00000000000000000000",
-        #                 "margin": "0.00000000000000000000",
-        #                 "profit_unreal": "0.00000000000000000000",
-        #                 "transfer": "37.24817690383456000000"
+        #         "data": [
+        #             {
+        #                 "available": "0.00000046",
+        #                 "ccy": "USDT",
+        #                 "frozen": "0",
+        #                 "margin": "0",
+        #                 "transferrable": "0.00000046",
+        #                 "unrealized_pnl": "0"
         #             }
-        #         },
+        #         ],
         #         "message": "OK"
         #     }
         #
         result = {'info': response}
-        balances = self.safe_value(response, 'data', {})
-        currencyIds = list(balances.keys())
-        for i in range(0, len(currencyIds)):
-            currencyId = currencyIds[i]
+        balances = self.safe_list(response, 'data', [])
+        for i in range(0, len(balances)):
+            entry = balances[i]
+            currencyId = self.safe_string(entry, 'ccy')
             code = self.safe_currency_code(currencyId)
-            balance = self.safe_value(balances, currencyId, {})
             account = self.account()
-            account['free'] = self.safe_string(balance, 'available')
-            account['used'] = self.safe_string(balance, 'frozen')
-            account['total'] = self.safe_string(balance, 'balance_total')
+            account['free'] = self.safe_string(entry, 'available')
+            account['used'] = self.safe_string(entry, 'frozen')
             result[code] = account
         return self.safe_balance(result)
 
     async def fetch_financial_balance(self, params={}):
         await self.load_markets()
-        response = await self.v1PrivateGetAccountInvestmentBalance(params)
+        response = await self.v2PrivateGetAssetsFinancialBalance(params)
         #
         #     {
-        #          "code": 0,
-        #          "data": [
-        #              {
-        #                  "asset": "CET",
-        #                  "available": "0",
-        #                  "frozen": "0",
-        #                  "lock": "0",
-        #              },
-        #              {
-        #                  "asset": "USDT",
-        #                  "available": "999900",
-        #                  "frozen": "0",
-        #                  "lock": "0"
-        #              }
-        #          ],
-        #          "message": "Success"
-        #      }
+        #         "code": 0,
+        #         "data": [
+        #             {
+        #                 "available": "0.00000046",
+        #                 "ccy": "USDT",
+        #                 "frozen": "0"
+        #             }
+        #         ],
+        #         "message": "OK"
+        #     }
         #
         result = {'info': response}
-        balances = self.safe_value(response, 'data', {})
+        balances = self.safe_list(response, 'data', [])
         for i in range(0, len(balances)):
-            balance = balances[i]
-            currencyId = self.safe_string(balance, 'asset')
+            entry = balances[i]
+            currencyId = self.safe_string(entry, 'ccy')
             code = self.safe_currency_code(currencyId)
             account = self.account()
-            account['free'] = self.safe_string(balance, 'available')
-            frozen = self.safe_string(balance, 'frozen')
-            locked = self.safe_string(balance, 'lock')
-            account['used'] = Precise.string_add(frozen, locked)
+            account['free'] = self.safe_string(entry, 'available')
+            account['used'] = self.safe_string(entry, 'frozen')
             result[code] = account
         return self.safe_balance(result)
 
     async def fetch_balance(self, params={}) -> Balances:
         """
         query for balance and get the amount of funds available for trading or funds locked in orders
-        :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot002_account001_account_info         # spot
-        :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot002_account004_investment_balance   # financial
-        :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot002_account006_margin_account       # margin
-        :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http016_asset_query       # swap
+        :see: https://docs.coinex.com/api/v2/assets/balance/http/get-spot-balance         # spot
+        :see: https://docs.coinex.com/api/v2/assets/balance/http/get-futures-balance      # swap
+        :see: https://docs.coinex.com/api/v2/assets/balance/http/get-marigin-balance      # margin
+        :see: https://docs.coinex.com/api/v2/assets/balance/http/get-financial-balance    # financial
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :param str [params.type]: 'margin', 'swap', 'financial', or 'spot'
         :returns dict: a `balance structure <https://docs.ccxt.com/#/?id=balance-structure>`
         """
         marketType = None
         marketType, params = self.handle_market_type_and_params('fetchBalance', None, params)
         marginMode = None
@@ -5444,23 +5399,27 @@
                     url += '?' + urlencoded
                 else:
                     body = self.json(query)
             elif version == 'v2':
                 self.check_required_credentials()
                 query = self.keysort(query)
                 urlencoded = self.rawencode(query)
-                preparedString = method + '/' + version + '/' + path + '?' + urlencoded + nonce + self.secret
+                preparedString = method + '/' + version + '/' + path
+                if urlencoded:
+                    preparedString += '?' + urlencoded
+                preparedString += nonce + self.secret
                 signature = self.hash(self.encode(preparedString), 'sha256')
                 headers = {
                     'X-COINEX-KEY': self.apiKey,
                     'X-COINEX-SIGN': signature,
                     'X-COINEX-TIMESTAMP': nonce,
                 }
                 if (method == 'GET') or (method == 'DELETE') or (method == 'PUT'):
-                    url += '?' + urlencoded
+                    if urlencoded:
+                        url += '?' + urlencoded
                 else:
                     body = self.json(query)
         return {'url': url, 'method': method, 'body': body, 'headers': headers}
 
     def handle_errors(self, httpCode, reason, url, method, headers, body, response, requestHeaders, requestBody):
         if response is None:
             return None
```

### Comparing `ccxt-4.3.7/ccxt/async_support/coinlist.py` & `ccxt-4.3.8/ccxt/async_support/coinlist.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/coinmate.py` & `ccxt-4.3.8/ccxt/async_support/coinmate.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/coinmetro.py` & `ccxt-4.3.8/ccxt/async_support/coinmetro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/coinone.py` & `ccxt-4.3.8/ccxt/async_support/coinone.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/coinsph.py` & `ccxt-4.3.8/ccxt/async_support/coinsph.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/coinspot.py` & `ccxt-4.3.8/ccxt/async_support/coinspot.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/cryptocom.py` & `ccxt-4.3.8/ccxt/async_support/cryptocom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/currencycom.py` & `ccxt-4.3.8/ccxt/async_support/currencycom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/delta.py` & `ccxt-4.3.8/ccxt/async_support/delta.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/deribit.py` & `ccxt-4.3.8/ccxt/async_support/deribit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/digifinex.py` & `ccxt-4.3.8/ccxt/async_support/digifinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/exmo.py` & `ccxt-4.3.8/ccxt/async_support/exmo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/flowbtc.py` & `ccxt-4.3.8/ccxt/async_support/flowbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/fmfwio.py` & `ccxt-4.3.8/ccxt/async_support/fmfwio.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/gate.py` & `ccxt-4.3.8/ccxt/async_support/gate.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/gemini.py` & `ccxt-4.3.8/ccxt/async_support/gemini.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/hitbtc.py` & `ccxt-4.3.8/ccxt/async_support/hitbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/hollaex.py` & `ccxt-4.3.8/ccxt/async_support/hollaex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/htx.py` & `ccxt-4.3.8/ccxt/async_support/htx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/huobijp.py` & `ccxt-4.3.8/ccxt/async_support/huobijp.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/hyperliquid.py` & `ccxt-4.3.8/ccxt/async_support/hyperliquid.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/idex.py` & `ccxt-4.3.8/ccxt/async_support/idex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/independentreserve.py` & `ccxt-4.3.8/ccxt/async_support/independentreserve.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/indodax.py` & `ccxt-4.3.8/ccxt/async_support/indodax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/kraken.py` & `ccxt-4.3.8/ccxt/async_support/kraken.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/krakenfutures.py` & `ccxt-4.3.8/ccxt/async_support/krakenfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/kucoin.py` & `ccxt-4.3.8/ccxt/async_support/kucoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/kucoinfutures.py` & `ccxt-4.3.8/ccxt/async_support/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/kuna.py` & `ccxt-4.3.8/ccxt/async_support/kuna.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/latoken.py` & `ccxt-4.3.8/ccxt/async_support/latoken.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/lbank.py` & `ccxt-4.3.8/ccxt/async_support/lbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/luno.py` & `ccxt-4.3.8/ccxt/async_support/luno.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/lykke.py` & `ccxt-4.3.8/ccxt/async_support/lykke.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/mercado.py` & `ccxt-4.3.8/ccxt/async_support/mercado.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/mexc.py` & `ccxt-4.3.8/ccxt/async_support/mexc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/ndax.py` & `ccxt-4.3.8/ccxt/async_support/ndax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/novadax.py` & `ccxt-4.3.8/ccxt/async_support/novadax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/oceanex.py` & `ccxt-4.3.8/ccxt/async_support/oceanex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/okcoin.py` & `ccxt-4.3.8/ccxt/async_support/okcoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/okx.py` & `ccxt-4.3.8/ccxt/async_support/okx.py`

 * *Files 0% similar despite different names*

```diff
@@ -7394,15 +7394,15 @@
         #                 "ts": "1646188520000"
         #             }
         #         ],
         #         "msg": ""
         #     }
         #
         rows = self.safe_list(response, 'data', [])
-        return self.parse_conversions(rows, 'baseCcy', 'quoteCcy', since, limit)
+        return self.parse_conversions(rows, code, 'baseCcy', 'quoteCcy', since, limit)
 
     def parse_conversion(self, conversion, fromCurrency: Currency = None, toCurrency: Currency = None) -> Conversion:
         #
         # fetchConvertQuote
         #
         #     {
         #         "baseCcy": "ETH",
```

### Comparing `ccxt-4.3.7/ccxt/async_support/onetrading.py` & `ccxt-4.3.8/ccxt/async_support/onetrading.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/p2b.py` & `ccxt-4.3.8/ccxt/async_support/p2b.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/paymium.py` & `ccxt-4.3.8/ccxt/async_support/paymium.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/phemex.py` & `ccxt-4.3.8/ccxt/async_support/phemex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/poloniex.py` & `ccxt-4.3.8/ccxt/async_support/poloniex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/poloniexfutures.py` & `ccxt-4.3.8/ccxt/async_support/poloniexfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/probit.py` & `ccxt-4.3.8/ccxt/async_support/probit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/timex.py` & `ccxt-4.3.8/ccxt/async_support/timex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/tokocrypto.py` & `ccxt-4.3.8/ccxt/async_support/tokocrypto.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/tradeogre.py` & `ccxt-4.3.8/ccxt/async_support/tradeogre.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/upbit.py` & `ccxt-4.3.8/ccxt/async_support/upbit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/wavesexchange.py` & `ccxt-4.3.8/ccxt/async_support/wavesexchange.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/wazirx.py` & `ccxt-4.3.8/ccxt/async_support/wazirx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/whitebit.py` & `ccxt-4.3.8/ccxt/async_support/whitebit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/woo.py` & `ccxt-4.3.8/ccxt/async_support/woo.py`

 * *Files 0% similar despite different names*

```diff
@@ -2960,15 +2960,15 @@
         #                 ...
         #             ]
         #         }
         #     }
         #
         data = self.safe_dict(response, 'data', {})
         rows = self.safe_list(data, 'tradeVos', [])
-        return self.parse_conversions(rows, 'sellAsset', 'buyAsset', since, limit)
+        return self.parse_conversions(rows, code, 'sellAsset', 'buyAsset', since, limit)
 
     def parse_conversion(self, conversion, fromCurrency: Currency = None, toCurrency: Currency = None) -> Conversion:
         #
         # fetchConvertQuote
         #
         #     {
         #         "quoteId": 123123123,
```

### Comparing `ccxt-4.3.7/ccxt/async_support/yobit.py` & `ccxt-4.3.8/ccxt/async_support/yobit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/zaif.py` & `ccxt-4.3.8/ccxt/async_support/zaif.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/async_support/zonda.py` & `ccxt-4.3.8/ccxt/async_support/zonda.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/base/__init__.py` & `ccxt-4.3.8/ccxt/base/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/base/decimal_to_precision.py` & `ccxt-4.3.8/ccxt/base/decimal_to_precision.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/base/errors.py` & `ccxt-4.3.8/ccxt/base/errors.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/base/exchange.py` & `ccxt-4.3.8/ccxt/base/exchange.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """Base exchange class"""
 
 # -----------------------------------------------------------------------------
 
-__version__ = '4.3.7'
+__version__ = '4.3.8'
 
 # -----------------------------------------------------------------------------
 
 from ccxt.base.errors import ExchangeError
 from ccxt.base.errors import NetworkError
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import AuthenticationError
@@ -5679,15 +5679,15 @@
             if (symbols is None) or self.in_array(market['symbol'], symbols):
                 leverageStructures[market['symbol']] = self.parse_leverage(info, market)
         return leverageStructures
 
     def parse_leverage(self, leverage, market: Market = None):
         raise NotSupported(self.id + ' parseLeverage() is not supported yet')
 
-    def parse_conversions(self, conversions: List[Any], fromCurrencyKey: Str = None, toCurrencyKey: Str = None, since: Int = None, limit: Int = None, params={}):
+    def parse_conversions(self, conversions: List[Any], code: Str = None, fromCurrencyKey: Str = None, toCurrencyKey: Str = None, since: Int = None, limit: Int = None, params={}):
         conversions = self.to_array(conversions)
         result = []
         fromCurrency = None
         toCurrency = None
         for i in range(0, len(conversions)):
             entry = conversions[i]
             fromId = self.safe_string(entry, fromCurrencyKey)
@@ -5695,16 +5695,24 @@
             if fromId is not None:
                 fromCurrency = self.currency(fromId)
             if toId is not None:
                 toCurrency = self.currency(toId)
             conversion = self.extend(self.parseConversion(entry, fromCurrency, toCurrency), params)
             result.append(conversion)
         sorted = self.sort_by(result, 'timestamp')
-        code = fromCurrency['code'] if (fromCurrency is not None) else None
-        return self.filter_by_currency_since_limit(sorted, code, since, limit)
+        currency = None
+        if code is not None:
+            currency = self.currency(code)
+            code = currency['code']
+        if code is None:
+            return self.filter_by_since_limit(sorted, since, limit)
+        fromConversion = self.filter_by(sorted, 'fromCurrency', code)
+        toConversion = self.filter_by(sorted, 'toCurrency', code)
+        both = self.array_concat(fromConversion, toConversion)
+        return self.filter_by_since_limit(both, since, limit)
 
     def parse_conversion(self, conversion, fromCurrency: Currency = None, toCurrency: Currency = None):
         raise NotSupported(self.id + ' parseConversion() is not supported yet')
 
     def convert_expire_date(self, date: str):
         # parse YYMMDD to datetime string
         year = date[0:2]
```

### Comparing `ccxt-4.3.7/ccxt/base/precise.py` & `ccxt-4.3.8/ccxt/base/precise.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/base/types.py` & `ccxt-4.3.8/ccxt/base/types.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/bequant.py` & `ccxt-4.3.8/ccxt/bequant.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/bigone.py` & `ccxt-4.3.8/ccxt/bigone.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/binance.py` & `ccxt-4.3.8/ccxt/binance.py`

 * *Files 0% similar despite different names*

```diff
@@ -38015,209 +38015,210 @@
 000947e0: 2020 2020 2020 2020 2020 2023 0a20 2020             #.   
 000947f0: 2020 2020 2072 6f77 7320 3d20 7365 6c66       rows = self
 00094800: 2e73 6166 655f 6c69 7374 2872 6573 706f  .safe_list(respo
 00094810: 6e73 652c 2072 6573 706f 6e73 6551 7565  nse, responseQue
 00094820: 7279 2c20 5b5d 290a 2020 2020 2020 2020  ry, []).        
 00094830: 7265 7475 726e 2073 656c 662e 7061 7273  return self.pars
 00094840: 655f 636f 6e76 6572 7369 6f6e 7328 726f  e_conversions(ro
-00094850: 7773 2c20 6672 6f6d 4375 7272 656e 6379  ws, fromCurrency
-00094860: 4b65 792c 2074 6f43 7572 7265 6e63 794b  Key, toCurrencyK
-00094870: 6579 2c20 7369 6e63 652c 206c 696d 6974  ey, since, limit
-00094880: 290a 0a20 2020 2064 6566 2070 6172 7365  )..    def parse
-00094890: 5f63 6f6e 7665 7273 696f 6e28 7365 6c66  _conversion(self
-000948a0: 2c20 636f 6e76 6572 7369 6f6e 2c20 6672  , conversion, fr
-000948b0: 6f6d 4375 7272 656e 6379 3a20 4375 7272  omCurrency: Curr
-000948c0: 656e 6379 203d 204e 6f6e 652c 2074 6f43  ency = None, toC
-000948d0: 7572 7265 6e63 793a 2043 7572 7265 6e63  urrency: Currenc
-000948e0: 7920 3d20 4e6f 6e65 2920 2d3e 2043 6f6e  y = None) -> Con
-000948f0: 7665 7273 696f 6e3a 0a20 2020 2020 2020  version:.       
-00094900: 2023 0a20 2020 2020 2020 2023 2066 6574   #.        # fet
-00094910: 6368 436f 6e76 6572 7451 756f 7465 0a20  chConvertQuote. 
-00094920: 2020 2020 2020 2023 0a20 2020 2020 2020         #.       
-00094930: 2023 2020 2020 207b 0a20 2020 2020 2020   #     {.       
-00094940: 2023 2020 2020 2020 2020 2022 7175 6f74   #         "quot
-00094950: 6549 6422 3a22 3132 3431 3535 3732 3536  eId":"1241557256
-00094960: 3422 2c0a 2020 2020 2020 2020 2320 2020  4",.        #   
-00094970: 2020 2020 2020 2272 6174 696f 223a 2233        "ratio":"3
-00094980: 3831 3633 2e37 222c 0a20 2020 2020 2020  8163.7",.       
-00094990: 2023 2020 2020 2020 2020 2022 696e 7665   #         "inve
-000949a0: 7273 6552 6174 696f 223a 2230 2e30 3030  rseRatio":"0.000
-000949b0: 3032 3632 222c 0a20 2020 2020 2020 2023  0262",.        #
-000949c0: 2020 2020 2020 2020 2022 7661 6c69 6454           "validT
-000949d0: 696d 6573 7461 6d70 223a 3136 3233 3331  imestamp":162331
-000949e0: 3934 3631 3637 302c 0a20 2020 2020 2020  9461670,.       
-000949f0: 2023 2020 2020 2020 2020 2022 746f 416d   #         "toAm
-00094a00: 6f75 6e74 223a 2233 3831 362e 3337 222c  ount":"3816.37",
-00094a10: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
-00094a20: 2020 2022 6672 6f6d 416d 6f75 6e74 223a     "fromAmount":
-00094a30: 2230 2e31 220a 2020 2020 2020 2020 2320  "0.1".        # 
-00094a40: 2020 2020 7d0a 2020 2020 2020 2020 230a      }.        #.
-00094a50: 2020 2020 2020 2020 2320 6372 6561 7465          # create
-00094a60: 436f 6e76 6572 7454 7261 6465 0a20 2020  ConvertTrade.   
-00094a70: 2020 2020 2023 0a20 2020 2020 2020 2023       #.        #
-00094a80: 2020 2020 207b 0a20 2020 2020 2020 2023       {.        #
-00094a90: 2020 2020 2020 2020 2022 6f72 6465 7249           "orderI
-00094aa0: 6422 3a22 3933 3332 3536 3237 3834 3236  d":"933256278426
-00094ab0: 3237 3434 3236 222c 0a20 2020 2020 2020  274426",.       
-00094ac0: 2023 2020 2020 2020 2020 2022 6372 6561   #         "crea
-00094ad0: 7465 5469 6d65 223a 3136 3233 3338 3133  teTime":16233813
-00094ae0: 3330 3437 322c 0a20 2020 2020 2020 2023  30472,.        #
-00094af0: 2020 2020 2020 2020 2022 6f72 6465 7253           "orderS
-00094b00: 7461 7475 7322 3a22 5052 4f43 4553 5322  tatus":"PROCESS"
-00094b10: 0a20 2020 2020 2020 2023 2020 2020 207d  .        #     }
-00094b20: 0a20 2020 2020 2020 2023 0a20 2020 2020  .        #.     
-00094b30: 2020 2023 2063 7265 6174 6543 6f6e 7665     # createConve
-00094b40: 7274 5472 6164 6520 4255 5344 0a20 2020  rtTrade BUSD.   
-00094b50: 2020 2020 2023 0a20 2020 2020 2020 2023       #.        #
-00094b60: 2020 2020 207b 0a20 2020 2020 2020 2023       {.        #
-00094b70: 2020 2020 2020 2020 2022 7472 616e 4964           "tranId
-00094b80: 223a 2031 3138 3236 3334 3037 3131 392c  ": 118263407119,
-00094b90: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
-00094ba0: 2020 2022 7374 6174 7573 223a 2022 5322     "status": "S"
-00094bb0: 0a20 2020 2020 2020 2023 2020 2020 207d  .        #     }
-00094bc0: 0a20 2020 2020 2020 2023 0a20 2020 2020  .        #.     
-00094bd0: 2020 2023 2066 6574 6368 436f 6e76 6572     # fetchConver
-00094be0: 7454 7261 6465 2c20 6665 7463 6843 6f6e  tTrade, fetchCon
-00094bf0: 7665 7274 5472 6164 6548 6973 746f 7279  vertTradeHistory
-00094c00: 2042 5553 440a 2020 2020 2020 2020 230a   BUSD.        #.
-00094c10: 2020 2020 2020 2020 2320 2020 2020 7b0a          #     {.
-00094c20: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-00094c30: 2020 2274 7261 6e49 6422 3a20 3131 3832    "tranId": 1182
-00094c40: 3633 3631 3539 3931 2c0a 2020 2020 2020  63615991,.      
-00094c50: 2020 2320 2020 2020 2020 2020 2274 7970    #         "typ
-00094c60: 6522 3a20 3234 342c 0a20 2020 2020 2020  e": 244,.       
-00094c70: 2023 2020 2020 2020 2020 2022 7469 6d65   #         "time
-00094c80: 223a 2031 3636 3434 3432 3037 3830 3030  ": 1664442078000
-00094c90: 2c0a 2020 2020 2020 2020 2320 2020 2020  ,.        #     
-00094ca0: 2020 2020 2264 6564 7563 7465 6441 7373      "deductedAss
-00094cb0: 6574 223a 2022 4255 5344 222c 0a20 2020  et": "BUSD",.   
-00094cc0: 2020 2020 2023 2020 2020 2020 2020 2022       #         "
-00094cd0: 6465 6475 6374 6564 416d 6f75 6e74 223a  deductedAmount":
-00094ce0: 2022 3122 2c0a 2020 2020 2020 2020 2320   "1",.        # 
-00094cf0: 2020 2020 2020 2020 2274 6172 6765 7441          "targetA
-00094d00: 7373 6574 223a 2022 5553 4443 222c 0a20  sset": "USDC",. 
-00094d10: 2020 2020 2020 2023 2020 2020 2020 2020         #        
-00094d20: 2022 7461 7267 6574 416d 6f75 6e74 223a   "targetAmount":
-00094d30: 2022 3122 2c0a 2020 2020 2020 2020 2320   "1",.        # 
-00094d40: 2020 2020 2020 2020 2273 7461 7475 7322          "status"
-00094d50: 3a20 2253 222c 0a20 2020 2020 2020 2023  : "S",.        #
-00094d60: 2020 2020 2020 2020 2022 6163 636f 756e           "accoun
-00094d70: 7454 7970 6522 3a20 224d 4149 4e22 0a20  tType": "MAIN". 
-00094d80: 2020 2020 2020 2023 2020 2020 207d 0a20         #     }. 
-00094d90: 2020 2020 2020 2023 0a20 2020 2020 2020         #.       
-00094da0: 2023 2066 6574 6368 436f 6e76 6572 7454   # fetchConvertT
-00094db0: 7261 6465 0a20 2020 2020 2020 2023 0a20  rade.        #. 
-00094dc0: 2020 2020 2020 2023 2020 2020 207b 0a20         #     {. 
-00094dd0: 2020 2020 2020 2023 2020 2020 2020 2020         #        
-00094de0: 2022 6f72 6465 7249 6422 3a39 3333 3235   "orderId":93325
-00094df0: 3632 3738 3432 3632 3734 3432 362c 0a20  6278426274426,. 
-00094e00: 2020 2020 2020 2023 2020 2020 2020 2020         #        
-00094e10: 2022 6f72 6465 7253 7461 7475 7322 3a22   "orderStatus":"
-00094e20: 5355 4343 4553 5322 2c0a 2020 2020 2020  SUCCESS",.      
-00094e30: 2020 2320 2020 2020 2020 2020 2266 726f    #         "fro
-00094e40: 6d41 7373 6574 223a 2242 5443 222c 0a20  mAsset":"BTC",. 
-00094e50: 2020 2020 2020 2023 2020 2020 2020 2020         #        
-00094e60: 2022 6672 6f6d 416d 6f75 6e74 223a 2230   "fromAmount":"0
-00094e70: 2e30 3030 3534 3431 3422 2c0a 2020 2020  .00054414",.    
-00094e80: 2020 2020 2320 2020 2020 2020 2020 2274      #         "t
-00094e90: 6f41 7373 6574 223a 2255 5344 5422 2c0a  oAsset":"USDT",.
-00094ea0: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-00094eb0: 2020 2274 6f41 6d6f 756e 7422 3a22 3230    "toAmount":"20
-00094ec0: 222c 0a20 2020 2020 2020 2023 2020 2020  ",.        #    
-00094ed0: 2020 2020 2022 7261 7469 6f22 3a22 3336       "ratio":"36
-00094ee0: 3735 3522 2c0a 2020 2020 2020 2020 2320  755",.        # 
-00094ef0: 2020 2020 2020 2020 2269 6e76 6572 7365          "inverse
-00094f00: 5261 7469 6f22 3a22 302e 3030 3030 3237  Ratio":"0.000027
-00094f10: 3231 222c 0a20 2020 2020 2020 2023 2020  21",.        #  
-00094f20: 2020 2020 2020 2022 6372 6561 7465 5469         "createTi
-00094f30: 6d65 223a 3136 3233 3338 3133 3330 3437  me":162338133047
-00094f40: 320a 2020 2020 2020 2020 2320 2020 2020  2.        #     
-00094f50: 7d0a 2020 2020 2020 2020 230a 2020 2020  }.        #.    
-00094f60: 2020 2020 2320 6665 7463 6843 6f6e 7665      # fetchConve
-00094f70: 7274 5472 6164 6548 6973 746f 7279 0a20  rtTradeHistory. 
-00094f80: 2020 2020 2020 2023 0a20 2020 2020 2020         #.       
-00094f90: 2023 2020 2020 207b 0a20 2020 2020 2020   #     {.       
-00094fa0: 2023 2020 2020 2020 2020 2022 7175 6f74   #         "quot
-00094fb0: 6549 6422 3a20 2266 3362 3931 6335 3235  eId": "f3b91c525
-00094fc0: 6232 3634 3463 3762 6331 6531 6364 3331  b2644c7bc1e1cd31
-00094fd0: 6236 6531 6161 3622 2c0a 2020 2020 2020  b6e1aa6",.      
-00094fe0: 2020 2320 2020 2020 2020 2020 226f 7264    #         "ord
-00094ff0: 6572 4964 223a 2039 3430 3730 3834 3037  erId": 940708407
-00095000: 3436 3230 3837 3139 352c 0a20 2020 2020  462087195,.     
-00095010: 2020 2023 2020 2020 2020 2020 2022 6f72     #         "or
-00095020: 6465 7253 7461 7475 7322 3a20 2253 5543  derStatus": "SUC
-00095030: 4345 5353 222c 0a20 2020 2020 2020 2023  CESS",.        #
-00095040: 2020 2020 2020 2020 2022 6672 6f6d 4173           "fromAs
-00095050: 7365 7422 3a20 2255 5344 5422 2c0a 2020  set": "USDT",.  
-00095060: 2020 2020 2020 2320 2020 2020 2020 2020        #         
-00095070: 2266 726f 6d41 6d6f 756e 7422 3a20 2232  "fromAmount": "2
-00095080: 3022 2c0a 2020 2020 2020 2020 2320 2020  0",.        #   
-00095090: 2020 2020 2020 2274 6f41 7373 6574 223a        "toAsset":
-000950a0: 2022 424e 4222 2c0a 2020 2020 2020 2020   "BNB",.        
-000950b0: 2320 2020 2020 2020 2020 2274 6f41 6d6f  #         "toAmo
-000950c0: 756e 7422 3a20 2230 2e30 3631 3534 3033  unt": "0.0615403
-000950d0: 3622 2c0a 2020 2020 2020 2020 2320 2020  6",.        #   
-000950e0: 2020 2020 2020 2272 6174 696f 223a 2022        "ratio": "
-000950f0: 302e 3030 3330 3737 3032 222c 0a20 2020  0.00307702",.   
-00095100: 2020 2020 2023 2020 2020 2020 2020 2022       #         "
-00095110: 696e 7665 7273 6552 6174 696f 223a 2022  inverseRatio": "
-00095120: 3332 342e 3939 222c 0a20 2020 2020 2020  324.99",.       
-00095130: 2023 2020 2020 2020 2020 2022 6372 6561   #         "crea
-00095140: 7465 5469 6d65 223a 2031 3632 3432 3438  teTime": 1624248
-00095150: 3837 3231 3834 0a20 2020 2020 2020 2023  872184.        #
-00095160: 2020 2020 207d 0a20 2020 2020 2020 2023       }.        #
-00095170: 0a20 2020 2020 2020 2074 696d 6573 7461  .        timesta
-00095180: 6d70 203d 2073 656c 662e 7361 6665 5f69  mp = self.safe_i
-00095190: 6e74 6567 6572 5f6e 2863 6f6e 7665 7273  nteger_n(convers
-000951a0: 696f 6e2c 205b 2774 696d 6527 2c20 2776  ion, ['time', 'v
-000951b0: 616c 6964 5469 6d65 7374 616d 7027 2c20  alidTimestamp', 
-000951c0: 2763 7265 6174 6554 696d 6527 5d29 0a20  'createTime']). 
-000951d0: 2020 2020 2020 2066 726f 6d43 7572 203d         fromCur =
-000951e0: 2073 656c 662e 7361 6665 5f73 7472 696e   self.safe_strin
-000951f0: 675f 3228 636f 6e76 6572 7369 6f6e 2c20  g_2(conversion, 
-00095200: 2764 6564 7563 7465 6441 7373 6574 272c  'deductedAsset',
-00095210: 2027 6672 6f6d 4173 7365 7427 290a 2020   'fromAsset').  
-00095220: 2020 2020 2020 6672 6f6d 436f 6465 203d        fromCode =
-00095230: 2073 656c 662e 7361 6665 5f63 7572 7265   self.safe_curre
-00095240: 6e63 795f 636f 6465 2866 726f 6d43 7572  ncy_code(fromCur
-00095250: 2c20 6672 6f6d 4375 7272 656e 6379 290a  , fromCurrency).
-00095260: 2020 2020 2020 2020 746f 203d 2073 656c          to = sel
-00095270: 662e 7361 6665 5f73 7472 696e 675f 3228  f.safe_string_2(
-00095280: 636f 6e76 6572 7369 6f6e 2c20 2774 6172  conversion, 'tar
-00095290: 6765 7441 7373 6574 272c 2027 746f 4173  getAsset', 'toAs
-000952a0: 7365 7427 290a 2020 2020 2020 2020 746f  set').        to
-000952b0: 436f 6465 203d 2073 656c 662e 7361 6665  Code = self.safe
-000952c0: 5f63 7572 7265 6e63 795f 636f 6465 2874  _currency_code(t
-000952d0: 6f2c 2074 6f43 7572 7265 6e63 7929 0a20  o, toCurrency). 
-000952e0: 2020 2020 2020 2072 6574 7572 6e20 7b0a         return {.
-000952f0: 2020 2020 2020 2020 2020 2020 2769 6e66              'inf
-00095300: 6f27 3a20 636f 6e76 6572 7369 6f6e 2c0a  o': conversion,.
-00095310: 2020 2020 2020 2020 2020 2020 2774 696d              'tim
-00095320: 6573 7461 6d70 273a 2074 696d 6573 7461  estamp': timesta
-00095330: 6d70 2c0a 2020 2020 2020 2020 2020 2020  mp,.            
-00095340: 2764 6174 6574 696d 6527 3a20 7365 6c66  'datetime': self
-00095350: 2e69 736f 3836 3031 2874 696d 6573 7461  .iso8601(timesta
-00095360: 6d70 292c 0a20 2020 2020 2020 2020 2020  mp),.           
-00095370: 2027 6964 273a 2073 656c 662e 7361 6665   'id': self.safe
-00095380: 5f73 7472 696e 675f 6e28 636f 6e76 6572  _string_n(conver
-00095390: 7369 6f6e 2c20 5b27 7472 616e 4964 272c  sion, ['tranId',
-000953a0: 2027 6f72 6465 7249 6427 2c20 2771 756f   'orderId', 'quo
-000953b0: 7465 4964 275d 292c 0a20 2020 2020 2020  teId']),.       
-000953c0: 2020 2020 2027 6672 6f6d 4375 7272 656e       'fromCurren
-000953d0: 6379 273a 2066 726f 6d43 6f64 652c 0a20  cy': fromCode,. 
-000953e0: 2020 2020 2020 2020 2020 2027 6672 6f6d             'from
-000953f0: 416d 6f75 6e74 273a 2073 656c 662e 7361  Amount': self.sa
-00095400: 6665 5f6e 756d 6265 725f 3228 636f 6e76  fe_number_2(conv
-00095410: 6572 7369 6f6e 2c20 2764 6564 7563 7465  ersion, 'deducte
-00095420: 6441 6d6f 756e 7427 2c20 2766 726f 6d41  dAmount', 'fromA
-00095430: 6d6f 756e 7427 292c 0a20 2020 2020 2020  mount'),.       
-00095440: 2020 2020 2027 746f 4375 7272 656e 6379       'toCurrency
-00095450: 273a 2074 6f43 6f64 652c 0a20 2020 2020  ': toCode,.     
-00095460: 2020 2020 2020 2027 746f 416d 6f75 6e74         'toAmount
-00095470: 273a 2073 656c 662e 7361 6665 5f6e 756d  ': self.safe_num
-00095480: 6265 725f 3228 636f 6e76 6572 7369 6f6e  ber_2(conversion
-00095490: 2c20 2774 6172 6765 7441 6d6f 756e 7427  , 'targetAmount'
-000954a0: 2c20 2774 6f41 6d6f 756e 7427 292c 0a20  , 'toAmount'),. 
-000954b0: 2020 2020 2020 2020 2020 2027 7072 6963             'pric
-000954c0: 6527 3a20 4e6f 6e65 2c0a 2020 2020 2020  e': None,.      
-000954d0: 2020 2020 2020 2766 6565 273a 204e 6f6e        'fee': Non
-000954e0: 652c 0a20 2020 2020 2020 207d 0a         e,.        }.
+00094850: 7773 2c20 636f 6465 2c20 6672 6f6d 4375  ws, code, fromCu
+00094860: 7272 656e 6379 4b65 792c 2074 6f43 7572  rrencyKey, toCur
+00094870: 7265 6e63 794b 6579 2c20 7369 6e63 652c  rencyKey, since,
+00094880: 206c 696d 6974 290a 0a20 2020 2064 6566   limit)..    def
+00094890: 2070 6172 7365 5f63 6f6e 7665 7273 696f   parse_conversio
+000948a0: 6e28 7365 6c66 2c20 636f 6e76 6572 7369  n(self, conversi
+000948b0: 6f6e 2c20 6672 6f6d 4375 7272 656e 6379  on, fromCurrency
+000948c0: 3a20 4375 7272 656e 6379 203d 204e 6f6e  : Currency = Non
+000948d0: 652c 2074 6f43 7572 7265 6e63 793a 2043  e, toCurrency: C
+000948e0: 7572 7265 6e63 7920 3d20 4e6f 6e65 2920  urrency = None) 
+000948f0: 2d3e 2043 6f6e 7665 7273 696f 6e3a 0a20  -> Conversion:. 
+00094900: 2020 2020 2020 2023 0a20 2020 2020 2020         #.       
+00094910: 2023 2066 6574 6368 436f 6e76 6572 7451   # fetchConvertQ
+00094920: 756f 7465 0a20 2020 2020 2020 2023 0a20  uote.        #. 
+00094930: 2020 2020 2020 2023 2020 2020 207b 0a20         #     {. 
+00094940: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+00094950: 2022 7175 6f74 6549 6422 3a22 3132 3431   "quoteId":"1241
+00094960: 3535 3732 3536 3422 2c0a 2020 2020 2020  5572564",.      
+00094970: 2020 2320 2020 2020 2020 2020 2272 6174    #         "rat
+00094980: 696f 223a 2233 3831 3633 2e37 222c 0a20  io":"38163.7",. 
+00094990: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+000949a0: 2022 696e 7665 7273 6552 6174 696f 223a   "inverseRatio":
+000949b0: 2230 2e30 3030 3032 3632 222c 0a20 2020  "0.0000262",.   
+000949c0: 2020 2020 2023 2020 2020 2020 2020 2022       #         "
+000949d0: 7661 6c69 6454 696d 6573 7461 6d70 223a  validTimestamp":
+000949e0: 3136 3233 3331 3934 3631 3637 302c 0a20  1623319461670,. 
+000949f0: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+00094a00: 2022 746f 416d 6f75 6e74 223a 2233 3831   "toAmount":"381
+00094a10: 362e 3337 222c 0a20 2020 2020 2020 2023  6.37",.        #
+00094a20: 2020 2020 2020 2020 2022 6672 6f6d 416d           "fromAm
+00094a30: 6f75 6e74 223a 2230 2e31 220a 2020 2020  ount":"0.1".    
+00094a40: 2020 2020 2320 2020 2020 7d0a 2020 2020      #     }.    
+00094a50: 2020 2020 230a 2020 2020 2020 2020 2320      #.        # 
+00094a60: 6372 6561 7465 436f 6e76 6572 7454 7261  createConvertTra
+00094a70: 6465 0a20 2020 2020 2020 2023 0a20 2020  de.        #.   
+00094a80: 2020 2020 2023 2020 2020 207b 0a20 2020       #     {.   
+00094a90: 2020 2020 2023 2020 2020 2020 2020 2022       #         "
+00094aa0: 6f72 6465 7249 6422 3a22 3933 3332 3536  orderId":"933256
+00094ab0: 3237 3834 3236 3237 3434 3236 222c 0a20  278426274426",. 
+00094ac0: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+00094ad0: 2022 6372 6561 7465 5469 6d65 223a 3136   "createTime":16
+00094ae0: 3233 3338 3133 3330 3437 322c 0a20 2020  23381330472,.   
+00094af0: 2020 2020 2023 2020 2020 2020 2020 2022       #         "
+00094b00: 6f72 6465 7253 7461 7475 7322 3a22 5052  orderStatus":"PR
+00094b10: 4f43 4553 5322 0a20 2020 2020 2020 2023  OCESS".        #
+00094b20: 2020 2020 207d 0a20 2020 2020 2020 2023       }.        #
+00094b30: 0a20 2020 2020 2020 2023 2063 7265 6174  .        # creat
+00094b40: 6543 6f6e 7665 7274 5472 6164 6520 4255  eConvertTrade BU
+00094b50: 5344 0a20 2020 2020 2020 2023 0a20 2020  SD.        #.   
+00094b60: 2020 2020 2023 2020 2020 207b 0a20 2020       #     {.   
+00094b70: 2020 2020 2023 2020 2020 2020 2020 2022       #         "
+00094b80: 7472 616e 4964 223a 2031 3138 3236 3334  tranId": 1182634
+00094b90: 3037 3131 392c 0a20 2020 2020 2020 2023  07119,.        #
+00094ba0: 2020 2020 2020 2020 2022 7374 6174 7573           "status
+00094bb0: 223a 2022 5322 0a20 2020 2020 2020 2023  ": "S".        #
+00094bc0: 2020 2020 207d 0a20 2020 2020 2020 2023       }.        #
+00094bd0: 0a20 2020 2020 2020 2023 2066 6574 6368  .        # fetch
+00094be0: 436f 6e76 6572 7454 7261 6465 2c20 6665  ConvertTrade, fe
+00094bf0: 7463 6843 6f6e 7665 7274 5472 6164 6548  tchConvertTradeH
+00094c00: 6973 746f 7279 2042 5553 440a 2020 2020  istory BUSD.    
+00094c10: 2020 2020 230a 2020 2020 2020 2020 2320      #.        # 
+00094c20: 2020 2020 7b0a 2020 2020 2020 2020 2320      {.        # 
+00094c30: 2020 2020 2020 2020 2274 7261 6e49 6422          "tranId"
+00094c40: 3a20 3131 3832 3633 3631 3539 3931 2c0a  : 118263615991,.
+00094c50: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+00094c60: 2020 2274 7970 6522 3a20 3234 342c 0a20    "type": 244,. 
+00094c70: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+00094c80: 2022 7469 6d65 223a 2031 3636 3434 3432   "time": 1664442
+00094c90: 3037 3830 3030 2c0a 2020 2020 2020 2020  078000,.        
+00094ca0: 2320 2020 2020 2020 2020 2264 6564 7563  #         "deduc
+00094cb0: 7465 6441 7373 6574 223a 2022 4255 5344  tedAsset": "BUSD
+00094cc0: 222c 0a20 2020 2020 2020 2023 2020 2020  ",.        #    
+00094cd0: 2020 2020 2022 6465 6475 6374 6564 416d       "deductedAm
+00094ce0: 6f75 6e74 223a 2022 3122 2c0a 2020 2020  ount": "1",.    
+00094cf0: 2020 2020 2320 2020 2020 2020 2020 2274      #         "t
+00094d00: 6172 6765 7441 7373 6574 223a 2022 5553  argetAsset": "US
+00094d10: 4443 222c 0a20 2020 2020 2020 2023 2020  DC",.        #  
+00094d20: 2020 2020 2020 2022 7461 7267 6574 416d         "targetAm
+00094d30: 6f75 6e74 223a 2022 3122 2c0a 2020 2020  ount": "1",.    
+00094d40: 2020 2020 2320 2020 2020 2020 2020 2273      #         "s
+00094d50: 7461 7475 7322 3a20 2253 222c 0a20 2020  tatus": "S",.   
+00094d60: 2020 2020 2023 2020 2020 2020 2020 2022       #         "
+00094d70: 6163 636f 756e 7454 7970 6522 3a20 224d  accountType": "M
+00094d80: 4149 4e22 0a20 2020 2020 2020 2023 2020  AIN".        #  
+00094d90: 2020 207d 0a20 2020 2020 2020 2023 0a20     }.        #. 
+00094da0: 2020 2020 2020 2023 2066 6574 6368 436f         # fetchCo
+00094db0: 6e76 6572 7454 7261 6465 0a20 2020 2020  nvertTrade.     
+00094dc0: 2020 2023 0a20 2020 2020 2020 2023 2020     #.        #  
+00094dd0: 2020 207b 0a20 2020 2020 2020 2023 2020     {.        #  
+00094de0: 2020 2020 2020 2022 6f72 6465 7249 6422         "orderId"
+00094df0: 3a39 3333 3235 3632 3738 3432 3632 3734  :933256278426274
+00094e00: 3432 362c 0a20 2020 2020 2020 2023 2020  426,.        #  
+00094e10: 2020 2020 2020 2022 6f72 6465 7253 7461         "orderSta
+00094e20: 7475 7322 3a22 5355 4343 4553 5322 2c0a  tus":"SUCCESS",.
+00094e30: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+00094e40: 2020 2266 726f 6d41 7373 6574 223a 2242    "fromAsset":"B
+00094e50: 5443 222c 0a20 2020 2020 2020 2023 2020  TC",.        #  
+00094e60: 2020 2020 2020 2022 6672 6f6d 416d 6f75         "fromAmou
+00094e70: 6e74 223a 2230 2e30 3030 3534 3431 3422  nt":"0.00054414"
+00094e80: 2c0a 2020 2020 2020 2020 2320 2020 2020  ,.        #     
+00094e90: 2020 2020 2274 6f41 7373 6574 223a 2255      "toAsset":"U
+00094ea0: 5344 5422 2c0a 2020 2020 2020 2020 2320  SDT",.        # 
+00094eb0: 2020 2020 2020 2020 2274 6f41 6d6f 756e          "toAmoun
+00094ec0: 7422 3a22 3230 222c 0a20 2020 2020 2020  t":"20",.       
+00094ed0: 2023 2020 2020 2020 2020 2022 7261 7469   #         "rati
+00094ee0: 6f22 3a22 3336 3735 3522 2c0a 2020 2020  o":"36755",.    
+00094ef0: 2020 2020 2320 2020 2020 2020 2020 2269      #         "i
+00094f00: 6e76 6572 7365 5261 7469 6f22 3a22 302e  nverseRatio":"0.
+00094f10: 3030 3030 3237 3231 222c 0a20 2020 2020  00002721",.     
+00094f20: 2020 2023 2020 2020 2020 2020 2022 6372     #         "cr
+00094f30: 6561 7465 5469 6d65 223a 3136 3233 3338  eateTime":162338
+00094f40: 3133 3330 3437 320a 2020 2020 2020 2020  1330472.        
+00094f50: 2320 2020 2020 7d0a 2020 2020 2020 2020  #     }.        
+00094f60: 230a 2020 2020 2020 2020 2320 6665 7463  #.        # fetc
+00094f70: 6843 6f6e 7665 7274 5472 6164 6548 6973  hConvertTradeHis
+00094f80: 746f 7279 0a20 2020 2020 2020 2023 0a20  tory.        #. 
+00094f90: 2020 2020 2020 2023 2020 2020 207b 0a20         #     {. 
+00094fa0: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+00094fb0: 2022 7175 6f74 6549 6422 3a20 2266 3362   "quoteId": "f3b
+00094fc0: 3931 6335 3235 6232 3634 3463 3762 6331  91c525b2644c7bc1
+00094fd0: 6531 6364 3331 6236 6531 6161 3622 2c0a  e1cd31b6e1aa6",.
+00094fe0: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+00094ff0: 2020 226f 7264 6572 4964 223a 2039 3430    "orderId": 940
+00095000: 3730 3834 3037 3436 3230 3837 3139 352c  708407462087195,
+00095010: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+00095020: 2020 2022 6f72 6465 7253 7461 7475 7322     "orderStatus"
+00095030: 3a20 2253 5543 4345 5353 222c 0a20 2020  : "SUCCESS",.   
+00095040: 2020 2020 2023 2020 2020 2020 2020 2022       #         "
+00095050: 6672 6f6d 4173 7365 7422 3a20 2255 5344  fromAsset": "USD
+00095060: 5422 2c0a 2020 2020 2020 2020 2320 2020  T",.        #   
+00095070: 2020 2020 2020 2266 726f 6d41 6d6f 756e        "fromAmoun
+00095080: 7422 3a20 2232 3022 2c0a 2020 2020 2020  t": "20",.      
+00095090: 2020 2320 2020 2020 2020 2020 2274 6f41    #         "toA
+000950a0: 7373 6574 223a 2022 424e 4222 2c0a 2020  sset": "BNB",.  
+000950b0: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+000950c0: 2274 6f41 6d6f 756e 7422 3a20 2230 2e30  "toAmount": "0.0
+000950d0: 3631 3534 3033 3622 2c0a 2020 2020 2020  6154036",.      
+000950e0: 2020 2320 2020 2020 2020 2020 2272 6174    #         "rat
+000950f0: 696f 223a 2022 302e 3030 3330 3737 3032  io": "0.00307702
+00095100: 222c 0a20 2020 2020 2020 2023 2020 2020  ",.        #    
+00095110: 2020 2020 2022 696e 7665 7273 6552 6174       "inverseRat
+00095120: 696f 223a 2022 3332 342e 3939 222c 0a20  io": "324.99",. 
+00095130: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+00095140: 2022 6372 6561 7465 5469 6d65 223a 2031   "createTime": 1
+00095150: 3632 3432 3438 3837 3231 3834 0a20 2020  624248872184.   
+00095160: 2020 2020 2023 2020 2020 207d 0a20 2020       #     }.   
+00095170: 2020 2020 2023 0a20 2020 2020 2020 2074       #.        t
+00095180: 696d 6573 7461 6d70 203d 2073 656c 662e  imestamp = self.
+00095190: 7361 6665 5f69 6e74 6567 6572 5f6e 2863  safe_integer_n(c
+000951a0: 6f6e 7665 7273 696f 6e2c 205b 2774 696d  onversion, ['tim
+000951b0: 6527 2c20 2776 616c 6964 5469 6d65 7374  e', 'validTimest
+000951c0: 616d 7027 2c20 2763 7265 6174 6554 696d  amp', 'createTim
+000951d0: 6527 5d29 0a20 2020 2020 2020 2066 726f  e']).        fro
+000951e0: 6d43 7572 203d 2073 656c 662e 7361 6665  mCur = self.safe
+000951f0: 5f73 7472 696e 675f 3228 636f 6e76 6572  _string_2(conver
+00095200: 7369 6f6e 2c20 2764 6564 7563 7465 6441  sion, 'deductedA
+00095210: 7373 6574 272c 2027 6672 6f6d 4173 7365  sset', 'fromAsse
+00095220: 7427 290a 2020 2020 2020 2020 6672 6f6d  t').        from
+00095230: 436f 6465 203d 2073 656c 662e 7361 6665  Code = self.safe
+00095240: 5f63 7572 7265 6e63 795f 636f 6465 2866  _currency_code(f
+00095250: 726f 6d43 7572 2c20 6672 6f6d 4375 7272  romCur, fromCurr
+00095260: 656e 6379 290a 2020 2020 2020 2020 746f  ency).        to
+00095270: 203d 2073 656c 662e 7361 6665 5f73 7472   = self.safe_str
+00095280: 696e 675f 3228 636f 6e76 6572 7369 6f6e  ing_2(conversion
+00095290: 2c20 2774 6172 6765 7441 7373 6574 272c  , 'targetAsset',
+000952a0: 2027 746f 4173 7365 7427 290a 2020 2020   'toAsset').    
+000952b0: 2020 2020 746f 436f 6465 203d 2073 656c      toCode = sel
+000952c0: 662e 7361 6665 5f63 7572 7265 6e63 795f  f.safe_currency_
+000952d0: 636f 6465 2874 6f2c 2074 6f43 7572 7265  code(to, toCurre
+000952e0: 6e63 7929 0a20 2020 2020 2020 2072 6574  ncy).        ret
+000952f0: 7572 6e20 7b0a 2020 2020 2020 2020 2020  urn {.          
+00095300: 2020 2769 6e66 6f27 3a20 636f 6e76 6572    'info': conver
+00095310: 7369 6f6e 2c0a 2020 2020 2020 2020 2020  sion,.          
+00095320: 2020 2774 696d 6573 7461 6d70 273a 2074    'timestamp': t
+00095330: 696d 6573 7461 6d70 2c0a 2020 2020 2020  imestamp,.      
+00095340: 2020 2020 2020 2764 6174 6574 696d 6527        'datetime'
+00095350: 3a20 7365 6c66 2e69 736f 3836 3031 2874  : self.iso8601(t
+00095360: 696d 6573 7461 6d70 292c 0a20 2020 2020  imestamp),.     
+00095370: 2020 2020 2020 2027 6964 273a 2073 656c         'id': sel
+00095380: 662e 7361 6665 5f73 7472 696e 675f 6e28  f.safe_string_n(
+00095390: 636f 6e76 6572 7369 6f6e 2c20 5b27 7472  conversion, ['tr
+000953a0: 616e 4964 272c 2027 6f72 6465 7249 6427  anId', 'orderId'
+000953b0: 2c20 2771 756f 7465 4964 275d 292c 0a20  , 'quoteId']),. 
+000953c0: 2020 2020 2020 2020 2020 2027 6672 6f6d             'from
+000953d0: 4375 7272 656e 6379 273a 2066 726f 6d43  Currency': fromC
+000953e0: 6f64 652c 0a20 2020 2020 2020 2020 2020  ode,.           
+000953f0: 2027 6672 6f6d 416d 6f75 6e74 273a 2073   'fromAmount': s
+00095400: 656c 662e 7361 6665 5f6e 756d 6265 725f  elf.safe_number_
+00095410: 3228 636f 6e76 6572 7369 6f6e 2c20 2764  2(conversion, 'd
+00095420: 6564 7563 7465 6441 6d6f 756e 7427 2c20  eductedAmount', 
+00095430: 2766 726f 6d41 6d6f 756e 7427 292c 0a20  'fromAmount'),. 
+00095440: 2020 2020 2020 2020 2020 2027 746f 4375             'toCu
+00095450: 7272 656e 6379 273a 2074 6f43 6f64 652c  rrency': toCode,
+00095460: 0a20 2020 2020 2020 2020 2020 2027 746f  .            'to
+00095470: 416d 6f75 6e74 273a 2073 656c 662e 7361  Amount': self.sa
+00095480: 6665 5f6e 756d 6265 725f 3228 636f 6e76  fe_number_2(conv
+00095490: 6572 7369 6f6e 2c20 2774 6172 6765 7441  ersion, 'targetA
+000954a0: 6d6f 756e 7427 2c20 2774 6f41 6d6f 756e  mount', 'toAmoun
+000954b0: 7427 292c 0a20 2020 2020 2020 2020 2020  t'),.           
+000954c0: 2027 7072 6963 6527 3a20 4e6f 6e65 2c0a   'price': None,.
+000954d0: 2020 2020 2020 2020 2020 2020 2766 6565              'fee
+000954e0: 273a 204e 6f6e 652c 0a20 2020 2020 2020  ': None,.       
+000954f0: 207d 0a                                   }.
```

### Comparing `ccxt-4.3.7/ccxt/binancecoinm.py` & `ccxt-4.3.8/ccxt/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/binanceus.py` & `ccxt-4.3.8/ccxt/binanceus.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/binanceusdm.py` & `ccxt-4.3.8/ccxt/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/bingx.py` & `ccxt-4.3.8/ccxt/bingx.py`

 * *Files 0% similar despite different names*

```diff
@@ -2313,15 +2313,15 @@
             #  takeProfit: '{"stopPrice":150,"workingType":"MARK_PRICE","type":"TAKE_PROFIT_MARKET","quantity":1}',
             if isinstance(takeProfit, str):
                 takeProfit = self.parse_json(takeProfit)
             takeProfitPrice = self.safe_number(takeProfit, 'stopPrice')
         return self.safe_order({
             'info': info,
             'id': self.safe_string_2(order, 'orderId', 'i'),
-            'clientOrderId': self.safe_string_n(order, ['clientOrderID', 'origClientOrderId', 'c']),
+            'clientOrderId': self.safe_string_n(order, ['clientOrderID', 'clientOrderId', 'origClientOrderId', 'c']),
             'symbol': self.safe_symbol(marketId, market, '-', marketType),
             'timestamp': timestamp,
             'datetime': self.iso8601(timestamp),
             'lastTradeTimestamp': lastTradeTimestamp,
             'lastUpdateTimestamp': self.safe_integer(order, 'updateTime'),
             'type': self.parse_order_type(self.safe_string_lower_2(order, 'type', 'o')),
             'timeInForce': self.safe_string(order, 'timeInForce'),
```

### Comparing `ccxt-4.3.7/ccxt/bit2c.py` & `ccxt-4.3.8/ccxt/bit2c.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/bitbank.py` & `ccxt-4.3.8/ccxt/bitbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/bitbns.py` & `ccxt-4.3.8/ccxt/bitbns.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/bitfinex.py` & `ccxt-4.3.8/ccxt/bitfinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/bitfinex2.py` & `ccxt-4.3.8/ccxt/bitfinex2.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/bitflyer.py` & `ccxt-4.3.8/ccxt/bitflyer.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/bitget.py` & `ccxt-4.3.8/ccxt/bitget.py`

 * *Files 0% similar despite different names*

```diff
@@ -8058,15 +8058,15 @@
         #             ],
         #             "endId": "1159296505255219205"
         #         }
         #     }
         #
         data = self.safe_dict(response, 'data', {})
         dataList = self.safe_list(data, 'dataList', [])
-        return self.parse_conversions(dataList, 'fromCoin', 'toCoin', since, limit)
+        return self.parse_conversions(dataList, code, 'fromCoin', 'toCoin', since, limit)
 
     def parse_conversion(self, conversion, fromCurrency: Currency = None, toCurrency: Currency = None) -> Conversion:
         #
         # fetchConvertQuote
         #
         #     {
         #         "fromCoin": "USDT",
```

### Comparing `ccxt-4.3.7/ccxt/bithumb.py` & `ccxt-4.3.8/ccxt/bithumb.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/bitmart.py` & `ccxt-4.3.8/ccxt/bitmart.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/bitmex.py` & `ccxt-4.3.8/ccxt/bitmex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/bitopro.py` & `ccxt-4.3.8/ccxt/bitopro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/bitrue.py` & `ccxt-4.3.8/ccxt/bitrue.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/bitso.py` & `ccxt-4.3.8/ccxt/bitso.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/bitstamp.py` & `ccxt-4.3.8/ccxt/bitstamp.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/bitteam.py` & `ccxt-4.3.8/ccxt/bitteam.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/bitvavo.py` & `ccxt-4.3.8/ccxt/bitvavo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/bl3p.py` & `ccxt-4.3.8/ccxt/bl3p.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/blockchaincom.py` & `ccxt-4.3.8/ccxt/blockchaincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/blofin.py` & `ccxt-4.3.8/ccxt/blofin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/btcalpha.py` & `ccxt-4.3.8/ccxt/btcalpha.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/btcbox.py` & `ccxt-4.3.8/ccxt/btcbox.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/btcmarkets.py` & `ccxt-4.3.8/ccxt/btcmarkets.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/btcturk.py` & `ccxt-4.3.8/ccxt/btcturk.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/bybit.py` & `ccxt-4.3.8/ccxt/bybit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/cex.py` & `ccxt-4.3.8/ccxt/cex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/coinbase.py` & `ccxt-4.3.8/ccxt/coinbase.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/coinbaseinternational.py` & `ccxt-4.3.8/ccxt/coinbaseinternational.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/coinbasepro.py` & `ccxt-4.3.8/ccxt/coinbasepro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/coincheck.py` & `ccxt-4.3.8/ccxt/coincheck.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/coinex.py` & `ccxt-4.3.8/ccxt/coinex.py`

 * *Files 1% similar despite different names*

```diff
@@ -1483,204 +1483,159 @@
         #     }
         #
         data = self.safe_list(response, 'data', [])
         return self.parse_ohlcvs(data, market, timeframe, since, limit)
 
     def fetch_margin_balance(self, params={}):
         self.load_markets()
-        symbol = self.safe_string(params, 'symbol')
-        marketId = self.safe_string(params, 'market')
-        market: Market = None
-        if symbol is not None:
-            market = self.market(symbol)
-            marketId = market['id']
-        elif marketId is None:
-            raise ArgumentsRequired(self.id + ' fetchMarginBalance() fetching a margin account requires a market parameter or a symbol parameter')
-        params = self.omit(params, ['symbol', 'market'])
-        request = {
-            'market': marketId,
-        }
-        response = self.v1PrivateGetMarginAccount(self.extend(request, params))
+        response = self.v2PrivateGetAssetsMarginBalance(params)
         #
-        #      {
-        #          "code":    0,
-        #           "data": {
-        #              "account_id":    126,
-        #              "leverage":    3,
-        #              "market_type":   "AAVEUSDT",
-        #              "sell_asset_type":   "AAVE",
-        #              "buy_asset_type":   "USDT",
-        #              "balance": {
-        #                  "sell_type": "0.3",     # borrowed
-        #                  "buy_type": "30"
-        #                  },
-        #              "frozen": {
-        #                  "sell_type": "0",
-        #                  "buy_type": "0"
-        #                  },
-        #              "loan": {
-        #                  "sell_type": "0.3",  # loan
-        #                  "buy_type": "0"
-        #                  },
-        #              "interest": {
-        #                  "sell_type": "0.0000125",
-        #                  "buy_type": "0"
-        #                  },
-        #              "can_transfer": {
-        #                  "sell_type": "0.02500646",
-        #                  "buy_type": "4.28635738"
-        #                  },
-        #              "warn_rate":   "",
-        #              "liquidation_price":   ""
-        #              },
-        #          "message": "Success"
-        #      }
+        #     {
+        #         "data": [
+        #             {
+        #                 "margin_account": "BTCUSDT",
+        #                 "base_ccy": "BTC",
+        #                 "quote_ccy": "USDT",
+        #                 "available": {
+        #                     "base_ccy": "0.00000026",
+        #                     "quote_ccy": "0"
+        #                 },
+        #                 "frozen": {
+        #                     "base_ccy": "0",
+        #                     "quote_ccy": "0"
+        #                 },
+        #                 "repaid": {
+        #                     "base_ccy": "0",
+        #                     "quote_ccy": "0"
+        #                 },
+        #                 "interest": {
+        #                     "base_ccy": "0",
+        #                     "quote_ccy": "0"
+        #                 },
+        #                 "rik_rate": "",
+        #                 "liq_price": ""
+        #             },
+        #         ],
+        #         "code": 0,
+        #         "message": "OK"
+        #     }
         #
         result = {'info': response}
-        data = self.safe_value(response, 'data', {})
-        free = self.safe_value(data, 'can_transfer', {})
-        total = self.safe_value(data, 'balance', {})
-        loan = self.safe_value(data, 'loan', {})
-        interest = self.safe_value(data, 'interest', {})
-        #
-        sellAccount = self.account()
-        sellCurrencyId = self.safe_string(data, 'sell_asset_type')
-        sellCurrencyCode = self.safe_currency_code(sellCurrencyId)
-        sellAccount['free'] = self.safe_string(free, 'sell_type')
-        sellAccount['total'] = self.safe_string(total, 'sell_type')
-        sellDebt = self.safe_string(loan, 'sell_type')
-        sellInterest = self.safe_string(interest, 'sell_type')
-        sellAccount['debt'] = Precise.string_add(sellDebt, sellInterest)
-        result[sellCurrencyCode] = sellAccount
-        #
-        buyAccount = self.account()
-        buyCurrencyId = self.safe_string(data, 'buy_asset_type')
-        buyCurrencyCode = self.safe_currency_code(buyCurrencyId)
-        buyAccount['free'] = self.safe_string(free, 'buy_type')
-        buyAccount['total'] = self.safe_string(total, 'buy_type')
-        buyDebt = self.safe_string(loan, 'buy_type')
-        buyInterest = self.safe_string(interest, 'buy_type')
-        buyAccount['debt'] = Precise.string_add(buyDebt, buyInterest)
-        result[buyCurrencyCode] = buyAccount
-        #
+        balances = self.safe_list(response, 'data', [])
+        for i in range(0, len(balances)):
+            entry = balances[i]
+            free = self.safe_dict(entry, 'available', {})
+            used = self.safe_dict(entry, 'frozen', {})
+            loan = self.safe_dict(entry, 'repaid', {})
+            interest = self.safe_dict(entry, 'interest', {})
+            baseAccount = self.account()
+            baseCurrencyId = self.safe_string(entry, 'base_ccy')
+            baseCurrencyCode = self.safe_currency_code(baseCurrencyId)
+            baseAccount['free'] = self.safe_string(free, 'base_ccy')
+            baseAccount['used'] = self.safe_string(used, 'base_ccy')
+            baseDebt = self.safe_string(loan, 'base_ccy')
+            baseInterest = self.safe_string(interest, 'base_ccy')
+            baseAccount['debt'] = Precise.string_add(baseDebt, baseInterest)
+            result[baseCurrencyCode] = baseAccount
         return self.safe_balance(result)
 
     def fetch_spot_balance(self, params={}):
         self.load_markets()
-        response = self.v1PrivateGetBalanceInfo(params)
+        response = self.v2PrivateGetAssetsSpotBalance(params)
         #
         #     {
-        #       "code": 0,
-        #       "data": {
-        #         "BCH": {                    # BCH account
-        #           "available": "13.60109",   # Available BCH
-        #           "frozen": "0.00000"        # Frozen BCH
-        #         },
-        #         "BTC": {                    # BTC account
-        #           "available": "32590.16",   # Available BTC
-        #           "frozen": "7000.00"        # Frozen BTC
-        #         },
-        #         "ETH": {                    # ETH account
-        #           "available": "5.06000",    # Available ETH
-        #           "frozen": "0.00000"        # Frozen ETH
-        #         }
-        #       },
-        #       "message": "Ok"
+        #         "code": 0,
+        #         "data": [
+        #             {
+        #                 "available": "0.00000046",
+        #                 "ccy": "USDT",
+        #                 "frozen": "0"
+        #             }
+        #         ],
+        #         "message": "OK"
         #     }
         #
         result = {'info': response}
-        balances = self.safe_value(response, 'data', {})
-        currencyIds = list(balances.keys())
-        for i in range(0, len(currencyIds)):
-            currencyId = currencyIds[i]
+        balances = self.safe_list(response, 'data', [])
+        for i in range(0, len(balances)):
+            entry = balances[i]
+            currencyId = self.safe_string(entry, 'ccy')
             code = self.safe_currency_code(currencyId)
-            balance = self.safe_value(balances, currencyId, {})
             account = self.account()
-            account['free'] = self.safe_string(balance, 'available')
-            account['used'] = self.safe_string(balance, 'frozen')
+            account['free'] = self.safe_string(entry, 'available')
+            account['used'] = self.safe_string(entry, 'frozen')
             result[code] = account
         return self.safe_balance(result)
 
     def fetch_swap_balance(self, params={}):
         self.load_markets()
-        response = self.v1PerpetualPrivateGetAssetQuery(params)
+        response = self.v2PrivateGetAssetsFuturesBalance(params)
         #
         #     {
         #         "code": 0,
-        #         "data": {
-        #             "USDT": {
-        #                 "available": "37.24817690383456000000",
-        #                 "balance_total": "37.24817690383456000000",
-        #                 "frozen": "0.00000000000000000000",
-        #                 "margin": "0.00000000000000000000",
-        #                 "profit_unreal": "0.00000000000000000000",
-        #                 "transfer": "37.24817690383456000000"
+        #         "data": [
+        #             {
+        #                 "available": "0.00000046",
+        #                 "ccy": "USDT",
+        #                 "frozen": "0",
+        #                 "margin": "0",
+        #                 "transferrable": "0.00000046",
+        #                 "unrealized_pnl": "0"
         #             }
-        #         },
+        #         ],
         #         "message": "OK"
         #     }
         #
         result = {'info': response}
-        balances = self.safe_value(response, 'data', {})
-        currencyIds = list(balances.keys())
-        for i in range(0, len(currencyIds)):
-            currencyId = currencyIds[i]
+        balances = self.safe_list(response, 'data', [])
+        for i in range(0, len(balances)):
+            entry = balances[i]
+            currencyId = self.safe_string(entry, 'ccy')
             code = self.safe_currency_code(currencyId)
-            balance = self.safe_value(balances, currencyId, {})
             account = self.account()
-            account['free'] = self.safe_string(balance, 'available')
-            account['used'] = self.safe_string(balance, 'frozen')
-            account['total'] = self.safe_string(balance, 'balance_total')
+            account['free'] = self.safe_string(entry, 'available')
+            account['used'] = self.safe_string(entry, 'frozen')
             result[code] = account
         return self.safe_balance(result)
 
     def fetch_financial_balance(self, params={}):
         self.load_markets()
-        response = self.v1PrivateGetAccountInvestmentBalance(params)
+        response = self.v2PrivateGetAssetsFinancialBalance(params)
         #
         #     {
-        #          "code": 0,
-        #          "data": [
-        #              {
-        #                  "asset": "CET",
-        #                  "available": "0",
-        #                  "frozen": "0",
-        #                  "lock": "0",
-        #              },
-        #              {
-        #                  "asset": "USDT",
-        #                  "available": "999900",
-        #                  "frozen": "0",
-        #                  "lock": "0"
-        #              }
-        #          ],
-        #          "message": "Success"
-        #      }
+        #         "code": 0,
+        #         "data": [
+        #             {
+        #                 "available": "0.00000046",
+        #                 "ccy": "USDT",
+        #                 "frozen": "0"
+        #             }
+        #         ],
+        #         "message": "OK"
+        #     }
         #
         result = {'info': response}
-        balances = self.safe_value(response, 'data', {})
+        balances = self.safe_list(response, 'data', [])
         for i in range(0, len(balances)):
-            balance = balances[i]
-            currencyId = self.safe_string(balance, 'asset')
+            entry = balances[i]
+            currencyId = self.safe_string(entry, 'ccy')
             code = self.safe_currency_code(currencyId)
             account = self.account()
-            account['free'] = self.safe_string(balance, 'available')
-            frozen = self.safe_string(balance, 'frozen')
-            locked = self.safe_string(balance, 'lock')
-            account['used'] = Precise.string_add(frozen, locked)
+            account['free'] = self.safe_string(entry, 'available')
+            account['used'] = self.safe_string(entry, 'frozen')
             result[code] = account
         return self.safe_balance(result)
 
     def fetch_balance(self, params={}) -> Balances:
         """
         query for balance and get the amount of funds available for trading or funds locked in orders
-        :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot002_account001_account_info         # spot
-        :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot002_account004_investment_balance   # financial
-        :see: https://viabtc.github.io/coinex_api_en_doc/spot/#docsspot002_account006_margin_account       # margin
-        :see: https://viabtc.github.io/coinex_api_en_doc/futures/#docsfutures001_http016_asset_query       # swap
+        :see: https://docs.coinex.com/api/v2/assets/balance/http/get-spot-balance         # spot
+        :see: https://docs.coinex.com/api/v2/assets/balance/http/get-futures-balance      # swap
+        :see: https://docs.coinex.com/api/v2/assets/balance/http/get-marigin-balance      # margin
+        :see: https://docs.coinex.com/api/v2/assets/balance/http/get-financial-balance    # financial
         :param dict [params]: extra parameters specific to the exchange API endpoint
         :param str [params.type]: 'margin', 'swap', 'financial', or 'spot'
         :returns dict: a `balance structure <https://docs.ccxt.com/#/?id=balance-structure>`
         """
         marketType = None
         marketType, params = self.handle_market_type_and_params('fetchBalance', None, params)
         marginMode = None
@@ -5443,23 +5398,27 @@
                     url += '?' + urlencoded
                 else:
                     body = self.json(query)
             elif version == 'v2':
                 self.check_required_credentials()
                 query = self.keysort(query)
                 urlencoded = self.rawencode(query)
-                preparedString = method + '/' + version + '/' + path + '?' + urlencoded + nonce + self.secret
+                preparedString = method + '/' + version + '/' + path
+                if urlencoded:
+                    preparedString += '?' + urlencoded
+                preparedString += nonce + self.secret
                 signature = self.hash(self.encode(preparedString), 'sha256')
                 headers = {
                     'X-COINEX-KEY': self.apiKey,
                     'X-COINEX-SIGN': signature,
                     'X-COINEX-TIMESTAMP': nonce,
                 }
                 if (method == 'GET') or (method == 'DELETE') or (method == 'PUT'):
-                    url += '?' + urlencoded
+                    if urlencoded:
+                        url += '?' + urlencoded
                 else:
                     body = self.json(query)
         return {'url': url, 'method': method, 'body': body, 'headers': headers}
 
     def handle_errors(self, httpCode, reason, url, method, headers, body, response, requestHeaders, requestBody):
         if response is None:
             return None
```

### Comparing `ccxt-4.3.7/ccxt/coinlist.py` & `ccxt-4.3.8/ccxt/coinlist.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/coinmate.py` & `ccxt-4.3.8/ccxt/coinmate.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/coinmetro.py` & `ccxt-4.3.8/ccxt/coinmetro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/coinone.py` & `ccxt-4.3.8/ccxt/coinone.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/coinsph.py` & `ccxt-4.3.8/ccxt/coinsph.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/coinspot.py` & `ccxt-4.3.8/ccxt/coinspot.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/cryptocom.py` & `ccxt-4.3.8/ccxt/cryptocom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/currencycom.py` & `ccxt-4.3.8/ccxt/currencycom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/delta.py` & `ccxt-4.3.8/ccxt/delta.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/deribit.py` & `ccxt-4.3.8/ccxt/deribit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/digifinex.py` & `ccxt-4.3.8/ccxt/digifinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/exmo.py` & `ccxt-4.3.8/ccxt/exmo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/flowbtc.py` & `ccxt-4.3.8/ccxt/flowbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/fmfwio.py` & `ccxt-4.3.8/ccxt/fmfwio.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/gate.py` & `ccxt-4.3.8/ccxt/gate.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/gemini.py` & `ccxt-4.3.8/ccxt/gemini.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/hitbtc.py` & `ccxt-4.3.8/ccxt/hitbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/hollaex.py` & `ccxt-4.3.8/ccxt/hollaex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/htx.py` & `ccxt-4.3.8/ccxt/htx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/huobijp.py` & `ccxt-4.3.8/ccxt/huobijp.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/hyperliquid.py` & `ccxt-4.3.8/ccxt/hyperliquid.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/idex.py` & `ccxt-4.3.8/ccxt/idex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/independentreserve.py` & `ccxt-4.3.8/ccxt/independentreserve.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/indodax.py` & `ccxt-4.3.8/ccxt/indodax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/kraken.py` & `ccxt-4.3.8/ccxt/kraken.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/krakenfutures.py` & `ccxt-4.3.8/ccxt/krakenfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/kucoin.py` & `ccxt-4.3.8/ccxt/kucoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/kucoinfutures.py` & `ccxt-4.3.8/ccxt/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/kuna.py` & `ccxt-4.3.8/ccxt/kuna.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/latoken.py` & `ccxt-4.3.8/ccxt/latoken.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/lbank.py` & `ccxt-4.3.8/ccxt/lbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/luno.py` & `ccxt-4.3.8/ccxt/luno.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/lykke.py` & `ccxt-4.3.8/ccxt/lykke.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/mercado.py` & `ccxt-4.3.8/ccxt/mercado.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/mexc.py` & `ccxt-4.3.8/ccxt/mexc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/ndax.py` & `ccxt-4.3.8/ccxt/ndax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/novadax.py` & `ccxt-4.3.8/ccxt/novadax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/oceanex.py` & `ccxt-4.3.8/ccxt/oceanex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/okcoin.py` & `ccxt-4.3.8/ccxt/okcoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/okx.py` & `ccxt-4.3.8/ccxt/okx.py`

 * *Files 0% similar despite different names*

```diff
@@ -7393,15 +7393,15 @@
         #                 "ts": "1646188520000"
         #             }
         #         ],
         #         "msg": ""
         #     }
         #
         rows = self.safe_list(response, 'data', [])
-        return self.parse_conversions(rows, 'baseCcy', 'quoteCcy', since, limit)
+        return self.parse_conversions(rows, code, 'baseCcy', 'quoteCcy', since, limit)
 
     def parse_conversion(self, conversion, fromCurrency: Currency = None, toCurrency: Currency = None) -> Conversion:
         #
         # fetchConvertQuote
         #
         #     {
         #         "baseCcy": "ETH",
```

### Comparing `ccxt-4.3.7/ccxt/onetrading.py` & `ccxt-4.3.8/ccxt/onetrading.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/p2b.py` & `ccxt-4.3.8/ccxt/p2b.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/paymium.py` & `ccxt-4.3.8/ccxt/paymium.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/phemex.py` & `ccxt-4.3.8/ccxt/phemex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/poloniex.py` & `ccxt-4.3.8/ccxt/poloniex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/poloniexfutures.py` & `ccxt-4.3.8/ccxt/poloniexfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/__init__.py` & `ccxt-4.3.8/ccxt/pro/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """CCXT: CryptoCurrency eXchange Trading Library (Async)"""
 
 # ----------------------------------------------------------------------------
 
-__version__ = '4.3.7'
+__version__ = '4.3.8'
 
 # ----------------------------------------------------------------------------
 
 from ccxt.async_support.base.exchange import Exchange  # noqa: F401
 
 # CCXT Pro exchanges (now this is mainly used for importing exchanges in WS tests)
```

### Comparing `ccxt-4.3.7/ccxt/pro/alpaca.py` & `ccxt-4.3.8/ccxt/pro/alpaca.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/ascendex.py` & `ccxt-4.3.8/ccxt/pro/ascendex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/bequant.py` & `ccxt-4.3.8/ccxt/pro/bequant.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/binance.py` & `ccxt-4.3.8/ccxt/pro/binance.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/binancecoinm.py` & `ccxt-4.3.8/ccxt/pro/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/binanceus.py` & `ccxt-4.3.8/ccxt/pro/binanceus.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/binanceusdm.py` & `ccxt-4.3.8/ccxt/pro/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/bingx.py` & `ccxt-4.3.8/ccxt/pro/bingx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/bitcoincom.py` & `ccxt-4.3.8/ccxt/pro/bitcoincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/bitfinex.py` & `ccxt-4.3.8/ccxt/pro/bitfinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/bitfinex2.py` & `ccxt-4.3.8/ccxt/pro/bitfinex2.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/bitget.py` & `ccxt-4.3.8/ccxt/pro/bitget.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/bithumb.py` & `ccxt-4.3.8/ccxt/pro/bithumb.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/bitmart.py` & `ccxt-4.3.8/ccxt/pro/bitmart.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/bitmex.py` & `ccxt-4.3.8/ccxt/pro/bitmex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/bitopro.py` & `ccxt-4.3.8/ccxt/pro/bitopro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/bitrue.py` & `ccxt-4.3.8/ccxt/pro/bitrue.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/bitstamp.py` & `ccxt-4.3.8/ccxt/pro/bitstamp.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/bitvavo.py` & `ccxt-4.3.8/ccxt/pro/bitvavo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/blockchaincom.py` & `ccxt-4.3.8/ccxt/pro/blockchaincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/bybit.py` & `ccxt-4.3.8/ccxt/pro/bybit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/cex.py` & `ccxt-4.3.8/ccxt/pro/cex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/coinbase.py` & `ccxt-4.3.8/ccxt/pro/coinbase.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/coinbaseinternational.py` & `ccxt-4.3.8/ccxt/pro/coinbaseinternational.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/coinbasepro.py` & `ccxt-4.3.8/ccxt/pro/coinbasepro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/coincheck.py` & `ccxt-4.3.8/ccxt/pro/coincheck.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/coinex.py` & `ccxt-4.3.8/ccxt/pro/coinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/coinone.py` & `ccxt-4.3.8/ccxt/pro/coinone.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/cryptocom.py` & `ccxt-4.3.8/ccxt/pro/cryptocom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/currencycom.py` & `ccxt-4.3.8/ccxt/pro/currencycom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/deribit.py` & `ccxt-4.3.8/ccxt/pro/deribit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/exmo.py` & `ccxt-4.3.8/ccxt/pro/exmo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/gate.py` & `ccxt-4.3.8/ccxt/pro/gate.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/gemini.py` & `ccxt-4.3.8/ccxt/pro/gemini.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/hitbtc.py` & `ccxt-4.3.8/ccxt/pro/hitbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/hollaex.py` & `ccxt-4.3.8/ccxt/pro/hollaex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/htx.py` & `ccxt-4.3.8/ccxt/pro/htx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/huobijp.py` & `ccxt-4.3.8/ccxt/pro/huobijp.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/hyperliquid.py` & `ccxt-4.3.8/ccxt/pro/hyperliquid.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/idex.py` & `ccxt-4.3.8/ccxt/pro/idex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/independentreserve.py` & `ccxt-4.3.8/ccxt/pro/independentreserve.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/kraken.py` & `ccxt-4.3.8/ccxt/pro/kraken.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/krakenfutures.py` & `ccxt-4.3.8/ccxt/pro/krakenfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/kucoin.py` & `ccxt-4.3.8/ccxt/pro/kucoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/kucoinfutures.py` & `ccxt-4.3.8/ccxt/pro/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/lbank.py` & `ccxt-4.3.8/ccxt/pro/lbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/luno.py` & `ccxt-4.3.8/ccxt/pro/luno.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/mexc.py` & `ccxt-4.3.8/ccxt/pro/mexc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/ndax.py` & `ccxt-4.3.8/ccxt/pro/ndax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/okcoin.py` & `ccxt-4.3.8/ccxt/pro/okcoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/okx.py` & `ccxt-4.3.8/ccxt/pro/okx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/onetrading.py` & `ccxt-4.3.8/ccxt/pro/onetrading.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/p2b.py` & `ccxt-4.3.8/ccxt/pro/p2b.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/phemex.py` & `ccxt-4.3.8/ccxt/pro/phemex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/poloniex.py` & `ccxt-4.3.8/ccxt/pro/poloniex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/poloniexfutures.py` & `ccxt-4.3.8/ccxt/pro/poloniexfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/probit.py` & `ccxt-4.3.8/ccxt/pro/probit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/upbit.py` & `ccxt-4.3.8/ccxt/pro/upbit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/wazirx.py` & `ccxt-4.3.8/ccxt/pro/wazirx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/whitebit.py` & `ccxt-4.3.8/ccxt/pro/whitebit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/pro/woo.py` & `ccxt-4.3.8/ccxt/pro/woo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/probit.py` & `ccxt-4.3.8/ccxt/probit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/ecdsa/__init__.py` & `ccxt-4.3.8/ccxt/static_dependencies/ecdsa/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/ecdsa/_version.py` & `ccxt-4.3.8/ccxt/static_dependencies/ecdsa/_version.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/ecdsa/curves.py` & `ccxt-4.3.8/ccxt/static_dependencies/ecdsa/curves.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/ecdsa/der.py` & `ccxt-4.3.8/ccxt/static_dependencies/ecdsa/der.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/ecdsa/ecdsa.py` & `ccxt-4.3.8/ccxt/static_dependencies/ecdsa/ecdsa.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/ecdsa/ellipticcurve.py` & `ccxt-4.3.8/ccxt/static_dependencies/ecdsa/ellipticcurve.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/ecdsa/keys.py` & `ccxt-4.3.8/ccxt/static_dependencies/ecdsa/keys.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/ecdsa/numbertheory.py` & `ccxt-4.3.8/ccxt/static_dependencies/ecdsa/numbertheory.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/ecdsa/rfc6979.py` & `ccxt-4.3.8/ccxt/static_dependencies/ecdsa/rfc6979.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/ecdsa/util.py` & `ccxt-4.3.8/ccxt/static_dependencies/ecdsa/util.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/ethereum/abi/base.py` & `ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/base.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/ethereum/abi/codec.py` & `ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/codec.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/ethereum/abi/decoding.py` & `ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/decoding.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/ethereum/abi/encoding.py` & `ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/encoding.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/ethereum/abi/exceptions.py` & `ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/exceptions.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/ethereum/abi/grammar.py` & `ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/grammar.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/ethereum/abi/registry.py` & `ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/registry.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/ethereum/abi/tools/_strategies.py` & `ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/tools/_strategies.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/ethereum/abi/utils/numeric.py` & `ccxt-4.3.8/ccxt/static_dependencies/ethereum/abi/utils/numeric.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/ethereum/account/encode_typed_data/encoding_and_hashing.py` & `ccxt-4.3.8/ccxt/static_dependencies/ethereum/account/encode_typed_data/encoding_and_hashing.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/ethereum/account/encode_typed_data/helpers.py` & `ccxt-4.3.8/ccxt/static_dependencies/ethereum/account/encode_typed_data/helpers.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/ethereum/account/messages.py` & `ccxt-4.3.8/ccxt/static_dependencies/ethereum/account/messages.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/ethereum/hexbytes/_utils.py` & `ccxt-4.3.8/ccxt/static_dependencies/ethereum/hexbytes/_utils.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/ethereum/hexbytes/main.py` & `ccxt-4.3.8/ccxt/static_dependencies/ethereum/hexbytes/main.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/ethereum/typing/__init__.py` & `ccxt-4.3.8/ccxt/static_dependencies/ethereum/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/ethereum/typing/evm.py` & `ccxt-4.3.8/ccxt/static_dependencies/ethereum/typing/evm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/ethereum/typing/networks.py` & `ccxt-4.3.8/ccxt/static_dependencies/ethereum/typing/networks.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/ethereum/utils/__init__.py` & `ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/ethereum/utils/abi.py` & `ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/abi.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/ethereum/utils/address.py` & `ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/address.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/ethereum/utils/applicators.py` & `ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/applicators.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/ethereum/utils/conversions.py` & `ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/conversions.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/ethereum/utils/currency.py` & `ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/currency.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/ethereum/utils/curried/__init__.py` & `ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/curried/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/ethereum/utils/decorators.py` & `ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/ethereum/utils/functional.py` & `ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/functional.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/ethereum/utils/hexadecimal.py` & `ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/hexadecimal.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/ethereum/utils/humanize.py` & `ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/humanize.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/ethereum/utils/logging.py` & `ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/ethereum/utils/module_loading.py` & `ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/module_loading.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/ethereum/utils/numeric.py` & `ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/numeric.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/ethereum/utils/toolz.py` & `ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/toolz.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/ethereum/utils/types.py` & `ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/types.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/ethereum/utils/units.py` & `ccxt-4.3.8/ccxt/static_dependencies/ethereum/utils/units.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/keccak/keccak.py` & `ccxt-4.3.8/ccxt/static_dependencies/keccak/keccak.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/msgpack/__init__.py` & `ccxt-4.3.8/ccxt/static_dependencies/msgpack/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/msgpack/exceptions.py` & `ccxt-4.3.8/ccxt/static_dependencies/msgpack/exceptions.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/msgpack/ext.py` & `ccxt-4.3.8/ccxt/static_dependencies/msgpack/ext.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/msgpack/fallback.py` & `ccxt-4.3.8/ccxt/static_dependencies/msgpack/fallback.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/parsimonious/exceptions.py` & `ccxt-4.3.8/ccxt/static_dependencies/parsimonious/exceptions.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/parsimonious/expressions.py` & `ccxt-4.3.8/ccxt/static_dependencies/parsimonious/expressions.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/parsimonious/grammar.py` & `ccxt-4.3.8/ccxt/static_dependencies/parsimonious/grammar.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/parsimonious/nodes.py` & `ccxt-4.3.8/ccxt/static_dependencies/parsimonious/nodes.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/parsimonious/utils.py` & `ccxt-4.3.8/ccxt/static_dependencies/parsimonious/utils.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/toolz/_signatures.py` & `ccxt-4.3.8/ccxt/static_dependencies/toolz/_signatures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/toolz/_version.py` & `ccxt-4.3.8/ccxt/static_dependencies/toolz/_version.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/toolz/compatibility.py` & `ccxt-4.3.8/ccxt/static_dependencies/toolz/compatibility.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/toolz/curried/__init__.py` & `ccxt-4.3.8/ccxt/static_dependencies/toolz/curried/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/toolz/curried/operator.py` & `ccxt-4.3.8/ccxt/static_dependencies/toolz/curried/operator.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/toolz/dicttoolz.py` & `ccxt-4.3.8/ccxt/static_dependencies/toolz/dicttoolz.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/toolz/functoolz.py` & `ccxt-4.3.8/ccxt/static_dependencies/toolz/functoolz.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/toolz/itertoolz.py` & `ccxt-4.3.8/ccxt/static_dependencies/toolz/itertoolz.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/static_dependencies/toolz/recipes.py` & `ccxt-4.3.8/ccxt/static_dependencies/toolz/recipes.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/test/base/__init__.py` & `ccxt-4.3.8/ccxt/test/base/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/test/base/test_account.py` & `ccxt-4.3.8/ccxt/test/base/test_account.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/test/base/test_balance.py` & `ccxt-4.3.8/ccxt/test/base/test_balance.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/test/base/test_borrow_interest.py` & `ccxt-4.3.8/ccxt/test/base/test_borrow_interest.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/test/base/test_borrow_rate.py` & `ccxt-4.3.8/ccxt/test/base/test_borrow_rate.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/test/base/test_calculate_fee.py` & `ccxt-4.3.8/ccxt/test/base/test_calculate_fee.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/test/base/test_crypto.py` & `ccxt-4.3.8/ccxt/test/base/test_crypto.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/test/base/test_currency.py` & `ccxt-4.3.8/ccxt/test/base/test_currency.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/test/base/test_datetime.py` & `ccxt-4.3.8/ccxt/test/base/test_datetime.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/test/base/test_decimal_to_precision.py` & `ccxt-4.3.8/ccxt/test/base/test_decimal_to_precision.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/test/base/test_deep_extend.py` & `ccxt-4.3.8/ccxt/test/base/test_deep_extend.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/test/base/test_deposit_withdrawal.py` & `ccxt-4.3.8/ccxt/test/base/test_deposit_withdrawal.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/test/base/test_exchange_datetime_functions.py` & `ccxt-4.3.8/ccxt/test/base/test_exchange_datetime_functions.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/test/base/test_funding_rate_history.py` & `ccxt-4.3.8/ccxt/test/base/test_funding_rate_history.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/test/base/test_last_price.py` & `ccxt-4.3.8/ccxt/test/base/test_last_price.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/test/base/test_ledger_entry.py` & `ccxt-4.3.8/ccxt/test/base/test_ledger_entry.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/test/base/test_ledger_item.py` & `ccxt-4.3.8/ccxt/test/base/test_ledger_item.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/test/base/test_leverage_tier.py` & `ccxt-4.3.8/ccxt/test/base/test_leverage_tier.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/test/base/test_margin_mode.py` & `ccxt-4.3.8/ccxt/test/base/test_margin_mode.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/test/base/test_margin_modification.py` & `ccxt-4.3.8/ccxt/test/base/test_margin_modification.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/test/base/test_market.py` & `ccxt-4.3.8/ccxt/test/base/test_market.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/test/base/test_number.py` & `ccxt-4.3.8/ccxt/test/base/test_number.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/test/base/test_ohlcv.py` & `ccxt-4.3.8/ccxt/test/base/test_ohlcv.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/test/base/test_open_interest.py` & `ccxt-4.3.8/ccxt/test/base/test_open_interest.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/test/base/test_order.py` & `ccxt-4.3.8/ccxt/test/base/test_order.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/test/base/test_order_book.py` & `ccxt-4.3.8/ccxt/test/base/test_order_book.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/test/base/test_position.py` & `ccxt-4.3.8/ccxt/test/base/test_position.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/test/base/test_shared_methods.py` & `ccxt-4.3.8/ccxt/test/base/test_shared_methods.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/test/base/test_status.py` & `ccxt-4.3.8/ccxt/test/base/test_status.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/test/base/test_throttle.py` & `ccxt-4.3.8/ccxt/test/base/test_throttle.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/test/base/test_ticker.py` & `ccxt-4.3.8/ccxt/test/base/test_ticker.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/test/base/test_trade.py` & `ccxt-4.3.8/ccxt/test/base/test_trade.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/test/base/test_trading_fee.py` & `ccxt-4.3.8/ccxt/test/base/test_trading_fee.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/test/base/test_transaction.py` & `ccxt-4.3.8/ccxt/test/base/test_transaction.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/test/test_async.py` & `ccxt-4.3.8/ccxt/test/test_async.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/test/test_sync.py` & `ccxt-4.3.8/ccxt/test/test_sync.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/timex.py` & `ccxt-4.3.8/ccxt/timex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/tokocrypto.py` & `ccxt-4.3.8/ccxt/tokocrypto.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/tradeogre.py` & `ccxt-4.3.8/ccxt/tradeogre.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/upbit.py` & `ccxt-4.3.8/ccxt/upbit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/wavesexchange.py` & `ccxt-4.3.8/ccxt/wavesexchange.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/wazirx.py` & `ccxt-4.3.8/ccxt/wazirx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/whitebit.py` & `ccxt-4.3.8/ccxt/whitebit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/woo.py` & `ccxt-4.3.8/ccxt/woo.py`

 * *Files 0% similar despite different names*

```diff
@@ -2960,15 +2960,15 @@
         #                 ...
         #             ]
         #         }
         #     }
         #
         data = self.safe_dict(response, 'data', {})
         rows = self.safe_list(data, 'tradeVos', [])
-        return self.parse_conversions(rows, 'sellAsset', 'buyAsset', since, limit)
+        return self.parse_conversions(rows, code, 'sellAsset', 'buyAsset', since, limit)
 
     def parse_conversion(self, conversion, fromCurrency: Currency = None, toCurrency: Currency = None) -> Conversion:
         #
         # fetchConvertQuote
         #
         #     {
         #         "quoteId": 123123123,
```

### Comparing `ccxt-4.3.7/ccxt/yobit.py` & `ccxt-4.3.8/ccxt/yobit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/zaif.py` & `ccxt-4.3.8/ccxt/zaif.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt/zonda.py` & `ccxt-4.3.8/ccxt/zonda.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/ccxt.egg-info/PKG-INFO` & `ccxt-4.3.8/ccxt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccxt
-Version: 4.3.7
+Version: 4.3.8
 Summary: A JavaScript / TypeScript / Python / C# / PHP cryptocurrency trading library with support for 100+ exchanges
 Home-page: https://ccxt.com
 Author: Igor Kroitor
 Author-email: igor.kroitor@gmail.com
 License: MIT
 Project-URL: Homepage, https://ccxt.com
 Project-URL: Documentation, https://github.com/ccxt/ccxt/wiki
@@ -222,21 +222,21 @@
         console.log(version, Object.keys(exchanges));
         ```
         
         ### JavaScript (for use with the `<script>` tag):
         
         All-in-one browser bundle (dependencies included), served from a CDN of your choice:
         
-        * jsDelivr: https://cdn.jsdelivr.net/npm/ccxt@4.3.7/dist/ccxt.browser.js
-        * unpkg: https://unpkg.com/ccxt@4.3.7/dist/ccxt.browser.js
+        * jsDelivr: https://cdn.jsdelivr.net/npm/ccxt@4.3.8/dist/ccxt.browser.js
+        * unpkg: https://unpkg.com/ccxt@4.3.8/dist/ccxt.browser.js
         
         CDNs are not updated in real-time and may have delays. Defaulting to the most recent version without specifying the version number is not recommended. Please, keep in mind that we are not responsible for the correct operation of those CDN servers.
         
         ```HTML
-        <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/ccxt@4.3.7/dist/ccxt.browser.js"></script>
+        <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/ccxt@4.3.8/dist/ccxt.browser.js"></script>
         ```
         
         Creates a global `ccxt` object:
         
         ```JavaScript
         console.log (ccxt.exchanges) // print all available exchanges
         ```
```

### Comparing `ccxt-4.3.7/ccxt.egg-info/SOURCES.txt` & `ccxt-4.3.8/ccxt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccxt-4.3.7/package.json` & `ccxt-4.3.8/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9772727272727273%*

 * *Differences: {"'version'": "'4.3.8'"}*

```diff
@@ -266,9 +266,9 @@
         "update-links": "node build/update-links",
         "validate-types": "node --loader ts-node/esm build/validate-types.ts",
         "vss": "node build/vss"
     },
     "type": "module",
     "types": "./js/ccxt.d.ts",
     "unpkg": "dist/ccxt.browser.js",
-    "version": "4.3.7"
+    "version": "4.3.8"
 }
```

### Comparing `ccxt-4.3.7/setup.py` & `ccxt-4.3.8/setup.py`

 * *Files identical despite different names*

