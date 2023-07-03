# Comparing `tmp/lemmy_nhl-1.5.0.tar.gz` & `tmp/lemmy_nhl-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lemmy_nhl-1.5.0.tar", last modified: Sat Jul  1 23:47:26 2023, max compression
+gzip compressed data, was "lemmy_nhl-1.5.1.tar", last modified: Mon Jul  3 02:22:59 2023, max compression
```

## Comparing `lemmy_nhl-1.5.0.tar` & `lemmy_nhl-1.5.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 23:47:26.097470 lemmy_nhl-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-01 23:47:14.000000 lemmy_nhl-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-01 23:47:26.097470 lemmy_nhl-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-07-01 23:47:14.000000 lemmy_nhl-1.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-01 23:47:14.000000 lemmy_nhl-1.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-01 23:47:26.097470 lemmy_nhl-1.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 23:47:26.093470 lemmy_nhl-1.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 23:47:26.097470 lemmy_nhl-1.5.0/src/lemmy_nhl/
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-01 23:47:14.000000 lemmy_nhl-1.5.0/src/lemmy_nhl/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6097 2023-07-01 23:47:14.000000 lemmy_nhl-1.5.0/src/lemmy_nhl/draft_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6323 2023-07-01 23:47:14.000000 lemmy_nhl-1.5.0/src/lemmy_nhl/lemmy_nhl_bot_daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)    12042 2023-07-01 23:47:14.000000 lemmy_nhl-1.5.0/src/lemmy_nhl/post_body.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 23:47:26.097470 lemmy_nhl-1.5.0/src/lemmy_nhl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-01 23:47:26.000000 lemmy_nhl-1.5.0/src/lemmy_nhl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-01 23:47:26.000000 lemmy_nhl-1.5.0/src/lemmy_nhl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 23:47:26.000000 lemmy_nhl-1.5.0/src/lemmy_nhl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-01 23:47:26.000000 lemmy_nhl-1.5.0/src/lemmy_nhl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-01 23:47:26.000000 lemmy_nhl-1.5.0/src/lemmy_nhl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-01 23:47:26.000000 lemmy_nhl-1.5.0/src/lemmy_nhl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:22:59.930413 lemmy_nhl-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-03 02:22:50.000000 lemmy_nhl-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-07-03 02:22:59.930413 lemmy_nhl-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-03 02:22:50.000000 lemmy_nhl-1.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-03 02:22:50.000000 lemmy_nhl-1.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-03 02:22:59.930413 lemmy_nhl-1.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:22:59.926413 lemmy_nhl-1.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:22:59.926413 lemmy_nhl-1.5.1/src/lemmy_nhl/
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-03 02:22:50.000000 lemmy_nhl-1.5.1/src/lemmy_nhl/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6353 2023-07-03 02:22:50.000000 lemmy_nhl-1.5.1/src/lemmy_nhl/draft_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-07-03 02:22:50.000000 lemmy_nhl-1.5.1/src/lemmy_nhl/lemmy_nhl_bot_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12042 2023-07-03 02:22:50.000000 lemmy_nhl-1.5.1/src/lemmy_nhl/post_body.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:22:59.926413 lemmy_nhl-1.5.1/src/lemmy_nhl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-07-03 02:22:59.000000 lemmy_nhl-1.5.1/src/lemmy_nhl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-03 02:22:59.000000 lemmy_nhl-1.5.1/src/lemmy_nhl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 02:22:59.000000 lemmy_nhl-1.5.1/src/lemmy_nhl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-03 02:22:59.000000 lemmy_nhl-1.5.1/src/lemmy_nhl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-03 02:22:59.000000 lemmy_nhl-1.5.1/src/lemmy_nhl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-03 02:22:59.000000 lemmy_nhl-1.5.1/src/lemmy_nhl.egg-info/top_level.txt
```

### Comparing `lemmy_nhl-1.5.0/LICENSE` & `lemmy_nhl-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lemmy_nhl-1.5.0/PKG-INFO` & `lemmy_nhl-1.5.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,49 @@
-Metadata-Version: 2.1
-Name: lemmy_nhl
-Version: 1.5.0
-Summary: bot to add live scores to lemmy community for hockey games
-Home-page: https://github.com/socphoenix/lemmy_nhl_bot
-Author: socphoenix
-License: Apache 2.0
-Keywords: lemmy,hockey,bot
-Description-Content-Type: text/markdown
-License-File: LICENSE
+# A few things to note currently:
 
-# DEV branch has been tested. A few things to note: 
 > Without modifying files, there is currently no way to test this. I've tested that it works with old data, and will be testing/
 > fixing whatever needs it during the first preseason game of the Flyers (or earlier if someone reports an issue before this).
 
 
 # lemmy_nhl_bot
-nhl linescore grabber/poster for lemmy
 
-This script requires the following to be installed from pip: plemmy, requests, json
+nhl linescore grabber/poster for lemmy. This app is meant to be run in the background to routinely add scores, standings, and team
+stats to a lemmy community focusing on a specific hockey team (standings are league wide, as is the draft function). After being
+configured, the main app is run in the background. It will check weekly for an updated schedule. Once per week
+(currently set to Sunday), it will post an updated League-wide standings page, and an updated team stats page. Once game days, it
+will start automatically at game time, and post scores and time updates every five seconds.
 
-> pip install plemmy  # source is https://github.com/tjkessler/plemmy/  Many thanks for tjkessler for the simple to use library!
+
+# Docker image
+
+There is a [branch](https://github.com/socphoenix/lemmy_nhl_bot/tree/docker) of this repo to aid in building a Docker image.
+To build and install with docker:
+
+> Download the following to a directory:
+>
+> [Dockerfile](https://github.com/socphoenix/lemmy_nhl_bot/blob/c056d557951d1e9bae1ab602c22b9e5b7788c03b/Dockerfile)
+> [config.py](https://github.com/socphoenix/lemmy_nhl_bot/blob/c056d557951d1e9bae1ab602c22b9e5b7788c03b/config.py)
+>
+> run:
+>
+> python3 config.py
+>
+> docker build -t lemmy_nhl_bot .
+
+
+# Building:
+
+    This script requires the following to be installed from pip: plemmy, requests, json
+
+> pip install plemmy   source is https://github.com/tjkessler/plemmy/  Many thanks for tjkessler for the simple to use library!
 
 > pip install requests
 
 > pip install json
 
-This has been tested with python 3.9 in FreeBSD and python3 in linux for a few basic outputs. Will be testing it on the first preseason game for live updates and pushing any needed fixes at that time in preperation for the regular season.
-
 
 ## Build the .whl
 > git clone https://github.com/socphoenix/lemmy_nhl_bot.git
 >
 > cd lemmy_nhl_bot
 >
 > git checkout dev
@@ -41,23 +54,34 @@
 >
 > pip install lemmy_nhl-2.0.0-py3-none-any.whl
 
 ## Usage:
 Before starting bot.py, please make sure to run config.py! It is needed to save your login token and teamID/community Name. Without
 these the script will crash!
 
-
 ### Run config.py:
 > Linux: lemmy_nhl_config
 
->FreeBSD: lemmy_nhl_config.py ##This requires path set. for sh (default shell): "PATH=${PATH}:/home/'put user here'/.local/bin" "export PATH"
+>FreeBSD: lemmy_nhl_config.py ##This requires path set. for sh (default shell): "PATH=${PATH}:/home/'put user here'/.local/bin" "export PATH" (as an interesting note, python seems to only add the path to the root user during install)
 
 ### run daemon
-Unix: lemmy_nhl_daemon   **** add " &" to run in the background. Working on creating service files but they are not done yet.
+
+Unix:
+ > lemmy_nhl_daemon
+ >
+ > add " &" to run in the background. Working on creating service files but they are not done yet.
 
 
 ### run draft bot
+
 Unix: lemmy_nhl_draft
 
 
+# See it in action!
 
 To see what the bot can currently do, look here: [pinned game](https://enterprise.lemmy.ml/post/417088), [stats](https://enterprise.lemmy.ml/post/417090), [standings](https://enterprise.lemmy.ml/post/417089)
+
+
+# Shared Libraries
+
+This uses the [Plemmy](https://github.com/tjkessler/plemmy/) library, which is also released under the Apache 2.0 license.
+Many thanks to tjkessler for the simple to use library!
```

### Comparing `lemmy_nhl-1.5.0/setup.cfg` & `lemmy_nhl-1.5.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lemmy_nhl
-version = 1.5.0
+version = 1.5.1
 author = socphoenix
 url = https://github.com/socphoenix/lemmy_nhl_bot
 description = bot to add live scores to lemmy community for hockey games
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = lemmy, hockey, bot
 license = Apache 2.0
```

### Comparing `lemmy_nhl-1.5.0/src/lemmy_nhl/config.py` & `lemmy_nhl-1.5.1/src/lemmy_nhl/config.py`

 * *Files identical despite different names*

### Comparing `lemmy_nhl-1.5.0/src/lemmy_nhl/draft_bot.py` & `lemmy_nhl-1.5.1/src/lemmy_nhl/draft_bot.py`

 * *Files 13% similar despite different names*

```diff
@@ -39,21 +39,32 @@
     server = server.rstrip("',)")
 
     #begin main program
     round1 = input("Is this the first Round? (y/n) ")
     round1 = round1.lower()
     srv = LemmyHttp(server)
     srv.key = token
-    request = srv.get_community(None, communityName)
-    print(request)
-    CID = request.json().get("community_view")
-    CID = CID["community"].get("id")
-    post = srv.create_post(CID, str(draftYear) + " Draft!", body="")
-    postID = post.json().get("post_view")
-    postID = postID["post"].get("id")
+    requested = False
+    while(requested == False):
+        try:
+            request = srv.get_community(None, communityName)
+            CID = request.json().get("community_view")
+            CID = CID["community"].get("id")
+            requested = True
+        except:
+            print("failed to get community, trying again")
+    requested = False
+    while(requested == False):
+        try:
+            post = srv.create_post(CID, str(draftYear) + " Draft!", body="")
+            postID = post.json().get("post_view")
+            postID = postID["post"].get("id")
+            requested = True
+        except:
+            print("failed to create post, trying again.")
 
 
     while(True):
         r = requests.get("https://statsapi.web.nhl.com/api/v1/draft")
         lister = r.json().get("drafts")[0].get("rounds")
         teams = lister[0].get("picks")
         body = ""
@@ -127,28 +138,24 @@
         #Round 6
         teams = lister[5].get("picks")
         i = 0
         j = len(teams)
         body6 = "# Round 6 \n" + "| Team Name | Pick # | Selection | \n"
         body6 = body6 + "| -------- | ------- | -------- |\n"
         while(i < j):
-            #print(i)
-            #teams[i].get("team")
             body6 = body6 + str(teams[i].get("team").get("name")) + " | " + str(teams[i].get("pickOverall")) + " | " + str(teams[i].get("prospect").get("fullName")) + " | \n"
             i = i + 1
 
         #Round 7
         teams = lister[6].get("picks")
         i = 0
         j = len(teams)
         body7 = "# Round 7 \n" + "| Team Name | Pick # | Selection | \n"
         body7 = body7 + "| -------- | ------- | -------- |\n"
         while(i < j):
-            #print(i)
-            #teams[i].get("team")
             body7 = body7 + str(teams[i].get("team").get("name")) + " | " + str(teams[i].get("pickOverall")) + " | " + str(teams[i].get("prospect").get("fullName")) + " | \n"
             if(str(teams[i].get("prospect").get("fullName")) != ""):
                 finished = True
             i = i + 1
 
         #update post this requires timeout enabled in plemmy, pull request has been submitted to get it merged upstream.
         try:
```

### Comparing `lemmy_nhl-1.5.0/src/lemmy_nhl/lemmy_nhl_bot_daemon.py` & `lemmy_nhl-1.5.1/src/lemmy_nhl/lemmy_nhl_bot_daemon.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,32 +17,33 @@
 newSchedule = False
 srv = ""
 # create time based services
 # check for game today:
 
 #is game
 def isGame():
-    global gameOver, games, gamePK
+    global gameOver, games, gamePK, srv, postID
     today = time.strftime("%Y, %m, %d")
     today = str(today)
     today = today.split(", ")
     for x in range(len(games)):
         gameToday = games[x][1]
         gameToday = gameToday.split("-")
         gamePK = games[x][0]
         if(today[0] == gameToday[0] and today[1] == gameToday[1] and today[2] == gameToday[2]):
             timeStart = games[x][2]
             curTime = time.strftime("%H:%M", time.gmtime())
             timeStart = timeStart.split(":")
             curTime = curTime.split(":")
             #compare 0, 1 on these if hour and minute >= to then start game
             if(int(curTime[0]) >= int(timeStart[0]) and int(curTime[1]) >= int(timeStart[1]) and gameOver == False):
-                   create_post_linescore()
-                   while(gameOver == False):
-                       gameTime()
+                create_post_linescore()
+                while(gameOver == False):
+                    gameTime()
+                srv.feature_post("Community", False, postID)
 
 #create post for linescore
 def create_post_linescore():
     global teamID, gamePK, isMod, srv, postID
     #get team Names/date/regular Season
     game_today = "https://statsapi.web.nhl.com/api/v1/game/" + str(gamePK) + "/linescore"
     game_today2 = "https://statsapi.web.nhl.com/api/v1/schedule?teamId="
@@ -58,19 +59,33 @@
     elif(gameType == "PR"):
         gameType = "Pre-Season"
     else:
         gameType = "Playoffs"
     postName = away_name + " vs. " + home_name + " " + gameType + " " + str(date)
     global CID, postID
     temp = CID
-    post = srv.create_post(temp, postName, body="")
-    postID = post.json().get("post_view")
-    postID = postID["post"].get("id")
+    posted = False
+    while(posted == False):
+        try:
+            post = srv.create_post(temp, postName, body="")
+            postID = post.json().get("post_view")
+            postID = postID["post"].get("id")
+            posted = True
+        except:
+            print("failed to post, trying again in 30 seconds")
+            time.sleep(30)
     if(isMod == "y"):
-        srv.feature_post("Community", True, postID)
+        feature = False
+        while(feature == False):
+            try:
+                srv.feature_post("Community", True, postID)
+                feature = True
+            except:
+                print("Failed to feature post, trying again in 30 seconds.")
+                time.sleep(30)
 
 
 #Linescore for game
 def gameTime():
     global gameOver, postID, gamePK, srv
     body2, gameOver = post_body.post_body_linescore(gamePK)
     try:
@@ -84,33 +99,46 @@
 #get community ID
 
 def create_post_stats():
     global CID, teamID, srv
     today = time.strftime("%m-%d-%Y")
     title = "Team Stats for the Season as of " + today
     body = post_body.post_body_stats(teamID)
-    srv.create_post(CID, title, body=body)
+    posted = False
+    while(posted == False):
+        try:
+            srv.create_post(CID, title, body=body)
+            posted = True
+        except:
+            print("failed to post, trying again in 30 seconds.")
+            time.sleep(30)
 
 def create_post_standings():
     today = time.strftime("%m-%d-%Y")
     global CID
     postName = "NHL Standings as of " + today
     body = post_body.post_body_standings()
-    post = srv.create_post(CID, postName, body=body)
+    posted = False
+    while(posted == False):
+        try:
+            post = srv.create_post(CID, postName, body=body)
+            posted = True
+        except:
+            print("failed to post, trying again in 30 seconds.")
+            time.sleep(30)
 
 #main loop segment
 def daemon():
     global token, communityName, server, teamID, isMod, games, standings, stats, post, CID, newSchedule, gameOver, srv
     dbLocation = os.path.expanduser("~/.cache/lnhl.db")
     if(os.path.exists(dbLocation) == False):
         print("Please run config.py first!")
         sys.exit()
 
     #sql database connection/data grabbing
-    dbLocation = os.path.expanduser("~/.cache/lnhl.db")
     con = sqlite3.connect(dbLocation)
     cur = con.cursor()
     #get login token
     r = cur.execute("SELECT token FROM user")
     temp = r.fetchall()
     token = str(temp[0])
     token = token.lstrip("('")
@@ -154,15 +182,15 @@
     CID = CID["community"].get("id")
 
 
     #main loop
     while(True):
         isGame()
         today = time.strftime("%a")
-        if(str(today) == "Sat" and standings == False):
+        if(str(today) == "Sun" and standings == False):
             create_post_standings()
             create_post_stats()
             standings = True
             stats = True
             newSchedule = True
             # get new schedule weekly to catch playoffs
             cur.execute("DELETE FROM schedule")
```

### Comparing `lemmy_nhl-1.5.0/src/lemmy_nhl/post_body.py` & `lemmy_nhl-1.5.1/src/lemmy_nhl/post_body.py`

 * *Files identical despite different names*

