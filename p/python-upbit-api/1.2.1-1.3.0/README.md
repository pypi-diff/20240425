# Comparing `tmp/python-upbit-api-1.2.1.tar.gz` & `tmp/python_upbit_api-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/jihye/PycharmProjects/python-upbit-api/dist/.tmp-7vhob2cz/python-upbit-api-1.2.1.tar", last modified: Fri Feb 23 13:53:01 2024, max compression
+gzip compressed data, was "/Users/jihye/PycharmProjects/python-upbit-api/dist/.tmp-byigf6nz/python_upbit_api-1.3.0.tar", last modified: Thu Apr 25 04:58:15 2024, max compression
```

## Comparing `python-upbit-api-1.2.1.tar` & `python_upbit_api-1.3.0.tar`

### file list

```diff
@@ -1,22 +1,20 @@
-drwxr-xr-x   0 jihye      (501) staff       (20)        0 2024-02-23 13:53:01.054101 python-upbit-api-1.2.1/
--rw-r--r--   0 jihye      (501) staff       (20)     1066 2023-04-28 03:15:30.000000 python-upbit-api-1.2.1/LICENSE
--rw-r--r--   0 jihye      (501) staff       (20)     9909 2024-02-23 13:53:01.053828 python-upbit-api-1.2.1/PKG-INFO
--rw-r--r--   0 jihye      (501) staff       (20)     7518 2023-05-22 03:07:38.000000 python-upbit-api-1.2.1/README.md
--rw-r--r--   0 jihye      (501) staff       (20)     1504 2024-02-23 13:52:31.000000 python-upbit-api-1.2.1/pyproject.toml
-drwxr-xr-x   0 jihye      (501) staff       (20)        0 2024-02-23 13:53:01.053444 python-upbit-api-1.2.1/python_upbit_api.egg-info/
--rw-r--r--   0 jihye      (501) staff       (20)     9909 2024-02-23 13:53:01.000000 python-upbit-api-1.2.1/python_upbit_api.egg-info/PKG-INFO
--rw-r--r--   0 jihye      (501) staff       (20)      386 2024-02-23 13:53:01.000000 python-upbit-api-1.2.1/python_upbit_api.egg-info/SOURCES.txt
--rw-r--r--   0 jihye      (501) staff       (20)        1 2024-02-23 13:53:01.000000 python-upbit-api-1.2.1/python_upbit_api.egg-info/dependency_links.txt
--rw-r--r--   0 jihye      (501) staff       (20)       44 2024-02-23 13:53:01.000000 python-upbit-api-1.2.1/python_upbit_api.egg-info/requires.txt
--rw-r--r--   0 jihye      (501) staff       (20)        6 2024-02-23 13:53:01.000000 python-upbit-api-1.2.1/python_upbit_api.egg-info/top_level.txt
--rw-r--r--   0 jihye      (501) staff       (20)       38 2024-02-23 13:53:01.054172 python-upbit-api-1.2.1/setup.cfg
-drwxr-xr-x   0 jihye      (501) staff       (20)        0 2024-02-23 13:53:01.051452 python-upbit-api-1.2.1/tests/
--rw-r--r--   0 jihye      (501) staff       (20)     1586 2023-05-30 04:07:24.000000 python-upbit-api-1.2.1/tests/test.py
--rw-r--r--   0 jihye      (501) staff       (20)     1248 2023-05-11 03:13:33.000000 python-upbit-api-1.2.1/tests/test_remaining_req.py
--rw-r--r--   0 jihye      (501) staff       (20)     3174 2023-05-12 04:51:11.000000 python-upbit-api-1.2.1/tests/test_upbit.py
--rw-r--r--   0 jihye      (501) staff       (20)      131 2024-02-23 13:52:31.000000 python-upbit-api-1.2.1/tests/test_websocket.py
-drwxr-xr-x   0 jihye      (501) staff       (20)        0 2024-02-23 13:53:01.052574 python-upbit-api-1.2.1/upbit/
--rw-r--r--   0 jihye      (501) staff       (20)     1248 2024-02-23 13:47:25.000000 python-upbit-api-1.2.1/upbit/__init__.py
--rw-r--r--   0 jihye      (501) staff       (20)     3469 2023-05-11 03:13:33.000000 python-upbit-api-1.2.1/upbit/exceptions.py
--rw-r--r--   0 jihye      (501) staff       (20)     3986 2023-11-06 04:26:15.000000 python-upbit-api-1.2.1/upbit/models.py
--rw-r--r--   0 jihye      (501) staff       (20)    69108 2024-02-23 13:28:19.000000 python-upbit-api-1.2.1/upbit/upbit.py
+drwxr-xr-x   0 jihye      (501) staff       (20)        0 2024-04-25 04:58:15.656610 python_upbit_api-1.3.0/
+-rw-r--r--   0 jihye      (501) staff       (20)     1066 2023-04-28 03:15:30.000000 python_upbit_api-1.3.0/LICENSE
+-rw-r--r--   0 jihye      (501) staff       (20)    10153 2024-04-25 04:58:15.656347 python_upbit_api-1.3.0/PKG-INFO
+-rw-r--r--   0 jihye      (501) staff       (20)     7762 2024-04-25 04:39:48.000000 python_upbit_api-1.3.0/README.md
+-rw-r--r--   0 jihye      (501) staff       (20)     1504 2024-04-25 04:57:14.000000 python_upbit_api-1.3.0/pyproject.toml
+drwxr-xr-x   0 jihye      (501) staff       (20)        0 2024-04-25 04:58:15.655989 python_upbit_api-1.3.0/python_upbit_api.egg-info/
+-rw-r--r--   0 jihye      (501) staff       (20)    10153 2024-04-25 04:58:15.000000 python_upbit_api-1.3.0/python_upbit_api.egg-info/PKG-INFO
+-rw-r--r--   0 jihye      (501) staff       (20)      348 2024-04-25 04:58:15.000000 python_upbit_api-1.3.0/python_upbit_api.egg-info/SOURCES.txt
+-rw-r--r--   0 jihye      (501) staff       (20)        1 2024-04-25 04:58:15.000000 python_upbit_api-1.3.0/python_upbit_api.egg-info/dependency_links.txt
+-rw-r--r--   0 jihye      (501) staff       (20)       44 2024-04-25 04:58:15.000000 python_upbit_api-1.3.0/python_upbit_api.egg-info/requires.txt
+-rw-r--r--   0 jihye      (501) staff       (20)        6 2024-04-25 04:58:15.000000 python_upbit_api-1.3.0/python_upbit_api.egg-info/top_level.txt
+-rw-r--r--   0 jihye      (501) staff       (20)       38 2024-04-25 04:58:15.656667 python_upbit_api-1.3.0/setup.cfg
+drwxr-xr-x   0 jihye      (501) staff       (20)        0 2024-04-25 04:58:15.653478 python_upbit_api-1.3.0/tests/
+-rw-r--r--   0 jihye      (501) staff       (20)     1248 2023-05-11 03:13:33.000000 python_upbit_api-1.3.0/tests/test_remaining_req.py
+-rw-r--r--   0 jihye      (501) staff       (20)     3174 2023-05-12 04:51:11.000000 python_upbit_api-1.3.0/tests/test_upbit.py
+drwxr-xr-x   0 jihye      (501) staff       (20)        0 2024-04-25 04:58:15.655091 python_upbit_api-1.3.0/upbit/
+-rw-r--r--   0 jihye      (501) staff       (20)     1248 2024-02-23 13:47:25.000000 python_upbit_api-1.3.0/upbit/__init__.py
+-rw-r--r--   0 jihye      (501) staff       (20)     3469 2023-05-11 03:13:33.000000 python_upbit_api-1.3.0/upbit/exceptions.py
+-rw-r--r--   0 jihye      (501) staff       (20)     3986 2024-04-25 04:12:09.000000 python_upbit_api-1.3.0/upbit/models.py
+-rw-r--r--   0 jihye      (501) staff       (20)    73825 2024-04-25 04:53:05.000000 python_upbit_api-1.3.0/upbit/upbit.py
```

### Comparing `python-upbit-api-1.2.1/LICENSE` & `python_upbit_api-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-upbit-api-1.2.1/PKG-INFO` & `python_upbit_api-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-upbit-api
-Version: 1.2.1
+Version: 1.3.0
 Summary: Python Upbit API Wrapper
 Author-email: 이지혜 Lee Jihye <ghe.lee19@gmail.com>
 Maintainer-email: 이지혜 Lee Jihye <ghe.lee19@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Lee Jihye
         
@@ -127,14 +127,17 @@
 |  | 출금 허용 주소 리스트 조회 | get_withdraw_addresses |
 | 입금 | 입금 리스트 조회   | get_deposits |
 |  | 개별 입금 조회    | get_deposit |
 |  | 입금 주소 생성 요청 | create_coin_address |
 |  | 전체 입금 주소 조회 | get_coin_addresses |
 |  | 개별 입금 주소 조회 | get_coin_address |
 |  | 원화 입금하기  | create_deposit_krw |
+|  | 계정주 확인(트래블룰 검증)가능 거래소 리스트 조회 | get_vasps |
+|  | 입금 UUID로 트래블룰 검증하기 | verify_travel_rule_by_uuid |
+|  | 입금 TxID로 트래블룰 검증하기 | verify_travel_rule_by_txid |
 | 서비스 정보 | 입출금 현황 | get_wallet_status |
 |  | API 키 리스트 조회 | get_api_keys |
 | 시세 종목 조회 | 마켓 코드 조회 | get_markets |
 | 시세 캔들 조회 | 분(Minute) 캔들 | get_candles_minute |
 |  | 일(Day) 캔들 | get_candles_day |
 |  | 주(Week) 캔들 | get_candles_week |
 |  | 월(Month) 캔들 | get_candles_month |
```

### Comparing `python-upbit-api-1.2.1/README.md` & `python_upbit_api-1.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -79,14 +79,17 @@
 |  | 출금 허용 주소 리스트 조회 | get_withdraw_addresses |
 | 입금 | 입금 리스트 조회   | get_deposits |
 |  | 개별 입금 조회    | get_deposit |
 |  | 입금 주소 생성 요청 | create_coin_address |
 |  | 전체 입금 주소 조회 | get_coin_addresses |
 |  | 개별 입금 주소 조회 | get_coin_address |
 |  | 원화 입금하기  | create_deposit_krw |
+|  | 계정주 확인(트래블룰 검증)가능 거래소 리스트 조회 | get_vasps |
+|  | 입금 UUID로 트래블룰 검증하기 | verify_travel_rule_by_uuid |
+|  | 입금 TxID로 트래블룰 검증하기 | verify_travel_rule_by_txid |
 | 서비스 정보 | 입출금 현황 | get_wallet_status |
 |  | API 키 리스트 조회 | get_api_keys |
 | 시세 종목 조회 | 마켓 코드 조회 | get_markets |
 | 시세 캔들 조회 | 분(Minute) 캔들 | get_candles_minute |
 |  | 일(Day) 캔들 | get_candles_day |
 |  | 주(Week) 캔들 | get_candles_week |
 |  | 월(Month) 캔들 | get_candles_month |
```

### Comparing `python-upbit-api-1.2.1/pyproject.toml` & `python_upbit_api-1.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #where = ["src"]  # ["."] by default
 include = ["upbit*"]  # ["*"] by default
 #exclude = ["tests*"]  # empty by default
 #namespaces = true  # true by default
 
 [project]
 name = "python-upbit-api"
-version = "1.2.1"
+version = "1.3.0"
 authors = [
     {name = "이지혜 Lee Jihye", email = "ghe.lee19@gmail.com"},
 ]
 maintainers = [
     {name = "이지혜 Lee Jihye", email = "ghe.lee19@gmail.com"},
 ]
 description = "Python Upbit API Wrapper"
```

### Comparing `python-upbit-api-1.2.1/python_upbit_api.egg-info/PKG-INFO` & `python_upbit_api-1.3.0/python_upbit_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-upbit-api
-Version: 1.2.1
+Version: 1.3.0
 Summary: Python Upbit API Wrapper
 Author-email: 이지혜 Lee Jihye <ghe.lee19@gmail.com>
 Maintainer-email: 이지혜 Lee Jihye <ghe.lee19@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Lee Jihye
         
@@ -127,14 +127,17 @@
 |  | 출금 허용 주소 리스트 조회 | get_withdraw_addresses |
 | 입금 | 입금 리스트 조회   | get_deposits |
 |  | 개별 입금 조회    | get_deposit |
 |  | 입금 주소 생성 요청 | create_coin_address |
 |  | 전체 입금 주소 조회 | get_coin_addresses |
 |  | 개별 입금 주소 조회 | get_coin_address |
 |  | 원화 입금하기  | create_deposit_krw |
+|  | 계정주 확인(트래블룰 검증)가능 거래소 리스트 조회 | get_vasps |
+|  | 입금 UUID로 트래블룰 검증하기 | verify_travel_rule_by_uuid |
+|  | 입금 TxID로 트래블룰 검증하기 | verify_travel_rule_by_txid |
 | 서비스 정보 | 입출금 현황 | get_wallet_status |
 |  | API 키 리스트 조회 | get_api_keys |
 | 시세 종목 조회 | 마켓 코드 조회 | get_markets |
 | 시세 캔들 조회 | 분(Minute) 캔들 | get_candles_minute |
 |  | 일(Day) 캔들 | get_candles_day |
 |  | 주(Week) 캔들 | get_candles_week |
 |  | 월(Month) 캔들 | get_candles_month |
```

### Comparing `python-upbit-api-1.2.1/tests/test_remaining_req.py` & `python_upbit_api-1.3.0/tests/test_remaining_req.py`

 * *Files identical despite different names*

### Comparing `python-upbit-api-1.2.1/tests/test_upbit.py` & `python_upbit_api-1.3.0/tests/test_upbit.py`

 * *Files identical despite different names*

### Comparing `python-upbit-api-1.2.1/upbit/__init__.py` & `python_upbit_api-1.3.0/upbit/__init__.py`

 * *Files identical despite different names*

### Comparing `python-upbit-api-1.2.1/upbit/exceptions.py` & `python_upbit_api-1.3.0/upbit/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-upbit-api-1.2.1/upbit/models.py` & `python_upbit_api-1.3.0/upbit/models.py`

 * *Files identical despite different names*

### Comparing `python-upbit-api-1.2.1/upbit/upbit.py` & `python_upbit_api-1.3.0/upbit/upbit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1211,14 +1211,132 @@
             "amount": amount,
             "two_factor_type": two_factor_type,
         }
         headers = self._get_request_headers(params, headers=kwargs.pop('headers', None))
 
         return self._request('post', url, headers=headers, json=params, **kwargs)
 
+    def get_vasps(self, **kwargs) -> Response:
+        """계정주 확인(트래블룰 검증)가능 거래소 리스트 조회
+
+        API 요청 및 응답에 대한 자세한 정보는 공식 문서 참고:
+        `Upbit API Doc <https://docs.upbit.com/reference/%ED%8A%B8%EB%9E%98%EB%B8%94%EB%A3%B0-%EA%B0%80%EB%8A%A5-%EA%B1%B0%EB%9E%98%EC%86%8C>`_
+
+        :param kwargs: `requests.Session.request` 호출에 사용할 파라미터
+
+        :raises upbit.exceptions.ApiKeyError: 인증 정보 없이 호출시 발생.
+
+        :return: API 서버 응답
+
+        Usage::
+
+            access_key = os.environ.get('UPBIT_OPEN_API_ACCESS_KEY')
+            secret_key = os.environ.get('UPBIT_OPEN_API_SECRET_KEY')
+            upbit = Upbit(access_key, secret_key)
+            res = upbit.get_vasps()
+            print(res.json())
+
+            [{
+              "vasp_name": "업비트 인도네시아",
+              "vasp_uuid": "00000000-0000-0000-0000-000000000000",
+              "depositable": True,
+              "withdrawable": True
+            }, ...]
+        """
+        url = self._endpoint + "/travel_rule/vasps"
+        headers = self._get_request_headers(headers=kwargs.pop('headers', None))
+
+        return self._request('get', url, headers=headers, **kwargs)
+
+    def verify_travel_rule_by_uuid(self, *,
+                                   vasp_uuid: str,
+                                   deposit_uuid: str,
+                                   **kwargs) -> Response:
+        """입금 UUID로 트래블룰 검증하기
+
+        API 요청 및 응답에 대한 자세한 정보는 공식 문서 참고:
+        `Upbit API Doc <https://docs.upbit.com/reference/%ED%8A%B8%EB%9E%98%EB%B8%94%EB%A3%B0-uuid>`_
+
+        :param vasp_uuid: 상대 거래소 UUID
+        :param deposit_uuid: 입금 UUID
+        :param kwargs: `requests.Session.request` 호출에 사용할 파라미터
+
+        :raises upbit.exceptions.ApiKeyError: 인증 정보 없이 호출시 발생.
+
+        :return: API 서버 응답
+
+        Usage::
+
+            access_key = os.environ.get('UPBIT_OPEN_API_ACCESS_KEY')
+            secret_key = os.environ.get('UPBIT_OPEN_API_SECRET_KEY')
+            upbit = Upbit(access_key, secret_key)
+            res = upbit.verify_travel_rule_by_uuid(deposit_uuid='xxx', vasp_uuid='xxx')
+            print(res.json())
+
+            {
+              "deposit_uuid": "00000000-0000-0000-0000-000000000000",
+              "verification_result": "verified",
+              "deposit_state": "PROCESSING"
+            }
+        """
+        url = self._endpoint + "/travel_rule/deposit/uuid"
+        params = {
+            "vasp_uuid": vasp_uuid,
+            "deposit_uuid": deposit_uuid,
+        }
+        headers = self._get_request_headers(params, headers=kwargs.pop('headers', None))
+
+        return self._request('post', url, headers=headers, json=params, **kwargs)
+
+    def verify_travel_rule_by_txid(self, *,
+                                   vasp_uuid: str,
+                                   txid: str,
+                                   currency: str,
+                                   net_type: str,
+                                   **kwargs) -> Response:
+        """입금 TxID로 트래블룰 검증하기
+
+        API 요청 및 응답에 대한 자세한 정보는 공식 문서 참고:
+        `Upbit API Doc <https://docs.upbit.com/reference/%ED%8A%B8%EB%9E%98%EB%B8%94%EB%A3%B0-txid>`_
+
+        :param vasp_uuid: 상대 거래소 UUID
+        :param txid: 입금 TxID
+        :param currency: 입금 화폐
+        :param net_type: 입금 네트워크 타입
+        :param kwargs: `requests.Session.request` 호출에 사용할 파라미터
+
+        :raises upbit.exceptions.ApiKeyError: 인증 정보 없이 호출시 발생.
+
+        :return: API 서버 응답
+
+        Usage::
+
+            access_key = os.environ.get('UPBIT_OPEN_API_ACCESS_KEY')
+            secret_key = os.environ.get('UPBIT_OPEN_API_SECRET_KEY')
+            upbit = Upbit(access_key, secret_key)
+            res = upbit.verify_travel_rule_by_txid(deposit_uuid='xxx', vasp_uuid='xxx')
+            print(res.json())
+
+            {
+              "deposit_uuid": "00000000-0000-0000-0000-000000000000",
+              "verification_result": "verified",
+              "deposit_state": "PROCESSING"
+            }
+        """
+        url = self._endpoint + "/travel_rule/deposit/txid"
+        params = {
+            "vasp_uuid": vasp_uuid,
+            "txid": txid,
+            "currency": currency,
+            "net_type": net_type,
+        }
+        headers = self._get_request_headers(params, headers=kwargs.pop('headers', None))
+
+        return self._request('post', url, headers=headers, json=params, **kwargs)
+
     # --------------------------------------------------------------------------
     # Exchange API > 서비스 정보
     # --------------------------------------------------------------------------
 
     def get_wallet_status(self,
                           **kwargs) -> Response:
         """입출금 현황 조회
```

