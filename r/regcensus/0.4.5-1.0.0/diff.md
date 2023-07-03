# Comparing `tmp/regcensus-0.4.5.tar.gz` & `tmp/regcensus-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regcensus-0.4.5.tar", last modified: Wed Aug 24 14:42:08 2022, max compression
+gzip compressed data, was "regcensus-1.0.0.tar", last modified: Mon Jul  3 13:39:36 2023, max compression
```

## Comparing `regcensus-0.4.5.tar` & `regcensus-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 jnelson  (535284464) 1921019053        0 2022-08-24 14:42:08.511191 regcensus-0.4.5/
--rw-r--r--   0 jnelson  (535284464) 1921019053       78 2021-07-30 15:35:00.000000 regcensus-0.4.5/.gitignore
--rw-r--r--   0 jnelson  (535284464) 1921019053     1098 2021-07-30 15:35:00.000000 regcensus-0.4.5/LICENSE
--rw-r--r--   0 jnelson  (535284464) 1921019053      401 2022-08-24 14:42:08.511404 regcensus-0.4.5/PKG-INFO
--rw-r--r--   0 jnelson  (535284464) 1921019053    14364 2022-01-14 22:34:44.000000 regcensus-0.4.5/README.md
-drwxr-xr-x   0 jnelson  (535284464) 1921019053        0 2022-08-24 14:42:08.487592 regcensus-0.4.5/regcensus/
--rw-r--r--   0 jnelson  (535284464) 1921019053      739 2022-08-24 14:33:56.000000 regcensus-0.4.5/regcensus/__init__.py
--rw-r--r--   0 jnelson  (535284464) 1921019053    19297 2022-08-24 14:35:44.000000 regcensus-0.4.5/regcensus/api.py
-drwxr-xr-x   0 jnelson  (535284464) 1921019053        0 2022-08-24 14:42:08.503281 regcensus-0.4.5/regcensus.egg-info/
--rw-r--r--   0 jnelson  (535284464) 1921019053      401 2022-08-24 14:42:08.000000 regcensus-0.4.5/regcensus.egg-info/PKG-INFO
--rw-r--r--   0 jnelson  (535284464) 1921019053      285 2022-08-24 14:42:08.000000 regcensus-0.4.5/regcensus.egg-info/SOURCES.txt
--rw-r--r--   0 jnelson  (535284464) 1921019053        1 2022-08-24 14:42:08.000000 regcensus-0.4.5/regcensus.egg-info/dependency_links.txt
--rw-r--r--   0 jnelson  (535284464) 1921019053       16 2022-08-24 14:42:08.000000 regcensus-0.4.5/regcensus.egg-info/requires.txt
--rw-r--r--   0 jnelson  (535284464) 1921019053       10 2022-08-24 14:42:08.000000 regcensus-0.4.5/regcensus.egg-info/top_level.txt
--rw-r--r--   0 jnelson  (535284464) 1921019053       15 2021-07-30 15:35:00.000000 regcensus-0.4.5/requirements.txt
--rw-r--r--   0 jnelson  (535284464) 1921019053      130 2022-08-24 14:42:08.515434 regcensus-0.4.5/setup.cfg
--rw-r--r--   0 jnelson  (535284464) 1921019053      583 2022-08-24 14:36:10.000000 regcensus-0.4.5/setup.py
-drwxr-xr-x   0 jnelson  (535284464) 1921019053        0 2022-08-24 14:42:08.510313 regcensus-0.4.5/tests/
--rw-r--r--   0 jnelson  (535284464) 1921019053    11290 2022-07-25 15:14:16.000000 regcensus-0.4.5/tests/test_api.py
+drwxr-xr-x   0 jnelson    (501) staff       (20)        0 2023-07-03 13:39:36.749439 regcensus-1.0.0/
+-rw-r--r--   0 jnelson    (501) staff       (20)       78 2023-04-26 13:32:43.000000 regcensus-1.0.0/.gitignore
+-rw-r--r--   0 jnelson    (501) staff       (20)     1098 2023-04-26 13:32:43.000000 regcensus-1.0.0/LICENSE
+-rw-r--r--   0 jnelson    (501) staff       (20)      401 2023-07-03 13:39:36.749516 regcensus-1.0.0/PKG-INFO
+-rw-r--r--   0 jnelson    (501) staff       (20)    14364 2023-04-26 13:32:43.000000 regcensus-1.0.0/README.md
+drwxr-xr-x   0 jnelson    (501) staff       (20)        0 2023-07-03 13:39:36.747865 regcensus-1.0.0/regcensus/
+-rw-r--r--   0 jnelson    (501) staff       (20)      793 2023-06-30 17:20:28.000000 regcensus-1.0.0/regcensus/__init__.py
+-rw-r--r--   0 jnelson    (501) staff       (20)    25044 2023-06-30 18:07:03.000000 regcensus-1.0.0/regcensus/api.py
+-rw-r--r--   0 jnelson    (501) staff       (20)     1047 2023-06-30 17:20:28.000000 regcensus-1.0.0/regcensus/cache.py
+drwxr-xr-x   0 jnelson    (501) staff       (20)        0 2023-07-03 13:39:36.748910 regcensus-1.0.0/regcensus.egg-info/
+-rw-r--r--   0 jnelson    (501) staff       (20)      401 2023-07-03 13:39:36.000000 regcensus-1.0.0/regcensus.egg-info/PKG-INFO
+-rw-r--r--   0 jnelson    (501) staff       (20)      304 2023-07-03 13:39:36.000000 regcensus-1.0.0/regcensus.egg-info/SOURCES.txt
+-rw-r--r--   0 jnelson    (501) staff       (20)        1 2023-07-03 13:39:36.000000 regcensus-1.0.0/regcensus.egg-info/dependency_links.txt
+-rw-r--r--   0 jnelson    (501) staff       (20)       16 2023-07-03 13:39:36.000000 regcensus-1.0.0/regcensus.egg-info/requires.txt
+-rw-r--r--   0 jnelson    (501) staff       (20)       10 2023-07-03 13:39:36.000000 regcensus-1.0.0/regcensus.egg-info/top_level.txt
+-rw-r--r--   0 jnelson    (501) staff       (20)       15 2023-04-26 13:32:44.000000 regcensus-1.0.0/requirements.txt
+-rw-r--r--   0 jnelson    (501) staff       (20)      130 2023-07-03 13:39:36.749830 regcensus-1.0.0/setup.cfg
+-rw-r--r--   0 jnelson    (501) staff       (20)      583 2023-06-30 17:20:34.000000 regcensus-1.0.0/setup.py
+drwxr-xr-x   0 jnelson    (501) staff       (20)        0 2023-07-03 13:39:36.749104 regcensus-1.0.0/tests/
+-rw-r--r--   0 jnelson    (501) staff       (20)    10074 2023-06-30 17:20:28.000000 regcensus-1.0.0/tests/test_api.py
```

### Comparing `regcensus-0.4.5/LICENSE` & `regcensus-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `regcensus-0.4.5/README.md` & `regcensus-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `regcensus-0.4.5/regcensus/__init__.py` & `regcensus-1.0.0/regcensus/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 __all__ = [
     'get_values',
     'get_document_values',
     'get_reading_time',
+    'get_datafinder',
     'get_series',
-    'get_periods',
     'get_agencies',
     'get_jurisdictions',
     'get_industries',
     'get_documents',
+    'get_documentation',
     'get_versions',
     'list_series',
     'list_dates',
     'list_document_types',
     'list_agencies',
     'list_clusters',
     'list_jurisdictions',
     'list_industries'
 ]
 
 from . api import (
     get_values,
     get_document_values,
     get_reading_time,
+    get_datafinder,
     get_series,
-    get_periods,
     get_agencies,
     get_jurisdictions,
     get_industries,
     get_documents,
+    get_documentation,
     get_versions,
     list_series,
     list_dates,
     list_document_types,
     list_agencies,
     list_clusters,
     list_jurisdictions,
```

### Comparing `regcensus-0.4.5/regcensus/api.py` & `regcensus-1.0.0/regcensus/api.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,77 +1,119 @@
+import json
 import re
 import requests
 import pandas as pd
 import pprint
 
+from regcensus.cache import Memoized
+
 pp = pprint.PrettyPrinter()
 
 date_format = re.compile(r'\d{4}(?:-\d{2}-\d{2})?')
 
-URL = 'https://api.quantgov.org'
+URL = 'https://64gzqlrrd2.execute-api.us-east-1.amazonaws.com/dev'
 
 
-def get_values(series, jurisdiction, date, documentType=None, summary=True,
+def get_values(series, jurisdiction, year, documentType=1, summary=True,
                dateIsRange=True, country=False, agency=None, cluster=None,
-               industry=None, filtered=True, industryLevel=None, version=None,
-               download=False, verbose=0):
+               label=None, industry=None, filtered=True,
+               labellevel=3, industryLevel=None,
+               labelsource='NAICS', version=None,
+               download=False, page=None, date=None, verbose=0):
     """
-    Get values for a specific jurisdiction and series
+    Get values for a specific jurisdiction, series, and year
 
     Args:
         jurisdiction: Jurisdiction ID(s) (name may also be passed)
         series: Series ID(s)
-        date: Year(s) of data
-        documentType (optional): ID for type of document
-        summary (optional): Return summary instead of document level data
+        year: Year(s) of data
+        documentType (optional): ID for type of document,
+            e.g. 1 is regulations, 2 is statutes
+        summary (optional): Return summary instead of document level data,
+            only one year of data is allowed for document level data
         dateIsRange (optional): Indicating whether the time parameter is range
             or should be treated as single data points
         country (optional): Get values for all subjurisdictions
         agency (optional): Agency ID (if no ID is passed and the series
             contains agency data, returns data for all agencies)
-        industry (optional): Industry code using the jurisdiction-specific
+        label (formerly industry) (optional):
+            Industry code using the jurisdiction-specific
             coding system (returns all 3-digit industries by default)
         filtered (optional): Exclude poorly-performing industry results
             (use of unfiltered results is NOT recommended)
-        industryLevel (optional): Level of NAICS industries to include
-            (default is 3 in the API)
+        labellevel (formerly industryLevel) (optional):
+            Level of NAICS industries to include
         version (optional): Version ID for datasets with multiple versions
             (if no ID is given, returns most recent version)
         download (optional): If not False, a path location for a
             downloaded csv of the results
         verbose (optional): Print out the url of the API call
             (useful for debugging)
 
     Returns: pandas dataframe with the values and various metadata
 
     Returns empty if required parameters are not given
     """
+    if date:
+        print('WARNING: date is deprecated, use year')
+        return
+
+    # If multiple jurisdiction names are given, find list of IDs
+    if type(jurisdiction) == list and re.search(
+            r'[A-Za-z]', str(jurisdiction[0])):
+        jurisdiction = [list_jurisdictions()[i] for i in jurisdiction]
+    # If jurisdiction name is passed, find ID
+    elif jurisdiction and re.search(r'[A-Za-z]', str(jurisdiction)):
+        jurisdiction = list_jurisdictions()[jurisdiction]
+
+    # Use /datafinder endpoint to get the appropriate values endpoint
+    try:
+        endpoint = get_endpoint(
+            series, jurisdiction, year, documentType, summary)
+    # If endpoint is not found with given parameters, print datafinder table
+    except IndexError:
+        print('No data was found for these parameters. '
+              'For this jurisdiction, consider the following:\n')
+        with pd.option_context(
+                'display.max_rows', None, 'display.max_columns', None):
+            print(get_datafinder(
+                jurisdiction, documentType).to_string(index=False))
+            return
+
+    if endpoint:
+        url_call = URL + endpoint + '?'
+    else:
+        with pd.option_context(
+                'display.max_rows', None, 'display.max_columns', None):
+            try:
+                print(
+                    'No data was found for these parameters. '
+                    'For this jurisdiction, consider the following:\n\n',
+                    get_datafinder(
+                        jurisdiction, documentType).to_string(index=False))
+            except TypeError:
+                print("Valid jurisdiction ID required. Consider the following:\n")
+                pp.pprint(list_jurisdictions())
+            return
 
     # If multiple series are given, parses the list into a string
     if type(series) == list:
-        url_call = (
-            URL + f'/summary?series={",".join(str(i) for i in series)}')
+        url_call += f'series={",".join(str(i) for i in series)}'
     elif type(series) in [int, str]:
-        url_call = URL + f'/summary?series={series}'
+        url_call += f'series={series}'
     # If no appropriate series is given, prints warning message and
     # list of available series, and function returns empty.
     else:
         print("Valid series ID required. Select from the following list:")
         pp.pprint(list_series())
         return
 
-    # If multiple jurisdiction names are given, parses the list into a string
-    if type(jurisdiction) == list and re.search(r'\D', str(jurisdiction[0])):
-        url_call += f'&jurisdictionName={",".join(i for i in jurisdiction)}'
     # If multiple jurisdiction IDs are given, parses the list into a string
-    elif type(jurisdiction) == list:
+    if type(jurisdiction) == list:
         url_call += f'&jurisdiction={",".join(str(i) for i in jurisdiction)}'
-    # If jurisdiction name is passed, use jurisdictionName
-    elif jurisdiction and re.search(r'\D', str(jurisdiction)):
-        url_call += f'&jurisdictionName={jurisdiction}'
     # If jurisdiction is just an ID, use jurisdiction
     elif type(jurisdiction) in [int, str]:
         url_call += f'&jurisdiction={jurisdiction}'
     # If no appropriate jurisdiction is given, prints warning message and
     # list of available jurisdictions, and function returns empty.
     else:
         print("Valid jurisdiction ID required.")
@@ -86,84 +128,118 @@
 
     # If multiple clusters are given, parses the list into a string
     if type(cluster) == list:
         url_call += f'&cluster={",".join(str(i) for i in cluster)}'
     elif cluster:
         url_call += f'&cluster={cluster}'
 
+    # Display deprecation message and rename industry args
+    if industry:
+        print('WARNING: industry is deprecated; use label')
+        label = industry
+    if industryLevel:
+        print('WARNING: industryLevel is deprecated; use labellevel')
+        labellevel = industryLevel
     # If multiple industries are given, parses the list into a string
-    if type(industry) == list:
-        url_call += f'&label={",".join(str(i) for i in industry)}'
-    elif industry:
-        url_call += f'&label={industry}'
+    if type(label) == list:
+        if labelsource == 'NAICS':
+            label = [list_industries(labellevel=labellevel,
+                                     labelsource=labelsource,
+                                     onlyID=True)[str(i)] for i in label]
+        url_call += f'&label={",".join(str(i) for i in label)}'
+    elif label:
+        if labelsource == 'NAICS':
+            label = list_industries(labellevel=labellevel,
+                                    labelsource=labelsource,
+                                    onlyID=True)[str(label)]
+        url_call += f'&label={label}'
     # Specify level of industry (NAICS only)
-    if industryLevel:
-        url_call += f'&labelLevel={industryLevel}'
+    if labellevel:
+        url_call += f'&labelLevel={labellevel}'
 
-    # If multiple dates are given, parses the list into a string
-    if type(date) == list:
-        url_call += f'&date={",".join(str(i) for i in date)}'
-        # Force dateIsRange to be false if more than 2 dates are given
-        if len(date) > 2:
-            dateIsRange = False
+    # If multiple years are given, parses the list into a string
+    if type(year) == list:
+        # If dateIsRange, parses the list to include all years
+        if dateIsRange and len(year) == 2:
+            year = range(int(year[0]), int(year[1]) + 1)
+        url_call += f'&year={",".join(str(i) for i in year)}'
     # Checks to see if date is in correct format
-    elif date_format.match(str(date)):
-        url_call += f'&date={date}'
-        # Force dateIsRange to be false if only 1 date is given
-        dateIsRange = False
+    elif date_format.match(str(year)):
+        url_call += f'&year={year}'
     # If no appropriate date is given, prints warning message and
     # list of available dates for the given jurisdiction(s),
     # and function returns empty.
     else:
         print("Valid date is required. Select from the following list:")
         dates = list_dates(jurisdiction, verbose=verbose)
         pp.pprint(dates)
         return
 
-    if dateIsRange:
-        url_call += '&dateIsRange=true'
-
     # Allows for document-level data to be retrieved.
     # Includes warning message explaning that this query may take a while.
     if not summary:
-        if industry:
+        if label:
             print('WARNING: Returning document-level industry results. '
                   'This query make take several minutes.')
         url_call = url_call.replace('/summary', '/documents')
 
     # Allows for unfiltered industry results to be retrieved. Includes
     # warning message explaining that these results should not be trusted.
-    if industry and not filtered:
+    if label and not filtered:
         print('WARNING: Returning unfiltered industry results. '
               'Use of these results is NOT recommended.')
         url_call += '&filteredOnly=false'
 
     # Adds documentType argument (default is 1 in API)
     if documentType:
-        url_call += f'&documentType={documentType}'
+        url_call += f'&documenttype={documentType}'
 
     # Adds country argument if country-level data is requested
     if country:
-        url_call += '&national=True'
+        print('WARNING: country is deprecated')
 
     # Adds version argument if different version is requested
     if version:
-        url_call += f'&version={version}'
+        # url_call += f'&version={version}'
+        print('WARNING: version is temporarily deprecated')
 
     # Prints the url call if verbosity is flagged
     if verbose:
         print(f'API call: {url_call.replace(" ", "%20")}')
 
+    # Allows user to manually select a page of the output
+    # If page is not passed, pagination is done automatically (see below)
+    # for output larger than 5000 rows
+    if page:
+        url_call += f'&page={page}'
+
     # Puts flattened JSON output into a pandas DataFrame
-    output = json_normalize(requests.get(url_call).json())
-    # Prints error message if call fails
-    if (output.columns[:3] == ['title', 'status', 'detail']).all():
-        print('WARNING:', output.iloc[0][-1])
+    try:
+        json_output = requests.get(url_call).json()
+        output = json_normalize(json.loads(json_output))
+    # Prints error message if call errors
+    except TypeError:
+        print_error(json_output)
         return
-    elif download:
+
+    # If output is truncated, paginates until all data is found
+    if len(output) == 5000 and not page:
+        full_output = output
+        page = 1
+        while len(output) == 5000:
+            if verbose:
+                print(f'Output truncated, found page {page}')
+            page += 1
+            output = json_normalize(json.loads(requests.get(
+                url_call + f'&page={page}').json()))
+            full_output = full_output.append(output)
+        output = full_output
+
+    # If download path is given, write csv instead of returning dataframe
+    if download:
         if type(download) == str:
             clean_columns(output).to_csv(download, index=False)
         else:
             print("Valid outpath required to download.")
     # Returns clean data if no error
     else:
         return clean_columns(output)
@@ -179,97 +255,141 @@
 
 
 def get_reading_time(*args, **kwargs):
     """
     Convert word counts to total reading time
     """
     results = get_values(series=2, *args, **kwargs)
-    results['seriesName'] = 'Reading Time'
-    results['seriesValue'] = results['seriesValue'].apply(reading_time)
+    results['series_name'] = 'Reading Time'
+    results['series_value'] = results['series_value'].apply(reading_time)
     results['footNote'] = (
         'Reading time calculation assumes an 8 hour work-day, '
         'a 5 day work-week, and a 50 week work-year.')
     return results
 
 
-def get_series(jurisdictionID=None, documentType=None, verbose=0):
+@Memoized
+def get_datafinder(jurisdiction, documentType=None):
     """
-    Get series metadata for all or one specific jurisdiction
+    Get API info for a specific jurisdition and documentType
 
-    Args: jurisdictionID (optional): ID for the jurisdiction
+    Returns: pandas dataframe with the series and years available,
+             along with the endpoints to access the data
+    """
+    if documentType:
+        output = clean_columns(json_normalize(json.loads(requests.get(
+            URL + (f'/datafinder?jurisdiction={jurisdiction}&'
+                   f'documenttype={documentType}')
+        ).json())))
+    else:
+        output = clean_columns(json_normalize(json.loads(requests.get(
+            URL + f'/datafinder?jurisdiction={jurisdiction}'
+        ).json())))
+    return output.rename({
+        'jurisdiction_id': 'jurisdiction',
+        'document_type_id': 'documentType',
+        'series_id': 'series'}, axis=1)
 
-    Returns: pandas dataframe with the metadata
+
+@Memoized
+def get_endpoint(series, jurisdiction, year, documentType, summary=True):
     """
-    url_call = series_url(jurisdictionID, documentType)
-    if verbose:
-        print(f'API call: {url_call}')
-    return clean_columns(json_normalize(requests.get(url_call).json()))
+    Get endpoint for a specific series, jurisdition, year, documentType combo
+
+    Returns the endpoint, e.g. '/state-summary' for summary-level state data
+    """
+    if type(year) == list:
+        year = [int(y) for y in year]
+    if type(series) == list:
+        series = [int(s) for s in series]
+    try:
+        datafinder = get_datafinder(jurisdiction, documentType).query(
+            f'series == {series} and year == {year}')
+        if summary:
+            endpoint = datafinder.summary_endpoints.values[0]
+        else:
+            endpoint = datafinder.document_endpoints.values[0]
+        # Handles document-level industry calls
+        if not endpoint:
+            endpoint = datafinder.label_endpoints.values[0]
+        return endpoint
+    except (KeyError, TypeError):
+        return
 
 
-def get_periods(jurisdictionID=None, documentType=None, verbose=0):
+@Memoized
+def get_series(verbose=0):
     """
-    Get date metadata for all or one specific jurisdiction
+    Get series metadata for all or one specific jurisdiction
 
     Args: jurisdictionID (optional): ID for the jurisdiction
 
     Returns: pandas dataframe with the metadata
     """
-    url_call = periods_url(jurisdictionID, documentType)
+    url_call = series_url()
     if verbose:
         print(f'API call: {url_call}')
-    return clean_columns(json_normalize(requests.get(url_call).json()))
+    return clean_columns(json_normalize(
+        json.loads(requests.get(url_call).json())))
 
 
+@Memoized
 def get_agencies(jurisdictionID=None, keyword=None, verbose=0):
     """
     Get metadata for all agencies of a specific jurisdiction
 
     Args: jurisdictionID: ID for the jurisdiction
 
     Returns: pandas dataframe with the metadata
     """
     url_call = agency_url(jurisdictionID, keyword)
     if not url_call:
         return
     if verbose:
         print(f'API call: {url_call}')
-    return clean_columns(json_normalize(requests.get(url_call).json()))
+    return clean_columns(json_normalize(
+        json.loads(requests.get(url_call).json())))
 
 
-def get_jurisdictions(jurisdictionID=None, verbose=0):
+@Memoized
+def get_jurisdictions(verbose=0):
     """
     Get metadata for all or one specific jurisdiction
 
     Args: jurisdictionID (optional): ID for the jurisdiction
 
     Returns: pandas dataframe with the metadata
     """
-    url_call = jurisdictions_url(jurisdictionID)
+    url_call = jurisdictions_url()
     if verbose:
         print(f'API call: {url_call}')
-    return clean_columns(json_normalize(requests.get(url_call).json()))
+    return clean_columns(json_normalize(
+        json.loads(requests.get(url_call).json())))
 
 
-def get_industries(keyword=None, codeLevel=3, standard=None, verbose=0):
+@Memoized
+def get_industries(keyword=None, labellevel=3, labelsource=None, verbose=0):
     """
     Get metadata for all industries available in a specific jurisdiction
 
     Args:
         keyword: search for keyword in industry name
-        codeLevel: NAICS level (2 to 6-digit)
-        standard: classification standard (NAICS, BEA, SOC)
+        labellevel: NAICS level (2 to 6-digit)
+        labelsource: classification standard (NAICS, BEA, SOC)
 
     Returns: pandas dataframe with the metadata
     """
-    url_call = industries_url(keyword, codeLevel, standard)
+    url_call = industries_url(keyword, labellevel, labelsource)
     if verbose:
         print(f'API call: {url_call}')
-    return clean_columns(json_normalize(requests.get(url_call).json()))
+    return clean_columns(json_normalize(
+        json.loads(requests.get(url_call).json())))
 
 
+@Memoized
 def get_documents(documentID=None, jurisdictionID=None, date=None,
                   documentType=1, verbose=0):
     """
     Get metadata for documents available in a specific jurisdiction or
     for a specific document ID
 
     Args:
@@ -277,243 +397,294 @@
         jurisdictionID: ID for the jurisdiction
         date: Year(s) of the documents
         documentType (optional): ID for type of document
 
     Returns: pandas dataframe with the metadata
     """
     if documentID:
-        url_call = URL + f'/documentMetadata/documents?documentID={documentID}'
+        print('documentID is no longer accessible as of version X.XX. '
+              'Use previous version of API or use jurisdictionID and date '
+              'combination')
+        return
     elif jurisdictionID and date:
-        url_call = URL + (f'/documentMetadata?jurisdiction={jurisdictionID}&'
-                          f'documentType={documentType}')
+        return get_values(
+            series=1,
+            jurisdiction=jurisdictionID,
+            year=date,
+            documentType=documentType,
+            summary=False)
     else:
-        print('Must include either "jurisdictionID and date" or "documentID."')
+        print('Must include "jurisdictionID and date"')
         return
-    if type(date) == list:
-        url_call += f'&date={",".join(str(i) for i in date)}'
-        if len(date) == 2:
-            url_call += '&dateIsRange=true'
-        else:
-            url_call += '&dateIsRange=false'
-    else:
-        url_call += f'&date={date}'
-    if verbose:
-        print(f'API call: {url_call}')
-    return clean_columns(json_normalize(requests.get(url_call).json()))
 
 
+@Memoized
 def get_versions(jurisdictionID, documentType=1, verbose=0):
     """
     Get metadata for versions available in a specific jurisdiction.
 
     Args:
         jurisdictionID: ID for the jurisdiction
         documentType (optional): ID for type of document
 
     Returns: pandas dataframe with the metadata
     """
     url_call = URL + (f'/version?jurisdiction={jurisdictionID}&'
                       f'documentType={documentType}')
     if verbose:
         print(f'API call: {url_call}')
-    return clean_columns(json_normalize(requests.get(url_call).json()))
+    return clean_columns(json_normalize(
+        json.loads(requests.get(url_call).json())))
 
 
-def list_document_types(jurisdictionID=None, verbose=0):
+@Memoized
+def get_documentation():
+    """
+    Get documentation for projects, including citations.
+    """
+    return clean_columns(json_normalize(json.loads(requests.get(
+        URL + '/documentation'
+    ).json())))
+
+
+@Memoized
+def list_document_types(jurisdictionID=None, reverse=False, verbose=0):
     """
     Args: jurisdictionID (optional): ID for the jurisdiction
 
     Returns: a dictionary containing names of documenttypes and associated IDs
     """
     if jurisdictionID:
         url_call = URL + f'/documenttypes?jurisdiction={jurisdictionID}'
     else:
         url_call = URL + '/documenttypes'
     if verbose:
         print(f'API call: {url_call}')
-    json = requests.get(url_call).json()
-    return dict(sorted({
-        d["subtypeName"]: d["documentSubtypeID"]
-        for d in json if d["subtypeName"]}.items()))
+    content = json.loads(requests.get(url_call).json())
+    if reverse:
+        return dict(sorted({
+            d["document_type_id"]: d["document_type"]
+            for d in content if d["document_type"]}.items()))
+    else:
+        return dict(sorted({
+            d["document_type"]: d["document_type_id"]
+            for d in content if d["document_type"]}.items()))
 
 
-def list_series(jurisdictionID, documentType=None):
+@Memoized
+def list_series(reverse=False):
     """
     Args:
         jurisdictionID: ID for the jurisdiction
         documentType (optional): ID for type of document
 
     Returns: dictionary containing names of series and associated IDs
     """
-    url_call = periods_url(jurisdictionID, documentType)
-    json = requests.get(url_call).json()
-    return dict(sorted({
-        s["series"]["seriesName"]: s["series"]["seriesID"]
-        for s in json}.items()))
+    url_call = series_url()
+    content = json.loads(requests.get(url_call).json())
+    if reverse:
+        return dict(sorted({
+            s["series_id"]: s["series_name"]
+            for s in content}.items()))
+    else:
+        return dict(sorted({
+            s["series_name"]: s["series_id"]
+            for s in content}.items()))
 
 
-def list_dates(jurisdictionID, documentType=None, verbose=0):
+@Memoized
+def list_dates(jurisdictionID, documentType=None):
     """
     Args:
         jurisdictionID: ID for the jurisdiction
         documentType (optional): ID for type of document
 
     Returns: list of dates available for the jurisdiction
     """
-    return sorted(get_periods(
-        jurisdictionID, documentType, verbose=verbose)['periodCode'].unique())
+    return sorted(get_datafinder(
+        jurisdictionID, documentType)['year'].unique())
 
 
-def list_agencies(jurisdictionID=None, keyword=None):
+@Memoized
+def list_agencies(jurisdictionID=None, keyword=None, reverse=False):
     """
     Args:
         jurisdictionID: ID for the jurisdiction
         keyword: search for keyword in agency name
 
     Returns: dictionary containing names of agencies and associated IDs
     """
     url_call = agency_url(jurisdictionID, keyword)
     if not url_call:
         return
-    json = requests.get(url_call).json()
+    content = json.loads(requests.get(url_call).json())
+
+    jurisdictions_df = get_jurisdictions()
+    jurisdiction_id_name = dict(zip(jurisdictions_df["jurisdiction_id"],
+                                    jurisdictions_df["jurisdiction_name"]))
+
     # Add jurisdiction name to key if keyword is used
-    if keyword:
-        return dict(sorted({
-            f'{a["agencyName"]} ({a["jurisdictionName"]})': a["agencyID"]
-            for a in json if a["agencyName"]}.items()))
+    if reverse:
+        if keyword:
+            return dict(sorted({
+                a["agency_id"]:
+                    f'{a["agency_name"]} ({jurisdiction_id_name[int(a["a_jurisdiction_id"])]})'
+                for a in content if a["agency_name"]}.items()))
+        else:
+            return dict(sorted({
+                a["agency_id"]: a["agency_name"]
+                for a in content if a["agency_name"]}.items()))
     else:
-        return dict(sorted({
-            a["agencyName"]: a["agencyID"]
-            for a in json if a["agencyName"]}.items()))
+        if keyword:
+            return dict(sorted({
+                f'{a["agency_name"]} ({jurisdiction_id_name[int(a["a_jurisdiction_id"])]})':
+                    a["agency_id"]
+                for a in content if a["agency_name"]}.items()))
+        else:
+            return dict(sorted({
+                a["agency_name"]: a["agency_id"]
+                for a in content if a["agency_name"]}.items()))
 
 
-def list_clusters():
+@Memoized
+def list_clusters(reverse=False):
     """
     Returns: dictionary containing names of clusters and associated IDs
     """
     url_call = URL + '/clusters'
-    json = requests.get(url_call).json()
-    return dict(sorted({
-        a["clusterName"]: a["agencyCluster"]
-        for a in json if a["clusterName"]}.items()))
+    content = json.loads(requests.get(url_call).json())
+    if reverse:
+        return dict(sorted({
+            a["agency_cluster"]: a["cluster_name"]
+            for a in content if a["cluster_name"]}.items()))
+    else:
+        return dict(sorted({
+            a["cluster_name"]: a["agency_cluster"]
+            for a in content if a["cluster_name"]}.items()))
 
 
-def list_jurisdictions():
+@Memoized
+def list_jurisdictions(reverse=False):
     """
     Returns: dictionary containing names of jurisdictions and associated IDs
     """
-    url_call = jurisdictions_url(None)
-    json = requests.get(url_call).json()
-    return dict(sorted({
-        j["jurisdictionName"]: j["jurisdictionID"] for j in json}.items()))
+    url_call = jurisdictions_url()
+    content = json.loads(requests.get(url_call).json())
+    if reverse:
+        return dict(sorted({
+            j["jurisdiction_id"]: j["jurisdiction_name"]
+            for j in content}.items()))
+    else:
+        return dict(sorted({
+            j["jurisdiction_name"]: j["jurisdiction_id"]
+            for j in content}.items()))
 
 
-def list_industries(keyword=None, codeLevel=3, standard='NAICS', onlyID=False):
+@Memoized
+def list_industries(
+        keyword=None, labellevel=3, labelsource='NAICS',
+        onlyID=False, reverse=False):
     """
     Args:
         keyword: search for keyword in industry name
         codeLevel: NAICS level (2 to 6-digit)
         standard: classification standard (NAICS (default), BEA, SOC)
         onlyID: uses the NAICS code instead of name as key of dictionary
 
     Returns: dictionary containing names of industries and associated IDs
     """
-    url_call = industries_url(keyword, codeLevel, standard)
-    json = requests.get(url_call).json()
+    url_call = industries_url(keyword, labellevel, labelsource)
+    content = json.loads(requests.get(url_call).json())
     # If industry has codes, include the code in the key
     try:
         if onlyID:
+            if reverse:
+                return dict(sorted({
+                    i["label_id"]: i["label_code"] for i in content}.items()))
+            else:
+                return dict(sorted({
+                    i["label_code"]: i["label_id"] for i in content}.items()))
+        else:
+            if reverse:
+                return dict(sorted({
+                    i["label_id"]: f'{i["label_name"]} ({i["label_code"]})'
+                    for i in content}.items()))
+            else:
+                return dict(sorted({
+                    f'{i["label_name"]} ({i["label_code"]})': i["label_id"]
+                    for i in content}.items()))
+    except KeyError:
+        if reverse:
             return dict(sorted({
-                i["industryCode"]: i["industryID"] for i in json}.items()))
+                i["label_id"]: i["label_name"] for i in content}.items()))
         else:
             return dict(sorted({
-                f'{i["industryName"]} ({i["industryCode"]})':
-                i["industryID"] for i in json}.items()))
-    except KeyError:
-        return dict(sorted({
-            i["industryName"]: i["industryID"] for i in json}.items()))
-
-
-def series_url(jurisdictionID, documentType=None):
-    """Gets url call for series endpoint."""
-    url_call = URL + '/dataseries'
-    if jurisdictionID and documentType:
-        url_call += (
-            f'?jurisdiction={jurisdictionID}&'
-            f'documentType={documentType}')
-    elif jurisdictionID:
-        url_call += f'?jurisdiction={jurisdictionID}'
-    elif documentType:
-        url_call += f'?documentType={documentType}'
-    return url_call
+                i["label_name"]: i["label_id"] for i in content}.items()))
 
 
-def periods_url(jurisdictionID, documentType=None):
-    """Gets url call for series endpoint."""
-    url_call = URL + '/seriesperiod'
-    if jurisdictionID and documentType:
-        url_call += (
-            f'?jurisdiction={jurisdictionID}&'
-            f'documentType={documentType}')
-    elif jurisdictionID:
-        url_call += f'?jurisdiction={jurisdictionID}'
-    elif documentType:
-        url_call += f'?documentType={documentType}'
-    return url_call
+def series_url():
+    """Gets url call for dataseries endpoint."""
+    return URL + '/dataseries'
 
 
 def agency_url(jurisdictionID, keyword):
     """Gets url call for agencies endpoint."""
     if keyword:
-        url_call = URL + (f'/agencies/keyword?'
+        url_call = URL + (f'/agencies-keyword?'
                           f'keyword={keyword}')
     elif jurisdictionID:
-        url_call = URL + (f'/agencies/jurisdictions?'
+        url_call = URL + (f'/agencies?'
                           f'jurisdiction={jurisdictionID}')
     else:
         print('Must include either "jurisdictionID" or "keyword."')
         return
     return url_call
 
 
-def jurisdictions_url(jurisdictionID):
+def jurisdictions_url():
     """Gets url call for jurisdictions endpoint."""
-    url_call = URL + '/jurisdictions/'
-    if jurisdictionID:
-        url_call += f'/specific?jurisdiction={jurisdictionID}'
-    return url_call
+    return URL + '/jurisdictions/'
 
 
-def industries_url(keyword, codeLevel, standard):
+def industries_url(keyword, labellevel, labelsource):
     """Gets url call for label (formerly industries) endpoint."""
     if keyword:
         url_call = (
-            URL + f'/label/keyword?'
-                  f'codeLevel={codeLevel}&keyword={keyword}')
+            URL + f'/labels?'
+                  f'labellevel={labellevel}&keyword={keyword}')
     else:
-        url_call = URL + f'/label?codeLevel={codeLevel}'
-    if standard:
-        url_call += f'&standard={standard}'
+        url_call = URL + f'/labels?labellevel={labellevel}'
+    if labelsource:
+        url_call += f'&labelsource={labelsource}'
     return url_call
 
 
 def clean_columns(df):
-    """Removes JSON prefixes from column names"""
-    df.columns = [c.split('.')[-1] for c in df.columns]
+    """Removes prefixes from column names"""
+    df.columns = [c.split('v_')[-1] for c in df.columns]
     return df
 
 
 def json_normalize(output):
     """Backwards compatability for old versions of pandas"""
     try:
         return pd.json_normalize(output)
     except AttributeError:
         return pd.io.json.json_normalize(output)
 
 
+def print_error(output):
+    """Handle and print out error for invalid API call"""
+    try:
+        print('ERROR:', output['message'])
+    except KeyError:
+        print('ERROR', output["errorMessage"])
+    return
+
+
 def reading_time(words, workday=8, workweek=5, workyear=50):
     """
     Returns a string detailing how long it takes to read a document based on
     how many words the document has. The function assumes an 8 hour work-day,
     a 5 day work-week, and a 50 week work-year.
     """
     text = ''
```

### Comparing `regcensus-0.4.5/setup.py` & `regcensus-1.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from distutils.core import setup
 import setuptools
 
 
 setup(
     name='regcensus',
-    version='0.4.5',
+    version='1.0.0',
     description='Python package for accessing data from the QuantGov API',
     url='https://github.com/QuantGov/regcensus-api-python',
     author='QuantGov',
     author_email='quantgov.info@gmail.com',
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `regcensus-0.4.5/tests/test_api.py` & `regcensus-1.0.0/tests/test_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,288 +11,272 @@
 
 
 # TEST FUNCTIONS
 
 # Tests for get_() functions
 def test_get_series():
     results = rc.get_series(verbose=1)
-    assert order_results(results, 'seriesID') == [
+    assert order_results(results, 'series_id') == [
         1, 2, 3, 4, 5, 6, 7, 8, 9, 10
     ]
 
 
 def test_get_agencies():
     results = rc.get_agencies(jurisdictionID=38, verbose=1)
-    assert order_results(results, 'agencyID') == [
+    assert order_results(results, 'agency_id') == [
         0, 9519, 9520, 9521, 9522, 9523, 9524, 9525, 9526, 9527
     ]
 
 
 def test_get_agencies_keyword():
     results = rc.get_agencies(keyword='Education', verbose=1)
-    assert order_results(results, 'agencyID') == [
-        46, 47, 48, 263, 264, 270, 271, 286, 394, 403
+    assert order_results(results, 'agency_id') == [
+        44, 45, 46, 47, 48, 49, 263, 264, 265, 266
     ]
 
 
 def test_get_agencies_error(capsys):
     results = rc.get_agencies()
     assert not results
     assert capsys.readouterr().out == (
         'Must include either "jurisdictionID" or "keyword."\n')
 
 
 def test_get_jurisdictions():
-    results = rc.get_jurisdictions(38, verbose=1)
-    assert order_results(results, 'jurisdictionID') == [38]
+    results = rc.get_jurisdictions(verbose=1)
+    assert order_results(results, 'jurisdiction_id') == [
+        2, 4, 10, 11, 14, 15, 17, 20, 23, 24
+    ]
 
 
 def test_get_industries():
     results = rc.get_industries(verbose=1)
-    assert order_results(results, 'industryCode') == [
-        '0', '111', '112', '114', '115', '211', '212', '213', '221', '236'
-    ]
-
-
-def test_get_industries_keyword():
-    results = rc.get_industries(keyword='Fishing', codeLevel=6, verbose=1)
-    assert order_results(results, 'industryCode') == [
-        '114111', '114112', '114119'
-    ]
-
-
-def test_get_documents_jurisdiction():
-    results = rc.get_documents(date=2020, jurisdictionID=44, verbose=1)
-    assert order_results(results, 'documentID') == [
-        3800000001, 3800000002, 3800000003, 3800000004, 3800000005,
-        3800000006, 3800000007, 3800000008, 3800000009, 3800000010
+    assert order_results(results, 'label_code') == [
+        '111', '112', '114', '115', '211', '212', '213', '221', '236', '311'
     ]
 
 
-def test_get_documents_missing_jurisdiction(capsys):
-    results = rc.get_documents(date=2020, jurisdictionID=None, verbose=1)
-    assert not results
-    assert capsys.readouterr().out == (
-        'Must include either "jurisdictionID and date" or "documentID."\n'
-    )
-
-
-def test_get_documents_document_id():
-    results = rc.get_documents(date=2020, documentID=3800000001, verbose=1)
-    assert results['documentReference'].values[0] == (
-        'Agency 01, Title 01, Chapter 01'
-    )
+# def test_get_industries_keyword():
+#     results = rc.get_industries(keyword='Fishing', labellevel=6, verbose=1)
+#     assert order_results(results, 'label_code') == [
+#         '114111', '114112', '114119'
+#     ]
 
 
-def test_get_versions():
-    results = rc.get_versions(38, verbose=1)
-    assert order_results(results, 'sourceName') == [
-        'Occupation Data (dataset)', 'Occupation Data (dataset)',
-        'RegData US 3.2 Annual (dataset)', 'RegData US 4.0 Annual (dataset)'
-    ]
+# def test_get_versions():
+#     results = rc.get_versions(38, verbose=1)
+#     assert order_results(results, 'source_name') == [
+#         'Occupation Data (dataset)', 'Occupation Data (dataset)',
+#         'RegData US 3.2 Annual (dataset)', 'RegData US 4.0 Annual (dataset)'
+#     ]
 
 
 # Tests for get_values()
 def test_get_document_values():
     results = rc.get_document_values(
-        series=[1, 2], jurisdiction=20, date='2020-06-02', verbose=1
+        series=[1, 2], jurisdiction=20, year=2020, verbose=1
     )
-    assert order_results(results, 'seriesValue', descending=True) == [
-        1958601.0, 466414.0, 248869.0, 236149.0, 133169.0,
-        103682.0, 98257.0, 90961.0, 90862.0, 90758.0
+    assert order_results(results, 'restrictions', descending=True) == [
+        27390, 11776, 3523, 2633, 1866, 1742, 1504, 1420, 1411, 1396
     ]
 
 
 def test_get_reading_time():
     results = rc.get_reading_time(
-        jurisdiction=20, date=[2015, 2021], documentType=1, verbose=1
+        jurisdiction=20, year=[2015, 2021], documentType=1, verbose=1
     )
-    assert order_results(results, 'seriesValue') == [
+    assert order_results(results, 'series_value') == [
         '23 weeks, 4 days',
         '23 weeks, 7 hours',
         '31 weeks, 2 days, 2 hours'
     ]
 
 
 def test_get_values_multiple_series():
     results = rc.get_values(
-        series=[1, 2], jurisdiction='United States', date=1970, verbose=1
+        series=[1, 2], jurisdiction='United States', year=1970, verbose=1
     )
-    assert order_results(results, 'seriesValue') == [409520.0, 33588985.0]
+    assert order_results(results, 'series_value') == [409520.0, 33588985.0]
 
 
 def test_get_values_incorrect_series(capsys):
-    results = rc.get_values(series=None, jurisdiction=38, date=2019)
+    results = rc.get_values(series=None, jurisdiction=38, year=2019)
     assert not results
-    assert capsys.readouterr().out == (
-        'Valid series ID required. Select from the following list:\n'
+    assert capsys.readouterr().out.split('\n')[0] == (
+        'No data was found for these parameters. For this jurisdiction, consider the following:'
     )
 
 
 def test_get_values_multiple_jurisdictions():
-    results = rc.get_values(series=1, jurisdiction=[58, 59], date=2019)
-    assert order_results(results, 'seriesValue') == [52569.0, 107063.0]
+    results = rc.get_values(series=1, jurisdiction=[58, 59], year=2019)
+    assert order_results(results, 'series_value') == [52569.0, 107063.0]
 
 
 def test_get_values_multiple_jurisdiction_names():
     results = rc.get_values(
-        series=1, jurisdiction=['Alaska', 'Alabama'], date=2019)
-    assert order_results(results, 'seriesValue') == [52569.0, 107063.0]
+        series=1, jurisdiction=['Alaska', 'Alabama'], year=2019)
+    assert order_results(results, 'series_value') == [52569.0, 107063.0]
 
 
 def test_get_values_all_industries():
     results = rc.get_values(
-        series=28, jurisdiction=58, date=2019, filtered=False
+        series=28, jurisdiction=58, year=2019, filtered=False
     )
-    assert order_results(results, 'seriesValue', descending=True) == [
-        2399.6540837686553, 2346.9849032768325,
-        2231.579487334733, 1910.4039869066692,
-        1858.660280573211, 1845.9105216636453,
-        1756.3024117016612, 1272.998498038447,
-        1214.762196061427, 1155.1694051386294
+    assert order_results(results, 'series_value', descending=True) == [
+        3596.1658897194,
+        3594.9787034937,
+        2399.6540837687,
+        2346.9849032768,
+        2231.5794873347,
+        1910.4039869067,
+        1858.6602805732,
+        1845.9105216636,
+        1756.3024117017,
+        1449.754496272
     ]
 
 
 def test_get_values_multiple_industries():
     results = rc.get_values(
-        series=28, jurisdiction=58, date=2019, industry=['22', '49', '50']
+        series=28, jurisdiction=58, year=2019, label=[111, 325, 621]
     )
-    assert order_results(results, 'seriesValue') == [
-        50.07550010907289, 649.0292048707197, 811.9319063696239
+    assert order_results(results, 'series_value') == [
+        16.4878001918,
+        18.2179003567,
+        28.033600058,
+        28.0808002906,
+        29.5395007168,
+        31.0861005918,
+        32.408500284,
+        33.9612003003,
+        35.1842004247,
+        35.3924005719
     ]
 
 
 def test_get_values_one_industry():
     results = rc.get_document_values(
-        series=28, jurisdiction=58, date='2019-05-15', industry='22'
+        series=28, jurisdiction=58, year=2019, label=111
     )
-    assert order_results(results, 'seriesValue', descending=True) == [
-        0.9902999997138977, 0.9789999723434448,
-        0.9735000133514404, 0.9034000039100647,
-        0.847599983215332, 0.6302000284194946,
-        0.5533000230789185, 0.3864000141620636,
-        0.3547999858856201, 0.3547999858856201
+    assert order_results(results, 'label_value', descending=True) == [
+        0.9903, 0.979, 0.9735, 0.9034, 0.8476,
+        0.6302, 0.5533, 0.3864, 0.3548, 0.3548
     ]
 
 
-def test_get_values_4digit_industries():
-    results = rc.get_values(
-        series=28, jurisdiction=38, date=2019, filtered=False, industryLevel=4
-    )
-    assert order_results(results, 'seriesValue', descending=True) == [
-        48819.60270605631,
-        19666.03264030083,
-        18530.05033682113,
-        15972.102057352553,
-        15476.846815471901,
-        15132.83348125431,
-        6506.98745361498,
-        6490.635489263841,
-        6228.529536121532,
-        5282.724979804712
-    ]
+# def test_get_values_4digit_industries():
+#     results = rc.get_values(
+#         series=28, jurisdiction=38, year=2019, filtered=False, industryLevel=4
+#     )
+#     assert order_results(results, 'series_value', descending=True) == [
+#         48819.60270605631,
+#         19666.03264030083,
+#         18530.05033682113,
+#         15972.102057352553,
+#         15476.846815471901,
+#         15132.83348125431,
+#         6506.98745361498,
+#         6490.635489263841,
+#         6228.529536121532,
+#         5282.724979804712
+#     ]
 
 
 def test_get_values_incorrect_jurisdiction(capsys):
-    results = rc.get_values(series=1, jurisdiction=None, date=2019)
+    results = rc.get_values(series=1, jurisdiction=None, year=2019)
     assert not results
-    assert capsys.readouterr().out == 'Valid jurisdiction ID required.\n'
+    assert capsys.readouterr().out.split('\n')[0] == (
+       'Valid jurisdiction ID required. Consider the following:'
+    )
 
 
-def test_get_values_date_range():
-    results = rc.get_values(series=1, jurisdiction=38, date=[1970, 2019])
-    assert order_results(results, 'seriesValue') == [
+def test_get_values_year_range():
+    results = rc.get_values(series=1, jurisdiction=38, year=[1970, 2019])
+    assert order_results(results, 'series_value') == [
         409520.0, 420478.0, 456373.0, 475121.0, 505136.0,
         530148.0, 554052.0, 579879.0, 590779.0, 625123.0
     ]
 
 
-def test_get_values_multiple_dates():
+def test_get_values_multiple_years():
     results = rc.get_values(
-        series=1, jurisdiction=38, date=[1970, 1980, 1990, 2000]
+        series=1, jurisdiction=38, year=[1970, 1980, 1990, 2000]
     )
-    assert order_results(results, 'seriesValue') == [
-        409520.0, 643935.0, 786512.0, 853667.0
+    assert order_results(results, 'series_value') == [
+        409520.0, 643935.0, 785747.0, 853667.0
     ]
 
 
-def test_get_values_incorrect_dates(capsys):
-    results = rc.get_values(series=1, jurisdiction=38, date=None, verbose=1)
+def test_get_values_incorrect_years(capsys):
+    results = rc.get_values(series=1, jurisdiction=38, year=None, verbose=1)
     assert not results
-    assert capsys.readouterr().out == (
-        'Valid date is required. Select from the following list:\n'
-        'API call: https://api.quantgov.org/seriesperiod?jurisdiction=38\n')
+    assert capsys.readouterr().out.split('\n')[0] == (
+        'No data was found for these parameters. For this jurisdiction, consider the following:'
+    )
 
 
-def test_get_values_country():
-    results = rc.get_values(series=1, jurisdiction=38, date=2019, country=True)
-    assert order_results(results, 'seriesValue') == [
-        43940.0, 50646.0, 51925.0, 52569.0, 60086.0,
-        63735.0, 70969.0, 78004.0, 82706.0, 92522.0
-    ]
+# def test_get_values_country():
+#     results = rc.get_values(series=1, jurisdiction=38, year=2019, country=True)
+#     assert order_results(results, 'series_value') == [
+#         43940.0, 50646.0, 51925.0, 52569.0, 60086.0,
+#         63735.0, 70969.0, 78004.0, 82706.0, 92522.0
+#     ]
 
 
 def test_get_values_agency():
-    results = rc.get_values(series=13, jurisdiction=66, date=2021, agency=8777)
-    assert order_results(results, 'seriesValue') == [4305.0]
+    results = rc.get_values(series=13, jurisdiction=66, year=2021, agency=8777)
+    assert order_results(results, 'series_value') == [4305.0]
 
 
 def test_get_values_all_agencies():
     results = rc.get_values(
-        series=13, jurisdiction=66, date=2021
+        series=13, jurisdiction=66, year=2021
     )
-    assert order_results(results, 'seriesValue') == [
+    assert order_results(results, 'series_value') == [
         0.0, 1.0, 1.0, 2.0, 2.0, 2.0, 4.0, 4.0, 5.0, 5.0
     ]
 
 
 def test_get_values_multiple_agencies():
     results = rc.get_values(
-        series=13, jurisdiction=66, date=2021, agency=[8777, 8813]
+        series=13, jurisdiction=66, year=2021, agency=[8777, 8813]
     )
-    assert order_results(results, 'seriesValue') == [3311.0, 4305.0]
+    assert order_results(results, 'series_value') == [3311.0, 4305.0]
 
 
-def test_get_values_version():
-    results = rc.get_values(
-        series=1, jurisdiction=38, date=2019, version=1, verbose=1
-    )
-    assert order_results(results, 'seriesValue') == [1078213.0]
+# def test_get_values_version():
+#     results = rc.get_values(
+#         series=1, jurisdiction=38, year=2019, version=1, verbose=1
+#     )
+#     assert order_results(results, 'series_value') == [1078213.0]
 
 
 def test_get_values_download():
     results = rc.get_values(
-        series=13, jurisdiction=66, date=2021, agency=8777, download='test.csv'
+        series=13, jurisdiction=66, year=2021, agency=8777, download='test.csv'
     )
     assert not results
     assert os.path.exists('test.csv')
     os.remove('test.csv')
 
 
 def test_get_values_incorrect_download(capsys):
     results = rc.get_values(
-        series=13, jurisdiction=66, date=2021, agency=8777, download=True
+        series=13, jurisdiction=66, year=2021, agency=8777, download=True
     )
     assert not results
     assert capsys.readouterr().out == 'Valid outpath required to download.\n'
 
 
 def test_get_values_error(capsys):
-    results = rc.get_values(series=1, jurisdiction=38, date=1900)
+    results = rc.get_values(series=1, jurisdiction=38, year=1900)
     assert not results
-    assert capsys.readouterr().out == (
-        'WARNING: SeriesValue was not found for the specified parameters. '
-        'Please check that you have selected the right combination of '
-        'parameters.  When in doubt, please use the /periods endpoint to '
-        'find out the combinations of series, jurisdiction, periods, '
-        'agencies, document types for which there are data available.'
-        '{parameters={jurisdiction=[US_UNITED_STATES], date=[1900], '
-        'labelLevel=[3], agency=null, dateIsRange=false, filteredOnly=false, '
-        'label=null, series=[SERIES_1], documentType=null, '
-        'national=false, cluster=null}}\n')
+    assert capsys.readouterr().out.split('\n')[0] == (
+        'No data was found for these parameters. For this jurisdiction, consider the following:'
+    )
 
 
 # Tests for list_() functions
 def test_list_document_types():
     results = rc.list_document_types()
     assert results['Regulation text All regulations'] == 1
 
@@ -300,24 +284,21 @@
 def test_list_document_types_jurisdiction():
     results = rc.list_document_types(jurisdictionID=38)
     assert results['Regulation text All regulations'] == 1
 
 
 def test_list_series():
     results = rc.list_series()
-    assert results['Complexity Conditionals'] == 53
+    assert results['Conditionals'] == 53
 
 
 def test_list_dates():
     results = rc.list_dates(44)
-    assert list(reversed(results))[:12] == [
-        '2021-05-11', '2021',
-        '2020-04-28', '2020',
-        '2019-07-01', '2019',
-        '2018-05-23', '2018'
+    assert list(reversed(results)) == [
+        2022, 2021, 2020, 2019, 2018
     ]
 
 
 def test_list_agencies():
     results = rc.list_agencies(jurisdictionID=66)
     assert results['wild animals'] == 8867
 
@@ -336,24 +317,24 @@
 
 def test_list_jurisdictions():
     results = rc.list_jurisdictions()
     assert results['Alabama'] == 59
 
 
 def test_list_industries():
-    results = rc.list_industries(codeLevel=6)
+    results = rc.list_industries(labellevel=6)
     assert results['Wood Container and Pallet Manufacturing (321920)'] == 1170
 
 
 def test_list_industries_onlyID():
-    results = rc.list_industries(codeLevel=6, onlyID=True)
+    results = rc.list_industries(labellevel=6, onlyID=True)
     assert results['321920'] == 1170
 
 
-def test_list_industries_keyword():
-    results = rc.list_industries(codeLevel=4, keyword='fishing')
-    assert results['Fishing (1141)'] == 126
+# def test_list_industries_keyword():
+#    results = rc.list_industries(labellevel=4, keyword='fishing')
+#    assert results['Fishing (1141)'] == 126
 
 
-def test_list_bea_industries():
-    results = rc.list_industries(standard='BEA')
-    assert results['Accommodation and food services (BEA) (79)'] == 1974
+# def test_list_bea_industries():
+#     results = rc.list_industries(labelsource='BEA')
+#     assert results['Accommodation and food services (BEA) (79)'] == 1974
```

