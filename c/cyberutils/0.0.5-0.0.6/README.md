# Comparing `tmp/cyberutils-0.0.5.tar.gz` & `tmp/cyberutils-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberutils-0.0.5.tar", max compression
+gzip compressed data, was "cyberutils-0.0.6.tar", max compression
```

## Comparing `cyberutils-0.0.5.tar` & `cyberutils-0.0.6.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0     1075 2023-06-07 03:24:28.597267 cyberutils-0.0.5/LICENSE
--rw-r--r--   0        0        0     3913 2023-06-07 03:24:28.597267 cyberutils-0.0.5/README.md
--rw-r--r--   0        0        0      166 2023-06-07 03:24:28.597267 cyberutils-0.0.5/cyberutils/__init__.py
--rw-r--r--   0        0        0       77 2023-06-07 03:24:28.597267 cyberutils-0.0.5/cyberutils/bash/__init__.py
--rw-r--r--   0        0        0     2268 2023-06-07 03:24:28.597267 cyberutils-0.0.5/cyberutils/bash/execution.py
--rw-r--r--   0        0        0       40 2023-06-07 03:24:28.597267 cyberutils-0.0.5/cyberutils/contract/__init__.py
--rw-r--r--   0        0        0     3070 2023-06-07 03:24:28.597267 cyberutils-0.0.5/cyberutils/contract/execution.py
--rw-r--r--   0        0        0       93 2023-06-07 03:24:28.597267 cyberutils-0.0.5/cyberutils/graphql/__init__.py
--rw-r--r--   0        0        0     2238 2023-06-07 03:24:28.597267 cyberutils-0.0.5/cyberutils/graphql/execution.py
--rw-r--r--   0        0        0     2032 2023-06-07 03:24:28.597267 cyberutils-0.0.5/cyberutils/graphql/queries.py
--rw-r--r--   0        0        0     1841 2023-06-07 03:24:28.597267 cyberutils-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     5392 1970-01-01 00:00:00.000000 cyberutils-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-04-25 01:33:39.045986 cyberutils-0.0.6/LICENSE
+-rw-r--r--   0        0        0     4348 2024-04-25 01:33:39.045986 cyberutils-0.0.6/README.md
+-rw-r--r--   0        0        0      166 2024-04-25 01:33:39.045986 cyberutils-0.0.6/cyberutils/__init__.py
+-rw-r--r--   0        0        0       77 2024-04-25 01:33:39.045986 cyberutils-0.0.6/cyberutils/bash/__init__.py
+-rw-r--r--   0        0        0     2268 2024-04-25 01:33:39.045986 cyberutils-0.0.6/cyberutils/bash/execution.py
+-rw-r--r--   0        0        0      120 2024-04-25 01:33:39.045986 cyberutils-0.0.6/cyberutils/contract/__init__.py
+-rw-r--r--   0        0        0     3116 2024-04-25 01:33:39.045986 cyberutils-0.0.6/cyberutils/contract/execution.py
+-rw-r--r--   0        0        0     2985 2024-04-25 01:33:39.045986 cyberutils-0.0.6/cyberutils/contract/instantiate.py
+-rw-r--r--   0        0        0      704 2024-04-25 01:33:39.045986 cyberutils-0.0.6/cyberutils/contract/query.py
+-rw-r--r--   0        0        0       93 2024-04-25 01:33:39.045986 cyberutils-0.0.6/cyberutils/graphql/__init__.py
+-rw-r--r--   0        0        0     2238 2024-04-25 01:33:39.045986 cyberutils-0.0.6/cyberutils/graphql/execution.py
+-rw-r--r--   0        0        0     2032 2024-04-25 01:33:39.045986 cyberutils-0.0.6/cyberutils/graphql/queries.py
+-rw-r--r--   0        0        0     1841 2024-04-25 01:33:39.045986 cyberutils-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     5827 1970-01-01 00:00:00.000000 cyberutils-0.0.6/PKG-INFO
```

### Comparing `cyberutils-0.0.5/LICENSE` & `cyberutils-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cyberutils-0.0.5/README.md` & `cyberutils-0.0.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -74,14 +74,31 @@
     gas=500_000,
     fee_amount=0,
     fee_denom='boot',
     contract_execute_schema=contract_schema_json['execute'],
     memo='the first transfer')
 ```
 
+### query a cosmwasm contract
+
+```python
+from cyberutils.contract import query_contract
+
+query_contract(
+    query={
+        'get_asset': {
+            'chain_name': 'osmosis',
+            'base': 'ibc/FE2CD1E6828EC0FAB8AF39BAC45BC25B965BA67CCBC50C13A14BD610B0D1E2C4'
+        }
+    },
+    contract_address='bostrom1w33tanvadg6fw04suylew9akcagcwngmkvns476wwu40fpq36pms92re6u',
+    node_lcd_url='https://lcd.bostrom.cybernode.ai'
+)
+```
+
 ### execute a graphql query
 
 ```python
 import pandas as pd
 
 from cyberutils.graphql import execute_graphql
```

#### html2text {}

```diff
@@ -20,19 +20,24 @@
 "bostrom1xszmhkfjs3s00z2nvtn7evqxw3dtus6yr8e4pw", "amount": "1000000" } } #
 load a contract schema for an execute message validation contract_schema_json =
 \ requests.get( url='https://raw.githubusercontent.com/Snedashkovsky/cw-plus/
 main/contracts/cw20-base/schema/cw20-base.json' ).json() # execution of a
 contract execute_contract( execute_msgs=[execute_msg], wallet=wallet,
 contract_address=CONTRACT_ADDRESS, lcd_client=lcd_client, gas=500_000,
 fee_amount=0, fee_denom='boot', contract_execute_schema=contract_schema_json
-['execute'], memo='the first transfer') ``` ### execute a graphql query
-```python import pandas as pd from cyberutils.graphql import execute_graphql
-res = await execute_graphql( request=""" query AllContracts { contracts
-(order_by: {tx: desc_nulls_last}) { address admin code_id creation_time creator
-fees gas height label tx } } """, graphql_url='https://
+['execute'], memo='the first transfer') ``` ### query a cosmwasm contract
+```python from cyberutils.contract import query_contract query_contract( query=
+{ 'get_asset': { 'chain_name': 'osmosis', 'base': 'ibc/
+FE2CD1E6828EC0FAB8AF39BAC45BC25B965BA67CCBC50C13A14BD610B0D1E2C4' } },
+contract_address='bostrom1w33tanvadg6fw04suylew9akcagcwngmkvns476wwu40fpq36pms92re6u',
+node_lcd_url='https://lcd.bostrom.cybernode.ai' ) ``` ### execute a graphql
+query ```python import pandas as pd from cyberutils.graphql import
+execute_graphql res = await execute_graphql( request=""" query AllContracts
+{ contracts(order_by: {tx: desc_nulls_last}) { address admin code_id
+creation_time creator fees gas height label tx } } """, graphql_url='https://
 index.bostrom.cybernode.ai/v1/graphql') pd.DataFrame(res['contracts']) ``` a
 query with variable values ```python import pandas as pd from
 cyberutils.graphql import execute_graphql res = await execute_graphql
 ( request=""" query ContractsCodeID($code_id: bigint) { contracts(order_by:
 {tx: desc_nulls_last}, where: {code_id: {_eq: $code_id}}) { address admin
 creation_time creator fees gas height label tx code_id } } """,
 variable_values={"code_id": "3"}, graphql_url='https://
```

### Comparing `cyberutils-0.0.5/cyberutils/bash/execution.py` & `cyberutils-0.0.6/cyberutils/bash/execution.py`

 * *Files identical despite different names*

### Comparing `cyberutils-0.0.5/cyberutils/contract/execution.py` & `cyberutils-0.0.6/cyberutils/contract/execution.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,39 +19,40 @@
                      gas: int = 300_000,
                      wallet: Optional[Wallet] = None,
                      sender: Optional[Union[str, AccAddress]] = None,
                      sign_and_broadcast_tx: bool = True,
                      contract_execute_schema: Optional[dict] = None,
                      memo: Optional[str] = None) -> Optional[Union[BlockTxBroadcastResult, Tx]]:
     """
-    Execute contract list of messages for a contract in a transaction or get an unsigned transaction
+    Execute contract list of messages for a contract in a transaction or get an unsigned transaction.
+    You can validate messages by contract execute schema.
     :param execute_msgs: list of execute messages
     :param contract_address: contract address
     :param lcd_client: network LCD client
     :param gas: amount of gas
     :param fee_amount: fee amount
     :param fee_denom: fee denom
     :param wallet: executable wallet
     :param sender: transaction sender address
     :param sign_and_broadcast_tx: sign and broadcast a transaction if true, otherwise return an unsigned transaction
     :param contract_execute_schema: schema of contract execute messages for message validation
-    :param memo: note(memo) of a transaction
+    :param memo: transaction note(memo)
     :return: a transaction result or an unsigned transaction
     """
     assert ((wallet or sender) and not sign_and_broadcast_tx) or (wallet and sign_and_broadcast_tx)
     if contract_execute_schema:
         for _execute_msg in execute_msgs:
             validate(_execute_msg, contract_execute_schema)
 
     _sender = wallet.key.acc_address if sender is None else AccAddress(sender)
     _msgs = \
         [MsgExecuteContract(
             sender=_sender,
             contract=AccAddress(contract_address),
-            execute_msg=execute_msg) for execute_msg in execute_msgs]
+            msg=execute_msg) for execute_msg in execute_msgs]
 
     if sign_and_broadcast_tx is False:
         return lcd_client.tx.create(
             signers=[SignerOptions(address=_sender)],
             options=CreateTxOptions(
                 msgs=_msgs,
                 memo=memo,
```

### Comparing `cyberutils-0.0.5/cyberutils/graphql/execution.py` & `cyberutils-0.0.6/cyberutils/graphql/execution.py`

 * *Files identical despite different names*

### Comparing `cyberutils-0.0.5/cyberutils/graphql/queries.py` & `cyberutils-0.0.6/cyberutils/graphql/queries.py`

 * *Files identical despite different names*

### Comparing `cyberutils-0.0.5/pyproject.toml` & `cyberutils-0.0.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 documentation = "https://github.com/Snedashkovsky/cyberutils"
 homepage = "https://github.com/Snedashkovsky/cyberutils"
 keywords = ["bostrom", "cyber", "knowledge-graph", "dex", "swap", "defi", "crypto", "blockchain", ]
 license = "MIT"
 packages = [{ include = "cyberutils" }]
 readme = "README.md"
 repository = "https://github.com/Snedashkovsky/cyberutils.git"
-version = "0.0.5"
+version = "0.0.6"
 
 [tool.poetry.dependencies]
 pandas = "^1.0.0"
 numpy = "^1.0.0"
 python-dotenv = "^0.20.0"
 tqdm = "^4.0.0"
 ipython = "^8.0.0"
```

### Comparing `cyberutils-0.0.5/PKG-INFO` & `cyberutils-0.0.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberutils
-Version: 0.0.5
+Version: 0.0.6
 Summary: the toolset for cyber protocol and cosmos ecosystem
 Home-page: https://github.com/Snedashkovsky/cyberutils
 License: MIT
 Keywords: bostrom,cyber,knowledge-graph,dex,swap,defi,crypto,blockchain
 Author: Snedashkovsky,
 Author-email: sn@cyberdrop.ai
 Requires-Python: >=3.9,<4.0
@@ -109,14 +109,31 @@
     gas=500_000,
     fee_amount=0,
     fee_denom='boot',
     contract_execute_schema=contract_schema_json['execute'],
     memo='the first transfer')
 ```
 
+### query a cosmwasm contract
+
+```python
+from cyberutils.contract import query_contract
+
+query_contract(
+    query={
+        'get_asset': {
+            'chain_name': 'osmosis',
+            'base': 'ibc/FE2CD1E6828EC0FAB8AF39BAC45BC25B965BA67CCBC50C13A14BD610B0D1E2C4'
+        }
+    },
+    contract_address='bostrom1w33tanvadg6fw04suylew9akcagcwngmkvns476wwu40fpq36pms92re6u',
+    node_lcd_url='https://lcd.bostrom.cybernode.ai'
+)
+```
+
 ### execute a graphql query
 
 ```python
 import pandas as pd
 
 from cyberutils.graphql import execute_graphql
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberutils Version: 0.0.5 Summary: the toolset for
+Metadata-Version: 2.1 Name: cyberutils Version: 0.0.6 Summary: the toolset for
 cyber protocol and cosmos ecosystem Home-page: https://github.com/
 Snedashkovsky/cyberutils License: MIT Keywords: bostrom,cyber,knowledge-
 graph,dex,swap,defi,crypto,blockchain Author: Snedashkovsky, Author-email:
 sn@cyberdrop.ai Requires-Python: >=3.9,<4.0 Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: English Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
@@ -40,19 +40,24 @@
 "bostrom1xszmhkfjs3s00z2nvtn7evqxw3dtus6yr8e4pw", "amount": "1000000" } } #
 load a contract schema for an execute message validation contract_schema_json =
 \ requests.get( url='https://raw.githubusercontent.com/Snedashkovsky/cw-plus/
 main/contracts/cw20-base/schema/cw20-base.json' ).json() # execution of a
 contract execute_contract( execute_msgs=[execute_msg], wallet=wallet,
 contract_address=CONTRACT_ADDRESS, lcd_client=lcd_client, gas=500_000,
 fee_amount=0, fee_denom='boot', contract_execute_schema=contract_schema_json
-['execute'], memo='the first transfer') ``` ### execute a graphql query
-```python import pandas as pd from cyberutils.graphql import execute_graphql
-res = await execute_graphql( request=""" query AllContracts { contracts
-(order_by: {tx: desc_nulls_last}) { address admin code_id creation_time creator
-fees gas height label tx } } """, graphql_url='https://
+['execute'], memo='the first transfer') ``` ### query a cosmwasm contract
+```python from cyberutils.contract import query_contract query_contract( query=
+{ 'get_asset': { 'chain_name': 'osmosis', 'base': 'ibc/
+FE2CD1E6828EC0FAB8AF39BAC45BC25B965BA67CCBC50C13A14BD610B0D1E2C4' } },
+contract_address='bostrom1w33tanvadg6fw04suylew9akcagcwngmkvns476wwu40fpq36pms92re6u',
+node_lcd_url='https://lcd.bostrom.cybernode.ai' ) ``` ### execute a graphql
+query ```python import pandas as pd from cyberutils.graphql import
+execute_graphql res = await execute_graphql( request=""" query AllContracts
+{ contracts(order_by: {tx: desc_nulls_last}) { address admin code_id
+creation_time creator fees gas height label tx } } """, graphql_url='https://
 index.bostrom.cybernode.ai/v1/graphql') pd.DataFrame(res['contracts']) ``` a
 query with variable values ```python import pandas as pd from
 cyberutils.graphql import execute_graphql res = await execute_graphql
 ( request=""" query ContractsCodeID($code_id: bigint) { contracts(order_by:
 {tx: desc_nulls_last}, where: {code_id: {_eq: $code_id}}) { address admin
 creation_time creator fees gas height label tx code_id } } """,
 variable_values={"code_id": "3"}, graphql_url='https://
```

