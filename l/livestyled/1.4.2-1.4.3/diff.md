# Comparing `tmp/livestyled-1.4.2.tar.gz` & `tmp/livestyled-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livestyled-1.4.2.tar", last modified: Thu Jan 12 13:18:31 2023, max compression
+gzip compressed data, was "livestyled-1.4.3.tar", last modified: Mon Jul  3 15:10:08 2023, max compression
```

## Comparing `livestyled-1.4.2.tar` & `livestyled-1.4.3.tar`

### file list

```diff
@@ -1,146 +1,147 @@
-drwxr-xr-x   0 tomrutherford   (501) staff       (20)        0 2023-01-12 13:18:31.070183 livestyled-1.4.2/
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1067 2022-11-28 12:03:16.000000 livestyled-1.4.2/LICENSE
--rw-r--r--   0 tomrutherford   (501) staff       (20)      110 2022-11-28 12:03:16.000000 livestyled-1.4.2/MANIFEST.in
--rw-r--r--   0 tomrutherford   (501) staff       (20)      180 2023-01-12 13:18:31.069866 livestyled-1.4.2/PKG-INFO
--rw-r--r--   0 tomrutherford   (501) staff       (20)      268 2022-11-28 12:03:16.000000 livestyled-1.4.2/README.md
-drwxr-xr-x   0 tomrutherford   (501) staff       (20)        0 2023-01-12 13:18:31.014409 livestyled-1.4.2/livestyled/
--rw-r--r--   0 tomrutherford   (501) staff       (20)       22 2023-01-12 13:18:11.000000 livestyled-1.4.2/livestyled/__init__.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)    11599 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/client.py
-drwxr-xr-x   0 tomrutherford   (501) staff       (20)        0 2023-01-12 13:18:31.035889 livestyled-1.4.2/livestyled/models/
--rw-r--r--   0 tomrutherford   (501) staff       (20)     3790 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/__init__.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1166 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/app.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1440 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/audience.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1018 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/audience_device.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2497 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/banner.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2578 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/booking.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1140 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/cohort.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1306 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/competition.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1975 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/device.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      680 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/device_consent.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1924 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/device_form_data.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2371 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/device_preference.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      408 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/device_push_consent.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2093 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/device_reality.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1557 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/device_token.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2284 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/event.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)       30 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/event_category.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      657 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/event_date.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)       27 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/event_stage.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     5870 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/fixture.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     4573 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/form.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2913 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/form_field.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     7288 2023-01-03 11:39:18.000000 livestyled-1.4.2/livestyled/models/fulfilment_point.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     4768 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/league_table.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1542 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/location.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1358 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/magic_field.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1654 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/news.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     5358 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/order.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)    14632 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/payment.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)    16830 2023-01-12 13:18:11.000000 livestyled-1.4.2/livestyled/models/product.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2475 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/push_broadcast.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1682 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/push_consent.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2894 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/reality.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1875 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/screen.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1119 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/season.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      654 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/sport_venue.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1155 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/storage.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1548 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/team.py
-drwxr-xr-x   0 tomrutherford   (501) staff       (20)        0 2023-01-12 13:18:31.039586 livestyled-1.4.2/livestyled/models/tests/
--rw-r--r--   0 tomrutherford   (501) staff       (20)        0 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/tests/__init__.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1111 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/tests/test_device_form_data.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1876 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/tests/test_fixture.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     3335 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/tests/test_form.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2548 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/tests/test_form_field.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      447 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/tests/test_order.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      455 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/tests/test_team.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     4890 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/tests/test_ticket.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)    13599 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/ticket.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2908 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/ticket_auth.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2365 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/ticket_integration.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     8877 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/user.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      526 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/user_cohort.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     4162 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/venue.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     3676 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/models/widget.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)    48299 2022-11-28 16:23:37.000000 livestyled-1.4.2/livestyled/resource_client.py
-drwxr-xr-x   0 tomrutherford   (501) staff       (20)        0 2023-01-12 13:18:31.059899 livestyled-1.4.2/livestyled/schemas/
--rw-r--r--   0 tomrutherford   (501) staff       (20)     4518 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/schemas/__init__.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1809 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/schemas/app.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1423 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/schemas/audience.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      741 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/schemas/audience_device.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      965 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/schemas/banner.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      952 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/schemas/booking.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      485 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/schemas/cohort.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      589 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/schemas/competition.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1714 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/schemas/device.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      904 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/schemas/device_consent.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1044 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/schemas/device_form_data.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      935 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/schemas/device_preference.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      939 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/schemas/device_reality.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      613 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/schemas/device_token.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1855 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/schemas/event.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      832 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/schemas/event_category.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      875 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/schemas/event_integration.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      748 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/schemas/event_stage.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     5097 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/schemas/fields.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1857 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/schemas/fixture.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1321 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/schemas/form.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      908 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/schemas/form_field.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2416 2023-01-03 11:39:18.000000 livestyled-1.4.2/livestyled/schemas/fulfilment_point.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1936 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/schemas/league_table.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      968 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/schemas/location.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      539 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/schemas/magic_field.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1148 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/schemas/news.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2874 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/schemas/order.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     5094 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/schemas/payment.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     5968 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/schemas/product.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1013 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/schemas/push_broadcast.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      610 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/schemas/push_consent.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1611 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/schemas/reality.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1229 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/schemas/screen.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      442 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/schemas/season.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      318 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/schemas/sport_venue.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      481 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/schemas/storage.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      598 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/schemas/team.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     5829 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/schemas/ticket.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1192 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/schemas/ticket_auth.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1077 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/schemas/ticket_integration.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     4404 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/schemas/user.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      341 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/schemas/user_cohort.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)       61 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/schemas/utils.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1529 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/schemas/venue.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1221 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/schemas/widget.py
-drwxr-xr-x   0 tomrutherford   (501) staff       (20)        0 2023-01-12 13:18:31.069418 livestyled-1.4.2/livestyled/tests/
--rw-r--r--   0 tomrutherford   (501) staff       (20)        0 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/tests/__init__.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2070 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/tests/test_app.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1352 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/tests/test_create_resource_from_data.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     4421 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/tests/test_device.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2646 2022-11-28 16:23:37.000000 livestyled-1.4.2/livestyled/tests/test_resource_audience_device.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1637 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/tests/test_resource_banners.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     3628 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/tests/test_resource_client_bookings.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      857 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/tests/test_resource_client_device.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1107 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/tests/test_resource_client_device_form_data.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1431 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/tests/test_resource_client_device_realities.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2242 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/tests/test_resource_client_events.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2085 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/tests/test_resource_client_fulfilment_points.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2596 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/tests/test_resource_client_locations.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     3128 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/tests/test_resource_client_news.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2450 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/tests/test_resource_client_orders.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     5123 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/tests/test_resource_client_products.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     4770 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/tests/test_resource_client_teams.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     7797 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/tests/test_resource_client_ticket.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     3362 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/tests/test_resource_client_ticket_auths.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2719 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/tests/test_resource_client_user.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     3103 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/tests/test_resource_device_preferences.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2010 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/tests/test_resource_screens.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)     2055 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/tests/test_resource_widgets.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      658 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/tests/utils.py
--rw-r--r--   0 tomrutherford   (501) staff       (20)      411 2022-11-28 12:03:16.000000 livestyled-1.4.2/livestyled/utils.py
-drwxr-xr-x   0 tomrutherford   (501) staff       (20)        0 2023-01-12 13:18:31.016380 livestyled-1.4.2/livestyled.egg-info/
--rw-r--r--   0 tomrutherford   (501) staff       (20)      180 2023-01-12 13:18:30.000000 livestyled-1.4.2/livestyled.egg-info/PKG-INFO
--rw-r--r--   0 tomrutherford   (501) staff       (20)     4633 2023-01-12 13:18:30.000000 livestyled-1.4.2/livestyled.egg-info/SOURCES.txt
--rw-r--r--   0 tomrutherford   (501) staff       (20)        1 2023-01-12 13:18:30.000000 livestyled-1.4.2/livestyled.egg-info/dependency_links.txt
--rw-r--r--   0 tomrutherford   (501) staff       (20)       68 2023-01-12 13:18:30.000000 livestyled-1.4.2/livestyled.egg-info/requires.txt
--rw-r--r--   0 tomrutherford   (501) staff       (20)       11 2023-01-12 13:18:30.000000 livestyled-1.4.2/livestyled.egg-info/top_level.txt
--rw-r--r--   0 tomrutherford   (501) staff       (20)       68 2022-11-28 12:03:16.000000 livestyled-1.4.2/requirements.txt
--rw-r--r--   0 tomrutherford   (501) staff       (20)       38 2023-01-12 13:18:31.070273 livestyled-1.4.2/setup.cfg
--rw-r--r--   0 tomrutherford   (501) staff       (20)     1338 2022-11-28 12:03:16.000000 livestyled-1.4.2/setup.py
+drwxr-xr-x   0 tomrutherford   (501) staff       (20)        0 2023-07-03 15:10:08.746814 livestyled-1.4.3/
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1067 2022-11-28 12:03:16.000000 livestyled-1.4.3/LICENSE
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      110 2022-11-28 12:03:16.000000 livestyled-1.4.3/MANIFEST.in
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      242 2023-07-03 15:10:08.745756 livestyled-1.4.3/PKG-INFO
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      268 2022-11-28 12:03:16.000000 livestyled-1.4.3/README.md
+drwxr-xr-x   0 tomrutherford   (501) staff       (20)        0 2023-07-03 15:10:07.601885 livestyled-1.4.3/livestyled/
+-rw-r--r--   0 tomrutherford   (501) staff       (20)       22 2023-07-03 15:09:05.000000 livestyled-1.4.3/livestyled/__init__.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)    11599 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/client.py
+drwxr-xr-x   0 tomrutherford   (501) staff       (20)        0 2023-07-03 15:10:08.073777 livestyled-1.4.3/livestyled/models/
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     3790 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/models/__init__.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1166 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/models/app.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1440 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/models/audience.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1018 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/models/audience_device.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2497 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/models/banner.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2578 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/models/booking.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1140 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/models/cohort.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1306 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/models/competition.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1975 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/models/device.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      680 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/models/device_consent.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1924 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/models/device_form_data.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2371 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/models/device_preference.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      408 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/models/device_push_consent.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2093 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/models/device_reality.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1557 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/models/device_token.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2284 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/models/event.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)       30 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/models/event_category.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      657 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/models/event_date.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)       27 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/models/event_stage.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     5870 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/models/fixture.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     4573 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/models/form.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2913 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/models/form_field.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     7288 2023-01-03 11:39:18.000000 livestyled-1.4.3/livestyled/models/fulfilment_point.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     4768 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/models/league_table.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1542 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/models/location.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1358 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/models/magic_field.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1654 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/models/news.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     5358 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/models/order.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)    14632 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/models/payment.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)    16830 2023-01-12 13:18:11.000000 livestyled-1.4.3/livestyled/models/product.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2475 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/models/push_broadcast.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1682 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/models/push_consent.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2894 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/models/reality.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1875 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/models/screen.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1119 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/models/season.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      654 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/models/sport_venue.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1155 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/models/storage.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1548 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/models/team.py
+drwxr-xr-x   0 tomrutherford   (501) staff       (20)        0 2023-07-03 15:10:08.129948 livestyled-1.4.3/livestyled/models/tests/
+-rw-r--r--   0 tomrutherford   (501) staff       (20)        0 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/models/tests/__init__.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1111 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/models/tests/test_device_form_data.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1876 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/models/tests/test_fixture.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     3335 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/models/tests/test_form.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2548 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/models/tests/test_form_field.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      447 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/models/tests/test_order.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      455 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/models/tests/test_team.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     4890 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/models/tests/test_ticket.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)    13756 2023-07-03 15:09:06.000000 livestyled-1.4.3/livestyled/models/ticket.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2908 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/models/ticket_auth.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2365 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/models/ticket_integration.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     8877 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/models/user.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      526 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/models/user_cohort.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     4162 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/models/venue.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     3676 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/models/widget.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)    48299 2022-11-28 16:23:37.000000 livestyled-1.4.3/livestyled/resource_client.py
+drwxr-xr-x   0 tomrutherford   (501) staff       (20)        0 2023-07-03 15:10:08.523009 livestyled-1.4.3/livestyled/schemas/
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     4518 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/schemas/__init__.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1809 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/schemas/app.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1423 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/schemas/audience.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      741 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/schemas/audience_device.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      965 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/schemas/banner.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      952 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/schemas/booking.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      485 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/schemas/cohort.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      589 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/schemas/competition.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1714 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/schemas/device.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      904 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/schemas/device_consent.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1044 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/schemas/device_form_data.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      935 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/schemas/device_preference.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      939 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/schemas/device_reality.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      613 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/schemas/device_token.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1855 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/schemas/event.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      832 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/schemas/event_category.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      875 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/schemas/event_integration.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      748 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/schemas/event_stage.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     5097 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/schemas/fields.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1857 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/schemas/fixture.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1321 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/schemas/form.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      908 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/schemas/form_field.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2416 2023-01-03 11:39:18.000000 livestyled-1.4.3/livestyled/schemas/fulfilment_point.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1936 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/schemas/league_table.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      968 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/schemas/location.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      539 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/schemas/magic_field.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1148 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/schemas/news.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2874 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/schemas/order.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     5094 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/schemas/payment.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     5968 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/schemas/product.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1013 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/schemas/push_broadcast.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      610 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/schemas/push_consent.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1611 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/schemas/reality.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1229 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/schemas/screen.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      442 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/schemas/season.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      318 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/schemas/sport_venue.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      481 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/schemas/storage.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      598 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/schemas/team.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     5905 2023-07-03 15:09:06.000000 livestyled-1.4.3/livestyled/schemas/ticket.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1192 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/schemas/ticket_auth.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1077 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/schemas/ticket_integration.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     4404 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/schemas/user.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      341 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/schemas/user_cohort.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)       61 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/schemas/utils.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1529 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/schemas/venue.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1221 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/schemas/widget.py
+drwxr-xr-x   0 tomrutherford   (501) staff       (20)        0 2023-07-03 15:10:08.744090 livestyled-1.4.3/livestyled/tests/
+-rw-r--r--   0 tomrutherford   (501) staff       (20)        0 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/tests/__init__.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2070 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/tests/test_app.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1352 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/tests/test_create_resource_from_data.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     4421 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/tests/test_device.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2646 2022-11-28 16:23:37.000000 livestyled-1.4.3/livestyled/tests/test_resource_audience_device.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1637 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/tests/test_resource_banners.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     3628 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/tests/test_resource_client_bookings.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      857 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/tests/test_resource_client_device.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1107 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/tests/test_resource_client_device_form_data.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1431 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/tests/test_resource_client_device_realities.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2242 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/tests/test_resource_client_events.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2085 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/tests/test_resource_client_fulfilment_points.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2596 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/tests/test_resource_client_locations.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     3128 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/tests/test_resource_client_news.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2450 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/tests/test_resource_client_orders.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     5123 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/tests/test_resource_client_products.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     4770 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/tests/test_resource_client_teams.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     7797 2023-07-03 14:52:27.000000 livestyled-1.4.3/livestyled/tests/test_resource_client_ticket.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     3362 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/tests/test_resource_client_ticket_auths.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2719 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/tests/test_resource_client_user.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     3103 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/tests/test_resource_device_preferences.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2010 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/tests/test_resource_screens.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     2055 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/tests/test_resource_widgets.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      658 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/tests/utils.py
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      411 2022-11-28 12:03:16.000000 livestyled-1.4.3/livestyled/utils.py
+drwxr-xr-x   0 tomrutherford   (501) staff       (20)        0 2023-07-03 15:10:07.631826 livestyled-1.4.3/livestyled.egg-info/
+-rw-r--r--   0 tomrutherford   (501) staff       (20)      242 2023-07-03 15:10:07.000000 livestyled-1.4.3/livestyled.egg-info/PKG-INFO
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     4670 2023-07-03 15:10:07.000000 livestyled-1.4.3/livestyled.egg-info/SOURCES.txt
+-rw-r--r--   0 tomrutherford   (501) staff       (20)        1 2023-07-03 15:10:07.000000 livestyled-1.4.3/livestyled.egg-info/dependency_links.txt
+-rw-r--r--   0 tomrutherford   (501) staff       (20)       27 2023-07-03 15:10:07.000000 livestyled-1.4.3/livestyled.egg-info/entry_points.txt
+-rw-r--r--   0 tomrutherford   (501) staff       (20)       68 2023-07-03 15:10:07.000000 livestyled-1.4.3/livestyled.egg-info/requires.txt
+-rw-r--r--   0 tomrutherford   (501) staff       (20)       11 2023-07-03 15:10:07.000000 livestyled-1.4.3/livestyled.egg-info/top_level.txt
+-rw-r--r--   0 tomrutherford   (501) staff       (20)       68 2022-11-28 12:03:16.000000 livestyled-1.4.3/requirements.txt
+-rw-r--r--   0 tomrutherford   (501) staff       (20)       38 2023-07-03 15:10:08.747113 livestyled-1.4.3/setup.cfg
+-rw-r--r--   0 tomrutherford   (501) staff       (20)     1338 2022-11-28 12:03:16.000000 livestyled-1.4.3/setup.py
```

### Comparing `livestyled-1.4.2/LICENSE` & `livestyled-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/client.py` & `livestyled-1.4.3/livestyled/client.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/models/__init__.py` & `livestyled-1.4.3/livestyled/models/__init__.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/models/app.py` & `livestyled-1.4.3/livestyled/models/app.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/models/audience.py` & `livestyled-1.4.3/livestyled/models/audience.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/models/audience_device.py` & `livestyled-1.4.3/livestyled/models/audience_device.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/models/banner.py` & `livestyled-1.4.3/livestyled/models/banner.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/models/booking.py` & `livestyled-1.4.3/livestyled/models/booking.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/models/cohort.py` & `livestyled-1.4.3/livestyled/models/cohort.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/models/competition.py` & `livestyled-1.4.3/livestyled/models/competition.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/models/device.py` & `livestyled-1.4.3/livestyled/models/device.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/models/device_consent.py` & `livestyled-1.4.3/livestyled/models/device_consent.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/models/device_form_data.py` & `livestyled-1.4.3/livestyled/models/device_form_data.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/models/device_preference.py` & `livestyled-1.4.3/livestyled/models/device_preference.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/models/device_reality.py` & `livestyled-1.4.3/livestyled/models/device_reality.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/models/device_token.py` & `livestyled-1.4.3/livestyled/models/device_token.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/models/event.py` & `livestyled-1.4.3/livestyled/models/event.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/models/event_date.py` & `livestyled-1.4.3/livestyled/models/event_date.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/models/fixture.py` & `livestyled-1.4.3/livestyled/models/fixture.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/models/form.py` & `livestyled-1.4.3/livestyled/models/form.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/models/form_field.py` & `livestyled-1.4.3/livestyled/models/form_field.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/models/fulfilment_point.py` & `livestyled-1.4.3/livestyled/models/fulfilment_point.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/models/league_table.py` & `livestyled-1.4.3/livestyled/models/league_table.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/models/location.py` & `livestyled-1.4.3/livestyled/models/location.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/models/magic_field.py` & `livestyled-1.4.3/livestyled/models/magic_field.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/models/news.py` & `livestyled-1.4.3/livestyled/models/news.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/models/order.py` & `livestyled-1.4.3/livestyled/models/order.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/models/payment.py` & `livestyled-1.4.3/livestyled/models/payment.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/models/product.py` & `livestyled-1.4.3/livestyled/models/product.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/models/push_broadcast.py` & `livestyled-1.4.3/livestyled/models/push_broadcast.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/models/push_consent.py` & `livestyled-1.4.3/livestyled/models/push_consent.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/models/reality.py` & `livestyled-1.4.3/livestyled/models/reality.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/models/screen.py` & `livestyled-1.4.3/livestyled/models/screen.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/models/season.py` & `livestyled-1.4.3/livestyled/models/season.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/models/sport_venue.py` & `livestyled-1.4.3/livestyled/models/sport_venue.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/models/storage.py` & `livestyled-1.4.3/livestyled/models/storage.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/models/team.py` & `livestyled-1.4.3/livestyled/models/team.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/models/tests/test_device_form_data.py` & `livestyled-1.4.3/livestyled/models/tests/test_device_form_data.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/models/tests/test_fixture.py` & `livestyled-1.4.3/livestyled/models/tests/test_fixture.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/models/tests/test_form.py` & `livestyled-1.4.3/livestyled/models/tests/test_form.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/models/tests/test_form_field.py` & `livestyled-1.4.3/livestyled/models/tests/test_form_field.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/models/tests/test_ticket.py` & `livestyled-1.4.3/livestyled/models/tests/test_ticket.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/models/ticket.py` & `livestyled-1.4.3/livestyled/models/ticket.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,16 @@
             venue=None,
             event=None,
             ticket_auth=None,
             event_date=None,
             currency=None,
             external_card_ref=None,
             additional_fields=[],
-            printed=True
+            printed=True,
+            timezone=None
     ):
         self.id = id
         self.external_ticket_id = external_ticket_id
         self.external_movement_id = external_movement_id
         self.seat = seat
         self.qr_code_url = qr_code_url
         self.session_date = session_date
@@ -162,14 +163,15 @@
             elif isinstance(currency, dict):
                 self.currency = Currency(**currency)
         else:
             self.currency = None
 
         self.additional_fields = additional_fields
         self.printed = printed
+        self.timezone = timezone
 
     @classmethod
     def placeholder(
             cls,
             id
     ):
         return cls(
@@ -215,15 +217,16 @@
             map_image_url=None,
             ticket_integration=None,
             venue=None,
             event=None,
             currency=None,
             external_card_ref=None,
             additional_fields=[],
-            printed=True
+            printed=True,
+            timezone=None
         )
 
     @classmethod
     def create_new(
             cls,
             user: User or str or int,
             external_ticket_id=None,
@@ -264,15 +267,16 @@
             map_image_url=None,
             ticket_integration=None,
             venue: Venue or str or int or None = None,
             event: Event or str or int or None = None,
             currency: Currency or None = None,
             external_card_ref=None,
             additional_fields=None,
-            printed=True
+            printed=True,
+            timezone=None
     ):
         if additional_fields is None:
             additional_fields = []
         ticket = Ticket(
             id=None,
             external_ticket_id=external_ticket_id,
             external_movement_id=external_movement_id,
@@ -315,15 +319,16 @@
             map_image_url=map_image_url,
             ticket_integration=ticket_integration,
             venue=venue,
             event=event,
             currency=currency,
             external_card_ref=external_card_ref,
             additional_fields=additional_fields,
-            printed=printed
+            printed=printed,
+            timezone=timezone
         )
         if isinstance(user, (str, int)):
             user = User.placeholder(id=user)
         ticket._user = user
         if isinstance(sharer, (str or int)):
             sharer = User.placeholder(id=sharer)
         ticket._sharer = sharer
@@ -383,15 +388,15 @@
         differences = {}
         fields = (
             'external_ticket_id', 'seat', 'qr_code_url', 'session_date', 'title', 'legacy_external_event_id',
             'external_event_id', 'barcode', 'sector_name', 'venue_name', 'venue_room', 'client_name', 'premium',
             'client_email', 'price', 'status', 'can_share', 'sharer_email', 'redeemed_at', 'redeemer_id', 'share_code',
             'redeemer_email', 'parent_ticket', 'shared_at', 'legal_long_text', 'legal_short_text', 'map_url',
             'map_image_url', 'ticket_integration', 'entrance', 'row', 'section', 'price_code', 'external_customer_ref',
-            'venue', 'event', 'event_date', 'currency', 'external_card_ref', 'additional_fields', 'printed'
+            'venue', 'event', 'event_date', 'currency', 'external_card_ref', 'additional_fields', 'printed', 'timezone'
         )
         for field in fields:
             if getattr(self, field) != getattr(other, field):
                 if field == 'additional_fields' and getattr(other, field):
                     if getattr(self, field):
                         additional_fields = []
                         for current in getattr(other, field):
```

### Comparing `livestyled-1.4.2/livestyled/models/ticket_auth.py` & `livestyled-1.4.3/livestyled/models/ticket_auth.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/models/ticket_integration.py` & `livestyled-1.4.3/livestyled/models/ticket_integration.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/models/user.py` & `livestyled-1.4.3/livestyled/models/user.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/models/user_cohort.py` & `livestyled-1.4.3/livestyled/models/user_cohort.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/models/venue.py` & `livestyled-1.4.3/livestyled/models/venue.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/models/widget.py` & `livestyled-1.4.3/livestyled/models/widget.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/resource_client.py` & `livestyled-1.4.3/livestyled/resource_client.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/schemas/__init__.py` & `livestyled-1.4.3/livestyled/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/schemas/app.py` & `livestyled-1.4.3/livestyled/schemas/app.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/schemas/audience.py` & `livestyled-1.4.3/livestyled/schemas/audience.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/schemas/audience_device.py` & `livestyled-1.4.3/livestyled/schemas/audience_device.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/schemas/banner.py` & `livestyled-1.4.3/livestyled/schemas/banner.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/schemas/booking.py` & `livestyled-1.4.3/livestyled/schemas/booking.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/schemas/competition.py` & `livestyled-1.4.3/livestyled/schemas/competition.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/schemas/device.py` & `livestyled-1.4.3/livestyled/schemas/device.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/schemas/device_consent.py` & `livestyled-1.4.3/livestyled/schemas/device_consent.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/schemas/device_form_data.py` & `livestyled-1.4.3/livestyled/schemas/device_form_data.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/schemas/device_preference.py` & `livestyled-1.4.3/livestyled/schemas/device_preference.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/schemas/device_reality.py` & `livestyled-1.4.3/livestyled/schemas/device_reality.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/schemas/device_token.py` & `livestyled-1.4.3/livestyled/schemas/device_token.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/schemas/event.py` & `livestyled-1.4.3/livestyled/schemas/event.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/schemas/event_category.py` & `livestyled-1.4.3/livestyled/schemas/event_category.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/schemas/event_integration.py` & `livestyled-1.4.3/livestyled/schemas/event_integration.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/schemas/event_stage.py` & `livestyled-1.4.3/livestyled/schemas/event_stage.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/schemas/fields.py` & `livestyled-1.4.3/livestyled/schemas/fields.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/schemas/fixture.py` & `livestyled-1.4.3/livestyled/schemas/fixture.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/schemas/form.py` & `livestyled-1.4.3/livestyled/schemas/form.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/schemas/form_field.py` & `livestyled-1.4.3/livestyled/schemas/form_field.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/schemas/fulfilment_point.py` & `livestyled-1.4.3/livestyled/schemas/fulfilment_point.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/schemas/league_table.py` & `livestyled-1.4.3/livestyled/schemas/league_table.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/schemas/location.py` & `livestyled-1.4.3/livestyled/schemas/location.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/schemas/magic_field.py` & `livestyled-1.4.3/livestyled/schemas/magic_field.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/schemas/news.py` & `livestyled-1.4.3/livestyled/schemas/news.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/schemas/order.py` & `livestyled-1.4.3/livestyled/schemas/order.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/schemas/payment.py` & `livestyled-1.4.3/livestyled/schemas/payment.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/schemas/product.py` & `livestyled-1.4.3/livestyled/schemas/product.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/schemas/push_broadcast.py` & `livestyled-1.4.3/livestyled/schemas/push_broadcast.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/schemas/push_consent.py` & `livestyled-1.4.3/livestyled/schemas/push_consent.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/schemas/reality.py` & `livestyled-1.4.3/livestyled/schemas/reality.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/schemas/screen.py` & `livestyled-1.4.3/livestyled/schemas/screen.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/schemas/team.py` & `livestyled-1.4.3/livestyled/schemas/team.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/schemas/ticket.py` & `livestyled-1.4.3/livestyled/schemas/ticket.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,7 +95,8 @@
     event = RelatedResourceLinkField(schema=EventSchema, required=False, missing=None)
     venue = RelatedResourceLinkField(schema=VenueSchema, required=False, missing=None)
     currency = RelatedResourceLinkField(schema=CurrencySchema, required=False, missing=None)
     external_card_ref = fields.String(data_key='externalCardRef', required=False, missing=None)
     additional_fields = fields.Nested(AdditionalFields, data_key='additionalFields', allow_none=True, missing=None,
                                       many=True)
     printed = fields.Boolean(allow_none=True, required=False, missing=True)
+    timezone = fields.String(allow_none=True, required=False, missing=None)
```

### Comparing `livestyled-1.4.2/livestyled/schemas/ticket_auth.py` & `livestyled-1.4.3/livestyled/schemas/ticket_auth.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/schemas/ticket_integration.py` & `livestyled-1.4.3/livestyled/schemas/ticket_integration.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/schemas/user.py` & `livestyled-1.4.3/livestyled/schemas/user.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/schemas/venue.py` & `livestyled-1.4.3/livestyled/schemas/venue.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/schemas/widget.py` & `livestyled-1.4.3/livestyled/schemas/widget.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/tests/test_app.py` & `livestyled-1.4.3/livestyled/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/tests/test_create_resource_from_data.py` & `livestyled-1.4.3/livestyled/tests/test_create_resource_from_data.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/tests/test_device.py` & `livestyled-1.4.3/livestyled/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/tests/test_resource_audience_device.py` & `livestyled-1.4.3/livestyled/tests/test_resource_audience_device.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/tests/test_resource_banners.py` & `livestyled-1.4.3/livestyled/tests/test_resource_banners.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/tests/test_resource_client_bookings.py` & `livestyled-1.4.3/livestyled/tests/test_resource_client_bookings.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/tests/test_resource_client_device.py` & `livestyled-1.4.3/livestyled/tests/test_resource_client_device.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/tests/test_resource_client_device_form_data.py` & `livestyled-1.4.3/livestyled/tests/test_resource_client_device_form_data.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/tests/test_resource_client_device_realities.py` & `livestyled-1.4.3/livestyled/tests/test_resource_client_device_realities.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/tests/test_resource_client_events.py` & `livestyled-1.4.3/livestyled/tests/test_resource_client_events.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/tests/test_resource_client_fulfilment_points.py` & `livestyled-1.4.3/livestyled/tests/test_resource_client_fulfilment_points.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/tests/test_resource_client_locations.py` & `livestyled-1.4.3/livestyled/tests/test_resource_client_locations.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/tests/test_resource_client_news.py` & `livestyled-1.4.3/livestyled/tests/test_resource_client_news.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/tests/test_resource_client_orders.py` & `livestyled-1.4.3/livestyled/tests/test_resource_client_orders.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/tests/test_resource_client_products.py` & `livestyled-1.4.3/livestyled/tests/test_resource_client_products.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/tests/test_resource_client_teams.py` & `livestyled-1.4.3/livestyled/tests/test_resource_client_teams.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/tests/test_resource_client_ticket.py` & `livestyled-1.4.3/livestyled/tests/test_resource_client_ticket.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/tests/test_resource_client_ticket_auths.py` & `livestyled-1.4.3/livestyled/tests/test_resource_client_ticket_auths.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/tests/test_resource_client_user.py` & `livestyled-1.4.3/livestyled/tests/test_resource_client_user.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/tests/test_resource_device_preferences.py` & `livestyled-1.4.3/livestyled/tests/test_resource_device_preferences.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/tests/test_resource_screens.py` & `livestyled-1.4.3/livestyled/tests/test_resource_screens.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/tests/test_resource_widgets.py` & `livestyled-1.4.3/livestyled/tests/test_resource_widgets.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled/tests/utils.py` & `livestyled-1.4.3/livestyled/tests/utils.py`

 * *Files identical despite different names*

### Comparing `livestyled-1.4.2/livestyled.egg-info/SOURCES.txt` & `livestyled-1.4.3/livestyled.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 livestyled/__init__.py
 livestyled/client.py
 livestyled/resource_client.py
 livestyled/utils.py
 livestyled.egg-info/PKG-INFO
 livestyled.egg-info/SOURCES.txt
 livestyled.egg-info/dependency_links.txt
+livestyled.egg-info/entry_points.txt
 livestyled.egg-info/requires.txt
 livestyled.egg-info/top_level.txt
 livestyled/models/__init__.py
 livestyled/models/app.py
 livestyled/models/audience.py
 livestyled/models/audience_device.py
 livestyled/models/banner.py
```

### Comparing `livestyled-1.4.2/setup.py` & `livestyled-1.4.3/setup.py`

 * *Files identical despite different names*

