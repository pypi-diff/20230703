# Comparing `tmp/piqueserver-1.0.0.tar.gz` & `tmp/piqueserver-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/piqueserver-1.0.0.tar", last modified: Mon Dec  2 01:46:37 2019, max compression
+gzip compressed data, was "piqueserver-1.1.1.tar", last modified: Mon Jul  3 17:47:04 2023, max compression
```

## Comparing `piqueserver-1.0.0.tar` & `piqueserver-1.1.1.tar`

### file list

```diff
@@ -1,157 +1,159 @@
-drwxr-xr-x   0 nota      (1000) nota      (1000)        0 2019-12-02 01:46:37.000000 piqueserver-1.0.0/
--rw-r--r--   0 nota      (1000) nota      (1000)      806 2019-12-02 00:53:49.000000 piqueserver-1.0.0/MANIFEST.in
--rw-r--r--   0 nota      (1000) nota      (1000)     8567 2019-12-02 01:46:37.000000 piqueserver-1.0.0/PKG-INFO
--rw-r--r--   0 nota      (1000) nota      (1000)     5733 2019-12-02 01:30:01.000000 piqueserver-1.0.0/README.rst
-drwxr-xr-x   0 nota      (1000) nota      (1000)        0 2019-12-02 01:46:37.000000 piqueserver-1.0.0/piqueserver/
--rw-r--r--   0 nota      (1000) nota      (1000)       33 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/__init__.py
--rw-r--r--   0 nota      (1000) nota      (1000)      194 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/__main__.py
--rw-r--r--   0 nota      (1000) nota      (1000)      326 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/auth.py
--rw-r--r--   0 nota      (1000) nota      (1000)     1632 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/banpublish.py
--rw-r--r--   0 nota      (1000) nota      (1000)     2912 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/bansubscribe.py
--rw-r--r--   0 nota      (1000) nota      (1000)    13157 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/commands.py
-drwxr-xr-x   0 nota      (1000) nota      (1000)        0 2019-12-02 01:46:37.000000 piqueserver-1.0.0/piqueserver/config/
--rw-r--r--   0 nota      (1000) nota      (1000)     1116 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/config/README.md
--rw-r--r--   0 nota      (1000) nota      (1000)    10869 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/config/config.toml
-drwxr-xr-x   0 nota      (1000) nota      (1000)        0 2019-12-02 01:46:37.000000 piqueserver-1.0.0/piqueserver/config/game_modes/
--rw-r--r--   0 nota      (1000) nota      (1000)      297 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/config/game_modes/README.md
-drwxr-xr-x   0 nota      (1000) nota      (1000)        0 2019-12-02 01:46:37.000000 piqueserver-1.0.0/piqueserver/config/maps/
--rw-r--r--   0 nota      (1000) nota      (1000)      221 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/config/maps/classicgen.txt
--rw-r--r--   0 nota      (1000) nota      (1000)     5067 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/config/maps/random.txt
-drwxr-xr-x   0 nota      (1000) nota      (1000)        0 2019-12-02 01:46:37.000000 piqueserver-1.0.0/piqueserver/config/scripts/
--rw-r--r--   0 nota      (1000) nota      (1000)      128 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/config/scripts/README.md
--rw-r--r--   0 nota      (1000) nota      (1000)    10030 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/config.py
--rw-r--r--   0 nota      (1000) nota      (1000)     3414 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/console.py
-drwxr-xr-x   0 nota      (1000) nota      (1000)        0 2019-12-02 01:46:37.000000 piqueserver-1.0.0/piqueserver/core_commands/
--rw-r--r--   0 nota      (1000) nota      (1000)      911 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/core_commands/__init__.py
--rw-r--r--   0 nota      (1000) nota      (1000)     9025 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/core_commands/game.py
--rw-r--r--   0 nota      (1000) nota      (1000)     2220 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/core_commands/info.py
--rw-r--r--   0 nota      (1000) nota      (1000)     3100 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/core_commands/map.py
--rw-r--r--   0 nota      (1000) nota      (1000)    11764 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/core_commands/moderation.py
--rw-r--r--   0 nota      (1000) nota      (1000)     6359 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/core_commands/movement.py
--rw-r--r--   0 nota      (1000) nota      (1000)     2908 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/core_commands/player.py
--rw-r--r--   0 nota      (1000) nota      (1000)     2105 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/core_commands/server.py
--rw-r--r--   0 nota      (1000) nota      (1000)     2228 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/core_commands/social.py
--rw-r--r--   0 nota      (1000) nota      (1000)     5087 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/extensions.py
-drwxr-xr-x   0 nota      (1000) nota      (1000)        0 2019-12-02 01:46:37.000000 piqueserver-1.0.0/piqueserver/game_modes/
--rw-r--r--   0 nota      (1000) nota      (1000)        0 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/game_modes/__init__.py
--rw-r--r--   0 nota      (1000) nota      (1000)    22210 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/game_modes/arena.py
--rw-r--r--   0 nota      (1000) nota      (1000)     4394 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/game_modes/babel.py
--rw-r--r--   0 nota      (1000) nota      (1000)     3183 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/game_modes/freeforall.py
--rw-r--r--   0 nota      (1000) nota      (1000)    10162 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/game_modes/infiltration.py
--rw-r--r--   0 nota      (1000) nota      (1000)     4465 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/game_modes/onectf.py
--rw-r--r--   0 nota      (1000) nota      (1000)    17121 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/game_modes/push.py
--rw-r--r--   0 nota      (1000) nota      (1000)     3448 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/game_modes/tdm.py
--rw-r--r--   0 nota      (1000) nota      (1000)     5604 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/game_modes/tow.py
--rw-r--r--   0 nota      (1000) nota      (1000)    11434 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/irc.py
--rw-r--r--   0 nota      (1000) nota      (1000)     5876 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/map.py
--rw-r--r--   0 nota      (1000) nota      (1000)     2863 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/networkdict.py
--rw-r--r--   0 nota      (1000) nota      (1000)    14712 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/player.py
--rw-r--r--   0 nota      (1000) nota      (1000)     1350 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/release.py
--rw-r--r--   0 nota      (1000) nota      (1000)     8097 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/run.py
--rw-r--r--   0 nota      (1000) nota      (1000)     1666 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/scheduler.py
-drwxr-xr-x   0 nota      (1000) nota      (1000)        0 2019-12-02 01:46:37.000000 piqueserver-1.0.0/piqueserver/scripts/
--rw-r--r--   0 nota      (1000) nota      (1000)        0 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/scripts/__init__.py
--rw-r--r--   0 nota      (1000) nota      (1000)     4486 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/scripts/afk.py
--rw-r--r--   0 nota      (1000) nota      (1000)    19788 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/scripts/aimbot2.py
--rw-r--r--   0 nota      (1000) nota      (1000)    12048 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/scripts/airstrike2.py
--rw-r--r--   0 nota      (1000) nota      (1000)     6204 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/scripts/analyze.py
--rw-r--r--   0 nota      (1000) nota      (1000)     1603 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/scripts/antijerk.py
--rw-r--r--   0 nota      (1000) nota      (1000)     1785 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/scripts/autohelp.py
--rw-r--r--   0 nota      (1000) nota      (1000)     9229 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/scripts/babel_script.py
--rw-r--r--   0 nota      (1000) nota      (1000)    11838 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/scripts/badmin.py
--rw-r--r--   0 nota      (1000) nota      (1000)     6532 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/scripts/blockinfo.py
--rw-r--r--   0 nota      (1000) nota      (1000)     5412 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/scripts/daycycle.py
--rw-r--r--   0 nota      (1000) nota      (1000)     1607 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/scripts/demolitionman.py
--rw-r--r--   0 nota      (1000) nota      (1000)     1946 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/scripts/dirtnade.py
--rw-r--r--   0 nota      (1000) nota      (1000)     2081 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/scripts/disco.py
--rw-r--r--   0 nota      (1000) nota      (1000)     1612 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/scripts/flagreturn.py
--rw-r--r--   0 nota      (1000) nota      (1000)     1728 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/scripts/geoip.py
--rw-r--r--   0 nota      (1000) nota      (1000)    11242 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/scripts/grownade.py
--rw-r--r--   0 nota      (1000) nota      (1000)     1582 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/scripts/map_extensions.py
--rw-r--r--   0 nota      (1000) nota      (1000)    13043 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/scripts/mapmakingtools.py
--rw-r--r--   0 nota      (1000) nota      (1000)    24376 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/scripts/markers.py
--rw-r--r--   0 nota      (1000) nota      (1000)     5463 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/scripts/match.py
--rw-r--r--   0 nota      (1000) nota      (1000)     1422 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/scripts/medkit.py
--rw-r--r--   0 nota      (1000) nota      (1000)      646 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/scripts/memcheck.py
--rw-r--r--   0 nota      (1000) nota      (1000)     9847 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/scripts/minefield.py
--rw-r--r--   0 nota      (1000) nota      (1000)      494 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/scripts/nointelonwalls.py
--rw-r--r--   0 nota      (1000) nota      (1000)     1169 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/scripts/nospadingwalls.py
--rw-r--r--   0 nota      (1000) nota      (1000)     2761 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/scripts/paint.py
--rw-r--r--   0 nota      (1000) nota      (1000)     1033 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/scripts/passreload.py
--rw-r--r--   0 nota      (1000) nota      (1000)     2409 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/scripts/protect.py
--rw-r--r--   0 nota      (1000) nota      (1000)     6746 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/scripts/rampage.py
--rw-r--r--   0 nota      (1000) nota      (1000)     2636 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/scripts/rangedamage.py
--rw-r--r--   0 nota      (1000) nota      (1000)     3398 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/scripts/rapid.py
--rw-r--r--   0 nota      (1000) nota      (1000)     2886 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/scripts/ratio.py
--rw-r--r--   0 nota      (1000) nota      (1000)    10952 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/scripts/rollback.py
--rw-r--r--   0 nota      (1000) nota      (1000)     7545 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/scripts/runningman.py
--rw-r--r--   0 nota      (1000) nota      (1000)     2241 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/scripts/savemap.py
--rw-r--r--   0 nota      (1000) nota      (1000)     1255 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/scripts/smartnade.py
--rw-r--r--   0 nota      (1000) nota      (1000)      743 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/scripts/spadenadefix.py
--rw-r--r--   0 nota      (1000) nota      (1000)     1431 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/scripts/spawn_protect.py
--rw-r--r--   0 nota      (1000) nota      (1000)     4483 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/scripts/spectatorcontrol.py
--rw-r--r--   0 nota      (1000) nota      (1000)    10969 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/scripts/squad.py
--rw-r--r--   0 nota      (1000) nota      (1000)     3441 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/scripts/strongblock.py
--rw-r--r--   0 nota      (1000) nota      (1000)     2049 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/scripts/timedmute.py
--rw-r--r--   0 nota      (1000) nota      (1000)     1585 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/scripts/trusted.py
--rw-r--r--   0 nota      (1000) nota      (1000)    11678 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/scripts/votekick.py
--rw-r--r--   0 nota      (1000) nota      (1000)     8754 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/scripts/votemap.py
--rw-r--r--   0 nota      (1000) nota      (1000)      658 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/scripts/welcome.py
--rw-r--r--   0 nota      (1000) nota      (1000)     6216 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/scripts/zoc.py
--rw-r--r--   0 nota      (1000) nota      (1000)    37831 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/server.py
--rw-r--r--   0 nota      (1000) nota      (1000)     2623 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/ssh.py
--rw-r--r--   0 nota      (1000) nota      (1000)     5739 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/statistics.py
--rw-r--r--   0 nota      (1000) nota      (1000)     5713 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/statusserver.py
-drwxr-xr-x   0 nota      (1000) nota      (1000)        0 2019-12-02 01:46:37.000000 piqueserver-1.0.0/piqueserver/utils/
--rw-r--r--   0 nota      (1000) nota      (1000)       76 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/utils/__init__.py
--rw-r--r--   0 nota      (1000) nota      (1000)      267 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/utils/_async.py
--rw-r--r--   0 nota      (1000) nota      (1000)     6642 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/utils/_timeparse.py
--rw-r--r--   0 nota      (1000) nota      (1000)       51 2019-12-02 00:54:42.000000 piqueserver-1.0.0/piqueserver/version.py
-drwxr-xr-x   0 nota      (1000) nota      (1000)        0 2019-12-02 01:46:37.000000 piqueserver-1.0.0/piqueserver/web/
--rw-r--r--   0 nota      (1000) nota      (1000)        0 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/web/__init__.py
-drwxr-xr-x   0 nota      (1000) nota      (1000)        0 2019-12-02 01:46:37.000000 piqueserver-1.0.0/piqueserver/web/templates/
--rw-r--r--   0 nota      (1000) nota      (1000)    11833 2019-12-02 00:53:49.000000 piqueserver-1.0.0/piqueserver/web/templates/status.html
-drwxr-xr-x   0 nota      (1000) nota      (1000)        0 2019-12-02 01:46:37.000000 piqueserver-1.0.0/piqueserver.egg-info/
--rw-r--r--   0 nota      (1000) nota      (1000)     8567 2019-12-02 01:46:37.000000 piqueserver-1.0.0/piqueserver.egg-info/PKG-INFO
--rw-r--r--   0 nota      (1000) nota      (1000)     4156 2019-12-02 01:46:37.000000 piqueserver-1.0.0/piqueserver.egg-info/SOURCES.txt
--rw-r--r--   0 nota      (1000) nota      (1000)        1 2019-12-02 01:46:37.000000 piqueserver-1.0.0/piqueserver.egg-info/dependency_links.txt
--rw-r--r--   0 nota      (1000) nota      (1000)       54 2019-12-02 01:46:37.000000 piqueserver-1.0.0/piqueserver.egg-info/entry_points.txt
--rw-r--r--   0 nota      (1000) nota      (1000)      203 2019-12-02 01:46:37.000000 piqueserver-1.0.0/piqueserver.egg-info/requires.txt
--rw-r--r--   0 nota      (1000) nota      (1000)       21 2019-12-02 01:46:37.000000 piqueserver-1.0.0/piqueserver.egg-info/top_level.txt
-drwxr-xr-x   0 nota      (1000) nota      (1000)        0 2019-12-02 01:46:37.000000 piqueserver-1.0.0/pyspades/
--rw-r--r--   0 nota      (1000) nota      (1000)     1111 2019-12-02 00:53:49.000000 piqueserver-1.0.0/pyspades/__init__.py
--rw-r--r--   0 nota      (1000) nota      (1000)     1779 2019-12-02 00:53:49.000000 piqueserver-1.0.0/pyspades/bytes.pxd
--rw-r--r--   0 nota      (1000) nota      (1000)     9683 2019-12-02 00:53:49.000000 piqueserver-1.0.0/pyspades/bytes.pyx
--rw-r--r--   0 nota      (1000) nota      (1000)     4222 2019-12-02 00:53:49.000000 piqueserver-1.0.0/pyspades/bytes_c.cpp
--rw-r--r--   0 nota      (1000) nota      (1000)     8890 2019-12-02 00:53:49.000000 piqueserver-1.0.0/pyspades/classicgen_c.cpp
--rw-r--r--   0 nota      (1000) nota      (1000)     1464 2019-12-02 00:53:49.000000 piqueserver-1.0.0/pyspades/collision.py
--rw-r--r--   0 nota      (1000) nota      (1000)      977 2019-12-02 00:53:49.000000 piqueserver-1.0.0/pyspades/color.py
--rw-r--r--   0 nota      (1000) nota      (1000)     2409 2019-12-02 00:53:49.000000 piqueserver-1.0.0/pyspades/common.pxd
--rw-r--r--   0 nota      (1000) nota      (1000)    14615 2019-12-02 00:53:49.000000 piqueserver-1.0.0/pyspades/common.pyx
--rw-r--r--   0 nota      (1000) nota      (1000)      365 2019-12-02 00:53:49.000000 piqueserver-1.0.0/pyspades/common_c.h
--rw-r--r--   0 nota      (1000) nota      (1000)     2409 2019-12-02 00:53:49.000000 piqueserver-1.0.0/pyspades/constants.py
--rw-r--r--   0 nota      (1000) nota      (1000)      299 2019-12-02 00:53:49.000000 piqueserver-1.0.0/pyspades/constants_c.h
--rw-r--r--   0 nota      (1000) nota      (1000)    28609 2019-12-02 00:53:49.000000 piqueserver-1.0.0/pyspades/contained.pyx
--rw-r--r--   0 nota      (1000) nota      (1000)     4973 2019-12-02 00:53:49.000000 piqueserver-1.0.0/pyspades/entities.py
--rw-r--r--   0 nota      (1000) nota      (1000)     5316 2019-12-02 00:53:49.000000 piqueserver-1.0.0/pyspades/gamemodes.py
--rw-r--r--   0 nota      (1000) nota      (1000)      886 2019-12-02 00:53:49.000000 piqueserver-1.0.0/pyspades/loaders.pxd
--rw-r--r--   0 nota      (1000) nota      (1000)     1400 2019-12-02 00:53:49.000000 piqueserver-1.0.0/pyspades/loaders.pyx
--rw-r--r--   0 nota      (1000) nota      (1000)     3132 2019-12-02 00:53:49.000000 piqueserver-1.0.0/pyspades/mapgenerator.py
--rw-r--r--   0 nota      (1000) nota      (1000)    20215 2019-12-02 00:53:49.000000 piqueserver-1.0.0/pyspades/mapmaker.pyx
--rw-r--r--   0 nota      (1000) nota      (1000)     3352 2019-12-02 00:53:49.000000 piqueserver-1.0.0/pyspades/master.py
--rw-r--r--   0 nota      (1000) nota      (1000)     4943 2019-12-02 00:53:49.000000 piqueserver-1.0.0/pyspades/packet.pyx
--rw-r--r--   0 nota      (1000) nota      (1000)    51435 2019-12-02 00:53:49.000000 piqueserver-1.0.0/pyspades/player.py
--rw-r--r--   0 nota      (1000) nota      (1000)     5850 2019-12-02 00:53:49.000000 piqueserver-1.0.0/pyspades/protocol.py
--rw-r--r--   0 nota      (1000) nota      (1000)    15912 2019-12-02 00:53:49.000000 piqueserver-1.0.0/pyspades/server.py
--rw-r--r--   0 nota      (1000) nota      (1000)     3117 2019-12-02 00:53:49.000000 piqueserver-1.0.0/pyspades/team.py
--rw-r--r--   0 nota      (1000) nota      (1000)     1654 2019-12-02 00:53:49.000000 piqueserver-1.0.0/pyspades/tools.py
--rw-r--r--   0 nota      (1000) nota      (1000)     2092 2019-12-02 00:53:49.000000 piqueserver-1.0.0/pyspades/types.py
--rw-r--r--   0 nota      (1000) nota      (1000)     1992 2019-12-02 00:53:49.000000 piqueserver-1.0.0/pyspades/vxl.pxd
--rw-r--r--   0 nota      (1000) nota      (1000)     9463 2019-12-02 00:53:49.000000 piqueserver-1.0.0/pyspades/vxl.pyx
--rw-r--r--   0 nota      (1000) nota      (1000)    15738 2019-12-02 00:53:49.000000 piqueserver-1.0.0/pyspades/vxl_c.cpp
--rw-r--r--   0 nota      (1000) nota      (1000)     2358 2019-12-02 00:53:49.000000 piqueserver-1.0.0/pyspades/vxl_c.h
--rw-r--r--   0 nota      (1000) nota      (1000)     4406 2019-12-02 00:53:49.000000 piqueserver-1.0.0/pyspades/weapon.py
--rw-r--r--   0 nota      (1000) nota      (1000)    14935 2019-12-02 00:53:49.000000 piqueserver-1.0.0/pyspades/world.pyx
--rw-r--r--   0 nota      (1000) nota      (1000)    19429 2019-12-02 00:53:49.000000 piqueserver-1.0.0/pyspades/world_c.cpp
--rw-r--r--   0 nota      (1000) nota      (1000)       80 2019-12-02 01:46:37.000000 piqueserver-1.0.0/setup.cfg
--rw-r--r--   0 nota      (1000) nota      (1000)     4879 2019-12-02 01:29:36.000000 piqueserver-1.0.0/setup.py
+drwxr-xr-x   0 nota      (1000) nota      (1000)        0 2023-07-03 17:47:04.779773 piqueserver-1.1.1/
+-rw-r--r--   0 nota      (1000) nota      (1000)    35147 2023-07-03 17:42:02.000000 piqueserver-1.1.1/COPYING.txt
+-rw-r--r--   0 nota      (1000) nota      (1000)    35141 2023-07-03 17:42:02.000000 piqueserver-1.1.1/LICENSE
+-rw-r--r--   0 nota      (1000) nota      (1000)      806 2023-07-03 17:42:02.000000 piqueserver-1.1.1/MANIFEST.in
+-rw-r--r--   0 nota      (1000) nota      (1000)     7480 2023-07-03 17:47:04.780773 piqueserver-1.1.1/PKG-INFO
+-rw-r--r--   0 nota      (1000) nota      (1000)     6187 2023-07-03 17:46:48.000000 piqueserver-1.1.1/README.rst
+drwxr-xr-x   0 nota      (1000) nota      (1000)        0 2023-07-03 17:47:04.775773 piqueserver-1.1.1/piqueserver/
+-rw-r--r--   0 nota      (1000) nota      (1000)       33 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/__init__.py
+-rw-r--r--   0 nota      (1000) nota      (1000)      194 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/__main__.py
+-rw-r--r--   0 nota      (1000) nota      (1000)      326 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/auth.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     1632 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/banpublish.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     3145 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/bansubscribe.py
+-rw-r--r--   0 nota      (1000) nota      (1000)    13204 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/commands.py
+drwxr-xr-x   0 nota      (1000) nota      (1000)        0 2023-07-03 17:47:04.775773 piqueserver-1.1.1/piqueserver/config/
+-rw-r--r--   0 nota      (1000) nota      (1000)     1116 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/config/README.md
+-rw-r--r--   0 nota      (1000) nota      (1000)    11263 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/config/config.toml
+drwxr-xr-x   0 nota      (1000) nota      (1000)        0 2023-07-03 17:47:04.776773 piqueserver-1.1.1/piqueserver/config/game_modes/
+-rw-r--r--   0 nota      (1000) nota      (1000)      297 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/config/game_modes/README.md
+drwxr-xr-x   0 nota      (1000) nota      (1000)        0 2023-07-03 17:47:04.776773 piqueserver-1.1.1/piqueserver/config/maps/
+-rw-r--r--   0 nota      (1000) nota      (1000)      221 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/config/maps/classicgen.txt
+-rw-r--r--   0 nota      (1000) nota      (1000)     5067 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/config/maps/random.txt
+drwxr-xr-x   0 nota      (1000) nota      (1000)        0 2023-07-03 17:47:04.776773 piqueserver-1.1.1/piqueserver/config/scripts/
+-rw-r--r--   0 nota      (1000) nota      (1000)      128 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/config/scripts/README.md
+-rw-r--r--   0 nota      (1000) nota      (1000)    10033 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/config.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     3324 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/console.py
+drwxr-xr-x   0 nota      (1000) nota      (1000)        0 2023-07-03 17:47:04.776773 piqueserver-1.1.1/piqueserver/core_commands/
+-rw-r--r--   0 nota      (1000) nota      (1000)      911 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/core_commands/__init__.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     9210 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/core_commands/game.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     2249 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/core_commands/info.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     3497 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/core_commands/map.py
+-rw-r--r--   0 nota      (1000) nota      (1000)    11857 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/core_commands/moderation.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     6367 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/core_commands/movement.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     2926 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/core_commands/player.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     2105 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/core_commands/server.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     2228 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/core_commands/social.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     5090 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/extensions.py
+drwxr-xr-x   0 nota      (1000) nota      (1000)        0 2023-07-03 17:47:04.776773 piqueserver-1.1.1/piqueserver/game_modes/
+-rw-r--r--   0 nota      (1000) nota      (1000)        0 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/game_modes/__init__.py
+-rw-r--r--   0 nota      (1000) nota      (1000)    22203 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/game_modes/arena.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     4285 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/game_modes/babel.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     5043 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/game_modes/freeforall.py
+-rw-r--r--   0 nota      (1000) nota      (1000)    10092 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/game_modes/infiltration.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     4532 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/game_modes/onectf.py
+-rw-r--r--   0 nota      (1000) nota      (1000)    17400 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/game_modes/push.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     5209 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/game_modes/tdm.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     5604 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/game_modes/tow.py
+-rw-r--r--   0 nota      (1000) nota      (1000)    11452 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/irc.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     5876 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/map.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     2953 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/networkdict.py
+-rw-r--r--   0 nota      (1000) nota      (1000)    16156 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/player.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     1350 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/release.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     8537 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/run.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     1666 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scheduler.py
+drwxr-xr-x   0 nota      (1000) nota      (1000)        0 2023-07-03 17:47:04.778773 piqueserver-1.1.1/piqueserver/scripts/
+-rw-r--r--   0 nota      (1000) nota      (1000)        0 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/__init__.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     4485 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/afk.py
+-rw-r--r--   0 nota      (1000) nota      (1000)    19815 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/aimbot2.py
+-rw-r--r--   0 nota      (1000) nota      (1000)    12194 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/airstrike2.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     6238 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/analyze.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     1602 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/antijerk.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     1795 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/autohelp.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     9288 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/babel_script.py
+-rw-r--r--   0 nota      (1000) nota      (1000)    11601 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/badmin.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     6554 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/blockinfo.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     5448 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/daycycle.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     1612 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/demolitionman.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     1946 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/dirtnade.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     2091 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/disco.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     1617 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/flagreturn.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     1734 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/geoip.py
+-rw-r--r--   0 nota      (1000) nota      (1000)    11241 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/grownade.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     1582 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/map_extensions.py
+-rw-r--r--   0 nota      (1000) nota      (1000)    13043 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/mapmakingtools.py
+-rw-r--r--   0 nota      (1000) nota      (1000)    24491 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/markers.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     5503 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/match.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     1476 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/medkit.py
+-rw-r--r--   0 nota      (1000) nota      (1000)      646 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/memcheck.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     9858 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/minefield.py
+-rw-r--r--   0 nota      (1000) nota      (1000)      494 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/nointelonwalls.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     1169 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/nospadingwalls.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     2761 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/paint.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     1033 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/passreload.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     2431 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/protect.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     6818 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/rampage.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     2635 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/rangedamage.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     3398 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/rapid.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     2904 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/ratio.py
+-rw-r--r--   0 nota      (1000) nota      (1000)    11023 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/rollback.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     7644 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/runningman.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     3250 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/savemap.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     1255 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/smartnade.py
+-rw-r--r--   0 nota      (1000) nota      (1000)      743 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/spadenadefix.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     1430 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/spawn_protect.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     4482 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/spectatorcontrol.py
+-rw-r--r--   0 nota      (1000) nota      (1000)    10982 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/squad.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     3441 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/strongblock.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     2064 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/timedmute.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     1585 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/trusted.py
+-rw-r--r--   0 nota      (1000) nota      (1000)    12461 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/votekick.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     8869 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/votemap.py
+-rw-r--r--   0 nota      (1000) nota      (1000)      662 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/welcome.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     6215 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/scripts/zoc.py
+-rw-r--r--   0 nota      (1000) nota      (1000)    37061 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/server.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     2623 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/ssh.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     5739 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/statistics.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     5620 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/statusserver.py
+drwxr-xr-x   0 nota      (1000) nota      (1000)        0 2023-07-03 17:47:04.778773 piqueserver-1.1.1/piqueserver/utils/
+-rw-r--r--   0 nota      (1000) nota      (1000)       86 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/utils/__init__.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     1786 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/utils/_async.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     6642 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/utils/_timeparse.py
+-rw-r--r--   0 nota      (1000) nota      (1000)       51 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/version.py
+drwxr-xr-x   0 nota      (1000) nota      (1000)        0 2023-07-03 17:47:04.778773 piqueserver-1.1.1/piqueserver/web/
+-rw-r--r--   0 nota      (1000) nota      (1000)        0 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/web/__init__.py
+drwxr-xr-x   0 nota      (1000) nota      (1000)        0 2023-07-03 17:47:04.778773 piqueserver-1.1.1/piqueserver/web/templates/
+-rw-r--r--   0 nota      (1000) nota      (1000)    11833 2023-07-03 17:42:02.000000 piqueserver-1.1.1/piqueserver/web/templates/status.html
+drwxr-xr-x   0 nota      (1000) nota      (1000)        0 2023-07-03 17:47:04.775773 piqueserver-1.1.1/piqueserver.egg-info/
+-rw-r--r--   0 nota      (1000) nota      (1000)     7480 2023-07-03 17:47:04.000000 piqueserver-1.1.1/piqueserver.egg-info/PKG-INFO
+-rw-r--r--   0 nota      (1000) nota      (1000)     4176 2023-07-03 17:47:04.000000 piqueserver-1.1.1/piqueserver.egg-info/SOURCES.txt
+-rw-r--r--   0 nota      (1000) nota      (1000)        1 2023-07-03 17:47:04.000000 piqueserver-1.1.1/piqueserver.egg-info/dependency_links.txt
+-rw-r--r--   0 nota      (1000) nota      (1000)       53 2023-07-03 17:47:04.000000 piqueserver-1.1.1/piqueserver.egg-info/entry_points.txt
+-rw-r--r--   0 nota      (1000) nota      (1000)      204 2023-07-03 17:47:04.000000 piqueserver-1.1.1/piqueserver.egg-info/requires.txt
+-rw-r--r--   0 nota      (1000) nota      (1000)       21 2023-07-03 17:47:04.000000 piqueserver-1.1.1/piqueserver.egg-info/top_level.txt
+drwxr-xr-x   0 nota      (1000) nota      (1000)        0 2023-07-03 17:47:04.779773 piqueserver-1.1.1/pyspades/
+-rw-r--r--   0 nota      (1000) nota      (1000)     1111 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/__init__.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     1779 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/bytes.pxd
+-rw-r--r--   0 nota      (1000) nota      (1000)     9683 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/bytes.pyx
+-rw-r--r--   0 nota      (1000) nota      (1000)     4510 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/bytes_c.cpp
+-rw-r--r--   0 nota      (1000) nota      (1000)     8890 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/classicgen_c.cpp
+-rw-r--r--   0 nota      (1000) nota      (1000)     1464 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/collision.py
+-rw-r--r--   0 nota      (1000) nota      (1000)      977 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/color.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     2409 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/common.pxd
+-rw-r--r--   0 nota      (1000) nota      (1000)    14662 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/common.pyx
+-rw-r--r--   0 nota      (1000) nota      (1000)      365 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/common_c.h
+-rw-r--r--   0 nota      (1000) nota      (1000)     2682 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/constants.py
+-rw-r--r--   0 nota      (1000) nota      (1000)      299 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/constants_c.h
+-rw-r--r--   0 nota      (1000) nota      (1000)    28609 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/contained.pyx
+-rw-r--r--   0 nota      (1000) nota      (1000)     4989 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/entities.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     5316 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/gamemodes.py
+-rw-r--r--   0 nota      (1000) nota      (1000)      886 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/loaders.pxd
+-rw-r--r--   0 nota      (1000) nota      (1000)     1400 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/loaders.pyx
+-rw-r--r--   0 nota      (1000) nota      (1000)     3132 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/mapgenerator.py
+-rw-r--r--   0 nota      (1000) nota      (1000)    20215 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/mapmaker.pyx
+-rw-r--r--   0 nota      (1000) nota      (1000)     3352 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/master.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     4943 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/packet.pyx
+-rw-r--r--   0 nota      (1000) nota      (1000)    53144 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/player.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     5776 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/protocol.py
+-rw-r--r--   0 nota      (1000) nota      (1000)    17863 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/server.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     3117 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/team.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     1654 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/tools.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     2962 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/types.py
+-rw-r--r--   0 nota      (1000) nota      (1000)     1992 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/vxl.pxd
+-rw-r--r--   0 nota      (1000) nota      (1000)     9463 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/vxl.pyx
+-rw-r--r--   0 nota      (1000) nota      (1000)    15738 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/vxl_c.cpp
+-rw-r--r--   0 nota      (1000) nota      (1000)     2358 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/vxl_c.h
+-rw-r--r--   0 nota      (1000) nota      (1000)     4406 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/weapon.py
+-rw-r--r--   0 nota      (1000) nota      (1000)    15029 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/world.pyx
+-rw-r--r--   0 nota      (1000) nota      (1000)    19626 2023-07-03 17:42:02.000000 piqueserver-1.1.1/pyspades/world_c.cpp
+-rw-r--r--   0 nota      (1000) nota      (1000)       80 2023-07-03 17:47:04.780773 piqueserver-1.1.1/setup.cfg
+-rw-r--r--   0 nota      (1000) nota      (1000)     4880 2023-07-03 17:42:02.000000 piqueserver-1.1.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `piqueserver-1.0.0/MANIFEST.in` & `piqueserver-1.1.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `piqueserver-1.0.0/PKG-INFO` & `piqueserver-1.1.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,215 +1,17 @@
 Metadata-Version: 2.1
 Name: piqueserver
-Version: 1.0.0
+Version: 1.1.1
 Summary: Open-Source server implementation for Ace of Spades 
 Home-page: https://github.com/piqueserver/piqueserver
 Author: Originally MatPow2 and PySnip contributors,now, StackOverflow and piqueserver authors
 Author-email: nate.shoffner@gmail.com
 Maintainer: noway421
 Maintainer-email: noway@2ch.hk
 License: GNU General Public License v3
-Description: piqueserver |Build Status| |Build status| |Coverage Status|
-        ===========================================================
-        
-        An Ace of Spades 0.75 server based on
-        `PySnip <https://github.com/NateShoffner/PySnip>`__.
-        
-        \:point_right: Chat with us!
-        ----------------------------
-        
-        -  Gitter: |Join the chat at https://gitter.im/piqueserver/piqueserver|
-        -  Matrix: ``#piqueserver:matrix.org`` (`Riot Webchat
-           link <https://riot.im/app/#/room/#piqueserver:matrix.org>`__)
-        -  Discord: Join with `this invite link <https://discord.gg/w6Te7xC>`__
-        -  Slack: Join with `this invite link <https://join.slack.com/t/piqueserver/shared_invite/enQtMjg5MDI3MTkwNTgxLTNhMDkyNDRkNzhiNmQyYjRkOTdjNGNkYzNhNTQ4NzZkY2JhZjQxYzIyMTQ0Y2JlYTI2ZGFjMTFmNjAwZTM2OGU>`__
-        -  IRC: (disabled due to spam) ``#piqueserver`` on freenode.net
-           (`web <http://webchat.freenode.net/?channels=%23piqueserver>`__)
-        
-        All of these are `bridged <https://matrix.org/docs/guides/faq.html#what-is-matrix>`__ together!
-        
-        \:tada: Features
-        ----------------
-        
-        -  Many administrator features
-        -  A lot of epic commands
-        -  A remote console (using SSH)
-        -  Map rotation
-        -  Map metadata (name, version, author, and map configuration)
-        -  Map extensions (water damage, etc.)
-        -  A map generator
-        -  An IRC client for managing your server
-        -  A JSON query webserver
-        -  A status server with map overview
-        -  Server/map scripts
-        -  Airstrikes
-        -  Melee attacks with the pickaxe
-        -  New gamemodes (deathmatch / runningman)
-        -  Rollback feature (rolling back to the original map)
-        -  Spectator mode
-        -  Dirt grenades
-        -  Platforms with buttons
-        -  Ban subscribe service
-        -  A ton of other features
-        
-        \:rocket: Installation
-        ----------------------
-        
-        Requirements
-        ~~~~~~~~~~~~
-        
-        Piqueserver requires python3.5.3 and above
-        
-        We currently provide builds for:
-         - Linux 32 and 64bit, Python 3.5, 3.6
-         - Windows 32 and 64bit, Python 3.5, 3.6
-         
-        If your system is not one of the above, you will also need a recent C++ Compiler.
-        
-        pip (stable version)
-        ~~~~~~~~~~~~~~~~~~~~
-        
-        .. code:: bash
-        
-            pip3 install piqueserver
-        
-        Optional features:
-        
-        - `ssh`: enable ssh manhole server support
-        - `from`: enable the `from` command to geolocate players by ip
-        
-        To install with optional features with pip:
-        
-        .. code:: bash
-        
-            pip3 install piqueserver[ssh,from]
-        
-        git (bleeding edge)
-        ~~~~~~~~~~~~~~~~~~~
-        
-        .. code:: bash
-        
-            git clone https://github.com/piqueserver/piqueserver
-            cd piqueserver
-            python3 -m venv venv
-            source venv/bin/activate
-        
-            # note: requirements.txt includes all optional deps too
-            pip install -r requirements.txt
-        
-            python setup.py install
-        
-            # now `piqueserver` will be available on the $PATH when venv active
-        
-        Arch Linux
-        ~~~~~~~~~~
-        
-        The `AUR package <https://aur.archlinux.org/packages/piqueserver-git/>`__
-        (git master) is currently broken. When it gets repaired (you can help!),
-        you'll be able to install manually or with your favourite AUR helper:
-        
-        .. code:: bash
-        
-            pacaur -S piqueserver-git
-        
-        \:rocket: Running
-        -----------------
-        
-        Then copy the default configuration as a base to work off
-        
-        .. code:: bash
-        
-            piqueserver --copy-config
-        
-        A-a-and lift off!
-        
-        .. code:: bash
-        
-            piqueserver
-        
-        Custom config location
-        ~~~~~~~~~~~~~~~~~~~~~~
-        
-        If you wish to use a different location to ``~/.config/piqueserver/``
-        for config files, specify a directory with the ``-d`` flag:
-        
-        .. code:: bash
-        
-            piqueserver --copy-config -d custom_dir
-            piqueserver -d custom_dir
-        
-        \:speech_balloon: FAQ
-        ---------------------
-        
-        What's the purpose?
-        ~~~~~~~~~~~~~~~~~~~
-        
-        The purpose of this repo is to be a continuation of PySnip.
-        
-        What if PySnip development returns?
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        Then they would merge our changes and development would be continued
-        there, I guess. The important thing is to keep AoS servers alive.
-        
-        Why should I use piqueserver instead of PySnip/PySpades?
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        -  Multi config installation
-        -  Docker support
-        -  Bug fixes
-        -  Improvements
-        -  Better anti-hacking
-        -  New scripts
-        
-        What about 0.76 support
-        ~~~~~~~~~~~~~~~~~~~~~~~
-        
-        Working with multiple versions is a pain. 0.76 will be suported in the
-        future only.
-        
-        Is that everything?
-        ~~~~~~~~~~~~~~~~~~~
-        
-        Please see also the
-        `Online Documentation <https://piqueserver.readthedocs.io/en/latest/>`__ for more
-        information (readthedocs.io has replaced our wiki).
-        
-        \:blush: Contribute
-        -------------------
-        
-        Don't be shy and submit us a PR or an issue! Help is always appreciated
-        
-        \:wrench: Development
-        ---------------------
-        
-        Use ``python3`` and ``pip`` to setup the development environment:
-        
-        .. code:: bash
-        
-            $ python3 -m venv venv && source venv/bin/activate
-            (venv) $ pip install -r requirements.txt
-            (venv) $ pip install -r dev-requirements.txt # includes dev tools
-            (venv) $ python setup.py develop             # install in-place
-            (venv) $ deactivate # Deactivate virtualenv
-        
-        --------------
-        
-        Brought to you with :heart: by the `piqueserver
-        team <https://github.com/orgs/piqueserver/people>`__.
-        
-        .. |Build Status| image:: https://travis-ci.org/piqueserver/piqueserver.svg?branch=master
-           :target: https://travis-ci.org/piqueserver/piqueserver
-        .. |Build status| image:: https://ci.appveyor.com/api/projects/status/3mayprg9le4lejmm/branch/master?svg=true
-           :target: https://ci.appveyor.com/project/piqueserver/piqueserver/branch/master
-        .. |Coverage Status| image:: https://coveralls.io/repos/github/piqueserver/piqueserver/badge.svg?branch=master
-           :target: https://coveralls.io/github/piqueserver/piqueserver?branch=master
-        .. |Join the chat at https://gitter.im/piqueserver/piqueserver| image:: https://badges.gitter.im/piqueserver/piqueserver.svg
-           :target: https://gitter.im/piqueserver/piqueserver?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
-        
 Keywords: ace of spades,aos,server,pyspades,pysnip,piqueserver
 Platform: Darwin
 Platform: Unix
 Platform: Win32
 Classifier: Intended Audience :: System Administrators
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: MacOS :: MacOS X
@@ -219,11 +21,218 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Twisted
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Games/Entertainment :: First Person Shooters
-Requires-Python: >=3.5.3
+Requires-Python: >=3.7.0
 Description-Content-Type: text/x-rst
-Provides-Extra: ssh
 Provides-Extra: from
+Provides-Extra: ssh
+License-File: LICENSE
+License-File: COPYING.txt
+
+piqueserver |Build Status| |Wheel Status| |Coverage Status|
+===========================================================
+
+An Ace of Spades 0.75 server based on
+`PySnip <https://github.com/NateShoffner/PySnip>`__.
+
+\:point_right: Chat with us!
+----------------------------
+
+-  Gitter: |Join the chat at https://gitter.im/piqueserver/piqueserver|
+-  Matrix: ``#piqueserver:matrix.org`` (`Riot Webchat
+   link <https://riot.im/app/#/room/#piqueserver:matrix.org>`__)
+-  Discord: Join with `this invite link <https://discord.gg/w6Te7xC>`__
+-  Slack: Join with `this invite link <https://join.slack.com/t/piqueserver/shared_invite/enQtMjg5MDI3MTkwNTgxLTNhMDkyNDRkNzhiNmQyYjRkOTdjNGNkYzNhNTQ4NzZkY2JhZjQxYzIyMTQ0Y2JlYTI2ZGFjMTFmNjAwZTM2OGU>`__
+-  IRC: (disabled due to spam) ``#piqueserver`` on freenode.net
+   (`web <http://webchat.freenode.net/?channels=%23piqueserver>`__)
+
+All of these are `bridged <https://matrix.org/docs/guides/faq.html#what-is-matrix>`__ together!
+
+\:tada: Features
+----------------
+
+-  Many administrator features
+-  A lot of epic commands
+-  A remote console (using SSH)
+-  Map rotation
+-  Map metadata (name, version, author, and map configuration)
+-  Map extensions (water damage, etc.)
+-  A map generator
+-  An IRC client for managing your server
+-  A JSON query webserver
+-  A status server with map overview
+-  Server/map scripts
+-  Airstrikes
+-  Melee attacks with the pickaxe
+-  New gamemodes (deathmatch / runningman)
+-  Rollback feature (rolling back to the original map)
+-  Spectator mode
+-  Dirt grenades
+-  Platforms with buttons
+-  Ban subscribe service
+-  A ton of other features
+
+\:rocket: Installation
+----------------------
+
+Requirements
+~~~~~~~~~~~~
+
+Piqueserver requires python 3.7 and above
+
+We currently provide builds for:
+ - Linux x86_64
+ - Windows x86 and x86_64
+ 
+If your system is not one of the above, you will also need a recent C++ Compiler.
+
+pip (stable version)
+~~~~~~~~~~~~~~~~~~~~
+
+.. code:: bash
+
+    pip3 install piqueserver
+
+Optional features:
+
+- `ssh`: enable ssh manhole server support
+- `from`: enable the `from` command to geolocate players by ip
+
+To install with optional features with pip:
+
+.. code:: bash
+
+    pip3 install piqueserver[ssh,from]
+
+git (bleeding edge)
+~~~~~~~~~~~~~~~~~~~
+
+.. code:: bash
+
+    git clone https://github.com/piqueserver/piqueserver
+    cd piqueserver
+    python3 -m venv venv
+    source venv/bin/activate
+
+    # note: requirements.txt includes all optional deps too
+    pip install -r requirements.txt
+
+    python setup.py install
+
+    # now `piqueserver` will be available on the $PATH when venv active
+
+Arch Linux
+~~~~~~~~~~
+
+The `AUR package <https://aur.archlinux.org/packages/piqueserver-git/>`__
+(git master) is currently broken. When it gets repaired (you can help!),
+you'll be able to install manually or with your favourite AUR helper:
+
+.. code:: bash
+
+    pacaur -S piqueserver-git
+
+\:rocket: Running
+-----------------
+
+Then copy the default configuration as a base to work off
+
+.. code:: bash
+
+    piqueserver --copy-config
+
+A-a-and lift off!
+
+.. code:: bash
+
+    piqueserver
+
+Custom config location
+~~~~~~~~~~~~~~~~~~~~~~
+
+If you wish to use a different location to ``~/.config/piqueserver/``
+for config files, specify a directory with the ``-d`` flag:
+
+.. code:: bash
+
+    piqueserver --copy-config -d custom_dir
+    piqueserver -d custom_dir
+
+\:speech_balloon: FAQ
+---------------------
+
+What's the purpose?
+~~~~~~~~~~~~~~~~~~~
+
+The purpose of this repo is to be a continuation of PySnip.
+
+What if PySnip development returns?
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Then they would merge our changes and development would be continued
+there, I guess. The important thing is to keep AoS servers alive.
+
+Why should I use piqueserver instead of PySnip/PySpades?
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+-  Multi config installation
+-  Docker support
+-  Bug fixes
+-  Improvements
+-  Better anti-hacking
+-  New scripts
+
+What about 0.76 support
+~~~~~~~~~~~~~~~~~~~~~~~
+
+Working with multiple versions is a pain. 0.76 will be suported in the
+future only.
+
+Is that everything?
+~~~~~~~~~~~~~~~~~~~
+
+Please see also the
+`Online Documentation <https://piqueserver.readthedocs.io/en/latest/>`__ for more
+information (readthedocs.io has replaced our wiki).
+
+Where can i find more scripts?
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+You can checkout the `Piqueserver Extras Repository <https://github.com/piqueserver/piqueserver-extras>`__, that contains scripts made by the community and ports from PySnip/PySpades script.
+Or in community forums, such as:
+`aloha.pk <https://aloha.pk/c/aos-modding/scripts/83>`__ and `BuildAndShoot <https://www.buildandshoot.com/forums/viewforum.php?f=19>`__
+
+\:blush: Contribute
+-------------------
+
+Don't be shy and submit us a PR or an issue! Help is always appreciated
+
+\:wrench: Development
+---------------------
+
+Use ``python3`` and ``pip`` to setup the development environment:
+
+.. code:: bash
+
+    $ python3 -m venv venv && source venv/bin/activate
+    (venv) $ pip install -r requirements.txt
+    (venv) $ pip install -r dev-requirements.txt # includes dev tools
+    (venv) $ python setup.py develop             # install in-place
+    (venv) $ deactivate # Deactivate virtualenv
+
+--------------
+
+Brought to you with :heart: by the `piqueserver
+team <https://github.com/orgs/piqueserver/people>`__.
+
+.. |Build Status| image:: https://github.com/piqueserver/piqueserver/actions/workflows/main.yml/badge.svg?branch=master
+   :target: https://github.com/piqueserver/piqueserver/actions/workflows/main.yml
+.. |Wheel Status| image:: https://github.com/piqueserver/piqueserver/actions/workflows/wheels.yml/badge.svg?branch=master
+   :target: https://github.com/piqueserver/piqueserver/actions/workflows/wheels.yml
+.. |Coverage Status| image:: https://coveralls.io/repos/github/piqueserver/piqueserver/badge.svg?branch=master
+   :target: https://coveralls.io/github/piqueserver/piqueserver?branch=master
+.. |Join the chat at https://gitter.im/piqueserver/piqueserver| image:: https://badges.gitter.im/piqueserver/piqueserver.svg
+   :target: https://gitter.im/piqueserver/piqueserver?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
```

### Comparing `piqueserver-1.0.0/README.rst` & `piqueserver-1.1.1/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-piqueserver |Build Status| |Build status| |Coverage Status|
+piqueserver |Build Status| |Wheel Status| |Coverage Status|
 ===========================================================
 
 An Ace of Spades 0.75 server based on
 `PySnip <https://github.com/NateShoffner/PySnip>`__.
 
 \:point_right: Chat with us!
 ----------------------------
@@ -43,19 +43,19 @@
 
 \:rocket: Installation
 ----------------------
 
 Requirements
 ~~~~~~~~~~~~
 
-Piqueserver requires python3.5.3 and above
+Piqueserver requires python 3.7 and above
 
 We currently provide builds for:
- - Linux 32 and 64bit, Python 3.5, 3.6
- - Windows 32 and 64bit, Python 3.5, 3.6
+ - Linux x86_64
+ - Windows x86 and x86_64
  
 If your system is not one of the above, you will also need a recent C++ Compiler.
 
 pip (stable version)
 ~~~~~~~~~~~~~~~~~~~~
 
 .. code:: bash
@@ -160,14 +160,21 @@
 Is that everything?
 ~~~~~~~~~~~~~~~~~~~
 
 Please see also the
 `Online Documentation <https://piqueserver.readthedocs.io/en/latest/>`__ for more
 information (readthedocs.io has replaced our wiki).
 
+Where can i find more scripts?
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+You can checkout the `Piqueserver Extras Repository <https://github.com/piqueserver/piqueserver-extras>`__, that contains scripts made by the community and ports from PySnip/PySpades script.
+Or in community forums, such as:
+`aloha.pk <https://aloha.pk/c/aos-modding/scripts/83>`__ and `BuildAndShoot <https://www.buildandshoot.com/forums/viewforum.php?f=19>`__
+
 \:blush: Contribute
 -------------------
 
 Don't be shy and submit us a PR or an issue! Help is always appreciated
 
 \:wrench: Development
 ---------------------
@@ -183,15 +190,15 @@
     (venv) $ deactivate # Deactivate virtualenv
 
 --------------
 
 Brought to you with :heart: by the `piqueserver
 team <https://github.com/orgs/piqueserver/people>`__.
 
-.. |Build Status| image:: https://travis-ci.org/piqueserver/piqueserver.svg?branch=master
-   :target: https://travis-ci.org/piqueserver/piqueserver
-.. |Build status| image:: https://ci.appveyor.com/api/projects/status/3mayprg9le4lejmm/branch/master?svg=true
-   :target: https://ci.appveyor.com/project/piqueserver/piqueserver/branch/master
+.. |Build Status| image:: https://github.com/piqueserver/piqueserver/actions/workflows/main.yml/badge.svg?branch=master
+   :target: https://github.com/piqueserver/piqueserver/actions/workflows/main.yml
+.. |Wheel Status| image:: https://github.com/piqueserver/piqueserver/actions/workflows/wheels.yml/badge.svg?branch=master
+   :target: https://github.com/piqueserver/piqueserver/actions/workflows/wheels.yml
 .. |Coverage Status| image:: https://coveralls.io/repos/github/piqueserver/piqueserver/badge.svg?branch=master
    :target: https://coveralls.io/github/piqueserver/piqueserver?branch=master
 .. |Join the chat at https://gitter.im/piqueserver/piqueserver| image:: https://badges.gitter.im/piqueserver/piqueserver.svg
    :target: https://gitter.im/piqueserver/piqueserver?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
```

### Comparing `piqueserver-1.0.0/piqueserver/banpublish.py` & `piqueserver-1.1.1/piqueserver/banpublish.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.0.0/piqueserver/bansubscribe.py` & `piqueserver-1.1.1/piqueserver/bansubscribe.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,22 +11,24 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with pyspades.  If not, see <http://www.gnu.org/licenses/>.
 
+import asyncio
 import json
-from twisted.internet.task import LoopingCall
-from twisted.internet.defer import DeferredList
-from twisted.web.client import getPage
+from itertools import chain
+from typing import List
+
+import aiohttp
 from twisted.logger import Logger
 
+from piqueserver.config import cast_duration, config
 from piqueserver.networkdict import NetworkDict
-from piqueserver.config import config, cast_duration
 
 log = Logger()
 
 # format is [{"ip" : "1.1.1.1", "reason : "blah"}, ...]
 
 
 def validate_bansub_config(c):
@@ -43,42 +45,47 @@
 bans_config_urls = bans_config.option('bansubscribe', default=[], validate=validate_bansub_config)
 bans_config_interval = bans_config.option('bansubscribe_interval', default="5min",
                                           cast=cast_duration)
 
 
 class BanManager:
     bans = None
-    new_bans = None
 
     def __init__(self, protocol):
         self.protocol = protocol
         self.urls = [(entry.get('url'), entry.get('whitelist')) for entry in
                      bans_config_urls.get()]
-        self.loop = LoopingCall(self.update_bans)
-        self.loop.start(bans_config_interval.get(), now=True)
 
-    def update_bans(self):
-        self.new_bans = NetworkDict()
-        defers = []
-        for url, url_filter in self.urls:
-            defers.append(getPage(url.encode('utf8')).addCallback(self.got_bans,
-                                                                  url_filter))
-        DeferredList(defers).addCallback(self.bans_finished)
-
-    def got_bans(self, data, name_filter):
-        bans = json.loads(data)
-        for entry in bans:
-            name = entry.get('name', None)
-            if name is not None and name in name_filter:
-                continue
-            self.new_bans[str(entry['ip'])] = str(entry['reason'])
-
-    def bans_finished(self, _result):
-        self.bans = self.new_bans
-        self.new_bans = None
+    async def start(self):
+        while True:
+            await self.update_bans()
+            await asyncio.sleep(bans_config_interval.get())
+
+    async def fetch_filtered_bans(self, url: str, whitelist: List[str]):
+        try:
+            async with aiohttp.ClientSession() as session:
+                async with session.get(url) as resp:
+                    # blacklist.spadille.net doesn't set json content type ¯\_(ツ)_/¯
+                    banslist = json.loads(await resp.text())
+                    return [ban for ban in banslist if ban.get('name', None) not in whitelist]
+        except Exception as e:
+            log.error("Failed to fetch bans from {url}: {err}", url=url, err=e)
+            return []
+
+    async def update_bans(self):
+        coros = []
+        for url, whitelist in self.urls:
+            coros.append(self.fetch_filtered_bans(url, whitelist))
+        log.info("fetching bans from bansubscribe urls")
+        banlists = await asyncio.gather(*coros)
+        bans = list(chain(*banlists))
+        new_bans = NetworkDict()
+        for ban in bans:
+            new_bans[ban['ip']] = ban['reason']
+        self.bans = new_bans
         log.info("successfully updated bans from bansubscribe urls")
 
     def get_ban(self, ip):
         if self.bans is None:
             return None
         try:
             return self.bans[ip]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `piqueserver-1.0.0/piqueserver/commands.py` & `piqueserver-1.1.1/piqueserver/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,39 +88,39 @@
 
 def add(func: Callable) -> None:
     """
     Function to add a command from scripts. Deprecated
     """
     warnings.warn(
         '@add is deprecated, use @command()',
-        DeprecationWarning)
+        DeprecationWarning, stacklevel=2)
     command()(func)
 
 
 def name(name: str) -> Callable:
     """
     Give the command a new name. Deprecated
     """
     warnings.warn(
         '@name is deprecated, use @command("name")',
-        DeprecationWarning)
+        DeprecationWarning, stacklevel=2)
 
     def dec(func: Callable) -> Callable:
         func.__name__ = name
         return func
     return dec
 
 
 def alias(name: str) -> Callable:
     """
     add a new alias to a command. Deprecated
     """
     warnings.warn(
         '@alias is deprecated, use @command("name", "alias1", "alias2")',
-        DeprecationWarning)
+        DeprecationWarning, stacklevel=2)
 
     def dec(func: Callable) -> Callable:
         try:
             func.aliases.append(name)
         except AttributeError:
             func.aliases = [name]
         return func
@@ -260,16 +260,16 @@
     ... @player_only
     ... def some_command(x):
     ...     pass
     """
     @functools.wraps(func)
     def _decorated(connection, *args, **kwargs):
         if connection not in connection.protocol.players.values():
-            raise CommandError("only players can't use this command")
-        func(connection, *args, **kwargs)
+            raise CommandError("only players can use this command")
+        return func(connection, *args, **kwargs)
     return _decorated
 
 def target_player(func: Callable):
     """This decorator converts first argument of a command to a `piqueserver.FeatureConnection`.
        It's intended for commands which accept single argument for target player eg. /fly [player].
        It implicitly uses invoker as target if no arguments are provided.
        It uses first argument are player name or id for targetting.
```

### Comparing `piqueserver-1.0.0/piqueserver/config/README.md` & `piqueserver-1.1.1/piqueserver/config/README.md`

 * *Files identical despite different names*

### Comparing `piqueserver-1.0.0/piqueserver/config/config.toml` & `piqueserver-1.1.1/piqueserver/config/config.toml`

 * *Files 4% similar despite different names*

```diff
@@ -164,14 +164,20 @@
 
 # time in seconds remaining when the time remaining should be announced
 time_announcements = [ 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 30, 60, 120, 180, 240, 300, 600, 900, 1200, 1800, 2400, 3000]
 
 # number of intel captures to win the game (default: 10)
 cap_limit = 10
 
+# Enable command ratelimit for preventing users abusing from command spam
+enable_command_ratelimit = true
+
+# Maximum commands to be executed in the given time
+command_ratelimit_amount = 4
+command_ratelimit_period = "5s"
 
 # Set this to true to automatically log all players in as admin on join.
 # Possibly useful for testing purposes.
 #everyone_is_admin = false
 
 [team1]
 # information about the team1
@@ -217,15 +223,15 @@
 
 # Bansubscribe allows you to inherit bans from another server with banpublish enabled.
 # `url` is the URL returning the json list, `whitelist` is a list of names which should
 # be exempt from the filter
 #bansubscribe = [
 #    { url = "http://www.blacklist.spadille.net/subscribe.json", whitelist = []},
 #]
-
+#bansubscribe_interval = "5min"
 
 
 [rights]
 # Rights allow you to specify the roles available and what permissions they have
 moderator = [
  "advancemap", "cancel", "dban", "fog",
  "from", "hackinfo", "hban",
@@ -317,18 +323,20 @@
 size = 4
 auto_squad = false
 
 
 # piqueserver.scripts.savemap
 # allows automatically saving a snapshot of the map on server close
 [savemap]
-
 # automatically load the saved map on map load
-load_saved_map = false
-
+load_saved_map = true
+# automatically save map at shutdown
+save_at_shutdown = false
+# automatically save map at map rotation or server shutdown
+always_save_map = false
 
 # piqueserver.scripts.rollback
 [rollback]
 rollback_on_game_end = false
 
 
 # piqueserver.scripts.afk
```

### Comparing `piqueserver-1.0.0/piqueserver/config/maps/random.txt` & `piqueserver-1.1.1/piqueserver/config/maps/random.txt`

 * *Files identical despite different names*

### Comparing `piqueserver-1.0.0/piqueserver/config.py` & `piqueserver-1.1.1/piqueserver/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with piqueserver.  If not, see <http://www.gnu.org/licenses/>.
 
-import collections
+from collections.abc import Mapping
 import json
 import os
 import sys
 
 import piqueserver
 import toml
 from piqueserver.utils import timeparse
@@ -33,15 +33,15 @@
 _path = os.environ.get('XDG_CONFIG_HOME', '~/.config') + '/piqueserver'
 DEFAULT_CONFIG_DIR = os.path.expanduser(_path)
 MAXMIND_DOWNLOAD = 'https://geolite.maxmind.com/download/geoip/database/GeoLite2-City.tar.gz'
 MAXMIND_DOWNLOAD_MD5 = MAXMIND_DOWNLOAD + '.md5'
 
 # (major, minor) versions of python we are supporting
 # used on startup to emit a warning if not running on a supported version
-SUPPORTED_PYTHONS = ((3, 5), (3, 6), (3, 7), (3, 8))
+SUPPORTED_PYTHONS = ((3, 7), (3, 8), (3, 9), (3, 10), (3, 11))
 
 
 class ConfigStore():
     '''
     Configuration store that manages global configuration.
 
     Usage example:
@@ -80,15 +80,15 @@
             option._validate(option.get())
         for section in self._sections.values():
             section._validate_all()
 
     # https://stackoverflow.com/a/3233356/
     def _nested_update(self, config_dict, updates):
         for k, v in updates.items():
-            if isinstance(v, collections.Mapping):
+            if isinstance(v, Mapping):
                 config_dict[k] = self._nested_update(config_dict.get(k, {}), v)
             else:
                 config_dict[k] = v
         return config_dict
 
     def get_dict(self):
         return self._raw_config
@@ -155,15 +155,15 @@
         '''
         Return the subset of the underlying dictionary that doesn't have any
         corresponding registered options.
         '''
 
         unused = {}
         for k, v in self.get_dict().items():
-            if isinstance(v, collections.Mapping):
+            if isinstance(v, Mapping):
                 if k in self._sections:
                     section_unused = self._sections[k].check_unused()
                     if section_unused:
                         unused[k] = section_unused
                 else:
                     if k not in self._options:
                         unused[k] = v
```

### Comparing `piqueserver-1.0.0/piqueserver/console.py` & `piqueserver-1.1.1/piqueserver/console.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,30 +40,27 @@
         def __init__(self, protocol):
             self.protocol = protocol
             protocol.makeConnection(self)
             self.get_input()
 
         def get_input(self):
             while msvcrt.kbhit():
-                c = msvcrt.getwch()
+                c = msvcrt.getwche()
                 if c == '\r':  # new line
                     c = '\n'
-                    stdout.write(c)
                     self.input += c
-                    self.protocol.dataReceived(self.input)
+                    self.protocol.dataReceived(self.input.encode())
                     self.input = ''
                 elif c in ('\xE0', '\x00'):
                     # ignore special characters
                     msvcrt.getwch()
                 elif c == '\x08':  # delete
                     self.input = self.input[:-1]
-                    stdout.write('\x08 \x08')
                 else:
                     self.input += c
-                    stdout.write(c)
             reactor.callLater(self.interval, self.get_input)
 
         def write(self, data):
             stdout.write(data)
 
         def writeSequence(self, seq):
             stdout.write(''.join(seq))
@@ -98,14 +95,14 @@
 
     # methods used to emulate the behaviour of regular Connection objects to
     # prevent errors when command writers didn't test that their scripts would
     # work when run on the console
     def send_chat(self, value: str, _):
         print(value)
 
-    def send_lines(self, lines: List[str]):
+    def send_lines(self, lines: List[str], type: str = None):
         print("\n".join(lines))
 
 
 def create_console(protocol):
     console = ConsoleInput(protocol)
     StandardIO(console)
```

### Comparing `piqueserver-1.0.0/piqueserver/core_commands/__init__.py` & `piqueserver-1.1.1/piqueserver/core_commands/__init__.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.0.0/piqueserver/core_commands/game.py` & `piqueserver-1.1.1/piqueserver/core_commands/game.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,73 +34,77 @@
             resetting_player = player
             if player.admin:
                 break
         if resetting_player is connection:
             return
     connection.protocol.reset_game(resetting_player)
     connection.protocol.on_game_end()
-    connection.protocol.send_chat(
+    connection.protocol.broadcast_chat(
         'Game has been reset by %s' % connection.name,
         irc=True)
 
 
 @command(admin_only=True)
 def lock(connection, value):
     """
     Make a specified team no longer joinable until it's unlocked
     /lock <blue|green|spectator>
     New players will be placed in the spectator team even if it's locked
     """
     team = get_team(connection, value)
     team.locked = True
-    connection.protocol.send_chat('%s team is now locked' % team.name)
+    connection.protocol.broadcast_chat('%s team is now locked' % team.name)
     connection.protocol.irc_say('* %s locked %s team' % (connection.name,
                                                          team.name))
 
 
 @command(admin_only=True)
 def unlock(connection, value):
     """
     Unlock a team
     /unlock <blue|green|spectator>
     """
     team = get_team(connection, value)
     team.locked = False
-    connection.protocol.send_chat('%s team is now unlocked' % team.name)
+    connection.protocol.broadcast_chat('%s team is now unlocked' % team.name)
     connection.protocol.irc_say('* %s unlocked %s team' % (connection.name,
                                                            team.name))
 
 
 @command(admin_only=True)
 @target_player
-def switch(connection, player):
+def switch(connection, player, team=None):
     """
     Switch teams either for yourself or for a given player
-    /switch [player]
+    /switch [player] [team]
     """
     protocol = connection.protocol
-    if player.team.spectator:
-        player.send_chat(
-            "The switch command can't be used on a spectating player.")
-        return
-    new_team = player.team.other
+    new_team = protocol.blue_team
+
+    if not player.team.spectator:
+        new_team = player.team.other
+
+    if team:
+        new_team = get_team(connection, team)
+
     if player.invisible:
         old_team = player.team
         player.team = new_team
         player.on_team_changed(old_team)
         player.spawn(player.world_object.position.get())
         player.send_chat('Switched to %s team' % player.team.name)
-        if connection is not player and connection in protocol.players.values():
+        if (connection is not player
+                and connection in protocol.players.values()):
             connection.send_chat('Switched %s to %s team' % (player.name,
                                                              player.team.name))
         protocol.irc_say('* %s silently switched teams' % player.name)
     else:
         player.respawn_time = protocol.respawn_time
         player.set_team(new_team)
-        protocol.send_chat('%s switched teams' % player.name, irc=True)
+        protocol.broadcast_chat('%s switched teams' % player.name, irc=True)
 
 
 @command('setbalance', admin_only=True)
 def set_balance(connection, value):
     """
     Turn automatic balancing on or off
     /setbalance <on|off>
@@ -109,19 +113,19 @@
     if should_balance is None:
         raise CommandError()
 
     protocol = connection.protocol
     protocol.balanced_teams = should_balance
 
     if should_balance:
-        protocol.send_chat('now balancing teams')
+        protocol.broadcast_chat('now balancing teams')
         connection.protocol.irc_say(
             '* %s turned on balanced teams' % connection.name)
     else:
-        protocol.send_chat('now no longer balancing teams')
+        protocol.broadcast_chat('now no longer balancing teams')
         connection.protocol.irc_say(
             '* %s turned off balanced teams' % connection.name)
 
 
 @command('togglebuild', 'tb', admin_only=True)
 def toggle_build(connection, player=None):
     """
@@ -129,24 +133,25 @@
     /togglebuild [player]
     """
     if player is not None:
         player = get_player(connection.protocol, player)
         value = not player.building
         player.building = value
         msg = '%s can build again' if value else '%s is disabled from building'
-        connection.protocol.send_chat(msg % player.name)
+        connection.protocol.broadcast_chat(msg % player.name)
         connection.protocol.irc_say('* %s %s building for %s' %
                                     (connection.name,
                                      ['disabled', 'enabled'][int(value)],
                                      player.name))
     else:
         value = not connection.protocol.building
         connection.protocol.building = value
         on_off = ['OFF', 'ON'][int(value)]
-        connection.protocol.send_chat('Building has been toggled %s!' % on_off)
+        connection.protocol.broadcast_chat(
+            'Building has been toggled %s!' % on_off)
         connection.protocol.irc_say(
             '* %s toggled building %s' % (connection.name,
                                           on_off))
 
 
 @command('togglekill', 'tk', admin_only=True)
 def toggle_kill(connection, player=None):
@@ -155,38 +160,40 @@
     /togglekill [player]
     """
     if player is not None:
         player = get_player(connection.protocol, player)
         value = not player.killing
         player.killing = value
         msg = '%s can kill again' if value else '%s is disabled from killing'
-        connection.protocol.send_chat(msg % player.name)
+        connection.protocol.broadcast_chat(msg % player.name)
         connection.protocol.irc_say('* %s %s killing for %s' %
                                     (connection.name,
-                                     ['disabled', 'enabled'][int(value)], player.name))
+                                     ['disabled', 'enabled'][int(value)],
+                                     player.name))
     else:
         value = not connection.protocol.killing
         connection.protocol.killing = value
         on_off = ['OFF', 'ON'][int(value)]
-        connection.protocol.send_chat('Killing has been toggled %s!' % on_off)
+        connection.protocol.broadcast_chat(
+            'Killing has been toggled %s!' % on_off)
         connection.protocol.irc_say(
             '* %s toggled killing %s' % (connection.name,
                                          on_off))
 
 
 @command('toggleteamkill', 'ttk', admin_only=True)
 def toggle_teamkill(connection):
     """
     Toggle friendly fire
     /toggleteamkill
     """
     value = not connection.protocol.friendly_fire
     connection.protocol.friendly_fire = value
     on_off = ['OFF', 'ON'][int(value)]
-    connection.protocol.send_chat(
+    connection.protocol.broadcast_chat(
         'Friendly fire has been toggled %s!' % on_off)
     connection.protocol.irc_say('* %s toggled friendly fire %s' % (
         connection.name, on_off))
 
 
 @command('globalchat', admin_only=True)
 def global_chat(connection, value=None):
@@ -199,15 +206,15 @@
     if enabled is True:
         connection.protocol.global_chat = True
     elif enabled is False:
         connection.protocol.global_chat = False
     else:
         connection.protocol.global_chat = not connection.protocol.global_chat
 
-    connection.protocol.send_chat(
+    connection.protocol.broadcast_chat(
         'Global chat %s' % (
             'enabled' if connection.protocol.global_chat else 'disabled'),
         irc=True)
 
 
 @command('timelimit', admin_only=True)
 def set_time_limit(connection, duration):
@@ -216,36 +223,37 @@
     /timelimit <duration>
     """
     limit = cast_duration(duration)
     span = prettify_timespan(limit)
     protocol = connection.protocol
     # takes time in minutes
     protocol.set_time_limit(limit/60)
-    protocol.send_chat('Time limit set to {}'.format(span), irc=True)
+    protocol.broadcast_chat('Time limit set to {}'.format(span), irc=True)
 
 
 @command(admin_only=True)
 def fog(connection, *args):
     """
     Set the fog color
     /fog red green blue (all values 0-255)
     /fog #aabbcc        (hex representation of rgb)
     /fog #abc           (short hex representation of rgb)
     """
-    if(len(args) == 3):
+    if (len(args) == 3):
         r = int(args[0])
         g = int(args[1])
         b = int(args[2])
-    elif(len(args) == 1 and args[0][0] == '#'):
+    elif (len(args) == 1 and args[0][0] == '#'):
         hex_code = args[0][1:]
 
         if (len(hex_code) != 3) and (len(hex_code) != 6):
             raise ValueError("Invalid hex code length")
 
-        if len(hex_code) == 3:  # it's a short hex code, turn it into a full one
+        # it's a short hex code, turn it into a full one
+        if len(hex_code) == 3:
             hex_code = (hex_code[0]*2) + (hex_code[1]*2) + (hex_code[2]*2)
 
         valid_characters = re.compile('[a-fA-F0-9]')
         for char in hex_code:
             if valid_characters.match(char) is None:
                 raise ValueError("Invalid hex code characters")
 
@@ -254,9 +262,10 @@
         b = int(hex_code[4:6], base=16)
     else:
         raise ValueError("Neither RGB or hex code provided")
 
     old_fog_color = connection.protocol.fog_color
     connection.protocol.set_fog_color((r, g, b))
     if old_fog_color == (r, g, b):
-        return 'Fog color changed successfully\nWarning: fog color set to same color as before'
+        return ('Fog color changed successfully\n'
+                'Warning: fog color set to same color as before')
     return 'Fog color changed successfully'
```

### Comparing `piqueserver-1.0.0/piqueserver/core_commands/info.py` & `piqueserver-1.1.1/piqueserver/core_commands/info.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     """
     Show you the server rules
     /rules
     """
     lines = connection.protocol.rules
     if lines is None:
         return
-    connection.send_lines(lines)
+    connection.send_lines(lines, 'rules')
 
 
 @command()
 def commands(connection):
     """
     Print all available commands
     /commands
@@ -53,15 +53,15 @@
     # More helpful output for regular players
     lines = []
     for cmd in _commands.values():
         if not has_permission(cmd, connection):
             continue
         desc, _, _ = get_command_help(cmd)
         lines.append("/{} {}".format(cmd.command_name, desc))
-    connection.send_lines(lines)
+    connection.send_lines(lines, 'commands')
 
 
 @command("help")
 def help_command(connection, command_name=None):
     """
     Gives description and usage info for a command
     /help <command_name>
@@ -71,8 +71,8 @@
         if command_name not in _commands:
             return 'Unknown command'
         command_func = _commands[command_name]
         desc, usage, _ = get_command_help(command_func)
         return 'Description: {}\n Usage: {}'.format(desc, usage)
     # Output help if present in config
     if connection.protocol.help:
-        return connection.send_lines(connection.protocol.help)
+        return connection.send_lines(connection.protocol.help, 'help')
```

### Comparing `piqueserver-1.0.0/piqueserver/core_commands/map.py` & `piqueserver-1.1.1/piqueserver/core_commands/map.py`

 * *Files 18% similar despite different names*

```diff
@@ -33,16 +33,16 @@
     maps, _map_list = parse_maps(pre_maps)
     if not maps:
         return 'Invalid map name'
 
     planned_map = maps[0]
     try:
         protocol.planned_map = check_rotation([planned_map])[0]
-        protocol.send_chat('%s changed next map to %s' %
-                           (name, planned_map), irc=True)
+        protocol.broadcast_chat('%s changed next map to %s' %
+                                (name, planned_map), irc=True)
     except MapNotFound:
         return 'Map %s not found' % (maps[0])
 
 
 @command('rotation', admin_only=True)
 def change_rotation(connection, *pre_maps):
     """
@@ -56,16 +56,16 @@
 
     if len(maps) == 0:
         return 'Usage: /rotation <map1> <map2> <map3> ...'
     try:
         protocol.set_map_rotation(maps)
     except MapNotFound as e:
         return 'Invalid map in map rotation (%s)' % e.map
-    protocol.send_chat("%s changed map rotation to %s." %
-                       (name, map_list), irc=True)
+    protocol.broadcast_chat("%s changed map rotation to %s." %
+                            (name, map_list), irc=True)
 
 
 @command('rotationadd', admin_only=True)
 def rotation_add(connection, *pre_maps):
     """
     Append a given map to the current map rotation and informs everyone on the server of it
     /rotationadd <map>
@@ -80,16 +80,16 @@
     map_list = ", ".join(maps) + map_list
     maps.extend(new_maps)
 
     try:
         protocol.set_map_rotation(maps)
     except MapNotFound as e:
         return 'Invalid map in map rotation (%s)' % e.map
-    protocol.send_chat("%s added %s to map rotation." %
-                       (name, " ".join(pre_maps)), irc=True)
+    protocol.broadcast_chat("%s added %s to map rotation." %
+                            (name, " ".join(pre_maps)), irc=True)
 
 
 @command('revertrotation', admin_only=True)
 def revert_rotation(connection):
     """
     Invert the current map rotation
     /revertrotation
@@ -97,14 +97,29 @@
     protocol = connection.protocol
     name = connection.name
     maps = protocol.config['maps']
     protocol.set_map_rotation(maps)
     protocol.irc_say("* %s reverted map rotation to %s" % (name, maps))
 
 
-@command('advancemap', admin_only=True)
+@command('advancemap', 'advance', admin_only=True)
 def advance(connection):
     """
     Force the next map to be immediately loaded instead of waiting for the time limit to end
     /advancemap
     """
     connection.protocol.advance_rotation('Map advance forced.')
+
+
+@command('loadmap', admin_only=True)
+def load_map(connection, map):
+    """
+    Instantly switches map to the specified
+    /loadmap <mapname>
+    """
+    protocol = connection.protocol
+
+    try:
+        protocol.planned_map = check_rotation([map])[0]
+        protocol.advance_rotation()
+    except MapNotFound:
+        return 'Map %s not found' % (map)
```

### Comparing `piqueserver-1.0.0/piqueserver/core_commands/moderation.py` & `piqueserver-1.1.1/piqueserver/core_commands/moderation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from random import choice
 from twisted.internet import reactor
 # aparently, we need to send packets in this file. For now, I give in.
-from pyspades.contained import CreatePlayer, SetTool, KillAction, InputData, SetColor, WeaponInput
+from pyspades.contained import (
+    CreatePlayer, SetTool, KillAction, InputData, SetColor, WeaponInput)
 from pyspades.constants import (GRENADE_KILL, FALL_KILL, NETWORK_FPS)
 from pyspades.common import (
     prettify_timespan,
     make_color)
 from piqueserver.commands import (
     command, CommandError, get_player, join_arguments, target_player)
 from piqueserver.utils import timeparse
@@ -14,16 +15,17 @@
 def has_digits(s: str) -> bool:
     return any(char.isdigit() for char in s)
 
 
 def get_ban_arguments(connection, args):
     """
     Parses duration and reason from arguments.
-    It handles duration in two ways: interger mintues and human-friendly duration.
-    It also handles cases where duration or reason are none.
+    It handles duration in two ways: interger mintues and
+    human-friendly duration. It also handles cases
+    where duration or reason are none.
     Note: It returns duration in seconds.
     """
     default_duration = connection.protocol.default_ban_time
     reason = None
     if len(args) < 1:
         return default_duration, reason
     if len(args) > 1:
@@ -163,44 +165,44 @@
 @command(admin_only=True)
 def say(connection, *arg):
     """
     Say something in chat as server message
     /say <text>
     """
     value = ' '.join(arg)
-    connection.protocol.send_chat(value)
+    connection.protocol.broadcast_chat(value)
     connection.protocol.irc_say(value)
 
 
 @command(admin_only=True)
 def mute(connection, value):
     """
     Mute a player
     /mute <player>
     """
     player = get_player(connection.protocol, value)
     if player.mute:
         return '%s is already muted' % player.name
     player.mute = True
     message = '%s has been muted by %s' % (player.name, connection.name)
-    connection.protocol.send_chat(message, irc=True)
+    connection.protocol.broadcast_chat(message, irc=True)
 
 
 @command(admin_only=True)
 def unmute(connection, value):
     """
     Unmute a player
     /unmute <player>
     """
     player = get_player(connection.protocol, value)
     if not player.mute:
         return '%s is not muted' % player.name
     player.mute = False
     message = '%s has been unmuted by %s' % (player.name, connection.name)
-    connection.protocol.send_chat(message, irc=True)
+    connection.protocol.broadcast_chat(message, irc=True)
 
 
 @command(admin_only=True)
 @target_player
 def ip(connection, player):
     """
     Get the IP of a user
@@ -314,26 +316,29 @@
     else:
         connection.god_build = False
 
     if connection.god:
         if player is None:
             return 'You have silently entered god mode'
         else:
-            # TODO: Do not send this if the specified player is the one who called the command
+            # TODO: Do not send this if the specified
+            #       player is the one who called the command
             connection.send_chat(
                 'Someone has made you silently enter godmode!')
             return 'You made ' + connection.name + ' silently enter god mode'
     else:
         if player is None:
             return 'You have silently returned to being a mere human'
         else:
-            # TODO: Do not send this if the specified player is the one who called the command
+            # TODO: Do not send this if the specified
+            #       player is the one who called the command
             connection.send_chat(
                 'Someone has made you silently return to being a mere human')
-            return 'You made ' + connection.name + ' silently return to being a mere human'
+            return ('You made ' + connection.name +
+                    ' silently return to being a mere human')
 
 
 @command(admin_only=True)
 def god(connection, player=None):
     """
     Go into god mode and inform everyone on the server of it
     /god [player]
@@ -345,15 +350,15 @@
 
     connection.god = not connection.god  # toggle godmode
 
     if connection.god:
         message = '%s entered GOD MODE!' % connection.name
     else:
         message = '%s returned to being a mere human' % connection.name
-    connection.protocol.send_chat(message, irc=True)
+    connection.protocol.broadcast_chat(message, irc=True)
 
 
 @command('godbuild', admin_only=True)
 @target_player
 def god_build(connection, player):
     """
     Place blocks that can be destroyed only by players with godmode activated
```

### Comparing `piqueserver-1.0.0/piqueserver/core_commands/movement.py` & `piqueserver-1.1.1/piqueserver/core_commands/movement.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 @command(admin_only=True)
 @target_player
 def unstick(connection, player):
     """
     Unstick yourself or another player and inform everyone on the server of it
     /unstick [player]
     """
-    connection.protocol.send_chat("%s unstuck %s" %
+    connection.protocol.broadcast_chat("%s unstuck %s" %
                                   (connection.name, player.name), irc=True)
     player.set_location_safe(player.get_location())
 
 
 @command('moves', admin_only=True)
 def move_silent(connection, *args):
     """
@@ -73,15 +73,15 @@
     if arg_count == 1 or arg_count == 3:
         # must be run by a player in this case because moving self
         if connection not in connection.protocol.players.values():
             raise ValueError("Both player and target player are required")
         player = connection.name
     # player specified
     elif arg_count == 2 or arg_count == 4:
-        if not (connection.rights.admin or connection.rights.move_others):
+        if not (connection.admin or connection.rights.move_others):
             raise PermissionDenied(
                 "moving other players requires the move_others right")
         player = args[0]
 
     player = get_player(connection.protocol, player)
 
     silent = connection.invisible or silent
@@ -94,15 +94,15 @@
     else:
         message = ('%s ' + ('silently ' if silent else '') + 'teleported %s '
                    'to location %s')
         message = message % (connection.name, player.name, position)
     if silent:
         connection.protocol.irc_say('* ' + message)
     else:
-        connection.protocol.send_chat(message, irc=True)
+        connection.protocol.broadcast_chat(message, irc=True)
 
 
 @command(admin_only=True)
 @target_player
 def where(connection, player):
     """
     Tell you the coordinates of yourself or of a given player
@@ -140,15 +140,15 @@
             ('silently ' if silent else '') + 'teleported to %s'
         message = message % (player.name, target.name)
     x, y, z = target.get_location()
     player.set_location(((x - 0.5), (y - 0.5), (z + 0.5)))
     if silent:
         connection.protocol.irc_say('* ' + message)
     else:
-        connection.protocol.send_chat(message, irc=True)
+        connection.protocol.broadcast_chat(message, irc=True)
 
 
 @command('tpsilent', 'tps', admin_only=True)
 def tpsilent(connection, player1, player2=None):
     """
     Silently teleport a player to another player
     /tpsilent [player] <target player>
```

### Comparing `piqueserver-1.0.0/piqueserver/core_commands/player.py` & `piqueserver-1.1.1/piqueserver/core_commands/player.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from piqueserver.commands import command, get_player, PermissionDenied, player_only, target_player
+from piqueserver.commands import (
+    command, get_player, PermissionDenied, player_only, target_player)
+
 
 @command("client", "cli")
 @target_player
 def client(connection, player):
     """
     Tell you information about your client or the client of a given player
     /client [player]
@@ -56,30 +58,30 @@
     else:
         if not connection.rights.kill and not connection.admin:
             raise PermissionDenied("you can't kill other players")
         player = get_player(connection.protocol, value, False)
     player.kill()
     if connection is not player:
         message = '%s killed %s' % (connection.name, player.name)
-        connection.protocol.send_chat(message, irc=True)
+        connection.protocol.broadcast_chat(message, irc=True)
 
 
 @command(admin_only=True)
 @target_player
 def heal(connection, player):
     """
     Heal and refill yourself or a given player and inform everyone on the server of this action
     /heal [player]
     """
     if connection is player:
         message = '%s was healed' % (connection.name)
     else:
         message = '%s was healed by %s' % (player.name, connection.name)
     player.refill()
-    connection.protocol.send_chat(message, irc=True)
+    connection.protocol.broadcast_chat(message, irc=True)
 
 
 @command()
 def deaf(connection, value=None):
     """
     Make you or a given player no longer receive chat messages
     /deaf [player]
```

### Comparing `piqueserver-1.0.0/piqueserver/core_commands/server.py` & `piqueserver-1.1.1/piqueserver/core_commands/server.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.0.0/piqueserver/core_commands/social.py` & `piqueserver-1.1.1/piqueserver/core_commands/social.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.0.0/piqueserver/extensions.py` & `piqueserver-1.1.1/piqueserver/extensions.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,24 +70,24 @@
         if not spec:
             log.error(
                 "{} '{}' not found in either {} directory or global scope".format(
                     script_type, script, script_dir))
             continue
         # namespace module name to avoid shadowing global modules
         # TODO: figure out if there are any right or better ways.
-        spec.name = 'piqueserver_{}_namespace_{}'.format(script_type, script)
+        spec.name = 'piqueserver._{}_namespace.{}'.format(script_type, script)
         spec.loader.name = spec.name
         # load module
         try:
             module = importlib.util.module_from_spec(spec)
             spec.loader.exec_module(module)
             script_objects.append(module)
             continue
         except Exception as e: # needs to be broad since we exec the module
-            log.error("Error while loading {} {}: {!r}".format(
+            log.failure("Error while loading {} {}: {!r}".format(
                 script_type, script, e))
 
     return script_objects
 
 
 def load_scripts_regular_extension(script_names, script_dir):
     ''' Wrapper for load function
```

### Comparing `piqueserver-1.0.0/piqueserver/game_modes/arena.py` & `piqueserver-1.1.1/piqueserver/game_modes/arena.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,48 @@
-# READ THE INSTRUCTIONS BELOW BEFORE YOU ASK QUESTIONS
+"""
+Arena, A game of team survival. The last team
+standing scores a point.
+
+A map that uses arena needs to be modified to have a starting area for each
+team. A starting area is enclosed and has a gate on it. Each block of a gate
+must have the EXACT same color to work properly. Between each rounds, the
+gate is rebuilt. The gates are destroyed simultaneously at the start of each
+round, releasing the players onto the map. Players are free to switch weapons
+between rounds.
+
+Spawn locations and gate locations MUST be present in the map metadata (map
+txt file) for arena to work properly.
+
+The spawn location/s for the green team are set by using the data from the
+``arena_green_spawns`` tuple in the extensions dictionary. Likewise, the blue
+spawn/s is set with the ``arena_blue_spawns`` key. ``arena_green_spawns`` and
+``arena_blue_spawns`` are tuples which contain tuples of spawn coordinates.
+Spawn locations are chosen randomly.
+
+.. note::
+
+    the script retains backwards compatibility With the old
+    ``arena_green_spawn`` and ``arena_blue_spawn``
+
+The ``arena_max_spawn_distance`` can be used to set ``MAX_SPAWN_DISTANCE`` on a
+map by map basis. See the comment by ``MAX_SPAWN_DISTANCE`` for more information
+
+The locations of gates is also determined in the map metadata. ``arena_gates``
+is a tuple of coordinates in the extension dictionary. Each gate needs only one
+block to be specified (since each gate is made of a uniform color)
+
+Sample extensions dictionary of an arena map with two gates: In this example
+there is one spawn location for blue and two spawn locations for green::
+
+    extensions = { 'arena': True, 'arena_blue_spawns' : ((128, 256, 60),),
+    'arena_green_spawns' : ((384, 256, 60), (123, 423, 51)), 'arena_gates':
+    ((192, 236, 59), (320, 245, 60)) }
 
-# Arena game mode written by Yourself A game of team survival. The last team
-# standing scores a point.
-
-# A map that uses arena needs to be modified to have a starting area for each
-# team. A starting area is enclosed and has a gate on it. Each block of a gate
-# must have the EXACT same color to work properly. Between each rounds, the
-# gate is rebuilt. The gates are destroyed simultaneously at the start of each
-# round, releasing the players onto the map. Players are free to switch weapons
-# between rounds.
-
-# Spawn locations and gate locations MUST be present in the map metadata (map
-# txt file) for arena to work properly.
-
-# The spawn location/s for the green team are set by using the data from the
-# 'arena_green_spawns' tuple in the extensions dictionary. Likewise, the blue
-# spawn/s is set with the 'arena_blue_spawns' key. 'arena_green_spawns' and
-# 'arena_blue_spawns' are tuples which contain tuples of spawn coordinates.
-# Spawn locations are chosen randomly.
-
-# NOTE THAT THE SCRIPT RETAINS BACKWARDS COMPATIBILITY with the old
-# 'arena_green_spawn' and 'arena_blue_spawn'
-
-# The 'arena_max_spawn_distance' can be used to set MAX_SPAWN_DISTANCE on a map
-# by map basis. See the comment by MAX_SPAWN_DISTANCE for more information
-
-# The locations of gates is also determined in the map metadata. 'arena_gates'
-# is a tuple of coordinates in the extension dictionary. Each gate needs only
-# one block to be specified (since each gate is made of a uniform color)
-
-# Sample extensions dictionary of an arena map with two gates: In this example
-# there is one spawn location for blue and two spawn locations for green.
-# extensions = { 'arena': True, 'arena_blue_spawns' : ((128, 256, 60),),
-# 'arena_green_spawns' : ((384, 256, 60), (123, 423, 51)), 'arena_gates':
-# ((192, 236, 59), (320, 245, 60)) }
+.. codeauthor:: Yourself
+"""
 
 import random
 import math
 from pyspades.contained import BlockAction, SetColor, BlockLine
 from pyspades import world
 from pyspades.constants import DESTROY_BLOCK, TEAM_CHANGE_KILL, CTF_MODE
 from twisted.internet import reactor
@@ -371,15 +376,15 @@
             green_count = get_team_alive_count(green_team)
             blue_count = get_team_alive_count(blue_team)
             if green_count > blue_count:
                 self.arena_win(green_team)
             elif green_count < blue_count:
                 self.arena_win(blue_team)
             else:
-                self.send_chat('Round ends in a tie.')
+                self.broadcast_chat('Round ends in a tie.')
             self.begin_arena_countdown()
 
         def arena_win(self, team, killer=None):
             if not self.arena_running:
                 return
             if self.arena_old_fog_color is None and TEAM_COLOR_TIME > 0:
                 self.arena_old_fog_color = self.fog_color
@@ -390,15 +395,15 @@
                     if player.world_object is not None and not player.world_object.dead:
                         killer = player
                         break
             if killer is not None:
                 self.arena_take_flag = True
                 killer.take_flag()
                 killer.capture_flag()
-            self.send_chat(team.name + ' team wins the round!')
+            self.broadcast_chat(team.name + ' team wins the round!')
             self.begin_arena_countdown()
 
         def arena_reset_fog_color(self):
             if self.arena_old_fog_color is not None:
                 # Shitty fix for disco on game end
                 self.old_fog_color = self.arena_old_fog_color
                 self.set_fog_color(self.arena_old_fog_color)
@@ -411,16 +416,16 @@
             blue_team = self.blue_team
             for team in (self.green_team, self.blue_team):
                 num = get_team_alive_count(team)
                 team.arena_message = '%i player' % num
                 if num != 1:
                     team.arena_message += 's'
                 team.arena_message += ' on ' + team.name
-            self.send_chat('%s and %s remain.' %
-                           (green_team.arena_message, blue_team.arena_message))
+            self.broadcast_chat('%s and %s remain.' %
+                                (green_team.arena_message, blue_team.arena_message))
 
         def on_map_change(self, map_):
             extensions = self.map_info.extensions
             if ALWAYS_ENABLED:
                 self.arena_enabled = True
             else:
                 if 'arena' in extensions:
@@ -472,15 +477,15 @@
                 self.arena_running = False
                 self.arena_counting_down = False
                 self.arena_limit_timer = None
                 self.arena_old_fog_color = None
                 self.old_respawn_time = None
                 self.old_building = None
                 self.old_killing = None
-            return protocol.on_map_change(self, map)
+            return protocol.on_map_change(self, map_)
 
         def build_gates(self):
             for gate in self.gates:
                 gate.build_gate()
 
         def destroy_gates(self):
             for gate in self.gates:
@@ -513,45 +518,45 @@
             self.arena_running = False
             self.arena_limit_timer = None
             self.arena_counting_down = True
             self.killing = False
             self.building = False
             self.build_gates()
             self.arena_spawn()
-            self.send_chat('The round will begin in %i seconds.' %
-                           SPAWN_ZONE_TIME)
+            self.broadcast_chat('The round will begin in %i seconds.' %
+                                SPAWN_ZONE_TIME)
             self.arena_countdown_timers = [
                 reactor.callLater(SPAWN_ZONE_TIME, self.begin_arena)]
             for time in range(1, 6):
                 self.arena_countdown_timers.append(reactor.callLater(
-                    SPAWN_ZONE_TIME - time, self.send_chat, str(time)))
+                    SPAWN_ZONE_TIME - time, self.broadcast_chat, str(time)))
 
         def delay_arena_countdown(self, amount):
             if self.arena_counting_down:
                 for timer in self.arena_countdown_timers:
                     if timer.cancelled == 0 and timer.called == 0:
                         timer.delay(amount)
 
         def begin_arena(self):
             self.arena_counting_down = False
             for team in (self.green_team, self.blue_team):
                 if team.count() == 0:
-                    self.send_chat(
+                    self.broadcast_chat(
                         'Not enough players on the %s team to begin.' %
                         team.name)
                     self.begin_arena_countdown()
                     return
             self.arena_running = True
             self.killing = True
             self.building = BUILDING_ENABLED
             self.refill_all()
             self.destroy_gates()
-            self.send_chat('Go!')
+            self.broadcast_chat('Go!')
             if MAX_ROUND_TIME > 0:
-                self.send_chat(
+                self.broadcast_chat(
                     'There is a time limit of %s for this round.' %
                     MAX_ROUND_TIME_TEXT)
                 self.arena_limit_timer = reactor.callLater(
                     MAX_ROUND_TIME, self.arena_time_limit)
 
         def on_base_spawn(self, x, y, z, base, entity_id):
             if not self.arena_enabled:
```

### Comparing `piqueserver-1.0.0/piqueserver/game_modes/babel.py` & `piqueserver-1.1.1/piqueserver/game_modes/babel.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
-babel.py last modified 2014-04-04 22:12:44
-Originally onectf.py by Yourself
-Modified to complement babel_script.py: http://aloha.pk/files/aos/pyspades/feature_server/scripts/babel_script.py
+Babel: reach the heavens by building a tower
+
+Derived from onectf.py by Yourself
 
 Release thread:
 http://www.buildandshoot.com/viewtopic.php?t=2586
 """
 
 from pyspades.constants import CTF_MODE
 from pyspades.collision import vector_collision
```

### Comparing `piqueserver-1.0.0/piqueserver/game_modes/freeforall.py` & `piqueserver-1.1.1/pyspades/team.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,90 +1,95 @@
-# Free for all script written by Yourself
-
-from random import randint
-
-from pyspades.constants import CTF_MODE
-
-# If ALWAYS_ENABLED is False, free for all can still be enabled in the map
-# metadata by setting the key 'free_for_all' to True in the extensions
-# dictionary
-ALWAYS_ENABLED = True
-
-# If WATER_SPANS is True, then players can spawn in water
-WATER_SPAWNS = False
-
-HIDE_POS = (0, 0, 63)
-
-
-def apply_script(protocol, connection, config):
-    class FreeForAllProtocol(protocol):
-        game_mode = CTF_MODE
-        free_for_all = False
-        old_friendly_fire = None
-
-        def on_map_change(self, map):
-            extensions = self.map_info.extensions
-            if ALWAYS_ENABLED:
-                self.free_for_all = True
-            else:
-                if 'free_for_all' in extensions:
-                    self.free_for_all = extensions['free_for_all']
-                else:
-                    self.free_for_all = False
-            if self.free_for_all:
-                self.old_friendly_fire = self.friendly_fire
-                self.friendly_fire = True
-            else:
-                if self.old_friendly_fire is not None:
-                    self.friendly_fire = self.old_friendly_fire
-                    self.old_friendly_fire = None
-            return protocol.on_map_change(self, map)
-
-        def on_base_spawn(self, x, y, z, base, entity_id):
-            if self.free_for_all:
-                return HIDE_POS
-            return protocol.on_base_spawn(self, x, y, z, base, entity_id)
-
-        def on_flag_spawn(self, x, y, z, flag, entity_id):
-            if self.free_for_all:
-                return HIDE_POS
-            return protocol.on_flag_spawn(self, x, y, z, flag, entity_id)
-
-    class FreeForAllConnection(connection):
-        score_hack = False
-
-        def on_spawn_location(self, pos):
-            if not self.score_hack and self.protocol.free_for_all:
-                while True:
-                    x = randint(0, 511)
-                    y = randint(0, 511)
-                    z = self.protocol.map.get_z(x, y)
-                    if z != 63 or WATER_SPAWNS:
-                        break
-                # Magic numbers taken from server.py spawn function
-                z -= 2.4
-                x += 0.5
-                y += 0.5
-                return (x, y, z)
-            return connection.on_spawn_location(self, pos)
-
-        def on_refill(self):
-            if self.protocol.free_for_all:
-                return False
-            return connection.on_refill(self)
-
-        def on_flag_take(self):
-            if self.protocol.free_for_all:
-                return False
-            return connection.on_flag_take(self)
-
-        def on_kill(self, by, type, grenade):
-            # Switch teams to add score hack
-            if by is not None and by.team is self.team and self is not by:
-                self.score_hack = True
-                pos = self.world_object.position
-                self.set_team(self.team.other)
-                self.spawn((pos.x, pos.y, pos.z))
-                self.score_hack = False
-            return connection.on_kill(self, by, type, grenade)
-
-    return FreeForAllProtocol, FreeForAllConnection
+from typing import Tuple
+from pyspades.constants import (
+    BLUE_FLAG, GREEN_FLAG,
+    CTF_MODE,
+    BLUE_BASE, GREEN_BASE,
+)
+from pyspades.entities import Flag, Base
+from pyspades.protocol import BaseProtocol
+
+
+class Team:
+    score = None
+    flag = None
+    base = None
+    other = None
+    protocol = None
+    name = None
+    kills = None
+
+    def __init__(self, team_id: int, name: str, color: Tuple[int, int, int],
+                 spectator: bool, protocol: BaseProtocol) -> None:
+        self.id = team_id
+        self.name = name
+        self.protocol = protocol
+        self.color = color
+        self.spectator = spectator
+
+    def get_players(self) -> None:
+        for player in self.protocol.players.values():
+            if player.team is self:
+                yield player
+
+    def count(self) -> int:
+        count = 0
+        for player in self.protocol.players.values():
+            if player.team is self:
+                count += 1
+        return count
+
+    def initialize(self) -> None:
+        if self.spectator:
+            return
+        self.score = 0
+        self.kills = 0
+        if self.protocol.game_mode == CTF_MODE:
+            self.set_flag()
+            self.set_base()
+
+    def set_flag(self) -> Flag:
+        entity_id = [BLUE_FLAG, GREEN_FLAG][self.id]
+        if self.flag is None:
+            self.flag = Flag(entity_id, self.protocol)
+            self.flag.team = self
+            self.protocol.entities.append(self.flag)
+        location = self.get_entity_location(entity_id)
+        returned = self.protocol.on_flag_spawn(location[0], location[1],
+                                               location[2], self.flag, entity_id)
+        if returned is not None:
+            location = returned
+        self.flag.set(*location)
+        self.flag.player = None
+        return self.flag
+
+    def set_base(self) -> Base:
+        entity_id = [BLUE_BASE, GREEN_BASE][self.id]
+        if self.base is None:
+            self.base = Base(entity_id, self.protocol)
+            self.base.team = self
+            self.protocol.entities.append(self.base)
+        location = self.get_entity_location(entity_id)
+        returned = self.protocol.on_base_spawn(location[0], location[1],
+                                               location[2], self.base, entity_id)
+        if returned is not None:
+            location = returned
+        self.base.set(*location)
+        return self.base
+
+    def get_entity_location(self, entity_id: int) -> Tuple[int, int, int]:
+        return self.get_random_location(True)
+
+    def get_random_location(self, force_land: bool = False) -> Tuple[int, int, int]:
+        x_offset = self.id * 384
+        return self.protocol.get_random_location(force_land, (
+            x_offset, 128, 128 + x_offset, 384))
+
+    def get_entities(self):
+        for item in self.protocol.entities:
+            if item.team is self:
+                yield item
+
+    def __repr__(self):
+        return "{}(id={}, name={}, color={}, spectator={}, protocol)".format(
+            self.__class__.__name__, self.id,
+            self.name, self.color, self.spectator
+        )
```

### Comparing `piqueserver-1.0.0/piqueserver/game_modes/infiltration.py` & `piqueserver-1.1.1/piqueserver/game_modes/infiltration.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 attackers, tries to infiltrate the defenders base and steal the intel.
 Defenders receive points for keeping the intel out of the attackers hands and
 attackers recieve points for capturing the intel.
 
 Options
 ^^^^^^^
 
-.. code-block:: guess
+.. code-block:: toml
+
     [infiltration]
     # Attackers get attacker_score_multiplier points for taking and capturing
     # the intel.
     attacker_score_multiplier = 10
 
     # Defenders gain 1 point for every defender_score_interval seconds that the
     # intel remains untouched.
@@ -24,15 +25,14 @@
 Originally created by: TheGrandmaster / hompy
 """
 
 from twisted.internet.reactor import callLater
 from twisted.internet.task import LoopingCall
 from pyspades import contained as loaders
 from pyspades.constants import *
-from pyspades.player import create_player, player_left, intel_capture
 
 from piqueserver.config import config, cast_duration
 
 ATTACKER_TEAM = 1  # 0 = blue, 1 = green
 
 INFIL_CONFIG = config.section("infiltration")
 ATTACKER_RATIO_OPTION = INFIL_CONFIG.option(
```

### Comparing `piqueserver-1.0.0/piqueserver/game_modes/onectf.py` & `piqueserver-1.1.1/piqueserver/game_modes/onectf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+One CTF: CTF with a single intel, placed in the center.
+"""
+
 from pyspades.constants import *
 from pyspades.collision import vector_collision
 
 FLAG_SPAWN_POS = (256, 256)
 
 HIDE_POS = (0, 0, 63)
 
@@ -45,22 +49,22 @@
                 self.onectf_reset_flags()
             return protocol.on_game_end(self)
 
         def on_map_change(self, map):
             self.one_ctf = self.reverse_one_ctf = False
             self.one_ctf_spawn_pos = FLAG_SPAWN_POS
             extensions = self.map_info.extensions
-            if ONE_CTF_MODE == ONE_CTF:
+            if "one_ctf" in extensions:
+                self.one_ctf = extensions['one_ctf']
+            elif not self.one_ctf and 'reverse_one_ctf' in extensions:
+                self.reverse_one_ctf = extensions['reverse_one_ctf']
+            elif ONE_CTF_MODE == ONE_CTF:
                 self.one_ctf = True
             elif ONE_CTF_MODE == REVERSE_ONE_CTF:
                 self.reverse_one_ctf = True
-            elif "one_ctf" in extensions:
-                self.one_ctf = extensions['one_ctf']
-            if not self.one_ctf and 'reverse_one_ctf' in extensions:
-                self.reverse_one_ctf = extensions['reverse_one_ctf']
             if 'one_ctf_spawn_pos' in extensions:
                 self.one_ctf_spawn_pos = extensions['one_ctf_spawn_pos']
             return protocol.on_map_change(self, map)
 
         def on_flag_spawn(self, x, y, z, flag, entity_id):
             pos = self.onectf_reset_flag(flag.team.other.flag)
             protocol.on_flag_spawn(self, pos[0], pos[1], pos[
```

### Comparing `piqueserver-1.0.0/piqueserver/game_modes/push.py` & `piqueserver-1.1.1/piqueserver/game_modes/push.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,58 @@
 """
-push.py last modified 2019-03-06
-Contributors: danhezee, StackOverflow, izzy, Danke, noway421, IAmYourFriend
+.. codeauthor:: danhezee, StackOverflow, izzy, Danke, noway421, IAmYourFriend
 
-The concept:
-    Each team spawns at a set location with the enemy intel. They must "push"
-    the intel towards their control point, which is also at a set location.
-    The only way to arrive there is by building bridges over the deadly water.
-    Further introduction to the game mode: https://youtu.be/DdisPY6vDD0
-
-How to setup new maps:
-    Spawn and CP locations must be configured via extensions in the map's
-    map_name.txt metadata. Example:
+The concept
+^^^^^^^^^^^
+
+Each team spawns at a set location with the enemy intel. They must "push"
+the intel towards their control point, which is also at a set location.
+The only way to arrive there is by building bridges over the deadly water.
+Further introduction to the game mode: https://youtu.be/DdisPY6vDD0
+
+
+Setting Up New Maps
+^^^^^^^^^^^^^^^^^^^
+
+Spawn and CP locations must be configured via extensions in the map's
+map_name.txt metadata:
 
 >>> extensions = {
 ...     'push': True,
 ...     'push_spawn_range' : 5,
 ...     'push_blue_spawn' : (91, 276, 59),
 ...     'push_blue_cp' : (91, 276, 59),
 ...     'push_green_spawn' : (78, 86, 59),
 ...     'push_green_cp' : (78, 86, 59),
 ...     'water_damage' : 100
 ... }
 
-Additional (but optional) extensions, to mark each teams build area and prevent
+Additional (but optional) extensions, to mark each team's build area and prevent
 the enemy from building there (and thereby helping the enemy). The build area
 is defined by x and y of upper left corner, followed by x and y of bottom right
-corner on the map. Example:
+corner on the map::
 
     'push_blue_build_area' : (64, 100, 243, 500),
     'push_green_build_area' : (268, 100, 447, 500),
 
+Commands
+^^^^^^^^
+
+* ``/r`` Quickly respawn to refill blocks and ammo (if enabled)
+* ``/resetintel <team>`` Manually reset the blue or green team's intel
+
 Options
 ^^^^^^^
 
-.. code-block:: guess
+.. code-block:: python
+
     [push]
     # Disallow removal of map blocks. This allows a larger variety of maps that
     # rely on more fragile structures. It also prevents griefing (like removing
-    # the map blocks before and after your teams bridge). Using server setting
-    # 'user_blocks_only' instead doesn't work reliable.
+    # the map blocks before and after your team's bridge).
     protect_map_blocks = true
 
     # Allow the usage of /r to quickly respawn. As players can't refill blocks at
     # their base, they would have to suicide otherwise. This is illogical, messes
     # up their kill-death ratio and gives them an undeserved punishing respawn time.
     allow_respawn_command = true
 
@@ -74,23 +84,28 @@
 from piqueserver.config import config, cast_duration
 from twisted.internet.task import LoopingCall
 from random import randint
 import colorsys
 import time
 
 PUSH_CONFIG = config.section("push")
-PROTECT_MAP_BLOCKS = PUSH_CONFIG.option("protect_map_blocks", default=True, cast=bool)
-ALLOW_RESPAWN_COMMAND = PUSH_CONFIG.option("allow_respawn_command", default=True, cast=bool)
-RESPAWN_CMD_DELAY = PUSH_CONFIG.option("respawn_cmd_delay", default="15sec", cast=cast_duration)
-INTEL_PICKUP_DELAY = PUSH_CONFIG.option("intel_pickup_delay", default="3sec", cast=cast_duration)
+PROTECT_MAP_BLOCKS = PUSH_CONFIG.option(
+    "protect_map_blocks", default=True, cast=bool)
+ALLOW_RESPAWN_COMMAND = PUSH_CONFIG.option(
+    "allow_respawn_command", default=True, cast=bool)
+RESPAWN_CMD_DELAY = PUSH_CONFIG.option(
+    "respawn_cmd_delay", default="15sec", cast=cast_duration)
+INTEL_PICKUP_DELAY = PUSH_CONFIG.option(
+    "intel_pickup_delay", default="3sec", cast=cast_duration)
 BLOCK_REMOVAL_DELAY = PUSH_CONFIG.option("block_removal_delay", default="15sec",
                                          cast=cast_duration)
 RESET_INTEL_AFTER_DROP = PUSH_CONFIG.option("reset_intel_after_drop", default="3min",
                                             cast=cast_duration)
-DEFAULT_CP_PROTECT_RANGE = PUSH_CONFIG.option("default_cp_protect_range", default=8, cast=int)
+DEFAULT_CP_PROTECT_RANGE = PUSH_CONFIG.option(
+    "default_cp_protect_range", default=8, cast=int)
 DISABLE_GRENADES_AT_SPAWN = PUSH_CONFIG.option("disable_grenades_at_spawn", default=False,
                                                cast=bool)
 
 CANT_DESTROY = "You can't destroy your team's blocks!"
 NO_BLOCKS = "Out of blocks! Refill at base or type /r"
 BUILDING_AT_CP = "You can't build near your base!"
 BUILDING_AT_ENEMY_AREA = "Don't build for your enemy!"
@@ -147,27 +162,35 @@
 def reset_intel_position(protocol, team):
     # Flag should always spawn on z-top to prevent griefers burying it under blocks
     pos = (team.other.spawn[0],
            team.other.spawn[1],
            protocol.map.get_z(team.other.spawn[0], team.other.spawn[1], 1))
     team.flag.set(*pos)  # If spawn not set, it would throw error.
     team.flag.update()
-    protocol.send_chat("The %s intel has been reset." % team.name)
+    protocol.broadcast_chat("The %s intel has been reset." % team.name)
 
 
 @command(admin_only=True)
 def resetintel(connection, value):
+    """
+    Manually reset the blue or green team's intel
+    /resetintel <team>
+    """
     team = get_team(connection, value)
     reset_intel_position(connection.protocol, team)
 
 
 @command('r')
 def respawn(connection):
+    """
+    Quickly respawn to refill blocks and ammo
+    /r
+    """
     if not ALLOW_RESPAWN_COMMAND.get():
-        return
+        return "Command is disabled"
     if connection.world_object is not None and not connection.world_object.dead:
         if (connection.last_spawn_time is None or connection.last_spawn_time +
                 RESPAWN_CMD_DELAY.get() <= get_now_in_secs()):
             if has_flag(connection):
                 connection.drop_flag()
             connection.spawn()
         else:
@@ -218,15 +241,15 @@
         def invalid_build_position(self, x, y, z):
             # prevent teams from building near their cp
             if self.is_in_invalid_area(x, y, create_area(self.team.cp[0], self.team.cp[1],
                                        self.protocol.cp_protect_range), BUILDING_AT_CP):
                 return True
             # prevent teams from building in enemy build area
             if self.team.build_area is not None and self.is_in_invalid_area(
-                        x, y, self.team.other.build_area, BUILDING_AT_ENEMY_AREA):
+                    x, y, self.team.other.build_area, BUILDING_AT_ENEMY_AREA):
                 return True
             return False
 
         def random_color(self):
             (h, l, s) = self.team.hls
             l = randint(self.team.light_range[0], self.team.light_range[1])
             color = byte_hls_to_rgb((h, l, s))
@@ -307,16 +330,18 @@
                             break
                 if is_last_block_removal:
                     continue
 
                 block_info = self.protocol.map.get_point(*block)
                 if block_info[0] is True:
                     block_hls = byte_rgb_to_hls(block_info[1])
-                    is_blue_block = compare_hs(block_hls, self.protocol.blue_team.hls)
-                    is_green_block = compare_hs(block_hls, self.protocol.green_team.hls)
+                    is_blue_block = compare_hs(
+                        block_hls, self.protocol.blue_team.hls)
+                    is_green_block = compare_hs(
+                        block_hls, self.protocol.green_team.hls)
                     is_team_block = ((self.team is self.protocol.blue_team and is_blue_block) or
                                      (self.team is self.protocol.green_team and is_green_block))
                     if is_team_block and not is_trusted:
                         self.send_chat(CANT_DESTROY)
                         return False
                     if PROTECT_MAP_BLOCKS.get() and not is_blue_block and not is_green_block:
                         return False
@@ -378,39 +403,41 @@
                     return timer_val
                 else:
                     return 0
             return timer_val
 
         def check_intel_locations(self):
             self.reset_intel_blue_timer = self.check_intel_location(
-                                              self.blue_team, self.reset_intel_blue_timer)
+                self.blue_team, self.reset_intel_blue_timer)
             self.reset_intel_green_timer = self.check_intel_location(
-                                              self.green_team, self.reset_intel_green_timer)
+                self.green_team, self.reset_intel_green_timer)
 
         def on_map_change(self, map):
             extensions = self.map_info.extensions
             for must_have in ('push_blue_spawn', 'push_green_spawn',
                               'push_blue_cp', 'push_green_cp'):
                 if must_have not in extensions:
-                    raise Exception("Missing push map metadata: %s" % must_have)
+                    raise Exception(
+                        "Missing push map metadata: %s" % must_have)
 
             extensions['water_damage'] = 100
             # distance from spawn center to randomly spawn in
             self.spawn_range = extensions.get('push_spawn_range', 5)
             # distance from cp where building is not allowed
             self.cp_protect_range = extensions.get('push_cp_protect_range',
                                                    DEFAULT_CP_PROTECT_RANGE.get())
 
             self.blue_team.spawn = extensions.get('push_blue_spawn')
             self.blue_team.cp = extensions.get('push_blue_cp')
             self.blue_team.build_area = extensions.get('push_blue_build_area')
 
             self.green_team.spawn = extensions.get('push_green_spawn')
             self.green_team.cp = extensions.get('push_green_cp')
-            self.green_team.build_area = extensions.get('push_green_build_area')
+            self.green_team.build_area = extensions.get(
+                'push_green_build_area')
 
             self.map_info.get_entity_location = get_entity_location
             self.map_info.get_spawn_location = get_spawn_location
 
             if self.check_loop is not None:
                 self.check_loop.stop()
             self.reset_intel_blue_timer = 0
```

### Comparing `piqueserver-1.0.0/piqueserver/game_modes/tow.py` & `piqueserver-1.1.1/piqueserver/game_modes/tow.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.0.0/piqueserver/irc.py` & `piqueserver-1.1.1/piqueserver/irc.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,15 +183,15 @@
 
     # methods used to emulate the behaviour of regular Connection objects to
     # prevent errors when command writers didn't test that their commands would
     # work when run from IRC
     def send_chat(self, value: str, _):
         self.send(value)
 
-    def send_lines(self, lines: List[str]):
+    def send_lines(self, lines: List[str], type: str = None):
         self.send("\n".join(lines))
 
 class IRCClientFactory(protocol.ClientFactory):
     protocol = IRCBot
     lost_reconnect_delay = 20
     failed_reconnect_delay = 60
     bot = None
```

### Comparing `piqueserver-1.0.0/piqueserver/map.py` & `piqueserver-1.1.1/piqueserver/map.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.0.0/piqueserver/networkdict.py` & `piqueserver-1.1.1/piqueserver/networkdict.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             ip = ip.supernet()
         return results
 
     def __setitem__(self, key, value):
         self.networks[ip_network(str(key), strict=False)] = value
 
     def __getitem__(self, key):
-        return self.get_entry(key)[1]
+        return self.get_entry(key)
 
     def get_entry(self, key):
         ip = ip_network(str(key))
         # See comment for remove()
         for _ in range(0, 32):
             try:
                 return self.networks[ip]
@@ -66,18 +66,21 @@
         raise KeyError(key)
 
     def __len__(self):
         return len(self.networks)
 
     def __delitem__(self, key):
         ip = ip_network(str(key), strict=False)
-        self.networks.popitem(ip)
+        self.networks.pop(ip)
 
     def pop(self, *arg, **kw):
-        network, value = self.networks.popitem(*arg, **kw)
+        if not arg or not kw:
+            network, value = self.networks.popitem()
+        else:
+            network, value = self.networks.pop(*arg, **kw)
         return get_cidr(network), value
 
     def iteritems(self):
         for network, value in self.networks.items():
             yield get_cidr(network), value
 
     def __contains__(self, key):
```

### Comparing `piqueserver-1.0.0/piqueserver/player.py` & `piqueserver-1.1.1/piqueserver/player.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,69 +1,74 @@
-import math
+import re
+import time
 from typing import List, Tuple, Optional, Union
 
 from twisted.internet import reactor
 from twisted.logger import Logger
 
 from piqueserver import commands
 from piqueserver.release import format_release
-import pyspades
 from pyspades.constants import (ERROR_BANNED, DESTROY_BLOCK, SPADE_DESTROY,
-                                GRENADE_DESTROY, ERROR_KICKED, BLOCK_TOOL)
+                                GRENADE_DESTROY, ERROR_KICKED)
 from pyspades.server import ServerConnection
-from pyspades.common import encode, escape_control_codes, prettify_timespan, Vertex3
-from pyspades.world import Character
-from pyspades.types import AttributeSet
+from pyspades.common import escape_control_codes, prettify_timespan
+from pyspades.types import AttributeSet, RateLimiter
 
 # TODO: move these where they belong
 from pyspades.team import Team
 from pyspades.world import Grenade
 CHAT_WINDOW_SIZE = 5
 CHAT_PER_SECOND = 0.5
 
 HookValue = Optional[bool]
 
 log = Logger()
 
 
 class FeatureConnection(ServerConnection):
-    printable_name = None
-    admin = False
-    last_switch = None
-    mute = False
-    deaf = False
-    login_retries = None
-    god = False
-    god_build = False
-    fly = False
-    invisible = False
-    building = True
-    killing = True
-    streak = 0
-    best_streak = 0
-    last_chat = None
-    chat_time = 0
-    chat_count = 0
-    user_types = None
-    rights = None
-    can_complete_line_build = True
+    def __init__(self, *args, **kwargs):
+        self.printable_name = None
+        self.admin = False
+        self.last_switch = None
+        self.mute = False
+        self.deaf = False
+        self.login_retries = None
+        self.god = False
+        self.god_build = False
+        self.fly = False
+        self.invisible = False
+        self.building = True
+        self.killing = True
+        self.streak = 0
+        self.best_streak = 0
+        self.chat_limiter = RateLimiter(
+            CHAT_WINDOW_SIZE, CHAT_WINDOW_SIZE / CHAT_PER_SECOND)
+        self.user_types = None
+        self.rights = None
+        self.can_complete_line_build = True
+        self.current_send_lines_types = []
+
+        super().__init__(*args, **kwargs)
+
+        self.command_limiter = RateLimiter(
+            self.protocol.command_limit_size, self.protocol.command_limit_time)
 
     def on_connect(self) -> None:
         protocol = self.protocol
         client_ip = self.address[0]
 
         if client_ip in self.protocol.bans:
             name, reason, timestamp = self.protocol.bans[client_ip]
 
             if timestamp is not None and reactor.seconds() >= timestamp:
                 protocol.remove_ban(client_ip)
                 protocol.save_bans()
             else:
-                log.info('banned user {} ({}) attempted to join'.format(name,
-                                                                        client_ip))
+                log.info('banned user {} ({}) attempted to join'
+                         .format(name, client_ip))
                 self.disconnect(ERROR_BANNED)
                 return
 
         manager = self.protocol.ban_manager
 
         if manager is not None:
             reason = manager.get_ban(client_ip)
@@ -73,15 +78,15 @@
                 self.disconnect(ERROR_BANNED)
                 return
 
         ServerConnection.on_connect(self)
 
     def on_join(self) -> None:
         if self.protocol.motd is not None:
-            self.send_lines(self.protocol.motd)
+            self.send_lines(self.protocol.motd, 'motd')
 
     def on_login(self, name: str) -> None:
         self.printable_name = escape_control_codes(name)
         if len(self.printable_name) > 15:
             self.kick(silent=True)
         log.info('{name} (IP {ip}, ID {pid}) entered the game!',
                  name=self.printable_name,
@@ -109,14 +114,23 @@
                                   (self.name, self.address[0]))
             self.protocol.player_memory.append((self.name, self.address[0]))
         else:
             log.info('{ip} disconnected', ip=self.address[0])
         ServerConnection.on_disconnect(self)
 
     def on_command(self, command: str, parameters: List[str]) -> None:
+        if not self.admin and self.protocol.command_antispam:
+            current_time = time.monotonic()
+            self.command_limiter.record_event(current_time)
+
+            if self.command_limiter.above_limit():
+                self.send_chat(
+                    "Please wait before executing your next command.")
+                return
+
         result = commands.handle_command(self, command, parameters)
 
         if result:
             for i in reversed(result.split("\n")):
                 self.send_chat(i)
 
     def _can_build(self) -> bool:
@@ -153,15 +167,15 @@
         elif self.protocol.user_blocks is not None:
             self.protocol.user_blocks.add((x, y, z))
 
     def on_block_destroy(self, x: int, y: int, z: int, mode: int) -> bool:
         map_on_block_destroy = self.protocol.map_info.on_block_destroy
         if map_on_block_destroy is not None:
             result = map_on_block_destroy(self, x, y, z, mode)
-            if result == False:
+            if not result:
                 return result
         if not self.building:
             return False
         if not self.god:
             if not self.protocol.building:
                 return False
             is_indestructable = self.protocol.is_indestructable
@@ -197,18 +211,18 @@
             return False
         elif player.god:
             if not player.invisible:
                 self.send_chat("You can't hurt %s! That player is in "
                                "*god mode*" % player.name)
             return False
         if self.god:
-            self.protocol.send_chat('%s, killing in god mode is forbidden!' %
-                                    self.name, irc=True)
-            self.protocol.send_chat('%s returned to being a mere human.' %
-                                    self.name, irc=True)
+            self.protocol.broadcast_chat(
+                '%s, killing in god mode is forbidden!' % self.name, irc=True)
+            self.protocol.broadcast_chat(
+                '%s returned to being a mere human.' % self.name, irc=True)
             self.god = False
             self.god_build = False
 
     def on_kill(self, killer: Optional['FeatureConnection'], _type: int,
                 grenade: None) -> None:
         self.streak = 0
         if killer is None or self.team is killer.team:
@@ -236,15 +250,15 @@
         if not self.protocol.fall_damage:
             return False
 
     def on_grenade(self, time_left: float) -> None:
         if self.god:
             self.refill()
 
-    def on_team_join(self, team: 'FeatureTeam') -> HookValue:
+    def on_team_join(self, team: Team) -> HookValue:
         if self.team is not None:
             if self.protocol.teamswitch_interval:
                 teamswitch_interval = self.protocol.teamswitch_interval
                 teamswitch_allowed = self.protocol.teamswitch_allowed
                 if not teamswitch_allowed:
                     self.send_chat('Switching teams is not allowed')
                     return False
@@ -287,79 +301,94 @@
                 self.protocol.irc_say(message)
             else:
                 self.send_chat('(Chat not sent - global chat disabled)')
                 return False
 
         # antispam:
         current_time = reactor.seconds()
-        if self.last_chat is None:
-            self.last_chat = current_time
-
-        else:
-            self.chat_time += current_time - self.last_chat
-
-            if self.chat_count > CHAT_WINDOW_SIZE:
-                if self.chat_count / self.chat_time > CHAT_PER_SECOND:
-                    self.mute = True
-                    self.protocol.send_chat(
-                        '%s has been muted for excessive spam' % (
-                            self.name),
-                        irc=True)
-
-                # reset if CHAT_WINDOW_SIZE messages were sent and not
-                # determined to be spam
-                self.chat_time = 0
-                self.chat_count = 0
-            else:
-                self.chat_count += 1
-            self.last_chat = current_time
+        self.chat_limiter.record_event(current_time)
+        if self.chat_limiter.above_limit():
+            self.mute = True
+            self.protocol.broadcast_chat(
+                '%s has been muted for excessive spam' % (
+                    self.name),
+                irc=True)
 
         log.info("<{name}> {message}", name=escape_control_codes(
             self.name), message=escape_control_codes(value))
 
         return value
 
     def kick(self, reason=None, silent=False):
         if not silent:
             if reason is not None:
                 message = '{} was kicked: {}'.format(self.name, reason)
             else:
                 message = '%s was kicked' % self.name
-            self.protocol.send_chat(message, irc=True)
+            self.protocol.broadcast_chat(message, irc=True)
             log.info(message)
         # FIXME: Client should handle disconnect events the same way in both
         # main and initial loading network loops
         self.disconnect(ERROR_KICKED)
 
     def ban(self, reason=None, duration=None):
         reason = ': ' + reason if reason is not None else ''
         duration = duration or None
         if duration is None:
             message = '{} permabanned{}'.format(self.name, reason)
         else:
             message = '{} banned for {}{}'.format(self.name,
                                                   prettify_timespan(duration), reason)
         if self.protocol.on_ban_attempt(self, reason, duration):
-            self.protocol.send_chat(message, irc=True)
+            self.protocol.broadcast_chat(message, irc=True)
             self.protocol.on_ban(self, reason, duration)
             if self.address[0] == "127.0.0.1":
-                self.protocol.send_chat("Ban ignored: localhost")
+                self.protocol.broadcast_chat("Ban ignored: localhost")
             else:
                 self.protocol.add_ban(self.address[0], reason, duration,
                                       self.name)
 
-    def send_lines(self, lines: List[str]) -> None:
+    def send_lines(self, lines: List[str], key: str = 'unknown') -> None:
+        """
+        Send a list of lines to the player.
+
+        'key' is a unique identifier for the lines being sent - for example,
+        a message saying '3 medkits are ready!' could use the key 'medkits.ready'.
+        The key is used to avoid sending two messages of the same variety at once,
+        to protect the server against a vulnerability which exploits this function.
+
+        The key should always be specified when calling this function. The default
+        value of 'unknown' exists simply for backwards compatibility.
+        """
+
+        # Detect if the send_lines key is already being sent to the player.
+        # If the caller of this function forgot to specify a key (thus,
+        # 'unknown' is used as per the default), we'll skip this detection.
+        if key != 'unknown':
+            if key in self.current_send_lines_types:
+                log.info(
+                    "Skipped sending lines to '{}': already being sent key "
+                    "'{}'".format(self.printable_name, key))
+                return
+
+            self.current_send_lines_types.append(key)
+
         current_time = 0
         for line in lines:
             reactor.callLater(current_time, self.send_chat, line)
             current_time += 2
 
+        reactor.callLater(current_time, self._completed_send_lines, key)
+
+    def _completed_send_lines(self, type: str) -> None:
+        self.current_send_lines_types.remove(type)
+
     def on_hack_attempt(self, reason):
-        log.warn('Hack attempt detected from {}: {}'.format(self.printable_name,
-                                                            reason))
+        log.warn('Hack attempt detected from {}: {}'
+                 .format(self.printable_name, reason))
         self.kick(reason)
 
     def on_user_login(self, user_type, verbose=True):
         log.info("'{username}' logged in as {user_type}", username=self.name,
                  user_type=user_type)
 
         if user_type == 'admin':
```

### Comparing `piqueserver-1.0.0/piqueserver/release.py` & `piqueserver-1.1.1/piqueserver/release.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.0.0/piqueserver/run.py` & `piqueserver-1.1.1/piqueserver/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,17 +3,14 @@
 import filecmp
 import shutil
 import sys
 import argparse
 import tarfile
 import json
 
-from piqueserver.config import (config, TOML_FORMAT, JSON_FORMAT,
-                                MAXMIND_DOWNLOAD, MAXMIND_DOWNLOAD_MD5,
-                                SUPPORTED_PYTHONS)
 import urllib.request
 import hashlib
 
 PKG_NAME = 'piqueserver'
 
 def get_git_rev():
     if not os.path.exists(".git"):
@@ -57,14 +54,15 @@
                 shutil.copy2(s, d)
             # skip if unchanged
             else:
                 pass
 
 
 def copy_config():
+    from piqueserver.config import config
     config_source = os.path.dirname(os.path.abspath(__file__)) + '/config'
     print('Attempting to copy example config to %s (origin: %s).' %
           (config.config_dir, config_source))
     try:
         copytree(config_source, config.config_dir)
     except Exception as e:  # pylint: disable=broad-except
         print(e)
@@ -72,14 +70,15 @@
 
     print('Complete! Please edit the files in %s to your liking.' %
           config.config_dir)
     return 0
 
 
 def update_geoip(target_dir):
+    from piqueserver.config import MAXMIND_DOWNLOAD, MAXMIND_DOWNLOAD_MD5
     db_filename = 'GeoLite2-City.mmdb'
     working_directory = os.path.join(target_dir, 'data/')
     zipped_path = os.path.join(working_directory,
                                os.path.basename(MAXMIND_DOWNLOAD))
     extracted_path = os.path.join(working_directory, db_filename)
 
     if not os.path.exists(target_dir):
@@ -120,24 +119,45 @@
     print('Cleaning up...')
     os.remove(zipped_path)
 
     return 0
 
 
 def main():
+    # We need to install the asyncio reactor before we add any imports like
+    # `twisted.internet.*` which install the default reactor.  We keep it here
+    # and not at package level to avoid installing the reactor more than once.
+    # Twisted throws an exception if you install the reactor more than once.
+    import asyncio
+
+    if sys.platform == 'win32' and sys.version_info >= (3, 7, 0):
+        # we (or twisted) do not support the ProactorEventLoop as it does not
+        # support adding file readers
+        asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
+
+    from twisted.internet import asyncioreactor
+    asyncioreactor.install(asyncio.get_event_loop())
+
+    from piqueserver.config import (config, TOML_FORMAT, JSON_FORMAT,
+                                    SUPPORTED_PYTHONS)
+
     if (sys.version_info.major, sys.version_info.minor) not in SUPPORTED_PYTHONS:
         print('Warning: you are running on an unsupported Python version.\n'
               'The server may not run correctly.\n'
               'Please see https://piqueserver.readthedocs.io/en/v1.0.0/supported-python-environments.html for more information.')
 
     description = '%s is an open-source Python server implementation ' \
                   'for the voxel-based game "Ace of Spades".' % PKG_NAME
     arg_parser = argparse.ArgumentParser(
         prog=PKG_NAME, description=description)
 
+    if not sys.warnoptions:
+        import warnings
+        warnings.filterwarnings("default", module="piqueserver[.*]")
+
     arg_parser.add_argument(
         '-c',
         '--config-file',
         default=None,
         help='specify the config file - '
         'default is "config.toml" in the config dir')
 
@@ -235,21 +255,14 @@
         print("Could not open Config file")
         print(e)
         return e.errno
 
     # update config with cli overrides
     if args.json_parameters:
         config.update_from_dict(json.loads(args.json_parameters))
-    # We need to install the asyncio reactor before 
-    # we add any imports like `twisted.internet.*` which install the default reactor.
-    # We keep it here and not at package level to avoid installing the reactor more than once.
-    # Twisted throws an exception if you install the reactor more than once.
-    import asyncio
-    from twisted.internet import asyncioreactor
-    asyncioreactor.install(asyncio.get_event_loop())
 
     from piqueserver import server
     server.run()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `piqueserver-1.0.0/piqueserver/scheduler.py` & `piqueserver-1.1.1/piqueserver/scheduler.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.0.0/piqueserver/scripts/afk.py` & `piqueserver-1.1.1/piqueserver/scripts/afk.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Kicks a player if inactive for too long.
 
 Options
 ^^^^^^^
 
-.. code-block:: guess
+.. code-block:: toml
 
    [afk]
    time_limit = "15min"
 
 .. codeauthor:: hompy
 """
```

### Comparing `piqueserver-1.0.0/piqueserver/scripts/aimbot2.py` & `piqueserver-1.1.1/piqueserver/scripts/aimbot2.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 * ``/accuracy <player>`` shows player's accuracy per weapon
 * ``/hackinfo <player>`` shows player's accuracy, K/D ratio and how often their cross-hair snaps onto another players head *admin only*
 
 Options
 ^^^^^^^
 
-.. code-block:: guess
+.. code-block:: toml
 
    [aimbot]
    collect_data = true # saves hits and shots of each weapon to a csv file
 
 .. codeauthor:: ?
 """
 import os
@@ -27,35 +27,35 @@
 
 from pyspades.constants import (
     WEAPON_TOOL, WEAPON_KILL, HEADSHOT_KILL,
     RIFLE_WEAPON, SMG_WEAPON, SHOTGUN_WEAPON,
 )
 from piqueserver.commands import command, admin, get_player
 from piqueserver.config import config
-from piqueserver.utils import parse
+from piqueserver.utils import timeparse
 
 DISABLED, KICK, BAN, WARN_ADMIN = range(4)
 
 # This controls which detection methods are enabled. If a player is detected
-# using one of these methods, the player is kicked.
+# using one of these methods, the given action is performed
 HEADSHOT_SNAP = WARN_ADMIN
 HIT_PERCENT = WARN_ADMIN
 KILLS_IN_TIME = WARN_ADMIN
 MULTIPLE_BULLETS = WARN_ADMIN
 
 # Minimum amount of time that must pass between admin warnings that are
 # triggered by the same detection method. Time is in seconds.
 WARN_INTERVAL_MINIMUM = 300
 
 # These controls are only used if banning is enabled
 # Time is given in minutes. Set to 0 for a permaban
-HEADSHOT_SNAP_BAN_DURATION = parse("23hours")
-HIT_PERCENT_BAN_DURATION = parse("1day")
-KILLS_IN_TIME_BAN_DURATION = parse("2day")
-MULTIPLE_BULLETS_BAN_DURATION = parse("1week")
+HEADSHOT_SNAP_BAN_DURATION = timeparse("23hours")
+HIT_PERCENT_BAN_DURATION = timeparse("1day")
+KILLS_IN_TIME_BAN_DURATION = timeparse("2day")
+MULTIPLE_BULLETS_BAN_DURATION = timeparse("1week")
 
 # If more than or equal to this number of weapon hit packets are received
 # from the client in half the weapon delay time, then an aimbot is detected.
 # This method of detection should have 100% detection and no false positives
 # with the current aimbot.
 # Note that the current aimbot does not modify the number of bullets
 # of the shotgun, so this method will not work if the player uses a shotgun.
```

### Comparing `piqueserver-1.0.0/piqueserver/scripts/airstrike2.py` & `piqueserver-1.1.1/piqueserver/scripts/airstrike2.py`

 * *Files 11% similar despite different names*

```diff
@@ -43,23 +43,28 @@
 ZOOMV_RAY_LENGTH = 192.0
 ARRIVAL_DELAY = 2  # seconds from airstrike notice to arrival
 
 
 @command('airstrike', 'a')
 @player_only
 def airstrike(connection, *args):
+    """
+    Triggers an airstrike. Be careful there's a large radius.
+    Aim your weapon and then hold v
+    """
     player = connection
+    kills_left = STREAK_REQUIREMENT - player.airstrike_streak
+    message = S_NO_STREAK.format(
+        streak=STREAK_REQUIREMENT, remaining=kills_left)
+
+    player.send_chat(message)
 
     if player.airstrike:
         return S_READY
 
-    kills_left = STREAK_REQUIREMENT - player.airstrike_streak
-    return S_NO_STREAK.format(streak=STREAK_REQUIREMENT,
-                              remaining=kills_left)
-
 # debug
 
 
 @command('givestrike', admin_only=True)
 @target_player
 def give_strike(connection, player):
     player.airstrike = True
@@ -112,19 +117,19 @@
         zoomv = None
         zoomv_nag = None
         last_zoomv_message = None
 
         def start_airstrike(self, x, y, z):
             coords = to_coordinates(x, y)
             message = S_ALLIED.format(player=self.name, coords=coords)
-            self.protocol.send_chat(message, global_message=False,
-                                    team=self.team)
+            self.protocol.broadcast_chat(message, global_message=False,
+                                         team=self.team)
             message = S_ENEMY.format(coords=coords)
-            self.protocol.send_chat(message, global_message=False,
-                                    team=self.team.other)
+            self.protocol.broadcast_chat(message, global_message=False,
+                                         team=self.team.other)
             self.team.last_airstrike = reactor.seconds()
 
             reactor.callLater(ARRIVAL_DELAY, self.do_airstrike, x, y, z)
 
         def do_airstrike(self, x, y, z):
             if self.name is None:
                 return
```

### Comparing `piqueserver-1.0.0/piqueserver/scripts/analyze.py` & `piqueserver-1.1.1/piqueserver/scripts/analyze.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         if connection.name in protocol.analyzers:
             del protocol.analyzers[connection.name]
             return 'You are no longer analyzing anyone.'
 
         return 'Please enter a target player to analyze.'
 
     player = get_player(protocol, player)
-    if player not in protocol.players:
+    if player.player_id not in protocol.players:
         raise ValueError("Target player is required")
 
     if connection.name in protocol.analyzers:
         if player.name == protocol.analyzers[connection.name]:
             del protocol.analyzers[connection.name]
             return 'You are no longer analyzing anyone.'
 
@@ -57,15 +57,15 @@
     class analyze_shotsConnection(connection):
         dist = ""
         weap = ""
         hs, bs, ls = 0, 0, 0
         prev_time = None
         body_part = ""
 
-        def on_hit(self, hit_amount, hit_player, type, grenade):
+        def on_unvalidated_hit(self, hit_amount, hit_player, type, grenade):
             if self.name in list(self.protocol.analyzers.values()):
                 if type == HEADSHOT_KILL or hit_amount in body_damage_values or hit_amount in limb_damage_values:
                     if not grenade:
                         dist = int(distance_3d_vector(
                             self.world_object.position, hit_player.world_object.position))
                         weap = self.weapon_object.name
                         self.pres_time = time.monotonic()
@@ -97,15 +97,15 @@
                                         counter = analyzer.ls
                                     if dt is not None:
                                         analyzer.send_chat('%s shot %s dist: %d blocks dT: %.0f ms %s %s(%d)' % (
                                             self.name, hit_player.name, dist, dt, weap, body_part, counter))
                                     else:
                                         analyzer.send_chat('%s shot %s dist: %d blocks dT: NA %s %s(%d)' % (
                                             self.name, hit_player.name, dist, weap, body_part, counter))
-            return connection.on_hit(self, hit_amount, hit_player, type, grenade)
+            return connection.on_unvalidated_hit(self, hit_amount, hit_player, type, grenade)
 
         def on_weapon_set(self, value):
             if self.name in list(self.protocol.analyzers.values()):
                 for name in self.protocol.analyzers:
                     if self.protocol.analyzers[name] == self.name:
                         analyzer = get_player(self.protocol, name)
                         analyzer.hs, analyzer.bs, analyzer.ls = 0, 0, 0
```

### Comparing `piqueserver-1.0.0/piqueserver/scripts/antijerk.py` & `piqueserver-1.1.1/piqueserver/scripts/antijerk.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Kicks jerks for 'PRESS ALT-F4 FOR AIRSTRIKES' and so on.
 
 Options
 ^^^^^^^
 
-.. code-block:: guess
+.. code-block:: toml
 
    [antijerk]
    ban_duration = "15min"
 
 .. codeauthor:: ?
 """
```

### Comparing `piqueserver-1.0.0/piqueserver/scripts/autohelp.py` & `piqueserver-1.1.1/piqueserver/scripts/autohelp.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,21 +23,21 @@
 
 def airstrike_howto_match(player, msg):
     return (not airstrike_chat_pattern.match(msg) is None)
 
 
 def apply_script(protocol, connection, config):
     def send_help_nick(connection):
-        connection.protocol.send_chat(
+        connection.protocol.broadcast_chat(
             "TO CHANGE YOUR NAME: Start Menu-> "
             "All Programs-> Ace of Spades-> Configuration")
         connection.protocol.irc_say("* Sent nick help to %s" % connection.name)
 
     def send_help_airstrike(connection):
-        connection.protocol.send_chat(
+        connection.protocol.broadcast_chat(
             "TO USE AN AIRSTRIKE: Once you have 15 points, "
             "get a 6 killstreak ->                  "
             "Then type /airstrike G4 if you want the strike to hit G4")
         connection.protocol.irc_say(
             "* Sent airstrike help to %s" % connection.name)
 
     class AutoHelpConnection(connection):
```

### Comparing `piqueserver-1.0.0/piqueserver/scripts/babel_script.py` & `piqueserver-1.1.1/piqueserver/scripts/babel_script.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 """
-babel_script.py last modified 2014-04-04 13:55:07
 Original script by Yourself
 Anti grief by izzy
 Return intel dropped from platform bug fix by a_girl
 
 Release thread:
 http://www.buildandshoot.com/viewtopic.php?t=2586
 
 How to install and configure:
 
-1) Save babel_script.py to 'scripts' folder:
-http://aloha.pk/files/aos/pyspades/feature_server/scripts/babel_script.py
-2) Save babel.py to 'scripts' folder:
-http://aloha.pk/files/aos/pyspades/feature_server/scripts/babel.py
-3) Set game_mode to "babel" in config.txt
-4) Add "babel_script" to scripts list in config.txt
-5) Set cap_limit to "10" in config.txt
+1) Set game_mode to "piqueserver.game_mode.babel" in config.txt
+2) Add "piqueserver.scripts.babel_script" to scripts list in config.txt
+3) Set cap_limit to "10" in config
 """
 
 from random import randint
 from pyspades.constants import (BLUE_BASE, GREEN_BASE, BLUE_FLAG, GREEN_FLAG,
                                 SPADE_TOOL, GRENADE_TOOL, WEAPON_TOOL)
 from twisted.internet import reactor
 
-# If ALWAYS_ENABLED is False, then babel can be enabled by setting 'babel': True
+# If ALWAYS_ENABLED is False, then babel
+# can be enabled by setting 'babel': True
 # in the map metadat extensions dictionary.
 ALWAYS_ENABLED = True
 
 PLATFORM_WIDTH = 100
 PLATFORM_HEIGHT = 32
 PLATFORM_COLOR = (0, 255, 255, 255)
 BLUE_BASE_COORDS = (256 - 138, 256)
@@ -63,18 +59,19 @@
 def coord_on_platform(x, y, z):
     if z <= 2:
         if (256 - PLATFORM_WIDTH <= x <= 256 + PLATFORM_WIDTH and
                 256 - PLATFORM_HEIGHT <= y <= 256 + PLATFORM_HEIGHT):
             return True
     if z == 1:
         if (256 - PLATFORM_WIDTH - 1 <= x <= 256 + PLATFORM_WIDTH + 1
-            and 256 - PLATFORM_HEIGHT - 1 <= y <= 256 + PLATFORM_HEIGHT + 1):
+                and 256 - PLATFORM_HEIGHT - 1 <= y <= 256 + PLATFORM_HEIGHT + 1):
             return True
     return False
 
+
 def apply_script(protocol, connection, config):
     allowed_intel_hold_time = config.get('allowed_intel_hold_time', 150)
 
     class TowerOfBabelConnection(connection):
         def get_protected_area(self, team):
             """returns minx, maxx, miny, maxy"""
             if team is self.protocol.blue_team:
@@ -105,47 +102,57 @@
         def on_line_build_attempt(self, points):
             for point in points:
                 if self.invalid_build_position(*point):
                     return False
             return connection.on_line_build_attempt(self, points)
 
         def is_trusted_for_block_destruction(self):
-            return self.admin or self.user_types.moderator or self.user_types.guard or self.user_types.trusted
+            return (self.admin or
+                    self.user_types.moderator or
+                    self.user_types.guard or
+                    self.user_types.trusted)
 
         # anti team destruction
         def on_block_destroy(self, x, y, z, mode):
             minx, maxx, miny, maxy = self.get_protected_area(self.team.other)
 
             position = self.world_object.position
 
-            if not self.is_trusted_for_block_destruction() and self.tool is SPADE_TOOL:
+            if (not self.is_trusted_for_block_destruction() and
+                    self.tool is SPADE_TOOL):
                 if minx <= position.x <= maxx and miny <= position.y <= maxy:
-                    self.send_chat('You can\'t destroy your team\'s blocks in this area. Attack the enemy\'s tower!')
+                    self.send_chat(
+                        'You can\'t destroy your team\'s'
+                        'blocks in this area. Attack the enemy\'s tower!')
                     return False
 
             if self.team is self.protocol.blue_team:
                 can_shoot_blocks = position.x <= 288
             else:
                 can_shoot_blocks = position.x >= 224
 
             if can_shoot_blocks:
                 if self.tool is WEAPON_TOOL:
-                    self.send_chat('You must be closer to the enemy\'s base to shoot blocks!')
+                    self.send_chat(
+                        'You must be closer to the enemy\'s'
+                        'base to shoot blocks!')
                 else:
-                    self.send_chat('You must be closer to the enemy\'s base to grenade blocks!')
+                    self.send_chat(
+                        'You must be closer to the enemy\'s'
+                        'base to grenade blocks!')
                 return False
             return connection.on_block_destroy(self, x, y, z, mode)
 
         auto_kill_intel_hog_call = None
 
         # kill intel carrier if held too long
         def auto_kill_intel_hog(self):
             self.auto_kill_intel_hog_call = None
             self.kill()
-            self.protocol.send_chat(
+            self.protocol.broadcast_chat(
                 'God punished %s for holding the intel too long' %
                 (self.name))
 
         def restore_default_fog_color(self):
             self.protocol.set_fog_color(
                 getattr(self.protocol.map_info.info, 'fog', (128, 232, 255)))
 
@@ -163,15 +170,17 @@
                 self.protocol.set_fog_color(
                     getattr(self.protocol.map_info.info, 'fog', (0, 255, 0)))
             reactor.callLater(0.25, self.restore_default_fog_color)
             return connection.on_flag_take(self)
 
         # return intel to platform if dropped
         def on_flag_drop(self):
-            x, y, z = self.world_object.position.x, self.world_object.position.y, self.world_object.position.z
+            x = self.world_object.position.x
+            y = self.world_object.position.y
+            z = self.world_object.position.z
             if self.auto_kill_intel_hog_call is not None:
                 self.auto_kill_intel_hog_call.cancel()
                 self.auto_kill_intel_hog_call = None
             if z >= 0:
                 self.reset_flag()
             elif (x >= (256 + PLATFORM_WIDTH)) or (x < (256 - PLATFORM_WIDTH)):
                 self.reset_flag()
@@ -180,15 +189,16 @@
             self.protocol.set_fog_color(
                 getattr(self.protocol.map_info.info, 'fog', (255, 0, 0)))
             reactor.callLater(0.25, self.restore_default_fog_color)
             return connection.on_flag_drop(self)
 
         def reset_flag(self):
             self.protocol.onectf_reset_flags()
-            self.protocol.send_chat('The intel has returned to the heavens')
+            self.protocol.broadcast_chat(
+                'The intel has returned to the heavens')
 
         def on_flag_capture(self):
             if self.auto_kill_intel_hog_call is not None:
                 self.auto_kill_intel_hog_call.cancel()
                 self.auto_kill_intel_hog_call = None
             return connection.on_flag_capture(self)
```

### Comparing `piqueserver-1.0.0/piqueserver/scripts/badmin.py` & `piqueserver-1.1.1/piqueserver/scripts/badmin.py`

 * *Files 5% similar despite different names*

```diff
@@ -188,24 +188,20 @@
          ttr,
          enemy_harmed,
          gscore))
     return gscore
 
 
 def check_percent(self):
-    # TODO: uncomment this when you find out what/where semi_hits and
-    #       semi_count should be defined. Possibly in aimbot2.py, but currently these
-    #       attributes don't exist anywhere
-    # if self.weapon == RIFLE_WEAPON:
-    #     if self.semi_hits == 0 or self.semi_count == 0:
-    #         return 0
-    #     else:
-    #         return (float(self.semi_hits) / float(self.semi_count)) * 100
-    # elif self.weapon == SMG_WEAPON:
-    if self.weapon == SMG_WEAPON:
+    if self.weapon == RIFLE_WEAPON:
+        if self.rifle_hits == 0 or self.rifle_count == 0:
+            return 0
+        else:
+            return (float(self.rifle_hits) / float(self.rifle_count)) * 100
+    elif self.weapon == SMG_WEAPON:
         if self.smg_hits == 0 or self.smg_count == 0:
             return 0
         else:
             return (float(self.smg_hits) / float(self.smg_count)) * 100
     elif self.weapon == SHOTGUN_WEAPON:
         if self.shotgun_hits == 0 or self.shotgun_count == 0:
             return 0
@@ -226,15 +222,15 @@
             (connection.name, punishment, reason))
         if punishment == "ban":
             connection.ban('@Badmin: ' + reason,
                            connection.protocol.votekick_ban_duration)
         elif punishment == "kick":
             connection.kick('@Badmin: ' + reason)
         elif punishment == "warn":
-            connection.protocol.send_chat(
+            connection.protocol.broadcast_chat(
                 " @Badmin: Hey %s, %s" % (connection.name, reason))
 
     class BadminConnection(connection):
 
         def on_chat(self, value, global_message):
             if slur_match(self, value) and LANGUAGE_FILTER_ENABLED:
                 reactor.callLater(1.0, send_slur_nick, self)
```

### Comparing `piqueserver-1.0.0/piqueserver/scripts/blockinfo.py` & `piqueserver-1.1.1/piqueserver/scripts/blockinfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ^^^^^^^^
 
 * ``/griefcheck or /gc <player> <minutes>`` gives you when, how many and whos blocks a player destroyed *admin only*
 
 Options
 ^^^^^^^
 
-.. code-block:: guess
+.. code-block:: toml
 
    [blockinfo]
    griefcheck_on_votekick = true
    irc_only = false
 
 .. codeauthor:: hompy
 """
@@ -24,15 +24,16 @@
 from twisted.internet.reactor import seconds
 from pyspades.collision import distance_3d_vector
 from pyspades.common import prettify_timespan
 from piqueserver.commands import command, admin, get_player
 from piqueserver.config import config
 
 blockinfo_config = config.section("blockinfo")
-GRIEFCHECK_ON_VOTEKICK = blockinfo_config.option("griefcheck_on_votekick", True)
+GRIEFCHECK_ON_VOTEKICK = blockinfo_config.option(
+    "griefcheck_on_votekick", True)
 IRC_ONLY = blockinfo_config.option("irc_only", False)
 
 
 @command('griefcheck', 'gc')
 def grief_check(connection, player, minutes=2):
     player = get_player(connection.protocol, player)
     protocol = connection.protocol
@@ -155,15 +156,15 @@
             self.block_info = None
             protocol.on_map_change(self, map)
 
         def on_votekick_start(self, instigator, victim, reason):
             result = protocol.on_votekick_start(
                 self, instigator, victim, reason)
             if result is None and GRIEFCHECK_ON_VOTEKICK.get():
-                message = grief_check(instigator, victim.name)
+                message = grief_check(instigator, "#%i" % victim.player_id)
                 if IRC_ONLY.get():
                     self.irc_say('* ' + message)
                 else:
-                    self.send_chat(message, irc=True)
+                    self.broadcast_chat(message, irc=True)
             return result
 
     return BlockInfoProtocol, BlockInfoConnection
```

### Comparing `piqueserver-1.0.0/piqueserver/scripts/daycycle.py` & `piqueserver-1.1.1/piqueserver/scripts/daycycle.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,35 +98,35 @@
             self.next_color()
             if not self.daycycle_loop.running:
                 self.daycycle_loop.start(self.day_update_frequency)
 
         def update_day_color(self):
             if self.current_time >= 24.00:
                 self.current_time = wrap(0.00, 24.00, self.current_time)
-            while (self.current_time < self.start_time or
+            while (self.current_time < self.daycycle_start_time or
                    self.current_time >= self.target_time):
                 self.next_color()
                 self.target_time = self.target_time or 24.00
-            t = ((self.current_time - self.start_time) /
-                 (self.target_time - self.start_time))
+            t = ((self.current_time - self.daycycle_start_time) /
+                 (self.target_time - self.daycycle_start_time))
             if self.hsv_transition:
                 new_color = interpolate_hsb(self.start_color,
                                             self.target_color, t)
                 new_color = hsb_to_rgb(*new_color)
             else:
                 new_color = interpolate_rgb(self.start_color,
                                             self.target_color, t)
             if (self.current_color is None or
                     rgb_distance(self.current_color, new_color) > 3):
                 self.current_color = new_color
                 self.set_fog_color(self.current_color)
             self.current_time += self.time_step * self.time_multiplier
 
         def next_color(self):
-            self.start_time, self.start_color, _ = (
+            self.daycycle_start_time, self.start_color, _ = (
                 self.day_colors[self.target_color_index])
             self.target_color_index = ((self.target_color_index + 1) %
                                        len(self.day_colors))
             self.target_time, self.target_color, self.hsv_transition = (
                 self.day_colors[self.target_color_index])
             if not self.hsv_transition:
                 self.start_color = hsb_to_rgb(*self.start_color)
```

### Comparing `piqueserver-1.0.0/piqueserver/scripts/demolitionman.py` & `piqueserver-1.1.1/piqueserver/scripts/demolitionman.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 @command(admin_only=True)
 def toggledemo(connection):
     connection.protocol.demolitionEnabled = not connection.protocol.demolitionEnabled
     message = 'Demolition is now disabled'
     if connection.protocol.demolitionEnabled:
         message = 'Demolition is now enabled'
-    connection.protocol.send_chat(message, irc=True)
+    connection.protocol.broadcast_chat(message, irc=True)
     return 'ok :)'
 
 
 def apply_script(protocol, connection, config):
     class DemolitionProtocol(protocol):
         demolitionEnabled = DEMOLITION_ENABLED_AT_ROUND_START
```

### Comparing `piqueserver-1.0.0/piqueserver/scripts/dirtnade.py` & `piqueserver-1.1.1/piqueserver/scripts/dirtnade.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.0.0/piqueserver/scripts/disco.py` & `piqueserver-1.1.1/piqueserver/scripts/disco.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
         def toggle_disco(self, message=False):
             self.disco = not self.disco
             if self.disco:
                 self.old_fog_color = self.fog_color
                 self.disco_loop.start(0.3)
                 if message:
-                    self.send_chat('DISCO PARTY MODE ENABLED!')
+                    self.broadcast_chat('DISCO PARTY MODE ENABLED!')
             else:
                 self.disco_loop.stop()
                 if self.old_fog_color is not None:
                     self.set_fog_color(self.old_fog_color)
                 if message:
-                    self.send_chat('The party has been stopped.')
+                    self.broadcast_chat('The party has been stopped.')
     return DiscoProtocol, connection
```

### Comparing `piqueserver-1.0.0/piqueserver/scripts/flagreturn.py` & `piqueserver-1.1.1/piqueserver/scripts/flagreturn.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,15 +25,15 @@
             if self.protocol.game_mode == CTF_MODE:
                 flag = self.team.flag
                 if flag.player is None and flag.out:
                     if vector_collision(self.world_object.position, flag):
                         flag.out = False
                         flag.set(*flag.start)
                         flag.update()
-                        self.protocol.send_chat('%s intel was returned by %s!' % (
+                        self.protocol.broadcast_chat('%s intel was returned by %s!' % (
                             self.team.name, self.name), global_message=None)
             return connection.on_position_update(self)
 
     class ReturnProtocol(protocol):
 
         def set_map(self, map):
             protocol.set_map(self, map)
```

### Comparing `piqueserver-1.0.0/piqueserver/scripts/geoip.py` & `piqueserver-1.1.1/piqueserver/scripts/geoip.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 '''
 Gets a player's location info using a geoip database.
 Location is formatted as a list of regions ordered by hierarchy (i.e. City, Region, Country)
 
 .. note::
-  This script depends on `geoip2` package and `piqueserver --update-geoip` needs to be executed after installing the package.
+
+  This script depends on ``geoip2`` package and ``piqueserver --update-geoip``
+  needs to be executed after installing the package.
 
 Commands
 ^^^^^^^^
-* ``/from ``         get active player's location
+* ``/from``         get active player's location
 * ``/from <player>`` get player's location info
 
 .. codeauthor:: ?
 '''
 
 import os
 from piqueserver.commands import (command, restrict, get_player, target_player)
```

### Comparing `piqueserver-1.0.0/piqueserver/scripts/grownade.py` & `piqueserver-1.1.1/piqueserver/scripts/grownade.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 You can adjust FLYING_MODELS and GROW_ON_WATER to allow growing in the air and
 on water, respectively. These are disabled by default so you can fly high and
 sprinkle tree-growing grenades without worrying about unseemly oddities.
 
 Options
 ^^^^^^^
 
-.. code-block:: guess
+.. code-block:: toml
 
     [grownade]
 
     flying_models = False # if False grenades exploding in midair will be ignored
     grow_on_water = False # if False grenades exploding in water will do nothing
 
 .. codeauthor:: hompy
```

### Comparing `piqueserver-1.0.0/piqueserver/scripts/map_extensions.py` & `piqueserver-1.1.1/piqueserver/scripts/map_extensions.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.0.0/piqueserver/scripts/mapmakingtools.py` & `piqueserver-1.1.1/piqueserver/scripts/mapmakingtools.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.0.0/piqueserver/scripts/markers.py` & `piqueserver-1.1.1/piqueserver/scripts/markers.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,27 +81,30 @@
 
 @command('togglemarkers', admin_only=True)
 def toggle_markers(connection, player=None):
     protocol = connection.protocol
     if player is not None:
         player = get_player(protocol, player)
         player.allow_markers = not player.allow_markers
-        message = S_PLAYER_ENABLED if player.allow_markers else S_PLAYER_DISABLED
+        message = S_PLAYER_ENABLED
+        if not player.allow_markers:
+            message = S_PLAYER_DISABLED
+
         message = message.format(player=player.name)
-        protocol.send_chat(message, irc=True)
+        protocol.broadcast_chat(message, irc=True)
     else:
         protocol.allow_markers = not protocol.allow_markers
         message = S_ENABLED if protocol.allow_markers else S_DISABLED
-        connection.protocol.send_chat(message, irc=True)
+        connection.protocol.broadcast_chat(message, irc=True)
 
 
 @command()
 @player_only
 def markers(connection):
-    connection.send_lines(S_HELP)
+    connection.send_lines(S_HELP, 'markers_help')
 
 
 class BaseMarker():
     name = 'Marker'
     triggers = []
     background = None
     background_class = None
@@ -248,15 +251,15 @@
     width, height = len(rows[0]), len(rows)
 
     # offset of the top left to the center
     off_x, off_y = -width // 2, -height // 2
 
     for y, row in enumerate(rows):
         # if anyone understands this code, tell us
-        columns = [''.join(l[y:]).split('.', 1)[0] for l in zip(*rows)]
+        columns = [''.join(a[y:]).split('.', 1)[0] for a in zip(*rows)]
         it = enumerate(columns)
         for x, column in it:
             h = len(row[x:].split('.', 1)[0])
             v = len(column)
             if h == v == 0:
                 continue
             if max(h, v) == 1:
@@ -636,21 +639,23 @@
 def apply_script(protocol, connection, config):
     class MarkerConnection(connection):
         allow_markers = True
         last_marker = None
         sneak_presses = None
 
         def send_markers(self):
-            def is_self(player): return player is self
+            def is_self(player):
+                return player is self
             send_me = partial(self.protocol.broadcast_contained, rule=is_self)
             for marker in self.protocol.markers:
                 marker.build(send_me)
 
         def destroy_markers(self):
-            def is_self(player): return player is self
+            def is_self(player):
+                return player is self
             send_me = partial(self.protocol.broadcast_contained, rule=is_self)
             for marker in self.protocol.markers:
                 marker.destroy(send_me)
 
         def make_marker(self, marker_class, location):
             marker_max = marker_class.maximum_instances
             if (marker_max is not None and
@@ -661,15 +666,16 @@
             self.last_marker = seconds()
 
         def on_animation_update(self, jump, crouch, sneak, sprint):
             markers_allowed = (VV_ENABLED and self.allow_markers and
                                self.protocol.allow_markers)
             if markers_allowed and sneak and self.world_object.sneak != sneak:
                 now = seconds()
-                if self.last_marker is None or now - self.last_marker > COOLDOWN:
+                if (self.last_marker is None or
+                        now - self.last_marker > COOLDOWN):
                     presses = self.sneak_presses
                     presses.append(now)
                     if len(presses) == 2 and presses[0] >= now - VV_TIMEFRAME:
                         location = self.get_there_location()
                         if location:
                             coords = to_coordinates(*location)
                             chat_message = ChatMessage()
```

### Comparing `piqueserver-1.0.0/piqueserver/scripts/match.py` & `piqueserver-1.1.1/piqueserver/scripts/match.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,42 +99,42 @@
             self.send_message_loop = LoopingCall(self.display_messages)
             self.send_message_loop.start(3)
 
         def start_timer(self, end):
             if self.timer_end is not None:
                 return 'Timer is running already.'
             self.timer_end = reactor.seconds() + end
-            self.send_chat('Timer started, ending in %s minutes' % (end / 60),
-                           irc=True)
+            self.broadcast_chat('Timer started, ending in %s minutes'
+                                % (end / 60), irc=True)
             self.display_timer(True)
 
         def stop_timer(self):
             if self.timer_call is not None:
                 self.timer_call.cancel()
-                self.send_chat('Timer stopped.')
+                self.broadcast_chat('Timer stopped.')
                 self.timer_call = None
             else:
                 return 'No timer in progress.'
 
         def display_timer(self, silent=False):
             time_left = self.timer_end - reactor.seconds()
             minutes_left = time_left / 60.0
             next_call = 60
             if not silent:
                 if time_left <= 0:
-                    self.send_chat('Timer ended!', irc=True)
+                    self.broadcast_chat('Timer ended!', irc=True)
                     self.timer_end = None
                     return
                 elif minutes_left <= 1:
-                    self.send_chat('%s seconds left' % int(time_left),
-                                   irc=True)
+                    self.broadcast_chat('%s seconds left' % int(time_left),
+                                        irc=True)
                     next_call = max(1, int(time_left / 2.0))
                 else:
-                    self.send_chat('%s minutes left' % int(minutes_left),
-                                   irc=True)
+                    self.broadcast_chat('%s minutes left' % int(minutes_left),
+                                        irc=True)
             self.timer_call = reactor.callLater(next_call, self.display_timer)
 
         def display_messages(self):
             if not self.messages:
                 return
             message = self.messages.pop(0)
             self.irc_say(message)
```

### Comparing `piqueserver-1.0.0/piqueserver/scripts/medkit.py` & `piqueserver-1.1.1/piqueserver/scripts/medkit.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ^^^^^^^^
 
 * ``/medkit or /m`` utilizes available medkits to heal
 
 Options
 ^^^^^^^
 
-.. code-block:: guess
+.. code-block:: toml
 
    [medkit]
    medkits = 1 # no. of medkits
    medkit_heal_amount = 40 # how much hp. it gives
 
 .. codeauthor:: Booboorocks998 & mat^2
 """
@@ -24,21 +24,25 @@
 
 medkit_config = config.section("medkit")
 default_medkits = medkit_config.option("medkits", 1)
 medkit_heal_amount = medkit_config.option("medkit_heal_amount", 40)
 
 @command('medkit', 'm')
 def medkit(connection):
-    if connection.medkits and connection.hp < 100:
-        connection.set_hp(connection.hp + connection.protocol.heal_amount,
-                          kill_type=FALL_KILL)
-        connection.medkits -= 1
-        connection.send_chat('You have been healed')
-    else:
-        connection.send_chat("You don't have any medkits or have full health!")
+    if not connection.medkits:
+        connection.send_chat("You don't have any medkits")
+        return
+    if connection.hp >= 100:
+        connection.send_chat("You already have full health!")
+        return
+
+    connection.set_hp(connection.hp + connection.protocol.heal_amount,
+                      kill_type=FALL_KILL)
+    connection.medkits -= 1
+    connection.send_chat('You have been healed')
 
 
 def apply_script(protocol, connection, config):
     class MedkitConnection(connection):
         medkits = 0
 
         def on_spawn(self, pos):
```

### Comparing `piqueserver-1.0.0/piqueserver/scripts/memcheck.py` & `piqueserver-1.1.1/piqueserver/scripts/memcheck.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.0.0/piqueserver/scripts/minefield.py` & `piqueserver-1.1.1/piqueserver/scripts/minefield.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,24 +35,24 @@
 ...     ]
 ... }
 
 .. codeauthor:: learn_more (MIT LICENSE)
 """
 # todo: reset intel in minefield
 
+from random import choice
+from piqueserver.commands import command, admin
+from twisted.internet.reactor import callLater
+from pyspades.constants import DESTROY_BLOCK, SPADE_DESTROY, BUILD_BLOCK
+from pyspades.collision import collision_3d
+from pyspades.common import Vertex3, make_color
+from pyspades.contained import GrenadePacket, BlockAction, SetColor
+from pyspades.world import Grenade
 MINEFIELD_VERSION = 1.6
 
-from pyspades.world import Grenade
-from pyspades.contained import GrenadePacket, BlockAction, SetColor
-from pyspades.common import Vertex3, make_color
-from pyspades.collision import collision_3d
-from pyspades.constants import DESTROY_BLOCK, SPADE_DESTROY, BUILD_BLOCK
-from twisted.internet.reactor import callLater
-from piqueserver.commands import command, admin
-from random import choice
 
 KILL_MESSAGES = [
     '{player} wandered into a minefield',
     '{player} should not walk into a minefield',
     '{player} was not carefull enough in the minefield',
     '{player} thought those mines were toys!',
     # JoJoe's messages
@@ -178,15 +178,15 @@
 
 
 @command(admin_only=True)
 def minedebug(connection):
     proto = connection.protocol
     proto.minefield_debug = not proto.minefield_debug
     message = 'Minefield is now in debug' if proto.minefield_debug else 'Minefield is no longer in debug'
-    proto.send_chat(message, global_message=True)
+    proto.broadcast_chat(message, global_message=True)
     return 'You toggled minefield debug'
 
 
 def apply_script(protocol, connection, config):
     class MineConnection(connection):
 
         def on_position_update(self):
@@ -205,25 +205,25 @@
                 message = MINEFIELD_DBG_MESSAGE.format(
                     x=x, y=y, z=z, m=self.protocol.minefieldAt(
                         x, y, z) or 'None')
                 self.send_chat(message)
                 return False
             if mode == DESTROY_BLOCK or mode == SPADE_DESTROY:
                 pos = self.world_object.position
-                #xx, yy, zz = x + 0.5, y + 0.5, z + 0.5
+                # xx, yy, zz = x + 0.5, y + 0.5, z + 0.5
                 if collision_3d(x, y, z, pos.x, pos.y, pos.z, 10):
                     self.protocol.check_mine(self, x, y, z)
             return connection.on_block_destroy(self, x, y, z, mode)
 
         def on_kill(self, killer, type, grenade):
             if grenade and grenade.name == MINEFIELD_MINE_ENT:
                 self.protocol.mine_kills += 1
                 message = choice(KILL_MESSAGES).format(
                     player=self.name, mine_kills=self.protocol.mine_kills)
-                self.protocol.send_chat(message, global_message=True)
+                self.protocol.broadcast_chat(message, global_message=True)
             connection.on_kill(self, killer, type, grenade)
 
     class MineProtocol(protocol):
         minefield_enabled = False
         minefields = []
         minefield_version = MINEFIELD_VERSION
         minefield_debug = False
```

### Comparing `piqueserver-1.0.0/piqueserver/scripts/nospadingwalls.py` & `piqueserver-1.1.1/piqueserver/scripts/nospadingwalls.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.0.0/piqueserver/scripts/paint.py` & `piqueserver-1.1.1/piqueserver/scripts/paint.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.0.0/piqueserver/scripts/passreload.py` & `piqueserver-1.1.1/piqueserver/scripts/passreload.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.0.0/piqueserver/scripts/protect.py` & `piqueserver-1.1.1/piqueserver/scripts/protect.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,23 +15,24 @@
 
 
 @command(admin_only=True)
 def protect(connection, value=None):
     protocol = connection.protocol
     if value is None:
         protocol.protected = None
-        protocol.send_chat('All areas unprotected', irc=True)
+        protocol.broadcast_chat('All areas unprotected', irc=True)
     else:
         if protocol.protected is None:
             protocol.protected = set()
         pos = coordinates(value)
         protocol.protected.symmetric_difference_update([pos])
         message = 'The area at %s is now %s' % (
-            value.upper(), 'protected' if pos in protocol.protected else 'unprotected')
-        protocol.send_chat(message, irc=True)
+            value.upper(),
+            'protected' if pos in protocol.protected else 'unprotected')
+        protocol.broadcast_chat(message, irc=True)
 
 
 def apply_script(protocol, connection, config):
     class ProtectConnection(connection):
 
         def _block_available(self, x, y, z):
             if not self.god and self.protocol.is_protected(x, y, z):
```

### Comparing `piqueserver-1.0.0/piqueserver/scripts/rampage.py` & `piqueserver-1.1.1/piqueserver/scripts/rampage.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 """
 
 from collections import deque
 from twisted.internet.reactor import callLater, seconds
 from twisted.internet.task import LoopingCall
 from pyspades import contained as loaders
 from pyspades.common import make_color
-from pyspades.constants import GRENADE_KILL, RIFLE_WEAPON, SMG_WEAPON, SHOTGUN_WEAPON
+from pyspades.constants import (
+    GRENADE_KILL, RIFLE_WEAPON, SMG_WEAPON, SHOTGUN_WEAPON)
 
 KILL_REQUIREMENT = 3
 TIME_REQUIREMENT = 8.0
 GRENADE_KILLS_COUNT = True
 RAMPAGE_REFILLS = True
 RAMPAGE_RELOADS = True
 RAMPAGE_DURATION = 20.0
@@ -28,15 +29,16 @@
     RIFLE_WEAPON: 0.16,
     SMG_WEAPON: 0.08,
     SHOTGUN_WEAPON: 0.18
 }
 RAMPAGE_FOG_COLOR = (255, 0, 0)
 
 
-def RAMPAGE_FOG_FUNC(): return RAMPAGE_FOG_COLOR
+def RAMPAGE_FOG_FUNC():
+    return RAMPAGE_FOG_COLOR
 
 
 ANNOUNCE_RAMPAGE = True
 S_RAMPAGE_START = '{player} IS ON A RAMPAGE!!'
 S_RAMPAGE_KILLED = "{victim}'s rampage was ended by {killer}"
 
 
@@ -102,23 +104,24 @@
                 weapon_reload.clip_ammo = weapon.current_ammo
                 weapon_reload.reserve_ammo = weapon.current_stock
                 weapon.set_shoot(was_shooting)
                 self.send_contained(weapon_reload)
             send_fog(self, RAMPAGE_FOG_COLOR)
             if ANNOUNCE_RAMPAGE:
                 message = S_RAMPAGE_START.format(player=self.name)
-                self.protocol.send_chat(message, global_message=None)
+                self.protocol.broadcast_chat(message, global_message=None)
 
         def end_rampage(self):
             self.rampage = False
             self.rapid_hack_detect = self.rampage_reenable_rapid_hack_detect
             if self.rampage_call and self.rampage_call.active():
                 self.rampage_call.cancel()
             self.rampage_call = None
-            if self.rampage_warning_call and self.rampage_warning_call.active():
+            if (self.rampage_warning_call and
+                    self.rampage_warning_call.active()):
                 self.rampage_warning_call.cancel()
             self.rampage_warning_call = None
             if self.rampage_rapid_loop and self.rampage_rapid_loop.running:
                 self.rampage_rapid_loop.stop()
             send_fog(self, self.protocol.fog_color)
 
         def on_connect(self):
@@ -141,15 +144,15 @@
             was_rampaging = self.rampage
             if self.rampage:
                 self.end_rampage()
             if killer is not None and killer is not self:
                 if was_rampaging and ANNOUNCE_RAMPAGE:
                     message = S_RAMPAGE_KILLED.format(victim=self.name,
                                                       killer=killer.name)
-                    self.protocol.send_chat(message, global_message=None)
+                    self.protocol.broadcast_chat(message, global_message=None)
                 if (not killer.rampage and killer.hp and
                     killer.team is not self.team and
                         (GRENADE_KILLS_COUNT or type != GRENADE_KILL)):
                     now = seconds()
                     killer.rampage_kills.append(now)
                     if (len(killer.rampage_kills) == KILL_REQUIREMENT and
                             killer.rampage_kills[0] >= now - TIME_REQUIREMENT):
@@ -159,23 +162,25 @@
         def on_grenade_thrown(self, grenade):
             if self.rampage:
                 resend_tool(self)
             connection.on_grenade_thrown(self, grenade)
 
         def on_shoot_set(self, fire):
             if (self.rampage and fire and
-                    self.rampage_rapid_loop and not self.rampage_rapid_loop.running):
+                self.rampage_rapid_loop and
+                    not self.rampage_rapid_loop.running):
                 interval = RAPID_INTERVALS[self.weapon]
                 self.rampage_rapid_loop.start(interval, now=False)
             connection.on_shoot_set(self, fire)
 
-    def send_fog_rule(player): return not player.rampage
+    def send_fog_rule(player):
+        return not player.rampage
 
     class RampageProtocol(protocol):
 
         def set_fog_color(self, color):
             self.fog_color = color
             fog_color = loaders.FogColor()
             fog_color.color = make_color(*color)
-            self.send_contained(fog_color, save=True, rule=send_fog_rule)
+            self.broadcast_contained(fog_color, save=True, rule=send_fog_rule)
 
     return RampageProtocol, RampageConnection
```

### Comparing `piqueserver-1.0.0/piqueserver/scripts/rangedamage.py` & `piqueserver-1.1.1/piqueserver/scripts/rangedamage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Changes the damage values depending on distance.
 
 Options
 ^^^^^^^
 
-.. code-block:: guess
+.. code-block:: toml
 
    [rangedamange.rifle]
    pct_per_block = 0 # percentage per block?
    multiplier = 1
 
    [rangedamange.smg]
    pct_per_block = 0
```

### Comparing `piqueserver-1.0.0/piqueserver/scripts/rapid.py` & `piqueserver-1.1.1/piqueserver/scripts/rapid.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.0.0/piqueserver/scripts/ratio.py` & `piqueserver-1.1.1/piqueserver/scripts/ratio.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
     class RatioProtocol(protocol):
 
         def on_votekick_start(self, instigator, victim, reason):
             result = protocol.on_votekick_start(
                 self, instigator, victim, reason)
             if result is None and RATIO_ON_VOTEKICK:
-                message = ratio(instigator, victim.name)
+                message = ratio(instigator, "#%i" % victim.player_id)
                 if IRC_ONLY:
                     self.irc_say('* ' + message)
                 else:
-                    self.send_chat(message, irc=True)
+                    self.broadcast_chat(message, irc=True)
             return result
 
     return RatioProtocol, RatioConnection
```

### Comparing `piqueserver-1.0.0/piqueserver/scripts/rollback.py` & `piqueserver-1.1.1/piqueserver/scripts/rollback.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 .. warning::
    ``/rollmap`` will take a long time if number of differing blocks is too high.
 
 Options
 ^^^^^^^
 
-.. code-block:: guess
+.. code-block:: toml
 
     [rollback]
     rollback_on_game_end = false
 
 .. codeauthor:: hompy
 """
 
@@ -45,20 +45,22 @@
 S_ROLLBACK_CANCELLED = 'Rollback cancelled by {player}'
 S_ROLLBACK_ENDED = 'Rollback ended. {result}'
 S_MAP_CHANGED = 'Map was changed'
 S_ROLLBACK_PROGRESS = 'Rollback progress {percent:.0%}'
 S_ROLLBACK_COLOR_PASS = 'Rollback doing color pass...'
 S_ROLLBACK_TIME_TAKEN = 'Time taken: {seconds:.3}s'
 
-NON_SURFACE_COLOR = (0, 0, 0)
+NON_SURFACE_COLOR = (69, 43, 30)
 
 rollback_config = config.section('rollback')
-ROLLBACK_ON_GAME_END_OPTION = rollback_config.option('rollback_on_game_end', False)
+ROLLBACK_ON_GAME_END_OPTION = rollback_config.option(
+    'rollback_on_game_end', False)
 config_dir = config.config_dir
 
+
 @command(admin_only=True)
 def rollmap(connection, mapname=None, value=None):
     start_x, start_y, end_x, end_y = 0, 0, 512, 512
     if value is not None:
         start_x, start_y = coordinates(value)
         end_x, end_y = start_x + 64, start_y + 64
     return connection.protocol.start_rollback(connection, mapname,
@@ -86,15 +88,16 @@
             return connection.on_block_destroy(self, x, y, z, value)
 
     class RollbackProtocol(protocol):
         rollback_in_progress = False
         rollback_max_rows = 10  # per 'cycle', intended to cap cpu usage
         # per 'cycle' cap for (unique packets * players)
         rollback_max_packets = 180
-        rollback_max_unique_packets = 12  # per 'cycle', each block op is at least 1
+        # per 'cycle', each block op is at least 1
+        rollback_max_unique_packets = 12
         rollback_time_between_cycles = 0.06
         rollback_time_between_progress_updates = 10.0
         rollback_start_time = None
         rollback_last_chat = None
         rollback_rows = None
         rollback_total_rows = None
 
@@ -113,17 +116,18 @@
                         return S_INVALID_MAP_NAME
                     map = Map(maps[0], os.path.join(config_dir, "maps")).data
                 except MapNotFound as error:
                     return error.message
             name = (connection.name if connection is not None
                     else S_AUTOMATIC_ROLLBACK_PLAYER_NAME)
             message = S_ROLLBACK_COMMENCED.format(player=name)
-            self.send_chat(message, irc=True)
+            self.broadcast_chat(message, irc=True)
             self.packet_generator = self.create_rollback_generator(
-                self.map, map, start_x, start_y, end_x, end_y, ignore_indestructable)
+                self.map, map, start_x, start_y,
+                end_x, end_y, ignore_indestructable)
             self.rollback_in_progress = True
             self.rollback_start_time = time.monotonic()
             self.rollback_last_chat = self.rollback_start_time
             self.rollback_rows = 0
             self.rollback_total_rows = end_x - start_x
             self.cycle_call = LoopingCall(self.rollback_cycle)
             self.cycle_call.start(self.rollback_time_between_cycles)
@@ -137,15 +141,15 @@
         def end_rollback(self, result):
             self.rollback_in_progress = False
             self.cycle_call.stop()
             self.cycle_call = None
             self.packet_generator = None
             self.update_entities()
             message = S_ROLLBACK_ENDED.format(result=result)
-            self.send_chat(message, irc=True)
+            self.broadcast_chat(message, irc=True)
 
         def rollback_cycle(self):
             if not self.rollback_in_progress:
                 return
             try:
                 sent_unique = sent_total = rows = 0
                 while True:
@@ -163,31 +167,31 @@
                 if (time.monotonic() - self.rollback_last_chat >
                         self.rollback_time_between_progress_updates):
                     self.rollback_last_chat = time.monotonic()
                     progress = float(self.rollback_rows) / \
                         self.rollback_total_rows
                     if progress < 1.0:
                         message = S_ROLLBACK_PROGRESS.format(percent=progress)
-                        self.send_chat(message)
+                        self.broadcast_chat(message)
                     else:
-                        self.send_chat(S_ROLLBACK_COLOR_PASS)
+                        self.broadcast_chat(S_ROLLBACK_COLOR_PASS)
             except (StopIteration):
                 elapsed = time.monotonic() - self.rollback_start_time
                 message = S_ROLLBACK_TIME_TAKEN.format(seconds=elapsed)
                 self.end_rollback(message)
 
         def create_rollback_generator(self, cur, new, start_x, start_y,
                                       end_x, end_y, ignore_indestructable):
             surface = {}
             block_action = BlockAction()
             block_action.player_id = 31
             set_color = SetColor()
             set_color.value = make_color(*NON_SURFACE_COLOR)
             set_color.player_id = 31
-            self.send_contained(set_color, save=True)
+            self.broadcast_contained(set_color, save=True)
             old = cur.copy()
             check_protected = hasattr(protocol, 'protected')
             for x in range(start_x, end_x):
                 block_action.x = x
                 for y in range(start_y, end_y):
                     block_action.y = y
                     if check_protected and self.is_protected(x, y, 0):
@@ -219,33 +223,33 @@
                                 if not old_is_surface or old_color != new_color:
                                     surface[(x, y, z)] = new_color
                                     action = DESTROY_BLOCK
                                     cur.remove_point(x, y, z)
                         if action is not None:
                             block_action.z = z
                             block_action.value = action
-                            self.send_contained(block_action, save=True)
+                            self.broadcast_contained(block_action, save=True)
                             yield 1
                 yield 0
             last_color = None
             block_action.value = BUILD_BLOCK
             for pos, color in sorted(iter(surface.items()),
                                      key=operator.itemgetter(1)):
                 x, y, z = pos
                 packets_sent = 0
                 if color != last_color:
                     set_color.value = make_color(*color)
-                    self.send_contained(set_color, save=True)
+                    self.broadcast_contained(set_color, save=True)
                     packets_sent += 1
                     last_color = color
                 cur.set_point(x, y, z, color)
                 block_action.x = x
                 block_action.y = y
                 block_action.z = z
-                self.send_contained(block_action, save=True)
+                self.broadcast_contained(block_action, save=True)
                 packets_sent += 1
                 yield packets_sent
 
         def on_map_change(self, map):
             self.rollback_map = map.copy()
             protocol.on_map_change(self, map)
```

### Comparing `piqueserver-1.0.0/piqueserver/scripts/runningman.py` & `piqueserver-1.1.1/piqueserver/scripts/runningman.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,23 +45,23 @@
 @command('runningman', admin_only=True)
 def running_man(connection):
     protocol = connection.protocol
     protocol.running_man = not protocol.running_man
     if not protocol.running_man:
         protocol.drop_all_links()
     message = S_ENABLED if protocol.running_man else S_DISABLED
-    protocol.send_chat(message, irc=True)
+    protocol.broadcast_chat(message, irc=True)
 
 
 @command(admin_only=True)
 def relink(connection):
     if not connection.protocol.running_man:
         return S_NOT_ENABLED
     connection.protocol.drop_all_links()
-    connection.protocol.send_chat(S_UNLINK_ALL, irc=True)
+    connection.protocol.broadcast_chat(S_UNLINK_ALL, irc=True)
 
 
 @command(admin_only=True)
 @target_player
 def unlink(connection, player):
     protocol = connection.protocol
     if not protocol.running_man:
@@ -112,41 +112,43 @@
             connection.on_position_update(self)
 
         def on_spawn(self, pos):
             if self.protocol.running_man:
                 if (self.link is None or
                         self.link_deaths >= MAX_LINK_DEATHS):
                     self.get_new_link()
-                if self.link is not None and self.link.hp is not None and self.link.hp > 0:
+                if (self.link is not None and
+                        self.link.hp is not None and self.link.hp > 0):
                     self.set_location_safe(
                         self.link.world_object.position.get())
             connection.on_spawn(self, pos)
 
         def on_team_changed(self, old_team):
             if self.protocol.running_man:
                 self.drop_link()
             return connection.on_team_changed(self, old_team)
 
         def on_flag_capture(self):
             if self.protocol.running_man:
                 for player in self.team.get_players():
                     player.drop_link(no_message=True)
                 message = S_FLAG_CAPTURED.format(team=self.team.name)
-                self.protocol.send_chat(message, global_message=None)
+                self.protocol.broadcast_chat(message, global_message=None)
             connection.on_flag_capture(self)
 
         def on_reset(self):
             if self.protocol.running_man:
                 self.drop_link()
             connection.on_reset(self)
 
         def can_be_linked_to(self, player):
             if self is player or self.link is player:
                 return False
-            if player.link is not None and player.link_deaths < MAX_LINK_DEATHS:
+            if (player.link is not None and
+                    player.link_deaths < MAX_LINK_DEATHS):
                 return False
             return True
 
         def get_new_link(self):
             available = list(filter(self.can_be_linked_to,
                                     self.team.get_players()))
             if not available:
@@ -162,15 +164,17 @@
             self.send_chat(message)
             message = S_LINKED.format(player=self.name)
             self.link.send_chat(message)
 
         def drop_link(self, force_message=False, no_message=False):
             if self.link is None:
                 return
-            if (self.link.hp is not None and (self.link.hp > 0 or force_message)) and not no_message:
+            if (self.link.hp is not None and
+                (self.link.hp > 0 or force_message)
+                    and not no_message):
                 self.link.send_chat(S_FREE)
             self.link.link = None
             self.link = None
 
         def grenade_suicide(self):
             protocol = self.protocol
             position = self.world_object.position
```

### Comparing `piqueserver-1.0.0/piqueserver/scripts/smartnade.py` & `piqueserver-1.1.1/piqueserver/scripts/smartnade.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.0.0/piqueserver/scripts/spadenadefix.py` & `piqueserver-1.1.1/piqueserver/scripts/spadenadefix.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.0.0/piqueserver/scripts/spawn_protect.py` & `piqueserver-1.1.1/piqueserver/scripts/spawn_protect.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Protects spawned players for a specified amount of seconds.
 
 Options
 ^^^^^^^
 
-.. code-block:: guess
+.. code-block:: toml
 
    [spawn_protect]
    protection_time = "3sec"
 
 .. codeauthor:: ? & kmsi <kmsiapps@gmail.com>
 """
```

### Comparing `piqueserver-1.0.0/piqueserver/scripts/spectatorcontrol.py` & `piqueserver-1.1.1/piqueserver/scripts/spectatorcontrol.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 Hope you enjoy!
 Tocksman
 
 Options
 ^^^^^^^
 
-.. code-block:: guess
+.. code-block:: toml
 
    [spectator_control]
    no_chat = false # determines whether spectators can chat or not in your server
    kick = false # determines whether spectators will be kicked after remaining for so long
    kick_time = "5min" # how long a spectator may remain before they are kicked
 
 .. codeauthor:: Tocksman (made for Goon Haven)
```

### Comparing `piqueserver-1.0.0/piqueserver/scripts/squad.py` & `piqueserver-1.1.1/piqueserver/scripts/squad.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 * ``/squad <key>`` to join a squad
 * ``/follow <player>`` to spawn near a specific player
 
 Options
 ^^^^^^^
 
-.. code-block:: guess
+.. code-block:: toml
 
     [squad]
     respawn_time = "10sec"
     auto_squad = true
 
 .. codeauthor:: Triplefox
 """
@@ -76,15 +76,15 @@
         allsquads = self.get_squads(self.team)
         result = []
         for squadkey in list(allsquads.keys()):
             result.append(self.print_squad(
                 squadkey, allsquads[squadkey]))
         result.append(('To join squads: /squad <squad name>. ' +
                        '/squad none to spawn normally.'))
-        self.send_lines(result)
+        self.send_lines(result, 'squad_list')
         return
 
     if squadkey.lower() == 'none':
         squad = None
         squad_pref = None
     else:
         squad = squadkey
```

### Comparing `piqueserver-1.0.0/piqueserver/scripts/strongblock.py` & `piqueserver-1.1.1/piqueserver/scripts/strongblock.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.0.0/piqueserver/scripts/timedmute.py` & `piqueserver-1.1.1/piqueserver/scripts/timedmute.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,36 +39,36 @@
 class TimedMute:
     player = None
     time = None
 
     def __init__(self, player, time=300, reason='None'):
         if time == 0:
             player.mute = True
-            player.protocol.send_chat(
+            player.protocol.broadcast_chat(
                 '%s was muted indefinitely (Reason: %s)' %
                 (player.name, reason), irc=True)
             return
 
         schedule = Scheduler(player.protocol)
         schedule.call_later(time, self.end)
         player.mute_schedule = schedule
 
-        player.protocol.send_chat(
+        player.protocol.broadcast_chat(
             '%s was muted for %s seconds (Reason: %s)' %
             (player.name, time, reason), irc=True)
         player.mute = True
 
         self.player = player
         self.time = time
 
     def end(self):
         self.player.mute = False
         message = '%s was unmuted after %s seconds' % (
             self.player.name, self.time)
-        self.player.protocol.send_chat(message, irc=True)
+        self.player.protocol.broadcast_chat(message, irc=True)
 
 
 def apply_script(protocol, connection, config):
     class TimedMuteConnection(connection):
         mute_schedule = None
 
         def on_disconnect(self):
```

### Comparing `piqueserver-1.0.0/piqueserver/scripts/trusted.py` & `piqueserver-1.1.1/piqueserver/scripts/trusted.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.0.0/piqueserver/scripts/votekick.py` & `piqueserver-1.1.1/piqueserver/scripts/votekick.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 * ``/togglevotekick or /tvk`` toggles votekicks on/off globally
 * ``/togglevotekick or /tvk <player>`` toggles votekicks on/off for specific players
 * ``/cancel`` cancels a votekick
 
 Options
 ^^^^^^^
 
-.. code-block:: guess
+.. code-block:: toml
 
     [votekick]
     # percentage of total number of players in the server required to vote to
     # successfully votekick a player
     percentage = 35
 
     # duration that votekicked player will be banned for
@@ -46,38 +46,42 @@
 S_IN_PROGRESS = 'Votekick already in progress'
 S_SELF_VOTEKICK = "You can't votekick yourself"
 S_NOT_ENOUGH_PLAYERS = "There aren't enough players to vote"
 S_VOTEKICK_IMMUNE = "You can't votekick this player"
 S_NOT_YET = "You can't start another votekick yet!"
 S_NEED_REASON = 'You must provide a reason for the votekick'
 S_CANT_CANCEL = "You didn't start the votekick!"
-S_YES = '{player} voted YES'
-S_ENDED = 'Votekick for {victim} has ended. {result}'
+S_YES = '{player} (#{player_id}) voted YES'
+S_ENDED = 'Votekick for {victim} (#{victim_id}) has ended. {result}'
 S_RESULT_TIMED_OUT = 'Votekick timed out'
 S_RESULT_CANCELLED = 'Cancelled'
 S_RESULT_BANNED = 'Banned by admin'
 S_RESULT_KICKED = 'Kicked by admin'
 S_RESULT_INSTIGATOR_KICKED = 'Instigator kicked by admin'
-S_RESULT_LEFT = '{victim} left during votekick'
-S_RESULT_INSTIGATOR_LEFT = 'Instigator {instigator} left'
+S_RESULT_LEFT = '{victim} (#{victim_id}) left during votekick'
+S_RESULT_INSTIGATOR_LEFT = 'Instigator {instigator} (#{instigator_id}) left'
 S_RESULT_PASSED = 'Player kicked'
-S_ANNOUNCE_IRC = '* {instigator} started a votekick against player {victim}. ' \
-    'Reason: {reason}'
-S_ANNOUNCE = '{instigator} started a VOTEKICK against {victim}. Say /Y to agree'
-S_ANNOUNCE_SELF = 'You started a votekick against {victim}. Say /CANCEL to ' \
-    'stop it'
-S_UPDATE = '{instigator} is votekicking {victim}. /Y to vote ({needed} left)'
+S_ANNOUNCE_IRC = '* {instigator} (#{instigator_id}) started a votekick' \
+    'against player {victim} (#{victim_id}). Reason: {reason}'
+S_ANNOUNCE = '{instigator} (#{instigator_id}) started a VOTEKICK against' \
+    '{victim} (#{victim_id}). Say /Y to agree'
+S_ANNOUNCE_SELF = 'You started a votekick against {victim} ({victim_id}).'\
+    ' Say /CANCEL to stop it'
+S_UPDATE = '{instigator} (#{instigator_id}) is votekicking' \
+    '{victim} (#{victim_id}). /Y to vote ({needed} left)'
 S_REASON = 'Reason: {reason}'
 
 # register options
 VOTEKICK_CONFIG = config.section('votekick')
 REQUIRED_PERCENTAGE_OPTION = VOTEKICK_CONFIG.option('percentage', 35.0)
-BAN_DURATION_OPTION = VOTEKICK_CONFIG.option('ban_duration', default="30min", cast=cast_duration)
+BAN_DURATION_OPTION = VOTEKICK_CONFIG.option(
+    'ban_duration', default="30min", cast=cast_duration)
 PUBLIC_VOTES_OPTION = VOTEKICK_CONFIG.option('public_votes', True)
 
+
 class VotekickFailure(Exception):
     pass
 
 
 @command('votekick')
 @player_only
 def start_votekick(connection, *args):
@@ -166,17 +170,14 @@
     return S_VOTEKICK_USER_SET.format(user=player.name, set=(
         'enabled' if player.votekick_enabled else 'disabled'))
 
 
 class Votekick:
     timeout = 120.0  # 2 minutes
     interval = 120.0  # 2 minutes
-    ban_duration = BAN_DURATION_OPTION.get()
-    public_votes = PUBLIC_VOTES_OPTION.get()
-    schedule = None
 
     @property
     def votes_remaining(self) -> int:
         return self.protocol.get_required_votes() - len(self.votes) + 1
 
     @classmethod
     def start(cls, instigator, victim, reason=None):
@@ -208,40 +209,49 @@
         self.protocol = protocol = instigator.protocol
         self.instigator = instigator
         self.victim = victim
         self.reason = reason
         self.votes = {instigator: True}
         self.ended = False
 
+        self.ban_duration = BAN_DURATION_OPTION.get()
+        self.public_votes = PUBLIC_VOTES_OPTION.get()
+
         protocol.irc_say(
             S_ANNOUNCE_IRC.format(
                 instigator=instigator.name,
+                instigator_id=instigator.player_id,
                 victim=victim.name,
+                victim_id=victim.player_id,
                 reason=self.reason))
-        protocol.send_chat(
+        protocol.broadcast_chat(
             S_ANNOUNCE.format(
                 instigator=instigator.name,
-                victim=victim.name),
+                instigator_id=instigator.player_id,
+                victim=victim.name,
+                victim_id=victim.player_id),
             sender=instigator)
-        protocol.send_chat(S_REASON.format(reason=self.reason),
-                           sender=instigator)
-        instigator.send_chat(S_ANNOUNCE_SELF.format(victim=victim.name))
+        protocol.broadcast_chat(S_REASON.format(reason=self.reason),
+                                sender=instigator)
+        instigator.send_chat(S_ANNOUNCE_SELF.format(
+            victim=victim.name, victim_id=victim.player_id))
 
         schedule = Scheduler(protocol)
         schedule.call_later(self.timeout, self.end, S_RESULT_TIMED_OUT)
         schedule.loop_call(30.0, self.send_chat_update)
         self.schedule = schedule
 
     def vote(self, player):
         if self.victim is player:
             return
         elif player in self.votes:
             return
         if self.public_votes:
-            self.protocol.send_chat(S_YES.format(player=player.name))
+            self.protocol.broadcast_chat(S_YES.format(
+                player=player.name, player_id=player.player_id))
         self.votes[player] = True
         if self.votes_remaining <= 0:
             # vote passed, ban or kick accordingly
             victim = self.victim
             self.end(S_RESULT_PASSED)
             print(victim.name, 'votekicked')
             if self.ban_duration > 0.0:
@@ -256,28 +266,33 @@
         if self.schedule:
             self.schedule.reset()
         self.schedule = None
         self.protocol.votekick = None
 
     def end(self, result):
         self.ended = True
-        message = S_ENDED.format(victim=self.victim.name, result=result)
-        self.protocol.send_chat(message, irc=True)
+        message = S_ENDED.format(
+            victim=self.victim.name,
+            victim_id=self.victim.player_id,
+            result=result)
+        self.protocol.broadcast_chat(message, irc=True)
         if not self.instigator.admin:
             self.instigator.last_votekick = seconds()
         self.protocol.on_votekick_end()
         self.release()
 
     def send_chat_update(self, target=None):
         # send only to target player if provided, otherwise broadcast to server
         target = target or self.protocol
         target.send_chat(
             S_UPDATE.format(
                 instigator=self.instigator.name,
+                instigator_id=self.instigator.player_id,
                 victim=self.victim.name,
+                victim_id=self.victim.player_id,
                 needed=self.votes_remaining))
         target.send_chat(S_REASON.format(reason=self.reason))
 
 
 def apply_script(protocol, connection, config):
 
     class VotekickProtocol(protocol):
@@ -313,19 +328,21 @@
 
         def on_disconnect(self):
             votekick = self.protocol.votekick
             if votekick:
                 if votekick.victim is self:
                     # victim leaves, gets votekick ban
                     reason = votekick.reason
-                    votekick.end(S_RESULT_LEFT.format(victim=self.name))
+                    votekick.end(S_RESULT_LEFT.format(
+                        victim=self.name, victim_id=self.player_id))
                     self.ban(reason, Votekick.ban_duration)
                 elif votekick.instigator is self:
                     # instigator leaves, votekick is called off
-                    s = S_RESULT_INSTIGATOR_LEFT.format(instigator=self.name)
+                    s = S_RESULT_INSTIGATOR_LEFT.format(
+                        instigator=self.name, instigator_id=self.player_id)
                     votekick.end(s)
                 else:
                     # make sure we still have enough players
                     votekick.votes.pop(self, None)
                     if votekick.votes_remaining <= 0:
                         votekick.end(S_NOT_ENOUGH_PLAYERS)
             connection.on_disconnect(self)
```

### Comparing `piqueserver-1.0.0/piqueserver/scripts/votemap.py` & `piqueserver-1.1.1/piqueserver/scripts/votemap.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 Commands
 ^^^^^^^^
 
 * ``/votemap`` initiates map voting
 * ``/vote <map name>`` vote for a map
 
-.. code-block:: guess
+.. code-block:: toml
 
     [votemap]
     public_votes = true
     extension_time = "15min"
     player_driven = false
     autoschedule = false
     percentage = 80
@@ -30,20 +30,22 @@
 from piqueserver.config import config, cast_duration
 
 votemap_config = config.section('votemap')
 
 VOTEMAP_AUTOSCHEDULE_OPTION = votemap_config.option('autoschedule', 180)
 VOTEMAP_PUBLIC_VOTES_OPTION = votemap_config.option('public_votes', True)
 # godwhoa: This option gets loaded into votemap_time but that doesn't get used anywhere.
-VOTEMAP_TIME_OPTION = votemap_config.option('time', default="2min", cast=cast_duration)
+VOTEMAP_TIME_OPTION = votemap_config.option(
+    'time', default="2min", cast=cast_duration)
 VOTEMAP_EXTENSION_TIME_OPTION = votemap_config.option('extension_time', default="15min",
-    cast=lambda x: cast_duration(x)/60)
+                                                      cast=lambda x: cast_duration(x)/60)
 VOTEMAP_PLAYER_DRIVEN_OPTION = votemap_config.option('player_driven', False)
 VOTEMAP_PERCENTAGE_OPTION = votemap_config.option('percentage', 80)
 
+
 def cancel_verify(connection, instigator):
     return (connection.admin or
             connection is instigator or
             connection.rights.cancel)
 
 
 class VoteMap:
@@ -101,73 +103,73 @@
             return "You can't start a vote now."
         return True
 
     def start(self):
         instigator = self.instigator
         protocol = self.protocol
         if instigator is None:
-            protocol.send_chat('Time to vote!', irc=True)
+            protocol.broadcast_chat('Time to vote!', irc=True)
         else:
-            protocol.send_chat(
+            protocol.broadcast_chat(
                 '* %s initiated a map vote.' % instigator.name, irc=True)
         self.schedule = schedule = Scheduler(protocol)
         schedule.call_later(self.vote_time, self.timeout)
         schedule.loop_call(30.0, self.update)
         self.protocol.votemap = self
         self.update()
 
     def vote(self, connection, mapname):
         mapname = mapname.lower()
         if mapname not in self.picks:
             connection.send_chat("Map %s is not available." % mapname)
             return
         self.votes[connection] = mapname
         if self.public_votes:
-            self.protocol.send_chat('%s voted for %s.' % (connection.name,
-                                                          mapname))
+            self.protocol.broadcast_chat('%s voted for %s.' % (connection.name,
+                                                               mapname))
         if self.votes_left()['count'] <= 0:
             self.on_majority()
 
     def cancel(self, connection=None):
         if connection is None:
             message = 'Cancelled'
         elif not cancel_verify(connection, self.instigator):
             return 'You did not start the vote.'
         else:
             message = 'Cancelled by %s' % connection.name
-        self.protocol.send_chat(message)
+        self.protocol.broadcast_chat(message)
         self.set_cooldown()
         self.finish()
 
     def update(self):
-        self.protocol.send_chat(
+        self.protocol.broadcast_chat(
             'Choose next map. Say /vote <name> to cast vote.')
         names = ' '.join(self.picks)
-        self.protocol.send_chat('Maps: %s' % names)
-        self.protocol.send_chat('To extend current map: /vote extend')
+        self.protocol.broadcast_chat('Maps: %s' % names)
+        self.protocol.broadcast_chat('To extend current map: /vote extend')
 
     def timeout(self):
         self.show_result()
         self.finish()
 
     def on_majority(self):
         self.show_result()
         self.finish()
 
     def show_result(self):
         result = self.votes_left()['name']
         if result == "extend":
             tl = self.protocol.set_time_limit(self.extension_time, True)
             span = prettify_timespan(tl * 60.0)
-            self.protocol.send_chat('Mapvote ended. Current map will '
-                                    'continue for %s.' % span, irc=True)
+            self.protocol.broadcast_chat('Mapvote ended. Current map will '
+                                         'continue for %s.' % span, irc=True)
             self.protocol.autoschedule_votemap()
         else:
-            self.protocol.send_chat('Mapvote ended. Next map will be: %s.' %
-                                    result, irc=True)
+            self.protocol.broadcast_chat('Mapvote ended. Next map will be: %s.' %
+                                         result, irc=True)
             self.protocol.planned_map = check_rotation([result])[0]
         self.set_cooldown()
 
     def set_cooldown(self):
         if self.instigator is not None and not self.instigator.admin:
             self.instigator.last_votemap = reactor.seconds()
```

### Comparing `piqueserver-1.0.0/piqueserver/scripts/welcome.py` & `piqueserver-1.1.1/piqueserver/scripts/welcome.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Greets specified people entering with messages
 
 Options
 ^^^^^^^
 
-.. code-block:: guess
+.. code-block:: toml
 
    [welcome]
    welcomes = { nota = "Hi notafile", feik = "Hi feik" }
 
 .. codeauthor: mat^2
 """
 from piqueserver.config import config
@@ -20,10 +20,10 @@
 def apply_script(protocol, connection, config):
     welcomes = welcomes_option.get()
 
     class EnterConnection(connection):
 
         def on_login(self, name):
             if name in welcomes:
-                self.protocol.send_chat(welcomes[name])
+                self.protocol.broadcast_chat(welcomes[name])
             connection.on_login(self, name)
     return protocol, EnterConnection
```

### Comparing `piqueserver-1.0.0/piqueserver/scripts/zoc.py` & `piqueserver-1.1.1/piqueserver/scripts/zoc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Zones of control: Dropped intel and tents exert influence
 over nearby area, restricting player ability to destroy.
 
 Options
 ^^^^^^^
 
-.. code-block:: guess
+.. code-block:: toml
 
    [zoc]
    radius = 32
    attack_distance = 64
    block_undo = 10
    block_cost = 5
    points_per_tick = 1
```

### Comparing `piqueserver-1.0.0/piqueserver/server.py` & `piqueserver-1.1.1/piqueserver/server.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,23 +22,24 @@
 import asyncio
 import itertools
 import json
 import os
 import random
 import sys
 import time
+import warnings
 from collections import deque
 from ipaddress import AddressValueError, IPv4Address, ip_address, ip_network
 from pprint import pprint
 from typing import Any, Callable, Dict, Iterator, List, Optional, Tuple
 
 import aiohttp
 from enet import Address, Packet, Peer
 from twisted.internet import reactor, threads
-from twisted.internet.defer import Deferred, ensureDeferred, inlineCallbacks
+from twisted.internet.defer import Deferred, ensureDeferred
 from twisted.internet.task import LoopingCall, coiterate, deferLater
 from twisted.internet.tcp import Port
 from twisted.logger import (FilteringLogObserver, Logger, LogLevel,
                             LogLevelFilterPredicate, globalLogBeginner,
                             textFileLogObserver)
 from twisted.python.logfile import DailyLogFile
 
@@ -48,15 +49,15 @@
 from piqueserver.config import cast_duration, config
 from piqueserver.console import create_console
 from piqueserver.map import Map, MapNotFound, RotationInfo, check_rotation
 from piqueserver.networkdict import NetworkDict
 from piqueserver.player import FeatureConnection
 from piqueserver.release import check_for_releases, format_release
 from piqueserver.scheduler import Scheduler
-from piqueserver.utils import as_deferred
+from piqueserver.utils import as_deferred, EndCall
 from piqueserver.bansubscribe import bans_config_urls
 from pyspades.bytes import NoDataLeft
 from pyspades.constants import CTF_MODE, ERROR_SHUTDOWN, TC_MODE
 from pyspades.master import MAX_SERVER_NAME_SIZE
 from pyspades.server import ServerProtocol, Team
 from pyspades.tools import make_server_identifier
 from pyspades.vxl import VXLData
@@ -102,15 +103,15 @@
     'default_time_limit', default="20min",
     cast=lambda x: cast_duration(x)/60)
 cap_limit = config.option('cap_limit', default=10,
                           validate=lambda x: isinstance(x, (int, float)))
 advance_on_win = config.option('advance_on_win', default=False,
                                validate=lambda x: isinstance(x, bool))
 everyone_is_admin = config.option('everyone_is_admin', default=False,
-                               validate=lambda x: isinstance(x, bool))
+                                  validate=lambda x: isinstance(x, bool))
 team1_name = team1_config.option(
     'name', default='Blue', validate=validate_team_name)
 team2_name = team2_config.option(
     'name', default='Green', validate=validate_team_name)
 team1_color = team1_config.option('color', default=(0, 0, 196))
 team2_color = team2_config.option('color', default=(0, 196, 0))
 friendly_fire = config.option('friendly_fire', default=False)
@@ -137,15 +138,14 @@
 balanced_teams = config.option('balanced_teams', default=2)
 login_retries = config.option('login_retries', 1)
 default_ban_duration = bans_config.option(
     'default_duration', default="1day", cast=cast_duration)
 speedhack_detect = config.option('speedhack_detect', True)
 rubberband_distance = config.option('rubberband_distance', default=10)
 user_blocks_only = config.option('user_blocks_only', False)
-debug_log_enabled = logging_config.option('debug_log', False)
 logging_profile_option = logging_config.option('profile', False)
 set_god_build = config.option('set_god_build', False)
 ssh_enabled = config.section('ssh').option('enabled', False)
 irc_options = config.option('irc', {})
 status_server_enabled = config.section(
     'status_server').option('enabled', False)
 ban_publish = bans_config.option('publish', False)
@@ -169,14 +169,18 @@
     '/help Prints this message',
 ])
 rules_option = config.option('rules')
 tips_option = config.option('tips')
 network_interface = config.option('network_interface', default='')
 scripts_option = config.option(
     'scripts', default=[], validate=extensions.check_scripts)
+cmd_antispam_enable = config.option("enable_command_ratelimit", True)
+cmd_command_limit_size = config.option("command_ratelimit_amount", 4)
+cmd_command_limit_time = config.option(
+    "command_ratelimit_period", "5s", cast=cast_duration)
 
 
 def ensure_dir_exists(filename: str) -> None:
     d = os.path.dirname(filename)
     os.makedirs(d, exist_ok=True)
 
 
@@ -193,78 +197,34 @@
         if get_location is not None:
             result = get_location(self, entity_id)
             if result is not None:
                 return result
         return Team.get_entity_location(self, entity_id)
 
 
-class EndCall:
-    _active = True
-
-    def __init__(self, protocol, delay: int, func: Callable, *arg, **kw) -> None:
-        self.protocol = protocol
-        protocol.end_calls.append(self)
-        self.delay = delay
-        self.func = func
-        self.arg = arg
-        self.kw = kw
-        self.call = None  # type: Deferred
-
-    def set(self, value: Optional[float]) -> None:
-        if value is None:
-            if self.call is not None:
-                self.call.cancel()
-                self.call = None
-        elif value is not None:
-            value = value - self.delay
-            if value <= 0.0:
-                self.cancel()
-            elif self.call:
-                # In Twisted==18.9.0, reset() is broken when using
-                # AsyncIOReactor
-                # self.call.reset(value)
-                self.call.cancel()
-                self.call = reactor.callLater(value, self.fire)
-            else:
-                self.call = reactor.callLater(value, self.fire)
-
-    def fire(self):
-        self.call = None
-        self.cancel()
-        self.func(*self.arg, **self.kw)
-
-    def cancel(self) -> None:
-        self.set(None)
-        self.protocol.end_calls.remove(self)
-        self._active = False
-
-    def active(self) -> bool:
-        return self._active and (self.call and self.call.active())
-
-
 class FeatureProtocol(ServerProtocol):
     connection_class = FeatureConnection
     bans = None
     ban_publish = None
     ban_manager = None
     everyone_is_admin = False
     player_memory = None
     irc_relay = None
     balanced_teams = None
     timestamps = None
     building = True
     killing = True
     global_chat = True
     remote_console = None
-    debug_log = None
     advance_call = None
     master_reconnect_call = None
     master = False
     ip = None
     identifier = None
+    command_antispam = False
 
     planned_map = None
 
     map_info = None
     spawns = None
     user_blocks = None
     god_blocks = None
@@ -317,17 +277,19 @@
             with open(os.path.join(config.config_dir, bans_file.get()), 'r') as f:
                 self.bans.read_list(json.load(f))
             log.debug("loaded {count} bans", count=len(self.bans))
         except FileNotFoundError:
             log.debug("skip loading bans: file unavailable",
                       count=len(self.bans))
         except IOError as e:
-            log.error('Could not read bans file ({}): {}'.format(bans_file.get(), e))
+            log.error('Could not read bans file ({}): {}'.format(
+                bans_file.get(), e))
         except ValueError as e:
-            log.error('Could not parse bans file ({}): {}'.format(bans_file.get(), e))
+            log.error('Could not parse bans file ({}): {}'.format(
+                bans_file.get(), e))
 
         self.hard_bans = set()  # possible DDoS'ers are added here
         self.player_memory = deque(maxlen=100)
         if len(self.name) > MAX_SERVER_NAME_SIZE:
             log.warn('(server name too long; it will be truncated to "%s")' % (
                 self.name[:MAX_SERVER_NAME_SIZE]))
         self.respawn_time = respawn_time_option.get()
@@ -363,28 +325,26 @@
         self.melee_damage = melee_damage.get()
         self.max_connections_per_ip = max_connections_per_ip.get()
         self.passwords = passwords.get()
         self.server_prefix = server_prefix.get()
         self.time_announcements = time_announcements.get()
         self.balanced_teams = balanced_teams.get()
         self.login_retries = login_retries.get()
+        self.command_antispam = cmd_antispam_enable.get()
+        self.command_limit_size = cmd_command_limit_size.get()
+        self.command_limit_time = cmd_command_limit_time.get()
 
         # voting configuration
         self.default_ban_time = default_ban_duration.get()
 
         self.speedhack_detect = speedhack_detect.get()
         self.rubberband_distance = rubberband_distance.get()
         if user_blocks_only.get():
             self.user_blocks = set()
         self.set_god_build = set_god_build.get()
-        self.debug_log = debug_log_enabled.get()
-        if self.debug_log:
-            # TODO: make this configurable
-            pyspades.debug.open_debug_log(
-                os.path.join(config.config_dir, 'debug.log'))
         if ssh_enabled.get():
             from piqueserver.ssh import RemoteConsole
             self.remote_console = RemoteConsole(self)
         irc = irc_options.get()
         if irc.get('enabled', False):
             from piqueserver.irc import IRCRelay
             self.irc_relay = IRCRelay(self, irc)
@@ -394,14 +354,15 @@
             ensureDeferred(self.status_server.listen())
         if ban_publish.get():
             from piqueserver.banpublish import PublishServer
             self.ban_publish = PublishServer(self, ban_publish_port.get())
         if bans_config_urls.get():
             from piqueserver import bansubscribe
             self.ban_manager = bansubscribe.BanManager(self)
+            ensureDeferred(as_deferred(self.ban_manager.start()))
         self.start_time = time.time()
         self.end_calls = []
         # TODO: why is this here?
         create_console(self)
 
         for user_type, func_names in rights.get().items():
             for func_name in func_names:
@@ -441,15 +402,15 @@
         reactor.addSystemEventTrigger(
             'before', 'shutdown', lambda: ensureDeferred(self.shutdown()))
 
     def _post_init(self):
         """called after the map has been loaded"""
         self.update_format()
         self.tip_frequency = tip_frequency.get()
-        if self.tips is not None and self.tip_frequency > 0:
+        if self.tips and self.tip_frequency > 0:
             reactor.callLater(self.tip_frequency * 60, self.send_tip)
 
         self.master = register_master_option.get()
         self.set_master()
 
     async def get_external_ip(self, ip_getter: str) -> Iterator[Deferred]:
         log.info(
@@ -504,20 +465,21 @@
 
         return time_limit
 
     def _next_time_announce(self):
         remaining = self.advance_call.getTime() - reactor.seconds()
         if remaining < 60.001:
             if remaining < 10.001:
-                self.send_chat('%s...' % int(round(remaining)))
+                self.broadcast_chat('%s...' % int(round(remaining)))
             else:
-                self.send_chat('%s seconds remaining.' % int(round(remaining)))
+                self.broadcast_chat('%s seconds remaining.' %
+                                    int(round(remaining)))
         else:
-            self.send_chat('%s minutes remaining.' %
-                           int(round(remaining / 60)))
+            self.broadcast_chat('%s minutes remaining.' %
+                                int(round(remaining / 60)))
 
     def _time_up(self):
         self.advance_call = None
         self.advance_rotation('Time up!')
 
     def advance_rotation(self, message: Optional[str] = None) -> Deferred:
         """
@@ -534,15 +496,15 @@
         self.planned_map = None
         self.on_advance(planned_map)
 
         async def do_advance():
             if message is not None:
                 log.info("advancing to map '{name}' ({reason}) in 10 seconds",
                          name=planned_map.full_name, reason=message)
-                self.send_chat(
+                self.broadcast_chat(
                     '{} Next map: {}.'.format(message, planned_map.full_name),
                     irc=True)
                 await sleep(10)
             else:
                 log.info("advancing to map '{name}'",
                          name=planned_map.full_name)
 
@@ -705,15 +667,15 @@
         """
         network = ip_network(str(ip), strict=False)
         for connection in list(self.connections.values()):
             if ip_address(connection.address[0]) in network:
                 name = connection.name
                 connection.kick(silent=True)
         if duration:
-            duration = reactor.seconds() + duration
+            duration = time.time() + duration
         else:
             duration = None
         self.bans[ip] = (name or '(unknown)', reason, duration)
         self.save_bans()
 
     def remove_ban(self, ip):
         results = self.bans.remove(ip)
@@ -844,29 +806,34 @@
             if me:
                 self.irc_relay.me(msg, do_filter=True)
             else:
                 self.irc_relay.send(msg, do_filter=True)
 
     def send_tip(self):
         line = self.tips[random.randrange(len(self.tips))]
-        self.send_chat(line)
+        self.broadcast_chat(line)
         reactor.callLater(self.tip_frequency * 60, self.send_tip)
 
     # pylint: disable=arguments-differ
     def broadcast_chat(self, value, global_message=True, sender=None,
                        team=None, irc=False):
         """
         Send a chat message to many users
         """
         if irc:
             self.irc_say('* %s' % value)
-        ServerProtocol.send_chat(self, value, global_message, sender, team)
+        ServerProtocol.broadcast_chat(
+            self, value, global_message, sender, team)
 
     # backwards compatability
-    send_chat = broadcast_chat
+    def send_chat(self, *args, **kwargs):
+        """Deprecated: see broadcast_chat"""
+        warnings.warn("use of deprecated send_chat, use broadcast_chat instead",
+                      DeprecationWarning, stacklevel=2)
+        self.broadcast_chat(*args, **kwargs)
 
     # log high CPU usage
 
     def update_world(self):
         last_time = self.last_time
         current_time = reactor.seconds()
         if last_time is not None:
```

### Comparing `piqueserver-1.0.0/piqueserver/ssh.py` & `piqueserver-1.1.1/piqueserver/ssh.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.0.0/piqueserver/statistics.py` & `piqueserver-1.1.1/piqueserver/statistics.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.0.0/piqueserver/statusserver.py` & `piqueserver-1.1.1/piqueserver/statusserver.py`

 * *Files 3% similar despite different names*

```diff
@@ -147,18 +147,17 @@
             web.get('/', self.index)
         ])
         return app
 
     async def listen(self):
         """Starts the status server on configured host/port"""
         app = self.create_app()
-        logger = Logger() if logging_option.get() else None
-        log_class = AccessLogger if logging_option.get() else None
-        runner = web.AppRunner(app,
-                               access_log=logger,
-                               access_log_class=log_class)
+        if logging_option.get():
+            runner = web.AppRunner(app, access_log=Logger(), access_log_class=AccessLogger)
+        else:
+            runner = web.AppRunner(app)
         await as_deferred(runner.setup())
         site = web.TCPSite(runner, host_option.get(), port_option.get())
         await as_deferred(site.start())
 
         # TODO: explain why we do this
         await Deferred()
```

### Comparing `piqueserver-1.0.0/piqueserver/utils/_timeparse.py` & `piqueserver-1.1.1/piqueserver/utils/_timeparse.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.0.0/piqueserver/web/templates/status.html` & `piqueserver-1.1.1/piqueserver/web/templates/status.html`

 * *Files identical despite different names*

### Comparing `piqueserver-1.0.0/piqueserver.egg-info/PKG-INFO` & `piqueserver-1.1.1/piqueserver.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,215 +1,17 @@
 Metadata-Version: 2.1
 Name: piqueserver
-Version: 1.0.0
+Version: 1.1.1
 Summary: Open-Source server implementation for Ace of Spades 
 Home-page: https://github.com/piqueserver/piqueserver
 Author: Originally MatPow2 and PySnip contributors,now, StackOverflow and piqueserver authors
 Author-email: nate.shoffner@gmail.com
 Maintainer: noway421
 Maintainer-email: noway@2ch.hk
 License: GNU General Public License v3
-Description: piqueserver |Build Status| |Build status| |Coverage Status|
-        ===========================================================
-        
-        An Ace of Spades 0.75 server based on
-        `PySnip <https://github.com/NateShoffner/PySnip>`__.
-        
-        \:point_right: Chat with us!
-        ----------------------------
-        
-        -  Gitter: |Join the chat at https://gitter.im/piqueserver/piqueserver|
-        -  Matrix: ``#piqueserver:matrix.org`` (`Riot Webchat
-           link <https://riot.im/app/#/room/#piqueserver:matrix.org>`__)
-        -  Discord: Join with `this invite link <https://discord.gg/w6Te7xC>`__
-        -  Slack: Join with `this invite link <https://join.slack.com/t/piqueserver/shared_invite/enQtMjg5MDI3MTkwNTgxLTNhMDkyNDRkNzhiNmQyYjRkOTdjNGNkYzNhNTQ4NzZkY2JhZjQxYzIyMTQ0Y2JlYTI2ZGFjMTFmNjAwZTM2OGU>`__
-        -  IRC: (disabled due to spam) ``#piqueserver`` on freenode.net
-           (`web <http://webchat.freenode.net/?channels=%23piqueserver>`__)
-        
-        All of these are `bridged <https://matrix.org/docs/guides/faq.html#what-is-matrix>`__ together!
-        
-        \:tada: Features
-        ----------------
-        
-        -  Many administrator features
-        -  A lot of epic commands
-        -  A remote console (using SSH)
-        -  Map rotation
-        -  Map metadata (name, version, author, and map configuration)
-        -  Map extensions (water damage, etc.)
-        -  A map generator
-        -  An IRC client for managing your server
-        -  A JSON query webserver
-        -  A status server with map overview
-        -  Server/map scripts
-        -  Airstrikes
-        -  Melee attacks with the pickaxe
-        -  New gamemodes (deathmatch / runningman)
-        -  Rollback feature (rolling back to the original map)
-        -  Spectator mode
-        -  Dirt grenades
-        -  Platforms with buttons
-        -  Ban subscribe service
-        -  A ton of other features
-        
-        \:rocket: Installation
-        ----------------------
-        
-        Requirements
-        ~~~~~~~~~~~~
-        
-        Piqueserver requires python3.5.3 and above
-        
-        We currently provide builds for:
-         - Linux 32 and 64bit, Python 3.5, 3.6
-         - Windows 32 and 64bit, Python 3.5, 3.6
-         
-        If your system is not one of the above, you will also need a recent C++ Compiler.
-        
-        pip (stable version)
-        ~~~~~~~~~~~~~~~~~~~~
-        
-        .. code:: bash
-        
-            pip3 install piqueserver
-        
-        Optional features:
-        
-        - `ssh`: enable ssh manhole server support
-        - `from`: enable the `from` command to geolocate players by ip
-        
-        To install with optional features with pip:
-        
-        .. code:: bash
-        
-            pip3 install piqueserver[ssh,from]
-        
-        git (bleeding edge)
-        ~~~~~~~~~~~~~~~~~~~
-        
-        .. code:: bash
-        
-            git clone https://github.com/piqueserver/piqueserver
-            cd piqueserver
-            python3 -m venv venv
-            source venv/bin/activate
-        
-            # note: requirements.txt includes all optional deps too
-            pip install -r requirements.txt
-        
-            python setup.py install
-        
-            # now `piqueserver` will be available on the $PATH when venv active
-        
-        Arch Linux
-        ~~~~~~~~~~
-        
-        The `AUR package <https://aur.archlinux.org/packages/piqueserver-git/>`__
-        (git master) is currently broken. When it gets repaired (you can help!),
-        you'll be able to install manually or with your favourite AUR helper:
-        
-        .. code:: bash
-        
-            pacaur -S piqueserver-git
-        
-        \:rocket: Running
-        -----------------
-        
-        Then copy the default configuration as a base to work off
-        
-        .. code:: bash
-        
-            piqueserver --copy-config
-        
-        A-a-and lift off!
-        
-        .. code:: bash
-        
-            piqueserver
-        
-        Custom config location
-        ~~~~~~~~~~~~~~~~~~~~~~
-        
-        If you wish to use a different location to ``~/.config/piqueserver/``
-        for config files, specify a directory with the ``-d`` flag:
-        
-        .. code:: bash
-        
-            piqueserver --copy-config -d custom_dir
-            piqueserver -d custom_dir
-        
-        \:speech_balloon: FAQ
-        ---------------------
-        
-        What's the purpose?
-        ~~~~~~~~~~~~~~~~~~~
-        
-        The purpose of this repo is to be a continuation of PySnip.
-        
-        What if PySnip development returns?
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        Then they would merge our changes and development would be continued
-        there, I guess. The important thing is to keep AoS servers alive.
-        
-        Why should I use piqueserver instead of PySnip/PySpades?
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        -  Multi config installation
-        -  Docker support
-        -  Bug fixes
-        -  Improvements
-        -  Better anti-hacking
-        -  New scripts
-        
-        What about 0.76 support
-        ~~~~~~~~~~~~~~~~~~~~~~~
-        
-        Working with multiple versions is a pain. 0.76 will be suported in the
-        future only.
-        
-        Is that everything?
-        ~~~~~~~~~~~~~~~~~~~
-        
-        Please see also the
-        `Online Documentation <https://piqueserver.readthedocs.io/en/latest/>`__ for more
-        information (readthedocs.io has replaced our wiki).
-        
-        \:blush: Contribute
-        -------------------
-        
-        Don't be shy and submit us a PR or an issue! Help is always appreciated
-        
-        \:wrench: Development
-        ---------------------
-        
-        Use ``python3`` and ``pip`` to setup the development environment:
-        
-        .. code:: bash
-        
-            $ python3 -m venv venv && source venv/bin/activate
-            (venv) $ pip install -r requirements.txt
-            (venv) $ pip install -r dev-requirements.txt # includes dev tools
-            (venv) $ python setup.py develop             # install in-place
-            (venv) $ deactivate # Deactivate virtualenv
-        
-        --------------
-        
-        Brought to you with :heart: by the `piqueserver
-        team <https://github.com/orgs/piqueserver/people>`__.
-        
-        .. |Build Status| image:: https://travis-ci.org/piqueserver/piqueserver.svg?branch=master
-           :target: https://travis-ci.org/piqueserver/piqueserver
-        .. |Build status| image:: https://ci.appveyor.com/api/projects/status/3mayprg9le4lejmm/branch/master?svg=true
-           :target: https://ci.appveyor.com/project/piqueserver/piqueserver/branch/master
-        .. |Coverage Status| image:: https://coveralls.io/repos/github/piqueserver/piqueserver/badge.svg?branch=master
-           :target: https://coveralls.io/github/piqueserver/piqueserver?branch=master
-        .. |Join the chat at https://gitter.im/piqueserver/piqueserver| image:: https://badges.gitter.im/piqueserver/piqueserver.svg
-           :target: https://gitter.im/piqueserver/piqueserver?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
-        
 Keywords: ace of spades,aos,server,pyspades,pysnip,piqueserver
 Platform: Darwin
 Platform: Unix
 Platform: Win32
 Classifier: Intended Audience :: System Administrators
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: MacOS :: MacOS X
@@ -219,11 +21,218 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Twisted
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Games/Entertainment :: First Person Shooters
-Requires-Python: >=3.5.3
+Requires-Python: >=3.7.0
 Description-Content-Type: text/x-rst
-Provides-Extra: ssh
 Provides-Extra: from
+Provides-Extra: ssh
+License-File: LICENSE
+License-File: COPYING.txt
+
+piqueserver |Build Status| |Wheel Status| |Coverage Status|
+===========================================================
+
+An Ace of Spades 0.75 server based on
+`PySnip <https://github.com/NateShoffner/PySnip>`__.
+
+\:point_right: Chat with us!
+----------------------------
+
+-  Gitter: |Join the chat at https://gitter.im/piqueserver/piqueserver|
+-  Matrix: ``#piqueserver:matrix.org`` (`Riot Webchat
+   link <https://riot.im/app/#/room/#piqueserver:matrix.org>`__)
+-  Discord: Join with `this invite link <https://discord.gg/w6Te7xC>`__
+-  Slack: Join with `this invite link <https://join.slack.com/t/piqueserver/shared_invite/enQtMjg5MDI3MTkwNTgxLTNhMDkyNDRkNzhiNmQyYjRkOTdjNGNkYzNhNTQ4NzZkY2JhZjQxYzIyMTQ0Y2JlYTI2ZGFjMTFmNjAwZTM2OGU>`__
+-  IRC: (disabled due to spam) ``#piqueserver`` on freenode.net
+   (`web <http://webchat.freenode.net/?channels=%23piqueserver>`__)
+
+All of these are `bridged <https://matrix.org/docs/guides/faq.html#what-is-matrix>`__ together!
+
+\:tada: Features
+----------------
+
+-  Many administrator features
+-  A lot of epic commands
+-  A remote console (using SSH)
+-  Map rotation
+-  Map metadata (name, version, author, and map configuration)
+-  Map extensions (water damage, etc.)
+-  A map generator
+-  An IRC client for managing your server
+-  A JSON query webserver
+-  A status server with map overview
+-  Server/map scripts
+-  Airstrikes
+-  Melee attacks with the pickaxe
+-  New gamemodes (deathmatch / runningman)
+-  Rollback feature (rolling back to the original map)
+-  Spectator mode
+-  Dirt grenades
+-  Platforms with buttons
+-  Ban subscribe service
+-  A ton of other features
+
+\:rocket: Installation
+----------------------
+
+Requirements
+~~~~~~~~~~~~
+
+Piqueserver requires python 3.7 and above
+
+We currently provide builds for:
+ - Linux x86_64
+ - Windows x86 and x86_64
+ 
+If your system is not one of the above, you will also need a recent C++ Compiler.
+
+pip (stable version)
+~~~~~~~~~~~~~~~~~~~~
+
+.. code:: bash
+
+    pip3 install piqueserver
+
+Optional features:
+
+- `ssh`: enable ssh manhole server support
+- `from`: enable the `from` command to geolocate players by ip
+
+To install with optional features with pip:
+
+.. code:: bash
+
+    pip3 install piqueserver[ssh,from]
+
+git (bleeding edge)
+~~~~~~~~~~~~~~~~~~~
+
+.. code:: bash
+
+    git clone https://github.com/piqueserver/piqueserver
+    cd piqueserver
+    python3 -m venv venv
+    source venv/bin/activate
+
+    # note: requirements.txt includes all optional deps too
+    pip install -r requirements.txt
+
+    python setup.py install
+
+    # now `piqueserver` will be available on the $PATH when venv active
+
+Arch Linux
+~~~~~~~~~~
+
+The `AUR package <https://aur.archlinux.org/packages/piqueserver-git/>`__
+(git master) is currently broken. When it gets repaired (you can help!),
+you'll be able to install manually or with your favourite AUR helper:
+
+.. code:: bash
+
+    pacaur -S piqueserver-git
+
+\:rocket: Running
+-----------------
+
+Then copy the default configuration as a base to work off
+
+.. code:: bash
+
+    piqueserver --copy-config
+
+A-a-and lift off!
+
+.. code:: bash
+
+    piqueserver
+
+Custom config location
+~~~~~~~~~~~~~~~~~~~~~~
+
+If you wish to use a different location to ``~/.config/piqueserver/``
+for config files, specify a directory with the ``-d`` flag:
+
+.. code:: bash
+
+    piqueserver --copy-config -d custom_dir
+    piqueserver -d custom_dir
+
+\:speech_balloon: FAQ
+---------------------
+
+What's the purpose?
+~~~~~~~~~~~~~~~~~~~
+
+The purpose of this repo is to be a continuation of PySnip.
+
+What if PySnip development returns?
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Then they would merge our changes and development would be continued
+there, I guess. The important thing is to keep AoS servers alive.
+
+Why should I use piqueserver instead of PySnip/PySpades?
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+-  Multi config installation
+-  Docker support
+-  Bug fixes
+-  Improvements
+-  Better anti-hacking
+-  New scripts
+
+What about 0.76 support
+~~~~~~~~~~~~~~~~~~~~~~~
+
+Working with multiple versions is a pain. 0.76 will be suported in the
+future only.
+
+Is that everything?
+~~~~~~~~~~~~~~~~~~~
+
+Please see also the
+`Online Documentation <https://piqueserver.readthedocs.io/en/latest/>`__ for more
+information (readthedocs.io has replaced our wiki).
+
+Where can i find more scripts?
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+You can checkout the `Piqueserver Extras Repository <https://github.com/piqueserver/piqueserver-extras>`__, that contains scripts made by the community and ports from PySnip/PySpades script.
+Or in community forums, such as:
+`aloha.pk <https://aloha.pk/c/aos-modding/scripts/83>`__ and `BuildAndShoot <https://www.buildandshoot.com/forums/viewforum.php?f=19>`__
+
+\:blush: Contribute
+-------------------
+
+Don't be shy and submit us a PR or an issue! Help is always appreciated
+
+\:wrench: Development
+---------------------
+
+Use ``python3`` and ``pip`` to setup the development environment:
+
+.. code:: bash
+
+    $ python3 -m venv venv && source venv/bin/activate
+    (venv) $ pip install -r requirements.txt
+    (venv) $ pip install -r dev-requirements.txt # includes dev tools
+    (venv) $ python setup.py develop             # install in-place
+    (venv) $ deactivate # Deactivate virtualenv
+
+--------------
+
+Brought to you with :heart: by the `piqueserver
+team <https://github.com/orgs/piqueserver/people>`__.
+
+.. |Build Status| image:: https://github.com/piqueserver/piqueserver/actions/workflows/main.yml/badge.svg?branch=master
+   :target: https://github.com/piqueserver/piqueserver/actions/workflows/main.yml
+.. |Wheel Status| image:: https://github.com/piqueserver/piqueserver/actions/workflows/wheels.yml/badge.svg?branch=master
+   :target: https://github.com/piqueserver/piqueserver/actions/workflows/wheels.yml
+.. |Coverage Status| image:: https://coveralls.io/repos/github/piqueserver/piqueserver/badge.svg?branch=master
+   :target: https://coveralls.io/github/piqueserver/piqueserver?branch=master
+.. |Join the chat at https://gitter.im/piqueserver/piqueserver| image:: https://badges.gitter.im/piqueserver/piqueserver.svg
+   :target: https://gitter.im/piqueserver/piqueserver?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
```

### Comparing `piqueserver-1.0.0/piqueserver.egg-info/SOURCES.txt` & `piqueserver-1.1.1/piqueserver.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+COPYING.txt
+LICENSE
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 ./pyspades/bytes.pyx
 ./pyspades/common.pyx
 ./pyspades/contained.pyx
```

### Comparing `piqueserver-1.0.0/pyspades/__init__.py` & `piqueserver-1.1.1/pyspades/__init__.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.0.0/pyspades/bytes.pxd` & `piqueserver-1.1.1/pyspades/bytes.pxd`

 * *Files identical despite different names*

### Comparing `piqueserver-1.0.0/pyspades/bytes.pyx` & `piqueserver-1.1.1/pyspades/bytes.pyx`

 * *Files identical despite different names*

### Comparing `piqueserver-1.0.0/pyspades/bytes_c.cpp` & `piqueserver-1.1.1/pyspades/bytes_c.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -90,15 +90,19 @@
     return (unsigned int)read_int(data, big_endian);
 }
 
 // float
 
 inline double read_float(char *data, int big_endian)
 {
-    return _PyFloat_Unpack4((const unsigned char *)data, !big_endian);
+    #if (PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 11)
+        return PyFloat_Unpack4((const char *)data, !big_endian);
+    #else
+        return _PyFloat_Unpack4((const unsigned char *)data, !big_endian);
+    #endif
 }
 
 /*
 write methods
 */
 
 // byte
@@ -162,15 +166,19 @@
 }
 
 // float
 
 inline void write_float(stringstream *ss, double value, int big_endian)
 {
     char out[4];
-    _PyFloat_Pack4(value, (unsigned char *)&out, !big_endian);
+    #if (PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 11)
+        PyFloat_Pack4(value, (char *)&out, !big_endian);
+    #else
+        _PyFloat_Pack4(value, (unsigned char *)&out, !big_endian);
+    #endif
     ss->write(out, 4);
 }
 
 inline void write_string(stringstream *ss, char *data, size_t size)
 {
     ss->write(data, size);
     ss->put(0);
```

### Comparing `piqueserver-1.0.0/pyspades/classicgen_c.cpp` & `piqueserver-1.1.1/pyspades/classicgen_c.cpp`

 * *Files identical despite different names*

### Comparing `piqueserver-1.0.0/pyspades/collision.py` & `piqueserver-1.1.1/pyspades/collision.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.0.0/pyspades/color.py` & `piqueserver-1.1.1/pyspades/color.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.0.0/pyspades/common.pxd` & `piqueserver-1.1.1/pyspades/common.pxd`

 * *Files identical despite different names*

### Comparing `piqueserver-1.0.0/pyspades/common.pyx` & `piqueserver-1.1.1/pyspades/common.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -81,14 +81,16 @@
         try:
             return value.encode('cp437', 'strict')
         except UnicodeError:
             return b'\xFF' + value.encode('utf-8', 'replace')
 
 def decode(value):
     if value is not None:
+        if value == b"":
+            return ""
         if value[0] == 0xFF:
             try:
                 return value[1:].decode('utf-8', 'strict')
             except UnicodeError: # fallback...
                 pass
         return value.decode('cp437', 'replace')
```

### Comparing `piqueserver-1.0.0/pyspades/constants.py` & `piqueserver-1.1.1/pyspades/constants.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,31 +23,35 @@
 # BUILD_BLOCK: place a single block
 # DESTROY_BLOCK: destroy a single block
 # SPADE_DESTROY: destroy the block as well as the blocks directly above and
 #   below it (spade right-click)
 # GRENADE_DESTROY: destroy a 3x3 area around the block
 BUILD_BLOCK, DESTROY_BLOCK, SPADE_DESTROY, GRENADE_DESTROY = range(4)
 BLUE_FLAG, GREEN_FLAG, BLUE_BASE, GREEN_BASE = range(4)
-CHAT_ALL, CHAT_TEAM, CHAT_SYSTEM = range(3)
+(CHAT_ALL, CHAT_TEAM, CHAT_SYSTEM, CHAT_BIG,
+    CHAT_INFO, CHAT_WARNING, CHAT_ERROR) = range(7)
 (WEAPON_KILL, HEADSHOT_KILL, MELEE_KILL, GRENADE_KILL, FALL_KILL,
     TEAM_CHANGE_KILL, CLASS_CHANGE_KILL) = range(7)
 (ERROR_UNDEFINED, ERROR_BANNED, ERROR_TOO_MANY_CONNECTIONS, ERROR_WRONG_VERSION,
     ERROR_FULL, ERROR_SHUTDOWN) = range(6)
 ERROR_KICKED, ERROR_INVALID_NAME = 10, 20
+EXTENSION_PLAYERLIMIT, EXTENSION_CHATTYPE, EXTENSION_KICKREASON = 192, 193, 194
 
 CTF_MODE, TC_MODE = range(2)
 TC_CAPTURE_DISTANCE = 16  # 16 blocks
 TC_CAPTURE_RATE = 0.05
 MIN_TERRITORY_COUNT = 3
 MAX_TERRITORY_COUNT = 7
 NEUTRAL_TEAM = 2
 SPAWN_RADIUS = 32
 MINE_RANGE = 3
 BUILD_TOLERANCE = 5
 
+FOG_DISTANCE = 128.0
+
 MELEE_DISTANCE = 3
 
 MAX_CHAT_SIZE = 90  # more like 95, but just to make sure
 
 RUBBERBAND_DISTANCE = 3
 
 MAX_TIMER_SPEED = 2000
@@ -75,7 +79,14 @@
 }
 
 WEAPON_INTERVAL = {
     RIFLE_WEAPON: 0.2,
     SMG_WEAPON: 0.05,
     SHOTGUN_WEAPON: 0.3
 }
+
+OPENSPADES_CHATTYPES = {
+    CHAT_BIG: "C% ",
+    CHAT_INFO: "N% ",
+    CHAT_WARNING: "%% ",
+    CHAT_ERROR: "!% "
+}
```

### Comparing `piqueserver-1.0.0/pyspades/contained.pyx` & `piqueserver-1.1.1/pyspades/contained.pyx`

 * *Files identical despite different names*

### Comparing `piqueserver-1.0.0/pyspades/entities.py` & `piqueserver-1.1.1/pyspades/entities.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from twisted.internet import reactor
 
 move_object = loaders.MoveObject()
 progress_bar = loaders.ProgressBar()
 territory_capture = loaders.TerritoryCapture()
 
+
 class Entity(Vertex3):
     team = None
 
     def __init__(self, entity_id, protocol, *arg, **kw):
         Vertex3.__init__(self, *arg, **kw)
         self.id = entity_id
         self.protocol = protocol
@@ -22,15 +23,15 @@
             state = NEUTRAL_TEAM
         else:
             state = self.team.id
         move_object.state = state
         move_object.x = self.x
         move_object.y = self.y
         move_object.z = self.z
-        self.protocol.send_contained(move_object, save=True)
+        self.protocol.broadcast_contained(move_object, save=True)
 
 
 class Flag(Entity):
     player = None
 
     def update(self):
         if self.player is not None:
@@ -102,15 +103,15 @@
         rate = self.rate
         progress = self.get_progress()
         if team.id:
             rate = -rate
             progress = 1 - progress
         progress_bar.progress = progress
         progress_bar.rate = rate
-        self.protocol.send_contained(progress_bar)
+        self.protocol.broadcast_contained(progress_bar)
 
     def finish(self):
         self.finish_call = None
         protocol = self.protocol
         if self.rate > 0:
             team = protocol.green_team
         else:
@@ -123,15 +124,15 @@
         if team.score >= protocol.max_score:
             protocol.reset_game(territory=self)
             protocol.on_game_end()
         else:
             territory_capture.object_index = self.id
             territory_capture.state = self.team.id
             territory_capture.winning = False
-            protocol.send_contained(territory_capture)
+            protocol.broadcast_contained(territory_capture)
 
     def get_progress(self, set=False):
         """
         Return progress (between 0 and 1 - 0 is full blue control,
         1 is full green control) and optionally set the current
         progress.
         """
```

### Comparing `piqueserver-1.0.0/pyspades/gamemodes.py` & `piqueserver-1.1.1/pyspades/gamemodes.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.0.0/pyspades/loaders.pxd` & `piqueserver-1.1.1/pyspades/loaders.pxd`

 * *Files identical despite different names*

### Comparing `piqueserver-1.0.0/pyspades/loaders.pyx` & `piqueserver-1.1.1/pyspades/loaders.pyx`

 * *Files identical despite different names*

### Comparing `piqueserver-1.0.0/pyspades/mapgenerator.py` & `piqueserver-1.1.1/pyspades/mapgenerator.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.0.0/pyspades/mapmaker.pyx` & `piqueserver-1.1.1/pyspades/mapmaker.pyx`

 * *Files identical despite different names*

### Comparing `piqueserver-1.0.0/pyspades/master.py` & `piqueserver-1.1.1/pyspades/master.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.0.0/pyspades/packet.pyx` & `piqueserver-1.1.1/pyspades/packet.pyx`

 * *Files identical despite different names*

### Comparing `piqueserver-1.0.0/pyspades/player.py` & `piqueserver-1.1.1/pyspades/player.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,50 @@
 import collections
 import math
 import random
 import re
 import shlex
 import textwrap
 from itertools import product
-from typing import Any, Dict, Optional, Sequence, Tuple, Union
+from typing import Dict, Optional, Sequence, Tuple, Union
 
 import enet
 from twisted.internet import reactor
 from twisted.logger import Logger
 
 from pyspades import contained as loaders
 from pyspades import world
 from pyspades.collision import collision_3d, vector_collision
 from pyspades.common import Vertex3, get_color, make_color
 from pyspades.constants import *
 from pyspades.constants import (BLOCK_TOOL, CTF_MODE, ERROR_FULL,
                                 ERROR_TOO_MANY_CONNECTIONS,
                                 ERROR_WRONG_VERSION, FALL_KILL, HEAD,
                                 HEADSHOT_KILL, HIT_TOLERANCE,
-                                MAX_BLOCK_DISTANCE, MAX_POSITION_RATE, MELEE,
-                                MELEE_DISTANCE, MELEE_KILL,
+                                FOG_DISTANCE, MAX_BLOCK_DISTANCE, MAX_POSITION_RATE,
+                                MELEE, MELEE_DISTANCE, MELEE_KILL,
                                 RAPID_WINDOW_ENTRIES, SPADE_TOOL,
                                 TC_CAPTURE_DISTANCE, TC_MODE, WEAPON_KILL,
                                 WEAPON_TOOL)
 from pyspades.mapgenerator import ProgressiveMapGenerator
 from pyspades.packet import call_packet_handler, register_packet_handler
 from pyspades.protocol import BaseConnection
 from pyspades.team import Team
 from pyspades.weapon import WEAPONS
+from pyspades.types import RateLimiter
 
 log = Logger()
 
 
 tc_data = loaders.TCState()
 
+
 def check_nan(*values) -> bool:
     for value in values:
-        if math.isnan(value):
+        if math.isnan(value) or math.isinf(value):
             return True
     return False
 
 
 def parse_command(value: str) -> Tuple[str, Sequence[str]]:
     try:
         splitted = shlex.split(value)
@@ -52,32 +54,14 @@
     if splitted:
         command = splitted.pop(0)
     else:
         command = ''
     return command, splitted
 
 
-class SlidingWindow:
-    def __init__(self, entries: Any) -> None:
-        self.entries = entries
-        self.window = collections.deque()  # type: Deque
-
-    def add(self, value) -> None:
-        self.window.append(value)
-        if len(self.window) <= self.entries:
-            return
-        self.window.popleft()
-
-    def check(self) -> bool:
-        return len(self.window) == self.entries
-
-    def get(self) -> Any:
-        return self.window[0], self.window[-1]
-
-
 class ServerConnection(BaseConnection):
     address = None  # Tuple[int, int]
     player_id = None
     map_packets_sent = 0
     team = None  # type: Team
     weapon = None
     weapon_object = None
@@ -110,15 +94,15 @@
     def __init__(self, *arg, **kw) -> None:
         BaseConnection.__init__(self, *arg, **kw)
         protocol = self.protocol
         address = self.peer.address
         self.total_blocks_removed = 0
         self.address = (address.host, address.port)
         self.respawn_time = protocol.respawn_time
-        self.rapids = SlidingWindow(RAPID_WINDOW_ENTRIES)
+        self.rapids = RateLimiter(RAPID_WINDOW_ENTRIES, MAX_RAPID_SPEED)
         self.client_info = {}
         self.proto_extensions = {}  # type: Dict[int, int]
         self.line_build_start_pos = None
 
     def on_connect(self) -> None:
         if self.local:
             return
@@ -308,15 +292,15 @@
 
         # remember the current state of the mouse buttons
         self.world_object.primary_fire = primary
         self.world_object.secondary_fire = secondary
         if self.filter_weapon_input:
             return
         contained.player_id = self.player_id
-        self.protocol.send_contained(contained, sender=self)
+        self.protocol.broadcast_contained(contained, sender=self)
 
     @register_packet_handler(loaders.InputData)
     def on_input_data_recieved(self, contained: loaders.InputData) -> None:
         if not self.hp:
             return
         world_object = self.world_object
         returned = self.on_walk_update(contained.up, contained.down,
@@ -361,59 +345,61 @@
                 self.send_contained(contained)
         if not self.freeze_animation:
             world_object.set_animation(
                 contained.jump, contained.crouch, contained.sneak,
                 contained.sprint)
         if self.filter_visibility_data or self.filter_animation_data:
             return
-        self.protocol.send_contained(contained, sender=self)
+        self.protocol.broadcast_contained(contained, sender=self)
 
     @register_packet_handler(loaders.WeaponReload)
     def on_reload_recieved(self, contained) -> None:
         if not self.hp:
             return
         self.weapon_object.reload()
         if self.filter_animation_data:
             return
         contained.player_id = self.player_id
-        self.protocol.send_contained(contained, sender=self)
+        self.protocol.broadcast_contained(contained, sender=self)
 
     @register_packet_handler(loaders.HitPacket)
     def on_hit_recieved(self, contained):
-        if not self.hp:
-            return
         world_object = self.world_object
         value = contained.value
         is_melee = value == MELEE
-        if not is_melee and self.weapon_object.is_empty():
-            return
+        if is_melee:
+            kill_type = MELEE_KILL
+        elif contained.value == HEAD:
+            kill_type = HEADSHOT_KILL
+        else:
+            kill_type = WEAPON_KILL
         try:
             player = self.protocol.players[contained.player_id]
         except KeyError:
             return
-        valid_hit = world_object.validate_hit(player.world_object,
-                                              value, HIT_TOLERANCE)
-        if not valid_hit:
-            return
         position1 = world_object.position
         position2 = player.world_object.position
         if is_melee:
-            if not vector_collision(position1, position2,
-                                    MELEE_DISTANCE):
-                return
             hit_amount = self.protocol.melee_damage
         else:
             hit_amount = self.weapon_object.get_damage(
                 value, position1, position2)
-        if is_melee:
-            kill_type = MELEE_KILL
-        elif contained.value == HEAD:
-            kill_type = HEADSHOT_KILL
-        else:
-            kill_type = WEAPON_KILL
+        self.on_unvalidated_hit(hit_amount, player, kill_type, None)
+        if not self.hp:
+            return
+        if not is_melee and self.weapon_object.is_empty():
+            return
+        valid_hit = world_object.validate_hit(player.world_object,
+                                              value, HIT_TOLERANCE,
+                                              self.rubberband_distance)
+        if not valid_hit:
+            return
+        if is_melee and not vector_collision(position1, position2,
+                                             MELEE_DISTANCE):
+            return
         returned = self.on_hit(hit_amount, player, kill_type, None)
         if returned == False:
             return
         elif returned is not None:
             hit_amount = returned
         player.hit(hit_amount, self, kill_type)
 
@@ -425,29 +411,34 @@
             self.on_hack_attempt("Invalid grenade data")
             return
         if not self.grenades:
             return
         self.grenades -= 1
         if not self.check_speedhack(*contained.position):
             contained.position = self.world_object.position.get()
+        if contained.value > 3.0:
+            contained.value = 3.0
+        velocity = Vertex3(*contained.velocity) - self.world_object.velocity
+        if velocity.length() > 2.0:  # cap at tested maximum
+            velocity = velocity.normal() * 2.0
+        velocity += self.world_object.velocity
         if self.on_grenade(contained.value) == False:
             return
         grenade = self.protocol.world.create_object(
             world.Grenade, contained.value,
             Vertex3(*contained.position), None,
-            Vertex3(*contained.velocity), self.grenade_exploded)
+            velocity, self.grenade_exploded)
         grenade.team = self.team
         log.debug("{player!r} ({world_object!r}) created {grenade!r}",
                   grenade=grenade, world_object=self.world_object, player=self)
         self.on_grenade_thrown(grenade)
         if self.filter_visibility_data:
             return
         contained.player_id = self.player_id
-        self.protocol.send_contained(contained,
-                                     sender=self)
+        self.protocol.broadcast_contained(contained, sender=self)
 
     @register_packet_handler(loaders.SetTool)
     def on_tool_change_recieved(self, contained: loaders.SetTool) -> None:
         if not self.hp:
             return
         if self.on_tool_set_attempt(contained.value) == False:
             return
@@ -462,58 +453,58 @@
         self.world_object.set_weapon(self.tool == WEAPON_TOOL)
         self.on_tool_changed(self.tool)
         if self.filter_visibility_data or self.filter_animation_data:
             return
         set_tool = loaders.SetTool()
         set_tool.player_id = self.player_id
         set_tool.value = contained.value
-        self.protocol.send_contained(set_tool, sender=self, save=True)
+        self.protocol.broadcast_contained(set_tool, sender=self, save=True)
 
     @register_packet_handler(loaders.SetColor)
     def on_color_change_recieved(self, contained: loaders.SetColor) -> None:
         if not self.hp:
             return
         color = get_color(contained.value)
         if self.on_color_set_attempt(color) == False:
             return
         self.color = color
         self.on_color_set(color)
         if self.filter_animation_data:
             return
         contained.player_id = self.player_id
-        self.protocol.send_contained(contained, sender=self,
-                                     save=True)
+        self.protocol.broadcast_contained(contained, sender=self, save=True)
 
     @register_packet_handler(loaders.BlockAction)
     def on_block_action_recieved(self, contained: loaders.BlockAction) -> None:
         world_object = self.world_object
         if not self.hp:
             return
         value = contained.value
+        if value == GRENADE_DESTROY:
+            return
         if value == BUILD_BLOCK:
             interval = TOOL_INTERVAL[BLOCK_TOOL]
         elif self.tool == WEAPON_TOOL:
             if self.weapon_object.is_empty():
                 return
             interval = WEAPON_INTERVAL[self.weapon]
         else:
             interval = TOOL_INTERVAL[self.tool]
         current_time = reactor.seconds()
         last_time = self.last_block
         self.last_block = current_time
         if (self.rapid_hack_detect and last_time is not None and
                 current_time - last_time < interval):
-            self.rapids.add(current_time)
-            if self.rapids.check():
-                start, end = self.rapids.get()
-                if end - start < MAX_RAPID_SPEED:
-                    log.info('RAPID HACK: {window}', window=self.rapids.window)
-                    self.on_hack_attempt('Rapid hack detected')
+            self.rapids.record_event(current_time)
+            if self.rapids.above_limit():
+                log.info('RAPID HACK: {events}',
+                         events=self.rapids.get_events())
+                self.on_hack_attempt('Rapid hack detected')
             return
-        map = self.protocol.map
+        map_ = self.protocol.map
         x = contained.x
         y = contained.y
         z = contained.z
         if z >= 62:
             return
         if value == BUILD_BLOCK:
             self.blocks -= 1
@@ -521,52 +512,66 @@
             if self.blocks < -BUILD_TOLERANCE:
                 return
             elif not collision_3d(pos.x, pos.y, pos.z, x, y, z,
                                   MAX_BLOCK_DISTANCE):
                 return
             elif self.on_block_build_attempt(x, y, z) == False:
                 return
-            elif not map.build_point(x, y, z, self.color):
+            elif not map_.build_point(x, y, z, self.color):
                 return
             self.on_block_build(x, y, z)
         else:
-            if not map.get_solid(x, y, z):
+            if not map_.get_solid(x, y, z):
                 return
             pos = world_object.position
             if self.tool == SPADE_TOOL and not collision_3d(
                     pos.x, pos.y, pos.z, x, y, z, MAX_DIG_DISTANCE):
                 return
             if self.on_block_destroy(x, y, z, value) == False:
                 return
             elif value == DESTROY_BLOCK:
-                count = map.destroy_point(x, y, z)
+                count = map_.destroy_point(x, y, z)
                 if count:
                     self.total_blocks_removed += count
                     self.blocks = min(50, self.blocks + 1)
                     self.on_block_removed(x, y, z)
             elif value == SPADE_DESTROY:
                 for xyz in ((x, y, z), (x, y, z + 1), (x, y, z - 1)):
-                    count = map.destroy_point(*xyz)
+                    count = map_.destroy_point(*xyz)
                     if count:
                         self.total_blocks_removed += count
                         self.on_block_removed(*xyz)
             self.last_block_destroy = reactor.seconds()
         block_action = loaders.BlockAction()
         block_action.x = x
         block_action.y = y
         block_action.z = z
         block_action.value = contained.value
         block_action.player_id = self.player_id
-        self.protocol.send_contained(block_action, save=True)
+        self.protocol.broadcast_contained(block_action, save=True)
         self.protocol.update_entities()
 
     @register_packet_handler(loaders.BlockLine)
     def on_block_line_recieved(self, contained):
         if not self.hp:
             return  # dead players can't build
+        if self.line_build_start_pos is None:
+            return
+
+        current_time = reactor.seconds()
+        last_time = self.last_block
+        self.last_block = current_time
+        if (self.rapid_hack_detect and last_time is not None and
+                current_time - last_time < TOOL_INTERVAL[BLOCK_TOOL]):
+            self.rapids.record_event(current_time)
+            if self.rapids.above_limit():
+                log.info('RAPID HACK: {events}',
+                         events=self.rapids.get_events())
+                self.on_hack_attempt('Rapid hack detected')
+            return
 
         map_ = self.protocol.map
 
         x1, y1, z1 = (contained.x1, contained.y1, contained.z1)
         x2, y2, z2 = (contained.x2, contained.y2, contained.z2)
         pos = self.world_object.position
         start_pos = self.line_build_start_pos
@@ -583,14 +588,21 @@
 
         # ensure that the player was within tolerance of the location
         # that the line build started at
         if not collision_3d(start_pos.x, start_pos.y, start_pos.z, x1, y1, z1,
                             MAX_BLOCK_DISTANCE):
             return
 
+        # check if block can be placed in that location
+        if not map_.has_neighbors(x1, y1, z1):
+            return
+
+        if not map_.has_neighbors(x2, y2, z2):
+            return
+
         points = world.cube_line(x1, y1, z1, x2, y2, z2)
 
         if not points:
             return
 
         if len(points) > (self.blocks + BUILD_TOLERANCE):
             return
@@ -604,22 +616,28 @@
                 continue
             if not map_.build_point(x, y, z, self.color):
                 break
 
         self.blocks -= len(points)
         self.on_line_build(points)
         contained.player_id = self.player_id
-        self.protocol.send_contained(contained, save=True)
+        self.protocol.broadcast_contained(contained, save=True)
         self.protocol.update_entities()
 
     @register_packet_handler(loaders.ChatMessage)
     def on_chat_message_recieved(self, contained: loaders.ChatMessage) -> None:
         if not self.name:
             return
+
         value = contained.value
+        if len(value) > 108:
+            log.info("TOO LONG MESSAGE (%i chars) FROM %s (#%i)" %
+                     (len(value), self.name, self.player_id))
+
+        value = value[:108]
         if value.startswith('/'):
             self.on_command(*parse_command(value[1:]))
         else:
             global_message = contained.chat_type == CHAT_ALL
             result = self.on_chat(value, global_message)
             if result == False:
                 return
@@ -666,28 +684,29 @@
             return
         team = ret or team
         self.set_team(team)
 
     @register_packet_handler(loaders.HandShakeReturn)
     def on_handshake_recieved(self, contained: loaders.HandShakeReturn) -> None:
         version_request = loaders.VersionRequest()
-        self.protocol.send_contained(version_request)
+        self.send_contained(version_request)
 
     @register_packet_handler(loaders.VersionResponse)
     def on_version_info_recieved(self, contained: loaders.VersionResponse) -> None:
         self.client_info["version"] = contained.version
-        self.client_info["os_info"] = contained.os_info
+        self.client_info["os_info"] = contained.os_info[:108]
         # TODO: Make this a dict lookup instead
         if contained.client == 'o':
             self.client_info["client"] = "OpenSpades"
         elif contained.client == 'B':
             self.client_info["client"] = "BetterSpades"
             # BetterSpades currently sends the client name in the OS info to
             # deal with old scripts that don't recognize the 'B' indentifier
-            match = re.match(r"\ABetterSpades \((.*)\)\Z", contained.os_info)
+            match = re.match(r"\ABetterSpades \((.*)\)\Z",
+                             contained.os_info[:108])
             if match:
                 self.client_info["os_info"] = match.groups()[0]
         elif contained.client == 'a':
             self.client_info["client"] = "ACE"
         else:
             self.client_info["client"] = "Unknown({})".format(contained.client)
 
@@ -766,19 +785,19 @@
     def set_location(self, location=None):
         if location is None:
             # used for rubberbanding
             position = self.world_object.position
             x, y, z = position.x, position.y, position.z
         else:
             x, y, z = location
-            if self.world_object is not None:
-                self.world_object.set_position(x, y, z)
             x += 0.5
             y += 0.5
             z -= 0.5
+            if self.world_object is not None:
+                self.world_object.set_position(x, y, z)
         position_data = loaders.PositionData()
         position_data.x = x
         position_data.y = y
         position_data.z = z
         self.send_contained(position_data)
 
     def refill(self, local: bool = False) -> None:
@@ -846,15 +865,15 @@
             create_player.weapon = self.weapon
         create_player.player_id = self.player_id
         create_player.name = self.name
         create_player.team = self.team.id
         if self.filter_visibility_data and not spectator:
             self.send_contained(create_player)
         else:
-            self.protocol.send_contained(create_player, save=True)
+            self.protocol.broadcast_contained(create_player, save=True)
         if not spectator:
             self.on_spawn((x, y, z))
 
         if not self.client_info:
             handshake_init = loaders.HandShakeInit()
             self.send_contained(handshake_init)
 
@@ -865,15 +884,15 @@
         if flag.player is not None:
             return
         if self.on_flag_take() == False:
             return
         flag.player = self
         intel_pickup = loaders.IntelPickup()
         intel_pickup.player_id = self.player_id
-        self.protocol.send_contained(intel_pickup, save=True)
+        self.protocol.broadcast_contained(intel_pickup, save=True)
 
     def capture_flag(self):
         other_team = self.team.other
         flag = other_team.flag
         player = flag.player
         if player is not self:
             return
@@ -884,15 +903,15 @@
                 self.team.score >= self.protocol.max_score):
             self.protocol.reset_game(self)
             self.protocol.on_game_end()
         else:
             intel_capture = loaders.IntelCapture()
             intel_capture.player_id = self.player_id
             intel_capture.winning = False
-            self.protocol.send_contained(intel_capture, save=True)
+            self.protocol.broadcast_contained(intel_capture, save=True)
             flag = other_team.set_flag()
             flag.update()
 
     def drop_flag(self) -> None:
         protocol = self.protocol
         game_mode = protocol.game_mode
         if game_mode == CTF_MODE:
@@ -911,29 +930,29 @@
 
                 flag.player = None
                 intel_drop = loaders.IntelDrop()
                 intel_drop.player_id = self.player_id
                 intel_drop.x = flag.x
                 intel_drop.y = flag.y
                 intel_drop.z = flag.z
-                self.protocol.send_contained(intel_drop, save=True)
+                self.protocol.broadcast_contained(intel_drop, save=True)
                 self.on_flag_drop()
                 break
         elif game_mode == TC_MODE:
             for entity in protocol.entities:
                 if self in entity.players:
                     entity.remove_player(self)
 
     def on_disconnect(self) -> None:
         if self.name is not None:
             self.drop_flag()
             player_left = loaders.PlayerLeft()
             player_left.player_id = self.player_id
-            self.protocol.send_contained(player_left, sender=self,
-                                         save=True)
+            self.protocol.broadcast_contained(player_left, sender=self,
+                                              save=True)
             del self.protocol.players[self.player_id]
         if self.player_id is not None:
             self.protocol.player_ids.put_back(self.player_id)
             self.protocol.update_master()
         self.reset()
 
     def reset(self) -> None:
@@ -952,23 +971,23 @@
 
     def hit(self, value, by=None, kill_type=WEAPON_KILL):
         if self.hp is None:
             return
         if by is not None and self.team is by.team:
             friendly_fire = self.protocol.friendly_fire
             friendly_fire_on_grief = self.protocol.friendly_fire_on_grief
-            if friendly_fire_on_grief:
+            if friendly_fire_on_grief and not friendly_fire:
                 if (kill_type == MELEE_KILL and
                         not self.protocol.spade_teamkills_on_grief):
                     return
                 hit_time = self.protocol.friendly_fire_time
                 if (self.last_block_destroy is None
                         or reactor.seconds() - self.last_block_destroy >= hit_time):
                     return
-            elif not friendly_fire:
+            if not friendly_fire:
                 return
         self.set_hp(self.hp - value, by, kill_type=kill_type)
 
     def set_hp(self, value: Union[int, float], hit_by: Optional['ServerConnection'] = None, kill_type: int = WEAPON_KILL,
                hit_indicator: Optional[Tuple[float, float, float]] = None, grenade: Optional[world.Grenade] = None) -> None:
         value = int(value)
         self.hp = max(0, min(100, value))
@@ -992,15 +1011,15 @@
     def set_weapon(self, weapon: int, local: bool = False, no_kill: bool = False) -> None:
         self.weapon = weapon
         if self.weapon_object is not None:
             self.weapon_object.reset()
         self.weapon_object = WEAPONS[weapon](self._on_reload)
         if not local:
             change_weapon = loaders.ChangeWeapon()
-            self.protocol.send_contained(change_weapon, save=True)
+            self.protocol.broadcast_contained(change_weapon, save=True)
             if not no_kill:
                 self.kill(kill_type=CLASS_CHANGE_KILL)
 
     def set_team(self, team):
         if team is self.team:
             return
         self.drop_flag()
@@ -1026,15 +1045,15 @@
             kill_action.killer_id = kill_action.player_id = self.player_id
         else:
             kill_action.killer_id = by.player_id
             kill_action.player_id = self.player_id
         if by is not None and by is not self:
             by.add_score(1)
         kill_action.respawn_time = self.get_respawn_time() + 1
-        self.protocol.send_contained(kill_action, save=True)
+        self.protocol.broadcast_contained(kill_action, save=True)
         self.world_object.dead = True
         self.respawn()
 
     def add_score(self, score):
         self.kills += score
 
     def _connection_ack(self) -> None:
@@ -1139,14 +1158,15 @@
         for player_list in (self.team.other.get_players(), (self,)):
             for player in player_list:
                 if not player.hp:
                     continue
                 damage = grenade.get_damage(player.world_object.position)
                 if damage == 0:
                     continue
+                self.on_unvalidated_hit(damage, player, GRENADE_KILL, grenade)
                 returned = self.on_hit(damage, player, GRENADE_KILL, grenade)
                 if returned == False:
                     continue
                 elif returned is not None:
                     damage = returned
                 player.set_hp(player.hp - damage, self,
                               hit_indicator=position.get(), kill_type=GRENADE_KILL,
@@ -1161,15 +1181,15 @@
                 self.on_block_removed(n_x, n_y, n_z)
         block_action = loaders.BlockAction()
         block_action.x = x
         block_action.y = y
         block_action.z = z
         block_action.value = GRENADE_DESTROY
         block_action.player_id = self.player_id
-        self.protocol.send_contained(block_action, save=True)
+        self.protocol.broadcast_contained(block_action, save=True)
         self.protocol.update_entities()
 
     def _on_fall(self, damage: int) -> None:
         if not self.hp:
             return
         returned = self.on_fall(damage)
         if returned is False:
@@ -1212,19 +1232,28 @@
 
     def continue_map_transfer(self) -> None:
         self.send_map()
 
     def send_data(self, data):
         self.protocol.transport.write(data, self.address)
 
-    def send_chat(self, value: str, global_message: bool = False) -> None:
+    def send_chat(self, value: str, global_message: bool = False, custom_type: int = CHAT_ALL) -> None:
         if self.deaf:
             return
         chat_message = loaders.ChatMessage()
-        if not global_message:
+        if custom_type > 2 and "client" in self.client_info:
+            if EXTENSION_CHATTYPE in self.proto_extensions:
+                chat_message.chat_type = custom_type
+            else:
+                value = OPENSPADES_CHATTYPES[custom_type] + value
+
+            chat_message.player_id = 35
+            prefix = ''
+
+        elif not global_message:
             chat_message.chat_type = CHAT_SYSTEM
             prefix = ''
         else:
             chat_message.chat_type = CHAT_TEAM
             # 34 is guaranteed to be out of range!
             chat_message.player_id = 35
             prefix = self.protocol.server_prefix + ' '
@@ -1234,38 +1263,38 @@
         for line in lines:
             chat_message.value = '{}{}'.format(prefix, line)
             self.send_contained(chat_message)
 
     def send_chat_warning(self, message):
         """
         Send a warning message. This gets displayed as a yellow popup
-        with sound for OpenSpades clients
+        with sound for OpenSpades/BetterSpades clients
         """
-        self.send_chat("%% " + str(message))
+        self.send_chat(message, custom_type=CHAT_WARNING)
 
     def send_chat_notice(self, message):
         """
-        Send a notice. This gets displayed as a popup for OpenSpades
+        Send a notice. This gets displayed as a popup for OpenSpades/Betterspades
         clients
         """
-        self.send_chat("N% " + str(message))
+        self.send_chat(message, custom_type=CHAT_INFO)
 
     def send_chat_error(self, message):
         """
         Send a error message. This gets displayed as a red popup with
-        sound for OpenSpades clients
+        sound for OpenSpades/Betterspades clients
         """
-        self.send_chat("!% " + str(message))
+        self.send_chat(message, custom_type=CHAT_ERROR)
 
     def send_chat_status(self, message):
         """
         Send a status message. This gets displayed in the center of the
-        screen for OpenSpades clients
+        screen for OpenSpades/Betterspades clients
         """
-        self.send_chat("C% " + str(message))
+        self.send_chat(message, custom_type=CHAT_BIG)
 
     # events/hooks
 
     def on_join(self):
         pass
 
     def on_login(self, name):
@@ -1285,14 +1314,17 @@
 
     def on_command(self, command, parameters):
         pass
 
     def on_hit(self, hit_amount, hit_player, kill_type, grenade):
         pass
 
+    def on_unvalidated_hit(self, hit_amount, hit_player, kill_type, grenade):
+        pass
+
     def on_kill(self, killer, kill_type, grenade):
         pass
 
     def on_team_join(self, team):
         pass
 
     def on_team_changed(self, old_team: Team) -> None:
```

### Comparing `piqueserver-1.0.0/pyspades/protocol.py` & `piqueserver-1.1.1/pyspades/protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with pyspades.  If not, see <http://www.gnu.org/licenses/>.
 
+import asyncio
 from twisted.internet import reactor
-from twisted.internet.task import LoopingCall
 from pyspades.bytes import ByteWriter
 
 import enet
 
 
 class BaseConnection:
     disconnected = False
@@ -85,16 +85,15 @@
         try:
             self.host = enet.Host(address, self.max_connections, 1)
         except MemoryError:
             # pyenet raises memoryerror when the enet host could not be created
             raise IOError("Failed  to Create Enet Host. Is the Port in use?")
 
         self.host.compress_with_range_coder()
-        self.update_loop = LoopingCall(self.update)
-        self.update_loop.start(update_interval, False)
+        self.update_loop = asyncio.ensure_future(self.update())
         self.connections = {}
         self.clients = {}
 
     def connect(self, connection_class, host, port, version, channel_count=1,
                 timeout=5.0):
         host = host.encode()
         peer = self.host.connect(enet.Address(host, port), channel_count,
```

### Comparing `piqueserver-1.0.0/pyspades/server.py` & `piqueserver-1.1.1/pyspades/server.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,16 +12,20 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with pyspades.  If not, see <http://www.gnu.org/licenses/>.
 
 import random
+import warnings
 from itertools import product
 import enet
+import time
+import asyncio
+import traceback
 
 from pyspades.protocol import BaseProtocol
 from pyspades.constants import (
     CTF_MODE, TC_MODE, GAME_VERSION, MIN_TERRITORY_COUNT, MAX_TERRITORY_COUNT,
     UPDATE_FREQUENCY, UPDATE_FPS, NETWORK_FPS)
 from pyspades.types import IDPool
 from pyspades.master import get_master_connection
@@ -30,15 +34,17 @@
 # importing tc_data is a quick hack since this file writes into it
 from pyspades.player import ServerConnection, tc_data
 from pyspades import world
 from pyspades.bytes import ByteWriter
 from pyspades import contained as loaders
 from pyspades.common import make_color
 from pyspades.mapgenerator import ProgressiveMapGenerator
+from twisted.logger import Logger
 
+log = Logger()
 
 
 class ServerProtocol(BaseProtocol):
     connection_class = ServerConnection
 
     name = 'pyspades server'
     game_mode = CTF_MODE
@@ -61,15 +67,14 @@
     world = None
     team_class = Team
     team1_color = (0, 0, 196)
     team2_color = (0, 196, 0)
     team1_name = 'Blue'
     team2_name = 'Green'
     spectator_name = 'Spectator'
-    loop_count = 0
     melee_damage = 100
     version = GAME_VERSION
     respawn_waves = False
 
     def __init__(self, *arg, **kw):
         # +2 to allow server->master and master->server connection since enet
         # allocates peers for both clients and hosts. this is done at
@@ -94,14 +99,17 @@
         # product(repeat=3) is the equivalent of 3 nested for loops
         self.pos_table = list(product(range(-5, 6), repeat=3))
 
         self.pos_table.sort(key=lambda vec: abs(vec[0] * 1.03) +
                             abs(vec[1] * 1.02) +
                             abs(vec[2] * 1.01))
 
+        self.last_network_update = self.world_time = time.monotonic()
+        self.loop_count = 0
+
     def _create_teams(self):
         """create the teams
         This Method is separate to simplify unit testing
         """
         self.team_spectator = self.team_class(-1, self.spectator_name,
                                               (0, 0, 0), True, self)
         self.team_1 = self.team_class(0, self.team1_name, self.team1_color,
@@ -166,15 +174,20 @@
             if player.saved_loaders is not None:
                 if save:
                     player.saved_loaders.append(data)
             else:
                 player.peer.send(0, packet)
 
     # backwards compatability
-    send_contained = broadcast_contained
+    def send_contained(self, *args, **kwargs):
+        """Deprecated: see broadcast_contained"""
+        warnings.warn("use of deprecated send_contained,"
+                      " use broadcast_contained instead",
+                      DeprecationWarning, stacklevel=2)
+        self.broadcast_contained(*args, **kwargs)
 
     def reset_tc(self):
         self.entities = self.get_cp_entities()
         for entity in self.entities:
             team = entity.team
             if team is None:
                 entity.progress = 0.5
@@ -205,34 +218,60 @@
             else:
                 # odd number - neutral
                 team = None
             flag.team = team
             entities.append(flag)
         return entities
 
-    def update(self):
-        self.loop_count += 1
-        BaseProtocol.update(self)
-        for player in self.connections.values():
-            if (player.map_data is not None and
-                    not player.peer.reliableDataInTransit):
-                player.continue_map_transfer()
-        self.world.update(UPDATE_FREQUENCY)
-        self.on_world_update()
-        if self.loop_count % int(UPDATE_FPS / NETWORK_FPS) == 0:
-            self.update_network()
+    async def update(self):
+        while True:
+            start_time = time.monotonic()
+            # Notify if update starts more than 4ms later than requested
+            lag = start_time - self.world_time - UPDATE_FREQUENCY
+            if lag > 0.004:
+                log.debug(
+                    "LAG before world update: {lag:.0f} ms", lag=lag * 1000)
+
+            BaseProtocol.update(self)
+            # Map transfer
+            for player in self.connections.values():
+                if (player.map_data is not None and
+                        not player.peer.reliableDataInTransit):
+                    player.continue_map_transfer()
+            # Update world
+            while (time.monotonic() - self.world_time) > UPDATE_FREQUENCY:
+                self.loop_count += 1
+                self.world.update(UPDATE_FREQUENCY)
+                try:
+                    self.on_world_update()
+                except Exception:
+                    traceback.print_exc()
+                self.world_time += UPDATE_FREQUENCY
+            # Update network
+            if time.monotonic() - self.last_network_update >= 1 / NETWORK_FPS:
+                self.last_network_update = self.world_time
+                self.update_network()
+
+            # Notify if update uses more than 70% of time budget
+            lag = time.monotonic() - start_time
+            if lag > (UPDATE_FREQUENCY * 0.7):
+                log.debug("world update LAG: {lag:.0f} ms", lag=lag * 1000)
+
+            delay = self.world_time + UPDATE_FREQUENCY - time.monotonic()
+            await asyncio.sleep(delay)
 
     def update_network(self):
+        if not len(self.players):
+            return
         items = []
-        highest_player_id = 0
-        for i in range(32):
+        highest_player_id = max(self.players)
+        for i in range(highest_player_id + 1):
             position = orientation = None
             try:
                 player = self.players[i]
-                highest_player_id = i
                 if (not player.filter_visibility_data and
                         not player.team.spectator):
                     world_object = player.world_object
                     position = world_object.position.get()
                     orientation = world_object.orientation.get()
             except (KeyError, TypeError, AttributeError):
                 pass
@@ -240,15 +279,15 @@
                 position = (0.0, 0.0, 0.0)
                 orientation = (0.0, 0.0, 0.0)
             items.append((position, orientation))
         world_update = loaders.WorldUpdate()
         # we only want to send as many items of the player list as needed, so
         # we slice it off at the highest player id
         world_update.items = items[:highest_player_id+1]
-        self.send_contained(world_update, unsequenced=True)
+        self.broadcast_contained(world_update, unsequenced=True)
 
     def set_map(self, map_obj):
         self.map = map_obj
         self.world.map = map_obj
         self.on_map_change(map_obj)
         self.team_1.initialize()
         self.team_2.initialize()
@@ -278,33 +317,34 @@
         self.team_2.initialize()
         if self.game_mode == CTF_MODE:
             if player is None:
                 player = list(self.players.values())[0]
             intel_capture = loaders.IntelCapture()
             intel_capture.player_id = player.player_id
             intel_capture.winning = True
-            self.send_contained(intel_capture, save=True)
+            self.broadcast_contained(intel_capture, save=True)
         elif self.game_mode == TC_MODE:
             if territory is None:
                 territory = self.entities[0]
             territory_capture = loaders.TerritoryCapture()
             territory_capture.object_index = territory.id
             territory_capture.winning = True
             territory_capture.state = territory.team.id
-            self.send_contained(territory_capture)
+            self.broadcast_contained(territory_capture)
             self.reset_tc()
         for entity in self.entities:
             entity.update()
         for player in self.players.values():
             if player.team is not None:
                 player.spawn()
 
     def get_name(self, name):
         '''
-        Sanitizes `name` and modifies it so that it doesn't collide with other names connected to the server.
+        Sanitizes `name` and modifies it so that it doesn't
+        collide with other names connected to the server.
 
         Returns the fixed name.
         '''
         name = name.replace('%', '')
         new_name = name
         names = [p.name.lower() for p in self.players.values()]
         i = 0
@@ -383,53 +423,58 @@
             if player.deaf:
                 continue
             if team is not None and player.team is not team:
                 continue
             player.send_chat(message, global_message)
 
     # backwards compatability
-    send_chat = broadcast_chat
+    def send_chat(self, *args, **kwargs):
+        """Deprecated: see broadcast_chat"""
+        warnings.warn("use of deprecated send_chat,"
+                      " use broadcast_chat instead",
+                      DeprecationWarning, stacklevel=2)
+        self.broadcast_chat(*args, **kwargs)
 
     def broadcast_chat_warning(self, message, team=None):
         """
         Send a warning message. This gets displayed
         as a yellow popup with sound for OpenSpades
         clients
         """
-        self.send_chat(self, "%% " + str(message), team=team)
+        self.broadcast_chat(self, "%% " + str(message), team=team)
 
     def broadcast_chat_notice(self, message, team=None):
         """
         Send a warning message. This gets displayed
         as a popup for OpenSpades
         clients
         """
-        self.send_chat(self, "N% " + str(message), team=team)
+        self.broadcast_chat(self, "N% " + str(message), team=team)
 
     def broadcast_chat_error(self, message, team=None):
         """
         Send a warning message. This gets displayed
         as a red popup with sound for OpenSpades
         clients
         """
-        self.send_chat(self, "!% " + str(message), team=team)
+        self.broadcast_chat(self, "!% " + str(message), team=team)
 
     def broadcast_chat_status(self, message, team=None):
         """
         Send a warning message. This gets displayed as a message in the status
         area at the top of the screen, where events such as intel pickups are
         also displayed.
         """
-        self.send_chat(self, "C% " + str(message), team=team)
+        self.broadcast_chat(self, "C% " + str(message), team=team)
 
     def set_fog_color(self, color):
         self.fog_color = color
         fog_color = loaders.FogColor()
         fog_color.color = make_color(*color)
-        self.send_contained(fog_color, save=True)
+        self.broadcast_contained(fog_color, save=True)
 
     def get_fog_color(self):
         return self.fog_color
 
     # events
 
     def on_cp_capture(self, cp):
```

### Comparing `piqueserver-1.0.0/pyspades/tools.py` & `piqueserver-1.1.1/pyspades/tools.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.0.0/pyspades/types.py` & `piqueserver-1.1.1/pyspades/types.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 AttributeSet is used for testing if various settings are active
 
 MultikeyDict is used to make player names accessible by both id and name
 """
 
 import itertools
-from collections import namedtuple
+from collections import deque
 
 
 class IDPool:
     """
     Manage pool of IDs
 
     >>> p = IDPool(start=10)
@@ -85,7 +85,36 @@
         return name in self
 
     def __setattr__(self, name, value):
         if value:
             self.add(name)
         else:
             self.discard(name)
+
+
+class RateLimiter:
+    """sliding window rate limiter
+
+    Triggers if more than a certain number of events happen in a certain amount
+    of time"""
+    def __init__(self, event_count: int, seconds: float) -> None:
+        """limit is event_count events in seconds"""
+        self._seconds = seconds
+        self._window = deque(maxlen=event_count)  # type: deque
+
+    def record_event(self, timestamp: float) -> None:
+        """record an event at the given timestamp"""
+        self._window.append(timestamp)
+
+    def above_limit(self) -> bool:
+        if len(self._window) != self._window.maxlen:
+            # not enough events yet
+            return False
+
+        start, end = self._window[0], self._window[-1]
+
+        if end - start < self._seconds:
+            return True
+        return False
+
+    def get_events(self) -> list:
+        return list(self._window)
```

### Comparing `piqueserver-1.0.0/pyspades/vxl.pxd` & `piqueserver-1.1.1/pyspades/vxl.pxd`

 * *Files identical despite different names*

### Comparing `piqueserver-1.0.0/pyspades/vxl.pyx` & `piqueserver-1.1.1/pyspades/vxl.pyx`

 * *Files identical despite different names*

### Comparing `piqueserver-1.0.0/pyspades/vxl_c.cpp` & `piqueserver-1.1.1/pyspades/vxl_c.cpp`

 * *Files identical despite different names*

### Comparing `piqueserver-1.0.0/pyspades/vxl_c.h` & `piqueserver-1.1.1/pyspades/vxl_c.h`

 * *Files identical despite different names*

### Comparing `piqueserver-1.0.0/pyspades/weapon.py` & `piqueserver-1.1.1/pyspades/weapon.py`

 * *Files identical despite different names*

### Comparing `piqueserver-1.0.0/pyspades/world.pyx` & `piqueserver-1.1.1/pyspades/world.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 cdef extern from "world_c.cpp":
     enum:
         CUBE_ARRAY_LENGTH
     int c_validate_hit "validate_hit" (
         float shooter_x, float shooter_y, float shooter_z,
         float orientation_x, float orientation_y, float orientation_z,
-        float victim_x, float victim_y, float victim_z, float tolerance)
+        float victim_x, float victim_y, float victim_z, float aim_tolerance, float dist_tolerance)
     int c_can_see "can_see" (MapData * map, float x0, float y0, float z0,
         float x1, float y1, float z1)
     int c_cast_ray "cast_ray" (MapData * map, float x0, float y0, float z0,
         float x1, float y1, float z1, float length, long* x, long* y, long* z)
     size_t cube_line_c "cube_line"(int, int, int, int, int, int, LongVector *)
     void set_globals(MapData * map, float total_time, float dt)
     struct PlayerType:
@@ -165,14 +165,15 @@
             self.primary_fire = self.secondary_fire = False
             self.jump = self.crouch = False
             self.up = self.down = self.left = self.right = False
 
     def set_orientation(self, x, y, z):
         """set the current orientation of the Player"""
         cdef Vertex3 v = Vertex3(x, y, z)
+        v.normalize()
         reorient_player(self.player, v.value)
 
     cpdef int can_see(self, float x, float y, float z):
         """return if the player can see a given coordinate. This only considers
         the map voxels, not any other objects"""
         cdef Vertex3 position = self.position
         return can_see(self.world.map, position.x, position.y, position.z,
@@ -185,15 +186,15 @@
         cdef Vertex3 direction = self.orientation.copy().normal()
         cdef long x, y, z
         if cast_ray(self.world.map, position.x, position.y, position.z,
             direction.x, direction.y, direction.z, length, &x, &y, &z):
             return x, y, z
         return None
 
-    def validate_hit(self, Character other, part, float tolerance):
+    def validate_hit(self, Character other, part, float aim_tolerance, float dist_tolerance):
         """check if a given hit is within a given tolerance of hitting another
         player. This is primarily used to prevent players from shooting at
         things they aren't facing at"""
         cdef Vertex3 position1 = self.position
         cdef Vertex3 orientation = self.orientation
         cdef Vertex3 position2 = other.position
         cdef float x, y, z
@@ -208,15 +209,15 @@
             z += 1.8
         elif part == MELEE:
             z += 0.9
         else:
             return False
         if not c_validate_hit(position1.x, position1.y, position1.z,
                               orientation.x, orientation.y, orientation.z,
-                              x, y, z, tolerance):
+                              x, y, z, aim_tolerance, dist_tolerance):
             return False
         return True
 
     def set_dead(self, value):
         """set the player's alive status. Also resets mouse buttons, movement
         stats and keys"""
         self.player.alive = not value
```

### Comparing `piqueserver-1.0.0/pyspades/world_c.cpp` & `piqueserver-1.1.1/pyspades/world_c.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 #define WEAPON_PRIMARY 1
 
 // common.h
 #define CUBE_ARRAY_LENGTH 64
 #include "common_c.h"
 #include <cmath>
 
+#define FOG_DISTANCE 128
+
 enum damage_index
 {
     BODY_TORSO,
     BODY_HEAD,
     BODY_ARMS,
     BODY_LEGS,
     BODY_MELEE
@@ -88,28 +90,31 @@
 {
     return sqrtf(pow(x2 - x1, 2) + pow(y2 - y1, 2) + pow(z2 - z1, 2));
 }
 
 int validate_hit(float shooter_x, float shooter_y, float shooter_z,
                  float orientation_x, float orientation_y, float orientation_z,
                  float ox, float oy, float oz,
-                 float tolerance)
+                 float aim_tolerance, float dist_tolerance)
 {
-    Orientation o;
-    get_orientation(&o, orientation_x, orientation_y, orientation_z);
     ox -= shooter_x;
     oy -= shooter_y;
+    if (sqrtf(ox * ox + oy * oy) > FOG_DISTANCE + dist_tolerance)
+        return 0;
     oz -= shooter_z;
+    
+    Orientation o;
+    get_orientation(&o, orientation_x, orientation_y, orientation_z);
     float cz = ox * o.f.x + oy * o.f.y + oz * o.f.z;
     float r = 1.f / cz;
     float cx = ox * o.s.x + oy * o.s.y + oz * o.s.z;
     float x = cx * r;
     float cy = ox * o.h.x + oy * o.h.y + oz * o.h.z;
     float y = cy * r;
-    r *= tolerance;
+    r *= aim_tolerance;
     int ret = (x - r < 0 && x + r > 0 && y - r < 0 && y + r > 0);
 #if 0
     if (!ret) {
         printf("hit test failed: %f %f %f\n", x, y, r);
     }
 #endif
     return ret;
@@ -233,16 +238,16 @@
     ftol(f.x * g.z - f.z * g.x, &p.x);
     ftol(g.x, &i.x);
     ftol(f.y * g.z - f.z * g.y, &p.y);
     ftol(g.y, &i.y);
     ftol(f.y * g.x - f.x * g.y, &p.z);
     ftol(g.z, &i.z);
 
-    if (cnt > 32)
-        cnt = 32;
+    if (cnt > FOG_DISTANCE)
+        cnt = FOG_DISTANCE;
     while (cnt)
     {
         if (((p.x | p.y) >= 0) && (a.z != c.z))
         {
             a.z += d.z;
             p.x -= i.x;
             p.y -= i.y;
@@ -493,14 +498,16 @@
     if (f > -0.25f)
         p->e.z += (f + 0.25f) / 0.25f;
 }
 
 inline void set_orientation_vectors(Vector *o, Vector *s, Vector *h)
 {
     float f = sqrtf(o->x * o->x + o->y * o->y);
+    if (f == 0)
+        return;
     s->x = -o->y / f;
     s->y = o->x / f;
     h->x = -o->z * s->y;
     h->y = o->z * s->x;
     h->z = o->x * s->y - o->y * s->x;
 }
```

### Comparing `piqueserver-1.0.0/setup.py` & `piqueserver-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
     maintainer_email='noway@2ch.hk',
     license='GNU General Public License v3',
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/piqueserver/piqueserver",
     keywords=['ace of spades', 'aos', 'server',
               'pyspades', 'pysnip', 'piqueserver'],
-    python_requires=">=3.5.3",
+    python_requires=">=3.7.0",
     classifiers=[
         'Intended Audience :: System Administrators',
         'Development Status :: 5 - Production/Stable',
         'Operating System :: MacOS :: MacOS X',
         'Operating System :: Unix',
         'Operating System :: Microsoft :: Windows',
         'Environment :: Console',
@@ -134,23 +134,23 @@
     platforms="Darwin, Unix, Win32",
 
     setup_requires=['Cython>=0.27,<1'],
     install_requires=[
         'pypiwin32;platform_system=="Windows"',
         'Cython>=0.27,<1',
         'Twisted[tls]',
-        'Jinja2>=2,<3',
-        'Pillow>=5.1.0,<7',
-        'aiohttp>=3.3.0,<3.7.0',
+        'Jinja2>=2,<4',
+        'Pillow>=5.1.0,<11',
+        'aiohttp>=3.3.0,<3.8.0',
         'pyenet',
         'toml',
         'packaging>=19.0'
     ],
     extras_require={
-        'from': ['geoip2>=2.9,<3.0'],
+        'from': ['geoip2>=2.9,<5.0'],
         'ssh': ['Twisted[tls,conch]'],
     },
     entry_points={
         'console_scripts': [
             '%s=%s.run:main' % (PKG_NAME, PKG_NAME)
         ],
     },
```

