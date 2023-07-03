# Comparing `tmp/spark_rapids_user_tools-23.6.0-149_22d8e21-py3-none-any.whl.zip` & `tmp/spark_rapids_user_tools-23.6.1-153_dcfbc66-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,82 +1,67 @@
-Zip file size: 271613 bytes, number of entries: 80
--rw-r--r--  2.0 unx      648 b- defN 23-Jun-28 20:30 spark_rapids_dataproc_tools/__init__.py
--rw-r--r--  2.0 unx    10120 b- defN 23-Jun-28 20:30 spark_rapids_dataproc_tools/cost_estimator.py
--rw-r--r--  2.0 unx    27693 b- defN 23-Jun-28 20:30 spark_rapids_dataproc_tools/dataproc_utils.py
--rw-r--r--  2.0 unx    15306 b- defN 23-Jun-28 20:30 spark_rapids_dataproc_tools/dataproc_wrapper.py
--rw-r--r--  2.0 unx    10514 b- defN 23-Jun-28 20:30 spark_rapids_dataproc_tools/diag.py
--rw-r--r--  2.0 unx     5344 b- defN 23-Jun-28 20:30 spark_rapids_dataproc_tools/diag_dataproc.py
--rw-r--r--  2.0 unx    63046 b- defN 23-Jun-28 20:30 spark_rapids_dataproc_tools/rapids_models.py
--rw-r--r--  2.0 unx     8782 b- defN 23-Jun-28 20:30 spark_rapids_dataproc_tools/utilities.py
--rw-r--r--  2.0 unx      921 b- defN 23-Jun-28 20:30 spark_rapids_dataproc_tools/csp/__init__.py
--rw-r--r--  2.0 unx     1671 b- defN 23-Jun-28 20:30 spark_rapids_dataproc_tools/csp/csp.py
--rw-r--r--  2.0 unx     5196 b- defN 23-Jun-28 20:30 spark_rapids_dataproc_tools/csp/dataproc.py
--rw-r--r--  2.0 unx     1154 b- defN 23-Jun-28 20:30 spark_rapids_dataproc_tools/diag_scripts/hello_world.py
--rw-r--r--  2.0 unx     1276 b- defN 23-Jun-28 20:30 spark_rapids_dataproc_tools/diag_scripts/perf.py
--rw-r--r--  2.0 unx     1273 b- defN 23-Jun-28 20:30 spark_rapids_dataproc_tools/resources/bootstrap-conf.yaml
--rw-r--r--  2.0 unx   684199 b- defN 23-Jun-28 20:30 spark_rapids_dataproc_tools/resources/gcloud-catalog.json
--rw-r--r--  2.0 unx     1416 b- defN 23-Jun-28 20:30 spark_rapids_dataproc_tools/resources/profiling-conf.yaml
--rw-r--r--  2.0 unx     2575 b- defN 23-Jun-28 20:30 spark_rapids_dataproc_tools/resources/qualification-conf.yaml
--rw-r--r--  2.0 unx      750 b- defN 23-Jun-28 20:30 spark_rapids_pytools/__init__.py
--rw-r--r--  2.0 unx      992 b- defN 23-Jun-28 20:30 spark_rapids_pytools/build.py
--rw-r--r--  2.0 unx     1324 b- defN 23-Jun-28 20:30 spark_rapids_pytools/wrapper.py
--rw-r--r--  2.0 unx      646 b- defN 23-Jun-28 20:30 spark_rapids_pytools/cloud_api/__init__.py
--rw-r--r--  2.0 unx     8507 b- defN 23-Jun-28 20:30 spark_rapids_pytools/cloud_api/azurestorage.py
--rw-r--r--  2.0 unx    12837 b- defN 23-Jun-28 20:30 spark_rapids_pytools/cloud_api/databricks_aws.py
--rw-r--r--  2.0 unx     1268 b- defN 23-Jun-28 20:30 spark_rapids_pytools/cloud_api/databricks_aws_job.py
--rw-r--r--  2.0 unx    16418 b- defN 23-Jun-28 20:30 spark_rapids_pytools/cloud_api/databricks_azure.py
--rw-r--r--  2.0 unx     2428 b- defN 23-Jun-28 20:30 spark_rapids_pytools/cloud_api/databricks_azure_job.py
--rw-r--r--  2.0 unx    24930 b- defN 23-Jun-28 20:30 spark_rapids_pytools/cloud_api/dataproc.py
--rw-r--r--  2.0 unx     1426 b- defN 23-Jun-28 20:30 spark_rapids_pytools/cloud_api/dataproc_job.py
--rw-r--r--  2.0 unx    22142 b- defN 23-Jun-28 20:30 spark_rapids_pytools/cloud_api/emr.py
--rw-r--r--  2.0 unx    11269 b- defN 23-Jun-28 20:30 spark_rapids_pytools/cloud_api/emr_job.py
--rw-r--r--  2.0 unx     4939 b- defN 23-Jun-28 20:30 spark_rapids_pytools/cloud_api/gstorage.py
--rw-r--r--  2.0 unx    13541 b- defN 23-Jun-28 20:30 spark_rapids_pytools/cloud_api/onprem.py
--rw-r--r--  2.0 unx     4055 b- defN 23-Jun-28 20:30 spark_rapids_pytools/cloud_api/s3storage.py
--rw-r--r--  2.0 unx    51283 b- defN 23-Jun-28 20:30 spark_rapids_pytools/cloud_api/sp_types.py
--rw-r--r--  2.0 unx      658 b- defN 23-Jun-28 20:30 spark_rapids_pytools/common/__init__.py
--rw-r--r--  2.0 unx      978 b- defN 23-Jun-28 20:30 spark_rapids_pytools/common/exceptions.py
--rw-r--r--  2.0 unx     5432 b- defN 23-Jun-28 20:30 spark_rapids_pytools/common/prop_manager.py
--rw-r--r--  2.0 unx    14712 b- defN 23-Jun-28 20:30 spark_rapids_pytools/common/sys_storage.py
--rw-r--r--  2.0 unx    14006 b- defN 23-Jun-28 20:30 spark_rapids_pytools/common/utilities.py
--rw-r--r--  2.0 unx      659 b- defN 23-Jun-28 20:30 spark_rapids_pytools/pricing/__init__.py
--rw-r--r--  2.0 unx     3429 b- defN 23-Jun-28 20:30 spark_rapids_pytools/pricing/databricks_azure_pricing.py
--rw-r--r--  2.0 unx     3522 b- defN 23-Jun-28 20:30 spark_rapids_pytools/pricing/databricks_pricing.py
--rw-r--r--  2.0 unx     4247 b- defN 23-Jun-28 20:30 spark_rapids_pytools/pricing/dataproc_pricing.py
--rw-r--r--  2.0 unx     4717 b- defN 23-Jun-28 20:30 spark_rapids_pytools/pricing/emr_pricing.py
--rw-r--r--  2.0 unx     6400 b- defN 23-Jun-28 20:30 spark_rapids_pytools/pricing/price_provider.py
--rw-r--r--  2.0 unx      666 b- defN 23-Jun-28 20:30 spark_rapids_pytools/rapids/__init__.py
--rw-r--r--  2.0 unx     8830 b- defN 23-Jun-28 20:30 spark_rapids_pytools/rapids/bootstrap.py
--rw-r--r--  2.0 unx     5140 b- defN 23-Jun-28 20:30 spark_rapids_pytools/rapids/diagnostic.py
--rw-r--r--  2.0 unx    13009 b- defN 23-Jun-28 20:30 spark_rapids_pytools/rapids/profiling.py
--rw-r--r--  2.0 unx    43658 b- defN 23-Jun-28 20:30 spark_rapids_pytools/rapids/qualification.py
--rw-r--r--  2.0 unx     6864 b- defN 23-Jun-28 20:30 spark_rapids_pytools/rapids/rapids_job.py
--rw-r--r--  2.0 unx    33590 b- defN 23-Jun-28 20:30 spark_rapids_pytools/rapids/rapids_tool.py
--rw-r--r--  2.0 unx     6576 b- defN 23-Jun-28 20:30 spark_rapids_pytools/rapids/tool_ctxt.py
--rw-r--r--  2.0 unx     1390 b- defN 23-Jun-28 20:30 spark_rapids_pytools/resources/bootstrap-conf.yaml
--rw-r--r--  2.0 unx    30566 b- defN 23-Jun-28 20:30 spark_rapids_pytools/resources/databricks-premium-catalog.json
--rw-r--r--  2.0 unx    10448 b- defN 23-Jun-28 20:30 spark_rapids_pytools/resources/databricks_aws-configs.json
--rw-r--r--  2.0 unx    10017 b- defN 23-Jun-28 20:30 spark_rapids_pytools/resources/databricks_azure-configs.json
--rw-r--r--  2.0 unx     8047 b- defN 23-Jun-28 20:30 spark_rapids_pytools/resources/dataproc-configs.json
--rw-r--r--  2.0 unx       30 b- defN 23-Jun-28 20:30 spark_rapids_pytools/resources/diagnostic-conf.yaml
--rw-r--r--  2.0 unx     8994 b- defN 23-Jun-28 20:30 spark_rapids_pytools/resources/emr-configs.json
--rw-r--r--  2.0 unx     4727 b- defN 23-Jun-28 20:30 spark_rapids_pytools/resources/onprem-configs.json
--rw-r--r--  2.0 unx    38903 b- defN 23-Jun-28 20:30 spark_rapids_pytools/resources/premium-databricks-azure-catalog.json
--rw-r--r--  2.0 unx     1460 b- defN 23-Jun-28 20:30 spark_rapids_pytools/resources/profiling-conf.yaml
--rw-r--r--  2.0 unx     4273 b- defN 23-Jun-28 20:30 spark_rapids_pytools/resources/qualification-conf.yaml
--rw-r--r--  2.0 unx      671 b- defN 23-Jun-28 20:30 spark_rapids_pytools/resources/templates/dataproc-create_gpu_cluster_script.ms
--rw-r--r--  2.0 unx      518 b- defN 23-Jun-28 20:30 spark_rapids_pytools/resources/templates/dataproc-run_bootstrap.ms
--rw-r--r--  2.0 unx      855 b- defN 23-Jun-28 20:30 spark_rapids_pytools/resources/templates/emr-create_gpu_cluster_script.ms
--rw-r--r--  2.0 unx      537 b- defN 23-Jun-28 20:30 spark_rapids_pytools/resources/templates/emr-run_bootstrap.ms
--rw-r--r--  2.0 unx      630 b- defN 23-Jun-28 20:30 spark_rapids_pytools/wrappers/__init__.py
--rw-r--r--  2.0 unx     8104 b- defN 23-Jun-28 20:30 spark_rapids_pytools/wrappers/databricks_aws_wrapper.py
--rw-r--r--  2.0 unx     7985 b- defN 23-Jun-28 20:30 spark_rapids_pytools/wrappers/databricks_azure_wrapper.py
--rw-r--r--  2.0 unx    16140 b- defN 23-Jun-28 20:30 spark_rapids_pytools/wrappers/dataproc_wrapper.py
--rw-r--r--  2.0 unx    17649 b- defN 23-Jun-28 20:30 spark_rapids_pytools/wrappers/emr_wrapper.py
--rw-r--r--  2.0 unx     4480 b- defN 23-Jun-28 20:30 spark_rapids_pytools/wrappers/onprem_wrapper.py
--rw-r--r--  2.0 unx    21086 b- defN 23-Jun-28 20:30 spark_rapids_user_tools-23.6.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     2939 b- defN 23-Jun-28 20:30 spark_rapids_user_tools-23.6.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-28 20:30 spark_rapids_user_tools-23.6.0.dist-info/WHEEL
--rw-r--r--  2.0 unx      152 b- defN 23-Jun-28 20:30 spark_rapids_user_tools-23.6.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       49 b- defN 23-Jun-28 20:30 spark_rapids_user_tools-23.6.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     8315 b- defN 23-Jun-28 20:30 spark_rapids_user_tools-23.6.0.dist-info/RECORD
-80 files, 1406039 bytes uncompressed, 257903 bytes compressed:  81.7%
+Zip file size: 158956 bytes, number of entries: 65
+-rw-r--r--  2.0 unx      750 b- defN 23-Jul-03 18:44 spark_rapids_pytools/__init__.py
+-rw-r--r--  2.0 unx      992 b- defN 23-Jul-03 18:44 spark_rapids_pytools/build.py
+-rw-r--r--  2.0 unx     1324 b- defN 23-Jul-03 18:44 spark_rapids_pytools/wrapper.py
+-rw-r--r--  2.0 unx      646 b- defN 23-Jul-03 18:44 spark_rapids_pytools/cloud_api/__init__.py
+-rw-r--r--  2.0 unx     8507 b- defN 23-Jul-03 18:44 spark_rapids_pytools/cloud_api/azurestorage.py
+-rw-r--r--  2.0 unx    12837 b- defN 23-Jul-03 18:44 spark_rapids_pytools/cloud_api/databricks_aws.py
+-rw-r--r--  2.0 unx     1268 b- defN 23-Jul-03 18:44 spark_rapids_pytools/cloud_api/databricks_aws_job.py
+-rw-r--r--  2.0 unx    16418 b- defN 23-Jul-03 18:44 spark_rapids_pytools/cloud_api/databricks_azure.py
+-rw-r--r--  2.0 unx     2428 b- defN 23-Jul-03 18:44 spark_rapids_pytools/cloud_api/databricks_azure_job.py
+-rw-r--r--  2.0 unx    24930 b- defN 23-Jul-03 18:44 spark_rapids_pytools/cloud_api/dataproc.py
+-rw-r--r--  2.0 unx     1426 b- defN 23-Jul-03 18:44 spark_rapids_pytools/cloud_api/dataproc_job.py
+-rw-r--r--  2.0 unx    22142 b- defN 23-Jul-03 18:44 spark_rapids_pytools/cloud_api/emr.py
+-rw-r--r--  2.0 unx    11269 b- defN 23-Jul-03 18:44 spark_rapids_pytools/cloud_api/emr_job.py
+-rw-r--r--  2.0 unx     4939 b- defN 23-Jul-03 18:44 spark_rapids_pytools/cloud_api/gstorage.py
+-rw-r--r--  2.0 unx    13541 b- defN 23-Jul-03 18:44 spark_rapids_pytools/cloud_api/onprem.py
+-rw-r--r--  2.0 unx     4055 b- defN 23-Jul-03 18:44 spark_rapids_pytools/cloud_api/s3storage.py
+-rw-r--r--  2.0 unx    51283 b- defN 23-Jul-03 18:44 spark_rapids_pytools/cloud_api/sp_types.py
+-rw-r--r--  2.0 unx      658 b- defN 23-Jul-03 18:44 spark_rapids_pytools/common/__init__.py
+-rw-r--r--  2.0 unx      978 b- defN 23-Jul-03 18:44 spark_rapids_pytools/common/exceptions.py
+-rw-r--r--  2.0 unx     5432 b- defN 23-Jul-03 18:44 spark_rapids_pytools/common/prop_manager.py
+-rw-r--r--  2.0 unx    14712 b- defN 23-Jul-03 18:44 spark_rapids_pytools/common/sys_storage.py
+-rw-r--r--  2.0 unx    14006 b- defN 23-Jul-03 18:44 spark_rapids_pytools/common/utilities.py
+-rw-r--r--  2.0 unx      659 b- defN 23-Jul-03 18:44 spark_rapids_pytools/pricing/__init__.py
+-rw-r--r--  2.0 unx     3429 b- defN 23-Jul-03 18:44 spark_rapids_pytools/pricing/databricks_azure_pricing.py
+-rw-r--r--  2.0 unx     3522 b- defN 23-Jul-03 18:44 spark_rapids_pytools/pricing/databricks_pricing.py
+-rw-r--r--  2.0 unx     4247 b- defN 23-Jul-03 18:44 spark_rapids_pytools/pricing/dataproc_pricing.py
+-rw-r--r--  2.0 unx     4717 b- defN 23-Jul-03 18:44 spark_rapids_pytools/pricing/emr_pricing.py
+-rw-r--r--  2.0 unx     6400 b- defN 23-Jul-03 18:44 spark_rapids_pytools/pricing/price_provider.py
+-rw-r--r--  2.0 unx      666 b- defN 23-Jul-03 18:44 spark_rapids_pytools/rapids/__init__.py
+-rw-r--r--  2.0 unx     8830 b- defN 23-Jul-03 18:44 spark_rapids_pytools/rapids/bootstrap.py
+-rw-r--r--  2.0 unx     6546 b- defN 23-Jul-03 18:44 spark_rapids_pytools/rapids/diagnostic.py
+-rw-r--r--  2.0 unx    13489 b- defN 23-Jul-03 18:44 spark_rapids_pytools/rapids/profiling.py
+-rw-r--r--  2.0 unx    43658 b- defN 23-Jul-03 18:44 spark_rapids_pytools/rapids/qualification.py
+-rw-r--r--  2.0 unx     6864 b- defN 23-Jul-03 18:44 spark_rapids_pytools/rapids/rapids_job.py
+-rw-r--r--  2.0 unx    33590 b- defN 23-Jul-03 18:44 spark_rapids_pytools/rapids/rapids_tool.py
+-rw-r--r--  2.0 unx     6576 b- defN 23-Jul-03 18:44 spark_rapids_pytools/rapids/tool_ctxt.py
+-rw-r--r--  2.0 unx     1390 b- defN 23-Jul-03 18:44 spark_rapids_pytools/resources/bootstrap-conf.yaml
+-rwxr-xr-x  2.0 unx     4453 b- defN 23-Jul-03 18:44 spark_rapids_pytools/resources/collect.sh
+-rw-r--r--  2.0 unx    30566 b- defN 23-Jul-03 18:44 spark_rapids_pytools/resources/databricks-premium-catalog.json
+-rw-r--r--  2.0 unx    10448 b- defN 23-Jul-03 18:44 spark_rapids_pytools/resources/databricks_aws-configs.json
+-rw-r--r--  2.0 unx    10017 b- defN 23-Jul-03 18:44 spark_rapids_pytools/resources/databricks_azure-configs.json
+-rw-r--r--  2.0 unx     8047 b- defN 23-Jul-03 18:44 spark_rapids_pytools/resources/dataproc-configs.json
+-rw-r--r--  2.0 unx       30 b- defN 23-Jul-03 18:44 spark_rapids_pytools/resources/diagnostic-conf.yaml
+-rw-r--r--  2.0 unx     8994 b- defN 23-Jul-03 18:44 spark_rapids_pytools/resources/emr-configs.json
+-rw-r--r--  2.0 unx     4727 b- defN 23-Jul-03 18:44 spark_rapids_pytools/resources/onprem-configs.json
+-rw-r--r--  2.0 unx    38903 b- defN 23-Jul-03 18:44 spark_rapids_pytools/resources/premium-databricks-azure-catalog.json
+-rw-r--r--  2.0 unx     1460 b- defN 23-Jul-03 18:44 spark_rapids_pytools/resources/profiling-conf.yaml
+-rw-r--r--  2.0 unx     4273 b- defN 23-Jul-03 18:44 spark_rapids_pytools/resources/qualification-conf.yaml
+-rw-r--r--  2.0 unx     2195 b- defN 23-Jul-03 18:44 spark_rapids_pytools/resources/dev/process_databricks_azure_pricing.py
+-rw-r--r--  2.0 unx      671 b- defN 23-Jul-03 18:44 spark_rapids_pytools/resources/templates/dataproc-create_gpu_cluster_script.ms
+-rw-r--r--  2.0 unx      518 b- defN 23-Jul-03 18:44 spark_rapids_pytools/resources/templates/dataproc-run_bootstrap.ms
+-rw-r--r--  2.0 unx      855 b- defN 23-Jul-03 18:44 spark_rapids_pytools/resources/templates/emr-create_gpu_cluster_script.ms
+-rw-r--r--  2.0 unx      537 b- defN 23-Jul-03 18:44 spark_rapids_pytools/resources/templates/emr-run_bootstrap.ms
+-rw-r--r--  2.0 unx      630 b- defN 23-Jul-03 18:44 spark_rapids_pytools/wrappers/__init__.py
+-rw-r--r--  2.0 unx    13207 b- defN 23-Jul-03 18:44 spark_rapids_pytools/wrappers/databricks_aws_wrapper.py
+-rw-r--r--  2.0 unx     7985 b- defN 23-Jul-03 18:44 spark_rapids_pytools/wrappers/databricks_azure_wrapper.py
+-rw-r--r--  2.0 unx    16647 b- defN 23-Jul-03 18:44 spark_rapids_pytools/wrappers/dataproc_wrapper.py
+-rw-r--r--  2.0 unx    18151 b- defN 23-Jul-03 18:44 spark_rapids_pytools/wrappers/emr_wrapper.py
+-rw-r--r--  2.0 unx     4480 b- defN 23-Jul-03 18:44 spark_rapids_pytools/wrappers/onprem_wrapper.py
+-rw-r--r--  2.0 unx    21086 b- defN 23-Jul-03 18:44 spark_rapids_user_tools-23.6.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2927 b- defN 23-Jul-03 18:44 spark_rapids_user_tools-23.6.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-03 18:44 spark_rapids_user_tools-23.6.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       78 b- defN 23-Jul-03 18:44 spark_rapids_user_tools-23.6.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       21 b- defN 23-Jul-03 18:44 spark_rapids_user_tools-23.6.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     6768 b- defN 23-Jul-03 18:44 spark_rapids_user_tools-23.6.1.dist-info/RECORD
+65 files, 577890 bytes uncompressed, 147760 bytes compressed:  74.4%
```

## zipnote {}

```diff
@@ -1,58 +1,7 @@
-Filename: spark_rapids_dataproc_tools/__init__.py
-Comment: 
-
-Filename: spark_rapids_dataproc_tools/cost_estimator.py
-Comment: 
-
-Filename: spark_rapids_dataproc_tools/dataproc_utils.py
-Comment: 
-
-Filename: spark_rapids_dataproc_tools/dataproc_wrapper.py
-Comment: 
-
-Filename: spark_rapids_dataproc_tools/diag.py
-Comment: 
-
-Filename: spark_rapids_dataproc_tools/diag_dataproc.py
-Comment: 
-
-Filename: spark_rapids_dataproc_tools/rapids_models.py
-Comment: 
-
-Filename: spark_rapids_dataproc_tools/utilities.py
-Comment: 
-
-Filename: spark_rapids_dataproc_tools/csp/__init__.py
-Comment: 
-
-Filename: spark_rapids_dataproc_tools/csp/csp.py
-Comment: 
-
-Filename: spark_rapids_dataproc_tools/csp/dataproc.py
-Comment: 
-
-Filename: spark_rapids_dataproc_tools/diag_scripts/hello_world.py
-Comment: 
-
-Filename: spark_rapids_dataproc_tools/diag_scripts/perf.py
-Comment: 
-
-Filename: spark_rapids_dataproc_tools/resources/bootstrap-conf.yaml
-Comment: 
-
-Filename: spark_rapids_dataproc_tools/resources/gcloud-catalog.json
-Comment: 
-
-Filename: spark_rapids_dataproc_tools/resources/profiling-conf.yaml
-Comment: 
-
-Filename: spark_rapids_dataproc_tools/resources/qualification-conf.yaml
-Comment: 
-
 Filename: spark_rapids_pytools/__init__.py
 Comment: 
 
 Filename: spark_rapids_pytools/build.py
 Comment: 
 
 Filename: spark_rapids_pytools/wrapper.py
@@ -156,14 +105,17 @@
 
 Filename: spark_rapids_pytools/rapids/tool_ctxt.py
 Comment: 
 
 Filename: spark_rapids_pytools/resources/bootstrap-conf.yaml
 Comment: 
 
+Filename: spark_rapids_pytools/resources/collect.sh
+Comment: 
+
 Filename: spark_rapids_pytools/resources/databricks-premium-catalog.json
 Comment: 
 
 Filename: spark_rapids_pytools/resources/databricks_aws-configs.json
 Comment: 
 
 Filename: spark_rapids_pytools/resources/databricks_azure-configs.json
@@ -186,14 +138,17 @@
 
 Filename: spark_rapids_pytools/resources/profiling-conf.yaml
 Comment: 
 
 Filename: spark_rapids_pytools/resources/qualification-conf.yaml
 Comment: 
 
+Filename: spark_rapids_pytools/resources/dev/process_databricks_azure_pricing.py
+Comment: 
+
 Filename: spark_rapids_pytools/resources/templates/dataproc-create_gpu_cluster_script.ms
 Comment: 
 
 Filename: spark_rapids_pytools/resources/templates/dataproc-run_bootstrap.ms
 Comment: 
 
 Filename: spark_rapids_pytools/resources/templates/emr-create_gpu_cluster_script.ms
@@ -216,26 +171,26 @@
 
 Filename: spark_rapids_pytools/wrappers/emr_wrapper.py
 Comment: 
 
 Filename: spark_rapids_pytools/wrappers/onprem_wrapper.py
 Comment: 
 
-Filename: spark_rapids_user_tools-23.6.0.dist-info/LICENSE
+Filename: spark_rapids_user_tools-23.6.1.dist-info/LICENSE
 Comment: 
 
-Filename: spark_rapids_user_tools-23.6.0.dist-info/METADATA
+Filename: spark_rapids_user_tools-23.6.1.dist-info/METADATA
 Comment: 
 
-Filename: spark_rapids_user_tools-23.6.0.dist-info/WHEEL
+Filename: spark_rapids_user_tools-23.6.1.dist-info/WHEEL
 Comment: 
 
-Filename: spark_rapids_user_tools-23.6.0.dist-info/entry_points.txt
+Filename: spark_rapids_user_tools-23.6.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: spark_rapids_user_tools-23.6.0.dist-info/top_level.txt
+Filename: spark_rapids_user_tools-23.6.1.dist-info/top_level.txt
 Comment: 
 
-Filename: spark_rapids_user_tools-23.6.0.dist-info/RECORD
+Filename: spark_rapids_user_tools-23.6.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## spark_rapids_pytools/__init__.py

```diff
@@ -12,9 +12,9 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """init file of the spark_rapids_pytools package."""
 
 from spark_rapids_pytools.build import get_version
 
-VERSION = '23.06.0'
+VERSION = '23.06.1'
 __version__ = get_version(VERSION)
```

## spark_rapids_pytools/wrapper.py

```diff
@@ -23,15 +23,15 @@
 from spark_rapids_pytools.wrappers.onprem_wrapper import OnPremWrapper
 
 
 def main():
     fire.Fire({
         'emr': EMRWrapper,
         'dataproc': DataprocWrapper,
-        'databricks_aws': DBAWSWrapper,
-        'databricks_azure': DBAzureWrapper,
+        'databricks-aws': DBAWSWrapper,
+        'databricks-azure': DBAzureWrapper,
         'onprem': OnPremWrapper
     })
 
 
 if __name__ == '__main__':
     main()
```

## spark_rapids_pytools/rapids/diagnostic.py

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Implementation class representing wrapper around diagnostic tool."""
 
+from concurrent.futures import ThreadPoolExecutor
 from dataclasses import dataclass
 
 from spark_rapids_pytools.cloud_api.sp_types import ClusterBase, SparkNodeType
 from spark_rapids_pytools.common.sys_storage import FSUtil
 from spark_rapids_pytools.common.utilities import Utils
 from spark_rapids_pytools.rapids.rapids_tool import RapidsTool
 
@@ -26,14 +27,33 @@
 class Diagnostic(RapidsTool):
     """
     Wrapper layer around Diagnostic Tool.
     """
     name = 'diagnostic'
     exec_cluster: ClusterBase = None
     all_nodes: list = None
+    thread_num: int = 3
+
+    def _process_custom_args(self):
+        thread_num = self.wrapper_options.get('threadNum', 3)
+        if thread_num < 1 or thread_num > 10:
+            raise RuntimeError(f'Invalid thread number: {thread_num} (Valid value: 1~10)')
+
+        self.thread_num = thread_num
+        self.logger.debug('Set thread number as: %d', self.thread_num)
+
+        self.logger.warning('This operation will collect sensitive information from your cluster, '
+                            'such as OS & HW info, Yarn/Spark configurations and log files etc.')
+        yes = self.wrapper_options.get('yes', False)
+        if yes:
+            self.logger.info('Confirmed by command line option.')
+        else:
+            user_input = input('Do you want to continue (yes/no): ')
+            if user_input.lower() not in ['yes', 'y']:
+                raise RuntimeError('User canceled the operation.')
 
     def requires_cluster_connection(self) -> bool:
         return True
 
     def _connect_to_execution_cluster(self):
         super()._connect_to_execution_cluster()
 
@@ -44,69 +64,82 @@
         super()._process_output_args()
 
         # Set remote output folder same as local output folder name
         output_path = self.ctxt.get_output_folder()
         folder_name = FSUtil.get_resource_name(output_path)
         self.ctxt.set_remote('outputFolder', folder_name)
 
-    def _upload_scripts(self):
+    def _upload_scripts(self, node):
         """
-        Upload scripts to both driver & worker nodes
+        Upload scripts to specified node
         :return:
         """
         script = Utils.resource_path('collect.sh')
 
         try:
-            for node in self.all_nodes:
-                self.logger.info('Uploading script to node: %s', node.get_name())
-                self.exec_cluster.scp_to_node(node, str(script), '/tmp/')
+            self.logger.info('Uploading script to node: %s', node.get_name())
+            self.exec_cluster.scp_to_node(node, str(script), '/tmp/')
 
         except Exception as e:
-            self.logger.error('Error while uploading script to remote node')
+            self.logger.error('Error while uploading script to node: %s', node.get_name())
             raise e
 
-    def _run_rapids_tool(self):
+    def _collect_info(self, node):
         """
-        Run diagnostic tool from both driver & worker nodes to collect info
+        Run task to collect info from specified node
         :return:
         """
-        self.logger.info('Uploading script to remote cluster nodes:')
-        self._upload_scripts()
+        self._upload_scripts(node)
 
-        self.logger.info('Collecting info on remote cluster nodes:')
         remote_output_folder = self.ctxt.get_remote('outputFolder')
         ssh_cmd = f'"PREFIX={remote_output_folder} /tmp/collect.sh"'
 
         try:
-            for node in self.all_nodes:
-                self.logger.info('Collecting info on node: %s', node.get_name())
-                self.exec_cluster.run_cmd_node(node, ssh_cmd)
+            self.logger.info('Collecting info on node: %s', node.get_name())
+            self.exec_cluster.run_cmd_node(node, ssh_cmd)
 
         except Exception as e:
-            self.logger.error('Error while collecting info from remote node')
+            self.logger.error('Error while collecting info from node: %s', node.get_name())
             raise e
 
+    def _run_rapids_tool(self):
+        """
+        Run diagnostic tool from both driver & worker nodes to collect info
+        :return:
+        """
+        with ThreadPoolExecutor(max_workers=self.thread_num) as executor:
+            for e in executor.map(self._collect_info, self.all_nodes):
+                # Raise exception if any error occurred
+                if e:
+                    raise e
+
     def _download_output(self):
         self.logger.info('Downloading results from remote nodes:')
 
         output_path = self.ctxt.get_output_folder()
         remote_output_folder = self.ctxt.get_remote('outputFolder')
         remote_output_result = f'/tmp/{remote_output_folder}*.tgz'
 
-        try:
-            for node in self.all_nodes:
+        def _download_result(node):
+            try:
                 node_output_path = FSUtil.build_path(output_path, node.get_name())
                 FSUtil.make_dirs(node_output_path, exist_ok=True)
 
                 self.logger.info('Downloading results from node: %s', node.get_name())
                 self.exec_cluster.scp_from_node(node, remote_output_result, node_output_path)
 
-        except Exception as e:
-            self.logger.error('Error while downloading collected info from remote node')
-            raise e
+            except Exception as e:
+                self.logger.error('Error while downloading collected info from node: %s', node.get_name())
+                raise e
+
+        with ThreadPoolExecutor(max_workers=self.thread_num) as executor:
+            for e in executor.map(_download_result, self.all_nodes):
+                # Raise exception if any error occurred
+                if e:
+                    raise e
 
     def _process_output(self):
         self.logger.info('Processing the collected results.')
 
         output_path = self.ctxt.get_output_folder()
         region = self.exec_cluster.get_region()
         worker_count = self.exec_cluster.get_nodes_cnt(SparkNodeType.WORKER)
```

## spark_rapids_pytools/rapids/profiling.py

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Implementation class representing wrapper around the RAPIDS acceleration Profiling tool."""
 
 import re
+from copy import deepcopy
 from dataclasses import dataclass
 from itertools import chain
 from typing import List
 
 import yaml
 from tabulate import tabulate
 
@@ -104,15 +105,22 @@
                 # the scala code expects a unit
                 'memory': f'{worker_hw_info.gpu_info.gpu_mem}MiB',
                 'count': worker_hw_info.gpu_info.num_gpus,
                 'name': worker_hw_info.gpu_info.get_gpu_device_name()
             },
             'softwareProperties': cluster_ob.get_all_spark_properties()
         }
-        self.logger.debug('Auto-tuner worker info: %s', worker_info)
+        worker_info_redacted = deepcopy(worker_info)
+        if worker_info_redacted['softwareProperties']:
+            for key in worker_info_redacted['softwareProperties']:
+                if 's3a.secret.key' in key:
+                    worker_info_redacted['softwareProperties'][key] = 'MY_S3A_SECRET_KEY'
+                elif 's3a.access.key' in key:
+                    worker_info_redacted['softwareProperties'][key] = 'MY_S3A_ACCESS_KEY'
+        self.logger.debug('Auto-tuner worker info: %s', worker_info_redacted)
         with open(file_path, 'w', encoding='utf-8') as worker_info_file:
             self.logger.debug('Opening file %s to write worker info', file_path)
             yaml.dump(worker_info, worker_info_file, sort_keys=False)
 
     def _generate_autotuner_input(self):
         gpu_cluster_obj = self.ctxt.get_ctxt('gpuClusterProxy')
         input_file_name = 'worker_info.yaml'
```

## spark_rapids_pytools/wrappers/databricks_aws_wrapper.py

```diff
@@ -13,14 +13,15 @@
 # limitations under the License.
 
 
 """Wrapper class to run tools associated with RAPIDS Accelerator for Apache Spark plugin on DATABRICKS_AWS."""
 
 from spark_rapids_pytools.cloud_api.sp_types import DeployMode, CloudPlatform
 from spark_rapids_pytools.common.utilities import ToolLogging
+from spark_rapids_pytools.rapids.profiling import ProfilingAsLocal
 from spark_rapids_pytools.rapids.qualification import QualFilterApp, QualificationAsLocal, QualGpuClusterReshapeType
 
 
 class CliDBAWSLocalMode:  # pylint: disable=too-few-public-methods
     """
     A wrapper that runs the RAPIDS Accelerator tools locally on the dev machine for DATABRICKS_AWS.
     """
@@ -122,15 +123,97 @@
         }
         QualificationAsLocal(platform_type=CloudPlatform.DATABRICKS_AWS,
                              cluster=None,
                              output_folder=local_folder,
                              wrapper_options=wrapper_qual_options,
                              rapids_options=rapids_options).launch()
 
+    @staticmethod
+    def profiling(gpu_cluster: str = None,
+                  worker_info: str = None,
+                  eventlogs: str = None,
+                  profile: str = None,
+                  aws_profile: str = None,
+                  local_folder: str = None,
+                  remote_folder: str = None,
+                  tools_jar: str = None,
+                  credentials_file: str = None,
+                  jvm_heap_size: int = 24,
+                  verbose: bool = False,
+                  **rapids_options) -> None:
+        """
+        The Profiling tool analyzes both CPU or GPU generated event logs and generates information
+        which can be used for debugging and profiling Apache Spark applications.
+
+        :param  gpu_cluster: The Databricks-cluster on which the Spark applications were executed. The argument
+                can be a Databricks-cluster or a valid path to the cluster's properties file (json format)
+                generated by the databricks-CLI. If missing, then the argument worker_info has to be provided.
+        :param  worker_info: A path pointing to a yaml file containing the system information of a
+                worker node. It is assumed that all workers are homogenous.
+                If missing, the wrapper pulls the worker info from the "gpu_cluster".
+        :param  eventlogs: Event log filenames or S3 storage directories
+                containing event logs (comma separated). If missing, the wrapper reads the Spark's
+                property `spark.eventLog.dir` defined in `gpu_cluster`. This property should be included
+                in the output of `databricks clusters get [--cluster-id CLUSTER_ID| --cluster-name CLUSTER_NAME]`.
+                Note that the wrapper will raise an exception if the property is not set.
+        :param profile: A named Databricks profile to get the settings/credentials of the Databricks CLI.
+        :param aws_profile: A named AWS profile to get the settings/credentials of the AWS account.
+        :param local_folder: Local work-directory path to store the output and to be used as root
+                directory for temporary folders/files. The final output will go into a subdirectory called
+                ${local_folder}/prof-${EXEC_ID} where exec_id is an auto-generated unique identifier of the
+                execution. If the argument is NONE, the default value is the env variable
+                RAPIDS_USER_TOOLS_OUTPUT_DIRECTORY if any; or the current working directory.
+        :param remote_folder: A S3 folder where the output is uploaded at the end of execution.
+                If no value is provided, the output will be only available on local disk.
+        :param tools_jar: Path to a bundled jar including Rapids tool. The path is a local filesystem,
+                or remote S3 url. If missing, the wrapper downloads the latest rapids-4-spark-tools_*.jar
+                from maven repo.
+        :param credentials_file: The local path of JSON file that contains the application credentials.
+               If missing, the wrapper looks for "DATABRICKS_CONFIG_FILE" environment variable
+               to provide the location of a credential file. The default credentials file exists as
+               "~/.databrickscfg" on Unix, Linux, or macOS.
+        :param verbose: True or False to enable verbosity to the wrapper script.
+        :param jvm_heap_size: The maximum heap size of the JVM in gigabytes.
+        :param rapids_options: A list of valid Profiling tool options.
+                Note that the wrapper ignores ["output-directory", "worker-info"] flags, and it does not support
+                multiple "spark-property" arguments.
+                For more details on Profiling tool options, please visit
+                https://nvidia.github.io/spark-rapids/docs/spark-profiling-tool.html#profiling-tool-options
+        """
+        if verbose:
+            # when debug is set to true set it in the environment.
+            ToolLogging.enable_debug_mode()
+        wrapper_prof_options = {
+            'platformOpts': {
+                # the databricks profile
+                'profile': profile,
+                'awsProfile': aws_profile,
+                'credentialFile': credentials_file,
+                'deployMode': DeployMode.LOCAL,
+            },
+            'migrationClustersProps': {
+                'gpuCluster': gpu_cluster
+            },
+            'jobSubmissionProps': {
+                'remoteFolder': remote_folder,
+                'platformArgs': {
+                    'jvmMaxHeapSize': jvm_heap_size
+                }
+            },
+            'eventlogs': eventlogs,
+            'toolsJar': tools_jar,
+            'autoTunerFileInput': worker_info
+        }
+        ProfilingAsLocal(platform_type=CloudPlatform.DATABRICKS_AWS,
+                         output_folder=local_folder,
+                         wrapper_options=wrapper_prof_options,
+                         rapids_options=rapids_options).launch()
+
 
 class DBAWSWrapper:  # pylint: disable=too-few-public-methods
     """
     A wrapper script to run RAPIDS Accelerator tools (Qualification, Profiling, and Bootstrap) on Databricks_AWS.
     """
 
     def __init__(self):
         self.qualification = CliDBAWSLocalMode.qualification
+        self.profiling = CliDBAWSLocalMode.profiling
```

## spark_rapids_pytools/wrappers/dataproc_wrapper.py

```diff
@@ -151,15 +151,15 @@
         :param  gpu_cluster: The Dataproc-cluster on which the Spark applications were executed. The argument
                 can be a Dataproc-cluster or a valid path to the cluster's properties file (json format)
                 generated by the gcloud-CLI. If missing, then the argument worker_info has to be provided
         :param  worker_info: A path pointing to a yaml file containing the system information of a
                 worker node. It is assumed that all workers are homogenous.
                 If missing, the wrapper pulls the worker info from the "gpu_cluster"
         :param  eventlogs: Event log filenames or gs storage directories
-                containing event logs (comma separated). If missing, the wrapper Reads the Spark's
+                containing event logs (comma separated). If missing, the wrapper reads the Spark's
                 property `spark.eventLog.dir` defined in `gpu_cluster`. This property should be included
                 in the output of `gcloud dataproc clusters describe`.
                 Note that the wrapper will raise an exception if the property is not set
         :param local_folder: Local work-directory path to store the output and to be used as root
                 directory for temporary folders/files. The final output will go into a subdirectory called
                 ${local_folder}/prof-${EXEC_ID} where exec_id is an auto-generated unique identifier of the
                 execution. If the argument is NONE, the default value is the env variable
@@ -236,30 +236,38 @@
                                    output_folder=output_folder,
                                    wrapper_options=wrapper_boot_options)
         bootstrap_tool.launch()
 
     @staticmethod
     def diagnostic(cluster: str,
                    output_folder: str = None,
+                   thread_num: int = 3,
+                   yes: bool = False,
                    verbose: bool = False) -> None:
         """
-        Diagnostic tool to collects information from Dataproc cluster, such as OS version, # of worker nodes,
-        Yarn configuration, Spark version and error logs etc.
+        Diagnostic tool to collect information from Dataproc cluster, such as OS version, # of worker nodes,
+        Yarn configuration, Spark version and error logs etc. Please note, some sensitive information might
+        be collected by this tool, e.g. access secret configured in configuration files or dumped to log files.
         :param cluster: Name of the Dataproc cluster running an accelerated computing instance class
         :param output_folder: Local path where the final recommendations will be saved.
                Note that this argument only accepts local filesystem. If the argument is NONE,
                the default value is the env variable "RAPIDS_USER_TOOLS_OUTPUT_DIRECTORY" if any;
                or the current working directory
+        :param thread_num: Number of threads to access remote cluster nodes in parallel. The valid value
+               is 1~10. The default value is 3.
+        :param yes: auto confirm to interactive question.
         :param verbose: True or False to enable verbosity to the wrapper script.
         """
         if verbose:
             # when debug is set to true set it in the environment.
             ToolLogging.enable_debug_mode()
         wrapper_diag_options = {
             'platformOpts': {},
+            'threadNum': thread_num,
+            'yes': yes,
         }
         diag_tool = Diagnostic(platform_type=CloudPlatform.DATAPROC,
                                cluster=cluster,
                                output_folder=output_folder,
                                wrapper_options=wrapper_diag_options)
         diag_tool.launch()
```

## spark_rapids_pytools/wrappers/emr_wrapper.py

```diff
@@ -160,38 +160,46 @@
         bootstrap_tool.launch()
 
     @staticmethod
     def diagnostic(cluster: str,
                    profile: str = None,
                    output_folder: str = None,
                    key_pair_path: str = None,
+                   thread_num: int = 3,
+                   yes: bool = False,
                    verbose: bool = False) -> None:
         """
-        Diagnostic tool to collects information from Dataproc cluster, such as OS version, # of worker nodes,
-        Yarn configuration, Spark version and error logs etc.
+        Diagnostic tool to collect information from EMR cluster, such as OS version, # of worker nodes,
+        Yarn configuration, Spark version and error logs etc. Please note, some sensitive information might
+        be collected by this tool, e.g. access secret configured in configuration files or dumped to log files.
         :param cluster: Name of the EMR cluster running an accelerated computing instance class g4dn.*
         :param profile: A named AWS profile to get the settings/credentials of the AWS account.
         :param output_folder: Local path where the archived result will be saved.
                Note that this argument only accepts local filesystem. If the argument is NONE,
                the default value is the env variable "RAPIDS_USER_TOOLS_OUTPUT_DIRECTORY" if any;
                or the current working directory.
         :param key_pair_path: A '.pem' file path that enables to connect to EC2 instances using SSH.
                If missing, the wrapper reads the env variable 'RAPIDS_USER_TOOLS_KEY_PAIR_PATH' if any.
                For more details on creating key pairs,
                visit https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/create-key-pairs.html.
+        :param thread_num: Number of threads to access remote cluster nodes in parallel. The valid value
+               is 1~10. The default value is 3.
+        :param yes: auto confirm to interactive question.
         :param verbose: True or False to enable verbosity to the wrapper script.
         """
         if verbose:
             # when debug is set to true set it in the environment.
             ToolLogging.enable_debug_mode()
         wrapper_diag_options = {
             'platformOpts': {
                 'profile': profile,
                 'keyPairPath': key_pair_path,
             },
+            'threadNum': thread_num,
+            'yes': yes,
         }
         diag_tool = Diagnostic(platform_type=CloudPlatform.EMR,
                                cluster=cluster,
                                output_folder=output_folder,
                                wrapper_options=wrapper_diag_options)
         diag_tool.launch()
```

## Comparing `spark_rapids_user_tools-23.6.0.dist-info/LICENSE` & `spark_rapids_user_tools-23.6.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `spark_rapids_user_tools-23.6.0.dist-info/METADATA` & `spark_rapids_user_tools-23.6.1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: spark-rapids-user-tools
-Version: 23.6.0
+Version: 23.6.1
 Summary: A simple wrapper process around cloud service providers to run tools for the RAPIDS Accelerator for Apache Spark.
-Author-email: Raza Jafri <raza.jafri@gmail.com>, Ahmed Hussein <a@ahussein.me>
+Author-email: NVIDIA Corporation <spark-rapids-support@nvidia.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: chevron (==0.14.0)
```

## Comparing `spark_rapids_user_tools-23.6.0.dist-info/RECORD` & `spark_rapids_user_tools-23.6.1.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,10 @@
-spark_rapids_dataproc_tools/__init__.py,sha256=9J-l7hjbbI2mJnqqK-jtlv9t9xZ6crJvbHL8u8xjags,648
-spark_rapids_dataproc_tools/cost_estimator.py,sha256=S29-6uYnrTzC82k8ieJfeKGvwbw-WYxGBeRmB43LRAg,10120
-spark_rapids_dataproc_tools/dataproc_utils.py,sha256=Ob4PA7sm9SEvKec142KsUhPdQUD3hjvLmqSncEGGKVM,27693
-spark_rapids_dataproc_tools/dataproc_wrapper.py,sha256=isPLQSE5ornegQ2CNkZJiKfm35ItgJYoQpTTiJ-adJM,15306
-spark_rapids_dataproc_tools/diag.py,sha256=raDYdKSTQzkQz-ZlqO5t4jcPniPu5mprNENkjQICiUM,10514
-spark_rapids_dataproc_tools/diag_dataproc.py,sha256=otMgpwr5xpcHGTspR_pH4dNbY2UuArwnMRnXeW9zxWQ,5344
-spark_rapids_dataproc_tools/rapids_models.py,sha256=EKlmZ9jtUlhIUmYnmBM-AQt_jUG4fLqFg6rPlv30pm8,63046
-spark_rapids_dataproc_tools/utilities.py,sha256=lY23B4lB4MdfznSNuSbX9R_Cfgh4CzwBLGuP9LhP56k,8782
-spark_rapids_dataproc_tools/csp/__init__.py,sha256=ySk_fqBwYU-spTD5AyN8wqyGCl2E-vdIbQhkJ6fVuno,921
-spark_rapids_dataproc_tools/csp/csp.py,sha256=sNDKuJMZ4LwfKuCQWOyzyavb-gdhNa-lz_CuIbf9L7Y,1671
-spark_rapids_dataproc_tools/csp/dataproc.py,sha256=NX1VvXqMTCCSw4whxD_6KoHWVSPQadXazjTtlRj6qGM,5196
-spark_rapids_dataproc_tools/diag_scripts/hello_world.py,sha256=d7OPcIZfQ_as5qJWkwno77kzsryU0_f4t8A6z-kIZP4,1154
-spark_rapids_dataproc_tools/diag_scripts/perf.py,sha256=7vUsfw7hWe2NoD8_37_f6c2AbocBIgAQVP2uSDj3H4I,1276
-spark_rapids_dataproc_tools/resources/bootstrap-conf.yaml,sha256=FfMyJqOt8VwK-FuVAASCenxBCk3EWkZbZ5Hwd9N8WlQ,1273
-spark_rapids_dataproc_tools/resources/gcloud-catalog.json,sha256=gsaT3fho6yLJGdpAMi6oRQjJtombuKa4vZaRPKqxMaM,684199
-spark_rapids_dataproc_tools/resources/profiling-conf.yaml,sha256=xluVs7e1AcbDXWUYt3_2FPZSiwGPCOJlsiwnnZT59nM,1416
-spark_rapids_dataproc_tools/resources/qualification-conf.yaml,sha256=ABoda4ZHAAE8uywI4vjjHgJ2pyzrShsL1zr7ksMbucA,2575
-spark_rapids_pytools/__init__.py,sha256=t6WfewYnib-Hsh60aegZzDazZQAeYUWQmwGej52_QA0,750
+spark_rapids_pytools/__init__.py,sha256=0swyb0tOSpVwpEU_yt3yo-AIZiPAiNZP-aZHixOPJhA,750
 spark_rapids_pytools/build.py,sha256=Ej4Pc2jPIyeVUUOyC67ZMc6Tj90NKj0DrXyniJc0FnY,992
-spark_rapids_pytools/wrapper.py,sha256=KQVpa4tNBqfRGa6iPFUO1DYlBGRprs72iSM2lpNoNHg,1324
+spark_rapids_pytools/wrapper.py,sha256=mKTxIpK3V_OKJ4ua3TSjasC5mITs_TRHU5dRfCqcde0,1324
 spark_rapids_pytools/cloud_api/__init__.py,sha256=NQSbmxhLzvnZrf4ltpgCLMjCEERPv5QoYo62LEdDBs8,646
 spark_rapids_pytools/cloud_api/azurestorage.py,sha256=yuFk7H5Y8aY0H5dOmeJBS03uhgS2nah5v0Kw2GJzDnE,8507
 spark_rapids_pytools/cloud_api/databricks_aws.py,sha256=g0XXBVeQwtVAjsm6Po3R3dUA-7CUqaRp9W7iFqkuU4I,12837
 spark_rapids_pytools/cloud_api/databricks_aws_job.py,sha256=ZNYM2pa8fObRhc9c9VcqCT6HxGJNfHeFhdoVYNek51E,1268
 spark_rapids_pytools/cloud_api/databricks_azure.py,sha256=D5FcZ-wo0lNf3NOMI6sXQGk8ur7RsYG1sBj1kys_kM0,16418
 spark_rapids_pytools/cloud_api/databricks_azure_job.py,sha256=u-wOcJXRyFCuEsXQypW8O09O5YQ2pt_gNcOlQjwpXYE,2428
 spark_rapids_pytools/cloud_api/dataproc.py,sha256=i4yoDrZ5D5vghN1KXq1HRXiNzefbRGi7GdpC40SCb84,24930
@@ -41,40 +24,42 @@
 spark_rapids_pytools/pricing/databricks_azure_pricing.py,sha256=HLto1Dbv61Awfo4icJiRiCkx3G8KDRfUBiTjloEy1WM,3429
 spark_rapids_pytools/pricing/databricks_pricing.py,sha256=q7pRBs2YGJAJnxItBUDYB00f3hdWsFKgK4sXZocjMC4,3522
 spark_rapids_pytools/pricing/dataproc_pricing.py,sha256=4-RuYxW9V0K0mqj2mqCJsKEUbvxPXHCwF4AsK1z6UXE,4247
 spark_rapids_pytools/pricing/emr_pricing.py,sha256=vat14Df8_1By-McNl2ot_75RAwjJkyTfXA24-iefrM4,4717
 spark_rapids_pytools/pricing/price_provider.py,sha256=zZt2ay-BN1vM0cZXkiEzY5kpnYx1brRCJcyfotU71lo,6400
 spark_rapids_pytools/rapids/__init__.py,sha256=xiYk9b76AV_v3fEELcYzXCUPvXQhCD687eJ5RCYQW7M,666
 spark_rapids_pytools/rapids/bootstrap.py,sha256=KEeF1Ux0mfqCW-6oyQOoImSuCm_MmoITm_t6qg9yB4s,8830
-spark_rapids_pytools/rapids/diagnostic.py,sha256=wwHvMq2Ohv1x-MoM_vMFZuPtPyZPPe_eO_kMndvTPYY,5140
-spark_rapids_pytools/rapids/profiling.py,sha256=D3Muau5k89CTAg7EA2q757OQsNsEboS6sgJJO_nQIwM,13009
+spark_rapids_pytools/rapids/diagnostic.py,sha256=pShr5Ndi8kxZXTbZ7fOkbWVk2opF1UYP0q4AJETGHGc,6546
+spark_rapids_pytools/rapids/profiling.py,sha256=n0l6-WKweQPBg_7g9rNb9YqIpsZcPVT3YosFZ3bmglQ,13489
 spark_rapids_pytools/rapids/qualification.py,sha256=5zKCPacUyWdVKhAupMncw6_4UgnDRt7kqQ8_kq0RfJ0,43658
 spark_rapids_pytools/rapids/rapids_job.py,sha256=w7D5jZPCsyb7PqupPfQ02bNnOYAwld7RLMHXqoovUTs,6864
 spark_rapids_pytools/rapids/rapids_tool.py,sha256=3USqFAQRUDKDtsBHUqQSP-EQHp-71USzcYKlmciZh3w,33590
 spark_rapids_pytools/rapids/tool_ctxt.py,sha256=8bWqooTKcIH5ShxTFrXPuSr1KEJeHXU5LdDq8F6ienU,6576
 spark_rapids_pytools/resources/bootstrap-conf.yaml,sha256=xATXdInBA2NFR2Le9uqioRwyqYB7TnFBYvoaT8NEDZQ,1390
+spark_rapids_pytools/resources/collect.sh,sha256=EdbNF90ZQUgaERPYY1p3fYdf3qvmU9f2WGD7RzYoLOE,4453
 spark_rapids_pytools/resources/databricks-premium-catalog.json,sha256=XBptMDeu7Abbrv6xC4C1oDuMuEIqnrGEqwrhJFutLJM,30566
 spark_rapids_pytools/resources/databricks_aws-configs.json,sha256=I_VqLdvavbQGUqCNcUqMpNrH5aF0xBZDdN7kuncNKQk,10448
 spark_rapids_pytools/resources/databricks_azure-configs.json,sha256=TSo17t28bRfeAjSWDZR4KqMhEUKoLzoqO5YknfiokYA,10017
 spark_rapids_pytools/resources/dataproc-configs.json,sha256=9rEXtuCKsLUMyoRsKAeW2OWckM1AXYsE3JuNjFAYmWA,8047
 spark_rapids_pytools/resources/diagnostic-conf.yaml,sha256=vS32UyRhj5ox2MZ8-6EgMjXEWlGeaw9izYiAdAoWpfE,30
 spark_rapids_pytools/resources/emr-configs.json,sha256=_F5XxM5kFen_iCAWW5Z_jdD6G626h4hH_Uf2dq2Dn6U,8994
 spark_rapids_pytools/resources/onprem-configs.json,sha256=TWqp95Ildys0-eGOrWNL-KpUqTTLVHLqzW4u48eNmhM,4727
 spark_rapids_pytools/resources/premium-databricks-azure-catalog.json,sha256=KGxUoiNPVTVzQaR3SN_FV9PH80fEnp6JnMhnv2YFOBY,38903
 spark_rapids_pytools/resources/profiling-conf.yaml,sha256=s7TR1agVORA4g28bYYK7jSMpgMT6s-awMySK0jT4kaA,1460
 spark_rapids_pytools/resources/qualification-conf.yaml,sha256=FwQGa9cFXQbEutN9aGb9IEzgRFdHTC7fP_QYTrFWmyc,4273
+spark_rapids_pytools/resources/dev/process_databricks_azure_pricing.py,sha256=lmXGoTdrwdrhh8UO7DSL-kgbLOJP1X0kgJPq6cJfF3U,2195
 spark_rapids_pytools/resources/templates/dataproc-create_gpu_cluster_script.ms,sha256=pigL0kAsg1VaP9Jn9-5oNblJRj0IbeZLh1T5Op8CQqA,671
 spark_rapids_pytools/resources/templates/dataproc-run_bootstrap.ms,sha256=lmnyouNCpbytpRVZ_YbQ6d6hCl3XaYxqzNomxSJwSSk,518
 spark_rapids_pytools/resources/templates/emr-create_gpu_cluster_script.ms,sha256=UIlW0GcYn2fovtcDNYPUmg99h0zKy-DxXGO-1Lr_xQs,855
 spark_rapids_pytools/resources/templates/emr-run_bootstrap.ms,sha256=7xqXBMIu5Tg02KCq_YN9oLLiE3c8jgWl8BUvFQZODhs,537
 spark_rapids_pytools/wrappers/__init__.py,sha256=CQ7Mf-YyBFNl6xmQGsPARv1w5GU3jGliByn5IHCcLkE,630
-spark_rapids_pytools/wrappers/databricks_aws_wrapper.py,sha256=FPuw9pnU8huyRfeGYGc9xljYe9xf9cSsuEg0iaHBYtE,8104
+spark_rapids_pytools/wrappers/databricks_aws_wrapper.py,sha256=-axS_C8sb3RvlOByfk6ZqYQvOSJ36GJwk4zwqiZ-t-c,13207
 spark_rapids_pytools/wrappers/databricks_azure_wrapper.py,sha256=5NElNnmmGg7v8WuFgraCAR1qX6X7w3N-NPwe7ypXi3o,7985
-spark_rapids_pytools/wrappers/dataproc_wrapper.py,sha256=L0gHQnHiO-5FPe2-ovHR1of0WGIyMzy0D2gYpyU-20E,16140
-spark_rapids_pytools/wrappers/emr_wrapper.py,sha256=fCYVPKnGxpQCZx4oz_NN-WawrXl5W69KVppMTQkhsHQ,17649
+spark_rapids_pytools/wrappers/dataproc_wrapper.py,sha256=96wdNER9NZVv8N0-YElje6pYuNUt2Oz_WpJ4fdLKnoE,16647
+spark_rapids_pytools/wrappers/emr_wrapper.py,sha256=v8bw3qDWc5vzrW8s6MWCl3uHv4H2423H8E-3G2x7dPI,18151
 spark_rapids_pytools/wrappers/onprem_wrapper.py,sha256=KFZrSMjk4xTLWC8lEhnD1ms1bZ75Sch0yLRL9swKULM,4480
-spark_rapids_user_tools-23.6.0.dist-info/LICENSE,sha256=RnI8IUCDrXfGVHFfYTsT8OKEuaOtkMGDQOn8foh7D00,21086
-spark_rapids_user_tools-23.6.0.dist-info/METADATA,sha256=DYBTM4x4PGdcxdS_QCsbT528z1jBQfQocqjcRnGZbgw,2939
-spark_rapids_user_tools-23.6.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-spark_rapids_user_tools-23.6.0.dist-info/entry_points.txt,sha256=OQT0O5JpYFfCtexjgM31__xoCugCT1eHZ9PDT-xq054,152
-spark_rapids_user_tools-23.6.0.dist-info/top_level.txt,sha256=u2CXaBsgoZoiL8XafMeC-8ITnOTUn7Bwrmz8fPjwjio,49
-spark_rapids_user_tools-23.6.0.dist-info/RECORD,,
+spark_rapids_user_tools-23.6.1.dist-info/LICENSE,sha256=RnI8IUCDrXfGVHFfYTsT8OKEuaOtkMGDQOn8foh7D00,21086
+spark_rapids_user_tools-23.6.1.dist-info/METADATA,sha256=LwgOAl_HA7lfnvfMBhFCuvxxfEGp4inf9aP4Wq3nygE,2927
+spark_rapids_user_tools-23.6.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+spark_rapids_user_tools-23.6.1.dist-info/entry_points.txt,sha256=GyaV1NES81c2p204FZjglRxwrzsI2yVmCtL5cUI4rZc,78
+spark_rapids_user_tools-23.6.1.dist-info/top_level.txt,sha256=47ZJrA6QPYYeI7JxABL1bTLJ7H9haiGWrN-6jVLYOXU,21
+spark_rapids_user_tools-23.6.1.dist-info/RECORD,,
```

