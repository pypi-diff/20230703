# Comparing `tmp/dry_scraper-0.1.4.tar.gz` & `tmp/dry_scraper-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dry_scraper-0.1.4.tar", max compression
+gzip compressed data, was "dry_scraper-0.1.5.tar", max compression
```

## Comparing `dry_scraper-0.1.4.tar` & `dry_scraper-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0    35149 2022-12-05 04:14:04.570059 dry_scraper-0.1.4/LICENSE
--rw-r--r--   0        0        0       50 2022-12-05 04:14:04.570059 dry_scraper-0.1.4/README.md
--rw-r--r--   0        0        0      547 2023-05-14 23:37:10.035820 dry_scraper-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2704 2023-05-14 23:33:44.497300 dry_scraper-0.1.4/src/dry_scraper/data_sources/data_source.py
--rw-r--r--   0        0        0       87 2023-05-14 23:33:44.497300 dry_scraper-0.1.4/src/dry_scraper/data_sources/nhl/__init__.py
--rw-r--r--   0        0        0    14305 2023-05-14 23:33:44.497300 dry_scraper-0.1.4/src/dry_scraper/data_sources/nhl/nhl_api_sources.py
--rw-r--r--   0        0        0      490 2023-01-14 00:52:26.603584 dry_scraper-0.1.4/src/dry_scraper/data_sources/nhl/pydantic_models/nhl_conferences_api_source.py
--rw-r--r--   0        0        0      848 2023-01-14 00:54:47.040256 dry_scraper-0.1.4/src/dry_scraper/data_sources/nhl/pydantic_models/nhl_divisions_api_source.py
--rw-r--r--   0        0        0     5323 2023-01-14 00:54:44.046922 dry_scraper-0.1.4/src/dry_scraper/data_sources/nhl/pydantic_models/nhl_game_content_api_source.py
--rw-r--r--   0        0        0    11296 2023-05-14 23:33:35.187214 dry_scraper-0.1.4/src/dry_scraper/data_sources/nhl/pydantic_models/nhl_game_live_feed_api_source.py
--rw-r--r--   0        0        0     1558 2023-01-14 00:54:44.046922 dry_scraper-0.1.4/src/dry_scraper/data_sources/nhl/pydantic_models/nhl_people_api_source.py
--rw-r--r--   0        0        0     1938 2023-05-14 23:33:35.187214 dry_scraper-0.1.4/src/dry_scraper/data_sources/nhl/pydantic_models/nhl_schedule_api_source.py
--rw-r--r--   0        0        0     1830 2023-01-14 00:52:26.603584 dry_scraper-0.1.4/src/dry_scraper/data_sources/nhl/pydantic_models/nhl_teams_api_source.py
--rw-r--r--   0        0        0    20946 2022-12-05 04:14:04.570059 dry_scraper-0.1.4/src/dry_scraper/shared.py
--rw-r--r--   0        0        0    35587 2022-12-05 04:14:04.570059 dry_scraper-0.1.4/src/dry_scraper/teams.py
--rw-r--r--   0        0        0      781 1970-01-01 00:00:00.000000 dry_scraper-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-12-05 04:14:04.570059 dry_scraper-0.1.5/LICENSE
+-rw-r--r--   0        0        0      646 2023-07-03 00:56:12.057381 dry_scraper-0.1.5/README.md
+-rw-r--r--   0        0        0      546 2023-07-01 23:34:52.916761 dry_scraper-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-30 22:46:11.776545 dry_scraper-0.1.5/src/dry_scraper/__init__.py
+-rw-r--r--   0        0        0     2444 2023-06-30 23:14:23.236239 dry_scraper-0.1.5/src/dry_scraper/data_source.py
+-rw-r--r--   0        0        0        0 2023-06-30 22:46:11.776545 dry_scraper-0.1.5/src/dry_scraper/nhl/__init__.py
+-rw-r--r--   0        0        0    26088 2023-07-03 00:36:30.136173 dry_scraper-0.1.5/src/dry_scraper/nhl/nhl_api_sources.py
+-rw-r--r--   0        0        0      490 2023-01-14 00:52:26.603584 dry_scraper-0.1.5/src/dry_scraper/nhl/pydantic_models/nhl_conferences_api_source.py
+-rw-r--r--   0        0        0      835 2023-07-02 23:21:46.796568 dry_scraper-0.1.5/src/dry_scraper/nhl/pydantic_models/nhl_divisions_api_source.py
+-rw-r--r--   0        0        0     5323 2023-01-14 00:54:44.046922 dry_scraper-0.1.5/src/dry_scraper/nhl/pydantic_models/nhl_game_content_api_source.py
+-rw-r--r--   0        0        0    11711 2023-07-02 23:21:46.793235 dry_scraper-0.1.5/src/dry_scraper/nhl/pydantic_models/nhl_game_live_feed_api_source.py
+-rw-r--r--   0        0        0     1555 2023-07-02 23:22:31.266974 dry_scraper-0.1.5/src/dry_scraper/nhl/pydantic_models/nhl_people_api_source.py
+-rw-r--r--   0        0        0     1912 2023-07-02 23:22:31.260307 dry_scraper-0.1.5/src/dry_scraper/nhl/pydantic_models/nhl_schedule_api_source.py
+-rw-r--r--   0        0        0     1804 2023-07-02 23:22:31.280308 dry_scraper-0.1.5/src/dry_scraper/nhl/pydantic_models/nhl_teams_api_source.py
+-rw-r--r--   0        0        0    20946 2022-12-05 04:14:04.570059 dry_scraper-0.1.5/src/dry_scraper/shared.py
+-rw-r--r--   0        0        0    30682 2023-07-02 23:22:46.757115 dry_scraper-0.1.5/src/dry_scraper/teams.py
+-rw-r--r--   0        0        0     1377 1970-01-01 00:00:00.000000 dry_scraper-0.1.5/PKG-INFO
```

### Comparing `dry_scraper-0.1.4/LICENSE` & `dry_scraper-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.4/src/dry_scraper/data_sources/data_source.py` & `dry_scraper-0.1.5/src/dry_scraper/data_source.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,20 +18,14 @@
     _url : str
         fully qualified URL location of data source, completed on instantiation
     _url_stub : ClassVar[str]
         partial URL location of data source
     _extension : ClassVar[str]
         file extension to be used when writing the raw data source to disk e.g. json, HTM
 
-    Methods
-    -------
-    fetch_content():# -> Self:
-        fetch content from self.url and store response in self.content
-    write_content():# -> Self:
-        write self.content to path and extension specified by the object
     """
 
     _content: str
     _url: str
     _url_stub: ClassVar[str]
     _extension: ClassVar[str]
 
@@ -57,18 +51,15 @@
 
     @property
     def extension(self) -> str:
         return self._extension
 
     def fetch_content(self) -> Self:
         """
-        Use requests.get to retrieve file at URL and store response in self.content
-
-        Returns:
-            self
+        Use requests.get to retrieve file at self.url and store response in self.content
         """
         try:
             response = requests.get(self.url, timeout=10)
             response.raise_for_status()
             self.content = response.text
         except requests.exceptions.HTTPError as errh:
             print(errh)
```

### Comparing `dry_scraper-0.1.4/src/dry_scraper/data_sources/nhl/pydantic_models/nhl_divisions_api_source.py` & `dry_scraper-0.1.5/src/dry_scraper/nhl/pydantic_models/nhl_divisions_api_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List, Optional, Literal
 
 from pydantic import BaseModel, Field, constr
 
-from dry_scraper.data_sources.nhl.pydantic_models.nhl_conferences_api_source import (
+from dry_scraper.nhl.pydantic_models.nhl_conferences_api_source import (
     ShortConference,
 )
 
 DivisionLink = constr(regex=r"^/api/v1/divisions/(\d+|null)$")
 
 
 class ShortDivision(BaseModel):
```

### Comparing `dry_scraper-0.1.4/src/dry_scraper/data_sources/nhl/pydantic_models/nhl_game_content_api_source.py` & `dry_scraper-0.1.5/src/dry_scraper/nhl/pydantic_models/nhl_game_content_api_source.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.4/src/dry_scraper/data_sources/nhl/pydantic_models/nhl_game_live_feed_api_source.py` & `dry_scraper-0.1.5/src/dry_scraper/nhl/pydantic_models/nhl_game_live_feed_api_source.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from datetime import datetime
 from pydantic import BaseModel, Field, constr
 from typing import List, Dict, Optional, Union
 
-from dry_scraper.data_sources.nhl.pydantic_models.nhl_people_api_source import (
+
+from dry_scraper.nhl.pydantic_models.nhl_people_api_source import (
     PersonIdString,
     PersonLink,
     Position,
     Player,
     Person,
 )
-from dry_scraper.data_sources.nhl.pydantic_models.nhl_teams_api_source import (
+from dry_scraper.nhl.pydantic_models.nhl_teams_api_source import (
     Team,
     ShortTeam,
     ShortVenue,
 )
 
 LiveFeedLink = constr(regex=r"^/api/v1/game/\d{10}/feed/live$")
 
@@ -211,15 +212,15 @@
     team_skater_stats: TeamSkaterStats = Field(alias="teamSkaterStats")
 
 
 class PlayerStatsPerson(BaseModel):
     id: PersonIdString
     full_name: str = Field(alias="fullName")
     link: constr(regex=r"^/api/v1/people/\d+$")
-    shoots_catches: str = Field(alias="shootsCatches")
+    shoots_catches: Optional[str] = Field(alias="shootsCatches")
     roster_status: str = Field(alias="rosterStatus")
 
 
 class GoalieStats(BaseModel):
     time_on_ice: str = Field(alias="timeOnIce")
     assists: int
     goals: int
@@ -386,7 +387,26 @@
     "player3_full_name": "str",
     "player3_player_type": "str",
     "player3_season_total": "int",
     "team_id": "int",
     "team_name": "str",
     "team_tricode": "str",
 }
+
+team_stats_df_model = {
+    "season": "int",
+    "gamePk": "int",
+    "team_id": "int",
+    "team_name": "str",
+    "home": "bool",
+    "goals": "int",
+    "pim": "int",
+    "shots": "int",
+    "power_play_percentage": "float",
+    "power_play_goals": "int",
+    "power_play_opportunities": "int",
+    "face_off_win_percentage": "float",
+    "blocked": "int",
+    "takeaways": "int",
+    "giveaways": "int",
+    "hits": "int",
+}
```

### Comparing `dry_scraper-0.1.4/src/dry_scraper/data_sources/nhl/pydantic_models/nhl_people_api_source.py` & `dry_scraper-0.1.5/src/dry_scraper/nhl/pydantic_models/nhl_people_api_source.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import date
 from typing import List, Optional
 
 from pydantic import BaseModel, constr, Field
 
-from dry_scraper.data_sources.nhl.pydantic_models.nhl_teams_api_source import ShortTeam
+from dry_scraper.nhl.pydantic_models.nhl_teams_api_source import ShortTeam
 
 PersonIdString = constr(regex=r"^(ID)?\d{4,7}$")
 
 
 PersonLink = constr(regex=r"^/api/v1/people/(\d+|null)$")
 
 
@@ -33,15 +33,15 @@
     nationality: str
     height: str
     weight: int
     active: bool
     alternate_captain: Optional[bool] = Field(alias="alternateCaptain")
     captain: Optional[bool]
     rookie: bool
-    shoots_catches: str = Field(alias="shootsCatches")
+    shoots_catches: Optional[str] = Field(alias="shootsCatches")
     roster_status: str = Field(alias="rosterStatus")
     current_team: Optional[ShortTeam] = Field(alias="currentTeam")
     primary_position: Position = Field(alias="primaryPosition")
 
 
 class Person(BaseModel):
     id: Optional[PersonIdString]
```

### Comparing `dry_scraper-0.1.4/src/dry_scraper/data_sources/nhl/pydantic_models/nhl_schedule_api_source.py` & `dry_scraper-0.1.5/src/dry_scraper/nhl/pydantic_models/nhl_schedule_api_source.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import datetime
 from typing import List, Optional
 
 from pydantic import BaseModel, Field
 
-from dry_scraper.data_sources.nhl.pydantic_models.nhl_game_live_feed_api_source import (
+from dry_scraper.nhl.pydantic_models.nhl_game_live_feed_api_source import (
     LiveFeedLink,
     Status,
 )
-from dry_scraper.data_sources.nhl.pydantic_models.nhl_teams_api_source import (
+from dry_scraper.nhl.pydantic_models.nhl_teams_api_source import (
     ShortTeam,
     ShortVenue,
 )
 
 
 class LeagueRecord(BaseModel):
     wins: int
```

### Comparing `dry_scraper-0.1.4/src/dry_scraper/data_sources/nhl/pydantic_models/nhl_teams_api_source.py` & `dry_scraper-0.1.5/src/dry_scraper/nhl/pydantic_models/nhl_teams_api_source.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Optional, List
 
 from pydantic import BaseModel, constr, Field, HttpUrl
 
-from dry_scraper.data_sources.nhl.pydantic_models.nhl_conferences_api_source import (
+from dry_scraper.nhl.pydantic_models.nhl_conferences_api_source import (
     ShortConference,
 )
-from dry_scraper.data_sources.nhl.pydantic_models.nhl_divisions_api_source import (
+from dry_scraper.nhl.pydantic_models.nhl_divisions_api_source import (
     NullDivision,
     ShortDivision,
 )
 
 VenueLink = constr(regex=r"^/api/v1/venues/(\d+|null)$")
 
 FranchiseLink = constr(regex=r"^/api/v1/franchises/(\d+|null)$")
```

### Comparing `dry_scraper-0.1.4/src/dry_scraper/shared.py` & `dry_scraper-0.1.5/src/dry_scraper/shared.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.4/src/dry_scraper/teams.py` & `dry_scraper-0.1.5/src/dry_scraper/teams.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,1258 +1,867 @@
+# noinspection DuplicatedCode
 TEAMS = {
     "ANA": {
         "abbreviation": "ANA",
         "active": True,
-        "conference": {
-            "id": 5,
-            "link": "/api/v1/conferences/5",
-            "name": "Western"
-        },
-        "division": {
-            "id": 15,
-            "link": "/api/v1/divisions/15",
-            "name": "Pacific"
-        },
+        "conference": {"id": 5, "link": "/api/v1/conferences/5", "name": "Western"},
+        "division": {"id": 15, "link": "/api/v1/divisions/15", "name": "Pacific"},
         "firstYearOfPlay": "1993",
         "franchise": {
             "franchiseId": 32,
             "link": "/api/v1/franchises/32",
-            "teamName": "Ducks"
+            "teamName": "Ducks",
         },
         "franchiseId": 32,
         "id": 24,
         "link": "/api/v1/teams/24",
         "locationName": "Anaheim",
         "name": "Anaheim Ducks",
         "officialSiteUrl": "http://www.anaheimducks.com",
         "shortName": "Anaheim",
         "teamName": "Ducks",
         "venue": {
             "city": "Anaheim",
             "link": "/api/v1/venues/null",
             "name": "Honda Center",
-            "timeZone": {
-                "id": "America/Los_Angeles",
-                "offset": -8,
-                "tz": "PST"
-            }
-        }
+            "timeZone": {"id": "America/Los_Angeles", "offset": -8, "tz": "PST"},
+        },
     },
     "ARI": {
         "abbreviation": "ARI",
         "active": True,
-        "conference": {
-            "id": 5,
-            "link": "/api/v1/conferences/5",
-            "name": "Western"
-        },
-        "division": {
-            "id": 15,
-            "link": "/api/v1/divisions/15",
-            "name": "Pacific"
-        },
+        "conference": {"id": 5, "link": "/api/v1/conferences/5", "name": "Western"},
+        "division": {"id": 15, "link": "/api/v1/divisions/15", "name": "Pacific"},
         "firstYearOfPlay": "1979",
         "franchise": {
             "franchiseId": 28,
             "link": "/api/v1/franchises/28",
-            "teamName": "Coyotes"
+            "teamName": "Coyotes",
         },
         "franchiseId": 28,
         "id": 53,
         "link": "/api/v1/teams/53",
         "locationName": "Arizona",
         "name": "Arizona Coyotes",
         "officialSiteUrl": "http://www.arizonacoyotes.com",
         "shortName": "Arizona",
         "teamName": "Coyotes",
         "venue": {
             "city": "Glendale",
             "link": "/api/v1/venues/null",
             "name": "Gila River Arena",
-            "timeZone": {
-                "id": "America/Phoenix",
-                "offset": -7,
-                "tz": "MST"
-            }
-        }
+            "timeZone": {"id": "America/Phoenix", "offset": -7, "tz": "MST"},
+        },
     },
     "BOS": {
         "abbreviation": "BOS",
         "active": True,
-        "conference": {
-            "id": 6,
-            "link": "/api/v1/conferences/6",
-            "name": "Eastern"
-        },
-        "division": {
-            "id": 17,
-            "link": "/api/v1/divisions/17",
-            "name": "Atlantic"
-        },
+        "conference": {"id": 6, "link": "/api/v1/conferences/6", "name": "Eastern"},
+        "division": {"id": 17, "link": "/api/v1/divisions/17", "name": "Atlantic"},
         "firstYearOfPlay": "1924",
         "franchise": {
             "franchiseId": 6,
             "link": "/api/v1/franchises/6",
-            "teamName": "Bruins"
+            "teamName": "Bruins",
         },
         "franchiseId": 6,
         "id": 6,
         "link": "/api/v1/teams/6",
         "locationName": "Boston",
         "name": "Boston Bruins",
         "officialSiteUrl": "http://www.bostonbruins.com",
         "shortName": "Boston",
         "teamName": "Bruins",
         "venue": {
             "city": "Boston",
             "link": "/api/v1/venues/null",
             "name": "TD Garden",
-            "timeZone": {
-                "id": "America/New_York",
-                "offset": -5,
-                "tz": "EST"
-            }
-        }
+            "timeZone": {"id": "America/New_York", "offset": -5, "tz": "EST"},
+        },
     },
     "BUF": {
         "abbreviation": "BUF",
         "active": True,
-        "conference": {
-            "id": 6,
-            "link": "/api/v1/conferences/6",
-            "name": "Eastern"
-        },
-        "division": {
-            "id": 17,
-            "link": "/api/v1/divisions/17",
-            "name": "Atlantic"
-        },
+        "conference": {"id": 6, "link": "/api/v1/conferences/6", "name": "Eastern"},
+        "division": {"id": 17, "link": "/api/v1/divisions/17", "name": "Atlantic"},
         "firstYearOfPlay": "1970",
         "franchise": {
             "franchiseId": 19,
             "link": "/api/v1/franchises/19",
-            "teamName": "Sabres"
+            "teamName": "Sabres",
         },
         "franchiseId": 19,
         "id": 7,
         "link": "/api/v1/teams/7",
         "locationName": "Buffalo",
         "name": "Buffalo Sabres",
         "officialSiteUrl": "http://www.sabres.com",
         "shortName": "Buffalo",
         "teamName": "Sabres",
         "venue": {
             "city": "Buffalo",
             "link": "/api/v1/venues/null",
             "name": "KeyBank Center",
-            "timeZone": {
-                "id": "America/New_York",
-                "offset": -5,
-                "tz": "EST"
-            }
-        }
+            "timeZone": {"id": "America/New_York", "offset": -5, "tz": "EST"},
+        },
     },
     "CAR": {
         "abbreviation": "CAR",
         "active": True,
-        "conference": {
-            "id": 6,
-            "link": "/api/v1/conferences/6",
-            "name": "Eastern"
-        },
-        "division": {
-            "id": 18,
-            "link": "/api/v1/divisions/18",
-            "name": "Metropolitan"
-        },
+        "conference": {"id": 6, "link": "/api/v1/conferences/6", "name": "Eastern"},
+        "division": {"id": 18, "link": "/api/v1/divisions/18", "name": "Metropolitan"},
         "firstYearOfPlay": "1979",
         "franchise": {
             "franchiseId": 26,
             "link": "/api/v1/franchises/26",
-            "teamName": "Hurricanes"
+            "teamName": "Hurricanes",
         },
         "franchiseId": 26,
         "id": 12,
         "link": "/api/v1/teams/12",
         "locationName": "Carolina",
         "name": "Carolina Hurricanes",
         "officialSiteUrl": "http://www.carolinahurricanes.com",
         "shortName": "Carolina",
         "teamName": "Hurricanes",
         "venue": {
             "city": "Raleigh",
             "link": "/api/v1/venues/null",
             "name": "PNC Arena",
-            "timeZone": {
-                "id": "America/New_York",
-                "offset": -5,
-                "tz": "EST"
-            }
-        }
+            "timeZone": {"id": "America/New_York", "offset": -5, "tz": "EST"},
+        },
     },
     "CBJ": {
         "abbreviation": "CBJ",
         "active": True,
-        "conference": {
-            "id": 6,
-            "link": "/api/v1/conferences/6",
-            "name": "Eastern"
-        },
-        "division": {
-            "id": 18,
-            "link": "/api/v1/divisions/18",
-            "name": "Metropolitan"
-        },
+        "conference": {"id": 6, "link": "/api/v1/conferences/6", "name": "Eastern"},
+        "division": {"id": 18, "link": "/api/v1/divisions/18", "name": "Metropolitan"},
         "firstYearOfPlay": "1997",
         "franchise": {
             "franchiseId": 36,
             "link": "/api/v1/franchises/36",
-            "teamName": "Blue Jackets"
+            "teamName": "Blue Jackets",
         },
         "franchiseId": 36,
         "id": 29,
         "link": "/api/v1/teams/29",
         "locationName": "Columbus",
         "name": "Columbus Blue Jackets",
         "officialSiteUrl": "http://www.bluejackets.com",
         "shortName": "Columbus",
         "teamName": "Blue Jackets",
         "venue": {
             "city": "Columbus",
             "link": "/api/v1/venues/null",
             "name": "Nationwide Arena",
-            "timeZone": {
-                "id": "America/New_York",
-                "offset": -5,
-                "tz": "EST"
-            }
-        }
+            "timeZone": {"id": "America/New_York", "offset": -5, "tz": "EST"},
+        },
     },
     "CGY": {
         "abbreviation": "CGY",
         "active": True,
-        "conference": {
-            "id": 5,
-            "link": "/api/v1/conferences/5",
-            "name": "Western"
-        },
-        "division": {
-            "id": 15,
-            "link": "/api/v1/divisions/15",
-            "name": "Pacific"
-        },
+        "conference": {"id": 5, "link": "/api/v1/conferences/5", "name": "Western"},
+        "division": {"id": 15, "link": "/api/v1/divisions/15", "name": "Pacific"},
         "firstYearOfPlay": "1980",
         "franchise": {
             "franchiseId": 21,
             "link": "/api/v1/franchises/21",
-            "teamName": "Flames"
+            "teamName": "Flames",
         },
         "franchiseId": 21,
         "id": 20,
         "link": "/api/v1/teams/20",
         "locationName": "Calgary",
         "name": "Calgary Flames",
         "officialSiteUrl": "http://www.calgaryflames.com",
         "shortName": "Calgary",
         "teamName": "Flames",
         "venue": {
             "city": "Calgary",
             "link": "/api/v1/venues/null",
             "name": "Scotiabank Saddledome",
-            "timeZone": {
-                "id": "America/Denver",
-                "offset": -7,
-                "tz": "MST"
-            }
-        }
+            "timeZone": {"id": "America/Denver", "offset": -7, "tz": "MST"},
+        },
     },
     "CHI": {
         "abbreviation": "CHI",
         "active": True,
-        "conference": {
-            "id": 5,
-            "link": "/api/v1/conferences/5",
-            "name": "Western"
-        },
-        "division": {
-            "id": 16,
-            "link": "/api/v1/divisions/16",
-            "name": "Central"
-        },
+        "conference": {"id": 5, "link": "/api/v1/conferences/5", "name": "Western"},
+        "division": {"id": 16, "link": "/api/v1/divisions/16", "name": "Central"},
         "firstYearOfPlay": "1926",
         "franchise": {
             "franchiseId": 11,
             "link": "/api/v1/franchises/11",
-            "teamName": "Blackhawks"
+            "teamName": "Blackhawks",
         },
         "franchiseId": 11,
         "id": 16,
         "link": "/api/v1/teams/16",
         "locationName": "Chicago",
         "name": "Chicago Blackhawks",
         "officialSiteUrl": "http://www.chicagoblackhawks.com",
         "shortName": "Chicago",
         "teamName": "Blackhawks",
         "venue": {
             "city": "Chicago",
             "link": "/api/v1/venues/null",
             "name": "United Center",
-            "timeZone": {
-                "id": "America/Chicago",
-                "offset": -6,
-                "tz": "CST"
-            }
-        }
+            "timeZone": {"id": "America/Chicago", "offset": -6, "tz": "CST"},
+        },
     },
     "COL": {
         "abbreviation": "COL",
         "active": True,
-        "conference": {
-            "id": 5,
-            "link": "/api/v1/conferences/5",
-            "name": "Western"
-        },
-        "division": {
-            "id": 16,
-            "link": "/api/v1/divisions/16",
-            "name": "Central"
-        },
+        "conference": {"id": 5, "link": "/api/v1/conferences/5", "name": "Western"},
+        "division": {"id": 16, "link": "/api/v1/divisions/16", "name": "Central"},
         "firstYearOfPlay": "1979",
         "franchise": {
             "franchiseId": 27,
             "link": "/api/v1/franchises/27",
-            "teamName": "Avalanche"
+            "teamName": "Avalanche",
         },
         "franchiseId": 27,
         "id": 21,
         "link": "/api/v1/teams/21",
         "locationName": "Colorado",
         "name": "Colorado Avalanche",
         "officialSiteUrl": "http://www.coloradoavalanche.com",
         "shortName": "Colorado",
         "teamName": "Avalanche",
         "venue": {
             "city": "Denver",
             "link": "/api/v1/venues/null",
             "name": "Pepsi Center",
-            "timeZone": {
-                "id": "America/Denver",
-                "offset": -7,
-                "tz": "MST"
-            }
-        }
+            "timeZone": {"id": "America/Denver", "offset": -7, "tz": "MST"},
+        },
     },
     "DAL": {
         "abbreviation": "DAL",
         "active": True,
-        "conference": {
-            "id": 5,
-            "link": "/api/v1/conferences/5",
-            "name": "Western"
-        },
-        "division": {
-            "id": 16,
-            "link": "/api/v1/divisions/16",
-            "name": "Central"
-        },
+        "conference": {"id": 5, "link": "/api/v1/conferences/5", "name": "Western"},
+        "division": {"id": 16, "link": "/api/v1/divisions/16", "name": "Central"},
         "firstYearOfPlay": "1967",
         "franchise": {
             "franchiseId": 15,
             "link": "/api/v1/franchises/15",
-            "teamName": "Stars"
+            "teamName": "Stars",
         },
         "franchiseId": 15,
         "id": 25,
         "link": "/api/v1/teams/25",
         "locationName": "Dallas",
         "name": "Dallas Stars",
         "officialSiteUrl": "http://www.dallasstars.com",
         "shortName": "Dallas",
         "teamName": "Stars",
         "venue": {
             "city": "Dallas",
             "link": "/api/v1/venues/null",
             "name": "American Airlines Center",
-            "timeZone": {
-                "id": "America/Chicago",
-                "offset": -6,
-                "tz": "CST"
-            }
-        }
+            "timeZone": {"id": "America/Chicago", "offset": -6, "tz": "CST"},
+        },
     },
     "DET": {
         "abbreviation": "DET",
         "active": True,
-        "conference": {
-            "id": 6,
-            "link": "/api/v1/conferences/6",
-            "name": "Eastern"
-        },
-        "division": {
-            "id": 17,
-            "link": "/api/v1/divisions/17",
-            "name": "Atlantic"
-        },
+        "conference": {"id": 6, "link": "/api/v1/conferences/6", "name": "Eastern"},
+        "division": {"id": 17, "link": "/api/v1/divisions/17", "name": "Atlantic"},
         "firstYearOfPlay": "1926",
         "franchise": {
             "franchiseId": 12,
             "link": "/api/v1/franchises/12",
-            "teamName": "Red Wings"
+            "teamName": "Red Wings",
         },
         "franchiseId": 12,
         "id": 17,
         "link": "/api/v1/teams/17",
         "locationName": "Detroit",
         "name": "Detroit Red Wings",
         "officialSiteUrl": "http://www.detroitredwings.com",
         "shortName": "Detroit",
         "teamName": "Red Wings",
         "venue": {
             "city": "Detroit",
             "link": "/api/v1/venues/null",
             "name": "Little Caesars Arena",
-            "timeZone": {
-                "id": "America/Detroit",
-                "offset": -5,
-                "tz": "EST"
-            }
-        }
+            "timeZone": {"id": "America/Detroit", "offset": -5, "tz": "EST"},
+        },
     },
     "EDM": {
         "abbreviation": "EDM",
         "active": True,
-        "conference": {
-            "id": 5,
-            "link": "/api/v1/conferences/5",
-            "name": "Western"
-        },
-        "division": {
-            "id": 15,
-            "link": "/api/v1/divisions/15",
-            "name": "Pacific"
-        },
+        "conference": {"id": 5, "link": "/api/v1/conferences/5", "name": "Western"},
+        "division": {"id": 15, "link": "/api/v1/divisions/15", "name": "Pacific"},
         "firstYearOfPlay": "1979",
         "franchise": {
             "franchiseId": 25,
             "link": "/api/v1/franchises/25",
-            "teamName": "Oilers"
+            "teamName": "Oilers",
         },
         "franchiseId": 25,
         "id": 22,
         "link": "/api/v1/teams/22",
         "locationName": "Edmonton",
         "name": "Edmonton Oilers",
         "officialSiteUrl": "http://www.edmontonoilers.com",
         "shortName": "Edmonton",
         "teamName": "Oilers",
         "venue": {
             "city": "Edmonton",
             "link": "/api/v1/venues/null",
             "name": "Rogers Place",
-            "timeZone": {
-                "id": "America/Edmonton",
-                "offset": -7,
-                "tz": "MST"
-            }
-        }
+            "timeZone": {"id": "America/Edmonton", "offset": -7, "tz": "MST"},
+        },
     },
     "FLA": {
         "abbreviation": "FLA",
         "active": True,
-        "conference": {
-            "id": 6,
-            "link": "/api/v1/conferences/6",
-            "name": "Eastern"
-        },
-        "division": {
-            "id": 17,
-            "link": "/api/v1/divisions/17",
-            "name": "Atlantic"
-        },
+        "conference": {"id": 6, "link": "/api/v1/conferences/6", "name": "Eastern"},
+        "division": {"id": 17, "link": "/api/v1/divisions/17", "name": "Atlantic"},
         "firstYearOfPlay": "1993",
         "franchise": {
             "franchiseId": 33,
             "link": "/api/v1/franchises/33",
-            "teamName": "Panthers"
+            "teamName": "Panthers",
         },
         "franchiseId": 33,
         "id": 13,
         "link": "/api/v1/teams/13",
         "locationName": "Florida",
         "name": "Florida Panthers",
         "officialSiteUrl": "http://www.floridapanthers.com",
         "shortName": "Florida",
         "teamName": "Panthers",
         "venue": {
             "city": "Sunrise",
             "link": "/api/v1/venues/null",
             "name": "BB&T Center",
-            "timeZone": {
-                "id": "America/New_York",
-                "offset": -5,
-                "tz": "EST"
-            }
-        }
+            "timeZone": {"id": "America/New_York", "offset": -5, "tz": "EST"},
+        },
     },
     "LAK": {
         "abbreviation": "LAK",
         "active": True,
-        "conference": {
-            "id": 5,
-            "link": "/api/v1/conferences/5",
-            "name": "Western"
-        },
-        "division": {
-            "id": 15,
-            "link": "/api/v1/divisions/15",
-            "name": "Pacific"
-        },
+        "conference": {"id": 5, "link": "/api/v1/conferences/5", "name": "Western"},
+        "division": {"id": 15, "link": "/api/v1/divisions/15", "name": "Pacific"},
         "firstYearOfPlay": "1967",
         "franchise": {
             "franchiseId": 14,
             "link": "/api/v1/franchises/14",
-            "teamName": "Kings"
+            "teamName": "Kings",
         },
         "franchiseId": 14,
         "id": 26,
         "link": "/api/v1/teams/26",
         "locationName": "Los Angeles",
         "name": "Los Angeles Kings",
         "officialSiteUrl": "http://www.lakings.com",
         "shortName": "Los Angeles",
         "teamName": "Kings",
         "venue": {
             "city": "Los Angeles",
             "link": "/api/v1/venues/null",
             "name": "STAPLES Center",
-            "timeZone": {
-                "id": "America/Los_Angeles",
-                "offset": -8,
-                "tz": "PST"
-            }
-        }
+            "timeZone": {"id": "America/Los_Angeles", "offset": -8, "tz": "PST"},
+        },
     },
     "MIN": {
         "abbreviation": "MIN",
         "active": True,
-        "conference": {
-            "id": 5,
-            "link": "/api/v1/conferences/5",
-            "name": "Western"
-        },
-        "division": {
-            "id": 16,
-            "link": "/api/v1/divisions/16",
-            "name": "Central"
-        },
+        "conference": {"id": 5, "link": "/api/v1/conferences/5", "name": "Western"},
+        "division": {"id": 16, "link": "/api/v1/divisions/16", "name": "Central"},
         "firstYearOfPlay": "1997",
         "franchise": {
             "franchiseId": 37,
             "link": "/api/v1/franchises/37",
-            "teamName": "Wild"
+            "teamName": "Wild",
         },
         "franchiseId": 37,
         "id": 30,
         "link": "/api/v1/teams/30",
         "locationName": "Minnesota",
         "name": "Minnesota Wild",
         "officialSiteUrl": "http://www.wild.com",
         "shortName": "Minnesota",
         "teamName": "Wild",
         "venue": {
             "city": "St. Paul",
             "link": "/api/v1/venues/null",
             "name": "Xcel Energy Center",
-            "timeZone": {
-                "id": "America/Chicago",
-                "offset": -6,
-                "tz": "CST"
-            }
-        }
+            "timeZone": {"id": "America/Chicago", "offset": -6, "tz": "CST"},
+        },
     },
     "MTL": {
         "abbreviation": "MTL",
         "active": True,
-        "conference": {
-            "id": 6,
-            "link": "/api/v1/conferences/6",
-            "name": "Eastern"
-        },
-        "division": {
-            "id": 17,
-            "link": "/api/v1/divisions/17",
-            "name": "Atlantic"
-        },
+        "conference": {"id": 6, "link": "/api/v1/conferences/6", "name": "Eastern"},
+        "division": {"id": 17, "link": "/api/v1/divisions/17", "name": "Atlantic"},
         "firstYearOfPlay": "1909",
         "franchise": {
             "franchiseId": 1,
             "link": "/api/v1/franchises/1",
-            "teamName": "Canadiens"
+            "teamName": "Canadiens",
         },
         "franchiseId": 1,
         "id": 8,
         "link": "/api/v1/teams/8",
         "locationName": "Montr\u00e9al",
         "name": "Montr\u00e9al Canadiens",
         "officialSiteUrl": "http://www.canadiens.com",
         "shortName": "Montr\u00e9al",
         "teamName": "Canadiens",
         "venue": {
             "city": "Montreal",
             "link": "/api/v1/venues/null",
             "name": "Centre Bell",
-            "timeZone": {
-                "id": "America/Montreal",
-                "offset": -5,
-                "tz": "EST"
-            }
-        }
+            "timeZone": {"id": "America/Montreal", "offset": -5, "tz": "EST"},
+        },
     },
     "NJD": {
         "abbreviation": "NJD",
         "active": True,
-        "conference": {
-            "id": 6,
-            "link": "/api/v1/conferences/6",
-            "name": "Eastern"
-        },
-        "division": {
-            "id": 18,
-            "link": "/api/v1/divisions/18",
-            "name": "Metropolitan"
-        },
+        "conference": {"id": 6, "link": "/api/v1/conferences/6", "name": "Eastern"},
+        "division": {"id": 18, "link": "/api/v1/divisions/18", "name": "Metropolitan"},
         "firstYearOfPlay": "1982",
         "franchise": {
             "franchiseId": 23,
             "link": "/api/v1/franchises/23",
-            "teamName": "Devils"
+            "teamName": "Devils",
         },
         "franchiseId": 23,
         "id": 1,
         "link": "/api/v1/teams/1",
         "locationName": "New Jersey",
         "name": "New Jersey Devils",
         "officialSiteUrl": "http://www.Truesince82.com",
         "shortName": "New Jersey",
         "teamName": "Devils",
         "venue": {
             "city": "Newark",
             "link": "/api/v1/venues/null",
             "name": "Prudential Center",
-            "timeZone": {
-                "id": "America/New_York",
-                "offset": -5,
-                "tz": "EST"
-            }
-        }
+            "timeZone": {"id": "America/New_York", "offset": -5, "tz": "EST"},
+        },
     },
     "NSH": {
         "abbreviation": "NSH",
         "active": True,
-        "conference": {
-            "id": 5,
-            "link": "/api/v1/conferences/5",
-            "name": "Western"
-        },
-        "division": {
-            "id": 16,
-            "link": "/api/v1/divisions/16",
-            "name": "Central"
-        },
+        "conference": {"id": 5, "link": "/api/v1/conferences/5", "name": "Western"},
+        "division": {"id": 16, "link": "/api/v1/divisions/16", "name": "Central"},
         "firstYearOfPlay": "1997",
         "franchise": {
             "franchiseId": 34,
             "link": "/api/v1/franchises/34",
-            "teamName": "Predators"
+            "teamName": "Predators",
         },
         "franchiseId": 34,
         "id": 18,
         "link": "/api/v1/teams/18",
         "locationName": "Nashville",
         "name": "Nashville Predators",
         "officialSiteUrl": "http://www.nashvillepredators.com",
         "shortName": "Nashville",
         "teamName": "Predators",
         "venue": {
             "city": "Nashville",
             "link": "/api/v1/venues/null",
             "name": "Bridgestone Arena",
-            "timeZone": {
-                "id": "America/Chicago",
-                "offset": -6,
-                "tz": "CST"
-            }
-        }
+            "timeZone": {"id": "America/Chicago", "offset": -6, "tz": "CST"},
+        },
     },
     "NYI": {
         "abbreviation": "NYI",
         "active": True,
-        "conference": {
-            "id": 6,
-            "link": "/api/v1/conferences/6",
-            "name": "Eastern"
-        },
-        "division": {
-            "id": 18,
-            "link": "/api/v1/divisions/18",
-            "name": "Metropolitan"
-        },
+        "conference": {"id": 6, "link": "/api/v1/conferences/6", "name": "Eastern"},
+        "division": {"id": 18, "link": "/api/v1/divisions/18", "name": "Metropolitan"},
         "firstYearOfPlay": "1972",
         "franchise": {
             "franchiseId": 22,
             "link": "/api/v1/franchises/22",
-            "teamName": "Islanders"
+            "teamName": "Islanders",
         },
         "franchiseId": 22,
         "id": 2,
         "link": "/api/v1/teams/2",
         "locationName": "New York",
         "name": "New York Islanders",
         "officialSiteUrl": "http://www.newyorkislanders.com",
         "shortName": "NY Islanders",
         "teamName": "Islanders",
         "venue": {
             "city": "Brooklyn",
             "link": "/api/v1/venues/null",
             "name": "Barclays Center",
-            "timeZone": {
-                "id": "America/New_York",
-                "offset": -5,
-                "tz": "EST"
-            }
-        }
+            "timeZone": {"id": "America/New_York", "offset": -5, "tz": "EST"},
+        },
     },
     "NYR": {
         "abbreviation": "NYR",
         "active": True,
-        "conference": {
-            "id": 6,
-            "link": "/api/v1/conferences/6",
-            "name": "Eastern"
-        },
-        "division": {
-            "id": 18,
-            "link": "/api/v1/divisions/18",
-            "name": "Metropolitan"
-        },
+        "conference": {"id": 6, "link": "/api/v1/conferences/6", "name": "Eastern"},
+        "division": {"id": 18, "link": "/api/v1/divisions/18", "name": "Metropolitan"},
         "firstYearOfPlay": "1926",
         "franchise": {
             "franchiseId": 10,
             "link": "/api/v1/franchises/10",
-            "teamName": "Rangers"
+            "teamName": "Rangers",
         },
         "franchiseId": 10,
         "id": 3,
         "link": "/api/v1/teams/3",
         "locationName": "New York",
         "name": "New York Rangers",
         "officialSiteUrl": "http://www.newyorkrangers.com",
         "shortName": "NY Rangers",
         "teamName": "Rangers",
         "venue": {
             "city": "New York",
             "link": "/api/v1/venues/null",
             "name": "Madison Square Garden",
-            "timeZone": {
-                "id": "America/New_York",
-                "offset": -5,
-                "tz": "EST"
-            }
-        }
+            "timeZone": {"id": "America/New_York", "offset": -5, "tz": "EST"},
+        },
     },
     "OTT": {
         "abbreviation": "OTT",
         "active": True,
-        "conference": {
-            "id": 6,
-            "link": "/api/v1/conferences/6",
-            "name": "Eastern"
-        },
-        "division": {
-            "id": 17,
-            "link": "/api/v1/divisions/17",
-            "name": "Atlantic"
-        },
+        "conference": {"id": 6, "link": "/api/v1/conferences/6", "name": "Eastern"},
+        "division": {"id": 17, "link": "/api/v1/divisions/17", "name": "Atlantic"},
         "firstYearOfPlay": "1990",
         "franchise": {
             "franchiseId": 30,
             "link": "/api/v1/franchises/30",
-            "teamName": "Senators"
+            "teamName": "Senators",
         },
         "franchiseId": 30,
         "id": 9,
         "link": "/api/v1/teams/9",
         "locationName": "Ottawa",
         "name": "Ottawa Senators",
         "officialSiteUrl": "http://www.ottawasenators.com",
         "shortName": "Ottawa",
         "teamName": "Senators",
         "venue": {
             "city": "Ottawa",
             "link": "/api/v1/venues/null",
             "name": "Canadian Tire Centre",
-            "timeZone": {
-                "id": "America/New_York",
-                "offset": -5,
-                "tz": "EST"
-            }
-        }
+            "timeZone": {"id": "America/New_York", "offset": -5, "tz": "EST"},
+        },
     },
     "PHI": {
         "abbreviation": "PHI",
         "active": True,
-        "conference": {
-            "id": 6,
-            "link": "/api/v1/conferences/6",
-            "name": "Eastern"
-        },
-        "division": {
-            "id": 18,
-            "link": "/api/v1/divisions/18",
-            "name": "Metropolitan"
-        },
+        "conference": {"id": 6, "link": "/api/v1/conferences/6", "name": "Eastern"},
+        "division": {"id": 18, "link": "/api/v1/divisions/18", "name": "Metropolitan"},
         "firstYearOfPlay": "1967",
         "franchise": {
             "franchiseId": 16,
             "link": "/api/v1/franchises/16",
-            "teamName": "Flyers"
+            "teamName": "Flyers",
         },
         "franchiseId": 16,
         "id": 4,
         "link": "/api/v1/teams/4",
         "locationName": "Philadelphia",
         "name": "Philadelphia Flyers",
         "officialSiteUrl": "http://www.philadelphiaflyers.com",
         "shortName": "Philadelphia",
         "teamName": "Flyers",
         "venue": {
             "city": "Philadelphia",
             "link": "/api/v1/venues/null",
             "name": "Wells Fargo Center",
-            "timeZone": {
-                "id": "America/New_York",
-                "offset": -5,
-                "tz": "EST"
-            }
-        }
+            "timeZone": {"id": "America/New_York", "offset": -5, "tz": "EST"},
+        },
     },
     "PHX": {
         "abbreviation": "ARI",
         "active": True,
-        "conference": {
-            "id": 5,
-            "link": "/api/v1/conferences/5",
-            "name": "Western"
-        },
-        "division": {
-            "id": 15,
-            "link": "/api/v1/divisions/15",
-            "name": "Pacific"
-        },
+        "conference": {"id": 5, "link": "/api/v1/conferences/5", "name": "Western"},
+        "division": {"id": 15, "link": "/api/v1/divisions/15", "name": "Pacific"},
         "firstYearOfPlay": "1979",
         "franchise": {
             "franchiseId": 28,
             "link": "/api/v1/franchises/28",
-            "teamName": "Coyotes"
+            "teamName": "Coyotes",
         },
         "franchiseId": 28,
         "id": 53,
         "link": "/api/v1/teams/53",
         "locationName": "Arizona",
         "name": "Arizona Coyotes",
         "officialSiteUrl": "http://www.arizonacoyotes.com",
         "shortName": "Arizona",
         "teamName": "Coyotes",
         "venue": {
             "city": "Glendale",
             "link": "/api/v1/venues/null",
             "name": "Gila River Arena",
-            "timeZone": {
-                "id": "America/Phoenix",
-                "offset": -7,
-                "tz": "MST"
-            }
-        }
+            "timeZone": {"id": "America/Phoenix", "offset": -7, "tz": "MST"},
+        },
     },
     "PIT": {
         "abbreviation": "PIT",
         "active": True,
-        "conference": {
-            "id": 6,
-            "link": "/api/v1/conferences/6",
-            "name": "Eastern"
-        },
-        "division": {
-            "id": 18,
-            "link": "/api/v1/divisions/18",
-            "name": "Metropolitan"
-        },
+        "conference": {"id": 6, "link": "/api/v1/conferences/6", "name": "Eastern"},
+        "division": {"id": 18, "link": "/api/v1/divisions/18", "name": "Metropolitan"},
         "firstYearOfPlay": "1967",
         "franchise": {
             "franchiseId": 17,
             "link": "/api/v1/franchises/17",
-            "teamName": "Penguins"
+            "teamName": "Penguins",
         },
         "franchiseId": 17,
         "id": 5,
         "link": "/api/v1/teams/5",
         "locationName": "Pittsburgh",
         "name": "Pittsburgh Penguins",
         "officialSiteUrl": "http://www.pittsburghpenguins.com",
         "shortName": "Pittsburgh",
         "teamName": "Penguins",
         "venue": {
             "city": "Pittsburgh",
             "link": "/api/v1/venues/null",
             "name": "PPG Paints Arena",
-            "timeZone": {
-                "id": "America/New_York",
-                "offset": -5,
-                "tz": "EST"
-            }
-        }
+            "timeZone": {"id": "America/New_York", "offset": -5, "tz": "EST"},
+        },
     },
     "SEA": {
         "id": 55,
         "name": "Seattle Kraken",
         "link": "/api/v1/teams/55",
         "venue": {
             "name": "Climate Pledge Arena",
             "link": "/api/v1/venues/null",
             "city": "Seattle",
-            "timeZone": {
-                "id": "America/Los_Angeles",
-                "offset": -7,
-                "tz": "PDT"
-            }
+            "timeZone": {"id": "America/Los_Angeles", "offset": -7, "tz": "PDT"},
         },
         "abbreviation": "SEA",
         "teamName": "Kraken",
         "locationName": "Seattle",
         "firstYearOfPlay": "2021",
         "division": {
             "id": 15,
             "name": "Pacific",
             "nameShort": "PAC",
             "link": "/api/v1/divisions/15",
-            "abbreviation": "P"
-        },
-        "conference": {
-            "id": 5,
-            "name": "Western",
-            "link": "/api/v1/conferences/5"
+            "abbreviation": "P",
         },
+        "conference": {"id": 5, "name": "Western", "link": "/api/v1/conferences/5"},
         "franchise": {
             "franchiseId": 39,
             "teamName": "Kraken",
-            "link": "/api/v1/franchises/39"
+            "link": "/api/v1/franchises/39",
         },
         "shortName": "Seattle",
         "officialSiteUrl": "https://www.nhl.com/seattle",
         "franchiseId": 39,
-        "active": True
+        "active": True,
     },
     "SJS": {
         "abbreviation": "SJS",
         "active": True,
-        "conference": {
-            "id": 5,
-            "link": "/api/v1/conferences/5",
-            "name": "Western"
-        },
-        "division": {
-            "id": 15,
-            "link": "/api/v1/divisions/15",
-            "name": "Pacific"
-        },
+        "conference": {"id": 5, "link": "/api/v1/conferences/5", "name": "Western"},
+        "division": {"id": 15, "link": "/api/v1/divisions/15", "name": "Pacific"},
         "firstYearOfPlay": "1990",
         "franchise": {
             "franchiseId": 29,
             "link": "/api/v1/franchises/29",
-            "teamName": "Sharks"
+            "teamName": "Sharks",
         },
         "franchiseId": 29,
         "id": 28,
         "link": "/api/v1/teams/28",
         "locationName": "San Jose",
         "name": "San Jose Sharks",
         "officialSiteUrl": "http://www.sjsharks.com",
         "shortName": "San Jose",
         "teamName": "Sharks",
         "venue": {
             "city": "San Jose",
             "link": "/api/v1/venues/null",
             "name": "SAP Center at San Jose",
-            "timeZone": {
-                "id": "America/Los_Angeles",
-                "offset": -8,
-                "tz": "PST"
-            }
-        }
+            "timeZone": {"id": "America/Los_Angeles", "offset": -8, "tz": "PST"},
+        },
     },
     "STL": {
         "abbreviation": "STL",
         "active": True,
-        "conference": {
-            "id": 5,
-            "link": "/api/v1/conferences/5",
-            "name": "Western"
-        },
-        "division": {
-            "id": 16,
-            "link": "/api/v1/divisions/16",
-            "name": "Central"
-        },
+        "conference": {"id": 5, "link": "/api/v1/conferences/5", "name": "Western"},
+        "division": {"id": 16, "link": "/api/v1/divisions/16", "name": "Central"},
         "firstYearOfPlay": "1967",
         "franchise": {
             "franchiseId": 18,
             "link": "/api/v1/franchises/18",
-            "teamName": "Blues"
+            "teamName": "Blues",
         },
         "franchiseId": 18,
         "id": 19,
         "link": "/api/v1/teams/19",
         "locationName": "St. Louis",
         "name": "St. Louis Blues",
         "officialSiteUrl": "http://www.stlouisblues.com",
         "shortName": "St Louis",
         "teamName": "Blues",
         "venue": {
             "city": "St. Louis",
             "link": "/api/v1/venues/null",
             "name": "Scottrade Center",
-            "timeZone": {
-                "id": "America/Chicago",
-                "offset": -6,
-                "tz": "CST"
-            }
-        }
+            "timeZone": {"id": "America/Chicago", "offset": -6, "tz": "CST"},
+        },
     },
     "TBL": {
         "abbreviation": "TBL",
         "active": True,
-        "conference": {
-            "id": 6,
-            "link": "/api/v1/conferences/6",
-            "name": "Eastern"
-        },
-        "division": {
-            "id": 17,
-            "link": "/api/v1/divisions/17",
-            "name": "Atlantic"
-        },
+        "conference": {"id": 6, "link": "/api/v1/conferences/6", "name": "Eastern"},
+        "division": {"id": 17, "link": "/api/v1/divisions/17", "name": "Atlantic"},
         "firstYearOfPlay": "1991",
         "franchise": {
             "franchiseId": 31,
             "link": "/api/v1/franchises/31",
-            "teamName": "Lightning"
+            "teamName": "Lightning",
         },
         "franchiseId": 31,
         "id": 14,
         "link": "/api/v1/teams/14",
         "locationName": "Tampa Bay",
         "name": "Tampa Bay Lightning",
         "officialSiteUrl": "http://www.tampabaylightning.com",
         "shortName": "Tampa Bay",
         "teamName": "Lightning",
         "venue": {
             "city": "Tampa",
             "link": "/api/v1/venues/null",
             "name": "Amalie Arena",
-            "timeZone": {
-                "id": "America/New_York",
-                "offset": -5,
-                "tz": "EST"
-            }
-        }
+            "timeZone": {"id": "America/New_York", "offset": -5, "tz": "EST"},
+        },
     },
     "TOR": {
         "abbreviation": "TOR",
         "active": True,
-        "conference": {
-            "id": 6,
-            "link": "/api/v1/conferences/6",
-            "name": "Eastern"
-        },
-        "division": {
-            "id": 17,
-            "link": "/api/v1/divisions/17",
-            "name": "Atlantic"
-        },
+        "conference": {"id": 6, "link": "/api/v1/conferences/6", "name": "Eastern"},
+        "division": {"id": 17, "link": "/api/v1/divisions/17", "name": "Atlantic"},
         "firstYearOfPlay": "1917",
         "franchise": {
             "franchiseId": 5,
             "link": "/api/v1/franchises/5",
-            "teamName": "Maple Leafs"
+            "teamName": "Maple Leafs",
         },
         "franchiseId": 5,
         "id": 10,
         "link": "/api/v1/teams/10",
         "locationName": "Toronto",
         "name": "Toronto Maple Leafs",
         "officialSiteUrl": "http://www.mapleleafs.com",
         "shortName": "Toronto",
         "teamName": "Maple Leafs",
         "venue": {
             "city": "Toronto",
             "link": "/api/v1/venues/null",
             "name": "Air Canada Centre",
-            "timeZone": {
-                "id": "America/Toronto",
-                "offset": -5,
-                "tz": "EST"
-            }
-        }
+            "timeZone": {"id": "America/Toronto", "offset": -5, "tz": "EST"},
+        },
     },
     "VAN": {
         "abbreviation": "VAN",
         "active": True,
-        "conference": {
-            "id": 5,
-            "link": "/api/v1/conferences/5",
-            "name": "Western"
-        },
-        "division": {
-            "id": 15,
-            "link": "/api/v1/divisions/15",
-            "name": "Pacific"
-        },
+        "conference": {"id": 5, "link": "/api/v1/conferences/5", "name": "Western"},
+        "division": {"id": 15, "link": "/api/v1/divisions/15", "name": "Pacific"},
         "firstYearOfPlay": "1970",
         "franchise": {
             "franchiseId": 20,
             "link": "/api/v1/franchises/20",
-            "teamName": "Canucks"
+            "teamName": "Canucks",
         },
         "franchiseId": 20,
         "id": 23,
         "link": "/api/v1/teams/23",
         "locationName": "Vancouver",
         "name": "Vancouver Canucks",
         "officialSiteUrl": "http://www.canucks.com",
         "shortName": "Vancouver",
         "teamName": "Canucks",
         "venue": {
             "city": "Vancouver",
             "link": "/api/v1/venues/null",
             "name": "Rogers Arena",
-            "timeZone": {
-                "id": "America/Vancouver",
-                "offset": -8,
-                "tz": "PST"
-            }
-        }
+            "timeZone": {"id": "America/Vancouver", "offset": -8, "tz": "PST"},
+        },
     },
     "VGK": {
         "abbreviation": "VGK",
         "active": True,
-        "conference": {
-            "id": 5,
-            "link": "/api/v1/conferences/5",
-            "name": "Western"
-        },
-        "division": {
-            "id": 15,
-            "link": "/api/v1/divisions/15",
-            "name": "Pacific"
-        },
+        "conference": {"id": 5, "link": "/api/v1/conferences/5", "name": "Western"},
+        "division": {"id": 15, "link": "/api/v1/divisions/15", "name": "Pacific"},
         "firstYearOfPlay": "2016",
         "franchise": {
             "franchiseId": 38,
             "link": "/api/v1/franchises/38",
-            "teamName": "Golden Knights"
+            "teamName": "Golden Knights",
         },
         "franchiseId": 38,
         "id": 54,
         "link": "/api/v1/teams/54",
         "locationName": "Vegas",
         "name": "Vegas Golden Knights",
         "officialSiteUrl": "http://www.vegasgoldenknights.com",
         "shortName": "Vegas",
         "teamName": "Golden Knights",
         "venue": {
             "city": "Las Vegas",
             "link": "/api/v1/venues/null",
             "name": "T-Mobile Arena",
-            "timeZone": {
-                "id": "America/Los_Angeles",
-                "offset": -8,
-                "tz": "PST"
-            }
-        }
+            "timeZone": {"id": "America/Los_Angeles", "offset": -8, "tz": "PST"},
+        },
     },
     "WPG": {
         "abbreviation": "WPG",
         "active": True,
-        "conference": {
-            "id": 5,
-            "link": "/api/v1/conferences/5",
-            "name": "Western"
-        },
-        "division": {
-            "id": 16,
-            "link": "/api/v1/divisions/16",
-            "name": "Central"
-        },
+        "conference": {"id": 5, "link": "/api/v1/conferences/5", "name": "Western"},
+        "division": {"id": 16, "link": "/api/v1/divisions/16", "name": "Central"},
         "firstYearOfPlay": "2011",
         "franchise": {
             "franchiseId": 35,
             "link": "/api/v1/franchises/35",
-            "teamName": "Jets"
+            "teamName": "Jets",
         },
         "franchiseId": 35,
         "id": 52,
         "link": "/api/v1/teams/52",
         "locationName": "Winnipeg",
         "name": "Winnipeg Jets",
         "officialSiteUrl": "http://winnipegjets.com",
         "shortName": "Winnipeg",
         "teamName": "Jets",
         "venue": {
             "city": "Winnipeg",
             "link": "/api/v1/venues/null",
             "name": "Bell MTS Place",
-            "timeZone": {
-                "id": "America/Winnipeg",
-                "offset": -6,
-                "tz": "CST"
-            }
-        }
+            "timeZone": {"id": "America/Winnipeg", "offset": -6, "tz": "CST"},
+        },
     },
     "WSH": {
         "abbreviation": "WSH",
         "active": True,
-        "conference": {
-            "id": 6,
-            "link": "/api/v1/conferences/6",
-            "name": "Eastern"
-        },
-        "division": {
-            "id": 18,
-            "link": "/api/v1/divisions/18",
-            "name": "Metropolitan"
-        },
+        "conference": {"id": 6, "link": "/api/v1/conferences/6", "name": "Eastern"},
+        "division": {"id": 18, "link": "/api/v1/divisions/18", "name": "Metropolitan"},
         "firstYearOfPlay": "1974",
         "franchise": {
             "franchiseId": 24,
             "link": "/api/v1/franchises/24",
-            "teamName": "Capitals"
+            "teamName": "Capitals",
         },
         "franchiseId": 24,
         "id": 15,
         "link": "/api/v1/teams/15",
         "locationName": "Washington",
         "name": "Washington Capitals",
         "officialSiteUrl": "http://www.washingtoncapitals.com",
         "shortName": "Washington",
         "teamName": "Capitals",
         "venue": {
             "city": "Washington",
             "link": "/api/v1/venues/null",
             "name": "Capital One Arena",
-            "timeZone": {
-                "id": "America/New_York",
-                "offset": -5,
-                "tz": "EST"
-            }
-        }
-    }
+            "timeZone": {"id": "America/New_York", "offset": -5, "tz": "EST"},
+        },
+    },
 }
```

