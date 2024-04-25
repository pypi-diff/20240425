# Comparing `tmp/espn_scraper-0.14.9.tar.gz` & `tmp/espn_scraper-0.15.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/espn_scraper-0.14.9.tar", last modified: Fri Apr 21 23:10:44 2017, max compression
+gzip compressed data, was "espn_scraper-0.15.0.tar", last modified: Thu Apr 25 00:32:54 2024, max compression
```

## Comparing `espn_scraper-0.14.9.tar` & `espn_scraper-0.15.0.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxrwxr-x   0 dan       (1000) dan       (1000)        0 2017-04-21 23:10:44.000000 espn_scraper-0.14.9/
--rw-rw-r--   0 dan       (1000) dan       (1000)      108 2017-04-21 23:10:44.000000 espn_scraper-0.14.9/setup.cfg
-drwxrwxr-x   0 dan       (1000) dan       (1000)        0 2017-04-21 23:10:44.000000 espn_scraper-0.14.9/espn_scraper/
--rw-rw-r--   0 dan       (1000) dan       (1000)    17253 2017-04-21 23:09:17.000000 espn_scraper-0.14.9/espn_scraper/__init__.py
--rw-rw-r--   0 dan       (1000) dan       (1000)      258 2017-04-21 23:10:44.000000 espn_scraper-0.14.9/PKG-INFO
--rw-rw-r--   0 dan       (1000) dan       (1000)      538 2017-04-21 23:09:40.000000 espn_scraper-0.14.9/setup.py
-drwxrwxr-x   0 dan       (1000) dan       (1000)        0 2017-04-21 23:10:44.000000 espn_scraper-0.14.9/espn_scraper.egg-info/
--rw-rw-r--   0 dan       (1000) dan       (1000)       13 2017-04-21 23:10:43.000000 espn_scraper-0.14.9/espn_scraper.egg-info/top_level.txt
--rw-rw-r--   0 dan       (1000) dan       (1000)        1 2017-03-23 22:38:03.000000 espn_scraper-0.14.9/espn_scraper.egg-info/not-zip-safe
--rw-rw-r--   0 dan       (1000) dan       (1000)       39 2017-04-21 23:10:43.000000 espn_scraper-0.14.9/espn_scraper.egg-info/requires.txt
--rw-rw-r--   0 dan       (1000) dan       (1000)      258 2017-04-21 23:10:43.000000 espn_scraper-0.14.9/espn_scraper.egg-info/PKG-INFO
--rw-rw-r--   0 dan       (1000) dan       (1000)        1 2017-04-21 23:10:43.000000 espn_scraper-0.14.9/espn_scraper.egg-info/dependency_links.txt
--rw-rw-r--   0 dan       (1000) dan       (1000)      257 2017-04-21 23:10:43.000000 espn_scraper-0.14.9/espn_scraper.egg-info/SOURCES.txt
+drwxrwxr-x   0 bob       (1000) bob       (1000)        0 2024-04-25 00:32:54.358389 espn_scraper-0.15.0/
+-rw-rw-r--   0 bob       (1000) bob       (1000)     1078 2024-04-24 15:47:10.000000 espn_scraper-0.15.0/LICENSE
+-rw-r--r--   0 bob       (1000) bob       (1000)      355 2024-04-25 00:32:54.358389 espn_scraper-0.15.0/PKG-INFO
+-rw-rw-r--   0 bob       (1000) bob       (1000)    11760 2024-04-24 23:51:27.000000 espn_scraper-0.15.0/README.md
+drwxrwxr-x   0 bob       (1000) bob       (1000)        0 2024-04-25 00:32:54.358389 espn_scraper-0.15.0/espn_scraper/
+-rw-rw-r--   0 bob       (1000) bob       (1000)    18079 2024-04-24 23:35:46.000000 espn_scraper-0.15.0/espn_scraper/__init__.py
+drwxrwxr-x   0 bob       (1000) bob       (1000)        0 2024-04-25 00:32:54.358389 espn_scraper-0.15.0/espn_scraper.egg-info/
+-rw-r--r--   0 bob       (1000) bob       (1000)      355 2024-04-25 00:32:54.000000 espn_scraper-0.15.0/espn_scraper.egg-info/PKG-INFO
+-rw-rw-r--   0 bob       (1000) bob       (1000)      275 2024-04-25 00:32:54.000000 espn_scraper-0.15.0/espn_scraper.egg-info/SOURCES.txt
+-rw-rw-r--   0 bob       (1000) bob       (1000)        1 2024-04-25 00:32:54.000000 espn_scraper-0.15.0/espn_scraper.egg-info/dependency_links.txt
+-rw-rw-r--   0 bob       (1000) bob       (1000)        1 2024-04-24 15:47:37.000000 espn_scraper-0.15.0/espn_scraper.egg-info/not-zip-safe
+-rw-rw-r--   0 bob       (1000) bob       (1000)       39 2024-04-25 00:32:54.000000 espn_scraper-0.15.0/espn_scraper.egg-info/requires.txt
+-rw-rw-r--   0 bob       (1000) bob       (1000)       13 2024-04-25 00:32:54.000000 espn_scraper-0.15.0/espn_scraper.egg-info/top_level.txt
+-rw-rw-r--   0 bob       (1000) bob       (1000)      108 2024-04-25 00:32:54.358389 espn_scraper-0.15.0/setup.cfg
+-rw-rw-r--   0 bob       (1000) bob       (1000)      539 2024-04-25 00:32:22.000000 espn_scraper-0.15.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `espn_scraper-0.14.9/espn_scraper/__init__.py` & `espn_scraper-0.15.0/espn_scraper/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,50 +2,63 @@
 import pytz
 from dateutil import parser
 from dateutil.relativedelta import relativedelta
 import datetime
 import os.path
 import requests
 from bs4 import BeautifulSoup
-BASE_URL = "http://www.espn.com"
+BASE_URL = "https://www.espn.com"
+QUERY_STRING = "_xhr=1"
+#ESPN seems to be blocking requests with default blank headers
+DEFAULT_HEADERS = {"User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/107.0.0.0 Safari/537.36"}
+API_v2_BASE_URL = "https://site.api.espn.com/apis/site/v2/sports"
 
 ## General functions
-def retry_request(url):
+def retry_request(url, headers=DEFAULT_HEADERS):
     """Get a url and return the request, try it up to 3 times if it fails initially"""
     session = requests.Session()
     session.mount("http://", requests.adapters.HTTPAdapter(max_retries=3))
-    res = session.get(url=url, allow_redirects=False)
+    res = session.get(url=url, allow_redirects=True, headers=headers)
     session.close()
     return res
 
 def get_soup(res):
     return BeautifulSoup(res.text, "lxml")
 
-def get_new_json(url):
+def get_new_json(url, headers=DEFAULT_HEADERS):
     print(url)
-    res = retry_request(url)
+    res = retry_request(url, headers)
     if res.status_code == 200:
         return res.json()
     else:
-        print("ERROR: ESPN", res.status_code)
-        return {"error_code": res.status_code, "error_msg": "ESPN Error"}
+        print("ERROR:", res.status_code)
+        return {"error_code": res.status_code, "error_msg": "URL Error"}
 
-def get_new_html_soup(url):
+def get_new_html_soup(url, headers=DEFAULT_HEADERS):
     print(url)
-    res = retry_request(url)
+    res = retry_request(url, headers)
     if res.status_code == 200:
         return get_soup(res)
     else:
         print("ERROR: ESPN", res.status_code)
         return {"error_code": res.status_code, "error_msg": "ESPN Error"}
 
 ## Get constants
 def get_date_leagues():
     return ["mlb","nba","ncb","ncw","wnba","nhl"]
 
+def longify_league(league):
+    if league == "ncb":
+        league = "mens-college-basketball"
+    elif league == "ncw":
+        league = "womens-college-basketball"
+    elif league == "ncf":
+        league = "college-football"
+    return league
+
 def get_week_leagues():
     return ["nfl","ncf"]
 
 def get_ncb_groups():
     return [50,55,56,100]
 
 def get_ncw_groups():
@@ -54,17 +67,14 @@
 def get_ncf_groups():
     return [80,81]
 
 def get_leagues():
     """ Return a list of supported leagues """
     return get_week_leagues() + get_date_leagues()
 
-def get_html_boxscore_leagues():
-    return ["wnba", "mlb", "nhl"]
-
 def get_no_scoreboard_json_leagues():
     """ Scoreboard json isn't easily available for some leagues, have to grab the game_ids from sportscenter_api url """
     return ["wnba", "nhl"]
 
 def get_sport(league):
     if league in ["nba","wnba","ncb","ncw"]:
         return "basketball"
@@ -72,45 +82,58 @@
         return "baseball"
     elif league in ["nfl","ncf"]:
         return "football"
     elif league in ["nhl"]:
         return "hockey"
 
 ## Get urls
-def get_sportscenter_api_url(sport, league, dates):
-    return "http://sportscenter.api.espn.com/apis/v1/events?sport={}&league={}&dates={}".format(sport, league, dates)
-
-def get_date_scoreboard_url(league, date, group=None):
-    """ Return a scoreboard url for a league that uses dates (nonfootball)"""
-    if league in get_date_leagues():
-        if league == "nhl":
-            return "{}/{}/scoreboard?date={}".format(BASE_URL, league, date)
-        else:
-            if group == None:
-                return "{}/{}/scoreboard/_/date/{}?xhr=1".format(BASE_URL, league, date)
-            else:
-                return "{}/{}/scoreboard/_/group/{}/date/{}?xhr=1".format(BASE_URL, league, group, date)
-    else:
-        raise ValueError("League must be {} to get date scoreboard url".format(get_date_leagues()))
-
-def get_week_scoreboard_url(league, season_year, season_type, week, group=None):
-    """ Return a scoreboard url for a league that uses weeks (football)"""
-    if league in get_week_leagues():
-        if group == None:
-            return "{}/{}/scoreboard/_/year/{}/seasontype/{}/week/{}?xhr=1".format(BASE_URL, league, season_year, season_type, week)
-        else:
-            return "{}/{}/scoreboard/_/group/{}/year/{}/seasontype/{}/week/{}?xhr=1".format(BASE_URL, league, group, season_year, season_type, week)
-    else:
-        raise ValueError("League must be {} to get week scoreboard url".format(get_week_leagues()))
+def get_sportscenter_api_url(league, dates, sport=None):
+    """ Alternative API endpoint """
+    if sport == None:
+        sport = get_sport(league)
+    return "https://sportscenter.api.espn.com/apis/v1/events?sport={}&league={}&dates={}".format(sport, league, dates)
+
+def get_date_scoreboard_url(league, dates, groups=None, sport=None, limit=None):
+    """ Return a scoreboard url for a league that uses dates (nonfootball, but function also works for football)"""
+    if sport == None:
+        sport = get_sport(league)
+    league = longify_league(league)
+    url = "{}/{}/{}/scoreboard?dates={}".format(API_v2_BASE_URL, sport, league, dates)
+    if groups !=None:
+        if limit == None:
+            limit = 1000
+        url+= "&groups={}".format(groups)
+    if limit != None:
+        url += "&limit={}".format(limit)
+    return url
+
+def get_week_scoreboard_url(league, season_year, season_type=None, week=None, groups=None, sport=None):
+    """ Return a scoreboard url for a league that uses weeks (football)
+    Example urls
+    By year: https://site.api.espn.com/apis/site/v2/sports/football/nfl/scoreboard?limit=1000&dates=2022
+    By year, seasontype, week: https://site.api.espn.com/apis/site/v2/sports/football/nfl/scoreboard?dates=2022&seasontype=2&week=1
+    By date range: https://site.api.espn.com/apis/site/v2/sports/football/nfl/scoreboard?dates=20200901-20210228
+    By date: https://site.api.espn.com/apis/site/v2/sports/football/nfl/scoreboard?dates=20200901"""
+
+    if sport == None:
+        sport = get_sport(league)
+    league = longify_league(league)
+    url = "{}/{}/{}/scoreboard?dates={}".format(API_v2_BASE_URL, sport, league, season_year)
+    if season_type != None:
+        url += "&seasontype={}".format(season_type)
+    if week != None:
+        url += "&week={}".format(week)
+    #TODO implement groups?
+    return url
 
 def get_game_url(url_type, league, espn_id):
-    valid_url_types = ["summary", "recap", "boxscore", "playbyplay", "conversation", "gamecast"]
+    valid_url_types = ["recap", "boxscore", "playbyplay", "conversation", "gamecast"]
     if url_type not in valid_url_types:
         raise ValueError("Unknown url_type for get_game_url. Valid url_types are {}".format(valid_url_types))
-    return "{}/{}/{}?gameId={}&xhr=1".format(BASE_URL, league, url_type, espn_id)
+    return "{}/{}/{}?gameId={}&{}".format(BASE_URL, league, url_type, espn_id, QUERY_STRING)
 
 def get_current_scoreboard_urls(league, offset=0):
     """ Return a list of the current scoreboard urls for a league 
     For date leagues optional offset is in days
     For week leagues optional offseet is in weeks """
     urls = []
     if league in get_date_leagues():
@@ -186,15 +209,15 @@
         return url.split("?date=")[1].split("&")[0]
     else:
         return url.split('/')[-1].split('?')[0]
 
 def get_data_type_from_url(url):
     """ Guess and return the data_type based on the url """
     data_type = None
-    valid_data_types = ["scoreboard", "summary", "recap", "boxscore", "playbyplay", "conversation", "gamecast"]
+    valid_data_types = ["scoreboard", "recap", "boxscore", "playbyplay", "conversation", "gamecast"]
     for valid_data_type in valid_data_types:
         if valid_data_type in url:
             data_type = valid_data_type
             break
     if data_type == None:
         raise ValueError("Unknown data_type for url. Url must contain one of {}".format(valid_data_types))
     return data_type
@@ -226,32 +249,29 @@
         return datetime.datetime(season_year,4,20, tzinfo=pytz.timezone("US/Eastern")).astimezone(pytz.utc), datetime.datetime(season_year,10,31, tzinfo=pytz.timezone("US/Eastern")).astimezone(pytz.utc)
     elif league == "nhl":
         # hardcode nhl start end dates, assumed to be Oct 1 thru June 30
         return datetime.datetime(season_year-1,10,1, tzinfo=pytz.timezone("US/Eastern")).astimezone(pytz.utc), datetime.datetime(season_year,6,30, tzinfo=pytz.timezone("US/Eastern")).astimezone(pytz.utc)
     else:
         raise ValueError("League must be {} to get season start and end datetimes".format(get_date_leagues()))
 
-def create_filename_ext(league, data_type):
-    """ Get a filename extension (either .html or .json depending on league and data_type) """
-    if league in get_html_boxscore_leagues() and data_type != "scoreboard":
-        return "html"
-    else:
-        return "json"
-
 def get_filename(cached_json_path, league, data_type, url):
     """ Build a full filename with directories for given league, data_type and url"""
     # add slash if necessary to cached_json_path
     if cached_json_path[-1] != "/":
         cached_json_path += "/"
     dir_path = cached_json_path + "/" + league + "/" + data_type + "/"
     # create a league directory and data_type directory in cached_json if doesn't already exist
     if not os.path.exists(dir_path):
         os.makedirs(dir_path)
     # create filename with / replaced with |
-    return dir_path + url.replace('/','|') + "." + create_filename_ext(league, data_type)
+    filename = dir_path + url.replace('/','|')
+    ext = ".json"
+    if filename.endswith(ext) == False:
+        filename = filename + ext
+    return filename
 
 def get_cached(filename):
     """ Return cached json if it exists """
     data = None
     if os.path.isfile(filename):
         ext = get_filename_ext(filename)
         if ext == "json":
@@ -260,121 +280,122 @@
         elif ext == "html":
             data = BeautifulSoup(open(filename), "lxml") 
     return data
 
 ## Get requests
 def get_teams(league):
     """ Returns a list of teams with ids and names """
-    url = BASE_URL + "/" + league + "/teams"
-    print(url)
-    soup = get_soup(retry_request(url))
-    if league == "wnba":
-        selector = "b a"
-    else:
-        selector = "a.bi"
-    team_links = soup.select(selector)
     teams = []
-    for team_link in team_links:
-        teams.append({'id': team_link['href'].split('/')[-2], 'name': team_link.text})
+    if league == "ncf":
+        # espn's college football teams page only lists fbs (blank division)
+        # need to grab teams from standings page instead if want all the fbs and fcs teams
+        for division in ["","fcs-i-aa"]:
+            url = BASE_URL + "/college-football/standings/_/view/" + division
+            print(url)
+            soup = get_soup(retry_request(url))
+            selector = ".hide-mobile"
+            team_divs = soup.select(selector)
+            for team_div in team_divs:
+                teams.append({'id': team_div.find("a")['href'].split('/')[-2], 'name': team_div.text})
+    else:
+        url = BASE_URL + "/" + league + "/teams"
+        print(url)
+        soup = get_soup(retry_request(url))
+        if league == "wnba":
+            selector = "div.pl3"
+        else:
+            selector = "div.mt3"
+        team_divs = soup.select(selector)
+        for team_div in team_divs:
+            teams.append({'id': team_div.find("a")['href'].split('/')[-2], 'name': team_div.find("h2").text})
     return teams
 
-def get_standings(league, season_year):
+def get_standings(league, season_year, college_division=None):
     standings = {"conferences": {}}
-    if league in ["wnba","nhl"]:
-        url = "{}/{}/standings/_/year/{}".format(BASE_URL, league, season_year)
-        print(url)
-        soup = get_soup(retry_request(url))
-        standings = {"conferences": {}}
-        # espn has malformed html where they forgot to include closing </table> tags so have to parse by table rows instead of by tables
-        trs = soup.find_all("tr", class_=["stathead","colhead","oddrow","evenrow"])
-        for tr in trs:
-            if "stathead" in tr["class"]:
-                conference_name = tr.text
-                standings["conferences"][conference_name] = {"divisions": {}}
-            elif "colhead" in tr["class"]:
-                division = tr.find("td").text
-                standings["conferences"][conference_name]["divisions"][division] = {"teams": []}
-            elif "oddrow" in tr["class"] or "evenrow" in tr["class"]:
-                team_a_tag = tr.find("td").find("a")
-                team = {}
-                team["name"] = team_a_tag.text
-                team["abbr"] = team_a_tag["href"].split("name/")[1].split("/")[0].upper()
-                standings["conferences"][conference_name]["divisions"][division]["teams"].append(team)
-    elif league in ["ncb","ncw"]:
-        url = "{}/{}/standings/_/year/{}".format(BASE_URL, league, season_year)
+    if league in ["nhl","nfl","mlb","nba","wnba","ncf","ncb","ncw"]:
+        if league == "ncf" and college_division == None:
+            # default to fbs
+            college_division = ""
+        if college_division:
+            valid_college_divisions = ["fbs", "fcs", "fcs-i-aa", "d2", "d3"]
+            if college_division == "fcs":
+                college_division = "fcs-i-aa"
+            if college_division in valid_college_divisions:
+                url = "{}/{}/standings/_/season/{}/view/{}".format(BASE_URL, league, season_year, college_division)
+            else:
+                raise ValueError("College division must be none or {}".format(",".join(valid_college_divisions)))
+        elif league in ["wnba"]:
+            url = "{}/{}/standings/_/season/{}/group/conference".format(BASE_URL, league, season_year)
+        else:
+            url = "{}/{}/standings/_/season/{}/group/division".format(BASE_URL, league, season_year)
+
         print(url)
         soup = get_soup(retry_request(url))
-        standings = {"conferences": {}}
-        conference_name = "i"
-        standings["conferences"][conference_name] = {"divisions": {}}
-        divs = soup.find_all("div", class_="mod-table")
-        for div in divs:
-            division = div.find("div", class_="mod-header").find("h4").text.split("Standings")[0]
-            standings["conferences"][conference_name]["divisions"][division] = {"teams": []}
-            trs = div.find("div", class_="mod-content").find("table", class_="tablehead").find_all("tr", class_=["oddrow","evenrow"])
+        standings_divs = soup.find_all("div", class_="standings__table")
+
+        for i in range(len(standings_divs)):
+            conference_name = standings_divs[i].find("div", class_="Table__Title").text
+            standings["conferences"][conference_name] = {"divisions": {}}
+            division = "" # default blank division name
+            teams_table = standings_divs[i].find("table", class_="Table--fixed-left")
+            trs = teams_table.find_all("tr")
             for tr in trs:
-                for c in tr["class"]:
-                    if "team" in c:
-                        team_a_tag = tr.find("td").find("a")
-                        team = {}
-                        team["name"] = team_a_tag.text
-                        team["id"] = int(c.split("-")[2])
-                        standings["conferences"][conference_name]["divisions"][division]["teams"].append(team)
-    elif league in ["nfl","ncf","nba","mlb"]:
-        url = "{}/{}/standings/_/season/{}/group/division".format(BASE_URL, league, season_year)
-        print(url)
-        soup = get_soup(retry_request(url))
-        conference_names = [x.text for x in soup.find_all("span", class_="long-caption")]
-        tables = soup.find_all("table", class_="standings")
-        for i in range(0, len(tables)):
-            standings["conferences"][conference_names[i]] = {"divisions": {}}
-            theads = tables[i].find_all("thead", class_="standings-categories")
-            for thead in theads:
-                division = thead.find("th").text
-                standings["conferences"][conference_names[i]]["divisions"][division] = {"teams": []}
-                nextSib = thead.nextSibling
-                while(nextSib and nextSib.name == "tr"):
-                    link = nextSib.find("abbr")
+                if "subgroup-headers" in tr["class"]:
+                    division = tr.text # replace default blank division name
+                    standings["conferences"][conference_name]["divisions"][division] = {"teams": []}
+                elif tr.text != "":
+                    if division == "" and standings["conferences"][conference_name]["divisions"] == {}:
+                        standings["conferences"][conference_name]["divisions"][division] = {"teams": []}
                     team = {}
-                    team["name"] = link["title"]
-                    team["abbr"] = link.text
-                    standings["conferences"][conference_names[i]]["divisions"][division]["teams"].append(team)
-                    nextSib = nextSib.nextSibling
+                    team_span_tag = tr.find("td", class_="Table__TD").find("span", class_="hide-mobile")
+                    team_a_tag = team_span_tag.find("a")
+                    if team_a_tag is None:
+                        # some teams are now defunct with no espn links
+                        team["name"] = team_span_tag.text.strip()
+                        team["abbr"] = ""
+                    else:
+                        team["name"] = team_a_tag.text
+                        if league in ["ncf","ncb","ncw"]:
+                            team["abbr"] = team_a_tag["href"].split("/id/")[1].split("/")[0].upper()
+                        else:
+                            team["abbr"] = team_a_tag["href"].split("/name/")[1].split("/")[0].upper()
+                    standings["conferences"][conference_name]["divisions"][division]["teams"].append(team)
+
     return standings
                 
 def get_calendar(league, date_or_season_year):
     """ Return a calendar for a league and season_year"""
     if league in get_week_leagues():
         url = get_week_scoreboard_url(league, date_or_season_year, 2, 1)
     elif league in get_date_leagues():
         url = get_date_scoreboard_url(league, date_or_season_year)
     # TODO use cached replies for older urls
-    return get_url(url)['content']['calendar']
+    return get_url(url)['leagues'][0]['calendar']
 
 def get_url(url, cached_path=None):
     """ Retrieve an ESPN JSON data or HTML BeautifulSoup, either from cache or make new request """
     data_type = get_data_type_from_url(url)
     league = get_league_from_url(url)
+    """
     if data_type == "scoreboard":
         # for wnba and nhl we'll use a different api to retrieve game_ids and basic game data
         if league in get_no_scoreboard_json_leagues():
             url = get_sportscenter_api_url(get_sport(league), league, get_date_from_scoreboard_url(url))
+    """
+    return get_cached_url(url, league, data_type, cached_path)
+
+def get_cached_url(url, league, data_type, cached_path, headers=DEFAULT_HEADERS):
+    """ get_url helper if want to specify the league and datatype (for non espn.com links) """
     if cached_path:
         filename = get_filename(cached_path, league, data_type, url)
         data = get_cached(filename)
     else:
         data = None
     if data == None:
-        ext = create_filename_ext(league, data_type)
-        if ext == "json":
-            data = get_new_json(url)
-            # dont cache if got an ESPN internal 500 error
-            if cached_path and "error_code" not in data:
-                with open(filename, 'w') as f:
-                    json.dump(data, f, ensure_ascii=False, indent=2, sort_keys=True)
-        elif ext == "html":
-            data = get_new_html_soup(url)
-            if cached_path and "error_code" not in data:
-                with open(filename, 'w') as f:
-                    f.write(data.prettify())
+        ext = "json"
+        data = get_new_json(url, headers)
+        # dont cache if got an ESPN internal 500 error
+        if cached_path and "error_code" not in data:
+            with open(filename, 'w') as f:
+                json.dump(data, f, ensure_ascii=False, indent=2, sort_keys=True)
     return data
```

### Comparing `espn_scraper-0.14.9/setup.py` & `espn_scraper-0.15.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 setup(name='espn_scraper',
-      version='0.14.9',
+      version='0.15.00',
       description='ESPN scraper for major sports',
       url='http://github.com/andr3w321/espn_scraper',
       author='Andrew Rennhack',
       author_email='andr3w321@gmail.com',
       license='MIT',
       install_requires=[
           'pytz',
```

