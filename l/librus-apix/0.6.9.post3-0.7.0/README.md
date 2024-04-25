# Comparing `tmp/librus_apix-0.6.9.post3.tar.gz` & `tmp/librus_apix-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "librus_apix-0.6.9.post3.tar", last modified: Sun Mar 31 00:00:31 2024, max compression
+gzip compressed data, was "librus_apix-0.7.0.tar", last modified: Thu Apr 25 19:37:11 2024, max compression
```

## Comparing `librus_apix-0.6.9.post3.tar` & `librus_apix-0.7.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 00:00:31.220137 librus_apix-0.6.9.post3/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-03-31 00:00:29.000000 librus_apix-0.6.9.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-31 00:00:31.220137 librus_apix-0.6.9.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-03-31 00:00:29.000000 librus_apix-0.6.9.post3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 00:00:31.220137 librus_apix-0.6.9.post3/librus_apix/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-03-31 00:00:29.000000 librus_apix-0.6.9.post3/librus_apix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-03-31 00:00:29.000000 librus_apix-0.6.9.post3/librus_apix/announcements.py
--rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-03-31 00:00:29.000000 librus_apix-0.6.9.post3/librus_apix/attendance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-03-31 00:00:29.000000 librus_apix-0.6.9.post3/librus_apix/completed_lessons.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-03-31 00:00:29.000000 librus_apix-0.6.9.post3/librus_apix/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5859 2024-03-31 00:00:29.000000 librus_apix-0.6.9.post3/librus_apix/get_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     9541 2024-03-31 00:00:29.000000 librus_apix-0.6.9.post3/librus_apix/grades.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-03-31 00:00:29.000000 librus_apix-0.6.9.post3/librus_apix/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-03-31 00:00:29.000000 librus_apix-0.6.9.post3/librus_apix/homework.py
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-03-31 00:00:29.000000 librus_apix-0.6.9.post3/librus_apix/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-03-31 00:00:29.000000 librus_apix-0.6.9.post3/librus_apix/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-03-31 00:00:29.000000 librus_apix-0.6.9.post3/librus_apix/student_information.py
--rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-03-31 00:00:29.000000 librus_apix-0.6.9.post3/librus_apix/timetable.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-03-31 00:00:29.000000 librus_apix-0.6.9.post3/librus_apix/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 00:00:31.220137 librus_apix-0.6.9.post3/librus_apix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-31 00:00:31.000000 librus_apix-0.6.9.post3/librus_apix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-31 00:00:31.000000 librus_apix-0.6.9.post3/librus_apix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 00:00:31.000000 librus_apix-0.6.9.post3/librus_apix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-31 00:00:31.000000 librus_apix-0.6.9.post3/librus_apix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-31 00:00:31.000000 librus_apix-0.6.9.post3/librus_apix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-31 00:00:29.000000 librus_apix-0.6.9.post3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-03-31 00:00:31.224137 librus_apix-0.6.9.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 00:00:29.000000 librus_apix-0.6.9.post3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:37:11.615558 librus_apix-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-25 19:37:09.000000 librus_apix-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-25 19:37:11.615558 librus_apix-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-04-25 19:37:09.000000 librus_apix-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:37:11.611558 librus_apix-0.7.0/librus_apix/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-25 19:37:09.000000 librus_apix-0.7.0/librus_apix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-25 19:37:09.000000 librus_apix-0.7.0/librus_apix/announcements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-04-25 19:37:09.000000 librus_apix-0.7.0/librus_apix/attendance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-25 19:37:09.000000 librus_apix-0.7.0/librus_apix/completed_lessons.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-25 19:37:09.000000 librus_apix-0.7.0/librus_apix/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6233 2024-04-25 19:37:09.000000 librus_apix-0.7.0/librus_apix/get_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9541 2024-04-25 19:37:09.000000 librus_apix-0.7.0/librus_apix/grades.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-25 19:37:09.000000 librus_apix-0.7.0/librus_apix/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-04-25 19:37:09.000000 librus_apix-0.7.0/librus_apix/homework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-04-25 19:37:09.000000 librus_apix-0.7.0/librus_apix/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-04-25 19:37:09.000000 librus_apix-0.7.0/librus_apix/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-25 19:37:09.000000 librus_apix-0.7.0/librus_apix/student_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-04-25 19:37:09.000000 librus_apix-0.7.0/librus_apix/timetable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-25 19:37:09.000000 librus_apix-0.7.0/librus_apix/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 19:37:11.615558 librus_apix-0.7.0/librus_apix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-25 19:37:11.000000 librus_apix-0.7.0/librus_apix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-25 19:37:11.000000 librus_apix-0.7.0/librus_apix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 19:37:11.000000 librus_apix-0.7.0/librus_apix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-25 19:37:11.000000 librus_apix-0.7.0/librus_apix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 19:37:11.000000 librus_apix-0.7.0/librus_apix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-25 19:37:09.000000 librus_apix-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-25 19:37:11.615558 librus_apix-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 19:37:09.000000 librus_apix-0.7.0/setup.py
```

### Comparing `librus_apix-0.6.9.post3/LICENSE` & `librus_apix-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `librus_apix-0.6.9.post3/README.md` & `librus_apix-0.7.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+<p align="center">
+  <img src="https://github.com/RustySnek/librus-apix/blob/main/logo.png" alt="librus-apix logo"/>
+</p>
+
 # Librus Synergia web scraper.
 
 ## Installation
 
 ```sh
 pip install librus-apix
 ```
@@ -86,14 +90,33 @@
   print(h.lesson, h.completion_date)
   href = h.href
   details = homework_detail(token, href)
   print(details)
 
 ```
 
+### Sending Messages
+```py
+from librus_apix.messages import get_recipients, send_message
+
+recipients = get_recipients(token, "teachers")
+my_recipient = recipient_id["John Brown"]
+my_second_recipient = recipient_id["Barbara Brown"]
+sent = send_message(token,
+                   "Message Title",
+                   "Message\n content",
+                   "teachers",
+                   [my_recipient, my_second_recipient]
+)
+if sent == True:
+  print("Sent!")
+else:
+  print("Error sending a message!")
+```
+
 ### Getting the Messages
 ```py
 from librus_apix.messages import get_recieved, message_content
 
 messages = get_recieved(token, page=1)
 for message in messages:
   print(message.title)
@@ -138,18 +161,29 @@
 ```py
 from librus_apix.student_information import student_information
 
 info = student_information(token)
 print(info.lucky_number)
 ```
 
+### Adding a proxy
+```py
+# Proxy can be added with
+token = get_token(u, p, proxy={"https": "http://my-proxy.xyz"})
+# or
+token.proxy = {"https": "http://my-proxy.xyz"}
+# or
+token = Token(token_key, proxy={"https": "http://my-proxy.xyz"})
+```
+
 ## Working on the Project
 
 ```sh
 git clone https://github.com/RustySnek/librus-apix
 cd librus-apix
 python -m venv venv
 source ./venv/bin/activate
 pip install requirements.txt
 # Installing library with editable flag
+sed -i "s/{{VERSION_PLACEHOLDER}}/1.0.0-dev/g" setup.cfg
 pip install -e .
 ```
```

### Comparing `librus_apix-0.6.9.post3/librus_apix/announcements.py` & `librus_apix-0.7.0/librus_apix/announcements.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.6.9.post3/librus_apix/attendance.py` & `librus_apix-0.7.0/librus_apix/attendance.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,19 +63,19 @@
             a["Semester"]
             ) for a in attendances]
 
 def get_attendance_frequency(token: Token):
     attendance = get_gateway_attendance(token)
     first_semester = [a for a in attendance if a[2] == 1]
     second_semester = [a for a in attendance if a[2] == 2]
-    f_attended = len([a for a in first_semester if a[0][0] == "ob"])
-    s_attended = len([a for a in second_semester if a[0][0] == "ob"])
-    f_freq = f_attended / len(first_semester)
-    s_freq = s_attended / len(second_semester)
-    overall_freq = len([a for a in attendance if a[0][0] == "ob"]) / len(attendance)
+    f_attended = len([a for a in first_semester if a[0][0] in ["wy", "ob", "sp"]])
+    s_attended = len([a for a in second_semester if a[0][0] in ["wy", "ob", "sp"]])
+    f_freq = f_attended / len(first_semester) if len(second_semester) != 0 else 1
+    s_freq = s_attended / len(second_semester) if len(second_semester) != 0 else 1
+    overall_freq = len([a for a in attendance if a[0][0] in ["wy", "ob", "sp"]]) / len(attendance) if len(attendance) != 0 else 1
     return f_freq, s_freq, overall_freq
     # ADD Lesson frequency
 
 def get_attendance(token: Token, sort_by: str = "all") -> List[List[Attendance]]:
     SORT = {
         "all": {"zmiany_logowanie_wszystkie": ""},
         "week": {"zmiany_logowanie_tydzien": "zmiany_logowanie_tydzien"},
```

### Comparing `librus_apix-0.6.9.post3/librus_apix/completed_lessons.py` & `librus_apix-0.7.0/librus_apix/completed_lessons.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.6.9.post3/librus_apix/grades.py` & `librus_apix-0.7.0/librus_apix/grades.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.6.9.post3/librus_apix/homework.py` & `librus_apix-0.7.0/librus_apix/homework.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.6.9.post3/librus_apix/schedule.py` & `librus_apix-0.7.0/librus_apix/schedule.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from typing import Union, List, Dict
 
 
 @dataclass
 class Event:
     title: str
     subject: str
-    data: str
+    data: dict
     day: str
     number: Union[int, str]
     hour: str
     href: str
 
 
 def schedule_detail(token: Token, prefix: str, detail_url: str) -> Dict[str, str]:
@@ -30,31 +30,35 @@
         raise ParseError("Error in parsing schedule details.")
     tr = div.find_all("tr", attrs={"class": ["line0", "line1"]})
     for s in tr:
         schedule[s.find("th").text.strip()] = s.find("td").text.strip()
     return schedule
 
 
-def get_schedule(token: Token, month: str, year: str) -> Dict[int, List[Event]]:
+def get_schedule(token: Token, month: str, year: str, include_empty: bool = False) -> Dict[int, List[Event]]:
     schedule = defaultdict(list)
     soup = no_access_check(
         BeautifulSoup(
             token.post(token.SCHEDULE_URL, data={"rok": year, "miesiac": month}).text,
             "lxml",
         )
     )
     days = soup.find_all("div", attrs={"class": "kalendarz-dzien"})
     if len(days) < 1:
         raise ParseError("Error in parsing days of the schedule.")
     for day in days:
         d = day.find("div", attrs={"class": "kalendarz-numer-dnia"}).text
+        if include_empty == True:
+            schedule[int(d)] = []
         tr = day.find_all("tr")
         if tr:
             for event in tr:
                 td = event.find("td")
+                title = td.attrs.get("title", "Nauczyciel: unknown<br />Opis: unknown")
+                additional_data = {key: val for key, val in [pair.split(": ", 1) for pair in title.split("<br />")]}
                 subject = "unspecified"
                 span = td.find("span")
                 if span:
                     subject = span.text
                     span.extract()
 
                 delimeter = "###"
@@ -63,14 +67,16 @@
                 data = (
                     td.text.replace("\xa0", " ")
                     .replace(", ", "")
                     .replace("\n", "")
                     .strip()
                     .split(delimeter)
                 )
+                if subject == "unspecified":
+                    subject = data[0]
                 if len(data) >= 2:
                     title = data[1]
                 else:
                     title = data[0]
 
                 number = "unknown"
                 hour = "unknown"
@@ -88,10 +94,10 @@
                     pass
                 try:
                     onclick = event.find("td").attrs["onclick"]
                     href = "/".join(onclick.split("'")[1].split("/")[2:])
                 except KeyError:
                     href = ""
 
-                event = Event(title, subject, data, d, number, hour, href)
+                event = Event(title, subject, additional_data, d, number, hour, href)
                 schedule[int(d)].append(event)
     return schedule
```

### Comparing `librus_apix-0.6.9.post3/librus_apix/student_information.py` & `librus_apix-0.7.0/librus_apix/student_information.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.6.9.post3/librus_apix/timetable.py` & `librus_apix-0.7.0/librus_apix/timetable.py`

 * *Files identical despite different names*

### Comparing `librus_apix-0.6.9.post3/librus_apix/urls.py` & `librus_apix-0.7.0/librus_apix/urls.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 }
 BASE_URL = "https://synergia.librus.pl"
 API_URL = "https://api.librus.pl"
 GRADES_URL = BASE_URL + "/przegladaj_oceny/uczen"
 TIMETABLE_URL = f"{BASE_URL}/przegladaj_plan_lekcji"
 ANNOUNCEMENTS_URL = f"{BASE_URL}/ogloszenia"
 MESSAGE_URL = f"{BASE_URL}/wiadomosci/1/5"
+RECIPIENTS_URL = f"{BASE_URL}/getRecipients"
+SEND_MESSAGE_URL = f"{BASE_URL}/wiadomosci/1/6"
 ATTENDANCE_URL = f"{BASE_URL}/przegladaj_nb/uczen"
 ATTENDANCE_DETAILS_URL = f"{BASE_URL}/przegladaj_nb/szczegoly/"
 SCHEDULE_URL = f"{BASE_URL}/terminarz/"
 HOMEWORK_URL = f"{BASE_URL}/moje_zadania"
 HOMEWORK_DETAILS_URL = f"{BASE_URL}/moje_zadania/podglad/"
 INFO_URL = f"{BASE_URL}/informacja"
 COMPLETED_LESSONS_URL = f"{BASE_URL}/zrealizowane_lekcje"
```

### Comparing `librus_apix-0.6.9.post3/librus_apix.egg-info/SOURCES.txt` & `librus_apix-0.7.0/librus_apix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `librus_apix-0.6.9.post3/setup.cfg` & `librus_apix-0.7.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [darglint]
 strictness = long
 docstring_style = google
 
 [metadata]
 name = librus_apix
-version = 0.6.9-3
+version = 0.7.0
 license = MIT
 description = Web Scraper for Librus Synergia
 long_description = ""
 author = Pascal Jodłowski
 url = https://github.com/poroknights/librus-apix
 keywords = librus, scraper, api, synergia
 classifiers =
```

