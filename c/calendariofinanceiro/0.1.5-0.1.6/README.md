# Comparing `tmp/calendariofinanceiro-0.1.5.tar.gz` & `tmp/calendariofinanceiro-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calendariofinanceiro-0.1.5.tar", max compression
+gzip compressed data, was "calendariofinanceiro-0.1.6.tar", max compression
```

## Comparing `calendariofinanceiro-0.1.5.tar` & `calendariofinanceiro-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       76 2023-08-28 20:15:59.350856 calendariofinanceiro-0.1.5/calendariofinanceiro/__init__.py
--rw-r--r--   0        0        0     3820 2023-08-28 20:54:35.258524 calendariofinanceiro-0.1.5/calendariofinanceiro/calendariofinanceiro.py
--rw-r--r--   0        0        0    22770 2023-08-28 20:15:25.257097 calendariofinanceiro-0.1.5/calendariofinanceiro/feriados.py
--rw-r--r--   0        0        0      113 2023-08-28 17:52:08.907154 calendariofinanceiro-0.1.5/calendariofinanceiro/feriados.pyi
--rw-r--r--   0        0        0     1093 2023-08-28 17:17:50.061981 calendariofinanceiro-0.1.5/LICENSE
--rw-r--r--   0        0        0      809 2023-10-16 19:04:21.850532 calendariofinanceiro-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2248 2023-08-29 18:51:55.681718 calendariofinanceiro-0.1.5/README.md
--rw-r--r--   0        0        0     3180 1970-01-01 00:00:00.000000 calendariofinanceiro-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       76 2023-08-28 20:15:59.350856 calendariofinanceiro-0.1.6/calendariofinanceiro/__init__.py
+-rw-r--r--   0        0        0     4431 2024-04-25 19:28:25.810759 calendariofinanceiro-0.1.6/calendariofinanceiro/calendariofinanceiro.py
+-rw-r--r--   0        0        0    22770 2023-08-28 20:15:25.257097 calendariofinanceiro-0.1.6/calendariofinanceiro/feriados.py
+-rw-r--r--   0        0        0      113 2023-08-28 17:52:08.907154 calendariofinanceiro-0.1.6/calendariofinanceiro/feriados.pyi
+-rw-r--r--   0        0        0     1093 2023-08-28 17:17:50.061981 calendariofinanceiro-0.1.6/LICENSE
+-rw-r--r--   0        0        0      809 2024-04-25 19:29:47.346297 calendariofinanceiro-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2248 2023-08-29 18:51:55.681718 calendariofinanceiro-0.1.6/README.md
+-rw-r--r--   0        0        0     3231 1970-01-01 00:00:00.000000 calendariofinanceiro-0.1.6/PKG-INFO
```

### Comparing `calendariofinanceiro-0.1.5/calendariofinanceiro/calendariofinanceiro.py` & `calendariofinanceiro-0.1.6/calendariofinanceiro/calendariofinanceiro.py`

 * *Files 14% similar despite different names*

```diff
@@ -95,7 +95,22 @@
         o fechamento do mês anterior.
         :return: A data de fechamento do mês anterior.
         """
         fechamento_m1 = self.soma_dias_uteis(
             date(data.year, data.month, 1), -1
         )
         return fechamento_m1
+
+    def busca_fechamento_mes_ano(self, mes: int, ano: int) -> date:
+        """
+        A partir de um mês e ano, constrói a data de fechamento referente.
+
+        :param mes: Mês de referência do fechamento (Janeiro=1)
+        :param ano: Ano de referência do fechamento
+        :return: A data de fechamento correspondente ao mês e ano passados.
+        """
+        proximo_mes = mes + 1 if mes < 12 else 1
+        proximo_ano = ano if mes < 12 else ano + 1
+        fechamento = self.soma_dias_uteis(
+            date(proximo_ano, proximo_mes, 1), -1
+        )
+        return fechamento
```

### Comparing `calendariofinanceiro-0.1.5/calendariofinanceiro/feriados.py` & `calendariofinanceiro-0.1.6/calendariofinanceiro/feriados.py`

 * *Files identical despite different names*

### Comparing `calendariofinanceiro-0.1.5/LICENSE` & `calendariofinanceiro-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `calendariofinanceiro-0.1.5/pyproject.toml` & `calendariofinanceiro-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "calendariofinanceiro"
-version = "0.1.5"
+version = "0.1.6"
 description = "O pacote CalendarioFinanceiro é uma ferramenta Python projetada para facilitar a manipulação de datas financeiras em diferentes calendários, como 'onshore' (Brasil) e 'offshore'. Com este pacote, você pode realizar operações como adicionar dias úteis a uma data, criar listas de dias úteis entre intervalos de datas e muito mais. Ele é uma solução eficiente para lidar com cálculos de datas em cenários financeiros, onde a consideração de dias úteis e feriados é essencial."
 authors = ["eduardo.barreto <edugobarreto@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 workdays = "^1.4"
```

### Comparing `calendariofinanceiro-0.1.5/README.md` & `calendariofinanceiro-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `calendariofinanceiro-0.1.5/PKG-INFO` & `calendariofinanceiro-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: calendariofinanceiro
-Version: 0.1.5
+Version: 0.1.6
 Summary: O pacote CalendarioFinanceiro é uma ferramenta Python projetada para facilitar a manipulação de datas financeiras em diferentes calendários, como 'onshore' (Brasil) e 'offshore'. Com este pacote, você pode realizar operações como adicionar dias úteis a uma data, criar listas de dias úteis entre intervalos de datas e muito mais. Ele é uma solução eficiente para lidar com cálculos de datas em cenários financeiros, onde a consideração de dias úteis e feriados é essencial.
 Author: eduardo.barreto
 Author-email: edugobarreto@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: workdays (>=1.4,<2.0)
 Description-Content-Type: text/markdown
 
 # CalendarioFinanceiro
 O pacote CalendarioFinanceiro fornece funcionalidades para trabalhar com dias úteis, considerando diferentes calendários, como "onshore" (Brasil) e "offshore".
 
 ## Instalação
```

