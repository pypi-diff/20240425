# Comparing `tmp/finvizlite-0.1.1.tar.gz` & `tmp/finvizlite-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/finvizlite-0.1.1.tar", last modified: Mon Oct 19 08:17:27 2020, max compression
+gzip compressed data, was "finvizlite-0.1.2.tar", last modified: Thu Apr 25 04:22:05 2024, max compression
```

## Comparing `finvizlite-0.1.1.tar` & `finvizlite-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxrwxr-x   0 tom       (1001) tom       (1001)        0 2020-10-19 08:17:27.592097 finvizlite-0.1.1/
--rw-rw-r--   0 tom       (1001) tom       (1001)     4008 2020-10-19 08:17:27.592097 finvizlite-0.1.1/PKG-INFO
--rw-rw-r--   0 tom       (1001) tom       (1001)     3321 2020-10-19 07:36:18.000000 finvizlite-0.1.1/README.md
-drwxrwxr-x   0 tom       (1001) tom       (1001)        0 2020-10-19 08:17:27.588097 finvizlite-0.1.1/finvizlite/
--rw-rw-r--   0 tom       (1001) tom       (1001)     2857 2020-10-19 06:39:29.000000 finvizlite-0.1.1/finvizlite/__init__.py
-drwxrwxr-x   0 tom       (1001) tom       (1001)        0 2020-10-19 08:17:27.592097 finvizlite-0.1.1/finvizlite.egg-info/
--rw-rw-r--   0 tom       (1001) tom       (1001)     4008 2020-10-19 08:17:27.000000 finvizlite-0.1.1/finvizlite.egg-info/PKG-INFO
--rw-rw-r--   0 tom       (1001) tom       (1001)      210 2020-10-19 08:17:27.000000 finvizlite-0.1.1/finvizlite.egg-info/SOURCES.txt
--rw-rw-r--   0 tom       (1001) tom       (1001)        1 2020-10-19 08:17:27.000000 finvizlite-0.1.1/finvizlite.egg-info/dependency_links.txt
--rw-rw-r--   0 tom       (1001) tom       (1001)       25 2020-10-19 08:17:27.000000 finvizlite-0.1.1/finvizlite.egg-info/requires.txt
--rw-rw-r--   0 tom       (1001) tom       (1001)       11 2020-10-19 08:17:27.000000 finvizlite-0.1.1/finvizlite.egg-info/top_level.txt
--rw-rw-r--   0 tom       (1001) tom       (1001)       38 2020-10-19 08:17:27.592097 finvizlite-0.1.1/setup.cfg
--rw-rw-r--   0 tom       (1001) tom       (1001)      707 2020-10-19 08:16:22.000000 finvizlite-0.1.1/setup.py
+drwxrwxr-x   0 bob       (1000) bob       (1000)        0 2024-04-25 04:22:05.638320 finvizlite-0.1.2/
+-rw-rw-r--   0 bob       (1000) bob       (1000)     1078 2024-04-25 03:22:22.000000 finvizlite-0.1.2/LICENSE
+-rw-r--r--   0 bob       (1000) bob       (1000)     3692 2024-04-25 04:22:05.638320 finvizlite-0.1.2/PKG-INFO
+-rw-rw-r--   0 bob       (1000) bob       (1000)     3321 2024-04-25 03:22:22.000000 finvizlite-0.1.2/README.md
+drwxrwxr-x   0 bob       (1000) bob       (1000)        0 2024-04-25 04:22:05.638320 finvizlite-0.1.2/finvizlite/
+-rw-rw-r--   0 bob       (1000) bob       (1000)     2966 2024-04-25 04:03:10.000000 finvizlite-0.1.2/finvizlite/__init__.py
+drwxrwxr-x   0 bob       (1000) bob       (1000)        0 2024-04-25 04:22:05.638320 finvizlite-0.1.2/finvizlite.egg-info/
+-rw-r--r--   0 bob       (1000) bob       (1000)     3692 2024-04-25 04:22:05.000000 finvizlite-0.1.2/finvizlite.egg-info/PKG-INFO
+-rw-rw-r--   0 bob       (1000) bob       (1000)      243 2024-04-25 04:22:05.000000 finvizlite-0.1.2/finvizlite.egg-info/SOURCES.txt
+-rw-rw-r--   0 bob       (1000) bob       (1000)        1 2024-04-25 04:22:05.000000 finvizlite-0.1.2/finvizlite.egg-info/dependency_links.txt
+-rw-rw-r--   0 bob       (1000) bob       (1000)       25 2024-04-25 04:22:05.000000 finvizlite-0.1.2/finvizlite.egg-info/requires.txt
+-rw-rw-r--   0 bob       (1000) bob       (1000)       11 2024-04-25 04:22:05.000000 finvizlite-0.1.2/finvizlite.egg-info/top_level.txt
+-rw-rw-r--   0 bob       (1000) bob       (1000)       38 2024-04-25 04:22:05.638320 finvizlite-0.1.2/setup.cfg
+-rw-rw-r--   0 bob       (1000) bob       (1000)      707 2024-04-25 04:19:11.000000 finvizlite-0.1.2/setup.py
+drwxrwxr-x   0 bob       (1000) bob       (1000)        0 2024-04-25 04:22:05.638320 finvizlite-0.1.2/tests/
+-rw-rw-r--   0 bob       (1000) bob       (1000)     1043 2024-04-25 04:09:21.000000 finvizlite-0.1.2/tests/test_finvizlite.py
```

### Comparing `finvizlite-0.1.1/PKG-INFO` & `finvizlite-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,60 +1,64 @@
 Metadata-Version: 2.1
 Name: finvizlite
-Version: 0.1.1
+Version: 0.1.2
 Summary: A lightweight finviz screener scraper
 Home-page: https://github.com/andr3w321/finvizlite
 Author: Andrew Rennhack
 Author-email: andr3w321@gmail.com
 License: MIT
-Description: # Finvizlite
-        
-        [![Build Status](https://travis-ci.org/andr3w321/finvizlite.svg?branch=main)](https://travis-ci.org/andr3w321/finvizlite)
-        
-        A lightweight finviz.com screener scraper for https://finviz.com/screener.ashx
-        All the code is about 80 lines long and can be found in `finvizlite/__init__.py`
-        
-        
-        ## Install
-        `pip install finvizlite`
-        
-        ## Quick start
-        
-        ```
-        import finvizlite as fl
-        
-        # To scrape a single page use fl.scrape(url)
-        df = fl.scrape("https://finviz.com/screener.ashx?v=141&o=-marketcap")
-        
-        # To scrape multiple pages use fl.scrape_all(url)
-        # scrape the dow tickers
-        df = fl.scrape_all("https://finviz.com/screener.ashx?v=141&f=idx_dji&o=-marketcap")
-        
-        # To print the scraped urls pass print_urls=True to scrape_all() or scrape()
-        >>> df = fl.scrape_all("https://finviz.com/screener.ashx?v=161&f=idx_dji&o=-marketcap", print_urls=True)
-        https://finviz.com/screener.ashx?v=161&f=idx_dji&o=-marketcap
-        https://finviz.com/screener.ashx?v=161&f=idx_dji&o=-marketcap&r=21
-        
-        # To limit the amount of tickers scraped pass rows=max_rows to scrape_all
-        >>> df = fl.scrape_all("https://finviz.com/screener.ashx?v=121&o=-marketcap", print_urls=True, rows=50)
-        https://finviz.com/screener.ashx?v=121&o=-marketcap
-        https://finviz.com/screener.ashx?v=121&o=-marketcap&r=21
-        https://finviz.com/screener.ashx?v=121&o=-marketcap&r=41
-        
-        # Download all the tickers from Overview page (takes ~2.5 mins)
-        df = fl.scrape_all("https://finviz.com/screener.ashx?v=111&o=-marketcap", print_urls=True)
-        
-        # Save to csv
-        df.to_csv("all_tickers.csv", index=False)
-        
-        # Speed up scraping. By default scrape_all sleeps 0.1 seconds between requests. You can shorten(or lengthen it) by passing the sleep_interval=time_in_seconds to scrape_url to speed up or slow down scraping, but you may run into "Too many requests" errors from finviz.com if you set it too low and make too many requests in a short time.
-        >>>df = fl.scrape_all("https://finviz.com/screener.ashx?v=111&o=-marketcap", sleep_interval=0)
-        ValueError: too many requests while getting https://finviz.com/screener.ashx?v=111&o=-marketcap&r=241
-        
-        # If you want a list of the pagination urls for some reason, pass print_df_only=False to scrape()
-        >>> urls, df = fl.scrape("https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap", return_df_only=False)
-        >>> urls
-        ['https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=21', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=41', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=61', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=81', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=101', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=121', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=141', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=161', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=181', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=201', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=221', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=241', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=261', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=281']
-        ```
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: bs4
+Requires-Dist: lxml
+Requires-Dist: pandas
+
+# Finvizlite
+
+[![Build Status](https://travis-ci.org/andr3w321/finvizlite.svg?branch=main)](https://travis-ci.org/andr3w321/finvizlite)
+
+A lightweight finviz.com screener scraper for https://finviz.com/screener.ashx
+All the code is about 80 lines long and can be found in `finvizlite/__init__.py`
+
+
+## Install
+`pip install finvizlite`
+
+## Quick start
+
+```
+import finvizlite as fl
+
+# To scrape a single page use fl.scrape(url)
+df = fl.scrape("https://finviz.com/screener.ashx?v=141&o=-marketcap")
+
+# To scrape multiple pages use fl.scrape_all(url)
+# scrape the dow tickers
+df = fl.scrape_all("https://finviz.com/screener.ashx?v=141&f=idx_dji&o=-marketcap")
+
+# To print the scraped urls pass print_urls=True to scrape_all() or scrape()
+>>> df = fl.scrape_all("https://finviz.com/screener.ashx?v=161&f=idx_dji&o=-marketcap", print_urls=True)
+https://finviz.com/screener.ashx?v=161&f=idx_dji&o=-marketcap
+https://finviz.com/screener.ashx?v=161&f=idx_dji&o=-marketcap&r=21
+
+# To limit the amount of tickers scraped pass rows=max_rows to scrape_all
+>>> df = fl.scrape_all("https://finviz.com/screener.ashx?v=121&o=-marketcap", print_urls=True, rows=50)
+https://finviz.com/screener.ashx?v=121&o=-marketcap
+https://finviz.com/screener.ashx?v=121&o=-marketcap&r=21
+https://finviz.com/screener.ashx?v=121&o=-marketcap&r=41
+
+# Download all the tickers from Overview page (takes ~2.5 mins)
+df = fl.scrape_all("https://finviz.com/screener.ashx?v=111&o=-marketcap", print_urls=True)
+
+# Save to csv
+df.to_csv("all_tickers.csv", index=False)
+
+# Speed up scraping. By default scrape_all sleeps 0.1 seconds between requests. You can shorten(or lengthen it) by passing the sleep_interval=time_in_seconds to scrape_url to speed up or slow down scraping, but you may run into "Too many requests" errors from finviz.com if you set it too low and make too many requests in a short time.
+>>>df = fl.scrape_all("https://finviz.com/screener.ashx?v=111&o=-marketcap", sleep_interval=0)
+ValueError: too many requests while getting https://finviz.com/screener.ashx?v=111&o=-marketcap&r=241
+
+# If you want a list of the pagination urls for some reason, pass print_df_only=False to scrape()
+>>> urls, df = fl.scrape("https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap", return_df_only=False)
+>>> urls
+['https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=21', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=41', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=61', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=81', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=101', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=121', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=141', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=161', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=181', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=201', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=221', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=241', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=261', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=281']
+```
```

### Comparing `finvizlite-0.1.1/README.md` & `finvizlite-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `finvizlite-0.1.1/finvizlite/__init__.py` & `finvizlite-0.1.2/finvizlite/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,16 +13,15 @@
     query = requests.utils.urlparse(old_url).query
     params = dict(x.split('=') for x in query.split("&"))
     params[param_field] = new_param_value
     pre_query_url = old_url.split("?")[0]
     new_url = pre_query_url + "?" + '&'.join('{}={}'.format(key, val) for key, val in params.items())
     return new_url
 
-def get_html(url):
-    hdr = {'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.11 (KHTML, like Gecko) Chrome/23.0.1271.64 Safari/537.11'}
+def get_html(url, hdr={'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.11 (KHTML, like Gecko) Chrome/23.0.1271.64 Safari/537.11'}):
     res = requests.get(url, headers=hdr)
     if res.status_code == 200:
         return res.text
     else:
         raise ValueError("{} getting {}", res.status_code, url)
 
 def get_pagination_urls(url, page_options):
@@ -32,22 +31,26 @@
         if "selected" not in page_options[i].attrs:
             urls.append(get_new_query_url(url, 'r', page_options[i]['value']))
     return urls
 
 def get_df(tables):
     data = []
     trs = tables[3].find_all("tr")
+    cols = []
+    ths = trs[0].find_all("th")
+    for th in ths:
+        cols.append(th.text)
     for tr in trs:
         row = []
         tds = tr.find_all("td")
         for td in tds:
             row.append(td.text)
         data.append(row)
     # don't return the header row
-    df = pd.DataFrame(data[1:], columns=data[0])
+    df = pd.DataFrame(data[1:], columns=cols)
     return df
 
 def scrape(url, return_df_only=True, print_urls=False):
     if print_urls:
         print(url)
     soup = BeautifulSoup(get_html(url), "lxml")
     if soup.text == "Too many requests.":
@@ -66,14 +69,15 @@
         return df
     else:
         return urls, df
 
 def scrape_all(url, sleep_interval=0.1, print_urls=False, rows=100000):
     pagination_urls, df = scrape(url, return_df_only=False, print_urls=print_urls)
     max_pages = rows_to_pages(rows)
+    dfs = [df]
     for i in range(0, len(pagination_urls)):
         if i >= max_pages-1:
             break
         time.sleep(sleep_interval)
         next_df = scrape(pagination_urls[i], return_df_only=True, print_urls=print_urls)
-        df = df.append(next_df, ignore_index=True)
-    return df[:rows]
+        dfs.append(next_df)
+    return pd.concat(dfs, ignore_index=True)[:rows]
```

### Comparing `finvizlite-0.1.1/finvizlite.egg-info/PKG-INFO` & `finvizlite-0.1.2/finvizlite.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,60 +1,64 @@
 Metadata-Version: 2.1
 Name: finvizlite
-Version: 0.1.1
+Version: 0.1.2
 Summary: A lightweight finviz screener scraper
 Home-page: https://github.com/andr3w321/finvizlite
 Author: Andrew Rennhack
 Author-email: andr3w321@gmail.com
 License: MIT
-Description: # Finvizlite
-        
-        [![Build Status](https://travis-ci.org/andr3w321/finvizlite.svg?branch=main)](https://travis-ci.org/andr3w321/finvizlite)
-        
-        A lightweight finviz.com screener scraper for https://finviz.com/screener.ashx
-        All the code is about 80 lines long and can be found in `finvizlite/__init__.py`
-        
-        
-        ## Install
-        `pip install finvizlite`
-        
-        ## Quick start
-        
-        ```
-        import finvizlite as fl
-        
-        # To scrape a single page use fl.scrape(url)
-        df = fl.scrape("https://finviz.com/screener.ashx?v=141&o=-marketcap")
-        
-        # To scrape multiple pages use fl.scrape_all(url)
-        # scrape the dow tickers
-        df = fl.scrape_all("https://finviz.com/screener.ashx?v=141&f=idx_dji&o=-marketcap")
-        
-        # To print the scraped urls pass print_urls=True to scrape_all() or scrape()
-        >>> df = fl.scrape_all("https://finviz.com/screener.ashx?v=161&f=idx_dji&o=-marketcap", print_urls=True)
-        https://finviz.com/screener.ashx?v=161&f=idx_dji&o=-marketcap
-        https://finviz.com/screener.ashx?v=161&f=idx_dji&o=-marketcap&r=21
-        
-        # To limit the amount of tickers scraped pass rows=max_rows to scrape_all
-        >>> df = fl.scrape_all("https://finviz.com/screener.ashx?v=121&o=-marketcap", print_urls=True, rows=50)
-        https://finviz.com/screener.ashx?v=121&o=-marketcap
-        https://finviz.com/screener.ashx?v=121&o=-marketcap&r=21
-        https://finviz.com/screener.ashx?v=121&o=-marketcap&r=41
-        
-        # Download all the tickers from Overview page (takes ~2.5 mins)
-        df = fl.scrape_all("https://finviz.com/screener.ashx?v=111&o=-marketcap", print_urls=True)
-        
-        # Save to csv
-        df.to_csv("all_tickers.csv", index=False)
-        
-        # Speed up scraping. By default scrape_all sleeps 0.1 seconds between requests. You can shorten(or lengthen it) by passing the sleep_interval=time_in_seconds to scrape_url to speed up or slow down scraping, but you may run into "Too many requests" errors from finviz.com if you set it too low and make too many requests in a short time.
-        >>>df = fl.scrape_all("https://finviz.com/screener.ashx?v=111&o=-marketcap", sleep_interval=0)
-        ValueError: too many requests while getting https://finviz.com/screener.ashx?v=111&o=-marketcap&r=241
-        
-        # If you want a list of the pagination urls for some reason, pass print_df_only=False to scrape()
-        >>> urls, df = fl.scrape("https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap", return_df_only=False)
-        >>> urls
-        ['https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=21', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=41', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=61', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=81', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=101', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=121', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=141', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=161', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=181', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=201', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=221', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=241', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=261', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=281']
-        ```
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: bs4
+Requires-Dist: lxml
+Requires-Dist: pandas
+
+# Finvizlite
+
+[![Build Status](https://travis-ci.org/andr3w321/finvizlite.svg?branch=main)](https://travis-ci.org/andr3w321/finvizlite)
+
+A lightweight finviz.com screener scraper for https://finviz.com/screener.ashx
+All the code is about 80 lines long and can be found in `finvizlite/__init__.py`
+
+
+## Install
+`pip install finvizlite`
+
+## Quick start
+
+```
+import finvizlite as fl
+
+# To scrape a single page use fl.scrape(url)
+df = fl.scrape("https://finviz.com/screener.ashx?v=141&o=-marketcap")
+
+# To scrape multiple pages use fl.scrape_all(url)
+# scrape the dow tickers
+df = fl.scrape_all("https://finviz.com/screener.ashx?v=141&f=idx_dji&o=-marketcap")
+
+# To print the scraped urls pass print_urls=True to scrape_all() or scrape()
+>>> df = fl.scrape_all("https://finviz.com/screener.ashx?v=161&f=idx_dji&o=-marketcap", print_urls=True)
+https://finviz.com/screener.ashx?v=161&f=idx_dji&o=-marketcap
+https://finviz.com/screener.ashx?v=161&f=idx_dji&o=-marketcap&r=21
+
+# To limit the amount of tickers scraped pass rows=max_rows to scrape_all
+>>> df = fl.scrape_all("https://finviz.com/screener.ashx?v=121&o=-marketcap", print_urls=True, rows=50)
+https://finviz.com/screener.ashx?v=121&o=-marketcap
+https://finviz.com/screener.ashx?v=121&o=-marketcap&r=21
+https://finviz.com/screener.ashx?v=121&o=-marketcap&r=41
+
+# Download all the tickers from Overview page (takes ~2.5 mins)
+df = fl.scrape_all("https://finviz.com/screener.ashx?v=111&o=-marketcap", print_urls=True)
+
+# Save to csv
+df.to_csv("all_tickers.csv", index=False)
+
+# Speed up scraping. By default scrape_all sleeps 0.1 seconds between requests. You can shorten(or lengthen it) by passing the sleep_interval=time_in_seconds to scrape_url to speed up or slow down scraping, but you may run into "Too many requests" errors from finviz.com if you set it too low and make too many requests in a short time.
+>>>df = fl.scrape_all("https://finviz.com/screener.ashx?v=111&o=-marketcap", sleep_interval=0)
+ValueError: too many requests while getting https://finviz.com/screener.ashx?v=111&o=-marketcap&r=241
+
+# If you want a list of the pagination urls for some reason, pass print_df_only=False to scrape()
+>>> urls, df = fl.scrape("https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap", return_df_only=False)
+>>> urls
+['https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=21', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=41', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=61', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=81', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=101', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=121', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=141', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=161', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=181', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=201', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=221', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=241', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=261', 'https://finviz.com/screener.ashx?v=111&f=sec_energy&o=-marketcap&r=281']
+```
```

### Comparing `finvizlite-0.1.1/setup.py` & `finvizlite-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 
 setup(name='finvizlite',
-      version='0.1.1',
+      version='0.1.2',
       description='A lightweight finviz screener scraper',
       long_description=README,
       long_description_content_type="text/markdown",
       url='https://github.com/andr3w321/finvizlite',
       author='Andrew Rennhack',
       author_email='andr3w321@gmail.com',
       license='MIT',
```

