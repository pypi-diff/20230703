# Comparing `tmp/lakeapi2sql-0.1.0.tar.gz` & `tmp/lakeapi2sql-0.2.0.tar.gz`

## Comparing `lakeapi2sql-0.1.0.tar` & `lakeapi2sql-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
--rw-r--r--   0        0        0      892 1970-01-01 00:00:00.000000 lakeapi2sql-0.1.0/Cargo.toml
--rw-r--r--   0     1001      123      118 2023-06-30 05:24:53.000000 lakeapi2sql-0.1.0/.editorconfig
--rw-r--r--   0     1001      123     2800 2023-06-30 05:24:53.000000 lakeapi2sql-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      123     3086 2023-06-30 05:24:53.000000 lakeapi2sql-0.1.0/.gitignore
--rw-r--r--   0     1001      123     1081 2023-06-30 05:24:53.000000 lakeapi2sql-0.1.0/LICENSE
--rw-r--r--   0     1001      123     1066 2023-06-30 05:24:53.000000 lakeapi2sql-0.1.0/README.md
--rw-r--r--   0     1001      123        0 2023-06-30 05:24:53.000000 lakeapi2sql-0.1.0/lakeapi2sql/__init__.py
--rw-r--r--   0     1001      123      306 2023-06-30 05:24:53.000000 lakeapi2sql-0.1.0/lakeapi2sql/bulk_insert.py
--rw-r--r--   0     1001      123      587 2023-06-30 05:24:53.000000 lakeapi2sql-0.1.0/pyproject.toml
--rw-r--r--   0     1001      123    13325 2023-06-30 05:24:53.000000 lakeapi2sql-0.1.0/src/arrow_convert.rs
--rw-r--r--   0     1001      123     2417 2023-06-30 05:24:53.000000 lakeapi2sql-0.1.0/src/bulk_insert.rs
--rw-r--r--   0     1001      123     1539 2023-06-30 05:24:53.000000 lakeapi2sql-0.1.0/src/connect.rs
--rw-r--r--   0     1001      123     1599 2023-06-30 05:24:53.000000 lakeapi2sql-0.1.0/src/lib.rs
--rw-r--r--   0     1001      123    46692 2023-06-30 05:24:53.000000 lakeapi2sql-0.1.0/Cargo.lock
--rw-r--r--   0        0        0     1419 1970-01-01 00:00:00.000000 lakeapi2sql-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      955 1970-01-01 00:00:00.000000 lakeapi2sql-0.2.0/Cargo.toml
+-rw-r--r--   0     1001      123      118 2023-07-03 09:37:40.000000 lakeapi2sql-0.2.0/.editorconfig
+-rw-r--r--   0     1001      123     2800 2023-07-03 09:37:40.000000 lakeapi2sql-0.2.0/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123     3086 2023-07-03 09:37:40.000000 lakeapi2sql-0.2.0/.gitignore
+-rw-r--r--   0     1001      123     1081 2023-07-03 09:37:40.000000 lakeapi2sql-0.2.0/LICENSE
+-rw-r--r--   0     1001      123     1066 2023-07-03 09:37:40.000000 lakeapi2sql-0.2.0/README.md
+-rw-r--r--   0     1001      123        0 2023-07-03 09:37:40.000000 lakeapi2sql-0.2.0/lakeapi2sql/__init__.py
+-rw-r--r--   0     1001      123      320 2023-07-03 09:37:40.000000 lakeapi2sql-0.2.0/lakeapi2sql/bulk_insert.py
+-rw-r--r--   0     1001      123      587 2023-07-03 09:37:40.000000 lakeapi2sql-0.2.0/pyproject.toml
+-rw-r--r--   0     1001      123    12800 2023-07-03 09:37:40.000000 lakeapi2sql-0.2.0/src/arrow_convert.rs
+-rw-r--r--   0     1001      123     2504 2023-07-03 09:37:40.000000 lakeapi2sql-0.2.0/src/bulk_insert.rs
+-rw-r--r--   0     1001      123     1568 2023-07-03 09:37:40.000000 lakeapi2sql-0.2.0/src/connect.rs
+-rw-r--r--   0     1001      123     2680 2023-07-03 09:37:40.000000 lakeapi2sql-0.2.0/src/lib.rs
+-rw-r--r--   0     1001      123        0 2023-07-03 09:37:40.000000 lakeapi2sql-0.2.0/test/__init__.py
+-rw-r--r--   0     1001      123     1977 2023-07-03 09:37:40.000000 lakeapi2sql-0.2.0/test/test_insert.py
+-rw-r--r--   0     1001      123    57698 2023-07-03 09:37:40.000000 lakeapi2sql-0.2.0/Cargo.lock
+-rw-r--r--   0        0        0     1419 1970-01-01 00:00:00.000000 lakeapi2sql-0.2.0/PKG-INFO
```

### Comparing `lakeapi2sql-0.1.0/Cargo.toml` & `lakeapi2sql-0.2.0/Cargo.toml`

 * *Files 9% similar despite different names*

```diff
@@ -5,19 +5,21 @@
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "lake2sql"
 crate-type = ["lib","cdylib"]
 
 [dependencies]
-arrow2 = {version = "0.17.2", features = ["io_ipc"] }
+arrow = {version = "42.0.0", features = ["ipc_compression"] }
 futures = "0.3.28"
+log = "0.4.19"
 pyo3-asyncio ={ version = "0.18", features = ["attributes", "tokio-runtime"] }
+pyo3-log = "0.8.2"
 reqwest = {version = "0.11.18", features = ["stream"]}
-tiberius = {version = "0.12.2", features = ["time"] }
+tiberius = {version = "0.12.2", features = ["time", "sql-browser-tokio"] }
 time = "0.3.22"
 tokio = {version ="1.28.2", features=["net", "macros"]}
 tokio-util = {version = "0.7.8", features=["compat","io-util","io"]}
 
 [target.'cfg(unix)'.dependencies]
 openssl = { version = "0.10", features = ["vendored"] }
```

### Comparing `lakeapi2sql-0.1.0/.github/workflows/CI.yml` & `lakeapi2sql-0.2.0/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.1.0/.gitignore` & `lakeapi2sql-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.1.0/LICENSE` & `lakeapi2sql-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.1.0/README.md` & `lakeapi2sql-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.1.0/pyproject.toml` & `lakeapi2sql-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["maturin>=1.1,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "lakeapi2sql"
 requires-python = ">=3.10"
-version = "0.1.0"
+version = "0.2.0"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
```

### Comparing `lakeapi2sql-0.1.0/src/arrow_convert.rs` & `lakeapi2sql-0.2.0/src/arrow_convert.rs`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,28 @@
-use arrow2::array::Array;
-use arrow2::array::BooleanArray;
-use arrow2::array::Float16Array;
-use arrow2::array::Int32Array;
-use arrow2::array::NullArray;
-use arrow2::array::PrimitiveArray;
-use arrow2::array::Utf8Array;
-use arrow2::chunk::Chunk;
+use arrow::array::Array;
+use arrow::array::BooleanArray;
+use arrow::array::Date32Array;
+use arrow::array::Date64Array;
+use arrow::array::Float16Array;
+use arrow::array::Float32Array;
+use arrow::array::Float64Array;
+use arrow::array::Int16Array;
+use arrow::array::Int32Array;
+use arrow::array::Int64Array;
+use arrow::array::Int8Array;
+use arrow::array::LargeStringArray;
+use arrow::array::StringArray;
+use arrow::array::Time32SecondArray;
+use arrow::array::TimestampMicrosecondArray;
+use arrow::array::TimestampMillisecondArray;
+use arrow::array::UInt16Array;
+use arrow::array::UInt32Array;
+use arrow::array::UInt64Array;
+use arrow::array::UInt8Array;
+use arrow::record_batch::RecordBatch;
 use std::borrow::Cow;
 use std::time::Duration as StdDuration;
 use tiberius::time::time::Date;
 use tiberius::time::time::PrimitiveDateTime;
 use tiberius::time::time::Time;
 use tiberius::ColumnData;
 use tiberius::IntoSql;
@@ -33,285 +46,274 @@
 fn to_time(val: Option<Time>) -> ColumnData<'static> {
     return match val.to_sql() {
         ColumnData::Time(x) => ColumnData::Time(x),
         _ => panic!("should be mapped"),
     };
 }
 
-pub(crate) fn get_token_rows<'a>(batch: &'a Chunk<Box<dyn Array>>) -> Vec<TokenRow<'a>> {
+pub(crate) fn get_token_rows<'a>(batch: &'a RecordBatch) -> Vec<TokenRow<'a>> {
     let unix_min_date =
         Date::from_calendar_date(1970, tiberius::time::time::Month::January, 1).unwrap();
     let unix_min: PrimitiveDateTime = unix_min_date.with_time(Time::from_hms(0, 0, 0).unwrap());
 
-    let cols = batch.columns();
-    let rows = batch.len();
-    let mut token_rows: Vec<TokenRow> = vec![TokenRow::new(); rows];
-
-    for col in cols {
+    let rows = batch.num_rows();
+    let mut token_rows: Vec<TokenRow> = vec![TokenRow::new(); rows.try_into().unwrap()];
+    for col in batch.columns() {
         //For docs: col.data_type().to_physical_type()
         match col.data_type() {
-            arrow2::datatypes::DataType::Boolean => {
+            arrow::datatypes::DataType::Boolean => {
                 let ba = col.as_any().downcast_ref::<BooleanArray>().unwrap();
 
                 let mut rowindex = 0;
                 for val in ba.iter() {
                     token_rows[rowindex].push(val.into_sql());
                     rowindex += 1;
                 }
             }
-            arrow2::datatypes::DataType::Int32 => {
+            arrow::datatypes::DataType::Int32 => {
                 let ba = col.as_any().downcast_ref::<Int32Array>().unwrap();
 
                 let mut rowindex = 0;
                 for val in ba.iter() {
-                    token_rows[rowindex].push(ColumnData::I32(val.copied()));
+                    token_rows[rowindex].push(ColumnData::I32(val));
                     rowindex += 1;
                 }
             }
-            arrow2::datatypes::DataType::Utf8 => {
-                let ba = col.as_any().downcast_ref::<Utf8Array<i32>>().unwrap();
+            arrow::datatypes::DataType::Utf8 => {
+                let ba = col.as_any().downcast_ref::<StringArray>().unwrap();
 
                 let mut rowindex = 0;
                 for val in ba.iter() {
                     token_rows[rowindex].push(ColumnData::String(match val {
                         Some(vs) => Some(Cow::from(vs)),
                         None => None,
                     }));
                     rowindex += 1;
                 }
             }
-            arrow2::datatypes::DataType::LargeUtf8 => {
-                let ba = col.as_any().downcast_ref::<Utf8Array<i64>>().unwrap();
+            arrow::datatypes::DataType::LargeUtf8 => {
+                let ba = col.as_any().downcast_ref::<LargeStringArray>().unwrap();
 
                 let mut rowindex = 0;
                 for val in ba.iter() {
                     token_rows[rowindex].push(ColumnData::String(match val {
                         Some(vs) => Some(Cow::from(vs)),
                         None => None,
                     }));
                     rowindex += 1;
                 }
             }
-            arrow2::datatypes::DataType::Timestamp(
-                arrow2::datatypes::TimeUnit::Millisecond,
+            arrow::datatypes::DataType::Timestamp(
+                arrow::datatypes::TimeUnit::Millisecond,
                 None,
             ) => {
-                let ba = col.as_any().downcast_ref::<PrimitiveArray<i64>>().unwrap();
+                let ba = col.as_any().downcast_ref::<TimestampMillisecondArray>().unwrap();
 
                 let mut rowindex = 0;
                 for val in ba.iter() {
                     let dt_val = match val {
-                        Some(vs) => Some(unix_min + StdDuration::from_millis(*vs as u64)),
+                        Some(vs) => Some(unix_min + StdDuration::from_millis(vs as u64)),
                         None => None,
                     };
                     token_rows[rowindex].push(to_datetime(dt_val));
                     rowindex += 1;
                 }
             }
-            arrow2::datatypes::DataType::Timestamp(
-                arrow2::datatypes::TimeUnit::Microsecond,
+            arrow::datatypes::DataType::Timestamp(
+                arrow::datatypes::TimeUnit::Microsecond,
                 None,
             ) => {
-                let ba = col.as_any().downcast_ref::<PrimitiveArray<i64>>().unwrap();
+                let ba = col.as_any().downcast_ref::<TimestampMicrosecondArray>().unwrap();
 
                 let mut rowindex = 0;
                 for val in ba.iter() {
                     let dt_val = match val {
-                        Some(vs) => Some(unix_min + StdDuration::from_micros(*vs as u64)),
+                        Some(vs) => Some(unix_min + StdDuration::from_micros(vs as u64)),
                         None => None,
                     };
                     token_rows[rowindex].push(to_datetime(dt_val));
                     rowindex += 1;
                 }
             }
-            arrow2::datatypes::DataType::Null => {
+            arrow::datatypes::DataType::Null => {
                 for rowindex in 0..rows {
                     token_rows[rowindex].push(ColumnData::I32(None));
                 }
             }
-            arrow2::datatypes::DataType::UInt8 => {
-                let ba = col.as_any().downcast_ref::<PrimitiveArray<u8>>().unwrap();
+            arrow::datatypes::DataType::UInt8 => {
+                let ba = col.as_any().downcast_ref::<UInt8Array>().unwrap();
 
                 let mut rowindex = 0;
                 for val in ba.iter() {
-                    token_rows[rowindex].push(ColumnData::U8(val.copied()));
+                    token_rows[rowindex].push(ColumnData::U8(val));
                     rowindex += 1;
                 }
             }
-            arrow2::datatypes::DataType::Int8 => {
-                let ba = col.as_any().downcast_ref::<PrimitiveArray<i8>>().unwrap();
+            arrow::datatypes::DataType::Int8 => {
+                let ba = col.as_any().downcast_ref::<Int8Array>().unwrap();
 
                 let mut rowindex = 0;
                 for val in ba.iter() {
                     token_rows[rowindex].push(ColumnData::I16(match val {
-                        Some(v) => Some(*v as i16),
+                        Some(v) => Some(v as i16),
                         None => None,
                     }));
                     rowindex += 1;
                 }
             }
-            arrow2::datatypes::DataType::Int16 => {
-                let ba = col.as_any().downcast_ref::<PrimitiveArray<i16>>().unwrap();
+            arrow::datatypes::DataType::Int16 => {
+                let ba = col.as_any().downcast_ref::<Int16Array>().unwrap();
 
                 let mut rowindex = 0;
                 for val in ba.iter() {
-                    token_rows[rowindex].push(ColumnData::I16(val.copied()));
+                    token_rows[rowindex].push(ColumnData::I16(val));
                     rowindex += 1;
                 }
             }
-            arrow2::datatypes::DataType::Int64 => {
-                let ba = col.as_any().downcast_ref::<PrimitiveArray<i64>>().unwrap();
+            arrow::datatypes::DataType::Int64 => {
+                let ba = col.as_any().downcast_ref::<Int64Array>().unwrap();
 
                 let mut rowindex = 0;
                 for val in ba.iter() {
-                    token_rows[rowindex].push(ColumnData::I64(val.copied()));
+                    token_rows[rowindex].push(ColumnData::I64(val));
                     rowindex += 1;
                 }
             }
-            arrow2::datatypes::DataType::UInt16 => {
-                let ba = col.as_any().downcast_ref::<PrimitiveArray<u16>>().unwrap();
+            arrow::datatypes::DataType::UInt16 => {
+                let ba = col.as_any().downcast_ref::<UInt16Array>().unwrap();
 
                 let mut rowindex = 0;
                 for val in ba.iter() {
                     token_rows[rowindex].push(ColumnData::I32(match val {
                         Some(x) => Some(x.clone().into()),
                         None => None,
                     }));
                     rowindex += 1;
                 }
             }
-            arrow2::datatypes::DataType::UInt32 => {
-                let ba = col.as_any().downcast_ref::<PrimitiveArray<u32>>().unwrap();
+            arrow::datatypes::DataType::UInt32 => {
+                let ba = col.as_any().downcast_ref::<UInt32Array>().unwrap();
 
                 let mut rowindex = 0;
                 for val in ba.iter() {
                     token_rows[rowindex].push(ColumnData::I64(match val {
                         Some(x) => Some(x.clone().into()),
                         None => None,
                     }));
                     rowindex += 1;
                 }
             }
-            arrow2::datatypes::DataType::UInt64 => {
-                let ba = col.as_any().downcast_ref::<PrimitiveArray<u64>>().unwrap();
+            arrow::datatypes::DataType::UInt64 => {
+                let ba = col.as_any().downcast_ref::<UInt64Array>().unwrap();
 
                 let mut rowindex = 0;
                 for val in ba.iter() {
                     token_rows[rowindex].push(ColumnData::I64(match val {
                         Some(x) => Some(x.clone() as i64),
                         None => None,
                     }));
                     rowindex += 1;
                 }
             }
-            arrow2::datatypes::DataType::Float16 => {
+            arrow::datatypes::DataType::Float16 => {
                 let ba = col.as_any().downcast_ref::<Float16Array>().unwrap();
 
                 let mut rowindex = 0;
                 for val in ba.iter() {
                     token_rows[rowindex].push(ColumnData::F32(match val {
                         Some(x) => Some(x.to_f32()),
                         None => None,
                     }));
                     rowindex += 1;
                 }
             }
-            arrow2::datatypes::DataType::Float32 => {
-                let ba = col.as_any().downcast_ref::<PrimitiveArray<f32>>().unwrap();
+            arrow::datatypes::DataType::Float32 => {
+                let ba = col.as_any().downcast_ref::<Float32Array>().unwrap();
 
                 let mut rowindex = 0;
                 for val in ba.iter() {
-                    token_rows[rowindex].push(ColumnData::F32(val.copied()));
+                    token_rows[rowindex].push(ColumnData::F32(val));
                     rowindex += 1;
                 }
             }
-            arrow2::datatypes::DataType::Float64 => {
-                let ba = col.as_any().downcast_ref::<PrimitiveArray<f64>>().unwrap();
+            arrow::datatypes::DataType::Float64 => {
+                let ba = col.as_any().downcast_ref::<Float64Array>().unwrap();
 
                 let mut rowindex = 0;
                 for val in ba.iter() {
-                    token_rows[rowindex].push(ColumnData::F64(val.copied()));
+                    token_rows[rowindex].push(ColumnData::F64(val));
                     rowindex += 1;
                 }
             }
-            arrow2::datatypes::DataType::Date32 => {
-                let ba = col.as_any().downcast_ref::<PrimitiveArray<i32>>().unwrap();
+            arrow::datatypes::DataType::Date32 => {
+                let ba = col.as_any().downcast_ref::<Date32Array>().unwrap();
 
                 let mut rowindex = 0;
                 for val in ba.iter() {
                     let dt_val = match val {
-                        Some(vs) => Some(unix_min_date + Duration::days(*vs as i64)),
+                        Some(vs) => Some(unix_min_date + Duration::days(vs as i64)),
                         None => None,
                     };
                     token_rows[rowindex].push(to_date(dt_val));
                     rowindex += 1;
                 }
             }
-            arrow2::datatypes::DataType::Date64 => {
-                let ba = col.as_any().downcast_ref::<PrimitiveArray<i64>>().unwrap();
+            arrow::datatypes::DataType::Date64 => {
+                let ba = col.as_any().downcast_ref::<Date64Array>().unwrap();
 
                 let mut rowindex = 0;
                 for val in ba.iter() {
                     let dt_val = match val {
-                        Some(vs) => Some(unix_min_date + Duration::days(*vs)),
+                        Some(vs) => Some(unix_min_date + Duration::days(vs)),
                         None => None,
                     };
                     token_rows[rowindex].push(to_date(dt_val));
                     rowindex += 1;
                 }
             }
-            arrow2::datatypes::DataType::Time32(unit) => {
-                let ba = col.as_any().downcast_ref::<PrimitiveArray<i32>>().unwrap();
+            arrow::datatypes::DataType::Time32(arrow::datatypes::TimeUnit::Second) => {
+                let ba = col.as_any().downcast_ref::<Time32SecondArray>().unwrap();
 
                 let mut rowindex = 0;
                 for val in ba.iter() {
                     let dt_val: Option<Time> = match val {
-                        Some(vs) => match unit {
-                            arrow2::datatypes::TimeUnit::Second => Some(
+                        Some(vs) =>  Some(
                                 Time::from_hms(
                                     // TODO: Testing
                                     (vs / 60 / 60).try_into().unwrap(),
                                     ((vs / 60) % 60).try_into().unwrap(),
                                     (vs % 60).try_into().unwrap(),
                                 )
                                 .unwrap(),
                             ),
-                            arrow2::datatypes::TimeUnit::Millisecond => Some(
-                                // TODO: Testing
-                                Time::from_hms_milli(
+                        None => None,
+                    };
+                    token_rows[rowindex].push(to_time(dt_val));
+                    rowindex += 1;
+                }
+            },
+            arrow::datatypes::DataType::Time32(arrow::datatypes::TimeUnit::Millisecond) => {
+                let ba = col.as_any().downcast_ref::<Time32SecondArray>().unwrap();
+
+                let mut rowindex = 0;
+                for val in ba.iter() {
+                    let dt_val: Option<Time> = match val {
+                        Some(vs) => Some(Time::from_hms_milli(
                                     (vs / 1000 / 60 / 60).try_into().unwrap(),
                                     ((vs / 1000 / 60) % 60).try_into().unwrap(),
                                     ((vs / 1000) % 60).try_into().unwrap(),
                                     (vs % 1000).try_into().unwrap(),
                                 )
-                                .unwrap(),
-                            ),
-                            _ => panic!("Not supported"),
-                        },
+                                .unwrap())                        ,
 
                         None => None,
                     };
                     token_rows[rowindex].push(to_time(dt_val));
                     rowindex += 1;
                 }
             }
-            arrow2::datatypes::DataType::Time64(_) => todo!(),
-            arrow2::datatypes::DataType::Duration(_) => todo!(),
-            arrow2::datatypes::DataType::Interval(_) => todo!(),
-            arrow2::datatypes::DataType::Binary => todo!(),
-            arrow2::datatypes::DataType::FixedSizeBinary(_) => todo!(),
-            arrow2::datatypes::DataType::LargeBinary => todo!(),
-            arrow2::datatypes::DataType::List(_) => todo!(),
-            arrow2::datatypes::DataType::FixedSizeList(_, _) => todo!(),
-            arrow2::datatypes::DataType::LargeList(_) => todo!(),
-            arrow2::datatypes::DataType::Struct(_) => todo!(),
-            arrow2::datatypes::DataType::Union(_, _, _) => todo!(),
-            arrow2::datatypes::DataType::Map(_, _) => todo!(),
-            arrow2::datatypes::DataType::Dictionary(_, _, _) => todo!(),
-            arrow2::datatypes::DataType::Decimal(_, _) => todo!(),
-            arrow2::datatypes::DataType::Decimal256(_, _) => todo!(),
-            arrow2::datatypes::DataType::Extension(_, _, _) => todo!(),
+            
             _ => todo!(), //other => panic!("Not supported {:?}", other),
         }
     }
     token_rows
 }
```

### Comparing `lakeapi2sql-0.1.0/src/bulk_insert.rs` & `lakeapi2sql-0.2.0/src/bulk_insert.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,77 +1,83 @@
-use std::{thread, time::Duration};
+use std::sync::Arc;
 
-use arrow2::{
-    array::Array,
-    chunk::Chunk,
-    io::ipc::read::{self, read_stream_metadata, StreamReader},
+use arrow::{
+    ipc::reader::{StreamReader}, datatypes::Schema, record_batch::RecordBatch,
 };
 use futures::stream::TryStreamExt;
 use tiberius::Client;
 use tokio::net::TcpStream;
 use tokio_util::compat::Compat;
 use tokio_util::compat::FuturesAsyncReadCompatExt;
 use tokio_util::io::SyncIoBridge;
+use log::info;
 
 use tokio::sync::mpsc;
 
 use crate::arrow_convert::get_token_rows;
 
 pub async fn bulk_insert<'a>(
     db_client: &'a mut Client<Compat<TcpStream>>,
     table_name: &str,
     url: &str,
     user: &str,
     password: &str,
-) -> Result<(), Box<dyn std::error::Error + Send + Sync>> {
+) -> Result<Arc<Schema>, Box<dyn std::error::Error + Send + Sync>> {
     //let mut row = TokenRow::new();
     //row.push(1.into_sql());
     //blk.send(row).await?;
     //blk.finalize().await?;
     let cclient = reqwest::Client::new();
 
     // a bit too complex if you ask me: https://github.com/benkay86/async-applied/tree/master/reqwest-tokio-compat
 
     let res = cclient
         .get(url)
         .basic_auth(user, Some(password))
         .send()
         .await?
         .error_for_status()?;
-
+    
+    info!("received http response");
     let res = res
         .bytes_stream()
         .map_err(|e| futures::io::Error::new(futures::io::ErrorKind::Other, e))
         .into_async_read()
         .compat();
-    let (tx, mut rx) = mpsc::channel::<Chunk<Box<dyn Array>>>(2);
-    let mut syncstr = SyncIoBridge::new(res);
-    let worker = tokio::task::spawn_blocking(move || {
-        let metadata = read_stream_metadata(&mut syncstr).unwrap();
-        let mut reader = StreamReader::new(syncstr, metadata, None);
+    let (tx, mut rx) = mpsc::channel::<RecordBatch>(2);
+    let syncstr = SyncIoBridge::new(res);
+    let worker = tokio::task::spawn_blocking(move || {       
+        
+        let mut reader = StreamReader::try_new(syncstr, None).unwrap();
+        let schema = reader.schema();
         loop {
             match reader.next() {
                 Some(x) => match x {
-                    Ok(read::StreamState::Some(b)) => {
+                    Ok(b) => {
                         tx.blocking_send(b).unwrap();
                     }
-                    Ok(read::StreamState::Waiting) => thread::sleep(Duration::from_millis(2000)),
                     Err(l) => println!("{:?}", l),
                 },
                 None => break,
             };
         }
+        Ok(schema)
     });
 
     while let Some(v) = rx.recv().await {
-        let rows = get_token_rows(&v);
+        let nrows = v.num_rows();
+        info!("received {nrows}");
+        let rows = get_token_rows(&v);        
         let mut blk: tiberius::BulkLoadRequest<'_, Compat<TcpStream>> =
             db_client.bulk_insert(table_name).await?;
         for row in rows {
             blk.send(row).await?;
         }
         blk.finalize().await?;
+        info!("Written {nrows}");
     }
-    worker.await.unwrap();
-
-    Ok(())
+    let schema = worker.await?;
+    if let Err(e) = schema {
+        return e;
+    }
+    Ok(schema.unwrap())
 }
```

### Comparing `lakeapi2sql-0.1.0/src/connect.rs` & `lakeapi2sql-0.2.0/src/connect.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+use tiberius::SqlBrowser;
 use tiberius::error::Error;
 use tiberius::AuthMethod;
 use tiberius::Client;
 use tiberius::Config;
 use tokio::net::TcpStream;
 use tokio_util::compat::Compat;
 use tokio_util::compat::TokioAsyncWriteCompatExt;
@@ -12,15 +13,16 @@
 ) -> Result<Client<Compat<TcpStream>>, Box<dyn std::error::Error + Send + Sync>> {
     let mut config = Config::from_ado_string(con_str)?;
     if let Some(tv) = aad_token.clone() {
         config.authentication(AuthMethod::AADToken(tv));
     }
 
     config.encryption(tiberius::EncryptionLevel::Required);
-    let tcp = TcpStream::connect(config.get_addr()).await?;
+    
+    let tcp = TcpStream::connect_named(&config).await?;
     tcp.set_nodelay(true)?;
 
     let client = match Client::connect(config, tcp.compat_write()).await {
         // Connection successful.
         Ok(client) => client,
         // The server wants us to redirect to a different address
         Err(Error::Routing { host, port }) => {
```

### Comparing `lakeapi2sql-0.1.0/Cargo.lock` & `lakeapi2sql-0.2.0/Cargo.lock`

 * *Files 9% similar despite different names*

```diff
@@ -5,60 +5,259 @@
 [[package]]
 name = "ahash"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2c99f64d1e06488f620f932677e24bc6e2897582980441ae90a671415bd7ec2f"
 dependencies = [
  "cfg-if",
+ "const-random",
  "getrandom 0.2.10",
  "once_cell",
  "version_check",
 ]
 
 [[package]]
+name = "aho-corasick"
+version = "1.0.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "43f6cb1bf222025340178f382c426f13757b2960e89779dfcb319c32542a5a41"
+dependencies = [
+ "memchr",
+]
+
+[[package]]
 name = "android-tzdata"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e999941b234f3131b00bc13c22d06e8c5ff726d1b6318ac7eb276997bbb4fef0"
 
 [[package]]
-name = "array-init-cursor"
-version = "0.2.0"
+name = "android_system_properties"
+version = "0.1.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
+dependencies = [
+ "libc",
+]
+
+[[package]]
+name = "arc-swap"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf7d0a018de4f6aa429b9d33d69edf69072b1c5b1cb8d3e4a5f7ef898fc3eb76"
+checksum = "bddcadddf5e9015d310179a59bb28c4d4b9920ad0f11e8e14dbadf654890c9a6"
 
 [[package]]
-name = "arrow-format"
-version = "0.8.1"
+name = "arrow"
+version = "42.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "07884ea216994cdc32a2d5f8274a8bee979cfe90274b83f86f440866ee3132c7"
+checksum = "773d18d72cd290f3f9e2149a714c8ac404b6c3fd614c684f0015449940fca899"
 dependencies = [
- "planus",
- "serde",
+ "ahash",
+ "arrow-arith",
+ "arrow-array",
+ "arrow-buffer",
+ "arrow-cast",
+ "arrow-csv",
+ "arrow-data",
+ "arrow-ipc",
+ "arrow-json",
+ "arrow-ord",
+ "arrow-row",
+ "arrow-schema",
+ "arrow-select",
+ "arrow-string",
+]
+
+[[package]]
+name = "arrow-arith"
+version = "42.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "93bc0da4b22ba63807fa2a74998e21209179c93c67856ae65d9218b81f3ef918"
+dependencies = [
+ "arrow-array",
+ "arrow-buffer",
+ "arrow-data",
+ "arrow-schema",
+ "chrono",
+ "half",
+ "num",
 ]
 
 [[package]]
-name = "arrow2"
-version = "0.17.2"
+name = "arrow-array"
+version = "42.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "15ae0428d69ab31d7b2adad22a752d6f11fef2e901d2262d0cad4f5cb08b7093"
+checksum = "ea9a0fd21121304cad96f307c938d861cb1e7f0c151b93047462cd9817d760fb"
 dependencies = [
  "ahash",
- "arrow-format",
- "bytemuck",
+ "arrow-buffer",
+ "arrow-data",
+ "arrow-schema",
  "chrono",
- "dyn-clone",
- "either",
- "ethnum",
- "foreign_vec",
- "getrandom 0.2.10",
- "hash_hasher",
- "num-traits",
- "rustc_version",
- "simdutf8",
+ "half",
+ "hashbrown 0.14.0",
+ "num",
+]
+
+[[package]]
+name = "arrow-buffer"
+version = "42.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "30ce342ecf5971004e23cef8b5fb3bacd2bbc48a381464144925074e1472e9eb"
+dependencies = [
+ "half",
+ "num",
+]
+
+[[package]]
+name = "arrow-cast"
+version = "42.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4b94a0ce7d27abbb02e2ee4db770f593127610f57b32625b0bc6a1a90d65f085"
+dependencies = [
+ "arrow-array",
+ "arrow-buffer",
+ "arrow-data",
+ "arrow-schema",
+ "arrow-select",
+ "chrono",
+ "half",
+ "lexical-core",
+ "num",
+]
+
+[[package]]
+name = "arrow-csv"
+version = "42.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0f3be10a00a43c4bf0d243c070754ebdde17c5d576b4928d9c3efbe3005a3853"
+dependencies = [
+ "arrow-array",
+ "arrow-buffer",
+ "arrow-cast",
+ "arrow-data",
+ "arrow-schema",
+ "chrono",
+ "csv",
+ "csv-core",
+ "lazy_static",
+ "lexical-core",
+ "regex",
+]
+
+[[package]]
+name = "arrow-data"
+version = "42.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1d9a83dad6a53d6907765106d3bc61d6d9d313cfe1751701b3ef0948e7283dc2"
+dependencies = [
+ "arrow-buffer",
+ "arrow-schema",
+ "half",
+ "num",
+]
+
+[[package]]
+name = "arrow-ipc"
+version = "42.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a46da5e438a854e0386b38774da88a98782c0973c6dbc5c949ca4e02faf9b016"
+dependencies = [
+ "arrow-array",
+ "arrow-buffer",
+ "arrow-cast",
+ "arrow-data",
+ "arrow-schema",
+ "flatbuffers",
+ "lz4",
+ "zstd",
+]
+
+[[package]]
+name = "arrow-json"
+version = "42.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d5f27a1fbc76553ad92dc1a9583e56b7058d8c418c4089b0b689f5b87e2da5e1"
+dependencies = [
+ "arrow-array",
+ "arrow-buffer",
+ "arrow-cast",
+ "arrow-data",
+ "arrow-schema",
+ "chrono",
+ "half",
+ "indexmap",
+ "lexical-core",
+ "num",
+ "serde",
+ "serde_json",
+]
+
+[[package]]
+name = "arrow-ord"
+version = "42.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f2373661f6c2233e18f6fa69c40999a9440231d1e8899be8bbbe73c7e24aa3b4"
+dependencies = [
+ "arrow-array",
+ "arrow-buffer",
+ "arrow-data",
+ "arrow-schema",
+ "arrow-select",
+ "half",
+ "num",
+]
+
+[[package]]
+name = "arrow-row"
+version = "42.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "377cd5158b7de4034a175e296726c40c3236e65d71d90a5dab2fb4fab526a8f4"
+dependencies = [
+ "ahash",
+ "arrow-array",
+ "arrow-buffer",
+ "arrow-data",
+ "arrow-schema",
+ "half",
+ "hashbrown 0.14.0",
+]
+
+[[package]]
+name = "arrow-schema"
+version = "42.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ba9ed245bd2d7d97ad1457cb281d4296e8b593588758b8fec6d67b2b2b0f2265"
+
+[[package]]
+name = "arrow-select"
+version = "42.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0dc9bd6aebc565b1d04bae64a0f4dda3abc677190eb7d960471b1b20e1cebed0"
+dependencies = [
+ "arrow-array",
+ "arrow-buffer",
+ "arrow-data",
+ "arrow-schema",
+ "num",
+]
+
+[[package]]
+name = "arrow-string"
+version = "42.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "23cf2baea2ef53787332050decf7d71aca836a352e188c8ad062892405955d2b"
+dependencies = [
+ "arrow-array",
+ "arrow-buffer",
+ "arrow-data",
+ "arrow-schema",
+ "arrow-select",
+ "regex",
+ "regex-syntax",
 ]
 
 [[package]]
 name = "async-native-tls"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d57d4cec3c647232e1094dc013546c0b33ce785d8aeb251e1f20dfaf8a9a13fe"
@@ -114,34 +313,14 @@
 [[package]]
 name = "bumpalo"
 version = "3.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a3e2c3daef883ecc1b5d58c15adae93470a91d425f3532ba1695849656af3fc1"
 
 [[package]]
-name = "bytemuck"
-version = "1.13.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "17febce684fd15d89027105661fec94afb475cb995fbc59d2865198446ba2eea"
-dependencies = [
- "bytemuck_derive",
-]
-
-[[package]]
-name = "bytemuck_derive"
-version = "1.4.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fdde5c9cd29ebd706ce1b35600920a33550e402fc998a2e53ad3b42c3c47a192"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn 2.0.18",
-]
-
-[[package]]
 name = "byteorder"
 version = "1.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "14c189c53d098945499cdfa7ecc63567cf3886b3332b312a5b4585d8d3a6a610"
 
 [[package]]
 name = "bytes"
@@ -150,38 +329,65 @@
 checksum = "89b2fd2a0dcf38d7971e2194b6b6eebab45ae01067456a7fd93d5547a61b70be"
 
 [[package]]
 name = "cc"
 version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
+dependencies = [
+ "jobserver",
+]
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
 version = "0.4.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ec837a71355b28f6556dbd569b37b3f363091c0bd4b2e735674521b4c5fd9bc5"
 dependencies = [
  "android-tzdata",
+ "iana-time-zone",
  "num-traits",
+ "winapi",
 ]
 
 [[package]]
 name = "connection-string"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "510ca239cf13b7f8d16a2b48f263de7b4f8c566f0af58d901031473c76afb1e3"
 
 [[package]]
+name = "const-random"
+version = "0.1.15"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "368a7a772ead6ce7e1de82bfb04c485f3db8ec744f72925af5735e29a22cc18e"
+dependencies = [
+ "const-random-macro",
+ "proc-macro-hack",
+]
+
+[[package]]
+name = "const-random-macro"
+version = "0.1.15"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9d7d6ab3c3a2282db210df5f02c4dab6e0a7057af0fb7ebd4070f30fe05c0ddb"
+dependencies = [
+ "getrandom 0.2.10",
+ "once_cell",
+ "proc-macro-hack",
+ "tiny-keccak",
+]
+
+[[package]]
 name = "core-foundation"
 version = "0.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "194a7a9e6de53fa55116934067c844d9d749312f75c6f6d0980e8c252f8c2146"
 dependencies = [
  "core-foundation-sys",
  "libc",
@@ -190,24 +396,39 @@
 [[package]]
 name = "core-foundation-sys"
 version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
 
 [[package]]
-name = "dyn-clone"
-version = "1.0.11"
+name = "crunchy"
+version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "68b0cf012f1230e43cd00ebb729c6bb58707ecfa8ad08b52ef3a4ccd2697fc30"
+checksum = "7a81dae078cea95a014a339291cec439d2f232ebe854a9d672b796c6afafa9b7"
 
 [[package]]
-name = "either"
-version = "1.8.1"
+name = "csv"
+version = "1.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
+checksum = "626ae34994d3d8d668f4269922248239db4ae42d538b14c398b74a52208e8086"
+dependencies = [
+ "csv-core",
+ "itoa",
+ "ryu",
+ "serde",
+]
+
+[[package]]
+name = "csv-core"
+version = "0.1.10"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2b2466559f260f48ad25fe6317b3c8dac77b5bdb5763ac7d9d6103530663bc90"
+dependencies = [
+ "memchr",
+]
 
 [[package]]
 name = "encoding"
 version = "0.2.33"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6b0d943856b990d12d3b55b359144ff341533e516d94098b1d3fc1ac666d36ec"
 dependencies = [
@@ -316,29 +537,33 @@
 checksum = "aa68f1b12764fab894d2755d2518754e71b4fd80ecfb822714a1206c2aab39bf"
 dependencies = [
  "cc",
  "libc",
 ]
 
 [[package]]
-name = "ethnum"
-version = "1.3.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0198b9d0078e0f30dedc7acbb21c974e838fc8fae3ee170128658a98cb2c1c04"
-
-[[package]]
 name = "fastrand"
 version = "1.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e51093e27b0797c359783294ca4f0a911c270184cb10f85783b118614a1501be"
 dependencies = [
  "instant",
 ]
 
 [[package]]
+name = "flatbuffers"
+version = "23.5.26"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4dac53e22462d78c16d64a1cd22371b54cc3fe94aa15e7886a2fa6e5d1ab8640"
+dependencies = [
+ "bitflags",
+ "rustc_version",
+]
+
+[[package]]
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
 
 [[package]]
 name = "foreign-types"
@@ -352,20 +577,14 @@
 [[package]]
 name = "foreign-types-shared"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "00b0228411908ca8685dba7fc2cdd70ec9990a6e753e89b6ac91a84c40fbaf4b"
 
 [[package]]
-name = "foreign_vec"
-version = "0.1.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ee1b05cbd864bcaecbd3455d6d967862d446e4ebfc3c2e5e5b9841e53cba6673"
-
-[[package]]
 name = "form_urlencoded"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a62bc1cf6f830c2ec14a513a9fb124d0a213a629668a4186f329db21fe045652"
 dependencies = [
  "percent-encoding",
 ]
@@ -473,18 +692,16 @@
 [[package]]
 name = "getrandom"
 version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "be4136b2a15dd319360be1c07d9933517ccf0be8f16bf62a3bee4f0d618df427"
 dependencies = [
  "cfg-if",
- "js-sys",
  "libc",
  "wasi 0.11.0+wasi-snapshot-preview1",
- "wasm-bindgen",
 ]
 
 [[package]]
 name = "h2"
 version = "0.3.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d357c7ae988e7d2182f7d7871d0b963962420b0678b0997ce7de72001aeab782"
@@ -499,26 +716,37 @@
  "slab",
  "tokio",
  "tokio-util",
  "tracing",
 ]
 
 [[package]]
-name = "hash_hasher"
-version = "2.0.3"
+name = "half"
+version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "74721d007512d0cb3338cd20f0654ac913920061a4c4d0d8708edb3f2a698c0c"
+checksum = "bc52e53916c08643f1b56ec082790d1e86a32e58dc5268f897f313fbae7b4872"
+dependencies = [
+ "cfg-if",
+ "crunchy",
+ "num-traits",
+]
 
 [[package]]
 name = "hashbrown"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
 
 [[package]]
+name = "hashbrown"
+version = "0.14.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2c6201b9ff9fd90a5a3bac2e56a830d0caa509576f0e503818ee82c181b3437a"
+
+[[package]]
 name = "hermit-abi"
 version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ee512640fe35acbfb4bb779db6f0d80704c2cacfa2e39b601ef3e3f47d1ae4c7"
 dependencies = [
  "libc",
 ]
@@ -597,14 +825,37 @@
  "hyper",
  "native-tls",
  "tokio",
  "tokio-native-tls",
 ]
 
 [[package]]
+name = "iana-time-zone"
+version = "0.1.57"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2fad5b825842d2b38bd206f3e81d6957625fd7f0a361e345c30e01a0ae2dd613"
+dependencies = [
+ "android_system_properties",
+ "core-foundation-sys",
+ "iana-time-zone-haiku",
+ "js-sys",
+ "wasm-bindgen",
+ "windows",
+]
+
+[[package]]
+name = "iana-time-zone-haiku"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f31827a206f56af32e590ba56d5d2d085f558508192593743f16b2306495269f"
+dependencies = [
+ "cc",
+]
+
+[[package]]
 name = "idna"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7d20d6b07bfbc108882d88ed8e37d39636dcc260e15e30c45e6ba089610b917c"
 dependencies = [
  "unicode-bidi",
  "unicode-normalization",
@@ -613,15 +864,15 @@
 [[package]]
 name = "indexmap"
 version = "1.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
 dependencies = [
  "autocfg",
- "hashbrown",
+ "hashbrown 0.12.3",
 ]
 
 [[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
@@ -655,51 +906,132 @@
 [[package]]
 name = "itoa"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
 
 [[package]]
+name = "jobserver"
+version = "0.1.26"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "936cfd212a0155903bcbc060e316fb6cc7cbf2e1907329391ebadc1fe0ce77c2"
+dependencies = [
+ "libc",
+]
+
+[[package]]
 name = "js-sys"
 version = "0.3.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c5f195fe497f702db0f318b07fdd68edb16955aed830df8363d837542f8f935a"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "lake2sql"
 version = "0.1.0"
 dependencies = [
- "arrow2",
+ "arrow",
  "futures",
+ "log",
  "openssl",
  "pyo3",
  "pyo3-asyncio",
+ "pyo3-log",
  "reqwest",
  "tiberius",
  "time",
  "tokio",
  "tokio-util",
 ]
 
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
+name = "lexical-core"
+version = "0.8.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2cde5de06e8d4c2faabc400238f9ae1c74d5412d03a7bd067645ccbc47070e46"
+dependencies = [
+ "lexical-parse-float",
+ "lexical-parse-integer",
+ "lexical-util",
+ "lexical-write-float",
+ "lexical-write-integer",
+]
+
+[[package]]
+name = "lexical-parse-float"
+version = "0.8.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "683b3a5ebd0130b8fb52ba0bdc718cc56815b6a097e28ae5a6997d0ad17dc05f"
+dependencies = [
+ "lexical-parse-integer",
+ "lexical-util",
+ "static_assertions",
+]
+
+[[package]]
+name = "lexical-parse-integer"
+version = "0.8.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6d0994485ed0c312f6d965766754ea177d07f9c00c9b82a5ee62ed5b47945ee9"
+dependencies = [
+ "lexical-util",
+ "static_assertions",
+]
+
+[[package]]
+name = "lexical-util"
+version = "0.8.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5255b9ff16ff898710eb9eb63cb39248ea8a5bb036bea8085b1a767ff6c4e3fc"
+dependencies = [
+ "static_assertions",
+]
+
+[[package]]
+name = "lexical-write-float"
+version = "0.8.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "accabaa1c4581f05a3923d1b4cfd124c329352288b7b9da09e766b0668116862"
+dependencies = [
+ "lexical-util",
+ "lexical-write-integer",
+ "static_assertions",
+]
+
+[[package]]
+name = "lexical-write-integer"
+version = "0.8.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e1b6f3d1f4422866b68192d62f77bc5c700bee84f3069f2469d7bc8c77852446"
+dependencies = [
+ "lexical-util",
+ "static_assertions",
+]
+
+[[package]]
 name = "libc"
 version = "0.2.146"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f92be4933c13fd498862a9e02a3055f8a8d9c039ce33db97306fd5a6caa7f29b"
 
 [[package]]
+name = "libm"
+version = "0.2.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f7012b1bbb0719e1097c47611d3898568c546d597c2e74d66f6087edd5233ff4"
+
+[[package]]
 name = "linux-raw-sys"
 version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ef53942eb7bf7ff43a617b3e2c1c4a5ecf5944a7c1bc12d7ee39bbb15e5c1519"
 
 [[package]]
 name = "lock_api"
@@ -714,14 +1046,34 @@
 [[package]]
 name = "log"
 version = "0.4.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b06a4cde4c0f271a446782e3eff8de789548ce57dbc8eca9292c27f4a42004b4"
 
 [[package]]
+name = "lz4"
+version = "1.24.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7e9e2dd86df36ce760a60f6ff6ad526f7ba1f14ba0356f8254fb6905e6494df1"
+dependencies = [
+ "libc",
+ "lz4-sys",
+]
+
+[[package]]
+name = "lz4-sys"
+version = "1.9.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "57d27b317e207b10f69f5e75494119e391a96f48861ae870d1da6edac98ca900"
+dependencies = [
+ "cc",
+ "libc",
+]
+
+[[package]]
 name = "md5"
 version = "0.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7e6bcd6433cff03a4bfc3d9834d504467db1f1cf6d0ea765d37d330249ed629d"
 
 [[package]]
 name = "memchr"
@@ -770,20 +1122,88 @@
  "schannel",
  "security-framework",
  "security-framework-sys",
  "tempfile",
 ]
 
 [[package]]
+name = "num"
+version = "0.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "43db66d1170d347f9a065114077f7dccb00c1b9478c89384490a3425279a4606"
+dependencies = [
+ "num-bigint",
+ "num-complex",
+ "num-integer",
+ "num-iter",
+ "num-rational",
+ "num-traits",
+]
+
+[[package]]
+name = "num-bigint"
+version = "0.4.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f93ab6289c7b344a8a9f60f88d80aa20032336fe78da341afc91c8a2341fc75f"
+dependencies = [
+ "autocfg",
+ "num-integer",
+ "num-traits",
+]
+
+[[package]]
+name = "num-complex"
+version = "0.4.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "02e0d21255c828d6f128a1e41534206671e8c3ea0c62f32291e808dc82cff17d"
+dependencies = [
+ "num-traits",
+]
+
+[[package]]
+name = "num-integer"
+version = "0.1.45"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
+dependencies = [
+ "autocfg",
+ "num-traits",
+]
+
+[[package]]
+name = "num-iter"
+version = "0.1.43"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7d03e6c028c5dc5cac6e2dec0efda81fc887605bb3d884578bb6d6bf7514e252"
+dependencies = [
+ "autocfg",
+ "num-integer",
+ "num-traits",
+]
+
+[[package]]
+name = "num-rational"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0638a1c9d0a3c0914158145bc76cff373a75a627e6ecbfb71cbe6f453a5a19b0"
+dependencies = [
+ "autocfg",
+ "num-bigint",
+ "num-integer",
+ "num-traits",
+]
+
+[[package]]
 name = "num-traits"
 version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
 dependencies = [
  "autocfg",
+ "libm",
 ]
 
 [[package]]
 name = "num_cpus"
 version = "1.15.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0fac9e2da13b5eb447a6ce3d392f23a29d8694bff781bf03a16cd9ac8697593b"
@@ -896,35 +1316,32 @@
 [[package]]
 name = "pkg-config"
 version = "0.3.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "26072860ba924cbfa98ea39c8c19b4dd6a4a25423dbdf219c1eca91aa0cf6964"
 
 [[package]]
-name = "planus"
-version = "0.3.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fc1691dd09e82f428ce8d6310bd6d5da2557c82ff17694d2a32cad7242aea89f"
-dependencies = [
- "array-init-cursor",
-]
-
-[[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "pretty-hex"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c6fa0831dd7cc608c38a5e323422a0077678fa5744aa2be4ad91c4ece8eec8d5"
 
 [[package]]
+name = "proc-macro-hack"
+version = "0.5.20+deprecated"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "dc375e1527247fe1a97d8b7156678dfe7c1af2fc075c9a4db3690ecd2a148068"
+
+[[package]]
 name = "proc-macro2"
 version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dec2b086b7a862cf4de201096214fa870344cf922b2b30c167badb3af3195406"
 dependencies = [
  "unicode-ident",
 ]
@@ -988,14 +1405,25 @@
 checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
+name = "pyo3-log"
+version = "0.8.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c94ff6535a6bae58d7d0b85e60d4c53f7f84d0d0aa35d6a28c3f3e70bfe51444"
+dependencies = [
+ "arc-swap",
+ "log",
+ "pyo3",
+]
+
+[[package]]
 name = "pyo3-macros"
 version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
@@ -1070,14 +1498,31 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
+name = "regex"
+version = "1.8.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d0ab3ca65655bb1e41f2a8c8cd662eb4fb035e67c3f78da1d61dffe89d07300f"
+dependencies = [
+ "aho-corasick",
+ "memchr",
+ "regex-syntax",
+]
+
+[[package]]
+name = "regex-syntax"
+version = "0.7.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
+
+[[package]]
 name = "reqwest"
 version = "0.11.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cde824a14b7c14f85caff81225f411faacc04a2013f41670f41443742b1c1c55"
 dependencies = [
  "base64",
  "bytes",
@@ -1186,28 +1631,14 @@
 checksum = "bebd363326d05ec3e2f532ab7660680f3b02130d780c299bca73469d521bc0ed"
 
 [[package]]
 name = "serde"
 version = "1.0.164"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9e8c8cf938e98f769bc164923b06dce91cea1751522f46f8466461af04c9027d"
-dependencies = [
- "serde_derive",
-]
-
-[[package]]
-name = "serde_derive"
-version = "1.0.164"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d9735b638ccc51c28bf6914d90a2e9725b377144fc612c49a611fddd1b631d68"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn 2.0.18",
-]
 
 [[package]]
 name = "serde_json"
 version = "1.0.97"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bdf3bf93142acad5821c99197022e170842cdbc1c30482b98750c688c640842a"
 dependencies = [
@@ -1225,20 +1656,14 @@
  "form_urlencoded",
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
-name = "simdutf8"
-version = "0.1.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f27f6278552951f1f2b8cf9da965d10969b2efdea95a6ec47987ab46edfe263a"
-
-[[package]]
 name = "slab"
 version = "0.4.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6528351c9bc8ab22353f9d776db39a20288e8d6c37ef8cfe3317cf875eecfc2d"
 dependencies = [
  "autocfg",
 ]
@@ -1256,14 +1681,20 @@
 checksum = "64a4a911eed85daf18834cfaa86a79b7d266ff93ff5ba14005426219480ed662"
 dependencies = [
  "libc",
  "winapi",
 ]
 
 [[package]]
+name = "static_assertions"
+version = "1.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a2eb9349b6444b326872e140eb1cf5e7c522154d69e7a0ffb0fb81c06b37543f"
+
+[[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
  "proc-macro2",
  "quote",
@@ -1338,14 +1769,16 @@
  "futures-util",
  "num-traits",
  "once_cell",
  "pin-project-lite",
  "pretty-hex",
  "thiserror",
  "time",
+ "tokio",
+ "tokio-util",
  "tracing",
  "uuid",
  "winauth",
 ]
 
 [[package]]
 name = "time"
@@ -1360,14 +1793,23 @@
 [[package]]
 name = "time-core"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7300fbefb4dadc1af235a9cef3737cea692a9d97e1b9cbcd4ebdae6f8868e6fb"
 
 [[package]]
+name = "tiny-keccak"
+version = "2.0.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2c9d3793400a45f954c52e73d068316d76b6f4e36977e3fcebb13a2721e80237"
+dependencies = [
+ "crunchy",
+]
+
+[[package]]
 name = "tinyvec"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87cc5ceb3875bb20c2890005a4e226a4651264a5c75edb2421b52861a0a0cb50"
 dependencies = [
  "tinyvec_macros",
 ]
@@ -1674,14 +2116,23 @@
  "byteorder",
  "md5",
  "rand",
  "winapi",
 ]
 
 [[package]]
+name = "windows"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e686886bc078bc1b0b600cac0147aadb815089b6e4da64016cbd754b6342700f"
+dependencies = [
+ "windows-targets",
+]
+
+[[package]]
 name = "windows-sys"
 version = "0.42.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
 dependencies = [
  "windows_aarch64_gnullvm 0.42.2",
  "windows_aarch64_msvc 0.42.2",
@@ -1804,7 +2255,37 @@
 name = "winreg"
 version = "0.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "80d0f4e272c85def139476380b12f9ac60926689dd2e01d4923222f40580869d"
 dependencies = [
  "winapi",
 ]
+
+[[package]]
+name = "zstd"
+version = "0.12.3+zstd.1.5.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "76eea132fb024e0e13fd9c2f5d5d595d8a967aa72382ac2f9d39fcc95afd0806"
+dependencies = [
+ "zstd-safe",
+]
+
+[[package]]
+name = "zstd-safe"
+version = "6.0.5+zstd.1.5.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d56d9e60b4b1758206c238a10165fbcae3ca37b01744e394c463463f6529d23b"
+dependencies = [
+ "libc",
+ "zstd-sys",
+]
+
+[[package]]
+name = "zstd-sys"
+version = "2.0.8+zstd.1.5.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5556e6ee25d32df2586c098bbfa278803692a20d0ab9565e049480d52707ec8c"
+dependencies = [
+ "cc",
+ "libc",
+ "pkg-config",
+]
```

### Comparing `lakeapi2sql-0.1.0/PKG-INFO` & `lakeapi2sql-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lakeapi2sql
-Version: 0.1.0
+Version: 0.2.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

