# Comparing `tmp/django-simple-captcha-0.5.8.zip` & `tmp/django-simple-captcha-0.5.9.zip`

## zipinfo {}

```diff
@@ -1,117 +1,118 @@
-Zip file size: 231608 bytes, number of entries: 115
--rw-r--r--  2.0 unx       57 b- defN 18-Jun-20 16:16 django-simple-captcha-0.5.8/.pep8
--rw-r--r--  2.0 unx     7135 b- defN 18-Jun-20 16:18 django-simple-captcha-0.5.8/CHANGES
--rw-r--r--  2.0 unx     1064 b- defN 14-May-08 15:40 django-simple-captcha-0.5.8/LICENSE
--rw-r--r--  2.0 unx      451 b- defN 15-Dec-04 08:55 django-simple-captcha-0.5.8/MANIFEST.in
--rw-r--r--  2.0 unx     2556 b- defN 18-Jun-20 16:20 django-simple-captcha-0.5.8/PKG-INFO
--rw-r--r--  2.0 unx     1362 b- defN 17-Dec-02 17:57 django-simple-captcha-0.5.8/README.rst
--rw-r--r--  2.0 unx       67 b- defN 18-Jun-20 16:20 django-simple-captcha-0.5.8/setup.cfg
--rw-r--r--  2.0 unx     2218 b- defN 18-Jun-20 16:16 django-simple-captcha-0.5.8/setup.py
--rw-r--r--  2.0 unx     2211 b- defN 18-Jun-20 16:16 django-simple-captcha-0.5.8/tox.ini
--rw-r--r--  2.0 unx      148 b- defN 18-Jun-20 16:16 django-simple-captcha-0.5.8/captcha/__init__.py
--rw-r--r--  2.0 unx     8984 b- defN 18-May-18 09:04 django-simple-captcha-0.5.8/captcha/fields.py
--rw-r--r--  2.0 unx     3121 b- defN 17-Nov-09 12:21 django-simple-captcha-0.5.8/captcha/helpers.py
--rw-r--r--  2.0 unx     2794 b- defN 17-Nov-09 12:21 django-simple-captcha-0.5.8/captcha/models.py
--rw-------  2.0 unx      429 b- defN 17-Nov-09 12:15 django-simple-captcha-0.5.8/captcha/urls.py
--rw-r--r--  2.0 unx     5962 b- defN 18-May-18 09:13 django-simple-captcha-0.5.8/captcha/views.py
--rw-r--r--  2.0 unx        0 b- defN 13-May-02 09:12 django-simple-captcha-0.5.8/captcha/conf/__init__.py
--rw-r--r--  2.0 unx     3693 b- defN 18-May-18 09:04 django-simple-captcha-0.5.8/captcha/conf/settings.py
--rw-r--r--  2.0 unx     5954 b- defN 13-May-02 09:12 django-simple-captcha-0.5.8/captcha/fonts/COPYRIGHT.TXT
--rw-r--r--  2.0 unx      320 b- defN 13-May-02 09:12 django-simple-captcha-0.5.8/captcha/fonts/README.TXT
--rw-r--r--  2.0 unx    65932 b- defN 13-May-02 09:12 django-simple-captcha-0.5.8/captcha/fonts/Vera.ttf
--rw-r--r--  2.0 unx      694 b- defN 18-Jun-20 16:17 django-simple-captcha-0.5.8/captcha/locale/bg/LC_MESSAGES/django.mo
--rw-------  2.0 unx     1060 b- defN 15-Aug-04 09:02 django-simple-captcha-0.5.8/captcha/locale/bg/LC_MESSAGES/django.po
--rw-r--r--  2.0 unx      638 b- defN 18-Jun-20 16:17 django-simple-captcha-0.5.8/captcha/locale/cs/LC_MESSAGES/django.mo
--rw-------  2.0 unx      950 b- defN 15-Aug-04 09:02 django-simple-captcha-0.5.8/captcha/locale/cs/LC_MESSAGES/django.po
--rw-r--r--  2.0 unx      675 b- defN 18-Jun-20 16:17 django-simple-captcha-0.5.8/captcha/locale/de/LC_MESSAGES/django.mo
--rw-------  2.0 unx     1002 b- defN 15-Aug-04 09:02 django-simple-captcha-0.5.8/captcha/locale/de/LC_MESSAGES/django.po
--rw-------  2.0 unx      904 b- defN 15-Aug-04 09:04 django-simple-captcha-0.5.8/captcha/locale/en/LC_MESSAGES/django.po
--rw-r--r--  2.0 unx      641 b- defN 18-Jun-20 16:17 django-simple-captcha-0.5.8/captcha/locale/es/LC_MESSAGES/django.mo
--rw-------  2.0 unx      968 b- defN 15-Aug-04 09:02 django-simple-captcha-0.5.8/captcha/locale/es/LC_MESSAGES/django.po
--rw-r--r--  2.0 unx      642 b- defN 18-Jun-20 16:17 django-simple-captcha-0.5.8/captcha/locale/fr/LC_MESSAGES/django.mo
--rw-------  2.0 unx      952 b- defN 15-Aug-04 09:02 django-simple-captcha-0.5.8/captcha/locale/fr/LC_MESSAGES/django.po
--rw-r--r--  2.0 unx      672 b- defN 18-Jun-20 16:17 django-simple-captcha-0.5.8/captcha/locale/it/LC_MESSAGES/django.mo
--rw-------  2.0 unx      994 b- defN 15-Aug-04 09:02 django-simple-captcha-0.5.8/captcha/locale/it/LC_MESSAGES/django.po
--rw-r--r--  2.0 unx      677 b- defN 18-Jun-20 16:17 django-simple-captcha-0.5.8/captcha/locale/ja/LC_MESSAGES/django.mo
--rw-------  2.0 unx     1007 b- defN 15-Aug-04 09:02 django-simple-captcha-0.5.8/captcha/locale/ja/LC_MESSAGES/django.po
--rw-r--r--  2.0 unx      671 b- defN 18-Jun-20 16:17 django-simple-captcha-0.5.8/captcha/locale/nl/LC_MESSAGES/django.mo
--rw-------  2.0 unx     1024 b- defN 15-Aug-04 09:02 django-simple-captcha-0.5.8/captcha/locale/nl/LC_MESSAGES/django.po
--rw-------  2.0 unx      721 b- defN 18-Jun-20 16:17 django-simple-captcha-0.5.8/captcha/locale/pl/LC_MESSAGES/django.mo
--rw-------  2.0 unx     1107 b- defN 16-Mar-13 18:42 django-simple-captcha-0.5.8/captcha/locale/pl/LC_MESSAGES/django.po
--rw-r--r--  2.0 unx      654 b- defN 18-Jun-20 16:17 django-simple-captcha-0.5.8/captcha/locale/pt_BR/LC_MESSAGES/django.mo
--rw-------  2.0 unx     1025 b- defN 15-Aug-04 09:02 django-simple-captcha-0.5.8/captcha/locale/pt_BR/LC_MESSAGES/django.po
--rw-r--r--  2.0 unx      765 b- defN 18-Jun-20 16:17 django-simple-captcha-0.5.8/captcha/locale/ru/LC_MESSAGES/django.mo
--rw-------  2.0 unx     1053 b- defN 15-Aug-04 09:02 django-simple-captcha-0.5.8/captcha/locale/ru/LC_MESSAGES/django.po
--rw-r--r--  2.0 unx      647 b- defN 18-Jun-20 16:17 django-simple-captcha-0.5.8/captcha/locale/sk/LC_MESSAGES/django.mo
--rw-------  2.0 unx      994 b- defN 15-Aug-04 09:02 django-simple-captcha-0.5.8/captcha/locale/sk/LC_MESSAGES/django.po
--rw-r--r--  2.0 unx      646 b- defN 18-Jun-20 16:17 django-simple-captcha-0.5.8/captcha/locale/tr/LC_MESSAGES/django.mo
--rw-------  2.0 unx      978 b- defN 15-Aug-04 09:02 django-simple-captcha-0.5.8/captcha/locale/tr/LC_MESSAGES/django.po
--rw-r--r--  2.0 unx      756 b- defN 18-Jun-20 16:17 django-simple-captcha-0.5.8/captcha/locale/uk/LC_MESSAGES/django.mo
--rw-------  2.0 unx     1082 b- defN 15-Aug-04 09:02 django-simple-captcha-0.5.8/captcha/locale/uk/LC_MESSAGES/django.po
--rw-r--r--  2.0 unx      643 b- defN 18-Jun-20 16:17 django-simple-captcha-0.5.8/captcha/locale/zh_CN/LC_MESSAGES/django.mo
--rw-------  2.0 unx     1005 b- defN 15-Aug-04 09:02 django-simple-captcha-0.5.8/captcha/locale/zh_CN/LC_MESSAGES/django.po
--rw-r--r--  2.0 unx      643 b- defN 16-Nov-16 11:07 django-simple-captcha-0.5.8/captcha/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--  2.0 unx     1005 b- defN 16-Nov-16 11:07 django-simple-captcha-0.5.8/captcha/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--  2.0 unx        0 b- defN 13-May-02 09:12 django-simple-captcha-0.5.8/captcha/management/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 13-May-02 09:12 django-simple-captcha-0.5.8/captcha/management/commands/__init__.py
--rw-------  2.0 unx      860 b- defN 16-Sep-18 09:26 django-simple-captcha-0.5.8/captcha/management/commands/captcha_clean.py
--rw-r--r--  2.0 unx     1116 b- defN 16-Sep-18 09:12 django-simple-captcha-0.5.8/captcha/management/commands/captcha_create_pool.py
--rw-r--r--  2.0 unx      758 b- defN 14-Aug-03 18:24 django-simple-captcha-0.5.8/captcha/migrations/0001_initial.py
--rw-r--r--  2.0 unx        0 b- defN 18-Jun-20 16:16 django-simple-captcha-0.5.8/captcha/migrations/__init__.py
--rw-------  2.0 unx       40 b- defN 15-Dec-02 08:58 django-simple-captcha-0.5.8/captcha/templates/captcha/field.html
--rw-------  2.0 unx       72 b- defN 15-Dec-02 08:58 django-simple-captcha-0.5.8/captcha/templates/captcha/hidden_field.html
--rw-------  2.0 unx      231 b- defN 15-Dec-02 08:58 django-simple-captcha-0.5.8/captcha/templates/captcha/image.html
--rw-r--r--  2.0 unx      131 b- defN 16-Dec-22 09:37 django-simple-captcha-0.5.8/captcha/templates/captcha/text_field.html
--rw-r--r--  2.0 unx      314 b- defN 18-May-18 09:04 django-simple-captcha-0.5.8/captcha/templates/captcha/widgets/captcha.html
--rw-------  2.0 unx       58 b- defN 15-Jul-19 16:43 django-simple-captcha-0.5.8/captcha/tests/__init__.py
--rw-r--r--  2.0 unx    22582 b- defN 18-May-18 09:04 django-simple-captcha-0.5.8/captcha/tests/tests.py
--rw-r--r--  2.0 unx      792 b- defN 16-Sep-18 09:13 django-simple-captcha-0.5.8/captcha/tests/urls.py
--rw-r--r--  2.0 unx     3823 b- defN 18-Feb-07 13:23 django-simple-captcha-0.5.8/captcha/tests/views.py
--rw-r--r--  2.0 unx        1 b- defN 18-Jun-20 16:20 django-simple-captcha-0.5.8/django_simple_captcha.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx        1 b- defN 13-May-02 09:12 django-simple-captcha-0.5.8/django_simple_captcha.egg-info/not-zip-safe
--rw-r--r--  2.0 unx     2556 b- defN 18-Jun-20 16:20 django-simple-captcha-0.5.8/django_simple_captcha.egg-info/PKG-INFO
--rw-r--r--  2.0 unx       93 b- defN 18-Jun-20 16:20 django-simple-captcha-0.5.8/django_simple_captcha.egg-info/requires.txt
--rw-r--r--  2.0 unx     4082 b- defN 18-Jun-20 16:20 django-simple-captcha-0.5.8/django_simple_captcha.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx        8 b- defN 18-Jun-20 16:20 django-simple-captcha-0.5.8/django_simple_captcha.egg-info/top_level.txt
--rw-r--r--  2.0 unx    11330 b- defN 18-May-18 09:04 django-simple-captcha-0.5.8/docs/advanced.rst
--rw-r--r--  2.0 unx     7135 b- defN 18-Jun-20 16:18 django-simple-captcha-0.5.8/docs/changes.rst
--rw-r--r--  2.0 unx     6538 b- defN 18-Jun-20 16:16 django-simple-captcha-0.5.8/docs/conf.py
--rw-------  2.0 unx     1127 b- defN 18-May-18 09:08 django-simple-captcha-0.5.8/docs/index.rst
--rw-r--r--  2.0 unx     3152 b- defN 13-May-02 09:12 django-simple-captcha-0.5.8/docs/Makefile
--rw-r--r--  2.0 unx     4976 b- defN 18-May-18 09:11 django-simple-captcha-0.5.8/docs/usage.rst
--rw-r--r--  2.0 unx     9633 b- defN 15-Mar-28 15:16 django-simple-captcha-0.5.8/docs/_static/captcha3.png
--rw-r--r--  2.0 unx     7859 b- defN 15-Mar-28 15:15 django-simple-captcha-0.5.8/docs/_static/dict.png
--rw-r--r--  2.0 unx     7491 b- defN 15-Mar-28 15:14 django-simple-captcha-0.5.8/docs/_static/math.png
--rw-r--r--  2.0 unx     8136 b- defN 15-Mar-28 15:14 django-simple-captcha-0.5.8/docs/_static/random_chars.png
--rw-r--r--  2.0 unx      126 b- defN 13-May-02 09:12 django-simple-captcha-0.5.8/testproject/.coveragerc
--rw-r--r--  2.0 unx        0 b- defN 13-May-02 09:12 django-simple-captcha-0.5.8/testproject/__init__.py
--rw-r--r--  2.0 unx      184 b- defN 17-Nov-08 13:38 django-simple-captcha-0.5.8/testproject/coverage.sh
--rw-r--r--  2.0 unx      127 b- defN 15-Apr-04 21:03 django-simple-captcha-0.5.8/testproject/forms.py
--rw-r--r--  2.0 unx       81 b- defN 18-Jun-20 16:16 django-simple-captcha-0.5.8/testproject/jinja2_settings.py
--rw-r--r--  2.0 unx      973 b- defN 13-May-02 09:12 django-simple-captcha-0.5.8/testproject/manage.py
--rw-r--r--  2.0 unx     1940 b- defN 17-Nov-08 13:38 django-simple-captcha-0.5.8/testproject/settings.py
--rw-r--r--  2.0 unx      240 b- defN 17-Feb-21 10:53 django-simple-captcha-0.5.8/testproject/urls.py
--rw-r--r--  2.0 unx      380 b- defN 17-Feb-21 11:48 django-simple-captcha-0.5.8/testproject/views.py
--rw-r--r--  2.0 unx     4392 b- defN 17-Nov-08 13:41 django-simple-captcha-0.5.8/testproject/htmlcov/_Users_marco_Code_django-simple-captcha_captcha___init___py.html
--rw-r--r--  2.0 unx     2700 b- defN 17-Nov-08 13:41 django-simple-captcha-0.5.8/testproject/htmlcov/_Users_marco_Code_django-simple-captcha_captcha_conf___init___py.html
--rw-r--r--  2.0 unx    24907 b- defN 17-Nov-08 13:41 django-simple-captcha-0.5.8/testproject/htmlcov/_Users_marco_Code_django-simple-captcha_captcha_conf_settings_py.html
--rw-r--r--  2.0 unx    68253 b- defN 17-Nov-08 13:41 django-simple-captcha-0.5.8/testproject/htmlcov/_Users_marco_Code_django-simple-captcha_captcha_fields_py.html
--rw-r--r--  2.0 unx    34108 b- defN 17-Nov-08 13:41 django-simple-captcha-0.5.8/testproject/htmlcov/_Users_marco_Code_django-simple-captcha_captcha_helpers_py.html
--rw-r--r--  2.0 unx    27440 b- defN 17-Nov-08 13:41 django-simple-captcha-0.5.8/testproject/htmlcov/_Users_marco_Code_django-simple-captcha_captcha_models_py.html
--rw-r--r--  2.0 unx     6218 b- defN 17-Nov-08 13:41 django-simple-captcha-0.5.8/testproject/htmlcov/_Users_marco_Code_django-simple-captcha_captcha_urls_py.html
--rw-r--r--  2.0 unx    58169 b- defN 17-Nov-08 13:41 django-simple-captcha-0.5.8/testproject/htmlcov/_Users_marco_Code_django-simple-captcha_captcha_views_py.html
--rw-r--r--  2.0 unx    18458 b- defN 17-Nov-08 13:41 django-simple-captcha-0.5.8/testproject/htmlcov/coverage_html.js
--rw-r--r--  2.0 unx     6779 b- defN 17-Nov-08 13:41 django-simple-captcha-0.5.8/testproject/htmlcov/index.html
--rw-r--r--  2.0 unx      731 b- defN 17-Nov-08 13:41 django-simple-captcha-0.5.8/testproject/htmlcov/jquery.ba-throttle-debounce.min.js
--rw-r--r--  2.0 unx     3065 b- defN 17-Nov-08 13:41 django-simple-captcha-0.5.8/testproject/htmlcov/jquery.hotkeys.js
--rw-r--r--  2.0 unx     1502 b- defN 17-Nov-08 13:41 django-simple-captcha-0.5.8/testproject/htmlcov/jquery.isonscreen.js
--rw-r--r--  2.0 unx    95785 b- defN 17-Nov-08 13:41 django-simple-captcha-0.5.8/testproject/htmlcov/jquery.min.js
--rw-r--r--  2.0 unx    12795 b- defN 17-Nov-08 13:41 django-simple-captcha-0.5.8/testproject/htmlcov/jquery.tablesorter.min.js
--rw-r--r--  2.0 unx      112 b- defN 17-Nov-08 13:41 django-simple-captcha-0.5.8/testproject/htmlcov/keybd_closed.png
--rw-r--r--  2.0 unx      112 b- defN 17-Nov-08 13:41 django-simple-captcha-0.5.8/testproject/htmlcov/keybd_open.png
--rw-r--r--  2.0 unx     2526 b- defN 17-Nov-08 13:41 django-simple-captcha-0.5.8/testproject/htmlcov/status.json
--rw-r--r--  2.0 unx     6757 b- defN 17-Nov-08 13:41 django-simple-captcha-0.5.8/testproject/htmlcov/style.css
--rw-r--r--  2.0 unx      225 b- defN 15-Apr-04 21:03 django-simple-captcha-0.5.8/testproject/templates/home.html
--rw-------  2.0 unx      245 b- defN 17-Nov-04 15:26 django-simple-captcha-0.5.8/testproject/templates/captcha_test/image.html
--rw-r--r--  2.0 unx      486 b- defN 17-Nov-09 12:21 django-simple-captcha-0.5.8/testproject/templates/captcha_test/image_html5_audio.html
-115 files, 627064 bytes uncompressed, 208452 bytes compressed:  66.8%
+Zip file size: 232013 bytes, number of entries: 116
+-rw-r--r--  2.0 unx       57 b- defN 18-Jun-20 16:16 django-simple-captcha-0.5.9/.pep8
+-rw-r--r--  2.0 unx     7218 b- defN 18-Jun-21 19:34 django-simple-captcha-0.5.9/CHANGES
+-rw-r--r--  2.0 unx     1064 b- defN 14-May-08 15:40 django-simple-captcha-0.5.9/LICENSE
+-rw-r--r--  2.0 unx      486 b- defN 18-Jun-21 19:34 django-simple-captcha-0.5.9/MANIFEST.in
+-rw-r--r--  2.0 unx     2556 b- defN 18-Jun-21 19:37 django-simple-captcha-0.5.9/PKG-INFO
+-rw-r--r--  2.0 unx     1362 b- defN 17-Dec-02 17:57 django-simple-captcha-0.5.9/README.rst
+-rw-r--r--  2.0 unx       67 b- defN 18-Jun-21 19:37 django-simple-captcha-0.5.9/setup.cfg
+-rw-r--r--  2.0 unx     2221 b- defN 18-Jun-20 21:49 django-simple-captcha-0.5.9/setup.py
+-rw-r--r--  2.0 unx     2211 b- defN 18-Jun-20 16:16 django-simple-captcha-0.5.9/tox.ini
+-rw-r--r--  2.0 unx      148 b- defN 18-Jun-21 19:35 django-simple-captcha-0.5.9/captcha/__init__.py
+-rw-r--r--  2.0 unx     8984 b- defN 18-May-18 09:04 django-simple-captcha-0.5.9/captcha/fields.py
+-rw-r--r--  2.0 unx     3121 b- defN 17-Nov-09 12:21 django-simple-captcha-0.5.9/captcha/helpers.py
+-rw-r--r--  2.0 unx     2794 b- defN 17-Nov-09 12:21 django-simple-captcha-0.5.9/captcha/models.py
+-rw-------  2.0 unx      429 b- defN 17-Nov-09 12:15 django-simple-captcha-0.5.9/captcha/urls.py
+-rw-r--r--  2.0 unx     5962 b- defN 18-May-18 09:13 django-simple-captcha-0.5.9/captcha/views.py
+-rw-r--r--  2.0 unx        0 b- defN 13-May-02 09:12 django-simple-captcha-0.5.9/captcha/conf/__init__.py
+-rw-r--r--  2.0 unx     3693 b- defN 18-May-18 09:04 django-simple-captcha-0.5.9/captcha/conf/settings.py
+-rw-r--r--  2.0 unx     5954 b- defN 13-May-02 09:12 django-simple-captcha-0.5.9/captcha/fonts/COPYRIGHT.TXT
+-rw-r--r--  2.0 unx      320 b- defN 13-May-02 09:12 django-simple-captcha-0.5.9/captcha/fonts/README.TXT
+-rw-r--r--  2.0 unx    65932 b- defN 13-May-02 09:12 django-simple-captcha-0.5.9/captcha/fonts/Vera.ttf
+-rw-r--r--  2.0 unx      186 b- defN 18-Jun-20 16:16 django-simple-captcha-0.5.9/captcha/jinja2/captcha/widgets/captcha.html
+-rw-r--r--  2.0 unx      694 b- defN 18-Jun-20 21:51 django-simple-captcha-0.5.9/captcha/locale/bg/LC_MESSAGES/django.mo
+-rw-------  2.0 unx     1060 b- defN 15-Aug-04 09:02 django-simple-captcha-0.5.9/captcha/locale/bg/LC_MESSAGES/django.po
+-rw-r--r--  2.0 unx      638 b- defN 18-Jun-20 21:51 django-simple-captcha-0.5.9/captcha/locale/cs/LC_MESSAGES/django.mo
+-rw-------  2.0 unx      950 b- defN 15-Aug-04 09:02 django-simple-captcha-0.5.9/captcha/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--  2.0 unx      675 b- defN 18-Jun-20 21:51 django-simple-captcha-0.5.9/captcha/locale/de/LC_MESSAGES/django.mo
+-rw-------  2.0 unx     1002 b- defN 15-Aug-04 09:02 django-simple-captcha-0.5.9/captcha/locale/de/LC_MESSAGES/django.po
+-rw-------  2.0 unx      904 b- defN 15-Aug-04 09:04 django-simple-captcha-0.5.9/captcha/locale/en/LC_MESSAGES/django.po
+-rw-r--r--  2.0 unx      641 b- defN 18-Jun-20 21:51 django-simple-captcha-0.5.9/captcha/locale/es/LC_MESSAGES/django.mo
+-rw-------  2.0 unx      968 b- defN 15-Aug-04 09:02 django-simple-captcha-0.5.9/captcha/locale/es/LC_MESSAGES/django.po
+-rw-r--r--  2.0 unx      642 b- defN 18-Jun-20 21:51 django-simple-captcha-0.5.9/captcha/locale/fr/LC_MESSAGES/django.mo
+-rw-------  2.0 unx      952 b- defN 15-Aug-04 09:02 django-simple-captcha-0.5.9/captcha/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--  2.0 unx      672 b- defN 18-Jun-20 21:51 django-simple-captcha-0.5.9/captcha/locale/it/LC_MESSAGES/django.mo
+-rw-------  2.0 unx      994 b- defN 15-Aug-04 09:02 django-simple-captcha-0.5.9/captcha/locale/it/LC_MESSAGES/django.po
+-rw-r--r--  2.0 unx      677 b- defN 18-Jun-20 21:51 django-simple-captcha-0.5.9/captcha/locale/ja/LC_MESSAGES/django.mo
+-rw-------  2.0 unx     1007 b- defN 15-Aug-04 09:02 django-simple-captcha-0.5.9/captcha/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--  2.0 unx      671 b- defN 18-Jun-20 21:51 django-simple-captcha-0.5.9/captcha/locale/nl/LC_MESSAGES/django.mo
+-rw-------  2.0 unx     1024 b- defN 15-Aug-04 09:02 django-simple-captcha-0.5.9/captcha/locale/nl/LC_MESSAGES/django.po
+-rw-------  2.0 unx      721 b- defN 18-Jun-20 21:51 django-simple-captcha-0.5.9/captcha/locale/pl/LC_MESSAGES/django.mo
+-rw-------  2.0 unx     1107 b- defN 16-Mar-13 18:42 django-simple-captcha-0.5.9/captcha/locale/pl/LC_MESSAGES/django.po
+-rw-r--r--  2.0 unx      654 b- defN 18-Jun-20 21:51 django-simple-captcha-0.5.9/captcha/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-------  2.0 unx     1025 b- defN 15-Aug-04 09:02 django-simple-captcha-0.5.9/captcha/locale/pt_BR/LC_MESSAGES/django.po
+-rw-r--r--  2.0 unx      765 b- defN 18-Jun-20 21:51 django-simple-captcha-0.5.9/captcha/locale/ru/LC_MESSAGES/django.mo
+-rw-------  2.0 unx     1053 b- defN 15-Aug-04 09:02 django-simple-captcha-0.5.9/captcha/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--  2.0 unx      647 b- defN 18-Jun-20 21:51 django-simple-captcha-0.5.9/captcha/locale/sk/LC_MESSAGES/django.mo
+-rw-------  2.0 unx      994 b- defN 15-Aug-04 09:02 django-simple-captcha-0.5.9/captcha/locale/sk/LC_MESSAGES/django.po
+-rw-r--r--  2.0 unx      646 b- defN 18-Jun-20 21:51 django-simple-captcha-0.5.9/captcha/locale/tr/LC_MESSAGES/django.mo
+-rw-------  2.0 unx      978 b- defN 15-Aug-04 09:02 django-simple-captcha-0.5.9/captcha/locale/tr/LC_MESSAGES/django.po
+-rw-r--r--  2.0 unx      756 b- defN 18-Jun-20 21:51 django-simple-captcha-0.5.9/captcha/locale/uk/LC_MESSAGES/django.mo
+-rw-------  2.0 unx     1082 b- defN 15-Aug-04 09:02 django-simple-captcha-0.5.9/captcha/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--  2.0 unx      643 b- defN 18-Jun-20 21:51 django-simple-captcha-0.5.9/captcha/locale/zh_CN/LC_MESSAGES/django.mo
+-rw-------  2.0 unx     1005 b- defN 15-Aug-04 09:02 django-simple-captcha-0.5.9/captcha/locale/zh_CN/LC_MESSAGES/django.po
+-rw-r--r--  2.0 unx      643 b- defN 16-Nov-16 11:07 django-simple-captcha-0.5.9/captcha/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--  2.0 unx     1005 b- defN 16-Nov-16 11:07 django-simple-captcha-0.5.9/captcha/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--  2.0 unx        0 b- defN 13-May-02 09:12 django-simple-captcha-0.5.9/captcha/management/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 13-May-02 09:12 django-simple-captcha-0.5.9/captcha/management/commands/__init__.py
+-rw-------  2.0 unx      860 b- defN 16-Sep-18 09:26 django-simple-captcha-0.5.9/captcha/management/commands/captcha_clean.py
+-rw-r--r--  2.0 unx     1116 b- defN 16-Sep-18 09:12 django-simple-captcha-0.5.9/captcha/management/commands/captcha_create_pool.py
+-rw-r--r--  2.0 unx      758 b- defN 14-Aug-03 18:24 django-simple-captcha-0.5.9/captcha/migrations/0001_initial.py
+-rw-r--r--  2.0 unx        0 b- defN 18-Jun-20 16:16 django-simple-captcha-0.5.9/captcha/migrations/__init__.py
+-rw-------  2.0 unx       40 b- defN 15-Dec-02 08:58 django-simple-captcha-0.5.9/captcha/templates/captcha/field.html
+-rw-------  2.0 unx       72 b- defN 15-Dec-02 08:58 django-simple-captcha-0.5.9/captcha/templates/captcha/hidden_field.html
+-rw-------  2.0 unx      231 b- defN 15-Dec-02 08:58 django-simple-captcha-0.5.9/captcha/templates/captcha/image.html
+-rw-r--r--  2.0 unx      131 b- defN 16-Dec-22 09:37 django-simple-captcha-0.5.9/captcha/templates/captcha/text_field.html
+-rw-r--r--  2.0 unx      314 b- defN 18-May-18 09:04 django-simple-captcha-0.5.9/captcha/templates/captcha/widgets/captcha.html
+-rw-------  2.0 unx       58 b- defN 15-Jul-19 16:43 django-simple-captcha-0.5.9/captcha/tests/__init__.py
+-rw-r--r--  2.0 unx    22582 b- defN 18-May-18 09:04 django-simple-captcha-0.5.9/captcha/tests/tests.py
+-rw-r--r--  2.0 unx      792 b- defN 16-Sep-18 09:13 django-simple-captcha-0.5.9/captcha/tests/urls.py
+-rw-r--r--  2.0 unx     3823 b- defN 18-Feb-07 13:23 django-simple-captcha-0.5.9/captcha/tests/views.py
+-rw-r--r--  2.0 unx        1 b- defN 18-Jun-21 19:37 django-simple-captcha-0.5.9/django_simple_captcha.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx        1 b- defN 13-May-02 09:12 django-simple-captcha-0.5.9/django_simple_captcha.egg-info/not-zip-safe
+-rw-r--r--  2.0 unx     2556 b- defN 18-Jun-21 19:37 django-simple-captcha-0.5.9/django_simple_captcha.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx       96 b- defN 18-Jun-21 19:37 django-simple-captcha-0.5.9/django_simple_captcha.egg-info/requires.txt
+-rw-r--r--  2.0 unx     4126 b- defN 18-Jun-21 19:37 django-simple-captcha-0.5.9/django_simple_captcha.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx        8 b- defN 18-Jun-21 19:37 django-simple-captcha-0.5.9/django_simple_captcha.egg-info/top_level.txt
+-rw-r--r--  2.0 unx    11330 b- defN 18-May-18 09:04 django-simple-captcha-0.5.9/docs/advanced.rst
+-rw-r--r--  2.0 unx     7218 b- defN 18-Jun-21 19:34 django-simple-captcha-0.5.9/docs/changes.rst
+-rw-r--r--  2.0 unx     6538 b- defN 18-Jun-21 19:37 django-simple-captcha-0.5.9/docs/conf.py
+-rw-------  2.0 unx     1127 b- defN 18-May-18 09:08 django-simple-captcha-0.5.9/docs/index.rst
+-rw-r--r--  2.0 unx     3152 b- defN 13-May-02 09:12 django-simple-captcha-0.5.9/docs/Makefile
+-rw-r--r--  2.0 unx     4976 b- defN 18-May-18 09:11 django-simple-captcha-0.5.9/docs/usage.rst
+-rw-r--r--  2.0 unx     9633 b- defN 15-Mar-28 15:16 django-simple-captcha-0.5.9/docs/_static/captcha3.png
+-rw-r--r--  2.0 unx     7859 b- defN 15-Mar-28 15:15 django-simple-captcha-0.5.9/docs/_static/dict.png
+-rw-r--r--  2.0 unx     7491 b- defN 15-Mar-28 15:14 django-simple-captcha-0.5.9/docs/_static/math.png
+-rw-r--r--  2.0 unx     8136 b- defN 15-Mar-28 15:14 django-simple-captcha-0.5.9/docs/_static/random_chars.png
+-rw-r--r--  2.0 unx      126 b- defN 13-May-02 09:12 django-simple-captcha-0.5.9/testproject/.coveragerc
+-rw-r--r--  2.0 unx        0 b- defN 13-May-02 09:12 django-simple-captcha-0.5.9/testproject/__init__.py
+-rw-r--r--  2.0 unx      184 b- defN 17-Nov-08 13:38 django-simple-captcha-0.5.9/testproject/coverage.sh
+-rw-r--r--  2.0 unx      127 b- defN 15-Apr-04 21:03 django-simple-captcha-0.5.9/testproject/forms.py
+-rw-r--r--  2.0 unx       81 b- defN 18-Jun-20 16:16 django-simple-captcha-0.5.9/testproject/jinja2_settings.py
+-rw-r--r--  2.0 unx      973 b- defN 13-May-02 09:12 django-simple-captcha-0.5.9/testproject/manage.py
+-rw-r--r--  2.0 unx     1940 b- defN 17-Nov-08 13:38 django-simple-captcha-0.5.9/testproject/settings.py
+-rw-r--r--  2.0 unx      240 b- defN 17-Feb-21 10:53 django-simple-captcha-0.5.9/testproject/urls.py
+-rw-r--r--  2.0 unx      380 b- defN 17-Feb-21 11:48 django-simple-captcha-0.5.9/testproject/views.py
+-rw-r--r--  2.0 unx     4392 b- defN 17-Nov-08 13:41 django-simple-captcha-0.5.9/testproject/htmlcov/_Users_marco_Code_django-simple-captcha_captcha___init___py.html
+-rw-r--r--  2.0 unx     2700 b- defN 17-Nov-08 13:41 django-simple-captcha-0.5.9/testproject/htmlcov/_Users_marco_Code_django-simple-captcha_captcha_conf___init___py.html
+-rw-r--r--  2.0 unx    24907 b- defN 17-Nov-08 13:41 django-simple-captcha-0.5.9/testproject/htmlcov/_Users_marco_Code_django-simple-captcha_captcha_conf_settings_py.html
+-rw-r--r--  2.0 unx    68253 b- defN 17-Nov-08 13:41 django-simple-captcha-0.5.9/testproject/htmlcov/_Users_marco_Code_django-simple-captcha_captcha_fields_py.html
+-rw-r--r--  2.0 unx    34108 b- defN 17-Nov-08 13:41 django-simple-captcha-0.5.9/testproject/htmlcov/_Users_marco_Code_django-simple-captcha_captcha_helpers_py.html
+-rw-r--r--  2.0 unx    27440 b- defN 17-Nov-08 13:41 django-simple-captcha-0.5.9/testproject/htmlcov/_Users_marco_Code_django-simple-captcha_captcha_models_py.html
+-rw-r--r--  2.0 unx     6218 b- defN 17-Nov-08 13:41 django-simple-captcha-0.5.9/testproject/htmlcov/_Users_marco_Code_django-simple-captcha_captcha_urls_py.html
+-rw-r--r--  2.0 unx    58169 b- defN 17-Nov-08 13:41 django-simple-captcha-0.5.9/testproject/htmlcov/_Users_marco_Code_django-simple-captcha_captcha_views_py.html
+-rw-r--r--  2.0 unx    18458 b- defN 17-Nov-08 13:41 django-simple-captcha-0.5.9/testproject/htmlcov/coverage_html.js
+-rw-r--r--  2.0 unx     6779 b- defN 17-Nov-08 13:41 django-simple-captcha-0.5.9/testproject/htmlcov/index.html
+-rw-r--r--  2.0 unx      731 b- defN 17-Nov-08 13:41 django-simple-captcha-0.5.9/testproject/htmlcov/jquery.ba-throttle-debounce.min.js
+-rw-r--r--  2.0 unx     3065 b- defN 17-Nov-08 13:41 django-simple-captcha-0.5.9/testproject/htmlcov/jquery.hotkeys.js
+-rw-r--r--  2.0 unx     1502 b- defN 17-Nov-08 13:41 django-simple-captcha-0.5.9/testproject/htmlcov/jquery.isonscreen.js
+-rw-r--r--  2.0 unx    95785 b- defN 17-Nov-08 13:41 django-simple-captcha-0.5.9/testproject/htmlcov/jquery.min.js
+-rw-r--r--  2.0 unx    12795 b- defN 17-Nov-08 13:41 django-simple-captcha-0.5.9/testproject/htmlcov/jquery.tablesorter.min.js
+-rw-r--r--  2.0 unx      112 b- defN 17-Nov-08 13:41 django-simple-captcha-0.5.9/testproject/htmlcov/keybd_closed.png
+-rw-r--r--  2.0 unx      112 b- defN 17-Nov-08 13:41 django-simple-captcha-0.5.9/testproject/htmlcov/keybd_open.png
+-rw-r--r--  2.0 unx     2526 b- defN 17-Nov-08 13:41 django-simple-captcha-0.5.9/testproject/htmlcov/status.json
+-rw-r--r--  2.0 unx     6757 b- defN 17-Nov-08 13:41 django-simple-captcha-0.5.9/testproject/htmlcov/style.css
+-rw-r--r--  2.0 unx      225 b- defN 15-Apr-04 21:03 django-simple-captcha-0.5.9/testproject/templates/home.html
+-rw-------  2.0 unx      245 b- defN 17-Nov-04 15:26 django-simple-captcha-0.5.9/testproject/templates/captcha_test/image.html
+-rw-r--r--  2.0 unx      486 b- defN 17-Nov-09 12:21 django-simple-captcha-0.5.9/testproject/templates/captcha_test/image_html5_audio.html
+116 files, 627501 bytes uncompressed, 208639 bytes compressed:  66.8%
```

## zipnote {}

```diff
@@ -1,346 +1,349 @@
-Filename: django-simple-captcha-0.5.8/.pep8
+Filename: django-simple-captcha-0.5.9/.pep8
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/CHANGES
+Filename: django-simple-captcha-0.5.9/CHANGES
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/LICENSE
+Filename: django-simple-captcha-0.5.9/LICENSE
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/MANIFEST.in
+Filename: django-simple-captcha-0.5.9/MANIFEST.in
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/PKG-INFO
+Filename: django-simple-captcha-0.5.9/PKG-INFO
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/README.rst
+Filename: django-simple-captcha-0.5.9/README.rst
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/setup.cfg
+Filename: django-simple-captcha-0.5.9/setup.cfg
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/setup.py
+Filename: django-simple-captcha-0.5.9/setup.py
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/tox.ini
+Filename: django-simple-captcha-0.5.9/tox.ini
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/__init__.py
+Filename: django-simple-captcha-0.5.9/captcha/__init__.py
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/fields.py
+Filename: django-simple-captcha-0.5.9/captcha/fields.py
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/helpers.py
+Filename: django-simple-captcha-0.5.9/captcha/helpers.py
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/models.py
+Filename: django-simple-captcha-0.5.9/captcha/models.py
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/urls.py
+Filename: django-simple-captcha-0.5.9/captcha/urls.py
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/views.py
+Filename: django-simple-captcha-0.5.9/captcha/views.py
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/conf/__init__.py
+Filename: django-simple-captcha-0.5.9/captcha/conf/__init__.py
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/conf/settings.py
+Filename: django-simple-captcha-0.5.9/captcha/conf/settings.py
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/fonts/COPYRIGHT.TXT
+Filename: django-simple-captcha-0.5.9/captcha/fonts/COPYRIGHT.TXT
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/fonts/README.TXT
+Filename: django-simple-captcha-0.5.9/captcha/fonts/README.TXT
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/fonts/Vera.ttf
+Filename: django-simple-captcha-0.5.9/captcha/fonts/Vera.ttf
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/locale/bg/LC_MESSAGES/django.mo
+Filename: django-simple-captcha-0.5.9/captcha/jinja2/captcha/widgets/captcha.html
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/locale/bg/LC_MESSAGES/django.po
+Filename: django-simple-captcha-0.5.9/captcha/locale/bg/LC_MESSAGES/django.mo
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/locale/cs/LC_MESSAGES/django.mo
+Filename: django-simple-captcha-0.5.9/captcha/locale/bg/LC_MESSAGES/django.po
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/locale/cs/LC_MESSAGES/django.po
+Filename: django-simple-captcha-0.5.9/captcha/locale/cs/LC_MESSAGES/django.mo
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/locale/de/LC_MESSAGES/django.mo
+Filename: django-simple-captcha-0.5.9/captcha/locale/cs/LC_MESSAGES/django.po
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/locale/de/LC_MESSAGES/django.po
+Filename: django-simple-captcha-0.5.9/captcha/locale/de/LC_MESSAGES/django.mo
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/locale/en/LC_MESSAGES/django.po
+Filename: django-simple-captcha-0.5.9/captcha/locale/de/LC_MESSAGES/django.po
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/locale/es/LC_MESSAGES/django.mo
+Filename: django-simple-captcha-0.5.9/captcha/locale/en/LC_MESSAGES/django.po
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/locale/es/LC_MESSAGES/django.po
+Filename: django-simple-captcha-0.5.9/captcha/locale/es/LC_MESSAGES/django.mo
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/locale/fr/LC_MESSAGES/django.mo
+Filename: django-simple-captcha-0.5.9/captcha/locale/es/LC_MESSAGES/django.po
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/locale/fr/LC_MESSAGES/django.po
+Filename: django-simple-captcha-0.5.9/captcha/locale/fr/LC_MESSAGES/django.mo
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/locale/it/LC_MESSAGES/django.mo
+Filename: django-simple-captcha-0.5.9/captcha/locale/fr/LC_MESSAGES/django.po
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/locale/it/LC_MESSAGES/django.po
+Filename: django-simple-captcha-0.5.9/captcha/locale/it/LC_MESSAGES/django.mo
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/locale/ja/LC_MESSAGES/django.mo
+Filename: django-simple-captcha-0.5.9/captcha/locale/it/LC_MESSAGES/django.po
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/locale/ja/LC_MESSAGES/django.po
+Filename: django-simple-captcha-0.5.9/captcha/locale/ja/LC_MESSAGES/django.mo
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/locale/nl/LC_MESSAGES/django.mo
+Filename: django-simple-captcha-0.5.9/captcha/locale/ja/LC_MESSAGES/django.po
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/locale/nl/LC_MESSAGES/django.po
+Filename: django-simple-captcha-0.5.9/captcha/locale/nl/LC_MESSAGES/django.mo
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/locale/pl/LC_MESSAGES/django.mo
+Filename: django-simple-captcha-0.5.9/captcha/locale/nl/LC_MESSAGES/django.po
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/locale/pl/LC_MESSAGES/django.po
+Filename: django-simple-captcha-0.5.9/captcha/locale/pl/LC_MESSAGES/django.mo
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/locale/pt_BR/LC_MESSAGES/django.mo
+Filename: django-simple-captcha-0.5.9/captcha/locale/pl/LC_MESSAGES/django.po
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/locale/pt_BR/LC_MESSAGES/django.po
+Filename: django-simple-captcha-0.5.9/captcha/locale/pt_BR/LC_MESSAGES/django.mo
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/locale/ru/LC_MESSAGES/django.mo
+Filename: django-simple-captcha-0.5.9/captcha/locale/pt_BR/LC_MESSAGES/django.po
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/locale/ru/LC_MESSAGES/django.po
+Filename: django-simple-captcha-0.5.9/captcha/locale/ru/LC_MESSAGES/django.mo
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/locale/sk/LC_MESSAGES/django.mo
+Filename: django-simple-captcha-0.5.9/captcha/locale/ru/LC_MESSAGES/django.po
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/locale/sk/LC_MESSAGES/django.po
+Filename: django-simple-captcha-0.5.9/captcha/locale/sk/LC_MESSAGES/django.mo
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/locale/tr/LC_MESSAGES/django.mo
+Filename: django-simple-captcha-0.5.9/captcha/locale/sk/LC_MESSAGES/django.po
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/locale/tr/LC_MESSAGES/django.po
+Filename: django-simple-captcha-0.5.9/captcha/locale/tr/LC_MESSAGES/django.mo
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/locale/uk/LC_MESSAGES/django.mo
+Filename: django-simple-captcha-0.5.9/captcha/locale/tr/LC_MESSAGES/django.po
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/locale/uk/LC_MESSAGES/django.po
+Filename: django-simple-captcha-0.5.9/captcha/locale/uk/LC_MESSAGES/django.mo
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/locale/zh_CN/LC_MESSAGES/django.mo
+Filename: django-simple-captcha-0.5.9/captcha/locale/uk/LC_MESSAGES/django.po
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/locale/zh_CN/LC_MESSAGES/django.po
+Filename: django-simple-captcha-0.5.9/captcha/locale/zh_CN/LC_MESSAGES/django.mo
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/locale/zh_Hans/LC_MESSAGES/django.mo
+Filename: django-simple-captcha-0.5.9/captcha/locale/zh_CN/LC_MESSAGES/django.po
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/locale/zh_Hans/LC_MESSAGES/django.po
+Filename: django-simple-captcha-0.5.9/captcha/locale/zh_Hans/LC_MESSAGES/django.mo
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/management/__init__.py
+Filename: django-simple-captcha-0.5.9/captcha/locale/zh_Hans/LC_MESSAGES/django.po
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/management/commands/__init__.py
+Filename: django-simple-captcha-0.5.9/captcha/management/__init__.py
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/management/commands/captcha_clean.py
+Filename: django-simple-captcha-0.5.9/captcha/management/commands/__init__.py
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/management/commands/captcha_create_pool.py
+Filename: django-simple-captcha-0.5.9/captcha/management/commands/captcha_clean.py
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/migrations/0001_initial.py
+Filename: django-simple-captcha-0.5.9/captcha/management/commands/captcha_create_pool.py
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/migrations/__init__.py
+Filename: django-simple-captcha-0.5.9/captcha/migrations/0001_initial.py
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/templates/captcha/field.html
+Filename: django-simple-captcha-0.5.9/captcha/migrations/__init__.py
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/templates/captcha/hidden_field.html
+Filename: django-simple-captcha-0.5.9/captcha/templates/captcha/field.html
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/templates/captcha/image.html
+Filename: django-simple-captcha-0.5.9/captcha/templates/captcha/hidden_field.html
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/templates/captcha/text_field.html
+Filename: django-simple-captcha-0.5.9/captcha/templates/captcha/image.html
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/templates/captcha/widgets/captcha.html
+Filename: django-simple-captcha-0.5.9/captcha/templates/captcha/text_field.html
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/tests/__init__.py
+Filename: django-simple-captcha-0.5.9/captcha/templates/captcha/widgets/captcha.html
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/tests/tests.py
+Filename: django-simple-captcha-0.5.9/captcha/tests/__init__.py
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/tests/urls.py
+Filename: django-simple-captcha-0.5.9/captcha/tests/tests.py
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/captcha/tests/views.py
+Filename: django-simple-captcha-0.5.9/captcha/tests/urls.py
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/django_simple_captcha.egg-info/dependency_links.txt
+Filename: django-simple-captcha-0.5.9/captcha/tests/views.py
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/django_simple_captcha.egg-info/not-zip-safe
+Filename: django-simple-captcha-0.5.9/django_simple_captcha.egg-info/dependency_links.txt
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/django_simple_captcha.egg-info/PKG-INFO
+Filename: django-simple-captcha-0.5.9/django_simple_captcha.egg-info/not-zip-safe
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/django_simple_captcha.egg-info/requires.txt
+Filename: django-simple-captcha-0.5.9/django_simple_captcha.egg-info/PKG-INFO
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/django_simple_captcha.egg-info/SOURCES.txt
+Filename: django-simple-captcha-0.5.9/django_simple_captcha.egg-info/requires.txt
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/django_simple_captcha.egg-info/top_level.txt
+Filename: django-simple-captcha-0.5.9/django_simple_captcha.egg-info/SOURCES.txt
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/docs/advanced.rst
+Filename: django-simple-captcha-0.5.9/django_simple_captcha.egg-info/top_level.txt
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/docs/changes.rst
+Filename: django-simple-captcha-0.5.9/docs/advanced.rst
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/docs/conf.py
+Filename: django-simple-captcha-0.5.9/docs/changes.rst
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/docs/index.rst
+Filename: django-simple-captcha-0.5.9/docs/conf.py
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/docs/Makefile
+Filename: django-simple-captcha-0.5.9/docs/index.rst
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/docs/usage.rst
+Filename: django-simple-captcha-0.5.9/docs/Makefile
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/docs/_static/captcha3.png
+Filename: django-simple-captcha-0.5.9/docs/usage.rst
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/docs/_static/dict.png
+Filename: django-simple-captcha-0.5.9/docs/_static/captcha3.png
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/docs/_static/math.png
+Filename: django-simple-captcha-0.5.9/docs/_static/dict.png
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/docs/_static/random_chars.png
+Filename: django-simple-captcha-0.5.9/docs/_static/math.png
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/testproject/.coveragerc
+Filename: django-simple-captcha-0.5.9/docs/_static/random_chars.png
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/testproject/__init__.py
+Filename: django-simple-captcha-0.5.9/testproject/.coveragerc
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/testproject/coverage.sh
+Filename: django-simple-captcha-0.5.9/testproject/__init__.py
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/testproject/forms.py
+Filename: django-simple-captcha-0.5.9/testproject/coverage.sh
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/testproject/jinja2_settings.py
+Filename: django-simple-captcha-0.5.9/testproject/forms.py
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/testproject/manage.py
+Filename: django-simple-captcha-0.5.9/testproject/jinja2_settings.py
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/testproject/settings.py
+Filename: django-simple-captcha-0.5.9/testproject/manage.py
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/testproject/urls.py
+Filename: django-simple-captcha-0.5.9/testproject/settings.py
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/testproject/views.py
+Filename: django-simple-captcha-0.5.9/testproject/urls.py
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/testproject/htmlcov/_Users_marco_Code_django-simple-captcha_captcha___init___py.html
+Filename: django-simple-captcha-0.5.9/testproject/views.py
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/testproject/htmlcov/_Users_marco_Code_django-simple-captcha_captcha_conf___init___py.html
+Filename: django-simple-captcha-0.5.9/testproject/htmlcov/_Users_marco_Code_django-simple-captcha_captcha___init___py.html
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/testproject/htmlcov/_Users_marco_Code_django-simple-captcha_captcha_conf_settings_py.html
+Filename: django-simple-captcha-0.5.9/testproject/htmlcov/_Users_marco_Code_django-simple-captcha_captcha_conf___init___py.html
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/testproject/htmlcov/_Users_marco_Code_django-simple-captcha_captcha_fields_py.html
+Filename: django-simple-captcha-0.5.9/testproject/htmlcov/_Users_marco_Code_django-simple-captcha_captcha_conf_settings_py.html
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/testproject/htmlcov/_Users_marco_Code_django-simple-captcha_captcha_helpers_py.html
+Filename: django-simple-captcha-0.5.9/testproject/htmlcov/_Users_marco_Code_django-simple-captcha_captcha_fields_py.html
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/testproject/htmlcov/_Users_marco_Code_django-simple-captcha_captcha_models_py.html
+Filename: django-simple-captcha-0.5.9/testproject/htmlcov/_Users_marco_Code_django-simple-captcha_captcha_helpers_py.html
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/testproject/htmlcov/_Users_marco_Code_django-simple-captcha_captcha_urls_py.html
+Filename: django-simple-captcha-0.5.9/testproject/htmlcov/_Users_marco_Code_django-simple-captcha_captcha_models_py.html
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/testproject/htmlcov/_Users_marco_Code_django-simple-captcha_captcha_views_py.html
+Filename: django-simple-captcha-0.5.9/testproject/htmlcov/_Users_marco_Code_django-simple-captcha_captcha_urls_py.html
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/testproject/htmlcov/coverage_html.js
+Filename: django-simple-captcha-0.5.9/testproject/htmlcov/_Users_marco_Code_django-simple-captcha_captcha_views_py.html
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/testproject/htmlcov/index.html
+Filename: django-simple-captcha-0.5.9/testproject/htmlcov/coverage_html.js
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/testproject/htmlcov/jquery.ba-throttle-debounce.min.js
+Filename: django-simple-captcha-0.5.9/testproject/htmlcov/index.html
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/testproject/htmlcov/jquery.hotkeys.js
+Filename: django-simple-captcha-0.5.9/testproject/htmlcov/jquery.ba-throttle-debounce.min.js
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/testproject/htmlcov/jquery.isonscreen.js
+Filename: django-simple-captcha-0.5.9/testproject/htmlcov/jquery.hotkeys.js
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/testproject/htmlcov/jquery.min.js
+Filename: django-simple-captcha-0.5.9/testproject/htmlcov/jquery.isonscreen.js
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/testproject/htmlcov/jquery.tablesorter.min.js
+Filename: django-simple-captcha-0.5.9/testproject/htmlcov/jquery.min.js
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/testproject/htmlcov/keybd_closed.png
+Filename: django-simple-captcha-0.5.9/testproject/htmlcov/jquery.tablesorter.min.js
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/testproject/htmlcov/keybd_open.png
+Filename: django-simple-captcha-0.5.9/testproject/htmlcov/keybd_closed.png
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/testproject/htmlcov/status.json
+Filename: django-simple-captcha-0.5.9/testproject/htmlcov/keybd_open.png
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/testproject/htmlcov/style.css
+Filename: django-simple-captcha-0.5.9/testproject/htmlcov/status.json
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/testproject/templates/home.html
+Filename: django-simple-captcha-0.5.9/testproject/htmlcov/style.css
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/testproject/templates/captcha_test/image.html
+Filename: django-simple-captcha-0.5.9/testproject/templates/home.html
 Comment: 
 
-Filename: django-simple-captcha-0.5.8/testproject/templates/captcha_test/image_html5_audio.html
+Filename: django-simple-captcha-0.5.9/testproject/templates/captcha_test/image.html
+Comment: 
+
+Filename: django-simple-captcha-0.5.9/testproject/templates/captcha_test/image_html5_audio.html
 Comment: 
 
 Zip file comment:
```

## Comparing `django-simple-captcha-0.5.8/CHANGES` & `django-simple-captcha-0.5.9/CHANGES`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Version History
 ===============
 
+Version 0.5.9
+-------------
+* Add missing Jinja2 templates in the pypi packages.
+
+
 Version 0.5.8
 -------------
 * Add support for Jinja2 templates (Issue #145, PR #146, thanks @ziima)
 * Cleanup, drop dependency on South (#141, #142 thanks @ziima)
 
 
 Version 0.5.7
```

## Comparing `django-simple-captcha-0.5.8/LICENSE` & `django-simple-captcha-0.5.9/LICENSE`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/PKG-INFO` & `django-simple-captcha-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-simple-captcha
-Version: 0.5.8
+Version: 0.5.9
 Summary: A very simple, yet powerful, Django captcha application
 Home-page: https://github.com/mbi/django-simple-captcha
 Author: Marco Bonetti
 Author-email: mbonetti@gmail.com
 License: MIT
 Description: *********************
         Django Simple Captcha
```

## Comparing `django-simple-captcha-0.5.8/README.rst` & `django-simple-captcha-0.5.9/README.rst`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/setup.py` & `django-simple-captcha-0.5.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         errno = tox.cmdline(args=args)
         sys.exit(errno)
 
 
 install_requires = [
     'six >=1.2.0',
     'Django >= 1.8',
-    'Pillow >=2.2.2,<5.0',
+    'Pillow >=2.2.2,!=5.1.0',
     'django-ranged-response == 0.2.0'
 ]
 EXTRAS_REQUIRE = {
     'test': ('testfixtures', ),
 }
```

## Comparing `django-simple-captcha-0.5.8/tox.ini` & `django-simple-captcha-0.5.9/tox.ini`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/captcha/fields.py` & `django-simple-captcha-0.5.9/captcha/fields.py`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/captcha/helpers.py` & `django-simple-captcha-0.5.9/captcha/helpers.py`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/captcha/models.py` & `django-simple-captcha-0.5.9/captcha/models.py`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/captcha/views.py` & `django-simple-captcha-0.5.9/captcha/views.py`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/captcha/conf/settings.py` & `django-simple-captcha-0.5.9/captcha/conf/settings.py`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/captcha/fonts/COPYRIGHT.TXT` & `django-simple-captcha-0.5.9/captcha/fonts/COPYRIGHT.TXT`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/captcha/fonts/Vera.ttf` & `django-simple-captcha-0.5.9/captcha/fonts/Vera.ttf`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/captcha/locale/bg/LC_MESSAGES/django.mo` & `django-simple-captcha-0.5.9/captcha/locale/bg/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/captcha/locale/bg/LC_MESSAGES/django.po` & `django-simple-captcha-0.5.9/captcha/locale/bg/LC_MESSAGES/django.po`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/captcha/locale/cs/LC_MESSAGES/django.mo` & `django-simple-captcha-0.5.9/captcha/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/captcha/locale/cs/LC_MESSAGES/django.po` & `django-simple-captcha-0.5.9/captcha/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/captcha/locale/de/LC_MESSAGES/django.mo` & `django-simple-captcha-0.5.9/captcha/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/captcha/locale/de/LC_MESSAGES/django.po` & `django-simple-captcha-0.5.9/captcha/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/captcha/locale/en/LC_MESSAGES/django.po` & `django-simple-captcha-0.5.9/captcha/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/captcha/locale/es/LC_MESSAGES/django.mo` & `django-simple-captcha-0.5.9/captcha/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/captcha/locale/es/LC_MESSAGES/django.po` & `django-simple-captcha-0.5.9/captcha/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/captcha/locale/fr/LC_MESSAGES/django.mo` & `django-simple-captcha-0.5.9/captcha/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/captcha/locale/fr/LC_MESSAGES/django.po` & `django-simple-captcha-0.5.9/captcha/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/captcha/locale/it/LC_MESSAGES/django.mo` & `django-simple-captcha-0.5.9/captcha/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/captcha/locale/it/LC_MESSAGES/django.po` & `django-simple-captcha-0.5.9/captcha/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/captcha/locale/ja/LC_MESSAGES/django.mo` & `django-simple-captcha-0.5.9/captcha/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/captcha/locale/ja/LC_MESSAGES/django.po` & `django-simple-captcha-0.5.9/captcha/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/captcha/locale/nl/LC_MESSAGES/django.mo` & `django-simple-captcha-0.5.9/captcha/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/captcha/locale/nl/LC_MESSAGES/django.po` & `django-simple-captcha-0.5.9/captcha/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/captcha/locale/pl/LC_MESSAGES/django.mo` & `django-simple-captcha-0.5.9/captcha/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/captcha/locale/pl/LC_MESSAGES/django.po` & `django-simple-captcha-0.5.9/captcha/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/captcha/locale/pt_BR/LC_MESSAGES/django.mo` & `django-simple-captcha-0.5.9/captcha/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/captcha/locale/pt_BR/LC_MESSAGES/django.po` & `django-simple-captcha-0.5.9/captcha/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/captcha/locale/ru/LC_MESSAGES/django.mo` & `django-simple-captcha-0.5.9/captcha/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/captcha/locale/ru/LC_MESSAGES/django.po` & `django-simple-captcha-0.5.9/captcha/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/captcha/locale/sk/LC_MESSAGES/django.mo` & `django-simple-captcha-0.5.9/captcha/locale/sk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/captcha/locale/sk/LC_MESSAGES/django.po` & `django-simple-captcha-0.5.9/captcha/locale/sk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/captcha/locale/tr/LC_MESSAGES/django.mo` & `django-simple-captcha-0.5.9/captcha/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/captcha/locale/tr/LC_MESSAGES/django.po` & `django-simple-captcha-0.5.9/captcha/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/captcha/locale/uk/LC_MESSAGES/django.mo` & `django-simple-captcha-0.5.9/captcha/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/captcha/locale/uk/LC_MESSAGES/django.po` & `django-simple-captcha-0.5.9/captcha/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/captcha/locale/zh_CN/LC_MESSAGES/django.mo` & `django-simple-captcha-0.5.9/captcha/locale/zh_CN/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/captcha/locale/zh_CN/LC_MESSAGES/django.po` & `django-simple-captcha-0.5.9/captcha/locale/zh_CN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/captcha/locale/zh_Hans/LC_MESSAGES/django.mo` & `django-simple-captcha-0.5.9/captcha/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/captcha/locale/zh_Hans/LC_MESSAGES/django.po` & `django-simple-captcha-0.5.9/captcha/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/captcha/management/commands/captcha_clean.py` & `django-simple-captcha-0.5.9/captcha/management/commands/captcha_clean.py`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/captcha/management/commands/captcha_create_pool.py` & `django-simple-captcha-0.5.9/captcha/management/commands/captcha_create_pool.py`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/captcha/migrations/0001_initial.py` & `django-simple-captcha-0.5.9/captcha/migrations/0001_initial.py`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/captcha/tests/tests.py` & `django-simple-captcha-0.5.9/captcha/tests/tests.py`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/captcha/tests/urls.py` & `django-simple-captcha-0.5.9/captcha/tests/urls.py`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/captcha/tests/views.py` & `django-simple-captcha-0.5.9/captcha/tests/views.py`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/django_simple_captcha.egg-info/PKG-INFO` & `django-simple-captcha-0.5.9/django_simple_captcha.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-simple-captcha
-Version: 0.5.8
+Version: 0.5.9
 Summary: A very simple, yet powerful, Django captcha application
 Home-page: https://github.com/mbi/django-simple-captcha
 Author: Marco Bonetti
 Author-email: mbonetti@gmail.com
 License: MIT
 Description: *********************
         Django Simple Captcha
```

## Comparing `django-simple-captcha-0.5.8/django_simple_captcha.egg-info/SOURCES.txt` & `django-simple-captcha-0.5.9/django_simple_captcha.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 captcha/urls.py
 captcha/views.py
 captcha/conf/__init__.py
 captcha/conf/settings.py
 captcha/fonts/COPYRIGHT.TXT
 captcha/fonts/README.TXT
 captcha/fonts/Vera.ttf
+captcha/jinja2/captcha/widgets/captcha.html
 captcha/locale/bg/LC_MESSAGES/django.mo
 captcha/locale/bg/LC_MESSAGES/django.po
 captcha/locale/cs/LC_MESSAGES/django.mo
 captcha/locale/cs/LC_MESSAGES/django.po
 captcha/locale/de/LC_MESSAGES/django.mo
 captcha/locale/de/LC_MESSAGES/django.po
 captcha/locale/en/LC_MESSAGES/django.po
```

## Comparing `django-simple-captcha-0.5.8/docs/advanced.rst` & `django-simple-captcha-0.5.9/docs/advanced.rst`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/docs/changes.rst` & `django-simple-captcha-0.5.9/docs/changes.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Version History
 ===============
 
+Version 0.5.9
+-------------
+* Add missing Jinja2 templates in the pypi packages.
+
+
 Version 0.5.8
 -------------
 * Add support for Jinja2 templates (Issue #145, PR #146, thanks @ziima)
 * Cleanup, drop dependency on South (#141, #142 thanks @ziima)
 
 
 Version 0.5.7
```

## Comparing `django-simple-captcha-0.5.8/docs/conf.py` & `django-simple-captcha-0.5.9/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 copyright = u('2011-2018 Marco Bonetti and contributors')
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = '0.5.8'
+version = '0.5.9'
 # The full version, including alpha/beta/rc tags.
 release = version
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 # language = None
```

## Comparing `django-simple-captcha-0.5.8/docs/index.rst` & `django-simple-captcha-0.5.9/docs/index.rst`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/docs/Makefile` & `django-simple-captcha-0.5.9/docs/Makefile`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/docs/usage.rst` & `django-simple-captcha-0.5.9/docs/usage.rst`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/docs/_static/captcha3.png` & `django-simple-captcha-0.5.9/docs/_static/captcha3.png`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/docs/_static/dict.png` & `django-simple-captcha-0.5.9/docs/_static/dict.png`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/docs/_static/math.png` & `django-simple-captcha-0.5.9/docs/_static/math.png`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/docs/_static/random_chars.png` & `django-simple-captcha-0.5.9/docs/_static/random_chars.png`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/testproject/manage.py` & `django-simple-captcha-0.5.9/testproject/manage.py`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/testproject/settings.py` & `django-simple-captcha-0.5.9/testproject/settings.py`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/testproject/htmlcov/_Users_marco_Code_django-simple-captcha_captcha___init___py.html` & `django-simple-captcha-0.5.9/testproject/htmlcov/_Users_marco_Code_django-simple-captcha_captcha___init___py.html`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/testproject/htmlcov/_Users_marco_Code_django-simple-captcha_captcha_conf___init___py.html` & `django-simple-captcha-0.5.9/testproject/htmlcov/_Users_marco_Code_django-simple-captcha_captcha_conf___init___py.html`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/testproject/htmlcov/_Users_marco_Code_django-simple-captcha_captcha_conf_settings_py.html` & `django-simple-captcha-0.5.9/testproject/htmlcov/_Users_marco_Code_django-simple-captcha_captcha_conf_settings_py.html`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/testproject/htmlcov/_Users_marco_Code_django-simple-captcha_captcha_fields_py.html` & `django-simple-captcha-0.5.9/testproject/htmlcov/_Users_marco_Code_django-simple-captcha_captcha_fields_py.html`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/testproject/htmlcov/_Users_marco_Code_django-simple-captcha_captcha_helpers_py.html` & `django-simple-captcha-0.5.9/testproject/htmlcov/_Users_marco_Code_django-simple-captcha_captcha_helpers_py.html`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/testproject/htmlcov/_Users_marco_Code_django-simple-captcha_captcha_models_py.html` & `django-simple-captcha-0.5.9/testproject/htmlcov/_Users_marco_Code_django-simple-captcha_captcha_models_py.html`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/testproject/htmlcov/_Users_marco_Code_django-simple-captcha_captcha_urls_py.html` & `django-simple-captcha-0.5.9/testproject/htmlcov/_Users_marco_Code_django-simple-captcha_captcha_urls_py.html`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/testproject/htmlcov/_Users_marco_Code_django-simple-captcha_captcha_views_py.html` & `django-simple-captcha-0.5.9/testproject/htmlcov/_Users_marco_Code_django-simple-captcha_captcha_views_py.html`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/testproject/htmlcov/coverage_html.js` & `django-simple-captcha-0.5.9/testproject/htmlcov/coverage_html.js`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/testproject/htmlcov/index.html` & `django-simple-captcha-0.5.9/testproject/htmlcov/index.html`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/testproject/htmlcov/jquery.ba-throttle-debounce.min.js` & `django-simple-captcha-0.5.9/testproject/htmlcov/jquery.ba-throttle-debounce.min.js`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/testproject/htmlcov/jquery.hotkeys.js` & `django-simple-captcha-0.5.9/testproject/htmlcov/jquery.hotkeys.js`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/testproject/htmlcov/jquery.isonscreen.js` & `django-simple-captcha-0.5.9/testproject/htmlcov/jquery.isonscreen.js`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/testproject/htmlcov/jquery.min.js` & `django-simple-captcha-0.5.9/testproject/htmlcov/jquery.min.js`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/testproject/htmlcov/jquery.tablesorter.min.js` & `django-simple-captcha-0.5.9/testproject/htmlcov/jquery.tablesorter.min.js`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/testproject/htmlcov/status.json` & `django-simple-captcha-0.5.9/testproject/htmlcov/status.json`

 * *Files identical despite different names*

## Comparing `django-simple-captcha-0.5.8/testproject/htmlcov/style.css` & `django-simple-captcha-0.5.9/testproject/htmlcov/style.css`

 * *Files identical despite different names*

