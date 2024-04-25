# Comparing `tmp/yut23_utils-0.1.1.tar.gz` & `tmp/yut23_utils-0.2.0.tar.gz`

## Comparing `yut23_utils-0.1.1.tar` & `yut23_utils-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,19 @@
--rw-r--r--   0        0        0     6069 2020-02-02 00:00:00.000000 yut23_utils-0.1.1/ruff_defaults.toml
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 yut23_utils-0.1.1/.github/workflows/lint.yml
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 yut23_utils-0.1.1/.github/workflows/test.yml
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 yut23_utils-0.1.1/src/yut23_utils/__about__.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 yut23_utils-0.1.1/src/yut23_utils/__init__.py
--rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 yut23_utils-0.1.1/src/yut23_utils/fp.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 yut23_utils-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     3587 2020-02-02 00:00:00.000000 yut23_utils-0.1.1/tests/test_fp.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 yut23_utils-0.1.1/.gitignore
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 yut23_utils-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 yut23_utils-0.1.1/README.md
--rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 yut23_utils-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 yut23_utils-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 yut23_utils-0.2.0/Makefile
+-rw-r--r--   0        0        0     6332 2020-02-02 00:00:00.000000 yut23_utils-0.2.0/ruff_defaults.toml
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 yut23_utils-0.2.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 yut23_utils-0.2.0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 yut23_utils-0.2.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 yut23_utils-0.2.0/.github/workflows/types.yml
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 yut23_utils-0.2.0/src/yut23_utils/__about__.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 yut23_utils-0.2.0/src/yut23_utils/__init__.py
+-rw-r--r--   0        0        0     3681 2020-02-02 00:00:00.000000 yut23_utils-0.2.0/src/yut23_utils/fp.py
+-rw-r--r--   0        0        0     6268 2020-02-02 00:00:00.000000 yut23_utils-0.2.0/src/yut23_utils/timing.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 yut23_utils-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 yut23_utils-0.2.0/tests/conftest.py
+-rw-r--r--   0        0        0     3891 2020-02-02 00:00:00.000000 yut23_utils-0.2.0/tests/test_fp.py
+-rw-r--r--   0        0        0     4641 2020-02-02 00:00:00.000000 yut23_utils-0.2.0/tests/test_timing.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 yut23_utils-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 yut23_utils-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 yut23_utils-0.2.0/README.md
+-rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 yut23_utils-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 yut23_utils-0.2.0/PKG-INFO
```

### Comparing `yut23_utils-0.1.1/ruff_defaults.toml` & `yut23_utils-0.2.0/ruff_defaults.toml`

 * *Files 13% similar despite different names*

```diff
@@ -45,14 +45,15 @@
   "B028",
   "B029",
   "B030",
   "B031",
   "B032",
   "B033",
   "B034",
+  "B035",
   "B904",
   "B905",
   "BLE001",
   "C400",
   "C401",
   "C402",
   "C403",
@@ -79,15 +80,14 @@
   "DTZ006",
   "DTZ007",
   "DTZ011",
   "DTZ012",
   "E101",
   "E401",
   "E402",
-  "E501",
   "E701",
   "E702",
   "E703",
   "E711",
   "E712",
   "E713",
   "E714",
@@ -169,14 +169,18 @@
   "ICN002",
   "ICN003",
   "INP001",
   "INT001",
   "INT002",
   "INT003",
   "ISC003",
+  "LOG001",
+  "LOG002",
+  "LOG007",
+  "LOG009",
   "N801",
   "N802",
   "N803",
   "N804",
   "N805",
   "N806",
   "N807",
@@ -189,16 +193,14 @@
   "N817",
   "N818",
   "N999",
   "PERF101",
   "PERF102",
   "PERF401",
   "PERF402",
-  "PGH001",
-  "PGH002",
   "PGH005",
   "PIE790",
   "PIE794",
   "PIE796",
   "PIE800",
   "PIE804",
   "PIE807",
@@ -212,14 +214,15 @@
   "PLC0414",
   "PLC3002",
   "PLE0100",
   "PLE0101",
   "PLE0116",
   "PLE0117",
   "PLE0118",
+  "PLE0237",
   "PLE0241",
   "PLE0302",
   "PLE0307",
   "PLE0604",
   "PLE0605",
   "PLE1142",
   "PLE1205",
@@ -326,14 +329,15 @@
   "PYI050",
   "PYI051",
   "PYI052",
   "PYI053",
   "PYI054",
   "PYI055",
   "PYI056",
+  "PYI058",
   "RET503",
   "RET504",
   "RET505",
   "RET506",
   "RET507",
   "RET508",
   "RSE102",
@@ -342,32 +346,36 @@
   "RUF003",
   "RUF005",
   "RUF006",
   "RUF007",
   "RUF008",
   "RUF009",
   "RUF010",
-  "RUF011",
   "RUF012",
   "RUF013",
   "RUF015",
   "RUF016",
+  "RUF017",
+  "RUF018",
+  "RUF019",
+  "RUF020",
   "RUF100",
-  "RUF200",
   "S101",
   "S102",
   "S103",
   "S104",
   "S105",
   "S106",
   "S107",
   "S108",
   "S110",
   "S112",
   "S113",
+  "S201",
+  "S202",
   "S301",
   "S302",
   "S303",
   "S304",
   "S305",
   "S306",
   "S307",
@@ -383,36 +391,44 @@
   "S318",
   "S319",
   "S320",
   "S321",
   "S323",
   "S324",
   "S501",
+  "S502",
+  "S503",
+  "S504",
+  "S505",
   "S506",
+  "S507",
   "S508",
   "S509",
   "S601",
   "S602",
   "S604",
   "S605",
   "S606",
   "S607",
   "S608",
   "S609",
+  "S611",
   "S612",
   "S701",
+  "S702",
   "SIM101",
   "SIM102",
   "SIM103",
   "SIM105",
   "SIM107",
   "SIM108",
   "SIM109",
   "SIM110",
   "SIM112",
+  "SIM113",
   "SIM114",
   "SIM115",
   "SIM116",
   "SIM117",
   "SIM118",
   "SIM201",
   "SIM202",
@@ -422,37 +438,43 @@
   "SIM212",
   "SIM220",
   "SIM221",
   "SIM222",
   "SIM223",
   "SIM300",
   "SIM910",
+  "SIM911",
   "SLF001",
   "SLOT000",
   "SLOT001",
   "SLOT002",
   "T100",
   "T201",
   "T203",
   "TCH001",
   "TCH002",
   "TCH003",
   "TCH004",
   "TCH005",
+  "TCH010",
   "TD004",
   "TD005",
   "TD006",
   "TD007",
   "TID251",
   "TID252",
   "TID253",
+  "TRIO100",
+  "TRIO105",
+  "TRIO109",
+  "TRIO110",
+  "TRIO115",
   "TRY002",
   "TRY003",
   "TRY004",
-  "TRY200",
   "TRY201",
   "TRY300",
   "TRY301",
   "TRY302",
   "TRY400",
   "TRY401",
   "UP001",
@@ -489,14 +511,15 @@
   "UP034",
   "UP035",
   "UP036",
   "UP037",
   "UP038",
   "UP039",
   "UP040",
+  "UP041",
   "W291",
   "W292",
   "W293",
   "W505",
   "W605",
   "YTT101",
   "YTT102",
```

### Comparing `yut23_utils-0.1.1/.github/workflows/lint.yml` & `yut23_utils-0.2.0/.github/workflows/types.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-name: lint
+name: types
 
 on:
   push:
     branches: [main]
   pull_request:
     branches: [main]
 
 concurrency:
-  group: lint-${{ github.head_ref }}
+  group: types-${{ github.head_ref }}
   cancel-in-progress: true
 
 env:
   PYTHONUNBUFFERED: "1"
   FORCE_COLOR: "1"
 
 jobs:
   run:
-    name: Lint with ruff
+    name: Check types with mypy
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
 
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
-          python-version: 3.8
+          python-version: 3.9
 
       - name: Install Hatch
         run: pip install --upgrade hatch
 
       - name: Run linter
-        run: hatch fmt --linter --check
+        run: hatch run types:check
```

### Comparing `yut23_utils-0.1.1/.github/workflows/test.yml` & `yut23_utils-0.2.0/.github/workflows/test.yml`

 * *Files 14% similar despite different names*

```diff
@@ -19,26 +19,32 @@
     name: Python ${{ matrix.python-version }} on ${{ startsWith(matrix.os, 'macos-') && 'macOS' || startsWith(matrix.os, 'windows-') && 'Windows' || 'Linux' }}
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest, windows-latest, macos-latest]
         python-version: ['3.9', '3.10', '3.11', '3.12']
+        # Python 3.9 is on macos-13 but not macos-latest (macos-14-arm64)
+        # https://github.com/actions/setup-python/issues/696#issuecomment-1637587760
+        exclude:
+          - {python-version: "3.9", os: "macos-latest"}
+        include:
+          - {python-version: "3.9", os: "macos-13"}
 
     steps:
       - uses: actions/checkout@v4
 
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install Hatch
         run: pip install --upgrade hatch
 
       - name: Run tests
         run: hatch run cov-ci
 
       - name: Upload coverage reports to Codecov
-        uses: codecov/codecov-action@v3
+        uses: codecov/codecov-action@v4
         env:
           CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `yut23_utils-0.1.1/src/yut23_utils/fp.py` & `yut23_utils-0.2.0/src/yut23_utils/fp.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,25 +20,30 @@
 
 def ulp_diff(a: float, b: float, /, *, include_sign: bool = False) -> int:
     """Return the number of representable FP64 values in the range [a, b)."""
     if not math.isfinite(a) or not math.isfinite(b):
         msg = "only finite values can be compared"
         raise ValueError(msg)
     if a == b:
+        # this case also covers 0.0 vs -0.0, which compare equal but have
+        # different representations
         return 0
     if a > b:
         # pylint: disable-next=arguments-out-of-order
         ulps = ulp_diff(b, a)
         if include_sign:
             ulps *= -1
         return ulps
+    # b is now greater than a in value
     if math.copysign(1.0, a) != math.copysign(1.0, b):
         # different signs: split the interval at zero
         return ulp_diff(a, -0.0) + ulp_diff(0.0, b)
-    return abs(float_to_int(a) - float_to_int(b))
+    # subtract the smaller in magnitude from the larger
+    smaller, larger = sorted((a, b), key=abs)
+    return float_to_int(larger) - float_to_int(smaller)
 
 
 def compare_ulp(a: float, b: float, /, ulps: int) -> bool:
     """Check if two numbers match to within a specified number of FP64 ULPs."""
     if ulps < 0:
         msg = "ulps must be non-negative"
         raise ValueError(msg)
```

### Comparing `yut23_utils-0.1.1/tests/test_fp.py` & `yut23_utils-0.2.0/tests/test_fp.py`

 * *Files 16% similar despite different names*

```diff
@@ -50,20 +50,26 @@
     note(f"a = {FloatInspector(a)}\nb = {FloatInspector(b)}")
     return a, b, ulps
 
 
 @given(float_pairs(max_ulps=100))
 @example((0.0, -5e-324, -1))
 @example((5e-324, 0.0, -1))
-@example((5e-324, -0.0, -1))
 @example((-5e-324, 5e-324, 2))
+@example((1, 2, 1 << 52))
+@example((2, 4, 1 << 52))
+@example((0, 1, 0x3FF << 52))
 def test_ulp_diff(args: tuple[float, float, int]) -> None:
     a, b, ulps = args
     assert ulp_diff(a, b) == abs(ulps)
+    assert ulp_diff(b, a) == abs(ulps)  # pylint: disable=arguments-out-of-order
     assert ulp_diff(a, b, include_sign=True) == ulps
+    assert ulp_diff(b, a, include_sign=True) == -ulps
+    assert ulp_diff(-b, -a, include_sign=True) == ulps
+    assert ulp_diff(-a, -b, include_sign=True) == -ulps
 
 
 @pytest.mark.parametrize(
     ("a", "b"),
     [
         (math.inf, 3.14),
         (math.inf, math.inf),
@@ -91,15 +97,15 @@
     if abs(ulps) > 0:
         assert not compare_ulp(a, b, abs(ulps) - 1)
     assert compare_ulp(a, b, abs(ulps) + 1)
 
 
 def test_compare_ulp_errors() -> None:
     with pytest.raises(ValueError, match="non-negative"):
-        compare_ulp(1.0, 1.0, -1)
+        compare_ulp(1.0, 1.0, ulps=-1)
 
 
 @given(st.floats())
 def test_float_inspector(x: float) -> None:
     fi = FloatInspector(x)
     note(f"fi={fi} (subnormal: {fi.is_subnormal()})")
     if not math.isnan(x):
```

### Comparing `yut23_utils-0.1.1/.gitignore` & `yut23_utils-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `yut23_utils-0.1.1/LICENSE.txt` & `yut23_utils-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `yut23_utils-0.1.1/README.md` & `yut23_utils-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `yut23_utils-0.1.1/pyproject.toml` & `yut23_utils-0.2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -33,40 +33,48 @@
 [tool.hatch.version]
 source = "regex_commit"
 path = "src/yut23_utils/__about__.py"
 tag_sign = false
 
 [tool.hatch.envs.default]
 dependencies = [
-  "coverage[toml]>=6.5",
+  "coverage[toml]>=7.2",
   "pytest",
   "hypothesis",
 ]
 [tool.hatch.envs.default.scripts]
-test = "pytest {args:tests}"
-test-cov = "coverage run -m pytest {args:tests}"
+# nested scripts don't consume {args}: https://github.com/pypa/hatch/issues/987
+# basically, the first word is recursively replaced by its script if present,
+# then formats are expanded
+test = "pytest {args}"
+test-ci = "pytest --hypothesis-profile=ci {args}"
+test-cov = "coverage run -m pytest {args}"
+test-cov-ci = "coverage run -m pytest --hypothesis-profile=ci {args}"
 cov-report = [
   "- coverage combine",
   "coverage report",
 ]
 cov = [
   "test-cov",
   "cov-report",
 ]
 cov-ci = [
-  "cov",
+  "test-cov-ci",
+  "cov-report",
   "- coverage xml",
 ]
 
 [[tool.hatch.envs.all.matrix]]
 python = ["3.9", "3.10", "3.11", "3.12"]
 
 [tool.hatch.envs.types]
 dependencies = [
   "mypy>=1.0.0",
+  "hypothesis",
+  "pytest",
 ]
 [tool.hatch.envs.types.scripts]
 check = "mypy --install-types --non-interactive {args:src/yut23_utils tests}"
 
 [tool.isort]
 known_first_party = ["yut23_utils"]
 
@@ -78,14 +86,15 @@
 [tool.ruff]
 target-version = "py39"
 line-length = 88
 extend = "ruff_defaults.toml"
 
 [tool.hatch.envs.hatch-static-analysis]
 config-path = "ruff_defaults.toml"
+dependencies = ["ruff==0.4.1"]
 
 [tool.ruff.lint.extend-per-file-ignores]
 # we expect unused imports in __init__.py, as it shouldn't have anything else
 "__init__.py" = ["F401"]
 
 [tool.coverage.run]
 source_pkgs = ["yut23_utils", "tests"]
@@ -96,13 +105,14 @@
 ]
 
 [tool.coverage.paths]
 yut23_utils = ["src/yut23_utils", "*/yut23-utils/src/yut23_utils"]
 tests = ["tests", "*/yut23-utils/tests"]
 
 [tool.coverage.report]
-exclude_lines = [
-  "no cov",
+exclude_also = [
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
   "def __repr__",
+  "raise AssertionError",
+  "raise NotImplementedError",
 ]
```

### Comparing `yut23_utils-0.1.1/PKG-INFO` & `yut23_utils-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yut23-utils
-Version: 0.1.1
+Version: 0.2.0
 Summary: Common code I find myself reaching for from multiple different repositories.
 Project-URL: Documentation, https://github.com/yut23/yut23-utils#readme
 Project-URL: Issues, https://github.com/yut23/yut23-utils/issues
 Project-URL: Source, https://github.com/yut23/yut23-utils
 Author-email: yut23 <yut23@gvljohnsons.com>
 License-Expression: BSD-3-Clause
 License-File: LICENSE.txt
```

