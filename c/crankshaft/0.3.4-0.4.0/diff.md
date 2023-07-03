# Comparing `tmp/crankshaft-0.3.4.tar.gz` & `tmp/crankshaft-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crankshaft-0.3.4.tar", max compression
+gzip compressed data, was "crankshaft-0.4.0.tar", max compression
```

## Comparing `crankshaft-0.3.4.tar` & `crankshaft-0.4.0.tar`

### file list

```diff
@@ -1,61 +1,62 @@
--rw-r--r--   0        0        0     1067 2023-06-18 19:37:51.797795 crankshaft-0.3.4/LICENSE
--rw-r--r--   0        0        0      336 2023-06-18 19:37:51.797795 crankshaft-0.3.4/README.md
--rw-r--r--   0        0        0      326 2023-06-18 19:39:33.866312 crankshaft-0.3.4/crankshaft/__init__.py
--rw-r--r--   0        0        0      120 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/api.bolt
--rw-r--r--   0        0        0      216 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/config.bolt
--rw-r--r--   0        0        0      513 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/defer.bolt
--rw-r--r--   0        0        0     3891 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/event_handler.bolt
--rw-r--r--   0        0        0     1441 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/events/on_entity_attack_player.bolt
--rw-r--r--   0        0        0      258 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/events/on_load.bolt
--rw-r--r--   0        0        0      355 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/events/on_player_airborne.bolt
--rw-r--r--   0        0        0      679 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/events/on_player_airborne_end.bolt
--rw-r--r--   0        0        0      680 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/events/on_player_airborne_start.bolt
--rw-r--r--   0        0        0     1441 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/events/on_player_attack_entity.bolt
--rw-r--r--   0        0        0      344 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/events/on_player_burn.bolt
--rw-r--r--   0        0        0      668 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/events/on_player_burn_end.bolt
--rw-r--r--   0        0        0      669 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/events/on_player_burn_start.bolt
--rw-r--r--   0        0        0      370 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/events/on_player_charge_bow.bolt
--rw-r--r--   0        0        0      797 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/events/on_player_charge_bow_end.bolt
--rw-r--r--   0        0        0      798 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/events/on_player_charge_bow_start.bolt
--rw-r--r--   0        0        0      346 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/events/on_player_glide.bolt
--rw-r--r--   0        0        0      671 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/events/on_player_glide_end.bolt
--rw-r--r--   0        0        0      672 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/events/on_player_glide_start.bolt
--rw-r--r--   0        0        0      637 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/events/on_player_inventory_change.bolt
--rw-r--r--   0        0        0      577 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/events/on_player_join.bolt
--rw-r--r--   0        0        0      585 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/events/on_player_jump.bolt
--rw-r--r--   0        0        0      686 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/events/on_player_land.bolt
--rw-r--r--   0        0        0      411 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/events/on_player_load.bolt
--rw-r--r--   0        0        0      597 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/events/on_player_shoot_bow.bolt
--rw-r--r--   0        0        0      349 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/events/on_player_sneak.bolt
--rw-r--r--   0        0        0      674 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/events/on_player_sneak_end.bolt
--rw-r--r--   0        0        0      675 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/events/on_player_sneak_start.bolt
--rw-r--r--   0        0        0      354 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/events/on_player_sprint.bolt
--rw-r--r--   0        0        0      679 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/events/on_player_sprint_end.bolt
--rw-r--r--   0        0        0      680 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/events/on_player_sprint_start.bolt
--rw-r--r--   0        0        0      347 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/events/on_player_swim.bolt
--rw-r--r--   0        0        0      672 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/events/on_player_swim_end.bolt
--rw-r--r--   0        0        0      673 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/events/on_player_swim_start.bolt
--rw-r--r--   0        0        0      271 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/events/on_player_tick.bolt
--rw-r--r--   0        0        0      537 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/events/on_player_use_coas.bolt
--rw-r--r--   0        0        0      258 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/events/on_tick.bolt
--rw-r--r--   0        0        0     2061 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/events.bolt
--rw-r--r--   0        0        0     3398 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/flag.bolt
--rw-r--r--   0        0        0      377 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/flags/is_airborne.bolt
--rw-r--r--   0        0        0      402 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/flags/is_baby.bolt
--rw-r--r--   0        0        0      411 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/flags/is_burning.bolt
--rw-r--r--   0        0        0     1248 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/flags/is_charging_bow.bolt
--rw-r--r--   0        0        0      377 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/flags/is_gliding.bolt
--rw-r--r--   0        0        0      379 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/flags/is_in_ground.bolt
--rw-r--r--   0        0        0      379 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/flags/is_on_ground.bolt
--rw-r--r--   0        0        0      158 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/flags/is_player.bolt
--rw-r--r--   0        0        0      414 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/flags/is_sneaking.bolt
--rw-r--r--   0        0        0      417 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/flags/is_sprinting.bolt
--rw-r--r--   0        0        0      414 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/flags/is_swimming.bolt
--rw-r--r--   0        0        0      535 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/flags.bolt
--rw-r--r--   0        0        0      443 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/lib/entity_hit_matching/api.bolt
--rw-r--r--   0        0        0      124 2023-06-18 19:37:51.797795 crankshaft-0.3.4/crankshaft/modules/lib/entity_hit_matching/credits.txt
--rw-r--r--   0        0        0    58208 2023-06-18 19:37:51.801795 crankshaft-0.3.4/crankshaft/modules/lib/entity_hit_matching/main.bolt
--rw-r--r--   0        0        0      208 2023-06-18 19:37:51.801795 crankshaft-0.3.4/crankshaft/modules/utils.bolt
--rw-r--r--   0        0        0        0 2023-06-18 19:37:51.801795 crankshaft-0.3.4/crankshaft/py.typed
--rw-r--r--   0        0        0     1260 2023-06-18 19:39:33.886312 crankshaft-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     1106 1970-01-01 00:00:00.000000 crankshaft-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-03 00:07:47.096212 crankshaft-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1564 2023-07-03 00:07:47.096212 crankshaft-0.4.0/README.md
+-rw-r--r--   0        0        0      326 2023-07-03 00:09:05.263384 crankshaft-0.4.0/crankshaft/__init__.py
+-rw-r--r--   0        0        0      133 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/api.bolt
+-rw-r--r--   0        0        0      216 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/config.bolt
+-rw-r--r--   0        0        0      513 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/defer.bolt
+-rw-r--r--   0        0        0     3872 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/event_handler.bolt
+-rw-r--r--   0        0        0     1605 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/events/on_entity_attack_player.bolt
+-rw-r--r--   0        0        0      207 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/events/on_load.bolt
+-rw-r--r--   0        0        0      344 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/events/on_player_airborne.bolt
+-rw-r--r--   0        0        0      644 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/events/on_player_airborne_end.bolt
+-rw-r--r--   0        0        0      646 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/events/on_player_airborne_start.bolt
+-rw-r--r--   0        0        0     1605 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/events/on_player_attack_entity.bolt
+-rw-r--r--   0        0        0      328 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/events/on_player_burn.bolt
+-rw-r--r--   0        0        0      629 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/events/on_player_burn_end.bolt
+-rw-r--r--   0        0        0      632 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/events/on_player_burn_start.bolt
+-rw-r--r--   0        0        0      362 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/events/on_player_charge_bow.bolt
+-rw-r--r--   0        0        0      662 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/events/on_player_charge_bow_end.bolt
+-rw-r--r--   0        0        0      665 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/events/on_player_charge_bow_start.bolt
+-rw-r--r--   0        0        0      332 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/events/on_player_glide.bolt
+-rw-r--r--   0        0        0      632 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/events/on_player_glide_end.bolt
+-rw-r--r--   0        0        0      636 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/events/on_player_glide_start.bolt
+-rw-r--r--   0        0        0      677 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/events/on_player_inventory_change.bolt
+-rw-r--r--   0        0        0      501 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/events/on_player_join.bolt
+-rw-r--r--   0        0        0      495 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/events/on_player_jump.bolt
+-rw-r--r--   0        0        0      608 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/events/on_player_land.bolt
+-rw-r--r--   0        0        0      471 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/events/on_player_load.bolt
+-rw-r--r--   0        0        0      506 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/events/on_player_shoot_bow.bolt
+-rw-r--r--   0        0        0      335 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/events/on_player_sneak.bolt
+-rw-r--r--   0        0        0      635 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/events/on_player_sneak_end.bolt
+-rw-r--r--   0        0        0      638 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/events/on_player_sneak_start.bolt
+-rw-r--r--   0        0        0      341 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/events/on_player_sprint.bolt
+-rw-r--r--   0        0        0      642 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/events/on_player_sprint_end.bolt
+-rw-r--r--   0        0        0      644 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/events/on_player_sprint_start.bolt
+-rw-r--r--   0        0        0      332 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/events/on_player_swim.bolt
+-rw-r--r--   0        0        0      632 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/events/on_player_swim_end.bolt
+-rw-r--r--   0        0        0      635 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/events/on_player_swim_start.bolt
+-rw-r--r--   0        0        0      263 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/events/on_player_tick.bolt
+-rw-r--r--   0        0        0      558 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/events/on_player_use_coas.bolt
+-rw-r--r--   0        0        0      573 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/events/on_player_use_wfoas.bolt
+-rw-r--r--   0        0        0      207 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/events/on_tick.bolt
+-rw-r--r--   0        0        0     2118 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/events.bolt
+-rw-r--r--   0        0        0     3398 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/flag.bolt
+-rw-r--r--   0        0        0      377 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/flags/is_airborne.bolt
+-rw-r--r--   0        0        0      402 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/flags/is_baby.bolt
+-rw-r--r--   0        0        0      411 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/flags/is_burning.bolt
+-rw-r--r--   0        0        0     1258 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/flags/is_charging_bow.bolt
+-rw-r--r--   0        0        0      377 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/flags/is_gliding.bolt
+-rw-r--r--   0        0        0      379 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/flags/is_in_ground.bolt
+-rw-r--r--   0        0        0      379 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/flags/is_on_ground.bolt
+-rw-r--r--   0        0        0      158 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/flags/is_player.bolt
+-rw-r--r--   0        0        0      414 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/flags/is_sneaking.bolt
+-rw-r--r--   0        0        0      417 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/flags/is_sprinting.bolt
+-rw-r--r--   0        0        0      414 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/flags/is_swimming.bolt
+-rw-r--r--   0        0        0      535 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/flags.bolt
+-rw-r--r--   0        0        0      443 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/lib/entity_hit_matching/api.bolt
+-rw-r--r--   0        0        0      124 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/lib/entity_hit_matching/credits.txt
+-rw-r--r--   0        0        0    58171 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/lib/entity_hit_matching/main.bolt
+-rw-r--r--   0        0        0      207 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/modules/utils.bolt
+-rw-r--r--   0        0        0        0 2023-07-03 00:07:47.096212 crankshaft-0.4.0/crankshaft/py.typed
+-rw-r--r--   0        0        0     1329 2023-07-03 00:09:05.287385 crankshaft-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2373 1970-01-01 00:00:00.000000 crankshaft-0.4.0/PKG-INFO
```

### Comparing `crankshaft-0.3.4/LICENSE` & `crankshaft-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `crankshaft-0.3.4/crankshaft/modules/defer.bolt` & `crankshaft-0.4.0/crankshaft/modules/defer.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.3.4/crankshaft/modules/events/on_entity_attack_player.bolt` & `crankshaft-0.4.0/crankshaft/modules/events/on_entity_attack_player.bolt`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,51 @@
 from wicked_expressions:api import StaticVar, this
 from wicked_expressions:nbtlib import Bool
 from lightning_rod:api import tag, untag
-from ../event_handler import Event
-from ../config import Config
+from ../event_handler import BuiltinEvent
 from ../lib/entity_hit_matching/api import append_player_trigger
+from ../config import Config
 from ../utils import selector
 
 
 def handler(event):
     has_owner = StaticVar(Bool)
-    attacker_tag = f"{Config.TAG_ROOT}.event_handler.{event.event_id}.attacker"
-    child_tag = f"{Config.TAG_ROOT}.event_handler.{event.event_id}.child"
+    victim_tag = f"{Config.TAG_ROOT}.event.{event.id}.victim"
+    attacker_tag = f"{Config.TAG_ROOT}.event.{event.id}.attacker"
+    direct_tag = f"{Config.TAG_ROOT}.event.{event.id}.direct"
+    victim = selector(f"@a[tag={victim_tag}, limit=1]")
     attacker = selector(f"@e[tag={attacker_tag}, limit=1]")
-    child = selector(f"@e[tag={child_tag}, limit=1]")
+    direct = selector(f"@e[tag={direct_tag}, limit=1]")
     entrypoint = event.path('entrypoint')
 
     append_player_trigger(entrypoint)
     function entrypoint:
         as @e if score @s reapermc.crankshaft.lib.ehm.id = $direct reapermc.crankshaft.lib.ehm.id function event.path('nested_0'):
             with has_owner.store(mode='success'):
                 this.Owner.get()
 
             if has_owner == 1:
-                execute function event.path('nested_1'):
-                    tag(child_tag)
+                tag(direct_tag)
 
-                    on origin:
-                        tag(attacker_tag)
+                on origin:
+                    tag(attacker_tag)
             else:
                 tag(attacker_tag)
 
-        event.trigger(attacker, child)
+        tag(victim_tag)
+
+        as attacker:
+            event.trigger(victim, direct)
 
         # cleanup 
+        as victim:
+            untag(victim_tag)
+
         as attacker:
             untag(attacker_tag)
         
-        as child:
-            untag(child_tag)
+        as direct:
+            untag(direct_tag)
+
 
-on_entity_attack_player = Event(handler=handler, event_id='on_entity_attack_player')
+on_entity_attack_player = BuiltinEvent('on_entity_attack_player')
+on_entity_attack_player.attach_handler(handler)
```

### Comparing `crankshaft-0.3.4/crankshaft/modules/events/on_player_airborne_end.bolt` & `crankshaft-0.4.0/crankshaft/modules/events/on_player_sprint_start.bolt`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from lightning_rod:api import tag, untag
-from ../event_handler import Event, Listener
+from ../event_handler import BuiltinEvent, Entrypoint
 from ./on_player_tick import on_player_tick
 from ../config import Config
-from ../flags/is_airborne import is_airborne
+from ../flags/is_sprinting import is_sprinting
 
 
 def handler(event):
-    event_fired_tag = f"{Config.TAG_ROOT}.event_handler.{event.event_id}"
+    event_fired_tag = f"{Config.TAG_ROOT}.event.{event.id}"
 
-    @Listener(on_player_tick, bypass_fork=True)
-    def player_tick():
-        if not is_airborne:
-            if entity @s[tag=event_fired_tag] function event.path('nest_0'):
-                untag(event_fired_tag)
-                event.trigger()
-        else:
+    if is_sprinting:
+        if entity @s[tag=!event_fired_tag] function event.path('nested_0'):
             tag(event_fired_tag)
+            event.trigger()
+    else:
+        untag(event_fired_tag)
 
-on_player_airborne_end = Event(handler=handler, event_id='on_player_airborne_end')
+
+on_player_sprint_start = BuiltinEvent('on_player_sprint_start')
+on_player_sprint_start.attach_handler(handler, on_player_tick, Entrypoint.EVENT)
```

### Comparing `crankshaft-0.3.4/crankshaft/modules/events/on_player_airborne_start.bolt` & `crankshaft-0.4.0/crankshaft/modules/events/on_player_swim_end.bolt`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from lightning_rod:api import tag, untag
-from ../event_handler import Event, Listener
+from ../event_handler import BuiltinEvent, Entrypoint
 from ./on_player_tick import on_player_tick
 from ../config import Config
-from ../flags/is_airborne import is_airborne
+from ../flags/is_swimming import is_swimming
 
 
 def handler(event):
-    event_fired_tag = f"{Config.TAG_ROOT}.event_handler.{event.event_id}"
+    event_fired_tag = f"{Config.TAG_ROOT}.event.{event.id}"
 
-    @Listener(on_player_tick, bypass_fork=True)
-    def player_tick():
-        if is_airborne:
-            if entity @s[tag=!event_fired_tag] function event.path('nest_0'):
-                tag(event_fired_tag)
-                event.trigger()
-        else:
+    if not is_swimming:
+        if entity @s[tag=event_fired_tag] function event.path('nested_0'):
             untag(event_fired_tag)
+            event.trigger()
+    else:
+        tag(event_fired_tag)
 
-on_player_airborne_start = Event(handler=handler, event_id='on_player_airborne_start')
+
+on_player_swim_end = BuiltinEvent('on_player_swim_end')
+on_player_swim_end.attach_handler(handler, on_player_tick, Entrypoint.EVENT)
```

### Comparing `crankshaft-0.3.4/crankshaft/modules/events/on_player_attack_entity.bolt` & `crankshaft-0.4.0/crankshaft/modules/events/on_player_attack_entity.bolt`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,51 @@
 from wicked_expressions:api import StaticVar, this
 from wicked_expressions:nbtlib import Bool
 from lightning_rod:api import tag, untag
-from ../event_handler import Event
+from ../event_handler import BuiltinEvent
 from ../lib/entity_hit_matching/api import append_target_trigger
-from ../utils import selector
 from ../config import Config
+from ../utils import selector
 
 
 def handler(event):
     has_owner = StaticVar(Bool)
-    attacker_tag = f"{Config.TAG_ROOT}.event_handler.{event.event_id}.attacker"
-    child_tag = f"{Config.TAG_ROOT}.event_handler.{event.event_id}.child"
+    victim_tag = f"{Config.TAG_ROOT}.event.{event.id}.victim"
+    attacker_tag = f"{Config.TAG_ROOT}.event.{event.id}.attacker"
+    direct_tag = f"{Config.TAG_ROOT}.event.{event.id}.direct"
+    victim = selector(f"@e[tag={victim_tag}, limit=1]")
     attacker = selector(f"@a[tag={attacker_tag}, limit=1]")
-    child = selector(f"@e[tag={child_tag}, limit=1]")
+    direct = selector(f"@e[tag={direct_tag}, limit=1]")
     entrypoint = event.path('entrypoint')
 
     append_target_trigger(entrypoint)
     function entrypoint:
         as @e if score @s reapermc.crankshaft.lib.ehm.id = $direct reapermc.crankshaft.lib.ehm.id function event.path('nested_0'):
             with has_owner.store(mode='success'):
                 this.Owner.get()
 
             if has_owner == 1:
-                execute function event.path('nested_1'):
-                    tag(child_tag)
+                tag(direct_tag)
 
-                    on origin:
-                        tag(attacker_tag)
+                on origin:
+                    tag(attacker_tag)
             else:
                 tag(attacker_tag)
 
-        event.trigger(attacker, child)
+        tag(victim_tag)
+
+        as attacker:
+            event.trigger(victim, direct)
 
         # cleanup 
+        as victim:
+            untag(victim_tag)
+
         as attacker:
             untag(attacker_tag)
         
-        as child:
-            untag(child_tag)
+        as direct:
+            untag(direct_tag)
+
 
-on_player_attack_entity = Event(handler=handler, event_id='on_player_attack_entity')
+on_player_attack_entity = BuiltinEvent('on_player_attack_entity')
+on_player_attack_entity.attach_handler(handler)
```

### Comparing `crankshaft-0.3.4/crankshaft/modules/events/on_player_burn_end.bolt` & `crankshaft-0.4.0/crankshaft/modules/events/on_player_sneak_start.bolt`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from lightning_rod:api import tag, untag
-from ../event_handler import Event, Listener
+from ../event_handler import BuiltinEvent, Entrypoint
 from ./on_player_tick import on_player_tick
 from ../config import Config
-from ../flags/is_burning import is_burning
+from ../flags/is_sneaking import is_sneaking
 
 
 def handler(event):
-    event_fired_tag = f"{Config.TAG_ROOT}.event_handler.{event.event_id}"
+    event_fired_tag = f"{Config.TAG_ROOT}.event.{event.id}"
 
-    @Listener(on_player_tick, bypass_fork=True)
-    def player_tick():
-        if not is_burning:
-            if entity @s[tag=event_fired_tag] function event.path('nest_0'):
-                untag(event_fired_tag)
-                event.trigger()
-        else:
+    if is_sneaking:
+        if entity @s[tag=!event_fired_tag] function event.path('nested_0'):
             tag(event_fired_tag)
+            event.trigger()
+    else:
+        untag(event_fired_tag)
 
-on_player_burn_end = Event(handler=handler, event_id='on_player_burn_end')
+
+on_player_sneak_start = BuiltinEvent('on_player_sneak_start')
+on_player_sneak_start.attach_handler(handler, on_player_tick, Entrypoint.EVENT)
```

### Comparing `crankshaft-0.3.4/crankshaft/modules/events/on_player_burn_start.bolt` & `crankshaft-0.4.0/crankshaft/modules/events/on_player_burn_start.bolt`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from lightning_rod:api import tag, untag
-from ../event_handler import Event, Listener
+from ../event_handler import BuiltinEvent, Entrypoint
 from ./on_player_tick import on_player_tick
 from ../config import Config
 from ../flags/is_burning import is_burning
 
 
 def handler(event):
-    event_fired_tag = f"{Config.TAG_ROOT}.event_handler.{event.event_id}"
+    event_fired_tag = f"{Config.TAG_ROOT}.event.{event.id}"
 
-    @Listener(on_player_tick, bypass_fork=True)
-    def player_tick():
-        if is_burning:
-            if entity @s[tag=!event_fired_tag] function event.path('nest_0'):
-                tag(event_fired_tag)
-                event.trigger()
-        else:
-            untag(event_fired_tag)
+    if is_burning:
+        if entity @s[tag=!event_fired_tag] function event.path('nested_0'):
+            tag(event_fired_tag)
+            event.trigger()
+    else:
+        untag(event_fired_tag)
 
-on_player_burn_start = Event(handler=handler, event_id='on_player_burn_start')
+
+on_player_burn_start = BuiltinEvent('on_player_burn_start')
+on_player_burn_start.attach_handler(handler, on_player_tick, Entrypoint.EVENT)
```

### Comparing `crankshaft-0.3.4/crankshaft/modules/events/on_player_charge_bow_end.bolt` & `crankshaft-0.4.0/crankshaft/modules/events/on_player_swim_start.bolt`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,19 @@
-from wicked_expressions:api import Scoreboard
 from lightning_rod:api import tag, untag
-from ../event_handler import Event, Listener
-from ../config import Config
-from ../flags/is_charging_bow import is_charging_bow
-from ./on_player_charge_bow import on_player_charge_bow
+from ../event_handler import BuiltinEvent, Entrypoint
 from ./on_player_tick import on_player_tick
+from ../config import Config
+from ../flags/is_swimming import is_swimming 
 
 
 def handler(event):
-    event_fired_tag = f"{Config.TAG_ROOT}.event_handler.{event.event_id}"
+    event_fired_tag = f"{Config.TAG_ROOT}.event.{event.id}"
 
-    @Listener(on_player_tick, bypass_fork=True)
-    def player_tick():
-        if not is_charging_bow:
-            if entity @s[tag=event_fired_tag] function event.path('nest_0'):
-                untag(event_fired_tag)
-                event.trigger()
-        else:
+    if is_swimming:
+        if entity @s[tag=!event_fired_tag] function event.path('nested_0'):
             tag(event_fired_tag)
+            event.trigger()
+    else:
+        untag(event_fired_tag)
 
-on_player_charge_bow_end = Event(handler=handler, event_id='on_player_charge_bow_end')
+on_player_swim_start = BuiltinEvent('on_player_swim_start')
+on_player_swim_start.attach_handler(handler, on_player_tick, Entrypoint.EVENT)
```

### Comparing `crankshaft-0.3.4/crankshaft/modules/events/on_player_join.bolt` & `crankshaft-0.4.0/crankshaft/modules/events/on_player_land.bolt`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,20 @@
-from wicked_expressions:api import Scoreboard
-from ../event_handler import Event, Listener
-from ../config import Config
+from lightning_rod:api import tag, untag
+from ../event_handler import BuiltinEvent, Entrypoint
 from ./on_player_tick import on_player_tick
+from ../config import Config
+from ../flags/is_airborne import is_airborne
 
 
 def handler(event):
-    @Listener(on_player_tick, bypass_fork=True)
-    def player_tick():
-        join_tracker = Scoreboard(f"{Config.SCOREBOARD_ROOT}.{event.event_id}", 'custom:leave_game')['@s']
+    available_tag = f"{Config.TAG_ROOT}.event.{event.id}"
+
+    if is_airborne:
+        tag(available_tag)
+    else:
+        if entity @s[tag=available_tag] function event.path('nested_0'):
+            untag(available_tag)
+            event.trigger()
 
-        if join_tracker >= 1:
-            execute function event.path('main'):
-                join_tracker = 0
-                event.trigger()
 
-on_player_join = Event(handler=handler, event_id='on_player_join')
+on_player_land = BuiltinEvent('on_player_land')
+on_player_land.attach_handler(handler, on_player_tick, Entrypoint.EVENT)
```

### Comparing `crankshaft-0.3.4/crankshaft/modules/events/on_player_land.bolt` & `crankshaft-0.4.0/crankshaft/modules/events/on_player_glide_start.bolt`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from lightning_rod:api import tag, untag
-from ../event_handler import Event, Listener
+from ../event_handler import BuiltinEvent, Entrypoint
 from ./on_player_tick import on_player_tick
 from ../config import Config
-from ../flags/is_airborne import is_airborne
+from ../flags/is_gliding import is_gliding 
 
 
 def handler(event):
-    @Listener(on_player_tick, bypass_fork=True)
-    def player_tick():
-        available_tag = f"{Config.TAG_ROOT}.event_handler.{event.event_id}"
+    event_fired_tag = f"{Config.TAG_ROOT}.event.{event.id}"
 
-        if is_airborne:
-            tag(available_tag)
-        else:
-            if entity @s[tag=available_tag]:
-                execute function event.path('main'):
-                    untag(available_tag)
-                    event.trigger()
+    if is_gliding:
+        if entity @s[tag=!event_fired_tag] function event.path('nested_0'):
+            tag(event_fired_tag)
+            event.trigger()
+    else:
+        untag(event_fired_tag)
 
-on_player_land = Event(handler=handler, event_id='on_player_land')
+
+on_player_glide_start = BuiltinEvent('on_player_glide_start')
+on_player_glide_start.attach_handler(handler, on_player_tick, Entrypoint.EVENT)
```

### Comparing `crankshaft-0.3.4/crankshaft/modules/events/on_player_sneak_start.bolt` & `crankshaft-0.4.0/crankshaft/modules/events/on_player_airborne_start.bolt`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from lightning_rod:api import tag, untag
-from ../event_handler import Event, Listener
+from ../event_handler import BuiltinEvent, Entrypoint
 from ./on_player_tick import on_player_tick
 from ../config import Config
-from ../flags/is_sneaking import is_sneaking 
+from ../flags/is_airborne import is_airborne
 
 
 def handler(event):
-    event_fired_tag = f"{Config.TAG_ROOT}.event_handler.{event.event_id}"
+    event_fired_tag = f"{Config.TAG_ROOT}.event.{event.id}"
 
-    @Listener(on_player_tick, bypass_fork=True)
-    def player_tick():
-        if is_sneaking:
-            if entity @s[tag=!event_fired_tag] function event.path('nest_0'):
-                tag(event_fired_tag)
-                event.trigger()
-        else:
-            untag(event_fired_tag)
+    if is_airborne:
+        if entity @s[tag=!event_fired_tag] function event.path('nested_0'):
+            tag(event_fired_tag)
+            event.trigger()
+    else:
+        untag(event_fired_tag)
 
-on_player_sneak_start = Event(handler=handler, event_id='on_player_sneak_start')
+
+on_player_airborne_start = BuiltinEvent('on_player_airborne_start')
+on_player_airborne_start.attach_handler(handler, on_player_tick, Entrypoint.EVENT)
```

### Comparing `crankshaft-0.3.4/crankshaft/modules/events/on_player_sprint_end.bolt` & `crankshaft-0.4.0/crankshaft/modules/events/on_player_charge_bow_end.bolt`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from lightning_rod:api import tag, untag
-from ../event_handler import Event, Listener
-from ./on_player_tick import on_player_tick
+from ../event_handler import BuiltinEvent, Entrypoint
 from ../config import Config
-from ../flags/is_sprinting import is_sprinting 
+from ../flags/is_charging_bow import is_charging_bow
+from ./on_player_tick import on_player_tick
 
 
 def handler(event):
-    event_fired_tag = f"{Config.TAG_ROOT}.event_handler.{event.event_id}"
+    event_fired_tag = f"{Config.TAG_ROOT}.event.{event.id}"
+
+    if not is_charging_bow:
+        if entity @s[tag=event_fired_tag] function event.path('nested_0'):
+            untag(event_fired_tag)
+            event.trigger()
+    else:
+        tag(event_fired_tag)
 
-    @Listener(on_player_tick, bypass_fork=True)
-    def player_tick():
-        if not is_sprinting:
-            if entity @s[tag=event_fired_tag] function event.path('nest_0'):
-                untag(event_fired_tag)
-                event.trigger()
-        else:
-            tag(event_fired_tag)
 
-on_player_sprint_end = Event(handler=handler, event_id='on_player_sprint_end')
+on_player_charge_bow_end = BuiltinEvent('on_player_charge_bow_end')
+on_player_charge_bow_end.attach_handler(handler, on_player_tick, Entrypoint.EVENT)
```

### Comparing `crankshaft-0.3.4/crankshaft/modules/events/on_player_sprint_start.bolt` & `crankshaft-0.4.0/crankshaft/modules/events/on_player_charge_bow_start.bolt`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from lightning_rod:api import tag, untag
-from ../event_handler import Event, Listener
-from ./on_player_tick import on_player_tick
+from ../event_handler import BuiltinEvent, Entrypoint
 from ../config import Config
-from ../flags/is_sprinting import is_sprinting 
+from ../flags/is_charging_bow import is_charging_bow
+from ./on_player_tick import on_player_tick
 
 
 def handler(event):
-    event_fired_tag = f"{Config.TAG_ROOT}.event_handler.{event.event_id}"
+    event_fired_tag = f"{Config.TAG_ROOT}.event.{event.id}"
+
+    if is_charging_bow:
+        if entity @s[tag=!event_fired_tag] function event.path('nested_0'):
+            tag(event_fired_tag)
+            event.trigger()
+    else:
+        untag(event_fired_tag)
 
-    @Listener(on_player_tick, bypass_fork=True)
-    def player_tick():
-        if is_sprinting:
-            if entity @s[tag=!event_fired_tag] function event.path('nest_0'):
-                tag(event_fired_tag)
-                event.trigger()
-        else:
-            untag(event_fired_tag)
 
-on_player_sprint_start = Event(handler=handler, event_id='on_player_sprint_start')
+on_player_charge_bow_start = BuiltinEvent('on_player_charge_bow_start')
+on_player_charge_bow_start.attach_handler(handler, on_player_tick, Entrypoint.EVENT)
```

### Comparing `crankshaft-0.3.4/crankshaft/modules/events/on_player_use_coas.bolt` & `crankshaft-0.4.0/crankshaft/modules/events/on_player_use_coas.bolt`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from wicked_expressions:api import Scoreboard
-from ../event_handler import Event, Listener
+from ../event_handler import BuiltinEvent, Entrypoint
 from ./on_player_tick import on_player_tick
 from ../config import Config
 
 
 def handler(event):
-    @Listener(on_player_tick, bypass_fork=True)
-    def player_tick():
-        used_coas = Scoreboard(f"{Config.SCOREBOARD_ROOT}.event_handler.{event.event_id}", 'used:carrot_on_a_stick')['@s']
-
-        if used_coas > 0:
-            used_coas = 0
-            event.trigger()
+    used_coas = Scoreboard(f"{Config.SCOREBOARD_ROOT}.event.{event.id}", 'used:carrot_on_a_stick')['@s']
 
-on_player_use_coas = Event(handler=handler, event_id='on_player_use_coas')
+    if not used_coas.exists():
+        used_coas = 0
+
+    if used_coas > 0:
+        used_coas = 0
+        event.trigger()
+
+
+on_player_use_coas = BuiltinEvent('on_player_use_coas')
+on_player_use_coas.attach_handler(handler, on_player_tick, Entrypoint.EVENT)
```

### Comparing `crankshaft-0.3.4/crankshaft/modules/events.bolt` & `crankshaft-0.4.0/crankshaft/modules/events.bolt`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,37 @@
-"""Module from which builtin events are imported."""
+"""Module from which builtin events are imported. Import order dictates event execution order."""
 
-# general
 from ./events/on_load import on_load
 from ./events/on_tick import on_tick
-
+from ./events/on_player_load import on_player_load
 from ./events/on_player_tick import on_player_tick
 from ./events/on_player_join import on_player_join
-from ./events/on_player_load import on_player_load
-
-# movement
 from ./events/on_player_jump import on_player_jump
 from ./events/on_player_land import on_player_land
-
 from ./events/on_player_sneak_start import on_player_sneak_start
 from ./events/on_player_sneak import on_player_sneak
 from ./events/on_player_sneak_end import on_player_sneak_end
-
 from ./events/on_player_sprint_start import on_player_sprint_start
 from ./events/on_player_sprint import on_player_sprint
 from ./events/on_player_sprint_end import on_player_sprint_end
-
 from ./events/on_player_glide_start import on_player_glide_start
 from ./events/on_player_glide import on_player_glide
 from ./events/on_player_glide_end import on_player_glide_end
-
 from ./events/on_player_swim_start import on_player_swim_start
 from ./events/on_player_swim import on_player_swim
 from ./events/on_player_swim_end import on_player_swim_end
-
 from ./events/on_player_burn_start import on_player_burn_start
 from ./events/on_player_burn import on_player_burn
 from ./events/on_player_burn_end import on_player_burn_end
-
 from ./events/on_player_airborne_start import on_player_airborne_start
 from ./events/on_player_airborne import on_player_airborne
 from ./events/on_player_airborne_end import on_player_airborne_end
-
-# used item
-from ./events/on_player_shoot_bow import on_player_shoot_bow
+from ./events/on_player_use_coas import on_player_use_coas
+from ./events/on_player_use_wfoas import on_player_use_wfoas
 from ./events/on_player_charge_bow_start import on_player_charge_bow_start
 from ./events/on_player_charge_bow import on_player_charge_bow
 from ./events/on_player_charge_bow_end import on_player_charge_bow_end
-
-# misc
+from ./events/on_player_shoot_bow import on_player_shoot_bow
 from ./events/on_player_inventory_change import on_player_inventory_change
 from ./events/on_player_attack_entity import on_player_attack_entity
 from ./events/on_entity_attack_player import on_entity_attack_player
-from ./events/on_player_use_coas import on_player_use_coas
+
```

### Comparing `crankshaft-0.3.4/crankshaft/modules/flag.bolt` & `crankshaft-0.4.0/crankshaft/modules/flag.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.3.4/crankshaft/modules/flags/is_charging_bow.bolt` & `crankshaft-0.4.0/crankshaft/modules/flags/is_charging_bow.bolt`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from wicked_expressions:api import Scoreboard 
 from lightning_rod:api import revoke_advancement
-from ../event_handler import Listener
 from ../flag import Flag
 from ../config import Config
-from ../events/on_player_tick import on_player_tick
 
 
 def body(flag):
     is_charging = Scoreboard(f"{Config.SCOREBOARD_ROOT}.flag.{flag.flag_id}")['@s']
     advancement_path = flag.path('advancement')
     reward_path = flag.path('advancement_reward')
+    p_tick_path = flag.path('p_tick')
 
-    @Listener(on_player_tick, bypass_fork=True)
-    def player_tick():
-        nonlocal is_charging
-
-        is_charging -= 1
+    merge function_tag minecraft:tick {"replace": false, "values": [p_tick_path]}
+    function p_tick_path:
+        as @a:
+            if is_charging > 0:
+                is_charging -= 1
 
     advancement advancement_path {
         "criteria": {
             "requirement": {
                 "trigger": "minecraft:using_item",
                 "conditions": {
                     "item": {
@@ -33,14 +32,14 @@
         "rewards": {
             "function": reward_path
         }
     }
 
     function reward_path:
         revoke_advancement(advancement_path)
-        is_charging = 2
+        is_charging = 1
     
     with flag.set_condition():
         if score var is_charging matches 1
 
 
 is_charging_bow = Flag(body=body, flag_id='is_charging_bow')
```

### Comparing `crankshaft-0.3.4/crankshaft/modules/flags.bolt` & `crankshaft-0.4.0/crankshaft/modules/flags.bolt`

 * *Files identical despite different names*

### Comparing `crankshaft-0.3.4/crankshaft/modules/lib/entity_hit_matching/main.bolt` & `crankshaft-0.4.0/crankshaft/modules/lib/entity_hit_matching/main.bolt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 from wicked_expressions:api import this
-from ../../event_handler import Listener
-from ../../events/on_tick import on_tick
-from ../../events/on_load import on_load
 from ../../config import Config
 
 ROOT_DIR = f"{Config.ROOT}/lib/entity_hit_matching"
 ROOT_GENERIC = f"{Config.SCOREBOARD_ROOT}.lib.ehm"
 
 TARGET_HURT_PLAYER = f"{ROOT_DIR}/player_is_hurt_by_target"
 PLAYER_HURT_TARGET = f"{ROOT_DIR}/target_is_hurt_by_player"
@@ -40,38 +37,36 @@
         "minecraft:chest_minecart",
         "minecraft:chest_boat",
         "minecraft:marker"
     ]
 }
 
 
-@Listener(on_load, bypass_fork=True)
-def load():
-	execute function f"{ROOT_DIR}/load":
-		# This objective tracks IDs, along with variables and constants
-		scoreboard objectives add f"{ROOT_GENERIC}.id" dummy
-		scoreboard players set #3 f"{ROOT_GENERIC}.id" 3
-
-		# These objectives track the individual bits of IDs
-		scoreboard objectives add f"{ROOT_GENERIC}.id.0" dummy
-		scoreboard objectives add f"{ROOT_GENERIC}.id.1" dummy
-		scoreboard objectives add f"{ROOT_GENERIC}.id.2" dummy
-		scoreboard objectives add f"{ROOT_GENERIC}.id.3" dummy
-		scoreboard objectives add f"{ROOT_GENERIC}.id.4" dummy
-		scoreboard objectives add f"{ROOT_GENERIC}.id.5" dummy
-		scoreboard objectives add f"{ROOT_GENERIC}.id.6" dummy
-		scoreboard objectives add f"{ROOT_GENERIC}.id.7" dummy
-		scoreboard objectives add f"{ROOT_GENERIC}.id.8" dummy
+merge function_tag minecraft:load {"replace": false, "values": [f"{ROOT_DIR}/load"]} 
+function f"{ROOT_DIR}/load":
+    # This objective tracks IDs, along with variables and constants
+    scoreboard objectives add f"{ROOT_GENERIC}.id" dummy
+    scoreboard players set #3 f"{ROOT_GENERIC}.id" 3
+
+    # These objectives track the individual bits of IDs
+    scoreboard objectives add f"{ROOT_GENERIC}.id.0" dummy
+    scoreboard objectives add f"{ROOT_GENERIC}.id.1" dummy
+    scoreboard objectives add f"{ROOT_GENERIC}.id.2" dummy
+    scoreboard objectives add f"{ROOT_GENERIC}.id.3" dummy
+    scoreboard objectives add f"{ROOT_GENERIC}.id.4" dummy
+    scoreboard objectives add f"{ROOT_GENERIC}.id.5" dummy
+    scoreboard objectives add f"{ROOT_GENERIC}.id.6" dummy
+    scoreboard objectives add f"{ROOT_GENERIC}.id.7" dummy
+    scoreboard objectives add f"{ROOT_GENERIC}.id.8" dummy
 #
 
-@Listener(on_tick, bypass_fork=True)
-def tick():
-	execute function f"{ROOT_DIR}/tick":
-		# Assigns IDs to the entities that need them
-		execute as @e unless score @s f"{ROOT_GENERIC}.id" = @s f"{ROOT_GENERIC}.id" run function f"{ROOT_DIR}/id/filter"
+merge function_tag minecraft:tick {"replace": false, "values": [f"{ROOT_DIR}/tick"]} 
+function f"{ROOT_DIR}/tick":
+    # Assigns IDs to the entities that need them
+    execute as @e unless score @s f"{ROOT_GENERIC}.id" = @s f"{ROOT_GENERIC}.id" run function f"{ROOT_DIR}/id/filter"
 #
 
 function f"{ROOT_DIR}/id/assign":
     # Removes existing ID-related function tags from the executor
     function f"{ROOT_DIR}/id/remove_tags"
 
     # Assigns a new ID to the executor
```

### Comparing `crankshaft-0.3.4/pyproject.toml` & `crankshaft-0.4.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 [tool.poetry]
 name = "crankshaft"
-version = "0.3.4"
-description = "Flow control library for the Bolt scripting language."
+version = "0.4.0"
+description = "Bolt datapack flow control library."
 authors = ["ArcticYeti <arcticyeti1@gmail.com>"]
 license = "MIT"
 
 homepage = "https://github.com/reapermc/crankshaft"
 readme = "README.md"
 
 keywords = [
   "beet",
+  "mecha",
   "bolt",
+  "python",
   "minecraft",
   "datapack",
   "minecraft-commands",
   "mcfunction",
+  "crankshaft",
   "library",
   "reapermc",
+  "flow-control",
+  "event",
+  "event-handler",
 ]
 
 include = ["crankshaft/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 beet = ">=0.84.0"
```

