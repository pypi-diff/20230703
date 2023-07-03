# Comparing `tmp/influxdb3-python-0.1.4.tar.gz` & `tmp/influxdb3-python-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "influxdb3-python-0.1.4.tar", last modified: Fri Jun  2 16:50:59 2023, max compression
+gzip compressed data, was "influxdb3-python-0.1.5.tar", last modified: Mon Jul  3 14:10:43 2023, max compression
```

## Comparing `influxdb3-python-0.1.4.tar` & `influxdb3-python-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:50:59.654442 influxdb3-python-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-02 16:50:50.000000 influxdb3-python-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-06-02 16:50:59.650442 influxdb3-python-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-06-02 16:50:50.000000 influxdb3-python-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:50:59.650442 influxdb3-python-0.1.4/influxdb3_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-06-02 16:50:59.000000 influxdb3-python-0.1.4/influxdb3_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-02 16:50:59.000000 influxdb3-python-0.1.4/influxdb3_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 16:50:59.000000 influxdb3-python-0.1.4/influxdb3_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-02 16:50:59.000000 influxdb3-python-0.1.4/influxdb3_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 16:50:59.000000 influxdb3-python-0.1.4/influxdb3_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:50:59.650442 influxdb3-python-0.1.4/influxdb_client_3/
--rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-06-02 16:50:50.000000 influxdb3-python-0.1.4/influxdb_client_3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-06-02 16:50:50.000000 influxdb3-python-0.1.4/influxdb_client_3/read_file.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 16:50:59.654442 influxdb3-python-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-02 16:50:50.000000 influxdb3-python-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:50:59.650442 influxdb3-python-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-02 16:50:50.000000 influxdb3-python-0.1.4/tests/test_influxdb_client_3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:43.538594 influxdb3-python-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-03 14:10:30.000000 influxdb3-python-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-07-03 14:10:43.538594 influxdb3-python-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-07-03 14:10:30.000000 influxdb3-python-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:43.538594 influxdb3-python-0.1.5/influxdb3_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-07-03 14:10:43.000000 influxdb3-python-0.1.5/influxdb3_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-03 14:10:43.000000 influxdb3-python-0.1.5/influxdb3_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 14:10:43.000000 influxdb3-python-0.1.5/influxdb3_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-03 14:10:43.000000 influxdb3-python-0.1.5/influxdb3_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-03 14:10:43.000000 influxdb3-python-0.1.5/influxdb3_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:43.538594 influxdb3-python-0.1.5/influxdb_client_3/
+-rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-07-03 14:10:30.000000 influxdb3-python-0.1.5/influxdb_client_3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-03 14:10:30.000000 influxdb3-python-0.1.5/influxdb_client_3/read_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 14:10:43.538594 influxdb3-python-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-03 14:10:30.000000 influxdb3-python-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:10:43.538594 influxdb3-python-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-03 14:10:30.000000 influxdb3-python-0.1.5/tests/test_influxdb_client_3.py
```

### Comparing `influxdb3-python-0.1.4/LICENSE` & `influxdb3-python-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.1.4/influxdb_client_3/__init__.py` & `influxdb3-python-0.1.5/influxdb_client_3/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,178 +1,173 @@
-# influxdb_client_3/__init__.py
-
+import json
+import urllib.parse
 import pyarrow as pa
-from pyarrow.flight import FlightClient, Ticket, FlightCallOptions
-from influxdb_client import InfluxDBClient as _InfluxDBClient
-from influxdb_client import WriteOptions as WriteOptions
-from influxdb_client.client.write_api import WriteApi as _WriteApi
-from influxdb_client.client.write_api import SYNCHRONOUS, ASYNCHRONOUS, PointSettings
+from influxdb_client import InfluxDBClient as _InfluxDBClient, WriteOptions, Point
+from influxdb_client.client.write_api import WriteApi as _WriteApi, SYNCHRONOUS, ASYNCHRONOUS, PointSettings
 from influxdb_client.domain.write_precision import WritePrecision
 from influxdb_client.client.exceptions import InfluxDBError
-from influxdb_client import Point
-import json
-
+from pyarrow.flight import FlightClient, Ticket, FlightCallOptions
 from influxdb_client_3.read_file import upload_file
 
 
 def write_client_options(**kwargs):
     return kwargs
 
 
 def flight_client_options(**kwargs):
     return kwargs  # You can replace this with a specific data structure if needed
 
-
 class InfluxDBClient3:
     def __init__(
             self,
             host=None,
             org=None,
             database=None,
             token=None,
-            _write_client_options=None,
-            _flight_client_options=None,
+            write_client_options=None,
+            flight_client_options=None,
             **kwargs):
         """
-        This class provides an interface for interacting with an InfluxDB server, simplifying common operations such as writing, querying.
-        * host (str, optional): The hostname or IP address of the InfluxDB server. Defaults to None.
-        * org (str, optional): The InfluxDB organization name to be used for operations. Defaults to None.
-        * database (str, optional): The database to be used for InfluxDB operations. Defaults to None.
-        * token (str, optional): The authentication token for accessing the InfluxDB server. Defaults to None.
-        * write_options (ANY, optional): Exposes InfuxDB WriteAPI options.
-        * **kwargs: Additional arguments to be passed to the InfluxDB Client.
+        Initialize an InfluxDB client.
+
+        :param host: The hostname or IP address of the InfluxDB server.
+        :type host: str
+        :param org: The InfluxDB organization name for operations.
+        :type org: str
+        :param database: The database for InfluxDB operations.
+        :type database: str
+        :param token: The authentication token for accessing the InfluxDB server.
+        :type token: str
+        :param write_client_options: Options for the WriteAPI.
+        :type write_client_options: dict
+        :param flight_client_options: Options for the FlightClient.
+        :type flight_client_options: dict
+        :param kwargs: Additional arguments for the InfluxDB Client.
         """
         self._org = org
         self._database = database
-        self._write_client_options = _write_client_options if _write_client_options is not None else write_client_options(write_options=SYNCHRONOUS)
+        self._write_client_options = write_client_options or {'write_options': SYNCHRONOUS}
+
+        # Extracting the hostname from URL if provided
+        parsed_url = urllib.parse.urlparse(host)
+        host = parsed_url.hostname or host
+
         self._client = _InfluxDBClient(
             url=f"https://{host}",
             token=token,
             org=self._org,
             **kwargs)
         
-        self._write_api = _WriteApi(
-            self._client, **self._write_client_options)
-
-        self._flight_client_options = _flight_client_options if _flight_client_options is not None else {}
-        self._flight_client = FlightClient(
-            f"grpc+tls://{host}:443",
-            **self._flight_client_options)
+        self._write_api = _WriteApi(self._client, **self._write_client_options)
+        self._flight_client_options = flight_client_options or {}
+        self._flight_client = FlightClient(f"grpc+tls://{host}:443", **self._flight_client_options)
         
-        # create an authorization header
-        self._options = FlightCallOptions(
-            headers=[(b"authorization", f"Bearer {token}".encode('utf-8'))])
+        # Create an authorization header
+        self._options = FlightCallOptions(headers=[(b"authorization", f"Bearer {token}".encode('utf-8'))])
 
     def write(self, record=None, **kwargs):
         """
         Write data to InfluxDB.
 
-        :type database: str
         :param record: The data point(s) to write.
         :type record: Point or list of Point objects
         :param kwargs: Additional arguments to pass to the write API.
         """
         try:
-            self._write_api.write(
-                bucket=self._database, record=record, **kwargs)
-        except Exception as e:
-            print(e)
+            self._write_api.write(bucket=self._database, record=record, **kwargs)
+        except InfluxDBError as e:
+            print(f"InfluxDB Error: {e}")
 
-    def write_file(
-            self,
-            file,
-            measurement_name=None,
-            tag_columns=[],
-            timestamp_column='time',
-            **kwargs):
+    def write_file(self, file, measurement_name=None, tag_columns=None, timestamp_column='time', **kwargs):
         """
-        Write data from a  file to InfluxDB.
+        Write data from a file to InfluxDB.
 
         :param file: The file to write.
+        :type file: str
+        :param measurement_name: The name of the measurement.
+        :type measurement_name: str
+        :param tag_columns: Tag columns.
+        :type tag_columns: list
+        :param timestamp_column: Timestamp column name. Defaults to 'time'.
+        :type timestamp_column: str
         :param kwargs: Additional arguments to pass to the write API.
         """
         try:
-            rf = upload_file(file)
-            Table = rf.load_file()
-
-            if isinstance(Table, pa.Table):
-                df = Table.to_pandas()
-            else:
-                df = Table
-            print(df)
-
-            measurement_column = None
-
-            if measurement_name is None:
-                if 'measurement' in df.columns:
-                        measurement_column = 'measurement'
-                elif 'iox::measurement' in df.columns:
-                        measurement_column = 'iox::measurement'
-
-                if measurement_column is not None:
-                    unique_measurements = df[measurement_column].unique()
-                    for measurement in unique_measurements:
-                        df_measurement = df[df[measurement_column] == measurement]
-                        df_measurement = df_measurement.drop(columns=[measurement_column])
-                        print(df_measurement)
-                        self._write_api.write(bucket=self._database, record=df_measurement,
-                                            data_frame_measurement_name=measurement,
-                                            data_frame_tag_columns=tag_columns,
-                                            data_frame_timestamp_column=timestamp_column)
-                else:
-                    print("'measurement' column not found in the dataframe.")
-            else:
-                if 'measurement' in df.columns:
-                    df = df.drop(columns=['measurement'])
-                self._write_api.write(bucket=self._database, record=df,
-                                    data_frame_measurement_name=measurement_name,
-                                    data_frame_tag_columns=tag_columns,
-                                    data_frame_timestamp_column=timestamp_column)
+            table = upload_file(file).load_file()
+            df = table.to_pandas() if isinstance(table, pa.Table) else table
+            self._process_dataframe(df, measurement_name, tag_columns or [], timestamp_column)
         except Exception as e:
-            print(e)
+            print(f"Error writing file: {e}")
 
-    def query(self, query, language="sql"):
-        # create a flight client pointing to the InfluxDB
-        # create a ticket
-        ticket_data = {
-            "database": self._database,
-            "sql_query": query,
-            "query_type": language}
-
-        ticket_bytes = json.dumps(ticket_data)
-        ticket = Ticket(ticket_bytes)
-
-        # execute the query and return all the data
+    def _process_dataframe(self, df, measurement_name, tag_columns, timestamp_column):
+        # This function is factored out for clarity.
+        # It processes a DataFrame before writing to InfluxDB.
+
+        measurement_column = None
+        if measurement_name is None:
+            measurement_column = next((col for col in ['measurement', 'iox::measurement'] if col in df.columns), None)
+            if measurement_column:
+                for measurement in df[measurement_column].unique():
+                    df_measurement = df[df[measurement_column] == measurement].drop(columns=[measurement_column])
+                    self._write_api.write(bucket=self._database, record=df_measurement,
+                                          data_frame_measurement_name=measurement,
+                                          data_frame_tag_columns=tag_columns,
+                                          data_frame_timestamp_column=timestamp_column)
+            else:
+                print("'measurement' column not found in the dataframe.")
+        else:
+            df = df.drop(columns=['measurement'], errors='ignore')
+            self._write_api.write(bucket=self._database, record=df,
+                                  data_frame_measurement_name=measurement_name,
+                                  data_frame_tag_columns=tag_columns,
+                                  data_frame_timestamp_column=timestamp_column)
+
+    def query(self, query, language="sql", mode="all"):
+        """
+        Query data from InfluxDB.
+
+        :param query: The query string.
+        :type query: str
+        :param language: The query language (default is "sql").
+        :type language: str
+        :param mode: The mode of fetching data (all, pandas, chunk, reader, schema).
+        :type mode: str
+        :return: The queried data.
+        """
+        ticket_data = {"database": self._database, "sql_query": query, "query_type": language}
+        ticket = Ticket(json.dumps(ticket_data).encode('utf-8'))
         flight_reader = self._flight_client.do_get(ticket, self._options)
 
-        # use read_all() to get all of the data as an Arrow table
-        # there are other functions to iterate through rows or read only parts of the data
-        # which is useful if you have huge data sets
-        return flight_reader.read_all()
+        mode_func = {
+            "all": flight_reader.read_all,
+            "pandas": flight_reader.read_pandas,
+            "chunk": lambda: flight_reader,
+            "reader": flight_reader.to_reader,
+            "schema": lambda: flight_reader.schema
+        }.get(mode, flight_reader.read_all)
+
+        return mode_func() if callable(mode_func) else mode_func
 
     def close(self):
-        # Clean up resources here.
-        # Call close method of _write_api and _flight_client, if they exist.
-        if hasattr(self._write_api, 'close'):
-            self._write_api.close()
-        if hasattr(self._flight_client, 'close'):
-            self._flight_client.close()
-        if hasattr(self._client, 'close'):
-            self._client.close()
+        """Close the client and clean up resources."""
+        self._write_api.close()
+        self._flight_client.close()
+        self._client.close()
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
 
 
 __all__ = [
     "InfluxDBClient3",
     "Point",
     "PointSettings",
     "SYNCHRONOUS",
     "ASYNCHRONOUS",
-    "write_client_options",
     "WritePrecision",
-    "flight_client_options",
-    "WriteOptions"]
+    "WriteOptions",
+    "write_client_options",
+    "flight_client_options"
+]
```

### Comparing `influxdb3-python-0.1.4/influxdb_client_3/read_file.py` & `influxdb3-python-0.1.5/influxdb_client_3/read_file.py`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.1.4/setup.py` & `influxdb3-python-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `influxdb3-python-0.1.4/tests/test_influxdb_client_3.py` & `influxdb3-python-0.1.5/tests/test_influxdb_client_3.py`

 * *Files identical despite different names*

