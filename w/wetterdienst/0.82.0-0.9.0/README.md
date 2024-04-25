# Comparing `tmp/wetterdienst-0.82.0.tar.gz` & `tmp/wetterdienst-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wetterdienst-0.82.0.tar", max compression
+gzip compressed data, was "wetterdienst-0.9.0.tar", last modified: Fri Oct  9 18:45:43 2020, max compression
```

## Comparing `wetterdienst-0.82.0.tar` & `wetterdienst-0.9.0.tar`

### file list

```diff
@@ -1,132 +1,54 @@
--rw-r--r--   0        0        0    28337 2024-04-25 21:09:05.499496 wetterdienst-0.82.0/CHANGELOG.rst
--rw-r--r--   0        0        0     3351 2024-04-25 21:09:05.499496 wetterdienst-0.82.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1079 2024-04-25 21:09:05.499496 wetterdienst-0.82.0/LICENSE
--rw-r--r--   0        0        0    14712 2024-04-25 21:09:05.499496 wetterdienst-0.82.0/README.rst
--rw-r--r--   0        0        0    11977 2024-04-25 21:09:05.515495 wetterdienst-0.82.0/pyproject.toml
--rw-r--r--   0        0        0     2230 2024-04-25 21:09:05.519495 wetterdienst-0.82.0/wetterdienst/__init__.py
--rw-r--r--   0        0        0     6147 2024-04-25 21:09:05.519495 wetterdienst-0.82.0/wetterdienst/api.py
--rw-r--r--   0        0        0      394 2024-04-25 21:09:05.519495 wetterdienst-0.82.0/wetterdienst/boot.py
--rw-r--r--   0        0        0      121 2024-04-25 21:09:05.519495 wetterdienst-0.82.0/wetterdienst/core/__init__.py
--rw-r--r--   0        0        0     1093 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/core/core.py
--rw-r--r--   0        0        0     2601 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/core/process.py
--rw-r--r--   0        0        0      121 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/core/timeseries/__init__.py
--rw-r--r--   0        0        0    20031 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/core/timeseries/export.py
--rw-r--r--   0        0        0    10213 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/core/timeseries/interpolate.py
--rw-r--r--   0        0        0    35988 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/core/timeseries/request.py
--rw-r--r--   0        0        0    20830 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/core/timeseries/result.py
--rw-r--r--   0        0        0     6513 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/core/timeseries/summarize.py
--rw-r--r--   0        0        0     2201 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/core/timeseries/tools.py
--rw-r--r--   0        0        0    25452 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/core/timeseries/values.py
--rw-r--r--   0        0        0      554 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/exceptions.py
--rw-r--r--   0        0        0      121 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/metadata/__init__.py
--rw-r--r--   0        0        0     1516 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/metadata/columns.py
--rw-r--r--   0        0        0      386 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/metadata/datarange.py
--rw-r--r--   0        0        0      322 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/metadata/extension.py
--rw-r--r--   0        0        0      239 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/metadata/kind.py
--rw-r--r--   0        0        0    34884 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/metadata/parameter.py
--rw-r--r--   0        0        0     2068 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/metadata/period.py
--rw-r--r--   0        0        0     2433 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/metadata/provider.py
--rw-r--r--   0        0        0     1625 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/metadata/resolution.py
--rw-r--r--   0        0        0      423 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/metadata/timezone.py
--rw-r--r--   0        0        0     3954 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/metadata/unit.py
--rw-r--r--   0        0        0      121 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/provider/__init__.py
--rw-r--r--   0        0        0      121 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/provider/dwd/__init__.py
--rw-r--r--   0        0        0      230 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/provider/dwd/dmo/__init__.py
--rw-r--r--   0        0        0    71153 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/provider/dwd/dmo/api.py
--rw-r--r--   0        0        0      121 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/provider/dwd/metadata/__init__.py
--rw-r--r--   0        0        0      392 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/provider/dwd/metadata/datetime.py
--rw-r--r--   0        0        0      263 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/provider/dwd/mosmix/__init__.py
--rw-r--r--   0        0        0     6484 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/provider/dwd/mosmix/access.py
--rw-r--r--   0        0        0    66790 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/provider/dwd/mosmix/api.py
--rw-r--r--   0        0        0      579 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/provider/dwd/observation/__init__.py
--rw-r--r--   0        0        0    22152 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/provider/dwd/observation/api.py
--rw-r--r--   0        0        0     2527 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/provider/dwd/observation/download.py
--rw-r--r--   0        0        0     4111 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/provider/dwd/observation/fields.py
--rw-r--r--   0        0        0     6884 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/provider/dwd/observation/fileindex.py
--rw-r--r--   0        0        0      503 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/provider/dwd/observation/metadata/__init__.py
--rw-r--r--   0        0        0     7886 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/provider/dwd/observation/metadata/dataset.py
--rw-r--r--   0        0        0    28214 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/provider/dwd/observation/metadata/parameter.py
--rw-r--r--   0        0        0      329 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/provider/dwd/observation/metadata/period.py
--rw-r--r--   0        0        0     1188 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/provider/dwd/observation/metadata/resolution.py
--rw-r--r--   0        0        0    35467 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/provider/dwd/observation/metadata/unit.py
--rw-r--r--   0        0        0    12989 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/provider/dwd/observation/metaindex.py
--rw-r--r--   0        0        0     9680 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/provider/dwd/observation/parser.py
--rw-r--r--   0        0        0      121 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/provider/dwd/observation/util/__init__.py
--rw-r--r--   0        0        0     1338 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/provider/dwd/observation/util/parameter.py
--rw-r--r--   0        0        0      652 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/provider/dwd/radar/README.rst
--rw-r--r--   0        0        0      437 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/provider/dwd/radar/__init__.py
--rw-r--r--   0        0        0    24192 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/provider/dwd/radar/api.py
--rw-r--r--   0        0        0     1158 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/provider/dwd/radar/cli.py
--rw-r--r--   0        0        0    10163 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/provider/dwd/radar/index.py
--rw-r--r--   0        0        0      584 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/provider/dwd/radar/metadata/__init__.py
--rw-r--r--   0        0        0     3518 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/provider/dwd/radar/metadata/parameter.py
--rw-r--r--   0        0        0      296 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/provider/dwd/radar/metadata/period.py
--rw-r--r--   0        0        0      347 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/provider/dwd/radar/metadata/resolution.py
--rw-r--r--   0        0        0     4191 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/provider/dwd/radar/sites.py
--rw-r--r--   0        0        0     1900 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/provider/dwd/radar/util.py
--rw-r--r--   0        0        0       62 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/provider/dwd/road/__init__.py
--rw-r--r--   0        0        0    17386 2024-04-25 21:09:05.523495 wetterdienst-0.82.0/wetterdienst/provider/dwd/road/api.py
--rw-r--r--   0        0        0      121 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/provider/ea/__init__.py
--rw-r--r--   0        0        0      253 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/provider/ea/hydrology/__init__.py
--rw-r--r--   0        0        0     7212 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/provider/ea/hydrology/api.py
--rw-r--r--   0        0        0      121 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/provider/eaufrance/__init__.py
--rw-r--r--   0        0        0      207 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/provider/eaufrance/hubeau/__init__.py
--rw-r--r--   0        0        0     9382 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/provider/eaufrance/hubeau/api.py
--rw-r--r--   0        0        0      121 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/provider/eccc/__init__.py
--rw-r--r--   0        0        0      331 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/provider/eccc/observation/__init__.py
--rw-r--r--   0        0        0    13438 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/provider/eccc/observation/api.py
--rw-r--r--   0        0        0      121 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/provider/eccc/observation/metadata/__init__.py
--rw-r--r--   0        0        0    10425 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/provider/eccc/observation/metadata/parameter.py
--rw-r--r--   0        0        0      352 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/provider/eccc/observation/metadata/resolution.py
--rw-r--r--   0        0        0    11362 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/provider/eccc/observation/metadata/unit.py
--rw-r--r--   0        0        0      121 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/provider/eumetnet/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/provider/eumetnet/opera/__init__.py
--rw-r--r--   0        0        0    11883 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/provider/eumetnet/opera/sites.json.gz
--rw-r--r--   0        0        0     5789 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/provider/eumetnet/opera/sites.py
--rw-r--r--   0        0        0      121 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/provider/geosphere/__init__.py
--rw-r--r--   0        0        0      322 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/provider/geosphere/observation/__init__.py
--rw-r--r--   0        0        0    47643 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/provider/geosphere/observation/api.py
--rw-r--r--   0        0        0      121 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/provider/imgw/__init__.py
--rw-r--r--   0        0        0      195 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/provider/imgw/hydrology/__init__.py
--rw-r--r--   0        0        0    16296 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/provider/imgw/hydrology/api.py
--rw-r--r--   0        0        0      199 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/provider/imgw/meteorology/__init__.py
--rw-r--r--   0        0        0    27715 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/provider/imgw/meteorology/api.py
--rw-r--r--   0        0        0      121 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/provider/noaa/__init__.py
--rw-r--r--   0        0        0      277 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/provider/noaa/ghcn/__init__.py
--rw-r--r--   0        0        0    22758 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/provider/noaa/ghcn/api.py
--rw-r--r--   0        0        0    54011 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/provider/noaa/ghcn/parameter.py
--rw-r--r--   0        0        0    41180 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/provider/noaa/ghcn/unit.py
--rw-r--r--   0        0        0      121 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/provider/nws/__init__.py
--rw-r--r--   0        0        0      235 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/provider/nws/observation/__init__.py
--rw-r--r--   0        0        0    11221 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/provider/nws/observation/api.py
--rw-r--r--   0        0        0      121 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/provider/wsv/__init__.py
--rw-r--r--   0        0        0      204 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/provider/wsv/pegel/__init__.py
--rw-r--r--   0        0        0    13323 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/provider/wsv/pegel/api.py
--rw-r--r--   0        0        0     6726 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/settings.py
--rw-r--r--   0        0        0        0 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/ui/__init__.py
--rw-r--r--   0        0        0    40526 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/ui/cli.py
--rw-r--r--   0        0        0    16961 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/ui/core.py
--rw-r--r--   0        0        0    24522 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/ui/restapi.py
--rw-r--r--   0        0        0        0 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/ui/streamlit/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/ui/streamlit/explorer/__init__.py
--rw-r--r--   0        0        0    11075 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/ui/streamlit/explorer/app.py
--rw-r--r--   0        0        0       38 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/ui/streamlit/explorer/requirements.txt
--rw-r--r--   0        0        0        0 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/ui/streamlit/warming_stripes/__init__.py
--rw-r--r--   0        0        0     6129 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/ui/streamlit/warming_stripes/app.py
--rw-r--r--   0        0        0       23 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/ui/streamlit/warming_stripes/requirements.txt
--rw-r--r--   0        0        0      121 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/util/__init__.py
--rw-r--r--   0        0        0      533 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/util/cache.py
--rw-r--r--   0        0        0     1353 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/util/cli.py
--rw-r--r--   0        0        0     3083 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/util/datetime.py
--rw-r--r--   0        0        0      874 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/util/eccodes.py
--rw-r--r--   0        0        0     2575 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/util/enumeration.py
--rw-r--r--   0        0        0     3118 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/util/geo.py
--rw-r--r--   0        0        0      502 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/util/io.py
--rw-r--r--   0        0        0      715 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/util/logging.py
--rw-r--r--   0        0        0     7253 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/util/network.py
--rw-r--r--   0        0        0      735 2024-04-25 21:09:05.527495 wetterdienst-0.82.0/wetterdienst/util/parameter.py
--rw-r--r--   0        0        0      646 2024-04-25 21:09:05.531495 wetterdienst-0.82.0/wetterdienst/util/pdf.py
--rw-r--r--   0        0        0     1628 2024-04-25 21:09:05.531495 wetterdienst-0.82.0/wetterdienst/util/polars_util.py
--rw-r--r--   0        0        0      882 2024-04-25 21:09:05.531495 wetterdienst-0.82.0/wetterdienst/util/python.py
--rw-r--r--   0        0        0     1445 2024-04-25 21:09:05.531495 wetterdienst-0.82.0/wetterdienst/util/url.py
--rw-r--r--   0        0        0    20757 1970-01-01 00:00:00.000000 wetterdienst-0.82.0/PKG-INFO
+-rw-r--r--   0        0        0     4121 2020-10-09 18:40:17.081995 wetterdienst-0.9.0/CHANGELOG.rst
+-rw-r--r--   0        0        0     1123 2020-10-09 18:40:17.081995 wetterdienst-0.9.0/LICENSE.rst
+-rw-r--r--   0        0        0     1123 2020-10-09 18:40:17.081995 wetterdienst-0.9.0/LICENSE.rst
+-rw-r--r--   0        0        0     5347 2020-10-09 18:40:17.081995 wetterdienst-0.9.0/README.rst
+-rw-r--r--   0        0        0     5569 2020-10-09 18:40:17.093996 wetterdienst-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      811 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/__init__.py
+-rw-r--r--   0        0        0    15631 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/cli.py
+-rw-r--r--   0        0        0       79 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/__init__.py
+-rw-r--r--   0        0        0     2457 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/index.py
+-rw-r--r--   0        0        0      227 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/metadata/__init__.py
+-rw-r--r--   0        0        0     2512 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/metadata/column_map.py
+-rw-r--r--   0        0        0    23344 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/metadata/column_names.py
+-rw-r--r--   0        0        0     7800 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/metadata/column_types.py
+-rw-r--r--   0        0        0      902 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/metadata/constants.py
+-rw-r--r--   0        0        0      265 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/metadata/datetime.py
+-rw-r--r--   0        0        0     4724 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/metadata/parameter.py
+-rw-r--r--   0        0        0     1723 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/metadata/period_type.py
+-rw-r--r--   0        0        0      939 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/metadata/time_resolution.py
+-rw-r--r--   0        0        0        0 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/mosmix/__init__.py
+-rw-r--r--   0        0        0     5566 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/mosmix/access.py
+-rw-r--r--   0        0        0     3916 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/mosmix/api.py
+-rw-r--r--   0        0        0     1080 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/network.py
+-rw-r--r--   0        0        0        0 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/observations/__init__.py
+-rw-r--r--   0        0        0     5539 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/observations/access.py
+-rw-r--r--   0        0        0    18455 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/observations/api.py
+-rw-r--r--   0        0        0     2708 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/observations/fields.py
+-rw-r--r--   0        0        0     3176 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/observations/fileindex.py
+-rw-r--r--   0        0        0    11418 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/observations/metaindex.py
+-rw-r--r--   0        0        0     4328 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/observations/parser.py
+-rw-r--r--   0        0        0    10122 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/observations/stations.py
+-rw-r--r--   0        0        0     3975 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/observations/store.py
+-rw-r--r--   0        0        0     6612 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/pandas.py
+-rw-r--r--   0        0        0        0 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/radar/__init__.py
+-rw-r--r--   0        0        0    12583 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/radar/access.py
+-rw-r--r--   0        0        0     9914 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/radar/api.py
+-rw-r--r--   0        0        0      989 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/radar/cli.py
+-rw-r--r--   0        0        0     9611 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/radar/index.py
+-rw-r--r--   0        0        0     3451 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/radar/metadata.py
+-rw-r--r--   0        0        0     6742 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/radar/sites.py
+-rw-r--r--   0        0        0     1445 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/radar/util.py
+-rw-r--r--   0        0        0     6004 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/dwd/util.py
+-rw-r--r--   0        0        0      362 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/exceptions.py
+-rw-r--r--   0        0        0      259 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/run.py
+-rw-r--r--   0        0        0     5065 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/service.py
+-rw-r--r--   0        0        0       80 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/util/__init__.py
+-rw-r--r--   0        0        0     1792 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/util/cache.py
+-rw-r--r--   0        0        0     1246 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/util/cli.py
+-rw-r--r--   0        0        0      887 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/util/datetime.py
+-rw-r--r--   0        0        0     1031 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/util/geo.py
+-rw-r--r--   0        0        0     1218 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/util/network.py
+-rw-r--r--   0        0        0     8691 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/util/pandas.py
+-rw-r--r--   0        0        0      371 2020-10-09 18:40:17.125996 wetterdienst-0.9.0/wetterdienst/util/pdf.py
+-rw-r--r--   0        0        0     8082 2020-10-09 18:45:44.075213 wetterdienst-0.9.0/setup.py
+-rw-r--r--   0        0        0     9752 2020-10-09 18:45:44.076029 wetterdienst-0.9.0/PKG-INFO
```

### Comparing `wetterdienst-0.82.0/LICENSE` & `wetterdienst-0.9.0/LICENSE.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2018-2023 earthobservations
+Copyright (c) 2018 earthobservations, Benjamin Gutzmann, Daniel Lassahn, Andreas Motl
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `wetterdienst-0.82.0/wetterdienst/provider/dwd/mosmix/access.py` & `wetterdienst-0.9.0/wetterdienst/dwd/mosmix/access.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,182 +1,174 @@
-# Copyright (C) 2018-2021, earthobservations developers.
-# Distributed under the MIT License. See LICENSE for more info.
 # Source:
 # https://github.com/jlewis91/dwdbulk/blob/master/dwdbulk/api/forecasts.py
-from __future__ import annotations
-
-import datetime as dt
 import logging
 from io import BytesIO
-from pathlib import Path
-from typing import TYPE_CHECKING
+from typing import List
+from zipfile import ZipFile
+from os.path import basename
 
-import polars as pl
-from fsspec.implementations.zip import ZipFileSystem
-from lxml.etree import iterparse  # noqa: S410
+from lxml import etree  # noqa:S410
+from pandas import DatetimeIndex
 from tqdm import tqdm
 
-from wetterdienst.util.cache import CacheExpiry
-from wetterdienst.util.io import read_in_chunks
-from wetterdienst.util.logging import TqdmToLogger
-from wetterdienst.util.network import NetworkFilesystemManager
-
-if TYPE_CHECKING:
-    from collections.abc import Iterator
-
-    from wetterdienst.settings import Settings
-
-try:
-    from backports.datetime_fromisoformat import MonkeyPatch
-except ImportError:
-    pass
-else:
-    MonkeyPatch.patch_fromisoformat()
+import numpy as np
+import pandas as pd
+
+from wetterdienst.dwd.network import create_dwd_session
 
 log = logging.getLogger(__name__)
 
 
 class KMLReader:
-    """Read DWD XML Weather Forecast File of Type KML."""
+    def __init__(self, station_ids: List = None, parameters: List = None):
 
-    def __init__(self, station_ids: list[str], parameters: list[str], settings: Settings) -> None:
         self.station_ids = station_ids
         self.parameters = parameters
+
         self.metadata = {}
+        self.root = None
         self.timesteps = []
-        self.nsmap = None
-        self.iter_elems = None
+        self.items = []
 
-        self.dwdfs = NetworkFilesystemManager.get(settings=settings, ttl=CacheExpiry.FIVE_MINUTES)
+        self.dwd_session = create_dwd_session()
 
-    def download(self, url: str) -> BytesIO:
-        """Download kml file as bytes.
-        https://stackoverflow.com/questions/37573483/progress-bar-while-download-file-over-http-with-requests
+    def download(self, url: str):
+        # https://stackoverflow.com/questions/37573483/progress-bar-while-download-file-over-http-with-requests  # noqa:E501,B950
 
-        block_size: int or None
-                    Bytes to download in one request; use instance value if None. If
-                    zero, will return a streaming Requests file-like instance.
+        response = self.dwd_session.get(url, stream=True)
+        response.raise_for_status()
 
-        :param url: url string to kml file
-        :return: content as bytes
-        """
-
-        response = self.dwdfs.open(url, block_size=0)
-        total = self.dwdfs.size(url)
+        total = int(response.headers.get("content-length", 0))
 
         buffer = BytesIO()
-
-        tqdm_out = TqdmToLogger(log, level=logging.INFO)
-
         with tqdm(
             desc=url,
             total=total,
             unit="iB",
             unit_scale=True,
             unit_divisor=1024,
-            file=tqdm_out,
         ) as bar:
-            for data in read_in_chunks(response, chunk_size=1024):
+            for data in response.iter_content(chunk_size=1024):
                 size = buffer.write(data)
                 bar.update(size)
 
         return buffer
 
-    def fetch(self, url) -> bytes:
+    def fetch(self, url) -> str:
         """
-        Fetch weather mosmix file (zipped xml).
+        Fetch weather forecast file (zipped xml).
         """
         buffer = self.download(url)
-        zfs = ZipFileSystem(buffer, "r")
-        return zfs.open(zfs.glob("*")[0]).read()
+        kmz = ZipFile(buffer, "r")
+        kml = kmz.open(kmz.namelist()[0], "r").read()
+        return kml
 
     def read(self, url: str):
         """
         Download and read DWD XML Weather Forecast File of Type KML.
         """
 
-        log.info(f"Downloading KMZ file {Path(url).name}")
+        log.info(f"Downloading KMZ file {basename(url)}")
         kml = self.fetch(url)
 
         log.info("Parsing KML data")
-        self.iter_elems = iterparse(BytesIO(kml), events=("start", "end"), resolve_entities=False)
+        # TODO: Check if XML parsing performance can be improved by using libxml2.
+        tree = etree.parse(BytesIO(kml))  # noqa:S320
+        self.root = root = tree.getroot()
 
         prod_items = {
             "issuer": "Issuer",
             "product_id": "ProductID",
             "generating_process": "GeneratingProcess",
             "issue_time": "IssueTime",
         }
 
-        nsmap = None
-
         # Get Basic Metadata
-        prod_definition = None
-        prod_definition_tag = None
-        for event, element in self.iter_elems:
-            if event == "start":
-                # get namespaces from root element
-                if nsmap is None:
-                    nsmap = element.nsmap
-                    prod_definition_tag = f"{{{nsmap['dwd']}}}ProductDefinition"
-            elif event == "end":
-                if element.tag == prod_definition_tag:
-                    prod_definition = element
-                    # stop processing after head
-                    # leave forecast data for iteration
-                    break
+        prod_definition = root.findall(
+            "kml:Document/kml:ExtendedData/dwd:ProductDefinition", root.nsmap
+        )[0]
 
-        self.metadata = {k: prod_definition.find(f"{{{nsmap['dwd']}}}{v}").text for k, v in prod_items.items()}
-        self.metadata["issue_time"] = dt.datetime.fromisoformat(self.metadata["issue_time"])
+        self.metadata = {
+            k: prod_definition.find(f"{{{root.nsmap['dwd']}}}{v}").text
+            for k, v in prod_items.items()
+        }
+        self.metadata["issue_time"] = pd.Timestamp(self.metadata["issue_time"])
 
         # Get time steps.
-        timesteps = prod_definition.findall(
-            "dwd:ForecastTimeSteps",
-            nsmap,
+        timesteps = root.findall(
+            "kml:Document/kml:ExtendedData/dwd:ProductDefinition/dwd:ForecastTimeSteps",
+            root.nsmap,
         )[0]
-        self.timesteps = [dt.datetime.fromisoformat(i.text) for i in timesteps.getchildren()]
+        self.timesteps = DatetimeIndex(
+            [pd.Timestamp(i.text) for i in timesteps.getchildren()]
+        )
 
-        # save namespace map for later iteration
-        self.nsmap = nsmap
+        # Find all kml:Placemark items.
+        self.items += root.findall("kml:Document/kml:Placemark", root.nsmap)
 
     def iter_items(self):
-        clear = True
-        placemark_tag = f"{{{self.nsmap['kml']}}}Placemark"
-        for event, element in self.iter_elems:
-            if event == "start":
-                if element.tag == placemark_tag:
-                    clear = False
-            elif event == "end":
-                if element.tag == placemark_tag:
-                    station_id = element.find("kml:name", self.nsmap).text
-                    if (self.station_ids is None) or station_id in self.station_ids:
-                        yield element
-                    clear = True
-                if clear:
-                    element.clear()
+        for item in self.items:
+            station_id = item.find("kml:name", self.root.nsmap).text
+
+            if (self.station_ids is None) or station_id in self.station_ids:
+                yield item
 
     def get_metadata(self):
-        """Get metadata as DataFrame."""
-        return pl.DataFrame([self.metadata])
+        return pd.DataFrame([self.metadata])
 
-    def get_forecasts(self) -> Iterator[pl.DataFrame]:
-        """Get forecasts as DataFrame."""
+    def get_stations(self):
+        stations = []
         for station_forecast in self.iter_items():
-            station_ids = station_forecast.find("kml:name", self.nsmap).text
+            station = {
+                "station_id": station_forecast.find("kml:name", self.root.nsmap).text,
+                "station_name": station_forecast.find(
+                    "kml:description", self.root.nsmap
+                ).text,
+            }
+
+            coordinates = station_forecast.find(
+                "kml:Point/kml:coordinates", self.root.nsmap
+            ).text.split(",")
+
+            station["longitude"] = float(coordinates[0])
+            station["latitude"] = float(coordinates[1])
+            station["height"] = float(coordinates[2])
 
-            measurement_list = station_forecast.findall("kml:ExtendedData/dwd:Forecast", self.nsmap)
+            stations.append(station)
 
-            data_dict = {"station_id": station_ids, "datetime": self.timesteps}
+        return pd.DataFrame(stations)
+
+    def get_forecasts(self):
+        df_list = []
+        for station_forecast in self.iter_items():
+            station_ids = station_forecast.find("kml:name", self.root.nsmap).text
+
+            measurement_list = station_forecast.findall(
+                "kml:ExtendedData/dwd:Forecast", self.root.nsmap
+            )
+            df = pd.DataFrame({"station_id": station_ids, "datetime": self.timesteps})
 
             for measurement_item in measurement_list:
-                measurement_parameter = measurement_item.get(f"{{{self.nsmap['dwd']}}}elementName")
-                if measurement_parameter.lower() in self.parameters:
+
+                measurement_parameter = measurement_item.get(
+                    f"{{{self.root.nsmap['dwd']}}}elementName"
+                )
+
+                if self.parameters is None or measurement_parameter in self.parameters:
                     measurement_string = measurement_item.getchildren()[0].text
+
                     measurement_values = " ".join(measurement_string.split()).split(" ")
-                    measurement_values = [None if i == "-" else float(i) for i in measurement_values]
+                    measurement_values = [
+                        np.nan if i == "-" else float(i) for i in measurement_values
+                    ]
+
                     assert len(measurement_values) == len(  # noqa:S101
-                        self.timesteps,
-                    ), "Number of time steps does not match number of measurement values"
-                    data_dict[measurement_parameter.lower()] = measurement_values
+                        self.timesteps
+                    ), "Number of timesteps does not match number of measurement values"
+
+                    df[measurement_parameter] = measurement_values
+
+                df_list.append(df)
+
+        df = pd.concat(df_list, axis=0)
 
-            station_forecast.clear()
-            yield pl.DataFrame(data_dict)
+        return df
```

### Comparing `wetterdienst-0.82.0/wetterdienst/provider/dwd/observation/metaindex.py` & `wetterdienst-0.9.0/wetterdienst/dwd/observations/metaindex.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,279 +1,290 @@
-# Copyright (C) 2018-2021, earthobservations developers.
-# Distributed under the MIT License. See LICENSE for more info.
-from __future__ import annotations
-
-import datetime as dt
-import logging
 import re
+import zipfile
+from functools import reduce
+from io import BytesIO
+from typing import Tuple, List
 from concurrent.futures import ThreadPoolExecutor
-from io import BytesIO, StringIO
-from typing import TYPE_CHECKING
+import datetime as dt
+from urllib.parse import urljoin
 
-import polars as pl
-from fsspec.implementations.zip import ZipFileSystem
+import pandas as pd
+from requests.exceptions import InvalidURL
 
-from wetterdienst.exceptions import MetaFileNotFoundError
-from wetterdienst.metadata.columns import Columns
-from wetterdienst.metadata.period import Period
-from wetterdienst.metadata.resolution import Resolution
-from wetterdienst.provider.dwd.observation.fileindex import build_path_to_parameter
-from wetterdienst.provider.dwd.observation.metadata.dataset import (
-    DWD_URBAN_DATASETS,
-    DwdObservationDataset,
+from wetterdienst.util.cache import metaindex_cache
+from wetterdienst.dwd.metadata.constants import (
+    DWDCDCBase,
+    DWD_SERVER,
+    DWD_CDC_PATH,
+    STATION_ID_REGEX,
+    NA_STRING,
+    STATION_DATA_SEP,
+)
+from wetterdienst.dwd.metadata.column_map import (
+    GERMAN_TO_ENGLISH_COLUMNS_MAPPING,
+    METADATA_DTYPE_MAPPING,
 )
-from wetterdienst.util.cache import CacheExpiry
-from wetterdienst.util.network import download_file, list_remote_files_fsspec
-from wetterdienst.util.polars_util import read_fwf_from_df
-
-if TYPE_CHECKING:
-    from wetterdienst.settings import Settings
-
-log = logging.getLogger(__name__)
-
-DWD_COLUMN_NAMES_MAPPING = {
-    "column_0": Columns.STATION_ID.value,
-    "column_1": Columns.START_DATE.value,
-    "column_2": Columns.END_DATE.value,
-    "column_3": Columns.HEIGHT.value,
-    "column_4": Columns.LATITUDE.value,
-    "column_5": Columns.LONGITUDE.value,
-    "column_6": Columns.NAME.value,
-    "column_7": Columns.STATE.value,
-}
+from wetterdienst.dwd.network import download_file_from_dwd
+from wetterdienst.dwd.index import build_path_to_parameter
+from wetterdienst.dwd.metadata.column_names import DWDMetaColumns
+from wetterdienst.dwd.metadata.parameter import Parameter
+from wetterdienst.dwd.metadata.period_type import PeriodType
+from wetterdienst import TimeResolution
+from wetterdienst.exceptions import MetaFileNotFound
+from wetterdienst.util.network import list_remote_files
 
 METADATA_COLUMNS = [
-    Columns.STATION_ID.value,
-    Columns.START_DATE.value,
-    Columns.END_DATE.value,
-    Columns.HEIGHT.value,
-    Columns.LATITUDE.value,
-    Columns.LONGITUDE.value,
-    Columns.NAME.value,
-    Columns.STATE.value,
+    DWDMetaColumns.STATION_ID.value,
+    DWDMetaColumns.FROM_DATE.value,
+    DWDMetaColumns.TO_DATE.value,
+    DWDMetaColumns.STATION_HEIGHT.value,
+    DWDMetaColumns.LATITUDE.value,
+    DWDMetaColumns.LONGITUDE.value,
+    DWDMetaColumns.STATION_NAME.value,
+    DWDMetaColumns.STATE.value,
 ]
 
-STATION_ID_REGEX = r"(?<!\d)\d{5}(?!\d)"
+META_FILE_IDENTIFIERS = ["beschreibung", "txt"]
+
+METADATA_1MIN_GEO_PREFIX = "Metadaten_Geographie_"
+
+META_DATA_FOLDER = "meta_data/"
+
+METADATA_FIXED_COLUMN_WIDTH = [
+    (0, 5),
+    (5, 14),
+    (14, 23),
+    (23, 38),
+    (38, 50),
+    (50, 60),
+    (60, 102),
+    (102, 200),
+]
 
 
+@metaindex_cache.cache_on_arguments()
 def create_meta_index_for_climate_observations(
-    dataset: DwdObservationDataset,
-    resolution: Resolution,
-    period: Period,
-    settings: Settings,
-) -> pl.LazyFrame:
+    parameter: Parameter, time_resolution: TimeResolution, period_type: PeriodType
+) -> pd.DataFrame:
     """
     Wrapper function that either calls the regular meta index function for general
     parameters or the special function for 1minute precipitation historical where meta
     index is created in a more complex way.
 
     Args:
-        dataset: observation measure
-        resolution: frequency/granularity of measurement interval
-        period: current, recent or historical files
+        parameter: observation measure
+        time_resolution: frequency/granularity of measurement interval
+        period_type: current, recent or historical files
 
     Returns:
         pandas.DataFrame with meta index for the selected set of arguments
     """
-    cond1 = (
-        resolution == Resolution.MINUTE_1
-        and period == Period.HISTORICAL
-        and dataset == DwdObservationDataset.PRECIPITATION
+    cond = (
+        time_resolution == TimeResolution.MINUTE_1
+        and period_type == PeriodType.HISTORICAL
+        and parameter == Parameter.PRECIPITATION
     )
 
-    cond2 = resolution == Resolution.SUBDAILY and dataset == DwdObservationDataset.WIND_EXTREME
-    cond3 = dataset in DWD_URBAN_DATASETS
-    if cond1:
-        meta_index = _create_meta_index_for_1minute_historical_precipitation(settings)
-    elif cond2:
-        meta_index = _create_meta_index_for_subdaily_extreme_wind(period, settings)
-    elif cond3:
-        meta_index = _create_meta_index_for_climate_observations(dataset, resolution, Period.RECENT, settings)
+    if cond:
+        meta_index = _create_meta_index_for_1minute_historical_precipitation()
     else:
-        meta_index = _create_meta_index_for_climate_observations(dataset, resolution, period, settings)
+        meta_index = _create_meta_index_for_climate_observations(
+            parameter, time_resolution, period_type
+        )
 
     # If no state column available, take state information from daily historical
     # precipitation
-    if cond1:
+    if DWDMetaColumns.STATE.value not in meta_index:
         mdp = _create_meta_index_for_climate_observations(
-            DwdObservationDataset.PRECIPITATION_MORE,
-            Resolution.DAILY,
-            Period.HISTORICAL,
-            settings=settings,
+            Parameter.PRECIPITATION_MORE, TimeResolution.DAILY, PeriodType.HISTORICAL
         )
 
-        meta_index = meta_index.join(
-            other=mdp.select([Columns.STATION_ID.value, Columns.STATE.value]),
-            on=[Columns.STATION_ID.value],
+        meta_index = pd.merge(
+            left=meta_index,
+            right=mdp.loc[
+                :, [DWDMetaColumns.STATION_ID.value, DWDMetaColumns.STATE.value]
+            ],
             how="left",
         )
 
-    meta_index = meta_index.with_columns(
-        pl.col(Columns.START_DATE.value).str.to_datetime("%Y%m%d"),
-        pl.col(Columns.END_DATE.value).str.to_datetime("%Y%m%d"),
-        pl.col(Columns.HEIGHT.value).cast(pl.Float64),
-        pl.col(Columns.LATITUDE.value).cast(pl.Float64),
-        pl.col(Columns.LONGITUDE.value).cast(pl.Float64),
+    meta_index[DWDMetaColumns.FROM_DATE.value] = pd.to_datetime(
+        meta_index[DWDMetaColumns.FROM_DATE.value], format="%Y%m%d"
+    )
+
+    meta_index[DWDMetaColumns.TO_DATE.value] = pd.to_datetime(
+        meta_index[DWDMetaColumns.TO_DATE.value], format="%Y%m%d"
     )
 
-    return meta_index.sort(by=[pl.col(Columns.STATION_ID.value)])
+    return meta_index.sort_values(DWDMetaColumns.STATION_ID.value).reset_index(
+        drop=True
+    )
 
 
 def _create_meta_index_for_climate_observations(
-    dataset: DwdObservationDataset,
-    resolution: Resolution,
-    period: Period,
-    settings: Settings,
-) -> pl.LazyFrame:
+    parameter: Parameter, time_resolution: TimeResolution, period_type: PeriodType
+) -> pd.DataFrame:
     """Function used to create meta index DataFrame parsed from the text files that are
     located in each data section of the station data directory of the weather service.
 
     Args:
-        dataset: observation measure
-        resolution: frequency/granularity of measurement interval
-        period: current, recent or historical files
+        parameter: observation measure
+        time_resolution: frequency/granularity of measurement interval
+        period_type: current, recent or historical files
     Return:
         DataFrame with parsed columns of the corresponding text file. Columns are
         translated into English and data is not yet complete as file existence is
         not checked.
 
     """
-    parameter_path = build_path_to_parameter(dataset, resolution, period)
-    if dataset in DWD_URBAN_DATASETS:
-        dwd_cdc_base = "observations_germany/climate_urban/"
-    else:
-        dwd_cdc_base = "observations_germany/climate/"
-    url = f"https://opendata.dwd.de/climate_environment/CDC/{dwd_cdc_base}/{parameter_path}"
-    remote_files = list_remote_files_fsspec(url, settings=settings, ttl=CacheExpiry.METAINDEX)
-    # TODO: remove workaround once station list at https://opendata.dwd.de/climate_environment/CDC/observations_germany/climate/5_minutes/precipitation/historical/2022/ is removed  # noqa: E501
-    if (
-        period == Period.HISTORICAL
-        and resolution == Resolution.MINUTE_5
-        and dataset == DwdObservationDataset.PRECIPITATION
-    ):
-        remote_files = [file for file in remote_files if file.split("/")[-2] != "2022"]
+    parameter_path = build_path_to_parameter(parameter, time_resolution, period_type)
+
+    url = reduce(
+        urljoin,
+        [
+            DWD_SERVER,
+            DWD_CDC_PATH,
+            DWDCDCBase.CLIMATE_OBSERVATIONS.value,
+            parameter_path,
+        ],
+    )
+
+    files_server = list_remote_files(url, recursive=True)
+
     # Find the one meta file from the files listed on the server
-    meta_file = _find_meta_file(remote_files, url, ["beschreibung", "txt"])
-    log.info(f"Downloading file {meta_file}.")
-    payload = download_file(meta_file, settings=settings, ttl=CacheExpiry.METAINDEX)
-    return _read_meta_df(payload)
+    meta_file = _find_meta_file(files_server, url)
+
+    try:
+        file = download_file_from_dwd(meta_file)
+    except InvalidURL as e:
+        raise InvalidURL(f"Error: reading metadata {meta_file} file failed.") from e
+
+    meta_index = pd.read_fwf(
+        filepath_or_buffer=file,
+        colspecs=METADATA_FIXED_COLUMN_WIDTH,
+        skiprows=[1],
+        dtype=str,
+        encoding="ISO-8859-1",
+    )
+
+    # Fix column names, as header is not aligned to fixed column widths
+    meta_index.columns = "".join(
+        [column for column in meta_index.columns if "unnamed" not in column.lower()]
+    ).split(" ")
+
+    meta_index = meta_index.rename(columns=str.upper)
+
+    meta_index = meta_index.rename(columns=GERMAN_TO_ENGLISH_COLUMNS_MAPPING)
 
+    return meta_index.astype(METADATA_DTYPE_MAPPING)
 
-def _find_meta_file(files: list[str], url: str, strings: list[str]) -> str:
+
+def _find_meta_file(files: List[str], url: str) -> str:
     """
     Function used to find meta file based on predefined strings that are usually found
     in those files
     Args:
         files: list of files found on server path
         url: the path that was searched for a meta file
 
     Returns:
         the matching file
     Raises:
-        MetaFileNotFoundError - for the case no file was found
+        MetaFileNotFound - for the case no file was found
     """
     for file in files:
         file_strings = file.split("/")[-1].lower().replace(".", "_").split("_")
-        if set(file_strings).issuperset(strings):
+        if set(file_strings).issuperset(META_FILE_IDENTIFIERS):
             return file
-    else:
-        raise MetaFileNotFoundError(f"No meta file was found amongst the files at {url}.")
-
-
-def _read_meta_df(file: BytesIO) -> pl.LazyFrame:
-    """Read metadata into DataFrame
-    :param file: metadata file loaded in bytes
-    :return: DataFrame with Stations
-    """
-    lines = file.readlines()[2:]
-    first = lines[0].decode("latin-1")
-    if first.startswith("SP"):
-        # Skip first line if it contains a header
-        lines = lines[1:]
-    lines = [line.decode("latin-1") for line in lines]
-    df = pl.DataFrame(lines)
-    column_specs = (
-        (0, 4),
-        (21, 29),
-        (30, 38),
-        (40, 53),
-        (55, 65),
-        (67, 75),
-        (76, 156),
-        (157, 200),
-    )
-    df = read_fwf_from_df(df, column_specs)
-    return df.rename(mapping=lambda col: DWD_COLUMN_NAMES_MAPPING.get(col, col)).lazy()
-
 
-def _create_meta_index_for_subdaily_extreme_wind(period: Period, settings: Settings) -> pl.LazyFrame:
-    """Create metadata DataFrame for subdaily wind extreme
+    raise MetaFileNotFound(f"No meta file was found amongst the files at {url}.")
 
-    :param period: period for which metadata is acquired
-    :return: pandas.DataFrame with combined information for both 3hourly (fx3) and 6hourly (fx6) wind extremes
-    """
-    parameter_path = build_path_to_parameter(DwdObservationDataset.WIND_EXTREME, Resolution.SUBDAILY, period)
-    url = f"https://opendata.dwd.de/climate_environment/CDC/observations_germany/climate/{parameter_path}"
-    remote_files = list_remote_files_fsspec(url, settings=settings, ttl=CacheExpiry.METAINDEX)
-    # Find the one meta file from the files listed on the server
-    meta_file_fx3 = _find_meta_file(remote_files, url, ["fx3", "beschreibung", "txt"])
-    meta_file_fx6 = _find_meta_file(remote_files, url, ["fx6", "beschreibung", "txt"])
-    log.info(f"Downloading file {meta_file_fx3}.")
-    payload_fx3 = download_file(meta_file_fx3, settings=settings, ttl=CacheExpiry.METAINDEX)
-    log.info(f"Downloading file {meta_file_fx6}.")
-    payload_fx6 = download_file(meta_file_fx6, settings=settings, ttl=CacheExpiry.METAINDEX)
-    df_fx3 = _read_meta_df(payload_fx3)
-    df_fx6 = _read_meta_df(payload_fx6)
-    df_fx6 = df_fx6.join(df_fx3.select(Columns.STATION_ID.value), on=[Columns.STATION_ID.value], how="inner")
-    return pl.concat([df_fx3, df_fx6])
 
-
-def _create_meta_index_for_1minute_historical_precipitation(settings: Settings) -> pl.LazyFrame:
+def _create_meta_index_for_1minute_historical_precipitation() -> pd.DataFrame:
     """
-    A helping function to create a raw index of metadata for stations_result of the set of
+    A helping function to create a raw index of metadata for stations of the set of
     parameters as given. This raw metadata is then used by other functions. This
     second/alternative function must be used for high resolution data, where the
     metadata is not available as file but instead saved in external files per each
     station.
     - especially for precipitation/1_minute/historical!
 
     """
-    parameter_path = f"{Resolution.MINUTE_1.value}/" f"{DwdObservationDataset.PRECIPITATION.value}/"
-    url = f"https://opendata.dwd.de/climate_environment/CDC/observations_germany/climate/{parameter_path}/meta_data/"
-    metadata_file_paths = list_remote_files_fsspec(url, settings=settings, ttl=CacheExpiry.METAINDEX)
-    station_ids = [re.findall(STATION_ID_REGEX, file).pop(0) for file in metadata_file_paths]
 
-    log.info(f"Downloading {len(metadata_file_paths)} files for 1minute precipitation historical metadata.")
+    parameter_path = f"{TimeResolution.MINUTE_1.value}/{Parameter.PRECIPITATION.value}/"
+
+    url = reduce(
+        urljoin,
+        [
+            DWD_SERVER,
+            DWD_CDC_PATH,
+            DWDCDCBase.CLIMATE_OBSERVATIONS.value,
+            parameter_path,
+            META_DATA_FOLDER,
+        ],
+    )
+
+    metadata_file_paths = list_remote_files(url, recursive=False)
+
+    station_ids = [
+        re.findall(STATION_ID_REGEX, file).pop(0) for file in metadata_file_paths
+    ]
+
+    meta_index_df = pd.DataFrame(columns=METADATA_COLUMNS)
+
     with ThreadPoolExecutor() as executor:
         metadata_files = executor.map(
-            lambda file: download_file(url=file, settings=settings, ttl=CacheExpiry.NO_CACHE),
-            metadata_file_paths,
+            _download_metadata_file_for_1minute_precipitation, metadata_file_paths
         )
 
-    metadata_dfs = [_parse_geo_metadata((file, station_id)) for file, station_id in zip(metadata_files, station_ids)]
+    with ThreadPoolExecutor() as executor:
+        metadata_dfs = executor.map(
+            _parse_geo_metadata, zip(metadata_files, station_ids)
+        )
 
-    meta_index_df = pl.concat(list(metadata_dfs))
+    meta_index_df = meta_index_df.append(other=list(metadata_dfs), ignore_index=True)
 
-    meta_index_df = meta_index_df.with_columns(
-        pl.when(pl.col(Columns.END_DATE.value).str.strip_chars().eq(""))
-        .then(pl.lit((dt.date.today() - dt.timedelta(days=1)).strftime("%Y%m%d")))
-        .otherwise(pl.col(Columns.END_DATE.value))
-        .alias(Columns.END_DATE.value),
-    )
+    missing_to_date_index = pd.isnull(meta_index_df[DWDMetaColumns.TO_DATE.value])
+
+    meta_index_df.loc[
+        missing_to_date_index, DWDMetaColumns.TO_DATE.value
+    ] = pd.Timestamp(dt.date.today() - dt.timedelta(days=1)).strftime("%Y%m%d")
+
+    meta_index_df = meta_index_df.astype(METADATA_DTYPE_MAPPING)
 
     # Drop empty state column again as it will be merged later on
-    meta_index_df = meta_index_df.select(pl.exclude(Columns.STATE.value))
+    meta_index_df = meta_index_df.drop(labels=DWDMetaColumns.STATE.value, axis=1)
+
+    return meta_index_df
 
-    meta_index_df = meta_index_df.with_columns(pl.all().str.strip_chars())
 
-    # Make station id str
-    return meta_index_df.with_columns(pl.col(Columns.STATION_ID.value).cast(str).str.pad_start(5, "0"))
+def _download_metadata_file_for_1minute_precipitation(metadata_file: str) -> BytesIO:
+    """A function that simply opens a filepath with help of the urllib library and then
+    writes the content to a BytesIO object and returns this object. For this case as it
+    opens lots of requests (there are approx 1000 different files to open for
+    1minute data), it will do the same at most three times for one file to assure
+    success reading the file.
+
+    Args:
+        metadata_file (str) - the file that shall be downloaded and returned as bytes.
+
+    Return:
+        A BytesIO object to which the opened file was written beforehand.
+
+    """
+    try:
+        file = download_file_from_dwd(metadata_file)
+    except InvalidURL as e:
+        raise InvalidURL(f"Reading metadata {metadata_file} file failed.") from e
+
+    return file
 
 
-def _parse_geo_metadata(metadata_file_and_station_id: tuple[BytesIO, str]) -> pl.LazyFrame:
+def _parse_geo_metadata(
+    metadata_file_and_station_id: Tuple[BytesIO, str]
+) -> pd.DataFrame:
     """A function that analysis the given file (bytes) and extracts geography of
     1minute metadata zip and catches the relevant information and create a similar file
     to those that can usually be found already prepared for other
     parameter combinations.
 
     Args:
         metadata_file_and_station_id (BytesIO, str) - the file that holds the
@@ -281,54 +292,67 @@
 
     Return:
         A pandas DataFrame with the combined data for one respective station.
 
     """
     metadata_file, station_id = metadata_file_and_station_id
 
-    zfs = ZipFileSystem(metadata_file, mode="r")
+    metadata_geo_filename = f"{METADATA_1MIN_GEO_PREFIX}{station_id}.txt"
 
-    file = zfs.open(f"Metadaten_Geographie_{station_id}.txt").read()
+    with zipfile.ZipFile(metadata_file, mode="r") as zip_file:
+        metadata_geo_bytes = BytesIO(zip_file.read(metadata_geo_filename))
 
-    df = _parse_zipped_data_into_df(file)
+    metadata_geo_df = _parse_zipped_data_into_df(metadata_geo_bytes)
 
-    df = df.rename(
-        mapping={
-            "Stations_id": Columns.STATION_ID.value,
-            "Stationshoehe": Columns.HEIGHT.value,
-            "Geogr.Breite": Columns.LATITUDE.value,
-            "Geogr.Laenge": Columns.LONGITUDE.value,
-            "von_datum": Columns.START_DATE.value,
-            "bis_datum": Columns.END_DATE.value,
-            "Stationsname": Columns.NAME.value,
-        },
-    )
+    metadata_geo_df = metadata_geo_df.rename(columns=str.upper)
+
+    metadata_geo_df = metadata_geo_df.rename(columns=GERMAN_TO_ENGLISH_COLUMNS_MAPPING)
 
-    df = df.with_columns(pl.col(Columns.START_DATE.value).first().cast(str), pl.col(Columns.END_DATE.value).cast(str))
+    metadata_geo_df[DWDMetaColumns.FROM_DATE.value] = metadata_geo_df.loc[
+        0, DWDMetaColumns.FROM_DATE.value
+    ]
 
-    df = df.last()
+    metadata_geo_df = metadata_geo_df.iloc[[-1], :]
 
-    return df.select([col for col in METADATA_COLUMNS if col != Columns.STATE.value])
+    return metadata_geo_df.reindex(columns=METADATA_COLUMNS)
 
 
-def _parse_zipped_data_into_df(file: bytes) -> pl.LazyFrame:
+def _parse_zipped_data_into_df(file: BytesIO) -> pd.DataFrame:
     """A wrapper for read_csv of pandas library that has set the typically used
     parameters in the found data of the
     german weather service.
 
     Args:
         file - the file that will be read
 
     Return:
         A pandas DataFrame with the read data.
 
     """
     try:
-        file_decoded = file.decode("utf-8")
+        # First try utf-8
+        file = pd.read_csv(
+            filepath_or_buffer=file,
+            sep=STATION_DATA_SEP,
+            na_values=NA_STRING,
+            dtype=str,
+            skipinitialspace=True,
+            encoding="utf-8",
+        )
     except UnicodeDecodeError:
-        file_decoded = file.decode("ISO-8859-1")
+        file.seek(0)
+
+        file = pd.read_csv(
+            filepath_or_buffer=file,
+            sep=STATION_DATA_SEP,
+            na_values=NA_STRING,
+            dtype=str,
+            skipinitialspace=True,
+            encoding="ISO-8859-1",
+        )
+
+    return file
+
 
-    return pl.read_csv(
-        source=StringIO(file_decoded),
-        separator=";",
-        null_values=["-999"],
-    ).lazy()
+def reset_meta_index_cache() -> None:
+    """ Function to reset cache of meta index """
+    metaindex_cache.invalidate()
```

### Comparing `wetterdienst-0.82.0/wetterdienst/provider/dwd/radar/cli.py` & `wetterdienst-0.9.0/wetterdienst/dwd/radar/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,8 @@
-# Copyright (C) 2018-2021, earthobservations developers.
-# Distributed under the MIT License. See LICENSE for more info.
 import sys
-from pathlib import Path
-
 import h5py
 
 
 def hdf5dump(thing, compact=False):
     """
     Like "h5dump -n 1", but better.
     """
@@ -20,27 +16,28 @@
         "startazT",
         "startelA",
         "stopazA",
         "stopazT",
         "stopelA",
     ]
 
-    def dumpattrs(item, indent=2):
-        for name, value in item.attrs.items():
-            if compact:
-                if name in blocklist:
-                    continue
-            print(" " * indent, "-", name, value)  # noqa: T201
-
-    with Path(thing).open("rb") as buffer:
+    with open(thing, "rb") as buffer:
         hdf = h5py.File(buffer, "r")
+
+        def dumpattrs(item, indent=2):
+            for name, value in item.attrs.items():
+                if compact:
+                    if name in blocklist:
+                        continue
+                print(" " * indent, "-", name, value)
+
         for group in hdf.keys():
-            print("name:", hdf[group].name)  # noqa: T201
+            print("name:", hdf[group].name)
             dumpattrs(hdf[group])
             for subgroup in hdf[group].keys():
-                print("  name:", subgroup)  # noqa: T201
+                print("  name:", subgroup)
                 dumpattrs(hdf[group][subgroup], indent=4)
 
 
 def wddump():
     filename = sys.argv[1]
     hdf5dump(filename, compact=True)
```

### Comparing `wetterdienst-0.82.0/wetterdienst/provider/dwd/radar/index.py` & `wetterdienst-0.9.0/wetterdienst/dwd/radar/index.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,32 @@
-# Copyright (C) 2018-2021, earthobservations developers.
-# Distributed under the MIT License. See LICENSE for more info.
-from __future__ import annotations
-
 import os
-from typing import TYPE_CHECKING
+from typing import Optional
+from urllib.parse import urljoin
 
-import polars as pl
+import pandas as pd
+from dateparser import parse
 
-from wetterdienst.metadata.extension import Extension
-from wetterdienst.metadata.period import Period
-from wetterdienst.metadata.resolution import Resolution
-from wetterdienst.provider.dwd.metadata.datetime import DatetimeFormat
-from wetterdienst.provider.dwd.radar.metadata import (
+from wetterdienst import TimeResolution, PeriodType
+from wetterdienst.dwd.metadata.constants import ArchiveFormat, DWD_SERVER, DWD_CDC_PATH
+from wetterdienst.dwd.metadata.column_names import DWDMetaColumns
+from wetterdienst.dwd.metadata.datetime import DatetimeFormat
+from wetterdienst.dwd.radar.sites import RadarSite
+from wetterdienst.dwd.radar.metadata import (
+    RadarParameter,
+    RadarDataFormat,
     RADAR_PARAMETERS_COMPOSITES,
-    RADAR_PARAMETERS_RADOLAN,
-    RADAR_PARAMETERS_RADVOR,
     RADAR_PARAMETERS_SITES,
     RADAR_PARAMETERS_SWEEPS,
-    DwdRadarDataFormat,
-    DwdRadarDataSubset,
-    DwdRadarParameter,
-)
-from wetterdienst.provider.dwd.radar.util import (
-    RADAR_DT_PATTERN,
-    RADOLAN_DT_PATTERN,
-    get_date_from_filename,
+    RADAR_PARAMETERS_RADOLAN,
+    RadarDataSubset,
+    RADAR_PARAMETERS_RADVOR,
 )
-from wetterdienst.util.cache import CacheExpiry
-from wetterdienst.util.network import list_remote_files_fsspec
-
-if TYPE_CHECKING:
-    from wetterdienst.provider.dwd.radar.sites import DwdRadarSite
-    from wetterdienst.settings import Settings
+from wetterdienst.dwd.radar.util import get_date_from_filename, RADOLAN_DT_PATTERN
+from wetterdienst.util.cache import fileindex_cache_five_minutes
+from wetterdienst.util.network import list_remote_files
 
 
 def use_cache() -> int:  # pragma: no cover
     """
     Only use caching when running the test suite to reduce its duration.
     In production, this won't always give us fresh enough data, especially
     when using the "MOST_RECENT" request option. So, let's skip it for that
@@ -47,217 +38,214 @@
     """
     if "PYTEST_CURRENT_TEST" in os.environ and "CI" not in os.environ:
         return 2 * 60
     else:
         return 0
 
 
+@fileindex_cache_five_minutes.cache_on_arguments(expiration_time=use_cache)
 def create_fileindex_radar(
-    parameter: DwdRadarParameter,
-    settings: Settings,
-    site: DwdRadarSite | None = None,
-    fmt: DwdRadarDataFormat | None = None,
-    subset: DwdRadarDataSubset | None = None,
-    resolution: Resolution | None = None,
-    period: Period | None = None,
+    parameter: RadarParameter,
+    site: Optional[RadarSite] = None,
+    format: Optional[RadarDataFormat] = None,
+    subset: Optional[RadarDataSubset] = None,
+    time_resolution: Optional[TimeResolution] = None,
+    period_type: Optional[PeriodType] = None,
     parse_datetime: bool = False,
-) -> pl.DataFrame:
+) -> pd.DataFrame:
     """
     Function to create a file index of the DWD radar data, which is shipped as
     bin bufr or odim-hdf5 data. The file index is created for a single parameter.
 
     :param parameter:       The radar moment to request
-    :param settings:
     :param site:            Site/station if parameter is one of
                             RADAR_PARAMETERS_SITES
-    :param fmt:          Data format (BINARY, BUFR, HDF5)
+    :param format:          Data format (BINARY, BUFR, HDF5)
     :param subset:          The subset (simple or polarimetric) for HDF5 data.
-    :param resolution: Time resolution for RadarParameter.RADOLAN_CDC,
+    :param time_resolution: Time resolution for RadarParameter.RADOLAN_CDC,
                             either daily or hourly or 5 minutes.
-    :param period:     Period type for RadarParameter.RADOLAN_CDC
+    :param period_type:     Period type for RadarParameter.RADOLAN_CDC
     :param parse_datetime:  Whether to parse datetimes from file names
 
     :return:                File index as pandas.DataFrame with FILENAME
                             and DATETIME columns
     """
+
     parameter_path = build_path_to_parameter(
         parameter=parameter,
         site=site,
-        fmt=fmt,
+        format=format,
         subset=subset,
-        resolution=resolution,
-        period=period,
+        time_resolution=time_resolution,
+        period_type=period_type,
+    )
+
+    url = urljoin(DWD_SERVER, parameter_path)
+
+    files_server = list_remote_files(url, recursive=True)
+
+    files_server = pd.DataFrame(
+        files_server, columns=[DWDMetaColumns.FILENAME.value], dtype="str"
     )
-    url = f"https://opendata.dwd.de/{parameter_path}"
-    files_serv = list_remote_files_fsspec(url, settings=settings, ttl=CacheExpiry.NO_CACHE)
-    df_fileindex = pl.DataFrame(files_serv, schema={"filename": pl.Utf8})
 
     # Some directories have both "---bin" and "---bufr" files within the same directory,
     # so we need to filter here by designated RadarDataFormat. Example:
     # https://opendata.dwd.de/weather/radar/sites/px/boo/
-    if fmt is not None:
-        if fmt == DwdRadarDataFormat.BINARY:
-            df_fileindex = df_fileindex.filter(pl.col("filename").str.contains("--bin", literal=True))
-        elif fmt == DwdRadarDataFormat.BUFR:
-            df_fileindex = df_fileindex.filter(pl.col("filename").str.contains("--buf", literal=True))
-
-    # Drop duplicates of files packed as .bz2, if not all files are .bz2
-    if not df_fileindex.get_column("filename").str.ends_with(".bz2").all():
-        df_fileindex = df_fileindex.filter(~pl.col("filename").str.ends_with(".bz2"))
-
-    if parameter in RADAR_PARAMETERS_SWEEPS:
-        formats = [DatetimeFormat.YMDHM.value]
-    elif site and parameter is DwdRadarParameter.PX250_REFLECTIVITY:
-        formats = [DatetimeFormat.YMDHM.value]
-    elif site and fmt is DwdRadarDataFormat.BUFR:
-        formats = [DatetimeFormat.YMDHM.value]
-    else:
-        formats = [DatetimeFormat.ymdhm.value]
+    if format is not None:
+        if format == RadarDataFormat.BINARY:
+            files_server = files_server[
+                files_server[DWDMetaColumns.FILENAME.value].str.contains("--bin")
+            ]
+        elif format == RadarDataFormat.BUFR:
+            files_server = files_server[
+                files_server[DWDMetaColumns.FILENAME.value].str.contains("--buf")
+            ]
 
     # Decode datetime of file for filtering.
     if parse_datetime:
-        df_fileindex = df_fileindex.with_columns(
-            pl.col("filename")
-            .map_elements(
-                lambda fn: get_date_from_filename(filename=fn, pattern=RADAR_DT_PATTERN, formats=formats),
-            )
-            .alias("datetime"),
-        )
 
-    return df_fileindex.drop_nulls()
+        files_server[DWDMetaColumns.DATETIME.value] = files_server[
+            DWDMetaColumns.FILENAME.value
+        ].apply(get_date_from_filename)
+
+        files_server = files_server.dropna()
+
+    return files_server
 
 
-def create_fileindex_radolan_cdc(resolution: Resolution, period: Period, settings: Settings) -> pl.DataFrame:
+@fileindex_cache_five_minutes.cache_on_arguments()
+def create_fileindex_radolan_cdc(
+    time_resolution: TimeResolution, period_type: PeriodType
+) -> pd.DataFrame:
     """
     Function used to create a file index for the RADOLAN_CDC product. The file index
     will include both recent as well as historical files. A datetime column is created
     from the filenames which contain some datetime formats. This datetime column is
     required for later filtering for the requested file.
 
-    :param resolution: Time resolution for RadarParameter.RADOLAN_CDC,
+    :param time_resolution: Time resolution for RadarParameter.RADOLAN_CDC,
                             either daily or hourly or 5 minutes.
-    :param period:     Period type for RadarParameter.RADOLAN_CDC
+    :param period_type:     Period type for RadarParameter.RADOLAN_CDC
 
     :return:                File index as DataFrame
     """
-    df_fileindex = create_fileindex_radar(
-        parameter=DwdRadarParameter.RADOLAN_CDC,
-        resolution=resolution,
-        period=period,
-        settings=settings,
+    file_index = create_fileindex_radar(
+        parameter=RadarParameter.RADOLAN_CDC,
+        time_resolution=time_resolution,
+        period_type=period_type,
     )
 
-    df_fileindex = df_fileindex.filter(
-        pl.col("filename").str.contains("/bin/", literal=True)
-        & (
-            pl.col("filename").str.ends_with(Extension.GZ.value) | pl.col("filename").str.ends_with(Extension.TAR.value)
-        ),
-    )
-
-    if period == Period.HISTORICAL:
-        formats = [DatetimeFormat.YM.value]
-    else:
-        formats = [DatetimeFormat.ymdhm.value]
+    file_index = file_index[
+        file_index[DWDMetaColumns.FILENAME.value].str.contains("/bin/")
+        & file_index[DWDMetaColumns.FILENAME.value].str.endswith(
+            (ArchiveFormat.GZ.value, ArchiveFormat.TAR_GZ.value)
+        )
+    ]
 
-    df_fileindex = df_fileindex.with_columns(
-        pl.col("filename")
-        .map_elements(
-            lambda fn: get_date_from_filename(filename=fn, pattern=RADOLAN_DT_PATTERN, formats=formats),
+    # Decode datetime of file for filtering.
+    file_index[DWDMetaColumns.DATETIME.value] = file_index[
+        DWDMetaColumns.FILENAME.value
+    ].apply(
+        lambda filename: parse(
+            RADOLAN_DT_PATTERN.findall(filename)[0],
+            date_formats=[DatetimeFormat.YM.value, DatetimeFormat.ymdhm.value],
         )
-        .alias("datetime"),
     )
 
-    return df_fileindex.drop_nulls()
+    return file_index
 
 
 def build_path_to_parameter(
-    parameter: DwdRadarParameter,
-    site: DwdRadarSite | None = None,
-    fmt: DwdRadarDataFormat | None = None,
-    subset: DwdRadarDataSubset | None = None,
-    resolution: Resolution | None = None,
-    period: Period | None = None,
+    parameter: RadarParameter,
+    site: Optional[RadarSite] = None,
+    format: Optional[RadarDataFormat] = None,
+    subset: Optional[RadarDataSubset] = None,
+    time_resolution: Optional[TimeResolution] = None,
+    period_type: Optional[PeriodType] = None,
 ) -> str:
     """
     Compute URL path to data product.
 
     Supports composite- and site-based radar data as well as RADOLAN_CDC.
 
     Composites
     ----------
-    - https://opendata.dwd.de/weather/radar/composite/
+    - https://opendata.dwd.de/weather/radar/composit/
     - https://opendata.dwd.de/weather/radar/radolan/
     - https://opendata.dwd.de/climate_environment/CDC/grids_germany/daily/radolan/
     - https://opendata.dwd.de/climate_environment/CDC/grids_germany/hourly/radolan/
     - https://opendata.dwd.de/climate_environment/CDC/grids_germany/5_minutes/radolan/
 
     Sites
     -----
     - https://opendata.dwd.de/weather/radar/sites/
 
 
     :param parameter:       The radar moment to request
     :param site:            Site/station if parameter is one of
                             RADAR_PARAMETERS_SITES
-    :param fmt:          Data format (BINARY, BUFR, HDF5)
+    :param format:          Data format (BINARY, BUFR, HDF5)
     :param subset:          The subset (simple or polarimetric) for HDF5 data.
-    :param resolution: Time resolution for RadarParameter.RADOLAN_CDC,
+    :param time_resolution: Time resolution for RadarParameter.RADOLAN_CDC,
                             either daily or hourly or 5 minutes.
-    :param period:     Period type for RadarParameter.RADOLAN_CDC
+    :param period_type:     Period type for RadarParameter.RADOLAN_CDC
 
     :return:                URL path to data product
     """
-    if parameter == DwdRadarParameter.RADOLAN_CDC:
-        if resolution == Resolution.MINUTE_5:
+    if parameter == RadarParameter.RADOLAN_CDC:
+        if time_resolution == TimeResolution.MINUTE_5:
             # See also page 4 on
-            # https://opendata.dwd.de/climate_environment/CDC/help/RADOLAN/Unterstuetzungsdokumente/
-            # Unterstuetzungsdokumente-Verwendung_von_RADOLAN-Produkten_im_ASCII-GIS-Rasterformat_in_GIS.pdf
-            return f"climate_environment/CDC/grids_germany/{resolution.value}/radolan/reproc/2017_002/bin"
+            # https://opendata.dwd.de/climate_environment/CDC/help/RADOLAN/Unterstuetzungsdokumente/Unterstuetzungsdokumente-Verwendung_von_RADOLAN-Produkten_im_ASCII-GIS-Rasterformat_in_GIS.pdf  # noqa:E501,B950
+            parameter_path = f"{DWD_CDC_PATH}/grids_germany/{time_resolution.value}/radolan/reproc/2017_002/bin"  # noqa:E501,B950
         else:
-            return f"climate_environment/CDC/grids_germany/{resolution.value}/radolan/{period.value}/bin"
+            parameter_path = f"{DWD_CDC_PATH}/grids_germany/{time_resolution.value}/radolan/{period_type.value}/bin"  # noqa:E501,B950
 
     elif parameter in RADAR_PARAMETERS_COMPOSITES:
-        return f"weather/radar/composite/{parameter.value}"
+        parameter_path = f"weather/radar/composit/{parameter.value}"
 
     elif parameter in RADAR_PARAMETERS_RADOLAN:
-        return f"weather/radar/radolan/{parameter.value}"
+        parameter_path = f"weather/radar/radolan/{parameter.value}"
 
     elif parameter in RADAR_PARAMETERS_RADVOR:
-        return f"weather/radar/radvor/{parameter.value}"
+        parameter_path = f"weather/radar/radvor/{parameter.value}"
 
     elif parameter in RADAR_PARAMETERS_SITES:
+
         # Sanity checks.
         if site is None:
             raise ValueError("Argument 'site' is missing")
 
-        if fmt is None:
+        if format is None:
+
             ambiguous_parameters = [
-                DwdRadarParameter.PE_ECHO_TOP,
-                DwdRadarParameter.PR_VELOCITY,
-                DwdRadarParameter.PX_REFLECTIVITY,
-                DwdRadarParameter.PZ_CAPPI,
+                RadarParameter.PE_ECHO_TOP,
+                RadarParameter.PL_VOLUME_SCAN,
+                RadarParameter.PR_VELOCITY,
+                RadarParameter.PX_REFLECTIVITY,
+                RadarParameter.PZ_CAPPI,
             ]
 
             candidates = None
             if parameter in ambiguous_parameters:
-                candidates = [DwdRadarDataFormat.BINARY, DwdRadarDataFormat.BUFR]
+                candidates = [RadarDataFormat.BINARY, RadarDataFormat.BUFR]
             if parameter in RADAR_PARAMETERS_SWEEPS:
-                candidates = [DwdRadarDataFormat.BUFR, DwdRadarDataFormat.HDF5]
+                candidates = [RadarDataFormat.BUFR, RadarDataFormat.HDF5]
 
             if candidates:
-                raise ValueError(f"Argument 'format' is missing, use one of {candidates}")
+                raise ValueError(
+                    f"Argument 'format' is missing, use one of {candidates}"
+                )
 
         # Compute path to BINARY/BUFR vs. HDF5.
         parameter_path = f"weather/radar/sites/{parameter.value}/{site.value}"
-        if fmt == DwdRadarDataFormat.HDF5:
+        if format == RadarDataFormat.HDF5:
             if subset is None:
-                candidates = [
-                    DwdRadarDataSubset.SIMPLE,
-                    DwdRadarDataSubset.POLARIMETRIC,
-                ]
-                raise ValueError(f"Argument 'subset' is missing, use one of {candidates}")
-            return f"{parameter_path}/{fmt.value}/filter_{subset.value}/"
-
-        return parameter_path
+                candidates = [RadarDataSubset.SIMPLE, RadarDataSubset.POLARIMETRIC]
+                raise ValueError(
+                    f"Argument 'subset' is missing, use one of {candidates}"
+                )
+            parameter_path = f"{parameter_path}/{format.value}/filter_{subset.value}/"
 
     else:  # pragma: no cover
         raise NotImplementedError(f"Acquisition for {parameter} not implemented yet")
+
+    return parameter_path
```

### Comparing `wetterdienst-0.82.0/wetterdienst/provider/dwd/radar/metadata/parameter.py` & `wetterdienst-0.9.0/wetterdienst/dwd/radar/metadata.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,75 @@
-# Copyright (C) 2018-2021, earthobservations developers.
-# Distributed under the MIT License. See LICENSE for more info.
 from enum import Enum
 
 
-class DwdRadarParameter(Enum):
+class RadarDate(Enum):
+    """
+    Enumeration for pointing to different radar dates.
+    """
+
+    LATEST = "latest"
+    CURRENT = "current"
+    MOST_RECENT = "most_recent"
+
+
+class RadarDataFormat(Enum):
+    """
+    Radar data formats.
+    """
+
+    BINARY = "binary"
+    BUFR = "bufr"
+    HDF5 = "hdf5"
+
+
+class RadarDataSubset(Enum):
+    """
+    HDF5 subset types for radar sweep data.
+
+    https://opendata.dwd.de/weather/radar/sites/sweep_pcp_v/boo/hdf5/
+    """
+
+    SIMPLE = "simple"
+    POLARIMETRIC = "polarimetric"
+
+
+class RadarParameter(Enum):
     """
     All available radar moments.
     """
 
     # /composites
-    # https://docs.wradlib.org/en/stable/notebooks/fileio/wradlib_radar_formats.html#German-Weather-Service:-RADOLAN-(quantitative)-composit  # noqa:B950,E501
+    # https://docs.wradlib.org/en/stable/notebooks/fileio/wradlib_radar_formats.html#German-Weather-Service:-RADOLAN-(quantitative)-composit  # noqa:E501,B950
 
-    # https://opendata.dwd.de/weather/radar/composite/
-    HG_REFLECTIVITY = "hg"
+    # https://opendata.dwd.de/weather/radar/composit/
+    FX_REFLECTIVITY = "fx"
     PG_REFLECTIVITY = "pg"
-    RV_REFLECTIVITY = "rv"
+    WX_REFLECTIVITY = "wx"
     WN_REFLECTIVITY = "wn"
+    RX_REFLECTIVITY = "rx"
 
     # /radolan
     # https://opendata.dwd.de/weather/radar/radolan/
     RW_REFLECTIVITY = "rw"
     RY_REFLECTIVITY = "ry"
     SF_REFLECTIVITY = "sf"
 
     # /radvor
     # https://opendata.dwd.de/weather/radar/radvor/
     RE_REFLECTIVITY = "re"
     RQ_REFLECTIVITY = "rq"
 
     # /sites
     # https://opendata.dwd.de/weather/radar/sites/
-    # https://docs.wradlib.org/en/stable/notebooks/fileio/wradlib_radar_formats.html#German-Weather-Service:-DX-format
+    # https://docs.wradlib.org/en/stable/notebooks/fileio/wradlib_radar_formats.html#German-Weather-Service:-DX-format  # noqa:E501,B950
     DX_REFLECTIVITY = "dx"
     LMAX_VOLUME_SCAN = "lmax"
     PE_ECHO_TOP = "pe"
     PF_REFLECTIVITY = "pf"
+    PL_VOLUME_SCAN = "pl"
     PR_VELOCITY = "pr"
     PX_REFLECTIVITY = "px"
     PX250_REFLECTIVITY = "px250"
     PZ_CAPPI = "pz"
 
     # OPERA HDF5 (ODIM_H5)
     # https://docs.wradlib.org/en/stable/notebooks/fileio/wradlib_radar_formats.html#HDF5
@@ -50,72 +81,43 @@
     # https://opendata.dwd.de/climate_environment/CDC/grids_germany/daily/radolan/
     # https://opendata.dwd.de/climate_environment/CDC/grids_germany/hourly/radolan/
     # https://opendata.dwd.de/climate_environment/CDC/grids_germany/5_minutes/radolan/
     RADOLAN_CDC = "radolan_cdc"
 
 
 RADAR_PARAMETERS_COMPOSITES = [
-    DwdRadarParameter.HG_REFLECTIVITY,
-    DwdRadarParameter.PG_REFLECTIVITY,
-    DwdRadarParameter.RV_REFLECTIVITY,
-    DwdRadarParameter.WN_REFLECTIVITY,
+    RadarParameter.FX_REFLECTIVITY,
+    RadarParameter.PG_REFLECTIVITY,
+    RadarParameter.WX_REFLECTIVITY,
+    RadarParameter.WN_REFLECTIVITY,
+    RadarParameter.RX_REFLECTIVITY,
 ]
 RADAR_PARAMETERS_RADOLAN = [
-    DwdRadarParameter.RW_REFLECTIVITY,
-    DwdRadarParameter.RY_REFLECTIVITY,
-    DwdRadarParameter.SF_REFLECTIVITY,
+    RadarParameter.RW_REFLECTIVITY,
+    RadarParameter.RY_REFLECTIVITY,
+    RadarParameter.SF_REFLECTIVITY,
 ]
 RADAR_PARAMETERS_RADVOR = [
-    DwdRadarParameter.RE_REFLECTIVITY,
-    DwdRadarParameter.RQ_REFLECTIVITY,
+    RadarParameter.RE_REFLECTIVITY,
+    RadarParameter.RQ_REFLECTIVITY,
 ]
 RADAR_PARAMETERS_SITES = [
-    DwdRadarParameter.DX_REFLECTIVITY,
-    DwdRadarParameter.LMAX_VOLUME_SCAN,
-    DwdRadarParameter.PE_ECHO_TOP,
-    DwdRadarParameter.PF_REFLECTIVITY,
-    DwdRadarParameter.PX_REFLECTIVITY,
-    DwdRadarParameter.PR_VELOCITY,
-    DwdRadarParameter.PX250_REFLECTIVITY,
-    DwdRadarParameter.PZ_CAPPI,
-    DwdRadarParameter.SWEEP_PCP_VELOCITY_H,
-    DwdRadarParameter.SWEEP_PCP_REFLECTIVITY_H,
-    DwdRadarParameter.SWEEP_VOL_VELOCITY_H,
-    DwdRadarParameter.SWEEP_VOL_REFLECTIVITY_H,
+    RadarParameter.DX_REFLECTIVITY,
+    RadarParameter.LMAX_VOLUME_SCAN,
+    RadarParameter.PE_ECHO_TOP,
+    RadarParameter.PF_REFLECTIVITY,
+    RadarParameter.PX_REFLECTIVITY,
+    RadarParameter.PL_VOLUME_SCAN,
+    RadarParameter.PR_VELOCITY,
+    RadarParameter.PX250_REFLECTIVITY,
+    RadarParameter.PZ_CAPPI,
+    RadarParameter.SWEEP_PCP_VELOCITY_H,
+    RadarParameter.SWEEP_PCP_REFLECTIVITY_H,
+    RadarParameter.SWEEP_VOL_VELOCITY_H,
+    RadarParameter.SWEEP_VOL_REFLECTIVITY_H,
 ]
 RADAR_PARAMETERS_SWEEPS = [
-    DwdRadarParameter.SWEEP_PCP_VELOCITY_H,
-    DwdRadarParameter.SWEEP_PCP_REFLECTIVITY_H,
-    DwdRadarParameter.SWEEP_VOL_VELOCITY_H,
-    DwdRadarParameter.SWEEP_VOL_REFLECTIVITY_H,
+    RadarParameter.SWEEP_PCP_VELOCITY_H,
+    RadarParameter.SWEEP_PCP_REFLECTIVITY_H,
+    RadarParameter.SWEEP_VOL_VELOCITY_H,
+    RadarParameter.SWEEP_VOL_REFLECTIVITY_H,
 ]
-
-
-class DwdRadarDate(Enum):
-    """
-    Enumeration for pointing to different radar dates.
-    """
-
-    LATEST = "latest"
-    CURRENT = "current"
-    MOST_RECENT = "most_recent"
-
-
-class DwdRadarDataFormat(Enum):
-    """
-    Radar data formats.
-    """
-
-    BINARY = "binary"
-    BUFR = "bufr"
-    HDF5 = "hdf5"
-
-
-class DwdRadarDataSubset(Enum):
-    """
-    HDF5 subset types for radar sweep data.
-
-    https://opendata.dwd.de/weather/radar/sites/sweep_pcp_v/boo/hdf5/
-    """
-
-    SIMPLE = "simple"
-    POLARIMETRIC = "polarimetric"
```

### Comparing `wetterdienst-0.82.0/wetterdienst/provider/dwd/radar/util.py` & `wetterdienst-0.9.0/wetterdienst/dwd/radar/util.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,11 @@
-# Copyright (C) 2018-2021, earthobservations developers.
-# Distributed under the MIT License. See LICENSE for more info.
-from __future__ import annotations
-
-import datetime as dt
 import re
-from typing import TYPE_CHECKING
+import dateparser
+from wetterdienst.dwd.metadata.datetime import DatetimeFormat
 
-if TYPE_CHECKING:
-    from io import BytesIO
 
 # 6-character timestamps are used for data within "RADOLAN_CDC/historical".
 # Examples:
 # - SF201901.tar.gz
 RADAR_DT_REGEX_SHORT = r"(?<!\d)\d{6}(?!\d)"
 
 # 10-character timestamps are used for data within
@@ -28,36 +22,23 @@
 # - sweep_pcp_v_0-20200926143033_10132--buf.bz2
 # - rab02-tt_10132-20200926161533-boo---buf
 # - ras07-stqual-vol5minng01_sweeph5onem_vradh_00-2020092614305700-boo-10132-hd5
 # - ras07-vol5minng01_sweeph5onem_vradh_00-2020092614305700-boo-10132-hd5
 RADAR_DT_REGEX_LONG = r"(?<!\d)\d{12}"
 
 
-RADAR_DT_PATTERN = re.compile(f"{RADAR_DT_REGEX_LONG}|{RADAR_DT_REGEX_MEDIUM}|{RADAR_DT_REGEX_SHORT}")
+RADAR_DT_PATTERN = re.compile(f"{RADAR_DT_REGEX_LONG}|{RADAR_DT_REGEX_MEDIUM}")
 RADOLAN_DT_PATTERN = re.compile(f"{RADAR_DT_REGEX_SHORT}|{RADAR_DT_REGEX_MEDIUM}")
 
 
-def get_date_from_filename(filename: str, pattern: re.Pattern, formats: list[str]) -> dt.datetime | None:
+def get_date_from_filename(filename):
     try:
-        date_string = pattern.findall(filename)[0]
+        datestr = RADAR_DT_PATTERN.findall(filename)[0]
+        return dateparser.parse(
+            datestr,
+            date_formats=[
+                DatetimeFormat.ymdhm.value,
+                DatetimeFormat.YMDHM.value,
+            ],
+        )
     except IndexError:
-        return None
-
-    for fmt in formats:
-        try:
-            return dt.datetime.strptime(date_string, fmt)
-        except ValueError:
-            pass
-    return None
-
-
-def verify_hdf5(buffer: BytesIO):
-    import h5py
-
-    buffer.seek(0)
-    try:
-        nc = h5py.File(buffer, mode="r")
-        nc.close()
-        buffer.seek(0)
-    except Exception:
-        buffer.seek(0)
-        raise
+        pass
```

### Comparing `wetterdienst-0.82.0/wetterdienst/provider/eumetnet/opera/sites.py` & `wetterdienst-0.9.0/wetterdienst/dwd/pandas.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,180 +1,205 @@
-# Copyright (C) 2018-2021, earthobservations developers.
-# Distributed under the MIT License. See LICENSE for more info.
-from __future__ import annotations
-
-import gzip
-import importlib.resources
+# Extending pandas
+# https://pandas.pydata.org/pandas-docs/stable/development/extending.html
 import json
-from typing import Any
-
-import requests
-
-
-class OperaRadarSites:
-    """
-    Provide information about all European OPERA radar sites.
-    """
-
-    data_file = importlib.resources.files(__package__) / "sites.json.gz"
 
-    def __init__(self):
-        self.sites = self.load()
-
-    def load(self) -> list[dict]:
-        """
-        Load and decode JSON file from filesystem.
-        """
-        with importlib.resources.as_file(self.data_file) as rf:
-            with gzip.open(rf, mode="rb") as f:
-                return json.load(f)
-
-    def all(self) -> list[dict]:  # noqa: A003
-        """
-        The whole list of OPERA radar sites.
-        """
-        return self.sites
+import pandas as pd
 
-    def to_dict(self) -> dict:
-        """
-        Dictionary of sites, keyed by ODIM code.
-        """
-        result = {}
-        for site in self.sites:
-            if site["odimcode"] is None:
-                continue
-            result[site["odimcode"]] = site
-        return result
+from wetterdienst.dwd.metadata import TimeResolution
+from wetterdienst.dwd.metadata.column_names import DWDMetaColumns
+from wetterdienst.dwd.util import parse_datetime, mktimerange
+
+
+POSSIBLE_ID_VARS = (
+    DWDMetaColumns.STATION_ID.value,
+    DWDMetaColumns.DATE.value,
+    DWDMetaColumns.FROM_DATE.value,
+    DWDMetaColumns.TO_DATE.value,
+)
+
+POSSIBLE_DATE_VARS = (
+    DWDMetaColumns.DATE.value,
+    DWDMetaColumns.FROM_DATE.value,
+    DWDMetaColumns.TO_DATE.value,
+)
+
+
+@pd.api.extensions.register_dataframe_accessor("dwd")
+class PandasDwdExtension:
+    def __init__(self, pandas_obj):
+        self.df = pandas_obj
+
+    def lower(self) -> pd.DataFrame:
+        """
+        Make Pandas DataFrame column names and parameters lowercase.
+
+        :return: Mungled DataFrame
+        """
+        df = self.df.rename(columns=str.lower)
+
+        for attribute in DWDMetaColumns.PARAMETER, DWDMetaColumns.ELEMENT:
+            attribute_name = attribute.value.lower()
+            if attribute_name in df:
+                df[attribute_name] = df[attribute_name].str.lower()
+
+        return df
+
+    def filter_by_date(
+        self, date: str, time_resolution: TimeResolution
+    ) -> pd.DataFrame:
+        """
+        Filter Pandas DataFrame by date or date interval.
+
+        Accepts different kinds of date formats, like:
+
+        - 2020-05-01
+        - 2020-06-15T12
+        - 2020-05
+        - 2019
+        - 2020-05-01/2020-05-05
+        - 2017-01/2019-12
+        - 2010/2020
+
+        :param date:
+        :param time_resolution:
+        :return: Filtered DataFrame
+        """
+
+        # Filter by date interval.
+        if "/" in date:
+            date_from, date_to = date.split("/")
+            date_from = parse_datetime(date_from)
+            date_to = parse_datetime(date_to)
+            if time_resolution in (
+                TimeResolution.ANNUAL,
+                TimeResolution.MONTHLY,
+            ):
+                date_from, date_to = mktimerange(time_resolution, date_from, date_to)
+                expression = (date_from <= self.df[DWDMetaColumns.FROM_DATE.value]) & (
+                    self.df[DWDMetaColumns.TO_DATE.value] <= date_to
+                )
+            else:
+                expression = (date_from <= self.df[DWDMetaColumns.DATE.value]) & (
+                    self.df[DWDMetaColumns.DATE.value] <= date_to
+                )
+            df = self.df[expression]
 
-    def by_odim_code(self, odim_code: str) -> dict:
-        """
-        Return radar site by ODIM code.
+        # Filter by specific date.
+        else:
+            date = parse_datetime(date)
+            if time_resolution in (
+                TimeResolution.ANNUAL,
+                TimeResolution.MONTHLY,
+            ):
+                date_from, date_to = mktimerange(time_resolution, date)
+                expression = (date_from <= self.df[DWDMetaColumns.FROM_DATE.value]) & (
+                    self.df[DWDMetaColumns.TO_DATE.value] <= date_to
+                )
+            else:
+                expression = date == self.df[DWDMetaColumns.DATE.value]
+            df = self.df[expression]
+
+        return df
+
+    def format(self, fmt: str) -> str:
+        """
+        Format/render Pandas DataFrame to given output format.
+
+        :param fmt: One of json, geojson, csv, excel.
+        :return: Rendered payload.
+        """
+
+        # Output as GeoJSON.
+        if fmt == "geojson":
+            output = json.dumps(self.df.dwd.to_geojson(), indent=4)
 
-        :param odim_code: The ODIM code, e.g. "atrau".
-        :return:          Single site information.
-        """
-        if len(odim_code) not in (3, 5):
-            raise ValueError("ODIM code must be three or five letters")
-        for site in self.sites:
-            if site["odimcode"] and odim_code.lower() in site["odimcode"]:
-                return site
         else:
-            raise KeyError("Radar site not found")
+            output = self.df.io.format(fmt=fmt)
 
-    def by_wmo_code(self, wmo_code: int) -> dict:
-        """
-        Return radar site by WMO code.
+        return output
 
-        :param wmo_code: The WMO code, e.g. 11038.
-        :return:        Single site information.
+    def to_geojson(self) -> dict:
         """
-        for site in self.sites:
-            if site["wmocode"] == wmo_code:
-                return site
-        else:
-            raise KeyError("Radar site not found")
+        Convert DWD station information into GeoJSON format.
 
-    def by_country_name(self, country_name: str) -> list[dict]:
-        """
-        Filter list of radar sites by country name.
+        Args:
+            df: Input DataFrame containing station information.
+
+        Return:
+             Dictionary in GeoJSON FeatureCollection format.
+        """
+        df = self.df.rename(columns=str.lower)
+
+        features = []
+        for _, station in df.iterrows():
+            features.append(
+                {
+                    "type": "Feature",
+                    "properties": {
+                        "id": station["station_id"],
+                        "name": station["station_name"],
+                        "state": station["state"],
+                        "from_date": station["from_date"].isoformat(),
+                        "to_date": station["to_date"].isoformat(),
+                        "has_file": station["has_file"],
+                    },
+                    "geometry": {
+                        # WGS84 is implied and coordinates represent decimal degrees
+                        # ordered as "longitude, latitude [,elevation]" with z expressed
+                        # as metres above mean sea level per WGS84.
+                        # -- http://wiki.geojson.org/RFC-001
+                        "type": "Point",
+                        "coordinates": [
+                            station["lon"],
+                            station["lat"],
+                            station["station_height"],
+                        ],
+                    },
+                }
+            )
+
+        return {
+            "type": "FeatureCollection",
+            "features": features,
+        }
+
+    def tidy_up_data(self) -> pd.DataFrame:
+        """
+        Function to create a tidy DataFrame by reshaping it, putting quality in a
+        separate column, so that for each timestamp there is a tuple of parameter, value
+        and quality.
+
+        :return:            The tidied DataFrame
+        """
+        id_vars = []
+        date_vars = []
+
+        # Add id columns based on metadata columns
+        for column in POSSIBLE_ID_VARS:
+            if column in self.df:
+                id_vars.append(column)
+                if column in POSSIBLE_DATE_VARS:
+                    date_vars.append(column)
+
+        # Extract quality
+        # Set empty quality for first columns until first QN column
+        quality = pd.Series(dtype=pd.Int64Dtype())
+        column_quality = pd.Series(dtype=pd.Int64Dtype())
+
+        for column in self.df:
+            # If is quality column, overwrite current "column quality"
+            if column.startswith("QN"):
+                column_quality = self.df.pop(column)
+            else:
+                quality = quality.append(column_quality)
+
+        df_tidy = self.df.melt(
+            id_vars=id_vars,
+            var_name=DWDMetaColumns.ELEMENT.value,
+            value_name=DWDMetaColumns.VALUE.value,
+        )
+
+        df_tidy[DWDMetaColumns.QUALITY.value] = quality.reset_index(drop=True).astype(
+            pd.Int64Dtype()
+        )
 
-        :param country_name: The country name, e.g. "Germany", "United Kingdom".
-        :return:             List of site information.
-        """
-        sites = [site for site in self.sites if site["country"] and site["country"].lower() == country_name.lower()]
-        if not sites:
-            raise KeyError("No radar sites for this country")
-        return sites
-
-
-class OperaRadarSitesGenerator:
-    """
-    Parse list of OPERA sites published by EUMETNET.
-
-    https://www.eumetnet.eu/wp-content/themes/aeron-child/observations-programme/current-activities/opera/database/OPERA_Database/OPERA_RADARS_DB.json
-    """
-
-    url = (
-        "https://www.eumetnet.eu/wp-content/themes/aeron-child/observations-programme/"
-        "current-activities/opera/database/OPERA_Database/OPERA_RADARS_DB.json"
-    )
-
-    def get_opera_radar_sites(self) -> list[dict]:  # pragma: no cover
-        data = requests.get(self.url, timeout=10).json()
-
-        # Filter empty elements and convert data types.
-        integer_values = ["maxrange", "number", "startyear", "status", "wmocode"]
-        float_values = [
-            "beam",
-            "diametrantenna",
-            "frequency",
-            "gain",
-            "heightantenna",
-            "heightofstation",
-            "latitude",
-            "longitude",
-        ]
-        boolean_values = ["doppler", "status"]
-
-        def asbool(obj: Any) -> bool:
-            # from sqlalchemy.util.asbool
-            if isinstance(obj, str):
-                obj = obj.strip().lower()
-                if obj in ["true", "yes", "on", "y", "t", "1"]:
-                    return True
-                elif obj in ["false", "no", "off", "n", "f", "0"]:
-                    return False
-                else:
-                    raise ValueError("String is not true/false: %r" % obj)
-            return bool(obj)
-
-        def convert_types(element: dict) -> dict[str, int | float | bool | None]:
-            converted = {}
-            for key, value in element.items():
-                try:
-                    if key in integer_values:
-                        value = int(value)
-                    if key in float_values:
-                        value = float(value)
-                    if key in boolean_values:
-                        value = asbool(value)
-                    if value == "":
-                        value = None
-                except ValueError:
-                    value = None
-                converted[key] = value
-            return converted
-
-        def filter_and_convert(elements):
-            for element in elements:
-                if element["location"] and element["latitude"] and element["longitude"]:
-                    yield convert_types(element)
-
-        return list(filter_and_convert(data))
-
-    def to_json(self, indent: int = 4) -> str:
-        """
-        Return JSON representation of all sites.
-        """
-        sites = self.get_opera_radar_sites()
-        return json.dumps(sites, indent=indent)
-
-    def export(self, indent: int = 4):
-        """
-        Generate "sites.json.gz".
-        """
-        sites = self.get_opera_radar_sites()
-        with importlib.resources.as_file(OperaRadarSites.data_file) as rf:
-            with gzip.open(rf, mode="wt", compresslevel=9, encoding="utf-8") as f:
-                json.dump(sites, f, indent=indent)
-
-
-if __name__ == "__main__":  # pragma: no cover
-    """
-    Generate "sites.json.gz".
-
-    Synopsis::
-
-        python wetterdienst/provider/eumetnet/opera/sites.py
-    """
-    orsg = OperaRadarSitesGenerator()
-    orsg.export()
+        return df_tidy
```

### Comparing `wetterdienst-0.82.0/wetterdienst/util/cli.py` & `wetterdienst-0.9.0/wetterdienst/util/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,49 @@
-# Copyright (C) 2018-2021, earthobservations developers.
-# Distributed under the MIT License. See LICENSE for more info.
-"""A set of utility functions"""
-
-from __future__ import annotations
-
-import logging
+""" A set of utility functions """
 import sys
-import textwrap
+import logging
+from typing import List
+
+from munch import Munch, munchify
 
 
 def setup_logging(level=logging.INFO) -> None:
-    log_format = "%(asctime)-15s [%(name)-40s] %(levelname)-7s: %(message)s"
+    log_format = "%(asctime)-15s [%(name)-30s] %(levelname)-7s: %(message)s"
     logging.basicConfig(format=log_format, stream=sys.stderr, level=level)
 
     # Silence INFO messages from numexpr.
     numexpr_logger = logging.getLogger("numexpr")
     numexpr_logger.setLevel(logging.WARN)
 
-    # Silence WARNING messages from pint.
-    pint_logger = logging.getLogger("pint")
-    pint_logger.setLevel(logging.ERROR)
 
+def normalize_options(options: dict) -> Munch:
+    normalized = {}
+    for key, value in options.items():
 
-def read_list(data: str | None, separator: str = ",") -> list[str]:
+        # Add primary variant.
+        chars = "--<>"
+        key = key.strip(chars)
+        normalized[key] = value
+
+        # Add secondary variant.
+        key = key.replace("-", "_")
+        normalized[key] = value
+
+    return munchify(normalized, factory=OptionMunch)
+
+
+def read_list(data: str, separator: str = u",") -> List[str]:
     if data is None:
         return []
 
     result = [x.strip() for x in data.split(separator)]
 
     if len(result) == 1 and not result[0]:
-        return []
+        result = []
 
     return result
 
 
-def docstring_format_verbatim(text: str) -> str:
-    """
-    Format docstring to be displayed verbatim as a help text by Click.
-
-    - https://click.palletsprojects.com/en/8.1.x/documentation/#preventing-rewrapping
-    - https://github.com/pallets/click/issues/56
-    """
-    text = textwrap.dedent(text)
-    lines = [line if line.strip() else "\b" for line in text.splitlines()]
-    return "\n".join(lines)
+class OptionMunch(Munch):
+    def __setattr__(self, k, v):
+        super().__setattr__(k.replace("-", "_"), v)
+        super().__setattr__(k.replace("_", "-"), v)
```

