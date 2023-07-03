# Comparing `tmp/livestyled-1.4.4.tar.gz` & `tmp/livestyled-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livestyled-1.4.4.tar", last modified: Mon Jul  3 15:42:48 2023, max compression
+gzip compressed data, was "livestyled-1.4.5.tar", last modified: Mon Jul  3 16:05:19 2023, max compression
```

## Comparing `livestyled-1.4.4.tar` & `livestyled-1.4.5.tar`

### file list

```diff
@@ -1,147 +1,147 @@
-drwxr-xr-x   0 tomrutherford   (501) staff       (20)        0 2023-07-03 15:42:48.614172 livestyled-1.4.4/
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1067 2022-11-28 12:03:16.000000 livestyled-1.4.4/LICENSE
--rw-r--r--   0 tomrutherford   (501) staff       (20)      110 2022-11-28 12:03:16.000000 livestyled-1.4.4/MANIFEST.in
--rw-r--r--   0 tomrutherford   (501) staff       (20)      242 2023-07-03 15:42:48.613294 livestyled-1.4.4/PKG-INFO
--rw-r--r--   0 tomrutherford   (501) staff       (20)      268 2022-11-28 12:03:16.000000 livestyled-1.4.4/README.md
-drwxr-xr-x   0 tomrutherford   (501) staff       (20)        0 2023-07-03 15:42:47.269645 livestyled-1.4.4/livestyled/
--rw-r--r--   0 tomrutherford   (501) staff       (20)       22 2023-07-03 15:42:35.000000 livestyled-1.4.4/livestyled/__init__.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)    11599 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/client.py
-drwxr-xr-x   0 tomrutherford   (501) staff       (20)        0 2023-07-03 15:42:47.798682 livestyled-1.4.4/livestyled/models/
--rw-r--r--   0 tomrutherford   (501) staff       (20)     3790 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/models/__init__.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1166 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/models/app.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1440 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/models/audience.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1018 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/models/audience_device.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2497 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/models/banner.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2578 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/models/booking.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1140 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/models/cohort.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1306 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/models/competition.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1975 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/models/device.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      680 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/models/device_consent.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1924 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/models/device_form_data.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2371 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/models/device_preference.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      408 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/models/device_push_consent.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2093 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/models/device_reality.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1557 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/models/device_token.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2284 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/models/event.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)       30 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/models/event_category.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      657 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/models/event_date.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)       27 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/models/event_stage.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     5870 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/models/fixture.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     4573 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/models/form.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2913 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/models/form_field.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     7288 2023-01-03 11:39:18.000000 livestyled-1.4.4/livestyled/models/fulfilment_point.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     4768 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/models/league_table.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1542 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/models/location.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1358 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/models/magic_field.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1654 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/models/news.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     5358 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/models/order.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)    14632 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/models/payment.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)    16830 2023-01-12 13:18:11.000000 livestyled-1.4.4/livestyled/models/product.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2475 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/models/push_broadcast.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1682 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/models/push_consent.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2894 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/models/reality.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1875 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/models/screen.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1119 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/models/season.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      654 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/models/sport_venue.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1155 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/models/storage.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1548 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/models/team.py
-drwxr-xr-x   0 tomrutherford   (501) staff       (20)        0 2023-07-03 15:42:47.859617 livestyled-1.4.4/livestyled/models/tests/
--rw-r--r--   0 tomrutherford   (501) staff       (20)        0 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/models/tests/__init__.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1111 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/models/tests/test_device_form_data.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1876 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/models/tests/test_fixture.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     3335 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/models/tests/test_form.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2548 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/models/tests/test_form_field.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      447 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/models/tests/test_order.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      455 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/models/tests/test_team.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     5022 2023-07-03 15:42:35.000000 livestyled-1.4.4/livestyled/models/tests/test_ticket.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)    13936 2023-07-03 15:42:35.000000 livestyled-1.4.4/livestyled/models/ticket.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2908 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/models/ticket_auth.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2365 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/models/ticket_integration.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     8877 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/models/user.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      526 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/models/user_cohort.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     4162 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/models/venue.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     3676 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/models/widget.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)    48299 2022-11-28 16:23:37.000000 livestyled-1.4.4/livestyled/resource_client.py
-drwxr-xr-x   0 tomrutherford   (501) staff       (20)        0 2023-07-03 15:42:48.359105 livestyled-1.4.4/livestyled/schemas/
--rw-r--r--   0 tomrutherford   (501) staff       (20)     4518 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/schemas/__init__.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1809 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/schemas/app.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1423 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/schemas/audience.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      741 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/schemas/audience_device.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      965 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/schemas/banner.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      952 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/schemas/booking.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      485 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/schemas/cohort.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      589 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/schemas/competition.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1714 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/schemas/device.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      904 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/schemas/device_consent.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1044 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/schemas/device_form_data.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      935 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/schemas/device_preference.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      939 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/schemas/device_reality.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      613 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/schemas/device_token.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1855 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/schemas/event.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      832 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/schemas/event_category.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      875 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/schemas/event_integration.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      748 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/schemas/event_stage.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     5097 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/schemas/fields.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1857 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/schemas/fixture.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1321 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/schemas/form.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      908 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/schemas/form_field.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2416 2023-01-03 11:39:18.000000 livestyled-1.4.4/livestyled/schemas/fulfilment_point.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1936 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/schemas/league_table.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      968 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/schemas/location.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      539 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/schemas/magic_field.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1148 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/schemas/news.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2874 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/schemas/order.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     5094 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/schemas/payment.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     5968 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/schemas/product.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1013 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/schemas/push_broadcast.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      610 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/schemas/push_consent.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1611 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/schemas/reality.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1229 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/schemas/screen.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      442 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/schemas/season.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      318 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/schemas/sport_venue.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      481 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/schemas/storage.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      598 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/schemas/team.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     5988 2023-07-03 15:42:35.000000 livestyled-1.4.4/livestyled/schemas/ticket.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1192 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/schemas/ticket_auth.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1077 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/schemas/ticket_integration.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     4404 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/schemas/user.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      341 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/schemas/user_cohort.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)       61 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/schemas/utils.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1529 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/schemas/venue.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1221 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/schemas/widget.py
-drwxr-xr-x   0 tomrutherford   (501) staff       (20)        0 2023-07-03 15:42:48.611805 livestyled-1.4.4/livestyled/tests/
--rw-r--r--   0 tomrutherford   (501) staff       (20)        0 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/tests/__init__.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2070 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/tests/test_app.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1352 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/tests/test_create_resource_from_data.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     4421 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/tests/test_device.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2646 2022-11-28 16:23:37.000000 livestyled-1.4.4/livestyled/tests/test_resource_audience_device.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1637 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/tests/test_resource_banners.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     3628 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/tests/test_resource_client_bookings.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      857 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/tests/test_resource_client_device.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1107 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/tests/test_resource_client_device_form_data.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1431 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/tests/test_resource_client_device_realities.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2242 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/tests/test_resource_client_events.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2085 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/tests/test_resource_client_fulfilment_points.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2596 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/tests/test_resource_client_locations.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     3128 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/tests/test_resource_client_news.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2450 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/tests/test_resource_client_orders.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     5123 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/tests/test_resource_client_products.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     4770 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/tests/test_resource_client_teams.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     7908 2023-07-03 15:42:35.000000 livestyled-1.4.4/livestyled/tests/test_resource_client_ticket.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     3362 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/tests/test_resource_client_ticket_auths.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2719 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/tests/test_resource_client_user.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     3103 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/tests/test_resource_device_preferences.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2010 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/tests/test_resource_screens.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2055 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/tests/test_resource_widgets.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      658 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/tests/utils.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      411 2022-11-28 12:03:16.000000 livestyled-1.4.4/livestyled/utils.py
-drwxr-xr-x   0 tomrutherford   (501) staff       (20)        0 2023-07-03 15:42:47.295376 livestyled-1.4.4/livestyled.egg-info/
--rw-r--r--   0 tomrutherford   (501) staff       (20)      242 2023-07-03 15:42:46.000000 livestyled-1.4.4/livestyled.egg-info/PKG-INFO
--rw-r--r--   0 tomrutherford   (501) staff       (20)     4670 2023-07-03 15:42:46.000000 livestyled-1.4.4/livestyled.egg-info/SOURCES.txt
--rw-r--r--   0 tomrutherford   (501) staff       (20)        1 2023-07-03 15:42:46.000000 livestyled-1.4.4/livestyled.egg-info/dependency_links.txt
--rw-r--r--   0 tomrutherford   (501) staff       (20)       27 2023-07-03 15:42:46.000000 livestyled-1.4.4/livestyled.egg-info/entry_points.txt
--rw-r--r--   0 tomrutherford   (501) staff       (20)       68 2023-07-03 15:42:46.000000 livestyled-1.4.4/livestyled.egg-info/requires.txt
--rw-r--r--   0 tomrutherford   (501) staff       (20)       11 2023-07-03 15:42:46.000000 livestyled-1.4.4/livestyled.egg-info/top_level.txt
--rw-r--r--   0 tomrutherford   (501) staff       (20)       68 2022-11-28 12:03:16.000000 livestyled-1.4.4/requirements.txt
--rw-r--r--   0 tomrutherford   (501) staff       (20)       38 2023-07-03 15:42:48.614389 livestyled-1.4.4/setup.cfg
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1338 2022-11-28 12:03:16.000000 livestyled-1.4.4/setup.py
+drwxr-xr-x   0 tomrutherford   (501) staff       (20)        0 2023-07-03 16:05:19.265147 livestyled-1.4.5/
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1067 2022-11-28 12:03:16.000000 livestyled-1.4.5/LICENSE
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      110 2022-11-28 12:03:16.000000 livestyled-1.4.5/MANIFEST.in
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      242 2023-07-03 16:05:19.264604 livestyled-1.4.5/PKG-INFO
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      268 2022-11-28 12:03:16.000000 livestyled-1.4.5/README.md
+drwxr-xr-x   0 tomrutherford   (501) staff       (20)        0 2023-07-03 16:05:17.771375 livestyled-1.4.5/livestyled/
+-rw-r--r--   0 tomrutherford   (501) staff       (20)       22 2023-07-03 16:05:13.000000 livestyled-1.4.5/livestyled/__init__.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)    11599 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/client.py
+drwxr-xr-x   0 tomrutherford   (501) staff       (20)        0 2023-07-03 16:05:18.327396 livestyled-1.4.5/livestyled/models/
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     3790 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/models/__init__.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1166 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/models/app.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1440 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/models/audience.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1018 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/models/audience_device.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2497 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/models/banner.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2578 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/models/booking.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1140 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/models/cohort.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1306 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/models/competition.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1975 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/models/device.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      680 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/models/device_consent.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1924 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/models/device_form_data.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2371 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/models/device_preference.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      408 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/models/device_push_consent.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2093 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/models/device_reality.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1557 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/models/device_token.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2284 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/models/event.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)       30 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/models/event_category.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      657 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/models/event_date.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)       27 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/models/event_stage.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     5870 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/models/fixture.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     4573 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/models/form.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2913 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/models/form_field.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     7288 2023-01-03 11:39:18.000000 livestyled-1.4.5/livestyled/models/fulfilment_point.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     4768 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/models/league_table.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1542 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/models/location.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1358 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/models/magic_field.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1654 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/models/news.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     5358 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/models/order.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)    14632 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/models/payment.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)    16830 2023-01-12 13:18:11.000000 livestyled-1.4.5/livestyled/models/product.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2475 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/models/push_broadcast.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1682 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/models/push_consent.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2894 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/models/reality.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1875 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/models/screen.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1119 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/models/season.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      654 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/models/sport_venue.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1155 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/models/storage.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1548 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/models/team.py
+drwxr-xr-x   0 tomrutherford   (501) staff       (20)        0 2023-07-03 16:05:18.418974 livestyled-1.4.5/livestyled/models/tests/
+-rw-r--r--   0 tomrutherford   (501) staff       (20)        0 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/models/tests/__init__.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1111 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/models/tests/test_device_form_data.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1876 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/models/tests/test_fixture.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     3335 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/models/tests/test_form.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2548 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/models/tests/test_form_field.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      447 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/models/tests/test_order.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      455 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/models/tests/test_team.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     5022 2023-07-03 15:42:35.000000 livestyled-1.4.5/livestyled/models/tests/test_ticket.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)    13936 2023-07-03 15:42:35.000000 livestyled-1.4.5/livestyled/models/ticket.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2908 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/models/ticket_auth.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2504 2023-07-03 16:05:13.000000 livestyled-1.4.5/livestyled/models/ticket_integration.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     8877 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/models/user.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      526 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/models/user_cohort.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     4162 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/models/venue.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     3676 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/models/widget.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)    48299 2022-11-28 16:23:37.000000 livestyled-1.4.5/livestyled/resource_client.py
+drwxr-xr-x   0 tomrutherford   (501) staff       (20)        0 2023-07-03 16:05:18.972785 livestyled-1.4.5/livestyled/schemas/
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     4518 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/schemas/__init__.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1809 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/schemas/app.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1423 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/schemas/audience.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      741 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/schemas/audience_device.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      965 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/schemas/banner.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      952 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/schemas/booking.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      485 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/schemas/cohort.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      589 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/schemas/competition.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1714 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/schemas/device.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      904 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/schemas/device_consent.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1044 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/schemas/device_form_data.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      935 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/schemas/device_preference.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      939 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/schemas/device_reality.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      613 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/schemas/device_token.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1855 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/schemas/event.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      832 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/schemas/event_category.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      875 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/schemas/event_integration.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      748 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/schemas/event_stage.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     5097 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/schemas/fields.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1857 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/schemas/fixture.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1321 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/schemas/form.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      908 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/schemas/form_field.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2416 2023-01-03 11:39:18.000000 livestyled-1.4.5/livestyled/schemas/fulfilment_point.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1936 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/schemas/league_table.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      968 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/schemas/location.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      539 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/schemas/magic_field.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1148 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/schemas/news.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2874 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/schemas/order.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     5094 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/schemas/payment.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     5968 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/schemas/product.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1013 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/schemas/push_broadcast.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      610 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/schemas/push_consent.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1611 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/schemas/reality.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1229 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/schemas/screen.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      442 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/schemas/season.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      318 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/schemas/sport_venue.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      481 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/schemas/storage.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      598 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/schemas/team.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     5988 2023-07-03 15:42:35.000000 livestyled-1.4.5/livestyled/schemas/ticket.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1192 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/schemas/ticket_auth.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1077 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/schemas/ticket_integration.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     4404 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/schemas/user.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      341 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/schemas/user_cohort.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)       61 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/schemas/utils.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1529 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/schemas/venue.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1221 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/schemas/widget.py
+drwxr-xr-x   0 tomrutherford   (501) staff       (20)        0 2023-07-03 16:05:19.263506 livestyled-1.4.5/livestyled/tests/
+-rw-r--r--   0 tomrutherford   (501) staff       (20)        0 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/tests/__init__.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2070 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/tests/test_app.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1352 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/tests/test_create_resource_from_data.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     4421 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/tests/test_device.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2646 2022-11-28 16:23:37.000000 livestyled-1.4.5/livestyled/tests/test_resource_audience_device.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1637 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/tests/test_resource_banners.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     3628 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/tests/test_resource_client_bookings.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      857 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/tests/test_resource_client_device.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1107 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/tests/test_resource_client_device_form_data.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1431 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/tests/test_resource_client_device_realities.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2242 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/tests/test_resource_client_events.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2085 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/tests/test_resource_client_fulfilment_points.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2596 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/tests/test_resource_client_locations.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     3128 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/tests/test_resource_client_news.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2450 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/tests/test_resource_client_orders.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     5123 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/tests/test_resource_client_products.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     4770 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/tests/test_resource_client_teams.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     7908 2023-07-03 15:42:35.000000 livestyled-1.4.5/livestyled/tests/test_resource_client_ticket.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     3362 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/tests/test_resource_client_ticket_auths.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2719 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/tests/test_resource_client_user.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     3103 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/tests/test_resource_device_preferences.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2010 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/tests/test_resource_screens.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2055 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/tests/test_resource_widgets.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      658 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/tests/utils.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      411 2022-11-28 12:03:16.000000 livestyled-1.4.5/livestyled/utils.py
+drwxr-xr-x   0 tomrutherford   (501) staff       (20)        0 2023-07-03 16:05:17.787330 livestyled-1.4.5/livestyled.egg-info/
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      242 2023-07-03 16:05:17.000000 livestyled-1.4.5/livestyled.egg-info/PKG-INFO
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     4670 2023-07-03 16:05:17.000000 livestyled-1.4.5/livestyled.egg-info/SOURCES.txt
+-rw-r--r--   0 tomrutherford   (501) staff       (20)        1 2023-07-03 16:05:17.000000 livestyled-1.4.5/livestyled.egg-info/dependency_links.txt
+-rw-r--r--   0 tomrutherford   (501) staff       (20)       27 2023-07-03 16:05:17.000000 livestyled-1.4.5/livestyled.egg-info/entry_points.txt
+-rw-r--r--   0 tomrutherford   (501) staff       (20)       68 2023-07-03 16:05:17.000000 livestyled-1.4.5/livestyled.egg-info/requires.txt
+-rw-r--r--   0 tomrutherford   (501) staff       (20)       11 2023-07-03 16:05:17.000000 livestyled-1.4.5/livestyled.egg-info/top_level.txt
+-rw-r--r--   0 tomrutherford   (501) staff       (20)       68 2022-11-28 12:03:16.000000 livestyled-1.4.5/requirements.txt
+-rw-r--r--   0 tomrutherford   (501) staff       (20)       38 2023-07-03 16:05:19.265308 livestyled-1.4.5/setup.cfg
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1338 2022-11-28 12:03:16.000000 livestyled-1.4.5/setup.py
```

### Comparing `livestyled-1.4.4/LICENSE` & `livestyled-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/client.py` & `livestyled-1.4.5/livestyled/client.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/models/__init__.py` & `livestyled-1.4.5/livestyled/models/__init__.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/models/app.py` & `livestyled-1.4.5/livestyled/models/app.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/models/audience.py` & `livestyled-1.4.5/livestyled/models/audience.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/models/audience_device.py` & `livestyled-1.4.5/livestyled/models/audience_device.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/models/banner.py` & `livestyled-1.4.5/livestyled/models/banner.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/models/booking.py` & `livestyled-1.4.5/livestyled/models/booking.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/models/cohort.py` & `livestyled-1.4.5/livestyled/models/cohort.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/models/competition.py` & `livestyled-1.4.5/livestyled/models/competition.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/models/device.py` & `livestyled-1.4.5/livestyled/models/device.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/models/device_consent.py` & `livestyled-1.4.5/livestyled/models/device_consent.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/models/device_form_data.py` & `livestyled-1.4.5/livestyled/models/device_form_data.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/models/device_preference.py` & `livestyled-1.4.5/livestyled/models/device_preference.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/models/device_reality.py` & `livestyled-1.4.5/livestyled/models/device_reality.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/models/device_token.py` & `livestyled-1.4.5/livestyled/models/device_token.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/models/event.py` & `livestyled-1.4.5/livestyled/models/event.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/models/event_date.py` & `livestyled-1.4.5/livestyled/models/event_date.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/models/fixture.py` & `livestyled-1.4.5/livestyled/models/fixture.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/models/form.py` & `livestyled-1.4.5/livestyled/models/form.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/models/form_field.py` & `livestyled-1.4.5/livestyled/models/form_field.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/models/fulfilment_point.py` & `livestyled-1.4.5/livestyled/models/fulfilment_point.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/models/league_table.py` & `livestyled-1.4.5/livestyled/models/league_table.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/models/location.py` & `livestyled-1.4.5/livestyled/models/location.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/models/magic_field.py` & `livestyled-1.4.5/livestyled/models/magic_field.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/models/news.py` & `livestyled-1.4.5/livestyled/models/news.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/models/order.py` & `livestyled-1.4.5/livestyled/models/order.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/models/payment.py` & `livestyled-1.4.5/livestyled/models/payment.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/models/product.py` & `livestyled-1.4.5/livestyled/models/product.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/models/push_broadcast.py` & `livestyled-1.4.5/livestyled/models/push_broadcast.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/models/push_consent.py` & `livestyled-1.4.5/livestyled/models/push_consent.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/models/reality.py` & `livestyled-1.4.5/livestyled/models/reality.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/models/screen.py` & `livestyled-1.4.5/livestyled/models/screen.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/models/season.py` & `livestyled-1.4.5/livestyled/models/season.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/models/sport_venue.py` & `livestyled-1.4.5/livestyled/models/sport_venue.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/models/storage.py` & `livestyled-1.4.5/livestyled/models/storage.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/models/team.py` & `livestyled-1.4.5/livestyled/models/team.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/models/tests/test_device_form_data.py` & `livestyled-1.4.5/livestyled/models/tests/test_device_form_data.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/models/tests/test_fixture.py` & `livestyled-1.4.5/livestyled/models/tests/test_fixture.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/models/tests/test_form.py` & `livestyled-1.4.5/livestyled/models/tests/test_form.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/models/tests/test_form_field.py` & `livestyled-1.4.5/livestyled/models/tests/test_form_field.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/models/tests/test_ticket.py` & `livestyled-1.4.5/livestyled/models/tests/test_ticket.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/models/ticket.py` & `livestyled-1.4.5/livestyled/models/ticket.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/models/ticket_auth.py` & `livestyled-1.4.5/livestyled/models/ticket_auth.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/models/ticket_integration.py` & `livestyled-1.4.5/livestyled/models/ticket_integration.py`

 * *Files 7% similar despite different names*

```diff
@@ -72,14 +72,19 @@
             can_share=can_share
         )
         return ticket_integration
 
     def __repr__(self):
         return '<TicketIntegration(id={self.id!r})>'.format(self=self)
 
+    def __eq__(self, other):
+        if isinstance(other, TicketIntegration):
+            return self.id == other.id
+        return False
+
     def diff(self, other):
         differences = {}
         fields = (
             'label', 'name', 'endpoint_url', 'adapter', 'config_payload',
             'auth_required', 'module', 'login_request', 'default', 'can_share'
         )
         for field in fields:
```

### Comparing `livestyled-1.4.4/livestyled/models/user.py` & `livestyled-1.4.5/livestyled/models/user.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/models/user_cohort.py` & `livestyled-1.4.5/livestyled/models/user_cohort.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/models/venue.py` & `livestyled-1.4.5/livestyled/models/venue.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/models/widget.py` & `livestyled-1.4.5/livestyled/models/widget.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/resource_client.py` & `livestyled-1.4.5/livestyled/resource_client.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/schemas/__init__.py` & `livestyled-1.4.5/livestyled/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/schemas/app.py` & `livestyled-1.4.5/livestyled/schemas/app.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/schemas/audience.py` & `livestyled-1.4.5/livestyled/schemas/audience.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/schemas/audience_device.py` & `livestyled-1.4.5/livestyled/schemas/audience_device.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/schemas/banner.py` & `livestyled-1.4.5/livestyled/schemas/banner.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/schemas/booking.py` & `livestyled-1.4.5/livestyled/schemas/booking.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/schemas/competition.py` & `livestyled-1.4.5/livestyled/schemas/competition.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/schemas/device.py` & `livestyled-1.4.5/livestyled/schemas/device.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/schemas/device_consent.py` & `livestyled-1.4.5/livestyled/schemas/device_consent.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/schemas/device_form_data.py` & `livestyled-1.4.5/livestyled/schemas/device_form_data.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/schemas/device_preference.py` & `livestyled-1.4.5/livestyled/schemas/device_preference.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/schemas/device_reality.py` & `livestyled-1.4.5/livestyled/schemas/device_reality.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/schemas/device_token.py` & `livestyled-1.4.5/livestyled/schemas/device_token.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/schemas/event.py` & `livestyled-1.4.5/livestyled/schemas/event.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/schemas/event_category.py` & `livestyled-1.4.5/livestyled/schemas/event_category.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/schemas/event_integration.py` & `livestyled-1.4.5/livestyled/schemas/event_integration.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/schemas/event_stage.py` & `livestyled-1.4.5/livestyled/schemas/event_stage.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/schemas/fields.py` & `livestyled-1.4.5/livestyled/schemas/fields.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/schemas/fixture.py` & `livestyled-1.4.5/livestyled/schemas/fixture.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/schemas/form.py` & `livestyled-1.4.5/livestyled/schemas/form.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/schemas/form_field.py` & `livestyled-1.4.5/livestyled/schemas/form_field.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/schemas/fulfilment_point.py` & `livestyled-1.4.5/livestyled/schemas/fulfilment_point.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/schemas/league_table.py` & `livestyled-1.4.5/livestyled/schemas/league_table.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/schemas/location.py` & `livestyled-1.4.5/livestyled/schemas/location.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/schemas/magic_field.py` & `livestyled-1.4.5/livestyled/schemas/magic_field.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/schemas/news.py` & `livestyled-1.4.5/livestyled/schemas/news.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/schemas/order.py` & `livestyled-1.4.5/livestyled/schemas/order.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/schemas/payment.py` & `livestyled-1.4.5/livestyled/schemas/payment.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/schemas/product.py` & `livestyled-1.4.5/livestyled/schemas/product.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/schemas/push_broadcast.py` & `livestyled-1.4.5/livestyled/schemas/push_broadcast.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/schemas/push_consent.py` & `livestyled-1.4.5/livestyled/schemas/push_consent.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/schemas/reality.py` & `livestyled-1.4.5/livestyled/schemas/reality.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/schemas/screen.py` & `livestyled-1.4.5/livestyled/schemas/screen.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/schemas/team.py` & `livestyled-1.4.5/livestyled/schemas/team.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/schemas/ticket.py` & `livestyled-1.4.5/livestyled/schemas/ticket.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/schemas/ticket_auth.py` & `livestyled-1.4.5/livestyled/schemas/ticket_auth.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/schemas/ticket_integration.py` & `livestyled-1.4.5/livestyled/schemas/ticket_integration.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/schemas/user.py` & `livestyled-1.4.5/livestyled/schemas/user.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/schemas/venue.py` & `livestyled-1.4.5/livestyled/schemas/venue.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/schemas/widget.py` & `livestyled-1.4.5/livestyled/schemas/widget.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/tests/test_app.py` & `livestyled-1.4.5/livestyled/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/tests/test_create_resource_from_data.py` & `livestyled-1.4.5/livestyled/tests/test_create_resource_from_data.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/tests/test_device.py` & `livestyled-1.4.5/livestyled/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/tests/test_resource_audience_device.py` & `livestyled-1.4.5/livestyled/tests/test_resource_audience_device.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/tests/test_resource_banners.py` & `livestyled-1.4.5/livestyled/tests/test_resource_banners.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/tests/test_resource_client_bookings.py` & `livestyled-1.4.5/livestyled/tests/test_resource_client_bookings.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/tests/test_resource_client_device.py` & `livestyled-1.4.5/livestyled/tests/test_resource_client_device.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/tests/test_resource_client_device_form_data.py` & `livestyled-1.4.5/livestyled/tests/test_resource_client_device_form_data.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/tests/test_resource_client_device_realities.py` & `livestyled-1.4.5/livestyled/tests/test_resource_client_device_realities.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/tests/test_resource_client_events.py` & `livestyled-1.4.5/livestyled/tests/test_resource_client_events.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/tests/test_resource_client_fulfilment_points.py` & `livestyled-1.4.5/livestyled/tests/test_resource_client_fulfilment_points.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/tests/test_resource_client_locations.py` & `livestyled-1.4.5/livestyled/tests/test_resource_client_locations.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/tests/test_resource_client_news.py` & `livestyled-1.4.5/livestyled/tests/test_resource_client_news.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/tests/test_resource_client_orders.py` & `livestyled-1.4.5/livestyled/tests/test_resource_client_orders.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/tests/test_resource_client_products.py` & `livestyled-1.4.5/livestyled/tests/test_resource_client_products.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/tests/test_resource_client_teams.py` & `livestyled-1.4.5/livestyled/tests/test_resource_client_teams.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/tests/test_resource_client_ticket.py` & `livestyled-1.4.5/livestyled/tests/test_resource_client_ticket.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/tests/test_resource_client_ticket_auths.py` & `livestyled-1.4.5/livestyled/tests/test_resource_client_ticket_auths.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/tests/test_resource_client_user.py` & `livestyled-1.4.5/livestyled/tests/test_resource_client_user.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/tests/test_resource_device_preferences.py` & `livestyled-1.4.5/livestyled/tests/test_resource_device_preferences.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/tests/test_resource_screens.py` & `livestyled-1.4.5/livestyled/tests/test_resource_screens.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/tests/test_resource_widgets.py` & `livestyled-1.4.5/livestyled/tests/test_resource_widgets.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled/tests/utils.py` & `livestyled-1.4.5/livestyled/tests/utils.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/livestyled.egg-info/SOURCES.txt` & `livestyled-1.4.5/livestyled.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.4/setup.py` & `livestyled-1.4.5/setup.py`

 * *Files identical despite different names*

