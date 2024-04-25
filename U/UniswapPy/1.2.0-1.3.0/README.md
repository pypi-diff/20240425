# Comparing `tmp/UniswapPy-1.2.0.tar.gz` & `tmp/UniswapPy-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UniswapPy-1.2.0.tar", last modified: Fri Apr 12 22:51:17 2024, max compression
+gzip compressed data, was "UniswapPy-1.3.0.tar", last modified: Thu Apr 25 15:01:13 2024, max compression
```

## Comparing `UniswapPy-1.2.0.tar` & `UniswapPy-1.3.0.tar`

### file list

```diff
@@ -1,116 +1,130 @@
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.019214 UniswapPy-1.2.0/
--rw-r--r--   0 ian_moore   (501) staff       (20)     1065 2024-02-07 00:37:32.000000 UniswapPy-1.2.0/LICENSE.txt
--rw-r--r--   0 ian_moore   (501) staff       (20)     3714 2024-04-12 22:51:17.019281 UniswapPy-1.2.0/PKG-INFO
--rw-r--r--   0 ian_moore   (501) staff       (20)     3418 2024-04-10 18:19:34.000000 UniswapPy-1.2.0/README.md
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.000437 UniswapPy-1.2.0/UniswapPy.egg-info/
--rw-r--r--   0 ian_moore   (501) staff       (20)     3714 2024-04-12 22:51:16.000000 UniswapPy-1.2.0/UniswapPy.egg-info/PKG-INFO
--rw-r--r--   0 ian_moore   (501) staff       (20)     3087 2024-04-12 22:51:16.000000 UniswapPy-1.2.0/UniswapPy.egg-info/SOURCES.txt
--rw-r--r--   0 ian_moore   (501) staff       (20)        1 2024-04-12 22:51:16.000000 UniswapPy-1.2.0/UniswapPy.egg-info/dependency_links.txt
--rw-r--r--   0 ian_moore   (501) staff       (20)        1 2024-02-11 00:15:12.000000 UniswapPy-1.2.0/UniswapPy.egg-info/not-zip-safe
--rw-r--r--   0 ian_moore   (501) staff       (20)       13 2024-04-12 22:51:16.000000 UniswapPy-1.2.0/UniswapPy.egg-info/requires.txt
--rw-r--r--   0 ian_moore   (501) staff       (20)       10 2024-04-12 22:51:16.000000 UniswapPy-1.2.0/UniswapPy.egg-info/top_level.txt
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:16.996923 UniswapPy-1.2.0/python/
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.000565 UniswapPy-1.2.0/python/prod/
--rw-r--r--   0 ian_moore   (501) staff       (20)      841 2024-04-10 18:17:44.000000 UniswapPy-1.2.0/python/prod/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:16.997413 UniswapPy-1.2.0/python/prod/cpt/
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.001459 UniswapPy-1.2.0/python/prod/cpt/exchg/
--rw-r--r--   0 ian_moore   (501) staff       (20)     7376 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/cpt/exchg/ChildUniswapExchange.py
--rw-r--r--   0 ian_moore   (501) staff       (20)    21514 2024-02-13 20:28:17.000000 UniswapPy-1.2.0/python/prod/cpt/exchg/UniswapExchange.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       99 2024-02-07 00:37:32.000000 UniswapPy-1.2.0/python/prod/cpt/exchg/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.001897 UniswapPy-1.2.0/python/prod/cpt/factory/
--rw-r--r--   0 ian_moore   (501) staff       (20)     3516 2024-02-13 21:52:11.000000 UniswapPy-1.2.0/python/prod/cpt/factory/UniswapFactory.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       44 2024-02-07 00:37:49.000000 UniswapPy-1.2.0/python/prod/cpt/factory/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.002563 UniswapPy-1.2.0/python/prod/cpt/index/
--rw-r--r--   0 ian_moore   (501) staff       (20)     1719 2024-02-13 21:41:28.000000 UniswapPy-1.2.0/python/prod/cpt/index/RebaseIndexToken.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     1712 2024-02-13 21:41:15.000000 UniswapPy-1.2.0/python/prod/cpt/index/SettlementLPToken.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       96 2024-02-07 00:37:32.000000 UniswapPy-1.2.0/python/prod/cpt/index/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.008665 UniswapPy-1.2.0/python/prod/cpt/quote/
--rw-r--r--   0 ian_moore   (501) staff       (20)     6938 2024-02-13 21:15:34.000000 UniswapPy-1.2.0/python/prod/cpt/quote/IndexTokenQuote.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     6990 2024-02-13 21:32:43.000000 UniswapPy-1.2.0/python/prod/cpt/quote/LPQuote.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     1752 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/cpt/quote/LPTokenQuote.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     4677 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/cpt/quote/TreeAmountQuote.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      157 2024-02-07 00:37:32.000000 UniswapPy-1.2.0/python/prod/cpt/quote/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.009281 UniswapPy-1.2.0/python/prod/cpt/vault/
--rw-r--r--   0 ian_moore   (501) staff       (20)    15329 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/cpt/vault/IndexVault.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      651 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/cpt/vault/Vault.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       59 2024-02-07 00:37:32.000000 UniswapPy-1.2.0/python/prod/cpt/vault/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.010123 UniswapPy-1.2.0/python/prod/cpt/wallet/
--rw-r--r--   0 ian_moore   (501) staff       (20)     2646 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/cpt/wallet/Wallets.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       28 2024-02-07 00:37:32.000000 UniswapPy-1.2.0/python/prod/cpt/wallet/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.011047 UniswapPy-1.2.0/python/prod/erc/
--rw-r--r--   0 ian_moore   (501) staff       (20)     1684 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/erc/DOAERC20.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     1456 2024-04-10 18:17:44.000000 UniswapPy-1.2.0/python/prod/erc/ERC20.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     1103 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/erc/IndexERC20.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     1720 2024-02-13 20:20:33.000000 UniswapPy-1.2.0/python/prod/erc/LPERC20.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      119 2024-02-07 00:37:32.000000 UniswapPy-1.2.0/python/prod/erc/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:16.998030 UniswapPy-1.2.0/python/prod/math/
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.011488 UniswapPy-1.2.0/python/prod/math/basic/
--rw-r--r--   0 ian_moore   (501) staff       (20)      500 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/math/basic/IDGenerator.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      485 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/math/basic/RoundFloat.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       52 2024-02-07 00:37:32.000000 UniswapPy-1.2.0/python/prod/math/basic/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.011883 UniswapPy-1.2.0/python/prod/math/interest/
--rw-r--r--   0 ian_moore   (501) staff       (20)      410 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/math/interest/CompoundReturn.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      519 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/math/interest/Yield.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       50 2024-02-07 00:37:32.000000 UniswapPy-1.2.0/python/prod/math/interest/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.012276 UniswapPy-1.2.0/python/prod/math/interest/ips/
--rw-r--r--   0 ian_moore   (501) staff       (20)      766 2024-02-07 00:37:32.000000 UniswapPy-1.2.0/python/prod/math/interest/ips/ConstantIPS.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      390 2024-02-07 00:37:32.000000 UniswapPy-1.2.0/python/prod/math/interest/ips/IPS.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       45 2024-02-07 00:37:32.000000 UniswapPy-1.2.0/python/prod/math/interest/ips/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.012539 UniswapPy-1.2.0/python/prod/math/interest/ips/aggregate/
--rw-r--r--   0 ian_moore   (501) staff       (20)      496 2024-02-07 00:37:32.000000 UniswapPy-1.2.0/python/prod/math/interest/ips/aggregate/AggregateIPS.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       27 2024-02-07 00:37:32.000000 UniswapPy-1.2.0/python/prod/math/interest/ips/aggregate/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.013315 UniswapPy-1.2.0/python/prod/math/model/
--rw-r--r--   0 ian_moore   (501) staff       (20)     2069 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/math/model/BrownianModel.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      504 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/math/model/EventSelectionModel.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      591 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/math/model/ModelQueue.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      762 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/math/model/TimeDeltaModel.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     1262 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/math/model/TokenDeltaModel.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      151 2024-02-07 00:37:32.000000 UniswapPy-1.2.0/python/prod/math/model/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.013671 UniswapPy-1.2.0/python/prod/math/risk/
--rw-r--r--   0 ian_moore   (501) staff       (20)     5556 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/math/risk/MaxDrop.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       22 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/math/risk/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.013911 UniswapPy-1.2.0/python/prod/process/
--rw-r--r--   0 ian_moore   (501) staff       (20)      300 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/process/Process.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       28 2024-02-07 00:37:32.000000 UniswapPy-1.2.0/python/prod/process/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.014263 UniswapPy-1.2.0/python/prod/process/burn/
--rw-r--r--   0 ian_moore   (501) staff       (20)     2470 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/process/burn/IndexTokenBurn.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       43 2024-02-07 00:37:32.000000 UniswapPy-1.2.0/python/prod/process/burn/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.014508 UniswapPy-1.2.0/python/prod/process/deposit/
--rw-r--r--   0 ian_moore   (501) staff       (20)     3690 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/process/deposit/SwapDeposit.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       36 2024-02-07 00:37:32.000000 UniswapPy-1.2.0/python/prod/process/deposit/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.014869 UniswapPy-1.2.0/python/prod/process/liquidity/
--rw-r--r--   0 ian_moore   (501) staff       (20)     2434 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/process/liquidity/AddLiquidity.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     2393 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/process/liquidity/RemoveLiquidity.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       83 2024-02-07 00:37:32.000000 UniswapPy-1.2.0/python/prod/process/liquidity/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.015111 UniswapPy-1.2.0/python/prod/process/mint/
--rw-r--r--   0 ian_moore   (501) staff       (20)     2747 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/process/mint/SwapIndexMint.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       40 2024-02-07 00:37:32.000000 UniswapPy-1.2.0/python/prod/process/mint/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.015850 UniswapPy-1.2.0/python/prod/process/swap/
--rw-r--r--   0 ian_moore   (501) staff       (20)     2329 2024-04-10 18:17:44.000000 UniswapPy-1.2.0/python/prod/process/swap/RandomSwap.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     1805 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/process/swap/Swap.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     3996 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/process/swap/WithdrawSwap.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       96 2024-02-07 00:37:32.000000 UniswapPy-1.2.0/python/prod/process/swap/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.017005 UniswapPy-1.2.0/python/prod/simulate/
--rw-r--r--   0 ian_moore   (501) staff       (20)     3383 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/simulate/Arbitrage.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     4185 2024-04-10 18:17:44.000000 UniswapPy-1.2.0/python/prod/simulate/CorrectReserves.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     3648 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/simulate/MarkovState.py
--rw-r--r--   0 ian_moore   (501) staff       (20)    15429 2024-04-10 18:17:44.000000 UniswapPy-1.2.0/python/prod/simulate/QuantTerminal.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     2712 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/simulate/SimpleLPSimulation.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     1850 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/simulate/SolveDeltas.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      244 2024-04-10 18:17:44.000000 UniswapPy-1.2.0/python/prod/simulate/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:16.998821 UniswapPy-1.2.0/python/prod/utils/
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.017254 UniswapPy-1.2.0/python/prod/utils/client/
--rw-r--r--   0 ian_moore   (501) staff       (20)     2164 2024-04-10 18:17:44.000000 UniswapPy-1.2.0/python/prod/utils/client/API0x.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       24 2024-04-10 18:17:44.000000 UniswapPy-1.2.0/python/prod/utils/client/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.018595 UniswapPy-1.2.0/python/prod/utils/data/
--rw-r--r--   0 ian_moore   (501) staff       (20)    10464 2024-04-10 18:17:44.000000 UniswapPy-1.2.0/python/prod/utils/data/Chain0x.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      261 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/utils/data/ExchangeData.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      324 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/utils/data/FactoryData.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      341 2024-03-25 21:57:46.000000 UniswapPy-1.2.0/python/prod/utils/data/UniswapExchangeData.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      157 2024-04-10 18:17:44.000000 UniswapPy-1.2.0/python/prod/utils/data/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.018973 UniswapPy-1.2.0/python/prod/utils/interfaces/
--rw-r--r--   0 ian_moore   (501) staff       (20)      439 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/utils/interfaces/IExchange.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      506 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/utils/interfaces/IExchangeFactory.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       79 2024-02-07 00:37:49.000000 UniswapPy-1.2.0/python/prod/utils/interfaces/__init__.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       79 2024-04-12 22:51:17.019490 UniswapPy-1.2.0/setup.cfg
--rw-r--r--   0 ian_moore   (501) staff       (20)     1440 2024-04-12 22:46:30.000000 UniswapPy-1.2.0/setup.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.911008 UniswapPy-1.3.0/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1065 2024-02-07 00:37:32.000000 UniswapPy-1.3.0/LICENSE.txt
+-rw-r--r--   0 ian_moore   (501) staff       (20)     4544 2024-04-25 15:01:13.911077 UniswapPy-1.3.0/PKG-INFO
+-rw-r--r--   0 ian_moore   (501) staff       (20)     4248 2024-04-25 14:42:37.000000 UniswapPy-1.3.0/README.md
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.891244 UniswapPy-1.3.0/UniswapPy.egg-info/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     4544 2024-04-25 15:01:13.000000 UniswapPy-1.3.0/UniswapPy.egg-info/PKG-INFO
+-rw-r--r--   0 ian_moore   (501) staff       (20)     3565 2024-04-25 15:01:13.000000 UniswapPy-1.3.0/UniswapPy.egg-info/SOURCES.txt
+-rw-r--r--   0 ian_moore   (501) staff       (20)        1 2024-04-25 15:01:13.000000 UniswapPy-1.3.0/UniswapPy.egg-info/dependency_links.txt
+-rw-r--r--   0 ian_moore   (501) staff       (20)        1 2024-02-11 00:15:12.000000 UniswapPy-1.3.0/UniswapPy.egg-info/not-zip-safe
+-rw-r--r--   0 ian_moore   (501) staff       (20)       13 2024-04-25 15:01:13.000000 UniswapPy-1.3.0/UniswapPy.egg-info/requires.txt
+-rw-r--r--   0 ian_moore   (501) staff       (20)       10 2024-04-25 15:01:13.000000 UniswapPy-1.3.0/UniswapPy.egg-info/top_level.txt
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.888201 UniswapPy-1.3.0/python/
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.891373 UniswapPy-1.3.0/python/prod/
+-rw-r--r--   0 ian_moore   (501) staff       (20)      880 2024-04-25 02:25:34.000000 UniswapPy-1.3.0/python/prod/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.888577 UniswapPy-1.3.0/python/prod/cpt/
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.892746 UniswapPy-1.3.0/python/prod/cpt/exchg/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     7376 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/cpt/exchg/ChildUniswapExchange.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)    21642 2024-04-25 02:25:34.000000 UniswapPy-1.3.0/python/prod/cpt/exchg/UniswapExchange.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)    40686 2024-04-25 02:33:33.000000 UniswapPy-1.3.0/python/prod/cpt/exchg/UniswapV3Exchange.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      148 2024-04-23 22:24:39.000000 UniswapPy-1.3.0/python/prod/cpt/exchg/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.893263 UniswapPy-1.3.0/python/prod/cpt/factory/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     4228 2024-04-25 02:27:11.000000 UniswapPy-1.3.0/python/prod/cpt/factory/UniswapFactory.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       44 2024-02-07 00:37:49.000000 UniswapPy-1.3.0/python/prod/cpt/factory/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.894048 UniswapPy-1.3.0/python/prod/cpt/index/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1719 2024-02-13 21:41:28.000000 UniswapPy-1.3.0/python/prod/cpt/index/RebaseIndexToken.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1712 2024-02-13 21:41:15.000000 UniswapPy-1.3.0/python/prod/cpt/index/SettlementLPToken.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       96 2024-02-07 00:37:32.000000 UniswapPy-1.3.0/python/prod/cpt/index/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.895102 UniswapPy-1.3.0/python/prod/cpt/quote/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     6938 2024-02-13 21:15:34.000000 UniswapPy-1.3.0/python/prod/cpt/quote/IndexTokenQuote.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     6990 2024-02-13 21:32:43.000000 UniswapPy-1.3.0/python/prod/cpt/quote/LPQuote.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1752 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/cpt/quote/LPTokenQuote.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     4677 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/cpt/quote/TreeAmountQuote.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      157 2024-02-07 00:37:32.000000 UniswapPy-1.3.0/python/prod/cpt/quote/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.895558 UniswapPy-1.3.0/python/prod/cpt/vault/
+-rw-r--r--   0 ian_moore   (501) staff       (20)    15329 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/cpt/vault/IndexVault.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      651 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/cpt/vault/Vault.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       59 2024-02-07 00:37:32.000000 UniswapPy-1.3.0/python/prod/cpt/vault/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.895912 UniswapPy-1.3.0/python/prod/cpt/wallet/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     2646 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/cpt/wallet/Wallets.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       28 2024-02-07 00:37:32.000000 UniswapPy-1.3.0/python/prod/cpt/wallet/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.897031 UniswapPy-1.3.0/python/prod/erc/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1684 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/erc/DOAERC20.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1456 2024-04-10 18:17:44.000000 UniswapPy-1.3.0/python/prod/erc/ERC20.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1103 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/erc/IndexERC20.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1720 2024-02-13 20:20:33.000000 UniswapPy-1.3.0/python/prod/erc/LPERC20.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      119 2024-02-07 00:37:32.000000 UniswapPy-1.3.0/python/prod/erc/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.889014 UniswapPy-1.3.0/python/prod/math/
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.897495 UniswapPy-1.3.0/python/prod/math/basic/
+-rw-r--r--   0 ian_moore   (501) staff       (20)      500 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/math/basic/IDGenerator.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      485 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/math/basic/RoundFloat.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       52 2024-02-07 00:37:32.000000 UniswapPy-1.3.0/python/prod/math/basic/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.897883 UniswapPy-1.3.0/python/prod/math/interest/
+-rw-r--r--   0 ian_moore   (501) staff       (20)      410 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/math/interest/CompoundReturn.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      519 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/math/interest/Yield.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       50 2024-02-07 00:37:32.000000 UniswapPy-1.3.0/python/prod/math/interest/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.898270 UniswapPy-1.3.0/python/prod/math/interest/ips/
+-rw-r--r--   0 ian_moore   (501) staff       (20)      766 2024-02-07 00:37:32.000000 UniswapPy-1.3.0/python/prod/math/interest/ips/ConstantIPS.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      390 2024-02-07 00:37:32.000000 UniswapPy-1.3.0/python/prod/math/interest/ips/IPS.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       45 2024-02-07 00:37:32.000000 UniswapPy-1.3.0/python/prod/math/interest/ips/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.898525 UniswapPy-1.3.0/python/prod/math/interest/ips/aggregate/
+-rw-r--r--   0 ian_moore   (501) staff       (20)      496 2024-02-07 00:37:32.000000 UniswapPy-1.3.0/python/prod/math/interest/ips/aggregate/AggregateIPS.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       27 2024-02-07 00:37:32.000000 UniswapPy-1.3.0/python/prod/math/interest/ips/aggregate/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.899289 UniswapPy-1.3.0/python/prod/math/model/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     2069 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/math/model/BrownianModel.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      504 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/math/model/EventSelectionModel.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      591 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/math/model/ModelQueue.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      762 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/math/model/TimeDeltaModel.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1262 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/math/model/TokenDeltaModel.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      151 2024-02-07 00:37:32.000000 UniswapPy-1.3.0/python/prod/math/model/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.899660 UniswapPy-1.3.0/python/prod/math/risk/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     5556 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/math/risk/MaxDrop.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       22 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/math/risk/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.899942 UniswapPy-1.3.0/python/prod/process/
+-rw-r--r--   0 ian_moore   (501) staff       (20)      300 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/process/Process.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       28 2024-02-07 00:37:32.000000 UniswapPy-1.3.0/python/prod/process/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.900315 UniswapPy-1.3.0/python/prod/process/burn/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     2470 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/process/burn/IndexTokenBurn.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       43 2024-02-07 00:37:32.000000 UniswapPy-1.3.0/python/prod/process/burn/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.900577 UniswapPy-1.3.0/python/prod/process/deposit/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     3690 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/process/deposit/SwapDeposit.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       36 2024-02-07 00:37:32.000000 UniswapPy-1.3.0/python/prod/process/deposit/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.901070 UniswapPy-1.3.0/python/prod/process/liquidity/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     2434 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/process/liquidity/AddLiquidity.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     2393 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/process/liquidity/RemoveLiquidity.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       83 2024-02-07 00:37:32.000000 UniswapPy-1.3.0/python/prod/process/liquidity/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.901427 UniswapPy-1.3.0/python/prod/process/mint/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     2747 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/process/mint/SwapIndexMint.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       40 2024-02-07 00:37:32.000000 UniswapPy-1.3.0/python/prod/process/mint/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.903885 UniswapPy-1.3.0/python/prod/process/swap/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     2329 2024-04-10 18:17:44.000000 UniswapPy-1.3.0/python/prod/process/swap/RandomSwap.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1805 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/process/swap/Swap.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     3996 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/process/swap/WithdrawSwap.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       96 2024-02-07 00:37:32.000000 UniswapPy-1.3.0/python/prod/process/swap/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.906994 UniswapPy-1.3.0/python/prod/simulate/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     3383 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/simulate/Arbitrage.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     4185 2024-04-10 18:17:44.000000 UniswapPy-1.3.0/python/prod/simulate/CorrectReserves.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     3648 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/simulate/MarkovState.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)    15429 2024-04-10 18:17:44.000000 UniswapPy-1.3.0/python/prod/simulate/QuantTerminal.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     2712 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/simulate/SimpleLPSimulation.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1850 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/simulate/SolveDeltas.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      244 2024-04-10 18:17:44.000000 UniswapPy-1.3.0/python/prod/simulate/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.889730 UniswapPy-1.3.0/python/prod/utils/
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.907597 UniswapPy-1.3.0/python/prod/utils/client/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     2164 2024-04-10 18:17:44.000000 UniswapPy-1.3.0/python/prod/utils/client/API0x.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       24 2024-04-10 18:17:44.000000 UniswapPy-1.3.0/python/prod/utils/client/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.908484 UniswapPy-1.3.0/python/prod/utils/data/
+-rw-r--r--   0 ian_moore   (501) staff       (20)    10464 2024-04-25 01:17:59.000000 UniswapPy-1.3.0/python/prod/utils/data/Chain0x.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      261 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/utils/data/ExchangeData.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      324 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/utils/data/FactoryData.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      628 2024-04-23 22:24:39.000000 UniswapPy-1.3.0/python/prod/utils/data/UniswapExchangeData.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      157 2024-04-10 18:17:44.000000 UniswapPy-1.3.0/python/prod/utils/data/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.908920 UniswapPy-1.3.0/python/prod/utils/interfaces/
+-rw-r--r--   0 ian_moore   (501) staff       (20)      439 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/utils/interfaces/IExchange.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      506 2024-02-11 00:47:28.000000 UniswapPy-1.3.0/python/prod/utils/interfaces/IExchangeFactory.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       79 2024-02-07 00:37:49.000000 UniswapPy-1.3.0/python/prod/utils/interfaces/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.889767 UniswapPy-1.3.0/python/prod/utils/tools/
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-25 15:01:13.910856 UniswapPy-1.3.0/python/prod/utils/tools/v3/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1331 2024-04-25 02:27:11.000000 UniswapPy-1.3.0/python/prod/utils/tools/v3/FullMath.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      844 2024-04-25 02:27:11.000000 UniswapPy-1.3.0/python/prod/utils/tools/v3/LiquidityMath.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     4659 2024-04-24 18:20:10.000000 UniswapPy-1.3.0/python/prod/utils/tools/v3/Position.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1928 2024-04-24 18:20:10.000000 UniswapPy-1.3.0/python/prod/utils/tools/v3/SafeMath.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     6201 2024-04-24 18:20:10.000000 UniswapPy-1.3.0/python/prod/utils/tools/v3/Shared.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)    10440 2024-04-24 18:20:10.000000 UniswapPy-1.3.0/python/prod/utils/tools/v3/SqrtPriceMath.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     4961 2024-04-24 18:20:10.000000 UniswapPy-1.3.0/python/prod/utils/tools/v3/SwapMath.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     7724 2024-04-24 18:20:10.000000 UniswapPy-1.3.0/python/prod/utils/tools/v3/Tick.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     6407 2024-04-24 18:20:10.000000 UniswapPy-1.3.0/python/prod/utils/tools/v3/TickMath.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     7573 2024-04-25 02:27:11.000000 UniswapPy-1.3.0/python/prod/utils/tools/v3/UniV3Utils.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      266 2024-04-25 02:27:11.000000 UniswapPy-1.3.0/python/prod/utils/tools/v3/__init__.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       79 2024-04-25 15:01:13.911280 UniswapPy-1.3.0/setup.cfg
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1478 2024-04-23 22:24:39.000000 UniswapPy-1.3.0/setup.py
```

### Comparing `UniswapPy-1.2.0/LICENSE.txt` & `UniswapPy-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.2.0/PKG-INFO` & `UniswapPy-1.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: UniswapPy
-Version: 1.2.0
+Version: 1.3.0
 Summary: Uniswap Analytics with Python
 Home-page: https://github.com/defipy-devs/uniswappy
 Author: icmoore
 Author-email: defipy.devs@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# UniswapPy: Uniswap Analytics with Python
-This package is a python re-factor of the original [Uniswap V2 pairing 
-code](https://github.com/Uniswap/v2-core/blob/master/contracts/UniswapV2Pair.sol) 
-and can be 
-utilized for the purpose of analysing and modelling its behavior for DeFi
+# UniswapPy: Uniswap V2 / V3 Analytics with Python
+This package contains python re-factors of both original Uniswap [V2](https://github.com/Uniswap/v2-core/blob/master/contracts/UniswapV2Pair.sol) and [V3](https://github.com/Uniswap/v3-core/blob/main/contracts/UniswapV3Pool.sol)
+pairing codes, and can be utilized for the purpose of analysing and modelling its behavior for DeFi
 
 ## Docs
 Visit [docs](https://defipy.org) for full documentation with walk-through 
 tutorials
 
 ## Installation 
 ```
@@ -26,54 +24,76 @@
 > pip install .
 ```
 or
 ```
 > pip install UniswapPy
 ```
 
-## Basic Usage
+## Uniswap V2
 
 * See [test notebook](https://github.com/icmoore/uniswappy/blob/main/notebooks/tutorials/pairingcode.ipynb) 
 for basic usage
 
 ```
-from uniswappy.erc import ERC20
-from uniswappy.cpt.factory import UniswapFactory
-from uniswappy.utils.data import UniswapExchangeData
+from uniswappy import *
 
 user_nm = 'user_intro'
-eth_amount = 1000
-dai_amount = 1000000
+eth_amount = 3162.277660168379
+dai_amount = 316227.7660168379
 
 dai = ERC20("DAI", "0x111")
 eth = ERC20("ETH", "0x09")
 exchg_data = UniswapExchangeData(tkn0 = eth, tkn1 = dai, symbol="LP", 
 address="0x011")
 
 factory = UniswapFactory("ETH pool factory", "0x2")
 lp = factory.deploy(exchg_data)
 lp.add_liquidity("user0", eth_amount, dai_amount, eth_amount, dai_amount)
 lp.summary()
 ```
 
 #### OUTPUT:
 Exchange ETH-DAI (LP) <br/>
-Reserves: ETH = 1000, DAI = 1000000 <br/>
-Liquidity: 31622.776601683792 <br/><br/>
+Reserves: ETH = 3162.277660168379, DAI = 316227.7660168379  <br/>
+Liquidity: 31622.776601683792 <br/><br/> 
+
+
+## Uniswap V3
+
+* See [test notebook](https://github.com/defipy-devs/uniswappy/blob/main/notebooks/tutorials/uniswap_v3.ipynb) 
+for basic usage
+
 ```
-from uniswappy.process.swap import Swap
+user = 'user_intro'
+fee = UniV3Utils.FeeAmount.MEDIUM
+tick_spacing = UniV3Utils.TICK_SPACINGS[fee]
+lwr_tick = UniV3Utils.getMinTick(tick_spacing)
+upr_tick = UniV3Utils.getMaxTick(tick_spacing)
+init_price = UniV3Utils.encodePriceSqrt(100, 1)
+
+dai = ERC20("DAI", "0x09")
+eth = ERC20("ETH", "0x111")
 
-out = Swap().apply(lp, dai, user_nm, 1000)
+exchg_data = UniswapExchangeData(tkn0 = eth, tkn1 = dai, symbol="LP", 
+                                   address="0x011", version = 'V3', 
+                                   tick_spacing = tick_spacing, 
+                                   fee = fee)
+
+factory = UniswapFactory("ETH pool factory", "0x2")
+lp = factory.deploy(exchg_data)
+lp.initialize(init_price)
+out = lp.mint(user, lwr_tick, upr_tick, 31622.776601683792)
 lp.summary()
 ```
 
 #### OUTPUT:
 Exchange ETH-DAI (LP) <br/>
-Reserves: ETH = 999.00399301896, DAI = 1001000 <br/>
-Liquidity: 31622.776601683792 <br/><br/>
+Reserves: ETH = 3162.277660168379, DAI = 316227.7660168379 <br/>
+Liquidity: 31622.776601683792 <br/><br/>  
+
 
 ## 0x Quant Terminal
 
 This application utilizes the 0x API to produce a mock Uniswap pool which allows end-users to stress test
 the limitations of a Uniswap pool setup using live price feeds from [0x API](https://0x.org); for backend setup, see 
 [notebook](https://github.com/defipy-devs/uniswappy/blob/main/notebooks/tutorials/quant_terminal.ipynb)
```

### Comparing `UniswapPy-1.2.0/README.md` & `UniswapPy-1.3.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-# UniswapPy: Uniswap Analytics with Python
-This package is a python re-factor of the original [Uniswap V2 pairing 
-code](https://github.com/Uniswap/v2-core/blob/master/contracts/UniswapV2Pair.sol) 
-and can be 
-utilized for the purpose of analysing and modelling its behavior for DeFi
+# UniswapPy: Uniswap V2 / V3 Analytics with Python
+This package contains python re-factors of both original Uniswap [V2](https://github.com/Uniswap/v2-core/blob/master/contracts/UniswapV2Pair.sol) and [V3](https://github.com/Uniswap/v3-core/blob/main/contracts/UniswapV3Pool.sol)
+pairing codes, and can be utilized for the purpose of analysing and modelling its behavior for DeFi
 
 ## Docs
 Visit [docs](https://defipy.org) for full documentation with walk-through 
 tutorials
 
 ## Installation 
 ```
@@ -14,54 +12,76 @@
 > pip install .
 ```
 or
 ```
 > pip install UniswapPy
 ```
 
-## Basic Usage
+## Uniswap V2
 
 * See [test notebook](https://github.com/icmoore/uniswappy/blob/main/notebooks/tutorials/pairingcode.ipynb) 
 for basic usage
 
 ```
-from uniswappy.erc import ERC20
-from uniswappy.cpt.factory import UniswapFactory
-from uniswappy.utils.data import UniswapExchangeData
+from uniswappy import *
 
 user_nm = 'user_intro'
-eth_amount = 1000
-dai_amount = 1000000
+eth_amount = 3162.277660168379
+dai_amount = 316227.7660168379
 
 dai = ERC20("DAI", "0x111")
 eth = ERC20("ETH", "0x09")
 exchg_data = UniswapExchangeData(tkn0 = eth, tkn1 = dai, symbol="LP", 
 address="0x011")
 
 factory = UniswapFactory("ETH pool factory", "0x2")
 lp = factory.deploy(exchg_data)
 lp.add_liquidity("user0", eth_amount, dai_amount, eth_amount, dai_amount)
 lp.summary()
 ```
 
 #### OUTPUT:
 Exchange ETH-DAI (LP) <br/>
-Reserves: ETH = 1000, DAI = 1000000 <br/>
-Liquidity: 31622.776601683792 <br/><br/>
+Reserves: ETH = 3162.277660168379, DAI = 316227.7660168379  <br/>
+Liquidity: 31622.776601683792 <br/><br/> 
+
+
+## Uniswap V3
+
+* See [test notebook](https://github.com/defipy-devs/uniswappy/blob/main/notebooks/tutorials/uniswap_v3.ipynb) 
+for basic usage
+
 ```
-from uniswappy.process.swap import Swap
+user = 'user_intro'
+fee = UniV3Utils.FeeAmount.MEDIUM
+tick_spacing = UniV3Utils.TICK_SPACINGS[fee]
+lwr_tick = UniV3Utils.getMinTick(tick_spacing)
+upr_tick = UniV3Utils.getMaxTick(tick_spacing)
+init_price = UniV3Utils.encodePriceSqrt(100, 1)
+
+dai = ERC20("DAI", "0x09")
+eth = ERC20("ETH", "0x111")
 
-out = Swap().apply(lp, dai, user_nm, 1000)
+exchg_data = UniswapExchangeData(tkn0 = eth, tkn1 = dai, symbol="LP", 
+                                   address="0x011", version = 'V3', 
+                                   tick_spacing = tick_spacing, 
+                                   fee = fee)
+
+factory = UniswapFactory("ETH pool factory", "0x2")
+lp = factory.deploy(exchg_data)
+lp.initialize(init_price)
+out = lp.mint(user, lwr_tick, upr_tick, 31622.776601683792)
 lp.summary()
 ```
 
 #### OUTPUT:
 Exchange ETH-DAI (LP) <br/>
-Reserves: ETH = 999.00399301896, DAI = 1001000 <br/>
-Liquidity: 31622.776601683792 <br/><br/>
+Reserves: ETH = 3162.277660168379, DAI = 316227.7660168379 <br/>
+Liquidity: 31622.776601683792 <br/><br/>  
+
 
 ## 0x Quant Terminal
 
 This application utilizes the 0x API to produce a mock Uniswap pool which allows end-users to stress test
 the limitations of a Uniswap pool setup using live price feeds from [0x API](https://0x.org); for backend setup, see 
 [notebook](https://github.com/defipy-devs/uniswappy/blob/main/notebooks/tutorials/quant_terminal.ipynb)
```

### Comparing `UniswapPy-1.2.0/UniswapPy.egg-info/PKG-INFO` & `UniswapPy-1.3.0/UniswapPy.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: UniswapPy
-Version: 1.2.0
+Version: 1.3.0
 Summary: Uniswap Analytics with Python
 Home-page: https://github.com/defipy-devs/uniswappy
 Author: icmoore
 Author-email: defipy.devs@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# UniswapPy: Uniswap Analytics with Python
-This package is a python re-factor of the original [Uniswap V2 pairing 
-code](https://github.com/Uniswap/v2-core/blob/master/contracts/UniswapV2Pair.sol) 
-and can be 
-utilized for the purpose of analysing and modelling its behavior for DeFi
+# UniswapPy: Uniswap V2 / V3 Analytics with Python
+This package contains python re-factors of both original Uniswap [V2](https://github.com/Uniswap/v2-core/blob/master/contracts/UniswapV2Pair.sol) and [V3](https://github.com/Uniswap/v3-core/blob/main/contracts/UniswapV3Pool.sol)
+pairing codes, and can be utilized for the purpose of analysing and modelling its behavior for DeFi
 
 ## Docs
 Visit [docs](https://defipy.org) for full documentation with walk-through 
 tutorials
 
 ## Installation 
 ```
@@ -26,54 +24,76 @@
 > pip install .
 ```
 or
 ```
 > pip install UniswapPy
 ```
 
-## Basic Usage
+## Uniswap V2
 
 * See [test notebook](https://github.com/icmoore/uniswappy/blob/main/notebooks/tutorials/pairingcode.ipynb) 
 for basic usage
 
 ```
-from uniswappy.erc import ERC20
-from uniswappy.cpt.factory import UniswapFactory
-from uniswappy.utils.data import UniswapExchangeData
+from uniswappy import *
 
 user_nm = 'user_intro'
-eth_amount = 1000
-dai_amount = 1000000
+eth_amount = 3162.277660168379
+dai_amount = 316227.7660168379
 
 dai = ERC20("DAI", "0x111")
 eth = ERC20("ETH", "0x09")
 exchg_data = UniswapExchangeData(tkn0 = eth, tkn1 = dai, symbol="LP", 
 address="0x011")
 
 factory = UniswapFactory("ETH pool factory", "0x2")
 lp = factory.deploy(exchg_data)
 lp.add_liquidity("user0", eth_amount, dai_amount, eth_amount, dai_amount)
 lp.summary()
 ```
 
 #### OUTPUT:
 Exchange ETH-DAI (LP) <br/>
-Reserves: ETH = 1000, DAI = 1000000 <br/>
-Liquidity: 31622.776601683792 <br/><br/>
+Reserves: ETH = 3162.277660168379, DAI = 316227.7660168379  <br/>
+Liquidity: 31622.776601683792 <br/><br/> 
+
+
+## Uniswap V3
+
+* See [test notebook](https://github.com/defipy-devs/uniswappy/blob/main/notebooks/tutorials/uniswap_v3.ipynb) 
+for basic usage
+
 ```
-from uniswappy.process.swap import Swap
+user = 'user_intro'
+fee = UniV3Utils.FeeAmount.MEDIUM
+tick_spacing = UniV3Utils.TICK_SPACINGS[fee]
+lwr_tick = UniV3Utils.getMinTick(tick_spacing)
+upr_tick = UniV3Utils.getMaxTick(tick_spacing)
+init_price = UniV3Utils.encodePriceSqrt(100, 1)
+
+dai = ERC20("DAI", "0x09")
+eth = ERC20("ETH", "0x111")
 
-out = Swap().apply(lp, dai, user_nm, 1000)
+exchg_data = UniswapExchangeData(tkn0 = eth, tkn1 = dai, symbol="LP", 
+                                   address="0x011", version = 'V3', 
+                                   tick_spacing = tick_spacing, 
+                                   fee = fee)
+
+factory = UniswapFactory("ETH pool factory", "0x2")
+lp = factory.deploy(exchg_data)
+lp.initialize(init_price)
+out = lp.mint(user, lwr_tick, upr_tick, 31622.776601683792)
 lp.summary()
 ```
 
 #### OUTPUT:
 Exchange ETH-DAI (LP) <br/>
-Reserves: ETH = 999.00399301896, DAI = 1001000 <br/>
-Liquidity: 31622.776601683792 <br/><br/>
+Reserves: ETH = 3162.277660168379, DAI = 316227.7660168379 <br/>
+Liquidity: 31622.776601683792 <br/><br/>  
+
 
 ## 0x Quant Terminal
 
 This application utilizes the 0x API to produce a mock Uniswap pool which allows end-users to stress test
 the limitations of a Uniswap pool setup using live price feeds from [0x API](https://0x.org); for backend setup, see 
 [notebook](https://github.com/defipy-devs/uniswappy/blob/main/notebooks/tutorials/quant_terminal.ipynb)
```

### Comparing `UniswapPy-1.2.0/UniswapPy.egg-info/SOURCES.txt` & `UniswapPy-1.3.0/UniswapPy.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 UniswapPy.egg-info/dependency_links.txt
 UniswapPy.egg-info/not-zip-safe
 UniswapPy.egg-info/requires.txt
 UniswapPy.egg-info/top_level.txt
 python/prod/__init__.py
 python/prod/cpt/exchg/ChildUniswapExchange.py
 python/prod/cpt/exchg/UniswapExchange.py
+python/prod/cpt/exchg/UniswapV3Exchange.py
 python/prod/cpt/exchg/__init__.py
 python/prod/cpt/factory/UniswapFactory.py
 python/prod/cpt/factory/__init__.py
 python/prod/cpt/index/RebaseIndexToken.py
 python/prod/cpt/index/SettlementLPToken.py
 python/prod/cpt/index/__init__.py
 python/prod/cpt/quote/IndexTokenQuote.py
@@ -78,8 +79,19 @@
 python/prod/utils/data/Chain0x.py
 python/prod/utils/data/ExchangeData.py
 python/prod/utils/data/FactoryData.py
 python/prod/utils/data/UniswapExchangeData.py
 python/prod/utils/data/__init__.py
 python/prod/utils/interfaces/IExchange.py
 python/prod/utils/interfaces/IExchangeFactory.py
-python/prod/utils/interfaces/__init__.py
+python/prod/utils/interfaces/__init__.py
+python/prod/utils/tools/v3/FullMath.py
+python/prod/utils/tools/v3/LiquidityMath.py
+python/prod/utils/tools/v3/Position.py
+python/prod/utils/tools/v3/SafeMath.py
+python/prod/utils/tools/v3/Shared.py
+python/prod/utils/tools/v3/SqrtPriceMath.py
+python/prod/utils/tools/v3/SwapMath.py
+python/prod/utils/tools/v3/Tick.py
+python/prod/utils/tools/v3/TickMath.py
+python/prod/utils/tools/v3/UniV3Utils.py
+python/prod/utils/tools/v3/__init__.py
```

### Comparing `UniswapPy-1.2.0/python/prod/__init__.py` & `UniswapPy-1.3.0/python/prod/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,8 +16,9 @@
 from uniswappy.process.deposit import *
 from uniswappy.process.liquidity import *
 from uniswappy.process.mint import *
 from uniswappy.process.swap import *
 from uniswappy.simulate import *
 from uniswappy.utils.interfaces import *
 from uniswappy.utils.data import *
-from uniswappy.utils.client import *
+from uniswappy.utils.client import *
+from uniswappy.utils.tools.v3 import *
```

### Comparing `UniswapPy-1.2.0/python/prod/cpt/exchg/ChildUniswapExchange.py` & `UniswapPy-1.3.0/python/prod/cpt/exchg/ChildUniswapExchange.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.2.0/python/prod/cpt/exchg/UniswapExchange.py` & `UniswapPy-1.3.0/python/prod/cpt/exchg/UniswapExchange.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import math
 
 MINIMUM_LIQUIDITY = 1e-15
 
 class UniswapExchange(IExchange, LPERC20):
     
     """ 
-        Uniswap Exchange  
+        Uniswap V2 Exchange  
 
         Parameters
         -----------------
         self.factory_struct : FactoryInit
             Factory initialization data
         self.exchg_struct : UniswapExchangeInit
             Exchange initialization data           
@@ -39,14 +39,19 @@
         self.name =  f"{self.token0}-{self.token1}"
         self.symbol = exchg_struct.symbol
         self.liquidity_providers = {}
         self.last_liquidity_deposit = 0
         self.total_supply = 0
 
     def summary(self):
+
+        """ summary
+            Summary print-out of exchange, reserves and liquidity               
+        """  
+        
         print(f"Exchange {self.name} ({self.symbol})")
         print(f"Reserves: {self.token0} = {self.reserve0}, {self.token1} = {self.reserve1}")
         print(f"Liquidity: {self.total_supply} \n")
 
     def add_liquidity(self, _from_addr, amountADesired, amountBDesired, amountAMin, amountBMin):
         
         """ add_liquidity
```

### Comparing `UniswapPy-1.2.0/python/prod/cpt/factory/UniswapFactory.py` & `UniswapPy-1.3.0/python/prod/cpt/factory/UniswapFactory.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright [2023] [Ian Moore]
 # Distributed under the MIT License (license terms are at http://opensource.org/licenses/MIT).
 # Email: defipy.devs@gmail.com
 
 from ..exchg import UniswapExchange 
+from ..exchg import UniswapV3Exchange 
 from ...erc import ERC20
 from ...erc import LPERC20
 from ...utils.interfaces import IExchangeFactory 
 from ...utils.data import UniswapExchangeData
 from ...utils.data import FactoryData
 
 class UniswapFactory(IExchangeFactory):
@@ -50,23 +51,33 @@
                 Newly created exchange that is also a LP token                    
         """  
         
         token0 = exchg_data.tkn0
         token1 = exchg_data.tkn1
         symbol = exchg_data.symbol
         address = exchg_data.address
+        precision = exchg_data.precision
 
         assert symbol not in self.token_from_exchange, 'UniswapV2Factory: EXCHANGE_CREATED'
             
         self.parent_lp = token0.parent_lp if token0.type == 'index' else self.parent_lp
         self.parent_lp = token1.parent_lp if token1.type == 'index' else self.parent_lp 
         
         factory_struct = FactoryData(self.token_from_exchange,  self.parent_lp, self.name, self.address)
-        exchg_struct = UniswapExchangeData(tkn0 = token0, tkn1 = token1, symbol=symbol, address=address)
-        exchange = UniswapExchange(factory_struct, exchg_struct)       
+
+        match exchg_data.version:
+            case UniswapExchangeData.VERSION_V2:
+                exchg_struct = UniswapExchangeData(tkn0 = token0, tkn1 = token1, symbol=symbol, address=address)
+                exchange = UniswapExchange(factory_struct, exchg_struct) 
+            case UniswapExchangeData.VERSION_V3: 
+                exchg_struct = UniswapExchangeData(tkn0 = token0, tkn1 = token1, symbol=symbol, 
+                                                   address=address, version = UniswapExchangeData.VERSION_V3, 
+                                                   precision = precision, 
+                                                   tick_spacing = exchg_data.tick_spacing, fee = exchg_data.fee)                
+                exchange = UniswapV3Exchange(factory_struct, exchg_struct) 
         
         self.exchange_from_token[token0.token_name] = exchange
         self.token_from_exchange[exchange.name] = {token0.token_name: token0, token1.token_name: token1}
         
         return exchange
 
     def get_exchange(self, token):
```

### Comparing `UniswapPy-1.2.0/python/prod/cpt/index/RebaseIndexToken.py` & `UniswapPy-1.3.0/python/prod/cpt/index/RebaseIndexToken.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.2.0/python/prod/cpt/index/SettlementLPToken.py` & `UniswapPy-1.3.0/python/prod/cpt/index/SettlementLPToken.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.2.0/python/prod/cpt/quote/IndexTokenQuote.py` & `UniswapPy-1.3.0/python/prod/cpt/quote/IndexTokenQuote.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.2.0/python/prod/cpt/quote/LPQuote.py` & `UniswapPy-1.3.0/python/prod/cpt/quote/LPQuote.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.2.0/python/prod/cpt/quote/LPTokenQuote.py` & `UniswapPy-1.3.0/python/prod/cpt/quote/LPTokenQuote.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.2.0/python/prod/cpt/quote/TreeAmountQuote.py` & `UniswapPy-1.3.0/python/prod/cpt/quote/TreeAmountQuote.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.2.0/python/prod/cpt/vault/IndexVault.py` & `UniswapPy-1.3.0/python/prod/cpt/vault/IndexVault.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.2.0/python/prod/cpt/vault/Vault.py` & `UniswapPy-1.3.0/python/prod/cpt/vault/Vault.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.2.0/python/prod/cpt/wallet/Wallets.py` & `UniswapPy-1.3.0/python/prod/cpt/wallet/Wallets.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.2.0/python/prod/erc/DOAERC20.py` & `UniswapPy-1.3.0/python/prod/erc/DOAERC20.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.2.0/python/prod/erc/ERC20.py` & `UniswapPy-1.3.0/python/prod/erc/ERC20.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.2.0/python/prod/erc/IndexERC20.py` & `UniswapPy-1.3.0/python/prod/erc/IndexERC20.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.2.0/python/prod/erc/LPERC20.py` & `UniswapPy-1.3.0/python/prod/erc/LPERC20.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.2.0/python/prod/math/interest/Yield.py` & `UniswapPy-1.3.0/python/prod/math/interest/Yield.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.2.0/python/prod/math/interest/ips/ConstantIPS.py` & `UniswapPy-1.3.0/python/prod/math/interest/ips/ConstantIPS.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.2.0/python/prod/math/model/BrownianModel.py` & `UniswapPy-1.3.0/python/prod/math/model/BrownianModel.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.2.0/python/prod/math/model/ModelQueue.py` & `UniswapPy-1.3.0/python/prod/math/model/ModelQueue.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.2.0/python/prod/math/model/TimeDeltaModel.py` & `UniswapPy-1.3.0/python/prod/math/model/TimeDeltaModel.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.2.0/python/prod/math/model/TokenDeltaModel.py` & `UniswapPy-1.3.0/python/prod/math/model/TokenDeltaModel.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.2.0/python/prod/math/risk/MaxDrop.py` & `UniswapPy-1.3.0/python/prod/math/risk/MaxDrop.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.2.0/python/prod/process/burn/IndexTokenBurn.py` & `UniswapPy-1.3.0/python/prod/process/burn/IndexTokenBurn.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.2.0/python/prod/process/deposit/SwapDeposit.py` & `UniswapPy-1.3.0/python/prod/process/deposit/SwapDeposit.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.2.0/python/prod/process/liquidity/AddLiquidity.py` & `UniswapPy-1.3.0/python/prod/process/liquidity/AddLiquidity.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.2.0/python/prod/process/liquidity/RemoveLiquidity.py` & `UniswapPy-1.3.0/python/prod/process/liquidity/RemoveLiquidity.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.2.0/python/prod/process/mint/SwapIndexMint.py` & `UniswapPy-1.3.0/python/prod/process/mint/SwapIndexMint.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.2.0/python/prod/process/swap/RandomSwap.py` & `UniswapPy-1.3.0/python/prod/process/swap/RandomSwap.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.2.0/python/prod/process/swap/Swap.py` & `UniswapPy-1.3.0/python/prod/process/swap/Swap.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.2.0/python/prod/process/swap/WithdrawSwap.py` & `UniswapPy-1.3.0/python/prod/process/swap/WithdrawSwap.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.2.0/python/prod/simulate/Arbitrage.py` & `UniswapPy-1.3.0/python/prod/simulate/Arbitrage.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.2.0/python/prod/simulate/CorrectReserves.py` & `UniswapPy-1.3.0/python/prod/simulate/CorrectReserves.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.2.0/python/prod/simulate/MarkovState.py` & `UniswapPy-1.3.0/python/prod/simulate/MarkovState.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.2.0/python/prod/simulate/QuantTerminal.py` & `UniswapPy-1.3.0/python/prod/simulate/QuantTerminal.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.2.0/python/prod/simulate/SimpleLPSimulation.py` & `UniswapPy-1.3.0/python/prod/simulate/SimpleLPSimulation.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.2.0/python/prod/simulate/SolveDeltas.py` & `UniswapPy-1.3.0/python/prod/simulate/SolveDeltas.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.2.0/python/prod/utils/client/API0x.py` & `UniswapPy-1.3.0/python/prod/utils/client/API0x.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.2.0/python/prod/utils/data/Chain0x.py` & `UniswapPy-1.3.0/python/prod/utils/data/Chain0x.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.2.0/setup.py` & `UniswapPy-1.3.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(name='UniswapPy',
-      version='1.2.0',
+      version='1.3.0',
       description='Uniswap Analytics with Python',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/defipy-devs/uniswappy',
       author = "icmoore",
       author_email = "defipy.devs@gmail.com",
       license='MIT',
@@ -33,13 +33,14 @@
           'uniswappy.process.deposit',
           'uniswappy.process.liquidity',
           'uniswappy.process.mint',
           'uniswappy.process.swap',
           'uniswappy.simulate',
           'uniswappy.utils.interfaces',
           'uniswappy.utils.data',
-          'uniswappy.utils.client'
+          'uniswappy.utils.client',
+          'uniswappy.utils.tools.v3'
       ],
       install_requires=[
           'scipy >= 1.7.3'         
       ],
       zip_safe=False)
```

