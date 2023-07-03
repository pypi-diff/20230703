# Comparing `tmp/honeybot-6.0.2.tar.gz` & `tmp/honeybot-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "honeybot-6.0.2.tar", last modified: Wed Nov 30 11:35:45 2022, max compression
+gzip compressed data, was "honeybot-6.1.0.tar", last modified: Mon Jul  3 13:00:17 2023, max compression
```

## Comparing `honeybot-6.0.2.tar` & `honeybot-6.1.0.tar`

### file list

```diff
@@ -1,328 +1,345 @@
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.503261 honeybot-6.0.2/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1081 2022-07-24 16:55:48.000000 honeybot-6.0.2/LICENSE
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    26501 2022-11-30 11:35:45.503261 honeybot-6.0.2/PKG-INFO
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    25435 2022-11-30 10:25:54.000000 honeybot-6.0.2/README.md
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      559 2022-11-30 10:25:54.000000 honeybot-6.0.2/pyproject.toml
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      354 2022-11-30 11:35:45.503261 honeybot-6.0.2/setup.cfg
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2228 2022-11-30 11:33:23.000000 honeybot-6.0.2/setup.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.375260 honeybot-6.0.2/src/
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.387261 honeybot-6.0.2/src/honeybot/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)       22 2022-11-30 11:33:49.000000 honeybot-6.0.2/src/honeybot/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)       33 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/__main__.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.391261 honeybot-6.0.2/src/honeybot/api/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/api/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      453 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/api/commands.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)       91 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/api/generate.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      469 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/api/init.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     8884 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/api/main.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      680 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/api/memory.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      897 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/api/print.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      512 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/api/utils.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     3307 2022-11-30 10:26:03.000000 honeybot-6.0.2/src/honeybot/gui_manager.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      118 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/lab.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1269 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/manage.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.391261 honeybot-6.0.2/src/honeybot/plugins/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/__init__.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.391261 honeybot-6.0.2/src/honeybot/plugins/core/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/core/__init__.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.391261 honeybot-6.0.2/src/honeybot/plugins/core/joins/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/core/joins/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      923 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/core/joins/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.391261 honeybot-6.0.2/src/honeybot/plugins/core/log/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/core/log/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1387 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/core/log/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.391261 honeybot-6.0.2/src/honeybot/plugins/core/uptime/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/core/uptime/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1066 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/core/uptime/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.391261 honeybot-6.0.2/src/honeybot/plugins/downloaded/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/__init__.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.391261 honeybot-6.0.2/src/honeybot/plugins/downloaded/abbreviation/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/abbreviation/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      178 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/abbreviation/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2601 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/abbreviation/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.391261 honeybot-6.0.2/src/honeybot/plugins/downloaded/age/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/age/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      196 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/age/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1406 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/age/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.391261 honeybot-6.0.2/src/honeybot/plugins/downloaded/bitcoin/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/bitcoin/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      297 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/bitcoin/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      962 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/bitcoin/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.395261 honeybot-6.0.2/src/honeybot/plugins/downloaded/blackjack/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/blackjack/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      310 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/blackjack/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     7927 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/blackjack/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.395261 honeybot-6.0.2/src/honeybot/plugins/downloaded/blackjack/poker_assets/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/blackjack/poker_assets/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2809 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/blackjack/poker_assets/best5.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1192 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/blackjack/poker_assets/board.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1667 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/blackjack/poker_assets/card.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2464 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/blackjack/poker_assets/deck.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1429 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/blackjack/poker_assets/game_init.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2303 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/blackjack/poker_assets/hand.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2500 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/blackjack/poker_assets/player.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      371 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/blackjack/poker_assets/pot.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     3064 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/blackjack/poker_assets/test.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.395261 honeybot-6.0.2/src/honeybot/plugins/downloaded/book_of_day/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/book_of_day/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      272 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/book_of_day/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      948 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/book_of_day/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.395261 honeybot-6.0.2/src/honeybot/plugins/downloaded/caesar_cipher/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/caesar_cipher/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      225 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/caesar_cipher/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      835 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/caesar_cipher/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.399261 honeybot-6.0.2/src/honeybot/plugins/downloaded/calc/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/calc/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      252 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/calc/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1815 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/calc/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.399261 honeybot-6.0.2/src/honeybot/plugins/downloaded/channeljoin/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/channeljoin/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      215 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/channeljoin/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1241 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/channeljoin/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.399261 honeybot-6.0.2/src/honeybot/plugins/downloaded/cointoss/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/cointoss/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      191 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/cointoss/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      677 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/cointoss/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.399261 honeybot-6.0.2/src/honeybot/plugins/downloaded/comic/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/comic/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      184 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/comic/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      839 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/comic/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.399261 honeybot-6.0.2/src/honeybot/plugins/downloaded/conv_sniff/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/conv_sniff/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      235 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/conv_sniff/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2713 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/conv_sniff/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.399261 honeybot-6.0.2/src/honeybot/plugins/downloaded/converter/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/converter/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      325 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/converter/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     4412 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/converter/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.399261 honeybot-6.0.2/src/honeybot/plugins/downloaded/corona/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/corona/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      286 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/corona/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     5735 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/corona/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.403261 honeybot-6.0.2/src/honeybot/plugins/downloaded/country/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/country/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      197 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/country/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    10451 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/country/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.403261 honeybot-6.0.2/src/honeybot/plugins/downloaded/dadjoke/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/dadjoke/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      256 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/dadjoke/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      836 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/dadjoke/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.403261 honeybot-6.0.2/src/honeybot/plugins/downloaded/date/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/date/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      205 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/date/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      851 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/date/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.403261 honeybot-6.0.2/src/honeybot/plugins/downloaded/debug/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/debug/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      207 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/debug/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      603 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/debug/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.403261 honeybot-6.0.2/src/honeybot/plugins/downloaded/diary/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/diary/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      402 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/diary/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     5421 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/diary/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.403261 honeybot-6.0.2/src/honeybot/plugins/downloaded/dictionary/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/dictionary/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      300 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/dictionary/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      879 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/dictionary/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.403261 honeybot-6.0.2/src/honeybot/plugins/downloaded/duckduckgo/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/duckduckgo/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      247 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/duckduckgo/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      941 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/duckduckgo/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.407261 honeybot-6.0.2/src/honeybot/plugins/downloaded/excuse/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/excuse/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      169 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/excuse/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      699 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/excuse/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.407261 honeybot-6.0.2/src/honeybot/plugins/downloaded/fact/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/fact/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      245 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/fact/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     8742 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/fact/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.407261 honeybot-6.0.2/src/honeybot/plugins/downloaded/google/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/google/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      214 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/google/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1361 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/google/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.407261 honeybot-6.0.2/src/honeybot/plugins/downloaded/greet/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/greet/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      197 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/greet/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      578 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/greet/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.407261 honeybot-6.0.2/src/honeybot/plugins/downloaded/hangman/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/hangman/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      287 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/hangman/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     7409 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/hangman/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.411261 honeybot-6.0.2/src/honeybot/plugins/downloaded/help/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/help/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      242 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/help/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      796 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/help/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.411261 honeybot-6.0.2/src/honeybot/plugins/downloaded/horoscope/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/horoscope/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      413 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/horoscope/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     8499 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/horoscope/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.471261 honeybot-6.0.2/src/honeybot/plugins/downloaded/installed_modules/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/installed_modules/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      214 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/installed_modules/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1160 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/installed_modules/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.471261 honeybot-6.0.2/src/honeybot/plugins/downloaded/joke/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/joke/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      199 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/joke/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     4503 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/joke/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.471261 honeybot-6.0.2/src/honeybot/plugins/downloaded/magic_ball/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/magic_ball/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      261 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/magic_ball/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1652 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/magic_ball/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.471261 honeybot-6.0.2/src/honeybot/plugins/downloaded/mail/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/mail/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      759 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/mail/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     4862 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/mail/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.471261 honeybot-6.0.2/src/honeybot/plugins/downloaded/maths/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/maths/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      369 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/maths/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2618 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/maths/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.471261 honeybot-6.0.2/src/honeybot/plugins/downloaded/memo/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/memo/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      255 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/memo/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1169 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/memo/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.475261 honeybot-6.0.2/src/honeybot/plugins/downloaded/monero/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/monero/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      341 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/monero/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1332 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/monero/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.475261 honeybot-6.0.2/src/honeybot/plugins/downloaded/monopoly/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/monopoly/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      939 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/monopoly/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    60781 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/monopoly/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.475261 honeybot-6.0.2/src/honeybot/plugins/downloaded/monopoly/monopoly_assets/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/monopoly/monopoly_assets/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     8387 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/monopoly/monopoly_assets/monopoly_assets.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1458 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/monopoly/monopoly_assets/monopoly_player.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.475261 honeybot-6.0.2/src/honeybot/plugins/downloaded/news/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/news/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      237 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/news/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1255 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/news/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.475261 honeybot-6.0.2/src/honeybot/plugins/downloaded/onthisday/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/onthisday/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      191 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/onthisday/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1478 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/onthisday/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.475261 honeybot-6.0.2/src/honeybot/plugins/downloaded/password_generator/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/password_generator/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      561 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/password_generator/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     4811 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/password_generator/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.479261 honeybot-6.0.2/src/honeybot/plugins/downloaded/proverb/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/proverb/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      180 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/proverb/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1870 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/proverb/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.479261 honeybot-6.0.2/src/honeybot/plugins/downloaded/pydocs/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/pydocs/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      298 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/pydocs/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      877 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/pydocs/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.479261 honeybot-6.0.2/src/honeybot/plugins/downloaded/pynews/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/pynews/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      229 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/pynews/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1282 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/pynews/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.479261 honeybot-6.0.2/src/honeybot/plugins/downloaded/pypi/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/pypi/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      197 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/pypi/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1438 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/pypi/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.479261 honeybot-6.0.2/src/honeybot/plugins/downloaded/quote/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/quote/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      172 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/quote/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     4903 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/quote/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.479261 honeybot-6.0.2/src/honeybot/plugins/downloaded/random_color/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/random_color/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      236 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/random_color/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      976 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/random_color/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.483261 honeybot-6.0.2/src/honeybot/plugins/downloaded/random_image/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/random_image/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      171 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/random_image/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      743 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/random_image/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.483261 honeybot-6.0.2/src/honeybot/plugins/downloaded/repostats/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/repostats/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      228 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/repostats/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1452 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/repostats/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.483261 honeybot-6.0.2/src/honeybot/plugins/downloaded/riddle/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/riddle/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      285 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/riddle/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     3845 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/riddle/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.483261 honeybot-6.0.2/src/honeybot/plugins/downloaded/roll/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/roll/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      201 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/roll/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1775 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/roll/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.491261 honeybot-6.0.2/src/honeybot/plugins/downloaded/roman_numeral/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/roman_numeral/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      250 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/roman_numeral/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2701 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/roman_numeral/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.491261 honeybot-6.0.2/src/honeybot/plugins/downloaded/russian_roulette/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/russian_roulette/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      514 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/russian_roulette/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1494 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/russian_roulette/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.491261 honeybot-6.0.2/src/honeybot/plugins/downloaded/selfTrivia/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/selfTrivia/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      249 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/selfTrivia/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     7419 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/selfTrivia/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.495261 honeybot-6.0.2/src/honeybot/plugins/downloaded/send_message/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/send_message/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      448 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/send_message/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     3200 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/send_message/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.495261 honeybot-6.0.2/src/honeybot/plugins/downloaded/story/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/story/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      211 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/story/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1125 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/story/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.495261 honeybot-6.0.2/src/honeybot/plugins/downloaded/sysinfo/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/sysinfo/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      316 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/sysinfo/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     8888 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/sysinfo/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.495261 honeybot-6.0.2/src/honeybot/plugins/downloaded/telephone_code/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/telephone_code/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      218 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/telephone_code/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    19078 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/telephone_code/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.499261 honeybot-6.0.2/src/honeybot/plugins/downloaded/test/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/test/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      147 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/test/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      510 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/test/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.499261 honeybot-6.0.2/src/honeybot/plugins/downloaded/todo/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/todo/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      675 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/todo/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     4444 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/todo/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.499261 honeybot-6.0.2/src/honeybot/plugins/downloaded/tpbquote/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/tpbquote/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      187 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/tpbquote/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      929 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/tpbquote/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.499261 honeybot-6.0.2/src/honeybot/plugins/downloaded/transfer-rumour/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/transfer-rumour/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      209 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/transfer-rumour/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1167 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/transfer-rumour/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.499261 honeybot-6.0.2/src/honeybot/plugins/downloaded/translate/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/translate/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      559 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/translate/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     9760 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/translate/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.499261 honeybot-6.0.2/src/honeybot/plugins/downloaded/url_shorten/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/url_shorten/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      235 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/url_shorten/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1023 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/url_shorten/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.499261 honeybot-6.0.2/src/honeybot/plugins/downloaded/username/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/username/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      227 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/username/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     6559 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/username/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.499261 honeybot-6.0.2/src/honeybot/plugins/downloaded/weather/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/weather/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      204 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/weather/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1189 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/weather/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.503261 honeybot-6.0.2/src/honeybot/plugins/downloaded/wikipedia/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/wikipedia/__init__.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      334 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/wikipedia/info.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1178 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/plugins/downloaded/wikipedia/main.py
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.503261 honeybot-6.0.2/src/honeybot/settings/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)       21 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/settings/AUTOJOIN_CHANNELS.conf
--rw-rw-r--   0 appinv    (1000) appinv    (1000)       73 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/settings/CONNECT.conf
--rw-rw-r--   0 appinv    (1000) appinv    (1000)       34 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/settings/FRIENDS.conf
--rw-rw-r--   0 appinv    (1000) appinv    (1000)       15 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/settings/OWNERS.conf
--rw-rw-r--   0 appinv    (1000) appinv    (1000)       29 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/settings/PLUGINS.conf
--rw-rw-r--   0 appinv    (1000) appinv    (1000)      748 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/settings/email_config.conf
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     1129 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/store.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     3885 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/test_core.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2384 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/test_legacy_core.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)     2293 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/test_plugin_script.py
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2022-11-30 10:25:54.000000 honeybot-6.0.2/src/honeybot/todo.txt
-drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2022-11-30 11:35:45.387261 honeybot-6.0.2/src/honeybot.egg-info/
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    26501 2022-11-30 11:35:45.000000 honeybot-6.0.2/src/honeybot.egg-info/PKG-INFO
--rw-rw-r--   0 appinv    (1000) appinv    (1000)    11851 2022-11-30 11:35:45.000000 honeybot-6.0.2/src/honeybot.egg-info/SOURCES.txt
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        1 2022-11-30 11:35:45.000000 honeybot-6.0.2/src/honeybot.egg-info/dependency_links.txt
--rw-rw-r--   0 appinv    (1000) appinv    (1000)       51 2022-11-30 11:35:45.000000 honeybot-6.0.2/src/honeybot.egg-info/entry_points.txt
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        1 2022-07-24 17:03:06.000000 honeybot-6.0.2/src/honeybot.egg-info/not-zip-safe
--rw-rw-r--   0 appinv    (1000) appinv    (1000)        9 2022-11-30 11:35:45.000000 honeybot-6.0.2/src/honeybot.egg-info/top_level.txt
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.969902 honeybot-6.1.0/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     1081 2023-07-02 06:22:37.000000 honeybot-6.1.0/LICENSE
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)    22495 2023-07-03 13:00:17.969902 honeybot-6.1.0/PKG-INFO
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)    21378 2023-07-02 06:22:37.000000 honeybot-6.1.0/README.md
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      559 2023-07-02 06:22:37.000000 honeybot-6.1.0/pyproject.toml
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      354 2023-07-03 13:00:17.973902 honeybot-6.1.0/setup.cfg
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     2310 2023-07-03 12:56:20.000000 honeybot-6.1.0/setup.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.901901 honeybot-6.1.0/src/
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.913901 honeybot-6.1.0/src/honeybot/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)       22 2023-07-03 12:56:52.000000 honeybot-6.1.0/src/honeybot/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)       33 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/__main__.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.917901 honeybot-6.1.0/src/honeybot/api/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/api/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      454 2023-07-03 12:56:20.000000 honeybot-6.1.0/src/honeybot/api/commands.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)       91 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/api/generate.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      667 2023-07-03 12:56:20.000000 honeybot-6.1.0/src/honeybot/api/init.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     9012 2023-07-03 12:56:20.000000 honeybot-6.1.0/src/honeybot/api/main.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      640 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/api/memory.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     1387 2023-07-03 12:56:20.000000 honeybot-6.1.0/src/honeybot/api/print.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      504 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/api/utils.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     3363 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/gui_manager.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      109 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/lab.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     1344 2023-07-03 12:56:20.000000 honeybot-6.1.0/src/honeybot/manage.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.917901 honeybot-6.1.0/src/honeybot/plugins/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/__init__.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.917901 honeybot-6.1.0/src/honeybot/plugins/core/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/core/__init__.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.917901 honeybot-6.1.0/src/honeybot/plugins/core/joins/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/core/joins/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      881 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/core/joins/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.917901 honeybot-6.1.0/src/honeybot/plugins/core/log/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/core/log/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     1335 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/core/log/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.917901 honeybot-6.1.0/src/honeybot/plugins/core/uptime/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/core/uptime/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     1027 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/core/uptime/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.917901 honeybot-6.1.0/src/honeybot/plugins/downloaded/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/__init__.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.917901 honeybot-6.1.0/src/honeybot/plugins/downloaded/abbreviation/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/abbreviation/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      178 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/abbreviation/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     2577 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/abbreviation/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.917901 honeybot-6.1.0/src/honeybot/plugins/downloaded/age/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/age/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      196 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/age/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     1367 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/age/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.917901 honeybot-6.1.0/src/honeybot/plugins/downloaded/basketball/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/basketball/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      495 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/basketball/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     8427 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/basketball/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.917901 honeybot-6.1.0/src/honeybot/plugins/downloaded/birthparadox/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/birthparadox/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      300 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/birthparadox/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     3733 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/birthparadox/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.917901 honeybot-6.1.0/src/honeybot/plugins/downloaded/bitcoin/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/bitcoin/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      297 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/bitcoin/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      938 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/bitcoin/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.921901 honeybot-6.1.0/src/honeybot/plugins/downloaded/blackjack/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/blackjack/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      310 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/blackjack/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     7900 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/blackjack/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.921901 honeybot-6.1.0/src/honeybot/plugins/downloaded/blackjack/poker_assets/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/blackjack/poker_assets/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     2809 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/blackjack/poker_assets/best5.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     1184 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/blackjack/poker_assets/board.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     1659 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/blackjack/poker_assets/card.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     2456 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/blackjack/poker_assets/deck.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     1429 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/blackjack/poker_assets/game_init.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     2295 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/blackjack/poker_assets/hand.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     2492 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/blackjack/poker_assets/player.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      363 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/blackjack/poker_assets/pot.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     3064 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/blackjack/poker_assets/test.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.921901 honeybot-6.1.0/src/honeybot/plugins/downloaded/book_of_day/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/book_of_day/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      272 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/book_of_day/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      948 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/book_of_day/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.921901 honeybot-6.1.0/src/honeybot/plugins/downloaded/caesar_cipher/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/caesar_cipher/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      225 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/caesar_cipher/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      803 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/caesar_cipher/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.925901 honeybot-6.1.0/src/honeybot/plugins/downloaded/calc/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/calc/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      252 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/calc/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     1791 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/calc/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.925901 honeybot-6.1.0/src/honeybot/plugins/downloaded/channeljoin/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/channeljoin/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      215 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/channeljoin/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     1212 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/channeljoin/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.925901 honeybot-6.1.0/src/honeybot/plugins/downloaded/cointoss/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/cointoss/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      191 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/cointoss/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      677 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/cointoss/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.925901 honeybot-6.1.0/src/honeybot/plugins/downloaded/comic/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/comic/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      184 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/comic/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      815 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/comic/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.925901 honeybot-6.1.0/src/honeybot/plugins/downloaded/conv_sniff/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/conv_sniff/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      235 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/conv_sniff/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     2689 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/conv_sniff/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.925901 honeybot-6.1.0/src/honeybot/plugins/downloaded/converter/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/converter/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      325 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/converter/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     4402 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/converter/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.929901 honeybot-6.1.0/src/honeybot/plugins/downloaded/corona/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/corona/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      286 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/corona/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     5711 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/corona/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.929901 honeybot-6.1.0/src/honeybot/plugins/downloaded/country/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/country/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      197 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/country/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)    10427 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/country/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.929901 honeybot-6.1.0/src/honeybot/plugins/downloaded/dadjoke/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/dadjoke/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      256 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/dadjoke/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      812 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/dadjoke/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.929901 honeybot-6.1.0/src/honeybot/plugins/downloaded/date/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/date/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      205 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/date/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      815 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/date/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.933901 honeybot-6.1.0/src/honeybot/plugins/downloaded/debug/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/debug/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      207 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/debug/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      579 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/debug/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.933901 honeybot-6.1.0/src/honeybot/plugins/downloaded/diary/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/diary/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      402 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/diary/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     5394 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/diary/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.933901 honeybot-6.1.0/src/honeybot/plugins/downloaded/dictionary/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/dictionary/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      300 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/dictionary/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      855 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/dictionary/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.933901 honeybot-6.1.0/src/honeybot/plugins/downloaded/duckduckgo/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/duckduckgo/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      247 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/duckduckgo/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      917 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/duckduckgo/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.933901 honeybot-6.1.0/src/honeybot/plugins/downloaded/emoji/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/emoji/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      172 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/emoji/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      467 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/emoji/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.937901 honeybot-6.1.0/src/honeybot/plugins/downloaded/excuse/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/excuse/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      169 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/excuse/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      675 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/excuse/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.937901 honeybot-6.1.0/src/honeybot/plugins/downloaded/fact/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/fact/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      245 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/fact/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     8715 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/fact/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.937901 honeybot-6.1.0/src/honeybot/plugins/downloaded/google/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/google/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      214 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/google/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     1337 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/google/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.937901 honeybot-6.1.0/src/honeybot/plugins/downloaded/greet/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/greet/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      197 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/greet/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      554 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/greet/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.937901 honeybot-6.1.0/src/honeybot/plugins/downloaded/hangman/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/hangman/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      287 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/hangman/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     7324 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/hangman/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.941901 honeybot-6.1.0/src/honeybot/plugins/downloaded/help/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/help/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      242 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/help/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      772 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/help/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.941901 honeybot-6.1.0/src/honeybot/plugins/downloaded/horoscope/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/horoscope/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      413 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/horoscope/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     8475 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/horoscope/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.941901 honeybot-6.1.0/src/honeybot/plugins/downloaded/installed_modules/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/installed_modules/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      214 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/installed_modules/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     1136 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/installed_modules/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.941901 honeybot-6.1.0/src/honeybot/plugins/downloaded/joke/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/joke/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      199 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/joke/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     4575 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/joke/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.941901 honeybot-6.1.0/src/honeybot/plugins/downloaded/magic_ball/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/magic_ball/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      261 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/magic_ball/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     1628 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/magic_ball/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.941901 honeybot-6.1.0/src/honeybot/plugins/downloaded/mail/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/mail/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      759 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/mail/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     4838 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/mail/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.945901 honeybot-6.1.0/src/honeybot/plugins/downloaded/maths/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/maths/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      369 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/maths/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     2562 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/maths/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.945901 honeybot-6.1.0/src/honeybot/plugins/downloaded/memo/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/memo/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      255 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/memo/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     1145 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/memo/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.945901 honeybot-6.1.0/src/honeybot/plugins/downloaded/monero/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/monero/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      341 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/monero/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     1298 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/monero/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.945901 honeybot-6.1.0/src/honeybot/plugins/downloaded/monopoly/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/monopoly/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      939 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/monopoly/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)    60676 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/monopoly/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.945901 honeybot-6.1.0/src/honeybot/plugins/downloaded/monopoly/monopoly_assets/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/monopoly/monopoly_assets/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     8294 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/monopoly/monopoly_assets/monopoly_assets.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     1458 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/monopoly/monopoly_assets/monopoly_player.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.949901 honeybot-6.1.0/src/honeybot/plugins/downloaded/movies_imdb/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/movies_imdb/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      347 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/movies_imdb/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     4610 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/movies_imdb/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.949901 honeybot-6.1.0/src/honeybot/plugins/downloaded/news/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/news/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      237 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/news/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     1255 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/news/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.949901 honeybot-6.1.0/src/honeybot/plugins/downloaded/onthisday/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/onthisday/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      191 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/onthisday/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     1454 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/onthisday/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.949901 honeybot-6.1.0/src/honeybot/plugins/downloaded/password_generator/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/password_generator/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      561 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/password_generator/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     4787 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/password_generator/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.949901 honeybot-6.1.0/src/honeybot/plugins/downloaded/proverb/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/proverb/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      180 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/proverb/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     1838 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/proverb/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.953902 honeybot-6.1.0/src/honeybot/plugins/downloaded/pydocs/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/pydocs/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      298 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/pydocs/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      853 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/pydocs/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.953902 honeybot-6.1.0/src/honeybot/plugins/downloaded/pynews/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/pynews/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      229 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/pynews/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     1258 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/pynews/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.953902 honeybot-6.1.0/src/honeybot/plugins/downloaded/pypi/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/pypi/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      197 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/pypi/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     1414 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/pypi/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.953902 honeybot-6.1.0/src/honeybot/plugins/downloaded/quote/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/quote/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      172 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/quote/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     4871 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/quote/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.953902 honeybot-6.1.0/src/honeybot/plugins/downloaded/random_color/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/random_color/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      236 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/random_color/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      952 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/random_color/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.953902 honeybot-6.1.0/src/honeybot/plugins/downloaded/random_image/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/random_image/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      171 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/random_image/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      719 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/random_image/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.957902 honeybot-6.1.0/src/honeybot/plugins/downloaded/repostats/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/repostats/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      228 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/repostats/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     1428 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/repostats/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.957902 honeybot-6.1.0/src/honeybot/plugins/downloaded/riddle/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/riddle/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      285 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/riddle/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     3821 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/riddle/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.957902 honeybot-6.1.0/src/honeybot/plugins/downloaded/roll/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/roll/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      201 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/roll/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     1751 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/roll/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.957902 honeybot-6.1.0/src/honeybot/plugins/downloaded/roman_numeral/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/roman_numeral/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      250 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/roman_numeral/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     2677 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/roman_numeral/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.957902 honeybot-6.1.0/src/honeybot/plugins/downloaded/russian_roulette/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/russian_roulette/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      514 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/russian_roulette/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     1470 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/russian_roulette/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.957902 honeybot-6.1.0/src/honeybot/plugins/downloaded/selfTrivia/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/selfTrivia/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      249 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/selfTrivia/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     7387 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/selfTrivia/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.961902 honeybot-6.1.0/src/honeybot/plugins/downloaded/send_message/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/send_message/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      448 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/send_message/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     3148 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/send_message/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.961902 honeybot-6.1.0/src/honeybot/plugins/downloaded/story/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/story/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      211 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/story/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     1101 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/story/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.961902 honeybot-6.1.0/src/honeybot/plugins/downloaded/sysinfo/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/sysinfo/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      316 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/sysinfo/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     8762 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/sysinfo/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.961902 honeybot-6.1.0/src/honeybot/plugins/downloaded/telephone_code/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/telephone_code/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      218 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/telephone_code/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)    19054 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/telephone_code/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.961902 honeybot-6.1.0/src/honeybot/plugins/downloaded/test/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/test/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      147 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/test/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      486 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/test/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.965902 honeybot-6.1.0/src/honeybot/plugins/downloaded/todo/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/todo/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      675 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/todo/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     4415 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/todo/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.965902 honeybot-6.1.0/src/honeybot/plugins/downloaded/tpbquote/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/tpbquote/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      187 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/tpbquote/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      905 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/tpbquote/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.965902 honeybot-6.1.0/src/honeybot/plugins/downloaded/transfer-rumour/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/transfer-rumour/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      209 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/transfer-rumour/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     1143 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/transfer-rumour/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.965902 honeybot-6.1.0/src/honeybot/plugins/downloaded/translate/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/translate/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      559 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/translate/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     9704 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/translate/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.965902 honeybot-6.1.0/src/honeybot/plugins/downloaded/url_shorten/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/url_shorten/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      235 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/url_shorten/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      999 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/url_shorten/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.965902 honeybot-6.1.0/src/honeybot/plugins/downloaded/username/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/username/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      227 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/username/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     6519 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/username/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.969902 honeybot-6.1.0/src/honeybot/plugins/downloaded/weather/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/weather/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      204 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/weather/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     1163 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/weather/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.969902 honeybot-6.1.0/src/honeybot/plugins/downloaded/wikipedia/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/wikipedia/__init__.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      334 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/wikipedia/info.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     1154 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/plugins/downloaded/wikipedia/main.py
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.969902 honeybot-6.1.0/src/honeybot/settings/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)       21 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/settings/AUTOJOIN_CHANNELS.conf
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)       73 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/settings/CONNECT.conf
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)       34 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/settings/FRIENDS.conf
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)       15 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/settings/OWNERS.conf
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)       40 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/settings/PLUGINS.conf
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)      748 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/settings/email_config.conf
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     1128 2023-07-03 12:56:20.000000 honeybot-6.1.0/src/honeybot/store.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     3885 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/test_core.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     2394 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/test_legacy_core.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)     2353 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/test_plugin_script.py
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        0 2023-07-02 06:22:37.000000 honeybot-6.1.0/src/honeybot/todo.txt
+drwxrwxr-x   0 appinv    (1000) appinv    (1000)        0 2023-07-03 13:00:17.913901 honeybot-6.1.0/src/honeybot.egg-info/
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)    22495 2023-07-03 13:00:17.000000 honeybot-6.1.0/src/honeybot.egg-info/PKG-INFO
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)    12508 2023-07-03 13:00:17.000000 honeybot-6.1.0/src/honeybot.egg-info/SOURCES.txt
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        1 2023-07-03 13:00:17.000000 honeybot-6.1.0/src/honeybot.egg-info/dependency_links.txt
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)       51 2023-07-03 13:00:17.000000 honeybot-6.1.0/src/honeybot.egg-info/entry_points.txt
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        1 2023-07-02 06:28:22.000000 honeybot-6.1.0/src/honeybot.egg-info/not-zip-safe
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)       13 2023-07-03 13:00:17.000000 honeybot-6.1.0/src/honeybot.egg-info/requires.txt
+-rw-rw-r--   0 appinv    (1000) appinv    (1000)        9 2023-07-03 13:00:17.000000 honeybot-6.1.0/src/honeybot.egg-info/top_level.txt
```

### Comparing `honeybot-6.0.2/LICENSE` & `honeybot-6.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `honeybot-6.0.2/PKG-INFO` & `honeybot-6.1.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,69 +1,59 @@
-Metadata-Version: 2.1
-Name: honeybot
-Version: 6.0.2
-Summary: IRC bot with vast collection of plugins. First timers friendly
-Home-page: https://github.com/pyhoneybot/honeybot
-Author: Abdur-Rahmaan Janhnageer
-Author-email: arj.python@gmail.com
-License: MIT
-Project-URL: Changelog, https://github.com/pyhoneybot/honeybot/blob/main/CHANGES.md
-Keywords: irc bot plugins
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # 🍯 honeybot py [ [docs](https://pyhoneybot.github.io/honeybot/) ]
 
 <div align="center">
 
-
-
-
 <img src="./assets/honeybot_real.png" width="64" />
 
 [![PyPI version](https://badge.fury.io/py/honeybot.png)](https://badge.fury.io/py/honeybot)
 [![First Timers Only](https://img.shields.io/badge/first--timers--only-friendly-blue.svg)](https://www.firsttimersonly.com/)
 ![Open Source Love](https://img.shields.io/badge/Open%20Source-%E2%9D%A4-pink.svg)
 ![Made in Moris](https://img.shields.io/badge/Made%20in-Moris-green.svg)
 [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/6329/badge)](https://bestpractices.coreinfrastructure.org/projects/6329)
 [![OpenSSF Scorecard](https://api.securityscorecards.dev/projects/github.com/pyhoneybot/honeybot/badge)](https://api.securityscorecards.dev/projects/github.com/pyhoneybot/honeybot)
 
 ## Launching pyhoneybot Rewards
- Contributed to pyhoneybot? Here is a big thank you from our community to you.
- Claim your badge and showcase them with pride.
- Let us inspire more folks !
 
- ![pyhoneybot Badges](https://aviyel.com/assets/uploads/rewards/share/project/84/512/share.png)
- ### **[Claim Now!](https://aviyel.com/projects/84/pyhoneybot/rewards)**
+Contributed to pyhoneybot? Here is a big thank you from our community to you.
+Claim your badge and showcase them with pride.
+Let us inspire more folks !
+
+![pyhoneybot Badges](https://aviyel.com/assets/uploads/rewards/share/project/84/512/share.png)
+
+### **[Claim Now!](https://aviyel.com/projects/84/pyhoneybot/rewards)**
 
 <hr>
-🇲🇺 🇺🇸 🇨🇦 🇦🇷 🇮🇳 🇬🇧 🇬🇬 🇧🇷 🇸🇽 🇵🇱 🇩🇪
+🇲🇺 🇺🇸 🇨🇦 🇦🇷 🇮🇳 🇬🇧 🇬🇬 🇧🇷 🇸🇽 🇵🇱 🇩🇪 🇲🇼
 
 </div>
 <div align="center">
 
 [![Open Source Helpers](https://www.codetriage.com/pyhoneybot/honeybot/badges/users.svg)](https://www.codetriage.com/pyhoneybot/honeybot)
 [![Discord](https://img.shields.io/badge/chat%20on-discord-green.svg)](https://discordapp.com/invite/E6zD4XT)
 
 </div>
 
+# Table of Contents
+
+- [📮 About](#-about)
+- [🕹 Project Motivation](#-project-motivation)
+- [✂ Current Features](#-current-features)
+- [:mountain: GUI clients](#mountain-gui-clients)
+- [⌚ Current Plugins](#-current-plugins)
+- [⚡ Quickstart](#-quickstart)
+- [💻 Seeing The Bot In Action](#-seeing-the-bot-in-action)
+- [Docker](#docker)
+- [🔧 Plugins Development](#-plugins-development)
+- [📃 Contributing Guide](#-contributing-guide)
+- [🔌 Todo Plugins](#-todo-plugins)
+- [☑ Allowing Plugins](#-allowing-plugins)
+- [:thought_balloon: Project Testimonials](https://github.com/deadex-ng/honeybot/blob/readme-fix/TESTIMONIALS.md)
+- [📧 Contact (Including vulnerabilities)](#-contact-including-vulnerabilities)
+- [🖊 Credits](#-credits)
+
 ## 📮 About
 
 HoneyBot is a python-based IRC bot. (**python3.7**) | If you want to just run the bot, go to the [quick start section](https://github.com/pyhoneybot/honeybot#-quickstart)
 
 > HoneyBot is my first time collaborating to an open source project and I'm loving it. Before discovering HoneyBot, I was very intimidated on the idea of working with other people and had no idea what an IRC even was. Now I realize how much fun and rewarding it is to work together on a project with dedicated and friendly individuals. The documentation is easy to follow and everyone is super helpful. I highly recommend any new programmer who want to contribute on an open source project to try out HoneyBot. Personally I enjoy working on this project more than my own schoolwork. --[@RiceAbove](https://github.com/RiceAbove)
 
 Feel free to contribute to the project!
@@ -132,18 +122,22 @@
 | 🛩 flight               | Gets flight info from flightradar24                                                   | [@AngeloGiacco](https://github.com/AngeloGiacco)                                                         |
 | 🎲 roll                | Rolls a dice                                                                          | [@GlennToms](https://github.com/GlennToms)                                                               |
 | ❓ help                | Show link to plugin's information page                                                | [@edumello](https://github.com/edumello)                                                                 |
 | ✅ channeljoin         | Join command for bot                                                                  | [@marceloyb](https://github.com/marceloyb)                                                               |
 | :page_with_curl: comic | Returns a random comic                                                                | [@mboekhold](https://github.com/mboekhold)                                                               |
 | 📝 todo                | Makes a to do list                                                                    | [@h-ranjan1110](https://github.com/h-ranjan1110)                                                         |
 | 🎱 Magic 8 Ball        | Answer questions using magic 8 ball                                                   | [@ZakariaTalhami](https://github.com/ZakariaTalhami)                                                     |
-| 🎟 Random Excuse       | Generates a random excuse for you.                                                   | [@rakeshseal0](https://github.com/rakeshseal0)
-| 🦆 DuckDuckGo Search    | Search queries in duckduckgo and return abstract.                                    | [@rakeshseal0](https://github.com/rakeshseal0)                                                     |
-| 🖼 Random Image        | Returns a random image url.                                                          | [@rakeshseal0](https://github.com/rakeshseal0) 
-| 🛢 URL Shortener       | Shortens a url                                                          | [@rakeshseal0](https://github.com/rakeshseal0) 
+| 🎟 Random Excuse        | Generates a random excuse for you.                                                    | [@rakeshseal0](https://github.com/rakeshseal0)                                                           |
+| 🦆 DuckDuckGo Search   | Search queries in duckduckgo and return abstract.                                     | [@rakeshseal0](https://github.com/rakeshseal0)                                                           |
+| 🖼 Random Image         | Returns a random image url.                                                           | [@rakeshseal0](https://github.com/rakeshseal0)                                                           |
+| 🛢 URL Shortener        | Shortens a url                                                                        | [@rakeshseal0](https://github.com/rakeshseal0)                                                           |
+| 😁 emoji               | Returns emoji meaning                                                                 | [@deadex-ng](https://github.com/deadex-ng)                                                               |
+| 🎂 birthday            | Shows birthday match probability on a people group.                                   | [@paulosgf](https://github.com/paulosgf)                                                                 |
+| 🏀 basketball          | Shows information about the medals of euroBasket and Basketball world cup             | [@kefthymic](https://github.com/kefthymic)                                                               |
+| 🎬 movies_imdb         | Returns certain information about a certain movie or shows 250 all time best movies   | [@ZoeyKats](https://github.com/ZoeyKats)                                                                 |
 
 ## ⚡ Quickstart
 
 setup
 
 ```bash
 mkdir botx
@@ -190,25 +184,26 @@
 
 then join channel `#ltch`
 
 you should see the bot as hbot ... or as it's name is in [settings](https://github.com/pyhoneybot/honeybot/blob/master/src/honeybot/settings/CONNECT.conf)
 
 ## Docker
 
-** Building Docker image **
+**Building Docker image**
+
 Change SERVER, PORT and NICKNAME variables to match your preferences
 
 ```
-docker build -t honeybot -f ./docker/Dockerfile .
+docker build -t "honeybot/honeybot:6.0.2" .
 ```
 
-** Running Docker image **
+**Running Docker image**
 
 ```
-docker run honeybot
+docker run -d --name=honeybot honeybot/honeybot:v6.0.2 honeybot run
 ```
 
 ## 🔧 Plugins Development
 
 Each plugin has a folder named after it. In it there is a file called main.py. In each there is a class called Plugin.
 
 ```python
@@ -311,153 +306,15 @@
 ## 📃 Contributing Guide
 
 <https://pyhoneybot.github.io/honeybot/How_Tos/contributing.html>
 
 - don't forget to add your country flag here after accepted PR. i'll have to hunt it down on your profile if not.
 - make sure to follow PEP8
 
-**About PR**
-
-first clone the project
-
-```
-git clone https://github.com/pyhoneybot/honeybot.git
-```
-
-cd into the project
-
-```
-cd honeybot
-```
-
-create a virtualenv to work with different python \ libs versions
-
-```
-python -m venv venv
-source venv/bin/activate
-```
-
-install the tools needed to make the constraint checks
-
-```
-pip install black isort bandit pre-commit
-pre-commit install
-```
-
-different changes to different files. for example, someone making a weather plugin first he creates a new branch
-
-```
-git checkout -b "weather-plugin"
-```
-
-test if all files are well formatted, complying with style and security rules, before send the PR
-
-```
-black --check --verbose --config ./pyproject.toml src/honeybot/plugins/downloaded/weather/main.py
-isort --check-only --settings-path ./pyproject.toml src/honeybot/plugins/downloaded/weather/main.py
-bandit -ll -c ./pyproject.toml -r src/honeybot/plugins/downloaded/weather/main.py 
-```
-
-then he commits
-
-```
-git add *
-git commit -m "added weather plugin"
-```
-
-or
-
-```
-git commit -a -m "did this"
-```
-
-then he push to create a PR with the branch
-
-```
-git push origin head
-```
-
-or
-
-```
-git push origin weather-plugin
-```
-
-now let us say he wants to work on another issue, adding a joke in the jokes plugin, he creates another branch
-
-```
-git checkout -b "add-jokes"
-```
-
-after, same as before
-
-```
-git add *
-git commit -m "added some jokes"
-git push origin head
-```
-
-now he wants to fix his weather plugin, he changes branch
-
-```
-git checkout weather-plugin
-```
-
-works, then commit
-
-```
-git add *
-git commit -m "fixed <issue>"
-```
-
-then a PR
-
-```
-git push origin head
-```
-
-**Why all these?**
-
-So as not to reject a whole PR just because of some oddities. Reject only unneeded part.
-
-**Updating the Documentation**
-
-If you created a new plugin you should add your plugin to the documentation.
-To do this, go into your cloned honeybot repo and then into the directory _docs/source/Plugins_ .
-Depending on the type of plugin write this into the development, fun, miscellaneous or utility RST file:
-
-```rst
-
-   <Plugin-Name>
-   ^^^^^^^^^^^^^
-   .. automodule:: plugins.<your-plugin-filename>
-      :members:
-```
-
-This allows sphinx to automatically pull the docstrings from the code of your plugin and parse them accordingly.
-
-A small guide on how to further contribute to the documentation of the project can be found [here](https://pyhoneybot.github.io/honeybot/How_Tos/documentation.html)
-
-## 🥄 Updating fork
-
-Now, other changes are ongoing, what if you need the latest changes?
-
-```
-git pull origin master
-```
-
-helps if you cloned your own repo. What if you want to update your local copy of someone else's repo that you forked?
-You do it like that
-
-```
-cd <your/local/cloned/repo/path/here>
-git remote add upstream https://github.com/pyhoneybot/honeybot.git
-git fetch upstream
-git pull upstream master
-```
+Check out [Contributing](https://github.com/pyhoneybot/honeybot/blob/master/CONTRIBUTING.md) to get started on contributing.
 
 ## 🔌 Todo Plugins
 
 - [x] 💐 humour
 - [x] 🌨️ weather
 - [x] ✉️ mail
 - [x] 🎛️ maths
@@ -472,42 +329,16 @@
 in PLUGINS.conf, add the plugin to allow on a new line !
 
 ```
 calc
 username
 ```
 
-## :thought_balloon: Project Testimonials
-
-[@TannerFry](https://github.com/TannerFry)
-
-> With experience in programming in Python, and implementing an SMTP email plugin for a different system, picking up HoneyBot and following the documentation provided for new-comers made it very simple to implement the same SMTP email plugin to the HoneyBot system. This was my first time contributing to an open-source
-> project on GitHub and it was an overall great experience. The welcoming of new contributors and documentation on how to contribute and implement plugins is great for people
-> who have never contributed to a project before, and Abdur-Rahmaan Janhangeer was extremely helpful when answering my questions and helping me along the way.
-
-[@RiceAbove](https://github.com/RiceAbove)
-
-> HoneyBot is my first time collaborating to an open source project and I'm loving it. Before discovering HoneyBot, I was very intimidated on the idea of working with other people and had no idea what an IRC even was. Now I realize how much fun and rewarding it is to work together on a project with dedicated and friendly individuals. The documentation is easy to follow and everyone is super helpful. I highly recommend any new programmer who want to contribute on an open source project to try out HoneyBot. Personally I enjoy working on this project more than my own schoolwork.
-
-[@justinwalker4179](https://github.com/IronPenguin4179)
-
-> HoneyBot is my first open source project and I had never worked with an IRC before. For school I was required to contribute to projects, but it was always so intimidating to me. I had always heard it gets easier once you've gotten over the fear wall, and that's what HoneyBot did for me. Excellent readme and quick feedback allowed me to make my first plugin. Now I've made many contributions, and look forward to any new issues I can get my hands on. Abdur-Rahmaan Janhangeer has been extremely helpful and I owe him and this project a lot for getting me into the open source world.
-
-[@mboekhold](https://github.com/mboekhold)
-
-> HoneyBot is a very friendly and welcoming community. They provided quick feedback and I would defenitely recommend this project to newcomers to give them that first boost on contributing to open source. HoneyBot helps you all the way there to issuing your first PR, step by step. I contributed a comic plugin, and I was thankful for meeting all the friendly and passionate people who are active in this community.
-
-[@Macr0Nerd](https://github.com/Macr0Nerd)
-
-> I came onto this project in October of 2018. At the time, my experience with open source was nil. I wasn't even sure I was good with python; I just happened to be better than everyone in class. Working on HoneyBot really opened my eyes to the power of community and programming, and has sent me on a path I don't wanna turn from. Just seeing how this project has evolved over the past year and how I've grown with it, I wouldn't trade it for the world. My name might not be on any of the recent plugins or doc strings, but I'll never forget that it'll always be tied to this project and a lot of the code. Also, I don't know if they'll check my commit so go look at the C++ Client! It's cool I promise!
-
 ## 📧 Contact (Including vulnerabilities)
 
 ### Email
 
 - Abdur-Rahmaan Janhangeer | arj.python@gmail.com
 
 ## 🖊 Credits
 
 - [@arwinneil](https://github.com/arwinneil), "Open Source" and "Made In Moris" badges
-
-
```

### Comparing `honeybot-6.0.2/pyproject.toml` & `honeybot-6.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `honeybot-6.0.2/setup.py` & `honeybot-6.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,32 +41,33 @@
     url="https://github.com/pyhoneybot/honeybot",
     project_urls={"Changelog": "https://github.com/pyhoneybot/honeybot/blob/main/CHANGES.md"},
     license="MIT",
     py_modules=[],
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     package_data={
-        "honeybot": ["settings/*.conf", "*.txt"]
+        "honeybot": ["settings/*.conf", "*.txt", "*.toml"]
     },
     python_requires=">=3.7.0",
     zip_safe=False,
     install_requires=[
-
+        "tomli>=2.0.0"
     ],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3 :: Only",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     entry_points={
         "console_scripts": [
             "honeybot=honeybot.manage:main",
         ]
```

### Comparing `honeybot-6.0.2/src/honeybot/api/main.py` & `honeybot-6.1.0/src/honeybot/api/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,57 +1,54 @@
-# -*- coding: utf-8 -*-
-
 import configparser
 import importlib
 import logging
 import os
 import pathlib
 import socket
 import subprocess
 import sys
 import time
 
 import pkg_resources
+import tomli
 
-try:
-    from honeybot.api import commands, memory
-    from honeybot.api.utils import configfile_to_list, get_requirements, prevent_none
-except Exception as e:
-    raise e
-
+from honeybot.api import commands, memory
+from honeybot.api import print as output
+from honeybot.api.utils import configfile_to_list, get_requirements, prevent_none
 
 plugins = []
 
 # Start logger
 logger = logging.getLogger("bot_core")
 
 """
 BOT CONNECTION SETUP
 """
 
 
-class Bot_core(object):
+class BotCore:
     def __init__(self, info, password=""):
         self.info = info
-        connect_config = configparser.ConfigParser()
-        connect_config.read(os.path.join(self.info["settings_path"], "CONNECT.conf"))
+        with open(info["toml_path"], "rb") as f:
+            self.configs = tomli.load(f)
         self.settings_path = self.info["settings_path"]
         self.root_path = self.info["cwd"]
-        self.server_url = connect_config["INFO"]["server_url"]
-        self.port = int(connect_config["INFO"]["port"])
-        self.name = connect_config["INFO"]["name"]
-        self.owners = configfile_to_list(self.info["settings_path"], "OWNERS")
+        self.server_url = self.configs["INFO"]["server_url"]
+        self.port = int(self.configs["INFO"]["port"])
+        self.name = self.configs["INFO"]["name"]
+        self.owners = self.configs["USERNAMES"]["owners"]
         self.password = password
-        self.friends = configfile_to_list(self.info["settings_path"], "FRIENDS")
-        self.autojoin_channels = configfile_to_list(self.info["settings_path"], "AUTOJOIN_CHANNELS")
+        self.friends = self.configs["USERNAMES"]["friends"]
+        self.autojoin_channels = self.configs["INFO"]["autojoin_channels"]
+        self.downloaded_plugins_to_load = self.configs["PLUGINS"]["downloaded"]
         self.required_modules = get_requirements()
         self.time = time.time()
 
         self.irc = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        self.isListenOn = 1
+        self.is_listen_on = 1
         dom = self.server_url.split(".")
         self.domain = ".".join(dom[-2:])
         self.sp_command = "hbot"
         self.plugins = []
         self.core_plugins = []
 
     """
@@ -84,15 +81,16 @@
                 "prefix": prevent_none(prefix),
                 "command": prevent_none(command),
                 "args": ["" if e is None else e for e in args],
                 "address": prevent_none(address),
                 "user": prevent_none(user),
             }
         except Exception as e:
-            logger.error(e)
+            # logger.error(e)
+            pass
 
     def bot_info(self):
         return {
             "name": self.name,
             "special_command": self.sp_command,
             "required_modules": self.required_modules,
             "owners": self.owners,
@@ -124,48 +122,42 @@
         self.send(commands.join_channel(channel))
 
     """
     PLUGIN UTILS
     """
 
     def is_valid_plug_name(self, name):
-        if (name.startswith("__")) or (name == ""):
+        if name.startswith("__") or name == "":
             return False
 
         return True
 
     """
     BOT UTIL
     """
 
     def print_running_infos(self):
-        print("Run infos:")
+        print(output.status("i") + " Run infos:")
         for key in self.info:
-            print(key, self.info[key])
-        print("-" * 3)
+            print(output.tab() + " " + key, self.info[key])
+        print(output.line())
 
     def load_plugins_from_folder(self, category_folder, from_conf=None, from_dir=None):
+        if from_dir is True:
+            dir_path = os.path.join(self.info["plugins_path"], "core")
+            to_load = [f for f in os.listdir(dir_path) if self.is_valid_plug_name(f)]
+        elif from_conf is True:
+            to_load = self.configs["PLUGINS"]["downloaded"]
 
-        if from_dir is not None:
-            to_load = [f for f in os.listdir(from_dir) if self.is_valid_plug_name(f)]
-        elif from_conf is not None:
-            to_load = []
-            plugs = from_conf
-            with open(plugs) as f:
-                to_load = f.read().split("\n")
-                to_load = list(filter(lambda x: x != "", to_load))
-
-        print("Loading", category_folder)
+        print(output.status("i") + " Loading from", category_folder)
         for folder in to_load:
-            print("loading plugin:", folder)
+            print(output.tab(), "loading plugin:", folder)
             try:
                 sys.path.append(self.root_path)
-                module = importlib.import_module(
-                    "plugins.{}.{}.main".format(category_folder, folder)
-                )
+                module = importlib.import_module(f"plugins.{category_folder}.{folder}.main")
                 obj = module
                 self.plugins.append(obj)
             except ModuleNotFoundError as e:
                 logger.warning(f"{folder}: module import error, skipped' {e}")
 
             try:
                 req_path = os.path.join(
@@ -182,36 +174,35 @@
                             for requirement in pkg_resources.parse_requirements(requirements_txt)
                         ]
                         print("installing", install_requires)
                         subprocess.check_call(
                             [sys.executable, "-m", "pip", "install", *install_requires]
                         )
             except Exception as e:
-                logger.debug(e)
+                # logger.debug(e)
+                pass
 
     def load_plugins(self):
         """
         Load plugins that are specified in the plugins list.
 
         Args:
             plugins_to_load (list of str): List of plugins to load.
 
         Examples:
             TODO
         """
 
-        logger.info("Loading plugins...")
+        print(output.status("i") + " Loading plugins...")
 
-        conf_path = os.path.join(self.settings_path, "PLUGINS.conf")
-        dir_path = os.path.join(self.info["plugins_path"], "core")
-        self.load_plugins_from_folder("downloaded", from_conf=conf_path)
-        self.load_plugins_from_folder("core", from_dir=dir_path)
+        self.load_plugins_from_folder("downloaded", from_conf=True)
+        self.load_plugins_from_folder("core", from_dir=True)
 
-        logger.info("Loaded plugins")
-        print("---")
+        print(output.status("x") + " Loaded plugins")
+        print(output.line())
 
     def run_plugins(self, incoming):
         """
         incoming is the unparsed string. refer to test.py
         """
 
         for plugin in self.plugins:
@@ -243,45 +234,53 @@
         self.send(commands.identify(self.password))
 
     def greet(self):
         self.send(commands.set_nick(self.name))
         self.send(commands.present(self.name))
         for channel in self.autojoin_channels:
             self.send(commands.join_channel(channel))
+        print(output.status("x"), "Joined channels:", ", ".join(self.autojoin_channels))
 
     def pull(self):
-        while self.isListenOn:
+        print(output.status("i"), "Listening to incoming messages")
+        while self.is_listen_on:
             try:
-                data = self.irc.recv(2048)
-                raw_msg = data.decode("UTF-8")
-                msg = raw_msg.strip("\n\r")
-                self.stay_alive(msg)
-                self.core_commands_parse(msg)
-                logger.info(msg)
-
-                if len(data) == 0:
-                    try:
-                        logger.critical(f"<must handle reconnection - {len(data)}==0>")
-                        sys.exit()
-                    except Exception as e:
-                        logger.info(e)
+                data = self.irc.recv(2048).decode("UTF-8", errors="replace")
+                for line in data.split("\r\n"):
+                    if line != "":
+                        self.core_commands_parse(line)
+
+            except KeyboardInterrupt:
+                self.is_listen_on = False
+                self.quit()
             except Exception as e:
-                logger.info(e)
+                # logger.error(e)
+                # print(e)
+                # logger.debug("there was an error")
+                # logger.debug(data)
+                # logger.debug("!!")
+                # logger.debug(line)
+                # logger.debug("-" * 50)
+                pass
+
+    def quit(self):
+        self.send(commands.quit())
+        self.is_listen_on = False
 
     """
     ONGOING REQUIREMENT/S
     """
 
     def stay_alive(self, incoming):
         if not incoming:
             logger.critical("<must handle reconnection - incoming is not True>")
             sys.exit()
         parts = incoming.split(":")
         if parts[0].strip().lower() == "ping":
-            logger.warning("ping detected from: {}".format(parts[1]))
+            logger.warning(f"ping detected from: {parts[1]}")
             self.send(commands.pong_return(self.domain))
             self.send(commands.pong_return(parts[1]))
 
     # all in one for registered bot
     def registered_run(self):
         self.connect()
         self.identify()
```

### Comparing `honeybot-6.0.2/src/honeybot/gui_manager.py` & `honeybot-6.1.0/src/honeybot/gui_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 current_path = os.path.split(os.path.abspath(__file__))[0]
 pluginPath = os.path.join(os.sep, current_path, "plugins")
 configPath = os.path.join(os.sep, current_path, "settings", "PLUGINS.conf")
 
 
 def get_unique_text(text):
-    uniques = sorted(set([i.strip() for i in text.split("\n") if i]))
+    uniques = sorted({i.strip() for i in text.split("\n") if i})
     uniques_text = "\n".join(uniques)
     return uniques_text
 
 
 def saveFile():
     text = tt.get(1.0, END)
     unique_text = get_unique_text(text)
@@ -78,16 +78,18 @@
 
 elements = [
     [
         [
             "MainLabel",
             Label(
                 window,
-                text="Select the plugins you wish to \
-                        load and add them to the config file",
+                text=(
+                    "Select the plugins you wish to                         load and add them to"
+                    " the config file"
+                ),
             ),
         ]
     ],
     [["listbox", Listbox(window, width=60)]],
     [["addBtn", Button(window, text="Add Plugin", width=10, command=clicked)]],
     [["label2", Label(window, text="Editable PLUGINS.conf file:")]],
     [["tt", Text(window, width=80)]],
```

### Comparing `honeybot-6.0.2/src/honeybot/manage.py` & `honeybot-6.1.0/src/honeybot/manage.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import logging
 import os
 import sys
 
 try:
     from honeybot.api.generate import gen_pluginsinfo
     from honeybot.api.init import init
-    from honeybot.api.main import Bot_core
+    from honeybot.api.main import BotCore
     from honeybot.api.print import print_connect_settings, print_honeybot_manifesto
 except Exception as e:
     print(e)
 
 
 logging.basicConfig(
     level=logging.DEBUG,
@@ -26,23 +26,24 @@
     parser.add_argument("botsetting", choices=["run", "gen_pluginsinfo", "init"])
 
     args = parser.parse_args()
 
     info = {
         "cwd": os.getcwd(),
         "settings_path": os.path.join(os.getcwd(), "settings"),
+        "toml_path": os.path.join(os.getcwd(), "settings", "settings.toml"),
         "plugins_path": os.path.join(os.getcwd(), "plugins"),
     }
 
     print_honeybot_manifesto(info)
     if args.botsetting == "run":
 
         print_connect_settings(info)
         try:
-            x = Bot_core(info)
+            x = BotCore(info)
             x.unregistered_run()
         except KeyboardInterrupt:
             print("interrupted")
             sys.exit()
 
     elif args.botsetting == "gen_pluginsinfo":
         gen_pluginsinfo()
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/core/joins/main.py` & `honeybot-6.1.0/src/honeybot/plugins/core/joins/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [joins.py]
 Joins Plugin
 
 [Author]
 Gico Carlo Evangelista, https://gicocarlo.me/
 
@@ -24,12 +23,12 @@
 
             # If someone joins and it is not the bot, greet user
             bot_name = bot_info["name"]
             if info["command"] == "JOIN" and user != bot_name:
 
                 # Greets joined user
                 channel = info["args"][0]
-                greet = "Hello {} welcome to {} !".format(user, channel)
-                methods["send"](info["address"], "{}".format(greet))
+                greet = f"Hello {user} welcome to {channel} !"
+                methods["send"](info["address"], f"{greet}")
 
         except Exception as e:
             print("woops plugin error ", e)
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/core/log/main.py` & `honeybot-6.1.0/src/honeybot/plugins/core/log/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [log.py]
 Log Plugin
 
 [Author]
 Gico Carlo Evangelista, https://gicocarlo.me/
 
@@ -15,15 +14,15 @@
 # standard python file handling
 
 import os
 from datetime import datetime
 
 # Makes a new log dir if not existent
 # Change according to where you have honeybot dir
-log_path = "{}/log".format(os.getcwd())
+log_path = f"{os.getcwd()}/log"
 if not os.path.exists(log_path):
     os.makedirs("log")
 
 # Current date
 curr_date = datetime.today().strftime("%d-%m-%Y")
 
 
@@ -32,22 +31,22 @@
         pass
 
     def run(self, incoming, methods, info, bot_info):
         msgs = info["args"][1:]
         try:
             if info["command"] == "PRIVMSG":
                 # Make log file (if not existent) using current date
-                f = open("log/{}.txt".format(curr_date), "a+")
+                f = open(f"log/{curr_date}.txt", "a+")
 
                 # Current time
                 curr_time = datetime.now().strftime("%H:%M:%S")
 
                 # Parse the user ID from info['prefix']
                 raw_user = info["prefix"]
                 user_index = raw_user.find("!")
                 user = raw_user[0:user_index]
 
                 # Logging the chat into txt file
-                f.write("{}: {}: {}\r\n".format(curr_time, user, msgs[0]))
+                f.write(f"{curr_time}: {user}: {msgs[0]}\r\n")
 
         except Exception as e:
             print("woops plugin error ", e)
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/core/uptime/main.py` & `honeybot-6.1.0/src/honeybot/plugins/core/uptime/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [uptime.py]
 Uptime Plugin
 
 [Author]
 Nick Wiley
 
@@ -29,15 +28,15 @@
         uptime = current_time - start_time
         hrs = int(uptime / 3600)
         uptime -= hrs * 3600
         mins = int(uptime / 60)
         uptime -= mins * 60
         sec = int(uptime)
 
-        msg = "Bot has been up for {0} hr, {1} min, and {2} sec.".format(hrs, mins, sec)
+        msg = f"Bot has been up for {hrs} hr, {mins} min, and {sec} sec."
         return msg
 
     def run(self, incoming, methods, info, bot_info):
         try:
             if info["command"] == "PRIVMSG" and info["args"][1] == ".uptime":
                 start_time = bot_info["time"]
                 methods["send"](info["address"], Plugin.__convert_time(start_time))
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/abbreviation/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/abbreviation/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [abbreviation.py]
 Abbreviation Plugin
 
 [Author]
 Erin Moon, Sourav Dutta
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/age/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/age/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [age.py]
 Age Plugin
 
 [Author]
 Justin Walker
 
@@ -24,15 +23,15 @@
     def __age(day, mo, yr):
         years = date.today().year - yr
         months = date.today().month - mo
         days = date.today().day - day
         if months < 0 or (months == 0 and day < 0):
             years -= 1
 
-        msg = "You are {0}yrs. {1}mo. and {2} days old.".format(years, abs(months), abs(days))
+        msg = f"You are {years}yrs. {abs(months)}mo. and {abs(days)} days old."
         return msg
 
     def run(self, incoming, methods, info, bot_info):
         try:
             msgs = info["args"][1:][0].split()
             print(len(msgs))
             if info["command"] == "PRIVMSG" and msgs[0] == ".age":
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/bitcoin/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/bitcoin/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [bitcoin.py]
 Bitcoin Price Checking Plugin
 
 [Author]
 Gabriele Ron
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/blackjack/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/blackjack/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [blackjack.py]
 Blackjack Plugin
 [Author]
 Angelo Giacco
 [About]
 Play blackjack
@@ -142,15 +141,15 @@
             name = info["prefix"].split("!")[0]
             Plugin.bj_created = True
             Plugin.round_started = False
             Plugin.initPlayer(methods, info)
             Plugin.DECK = poker_assets.deck.Deck()
             methods["send"](
                 info["address"],
-                name + " has started a game of blackjack! " "Use .blackjack join to join in!",
+                name + " has started a game of blackjack! Use .blackjack join to join in!",
             )
         else:
             methods["send"](info["address"], "A game already exists!")
 
     def start(methods, info):
         """start the game"""
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/blackjack/poker_assets/best5.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/blackjack/poker_assets/best5.py`

 * *Files identical despite different names*

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/blackjack/poker_assets/board.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/blackjack/poker_assets/board.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """ board class """
 
 # pylint: disable=E1601
 
 
-class Board(object):
+class Board:
     """board class"""
 
     def __init__(self, board):
         """board initialization"""
 
         self.__board = board
         self.__flop = board[:3]
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/blackjack/poker_assets/card.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/blackjack/poker_assets/card.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """ card class """
 
 # pylint: disable=E1601
 
 
-class Card(object):
+class Card:
     """card class"""
 
     def __init__(self, card):
         """card initialization; Card('8s'), Card('QC')"""
         values = [
             0,
             1,
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/blackjack/poker_assets/deck.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/blackjack/poker_assets/deck.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # pylint: disable=E1601, W0612
 
 import random
 
 import card
 
 
-class Deck(object):
+class Deck:
     """deck class"""
 
     colors = ["C", "D", "H", "S"]
     figures = ["2", "3", "4", "5", "6", "7", "8", "9", "T", "J", "Q", "K", "A"]
 
     i = 0
     for color in colors:
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/blackjack/poker_assets/game_init.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/blackjack/poker_assets/game_init.py`

 * *Files identical despite different names*

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/blackjack/poker_assets/hand.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/blackjack/poker_assets/hand.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # import deuces "deuces==0.2",
 # import best5
 # import board
 # import card
 
 
-class Hand(object):
+class Hand:
     """hand class"""
 
     def __init__(self, hand):
         """hand initialization"""
 
         self.__hand = hand
         self.__card1 = hand[0]
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/blackjack/poker_assets/player.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/blackjack/poker_assets/player.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """ player class """
 # pylint: disable=E1601
 
 import game_init
 
 
-class Player(object):
+class Player:
     """player class"""
 
     def __init__(self, nr, chips, username):
         """player initialization"""
 
         self.__position_nr = nr
         self.__general_name = "player" + str(nr)
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/blackjack/poker_assets/test.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/blackjack/poker_assets/test.py`

 * *Files identical despite different names*

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/book_of_day/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/book_of_day/main.py`

 * *Files identical despite different names*

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/caesar_cipher/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/caesar_cipher/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [calc.py]
 Caesar Cipher plugin
 
 [Author]
 Kyle Galloway
 
@@ -26,10 +25,10 @@
 
             if info["command"] == "PRIVMSG":
                 if len(msgs) > 1:
                     if msgs[0] == ".caesar_cipher":
                         expr = msgs[1]
                         encoded = codecs.encode(expr, "rot-13")
                         print(encoded)
-                        methods["send"](info["address"], "{}".format(encoded))
+                        methods["send"](info["address"], f"{encoded}")
         except Exception as e:
             print("woops plugin", __file__, e)
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/calc/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/calc/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [calc.py]
 Maths Operation Plugin
 
 [Author]
 Abdur-Rahmaan Janhangeer, pythonmembers.club
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/channeljoin/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/channeljoin/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [channeljoin.py]
 Join Plugin
 
 [Author]
 Marcelo Benesciutti
 
@@ -22,15 +21,15 @@
     def run(self, incoming, methods, info, bot_info):
         try:
             msgs = info["args"][1:][0].split()
             if info["command"] == "PRIVMSG" and msgs[0] == ".channeljoin":
                 raw_user = info["prefix"]
                 user_index = raw_user.find("!")
                 user = raw_user[0:user_index]
-                with open("settings/OWNERS.conf", "r") as f:
+                with open("settings/OWNERS.conf") as f:
                     for owner in f:
                         if owner.strip() == user:
                             methods["join"](msgs[1])
                             break
                     else:
                         methods["send"](
                             info["address"],
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/cointoss/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/cointoss/main.py`

 * *Files identical despite different names*

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/conv_sniff/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/conv_sniff/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [conv_sniff.py]
 Conversation Sniffer Plugin
 
 [Author]
 Abdur-Rahmaan Janhangeer, pythonmembers.club
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/converter/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/converter/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,15 @@
             base_url = "https://www.x-rates.com/calculator/?"
             url = base_url + "from=" + base_cur + "&to=" + target_cur + "&amount=" + str(amount)
             page = requests.get(url)
             soup = BeautifulSoup(page.text, "html.parser")
 
             part1 = soup.find(class_="ccOutputTrail").previous_sibling
             part2 = soup.find(class_="ccOutputTrail").get_text(strip=True)
-            converted = "{}{}".format(part1, part2)
+            converted = f"{part1}{part2}"
             return str(amount) + base_cur + " is equal to " + converted + target_cur
 
     def run(self, incoming, methods, info, bot_info):
         try:
             msgs = info["args"][1:][0].split()
             if info["command"] == "PRIVMSG" and msgs[0] == ".convert":
                 if len(msgs) == 3:
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/corona/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/corona/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [corona.py]
 Coronavirus Plugin
 
 [Author]
 Angelo Giacco
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/country/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/country/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [countries.py]
 Country-Capital Plugin
 
 [Author]
 Phil Beld
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/dadjoke/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/dadjoke/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [dadjoke.py]
 Dad joke plugin
 
 [Author]
 moffetma Oregon State University CS
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/date/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/greet/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,29 @@
-# -*- coding: utf-8 -*-
 """
-[date.py]
-Date Plugin
+[greet.py]
+Greet Plugin
 
 [Author]
-Gico Carlo Evangelista, https://gicocarlo.me/
+Abdur-Rahmaan Janhangeer, pythonmembers.club
 
 [About]
-Will post the current date
+responds to .hi, demo of a basic plugin
 
 [Commands]
->>> .date today
-returns the current date
+>>> .hi
+returns hoo
 """
 
-from datetime import date
-
 
 class Plugin:
     def __init__(self):
         pass
 
-    # Date attribute
-    # Returns date in string format
-    def __date():
-        curr_date = date.today()
-        day = curr_date.strftime("%d")
-        month = curr_date.strftime("%B")
-        year = curr_date.strftime("%Y")
-        return "Today is {} {}, {}".format(month, day, year)
-
     def run(self, incoming, methods, info, bot_info):
+
         try:
-            if info["command"] == "PRIVMSG" and info["args"][1] == ".date today":
-                methods["send"](info["address"], Plugin.__date())
+            # if '!~' in info['prefix']:
+            # print(info)
+            if info["command"] == "PRIVMSG" and info["args"][1] == ".hi":
+                methods["send"](info["address"], "hooo")
         except Exception as e:
             print("woops plug", e)
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/diary/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/diary/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [diary.py]
 Diary Plugin
 
 [Author]
 Angelo Giacco
 
@@ -86,15 +85,15 @@
             print([x.strip("\n") for x in entry])
             return [x.strip("\n") for x in entry]
 
     def delete(self, time):
         """check if entry exists and if it does delete it"""
         path = Plugin.get_path(self, time)
         if not os.path.exists(path):
-            return "There is no diary entry for that date. " "Check the date is entered correctly!"
+            return "There is no diary entry for that date. Check the date is entered correctly!"
         else:
             os.remove(path)
             return "Entry deleted successfully!"
 
     def run(self, incoming, methods, info, bot_info):
         try:
             owner = bot_info["owners"]
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/dictionary/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/dictionary/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [dictionary.py]
 Dictionary Plugin
 
 [Author]
 Nishant, JPMorgan Chase & Co.
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/duckduckgo/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/duckduckgo/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [duckduckgo.py]
 Duckduckgo Plugin
 
 [Author]
 Rakesh Seal
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/excuse/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/excuse/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [excuse.py]
 Random excuse Plugin
 
 [Author]
 Rakesh Seal
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/fact/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/fact/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [fact.py]
 Fact Plugin
 
 [Author]
 Justin Walker
 
@@ -35,16 +34,16 @@
 
 
 FACT_LIST = [
     "On Good Friday in 1930, the BBC reported, 'There is no news.' "
     + "Instead, they played piano music."
     "Amelia Earhart and Eleanor Roosevelt once sneaked out of a White"
     + "House event, commandeered an airplane, and went on a joyride to Baltimore."
-    "The 100 folds in a chef's toque are said to represent 100 ways " + "to cook an egg."
-    "The world’s oldest surviving piano is at the Metropolitan Museum of Art "
+    "The 100 folds in a chef's toque are said to represent 100 ways "
+    + "to cook an egg.The world’s oldest surviving piano is at the Metropolitan Museum of Art "
     + "in New York City. The instrument dates back to 1720, and was made by "
     + "an Italian man named Bartolomeo Cristofori."
     "The modern popped collar originated as a way to keep tennis players’"
     + "necks from getting sunburnt."
     "In 2006, an Australian man tried to sell New Zealand on Ebay. The "
     + "price reached $3,000 before it was shut down.",
     "Google's founders were willing to sell to excite for under $1 million"
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/google/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/google/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [googleSearch.py]
 Google Search Plugin
 
 [Author]
 Justin Walker
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/hangman/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/hangman/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [hangman.py]
 Hangman Game Plugin
 
 [Author]
 Justin Walker
 
@@ -148,15 +147,15 @@
             "hidden",
         ]
         randIndex = random.randint(0, len(self.wordChoices) - 1)
         self.gameWord = self.wordChoices[randIndex]
         print(self.gameWord)
         self.display = "-" * len(self.gameWord)
         self.guessCount = len(self.display) + 3
-        self.display_message = " You have {0} guesses remaining.".format(self.guessCount)
+        self.display_message = f" You have {self.guessCount} guesses remaining."
         self.endGame = False
         self.endMessage = "You shouldn't be able to see this."
 
     # guess_letter is used when user enters a single character guess.
 
     def guess_letter(self, guessLetter):
         # First find at which indeces the guessed letter is in the word.
@@ -187,31 +186,31 @@
     # guess_word is for when user tries to guess the complete word.
 
     def guess_word(self, wordGuess):
         if wordGuess.lower() == self.gameWord:
             self.display = self.gameWord
             self.check_win()
         else:
-            self.display_message = "'{0}' was incorrect. ".format(
-                wordGuess
-            ) + "You have {0} guesses remaining.".format(self.guessCount)
+            self.display_message = (
+                f"'{wordGuess}' was incorrect. " + f"You have {self.guessCount} guesses remaining."
+            )
 
     # check_win determines if the user has guessed the entire word after each
     # guess. If the user hasn't won, they lost one of their guesses.
 
     def check_win(self):
         win = True
         for letter in self.display:
             if letter == "-":
                 win = False
 
         if win is True:
-            self.display = "'{0}' is correct. You win!".format(self.gameWord)
+            self.display = f"'{self.gameWord}' is correct. You win!"
             self.display_message = (
-                " You had {0} guesses remaining.".format(self.guessCount)
+                f" You had {self.guessCount} guesses remaining."
                 + "\nUse 'start' command to try again."
             )
             self.endGame = True
             self.endMessage = self.display + self.display_message
         else:
             self.decrement_guesses()
 
@@ -219,20 +218,20 @@
     # count reaches 0.
 
     def decrement_guesses(self):
         self.guessCount -= 1
         if self.guessCount == 0:
             self.endMessage = (
                 "You have no more guesses.\n"
-                + "The correct word was '{0}'.\n".format(self.gameWord)
+                + f"The correct word was '{self.gameWord}'.\n"
                 + "You lose. Use start command to try again"
             )
             self.endGame = True
         else:
-            self.display_message = " You have {0} guesses remaining.".format(self.guessCount)
+            self.display_message = f" You have {self.guessCount} guesses remaining."
 
     # display_screen is to output what the user should see in the game's current
     # state.
 
     def display_screen(self):
         if self.endGame is False:
             return self.display + self.display_message
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/help/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/help/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [help.py]
 Help Plugin
 
 [Author]
 Eduardo Moraes de Mello, https://github.com/edumello
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/horoscope/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/horoscope/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [horoscope.py]
 Horoscope Plugin
 
 [Author]
 Angelo Giacco
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/installed_modules/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/installed_modules/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [installed_module.py]
 Installation checker
 
 [Author]
 Abdur-Rahmaan Janhangeer, pythonmembers.club
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/joke/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/joke/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [joke.py]
 Joke Plugin
 
 [Author]
 Abdur-Rahmaan Janhangeer, pythonmembers.club
 
@@ -18,24 +17,24 @@
 
 class Plugin:
     def __init__(self):
         pass
 
     def joke(self):
         jokes = [
-            "Why did the physics teacher break up with the biology teacher? There was no \
-    chemistry.",
-            "I asked my daughter if she’d seen my newspaper. She told me that newspapers \
-    are old school.She said that people use tablets nowadays and handed me her \
-    iPad. The fly didn’t stand a chance",
-            "A recent scientific study showed that out of 2,293,618,367 people, 94% are \
-    too lazy to actually read that number.",
+            "Why did the physics teacher break up with the biology teacher? There was no    "
+            " chemistry.",
+            "I asked my daughter if she’d seen my newspaper. She told me that newspapers     are"
+            " old school.She said that people use tablets nowadays and handed me her     iPad. The"
+            " fly didn’t stand a chance",
+            "A recent scientific study showed that out of 2,293,618,367 people, 94% are     too"
+            " lazy to actually read that number.",
             "Why is it a bad idea to insult an octopus? because it is well armed",
-            'Two cannibals are eating a clown, one looks to the other and asks "Does this \
-    taste funny to you?"',
+            'Two cannibals are eating a clown, one looks to the other and asks "Does this     taste'
+            ' funny to you?"',
             "What is red and smells like blue paint? Red Paint.",
             "How many South Americans does it take to change a lightbulb? A Brazilian!",
             "I have just invented a new word. Plagiarism.",
             "Why should you never trust an atom? Because they make up everything.",
             "What is brown and sticky? A stick!",
             "I tried to take a bite out of the fog, but I mist.",
             "What did the bodybuilder say when he ran out of protein powder? No whey.",
@@ -50,38 +49,38 @@
             "How many apples grow on a tree? All of them!",
             "Did you hear the rumor about the butter?" + " Well, I'm not going to spread it...",
             "How does a penguin build his home? Igloos it together!",
             "How to make a tissue dance? Put a little boogie in it!",
             "If you saw a robbery at the Apple store, would you be an iWitness?",
             "Why did the blind man turn down the job? He couldn't see himself doing it.",
             "Want to hear a joke about construction? We're still working on it.",
-            'As I handed my dad his 50th birthday card, he looked at me with tears in his \
-    eyes and said, "You know, one would have been enough."',
-            'I caught my wife yelling at the TV saying, "Don\'t go into the church you idiot!", \
-    She was watching our wedding video again.',
+            "As I handed my dad his 50th birthday card, he looked at me with tears in his     eyes"
+            ' and said, "You know, one would have been enough."',
+            'I caught my wife yelling at the TV saying, "Don\'t go into the church you idiot!",    '
+            " She was watching our wedding video again.",
             "When a woman is giving birth, she is literally kidding.",
             "My wife yelled at me agai for having no sense of direction."
             + " So I packed up my stuff and right.",
             'My son asked, "Can I have a book mark?" and I burst into tears.'
             + " 11 years old and he still doesn't know my name in Brian.",
             "If a child refuses to sleep during nap time,"
             + " are they guilty of resisting a rest?",
             "Geology rocks, but Geography is where it's at.",
             "Scientists were starting to get bored watching the Earth turn,"
             + " and so after 24 hours, they called it a day.",
-            "My wife yelled at me an said, \"You haven't listened to anything I've said!\", which \
-    I thought was an interesting way to start a conversation.",
+            "My wife yelled at me an said, \"You haven't listened to anything I've said!\", which  "
+            "   I thought was an interesting way to start a conversation.",
             "I’d tell you a Fibonacci joke, but’s it’s probably as bad"
             + " as the last two you’ve heard combined.",
             "What did the pirate say on his 80th birthday? AYE MATEY.",
             "It's hard to explain puns to kleptomaniacs"
             + " because they always take things literally.",
         ]
 
-        return "{}".format(random.choice(jokes))
+        return f"{random.choice(jokes)}"
 
     def run(self, incoming, methods, info, bot_info):
         try:
             # if '!~' in info['prefix']:
             # print(info)
             msgs = info["args"][1:]
             if info["command"] == "PRIVMSG" and msgs[0] == ".joke":
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/magic_ball/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/magic_ball/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [magic_ball.py]
 Magic 8 ball Plugin
 
 [Author]
 Zakaria Talhami
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/mail/info.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/mail/info.py`

 * *Files identical despite different names*

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/mail/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/mail/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [mail.py]
 Email plugin
 
 [Author]
 Tanner Fry
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/maths/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/maths/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [maths.py]
 Miscellaneous Maths Operations Plugin
 
 [Author]
 Abdur-Rahmaan Janhangeer, pythonmembers.club
 
@@ -36,37 +35,37 @@
             # print(info)
             msgs = info["args"][1:][0].split()
             if info["command"] == "PRIVMSG":
                 if len(msgs) > 1:
                     if msgs[0] == ".sin":
                         try:
                             sine = math.sin(float(msgs[1]))
-                            methods["send"](info["address"], "{}".format(sine))
+                            methods["send"](info["address"], f"{sine}")
                         except ValueError:
                             methods["send"](info["address"], ".sin must have numbers")
                     elif msgs[0] == ".cos":
                         try:
                             cosine = math.cos(float(msgs[1]))
-                            methods["send"](info["address"], "{}".format(cosine))
+                            methods["send"](info["address"], f"{cosine}")
                         except ValueError:
                             methods["send"](info["address"], ".cos must have numbers")
                     elif msgs[0] == ".tan":
                         try:
                             tangent = math.tan(float(msgs[1]))
-                            methods["send"](info["address"], "{}".format(tangent))
+                            methods["send"](info["address"], f"{tangent}")
                         except ValueError:
                             methods["send"](info["address"], ".tan must have numbers")
                     elif msgs[0] == ".rand":
                         try:
                             if int(msgs[1]) >= int(msgs[2]):
                                 methods["send"](
                                     info["address"],
                                     ".rand requires two integers that are not "
                                     "equal and the first must be biggest",
                                 )
                             else:
                                 rand = random.randint(int(msgs[1]), int(msgs[2]))
-                                methods["send"](info["address"], "{}".format(rand))
+                                methods["send"](info["address"], f"{rand}")
                         except ValueError:
                             methods["send"](info["address"], ".rand must have numbers")
         except Exception as e:
             print("\n*error*\nwoops plugin", __file__, e, "\n")
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/memo/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/memo/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [memo.py]
 Memory Use Illustration Plugin
 
 [Author]
 Abdur-Rahmaan Janhangeer, pythonmembers.club
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/monero/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/monero/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [monero.py]
 Monero Price Checking Plugin
 
 [Author]
 A. Eigenbrot
 
@@ -40,11 +39,11 @@
 
                 session = Session()
                 headers = {"Accepts": "application/json"}
                 session.headers.update(headers)
 
                 result = session.get(api_url, params=params)
                 data = json.loads(result.text)
-                methods["send"](info["address"], "{} {}".format(data[currency], currency))
+                methods["send"](info["address"], f"{data[currency]} {currency}")
 
         except Exception as e:
             print("woops! monero plugin error:", e)
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/monopoly/info.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/monopoly/info.py`

 * *Files identical despite different names*

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/monopoly/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/monopoly/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [monopoly.py]
 Monopoly Plugin
 [Author]
 Angelo Giacco
 [About]
 Play monopoly
@@ -923,15 +922,15 @@
 
     def start(methods, info):
         """start the game and shuffle decks"""
         if Plugin.start_join_req:
             random.shuffle(Plugin.players)
             methods["send"](
                 info["address"],
-                "The monopoly game has started, " "player order has been randomly generated:",
+                "The monopoly game has started, player order has been randomly generated:",
             )
             for player in Plugin.players:
                 name = player.getName()
                 methods["send"](info["address"], name)
             Plugin.get_info(methods, info)
             Plugin.turn = 0
             Plugin.stage = 1
@@ -1002,16 +1001,15 @@
                             # buy a house option
                             if isinstance(new_location, monopoly_assets.Property):
                                 Plugin.offer_house(methods, info, player, new_location)
                             else:
                                 methods["send"](
                                     info["address"],
                                     "You have landed on your own property "
-                                    + "but you cannot buy houses "
-                                    "for railroads or utilities",
+                                    + "but you cannot buy houses for railroads or utilities",
                                 )
                                 Plugin.next_turn()
 
                         else:
                             rent = Plugin.get_rent(new_location, owner, move_amount)
                             methods["send"](
                                 info["address"],
@@ -1096,16 +1094,15 @@
                             # buy a house option
                             if isinstance(new_location, monopoly_assets.Property):
                                 Plugin.offer_house(methods, info, player, new_location)
                             else:
                                 methods["send"](
                                     info["address"],
                                     "You have landed on your own property "
-                                    + "but you cannot buy houses "
-                                    "for railroads or utilities",
+                                    + "but you cannot buy houses for railroads or utilities",
                                 )
                                 Plugin.next_turn()
                         else:
                             rent = Plugin.get_rent(new_location, owner, move_amount)
                             methods["send"](
                                 info["address"],
                                 player.getName()
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/monopoly/monopoly_assets/monopoly_assets.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/monopoly/monopoly_assets/monopoly_assets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Game Objects
-class Space(object):
+class Space:
     def __init__(self, name):
         self.name = name
 
     def get_name(self):
         return self.name
 
 
@@ -28,15 +28,15 @@
         one_house_rent,
         two_house_rent,
         three_house_rent,
         four_house_rent,
         hotel_rent,
         house_cost,
     ):
-        super(Property, self).__init__(name)
+        super().__init__(name)
         self.price = price
         self.color = color
         self.house_count = 0  # 5 means hotel
         self.rents = {
             0: rent,
             1: one_house_rent,
             2: two_house_rent,
@@ -62,15 +62,15 @@
             "A house costs " + str(self.house_cost) + " to build.",
         ]
         return " ".join(information)
 
 
 class Railroad(Space):
     def __init__(self, name):
-        super(Railroad, self).__init__(name)
+        super().__init__(name)
         self.price = 200
         self.rents = {1: 25, 2: 50, 3: 100, 4: 200}
 
     def info(self):
         information = [
             self.name + " is a railroad that costs " + str(self.price) + ".",
             "If a player has one railroad only the rent is " + str(self.rents[1]) + ".",
@@ -79,15 +79,15 @@
             "If a player has four railroads only the rent is " + str(self.rents[4]) + ".",
         ]
         return " ".join(information)
 
 
 class Utility(Space):
     def __init__(self, name):
-        super(Utility, self).__init__(name)
+        super().__init__(name)
         self.price = 150
         self.rents = {1: "4 *", 2: "10 *"}
 
     def info(self):
         return (
             self.name
             + " is a utility that costs "
@@ -153,49 +153,45 @@
         "Take a walk on the board walk, advance token to board walk": [
             2,
             (board_spaces[39],),
         ]
     },
     {"Advance to go, collect $200": [3, ()]},
     {
-        "Advance token to the nearest Railroad and pay owner Twice the Rental owed."
-        " If Railroad is unowned you may buy it from the bank": [
+        "Advance token to the nearest Railroad and pay owner Twice the Rental owed. If Railroad is unowned you may buy it from the bank": [
             4,
             (),
         ]
     },
     {
-        "Advance token to the nearest Railroad and pay owner Twice the Rental owed."
-        " If Railroad is unowned you may buy it from the bank": [
+        "Advance token to the nearest Railroad and pay owner Twice the Rental owed. If Railroad is unowned you may buy it from the bank": [
             4,
             (),
         ]
     },
     {"Get out of jail free. This card may be kept until needed or sold": [5, ()]},
     {"Go directly to jail. Do not pass Go, do not collect $200": [6, ()]},
     {"Bank pays you dividend of $50": [7, (50,)]},
     {"Advance to Illinois Ave": [2, (board_spaces[24],)]},
     {"Pay poor tax of $15": [8, (15,)]},
     {
-        "Make general repairs on all your property. "
-        "For each house pay $25, for each hotel $100": [
+        "Make general repairs on all your property. For each house pay $25, for each hotel $100": [
             9,
             (25, 100),
         ]
     },
     {
         "Advance to St. Charles Place. If you pass Go, collect $200": [
             2,
             (board_spaces[11],),
         ]
     },
     {"Your building and loan matures. Collect $150": [7, (150,)]},
     {
-        "Advance token to nearest utility. If Unowned you may buy it from the bank. "
-        "If owned throw dice and pay owner ten times the amount thrown.": [
+        "Advance token to nearest utility. If Unowned you may buy it from the bank. If owned throw dice and pay owner ten times the amount thrown.": [
             10,
             (),
         ]
     },
     {"Go back 3 spaces": [11, ()]},
 ]
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/monopoly/monopoly_assets/monopoly_player.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/monopoly/monopoly_assets/monopoly_player.py`

 * *Files identical despite different names*

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/news/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/news/main.py`

 * *Files identical despite different names*

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/onthisday/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/onthisday/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [onthisday.py]
 On This Day
 [Author]
 Kenneth Gargan
 [About]
 Gets an interesting fact about today!
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/password_generator/info.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/password_generator/info.py`

 * *Files identical despite different names*

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/password_generator/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/password_generator/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [password_generator.py]
 Password Generator Plugin
 
 [Author]
 Nishant, JPMorgan Chase & Co.
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/proverb/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/proverb/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [proverb.py]
 Proverb Plugin
 
 [Author]
 Sushant Kumar
 
@@ -41,15 +40,15 @@
             "Charity begins at home",
             "The dog that bites does not bark",
             "A snake may shed its skin, but it's still a snake",
             "Until the rotten tooth is pulled out, the mouth must chew with caution",
             "Todays flat tits were yesterdays pointed ones",
         ]
 
-        return "{}".format(random.choice(proverbs))
+        return f"{random.choice(proverbs)}"
 
     def run(self, incoming, methods, info, bot_info):
         try:
             # if '!~' in info['prefix']:
             # print(info)
             msgs = info["args"][1:]
             if info["command"] == "PRIVMSG" and msgs[0] == ".proverb":
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/pynews/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/pynews/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [pynews.py]
 Python news checking plugin
 
 [Author]
 Sam Deans
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/pypi/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/pypi/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [pypi.py]
 Pypi Search Plugin
 [Author]
 Donald Lieu
 [About]
 Searches for Python packages on pypi.org
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/quote/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/quote/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [quote.py]
 Quotes Plugin
 
 [Author]
 German Corpaz
 
@@ -81,15 +80,15 @@
             "Change your thoughts and you change your world.",
             "Education is the most powerful weapon which " + "you can use to change the world.",
             "Today you are you! That is truer than true! "
             + "There is no one alive who is you-er than you!",
             "The future belongs to those who believe in the beauty of their dreams.",
         ]
 
-        return "{}".format(random.choice(quotes))
+        return f"{random.choice(quotes)}"
 
     def run(self, incoming, methods, info, bot_info):
         try:
             msgs = info["args"][1:]
             if info["command"] == "PRIVMSG" and msgs[0] == ".quote":
                 methods["send"](info["address"], Plugin.quote(self))
         except Exception as e:
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/random_color/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/random_color/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [random_color.py]
 Random Color Plugin
 
 [Author]
 Jeet Trivedi
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/random_image/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/random_image/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [random_image.py]
 Random Image Plugin
 
 [Author]
 Rakesh Seal
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/repostats/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/repostats/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [repostats.py]
 Repostats Plugin
 
 [Author]
 Shreyansh Sancheti
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/riddle/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/riddle/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [riddle.py]
 Riddle Plugin
 
 [Author]
 Angelo Giacco
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/roll/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/roll/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [roll.py]
 Dice_Roll Plugin
 
 [Author]
 Glenn Toms
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/roman_numeral/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/roman_numeral/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [roman_numeral.py]
 Roman Numeral Converter Plugin
 
 [Author]
 Nick Wiley
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/russian_roulette/info.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/russian_roulette/info.py`

 * *Files identical despite different names*

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/russian_roulette/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/russian_roulette/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [russian_roulette.py]
 Russian Roulette Plugin
 
 [Author]
 Angelo Giacco
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/selfTrivia/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/selfTrivia/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [quote.py]
 Self Trivia Plugin
 
 [Author]
 Angel Jimenez
 
@@ -114,15 +113,15 @@
             "Is a dolphin a mammal?",  # Yes.
             "What do many children ride on to go to school?",  # A school bus.
             "Thirsty people need?",  # Water.
             "What do you wear on your head?",  # Hat.
             "Who painted the Mona Lisa?",  # Leonardo da Vinci.
         ]
 
-        return "{}".format(random.choice(questions))
+        return f"{random.choice(questions)}"
 
     def run(self, incoming, methods, info, bot_info):
         try:
             msgs = info["args"][1:]
             if info["command"] == "PRIVMSG" and msgs[0] == ".selfTrivia":
                 methods["send"](info["address"], Plugin.trivia(self))
         except Exception as e:
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/send_message/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/send_message/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [send_message.py]
 Send Message Plugin
 
 [Author]
 Justin Walker
 
@@ -42,15 +41,15 @@
                     message = Plugin.send_general_message(msgs, sender, sender_channel)
                     methods["send"](channel_destination, message)
                 # Checks for specific message type
                 elif len(msgs) >= 6 and msgs[2] == ".u" and msgs[4] == ".m":
                     recipient = msgs[3]
 
                     # Sends whois to server to determine online status
-                    methods["send_raw"]("whois {0} \r\n".format(recipient))
+                    methods["send_raw"](f"whois {recipient} \r\n")
 
                     # Recieves message back from server and converts to be
                     # usable.
                     data = self.irc.recv(2048)
                     raw_msg = data.decode("UTF-8")
                     msg = raw_msg.strip("\n\r")
 
@@ -71,18 +70,18 @@
         except Exception as e:
             print("woops plugin error: ", e)
 
     def send_general_message(msgs, sender, sender_channel):
         message = ""
         for word in msgs[2:]:
             message += word + " "
-        complete_message = "{0} from {1} says: {2}".format(sender, sender_channel, message.rstrip())
+        complete_message = f"{sender} from {sender_channel} says: {message.rstrip()}"
         return complete_message
 
     def send_specific_message(msgs, recipient, sender, sender_channel):
         message = ""
         for word in msgs[5:]:
             message += word + " "
-        complete_message = "{0} from {1} says to {2}: {3}".format(
+        complete_message = "{} from {} says to {}: {}".format(
             sender, sender_channel, recipient, message.rstrip()
         )
         return complete_message
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/story/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/story/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [story.py]
 Story Plugin
 
 [Author]
 Tuan Thai
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/sysinfo/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/sysinfo/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [sysinfo.py]
 System Information Plugin.
 
 [Author]
 Girish Mahabir
 
@@ -65,31 +64,29 @@
                 # Data and Time computer was booted.
                 # Boot Time.
                 methods["send"](info["address"], "=" * 40 + "Boot Time" + "=" * 40)
                 boot_time_timestamp = psutil.boot_time()
                 bt = datetime.fromtimestamp(boot_time_timestamp)
                 methods["send"](
                     info["address"],
-                    f"Boot Time: "
-                    f"{bt.year}/{bt.month}/{bt.day} "
-                    f"{bt.hour}:{bt.minute}:{bt.second}",
+                    f"Boot Time: {bt.year}/{bt.month}/{bt.day} {bt.hour}:{bt.minute}:{bt.second}",
                 )
 
             if info["command"] == "PRIVMSG" and info["args"][1] == ".cpuinfo":
                 # CPU Information.
                 # Let's Print, CPU information.
                 methods["send"](info["address"], "=" * 40 + "CPU Info" + "=" * 40)
                 # Number of cores.
                 methods["send"](
                     info["address"],
-                    "Physical cores: {}".format(psutil.cpu_count(logical=False)),
+                    f"Physical cores: {psutil.cpu_count(logical=False)}",
                 )
                 methods["send"](
                     info["address"],
-                    "Total cores: {}".format(psutil.cpu_count(logical=True)),
+                    f"Total cores: {psutil.cpu_count(logical=True)}",
                 )
                 # CPU frequencies.
                 cpufreq = psutil.cpu_freq()
                 methods["send"](info["address"], f"Max Frequency: {cpufreq.max:.2f}Mhz")
                 methods["send"](info["address"], f"Min Frequency: {cpufreq.min:.2f}Mhz")
                 methods["send"](info["address"], f"Current Frequency: {cpufreq.current:.2f}Mhz")
                 # CPU usage.
@@ -129,23 +126,22 @@
                                 info["address"],
                                 f"IP Address: {address.address}  ||  "
                                 f"Netmask: {address.netmask}".format(),
                             )
                         elif str(address.family) == "AddressFamily.AF_PACKET":
                             methods["send"](
                                 info["address"],
-                                f"MAC Address: {address.address}"
-                                f" ||  Netmask: {address.netmask}",
+                                f"MAC Address: {address.address} ||  Netmask: {address.netmask}",
                             )
                 # Get IO statistics since boot.
                 net_io = psutil.net_io_counters()
                 methods["send"](
                     info["address"],
                     f"Total Bytes Sent: {self.get_size(net_io.bytes_sent)}"
-                    f" ||  Total Bytes Received: "
+                    " ||  Total Bytes Received: "
                     f"{self.get_size(net_io.bytes_recv)}",
                 )
 
             if info["command"] == "PRIVMSG" and info["args"][1] == ".diskinfo":
                 # Disk Information
                 methods["send"](
                     info["address"],
@@ -164,15 +160,15 @@
                         partition_usage = psutil.disk_usage(partition.mountpoint)
                     except PermissionError:
                         # This can be catch due to disks that
                         # isn't ready.
                         continue
                     methods["send"](
                         info["address"],
-                        f"  Total Size: "
+                        "  Total Size: "
                         f"{self.get_size(partition_usage.total)}\n  "
                         f"Used: {self.get_size(partition_usage.used)}\n  "
                         f"Free: {self.get_size(partition_usage.free)}\n  "
                         f"Percentage: {partition_usage.percent}%",
                     )
                 # Get IO statistics since boot.
                 disk_io = psutil.disk_io_counters()
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/telephone_code/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/telephone_code/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [countries.py]
 Country-Code Plugin
 
 [Author]
 Sarvesh Dubey
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/todo/info.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/todo/info.py`

 * *Files identical despite different names*

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/todo/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/todo/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [todo.py]
 Todo list Plugin
 
 [Author]
 Himanshu Ranjan
 
@@ -44,50 +43,46 @@
     def __init__(self):
         pass
 
     def get_help(info, methods):
         """help function to give information about commands."""
         methods["send"](
             info["address"],
-            ".todo add  <Your Task Here> \
-            (It adds the task to do the todo list.)",
+            ".todo add  <Your Task Here>             (It adds the task to do the todo list.)",
         )
         methods["send"](
             info["address"],
-            ".todo delete  <index> \
-            (To delete a task input it's index number as shown in the list.)",
+            ".todo delete  <index>             (To delete a task input it's index number as shown"
+            " in the list.)",
         )
         methods["send"](
             info["address"],
-            ".todo show \
-            (It shows all the task currently on the list.)",
+            ".todo show             (It shows all the task currently on the list.)",
         )
         methods["send"](
             info["address"],
-            ".todo clear \
-            (This will delete all the task in the list.)",
+            ".todo clear             (This will delete all the task in the list.)",
         )
         methods["send"](
             info["address"],
-            ".todo help \
-            (sends messages explaining how to use the todo plugin.)",
+            ".todo help             (sends messages explaining how to use the todo plugin.)",
         )
 
     def showlist(info, methods):
         """It prints the todo file on the screen"""
         # Parse the user ID from info['prefix']
         raw_user = info["prefix"]
         user_index = raw_user.find("!")
         user = raw_user[0:user_index]
 
         if os.stat("todo.txt").st_size == 0:
             methods["send"](info["address"], "Awesome " + user + ". You Have No Task Pending!")
         else:
             methods["send"](info["address"], "Hi, " + user + ". These are your tasks.")
-            with open("todo.txt", "r") as f:
+            with open("todo.txt") as f:
                 lines = f.readlines()
             count = 1
             for line in lines:
                 methods["send"](info["address"], str(count) + ". " + line)
                 count = count + 1
 
     def run(self, incoming, methods, info, bot_info):
@@ -107,15 +102,15 @@
                         todo.write(task.rstrip("\n") + "\n" + content)
                     Plugin.showlist(info, methods)
 
                 # deleting the line of given index
                 elif msgs[1] == "delete":
                     line_no = int(msgs[2])
 
-                    with open("todo.txt", "r") as f:
+                    with open("todo.txt") as f:
                         lines = f.readlines()
 
                     count = 1
                     with open("todo.txt", "w") as f:
                         for line in lines:
                             if count != line_no:
                                 f.write(line)
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/tpbquote/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/tpbquote/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [Quote.py]
 Quote Plugin
 
 [Author]
 Divyanshu Mehta
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/transfer-rumour/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/transfer-rumour/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [transfer-rumour.py]
 Transfer Rumour Plugin
 
 [Author]
 Angelo Giacco
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/translate/info.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/translate/info.py`

 * *Files identical despite different names*

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/translate/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/translate/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 """
 [translate.py]
 Translate Plugin
 
 [Author]
 Ahmed Deeb
 
@@ -183,22 +181,22 @@
     retval = f.read()
     f.close()
     return retval
 
 
 class ZipCache(FileCache):
     def __init__(self, cache=".cache"):  # TODO: allow user configurable?
-        super(ZipCache, self).__init__(cache)
+        super().__init__(cache)
 
     def get(self, key):
         cacheFullPath = os.path.join(self.cache, self.safe(key))
         retval = None
         try:
             retval = load_cached_key(cacheFullPath)
-        except IOError:
+        except OSError:
             pass
         return retval
 
     def set(self, key, value):
         retval = None
         cacheFullPath = os.path.join(self.cache, self.safe(key))
         save_cached_key(cacheFullPath, value)
@@ -225,15 +223,15 @@
         result.status = code
         return result
 
 
 # Translator Class #
 
 
-class Plugin(object):
+class Plugin:
     """
     Google Translator object.
 
     Examples
     --------
     translator = Plugin()
 
@@ -264,17 +262,17 @@
         """
         params = "&".join(map("=".join, params))
         return params
 
     def _build_uri(self, extra_url, params):
         params = [("key", api)] + params
         params = self._urlencode(params)
-        url = "%s?%s" % (urlparse.urljoin(self.base_url, extra_url), params)
+        url = f"{urlparse.urljoin(self.base_url, extra_url)}?{params}"
         if len(url) > 2000:  # for GET requests only, POST is 5K
-            raise ValueError("Query is too long. URL can only be 2000 " "characters")
+            raise ValueError("Query is too long. URL can only be 2000 characters")
         return url
 
     def _fetch_data(self, url):
         connection = self.connection
         resp, content = connection.request(
             url, headers={"user-agent": api, "cache-control": self.cache_control}
         )
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/url_shorten/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/url_shorten/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [url_shorten.py]
 URL Shortener Plugin
 
 [Author]
 Rakesh Seal
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/username/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/username/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [username.py]
 Username Generator Plugin
 
 [Author]
 Abdur-Rahmaan Janhangeer, pythonmembers.club
 
@@ -29,15 +28,15 @@
             "hopeful",
             "young",
             "sloppy",
             "magic",
             "intelligent",
             "uncommon",
             "cute",
-            "dangerous" "innocent",
+            "dangerousinnocent",
             "spooky",
             "crazy",
             "young",
             "desperate",
             "epic",
             "anonymous",
             "acceptable",
@@ -173,15 +172,15 @@
             "tree",
             "ant",
             "spider",
             "moon",
             "bug",
             "name",
             "heisenberg",
-            "dragon" "snake",
+            "dragonsnake",
             "lion",
             "rebel",
             "patriot",
             "flower",
             "popsicle",
             "sun",
             "failure",
@@ -273,15 +272,15 @@
             "vest",
             "water",
             "wing",
             "winter",
             "woman",
             "women",
         ]
-        return "{}{}".format(random.choice(p1), random.choice(p2))
+        return f"{random.choice(p1)}{random.choice(p2)}"
 
     def run(self, incoming, methods, info, bot_info):
         try:
             # if '!~' in info['prefix']:
             # print(info)
             msgs = info["args"][1:]
             if info["command"] == "PRIVMSG" and msgs[0] == ".uname":
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/weather/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/weather/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [weather.py]
 Weather Plugin
 
 [Author]
 Gabriele Ron
 
@@ -23,17 +22,17 @@
 
     def run(self, incoming, methods, info, bot_info):
         try:
             msgs = info["args"][1:][0].split()
 
             if info["command"] == "PRIVMSG" and msgs[0] == ".weather":
                 api_url = (
-                    f"https://api.openweathermap.org/data/2.5/weather?"
+                    "https://api.openweathermap.org/data/2.5/weather?"
                     f"q={msgs[1]},{msgs[2]}"
-                    f"&APPID=8801bc666d30a8cc9294feaf60c01117&units=metric"
+                    "&APPID=8801bc666d30a8cc9294feaf60c01117&units=metric"
                 )
                 response = requests.get(api_url)
                 response_json = response.json()
 
                 weather = (
                     f"The weather for {response_json['name']} is "
                     f"{response_json['weather'][0]['description']} at "
```

### Comparing `honeybot-6.0.2/src/honeybot/plugins/downloaded/wikipedia/main.py` & `honeybot-6.1.0/src/honeybot/plugins/downloaded/wikipedia/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 [wikipedia.py]
 Wikipedia Plugin
 
 [Author]
 Gabriele Ron
```

### Comparing `honeybot-6.0.2/src/honeybot/settings/email_config.conf` & `honeybot-6.1.0/src/honeybot/settings/email_config.conf`

 * *Files identical despite different names*

### Comparing `honeybot-6.0.2/src/honeybot/store.py` & `honeybot-6.1.0/src/honeybot/store.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import importlib
 import json
 import os
 
 BASE_DIR = "plugins/downloaded"
-STORE_DIR = "../../honeybot-store"
+STORE_DIR = "../../honeybot-store"  # ...
 
 plugins = {"plugins": []}
 dirs = [d for d in os.listdir(BASE_DIR) if not d.startswith("__")]
 
 
 def pinfo(folder, attrib):
     try:
-        mod = importlib.import_module("plugins.downloaded.{}.info".format(folder))
+        mod = importlib.import_module(f"plugins.downloaded.{folder}.info")
         return getattr(mod, attrib)
     except Exception as e:
         if attrib == "ORIGINAL_AUTHORS":
             return []
         else:
             return ""
```

### Comparing `honeybot-6.0.2/src/honeybot/test_core.py` & `honeybot-6.1.0/src/honeybot/test_core.py`

 * *Files identical despite different names*

### Comparing `honeybot-6.0.2/src/honeybot/test_legacy_core.py` & `honeybot-6.1.0/src/honeybot/test_legacy_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,18 @@
 'args': ['##bottestingmu', 'ef']
 }
 """
 config = configparser.ConfigParser()
 config.read("settings/CONNECT.conf")
 
 # incoming
-incoming = ":appinv!c5e342c5@gateway/web/cgi-irc/kiwiirc.com/ip.200.200.22.200 \
-        PRIVMSG ##bottestingmu :ef"
+incoming = (
+    ":appinv!c5e342c5@gateway/web/cgi-irc/kiwiirc.com/ip.200.200.22.200         PRIVMSG"
+    " ##bottestingmu :ef"
+)
 bot = Bot()
 
 
 class HoneybotTests(unittest.TestCase):
     """
     basic info
     """
@@ -39,16 +41,15 @@
     """
     info function
     """
 
     def test_info_prefix(self):
         self.assertEqual(
             bot.info(incoming)["prefix"],
-            "appinv!c5e342c5@gateway/web/cgi-irc/kiwiirc.com/\
-                    ip.200.200.22.200",
+            "appinv!c5e342c5@gateway/web/cgi-irc/kiwiirc.com/                    ip.200.200.22.200",
         )
 
     def test_info_command(self):
         self.assertEqual(bot.info(incoming)["command"], "PRIVMSG")
 
     def test_info_address(self):
         self.assertEqual(bot.info(incoming)["address"], "##bottestingmu")
@@ -57,15 +58,15 @@
         self.assertEqual(bot.info(incoming)["args"], ["##bottestingmu", "ef"])
 
     """
     commands
     """
 
     def test_set_nick_command(self):
-        self.assertEqual(bot.set_nick_command(), "NICK {0}\r\n".format(config["INFO"]["name"]))
+        self.assertEqual(bot.set_nick_command(), "NICK {}\r\n".format(config["INFO"]["name"]))
 
     def test_present_command(self):
         self.assertEqual(
             bot.present_command(),
             "USER {0} {0} {0} : {0} IRC\r\n".format(config["INFO"]["name"]),
         )
```

### Comparing `honeybot-6.0.2/src/honeybot/test_plugin_script.py` & `honeybot-6.1.0/src/honeybot/test_plugin_script.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-# -*- coding: utf-8 -*-
 """ Change to your plugin file name below.
                     ↓↓↓↓  """
 import time
 
-from plugins import roman_numeral as test_plugin
+from plugins import basketball as test_plugin
 
 test_plugin = test_plugin.Plugin
 
 
 class Tester:
     def __init__(self, test_type, command):
 
@@ -24,22 +23,25 @@
             "prefix": "TestAccount!~TestIdentity@192.168.123.123",
         }
         bot_info = {"time": time.time() - 12561}
         # time.sleep(5)
 
         # Update info with MOCK data.
         if test_type == "message":
-            incoming = f":TestAccount!~TestIdentity@192.168.123.123 \
-                PRIVMSG ##TestChannel :{command}"
+            incoming = (
+                ":TestAccount!~TestIdentity@192.168.123.123                 PRIVMSG ##TestChannel"
+                f" :{command}"
+            )
             info["command"] = "PRIVMSG"
             info["args"] = [0, command]
 
         if test_type == "user_join":
-            incoming = ":TestAccount!~TestIdentity@192.168.123.123 \
-                JOIN ##TestChannel"
+            incoming = (
+                ":TestAccount!~TestIdentity@192.168.123.123                 JOIN ##TestChannel"
+            )
             info["command"] = "JOIN"
 
         if test_type == "user_quit":
             incoming = ":TestAccount!~TestIdentity@192.168.123.123 QUIT :"
             info["command"] = "QUIT"
 
         # Run plugin with above details
@@ -65,12 +67,12 @@
             3.1 Uses command as if a user was testing sending a message.
         4. join
             4.1 User joining a channel
         4. quit
             4.1 User quitting a channel
     """
 
-    incoming_command_test = ".roman 420"
+    incoming_command_test = ".basketball eu all"
 
     Tester("message", incoming_command_test)
     # Tester('user_join', incoming_command_test)
     # Tester('user_quit', incoming_command_test)
```

### Comparing `honeybot-6.0.2/src/honeybot.egg-info/SOURCES.txt` & `honeybot-6.1.0/src/honeybot.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 src/honeybot/test_plugin_script.py
 src/honeybot/todo.txt
 src/honeybot.egg-info/PKG-INFO
 src/honeybot.egg-info/SOURCES.txt
 src/honeybot.egg-info/dependency_links.txt
 src/honeybot.egg-info/entry_points.txt
 src/honeybot.egg-info/not-zip-safe
+src/honeybot.egg-info/requires.txt
 src/honeybot.egg-info/top_level.txt
 src/honeybot/api/__init__.py
 src/honeybot/api/commands.py
 src/honeybot/api/generate.py
 src/honeybot/api/init.py
 src/honeybot/api/main.py
 src/honeybot/api/memory.py
@@ -38,14 +39,20 @@
 src/honeybot/plugins/downloaded/__init__.py
 src/honeybot/plugins/downloaded/abbreviation/__init__.py
 src/honeybot/plugins/downloaded/abbreviation/info.py
 src/honeybot/plugins/downloaded/abbreviation/main.py
 src/honeybot/plugins/downloaded/age/__init__.py
 src/honeybot/plugins/downloaded/age/info.py
 src/honeybot/plugins/downloaded/age/main.py
+src/honeybot/plugins/downloaded/basketball/__init__.py
+src/honeybot/plugins/downloaded/basketball/info.py
+src/honeybot/plugins/downloaded/basketball/main.py
+src/honeybot/plugins/downloaded/birthparadox/__init__.py
+src/honeybot/plugins/downloaded/birthparadox/info.py
+src/honeybot/plugins/downloaded/birthparadox/main.py
 src/honeybot/plugins/downloaded/bitcoin/__init__.py
 src/honeybot/plugins/downloaded/bitcoin/info.py
 src/honeybot/plugins/downloaded/bitcoin/main.py
 src/honeybot/plugins/downloaded/blackjack/__init__.py
 src/honeybot/plugins/downloaded/blackjack/info.py
 src/honeybot/plugins/downloaded/blackjack/main.py
 src/honeybot/plugins/downloaded/blackjack/poker_assets/__init__.py
@@ -102,14 +109,17 @@
 src/honeybot/plugins/downloaded/diary/main.py
 src/honeybot/plugins/downloaded/dictionary/__init__.py
 src/honeybot/plugins/downloaded/dictionary/info.py
 src/honeybot/plugins/downloaded/dictionary/main.py
 src/honeybot/plugins/downloaded/duckduckgo/__init__.py
 src/honeybot/plugins/downloaded/duckduckgo/info.py
 src/honeybot/plugins/downloaded/duckduckgo/main.py
+src/honeybot/plugins/downloaded/emoji/__init__.py
+src/honeybot/plugins/downloaded/emoji/info.py
+src/honeybot/plugins/downloaded/emoji/main.py
 src/honeybot/plugins/downloaded/excuse/__init__.py
 src/honeybot/plugins/downloaded/excuse/info.py
 src/honeybot/plugins/downloaded/excuse/main.py
 src/honeybot/plugins/downloaded/fact/__init__.py
 src/honeybot/plugins/downloaded/fact/info.py
 src/honeybot/plugins/downloaded/fact/main.py
 src/honeybot/plugins/downloaded/google/__init__.py
@@ -150,14 +160,17 @@
 src/honeybot/plugins/downloaded/monero/main.py
 src/honeybot/plugins/downloaded/monopoly/__init__.py
 src/honeybot/plugins/downloaded/monopoly/info.py
 src/honeybot/plugins/downloaded/monopoly/main.py
 src/honeybot/plugins/downloaded/monopoly/monopoly_assets/__init__.py
 src/honeybot/plugins/downloaded/monopoly/monopoly_assets/monopoly_assets.py
 src/honeybot/plugins/downloaded/monopoly/monopoly_assets/monopoly_player.py
+src/honeybot/plugins/downloaded/movies_imdb/__init__.py
+src/honeybot/plugins/downloaded/movies_imdb/info.py
+src/honeybot/plugins/downloaded/movies_imdb/main.py
 src/honeybot/plugins/downloaded/news/__init__.py
 src/honeybot/plugins/downloaded/news/info.py
 src/honeybot/plugins/downloaded/news/main.py
 src/honeybot/plugins/downloaded/onthisday/__init__.py
 src/honeybot/plugins/downloaded/onthisday/info.py
 src/honeybot/plugins/downloaded/onthisday/main.py
 src/honeybot/plugins/downloaded/password_generator/__init__.py
```

