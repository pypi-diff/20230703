# Comparing `tmp/mpyl-1.0.6-py3-none-any.whl.zip` & `tmp/mpyl-1.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,90 +1,91 @@
-Zip file size: 133968 bytes, number of entries: 88
--rw-r--r--  2.0 unx      766 b- defN 23-Jun-23 12:50 mpyl/__init__.py
--rw-r--r--  2.0 unx      215 b- defN 23-Jun-23 12:50 mpyl/__main__.py
--rw-r--r--  2.0 unx      162 b- defN 23-Jun-23 12:50 mpyl/constants.py
--rw-r--r--  2.0 unx    13526 b- defN 23-Jun-23 12:50 mpyl/project.py
--rw-r--r--  2.0 unx     1708 b- defN 23-Jun-23 12:50 mpyl/validation.py
--rw-r--r--  2.0 unx     2163 b- defN 23-Jun-23 12:50 mpyl/cli/__init__.py
--rw-r--r--  2.0 unx    10619 b- defN 23-Jun-23 12:50 mpyl/cli/build.py
--rw-r--r--  2.0 unx      341 b- defN 23-Jun-23 12:50 mpyl/cli/health.py
--rw-r--r--  2.0 unx     2170 b- defN 23-Jun-23 12:50 mpyl/cli/meta_info.py
--rw-r--r--  2.0 unx     3915 b- defN 23-Jun-23 12:50 mpyl/cli/projects.py
--rw-r--r--  2.0 unx       34 b- defN 23-Jun-23 12:50 mpyl/cli/commands/__init__.py
--rw-r--r--  2.0 unx      439 b- defN 23-Jun-23 12:50 mpyl/cli/commands/build/__init__.py
--rw-r--r--  2.0 unx     3923 b- defN 23-Jun-23 12:50 mpyl/cli/commands/build/jenkins.py
--rw-r--r--  2.0 unx     5814 b- defN 23-Jun-23 12:50 mpyl/cli/commands/build/mpyl.py
--rw-r--r--  2.0 unx       38 b- defN 23-Jun-23 12:50 mpyl/cli/commands/health/__init__.py
--rw-r--r--  2.0 unx     5200 b- defN 23-Jun-23 12:50 mpyl/cli/commands/health/checks.py
--rw-r--r--  2.0 unx       46 b- defN 23-Jun-23 12:50 mpyl/cli/commands/projects/__init__.py
--rw-r--r--  2.0 unx     1039 b- defN 23-Jun-23 12:50 mpyl/cli/commands/projects/formatting.py
--rw-r--r--  2.0 unx      620 b- defN 23-Jun-23 12:50 mpyl/projects/__init__.py
--rw-r--r--  2.0 unx     1993 b- defN 23-Jun-23 12:50 mpyl/projects/find.py
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-23 12:50 mpyl/reporting/__init__.py
--rw-r--r--  2.0 unx       76 b- defN 23-Jun-23 12:50 mpyl/reporting/formatting/__init__.py
--rw-r--r--  2.0 unx     4909 b- defN 23-Jun-23 12:50 mpyl/reporting/formatting/markdown.py
--rw-r--r--  2.0 unx     1413 b- defN 23-Jun-23 12:50 mpyl/reporting/formatting/text.py
--rw-r--r--  2.0 unx     1096 b- defN 23-Jun-23 12:50 mpyl/reporting/targets/__init__.py
--rw-r--r--  2.0 unx     7939 b- defN 23-Jun-23 12:50 mpyl/reporting/targets/github.py
--rw-r--r--  2.0 unx     9004 b- defN 23-Jun-23 12:50 mpyl/reporting/targets/jira.py
--rw-r--r--  2.0 unx     7366 b- defN 23-Jun-23 12:50 mpyl/reporting/targets/slack.py
--rw-r--r--  2.0 unx     8433 b- defN 23-Jun-23 12:50 mpyl/schema/mpyl_config.schema.yml
--rw-r--r--  2.0 unx    25500 b- defN 23-Jun-23 12:50 mpyl/schema/project.schema.yml
--rw-r--r--  2.0 unx     2787 b- defN 23-Jun-23 12:50 mpyl/schema/run_properties.schema.yml
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-23 12:50 mpyl/stages/__init__.py
--rw-r--r--  2.0 unx     3506 b- defN 23-Jun-23 12:50 mpyl/stages/discovery.py
--rw-r--r--  2.0 unx     6135 b- defN 23-Jun-23 12:50 mpyl/steps/__init__.py
--rw-r--r--  2.0 unx     5977 b- defN 23-Jun-23 12:50 mpyl/steps/models.py
--rw-r--r--  2.0 unx     3429 b- defN 23-Jun-23 12:50 mpyl/steps/run.py
--rw-r--r--  2.0 unx     8405 b- defN 23-Jun-23 12:50 mpyl/steps/steps.py
--rw-r--r--  2.0 unx       59 b- defN 23-Jun-23 12:50 mpyl/steps/build/__init__.py
--rw-r--r--  2.0 unx     2093 b- defN 23-Jun-23 12:50 mpyl/steps/build/docker_after_build.py
--rw-r--r--  2.0 unx     2865 b- defN 23-Jun-23 12:50 mpyl/steps/build/dockerbuild.py
--rw-r--r--  2.0 unx      765 b- defN 23-Jun-23 12:50 mpyl/steps/build/echo.py
--rw-r--r--  2.0 unx     2402 b- defN 23-Jun-23 12:50 mpyl/steps/build/sbt.py
--rw-r--r--  2.0 unx       60 b- defN 23-Jun-23 12:50 mpyl/steps/deploy/__init__.py
--rw-r--r--  2.0 unx     2496 b- defN 23-Jun-23 12:50 mpyl/steps/deploy/cloudfront_kubernetes_deploy.py
--rw-r--r--  2.0 unx     1001 b- defN 23-Jun-23 12:50 mpyl/steps/deploy/echo.py
--rw-r--r--  2.0 unx     1310 b- defN 23-Jun-23 12:50 mpyl/steps/deploy/ephemeral_docker_deploy.py
--rw-r--r--  2.0 unx     3415 b- defN 23-Jun-23 12:50 mpyl/steps/deploy/kubernetes.py
--rw-r--r--  2.0 unx     1412 b- defN 23-Jun-23 12:50 mpyl/steps/deploy/kubernetes_job.py
--rw-r--r--  2.0 unx     1380 b- defN 23-Jun-23 12:50 mpyl/steps/deploy/kubernetes_spark_job.py
--rw-r--r--  2.0 unx     3390 b- defN 23-Jun-23 12:50 mpyl/steps/deploy/k8s/__init__.py
--rw-r--r--  2.0 unx    18819 b- defN 23-Jun-23 12:50 mpyl/steps/deploy/k8s/chart.py
--rw-r--r--  2.0 unx     2856 b- defN 23-Jun-23 12:50 mpyl/steps/deploy/k8s/helm.py
--rw-r--r--  2.0 unx     1685 b- defN 23-Jun-23 12:50 mpyl/steps/deploy/k8s/rancher.py
--rw-r--r--  2.0 unx     4467 b- defN 23-Jun-23 12:50 mpyl/steps/deploy/k8s/resources/__init__.py
--rw-r--r--  2.0 unx      591 b- defN 23-Jun-23 12:50 mpyl/steps/deploy/k8s/resources/sealed_secret.py
--rw-r--r--  2.0 unx     6143 b- defN 23-Jun-23 12:50 mpyl/steps/deploy/k8s/resources/spark.py
--rw-r--r--  2.0 unx     1948 b- defN 23-Jun-23 12:50 mpyl/steps/deploy/k8s/resources/traefik.py
--rw-r--r--  2.0 unx   168371 b- defN 23-Jun-23 12:50 mpyl/steps/deploy/k8s/resources/schema/sparkoperator.k8s.io_scheduledsparkapplications.schema.yml
--rw-r--r--  2.0 unx   151469 b- defN 23-Jun-23 12:50 mpyl/steps/deploy/k8s/resources/schema/sparkoperator.k8s.io_sparkapplications.schema.yml
--rw-r--r--  2.0 unx    11703 b- defN 23-Jun-23 12:50 mpyl/steps/deploy/k8s/resources/schema/traefik.ingress.schema.yml
--rw-r--r--  2.0 unx    42950 b- defN 23-Jun-23 12:50 mpyl/steps/deploy/k8s/resources/schema/traefik.middleware.schema.yml
--rw-r--r--  2.0 unx       64 b- defN 23-Jun-23 12:50 mpyl/steps/postdeploy/__init__.py
--rw-r--r--  2.0 unx     6004 b- defN 23-Jun-23 12:50 mpyl/steps/postdeploy/cypress_test.py
--rw-r--r--  2.0 unx       58 b- defN 23-Jun-23 12:50 mpyl/steps/test/__init__.py
--rw-r--r--  2.0 unx     1428 b- defN 23-Jun-23 12:50 mpyl/steps/test/after_test.py
--rw-r--r--  2.0 unx     2453 b- defN 23-Jun-23 12:50 mpyl/steps/test/before_test.py
--rw-r--r--  2.0 unx     3609 b- defN 23-Jun-23 12:50 mpyl/steps/test/dockertest.py
--rw-r--r--  2.0 unx     1789 b- defN 23-Jun-23 12:50 mpyl/steps/test/echo.py
--rw-r--r--  2.0 unx     5013 b- defN 23-Jun-23 12:50 mpyl/steps/test/sbt.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-23 12:50 mpyl/utilities/__init__.py
--rw-r--r--  2.0 unx      749 b- defN 23-Jun-23 12:50 mpyl/utilities/cypress/__init__.py
--rw-r--r--  2.0 unx     6470 b- defN 23-Jun-23 12:50 mpyl/utilities/docker/__init__.py
--rw-r--r--  2.0 unx     1739 b- defN 23-Jun-23 12:50 mpyl/utilities/github/__init__.py
--rw-r--r--  2.0 unx     1533 b- defN 23-Jun-23 12:50 mpyl/utilities/jenkins/__init__.py
--rw-r--r--  2.0 unx     7627 b- defN 23-Jun-23 12:50 mpyl/utilities/jenkins/runner.py
--rw-r--r--  2.0 unx     1382 b- defN 23-Jun-23 12:50 mpyl/utilities/junit/__init__.py
--rw-r--r--  2.0 unx      254 b- defN 23-Jun-23 12:50 mpyl/utilities/logging/__init__.py
--rw-r--r--  2.0 unx      847 b- defN 23-Jun-23 12:50 mpyl/utilities/pyaml_env/__init__.py
--rw-r--r--  2.0 unx     6568 b- defN 23-Jun-23 12:50 mpyl/utilities/repo/__init__.py
--rw-r--r--  2.0 unx     4622 b- defN 23-Jun-23 12:50 mpyl/utilities/s3/__init__.py
--rw-r--r--  2.0 unx     1551 b- defN 23-Jun-23 12:50 mpyl/utilities/sbt/__init__.py
--rw-r--r--  2.0 unx     2110 b- defN 23-Jun-23 12:50 mpyl/utilities/subprocess/__init__.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jun-23 12:52 mpyl-1.0.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     5945 b- defN 23-Jun-23 12:52 mpyl-1.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-23 12:52 mpyl-1.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       35 b- defN 23-Jun-23 12:51 mpyl-1.0.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 23-Jun-23 12:51 mpyl-1.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     7763 b- defN 23-Jun-23 12:52 mpyl-1.0.6.dist-info/RECORD
-88 files, 665515 bytes uncompressed, 121594 bytes compressed:  81.7%
+Zip file size: 136020 bytes, number of entries: 89
+-rw-r--r--  2.0 unx      766 b- defN 23-Jul-03 10:09 mpyl/__init__.py
+-rw-r--r--  2.0 unx      215 b- defN 23-Jul-03 10:09 mpyl/__main__.py
+-rw-r--r--  2.0 unx      162 b- defN 23-Jul-03 10:09 mpyl/constants.py
+-rw-r--r--  2.0 unx    13948 b- defN 23-Jul-03 10:09 mpyl/project.py
+-rw-r--r--  2.0 unx     1710 b- defN 23-Jul-03 10:09 mpyl/validation.py
+-rw-r--r--  2.0 unx     2789 b- defN 23-Jul-03 10:09 mpyl/cli/__init__.py
+-rw-r--r--  2.0 unx    11043 b- defN 23-Jul-03 10:09 mpyl/cli/build.py
+-rw-r--r--  2.0 unx      341 b- defN 23-Jul-03 10:09 mpyl/cli/health.py
+-rw-r--r--  2.0 unx     2170 b- defN 23-Jul-03 10:09 mpyl/cli/meta_info.py
+-rw-r--r--  2.0 unx     3853 b- defN 23-Jul-03 10:09 mpyl/cli/projects.py
+-rw-r--r--  2.0 unx       34 b- defN 23-Jul-03 10:09 mpyl/cli/commands/__init__.py
+-rw-r--r--  2.0 unx      439 b- defN 23-Jul-03 10:09 mpyl/cli/commands/build/__init__.py
+-rw-r--r--  2.0 unx     3923 b- defN 23-Jul-03 10:09 mpyl/cli/commands/build/jenkins.py
+-rw-r--r--  2.0 unx     5901 b- defN 23-Jul-03 10:09 mpyl/cli/commands/build/mpyl.py
+-rw-r--r--  2.0 unx       38 b- defN 23-Jul-03 10:09 mpyl/cli/commands/health/__init__.py
+-rw-r--r--  2.0 unx     5535 b- defN 23-Jul-03 10:09 mpyl/cli/commands/health/checks.py
+-rw-r--r--  2.0 unx       46 b- defN 23-Jul-03 10:09 mpyl/cli/commands/projects/__init__.py
+-rw-r--r--  2.0 unx     1061 b- defN 23-Jul-03 10:09 mpyl/cli/commands/projects/formatting.py
+-rw-r--r--  2.0 unx      620 b- defN 23-Jul-03 10:09 mpyl/projects/__init__.py
+-rw-r--r--  2.0 unx     2202 b- defN 23-Jul-03 10:09 mpyl/projects/find.py
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-03 10:09 mpyl/reporting/__init__.py
+-rw-r--r--  2.0 unx       76 b- defN 23-Jul-03 10:09 mpyl/reporting/formatting/__init__.py
+-rw-r--r--  2.0 unx     5213 b- defN 23-Jul-03 10:09 mpyl/reporting/formatting/markdown.py
+-rw-r--r--  2.0 unx     1411 b- defN 23-Jul-03 10:09 mpyl/reporting/formatting/text.py
+-rw-r--r--  2.0 unx     1139 b- defN 23-Jul-03 10:09 mpyl/reporting/targets/__init__.py
+-rw-r--r--  2.0 unx     8453 b- defN 23-Jul-03 10:09 mpyl/reporting/targets/github.py
+-rw-r--r--  2.0 unx     9331 b- defN 23-Jul-03 10:09 mpyl/reporting/targets/jira.py
+-rw-r--r--  2.0 unx     7997 b- defN 23-Jul-03 10:09 mpyl/reporting/targets/slack.py
+-rw-r--r--  2.0 unx     8433 b- defN 23-Jul-03 10:09 mpyl/schema/mpyl_config.schema.yml
+-rw-r--r--  2.0 unx    25500 b- defN 23-Jul-03 10:09 mpyl/schema/project.schema.yml
+-rw-r--r--  2.0 unx     2914 b- defN 23-Jul-03 10:09 mpyl/schema/run_properties.schema.yml
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-03 10:09 mpyl/stages/__init__.py
+-rw-r--r--  2.0 unx     3698 b- defN 23-Jul-03 10:09 mpyl/stages/discovery.py
+-rw-r--r--  2.0 unx     6437 b- defN 23-Jul-03 10:09 mpyl/steps/__init__.py
+-rw-r--r--  2.0 unx     1442 b- defN 23-Jul-03 10:09 mpyl/steps/collection.py
+-rw-r--r--  2.0 unx     6085 b- defN 23-Jul-03 10:09 mpyl/steps/models.py
+-rw-r--r--  2.0 unx     3505 b- defN 23-Jul-03 10:09 mpyl/steps/run.py
+-rw-r--r--  2.0 unx     7278 b- defN 23-Jul-03 10:09 mpyl/steps/steps.py
+-rw-r--r--  2.0 unx       59 b- defN 23-Jul-03 10:09 mpyl/steps/build/__init__.py
+-rw-r--r--  2.0 unx     2093 b- defN 23-Jul-03 10:09 mpyl/steps/build/docker_after_build.py
+-rw-r--r--  2.0 unx     2865 b- defN 23-Jul-03 10:09 mpyl/steps/build/dockerbuild.py
+-rw-r--r--  2.0 unx      996 b- defN 23-Jul-03 10:09 mpyl/steps/build/echo.py
+-rw-r--r--  2.0 unx     2402 b- defN 23-Jul-03 10:09 mpyl/steps/build/sbt.py
+-rw-r--r--  2.0 unx       60 b- defN 23-Jul-03 10:09 mpyl/steps/deploy/__init__.py
+-rw-r--r--  2.0 unx     2767 b- defN 23-Jul-03 10:09 mpyl/steps/deploy/cloudfront_kubernetes_deploy.py
+-rw-r--r--  2.0 unx     1196 b- defN 23-Jul-03 10:09 mpyl/steps/deploy/echo.py
+-rw-r--r--  2.0 unx     1472 b- defN 23-Jul-03 10:09 mpyl/steps/deploy/ephemeral_docker_deploy.py
+-rw-r--r--  2.0 unx     3896 b- defN 23-Jul-03 10:09 mpyl/steps/deploy/kubernetes.py
+-rw-r--r--  2.0 unx     1588 b- defN 23-Jul-03 10:09 mpyl/steps/deploy/kubernetes_job.py
+-rw-r--r--  2.0 unx     1571 b- defN 23-Jul-03 10:09 mpyl/steps/deploy/kubernetes_spark_job.py
+-rw-r--r--  2.0 unx     3518 b- defN 23-Jul-03 10:09 mpyl/steps/deploy/k8s/__init__.py
+-rw-r--r--  2.0 unx    20536 b- defN 23-Jul-03 10:09 mpyl/steps/deploy/k8s/chart.py
+-rw-r--r--  2.0 unx     2989 b- defN 23-Jul-03 10:09 mpyl/steps/deploy/k8s/helm.py
+-rw-r--r--  2.0 unx     1732 b- defN 23-Jul-03 10:09 mpyl/steps/deploy/k8s/rancher.py
+-rw-r--r--  2.0 unx     4719 b- defN 23-Jul-03 10:09 mpyl/steps/deploy/k8s/resources/__init__.py
+-rw-r--r--  2.0 unx      616 b- defN 23-Jul-03 10:09 mpyl/steps/deploy/k8s/resources/sealed_secret.py
+-rw-r--r--  2.0 unx     5850 b- defN 23-Jul-03 10:09 mpyl/steps/deploy/k8s/resources/spark.py
+-rw-r--r--  2.0 unx     2287 b- defN 23-Jul-03 10:09 mpyl/steps/deploy/k8s/resources/traefik.py
+-rw-r--r--  2.0 unx   168371 b- defN 23-Jul-03 10:09 mpyl/steps/deploy/k8s/resources/schema/sparkoperator.k8s.io_scheduledsparkapplications.schema.yml
+-rw-r--r--  2.0 unx   151469 b- defN 23-Jul-03 10:09 mpyl/steps/deploy/k8s/resources/schema/sparkoperator.k8s.io_sparkapplications.schema.yml
+-rw-r--r--  2.0 unx    11703 b- defN 23-Jul-03 10:09 mpyl/steps/deploy/k8s/resources/schema/traefik.ingress.schema.yml
+-rw-r--r--  2.0 unx    42950 b- defN 23-Jul-03 10:09 mpyl/steps/deploy/k8s/resources/schema/traefik.middleware.schema.yml
+-rw-r--r--  2.0 unx       64 b- defN 23-Jul-03 10:09 mpyl/steps/postdeploy/__init__.py
+-rw-r--r--  2.0 unx     6496 b- defN 23-Jul-03 10:09 mpyl/steps/postdeploy/cypress_test.py
+-rw-r--r--  2.0 unx       58 b- defN 23-Jul-03 10:09 mpyl/steps/test/__init__.py
+-rw-r--r--  2.0 unx     1560 b- defN 23-Jul-03 10:09 mpyl/steps/test/after_test.py
+-rw-r--r--  2.0 unx     2596 b- defN 23-Jul-03 10:09 mpyl/steps/test/before_test.py
+-rw-r--r--  2.0 unx     3886 b- defN 23-Jul-03 10:09 mpyl/steps/test/dockertest.py
+-rw-r--r--  2.0 unx     1929 b- defN 23-Jul-03 10:09 mpyl/steps/test/echo.py
+-rw-r--r--  2.0 unx     5075 b- defN 23-Jul-03 10:09 mpyl/steps/test/sbt.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-03 10:09 mpyl/utilities/__init__.py
+-rw-r--r--  2.0 unx      768 b- defN 23-Jul-03 10:09 mpyl/utilities/cypress/__init__.py
+-rw-r--r--  2.0 unx     6693 b- defN 23-Jul-03 10:09 mpyl/utilities/docker/__init__.py
+-rw-r--r--  2.0 unx     1781 b- defN 23-Jul-03 10:09 mpyl/utilities/github/__init__.py
+-rw-r--r--  2.0 unx     1551 b- defN 23-Jul-03 10:09 mpyl/utilities/jenkins/__init__.py
+-rw-r--r--  2.0 unx     7903 b- defN 23-Jul-03 10:09 mpyl/utilities/jenkins/runner.py
+-rw-r--r--  2.0 unx     1431 b- defN 23-Jul-03 10:09 mpyl/utilities/junit/__init__.py
+-rw-r--r--  2.0 unx      254 b- defN 23-Jul-03 10:09 mpyl/utilities/logging/__init__.py
+-rw-r--r--  2.0 unx      880 b- defN 23-Jul-03 10:09 mpyl/utilities/pyaml_env/__init__.py
+-rw-r--r--  2.0 unx     7098 b- defN 23-Jul-03 10:09 mpyl/utilities/repo/__init__.py
+-rw-r--r--  2.0 unx     4764 b- defN 23-Jul-03 10:09 mpyl/utilities/s3/__init__.py
+-rw-r--r--  2.0 unx     1612 b- defN 23-Jul-03 10:09 mpyl/utilities/sbt/__init__.py
+-rw-r--r--  2.0 unx     2326 b- defN 23-Jul-03 10:09 mpyl/utilities/subprocess/__init__.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-03 10:10 mpyl-1.0.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6083 b- defN 23-Jul-03 10:10 mpyl-1.0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-03 10:10 mpyl-1.0.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       35 b- defN 23-Jul-03 10:10 mpyl-1.0.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 23-Jul-03 10:10 mpyl-1.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     7844 b- defN 23-Jul-03 10:10 mpyl-1.0.7.dist-info/RECORD
+89 files, 677646 bytes uncompressed, 123522 bytes compressed:  81.8%
```

## zipnote {}

```diff
@@ -96,14 +96,17 @@
 
 Filename: mpyl/stages/discovery.py
 Comment: 
 
 Filename: mpyl/steps/__init__.py
 Comment: 
 
+Filename: mpyl/steps/collection.py
+Comment: 
+
 Filename: mpyl/steps/models.py
 Comment: 
 
 Filename: mpyl/steps/run.py
 Comment: 
 
 Filename: mpyl/steps/steps.py
@@ -240,26 +243,26 @@
 
 Filename: mpyl/utilities/sbt/__init__.py
 Comment: 
 
 Filename: mpyl/utilities/subprocess/__init__.py
 Comment: 
 
-Filename: mpyl-1.0.6.dist-info/LICENSE
+Filename: mpyl-1.0.7.dist-info/LICENSE
 Comment: 
 
-Filename: mpyl-1.0.6.dist-info/METADATA
+Filename: mpyl-1.0.7.dist-info/METADATA
 Comment: 
 
-Filename: mpyl-1.0.6.dist-info/WHEEL
+Filename: mpyl-1.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: mpyl-1.0.6.dist-info/entry_points.txt
+Filename: mpyl-1.0.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: mpyl-1.0.6.dist-info/top_level.txt
+Filename: mpyl-1.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: mpyl-1.0.6.dist-info/RECORD
+Filename: mpyl-1.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mpyl/__init__.py

```diff
@@ -13,15 +13,15 @@
 from .cli.meta_info import get_version
 from .cli.meta_info import version
 from .cli.projects import projects
 from .utilities.pyaml_env import parse_config
 from .utilities.repo import RepoConfig, Repository
 
 
-@click.group(name='mpyl')
+@click.group(name="mpyl")
 def main_group():
     """Command Line Interface for MPyL"""
 
 
 def main():
     main_group.help = f"Command Line Interface for MPyL {get_version()}"
     main_group.add_command(projects)
```

## mpyl/__main__.py

```diff
@@ -1,9 +1,9 @@
 """Entrypoint for cli"""
 
-if __name__ == '__main__' and __package__ is None:
+if __name__ == "__main__" and __package__ is None:
     # https://peps.python.org/pep-0366/
     __package__ = "mpyl"  # pylint: disable=redefined-builtin
 
     from . import main
 
     main()
```

## mpyl/constants.py

```diff
@@ -1,5 +1,5 @@
 """"Constants for mpyl."""
 
-BUILD_ARTIFACTS_FOLDER = '.mpyl'
-DEFAULT_CONFIG_FILE_NAME = 'mpyl_config.yml'
-DEFAULT_RUN_PROPERTIES_FILE_NAME = 'run_properties.yml'
+BUILD_ARTIFACTS_FOLDER = ".mpyl"
+DEFAULT_CONFIG_FILE_NAME = "mpyl_config.yml"
+DEFAULT_RUN_PROPERTIES_FILE_NAME = "run_properties.yml"
```

## mpyl/project.py

```diff
@@ -25,44 +25,44 @@
 import jsonschema
 from mypy.checker import Generic
 from ruamel.yaml import YAML
 
 from .constants import BUILD_ARTIFACTS_FOLDER
 from .validation import validate
 
-T = TypeVar('T')
+T = TypeVar("T")
 
 
 def without_keys(dictionary: dict, keys: set[str]):
     return {k: dictionary[k] for k in dictionary.keys() - keys}
 
 
 @dataclass(frozen=True)
 class Target(Enum):
     def __eq__(self, other):
         return self.value == other.value
 
     def __str__(self):
         return str(self.value)
 
-    PULL_REQUEST = 'PullRequest'
-    PULL_REQUEST_BASE = 'PullRequestBase'
-    ACCEPTANCE = 'Acceptance'
-    PRODUCTION = 'Production'
+    PULL_REQUEST = "PullRequest"
+    PULL_REQUEST_BASE = "PullRequestBase"
+    ACCEPTANCE = "Acceptance"
+    PRODUCTION = "Production"
 
 
 @dataclass(frozen=True)
 class Stage(Enum):
     def __eq__(self, other):
         return self.value == other.value
 
-    BUILD = 'build'
-    TEST = 'test'
-    DEPLOY = 'deploy'
-    POST_DEPLOY = 'postdeploy'
+    BUILD = "build"
+    TEST = "test"
+    DEPLOY = "deploy"
+    POST_DEPLOY = "postdeploy"
 
 
 @dataclass(frozen=True)
 class TargetProperty(Generic[T]):
     pr: Optional[T]  # pylint: disable=invalid-name
     test: Optional[T]
     acceptance: Optional[T]
@@ -82,27 +82,37 @@
             return self.production
         return None
 
     @staticmethod
     def from_config(values: dict):
         if not values:
             return None
-        return TargetProperty(pr=values.get('pr'), test=values.get('test'), acceptance=values.get('acceptance'),
-                              production=values.get('production'), all=values.get('all'))
+        return TargetProperty(
+            pr=values.get("pr"),
+            test=values.get("test"),
+            acceptance=values.get("acceptance"),
+            production=values.get("production"),
+            all=values.get("all"),
+        )
 
 
 @dataclass(frozen=True)
 class KeyValueProperty(TargetProperty[str]):
     key: str
 
     @staticmethod
     def from_config(values: dict):
-        return KeyValueProperty(key=values['key'], pr=values.get('pr'), test=values.get('test'),
-                                acceptance=values.get('acceptance'), production=values.get('production'),
-                                all=values.get('all'))
+        return KeyValueProperty(
+            key=values["key"],
+            pr=values.get("pr"),
+            test=values.get("test"),
+            acceptance=values.get("acceptance"),
+            production=values.get("production"),
+            all=values.get("all"),
+        )
 
 
 @dataclass(frozen=True)
 class StageSpecificProperty(Generic[T]):
     build: Optional[T]
     test: Optional[T]
     deploy: Optional[T]
@@ -116,32 +126,38 @@
         if stage == Stage.DEPLOY:
             return self.deploy
         return self.postdeploy
 
 
 @dataclass(frozen=True)
 class Stages(StageSpecificProperty[str]):
-
     @staticmethod
     def from_config(values: dict):
-        return Stages(build=values.get('build'), test=values.get('test'), deploy=values.get('deploy'),
-                      postdeploy=values.get('postdeploy'))
+        return Stages(
+            build=values.get("build"),
+            test=values.get("test"),
+            deploy=values.get("deploy"),
+            postdeploy=values.get("postdeploy"),
+        )
 
 
 @dataclass(frozen=True)
 class Dependencies(StageSpecificProperty[set[str]]):
-
     def set_for_stage(self, stage: Stage) -> set[str]:
         deps_for_stage = self.for_stage(stage)
         return deps_for_stage if deps_for_stage else set()
 
     @staticmethod
     def from_config(values: dict):
-        return Dependencies(build=set(values.get('build', [])), test=set(values.get('test', [])),
-                            deploy=set(values.get('deploy', [])), postdeploy=set(values.get('postdeploy', [])))
+        return Dependencies(
+            build=set(values.get("build", [])),
+            test=set(values.get("test", [])),
+            deploy=set(values.get("deploy", [])),
+            postdeploy=set(values.get("postdeploy", [])),
+        )
 
 
 @dataclass(frozen=True)
 class Env:
     @staticmethod
     def from_config(values: list[dict]):
         return list(map(KeyValueProperty.from_config, values))
@@ -150,151 +166,162 @@
 @dataclass(frozen=True)
 class Properties:
     env: list[KeyValueProperty]
     sealed_secret: list[KeyValueProperty]
 
     @staticmethod
     def from_config(values: Dict[Any, Any]):
-        return Properties(env=list(map(KeyValueProperty.from_config, values.get('env', []))),
-                          sealed_secret=list(
-                              map(KeyValueProperty.from_config, values.get('sealedSecret', []))))
+        return Properties(
+            env=list(map(KeyValueProperty.from_config, values.get("env", []))),
+            sealed_secret=list(
+                map(KeyValueProperty.from_config, values.get("sealedSecret", []))
+            ),
+        )
 
 
 @dataclass(frozen=True)
 class Probe:
     path: TargetProperty[str]
     values: dict
 
     @staticmethod
     def from_config(values: dict):
         if not values:
             return None
-        return Probe(path=TargetProperty.from_config(values['path']), values=values)
+        return Probe(path=TargetProperty.from_config(values["path"]), values=values)
 
 
 @dataclass(frozen=True)
 class Metrics:
     path: str
     enabled: bool
 
     @staticmethod
     def from_config(values: dict):
         if not values:
             return None
-        return Metrics(path=values.get('path', '/metrics'), enabled=values.get('enabled', False))
+        return Metrics(
+            path=values.get("path", "/metrics"), enabled=values.get("enabled", False)
+        )
 
 
 @dataclass(frozen=True)
 class Resources:
     instances: Optional[TargetProperty[int]]
     cpus: Optional[TargetProperty[float]]
     mem: Optional[TargetProperty[int]]
     disk: Optional[TargetProperty[int]]
 
     @staticmethod
     def from_config(values: dict):
-        limits = values.get('limit', {})
+        limits = values.get("limit", {})
         return Resources(
-            instances=TargetProperty.from_config(limits.get('instances', {})),
-            cpus=TargetProperty.from_config(limits.get('cpus', {})),
-            mem=TargetProperty.from_config(limits.get('mem', {})),
-            disk=TargetProperty.from_config(limits.get('disk', {}))
+            instances=TargetProperty.from_config(limits.get("instances", {})),
+            cpus=TargetProperty.from_config(limits.get("cpus", {})),
+            mem=TargetProperty.from_config(limits.get("mem", {})),
+            disk=TargetProperty.from_config(limits.get("disk", {})),
         )
 
 
 @dataclass(frozen=True)
 class Job:
     cron: dict
     job: dict
     spark: dict
 
     @staticmethod
     def from_config(values: dict):
         if not values:
             return None
-        return Job(cron=values.get('cron', {}), job=without_keys(values, {'cron'}), spark=values.get('spark', {}))
+        return Job(
+            cron=values.get("cron", {}),
+            job=without_keys(values, {"cron"}),
+            spark=values.get("spark", {}),
+        )
 
 
 @dataclass(frozen=True)
 class Kubernetes:
     port_mappings: dict[int, int]
     liveness_probe: Optional[Probe]
     startup_probe: Optional[Probe]
     metrics: Optional[Metrics]
     resources: Resources
     job: Optional[Job]
 
     @staticmethod
     def from_config(values: dict):
         return Kubernetes(
-            port_mappings=values.get('portMappings', {}),
-            liveness_probe=Probe.from_config(values.get('livenessProbe', {})),
-            startup_probe=Probe.from_config(values.get('startupProbe', {})),
-            metrics=Metrics.from_config(values.get('metrics', {})),
-            resources=Resources.from_config(values.get('resources', {})),
-            job=Job.from_config(values.get('job', {}))
+            port_mappings=values.get("portMappings", {}),
+            liveness_probe=Probe.from_config(values.get("livenessProbe", {})),
+            startup_probe=Probe.from_config(values.get("startupProbe", {})),
+            metrics=Metrics.from_config(values.get("metrics", {})),
+            resources=Resources.from_config(values.get("resources", {})),
+            job=Job.from_config(values.get("job", {})),
         )
 
 
 @dataclass(frozen=True)
 class Host:
     host: TargetProperty[str]
     service_port: Optional[int]
     tls: TargetProperty[str]
     whitelists: TargetProperty[list[str]]
 
     @staticmethod
     def from_config(values: dict):
         return Host(
-            host=TargetProperty.from_config(values.get('host', {})),
-            service_port=values.get('servicePort'),
-            tls=TargetProperty.from_config(values.get('tls', {})),
-            whitelists=TargetProperty.from_config(values.get('whitelists', {}))
+            host=TargetProperty.from_config(values.get("host", {})),
+            service_port=values.get("servicePort"),
+            tls=TargetProperty.from_config(values.get("tls", {})),
+            whitelists=TargetProperty.from_config(values.get("whitelists", {})),
         )
 
 
 @dataclass(frozen=True)
 class Traefik:
     hosts: list[Host]
 
     @staticmethod
     def from_config(values: dict):
-        hosts = values.get('hosts')
+        hosts = values.get("hosts")
         return Traefik(hosts=(list(map(Host.from_config, hosts) if hosts else [])))
 
 
 @dataclass(frozen=True)
 class S3Bucket:
     bucket: TargetProperty[str]
 
     @staticmethod
     def from_config(values: dict):
-        return S3Bucket(bucket=TargetProperty.from_config(values.get('bucket', {})))
+        return S3Bucket(bucket=TargetProperty.from_config(values.get("bucket", {})))
 
 
 @dataclass(frozen=True)
 class Deployment:
     namespace: Optional[str]
     properties: Properties
     kubernetes: Optional[Kubernetes]
     traefik: Optional[Traefik]
     s3_bucket: Optional[S3Bucket]
 
     @staticmethod
     def from_config(values: dict):
-        props = values.get('properties')
-        kubernetes = values.get('kubernetes')
-        traefik = values.get('traefik')
-        s3_bucket = values.get('s3')
-
-        return Deployment(namespace=values.get('namespace'),
-                          properties=Properties.from_config(props) if props else None,
-                          kubernetes=Kubernetes.from_config(kubernetes) if kubernetes else None,
-                          traefik=Traefik.from_config(traefik) if traefik else None,
-                          s3_bucket=S3Bucket.from_config(s3_bucket) if s3_bucket else None)
+        props = values.get("properties")
+        kubernetes = values.get("kubernetes")
+        traefik = values.get("traefik")
+        s3_bucket = values.get("s3")
+
+        return Deployment(
+            namespace=values.get("namespace"),
+            properties=Properties.from_config(props) if props else None,
+            kubernetes=Kubernetes.from_config(kubernetes) if kubernetes else None,
+            traefik=Traefik.from_config(traefik) if traefik else None,
+            s3_bucket=S3Bucket.from_config(s3_bucket) if s3_bucket else None,
+        )
 
 
 @dataclass(frozen=True)
 class ProjectName:
     name: str
     namespace: Optional[str]
 
@@ -318,21 +345,25 @@
     def __hash__(self):
         return hash(self.path)
 
     @property
     def to_name(self) -> ProjectName:
         return ProjectName(
             name=self.name,
-            namespace=self.deployment.namespace if self.deployment and self.deployment.namespace else None
+            namespace=self.deployment.namespace
+            if self.deployment and self.deployment.namespace
+            else None,
         )
 
     @property
     def kubernetes(self) -> Kubernetes:
         if self.deployment is None or self.deployment.kubernetes is None:
-            raise KeyError(f"Project '{self.name}' does not have kubernetes configuration")
+            raise KeyError(
+                f"Project '{self.name}' does not have kubernetes configuration"
+            )
         return self.deployment.kubernetes
 
     @property
     def s3_bucket(self) -> S3Bucket:
         if self.deployment is None or self.deployment.s3_bucket is None:
             raise KeyError(f"Project '{self.name}' does not have s3 configuration")
         return self.deployment.s3_bucket
@@ -340,98 +371,115 @@
     @property
     def resources(self) -> Resources:
         return self.kubernetes.resources
 
     @property
     def job(self) -> Job:
         if self.kubernetes.job is None:
-            raise KeyError(f"Project '{self.name}' does not have kubernetes.job configuration")
+            raise KeyError(
+                f"Project '{self.name}' does not have kubernetes.job configuration"
+            )
         return self.kubernetes.job
 
     @staticmethod
     def project_yaml_path() -> str:
-        return 'deployment/project.yml'
+        return "deployment/project.yml"
 
     @property
     def root_path(self) -> str:
-        return self.path.replace(Project.project_yaml_path(), '')
+        return self.path.replace(Project.project_yaml_path(), "")
 
     @property
     def deployment_path(self) -> str:
-        return str(Path(self.root_path, 'deployment'))
+        return str(Path(self.root_path, "deployment"))
 
     @property
     def target_path(self) -> str:
         return str(Path(self.deployment_path, BUILD_ARTIFACTS_FOLDER))
 
     @property
     def test_containers_path(self) -> str:
-        return str(Path(self.deployment_path, 'docker-compose-test.yml'))
+        return str(Path(self.deployment_path, "docker-compose-test.yml"))
 
     @property
     def test_report_path(self) -> str:
-        return str(Path(self.root_path, 'target/test-reports'))
+        return str(Path(self.root_path, "target/test-reports"))
 
     @staticmethod
     def from_config(values: dict, project_path: Path):
-        deployment = values.get('deployment')
-        dependencies = values.get('dependencies')
-        return Project(name=values['name'], description=values['description'], path=str(project_path),
-                       stages=Stages.from_config(values.get('stages', {})), maintainer=values.get('maintainer', []),
-                       deployment=Deployment.from_config(deployment) if deployment else None,
-                       dependencies=Dependencies.from_config(dependencies) if dependencies else None)
+        deployment = values.get("deployment")
+        dependencies = values.get("dependencies")
+        return Project(
+            name=values["name"],
+            description=values["description"],
+            path=str(project_path),
+            stages=Stages.from_config(values.get("stages", {})),
+            maintainer=values.get("maintainer", []),
+            deployment=Deployment.from_config(deployment) if deployment else None,
+            dependencies=Dependencies.from_config(dependencies)
+            if dependencies
+            else None,
+        )
 
 
 def validate_project(file: TextIO) -> dict:
     """
     :file the file to validate
     :return: the validated schema
     :raises `jsonschema.exceptions.ValidationError` when validation fails
     """
-    yaml_values = YAML(typ='unsafe').load(file)
+    yaml_values = YAML(typ="unsafe").load(file)
     template = pkgutil.get_data(__name__, "schema/project.schema.yml")
     if not template:
-        raise ValueError('Schema project.schema.yml not found in package')
-    validate(yaml_values, template.decode('utf-8'))
+        raise ValueError("Schema project.schema.yml not found in package")
+    validate(yaml_values, template.decode("utf-8"))
 
     return yaml_values
 
 
 def load_project(root_dir: Path, project_path: Path, strict: bool = True) -> Project:
     """
     Load a `project.yml` to `Project` data class
     :param root_dir: root source directory
     :param project_path: relative path from `root_dir` to the `project.yml`
     :param strict: indicates whether the schema should be validated
     :return: `Project` data class
     """
-    with open(root_dir / project_path, encoding='utf-8') as file:
+    with open(root_dir / project_path, encoding="utf-8") as file:
         try:
             start = time.time()
-            yaml_values = validate_project(file) if strict else YAML(typ='unsafe').load(file)
+            yaml_values = (
+                validate_project(file) if strict else YAML(typ="unsafe").load(file)
+            )
             project = Project.from_config(yaml_values, project_path)
-            logging.debug(f'Loaded project {project.path} in {(time.time() - start) * 1000} ms')
+            logging.debug(
+                f"Loaded project {project.path} in {(time.time() - start) * 1000} ms"
+            )
             return project
         except jsonschema.exceptions.ValidationError as exc:
-            logging.warning(f'{project_path} does not comply with schema: {exc.message}')
+            logging.warning(
+                f"{project_path} does not comply with schema: {exc.message}"
+            )
             raise
         except TypeError:
             traceback.print_exc()
-            logging.warning('Type error', exc_info=True)
+            logging.warning("Type error", exc_info=True)
             raise
         except Exception:
-            logging.warning(f'Failed to load {project_path}', exc_info=True)
+            logging.warning(f"Failed to load {project_path}", exc_info=True)
             raise
 
 
 def get_env_variables(project: Project, target: Target) -> dict[str, str]:
     if project.deployment is None:
-        raise KeyError(f'No deployment information was found for project: {project.name}')
+        raise KeyError(
+            f"No deployment information was found for project: {project.name}"
+        )
     if len(project.deployment.properties.env) == 0:
-        raise KeyError(f'No properties.env is defined for project: {project.name}')
+        raise KeyError(f"No properties.env is defined for project: {project.name}")
 
     env_variables: dict[str, str] = {
-        env_variable.key: env_variable.get_value(target) for env_variable in
-        project.deployment.properties.env
+        env_variable.key: env_variable.get_value(target)
+        for env_variable in project.deployment.properties.env
     }
 
     return env_variables
```

## mpyl/validation.py

```diff
@@ -13,36 +13,41 @@
 @lru_cache(maxsize=10)
 def load_schema(schema_string: str) -> Draft7Validator:
     schema = yaml.load(schema_string)
     project_schema_string = pkgutil.get_data(__name__, "schema/project.schema.yml")
     if not project_schema_string:
         raise ImportError("'schema/project.schema.yml' was not found in bundle")
 
-    project_schema = yaml.load(project_schema_string.decode('utf-8'))
+    project_schema = yaml.load(project_schema_string.decode("utf-8"))
 
     def load_schema_from_local(uri):
-        if 'project.schema.yml' in uri:
+        if "project.schema.yml" in uri:
             return project_schema
         return {}
 
-    resolver = RefResolver(referrer=schema, base_uri="", handlers={"": load_schema_from_local})
+    resolver = RefResolver(
+        referrer=schema, base_uri="", handlers={"": load_schema_from_local}
+    )
     all_validators = dict(Draft7Validator.VALIDATORS)
-    existing_validator = all_validators['type']
+    existing_validator = all_validators["type"]
 
     def allow_none_validator(validator, types, instance, yaml_schema):
         for field_type in types:
             if field_type is None and instance is None:
                 return None
 
         return existing_validator(validator, types, instance, yaml_schema)
 
-    all_validators['type'] = allow_none_validator
+    all_validators["type"] = allow_none_validator
     type_checker = Draft7Validator.TYPE_CHECKER
 
-    extended_validator = validators.extend(jsonschema.validators.Draft7Validator, validators=all_validators,
-                                           type_checker=type_checker)
+    extended_validator = validators.extend(
+        jsonschema.validators.Draft7Validator,
+        validators=all_validators,
+        type_checker=type_checker,
+    )
     return extended_validator(schema=schema, resolver=resolver)
 
 
 def validate(values: dict, schema_string: str):
     schema = load_schema(schema_string)
     return schema.validate(values)
```

## mpyl/cli/__init__.py

```diff
@@ -1,27 +1,33 @@
 """Command Line Interface parsing for MPyL"""
 import asyncio
 import importlib
 import logging
 from dataclasses import dataclass
 from importlib.metadata import version as version_meta
+from pathlib import Path
 from typing import Optional
 
 import aiohttp
+import click
 import requests
 from aiohttp import ClientConnectorError, ClientTimeout
+from click import BadParameter
 
 from rich.console import Console
 from rich.logging import RichHandler
 
+from ..utilities.pyaml_env import parse_config
 from ..utilities.repo import Repository
 
-CONFIG_PATH_HELP = 'Path to the config.yml. Needs to comply with schema at ' \
-                   'https://vandebron.github.io/mpyl/schema/mpyl_config.schema.yml ' \
-                   'Can be set via `MPYL_CONFIG_PATH` env var. '
+CONFIG_PATH_HELP = (
+    "Path to the config.yml. Needs to comply with schema at "
+    "https://vandebron.github.io/mpyl/schema/mpyl_config.schema.yml "
+    "Can be set via `MPYL_CONFIG_PATH` env var. "
+)
 
 
 @dataclass(frozen=True)
 class CliContext:
     config: dict
     repo: Repository
     console: Console
@@ -30,22 +36,26 @@
 
 
 async def fetch_latest_version() -> Optional[str]:
     try:
         async with aiohttp.ClientSession(timeout=ClientTimeout(total=10)) as session:
             async with session.get("https://pypi.org/pypi/mpyl/json") as response:
                 body = await response.json()
-                return body.get('info', {}).get('version')
-    except (asyncio.exceptions.TimeoutError, ClientConnectorError, requests.exceptions.RequestException):
+                return body.get("info", {}).get("version")
+    except (
+        asyncio.exceptions.TimeoutError,
+        ClientConnectorError,
+        requests.exceptions.RequestException,
+    ):
         return None
 
 
 def get_meta_version():
     try:
-        return version_meta('mpyl')
+        return version_meta("mpyl")
     except importlib.metadata.PackageNotFoundError:
         return None
 
 
 async def check_updates(meta: str) -> Optional[str]:
     latest = await fetch_latest_version()
     if latest and meta != latest:
@@ -53,21 +63,43 @@
     return None
 
 
 def get_version():
     try:
         return f"v{version_meta('mpyl')}"
     except importlib.metadata.PackageNotFoundError:
-        return '(local)'
+        return "(local)"
 
 
 FORMAT = "%(message)s"
 
 
 def create_console_logger(local: bool, verbose: bool) -> Console:
-    console = Console(markup=True, width=None if local else 135, no_color=False, log_path=False, log_time=False,
-                      color_system='256')
+    console = Console(
+        markup=True,
+        width=None if local else 135,
+        no_color=False,
+        log_path=False,
+        log_time=False,
+        color_system="256",
+    )
     logging.basicConfig(
-        level="DEBUG" if verbose else "INFO", format=FORMAT, datefmt="[%X]",
-        handlers=[RichHandler(markup=True, console=console, show_path=local)]
+        level="DEBUG" if verbose else "INFO",
+        format=FORMAT,
+        datefmt="[%X]",
+        handlers=[RichHandler(markup=True, console=console, show_path=local)],
     )
     return console
+
+
+def parse_config_from_supplied_location(ctx: click.Context, param) -> dict[str, str]:
+    if (
+        not ctx.parent
+        or ctx.parent.params["config"] is None
+        or not Path(ctx.parent.params["config"]).exists()
+    ):
+        raise BadParameter(
+            "Either --config parameter must or MPYL_CONFIG_PATH env var must be set",
+            ctx=ctx,
+            param=param,
+        )
+    return parse_config(ctx.parent.params["config"])
```

## mpyl/cli/build.py

```diff
@@ -2,82 +2,138 @@
 import asyncio
 import shutil
 from pathlib import Path
 from typing import Optional
 
 import click
 import questionary
-from click import ParamType, BadParameter
+from click import ParamType
 from click.shell_completion import CompletionItem
 from github import Github
 from github.GitRelease import GitRelease
 from questionary import Choice
 from rich.console import Console
 from rich.markdown import Markdown
 
-from . import CliContext, CONFIG_PATH_HELP, check_updates, get_meta_version
+from . import (
+    CliContext,
+    CONFIG_PATH_HELP,
+    check_updates,
+    get_meta_version,
+    parse_config_from_supplied_location,
+)
 from . import create_console_logger
 from .commands.build.jenkins import JenkinsRunParameters, run_jenkins, get_token
-from .commands.build.mpyl import MpylRunParameters, run_mpyl, MpylCliParameters, MpylRunConfig, find_build_set
-from ..constants import DEFAULT_CONFIG_FILE_NAME, DEFAULT_RUN_PROPERTIES_FILE_NAME, BUILD_ARTIFACTS_FOLDER
+from .commands.build.mpyl import (
+    MpylRunParameters,
+    run_mpyl,
+    MpylCliParameters,
+    MpylRunConfig,
+    find_build_set,
+)
+from ..constants import (
+    DEFAULT_CONFIG_FILE_NAME,
+    DEFAULT_RUN_PROPERTIES_FILE_NAME,
+    BUILD_ARTIFACTS_FOLDER,
+)
 from ..project import load_project
 from ..reporting.formatting.markdown import run_result_to_markdown
 from ..steps.models import RunProperties
 from ..steps.run import RunResult
 from ..utilities.github import GithubConfig
 from ..utilities.pyaml_env import parse_config
 from ..utilities.repo import Repository, RepoConfig
 
 
 async def warn_if_update(console: Console):
     version = get_meta_version()
     update = await check_updates(meta=version)
     if update:
-        console.print(Markdown(f"⚠️  **You can upgrade from {version} to {update} :** `pip install -U mpyl=={update}`"))
+        console.print(
+            Markdown(
+                f"⚠️  **You can upgrade from {version} to {update} :** `pip install -U mpyl=={update}`"
+            )
+        )
 
 
-@click.group('build')
-@click.option('--config', '-c', required=True, type=click.Path(exists=True), help=CONFIG_PATH_HELP,
-              envvar="MPYL_CONFIG_PATH", default=DEFAULT_CONFIG_FILE_NAME)
-@click.option('--properties', '-p', required=False, type=click.Path(exists=False), help='Path to run properties',
-              envvar="MPYL_RUN_PROPERTIES_PATH", default=DEFAULT_RUN_PROPERTIES_FILE_NAME, show_default=True)
-@click.option('--verbose', '-v', is_flag=True, default=False, show_default=True, help='Verbose output')
+@click.group("build")
+@click.option(
+    "--config",
+    "-c",
+    required=True,
+    type=click.Path(exists=True),
+    help=CONFIG_PATH_HELP,
+    envvar="MPYL_CONFIG_PATH",
+    default=DEFAULT_CONFIG_FILE_NAME,
+)
+@click.option(
+    "--properties",
+    "-p",
+    required=False,
+    type=click.Path(exists=False),
+    help="Path to run properties",
+    envvar="MPYL_RUN_PROPERTIES_PATH",
+    default=DEFAULT_RUN_PROPERTIES_FILE_NAME,
+    show_default=True,
+)
+@click.option(
+    "--verbose",
+    "-v",
+    is_flag=True,
+    default=False,
+    show_default=True,
+    help="Verbose output",
+)
 @click.pass_context
 def build(ctx, config, properties, verbose):
     """Pipeline build commands"""
     console = create_console_logger(local=False, verbose=verbose)
     parsed_config = parse_config(config)
     parsed_properties = parse_config(properties)
 
     repo = ctx.with_resource(Repository(config=RepoConfig.from_config(parsed_config)))
     ctx.obj = CliContext(parsed_config, repo, console, verbose, parsed_properties)
 
 
-@build.command(help='Run an MPyL build')
-@click.option('--ci', is_flag=True,
-              help='Run as CI build instead of local. Ignores unversioned changes.')
-@click.option('--all', 'all_', is_flag=True, help='Build all projects, regardless of changes on branch')
+@build.command(help="Run an MPyL build")
 @click.option(
-    '--tag', '-t',
-    help='Tag to build',
-    type=click.STRING,
-    required=False
+    "--ci",
+    is_flag=True,
+    help="Run as CI build instead of local. Ignores unversioned changes.",
+)
+@click.option(
+    "--all",
+    "all_",
+    is_flag=True,
+    help="Build all projects, regardless of changes on branch",
 )
+@click.option("--tag", "-t", help="Tag to build", type=click.STRING, required=False)
 @click.pass_obj
 def run(obj: CliContext, ci, all_, tag):  # pylint: disable=invalid-name
     asyncio.run(warn_if_update(obj.console))
-    run_properties = RunProperties.from_configuration(obj.run_properties, obj.config) if ci \
-        else RunProperties.for_local_run(obj.config, obj.repo.get_sha, obj.repo.get_branch, tag)
+    run_properties = (
+        RunProperties.from_configuration(obj.run_properties, obj.config)
+        if ci
+        else RunProperties.for_local_run(
+            obj.config, obj.repo.get_sha, obj.repo.get_branch, tag
+        )
+    )
 
-    parameters = MpylCliParameters(local=not ci, pull_main=all_, all=all_, verbose=obj.verbose, tag=tag,
-                                   target=run_properties.target)
+    parameters = MpylCliParameters(
+        local=not ci,
+        pull_main=all_,
+        all=all_,
+        verbose=obj.verbose,
+        tag=tag,
+        target=run_properties.target,
+    )
     obj.console.log(parameters)
     run_parameters = MpylRunParameters(
         run_config=MpylRunConfig(config=obj.config, run_properties=run_properties),
-        parameters=parameters
+        parameters=parameters,
     )
     run_mpyl(run_parameters, None)
 
 
 @build.command(help="The status of the current local branch from MPyL's perspective")
 @click.pass_obj
 def status(obj: CliContext):
@@ -91,176 +147,232 @@
 
 def __print_status(obj: CliContext):
     run_properties = RunProperties.from_configuration(obj.run_properties, obj.config)
     branch = run_properties.versioning.branch
     if not branch:
         branch = obj.repo.get_branch
         obj.console.log(
-            f'Branch not specified in `{DEFAULT_RUN_PROPERTIES_FILE_NAME}`. Branch determined via git: {branch}')
+            f"Branch not specified in `{DEFAULT_RUN_PROPERTIES_FILE_NAME}`. Branch determined via git: {branch}"
+        )
 
     if branch and obj.repo.main_branch == obj.repo.get_branch:
-        obj.console.log(f'On main branch ({branch}), cannot determine build status')
+        obj.console.log(f"On main branch ({branch}), cannot determine build status")
         return
     tag = obj.repo.get_tag if not branch else None
     version = run_properties.versioning
     revision = "Tag" if tag else "Branch"
-    obj.console.print(Markdown(f"**{revision}:** `{version.branch or version.tag}` at `{version.revision}`"))
+    obj.console.print(
+        Markdown(
+            f"**{revision}:** `{version.branch or version.tag}` at `{version.revision}`"
+        )
+    )
 
     if obj.repo.main_branch_pulled:
-        changes = obj.repo.changes_in_branch_including_local() if branch else obj.repo.changes_in_merge_commit()
+        changes = (
+            obj.repo.changes_in_branch_including_local()
+            if branch
+            else obj.repo.changes_in_merge_commit()
+        )
         build_set = find_build_set(obj.repo, changes, False)
         result = RunResult(run_properties=run_properties, run_plan=build_set)
         if result.run_plan:
-            obj.console.print(Markdown("**Execution plan:**  \n" + run_result_to_markdown(result)))
+            obj.console.print(
+                Markdown("**Execution plan:**  \n" + run_result_to_markdown(result))
+            )
         else:
             obj.console.print("No changes detected, nothing to do.")
 
 
 class Pipeline(ParamType):
-    name = 'pipeline'
+    name = "pipeline"
 
     def shell_complete(self, ctx: click.Context, param, incomplete: str):
-        if not ctx.parent or ctx.parent.params['config'] is None or not Path(ctx.parent.params['config']).exists():
-            raise BadParameter('Either --config parameter must or MPYL_CONFIG_PATH env var must be set', ctx=ctx,
-                               param=param)
+        config: dict = parse_config_from_supplied_location(ctx, param)
 
-        config: dict = parse_config(ctx.parent.params['config'])
-        parsed_config: dict[str, str] = config['jenkins']['pipelines']
+        pipelines: dict[str, str] = config["jenkins"]["pipelines"]
 
         return [
-            CompletionItem(value=pl[0], help=pl[1]) for pl in parsed_config.items() if
-            incomplete in pl[0]
+            CompletionItem(value=pl[0], help=pl[1])
+            for pl in pipelines.items()
+            if incomplete in pl[0]
         ]
 
 
 def select_tag(ctx) -> str:
     console = Console()
     with console.status("Fetching tags...") as spinner:
         github_config = GithubConfig.from_config(ctx.obj.config)
         github = Github(login_or_token=get_token(github_config))
 
         repo = github.get_repo(github_config.repository)
 
         def to_choice(git_release: GitRelease):
-            title = git_release.title + " " + git_release.body.split('* ')[-1].splitlines()[0]
+            title = (
+                git_release.title
+                + " "
+                + git_release.body.split("* ")[-1].splitlines()[0]
+            )
             return Choice(title=title, value=git_release.title)
 
         choices = map(to_choice, repo.get_releases())
         user_name = github.get_user().login
 
         def by_choice(choice: Choice):
             # prioritize own tags
             if user_name in str(choice.title):
                 return f"9{choice.value}"
             return choice.value
 
         sorted_choices = sorted(choices, key=by_choice, reverse=True)
 
         spinner.stop()
-        release_id = questionary.select("Which tag do you want to release?", show_selected=True,
-                                        choices=sorted_choices).ask()
+        release_id = questionary.select(
+            "Which tag do you want to release?",
+            show_selected=True,
+            choices=sorted_choices,
+        ).ask()
         release = repo.get_release(release_id)
         return release.tag_name
 
 
 def ask_for_input(ctx, _param, value) -> Optional[str]:
     if value == "not_set":
         return None
     if value == "prompt":
         return select_tag(ctx)
     return value
 
 
-@build.command(help='Run a multi branch pipeline build on Jenkins')
+@build.command(help="Run a multi branch pipeline build on Jenkins")
 @click.option(
-    '--user', '-u',
-    help='Authentication API user. Can be set via env var JENKINS_USER',
+    "--user",
+    "-u",
+    help="Authentication API user. Can be set via env var JENKINS_USER",
     envvar="JENKINS_USER",
     type=click.STRING,
-    required=True
+    required=True,
 )
 @click.option(
-    '--password', '-p',
-    help='Authentication API password. Can be set via env var JENKINS_PASSWORD',
+    "--password",
+    "-p",
+    help="Authentication API password. Can be set via env var JENKINS_PASSWORD",
     envvar="JENKINS_PASSWORD",
     type=click.STRING,
-    required=True
+    required=True,
 )
 @click.option(
-    '--pipeline', '-pl',
-    help='The pipeline to run. Must be one of the pipelines listed in `jenkins.pipelines`. '
-         'Default value is `jenkins.defaultPipeline`',
+    "--pipeline",
+    "-pl",
+    help="The pipeline to run. Must be one of the pipelines listed in `jenkins.pipelines`. "
+    "Default value is `jenkins.defaultPipeline`",
     type=Pipeline(),
-    required=False
+    required=False,
 )
 @click.option(
-    '--test', '-t',
-    help='A specific test version on https://test.pypi.org/project/mpyl/ to use for the build.',
+    "--test",
+    "-t",
+    help="A specific test version on https://test.pypi.org/project/mpyl/ to use for the build.",
     type=click.STRING,
-    required=False
+    required=False,
 )
 @click.option(
-    '--arguments', '-a',
+    "--arguments",
+    "-a",
     multiple=True,
-    help='A series of arguments to pass to the pipeline. Note that will run within the pipenv in jenkins. '
-         'To execute `mpyl build status`, pass `-a run -a mpyl -a build -a status`',
+    help="A series of arguments to pass to the pipeline. Note that will run within the pipenv in jenkins. "
+    "To execute `mpyl build status`, pass `-a run -a mpyl -a build -a status`",
 )
 @click.option(
-    '--background', '-bg',
+    "--background",
+    "-bg",
     help="Starts Jenkins build in a 'fire and forget' fashion. "
-         "Can be set via env var MPYL_JENKINS_BACKGROUND",
+    "Can be set via env var MPYL_JENKINS_BACKGROUND",
     envvar="MPYL_JENKINS_BACKGROUND",
     is_flag=True,
-    default=False
+    default=False,
 )
 @click.option(
-    '--silent', '-s',
+    "--silent",
+    "-s",
     help="Indicates whether to show Jenkins' logging or not. "
-         "Can be set via env var MPYL_JENKINS_SILENT",
+    "Can be set via env var MPYL_JENKINS_SILENT",
     envvar="MPYL_JENKINS_SILENT",
     is_flag=True,
-    default=False
+    default=False,
+)
+@click.option(
+    "--tag",
+    "-tg",
+    is_flag=False,
+    flag_value="prompt",
+    default="not_set",
+    callback=ask_for_input,
 )
-@click.option('--tag', '-tg', is_flag=False, flag_value="prompt", default="not_set", callback=ask_for_input)
 @click.pass_context
-def jenkins(ctx, user, password, pipeline, test, arguments, background, silent,  # pylint: disable=too-many-arguments
-            tag):
+def jenkins(  # pylint: disable=too-many-arguments
+    ctx,
+    user,
+    password,
+    pipeline,
+    test,
+    arguments,
+    background,
+    silent,
+    tag,
+):
     try:
         upgrade_check = asyncio.wait_for(warn_if_update(ctx.obj.console), timeout=5)
-        selected_pipeline = pipeline if pipeline else ctx.obj.config['jenkins']['defaultPipeline']
-        pipeline_parameters = {'TEST': 'true', 'VERSION': test} if test else {}
+        selected_pipeline = (
+            pipeline if pipeline else ctx.obj.config["jenkins"]["defaultPipeline"]
+        )
+        pipeline_parameters = {"TEST": "true", "VERSION": test} if test else {}
         if arguments:
-            pipeline_parameters['BUILD_PARAMS'] = " ".join(arguments)
+            pipeline_parameters["BUILD_PARAMS"] = " ".join(arguments)
 
         run_argument = JenkinsRunParameters(
-            jenkins_user=user, jenkins_password=password, config=ctx.obj.config,
-            pipeline=selected_pipeline, pipeline_parameters=pipeline_parameters,
+            jenkins_user=user,
+            jenkins_password=password,
+            config=ctx.obj.config,
+            pipeline=selected_pipeline,
+            pipeline_parameters=pipeline_parameters,
             verbose=not silent or ctx.obj.verbose,
-            follow=not background, tag=tag
+            follow=not background,
+            tag=tag,
         )
 
         run_jenkins(run_argument)
         asyncio.get_event_loop().run_until_complete(upgrade_check)
     except asyncio.exceptions.TimeoutError:
         pass
 
 
-@build.command(help=f'Clean MPyL metadata in `{BUILD_ARTIFACTS_FOLDER}` folders')
-@click.option('--filter', '-f', 'filter_', required=False, type=click.STRING, help='Filter based on filepath ')
+@build.command(help=f"Clean MPyL metadata in `{BUILD_ARTIFACTS_FOLDER}` folders")
+@click.option(
+    "--filter",
+    "-f",
+    "filter_",
+    required=False,
+    type=click.STRING,
+    help="Filter based on filepath ",
+)
 @click.pass_obj
 def clean(obj: CliContext, filter_):
     found_projects: list[Path] = [
-        Path(load_project(obj.repo.root_dir(), Path(project_path), strict=False).target_path)
-        for project_path in obj.repo.find_projects(filter_ if filter_ else '')
+        Path(
+            load_project(
+                obj.repo.root_dir(), Path(project_path), strict=False
+            ).target_path
+        )
+        for project_path in obj.repo.find_projects(filter_ if filter_ else "")
     ]
 
     paths_to_clean = [path for path in found_projects if path.exists()]
     if paths_to_clean:
         for target_path in paths_to_clean:
             shutil.rmtree(target_path)
             obj.console.print(f"🧹 Cleaned up {target_path}")
     else:
         obj.console.print("Nothing to clean")
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     build()  # pylint: disable=no-value-for-parameter
```

## mpyl/cli/health.py

```diff
@@ -3,12 +3,12 @@
 import click
 from rich.console import Console
 
 from . import create_console_logger
 from .commands.health.checks import perform_health_checks
 
 
-@click.command('health')
+@click.command("health")
 def health():
     """Health check"""
     console: Console = create_console_logger(local=False, verbose=False)
     perform_health_checks(console)
```

## mpyl/cli/meta_info.py

```diff
@@ -38,20 +38,20 @@
 
 
 def simple_version():
     return f"MPyL {get_version()}"
 
 
 def about():
-    dist = distribution('mpyl')
+    dist = distribution("mpyl")
     details = os.linesep.join(str(dist.metadata).split(os.linesep)[1:16])
-    return f'{details}{VDB_LOGO}'
+    return f"{details}{VDB_LOGO}"
 
 
 @click.command()
-@click.option('--verbose', '-v', is_flag=True, default=False, help="Print more output.")
+@click.option("--verbose", "-v", is_flag=True, default=False, help="Print more output.")
 def version(verbose):
     """Version information"""
     if verbose:
         click.echo(about())
     else:
         click.echo(simple_version())
```

## mpyl/cli/projects.py

```diff
@@ -1,99 +1,128 @@
 """Commands related to projects and how they relate"""
 from dataclasses import dataclass
 from pathlib import Path
 
 import click
 import jsonschema
-from click import ParamType, BadParameter
+from click import ParamType
 from click.shell_completion import CompletionItem
 from rich.markdown import Markdown
 
-from . import CliContext, CONFIG_PATH_HELP, create_console_logger
+from . import (
+    CliContext,
+    CONFIG_PATH_HELP,
+    create_console_logger,
+    parse_config_from_supplied_location,
+)
 from .commands.projects.formatting import print_project
 from ..constants import DEFAULT_CONFIG_FILE_NAME
 from ..project import validate_project, load_project, Project
 from ..utilities.pyaml_env import parse_config
 from ..utilities.repo import Repository, RepoConfig
 
 
 @dataclass
 class ProjectsContext:
     cli: CliContext
     filter: str
 
 
-@click.group('projects')
-@click.option('--config', '-c', required=True, type=click.Path(exists=True), help=CONFIG_PATH_HELP,
-              envvar="MPYL_CONFIG_PATH", default=DEFAULT_CONFIG_FILE_NAME)
-@click.option('--verbose', '-v', is_flag=True, default=False)
-@click.option('--filter', '-f', 'filter_', required=False, type=click.STRING, help='Filter based on filepath ')
+@click.group("projects")
+@click.option(
+    "--config",
+    "-c",
+    required=True,
+    type=click.Path(exists=True),
+    help=CONFIG_PATH_HELP,
+    envvar="MPYL_CONFIG_PATH",
+    default=DEFAULT_CONFIG_FILE_NAME,
+)
+@click.option("--verbose", "-v", is_flag=True, default=False)
+@click.option(
+    "--filter",
+    "-f",
+    "filter_",
+    required=False,
+    type=click.STRING,
+    help="Filter based on filepath ",
+)
 @click.pass_context
 def projects(ctx, config, verbose, filter_):
     """Commands related to projects"""
     console = create_console_logger(local=False, verbose=verbose)
     parsed_config = parse_config(config)
     ctx.obj = ProjectsContext(
-        cli=CliContext(config=parsed_config,
-                       repo=ctx.with_resource(Repository(config=RepoConfig.from_config(parsed_config))),
-                       console=console, verbose=verbose, run_properties={}), filter=filter_ if filter_ else '')
+        cli=CliContext(
+            config=parsed_config,
+            repo=ctx.with_resource(
+                Repository(config=RepoConfig.from_config(parsed_config))
+            ),
+            console=console,
+            verbose=verbose,
+            run_properties={},
+        ),
+        filter=filter_ if filter_ else "",
+    )
 
 
-@projects.command(name='list', help='List found projects')
+@projects.command(name="list", help="List found projects")
 @click.pass_obj
 def list_projects(obj: ProjectsContext):
     found_projects = obj.cli.repo.find_projects(obj.filter)
 
     for proj in found_projects:
         name = load_project(obj.cli.repo.root_dir(), Path(proj), False).name
         obj.cli.console.print(Markdown(f"{proj} `{name}`"))
 
 
 class ProjectPath(ParamType):
-    name = 'project_path'
+    name = "project_path"
 
     def shell_complete(self, ctx: click.Context, param, incomplete: str):
-        if not ctx.parent or ctx.parent.params['config'] is None or not Path(ctx.parent.params['config']).exists():
-            raise BadParameter('Either --config parameter must or MPYL_CONFIG_PATH env var must be set', ctx=ctx,
-                               param=param)
-
-        parsed_config = parse_config(ctx.parent.params['config'])
-        repo = ctx.with_resource(Repository(config=RepoConfig.from_config(parsed_config)))
+        parsed_config = parse_config_from_supplied_location(ctx, param)
+        repo = ctx.with_resource(
+            Repository(config=RepoConfig.from_config(parsed_config))
+        )
         found_projects = repo.find_projects(incomplete)
         return [
-            CompletionItem(value=proj.replace(f'/{Project.project_yaml_path()}', ''))
+            CompletionItem(value=proj.replace(f"/{Project.project_yaml_path()}", ""))
             for proj in found_projects
         ]
 
 
-@projects.command(name='show', help='Show details of a project')
-@click.argument('name', required=True, type=ProjectPath())
+@projects.command(name="show", help="Show details of a project")
+@click.argument("name", required=True, type=ProjectPath())
 @click.pass_obj
 def show_project(obj, name):
-    print_project(obj.cli.repo, obj.cli.console, f'{name}/{Project.project_yaml_path()}')
+    print_project(
+        obj.cli.repo, obj.cli.console, f"{name}/{Project.project_yaml_path()}"
+    )
 
 
-@projects.command(help='Validate the yaml of found projects against their schema')
+@projects.command(help="Validate the yaml of found projects against their schema")
 @click.pass_obj
 def lint(obj: ProjectsContext):
     found_projects = obj.cli.repo.find_projects(obj.filter)
     invalid = 0
     valid = 0
     for project in found_projects:
         try:
             project_path = Path(obj.cli.repo.root_dir()) / Path(project)
-            with open(project_path, encoding='utf-8') as file:
+            with open(project_path, encoding="utf-8") as file:
                 validate_project(file)
         except jsonschema.exceptions.ValidationError as exc:
-            obj.cli.console.print(f'❌ {project}: {exc.message}')
+            obj.cli.console.print(f"❌ {project}: {exc.message}")
             invalid += 1
         else:
             valid += 1
             if obj.cli.verbose:
-                obj.cli.console.print(f'✅ {project}')
-    obj.cli.console.print(f'Validated {valid + invalid} projects. {valid} valid, {invalid} invalid')
+                obj.cli.console.print(f"✅ {project}")
+    obj.cli.console.print(
+        f"Validated {valid + invalid} projects. {valid} valid, {invalid} invalid"
+    )
     if invalid > 0:
         click.get_current_context().exit(1)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     projects()  # pylint: disable=no-value-for-parameter
```

## mpyl/cli/commands/build/mpyl.py

```diff
@@ -66,15 +66,14 @@
 
 
 def run_mpyl(mpyl_run_parameters: MpylRunParameters, reporter: Optional[Reporter]) -> RunResult:
     params = mpyl_run_parameters.parameters
     console_properties = mpyl_run_parameters.run_config.run_properties.console
     console = Console(markup=False, width=None if params.local else console_properties.width, no_color=False,
                       log_path=False, color_system='256')
-    print(f"Logging properties: {console_properties}, console: {console}")
     logging.raiseExceptions = False
     logging.basicConfig(
         level="DEBUG" if params.verbose else console_properties.log_level, format=FORMAT, datefmt="[%X]",
         handlers=[RichHandler(markup=False, console=console, show_path=params.local)]
     )
     logger = logging.getLogger('mpyl')
     try:
@@ -122,22 +121,26 @@
                 Stage.DEPLOY: for_stage(all_projects, Stage.DEPLOY),
                 Stage.POST_DEPLOY: for_stage(all_projects, Stage.POST_DEPLOY)}
 
     return find_invalidated_projects_per_stage(all_projects, changes_in_branch)
 
 
 def run_build(accumulator: RunResult, executor: Steps, reporter: Optional[Reporter] = None, dry_run: bool = True):
-    for stage, projects in accumulator.run_plan.items():
-        for proj in projects:
-            result = executor.execute(stage, proj, dry_run)
-            accumulator.append(result)
-            if reporter:
-                reporter.send_report(accumulator)
+    try:
+        for stage, projects in accumulator.run_plan.items():
+            for proj in projects:
+                result = executor.execute(stage, proj, dry_run)
+                accumulator.append(result)
+                if reporter:
+                    reporter.send_report(accumulator)
+
+                if not result.output.success and stage == Stage.DEPLOY:
+                    logging.warning(f'Deployment failed for {proj.name}')
+                    return accumulator
 
-            if not result.output.success and stage == Stage.DEPLOY:
-                logging.warning(f'Deployment failed for {proj.name}')
+            if accumulator.failed_result:
+                logging.warning(f'One of the builds failed at {stage}')
                 return accumulator
-
-        if accumulator.failed_result:
-            logging.warning(f'One of the builds failed at {stage}')
-            return accumulator
-    return accumulator
+        return accumulator
+    except ExecutionException as exc:
+        accumulator.exception = exc
+        return accumulator
```

## mpyl/cli/commands/health/checks.py

```diff
@@ -22,110 +22,145 @@
 
 
 class HealthConsole:
     def __init__(self, console: Console):
         self.console = console
 
     def title(self, title: str):
-        self.console.print(Markdown(f'*{title}*'))
+        self.console.print(Markdown(f"*{title}*"))
 
     def check(self, check: str, success: bool):
-        icon = '✅' if success else '❌'
-        self.console.print(Markdown(f'&nbsp;&nbsp;{icon} {check}'))
+        icon = "✅" if success else "❌"
+        self.console.print(Markdown(f"&nbsp;&nbsp;{icon} {check}"))
 
 
 def perform_health_checks(bare_console: Console):
     console = HealthConsole(bare_console)
-    console.title('Version')
+    load_dotenv(Path(".env"))
+
+    console.title("Version")
     __check_version(console)
 
-    console.title('MPyL configuration')
-    __check_config(console, env_var='MPYL_CONFIG_PATH', default=DEFAULT_CONFIG_FILE_NAME,
-                   schema_path='../../../schema/mpyl_config.schema.yml', name='config')
-
-    console.title('Run configuration')
-    __check_config(console, env_var='MPYL_RUN_PROPERTIES_PATH', default=DEFAULT_RUN_PROPERTIES_FILE_NAME,
-                   schema_path='../../../schema/run_properties.schema.yml', name='run properties')
+    console.title("MPyL configuration")
+    __check_config(
+        console,
+        env_var="MPYL_CONFIG_PATH",
+        default=DEFAULT_CONFIG_FILE_NAME,
+        schema_path="../../../schema/mpyl_config.schema.yml",
+        name="config",
+    )
+
+    console.title("Run configuration")
+    __check_config(
+        console,
+        env_var="MPYL_RUN_PROPERTIES_PATH",
+        default=DEFAULT_RUN_PROPERTIES_FILE_NAME,
+        schema_path="../../../schema/run_properties.schema.yml",
+        name="run properties",
+    )
 
-    console.title('Jenkins')
+    console.title("Jenkins")
     __check_jenkins(console)
 
 
 def __check_jenkins(console: HealthConsole):
-    path = os.environ.get('MPYL_CONFIG_PATH', default=DEFAULT_CONFIG_FILE_NAME)
+    path = os.environ.get("MPYL_CONFIG_PATH", default=DEFAULT_CONFIG_FILE_NAME)
     if not os.path.exists(path):
-        console.check(f'Configuration not found at: `{path}`', success=False)
+        console.check(f"Configuration not found at: `{path}`", success=False)
         return
 
     parsed = parse_config(Path(path))
 
     try:
         jenkins_conf = JenkinsConfig.from_config(parsed)
-        console.check(f'Jenkins configured for pipeline `{jenkins_conf.default_pipeline}` '
-                      f'at [{jenkins_conf.url}]({jenkins_conf.url})', success=True)
+        console.check(
+            f"Jenkins configured for pipeline `{jenkins_conf.default_pipeline}` "
+            f"at [{jenkins_conf.url}]({jenkins_conf.url})",
+            success=True,
+        )
     except KeyError as exc:
-        console.check(f'Jenkins config not valid: {exc}', success=False)
+        console.check(f"Jenkins config not valid: {exc}", success=False)
 
-    gh_is_installed = shutil.which('gh')
+    gh_is_installed = shutil.which("gh")
     if gh_is_installed:
-        console.check('Github cli client `gh` installed', success=True)
+        console.check("Github cli client `gh` installed", success=True)
     else:
         console.check(
-            'Github cli client `gh` not found. Install via [https://cli.github.com/](https://cli.github.com/) '
-            'and run `gh auth login`', success=False)
+            "Github cli client `gh` not found. Install via [https://cli.github.com/](https://cli.github.com/) "
+            "and run `gh auth login`",
+            success=False,
+        )
 
     if gh_is_installed:
         try:
             get_token(GithubConfig.from_config(parsed))
-            console.check('Github token found', success=True)
+            console.check("Github token found", success=True)
         except CalledProcessError:
-            console.check('Github token not found. Log in with `gh auth login`', success=False)
+            console.check(
+                "Github token not found. Log in with `gh auth login`", success=False
+            )
 
-    if os.environ.get('JENKINS_USER'):
-        console.check('Jenkins user set', success=True)
+    if os.environ.get("JENKINS_USER"):
+        console.check("Jenkins user set", success=True)
     else:
-        jenkins_url = f'{JenkinsConfig.from_config(parsed).url}user/me@vandebron.nl/configure'
-        message = f'Jenkins user not set via JENKINS_USER env var. Create a user API token in Jenkins' \
-                  f' (user:password) API token: {jenkins_url}'
+        jenkins_url = (
+            f"{JenkinsConfig.from_config(parsed).url}user/me@vandebron.nl/configure"
+        )
+        message = (
+            f"Jenkins user not set via JENKINS_USER env var. Create a user API token in Jenkins"
+            f" (user:password) API token: {jenkins_url}"
+        )
         console.check(message, success=False)
 
-    if os.environ.get('JENKINS_PASSWORD'):
-        console.check('Jenkins password set', success=True)
+    if os.environ.get("JENKINS_PASSWORD"):
+        console.check("Jenkins password set", success=True)
     else:
-        console.check('Jenkins password not set via JENKINS_PASSWORD env var', success=False)
+        console.check(
+            "Jenkins password not set via JENKINS_PASSWORD env var", success=False
+        )
 
 
 def __check_version(console):
     update = asyncio.get_event_loop().run_until_complete(fetch_latest_version())
     meta_version = get_meta_version()
     if update and meta_version:
         if meta_version == update:
-            console.check(f'At latest version: {update}', success=True)
+            console.check(f"At latest version: {update}", success=True)
         else:
-            console.check(f'Outdated version: {meta_version} (latest: {update})', success=False)
+            console.check(
+                f"Outdated version: {meta_version} (latest: {update})", success=False
+            )
     else:
-        console.check('Could not determine latest version', success=False)
+        console.check("Could not determine latest version", success=False)
 
 
 def __check_config(console, env_var, default, schema_path, name):
-    path = os.environ.get(env_var, default=default)
-    location = f"{name} at `/{path}` via environment variable `{env_var}`" if os.environ.get(
-        env_var) else f"{name} at `/{path}`"
+    path_env = os.environ.get(env_var)
+    path = path_env or default
+    location = (
+        f"{name} at `/{path}` via environment variable `{env_var}`"
+        if path_env
+        else f"{name} at `/{path}`"
+    )
     if os.path.exists(path):
         console.check(f"Found {location}", success=True)
 
         if load_dotenv(Path(".env")):
             console.check("Set env variables via .env file", success=True)
 
         parsed = parse_config(path)
         schema_dict = pkgutil.get_data(__name__, schema_path)
         if schema_dict:
             try:
-                validate(parsed, schema_dict.decode('utf-8'))
-                console.check(f'{name.capitalize()} is valid', success=True)
+                validate(parsed, schema_dict.decode("utf-8"))
+                console.check(f"{name.capitalize()} is valid", success=True)
             except jsonschema.exceptions.ValidationError as exc:
                 console.check(
                     f"{name.capitalize()} is invalid: {exc.message} at '{'.'.join(exc.path)}'. 🤔Did you rebase"
                     f" your branch onto {parsed['cvs']['git']['mainBranch']}?",
-                    success=False)
+                    success=False,
+                )
     else:
-        console.check(f"Could not find {location}. Location can be specified with env var '{env_var}'", success=False)
+        console.check(
+            f"Could not find {location}. Location can be specified with env var '{env_var}'",
+            success=False,
+        )
```

## mpyl/cli/commands/projects/formatting.py

```diff
@@ -19,9 +19,11 @@
     table = Table(title=f"Project {project.name}", show_header=False)
     table.add_row("Name", project.name)
     table.add_row("Path", project.path)
     table.add_row("Description", project.description)
     table.add_row("Maintainer", f"{project.maintainer}")
     table.add_row("Stages", f"{project.stages}")
     if with_dependencies.dependent_projects:
-        table.add_row("Dependent projects", f"{set(with_dependencies.dependent_projects.keys())}")
+        table.add_row(
+            "Dependent projects", f"{set(with_dependencies.dependent_projects.keys())}"
+        )
     console.print(table)
```

## mpyl/projects/find.py

```diff
@@ -2,42 +2,64 @@
 from pathlib import Path
 from typing import Optional
 
 from . import ProjectWithDependents, Protocol, Contract, Dependency
 from ..project import Project, load_project, Stage
 
 
-def load_projects(root_dir: Path, paths: list[str], strict: bool = False) -> set[Project]:
+def load_projects(
+    root_dir: Path, paths: list[str], strict: bool = False
+) -> set[Project]:
     return set(map(lambda p: load_project(root_dir, Path(p), strict), paths))
 
 
-def find_by_contract_dep(dep: str, projects: list[ProjectWithDependents]) -> Optional[ProjectWithDependents]:
+def find_by_contract_dep(
+    dep: str, projects: list[ProjectWithDependents]
+) -> Optional[ProjectWithDependents]:
     for project in projects:
-        if project.project.root_path.replace('./', '') in dep:
+        if project.project.root_path.replace("./", "") in dep:
             return project
     return None
 
 
-def find_dependencies(project: Project, other_projects: set[Project]) -> ProjectWithDependents:
+def find_dependencies(
+    project: Project, other_projects: set[Project]
+) -> ProjectWithDependents:
     mapped = list(map(lambda p: ProjectWithDependents(p, {}), other_projects))
 
-    def recursively_find(proj: ProjectWithDependents, other: list[ProjectWithDependents], discovery_stack: list[str]):
+    def recursively_find(
+        proj: ProjectWithDependents,
+        other: list[ProjectWithDependents],
+        discovery_stack: list[str],
+    ):
         dependent_projects = {}
-        for dep in proj.project.dependencies.set_for_stage(Stage.TEST) if proj.project.dependencies else set():
+        for dep in (
+            proj.project.dependencies.set_for_stage(Stage.TEST)
+            if proj.project.dependencies
+            else set()
+        ):
             found = find_by_contract_dep(dep, other)
             if found:
                 if found.name not in discovery_stack:
                     discovery_stack.append(found.name)
                     recursively_find(found, other, discovery_stack[:])
-                    dependent_projects[found.name] = Dependency(found.project, {Contract(Protocol.UNKNOWN, dep)})
+                    dependent_projects[found.name] = Dependency(
+                        found.project, {Contract(Protocol.UNKNOWN, dep)}
+                    )
                 elif found.name in dependent_projects:
-                    dependent_projects[found.name].contracts.add(Contract(Protocol.UNKNOWN, dep))
+                    dependent_projects[found.name].contracts.add(
+                        Contract(Protocol.UNKNOWN, dep)
+                    )
 
         proj.dependent_projects = dependent_projects
         return proj
 
-    return recursively_find(ProjectWithDependents(project=project, dependent_projects={}), mapped, [])
+    return recursively_find(
+        ProjectWithDependents(project=project, dependent_projects={}), mapped, []
+    )
 
 
-def find_all_dependencies(root_dir: Path, paths: list[str]) -> list[ProjectWithDependents]:
+def find_all_dependencies(
+    root_dir: Path, paths: list[str]
+) -> list[ProjectWithDependents]:
     projects = load_projects(root_dir, paths)
     return list(map(lambda p: find_dependencies(p, projects), projects))
```

## mpyl/reporting/formatting/markdown.py

```diff
@@ -7,92 +7,104 @@
 from junitparser import TestSuite
 
 from ...project import Stage, Project
 from ...steps import Output, ArtifactType
 from ...steps.models import Artifact
 from ...steps.run import RunResult
 from ...steps.steps import StepResult
-from ...utilities.junit import TestRunSummary, sum_suites, TEST_RESULTS_URL_KEY, TEST_RESULTS_URL_NAME_KEY, \
-    to_test_suites
+from ...utilities.junit import (
+    TestRunSummary,
+    sum_suites,
+    TEST_RESULTS_URL_KEY,
+    TEST_RESULTS_URL_NAME_KEY,
+    to_test_suites,
+)
 
 
 def summary_to_markdown(summary: TestRunSummary):
-    return f"🧪 {summary.tests} ❌ {summary.failures} " \
-           f"💔 {summary.errors} 🙈 {summary.skipped}"
+    return (
+        f"🧪 {summary.tests} ❌ {summary.failures} "
+        f"💔 {summary.errors} 🙈 {summary.skipped}"
+    )
 
 
 def __add_link_if_service(name: str, output: Output) -> str:
-    if output.produced_artifact and output.produced_artifact.artifact_type == ArtifactType.DEPLOYED_HELM_APP:
-        url = output.produced_artifact.spec.get('url')
+    if (
+        output.produced_artifact
+        and output.produced_artifact.artifact_type == ArtifactType.DEPLOYED_HELM_APP
+    ):
+        url = output.produced_artifact.spec.get("url")
         if url:
-            return f'[{name}]({url})'
+            return f"[{name}]({url})"
 
     return name
 
 
 def wrap_project_name(proj: Project, result: list[StepResult]):
     project_name = proj.name
-    encapsulation = '_'
+    encapsulation = "_"
     found_result = next((r for r in result if r.project.name == project_name), None)
     if found_result:
         project_name = __add_link_if_service(project_name, found_result.output)
-        encapsulation = '*' if found_result.output.success else '~~'
+        encapsulation = "*" if found_result.output.success else "~~"
 
-    return f'{encapsulation}{project_name}{encapsulation}'
+    return f"{encapsulation}{project_name}{encapsulation}"
 
 
 def __to_oneliner(result: list[StepResult], plan: set[Project]) -> str:
     project_names: list[str] = []
     if plan:
-        sorted_plan = sorted(plan, key=operator.attrgetter('name'))
+        sorted_plan = sorted(plan, key=operator.attrgetter("name"))
         for proj in sorted_plan:
             project_names.append(wrap_project_name(proj, result))
     else:
-        project_names = list(map(lambda r: f'_{r.project.name}_', result))
+        project_names = list(map(lambda r: f"_{r.project.name}_", result))
 
     return f'{", ".join(project_names)}'
 
 
 def stage_to_icon(stage: Stage):
     if stage == Stage.BUILD:
-        return '🏗️'
+        return "🏗️"
     if stage == Stage.TEST:
-        return '📋'
+        return "📋"
     if stage == Stage.DEPLOY:
-        return '🚀'
+        return "🚀"
     if stage == Stage.POST_DEPLOY:
-        return '🦺'
-    return '➡️'
+        return "🦺"
+    return "➡️"
 
 
 def markdown_for_stage(run_result: RunResult, stage: Stage):
     step_results: list[StepResult] = run_result.results_for_stage(stage)
     plan: set[Project] = run_result.plan_for_stage(stage)
     if not step_results and not plan:
-        return ''
+        return ""
 
     result = f"{stage_to_icon(stage)} {__to_oneliner(step_results, plan)}  \n"
     test_artifacts = _collect_test_artifacts(step_results)
     test_results = _collect_test_results(test_artifacts)
 
     if test_results:
         result += to_markdown_test_report(test_results)
         unique_artifacts = _collect_unique_test_artifacts_with_url(test_artifacts)
 
         for unique_artifact in unique_artifacts:
-            result += f' [{unique_artifact.spec[TEST_RESULTS_URL_NAME_KEY]}]' \
-                      f'({unique_artifact.spec[TEST_RESULTS_URL_KEY]})'
+            result += (
+                f" [{unique_artifact.spec[TEST_RESULTS_URL_NAME_KEY]}]"
+                f"({unique_artifact.spec[TEST_RESULTS_URL_KEY]})"
+            )
 
-        result += '  \n'
+        result += "  \n"
 
     return result
 
 
 def run_result_to_markdown(run_result: RunResult) -> str:
-    result: str = f'{run_result.status_line}  \n'
+    result: str = f"{run_result.status_line}  \n"
     exception = run_result.exception
     if exception:
         result += f"For _{exception.executor}_ on _{exception.project_name}_ at _{exception.stage}_ \n"
         result += f"\n\n{exception}\n\n"
     elif run_result.failed_result:
         failed = run_result.failed_result
         result += f"For _{failed.project.name}_ at _{failed.stage}_ \n"
@@ -106,31 +118,50 @@
 
 def to_markdown_test_report(suites: list[TestSuite]):
     total_tests = sum_suites(suites)
     return f"{summary_to_markdown(total_tests)}"
 
 
 def _collect_test_artifacts(step_results: list[StepResult]) -> list[Artifact]:
-    return [res.output.produced_artifact for res in step_results if
-            (res.output.produced_artifact and
-             res.output.produced_artifact.artifact_type == ArtifactType.JUNIT_TESTS)]
+    return [
+        res.output.produced_artifact
+        for res in step_results
+        if (
+            res.output.produced_artifact
+            and res.output.produced_artifact.artifact_type == ArtifactType.JUNIT_TESTS
+        )
+    ]
 
 
 def _collect_test_results(test_artifacts: list[Artifact]) -> list[TestSuite]:
     suites: list[list[TestSuite]] = list(map(to_test_suites, test_artifacts))
 
     return list(itertools.chain(*suites))
 
 
-def _collect_unique_test_artifacts_with_url(test_artifacts: list[Artifact]) -> list[Artifact]:
+def _collect_unique_test_artifacts_with_url(
+    test_artifacts: list[Artifact],
+) -> list[Artifact]:
     unique_artifacts: list[Artifact] = []
     for test_artifact in test_artifacts:
-        if TEST_RESULTS_URL_KEY in test_artifact.spec and test_artifact.spec[TEST_RESULTS_URL_KEY] != '':
-            duplicate_artifact = next((x for x in unique_artifacts if
-                                       x.spec[TEST_RESULTS_URL_KEY] == test_artifact.spec[TEST_RESULTS_URL_KEY]), None)
+        if (
+            TEST_RESULTS_URL_KEY in test_artifact.spec
+            and test_artifact.spec[TEST_RESULTS_URL_KEY] != ""
+        ):
+            duplicate_artifact = next(
+                (
+                    x
+                    for x in unique_artifacts
+                    if x.spec[TEST_RESULTS_URL_KEY]
+                    == test_artifact.spec[TEST_RESULTS_URL_KEY]
+                ),
+                None,
+            )
             if not duplicate_artifact:
-                test_artifact.spec[TEST_RESULTS_URL_NAME_KEY] = test_artifact.producing_step
+                test_artifact.spec[
+                    TEST_RESULTS_URL_NAME_KEY
+                ] = test_artifact.producing_step
                 unique_artifacts.append(test_artifact)
             else:
-                duplicate_artifact.spec[TEST_RESULTS_URL_NAME_KEY] = 'link'
+                duplicate_artifact.spec[TEST_RESULTS_URL_NAME_KEY] = "link"
 
     return unique_artifacts
```

## mpyl/reporting/formatting/text.py

```diff
@@ -20,15 +20,15 @@
                 if artifact and artifact.artifact_type == ArtifactType.JUNIT_TESTS:
                     result += to_test_report(artifact)
 
     return result
 
 
 def to_test_report(artifact: Artifact) -> str:
-    """ Gather the first test suites and test cases. Output is truncated to around 200 lines to not overwhelm Github """
+    """Gather the first test suites and test cases. Output is truncated to around 200 lines to not overwhelm Github"""
     test_result = []
     suites = to_test_suites(artifact)
     total_tests = sum_suites(suites)
     test_result.append(f"{total_tests} \n\n")
     for suite in suites:
         test_result.append(f"Suite {suite.name}\n")
         if len(test_result) > 200:
```

## mpyl/reporting/targets/__init__.py

```diff
@@ -26,16 +26,20 @@
         self.outcomes = []
 
     def add(self, outcome: ReportOutcome):
         self.outcomes.append(outcome)
 
     @property
     def failures(self) -> list[str]:
-        return [f'{type(outcome).__name__} failed with exception {outcome.exception}' for outcome in self.outcomes if
-                not outcome.success]
+        return [
+            f"{type(outcome).__name__} failed with exception {outcome.exception}"
+            for outcome in self.outcomes
+            if not outcome.success
+        ]
 
 
 class Reporter:
-
     @abstractmethod
-    def send_report(self, results: RunResult, text: Optional[str] = None) -> ReportOutcome:
+    def send_report(
+        self, results: RunResult, text: Optional[str] = None
+    ) -> ReportOutcome:
         pass
```

## mpyl/reporting/targets/github.py

```diff
@@ -48,42 +48,50 @@
 from ...reporting.formatting.text import to_string
 from ...steps.models import RunProperties
 from ...steps.run import RunResult
 from ...utilities.github import GithubConfig, get_pr_for_branch, GithubAppConfig
 from ...utilities.repo import Repository, RepoConfig
 
 
-def compose_message_body(results: RunResult, _unused_config: Optional[Dict] = None) -> str:
+def compose_message_body(
+    results: RunResult, _unused_config: Optional[Dict] = None
+) -> str:
     return run_result_to_markdown(results)
 
 
 class GithubOutcome(ReportOutcome):
     pass
 
 
 class GithubUpdateStategy(Enum):
-    BODY = 'body'
-    COMMENT = 'comment'
+    BODY = "body"
+    COMMENT = "comment"
 
 
 class PullRequestReporter(Reporter):
     _config: GithubConfig
 
-    def __init__(self, config: Dict,
-                 compose_function: Callable[[RunResult, Optional[Dict]], str] = compose_message_body,
-                 update_stategy: GithubUpdateStategy = GithubUpdateStategy.BODY):
+    def __init__(
+        self,
+        config: Dict,
+        compose_function: Callable[
+            [RunResult, Optional[Dict]], str
+        ] = compose_message_body,
+        update_stategy: GithubUpdateStategy = GithubUpdateStategy.BODY,
+    ):
         self._raw_config = config
         self._config = GithubConfig.from_config(config)
         self.git_repository = Repository(RepoConfig.from_config(config))
         self.compose_function = compose_function
         self.update_strategy: GithubUpdateStategy = update_stategy
-
         self.body_separator = "----"
 
-    def _get_pull_request(self, repo: GithubRepository, run_properties: RunProperties) -> Optional[PullRequest]:
+    def _get_pull_request(
+        self, repo: GithubRepository, run_properties: RunProperties
+    ) -> Optional[PullRequest]:
         if run_properties.versioning.pr_number:
             return repo.get_pull(run_properties.versioning.pr_number)
 
         current_branch = self.git_repository.get_branch
         if current_branch:
             return get_pr_for_branch(repo, current_branch)
         return None
@@ -91,40 +99,47 @@
     def _update_pr(self) -> Callable[[PullRequest, RunResult], None]:
         if self.update_strategy == GithubUpdateStategy.COMMENT:
             return self._change_pr_comment
         return self._change_pr_body
 
     def _extract_pr_header(self, current_body: Optional[str]) -> str:
         body_header = current_body.split(self.body_separator)[0] if current_body else ""
-        return body_header.rstrip("\n") + f"\n{self.body_separator}\n"
+        return body_header.rstrip("\n") + f"\n\n{self.body_separator}\n"
 
     def _change_pr_body(self, pull_request: PullRequest, results: RunResult):
         pull_request.edit(
-            body=self._extract_pr_header(pull_request.body) + self.compose_function(results, self._raw_config)
+            body=self._extract_pr_header(pull_request.body)
+            + self.compose_function(results, self._raw_config)
         )
 
     def _change_pr_comment(self, pull_request: PullRequest, results: RunResult):
         github = Github(self._config.token)
         comments = pull_request.get_issue_comments()
         authenticated_user = github.get_user()
         comments_for_user = [c for c in comments if c.user.id == authenticated_user.id]
         if comments_for_user:
             comment_to_update: IssueComment = comments_for_user.pop()
             comment_to_update.edit(self.compose_function(results, self._raw_config))
         else:
-            pull_request.create_issue_comment(self.compose_function(results, self._raw_config))
-
-    def send_report(self, results: RunResult, text: Optional[str] = None) -> GithubOutcome:
+            pull_request.create_issue_comment(
+                self.compose_function(results, self._raw_config)
+            )
+
+    def send_report(
+        self, results: RunResult, text: Optional[str] = None
+    ) -> GithubOutcome:
         try:
             github = Github(self._config.token)
             repo = github.get_repo(self._config.repository)
 
             pull_request = self._get_pull_request(repo, results.run_properties)
             if not pull_request:
-                return GithubOutcome(success=False, exception=Exception('No pull request found'))
+                return GithubOutcome(
+                    success=False, exception=Exception("No pull request found")
+                )
 
             self._update_pr()(pull_request, results)
             return GithubOutcome(success=True)
         except GithubException as exc:
             return GithubOutcome(success=False, exception=exc)
 
 
@@ -137,40 +152,66 @@
         self._github_config = GithubConfig.from_config(config)
         self._check_run_id = None
         self._logger = logger
 
     @staticmethod
     def _to_output(results: RunResult) -> dict:
         build_id = results.run_properties.details.build_id
-        summary = ':white_check_mark: Build successful' if results.is_success else ':x: Build failed'
-        return {'title': f'Build {build_id}', 'summary': summary + '\n' + run_result_to_markdown(results),
-                'text': to_string(results)}
-
-    def send_report(self, results: RunResult, text: Optional[str] = None) -> GithubOutcome:
+        summary = (
+            ":white_check_mark: Build successful"
+            if results.is_success
+            else ":x: Build failed"
+        )
+        return {
+            "title": f"Build {build_id}",
+            "summary": summary + "\n" + run_result_to_markdown(results),
+            "text": to_string(results),
+        }
+
+    def send_report(
+        self, results: RunResult, text: Optional[str] = None
+    ) -> GithubOutcome:
         try:
             config: GithubAppConfig = self._github_config.get_app_config
             if not config:
                 raise KeyError("github.app config needs to be defined")
 
-            private_key = Path(config.private_app_key_path or '').read_text(
-                encoding='utf-8') if config.private_app_key_path else base64.b64decode(
-                config.private_key_base_64_encoded or '').decode('utf-8')
-
-            integration = GithubIntegration(integration_id=config.app_key, private_key=private_key)
-
-            install = integration.get_installation(self._github_config.owner, self._github_config.repo_name)
+            private_key = (
+                Path(config.private_app_key_path or "").read_text(encoding="utf-8")
+                if config.private_app_key_path
+                else base64.b64decode(config.private_key_base_64_encoded or "").decode(
+                    "utf-8"
+                )
+            )
+
+            integration = GithubIntegration(
+                integration_id=config.app_key, private_key=private_key
+            )
+
+            install = integration.get_installation(
+                self._github_config.owner, self._github_config.repo_name
+            )
             access_token = integration.get_access_token(install.id)
             github = Github(login_or_token=access_token.token)
             repo = github.get_repo(self._github_config.repository)
             if self._check_run_id and results:
                 run = repo.get_check_run(self._check_run_id)
-                conclusion = 'success' if results is None or results.is_success else 'failure'
-                self._logger.info(f'Setting check to {conclusion}')
-                run.edit(completed_at=datetime.now(), conclusion=conclusion, output=self._to_output(results))
+                conclusion = (
+                    "success" if results is None or results.is_success else "failure"
+                )
+                self._logger.info(f"Setting check to {conclusion}")
+                run.edit(
+                    completed_at=datetime.now(),
+                    conclusion=conclusion,
+                    output=self._to_output(results),
+                )
             else:
                 with Repository(RepoConfig.from_config(self._config)) as git_repository:
-                    self._check_run_id = repo.create_check_run(name='Pipeline build', head_sha=git_repository.get_sha,
-                                                               status='in_progress').id
+                    self._check_run_id = repo.create_check_run(
+                        name="Pipeline build",
+                        head_sha=git_repository.get_sha,
+                        status="in_progress",
+                    ).id
             return GithubOutcome(success=True)
         except GithubException as exc:
-            self._logger.warning(f'Unexpected exception: {exc}', exc_info=True)
+            self._logger.warning(f"Unexpected exception: {exc}", exc_info=True)
             return GithubOutcome(success=False, exception=exc)
```

## mpyl/reporting/targets/jira.py

```diff
@@ -49,28 +49,36 @@
     status_name: str
     user_avatar: str
     user_email: str
     assignee_email: Optional[str]
 
     @staticmethod
     def from_issue_response(response):
-        jira_url = "{uri.scheme}://{uri.netloc}".format(uri=urlsplit(response['self']))
-        fields = response['fields']
-        ticket_id = response['key']
-        assignee = fields.get('assignee')
-        user = assignee or fields.get('reporter') or fields.get('creator')
-        avatar = user['avatarUrls']['24x24'] if user else ''
-        status_name = fields['status']['name']
-        assignee_email = assignee['emailAddress'] if assignee else None
+        jira_url = "{uri.scheme}://{uri.netloc}".format(uri=urlsplit(response["self"]))
+        fields = response["fields"]
+        ticket_id = response["key"]
+        assignee = fields.get("assignee")
+        user = assignee or fields.get("reporter") or fields.get("creator")
+        avatar = user["avatarUrls"]["24x24"] if user else ""
+        status_name = fields["status"]["name"]
+        assignee_email = assignee["emailAddress"] if assignee else None
         ticket_url = f"{jira_url}/browse/{ticket_id}"
 
-        return JiraTicket(jira_url=jira_url, ticket_id=ticket_id, ticket_url=ticket_url,
-                          issue_type=fields['issuetype']['name'], summary=fields['summary'], status_name=status_name,
-                          description=fields['description'], user_avatar=avatar, user_email=user['emailAddress'],
-                          assignee_email=assignee_email)
+        return JiraTicket(
+            jira_url=jira_url,
+            ticket_id=ticket_id,
+            ticket_url=ticket_url,
+            issue_type=fields["issuetype"]["name"],
+            summary=fields["summary"],
+            status_name=status_name,
+            description=fields["description"],
+            user_avatar=avatar,
+            user_email=user["emailAddress"],
+            assignee_email=assignee_email,
+        )
 
 
 def extract_ticket_from_branch(branch: str, pattern: Pattern) -> Optional[str]:
     ticket: Optional[str] = next(iter(re.findall(pattern, branch)), None)
     if ticket:
         return ticket.upper()
     return None
@@ -82,106 +90,136 @@
     user_name: str
     password: str
     ticket_pattern: Pattern
     token: Optional[str]
 
     @staticmethod
     def from_config(config: dict):
-        jira_config = config.get('jira')
+        jira_config = config.get("jira")
         if not jira_config:
-            raise KeyError(f'jira section needs to be defined in {DEFAULT_CONFIG_FILE_NAME}')
-        return JiraConfig(site=jira_config['site'], user_name=jira_config['userName'], password=jira_config['password'],
-                          ticket_pattern=re.compile(jira_config.get('ticketPattern', '[A-Za-z]{2,}-\\d+')),
-                          token=jira_config.get('token'))
+            raise KeyError(
+                f"jira section needs to be defined in {DEFAULT_CONFIG_FILE_NAME}"
+            )
+        return JiraConfig(
+            site=jira_config["site"],
+            user_name=jira_config["userName"],
+            password=jira_config["password"],
+            ticket_pattern=re.compile(
+                jira_config.get("ticketPattern", "[A-Za-z]{2,}-\\d+")
+            ),
+            token=jira_config.get("token"),
+        )
 
 
 def create_jira_for_config(jira_config: JiraConfig):
-    return Jira(
-        url=jira_config.site,
-        token=jira_config.token,
-        api_version='2',
-        cloud=True
-    ) if jira_config.token else Jira(
-        url=jira_config.site,
-        username=jira_config.user_name,
-        password=jira_config.password,
-        api_version='2',
-        cloud=True
+    return (
+        Jira(url=jira_config.site, token=jira_config.token, api_version="2", cloud=True)
+        if jira_config.token
+        else Jira(
+            url=jira_config.site,
+            username=jira_config.user_name,
+            password=jira_config.password,
+            api_version="2",
+            cloud=True,
+        )
     )
 
 
 def to_github_markdown(jira_markdown: str, jira_url: str) -> str:
-    jira_markdown = re.sub(r'\[(.*)/(.*)\|(.*)\|smart-link\]', r'[\2](\3)', jira_markdown)
-    jira_markdown = re.sub(r'\[(.*)\|(.*)\]', r'[\1](\2)', jira_markdown)
-    jira_markdown = re.sub(r'\[~accountid:(.*)\]', rf'[👩‍💻]({jira_url}/jira/people/\1)', jira_markdown)
-    jira_markdown = re.sub(r'\{\{(.*)\}\}', r'`\1`', jira_markdown)
-    jira_markdown = re.sub(r'\{quote}(.*)\{quote}', r'> \1', jira_markdown)
-    jira_markdown = re.sub(r'\{noformat\}((.|\n)*)\{noformat\}', r'```\n\1\n```', jira_markdown)
-    jira_markdown = re.sub(r'\{code:+(.*)\}((.|\n)*)\{code\}', r'```\1\n\2\n```', jira_markdown)
-    jira_markdown = re.sub(r'\{noformat\}((.|\n)*)', r'```\n\1\n```', jira_markdown)
-    jira_markdown = re.sub(r'\*(.*)\*', r'**\1**', jira_markdown)
-    jira_markdown = re.sub(r'_(.*)_', r'*\1*', jira_markdown)
-    jira_markdown = re.sub(r'!.*\|.*!', r'', jira_markdown)
-
-    jira_markdown = jira_markdown.replace('# ', '- ')
-    jira_markdown = jira_markdown.replace('h1. ', '### ')
-    jira_markdown = jira_markdown.replace('h2. ', '#### ')
-    jira_markdown = jira_markdown.replace('h3. ', '##### ')
-    jira_markdown = jira_markdown.replace('h4. ', '###### ')
-    jira_markdown = jira_markdown.replace('h5. ', '###### ')
-    jira_markdown = jira_markdown.replace('h6. ', '###### ')
+    jira_markdown = re.sub(
+        r"\[(.*)/(.*)\|(.*)\|smart-link\]", r"[\2](\3)", jira_markdown
+    )
+    jira_markdown = re.sub(r"\[(.*)\|(.*)\]", r"[\1](\2)", jira_markdown)
+    jira_markdown = re.sub(
+        r"\[~accountid:(.*)\]", rf"[👩‍💻]({jira_url}/jira/people/\1)", jira_markdown
+    )
+    jira_markdown = re.sub(r"\{\{(.*)\}\}", r"`\1`", jira_markdown)
+    jira_markdown = re.sub(r"\{quote}(.*)\{quote}", r"> \1", jira_markdown)
+    jira_markdown = re.sub(
+        r"\{noformat\}((.|\n)*)\{noformat\}", r"```\n\1\n```", jira_markdown
+    )
+    jira_markdown = re.sub(
+        r"\{code:+(.*)\}((.|\n)*)\{code\}", r"```\1\n\2\n```", jira_markdown
+    )
+    jira_markdown = re.sub(r"\{noformat\}((.|\n)*)", r"```\n\1\n```", jira_markdown)
+    jira_markdown = re.sub(r"\*(.*)\*", r"**\1**", jira_markdown)
+    jira_markdown = re.sub(r"_(.*)_", r"*\1*", jira_markdown)
+    jira_markdown = re.sub(r"!.*\|.*!", r"", jira_markdown)
+
+    jira_markdown = jira_markdown.replace("# ", "- ")
+    jira_markdown = jira_markdown.replace("h1. ", "### ")
+    jira_markdown = jira_markdown.replace("h2. ", "#### ")
+    jira_markdown = jira_markdown.replace("h3. ", "##### ")
+    jira_markdown = jira_markdown.replace("h4. ", "###### ")
+    jira_markdown = jira_markdown.replace("h5. ", "###### ")
+    jira_markdown = jira_markdown.replace("h6. ", "###### ")
     return jira_markdown
 
 
 def to_markdown_summary(ticket: JiraTicket, run_result: RunResult) -> str:
-    description_markdown = to_github_markdown(ticket.description, ticket.ticket_url) if ticket.description else ""
+    description_markdown = (
+        to_github_markdown(ticket.description, ticket.ticket_url)
+        if ticket.description
+        else ""
+    )
     lines = description_markdown.splitlines()
     max_message_length = 288
     if len(lines) > max_message_length:
         description_markdown = "\n".join(lines[:max_message_length]) + "\n..."
 
     details = run_result.run_properties.details
 
-    build_status = f"🏗️ Build [{details.build_id}]({details.run_url}) {run_result.status_line}, " \
-                   f"started by _{details.user}_  \n{markdown_for_stage(run_result, Stage.DEPLOY)}"
-    return f"📕 [{ticket.ticket_id}]({ticket.ticket_url}) {ticket.summary} " \
-           f'<img src="{ticket.user_avatar}" width="24" height="24" alt="{ticket.user_email}" /> \n' \
-           f"{description_markdown}\n\n" \
-           f"{build_status}"
+    build_status = (
+        f"🏗️ Build [{details.build_id}]({details.run_url}) {run_result.status_line}, "
+        f"started by _{details.user}_  \n{markdown_for_stage(run_result, Stage.DEPLOY)}"
+    )
+    return (
+        f"### 📕 [{ticket.ticket_id}]({ticket.ticket_url}) {ticket.summary} "
+        f'<img src="{ticket.user_avatar}" width="24" height="24" alt="{ticket.user_email}" /> \n'
+        f"{description_markdown}\n\n"
+        f"{build_status}"
+    )
 
 
 def compose_build_status(result: RunResult, config: dict) -> str:
     jira_config = JiraConfig.from_config(config=config)
     jira_client = create_jira_for_config(jira_config)
     branch = result.run_properties.versioning.branch
     if not branch:
         return " # ⚠️ `versioning.branch` not set, cannot find corresponding ticket"
     ticket_id = extract_ticket_from_branch(branch, jira_config.ticket_pattern)
     if not ticket_id:
-        return f" # ⚠️ Could not find ticket corresponding to `{branch}. " \
-               f"Does your branch name follow the correct pattern?"
+        return (
+            f" # ⚠️ Could not find ticket corresponding to `{branch}. "
+            f"Does your branch name follow the correct pattern?"
+        )
     issue = jira_client.get_issue(ticket_id)
     jira_ticket = JiraTicket.from_issue_response(issue)
     return to_markdown_summary(jira_ticket, result)
 
 
 class JiraOutcome(ReportOutcome):
     pass
 
 
 class JiraReporter(Reporter):
-
     def __init__(self, config: dict, branch: str, logger: Logger):
         jira_config = JiraConfig.from_config(config)
-        self._ticket = extract_ticket_from_branch(branch, jira_config.ticket_pattern) if branch else None
+        self._ticket = (
+            extract_ticket_from_branch(branch, jira_config.ticket_pattern)
+            if branch
+            else None
+        )
         self._config = jira_config
         self._jira = create_jira_for_config(jira_config)
         self._logger = logger
 
-    def send_report(self, results: RunResult, text: Optional[str] = None) -> JiraOutcome:
+    def send_report(
+        self, results: RunResult, text: Optional[str] = None
+    ) -> JiraOutcome:
         if not self._ticket:
             return JiraOutcome(success=True)
 
         try:
             issue_response = self._jira.get_issue(self._ticket)
 
             ticket = JiraTicket.from_issue_response(issue_response)
@@ -190,26 +228,26 @@
 
             user_email = results.run_properties.details.user_email
             if user_email:
                 self.__assign_ticket(user_email, ticket)
             return JiraOutcome(success=True)
 
         except requests.exceptions.HTTPError as exc:
-            self._logger.warning(f'Could not handle Jira ticket {self._ticket}: {exc}')
+            self._logger.warning(f"Could not handle Jira ticket {self._ticket}: {exc}")
             return JiraOutcome(success=False, exception=exc)
 
     def __assign_ticket(self, run_user_email: str, ticket: JiraTicket):
         if ticket.assignee_email is None:
             jira_user = self._jira.user_find_by_user_string(query=run_user_email)
             if jira_user:
-                account_id = jira_user.pop().get('accountId')
-                self._logger.info(f'Assigning {ticket.ticket_id} to {account_id}')
+                account_id = jira_user.pop().get("accountId")
+                self._logger.info(f"Assigning {ticket.ticket_id} to {account_id}")
                 self._jira.assign_issue(self._ticket, account_id=account_id)
 
     def __move_ticket_forward(self, ticket: JiraTicket):
         transitions = self._jira.get_issue_transitions(self._ticket)
         for idx, transition in enumerate(transitions):
-            if transition['name'] == ticket.status_name:
+            if transition["name"] == ticket.status_name:
                 if idx == 0:
-                    target_state = transitions[idx + 1]['name']
-                    self._logger.info(f'Moving {ticket.ticket_id} to {target_state}')
+                    target_state = transitions[idx + 1]["name"]
+                    self._logger.info(f"Moving {ticket.ticket_id} to {target_state}")
                     self._jira.issue_transition(self._ticket, target_state)
```

## mpyl/reporting/targets/slack.py

```diff
@@ -32,32 +32,39 @@
 """
 import re
 from dataclasses import dataclass
 from typing import Dict, Optional
 
 from slack_sdk import WebClient
 from slack_sdk.errors import SlackClientError, SlackApiError
-from slack_sdk.models.blocks import HeaderBlock, SectionBlock, MarkdownTextObject, ContextBlock, ImageElement, Block
+from slack_sdk.models.blocks import (
+    HeaderBlock,
+    SectionBlock,
+    MarkdownTextObject,
+    ContextBlock,
+    ImageElement,
+    Block,
+)
 
 from . import Reporter, ReportOutcome
 from ..formatting.markdown import run_result_to_markdown
 from ...steps.models import RunProperties
 from ...steps.run import RunResult
 
 
 def to_slack_markdown(markdown: str) -> str:
     regex_replace = (
-        (re.compile(r'\[(.*?)\]\((.*?)\)'), r'<\2|\1>'),
-        (re.compile(r'^- ', flags=re.M), '• '),
-        (re.compile(r'^  - ', flags=re.M), '  ◦ '),
-        (re.compile(r'^    - ', flags=re.M), '    ⬩ '),
-        (re.compile(r'^      - ', flags=re.M), '    ◽ '),
-        (re.compile(r'^#+ (.+)$', flags=re.M), r'*\1*'),
-        (re.compile(r'\*\*'), '*'),
-        (re.compile(r'~~'), '~'),
+        (re.compile(r"\[(.*?)\]\((.*?)\)"), r"<\2|\1>"),
+        (re.compile(r"^- ", flags=re.M), "• "),
+        (re.compile(r"^  - ", flags=re.M), "  ◦ "),
+        (re.compile(r"^    - ", flags=re.M), "    ⬩ "),
+        (re.compile(r"^      - ", flags=re.M), "    ◽ "),
+        (re.compile(r"^#+ (.+)$", flags=re.M), r"*\1*"),
+        (re.compile(r"\*\*"), "*"),
+        (re.compile(r"~~"), "~"),
     )
     for pattern, replacement in regex_replace:
         markdown = re.sub(pattern, replacement, markdown)
     return markdown
 
 
 @dataclass(frozen=True)
@@ -84,105 +91,160 @@
     pass
 
 
 class SlackReporter(Reporter):
     _icons: SlackIcons
     _message_identifier: Optional[MessageIdentifier]
 
-    def __init__(self,
-                 config: Dict,
-                 channel: Optional[str],
-                 versioning_identifier: str,
-                 target: str,
-                 message_identifier: Optional[MessageIdentifier] = None):
-
-        slack_config = config.get('slack')
+    def __init__(
+        self,
+        config: Dict,
+        channel: Optional[str],
+        versioning_identifier: str,
+        target: str,
+        message_identifier: Optional[MessageIdentifier] = None,
+    ):
+        slack_config = config.get("slack")
         if not slack_config:
-            raise ValueError('slack config not set')
-        self._client = WebClient(token=slack_config['botToken'])
+            raise ValueError("slack config not set")
+        self._client = WebClient(token=slack_config["botToken"])
         self._channel = channel
-        self._title = f'MPyL run for {versioning_identifier} on {target}'
-        icons = slack_config['icons']
-        self._icons = SlackIcons(success=icons['success'], failure=icons['failure'], building=icons['building'])
+        self._title = f"MPyL run for {versioning_identifier} on {target}"
+        icons = slack_config["icons"]
+        self._icons = SlackIcons(
+            success=icons["success"],
+            failure=icons["failure"],
+            building=icons["building"],
+        )
         self._message_identifier = message_identifier
 
-    def send_report(self, results: RunResult, text: Optional[str] = None) -> ReportOutcome:
+    def send_report(
+        self, results: RunResult, text: Optional[str] = None
+    ) -> ReportOutcome:
         try:
-            user_info = self.__get_user_info(results.run_properties.details.user_email)
+            email = results.run_properties.details.user_email
+            user_info = self.__get_user_info(email)
 
             if not self._channel and user_info.initiator:
                 self._channel = self.__open_conversation_with_user(user_info.initiator)
 
             if not self._channel:
-                raise ValueError('Channel not explicitly set and initiator could not be determined')
+                return SlackOutcome(
+                    success=False,
+                    exception=ValueError(
+                        f"Channel not explicitly set and initiator for {email} could not be determined"
+                    ),
+                )
 
             body = to_slack_markdown(text if text else run_result_to_markdown(results))
             blocks = self.__compose_blocks(results, body, user_info)
 
             if self._message_identifier:
-                self._client.chat_update(channel=self._message_identifier.channel_id,
-                                         ts=self._message_identifier.time_stamp,
-                                         icon_emoji=':robot_face:', mrkdwn=True, blocks=blocks, text=body)
+                self._client.chat_update(
+                    channel=self._message_identifier.channel_id,
+                    ts=self._message_identifier.time_stamp,
+                    icon_emoji=":robot_face:",
+                    mrkdwn=True,
+                    blocks=blocks,
+                    text=body,
+                )
                 return SlackOutcome(success=True)
 
-            response = self._client.chat_postMessage(channel=self._channel, icon_emoji=':robot_face:', mrkdwn=True,
-                                                     blocks=blocks, text=body)
-            self._message_identifier = MessageIdentifier(channel_id=response['channel'], time_stamp=response['ts'])
+            response = self._client.chat_postMessage(
+                channel=self._channel,
+                icon_emoji=":robot_face:",
+                mrkdwn=True,
+                blocks=blocks,
+                text=body,
+            )
+            self._message_identifier = MessageIdentifier(
+                channel_id=response["channel"], time_stamp=response["ts"]
+            )
             return SlackOutcome(success=True)
         except SlackClientError as slack_exception:
             return SlackOutcome(success=False, exception=slack_exception)
 
     def send_progress_update(self, results: RunResult, text: Optional[str]):
         if not self._message_identifier:
-            raise ValueError('Message identifier not set. Cannot call update before `send_report` has been called')
+            raise ValueError(
+                "Message identifier not set. Cannot call update before `send_report` has been called"
+            )
 
         result_markdown = text if text else run_result_to_markdown(results)
         body = to_slack_markdown(result_markdown)
-        blocks = self.__compose_blocks(results, body, self.__get_user_info(results.run_properties.details.user_email))
-        self._client.chat_update(channel=self._message_identifier.channel_id, ts=self._message_identifier.time_stamp,
-                                 icon_emoji=':robot_face:', mrkdwn=True, blocks=blocks, text=body)
+        blocks = self.__compose_blocks(
+            results,
+            body,
+            self.__get_user_info(results.run_properties.details.user_email),
+        )
+        self._client.chat_update(
+            channel=self._message_identifier.channel_id,
+            ts=self._message_identifier.time_stamp,
+            icon_emoji=":robot_face:",
+            mrkdwn=True,
+            blocks=blocks,
+            text=body,
+        )
 
     def __open_conversation_with_user(self, user_id: str):
         opened_channel = self._client.conversations_open(users=[user_id])
-        return opened_channel['channel']['id']
+        return opened_channel["channel"]["id"]
 
     def __get_user_info(self, user_email: Optional[str]):
         profile_data: dict[str, str] = {}
         user_id = None
         if user_email:
             try:
                 user = self._client.users_lookupByEmail(email=user_email)
-                user_id = user['user']['id']
+                user_id = user["user"]["id"]
                 resp = self._client.users_profile_get(user=user_id)
-                profile_data = resp.get('profile', {})
+                profile_data = resp.get("profile", {})
             except SlackApiError:
                 profile_data = {}
 
-        return UserInfo(user_name=profile_data.get('real_name_normalized', 'Anonymous'),
-                        profile_image=profile_data.get('image_24',
-                                                       'https://avatars.githubusercontent.com/u/18010732'),
-                        initiator=user_id)
+        return UserInfo(
+            user_name=profile_data.get("real_name_normalized", "Anonymous"),
+            profile_image=profile_data.get(
+                "image_24", "https://avatars.githubusercontent.com/u/18010732"
+            ),
+            initiator=user_id,
+        )
 
     def __get_icon(self, results: RunResult):
         if results.is_in_progress:
             return self._icons.building
         if results.is_success:
             return self._icons.success
         return self._icons.failure
 
-    def __compose_blocks(self, results: RunResult, text: str, user_info: UserInfo) -> list[Block]:
+    def __compose_blocks(
+        self, results: RunResult, text: str, user_info: UserInfo
+    ) -> list[Block]:
         icon = self.__get_icon(results)
 
-        context = self.compose_context(results.run_properties, icon, user_info.user_name)
-        return [HeaderBlock(text=self._title),
-                SectionBlock(text=MarkdownTextObject(text=text)),
-                ContextBlock(elements=[MarkdownTextObject(text=context),
-                                       ImageElement(image_url=user_info.profile_image, alt_text=user_info.user_name)])
+        context = self.compose_context(
+            results.run_properties, icon, user_info.user_name
+        )
+        return [
+            HeaderBlock(text=self._title),
+            SectionBlock(text=MarkdownTextObject(text=text)),
+            ContextBlock(
+                elements=[
+                    MarkdownTextObject(text=context),
+                    ImageElement(
+                        image_url=user_info.profile_image, alt_text=user_info.user_name
+                    ),
                 ]
+            ),
+        ]
 
     @staticmethod
-    def compose_context(build_props: RunProperties, icon: str, user: Optional[str]) -> str:
+    def compose_context(
+        build_props: RunProperties, icon: str, user: Optional[str]
+    ) -> str:
         details = build_props.details
         user_name = user if user else details.user
-        return f":{icon}: Build <{details.run_url}|{details.build_id.upper()}> for " \
-               f"<{details.change_url}|{build_props.versioning.identifier.upper()}> " \
-               f"started by _{user_name}_"
+        return (
+            f":{icon}: Build <{details.run_url}|{details.build_id.upper()}> for "
+            f"<{details.change_url}|{build_props.versioning.identifier.upper()}> "
+            f"started by _{user_name}_"
+        )
```

## mpyl/schema/run_properties.schema.yml

```diff
@@ -47,25 +47,19 @@
             description: Email of of the user that triggered the run
             type: ["string", "null"]
             format: idn-email
       parameters:
         description: defines the run properties
         type: object
         additionalProperties: false
-        required:
-          - deploy_target
         properties:
           deploy_target:
             description: The deploy target.
-            type: string
-            enum:
-              - 'PullRequest'
-              - 'PullRequestBase'
-              - 'Acceptance'
-              - 'Production'
+            type: ["string", "null"]
+            enum: [ null,  'PullRequest', 'PullRequestBase', 'Production' ]
       console:
         type: object
         additionalProperties: false
         properties:
           width:
             description: "The width of the console in characters, 0 means no limit"
             type: integer
@@ -89,7 +83,18 @@
             type: ["string", "null"]
           pr_number:
             description: id of the pull request
             type: ["string", "null"]
           tag:
             description: reference that points to the MPyL version
             type: ["string", "null"]
+  stages:
+    description: defines stages in a run
+    type: array
+    items:
+      type: object
+      additionalProperties: false
+      properties:
+        name:
+          type: string
+        icon:
+          type: string
```

## mpyl/stages/discovery.py

```diff
@@ -18,15 +18,17 @@
     projects_to_deploy: set[Project]
 
 
 def is_invalidated(project: Project, stage: Stage, path: str) -> bool:
     deps = project.dependencies
     deps_for_stage = deps.set_for_stage(stage) if deps else {}
 
-    touched_dependency = next(filter(path.startswith, deps_for_stage), None) if deps else None
+    touched_dependency = (
+        next(filter(path.startswith, deps_for_stage), None) if deps else None
+    )
     startswith: bool = path.startswith(project.root_path)
     return startswith or touched_dependency is not None
 
 
 def output_invalidated(output: Optional[Output], revision_hash: str) -> bool:
     if output is None:
         return True
@@ -37,53 +39,78 @@
     artifact = output.produced_artifact
     if artifact.revision != revision_hash:
         return True
 
     return False
 
 
-def _to_relevant_changes(project: Project, stage: Stage, change_history: list[Revision]) -> set[str]:
+def _to_relevant_changes(
+    project: Project, stage: Stage, change_history: list[Revision]
+) -> set[str]:
     output: Output = Output.try_read(project.target_path, stage)
     relevant = set()
     for history in reversed(sorted(change_history, key=lambda c: c.ord)):
         if stage == Stage.DEPLOY or output_invalidated(output, history.hash):
             relevant.update(history.files_touched)
         else:
             return relevant
 
     return relevant
 
 
-def are_invalidated(project: Project, stage: Stage, change_history: list[Revision]) -> bool:
+def _are_invalidated(
+    project: Project, stage: Stage, change_history: list[Revision]
+) -> bool:
     if project.stages.for_stage(stage) is None:
         return False
 
     relevant_changes = _to_relevant_changes(project, stage, change_history)
-    return len(set(filter(lambda c: is_invalidated(project, stage, c), relevant_changes))) > 0
+    return (
+        len(set(filter(lambda c: is_invalidated(project, stage, c), relevant_changes)))
+        > 0
+    )
 
 
-def find_invalidated_projects_for_stage(all_projects: set[Project], stage: Stage,
-                                        change_history: list[Revision]) -> set[Project]:
-    return set(filter(lambda p: are_invalidated(p, stage, change_history), all_projects))
+def find_invalidated_projects_for_stage(
+    all_projects: set[Project], stage: Stage, change_history: list[Revision]
+) -> set[Project]:
+    return set(
+        filter(lambda p: _are_invalidated(p, stage, change_history), all_projects)
+    )
 
 
 def find_deploy_set(repo_config: RepoConfig, tag: Optional[str]) -> DeploySet:
     with Repository(repo_config) as repo:
-        changes_in_branch = repo.changes_in_tagged_commit(tag) if tag else repo.changes_in_branch_including_local()
+        changes_in_branch = (
+            repo.changes_in_tagged_commit(tag)
+            if tag
+            else repo.changes_in_branch_including_local()
+        )
         project_paths = repo.find_projects()
-        all_projects = set(map(lambda p: load_project(Path(""), Path(p), False), project_paths))
-        return DeploySet(all_projects,
-                         find_invalidated_projects_for_stage(all_projects, Stage.DEPLOY, changes_in_branch))
+        all_projects = set(
+            map(lambda p: load_project(Path(""), Path(p), False), project_paths)
+        )
+        return DeploySet(
+            all_projects,
+            find_invalidated_projects_for_stage(
+                all_projects, Stage.DEPLOY, changes_in_branch
+            ),
+        )
 
 
-def find_invalidated_projects_per_stage(all_projects: set[Project], change_history: list[Revision]) \
-        -> dict[Stage, set[Project]]:
+def find_invalidated_projects_per_stage(
+    all_projects: set[Project], change_history: list[Revision]
+) -> dict[Stage, set[Project]]:
     projects_for_stage = {}
     for stage in Stage:
-        projects = find_invalidated_projects_for_stage(all_projects, stage, change_history)
+        projects = find_invalidated_projects_for_stage(
+            all_projects, stage, change_history
+        )
         if projects:
-            projects_for_stage[stage] = set(sorted(projects, key=operator.attrgetter('name')))
+            projects_for_stage[stage] = set(
+                sorted(projects, key=operator.attrgetter("name"))
+            )
     return projects_for_stage
 
 
 def for_stage(projects: set[Project], stage: Stage) -> set[Project]:
     return set(filter(lambda p: p.stages.for_stage(stage), projects))
```

## mpyl/steps/__init__.py

```diff
@@ -54,51 +54,56 @@
 
 ##### Step input
 The step receives an `mpyl.steps.models.Input` for `execute`. If your step needs configuration settings, like for
 example `mpyl.utilities.docker.DockerConfig`, this can be constructed from the `mpyl.steps.models.RunProperties.config`
 dictionary on `mpyl.steps.models.Input.run_properties`.
 Make sure to update the schema under `src/mpyl/schema/mpyl_config.schema.yml` accordingly, so that the configuration
 remains type safe and mistakes are found as early as possible.
+
+##### Registration with the executor
+Importing the module in which your step is defined is enough to register it.
+Steps are automatically registered with the `mpyl.steps.steps.Steps` executor via the `IPluginRegistry` metaclass.
 """
 from __future__ import annotations
 
 from dataclasses import dataclass
 from logging import Logger
 from typing import Optional, List
 
 from .models import ArtifactType, Input, Output
 from ..project import Stage
 
 
 class IPluginRegistry(type):
-    plugin_registries: List[type] = []
+    plugins: List[type] = []
 
     def __init__(cls, name, _bases, _attrs):
         super().__init__(cls)
-        if name != 'Step':
-            IPluginRegistry.plugin_registries.append(cls)
+        if name != "Step":
+            IPluginRegistry.plugins.append(cls)
 
 
 @dataclass(frozen=True)
 class Meta:
     name: str
     """External, unique identifier. The step can be referred to by this name from `project.yml`"""
     description: str
     version: str
     stage: Stage
     """The stage that this step relates to"""
 
     def __str__(self) -> str:
-        return f'{self.name}: {self.version}'
+        return f"{self.name}: {self.version}"
 
 
 class Step(metaclass=IPluginRegistry):
-    """ Abstract base class for execution steps. Any execution step (e.g. build, test, deploy) will need to implement
+    """Abstract base class for execution steps. Any execution step (e.g. build, test, deploy) will need to implement
     this interface.
     """
+
     meta: Meta
     """Information _about_ the specific instance of `Step`. For example its name, description, version or the stage
     to which it applies.
     """
     produced_artifact: ArtifactType
     """The type of the artifact produced by this step """
     required_artifact: ArtifactType
@@ -106,23 +111,34 @@
     of an earlier step. For example: a step in the `Deploy` stage, may need to deploy a docker image that was produced
     in the `Build` stage."""
     before: Optional[Step]
     after: Optional[Step]
     """Will be executed after completion of this step. Can be used for shared post processing steps, like pushing the
     produced docker image to a registry or filing test results."""
 
-    def __init__(self, logger: Logger, meta: Meta, produced_artifact: ArtifactType,
-                 required_artifact: ArtifactType, before: Optional[Step] = None, after: Optional[Step] = None) -> None:
-        self._logger = logger.getChild(meta.name.replace(' ', ''))
+    def __init__(
+        self,
+        logger: Logger,
+        meta: Meta,
+        produced_artifact: ArtifactType,
+        required_artifact: ArtifactType,
+        before: Optional[Step] = None,
+        after: Optional[Step] = None,
+    ) -> None:
+        self._logger = logger.getChild(meta.name.replace(" ", ""))
         self.meta = meta
         self.produced_artifact = produced_artifact
         self.required_artifact = required_artifact
         self.before = before
         self.after = after
 
     def execute(self, step_input: Input) -> Output:
-        """ Execute an individual step for a specific `project` at a specific `stage` of the pipeline.
+        """Execute an individual step for a specific `project` at a specific `stage` of the pipeline.
         :param step_input: The input of the project along with its build properties and required artifact (if any).
         :return Output: The result of the execution. `success` will be `False` if any exception was thrown during
         execution.
         """
-        return Output(success=False, message=f"Not implemented for {step_input.project.name}", produced_artifact=None)
+        return Output(
+            success=False,
+            message=f"Not implemented for {step_input.project.name}",
+            produced_artifact=None,
+        )
```

## mpyl/steps/models.py

```diff
@@ -19,19 +19,19 @@
     revision: str
     branch: Optional[str]
     pr_number: Optional[int]
     tag: Optional[str]
 
     def __post_init__(self):
         if not self.pr_number and not self.tag:
-            raise ValueError('Either pr_number or tag need to be set')
+            raise ValueError("Either pr_number or tag need to be set")
 
     @property
     def identifier(self) -> str:
-        return self.tag if self.tag else f'pr-{self.pr_number}'
+        return self.tag if self.tag else f"pr-{self.pr_number}"
 
 
 @dataclass(frozen=True)
 class RunContext:
     build_id: str
     """Uniquely identifies the run. Typically a monotonically increasing number"""
     run_url: str
@@ -43,95 +43,116 @@
     user: str
     """Name of of the user that triggered the run"""
     user_email: Optional[str]
     """Email of of the user that triggered the run"""
 
     @staticmethod
     def from_configuration(run_details: Dict):
-        return RunContext(build_id=run_details['id'], run_url=run_details['run_url'],
-                          change_url=run_details['change_url'], tests_url=run_details['tests_url'],
-                          user=run_details['user'], user_email=run_details['user_email'])
+        return RunContext(
+            build_id=run_details["id"],
+            run_url=run_details["run_url"],
+            change_url=run_details["change_url"],
+            tests_url=run_details["tests_url"],
+            user=run_details["user"],
+            user_email=run_details["user_email"],
+        )
 
 
 @dataclass(frozen=True)
 class ConsoleProperties:
     log_level: str
     width: Optional[int]
 
     @staticmethod
     def from_configuration(build_config: Dict):
-        console_config = build_config['console']
-        width = console_config.get('width', 130)
-        return ConsoleProperties(console_config.get('logLevel', 'INFO'), None if width == 0 else width)
+        console_config = build_config["console"]
+        width = console_config.get("width", 130)
+        return ConsoleProperties(
+            console_config.get("logLevel", "INFO"), None if width == 0 else width
+        )
 
 
 @yaml_object(yaml)
 @dataclass(frozen=True)
 class RunProperties:
-    """ Contains information that is specific to a particular run of the pipeline"""
+    """Contains information that is specific to a particular run of the pipeline"""
+
     details: RunContext
     """Run specific details"""
     target: Target
     """The deploy target"""
     versioning: VersioningProperties
     config: dict
     """Globally specified configuration, to be used by specific steps. Complies with the schema as
     specified in `mpyl_config.schema.yml`
      """
     console: ConsoleProperties
     """Settings for the console output"""
 
     @staticmethod
-    def for_local_run(config: Dict, revision: str, branch: Optional[str], tag: Optional[str]):
-        return RunProperties(details=RunContext("", "", "", "", "", None), target=Target.PULL_REQUEST,
-                             versioning=VersioningProperties(revision, branch, 123, tag), config=config,
-                             console=ConsoleProperties("INFO", 130))
+    def for_local_run(
+        config: Dict, revision: str, branch: Optional[str], tag: Optional[str]
+    ):
+        return RunProperties(
+            details=RunContext("", "", "", "", "", None),
+            target=Target.PULL_REQUEST,
+            versioning=VersioningProperties(revision, branch, 123, tag),
+            config=config,
+            console=ConsoleProperties("INFO", 130),
+        )
 
     @staticmethod
     def from_configuration(run_properties: Dict, config: Dict):
         build_dict = pkgutil.get_data(__name__, "../schema/run_properties.schema.yml")
 
         if build_dict:
-            validate(run_properties, build_dict.decode('utf-8'))
+            validate(run_properties, build_dict.decode("utf-8"))
 
-        build = run_properties['build']
-        versioning_config = build['versioning']
+        build = run_properties["build"]
+        versioning_config = build["versioning"]
 
-        pr_num: str = versioning_config.get('pr_number')
-        tag: str = versioning_config.get('tag')
+        pr_num: str = versioning_config.get("pr_number")
+        tag: str = versioning_config.get("tag")
 
-        versioning = VersioningProperties(revision=versioning_config['revision'],
-                                          branch=versioning_config['branch'],
-                                          pr_number=int(pr_num) if pr_num else None,
-                                          tag=tag)
+        versioning = VersioningProperties(
+            revision=versioning_config["revision"],
+            branch=versioning_config["branch"],
+            pr_number=int(pr_num) if pr_num else None,
+            tag=tag,
+        )
         console = ConsoleProperties.from_configuration(build)
 
         return RunProperties(
-            details=RunContext.from_configuration(build['run']),
-            target=Target(build['parameters']['deploy_target']),
+            details=RunContext.from_configuration(build["run"]),
+            target=Target(
+                build["parameters"].get("deploy_target", None)
+                or Target.PULL_REQUEST.value
+            ),
             versioning=versioning,
             config=config,
             console=console,
         )
 
 
 @yaml_object(yaml)
 @dataclass(frozen=True)
 class ArtifactType(Enum):
     def __eq__(self, other):
         return self.value == other.value
 
     @classmethod
     def from_yaml(cls, _, node):
-        return ArtifactType(int(node.value.split('-')[1]))
+        return ArtifactType(int(node.value.split("-")[1]))
 
     @classmethod
     def to_yaml(cls, representer, node):
-        return representer.represent_scalar('!ArtifactType',
-                                            f'{node._name_}-{node._value_}')  # pylint: disable=protected-access
+        return representer.represent_scalar(
+            "!ArtifactType",
+            f"{node._name_}-{node._value_}",  # pylint: disable=protected-access
+        )
 
     DOCKER_IMAGE = 1
     """A docker image"""
     JUNIT_TESTS = 2
     """A test suite in junit compatible `.xml` format"""
     DEPLOYED_HELM_APP = 3
     """A helm chart deployed to kubernetes"""
@@ -166,22 +187,26 @@
 
     @staticmethod
     def path(target_path: str, stage: Stage):
         return Path(target_path, f"{stage.name}.yml")
 
     def write(self, target_path: str, stage: Stage):
         Path(target_path).mkdir(parents=True, exist_ok=True)
-        with Output.path(target_path, stage).open(mode='w+', encoding='utf-8') as file:
+        with Output.path(target_path, stage).open(mode="w+", encoding="utf-8") as file:
             yaml.dump(self, file)
 
     @staticmethod
     def try_read(target_path: str, stage: Stage):
         path = Output.path(target_path, stage)
         if path.exists():
-            with open(path, encoding='utf-8') as file:
+            with open(path, encoding="utf-8") as file:
                 return yaml.load(file)
         return None
 
 
 def input_to_artifact(artifact_type: ArtifactType, step_input: Input, spec: dict):
-    return Artifact(artifact_type=artifact_type, revision=step_input.run_properties.versioning.revision,
-                    producing_step=step_input.project.name, spec=spec)
+    return Artifact(
+        artifact_type=artifact_type,
+        revision=step_input.run_properties.versioning.revision,
+        producing_step=step_input.project.name,
+        spec=spec,
+    )
```

## mpyl/steps/run.py

```diff
@@ -23,34 +23,36 @@
         self._run_plan = run_plan
         self._exception = None
         self._results = []
 
     @property
     def status_line(self) -> str:
         if self._exception:
-            return '❗ Failed with exception'
+            return "❗ Failed with exception"
         if self.is_in_progress:
-            return '🏗️ Building'
+            return "🏗️ Building"
         if not self.has_results:
-            return '🦥 Nothing to do'
+            return "🦥 Nothing to do"
         if self._results_success():
-            return '✅ Successful'
+            return "✅ Successful"
 
-        return '❌ Failed'
+        return "❌ Failed"
 
     @property
     def failed_result(self) -> Optional[StepResult]:
         return next((r for r in self._results if not r.output.success), None)
 
     @property
     def progress_fraction(self) -> float:
         unfinished = 0
         finished = 0
         for stage, projects in self.run_plan.items():
-            finished_project_names = set(map(lambda r: r.project.name, self.results_for_stage(stage)))
+            finished_project_names = set(
+                map(lambda r: r.project.name, self.results_for_stage(stage))
+            )
             for project in projects:
                 if project.name in finished_project_names:
                     finished += 1
                 else:
                     unfinished += 1
 
         total = unfinished + finished
@@ -93,25 +95,29 @@
 
     @property
     def has_results(self):
         return len(self._results) > 0
 
     @property
     def is_in_progress(self):
-        return len(self.run_plan.items()) > 0 and self.is_success and not self.is_finished
+        return (
+            len(self.run_plan.items()) > 0 and self.is_success and not self.is_finished
+        )
 
     def _results_success(self):
         return not self.has_results or all(r.output.success for r in self._results)
 
     @staticmethod
     def sort_chronologically(results: list[StepResult]) -> list[StepResult]:
-        return sorted(results, key=operator.attrgetter('timestamp'))
+        return sorted(results, key=operator.attrgetter("timestamp"))
 
     def results_for_stage(self, stage: Stage) -> list[StepResult]:
-        return RunResult.sort_chronologically([res for res in self._results if res.stage == stage])
+        return RunResult.sort_chronologically(
+            [res for res in self._results if res.stage == stage]
+        )
 
     def plan_for_stage(self, stage: Stage) -> set[Project]:
         plan: Optional[set[Project]] = self.run_plan.get(stage)
         if plan:
             return plan
 
         return set()
```

## mpyl/steps/steps.py

```diff
@@ -6,37 +6,25 @@
 from datetime import datetime
 from logging import Logger
 from typing import Optional
 
 from ruamel.yaml import YAML  # type: ignore
 
 from . import Step
-from .build.dockerbuild import BuildDocker
-from .build.echo import BuildEcho
-from .build.sbt import BuildSbt
-from .deploy.cloudfront_kubernetes_deploy import CloudFrontKubernetesDeploy
-from .deploy.echo import DeployEcho
-from .deploy.ephemeral_docker_deploy import EphemeralDockerDeploy
-from .deploy.kubernetes import DeployKubernetes
-from .deploy.kubernetes_job import DeployKubernetesJob
-from .deploy.kubernetes_spark_job import DeployKubernetesSparkJob
+from .collection import StepsCollection
 from .models import Output, Input, RunProperties, ArtifactType, Artifact
-from .postdeploy.cypress_test import CypressTest
-from .test.dockertest import TestDocker
-from .test.echo import TestEcho
-from .test.sbt import TestSbt
 from ..project import Project
 from ..project import Stage
 from ..validation import validate
 
 yaml = YAML()
 
 
 class ExecutionException(Exception):
-    """ Exception thrown when a step execution fails. """
+    """Exception thrown when a step execution fails."""
 
     def __init__(self, project_name: str, executor: str, stage: str, message: str):
         self.project_name = project_name
         self.executor = executor
         self.stage = stage
         self.message = message
         super().__init__(self.message)
@@ -47,146 +35,179 @@
     stage: Stage
     project: Project
     output: Output
     timestamp: datetime = datetime.now()
 
 
 class Steps:
-    """ Executor of individual steps within a pipeline. """
-    _step_executors: dict[Stage, set[Step]]
+    """Executor of individual steps within a pipeline."""
+
     _logger: Logger
     _properties: RunProperties
 
-    def __init__(self, logger: Logger, properties: RunProperties) -> None:
+    def __init__(
+        self,
+        logger: Logger,
+        properties: RunProperties,
+        steps_collection: Optional[StepsCollection] = None,
+    ) -> None:
+        self._logger = logger
+        self._properties = properties
+        self._steps_collection = steps_collection or StepsCollection(logger)
+
         schema_dict = pkgutil.get_data(__name__, "../schema/mpyl_config.schema.yml")
 
         if schema_dict:
-            validate(properties.config, schema_dict.decode('utf-8'))
-
-        self._logger = logger
-
-        self._step_executors: dict[Stage, set[Step]] = {
-            Stage.BUILD: {
-                BuildEcho(logger),
-                BuildSbt(logger),
-                BuildDocker(logger)
-            },
-            Stage.TEST: {
-                TestEcho(logger),
-                TestSbt(logger),
-                TestDocker(logger)
-            },
-            Stage.DEPLOY: {
-                CloudFrontKubernetesDeploy(logger),
-                DeployEcho(logger),
-                DeployKubernetes(logger),
-                DeployKubernetesJob(logger),
-                DeployKubernetesSparkJob(logger),
-                EphemeralDockerDeploy(logger)
-            },
-            Stage.POST_DEPLOY: {
-                CypressTest(logger)
-            }
-        }
+            validate(properties.config, schema_dict.decode("utf-8"))
 
-        self._properties = properties
-        for stage, steps in self._step_executors.items():
-            self._logger.debug(f"Registered executors for stage {stage.name}: "  # pylint: disable=E1101
-                               f"{[step.meta.name for step in steps]}")
-
-    def _find_executor(self, stage: Stage, step_name: str) -> Optional[Step]:
-        executors = filter(lambda e: e.meta.stage == stage and step_name == e.meta.name, self._step_executors[stage])
-        return next(executors, None)
-
-    def _execute(self, executor: Step, project: Project, properties: RunProperties,
-                 artifact: Optional[Artifact], dry_run: bool = False) -> Output:
-        result = executor.execute(Input(project, properties, required_artifact=artifact, dry_run=dry_run))
+    def _execute(
+        self,
+        executor: Step,
+        project: Project,
+        properties: RunProperties,
+        artifact: Optional[Artifact],
+        dry_run: bool = False,
+    ) -> Output:
+        result = executor.execute(
+            Input(project, properties, required_artifact=artifact, dry_run=dry_run)
+        )
         if result.success:
             self._logger.info(
-                f"Execution of {executor.meta.name} succeeded for '{project.name}' with outcome '{result.message}'")
+                f"Execution of {executor.meta.name} succeeded for '{project.name}' with outcome '{result.message}'"
+            )
         else:
             self._logger.warning(
-                f"Execution of {executor.meta.name} failed for '{project.name}' with outcome '{result.message}'")
+                f"Execution of {executor.meta.name} failed for '{project.name}' with outcome '{result.message}'"
+            )
         return result
 
     @staticmethod
-    def _find_required_artifact(project: Project, required_artifact: Optional[ArtifactType]) -> Optional[Artifact]:
+    def _find_required_artifact(
+        project: Project, required_artifact: Optional[ArtifactType]
+    ) -> Optional[Artifact]:
         if not required_artifact or required_artifact == ArtifactType.NONE:
             return None
 
         for stage in Stage:
             output: Optional[Output] = Output.try_read(project.target_path, stage)
-            if output and output.produced_artifact and output.produced_artifact.artifact_type == required_artifact:
+            if (
+                output
+                and output.produced_artifact
+                and output.produced_artifact.artifact_type == required_artifact
+            ):
                 return output.produced_artifact
 
-        raise ValueError(f"Artifact {required_artifact} required for {project.name} not found")
-
-    def _execute_after_(self, main_result: Output, step: Step, project: Project, stage: Stage,
-                        dry_run: bool = False) -> Output:
+        raise ValueError(
+            f"Artifact {required_artifact} required for {project.name} not found"
+        )
+
+    def _execute_after_(
+        self,
+        main_result: Output,
+        step: Step,
+        project: Project,
+        stage: Stage,
+        dry_run: bool = False,
+    ) -> Output:
         main_step_artifact = main_result.produced_artifact
-        after_result = self._execute(step, project, self._properties, main_step_artifact, dry_run)
-        if after_result.produced_artifact and after_result.produced_artifact.artifact_type != ArtifactType.NONE:
+        after_result = self._execute(
+            step, project, self._properties, main_step_artifact, dry_run
+        )
+        if (
+            after_result.produced_artifact
+            and after_result.produced_artifact.artifact_type != ArtifactType.NONE
+        ):
             after_result.write(project.target_path, stage)
         else:
             after_result.produced_artifact = main_step_artifact
 
         if not main_result.success:
             after_result.message = main_result.message
             after_result.success = False
 
         return after_result
 
     def _validate_project_against_config(self, project: Project) -> Optional[Output]:
-        allowed_maintainers = set(self._properties.config.get('project', {}).get('allowedMaintainers', []))
+        allowed_maintainers = set(
+            self._properties.config.get("project", {}).get("allowedMaintainers", [])
+        )
         not_allowed = set(project.maintainer).difference(allowed_maintainers)
         if not_allowed:
-            return Output(success=False, message=f"Maintainer(s) '{', '.join(not_allowed)}' not defined in config")
+            return Output(
+                success=False,
+                message=f"Maintainer(s) '{', '.join(not_allowed)}' not defined in config",
+            )
         return None
 
-    def _execute_stage(self, stage: Stage, project: Project, dry_run: bool = False) -> Output:
-        stage_name = project.stages.for_stage(stage)
-        if stage_name is None:
-            return Output(success=False, message=f"Stage '{stage.value}' not defined on project '{project.name}'")
+    def _execute_stage(
+        self, stage: Stage, project: Project, dry_run: bool = False
+    ) -> Output:
+        step_name = project.stages.for_stage(stage)
+        if step_name is None:
+            return Output(
+                success=False,
+                message=f"Stage '{stage.value}' not defined on project '{project.name}'",
+            )
 
         invalid_maintainers = self._validate_project_against_config(project)
         if invalid_maintainers:
             return invalid_maintainers
 
-        executor: Optional[Step] = self._find_executor(stage, stage_name)
-        if executor:
-            try:
-                self._logger.info(f'Executing {stage} for {project.name}')
-                artifact: Optional[Artifact] = self._find_required_artifact(project, executor.required_artifact)
-                if executor.before:
-                    before_result = self._execute(executor.before, project, self._properties,
-                                                  self._find_required_artifact(project,
-                                                                               executor.before.required_artifact),
-                                                  dry_run)
-                    if not before_result.success:
-                        return before_result
-
-                result = self._execute(executor, project, self._properties, artifact, dry_run)
-                result.write(project.target_path, stage)
-
-                if executor.after:
-                    return self._execute_after_(result, executor.after, project, stage, dry_run)
-
-                return result
-            except Exception as exc:
-                message = str(exc)
-                self._logger.warning(
-                    f"Execution of '{executor.meta.name}' for project '{project.name}' in stage {stage} "
-                    f"failed with exception: {message}", exc_info=True)
-                raise ExecutionException(project.name, executor.meta.name, stage.name, message) from exc
-        else:
-            self._logger.warning(f"No executor found for {stage_name} in stage {stage}")
-
-        return Output(success=False, message=f"Executor '{stage_name}' for '{stage.value}' not known or registered")
-
-    def execute(self, stage: Stage, project: Project, dry_run: bool = False) -> StepResult:
+        executor: Optional[Step] = self._steps_collection.get_executor(stage, step_name)
+        if not executor:
+            self._logger.warning(f"No executor found for {step_name} in stage {stage}")
+
+            return Output(
+                success=False,
+                message=f"Executor '{step_name}' for '{stage.value}' not known or registered",
+            )
+
+        try:
+            self._logger.info(f"Executing {stage} for {project.name}")
+            artifact: Optional[Artifact] = self._find_required_artifact(
+                project, executor.required_artifact
+            )
+            if executor.before:
+                before_result = self._execute(
+                    executor.before,
+                    project,
+                    self._properties,
+                    self._find_required_artifact(
+                        project, executor.before.required_artifact
+                    ),
+                    dry_run,
+                )
+                if not before_result.success:
+                    return before_result
+
+            result = self._execute(
+                executor, project, self._properties, artifact, dry_run
+            )
+            result.write(project.target_path, stage)
+
+            if executor.after:
+                return self._execute_after_(
+                    result, executor.after, project, stage, dry_run
+                )
+
+            return result
+        except Exception as exc:
+            message = str(exc)
+            self._logger.warning(
+                f"Execution of '{executor.meta.name}' for project '{project.name}' in stage {stage} "
+                f"failed with exception: {message}",
+                exc_info=True,
+            )
+            raise ExecutionException(
+                project.name, executor.meta.name, stage.name, message
+            ) from exc
+
+    def execute(
+        self, stage: Stage, project: Project, dry_run: bool = False
+    ) -> StepResult:
         """
         :param stage: the stage to execute
         :param project: the project metadata
         :param dry_run: indicates whether artifacts should be submitted or deployed for real
         :return: StepResult
         :raise ExecutionException
         """
```

## mpyl/steps/build/echo.py

```diff
@@ -1,22 +1,25 @@
 """ Dummy build step to test the framework. """
 
 from logging import Logger
 
 from .. import Step, Meta
-from ..models import Input, Output, ArtifactType
+from ..models import Input, Output, ArtifactType, input_to_artifact
 from ...project import Stage
+from ...utilities.docker import docker_image_tag
 
 
 class BuildEcho(Step):
 
     def __init__(self, logger: Logger) -> None:
         super().__init__(logger, Meta(
             name='Echo Build',
             description='Dummy build step to test the framework',
             version='0.0.1',
             stage=Stage.BUILD
         ), produced_artifact=ArtifactType.NONE, required_artifact=ArtifactType.NONE)
 
     def execute(self, step_input: Input) -> Output:
         self._logger.info(f"Building project {step_input.project.name}")
-        return Output(success=True, message=f"Built {step_input.project.name}", produced_artifact=None)
+        artifact = input_to_artifact(ArtifactType.DOCKER_IMAGE, step_input,
+                                     spec={'image': docker_image_tag(step_input)})
+        return Output(success=True, message=f"Built {step_input.project.name}", produced_artifact=artifact)
```

## mpyl/steps/deploy/cloudfront_kubernetes_deploy.py

```diff
@@ -6,52 +6,71 @@
 from .kubernetes import DeployKubernetes
 from .. import Step, Meta
 from ...project import Stage
 from ..models import Input, Output, ArtifactType
 from ...utilities.docker import docker_image_tag, docker_copy, create_container
 from ...utilities.s3 import S3Client, S3ClientConfig
 
-STATIC_FOLDER = 'static'
+STATIC_FOLDER = "static"
 
 
 class CloudFrontKubernetesDeploy(Step):
-
     def __init__(self, logger: Logger) -> None:
-        super().__init__(logger, Meta(
-            name='CloudFront Kubernetes Deploy',
-            description='uploads the build output to an s3 bucket',
-            version='0.0.1',
-            stage=Stage.DEPLOY,
-        ), produced_artifact=ArtifactType.NONE, required_artifact=ArtifactType.DOCKER_IMAGE)
+        super().__init__(
+            logger,
+            Meta(
+                name="CloudFront Kubernetes Deploy",
+                description="uploads the build output to an s3 bucket",
+                version="0.0.1",
+                stage=Stage.DEPLOY,
+            ),
+            produced_artifact=ArtifactType.NONE,
+            required_artifact=ArtifactType.DOCKER_IMAGE,
+        )
 
     def execute(self, step_input: Input) -> Output:
         with tempfile.TemporaryDirectory() as tmp_folder:
-            self.__copy_docker_assets(logger=self._logger, step_input=step_input, tmp_folder=tmp_folder)
+            self.__copy_docker_assets(
+                logger=self._logger, step_input=step_input, tmp_folder=tmp_folder
+            )
 
             if not step_input.dry_run:
-                self.__upload_to_s3(logger=self._logger, step_input=step_input, tmp_folder=tmp_folder)
+                self.__upload_to_s3(
+                    logger=self._logger, step_input=step_input, tmp_folder=tmp_folder
+                )
 
         return DeployKubernetes(self._logger).execute(step_input)
 
     @staticmethod
     def __copy_docker_assets(logger: Logger, step_input: Input, tmp_folder: str):
         """
         Copies the static assets from the docker image to a temp folder
         """
         image_name = docker_image_tag(step_input)
-        container_path = f'{step_input.project.name}/{STATIC_FOLDER}'
+        container_path = f"{step_input.project.name}/{STATIC_FOLDER}"
         container = create_container(logger, image_name)
-        docker_copy(logger=logger, container_path=container_path, dst_path=tmp_folder, container=container)
+        docker_copy(
+            logger=logger,
+            container_path=container_path,
+            dst_path=tmp_folder,
+            container=container,
+        )
 
     @staticmethod
     def __upload_to_s3(logger: Logger, step_input: Input, tmp_folder: str):
         """
         Creates an S3 client and uploads the static assets stored in the temp folder
         """
         logger.info("Creating S3 client")
-        bucket_name = step_input.project.s3_bucket.bucket.get_value(step_input.run_properties.target)
-        s3_config = S3ClientConfig(run_properties=step_input.run_properties, bucket_name=bucket_name)
+        bucket_name = step_input.project.s3_bucket.bucket.get_value(
+            step_input.run_properties.target
+        )
+        s3_config = S3ClientConfig(
+            run_properties=step_input.run_properties, bucket_name=bucket_name
+        )
         s3_client = S3Client(logger, s3_config)
 
-        logger.info(f"Uploading assets to '{s3_config.bucket_root_path}' in bucket '{s3_config.bucket_name}'")
+        logger.info(
+            f"Uploading assets to '{s3_config.bucket_root_path}' in bucket '{s3_config.bucket_name}'"
+        )
         s3_client.upload_directory(directory=tmp_folder)
-        logger.info('Upload complete')
+        logger.info("Upload complete")
```

## mpyl/steps/deploy/echo.py

```diff
@@ -4,23 +4,36 @@
 
 from .. import Step, Meta
 from ..models import Input, Output, ArtifactType
 from ...project import Stage
 
 
 class DeployEcho(Step):
-
     def __init__(self, logger: Logger) -> None:
-        super().__init__(logger, Meta(
-            name='Echo Deploy',
-            description='Dummy deploy step to test the framework',
-            version='0.0.1',
-            stage=Stage.DEPLOY
-        ), ArtifactType.NONE, ArtifactType.DOCKER_IMAGE)
+        super().__init__(
+            logger,
+            Meta(
+                name="Echo Deploy",
+                description="Dummy deploy step to test the framework",
+                version="0.0.1",
+                stage=Stage.DEPLOY,
+            ),
+            ArtifactType.NONE,
+            ArtifactType.DOCKER_IMAGE,
+        )
 
     def execute(self, step_input: Input) -> Output:
         artifact = step_input.required_artifact
         if not artifact:
-            return Output(success=False, message=f"Step requires artifact of type {self.required_artifact}")
-
-        self._logger.info(f"Deploying project {step_input.project.name} with artifact: {artifact.spec}")
-        return Output(success=True, message=f"Deployed project {step_input.project.name}", produced_artifact=None)
+            return Output(
+                success=False,
+                message=f"Step requires artifact of type {self.required_artifact}",
+            )
+
+        self._logger.info(
+            f"Deploying project {step_input.project.name} with artifact: {artifact.spec}"
+        )
+        return Output(
+            success=True,
+            message=f"Deployed project {step_input.project.name}",
+            produced_artifact=None,
+        )
```

## mpyl/steps/deploy/ephemeral_docker_deploy.py

```diff
@@ -7,24 +7,36 @@
 from .. import Step, Meta
 from ..models import Input, Output, ArtifactType
 from ...project import Stage, get_env_variables
 from ...utilities.docker import docker_image_tag
 
 
 class EphemeralDockerDeploy(Step):
-
     def __init__(self, logger: Logger) -> None:
-        super().__init__(logger, Meta(
-            name='Deploy From Docker Container',
-            description='Runs and removes the docker container built during the build stage. '
-                        'Useful for custom deploy steps depending on technology not bundled with MPyL',
-            version='0.0.1',
-            stage=Stage.DEPLOY
-        ), produced_artifact=ArtifactType.NONE, required_artifact=ArtifactType.DOCKER_IMAGE)
+        super().__init__(
+            logger,
+            Meta(
+                name="Deploy From Docker Container",
+                description="Runs and removes the docker container built during the build stage. "
+                "Useful for custom deploy steps depending on technology not bundled with MPyL",
+                version="0.0.1",
+                stage=Stage.DEPLOY,
+            ),
+            produced_artifact=ArtifactType.NONE,
+            required_artifact=ArtifactType.DOCKER_IMAGE,
+        )
 
     def execute(self, step_input: Input) -> Output:
-        env_variables = get_env_variables(step_input.project, step_input.run_properties.target)
+        env_variables = get_env_variables(
+            step_input.project, step_input.run_properties.target
+        )
         docker_image_name = docker_image_tag(step_input)
-        docker_run_result = docker.run(image=docker_image_name, remove=True, envs=env_variables)
+        docker_run_result = docker.run(
+            image=docker_image_name, remove=True, envs=env_variables
+        )
         self._logger.info(docker_run_result)
 
-        return Output(success=True, message=f"Deployed project {step_input.project.name}", produced_artifact=None)
+        return Output(
+            success=True,
+            message=f"Deployed project {step_input.project.name}",
+            produced_artifact=None,
+        )
```

## mpyl/steps/deploy/kubernetes.py

```diff
@@ -7,65 +7,99 @@
 from .k8s.chart import ChartBuilder, to_service_chart
 from .. import Step, Meta
 from ..models import Input, Output, ArtifactType, input_to_artifact
 from ...project import Stage, Target
 from ...stages.discovery import find_deploy_set
 from ...utilities.repo import RepoConfig
 
-DEPLOYED_SERVICE_KEY = 'url'
+DEPLOYED_SERVICE_KEY = "url"
 
 
 class DeployKubernetes(Step):
-
     def __init__(self, logger: Logger) -> None:
-        super().__init__(logger, Meta(
-            name='Kubernetes Deploy',
-            description='Deploy to k8s',
-            version='0.0.1',
-            stage=Stage.DEPLOY
-        ), produced_artifact=ArtifactType.NONE, required_artifact=ArtifactType.DOCKER_IMAGE)
+        super().__init__(
+            logger,
+            Meta(
+                name="Kubernetes Deploy",
+                description="Deploy to k8s",
+                version="0.0.1",
+                stage=Stage.DEPLOY,
+            ),
+            produced_artifact=ArtifactType.NONE,
+            required_artifact=ArtifactType.DOCKER_IMAGE,
+        )
 
     @staticmethod
     def match_to_url(match: str) -> str:
-        return 'https://' + next(iter(re.findall(r'`(.*)`', match.split(',')[-1])))
+        return "https://" + next(iter(re.findall(r"`(.*)`", match.split(",")[-1])))
 
     @staticmethod
-    def try_extract_hostname(chart: dict[str, CustomResourceDefinition]) -> Optional[str]:
-        ingress = chart.get('ingress-https-route')
+    def try_extract_hostname(
+        chart: dict[str, CustomResourceDefinition]
+    ) -> Optional[str]:
+        ingress = chart.get("ingress-https-route")
         if ingress:
-            routes = ingress.spec.get('routes', {})
+            routes = ingress.spec.get("routes", {})
             if routes:
-                match = routes[0].get('match')
+                match = routes[0].get("match")
                 return DeployKubernetes.match_to_url(match)
         return None
 
     def execute(self, step_input: Input) -> Output:
         properties = step_input.run_properties
-        builder = ChartBuilder(step_input, find_deploy_set(repo_config=RepoConfig.from_config(properties.config),
-                                                           tag=step_input.run_properties.versioning.tag))
+        builder = ChartBuilder(
+            step_input,
+            find_deploy_set(
+                repo_config=RepoConfig.from_config(properties.config),
+                tag=step_input.run_properties.versioning.tag,
+            ),
+        )
         chart = to_service_chart(builder)
 
         target_cluster = cluster_config(properties.target, properties)
-        deploy_result = deploy_helm_chart(self._logger, chart, step_input, target_cluster, builder.release_name)
+        deploy_result = deploy_helm_chart(
+            self._logger, chart, step_input, target_cluster, builder.release_name
+        )
         if deploy_result.success:
             hostname = self.try_extract_hostname(chart)
             spec = {}
             if hostname:
-                has_specific_routes_configured: bool = bool(builder.deployment.traefik is not None)
-                self._logger.info(f"Service {step_input.project.name} reachable at: {hostname}")
+                has_specific_routes_configured: bool = bool(
+                    builder.deployment.traefik is not None
+                )
+                self._logger.info(
+                    f"Service {step_input.project.name} reachable at: {hostname}"
+                )
 
-                endpoint = '/' if has_specific_routes_configured else '/swagger/index.html'
-                spec[DEPLOYED_SERVICE_KEY] = f'{hostname}{endpoint}'
-            artifact = input_to_artifact(ArtifactType.DEPLOYED_HELM_APP, step_input, spec=spec)
+                endpoint = (
+                    "/" if has_specific_routes_configured else "/swagger/index.html"
+                )
+                spec[DEPLOYED_SERVICE_KEY] = f"{hostname}{endpoint}"
+            artifact = input_to_artifact(
+                ArtifactType.DEPLOYED_HELM_APP, step_input, spec=spec
+            )
             if properties.target == Target.PRODUCTION:
                 self._logger.info(
                     f"Release to production successful, updating base images in {Target.PULL_REQUEST_BASE} "
-                    f"to make sure the Test environment is in sync with production")
+                    f"to make sure the Test environment is in sync with production"
+                )
                 target_cluster = cluster_config(Target.PRODUCTION, properties)
-                deploy_to_prod_result = deploy_helm_chart(self._logger, chart, step_input, target_cluster,
-                                                          builder.release_name)
-                return Output(success=True, message=deploy_result.message + '\n' + deploy_to_prod_result.message,
-                              produced_artifact=artifact)
-
-            return Output(success=True, message=deploy_result.message, produced_artifact=artifact)
+                deploy_to_prod_result = deploy_helm_chart(
+                    self._logger,
+                    chart,
+                    step_input,
+                    target_cluster,
+                    builder.release_name,
+                )
+                return Output(
+                    success=True,
+                    message=deploy_result.message
+                    + "\n"
+                    + deploy_to_prod_result.message,
+                    produced_artifact=artifact,
+                )
+
+            return Output(
+                success=True, message=deploy_result.message, produced_artifact=artifact
+            )
 
         return deploy_result
```

## mpyl/steps/deploy/kubernetes_job.py

```diff
@@ -8,24 +8,41 @@
 from ..models import Input, Output, ArtifactType
 from ...project import Stage
 from ...stages.discovery import find_deploy_set
 from ...utilities.repo import RepoConfig
 
 
 class DeployKubernetesJob(Step):
-
     def __init__(self, logger: Logger) -> None:
-        super().__init__(logger, Meta(
-            name='Kubernetes Job Deploy',
-            description='Deploy a job to k8s',
-            version='0.0.1',
-            stage=Stage.DEPLOY
-        ), produced_artifact=ArtifactType.NONE, required_artifact=ArtifactType.DOCKER_IMAGE)
+        super().__init__(
+            logger,
+            Meta(
+                name="Kubernetes Job Deploy",
+                description="Deploy a job to k8s",
+                version="0.0.1",
+                stage=Stage.DEPLOY,
+            ),
+            produced_artifact=ArtifactType.NONE,
+            required_artifact=ArtifactType.DOCKER_IMAGE,
+        )
 
     def execute(self, step_input: Input) -> Output:
         run_properties = step_input.run_properties
-        builder = ChartBuilder(step_input, find_deploy_set(repo_config=RepoConfig.from_config(run_properties.config),
-                                                           tag=step_input.run_properties.versioning.tag))
-        chart = to_cron_job_chart(builder) if builder.is_cron_job else to_job_chart(builder)
+        builder = ChartBuilder(
+            step_input,
+            find_deploy_set(
+                repo_config=RepoConfig.from_config(run_properties.config),
+                tag=step_input.run_properties.versioning.tag,
+            ),
+        )
+        chart = (
+            to_cron_job_chart(builder) if builder.is_cron_job else to_job_chart(builder)
+        )
         target_cluster = cluster_config(run_properties.target, run_properties)
-        return deploy_helm_chart(self._logger, chart, step_input, target_cluster, builder.release_name,
-                                 delete_existing=True)
+        return deploy_helm_chart(
+            self._logger,
+            chart,
+            step_input,
+            target_cluster,
+            builder.release_name,
+            delete_existing=True,
+        )
```

## mpyl/steps/deploy/kubernetes_spark_job.py

```diff
@@ -8,24 +8,40 @@
 from ..models import Input, Output, ArtifactType
 from ...project import Stage
 from ...stages.discovery import find_deploy_set
 from ...utilities.repo import RepoConfig
 
 
 class DeployKubernetesSparkJob(Step):
-
     def __init__(self, logger: Logger) -> None:
-        super().__init__(logger, Meta(
-            name='Kubernetes Spark Job Deploy',
-            description='Deploy a Spark Job to the Spark Operator',
-            version='0.0.1',
-            stage=Stage.DEPLOY
-        ), produced_artifact=ArtifactType.NONE, required_artifact=ArtifactType.DOCKER_IMAGE)
+        super().__init__(
+            logger,
+            Meta(
+                name="Kubernetes Spark Job Deploy",
+                description="Deploy a Spark Job to the Spark Operator",
+                version="0.0.1",
+                stage=Stage.DEPLOY,
+            ),
+            produced_artifact=ArtifactType.NONE,
+            required_artifact=ArtifactType.DOCKER_IMAGE,
+        )
 
     def execute(self, step_input: Input) -> Output:
         run_properties = step_input.run_properties
         chart = to_spark_job_chart(
-            ChartBuilder(step_input, find_deploy_set(repo_config=RepoConfig.from_config(run_properties.config),
-                                                     tag=step_input.run_properties.versioning.tag)))
+            ChartBuilder(
+                step_input,
+                find_deploy_set(
+                    repo_config=RepoConfig.from_config(run_properties.config),
+                    tag=step_input.run_properties.versioning.tag,
+                ),
+            )
+        )
         target_cluster = cluster_config(run_properties.target, run_properties)
-        return deploy_helm_chart(self._logger, chart, step_input, target_cluster, ChartBuilder(step_input).release_name,
-                                 delete_existing=True)
+        return deploy_helm_chart(
+            self._logger,
+            chart,
+            step_input,
+            target_cluster,
+            ChartBuilder(step_input).release_name,
+            delete_existing=True,
+        )
```

## mpyl/steps/deploy/k8s/__init__.py

```diff
@@ -5,15 +5,19 @@
 from kubernetes import config, client
 
 from ...deploy.k8s.resources import CustomResourceDefinition
 from ...models import RunProperties
 from ....project import Project, Target, ProjectName
 from ....steps import Input, Output
 from ....steps.deploy.k8s import helm
-from ....steps.deploy.k8s.rancher import cluster_config, rancher_namespace_metadata, ClusterConfig
+from ....steps.deploy.k8s.rancher import (
+    cluster_config,
+    rancher_namespace_metadata,
+    ClusterConfig,
+)
 
 
 def get_namespace(run_properties: RunProperties, project: Project) -> Optional[str]:
     if run_properties.target == Target.PULL_REQUEST:
         return run_properties.versioning.identifier
 
     return get_namespace_from_project(project)
@@ -30,51 +34,76 @@
     properties = step_input.run_properties
 
     config.load_kube_config(context=context)
     logger.info(f"Deploying target {properties.target} and k8s context {context}")
     api = client.CoreV1Api()
 
     namespace = get_namespace(properties, step_input.project)
-    meta_data = rancher_namespace_metadata(namespace or step_input.project.name, step_input)
-    namespaces = api.list_namespace(field_selector=f'metadata.name={namespace}')
+    meta_data = rancher_namespace_metadata(
+        namespace or step_input.project.name, step_input
+    )
+    namespaces = api.list_namespace(field_selector=f"metadata.name={namespace}")
 
     if len(namespaces.items) == 0 and not step_input.dry_run:
-        api.create_namespace(client.V1Namespace(api_version='v1', kind='Namespace', metadata=meta_data))
+        api.create_namespace(
+            client.V1Namespace(api_version="v1", kind="Namespace", metadata=meta_data)
+        )
     else:
         logger.info(f"Found namespace {namespace}")
 
     return namespace
 
 
-def deploy_helm_chart(logger: Logger, chart: dict[str, CustomResourceDefinition], step_input: Input,
-                      target_cluster: ClusterConfig,
-                      release_name: str, delete_existing: bool = False) -> Output:
+def deploy_helm_chart(
+    logger: Logger,
+    chart: dict[str, CustomResourceDefinition],
+    step_input: Input,
+    target_cluster: ClusterConfig,
+    release_name: str,
+    delete_existing: bool = False,
+) -> Output:
     namespace = upsert_namespace(logger, step_input, target_cluster.context)
 
-    return helm.install(logger, chart, step_input, release_name, namespace, target_cluster.context, delete_existing)
-
-
-def substitute_namespaces(env_vars: dict[str, str], all_projects: set[ProjectName],
-                          projects_to_deploy: set[ProjectName],
-                          pr_identifier: Optional[int]) -> dict[str, str]:
+    return helm.install(
+        logger,
+        chart,
+        step_input,
+        release_name,
+        namespace,
+        target_cluster.context,
+        delete_existing,
+    )
+
+
+def substitute_namespaces(
+    env_vars: dict[str, str],
+    all_projects: set[ProjectName],
+    projects_to_deploy: set[ProjectName],
+    pr_identifier: Optional[int],
+) -> dict[str, str]:
     env = env_vars.copy()
 
     def get_namespace_for_linked_project(project_name: ProjectName):
         is_part_of_same_deploy_set = project_name in projects_to_deploy
         if is_part_of_same_deploy_set and pr_identifier:
-            return f'pr-{pr_identifier}'
+            return f"pr-{pr_identifier}"
         return project_name.namespace
 
     def replace_namespace(env_value, project_name, namespace):
-        search_value = project_name + '.{namespace}'
-        replace_value = project_name + '.' + namespace
+        search_value = project_name + ".{namespace}"
+        replace_value = project_name + "." + namespace
         return env_value.replace(search_value, replace_value)
 
     for project in all_projects:
         if project.namespace:
             linked_project_namespace = get_namespace_for_linked_project(project)
             for key, value in env.items():
-                replaced_namespace = replace_namespace(value, project.name, linked_project_namespace)
-                updated_pr = replaced_namespace.replace('{PR-NUMBER}',
-                                                        str(pr_identifier)) if pr_identifier else replaced_namespace
+                replaced_namespace = replace_namespace(
+                    value, project.name, linked_project_namespace
+                )
+                updated_pr = (
+                    replaced_namespace.replace("{PR-NUMBER}", str(pr_identifier))
+                    if pr_identifier
+                    else replaced_namespace
+                )
                 env[key] = updated_pr
     return env
```

## mpyl/steps/deploy/k8s/chart.py

```diff
@@ -2,30 +2,77 @@
 Data classes for the composition of Custom Resource Definitions.
 More info: https://kubernetes.io/docs/concepts/extend-kubernetes/api-extension/custom-resources/
 """
 import itertools
 from dataclasses import dataclass
 from typing import Dict, Optional
 
-from kubernetes.client import V1Deployment, V1Container, V1DeploymentSpec, V1ObjectMeta, V1PodSpec, \
-    V1RollingUpdateDeployment, V1LabelSelector, V1ContainerPort, V1EnvVar, V1Service, \
-    V1ServiceSpec, V1ServicePort, V1ServiceAccount, V1LocalObjectReference, \
-    V1EnvVarSource, V1SecretKeySelector, V1Probe, ApiClient, V1HTTPGetAction, V1ResourceRequirements, \
-    V1PodTemplateSpec, V1DeploymentStrategy, V1Job, V1JobSpec, V1CronJob, V1CronJobSpec, V1JobTemplateSpec, V1ConfigMap
+from kubernetes.client import (
+    V1Deployment,
+    V1Container,
+    V1DeploymentSpec,
+    V1ObjectMeta,
+    V1PodSpec,
+    V1RollingUpdateDeployment,
+    V1LabelSelector,
+    V1ContainerPort,
+    V1EnvVar,
+    V1Service,
+    V1ServiceSpec,
+    V1ServicePort,
+    V1ServiceAccount,
+    V1LocalObjectReference,
+    V1EnvVarSource,
+    V1SecretKeySelector,
+    V1Probe,
+    ApiClient,
+    V1HTTPGetAction,
+    V1ResourceRequirements,
+    V1PodTemplateSpec,
+    V1DeploymentStrategy,
+    V1Job,
+    V1JobSpec,
+    V1CronJob,
+    V1CronJobSpec,
+    V1JobTemplateSpec,
+    V1ConfigMap,
+)
 from ruamel.yaml import YAML
 
 from . import substitute_namespaces
-from .resources import CustomResourceDefinition, to_dict  # pylint: disable = no-name-in-module
+from .resources import (
+    CustomResourceDefinition,
+    to_dict,
+)  # pylint: disable = no-name-in-module
 from .resources.sealed_secret import V1SealedSecret
-from .resources.spark import to_spark_body, get_spark_config_map_data, V1SparkApplication
-from .resources.traefik import V1AlphaIngressRoute, V1AlphaMiddleware, \
-    HostWrapper  # pylint: disable = no-name-in-module
+from .resources.spark import (
+    to_spark_body,
+    get_spark_config_map_data,
+    V1SparkApplication,
+)
+from .resources.traefik import (
+    V1AlphaIngressRoute,
+    V1AlphaMiddleware,
+    HostWrapper,
+)  # pylint: disable = no-name-in-module
 from ...models import Input, ArtifactType
-from ....project import Project, KeyValueProperty, Probe, Deployment, TargetProperty, Resources, Target, Kubernetes, \
-    Job, Traefik, Host, get_env_variables
+from ....project import (
+    Project,
+    KeyValueProperty,
+    Probe,
+    Deployment,
+    TargetProperty,
+    Resources,
+    Target,
+    Kubernetes,
+    Job,
+    Traefik,
+    Host,
+    get_env_variables,
+)
 from ....stages.discovery import DeploySet
 
 yaml = YAML()
 
 # Determined (unscientifically) to be sensible factors.
 # Based on actual CPU usage, pods rarely use more than 10% of the allocated CPU. 60% usage is healthy, so we
 # scale down to 20% in order to keep some slack.
@@ -42,57 +89,62 @@
 
     return value
 
 
 def with_target(dictionary: dict, target: Target) -> dict:
     def with_targets_parsed(obj):
         if isinstance(obj, dict):
-            return type(obj)((k, try_parse_target(with_targets_parsed(v), target)) for k, v in obj.items())
+            return type(obj)(
+                (k, try_parse_target(with_targets_parsed(v), target))
+                for k, v in obj.items()
+            )
 
         return obj
 
     return with_targets_parsed(dictionary)
 
 
 @dataclass(frozen=True)
 class ResourceDefaults:
     instances: TargetProperty[int]
     cpus: TargetProperty[float]
     mem: TargetProperty[int]
 
     @staticmethod
     def from_config(resources: dict):
-        limit = resources['limit']
-        return ResourceDefaults(instances=TargetProperty.from_config(resources['instances']),
-                                cpus=TargetProperty.from_config(limit['cpus']),
-                                mem=TargetProperty.from_config(limit['mem']))
+        limit = resources["limit"]
+        return ResourceDefaults(
+            instances=TargetProperty.from_config(resources["instances"]),
+            cpus=TargetProperty.from_config(limit["cpus"]),
+            mem=TargetProperty.from_config(limit["mem"]),
+        )
 
 
 @dataclass(frozen=True)
 class DeploymentDefaults:
     resources_defaults: ResourceDefaults
     liveness_probe_defaults: dict
     startup_probe_defaults: dict
     job_defaults: dict
     treafik_defaults: dict
     white_lists: dict
 
     @staticmethod
     def from_config(config: dict):
-        deployment_values = config.get('project', {}).get('deployment', {})
+        deployment_values = config.get("project", {}).get("deployment", {})
         if deployment_values is None:
             raise KeyError("Configuration should have project.deployment section")
-        kubernetes = deployment_values.get('kubernetes', {})
+        kubernetes = deployment_values.get("kubernetes", {})
         return DeploymentDefaults(
-            resources_defaults=ResourceDefaults.from_config(kubernetes['resources']),
-            liveness_probe_defaults=kubernetes['livenessProbe'],
-            startup_probe_defaults=kubernetes['startupProbe'],
-            job_defaults=kubernetes.get('job', {}),
-            treafik_defaults=deployment_values.get('traefik', {}),
-            white_lists=config.get('whiteLists', {})
+            resources_defaults=ResourceDefaults.from_config(kubernetes["resources"]),
+            liveness_probe_defaults=kubernetes["livenessProbe"],
+            startup_probe_defaults=kubernetes["startupProbe"],
+            job_defaults=kubernetes.get("job", {}),
+            treafik_defaults=deployment_values.get("traefik", {}),
+            white_lists=config.get("whiteLists", {}),
         )
 
 
 class ChartBuilder:
     step_input: Input
     project: Project
     mappings: dict[int, int]
@@ -107,176 +159,271 @@
     def __init__(self, step_input: Input, deploy_set: Optional[DeploySet] = None):
         self.step_input = step_input
         project = self.step_input.project
         self.project = project
         if project.deployment is None:
             raise AttributeError("deployment field should be set")
 
-        self.config_defaults = DeploymentDefaults.from_config(step_input.run_properties.config)
+        self.config_defaults = DeploymentDefaults.from_config(
+            step_input.run_properties.config
+        )
 
         self.deployment = project.deployment
         properties = self.deployment.properties
         self.env = properties.env if properties and properties.env else []
-        self.sealed_secrets = properties.sealed_secret if properties and properties.sealed_secret else []
+        self.sealed_secrets = (
+            properties.sealed_secret if properties and properties.sealed_secret else []
+        )
         self.mappings = self.project.kubernetes.port_mappings
         self.target = step_input.run_properties.target
         self.release_name = self.project.name.lower()
         self.deploy_set = deploy_set
 
     def _to_labels(self) -> Dict:
         run_properties = self.step_input.run_properties
-        app_labels = {'name': self.release_name, 'app.kubernetes.io/version': run_properties.versioning.identifier,
-                      'app.kubernetes.io/managed-by': 'Helm', 'app.kubernetes.io/name': self.release_name,
-                      'app.kubernetes.io/instance': self.release_name}
+        app_labels = {
+            "name": self.release_name,
+            "app.kubernetes.io/version": run_properties.versioning.identifier,
+            "app.kubernetes.io/managed-by": "Helm",
+            "app.kubernetes.io/name": self.release_name,
+            "app.kubernetes.io/instance": self.release_name,
+        }
 
         if len(self.project.maintainer) > 0:
-            app_labels['maintainers'] = ".".join(self.project.maintainer).replace(' ', '_')
-            app_labels["maintainer"] = self.project.maintainer[0].replace(' ', '_')
+            app_labels["maintainers"] = ".".join(self.project.maintainer).replace(
+                " ", "_"
+            )
+            app_labels["maintainer"] = self.project.maintainer[0].replace(" ", "_")
 
-        app_labels['version'] = run_properties.versioning.identifier
+        app_labels["version"] = run_properties.versioning.identifier
 
         if run_properties.versioning.revision:
-            app_labels['revision'] = run_properties.versioning.revision
+            app_labels["revision"] = run_properties.versioning.revision
 
         return app_labels
 
     def _to_annotations(self) -> Dict:
-        return {'description': self.project.description}
+        return {"description": self.project.description}
 
     def _to_image_annotation(self) -> Dict:
-        return {'image': self._get_image()}
+        return {"image": self._get_image()}
 
-    def _to_object_meta(self, name: Optional[str] = None, annotations: Optional[Dict] = None):
-        return V1ObjectMeta(name=name if name else self.release_name, labels=self._to_labels(),
-                            annotations=annotations)
+    def _to_object_meta(
+        self, name: Optional[str] = None, annotations: Optional[Dict] = None
+    ):
+        return V1ObjectMeta(
+            name=name if name else self.release_name,
+            labels=self._to_labels(),
+            annotations=annotations,
+        )
 
     def _to_selector(self):
-        return V1LabelSelector(match_labels={"app.kubernetes.io/instance": self.release_name,
-                                             "app.kubernetes.io/name": self.release_name})
+        return V1LabelSelector(
+            match_labels={
+                "app.kubernetes.io/instance": self.release_name,
+                "app.kubernetes.io/name": self.release_name,
+            }
+        )
 
     @staticmethod
     def _to_k8s_model(values: dict, model_type):
-        return ApiClient()._ApiClient__deserialize(values, model_type)  # pylint: disable=protected-access
+        return ApiClient()._ApiClient__deserialize(  # pylint: disable=protected-access
+            values, model_type
+        )
 
     @staticmethod
     def _to_probe(probe: Probe, defaults: dict, target: Target) -> V1Probe:
         values = defaults.copy()
         values.update(probe.values)
         v1_probe: V1Probe = ChartBuilder._to_k8s_model(values, V1Probe)
         path = probe.path.get_value(target)
-        v1_probe.http_get = V1HTTPGetAction(path='/health' if path is None else path, port='port-0')
+        v1_probe.http_get = V1HTTPGetAction(
+            path="/health" if path is None else path, port="port-0"
+        )
         return v1_probe
 
     def to_service(self) -> V1Service:
-        service_ports = list(map(lambda key: V1ServicePort(port=key, target_port=self.mappings[key], protocol="TCP",
-                                                           name=f"{key}-webservice-port"), self.mappings.keys()))
+        service_ports = list(
+            map(
+                lambda key: V1ServicePort(
+                    port=key,
+                    target_port=self.mappings[key],
+                    protocol="TCP",
+                    name=f"{key}-webservice-port",
+                ),
+                self.mappings.keys(),
+            )
+        )
 
-        return V1Service(api_version='v1', kind='Service',
-                         metadata=V1ObjectMeta(annotations=self._to_annotations(), name=self.release_name,
-                                               labels=self._to_labels()),
-                         spec=V1ServiceSpec(type="ClusterIP", ports=service_ports,
-                                            selector=self._to_selector().match_labels))
+        return V1Service(
+            api_version="v1",
+            kind="Service",
+            metadata=V1ObjectMeta(
+                annotations=self._to_annotations(),
+                name=self.release_name,
+                labels=self._to_labels(),
+            ),
+            spec=V1ServiceSpec(
+                type="ClusterIP",
+                ports=service_ports,
+                selector=self._to_selector().match_labels,
+            ),
+        )
 
     def to_job(self) -> V1Job:
         job_container = V1Container(
-            name=self.release_name, image=self._get_image(), env=self._get_env_vars(), image_pull_policy="Always",
-            resources=self._get_resources()
+            name=self.release_name,
+            image=self._get_image(),
+            env=self._get_env_vars(),
+            image_pull_policy="Always",
+            resources=self._get_resources(),
         )
 
         pod_template = V1PodTemplateSpec(
             metadata=self._to_object_meta(annotations=self._to_image_annotation()),
-            spec=V1PodSpec(containers=[job_container], service_account=self.release_name,
-                           service_account_name=self.release_name, restart_policy="Never")
+            spec=V1PodSpec(
+                containers=[job_container],
+                service_account=self.release_name,
+                service_account_name=self.release_name,
+                restart_policy="Never",
+            ),
         )
 
         defaults = with_target(self.config_defaults.job_defaults, self.target)
         specified = defaults | with_target(self.project.job.job, self.target)
 
         template_dict = to_dict(pod_template)
-        specified['template'] = template_dict
+        specified["template"] = template_dict
         spec: V1JobSpec = ChartBuilder._to_k8s_model(specified, V1JobSpec)
 
-        return V1Job(api_version='batch/v1', kind='Job', metadata=self._to_object_meta(), spec=spec)
+        return V1Job(
+            api_version="batch/v1",
+            kind="Job",
+            metadata=self._to_object_meta(),
+            spec=spec,
+        )
 
     def to_cron_job(self) -> V1CronJob:
         values = self.project.job.cron
         job_template = V1JobTemplateSpec(spec=self.to_job().spec)
         template_dict = to_dict(job_template)
-        values['jobTemplate'] = template_dict
-        v1_cron_job_spec: V1CronJobSpec = ChartBuilder._to_k8s_model(values, V1CronJobSpec)
-        return V1CronJob(api_version='batch/v1', kind='CronJob', metadata=self._to_object_meta(), spec=v1_cron_job_spec)
+        values["jobTemplate"] = template_dict
+        v1_cron_job_spec: V1CronJobSpec = ChartBuilder._to_k8s_model(
+            values, V1CronJobSpec
+        )
+        return V1CronJob(
+            api_version="batch/v1",
+            kind="CronJob",
+            metadata=self._to_object_meta(),
+            spec=v1_cron_job_spec,
+        )
 
     def to_spark_application(self) -> V1SparkApplication:
         return V1SparkApplication(
-            schedule=self._get_job().cron['schedule'],
+            schedule=self._get_job().cron["schedule"],
             body=to_spark_body(
                 project_name=self.release_name,
                 env_vars=get_env_variables(self.project, self.target),
-                spark=self._get_job().spark
+                spark=self._get_job().spark,
             ),
         )
 
     def to_spark_config_map(self) -> V1ConfigMap:
         return V1ConfigMap(
-            api_version='v1',
-            kind='ConfigMap',
+            api_version="v1",
+            kind="ConfigMap",
             data=get_spark_config_map_data(),
-            metadata=self._to_object_meta()
+            metadata=self._to_object_meta(),
         )
 
     def __find_default_port(self) -> int:
         found = next(iter(self.mappings.keys()))
         if found:
             return int(found)
         raise KeyError("No default port found. Did you define a port mapping?")
 
     def create_host_wrappers(self) -> list[HostWrapper]:
-        default_hosts: list[Host] = Traefik.from_config(self.config_defaults.treafik_defaults).hosts
+        default_hosts: list[Host] = Traefik.from_config(
+            self.config_defaults.treafik_defaults
+        ).hosts
 
-        hosts: list[Host] = self.deployment.traefik.hosts if self.deployment.traefik else []
+        hosts: list[Host] = (
+            self.deployment.traefik.hosts if self.deployment.traefik else []
+        )
 
         first_host = next(iter(hosts), None)
-        service_port = first_host.service_port if first_host and first_host.service_port else self.__find_default_port()
-
-        configured_addresses = self.config_defaults.white_lists['addresses']
-        address_dictionary = {address['name']: address['values'] for address in configured_addresses}
+        service_port = (
+            first_host.service_port
+            if first_host and first_host.service_port
+            else self.__find_default_port()
+        )
 
-        def to_white_list(configured: Optional[TargetProperty[list[str]]]) -> dict[str, list[str]]:
-            white_lists = self.config_defaults.white_lists['default'].copy()
+        configured_addresses = self.config_defaults.white_lists["addresses"]
+        address_dictionary = {
+            address["name"]: address["values"] for address in configured_addresses
+        }
+
+        def to_white_list(
+            configured: Optional[TargetProperty[list[str]]],
+        ) -> dict[str, list[str]]:
+            white_lists = self.config_defaults.white_lists["default"].copy()
             if configured and configured.get_value(self.target):
                 white_lists.extend(configured.get_value(self.target))
 
-            return dict(filter(lambda x: x[0] in white_lists, address_dictionary.items()))
-
-        return [HostWrapper(host=host, name=self.release_name, index=idx, service_port=service_port,
-                            white_lists=to_white_list(host.whitelists)) for
-                idx, host in enumerate(hosts if hosts else default_hosts)]
+            return dict(
+                filter(lambda x: x[0] in white_lists, address_dictionary.items())
+            )
+
+        return [
+            HostWrapper(
+                host=host,
+                name=self.release_name,
+                index=idx,
+                service_port=service_port,
+                white_lists=to_white_list(host.whitelists),
+            )
+            for idx, host in enumerate(hosts if hosts else default_hosts)
+        ]
 
     def to_ingress_routes(self) -> V1AlphaIngressRoute:
         hosts = self.create_host_wrappers()
 
-        return V1AlphaIngressRoute(metadata=self._to_object_meta(), hosts=hosts, target=self.target,
-                                   pr_number=self.step_input.run_properties.versioning.pr_number)
+        return V1AlphaIngressRoute(
+            metadata=self._to_object_meta(),
+            hosts=hosts,
+            target=self.target,
+            pr_number=self.step_input.run_properties.versioning.pr_number,
+        )
 
     def to_middlewares(self) -> dict[str, V1AlphaMiddleware]:
         hosts: list[HostWrapper] = self.create_host_wrappers()
 
         def to_metadata(host: HostWrapper) -> V1ObjectMeta:
             metadata = self._to_object_meta(name=host.full_name)
             # metadata.annotations = host.white_lists
-            metadata.annotations = {k: ", ".join(v) for k, v in host.white_lists.items()}
+            metadata.annotations = {
+                k: ", ".join(v) for k, v in host.white_lists.items()
+            }
             return metadata
 
-        return {host.full_name: V1AlphaMiddleware(
-            metadata=to_metadata(host),
-            source_ranges=list(itertools.chain(*host.white_lists.values()))) for host in hosts}
+        return {
+            host.full_name: V1AlphaMiddleware(
+                metadata=to_metadata(host),
+                source_ranges=list(itertools.chain(*host.white_lists.values())),
+            )
+            for host in hosts
+        }
 
     def to_service_account(self) -> V1ServiceAccount:
-        return V1ServiceAccount(api_version="v1", kind="ServiceAccount", metadata=self._to_object_meta(),
-                                image_pull_secrets=[V1LocalObjectReference("bigdataregistry")])
+        return V1ServiceAccount(
+            api_version="v1",
+            kind="ServiceAccount",
+            metadata=self._to_object_meta(),
+            image_pull_secrets=[V1LocalObjectReference("bigdataregistry")],
+        )
 
     def to_sealed_secrets(self) -> V1SealedSecret:
         secrets: dict[str, str] = {}
         for secret in self.sealed_secrets:
             secrets[secret.key] = secret.get_value(self.target)
 
         return V1SealedSecret(name=self.release_name, secrets=secrets)
@@ -286,23 +433,29 @@
         cpus = resources.cpus if resources and resources.cpus else defaults.cpus
         cpus_limit = cpus.get_value(target=target) * 1000.0
         cpus_request = cpus_limit * CPU_REQUEST_SCALE_FACTOR
 
         mem = resources.mem if resources and resources.mem else defaults.mem
         mem_limit = mem.get_value(target=target)
         mem_request = mem_limit * MEM_REQUEST_SCALE_FACTOR
-        return V1ResourceRequirements(limits={'cpu': f'{int(cpus_limit)}m', 'memory': f'{int(mem_limit)}Mi'},
-                                      requests={'cpu': f'{int(cpus_request)}m', 'memory': f'{int(mem_request)}Mi'})
+        return V1ResourceRequirements(
+            limits={"cpu": f"{int(cpus_limit)}m", "memory": f"{int(mem_limit)}Mi"},
+            requests={
+                "cpu": f"{int(cpus_request)}m",
+                "memory": f"{int(mem_request)}Mi",
+            },
+        )
 
     def _get_image(self):
         docker_image = self.step_input.required_artifact
         if not docker_image or docker_image.artifact_type != ArtifactType.DOCKER_IMAGE:
             raise ValueError(
-                f'Required artifact of type {ArtifactType.DOCKER_IMAGE.name} must be defined')  # pylint: disable=E1101
-        return docker_image.spec['image']
+                f"Required artifact of type {ArtifactType.DOCKER_IMAGE.name} must be defined"
+            )  # pylint: disable=E1101
+        return docker_image.spec["image"]
 
     def _get_resources(self):
         resources = self.project.kubernetes.resources
         defaults = self.config_defaults.resources_defaults
         return ChartBuilder._to_resources(resources, defaults, self.target)
 
     def _get_kubernetes(self) -> Kubernetes:
@@ -314,37 +467,57 @@
     def _get_job(self) -> Job:
         job = self._get_kubernetes().job
         if job is None:
             raise AttributeError("deployment.kubernetes.job field should be set")
         return job
 
     def _get_env_vars(self):
-        raw_env_vars = {e.key: e.get_value(self.target) for e in self.env if e.get_value(self.target) is not None}
-        substituted = substitute_namespaces(raw_env_vars,
-                                            {p.to_name for p in self.deploy_set.all_projects},
-                                            {p.to_name for p in self.deploy_set.projects_to_deploy},
-                                            self.step_input.run_properties.versioning.pr_number)
+        raw_env_vars = {
+            e.key: e.get_value(self.target)
+            for e in self.env
+            if e.get_value(self.target) is not None
+        }
+        substituted = substitute_namespaces(
+            raw_env_vars,
+            {p.to_name for p in self.deploy_set.all_projects},
+            {p.to_name for p in self.deploy_set.projects_to_deploy},
+            self.step_input.run_properties.versioning.pr_number,
+        )
 
-        env_vars = [V1EnvVar(name=key, value=value) for key, value in substituted.items()]
+        env_vars = [
+            V1EnvVar(name=key, value=value) for key, value in substituted.items()
+        ]
 
         sealed_for_target = list(
-            filter(lambda v: v.get_value(self.target) is not None, self.sealed_secrets))
-        sealed_secrets = list(map(lambda e: V1EnvVar(name=e.key, value_from=V1EnvVarSource(
-            secret_key_ref=V1SecretKeySelector(key=e.key, name=self.release_name, optional=False))),
-                                  sealed_for_target))
+            filter(lambda v: v.get_value(self.target) is not None, self.sealed_secrets)
+        )
+        sealed_secrets = list(
+            map(
+                lambda e: V1EnvVar(
+                    name=e.key,
+                    value_from=V1EnvVarSource(
+                        secret_key_ref=V1SecretKeySelector(
+                            key=e.key, name=self.release_name, optional=False
+                        )
+                    ),
+                ),
+                sealed_for_target,
+            )
+        )
         return env_vars + sealed_secrets
 
     @property
     def is_cron_job(self) -> bool:
         return len(self._get_job().cron.keys()) > 0
 
     def to_deployment(self) -> V1Deployment:
-
         ports = [
-            V1ContainerPort(container_port=self.mappings[key], protocol="TCP", name=f'port-{idx}')
+            V1ContainerPort(
+                container_port=self.mappings[key], protocol="TCP", name=f"port-{idx}"
+            )
             for idx, key in enumerate(self.mappings.keys())
         ]
 
         project = self.project
         resources = project.resources
         kubernetes = project.kubernetes
         defaults = self.config_defaults.resources_defaults
@@ -355,67 +528,84 @@
             env=self._get_env_vars(),
             ports=ports,
             image_pull_policy="Always",
             resources=ChartBuilder._to_resources(resources, defaults, self.target),
             liveness_probe=ChartBuilder._to_probe(
                 kubernetes.liveness_probe,
                 self.config_defaults.liveness_probe_defaults,
-                self.target
-            ) if kubernetes.liveness_probe else None,
+                self.target,
+            )
+            if kubernetes.liveness_probe
+            else None,
             startup_probe=ChartBuilder._to_probe(
                 kubernetes.startup_probe,
                 self.config_defaults.startup_probe_defaults,
-                self.target)
-            if kubernetes.startup_probe else None
+                self.target,
+            )
+            if kubernetes.startup_probe
+            else None,
         )
 
         instances = resources.instances if resources.instances else defaults.instances
 
         return V1Deployment(
             api_version="apps/v1",
             kind="Deployment",
-            metadata=V1ObjectMeta(annotations=self._to_annotations(), name=self.release_name,
-                                  labels=self._to_labels()),
+            metadata=V1ObjectMeta(
+                annotations=self._to_annotations(),
+                name=self.release_name,
+                labels=self._to_labels(),
+            ),
             spec=V1DeploymentSpec(
                 replicas=instances.get_value(target=self.target),
                 template=V1PodTemplateSpec(
                     metadata=self._to_object_meta(),
-                    spec=V1PodSpec(containers=[container], service_account=self.release_name,
-                                   service_account_name=self.release_name),
+                    spec=V1PodSpec(
+                        containers=[container],
+                        service_account=self.release_name,
+                        service_account_name=self.release_name,
+                    ),
                 ),
                 strategy=V1DeploymentStrategy(
-                    rolling_update=V1RollingUpdateDeployment(max_surge="25%", max_unavailable="25%"),
-                    type="RollingUpdate"),
+                    rolling_update=V1RollingUpdateDeployment(
+                        max_surge="25%", max_unavailable="25%"
+                    ),
+                    type="RollingUpdate",
+                ),
                 selector=self._to_selector(),
             ),
         )
 
     def to_common_chart(self) -> dict[str, CustomResourceDefinition]:
-        chart = {'service-account': self.to_service_account()}
+        chart = {"service-account": self.to_service_account()}
 
         if self.sealed_secrets:
-            chart['sealed-secrets'] = self.to_sealed_secrets()
+            chart["sealed-secrets"] = self.to_sealed_secrets()
 
         return chart
 
 
 def to_service_chart(builder: ChartBuilder) -> dict[str, CustomResourceDefinition]:
-    return builder.to_common_chart() | {
-        'deployment': builder.to_deployment(),
-        'service': builder.to_service(),
-        'ingress-https-route': builder.to_ingress_routes()
-    } | builder.to_middlewares()
+    return (
+        builder.to_common_chart()
+        | {
+            "deployment": builder.to_deployment(),
+            "service": builder.to_service(),
+            "ingress-https-route": builder.to_ingress_routes(),
+        }
+        | builder.to_middlewares()
+    )
 
 
 def to_job_chart(builder: ChartBuilder) -> dict[str, CustomResourceDefinition]:
-    return builder.to_common_chart() | {'job': builder.to_job()}
+    return builder.to_common_chart() | {"job": builder.to_job()}
 
 
 def to_cron_job_chart(builder: ChartBuilder) -> dict[str, CustomResourceDefinition]:
-    return builder.to_common_chart() | {'cronjob': builder.to_cron_job()}
+    return builder.to_common_chart() | {"cronjob": builder.to_cron_job()}
 
 
 def to_spark_job_chart(builder: ChartBuilder) -> dict[str, CustomResourceDefinition]:
     return builder.to_common_chart() | {
-        'spark': builder.to_spark_application(),
-        'config-map': builder.to_spark_config_map()
+        "spark": builder.to_spark_application(),
+        "config-map": builder.to_spark_config_map(),
     }
```

## mpyl/steps/deploy/k8s/helm.py

```diff
@@ -17,48 +17,71 @@
 description: A helm chart used by the MPyL pipeline
 type: application
 version: 0.1.0
 appVersion: "{run_properties.versioning.identifier}"
 """
 
 
-def write_chart(chart: dict[str, CustomResourceDefinition], chart_path: Path, chart_metadata: str) -> None:
+def write_chart(
+    chart: dict[str, CustomResourceDefinition], chart_path: Path, chart_metadata: str
+) -> None:
     shutil.rmtree(chart_path, ignore_errors=True)
     template_path = chart_path / Path("templates")
     template_path.mkdir(parents=True, exist_ok=True)
 
-    with open(chart_path / Path("Chart.yaml"), mode='w+', encoding='utf-8') as file:
+    with open(chart_path / Path("Chart.yaml"), mode="w+", encoding="utf-8") as file:
         file.write(chart_metadata)
-    with open(chart_path / Path("values.yaml"), mode='w+', encoding='utf-8') as file:
-        file.write("# This file is intentionally left empty. All values in /templates have been pre-interpolated")
-
-    my_dictionary: dict[str, str] = dict(map(lambda item: (item[0], to_yaml(item[1])), chart.items()))
+    with open(chart_path / Path("values.yaml"), mode="w+", encoding="utf-8") as file:
+        file.write(
+            "# This file is intentionally left empty. All values in /templates have been pre-interpolated"
+        )
+
+    my_dictionary: dict[str, str] = dict(
+        map(lambda item: (item[0], to_yaml(item[1])), chart.items())
+    )
 
     for name, template in my_dictionary.items():
-        with open(template_path / name, mode='w+', encoding='utf-8') as file:
+        with open(template_path / name, mode="w+", encoding="utf-8") as file:
             file.write(template)
 
 
-def __remove_existing_chart(logger: Logger, chart_name: str, name_space: str, kube_context: str) -> Output:
-    found_chart = custom_check_output(logger, f"helm list -f ^{chart_name}$ -n {name_space}", capture_stdout=True)
+def __remove_existing_chart(
+    logger: Logger, chart_name: str, name_space: str, kube_context: str
+) -> Output:
+    found_chart = custom_check_output(
+        logger, f"helm list -f ^{chart_name}$ -n {name_space}", capture_stdout=True
+    )
     if chart_name in found_chart.message:
-        cmd = f"helm uninstall {chart_name} -n {name_space} --kube-context {kube_context}"
+        cmd = (
+            f"helm uninstall {chart_name} -n {name_space} --kube-context {kube_context}"
+        )
         return custom_check_output(Logger("helm"), cmd)
-    return Output(success=True, message=f"No existing chart {chart_name} found to delete")
+    return Output(
+        success=True, message=f"No existing chart {chart_name} found to delete"
+    )
 
 
-def install(logger: Logger, chart: dict[str, CustomResourceDefinition], step_input: Input, chart_name: str,
-            name_space: str, kube_context: str, delete_existing: bool = False) -> Output:
+def install(
+    logger: Logger,
+    chart: dict[str, CustomResourceDefinition],
+    step_input: Input,
+    chart_name: str,
+    name_space: str,
+    kube_context: str,
+    delete_existing: bool = False,
+) -> Output:
     if delete_existing:
         removed = __remove_existing_chart(logger, chart_name, name_space, kube_context)
         if not removed.success:
             return removed
 
     chart_path = Path(step_input.project.target_path) / "chart"
     logger.info(f"Writing HELM chart to {chart_path}")
-    write_chart(chart, chart_path, to_chart_metadata(chart_name, step_input.run_properties))
+    write_chart(
+        chart, chart_path, to_chart_metadata(chart_name, step_input.run_properties)
+    )
 
     cmd = f"helm upgrade -i {chart_name} -n {name_space} --kube-context {kube_context} {chart_path}"
     if step_input.dry_run:
         cmd = f"helm upgrade -i {chart_name} -n namespace --kube-context {kube_context} {chart_path} --debug --dry-run"
 
     return custom_check_output(logger, cmd)
```

## mpyl/steps/deploy/k8s/rancher.py

```diff
@@ -12,37 +12,43 @@
     project_id: str
     cluster_id: str
     cluster_env: str
     context: str
 
     @staticmethod
     def from_config(config: dict):
-        return ClusterConfig(project_id=config['clusterId'], cluster_id=config['clusterId'],
-                             cluster_env=config['clusterEnv'], context=config['context'])
+        return ClusterConfig(
+            project_id=config["clusterId"],
+            cluster_id=config["clusterId"],
+            cluster_env=config["clusterEnv"],
+            context=config["context"],
+        )
 
 
 def cluster_config(target: Target, run_properties: RunProperties) -> ClusterConfig:
-    cluster_configs = run_properties.config['kubernetes']['rancher']['cluster']
+    cluster_configs = run_properties.config["kubernetes"]["rancher"]["cluster"]
 
     if target in {Target.PULL_REQUEST, Target.PULL_REQUEST_BASE}:
-        return ClusterConfig.from_config(cluster_configs['test'])
+        return ClusterConfig.from_config(cluster_configs["test"])
     if target == Target.ACCEPTANCE:
-        return ClusterConfig.from_config(cluster_configs['acceptance'])
+        return ClusterConfig.from_config(cluster_configs["acceptance"])
     if target == Target.PRODUCTION:
-        return ClusterConfig.from_config(cluster_configs['production'])
+        return ClusterConfig.from_config(cluster_configs["production"])
     raise ValueError(f"Unknown target {target}")
 
 
 def rancher_namespace_metadata(namespace: str, step_input: Input):
-    rancher_config = cluster_config(step_input.run_properties.target, step_input.run_properties)
+    rancher_config = cluster_config(
+        step_input.run_properties.target, step_input.run_properties
+    )
 
     return {
-        'annotations': {
-            'field.cattle.io/projectId': f'{rancher_config.cluster_id}:{rancher_config.project_id}',
-            'lifecycle.cattle.io/create.namespace-auth': 'true'
+        "annotations": {
+            "field.cattle.io/projectId": f"{rancher_config.cluster_id}:{rancher_config.project_id}",
+            "lifecycle.cattle.io/create.namespace-auth": "true",
         },
-        'labels': {
-            'field.cattle.io/projectId': rancher_config.project_id,
-            'kubernetes.io/metadata.name': namespace
+        "labels": {
+            "field.cattle.io/projectId": rancher_config.project_id,
+            "kubernetes.io/metadata.name": namespace,
         },
-        'name': namespace
+        "name": namespace,
     }
```

## mpyl/steps/deploy/k8s/resources/__init__.py

```diff
@@ -13,29 +13,36 @@
 from ruamel.yaml import YAML
 
 yaml = YAML()
 
 
 class CustomResourceDefinition:
     openapi_types = {
-        'api_version': 'str',
-        'kind': 'str',
-        'metadata': 'V1ObjectMeta',
-        'spec': 'dict'
+        "api_version": "str",
+        "kind": "str",
+        "metadata": "V1ObjectMeta",
+        "spec": "dict",
     }
 
     attribute_map = {
-        'api_version': 'apiVersion',
-        'kind': 'kind',
-        'metadata': 'metadata',
-        'spec': 'spec'
+        "api_version": "apiVersion",
+        "kind": "kind",
+        "metadata": "metadata",
+        "spec": "spec",
     }
 
-    def __init__(self, api_version: str, kind: str, metadata: V1ObjectMeta, spec: dict,
-                 local_vars_configuration=None, schema: Optional[str] = None):  # noqa: E501
+    def __init__(
+        self,
+        api_version: str,
+        kind: str,
+        metadata: V1ObjectMeta,
+        spec: dict,
+        local_vars_configuration=None,
+        schema: Optional[str] = None,
+    ):  # noqa: E501
         """V1CSIDriver - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._api_version = api_version
         self._kind = kind
@@ -81,66 +88,81 @@
 
     @property
     def spec(self) -> dict:
         return self._spec
 
     @spec.setter
     def spec(self, spec):
-        if self.local_vars_configuration.client_side_validation and spec is None:  # noqa: E501
-            raise ValueError("Invalid value for `spec`, must not be `None`")  # noqa: E501
+        if (
+            self.local_vars_configuration.client_side_validation and spec is None
+        ):  # noqa: E501
+            raise ValueError(
+                "Invalid value for `spec`, must not be `None`"
+            )  # noqa: E501
         self._spec = spec
 
 
 def to_dict(obj):
     result = {}
 
     for attr, _ in six.iteritems(obj.openapi_types):
         value = getattr(obj, attr)
         key = obj.attribute_map.get(attr)
         if isinstance(value, list):
-            result[key] = list(map(
-                lambda x: to_dict(x) if hasattr(x, "to_dict") else x,
-                value
-            ))
+            result[key] = list(
+                map(lambda x: to_dict(x) if hasattr(x, "to_dict") else x, value)
+            )
         elif hasattr(value, "to_dict"):
             result[key] = to_dict(value)
         elif isinstance(value, dict):
-            result[key] = dict(map(
-                lambda item: (item[0], to_dict(item[1]))
-                if hasattr(item[1], "to_dict") else item,
-                value.items()
-            ))
+            result[key] = dict(
+                map(
+                    lambda item: (item[0], to_dict(item[1]))
+                    if hasattr(item[1], "to_dict")
+                    else item,
+                    value.items(),
+                )
+            )
         else:
             result[key] = value
 
     return result
 
 
 def to_yaml(resource: object) -> str:
     def remove_none(obj):
         if isinstance(obj, (list, tuple, set)):
             return type(obj)(remove_none(x) for x in obj if x is not None)
         if isinstance(obj, dict):
-            return type(obj)((remove_none(k), remove_none(v))
-                             for k, v in obj.items() if k is not None and v is not None)
+            return type(obj)(
+                (remove_none(k), remove_none(v))
+                for k, v in obj.items()
+                if k is not None and v is not None
+            )
         return obj
 
-    resource_dict = to_dict(resource) if (
-            hasattr(resource, "openapi_types") and hasattr(resource, "attribute_map")) else {}
+    resource_dict = (
+        to_dict(resource)
+        if (hasattr(resource, "openapi_types") and hasattr(resource, "attribute_map"))
+        else {}
+    )
     yaml_values = remove_none(resource_dict)
 
-    if hasattr(resource, 'schema') and resource.schema:
-        template = pkgutil.get_data(__name__, f'schema/{resource.schema}')
+    if hasattr(resource, "schema") and resource.schema:
+        template = pkgutil.get_data(__name__, f"schema/{resource.schema}")
         if template:
-            schema = yaml.load(template.decode('utf-8'))
+            schema = yaml.load(template.decode("utf-8"))
             try:
                 jsonschema.validate(yaml_values, schema)
             except ValidationError as err:
                 raise ValueError(
-                    f'Schema validation failed with {err.message} at {".".join(map(str, err.schema_path))}') from err
+                    f'Schema validation failed with {err.message} at {".".join(map(str, err.schema_path))}'
+                ) from err
         else:
-            raise ValueError(f'Schema {resource.schema} defined but not found in package')
+            raise ValueError(
+                f"Schema {resource.schema} defined but not found in package"
+            )
 
     stream = StringIO()
     yaml.dump(yaml_values, stream)
 
     return stream.getvalue()
```

## mpyl/steps/deploy/k8s/resources/sealed_secret.py

```diff
@@ -5,11 +5,17 @@
 from kubernetes.client import V1ObjectMeta
 
 from . import CustomResourceDefinition
 
 
 class V1SealedSecret(CustomResourceDefinition):
     def __init__(self, name: str, secrets: dict[str, str]):
-        super().__init__(api_version="bitnami.com/v1alpha1", kind="SealedSecret",
-                         metadata=V1ObjectMeta(name=name, labels={'chart': 'service-0.1.0'},
-                                               annotations={'sealedsecrets.bitnami.com/cluster-wide': 'true'}),
-                         spec={'encryptedData': secrets})
+        super().__init__(
+            api_version="bitnami.com/v1alpha1",
+            kind="SealedSecret",
+            metadata=V1ObjectMeta(
+                name=name,
+                labels={"chart": "service-0.1.0"},
+                annotations={"sealedsecrets.bitnami.com/cluster-wide": "true"},
+            ),
+            spec={"encryptedData": secrets},
+        )
```

## mpyl/steps/deploy/k8s/resources/spark.py

```diff
@@ -6,127 +6,125 @@
 from kubernetes.client import V1ObjectMeta
 
 from .. import CustomResourceDefinition
 
 
 def to_spark_body(project_name: str, env_vars: dict, spark: dict) -> dict:
     static_body = {
-        'type': 'Scala',
-        'mode': 'cluster',
-        'imagePullPolicy': 'Always',
-        'sparkVersion': '3.1.1',
-        'restartPolicy': {
-            'type': 'Never'
-        },
-        'sparkConfigMap': project_name,
-        'image': 'bigdataregistry.azurecr.io/send-slack-notification:PR-1231',
-        'arguments': [
-            'python',
-            '-m',
-            'job_testing_mpl_k8s.main_send_slack_notification'
+        "type": "Scala",
+        "mode": "cluster",
+        "imagePullPolicy": "Always",
+        "sparkVersion": "3.1.1",
+        "restartPolicy": {"type": "Never"},
+        "sparkConfigMap": project_name,
+        "image": "bigdataregistry.azurecr.io/send-slack-notification:PR-1231",
+        "arguments": [
+            "python",
+            "-m",
+            "job_testing_mpl_k8s.main_send_slack_notification",
         ],
-        'driver': {
-            'cores': 1,
-            'coreLimit': '1200m',
-            'memory': '5G',
-            'memoryOverhead': '1024',
-            'labels': {
-                'version': '3.1.1'
-            },
-            'serviceAccount': project_name,
-            'envVars': env_vars,
-            'envSecretKeyRefs': None
+        "driver": {
+            "cores": 1,
+            "coreLimit": "1200m",
+            "memory": "5G",
+            "memoryOverhead": "1024",
+            "labels": {"version": "3.1.1"},
+            "serviceAccount": project_name,
+            "envVars": env_vars,
+            "envSecretKeyRefs": None,
         },
-        'executor': {
-            'cores': 1,
-            'instances': 1,
-            'memory': '3G',
-            'memoryOverhead': '2048',
-            'labels': {
-                'version': '3.1.1'
-            },
-            'envVars': env_vars,
-            'envSecretKeyRefs': None
+        "executor": {
+            "cores": 1,
+            "instances": 1,
+            "memory": "3G",
+            "memoryOverhead": "2048",
+            "labels": {"version": "3.1.1"},
+            "envVars": env_vars,
+            "envSecretKeyRefs": None,
         },
-        'deps': {
-            'jars': [
-                'https://repo1.maven.org/maven2/com/microsoft/sqlserver/'
-                'mssql-jdbc/11.2.1.jre8/mssql-jdbc-11.2.1.jre8.jar'
+        "deps": {
+            "jars": [
+                "https://repo1.maven.org/maven2/com/microsoft/sqlserver/"
+                "mssql-jdbc/11.2.1.jre8/mssql-jdbc-11.2.1.jre8.jar"
             ]
         },
-        'sparkConf': {
-            'spark.driver.extraClassPath': 'mssql-jdbc-11.2.1.jre8.jar',
-            'spark.executor.extraClassPath': 'mssql-jdbc-11.2.1.jre8.jar',
-            'spark.sql.legacy.timeParserPolicy': 'LEGACY',
-            'spark.sql.broadcastTimeout': '600'
-        }
+        "sparkConf": {
+            "spark.driver.extraClassPath": "mssql-jdbc-11.2.1.jre8.jar",
+            "spark.executor.extraClassPath": "mssql-jdbc-11.2.1.jre8.jar",
+            "spark.sql.legacy.timeParserPolicy": "LEGACY",
+            "spark.sql.broadcastTimeout": "600",
+        },
     }
 
     return static_body | spark
 
 
 def get_spark_config_map_data() -> dict:
     return {
-        'log4j.properties':
-            '#\n'
-            '# Licensed to the Apache Software Foundation (ASF) under one or more\n'
-            '# contributor license agreements.  See the NOTICE file distributed with\n'
-            '# this work for additional information regarding copyright ownership.\n'
-            '# The ASF licenses this file to You under the Apache License, Version 2.0\n'
-            '# (the "License"); you may not use this file except in compliance with\n'
-            '# the License.  You may obtain a copy of the License at\n'
-            '#\n'
-            '#    http://www.apache.org/licenses/LICENSE-2.0\n'
-            '#\n'
-            '# Unless required by applicable law or agreed to in writing, software\n'
-            '# distributed under the License is distributed on an "AS IS" BASIS,\n'
-            '# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.\n'
-            '# See the License for the specific language governing permissions and\n'
-            '# limitations under the License.\n'
-            '#\n'
-            '#log everything to file at the beginning\n'
-            'log4j.rootCategory=INFO, console, sparklog\n'
-            '#afterwards log only our messages to the console\n'
-            'log4j.logger.nl.vandebron.sparkplug=INFO, console\n'
-            '#configure ConsoleAppender\n'
-            'log4j.appender.console=org.apache.log4j.ConsoleAppender\n'
-            'log4j.appender.console.target=System.out\n'
-            'log4j.appender.console.layout=org.apache.log4j.PatternLayout\n'
-            'log4j.appender.console.layout.ConversionPattern=%d{yy/MM/dd HH:mm:ss} %p %c{1}: %m%n\n'
-            'log4j.appender.sparklog=org.apache.log4j.FileAppender\n'
-            '#this must be overwritten programmatically when setting the appender\n'
-            'log4j.appender.sparklog.File=/dev/null\n'
-            'log4j.appender.sparklog.layout=org.apache.log4j.PatternLayout\n'
-            'log4j.appender.sparklog.layout.ConversionPattern=%d %-5p [%c{1}] %m%n\n'
-            'log4j.appender.sparklog.Threshold=INFO\n'
-            'log4j.appender.sparklog.Append=true\n'
-            '# Set the default spark-shell log level to WARN. When running the spark-shell, the\n'
-            '# log level for this class is used to overwrite the root logger\'s log level, so that\n'
-            '# the user can have different defaults for the shell and regular Spark apps.\n'
-            'log4j.logger.org.apache.spark.repl.Main=WARN\n'
-            '# Settings to quiet third party logs that are too verbose\n'
-            'log4j.logger.org.spark_project.jetty=WARN\n'
-            'log4j.logger.org.spark_project.jetty.util.component.AbstractLifeCycle=ERROR\n'
-            'log4j.logger.org.apache.spark.repl.SparkIMain$exprTyper=INFO\n'
-            'log4j.logger.org.apache.spark.repl.SparkILoop$SparkILoopInterpreter=INFO\n'
-            'log4j.logger.org.apache.parquet=ERROR\n'
-            'log4j.logger.parquet=ERROR\n'
-            '# SPARK-9183: Settings to avoid annoying messages when looking up '
-            'nonexistent UDFs in SparkSQL with Hive support\n'
-            'log4j.logger.org.apache.hadoop.hive.metastore.RetryingHMSHandler=FATAL\n'
-            'log4j.logger.org.apache.hadoop.hive.ql.exec.FunctionRegistry=ERROR',
+        "log4j.properties": "#\n"
+        "# Licensed to the Apache Software Foundation (ASF) under one or more\n"
+        "# contributor license agreements.  See the NOTICE file distributed with\n"
+        "# this work for additional information regarding copyright ownership.\n"
+        "# The ASF licenses this file to You under the Apache License, Version 2.0\n"
+        '# (the "License"); you may not use this file except in compliance with\n'
+        "# the License.  You may obtain a copy of the License at\n"
+        "#\n"
+        "#    http://www.apache.org/licenses/LICENSE-2.0\n"
+        "#\n"
+        "# Unless required by applicable law or agreed to in writing, software\n"
+        '# distributed under the License is distributed on an "AS IS" BASIS,\n'
+        "# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.\n"
+        "# See the License for the specific language governing permissions and\n"
+        "# limitations under the License.\n"
+        "#\n"
+        "#log everything to file at the beginning\n"
+        "log4j.rootCategory=INFO, console, sparklog\n"
+        "#afterwards log only our messages to the console\n"
+        "log4j.logger.nl.vandebron.sparkplug=INFO, console\n"
+        "#configure ConsoleAppender\n"
+        "log4j.appender.console=org.apache.log4j.ConsoleAppender\n"
+        "log4j.appender.console.target=System.out\n"
+        "log4j.appender.console.layout=org.apache.log4j.PatternLayout\n"
+        "log4j.appender.console.layout.ConversionPattern=%d{yy/MM/dd HH:mm:ss} %p %c{1}: %m%n\n"
+        "log4j.appender.sparklog=org.apache.log4j.FileAppender\n"
+        "#this must be overwritten programmatically when setting the appender\n"
+        "log4j.appender.sparklog.File=/dev/null\n"
+        "log4j.appender.sparklog.layout=org.apache.log4j.PatternLayout\n"
+        "log4j.appender.sparklog.layout.ConversionPattern=%d %-5p [%c{1}] %m%n\n"
+        "log4j.appender.sparklog.Threshold=INFO\n"
+        "log4j.appender.sparklog.Append=true\n"
+        "# Set the default spark-shell log level to WARN. When running the spark-shell, the\n"
+        "# log level for this class is used to overwrite the root logger's log level, so that\n"
+        "# the user can have different defaults for the shell and regular Spark apps.\n"
+        "log4j.logger.org.apache.spark.repl.Main=WARN\n"
+        "# Settings to quiet third party logs that are too verbose\n"
+        "log4j.logger.org.spark_project.jetty=WARN\n"
+        "log4j.logger.org.spark_project.jetty.util.component.AbstractLifeCycle=ERROR\n"
+        "log4j.logger.org.apache.spark.repl.SparkIMain$exprTyper=INFO\n"
+        "log4j.logger.org.apache.spark.repl.SparkILoop$SparkILoopInterpreter=INFO\n"
+        "log4j.logger.org.apache.parquet=ERROR\n"
+        "log4j.logger.parquet=ERROR\n"
+        "# SPARK-9183: Settings to avoid annoying messages when looking up "
+        "nonexistent UDFs in SparkSQL with Hive support\n"
+        "log4j.logger.org.apache.hadoop.hive.metastore.RetryingHMSHandler=FATAL\n"
+        "log4j.logger.org.apache.hadoop.hive.ql.exec.FunctionRegistry=ERROR",
     }
 
 
 class V1SparkApplication(CustomResourceDefinition):
     def __init__(self, schedule: Optional[str], body: dict):
         if schedule:
-            super().__init__(api_version="sparkoperator.k8s.io/v1beta2", kind="ScheduledSparkApplication",
-                             metadata=V1ObjectMeta(name="sparkapplications.sparkoperator.k8s.io"),
-                             schema="sparkoperator.k8s.io_scheduledsparkapplications.schema.yml",
-                             spec={'schedule': schedule,
-                                   'template': body})
+            super().__init__(
+                api_version="sparkoperator.k8s.io/v1beta2",
+                kind="ScheduledSparkApplication",
+                metadata=V1ObjectMeta(name="sparkapplications.sparkoperator.k8s.io"),
+                schema="sparkoperator.k8s.io_scheduledsparkapplications.schema.yml",
+                spec={"schedule": schedule, "template": body},
+            )
         else:
-            super().__init__(api_version="sparkoperator.k8s.io/v1beta2", kind="SparkApplication",
-                             metadata=V1ObjectMeta(name="sparkapplications.sparkoperator.k8s.io"),
-                             schema="sparkoperator.k8s.io_sparkapplications.schema.yml",
-                             spec={'spec': body})
+            super().__init__(
+                api_version="sparkoperator.k8s.io/v1beta2",
+                kind="SparkApplication",
+                metadata=V1ObjectMeta(name="sparkapplications.sparkoperator.k8s.io"),
+                schema="sparkoperator.k8s.io_sparkapplications.schema.yml",
+                spec={"spec": body},
+            )
```

## mpyl/steps/deploy/k8s/resources/traefik.py

```diff
@@ -16,35 +16,63 @@
     name: str
     index: int
     service_port: int
     white_lists: dict[str, list[str]]
 
     @property
     def full_name(self) -> str:
-        return f'{self.name}-ingress-{self.index}-whitelist'
+        return f"{self.name}-ingress-{self.index}-whitelist"
 
 
 class V1AlphaIngressRoute(CustomResourceDefinition):
-
-    def __init__(self, metadata: V1ObjectMeta, hosts: list[HostWrapper], target: Target,
-                 pr_number: Optional[int]):
+    def __init__(
+        self,
+        metadata: V1ObjectMeta,
+        hosts: list[HostWrapper],
+        target: Target,
+        pr_number: Optional[int],
+    ):
         def _interpolate_names(host: str, name: str) -> str:
-            host = host.replace('{SERVICE-NAME}', name)
+            host = host.replace("{SERVICE-NAME}", name)
             if pr_number:
-                return host.replace('{PR-NUMBER}', str(pr_number))
+                return host.replace("{PR-NUMBER}", str(pr_number))
             return host
 
-        routes = [{'kind': 'Rule', 'match': _interpolate_names(host.host.host.get_value(target), host.name),
-                   'services': [{'name': host.name, 'kind': 'Service', 'port': host.service_port}],
-                   'middlewares':
-                       [{'name': host.full_name}, {'name': 'traefik-https-redirect@kubernetescrd'}]} for host in hosts]
-
-        super().__init__(api_version='traefik.containo.us/v1alpha1', kind="IngressRoute", metadata=metadata,
-                         spec={'routes': routes, 'entryPoints': ['websecure'],
-                               'tls': {'secretName': 'le-prod-wildcard-cert'}}, schema='traefik.ingress.schema.yml')
+        routes = [
+            {
+                "kind": "Rule",
+                "match": _interpolate_names(
+                    host.host.host.get_value(target), host.name
+                ),
+                "services": [
+                    {"name": host.name, "kind": "Service", "port": host.service_port}
+                ],
+                "middlewares": [
+                    {"name": host.full_name},
+                    {"name": "traefik-https-redirect@kubernetescrd"},
+                ],
+            }
+            for host in hosts
+        ]
+
+        super().__init__(
+            api_version="traefik.containo.us/v1alpha1",
+            kind="IngressRoute",
+            metadata=metadata,
+            spec={
+                "routes": routes,
+                "entryPoints": ["websecure"],
+                "tls": {"secretName": "le-prod-wildcard-cert"},
+            },
+            schema="traefik.ingress.schema.yml",
+        )
 
 
 class V1AlphaMiddleware(CustomResourceDefinition):
-
     def __init__(self, metadata: V1ObjectMeta, source_ranges: list[str]):
-        super().__init__(api_version='traefik.containo.us/v1alpha1', kind="Middleware", metadata=metadata,
-                         spec={'ipWhiteList': {'sourceRange': source_ranges}}, schema='traefik.middleware.schema.yml')
+        super().__init__(
+            api_version="traefik.containo.us/v1alpha1",
+            kind="Middleware",
+            metadata=metadata,
+            spec={"ipWhiteList": {"sourceRange": source_ranges}},
+            schema="traefik.middleware.schema.yml",
+        )
```

## mpyl/steps/postdeploy/cypress_test.py

```diff
@@ -12,97 +12,163 @@
 from ...utilities.cypress import CypressConfig
 from ...utilities.docker import execute_with_stream
 from ...utilities.junit import TEST_OUTPUT_PATH_KEY, TEST_RESULTS_URL_KEY
 
 
 class CypressTest(Step):
     def __init__(self, logger: Logger) -> None:
-        super().__init__(logger, Meta(
-            name='Cypress Test',
-            description='Step to run cypress tests',
-            version='0.0.1',
-            stage=Stage.POST_DEPLOY
-        ), produced_artifact=ArtifactType.JUNIT_TESTS, required_artifact=ArtifactType.NONE)
+        super().__init__(
+            logger,
+            Meta(
+                name="Cypress Test",
+                description="Step to run cypress tests",
+                version="0.0.1",
+                stage=Stage.POST_DEPLOY,
+            ),
+            produced_artifact=ArtifactType.JUNIT_TESTS,
+            required_artifact=ArtifactType.NONE,
+        )
 
     def execute(self, step_input: Input) -> Output:
         if step_input.run_properties.target == Target.PRODUCTION:
-            return Output(success=True, message="Cypress tests are not run on production")
-
-        self._logger.info(f"Running cypress tests for project {step_input.project.name}")
+            return Output(
+                success=True, message="Cypress tests are not run on production"
+            )
+
+        self._logger.info(
+            f"Running cypress tests for project {step_input.project.name}"
+        )
         cypress_config = CypressConfig.from_config(step_input.run_properties.config)
         volume_path = os.path.join(os.getcwd(), cypress_config.cypress_source_code_path)
 
-        if step_input.project.dependencies and step_input.project.dependencies.postdeploy:
-            specs_string = ', '.join(step_input.project.dependencies.postdeploy)
+        if (
+            step_input.project.dependencies
+            and step_input.project.dependencies.postdeploy
+        ):
+            specs_string = ", ".join(step_input.project.dependencies.postdeploy)
         else:
             raise ValueError("No cypress specs are defined in the project dependencies")
 
         custom_image_tag = "mpyl/cypress"
-        docker.build(context_path=volume_path, tags=[custom_image_tag], file=f"{volume_path}/Dockerfile-mpyl")
-        docker_container = docker.run(image=custom_image_tag, interactive=True, detach=True,
-                                      volumes=[
-                                          (volume_path, "/cypress"),
-                                          (os.path.expanduser(cypress_config.kubectl_config_path), "/root/.kube/config")
-                                      ],
-                                      workdir="/cypress")
+        docker.build(
+            context_path=volume_path,
+            tags=[custom_image_tag],
+            file=f"{volume_path}/Dockerfile-mpyl",
+        )
+        docker_container = docker.run(
+            image=custom_image_tag,
+            interactive=True,
+            detach=True,
+            volumes=[
+                (volume_path, "/cypress"),
+                (
+                    os.path.expanduser(cypress_config.kubectl_config_path),
+                    "/root/.kube/config",
+                ),
+            ],
+            workdir="/cypress",
+        )
         if not isinstance(docker_container, Container):
             raise TypeError("Docker run command should return a container")
 
         reports_folder = f"reports/{step_input.project.name}"
-        artifact = input_to_artifact(artifact_type=ArtifactType.JUNIT_TESTS, step_input=step_input,
-                                     spec={TEST_OUTPUT_PATH_KEY: f"{volume_path}/{reports_folder}",
-                                           TEST_RESULTS_URL_KEY: ''})
+        artifact = input_to_artifact(
+            artifact_type=ArtifactType.JUNIT_TESTS,
+            step_input=step_input,
+            spec={
+                TEST_OUTPUT_PATH_KEY: f"{volume_path}/{reports_folder}",
+                TEST_RESULTS_URL_KEY: "",
+            },
+        )
 
         try:
-            execute_with_stream(logger=self._logger, container=docker_container,
-                                command='bash -c "cp cypress.env.json.example cypress.env.json && '
-                                        f"sed -i 's/acceptance/"
-                                        f"{CypressTest._target_to_test_target(step_input.run_properties.target)}"
-                                        f"/' cypress.env.json && "
-                                        f"sed -i 's/{{PR_NUMBER}}/{step_input.run_properties.versioning.pr_number}/' "
-                                        'cypress.env.json"',
-                                task_name="Preparing env file")
-            execute_with_stream(logger=self._logger, container=docker_container, command="yarn install",
-                                task_name="Running yarn install")
-            execute_with_stream(logger=self._logger, container=docker_container, command="yarn cypress install",
-                                task_name="Installing cypress")
-            execute_with_stream(logger=self._logger, container=docker_container, command="yarn cypress verify",
-                                task_name="Verifying cypress")
-            execute_with_stream(logger=self._logger, container=docker_container, command="yarn tsc",
-                                task_name="Compiling typescript")
-            execute_with_stream(logger=self._logger, container=docker_container, command=f"rm -rf {reports_folder}",
-                                task_name="Remove old report files")
-
-            run_command = f'bash -c "yarn cypress run --spec {specs_string} --reporter-options mochaFile=' \
-                          f'"{reports_folder}/[hash].xml" || true"'
+            execute_with_stream(
+                logger=self._logger,
+                container=docker_container,
+                command='bash -c "cp cypress.env.json.example cypress.env.json && '
+                f"sed -i 's/acceptance/"
+                f"{CypressTest._target_to_test_target(step_input.run_properties.target)}"
+                f"/' cypress.env.json && "
+                f"sed -i 's/{{PR_NUMBER}}/{step_input.run_properties.versioning.pr_number}/' "
+                'cypress.env.json"',
+                task_name="Preparing env file",
+            )
+            execute_with_stream(
+                logger=self._logger,
+                container=docker_container,
+                command="yarn install",
+                task_name="Running yarn install",
+            )
+            execute_with_stream(
+                logger=self._logger,
+                container=docker_container,
+                command="yarn cypress install",
+                task_name="Installing cypress",
+            )
+            execute_with_stream(
+                logger=self._logger,
+                container=docker_container,
+                command="yarn cypress verify",
+                task_name="Verifying cypress",
+            )
+            execute_with_stream(
+                logger=self._logger,
+                container=docker_container,
+                command="yarn tsc",
+                task_name="Compiling typescript",
+            )
+            execute_with_stream(
+                logger=self._logger,
+                container=docker_container,
+                command=f"rm -rf {reports_folder}",
+                task_name="Remove old report files",
+            )
+
+            run_command = (
+                f'bash -c "yarn cypress run --spec {specs_string} --reporter-options mochaFile='
+                f'"{reports_folder}/[hash].xml" || true"'
+            )
             record_key = cypress_config.record_key
             if record_key:
-                run_command = f'bash -c "yarn cypress run --spec {specs_string} --reporter-options ' \
-                              f'"mochaFile={reports_folder}/[hash].xml" --record --key ' \
-                              f'b6a2aab1-0b80-4ca0-a56c-1c8d98a8189c || true "'
-            result = execute_with_stream(logger=self._logger, container=docker_container, command=run_command,
-                                         task_name="Running cypress tests")
+                run_command = (
+                    f'bash -c "yarn cypress run --spec {specs_string} --reporter-options '
+                    f'"mochaFile={reports_folder}/[hash].xml" --record --key '
+                    f'b6a2aab1-0b80-4ca0-a56c-1c8d98a8189c || true "'
+                )
+            result = execute_with_stream(
+                logger=self._logger,
+                container=docker_container,
+                command=run_command,
+                task_name="Running cypress tests",
+            )
 
             for stdout in result:
                 if record_key and "Recorded Run" in stdout:
-                    artifact.spec[TEST_RESULTS_URL_KEY] = stdout.rstrip().rsplit('Recorded Run: ', 1)[1]
+                    artifact.spec[TEST_RESULTS_URL_KEY] = stdout.rstrip().rsplit(
+                        "Recorded Run: ", 1
+                    )[1]
                 if "error Command failed with exit code" in stdout:
                     raise DockerException(command_launched=[run_command], return_code=1)
         except DockerException:
-            return Output(success=False,
-                          message=f"Cypress tests for project {step_input.project.name} have one or more failures",
-                          produced_artifact=artifact)
+            return Output(
+                success=False,
+                message=f"Cypress tests for project {step_input.project.name} have one or more failures",
+                produced_artifact=artifact,
+            )
         finally:
             docker_container.stop()
             docker_container.remove()
 
-        return Output(success=True, message=f"Cypress tests for project {step_input.project.name} passed",
-                      produced_artifact=artifact)
+        return Output(
+            success=True,
+            message=f"Cypress tests for project {step_input.project.name} passed",
+            produced_artifact=artifact,
+        )
 
     @staticmethod
     def _target_to_test_target(target: Target) -> str:
         if target == Target.PULL_REQUEST_BASE:
-            return 'test'
+            return "test"
         if target == Target.ACCEPTANCE:
-            return 'acceptance'
+            return "acceptance"
 
-        return 'pr'
+        return "pr"
```

## mpyl/steps/test/after_test.py

```diff
@@ -8,25 +8,37 @@
 from ..models import Input, Output, ArtifactType
 from ...project import Stage
 from ...utilities.docker import stream_docker_logging
 
 
 class IntegrationTestAfter(Step):
     def __init__(self, logger: Logger) -> None:
-        super().__init__(logger=logger,
-                         meta=Meta(name='After Test', description='After test step', version='0.0.1', stage=Stage.TEST),
-                         produced_artifact=ArtifactType.NONE, required_artifact=ArtifactType.NONE)
+        super().__init__(
+            logger=logger,
+            meta=Meta(
+                name="After Test",
+                description="After test step",
+                version="0.0.1",
+                stage=Stage.TEST,
+            ),
+            produced_artifact=ArtifactType.NONE,
+            required_artifact=ArtifactType.NONE,
+        )
 
     def execute(self, step_input: Input) -> Output:
         compose_file = step_input.project.test_containers_path
         if not os.path.exists(compose_file):
-            return Output(success=True, message='No containers to stop')
+            return Output(success=True, message="No containers to stop")
 
         self._logger.debug(f"Stopping containers in {compose_file}")
         docker_client = DockerClient(compose_files=[compose_file])
         logs = docker_client.compose.logs(stream=True)
-        stream_docker_logging(logger=self._logger, generator=logs, task_name=f'Stop {compose_file}')
+        stream_docker_logging(
+            logger=self._logger, generator=logs, task_name=f"Stop {compose_file}"
+        )
 
         docker_client.compose.down(remove_orphans=True)
-        container_names = list(map(lambda l: l.name, docker_client.compose.ps(all=True)))
+        container_names = list(
+            map(lambda l: l.name, docker_client.compose.ps(all=True))
+        )
 
         return Output(success=True, message=f"Stopped {', '.join(container_names)}")
```

## mpyl/steps/test/before_test.py

```diff
@@ -10,49 +10,60 @@
 from ..models import Input, Output, ArtifactType
 from ...project import Stage
 from ...utilities.docker import stream_docker_logging, DockerComposeConfig
 
 
 class IntegrationTestBefore(Step):
     def __init__(self, logger: Logger) -> None:
-        super().__init__(logger=logger, meta=Meta(
-            name='Before Test',
-            description='Before test step',
-            version='0.0.1',
-            stage=Stage.TEST
-        ), produced_artifact=ArtifactType.NONE, required_artifact=ArtifactType.NONE)
+        super().__init__(
+            logger=logger,
+            meta=Meta(
+                name="Before Test",
+                description="Before test step",
+                version="0.0.1",
+                stage=Stage.TEST,
+            ),
+            produced_artifact=ArtifactType.NONE,
+            required_artifact=ArtifactType.NONE,
+        )
 
     def execute(self, step_input: Input) -> Output:
         compose_file = step_input.project.test_containers_path
         if not os.path.exists(compose_file):
-            return Output(success=True, message='No containers to start')
+            return Output(success=True, message="No containers to start")
 
         config = DockerComposeConfig.from_yaml(step_input.run_properties.config)
 
         self._logger.debug(f"Starting containers in {compose_file}")
         docker_client = DockerClient(compose_files=[compose_file])
         docker_client.compose.down(remove_orphans=True)
         docker_client.compose.build()
         docker_client.compose.up(detach=True, color=True, quiet=False)
 
         goal_reached = False
         logs = docker_client.compose.logs(stream=True)
-        stream_docker_logging(logger=self._logger, generator=logs, task_name=f'Start {compose_file}')
+        stream_docker_logging(
+            logger=self._logger, generator=logs, task_name=f"Start {compose_file}"
+        )
 
         poll = 0
         while not goal_reached:
             proj: ComposeProject = docker_client.compose.ls()[0]
-            goal_reached = (proj.created + proj.restarting + proj.exited + proj.paused + proj.dead) == 0
+            goal_reached = (
+                proj.created + proj.restarting + proj.exited + proj.paused + proj.dead
+            ) == 0
             if not goal_reached:
-                self._logger.debug(f'Project stats: {proj}')
+                self._logger.debug(f"Project stats: {proj}")
 
             poll += 1
             if poll >= config.failure_threshold:
-                return Output(success=False,
-                              message=f"Failed to start services in {compose_file} "
-                                      f"within {config.total_duration} seconds.")
+                return Output(
+                    success=False,
+                    message=f"Failed to start services in {compose_file} "
+                    f"within {config.total_duration} seconds.",
+                )
 
             time.sleep(config.period_seconds)
         running_containers: list[Container] = docker_client.compose.ps()
         container_names = list(map(lambda l: l.name, running_containers))
 
         return Output(success=True, message=f"Started {', '.join(container_names)}")
```

## mpyl/steps/test/dockertest.py

```diff
@@ -3,77 +3,116 @@
 
 ## 🧪 Testing inside a container
 
 When unit tests are run within a docker container the test results need to be written to a folder inside it.
 This means that the test step _within the docker container_ should not return a system error.
 Otherwise, building of the container would stop and the test results would not be committed to a layer.
 
-The test results need to be writted  written to a folder named `$WORKDIR/target/test-reports/` for
+The test results need to be written to a folder named `$WORKDIR/target/test-reports/` for
 `TestDocker.extract_test_results` to find and extract them.
 
 
 """
 from logging import Logger
 
 from python_on_whales import Container
 
 from .after_test import IntegrationTestAfter
 from .before_test import IntegrationTestBefore
 from .. import Step, Meta
 from ..models import Input, Output, ArtifactType, input_to_artifact, Artifact
 from ...project import Stage, Project
-from ...utilities.docker import DockerConfig, build, docker_image_tag, docker_file_path, docker_copy, \
-    remove_container, create_container
-from ...utilities.junit import to_test_suites, sum_suites, TEST_OUTPUT_PATH_KEY, TEST_RESULTS_URL_KEY
+from ...utilities.docker import (
+    DockerConfig,
+    build,
+    docker_image_tag,
+    docker_file_path,
+    docker_copy,
+    remove_container,
+    create_container,
+)
+from ...utilities.junit import (
+    to_test_suites,
+    sum_suites,
+    TEST_OUTPUT_PATH_KEY,
+    TEST_RESULTS_URL_KEY,
+)
 
 
 class TestDocker(Step):
     def __init__(self, logger: Logger) -> None:
-        meta = Meta(name='Docker Test', description='Test docker image', version='0.0.1', stage=Stage.TEST)
         super().__init__(
-            logger=logger, meta=meta,
+            logger=logger,
+            meta=Meta(
+                name="Docker Test",
+                description="Test docker image",
+                version="0.0.1",
+                stage=Stage.TEST,
+            ),
             produced_artifact=ArtifactType.JUNIT_TESTS,
             required_artifact=ArtifactType.NONE,
             before=IntegrationTestBefore(logger),
-            after=IntegrationTestAfter(logger)
+            after=IntegrationTestAfter(logger),
         )
 
     def execute(self, step_input: Input) -> Output:
         docker_config = DockerConfig.from_dict(step_input.run_properties.config)
         test_target = docker_config.test_target
         if not test_target:
-            raise ValueError('docker.testTarget must be specified')
+            raise ValueError("docker.testTarget must be specified")
 
-        tag = docker_image_tag(step_input) + '-test'
+        tag = docker_image_tag(step_input) + "-test"
         project = step_input.project
         dockerfile = docker_file_path(project=project, docker_config=docker_config)
-        success = build(logger=self._logger, root_path=docker_config.root_folder,
-                        file_path=dockerfile, image_tag=tag, target=test_target)
+        success = build(
+            logger=self._logger,
+            root_path=docker_config.root_folder,
+            file_path=dockerfile,
+            image_tag=tag,
+            target=test_target,
+        )
         container = create_container(self._logger, tag)
 
         if success:
-            artifact = self.extract_test_results(self._logger, project, container, step_input)
+            artifact = self.extract_test_results(
+                self._logger, project, container, step_input
+            )
 
             suite = to_test_suites(artifact)
             summary = sum_suites(suite)
 
-            output = Output(success=summary.is_success,
-                            message=f"Tests results produced for {project.name} ({summary})",
-                            produced_artifact=artifact)
+            output = Output(
+                success=summary.is_success,
+                message=f"Tests results produced for {project.name} ({summary})",
+                produced_artifact=artifact,
+            )
         else:
-            output = Output(success=False,
-                            message=f"Tests failed to run for {project.name}. No test results have been recorded.",
-                            produced_artifact=None)
+            output = Output(
+                success=False,
+                message=f"Tests failed to run for {project.name}. No test results have been recorded.",
+                produced_artifact=None,
+            )
 
         remove_container(self._logger, container)
 
         return output
 
     @staticmethod
-    def extract_test_results(logger: Logger, project: Project, container: Container, step_input: Input) -> Artifact:
-        path_in_container = f'{project.test_report_path}/.'
-        docker_copy(logger=logger, container_path=path_in_container, dst_path=project.test_report_path,
-                    container=container)
-
-        return input_to_artifact(artifact_type=ArtifactType.JUNIT_TESTS, step_input=step_input,
-                                 spec={TEST_OUTPUT_PATH_KEY: project.test_report_path,
-                                       TEST_RESULTS_URL_KEY: step_input.run_properties.details.tests_url})
+    def extract_test_results(
+        logger: Logger, project: Project, container: Container, step_input: Input
+    ) -> Artifact:
+        path_in_container = f"{project.test_report_path}/."
+        docker_copy(
+            logger=logger,
+            container_path=path_in_container,
+            dst_path=project.test_report_path,
+            container=container,
+        )
+
+        return input_to_artifact(
+            artifact_type=ArtifactType.JUNIT_TESTS,
+            step_input=step_input,
+            spec={
+                TEST_OUTPUT_PATH_KEY: project.test_report_path,
+                TEST_RESULTS_URL_KEY: step_input.run_properties.details.tests_url,
+            },
+        )
```

## mpyl/steps/test/echo.py

```diff
@@ -16,26 +16,39 @@
     </testcase>
   </testsuite>
 </testsuites>
 """.strip()
 
 
 class TestEcho(Step):
-
     def __init__(self, logger: Logger) -> None:
-        super().__init__(logger, Meta(
-            name='Echo Test',
-            description='Dummy test step to test the framework',
-            version='0.0.1',
-            stage=Stage.TEST
-        ), produced_artifact=ArtifactType.JUNIT_TESTS, required_artifact=ArtifactType.NONE)
+        super().__init__(
+            logger,
+            Meta(
+                name="Echo Test",
+                description="Dummy test step to test the framework",
+                version="0.0.1",
+                stage=Stage.TEST,
+            ),
+            produced_artifact=ArtifactType.JUNIT_TESTS,
+            required_artifact=ArtifactType.NONE,
+        )
 
     def execute(self, step_input: Input) -> Output:
         self._logger.info(f"Testing project {step_input.project.name}")
         path = Path(step_input.project.target_path, "test_results")
         path.mkdir(parents=True, exist_ok=True)
-        Path(path, "test.xml").write_text(SAMPLE_JUNIT_RESULT, encoding='utf-8')
+        Path(path, "test.xml").write_text(SAMPLE_JUNIT_RESULT, encoding="utf-8")
 
-        artifact = input_to_artifact(artifact_type=ArtifactType.JUNIT_TESTS, step_input=step_input,
-                                     spec={TEST_OUTPUT_PATH_KEY: str(path),
-                                           TEST_RESULTS_URL_KEY: step_input.run_properties.details.tests_url})
-        return Output(success=True, message=f"Tested {step_input.project.name}", produced_artifact=artifact)
+        artifact = input_to_artifact(
+            artifact_type=ArtifactType.JUNIT_TESTS,
+            step_input=step_input,
+            spec={
+                TEST_OUTPUT_PATH_KEY: str(path),
+                TEST_RESULTS_URL_KEY: step_input.run_properties.details.tests_url,
+            },
+        )
+        return Output(
+            success=True,
+            message=f"Tested {step_input.project.name}",
+            produced_artifact=artifact,
+        )
```

## mpyl/steps/test/sbt.py

```diff
@@ -4,99 +4,125 @@
 
 from .after_test import IntegrationTestAfter
 from .before_test import IntegrationTestBefore
 from .. import Input, Output, Step
 from ..models import Artifact, input_to_artifact
 from ...project import Stage, Project
 from ...steps import Meta, ArtifactType
-from ...utilities.junit import TEST_OUTPUT_PATH_KEY, to_test_suites, sum_suites, TEST_RESULTS_URL_KEY
+from ...utilities.junit import (
+    TEST_OUTPUT_PATH_KEY,
+    to_test_suites,
+    sum_suites,
+    TEST_RESULTS_URL_KEY,
+)
 from ...utilities.sbt import SbtConfig
 from ...utilities.subprocess import custom_check_output
 
 
 class TestSbt(Step):
     def __init__(self, logger: Logger) -> None:
-        meta = Meta(name='Sbt Test', description='Run sbt tests', version='0.0.1', stage=Stage.TEST)
         super().__init__(
             logger=logger,
-            meta=meta,
+            meta=Meta(
+                name="Sbt Test",
+                description="Run sbt tests",
+                version="0.0.1",
+                stage=Stage.TEST,
+            ),
             produced_artifact=ArtifactType.JUNIT_TESTS,
             required_artifact=ArtifactType.NONE,
             before=IntegrationTestBefore(logger),
-            after=IntegrationTestAfter(logger)
+            after=IntegrationTestAfter(logger),
         )
 
     def _test_with_coverage(self, step_input: Input, sbt_config: SbtConfig) -> Output:
-        command_compile = self._construct_sbt_command(step_input, sbt_config,
-                                                      self._construct_sbt_command_compile_with_coverage)
+        command_compile = self._construct_sbt_command(
+            step_input, sbt_config, self._construct_sbt_command_compile_with_coverage
+        )
         compile_outcome = custom_check_output(self._logger, command_compile)
         project_name = step_input.project.name
         if not compile_outcome.success:
-            return Output(success=False, message=f"Tests failed to compile for {project_name}",
-                          produced_artifact=None)
+            return Output(
+                success=False,
+                message=f"Tests failed to compile for {project_name}",
+                produced_artifact=None,
+            )
 
-        command_test = self._construct_sbt_command(step_input, sbt_config,
-                                                   self._construct_sbt_command_test_with_coverage)
+        command_test = self._construct_sbt_command(
+            step_input, sbt_config, self._construct_sbt_command_test_with_coverage
+        )
         test_outcome = custom_check_output(self._logger, command_test)
         artifact = self._extract_test_report(step_input.project, step_input)
         if not test_outcome.success:
-            return Output(success=False,
-                          message=f"Tests failed to run for {project_name}. No test results have been recorded.",
-                          produced_artifact=artifact)
+            return Output(
+                success=False,
+                message=f"Tests failed to run for {project_name}. No test results have been recorded.",
+                produced_artifact=artifact,
+            )
         return Output(success=True, message="Success", produced_artifact=artifact)
 
-    def _test_without_coverage(self, step_input: Input, sbt_config: SbtConfig) -> Output:
-        command_test_without_coverage = self._construct_sbt_command(step_input, sbt_config,
-                                                                    self._construct_sbt_command_test_without_coverage)
+    def _test_without_coverage(
+        self, step_input: Input, sbt_config: SbtConfig
+    ) -> Output:
+        command_test_without_coverage = self._construct_sbt_command(
+            step_input, sbt_config, self._construct_sbt_command_test_without_coverage
+        )
         run_outcome = custom_check_output(self._logger, command_test_without_coverage)
         artifact = self._extract_test_report(step_input.project, step_input)
         if not run_outcome.success:
-            return Output(success=False, message=f"Tests without coverage failed to run for {step_input.project.name}",
-                          produced_artifact=artifact)
+            return Output(
+                success=False,
+                message=f"Tests without coverage failed to run for {step_input.project.name}",
+                produced_artifact=artifact,
+            )
         return Output(success=True, message="Success", produced_artifact=artifact)
 
     def execute(self, step_input: Input) -> Output:
         project = step_input.project
         sbt_config = SbtConfig.from_config(config=step_input.run_properties.config)
-        self._logger.debug(f'Config {sbt_config}')
+        self._logger.debug(f"Config {sbt_config}")
 
-        test_result = self._test_with_coverage(step_input, sbt_config) if sbt_config.test_with_coverage \
+        test_result = (
+            self._test_with_coverage(step_input, sbt_config)
+            if sbt_config.test_with_coverage
             else self._test_without_coverage(step_input, sbt_config)
+        )
 
         if test_result.produced_artifact:
             suite = to_test_suites(test_result.produced_artifact)
             summary = sum_suites(suite)
-            return Output(success=summary.is_success,
-                          message=f"Tests results produced for {project.name} ({summary})",
-                          produced_artifact=test_result.produced_artifact)
+            return Output(
+                success=summary.is_success,
+                message=f"Tests results produced for {project.name} ({summary})",
+                produced_artifact=test_result.produced_artifact,
+            )
 
         return test_result
 
     @staticmethod
     def _construct_sbt_command_compile_with_coverage(step_input: Input) -> list[str]:
-        return [
-            f'project {step_input.project.name}',
-            'coverageOn',
-            'test:compile'
-        ]
+        return [f"project {step_input.project.name}", "coverageOn", "test:compile"]
 
     @staticmethod
     def _construct_sbt_command_test_with_coverage(step_input: Input):
-        return [
-            f'project {step_input.project.name}',
-            'test',
-            'coverageOff'
-        ]
+        return [f"project {step_input.project.name}", "test", "coverageOff"]
 
     @staticmethod
     def _construct_sbt_command_test_without_coverage(step_input: Input):
-        return [f'{step_input.project.name}/test']
+        return [f"{step_input.project.name}/test"]
 
     @staticmethod
-    def _construct_sbt_command(step_input: Input, config: SbtConfig, commands_fn: Callable[[Input], list[str]]):
+    def _construct_sbt_command(
+        step_input: Input, config: SbtConfig, commands_fn: Callable[[Input], list[str]]
+    ):
         return config.to_command(config.test_with_client, commands_fn(step_input))
 
     @staticmethod
     def _extract_test_report(project: Project, step_input: Input) -> Artifact:
-        return input_to_artifact(artifact_type=ArtifactType.JUNIT_TESTS, step_input=step_input,
-                                 spec={TEST_OUTPUT_PATH_KEY: f'{project.test_report_path}',
-                                       TEST_RESULTS_URL_KEY: step_input.run_properties.details.tests_url})
+        return input_to_artifact(
+            artifact_type=ArtifactType.JUNIT_TESTS,
+            step_input=step_input,
+            spec={
+                TEST_OUTPUT_PATH_KEY: f"{project.test_report_path}",
+                TEST_RESULTS_URL_KEY: step_input.run_properties.details.tests_url,
+            },
+        )
```

## mpyl/utilities/cypress/__init__.py

```diff
@@ -7,14 +7,18 @@
 class CypressConfig:
     cypress_source_code_path: str
     kubectl_config_path: str
     record_key: Optional[str]
 
     @staticmethod
     def from_config(config: dict):
-        cypress_config = config.get('cypress')
+        cypress_config = config.get("cypress")
         if not cypress_config:
-            raise KeyError('Cypress section needs to be defined in mpyl_config.yml')
+            raise KeyError("Cypress section needs to be defined in mpyl_config.yml")
 
-        return CypressConfig(cypress_source_code_path=cypress_config.get('cypressSourceCodePath'),
-                             record_key=cypress_config.get('recordKey'),
-                             kubectl_config_path=cypress_config.get('kubectlConfigPath', '~/.kube/config'))
+        return CypressConfig(
+            cypress_source_code_path=cypress_config.get("cypressSourceCodePath"),
+            record_key=cypress_config.get("recordKey"),
+            kubectl_config_path=cypress_config.get(
+                "kubectlConfigPath", "~/.kube/config"
+            ),
+        )
```

## mpyl/utilities/docker/__init__.py

```diff
@@ -25,19 +25,21 @@
 
     @property
     def total_duration(self):
         return self.period_seconds * self.failure_threshold
 
     @staticmethod
     def from_yaml(config: dict):
-        compose_config = config.get('docker', {}).get('compose')
+        compose_config = config.get("docker", {}).get("compose")
         if not compose_config:
-            raise KeyError('docker.compose needs to be defined')
-        return DockerComposeConfig(period_seconds=int(compose_config['periodSeconds']),
-                                   failure_threshold=int(compose_config['failureThreshold']))
+            raise KeyError("docker.compose needs to be defined")
+        return DockerComposeConfig(
+            period_seconds=int(compose_config["periodSeconds"]),
+            failure_threshold=int(compose_config["failureThreshold"]),
+        )
 
 
 @dataclass(frozen=True)
 class DockerConfig:
     host_name: str
     user_name: str
     password: str
@@ -45,120 +47,151 @@
     build_target: Optional[str]
     test_target: Optional[str]
     docker_file_name: str
 
     @staticmethod
     def from_dict(config: Dict):
         try:
-            registry: Dict = config['docker']['registry']
-            build_config: Dict = config['docker']['build']
+            registry: Dict = config["docker"]["registry"]
+            build_config: Dict = config["docker"]["build"]
             return DockerConfig(
-                host_name=registry['hostName'],
-                user_name=registry['userName'],
-                password=registry['password'],
-                root_folder=build_config['rootFolder'],
-                build_target=build_config.get('buildTarget', None),
-                test_target=build_config.get('testTarget', None),
-                docker_file_name=build_config['dockerFileName']
+                host_name=registry["hostName"],
+                user_name=registry["userName"],
+                password=registry["password"],
+                root_folder=build_config["rootFolder"],
+                build_target=build_config.get("buildTarget", None),
+                test_target=build_config.get("testTarget", None),
+                docker_file_name=build_config["dockerFileName"],
             )
         except KeyError as exc:
-            raise KeyError(f'Docker config could not be loaded from {config}') from exc
+            raise KeyError(f"Docker config could not be loaded from {config}") from exc
 
 
-def execute_with_stream(logger: Logger, container: Container, command: str, task_name: str):
-    result = cast(Iterator[tuple[str, bytes]], container.execute(command=shlex.split(command), stream=True))
+def execute_with_stream(
+    logger: Logger, container: Container, command: str, task_name: str
+):
+    result = cast(
+        Iterator[tuple[str, bytes]],
+        container.execute(command=shlex.split(command), stream=True),
+    )
     result_list = stream_docker_logging(logger, result, task_name)
 
     return result_list
 
 
-def stream_docker_logging(logger: Logger, generator: Union[Iterator[str], Iterator[tuple[str, bytes]]], task_name: str,
-                          level=logging.INFO) -> list[str]:
+def stream_docker_logging(
+    logger: Logger,
+    generator: Union[Iterator[str], Iterator[tuple[str, bytes]]],
+    task_name: str,
+    level=logging.INFO,
+) -> list[str]:
     copied_logs = []
 
     while True:
         try:
             next_item = next(generator)
-            log_line = next_item[1].decode(errors="replace") if isinstance(next_item, tuple) else next_item
+            log_line = (
+                next_item[1].decode(errors="replace")
+                if isinstance(next_item, tuple)
+                else next_item
+            )
             copied_logs.append(log_line)
             logger.log(level, try_parse_ansi(log_line))
         except StopIteration:
-            logger.info(f'{task_name} complete.')
+            logger.info(f"{task_name} complete.")
             return copied_logs
 
 
 def docker_image_tag(step_input: Input):
     git = step_input.run_properties.versioning
     tag = git.tag if git.tag else f"pr-{git.pr_number}"
-    return f"{step_input.project.name.lower()}:{tag}".replace('/', '_')
+    return f"{step_input.project.name.lower()}:{tag}".replace("/", "_")
 
 
 def docker_file_path(project: Project, docker_config: DockerConfig):
-    return f'{project.deployment_path}/{docker_config.docker_file_name}'
+    return f"{project.deployment_path}/{docker_config.docker_file_name}"
 
 
-def docker_copy(logger: Logger, container_path: str, dst_path: str, container: Container):
+def docker_copy(
+    logger: Logger, container_path: str, dst_path: str, container: Container
+):
     """
     Copies the contents of the specified path within the container to a locally created destination
 
     :param logger: the logger
     :param container_path: the path of the directory in the container to copy
     :param dst_path: the path to copy the container content to
     :param container: the container to copy from
     """
     shutil.rmtree(dst_path, ignore_errors=True)
     Path(dst_path).mkdir(parents=True, exist_ok=True)
 
     if not docker.container.exists(container.id):
-        raise ValueError(f'Container {container.id} does not exist')
+        raise ValueError(f"Container {container.id} does not exist")
 
     logger.info(
         f"Copying contents from container {container.id} at "
         f"path {container_path} to host at {dst_path}"
     )
     try:
-        docker.copy(f'{container.id}:{container_path}', dst_path)
+        docker.copy(f"{container.id}:{container_path}", dst_path)
     except NoSuchContainer as exc:
-        logger.warning(f'Could not find data in container {container.name} at expected location {container_path}')
+        logger.warning(
+            f"Could not find data in container {container.name} at expected location {container_path}"
+        )
         raise exc
 
 
-def build(logger: Logger, root_path: str, file_path: str, image_tag: str, target: str) -> bool:
+def build(
+    logger: Logger, root_path: str, file_path: str, image_tag: str, target: str
+) -> bool:
     """
     :param logger: the logger
     :param root_path: the root path to which `docker_file_path` is relative
     :param file_path: path to the docker file to be built
     :param image_tag: the tag of the image
     :param target: the 'target' within the multi-stage docker image
     :return: True if success, False if failure
     """
     logger.info(f"Building docker image with {file_path} and target {target}")
 
     try:
-        logs = docker.buildx.build(context_path=root_path, file=file_path, tags=[image_tag], target=target,
-                                   stream_logs=True)
+        logs = docker.buildx.build(
+            context_path=root_path,
+            file=file_path,
+            tags=[image_tag],
+            target=target,
+            stream_logs=True,
+        )
         if logs is not None and not isinstance(logs, Image):
-            stream_docker_logging(logger=logger, generator=logs, task_name=f'Build {file_path}:{target}')
+            stream_docker_logging(
+                logger=logger, generator=logs, task_name=f"Build {file_path}:{target}"
+            )
         logger.debug(logs)
         return True
 
     except DockerException as exc:
         command = " ".join(exc.docker_command)
-        logger.warning(f"Docker build failed with command {command} and exit code {exc.return_code}")
+        logger.warning(
+            f"Docker build failed with command {command} and exit code {exc.return_code}"
+        )
         return False
     except Exception as exc:  # pylint: disable=broad-exception-caught
         print(f"Docker build failed with {exc.__class__.__name__}")
         print_exc()
         return False
 
 
 def login(logger: Logger, docker_config: DockerConfig) -> None:
     logger.info(f"Logging in with user '{docker_config.user_name}'")
-    docker.login(server=f'https://{docker_config.host_name}', username=docker_config.user_name,
-                 password=docker_config.password)
+    docker.login(
+        server=f"https://{docker_config.host_name}",
+        username=docker_config.user_name,
+        password=docker_config.password,
+    )
     logger.debug(f"Logged in as '{docker_config.user_name}'")
 
 
 def create_container(logger: Logger, image_name: str) -> Container:
     logger.info(f"Creating container from image {image_name}")
     container = docker.create(image_name)
     logger.info(f"Created container {container.id}")
```

## mpyl/utilities/github/__init__.py

```diff
@@ -9,48 +9,52 @@
 @dataclass
 class GithubAppConfig:
     private_app_key_path: Optional[str]
     private_key_base_64_encoded: Optional[str]
     app_key: str
 
     def __init__(self, config: Dict):
-        self.private_app_key_path = config.get('privateKeyPath')
-        self.private_key_base_64_encoded = config.get('privateKeyBase64Encoded')
+        self.private_app_key_path = config.get("privateKeyPath")
+        self.private_key_base_64_encoded = config.get("privateKeyBase64Encoded")
         if not self.private_key_base_64_encoded and not self.private_app_key_path:
-            raise KeyError("When github.app is configured, either 'privateKeyPath' "
-                           "or 'privateKeyBase64Encoded' need to be defined")
+            raise KeyError(
+                "When github.app is configured, either 'privateKeyPath' "
+                "or 'privateKeyBase64Encoded' need to be defined"
+            )
 
-        self.app_key = config['appId']
+        self.app_key = config["appId"]
 
 
 @dataclass(frozen=True)
 class GithubConfig:
     repository: str
     owner: str
     repo_name: str
     token: str
     app_config: dict
 
     @staticmethod
     def from_config(config: Dict):
-        github = config['cvs']['github']
-        repo_parts = github['repository'].split('/')
+        github = config["cvs"]["github"]
+        repo_parts = github["repository"].split("/")
         return GithubConfig(
-            repository=(github['repository']),
+            repository=(github["repository"]),
             owner=repo_parts[0],
             repo_name=repo_parts[1],
-            token=github['token'],
-            app_config=github.get('app', {})
+            token=github["token"],
+            app_config=github.get("app", {}),
         )
 
     @property
     def get_app_config(self) -> GithubAppConfig:
         return GithubAppConfig(self.app_config)
 
 
 def get_pr_for_branch(repo: Repository, branch: str) -> PullRequest:
-    pulls = repo.get_pulls(head=f'{repo.full_name}:{branch}').get_page(0)
+    pulls = repo.get_pulls(head=f"{repo.full_name}:{branch}").get_page(0)
 
     if len(pulls) == 0:
-        raise ValueError(f'No PR related to {branch} was found. Did you create it yet? `gh pr create --draft`')
+        raise ValueError(
+            f"No PR related to {branch} was found. Did you create it yet? `gh pr create --draft`"
+        )
 
     return pulls.pop()
```

## mpyl/utilities/jenkins/__init__.py

```diff
@@ -8,19 +8,22 @@
 class JenkinsConfig:
     url: str
     pipelines: dict[str, str]
     default: str
 
     @staticmethod
     def from_config(values: dict):
-        jenkins_config = values.get('jenkins')
+        jenkins_config = values.get("jenkins")
         if not jenkins_config:
-            raise KeyError('jenkins should be defined in config')
-        return JenkinsConfig(url=jenkins_config['url'], pipelines=jenkins_config['pipelines'],
-                             default=jenkins_config['defaultPipeline'])
+            raise KeyError("jenkins should be defined in config")
+        return JenkinsConfig(
+            url=jenkins_config["url"],
+            pipelines=jenkins_config["pipelines"],
+            default=jenkins_config["defaultPipeline"],
+        )
 
     @property
     def default_pipeline(self) -> str:
         return self.pipelines[self.default]
 
 
 @dataclass(frozen=True)
@@ -29,23 +32,23 @@
     tag: str
     url: str
     pipeline: str
     body: str
     jenkins_config: JenkinsConfig
 
     def _to_path(self):
-        return f'PR-{self.tag}' if self.target == Target.PULL_REQUEST else self.tag
+        return f"PR-{self.tag}" if self.target == Target.PULL_REQUEST else self.tag
 
     def pipeline_location(self) -> str:
         return f'{self.jenkins_config.url}job/{self.jenkins_config.pipelines[self.pipeline].replace(" ", "%20")}/'
 
     def job_location(self) -> str:
-        return f'{self.pipeline_location}job/{self._to_path()}/'
+        return f"{self.pipeline_location}job/{self._to_path()}/"
 
     def job_name(self) -> str:
-        return f'{self.jenkins_config.pipelines[self.pipeline]}/{self._to_path()}'
+        return f"{self.jenkins_config.pipelines[self.pipeline]}/{self._to_path()}"
 
     def build_location(self) -> str:
-        return f'{self.pipeline_location()}view/change-requests/job/{self._to_path()}/lastBuild/'
+        return f"{self.pipeline_location()}view/change-requests/job/{self._to_path()}/lastBuild/"
 
     def human_readable(self) -> str:
-        return f'[link={self.url}]#{self.tag}[/link]'
+        return f"[link={self.url}]#{self.tag}[/link]"
```

## mpyl/utilities/jenkins/runner.py

```diff
@@ -10,16 +10,22 @@
 from jenkinsapi.constants import STATUS_SUCCESS, STATUS_ABORTED
 from jenkinsapi.custom_exceptions import JenkinsAPIException
 from jenkinsapi.jenkins import Jenkins
 from jenkinsapi.job import Job
 from rich.console import Group
 from rich.errors import MarkupError
 from rich.live import Live
-from rich.progress import Progress, TimeElapsedColumn, TextColumn, BarColumn, TaskProgressColumn, \
-    TimeRemainingColumn
+from rich.progress import (
+    Progress,
+    TimeElapsedColumn,
+    TextColumn,
+    BarColumn,
+    TaskProgressColumn,
+    TimeRemainingColumn,
+)
 from rich.prompt import Confirm
 from rich.status import Status
 from rich.table import Column
 
 from . import Pipeline
 from ...cli.commands.build import play_sound, Sound
 from ..logging import try_parse_ansi
@@ -30,27 +36,23 @@
     Return generator which streams parts of text console.
     Workaround for https://github.com/pycontribs/jenkinsapi/pull/843
     """
     url = f"{self.baseurl}/logText/progressiveText"
     size = 0
     more_data = True
     while more_data:
-        resp = self.job.jenkins.requester.get_url(
-            url, params={"start": size}
-        )
+        resp = self.job.jenkins.requester.get_url(url, params={"start": size})
         content = resp.content
         if content:
             if isinstance(content, str):
                 yield content
             elif isinstance(content, bytes):
                 yield content.decode(resp.encoding)
             else:
-                raise JenkinsAPIException(
-                    "Unknown content type for console"
-                )
+                raise JenkinsAPIException("Unknown content type for console")
         size = resp.headers["X-Text-Size"]
         more_data = resp.headers.get("X-More-Data")
         time.sleep(interval)
 
 
 Build.stream_utf_8_logs = stream_utf_8_logs
 
@@ -63,77 +65,101 @@
     follow: bool
     verbose: bool
 
     def get_job(self, name: str) -> Job:
         try:
             return self.jenkins.get_job(name)
         except KeyError:
-            self.status.update(f'Job for {self.pipeline.human_readable()} not found. This could take a while. '
-                               'Triggering build scan...')
-            requests.post(f'{self.pipeline.pipeline_location()}/build?delay=0#',
-                          auth=(self.jenkins.username, self.jenkins.password), timeout=10)
+            self.status.update(
+                f"Job for {self.pipeline.human_readable()} not found. This could take a while. "
+                "Triggering build scan..."
+            )
+            requests.post(
+                f"{self.pipeline.pipeline_location()}/build?delay=0#",
+                auth=(self.jenkins.username, self.jenkins.password),
+                timeout=10,
+            )
 
             while True:
                 try:
                     self.jenkins.jobs_container = None  # force update of job info
                     return self.jenkins.get_job(name)
                 except KeyError:
-                    self.status.update(f'Waiting for {self.pipeline.human_readable()} to appear...')
+                    self.status.update(
+                        f"Waiting for {self.pipeline.human_readable()} to appear..."
+                    )
                     time.sleep(1)
 
     def await_parameter_build(self, build_job: Job):
         queue = build_job.invoke()
         param_build = queue.block_until_building(delay=3)
-        self.status.console.log(f'Build in Jenkins {queue.get_build().get_build_url()}')
-        self.status.update('Running initial build to set parameters. This may take a minute..')
+        self.status.console.log(f"Build in Jenkins {queue.get_build().get_build_url()}")
+        self.status.update(
+            "Running initial build to set parameters. This may take a minute.."
+        )
         while build_job.is_running():
             time.sleep(1)
-        self.status.console.log('Build parameters retrieved')
+        self.status.console.log("Build parameters retrieved")
 
         if not param_build.is_good:
-            self.status.console.log(f"⚠️ Failed to get parameters: {param_build.get_build_url()}")
+            self.status.console.log(
+                f"⚠️ Failed to get parameters: {param_build.get_build_url()}"
+            )
             sys.exit()
 
     @staticmethod
     def to_icon(build_result: Build) -> str:
         status = build_result.get_status()
         if status == STATUS_SUCCESS:
-            return '✅ '
+            return "✅ "
         if status == STATUS_ABORTED:
-            return '🚫 '
-        return '❌ '
-
-    def follow_logs(self, job: Job, build_number: int, duration_estimation: int, verbose: bool = False):
+            return "🚫 "
+        return "❌ "
 
+    def follow_logs(
+        self,
+        job: Job,
+        build_number: int,
+        duration_estimation: int,
+        verbose: bool = False,
+    ):
         build_to_follow: Build = job.get_build(build_number)
-        self.status.console.log(f'{build_to_follow} {self.pipeline.build_location()}')
+        self.status.console.log(f"{build_to_follow} {self.pipeline.build_location()}")
 
         self._stream_logs(build_to_follow, duration_estimation, verbose)
 
         build_to_follow.block_until_complete()
         finished_build = job.get_last_build()
         self.status.console.log(
-            f'[link={finished_build.get_build_url()}][i]Build[/link] for {self.pipeline.human_readable()} '
-            f'ended with outcome {self.to_icon(finished_build)}', markup=True)
+            f"[link={finished_build.get_build_url()}][i]Build[/link] for {self.pipeline.human_readable()} "
+            f"ended with outcome {self.to_icon(finished_build)}",
+            markup=True,
+        )
         self.status.console.log()
 
         play_sound(Sound.SUCCESS if finished_build.is_good() else Sound.FAILURE)
         sys.exit()
 
     def _stream_logs(self, build_to_follow, duration_estimation, verbose):
         progress = Progress(
             TimeElapsedColumn(),
             BarColumn(bar_width=None),
             TaskProgressColumn(),
             TimeRemainingColumn(),
         )
-        log_line = Progress(TextColumn('{task.description}', table_column=Column(overflow='crop', no_wrap=True)))
+        log_line = Progress(
+            TextColumn(
+                "{task.description}", table_column=Column(overflow="crop", no_wrap=True)
+            )
+        )
         live = Live(Group(log_line, progress) if not verbose else progress)
         with live:
-            build_task_id = progress.add_task("", total=duration_estimation, visible=duration_estimation > 0)
+            build_task_id = progress.add_task(
+                "", total=duration_estimation, visible=duration_estimation > 0
+            )
             start_time = time.time()
             label_task_id = log_line.add_task("status")
 
             def cancel_handler(_sig, _frame):
                 live.stop()
                 stop_build = Confirm.ask("Stop build?")
                 if stop_build:
@@ -141,15 +167,15 @@
                     live.start()
                 else:
                     sys.exit()
 
             signal.signal(signal.SIGINT, cancel_handler)
             for line in build_to_follow.stream_utf_8_logs():
                 elapsed_time = time.time() - start_time
-                lines = line.rstrip().split('\n')
+                lines = line.rstrip().split("\n")
 
                 try:
                     text = "".join(lines)
                     if verbose:
                         progress.log(try_parse_ansi(text))
                     else:
                         log_line.update(label_task_id, description=text)
@@ -163,36 +189,41 @@
         if not list(job.get_build_ids()):
             self.await_parameter_build(job)
 
         build = job.get_last_build()
         last_build_number = build.get_number()
         if job.is_running():
             self.status.console.log(
-                f"Build {last_build_number} 🏗️ for {self.pipeline.human_readable()} is still running.")
+                f"Build {last_build_number} 🏗️ for {self.pipeline.human_readable()} is still running."
+            )
             self.status.console.log(f"{build.get_build_url()}")
             self.follow_logs(job, last_build_number, 0)
 
         self.status.update("Starting build...")
 
         last_build = 0
 
         self.jenkins.build_job(self.pipeline.job_name(), params=pipeline_parameters)
 
         if last_build_number > 1:
             last_build = build.get_duration().seconds
-            self.status.console.log(f'Last build {last_build_number} {self.to_icon(build)} took'
-                                    f' {str(datetime.timedelta(seconds=last_build))}')
+            self.status.console.log(
+                f"Last build {last_build_number} {self.to_icon(build)} took"
+                f" {str(datetime.timedelta(seconds=last_build))}"
+            )
 
         new_build_number = last_build_number + 1
 
         self.status.update("Waiting for build to start....")
         while job.get_last_buildnumber() != new_build_number:
             time.sleep(1)
         self.status.stop()
 
         if self.follow:
             self.follow_logs(job, new_build_number, last_build, self.verbose)
         else:
-            self.status.console.log(f'Build {new_build_number} started '
-                                    f'for {self.pipeline.human_readable()} at '
-                                    f'{job.get_build(new_build_number).get_build_url()}')
+            self.status.console.log(
+                f"Build {new_build_number} started "
+                f"for {self.pipeline.human_readable()} at "
+                f"{job.get_build(new_build_number).get_build_url()}"
+            )
             self.status.stop()
```

## mpyl/utilities/junit/__init__.py

```diff
@@ -3,17 +3,17 @@
 from dataclasses import dataclass
 from pathlib import Path
 
 from junitparser import JUnitXml, TestSuite
 
 from ...steps.models import Artifact, ArtifactType
 
-TEST_OUTPUT_PATH_KEY = 'test_output_path'
-TEST_RESULTS_URL_KEY = 'test_results_url'
-TEST_RESULTS_URL_NAME_KEY = 'test_results_url_name'
+TEST_OUTPUT_PATH_KEY = "test_output_path"
+TEST_RESULTS_URL_KEY = "test_results_url"
+TEST_RESULTS_URL_NAME_KEY = "test_results_url_name"
 
 
 @dataclass(frozen=True)
 class TestRunSummary:
     tests: int
     failures: int
     errors: int
@@ -22,21 +22,29 @@
     @property
     def is_success(self):
         return self.errors == 0 and self.failures == 0
 
 
 def to_test_suites(artifact: Artifact) -> list[TestSuite]:
     if artifact.artifact_type != ArtifactType.JUNIT_TESTS:
-        raise ValueError(f'Artifact {artifact} should be of type {ArtifactType.JUNIT_TESTS}')
+        raise ValueError(
+            f"Artifact {artifact} should be of type {ArtifactType.JUNIT_TESTS}"
+        )
     junit_result_path = artifact.spec[TEST_OUTPUT_PATH_KEY]
 
     xml = JUnitXml()
-    for file_name in [fn for fn in os.listdir(junit_result_path) if fn.endswith('.xml')]:
+    for file_name in [
+        fn for fn in os.listdir(junit_result_path) if fn.endswith(".xml")
+    ]:
         xml += JUnitXml.fromfile(Path(junit_result_path, file_name).as_posix())
 
     suites = [TestSuite.fromelem(s) for s in xml]
     return sorted(suites, key=lambda s: s.time)
 
 
 def sum_suites(suites: list[TestSuite]) -> TestRunSummary:
-    return TestRunSummary(tests=sum(s.tests for s in suites), failures=sum(s.failures for s in suites),
-                          errors=sum(s.errors for s in suites), skipped=sum(s.skipped for s in suites))
+    return TestRunSummary(
+        tests=sum(s.tests for s in suites),
+        failures=sum(s.failures for s in suites),
+        errors=sum(s.errors for s in suites),
+        skipped=sum(s.skipped for s in suites),
+    )
```

## mpyl/utilities/pyaml_env/__init__.py

```diff
@@ -6,19 +6,22 @@
 from pyaml_env import parse_config as original_parse_config
 from dotenv import load_dotenv
 
 
 def parse_config(path: Path) -> dict[str, str]:
     load_dotenv(Path(".env"))
 
-    def default_to_none(obj, default_value='N/A'):
+    def default_to_none(obj, default_value="N/A"):
         if isinstance(obj, (list, tuple, set)):
             return type(obj)(default_to_none(x) for x in obj if x is not default_value)
         if isinstance(obj, dict):
-            return type(obj)((default_to_none(k), default_to_none(v))
-                             for k, v in obj.items() if k is not default_value and v is not default_value)
+            return type(obj)(
+                (default_to_none(k), default_to_none(v))
+                for k, v in obj.items()
+                if k is not default_value and v is not default_value
+            )
         if obj == default_value:
             return None
         return obj
 
     parsed = original_parse_config(str(path))
     return default_to_none(parsed)
```

## mpyl/utilities/repo/__init__.py

```diff
@@ -34,46 +34,53 @@
     @property
     def to_url_with_credentials(self):
         parsed = urlparse(self.url)
         return f"{parsed.scheme}://{self.user_name}:{self.password}@{parsed.netloc}{parsed.path}"
 
     @staticmethod
     def from_config(config: Dict):
-        return RepoCredentials(url=config['url'], user_name=config['userName'], password=config['password'])
+        return RepoCredentials(
+            url=config["url"], user_name=config["userName"], password=config["password"]
+        )
 
 
 @dataclass(frozen=True)
 class RepoConfig:
     main_branch: str
     ignore_patterns: list[str]
     repo_credentials: Optional[RepoCredentials]
 
     @staticmethod
     def from_config(config: Dict):
-        git_config = config['cvs']['git']
-        maybe_remote_config = git_config.get('remote', None)
+        git_config = config["cvs"]["git"]
+        maybe_remote_config = git_config.get("remote", None)
         return RepoConfig(
-            main_branch=git_config['mainBranch'],
-            ignore_patterns=git_config.get('ignorePatterns', []),
-            repo_credentials=RepoCredentials.from_config(maybe_remote_config) if maybe_remote_config else None
+            main_branch=git_config["mainBranch"],
+            ignore_patterns=git_config.get("ignorePatterns", []),
+            repo_credentials=RepoCredentials.from_config(maybe_remote_config)
+            if maybe_remote_config
+            else None,
         )
 
 
 class Repository:
-
     def __init__(self, config: RepoConfig):
         self._config = config
-        self._root_dir = Git().rev_parse('--show-toplevel')
-        self._repo = Repo(self._root_dir)  # pylint: disable=attribute-defined-outside-init
+        self._root_dir = Git().rev_parse("--show-toplevel")
+        self._repo = Repo(
+            self._root_dir
+        )  # pylint: disable=attribute-defined-outside-init
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self._repo.close()
+        if exc_val:
+            raise exc_val
         return self
 
     @property
     def get_sha(self):
         return self._repo.head.commit.hexsha
 
     @property
@@ -105,75 +112,112 @@
         return self._config.main_branch
 
     def __get_filter_patterns(self):
         return ["--"] + [f":!{pattern}" for pattern in self._config.ignore_patterns]
 
     @property
     def latest_tag(self) -> str:
-        return str(sorted(self._repo.tags, key=lambda t: t.commit.committed_datetime)[-1])
+        return str(
+            sorted(self._repo.tags, key=lambda t: t.commit.committed_datetime)[-1]
+        )
 
-    def __to_revision(self, count: int, revision: Commit, files_touched_in_branch: set[str]) -> Revision:
+    def __to_revision(
+        self, count: int, revision: Commit, files_touched_in_branch: set[str]
+    ) -> Revision:
         files_in_revision = set(
-            self._repo.git.diff_tree(self.__get_filter_patterns(), no_commit_id=True, name_only=True,
-                                     r=str(revision)).splitlines())
+            self._repo.git.diff_tree(
+                self.__get_filter_patterns(),
+                no_commit_id=True,
+                name_only=True,
+                r=str(revision),
+            ).splitlines()
+        )
         intersection = files_in_revision.intersection(files_touched_in_branch)
         return Revision(count, str(revision), intersection)
 
     def changes_in_branch(self) -> list[Revision]:
-        revisions = list(reversed(list(self._repo.iter_commits(f"{self._config.main_branch}..HEAD"))))
+        revisions = list(
+            reversed(list(self._repo.iter_commits(f"{self._config.main_branch}..HEAD")))
+        )
+        if not revisions:
+            return []
+
         files_touched_in_branch = set(
-            self._repo.git.diff(f'{revisions[0].hexsha}..{revisions[-1].hexsha}', name_only=True).splitlines())
-        return [self.__to_revision(count, rev, files_touched_in_branch) for count, rev in enumerate(revisions)]
+            self._repo.git.diff(
+                f"{revisions[0].hexsha}..{revisions[-1].hexsha}", name_only=True
+            ).splitlines()
+        )
+        return [
+            self.__to_revision(count, rev, files_touched_in_branch)
+            for count, rev in enumerate(revisions)
+        ]
 
     def changes_in_commit(self) -> set[str]:
-        changed: set[str] = set(self._repo.git.diff(self.__get_filter_patterns(), None, name_only=True).splitlines())
+        changed: set[str] = set(
+            self._repo.git.diff(
+                self.__get_filter_patterns(), None, name_only=True
+            ).splitlines()
+        )
         return changed.union(self._repo.untracked_files)
 
     def changes_in_branch_including_local(self) -> list[Revision]:
         in_branch = self.changes_in_branch()
-        in_branch.append(Revision(len(in_branch), self.get_sha, self.changes_in_commit()))
+        in_branch.append(
+            Revision(len(in_branch), self.get_sha, self.changes_in_commit())
+        )
         return in_branch
 
     def changes_in_tagged_commit(self, current_tag: str) -> list[Revision]:
         curr_rev_tag = self.get_tag
 
         if curr_rev_tag != current_tag:
-            logging.error(f"HEAD is not at {curr_rev_tag} not at expected {current_tag}")
+            logging.error(
+                f"HEAD is not at {curr_rev_tag} not at expected {current_tag}"
+            )
             return []
 
         return self.changes_in_merge_commit()
 
     def changes_in_merge_commit(self):
         parent_revs = self._repo.head.commit.parents
         if not parent_revs:
-            logging.error("HEAD is not at merge commit, cannot determine changed files.")
+            logging.error(
+                "HEAD is not at merge commit, cannot determine changed files."
+            )
             return []
         logging.debug(f"Parent revisions: {parent_revs}")
-        files_changed = self._repo.git.diff(f"{str(self._repo.head.commit)}..{str(parent_revs[0])}",
-                                            name_only=True).splitlines()
+        files_changed = self._repo.git.diff(
+            f"{str(self._repo.head.commit)}..{str(parent_revs[0])}", name_only=True
+        ).splitlines()
         return [Revision(ord=0, hash=str(self.get_sha), files_touched=files_changed)]
 
     @property
     def main_branch_pulled(self) -> bool:
         if self._repo.head.is_detached:
             return False
         branch_names = list(map(lambda n: n.name, self._repo.references))
-        return f'{self._config.main_branch}' in branch_names
+        return f"{self._config.main_branch}" in branch_names
 
     def __get_remote(self) -> Remote:
-        default_remote = self._repo.remote('origin')
-        if 'https:' not in default_remote.url or self._config.repo_credentials is None:
+        default_remote = self._repo.remote("origin")
+        if "https:" not in default_remote.url or self._config.repo_credentials is None:
             return default_remote
 
-        return default_remote.set_url(self._config.repo_credentials.to_url_with_credentials)
+        return default_remote.set_url(
+            self._config.repo_credentials.to_url_with_credentials
+        )
 
     def pull_main_branch(self):
         remote = self.__get_remote()
         main = self._config.main_branch
         return remote.fetch(f"+refs/heads/{main}:refs/heads/{main}")
 
-    def find_projects(self, folder_pattern: str = '') -> list[str]:
-        """ returns a set of all project.yml files
+    def find_projects(self, folder_pattern: str = "") -> list[str]:
+        """returns a set of all project.yml files
         :type folder_pattern: project paths are filtered on this pattern
         """
-        projects = set(self._repo.git.ls_files(f'*{folder_pattern}*/{Project.project_yaml_path()}').splitlines())
+        projects = set(
+            self._repo.git.ls_files(
+                f"*{folder_pattern}*/{Project.project_yaml_path()}"
+            ).splitlines()
+        )
         return sorted(projects)
```

## mpyl/utilities/s3/__init__.py

```diff
@@ -11,74 +11,81 @@
 
 from ...project import Project
 from ...steps.models import RunProperties
 
 
 @dataclass
 class S3ClientConfig:
-    service_name = 's3'
-    region_name = 'eu-central-1'
+    service_name = "s3"
+    region_name = "eu-central-1"
     access_key_id: Optional[str]
     secret_access_key: Optional[str]
     bucket_name: str
     bucket_root_path: str
 
     def __init__(self, run_properties: RunProperties, bucket_name: str):
-        s3_connection_info = run_properties.config.get('s3', None)
-        self.access_key_id = s3_connection_info.get('accessKeyId')
-        self.secret_access_key = s3_connection_info.get('secretAccessKey')
+        s3_connection_info = run_properties.config.get("s3", None)
+        self.access_key_id = s3_connection_info.get("accessKeyId")
+        self.secret_access_key = s3_connection_info.get("secretAccessKey")
         self.bucket_name = bucket_name
         self.bucket_root_path = run_properties.versioning.identifier
 
 
 class S3Client:
-
     def __init__(self, logger: Logger, config: S3ClientConfig):
         """
         Creates a client that provides a wrapper for uploading a directory to an S3 bucket
 
         :param config: the S3 client config containing the necessary credentials and bucket information
         """
-        self._client = boto3.client(service_name=config.service_name,
-                                    region_name=config.region_name,
-                                    aws_access_key_id=config.access_key_id,
-                                    aws_secret_access_key=config.secret_access_key)
+        self._client = boto3.client(
+            service_name=config.service_name,
+            region_name=config.region_name,
+            aws_access_key_id=config.access_key_id,
+            aws_secret_access_key=config.secret_access_key,
+        )
         self._buck_name = config.bucket_name
         self._bucket_root_path = config.bucket_root_path
         self._logger = logger
         self.__validate_bucket()
 
     def __validate_bucket(self):
         """
         Validates that the bucket exists and that the user has access to it
         """
         try:
             self._client.head_bucket(Bucket=self._buck_name)
             self._logger.info(f"{self._buck_name} is a valid bucket")
         except ClientError as exc:
-            error_code = int(exc.response['Error']['Code'])
+            error_code = int(exc.response["Error"]["Code"])
             if error_code == HTTPStatus.FORBIDDEN:
-                self._logger.warning(f"Unable to access bucket {self._buck_name}: Forbidden")
+                self._logger.warning(
+                    f"Unable to access bucket {self._buck_name}: Forbidden"
+                )
             elif error_code == HTTPStatus.NOT_FOUND:
-                self._logger.warning(f"Unable to access bucket {self._buck_name}: Not found")
+                self._logger.warning(
+                    f"Unable to access bucket {self._buck_name}: Not found"
+                )
             raise exc
 
     def upload_directory(self, directory: str):
         """
         Uploads all files in a directory and its subdirectories to the S3 bucket
 
         Note: boto3 does not provide a sync method, so we have to walk the directory and upload each file individually
 
         :param directory: the name of the root directory containing the content to upload
         """
         walks = walk(directory)
         for path, _, filenames in walks:
             for filename in filenames:
-                src_path = f'{path}/{filename}'
-                dst_path = self.create_file_dst(root_path=self._bucket_root_path, file_path=path, filename=filename)
+                src_path = f"{path}/{filename}"
+                dst_path = self.create_file_dst(
+                    root_path=self._bucket_root_path, file_path=path, filename=filename
+                )
                 self.upload_file(src_path=src_path, dst_path=dst_path)
 
     @staticmethod
     def create_file_dst(root_path: str, file_path: str, filename: str):
         """
         Creates the bucket key for a given file based on its relative path and the given bucket root path
         i.e. /root/path/relative/path/filename
@@ -90,24 +97,30 @@
         :param file_path: the relative path of the file
         :param filename: the name of the file
         :return: the full destination path/key in the s3 bucket
         """
         path_parts = pathlib.Path(file_path).parts
         non_tmp_parts = path_parts[3:]
         relative_path = f"{'/'.join(filter(None, non_tmp_parts))}"
-        return f'{root_path}/{relative_path}/{filename}' if non_tmp_parts else f'{root_path}/{filename}'
+        return (
+            f"{root_path}/{relative_path}/{filename}"
+            if non_tmp_parts
+            else f"{root_path}/{filename}"
+        )
 
     def upload_file(self, src_path: str, dst_path: str):
         """
         Uploads an individual file to the S3 bucket
 
         :param src_path: the local relative path of the file
         :param dst_path: the destination path within the bucket
         """
         self._logger.debug(f"Uploading to bucket: {self._buck_name}")
         self._logger.debug(f"Uploading file at '{src_path}' to '{dst_path}'")
 
         try:
             self._client.upload_file(src_path, self._buck_name, dst_path)
         except ClientError as exc:
-            self._logger.warning(f'Unexpected exception uploading file: {src_path} - {exc}')
+            self._logger.warning(
+                f"Unexpected exception uploading file: {src_path} - {exc}"
+            )
             raise exc
```

## mpyl/utilities/sbt/__init__.py

```diff
@@ -13,31 +13,35 @@
     test_with_coverage: bool
     verbose: bool
     build_with_client: bool
     test_with_client: bool
 
     @staticmethod
     def from_config(config: Dict):
-        sbt_config = config.get('sbt', None)
+        sbt_config = config.get("sbt", None)
         if not sbt_config:
             raise KeyError(f"'sbt' could not be loaded from {config}")
         return SbtConfig(
-            sbt_command=sbt_config['command'],
-            sbt_client_command=sbt_config['clientCommand'],
-            java_opts=sbt_config['javaOpts'],
-            sbt_opts=sbt_config['sbtOpts'],
-            test_with_coverage=(str(sbt_config['testWithCoverage']).lower() == 'true'),
-            verbose=(str(sbt_config['verbose']).lower() == 'true'),
-            build_with_client=(str(sbt_config.get('clientMode', {}).get('build')).lower() == 'true'),
-            test_with_client=(str(sbt_config.get('clientMode', {}).get('test')).lower() == 'true')
+            sbt_command=sbt_config["command"],
+            sbt_client_command=sbt_config["clientCommand"],
+            java_opts=sbt_config["javaOpts"],
+            sbt_opts=sbt_config["sbtOpts"],
+            test_with_coverage=(str(sbt_config["testWithCoverage"]).lower() == "true"),
+            verbose=(str(sbt_config["verbose"]).lower() == "true"),
+            build_with_client=(
+                str(sbt_config.get("clientMode", {}).get("build")).lower() == "true"
+            ),
+            test_with_client=(
+                str(sbt_config.get("clientMode", {}).get("test")).lower() == "true"
+            ),
         )
 
     def to_command(self, client_mode: bool, sbt_commands: list[str]):
         cmd = [self.sbt_client_command if client_mode else self.sbt_command]
         if self.verbose:
-            cmd.append('-v')
-        cmd.extend([f'-J{opt}' for opt in self.java_opts.split(' ')])
-        cmd.extend([f'-D{opt}' for opt in self.sbt_opts.split(' ')])
+            cmd.append("-v")
+        cmd.extend([f"-J{opt}" for opt in self.java_opts.split(" ")])
+        cmd.extend([f"-D{opt}" for opt in self.sbt_opts.split(" ")])
 
         joined_commands = "; ".join(sbt_commands)
         cmd.append(joined_commands)
         return cmd
```

## mpyl/utilities/subprocess/__init__.py

```diff
@@ -3,50 +3,62 @@
 import subprocess
 from logging import Logger
 from typing import Union
 
 from ...steps.models import Output
 
 
-def custom_check_output(logger: Logger, command: Union[str, list[str]], capture_stdout: bool = False) -> Output:
+def custom_check_output(
+    logger: Logger, command: Union[str, list[str]], capture_stdout: bool = False
+) -> Output:
     """
     Wrapper around subprocess.Popen
     ⚠️ Using this function implies an implicit runtime OS dependency.
     Avoid this if at all possible. For example, to run docker commands, use the bundled docker client (python-on-whales)
     which makes the dependency on docker explicit and adds a lot of convenience methods.
     """
     if isinstance(command, str):
-        command = command.split(' ')
+        command = command.split(" ")
 
-    command_argument = ' '.join(command)
+    command_argument = " ".join(command)
     logger.info(f"Executing: '{command_argument}'")
     try:
         if capture_stdout:
-            out = subprocess.check_output(command, stderr=subprocess.STDOUT).decode("utf-8")
+            out = subprocess.check_output(command, stderr=subprocess.STDOUT).decode(
+                "utf-8"
+            )
             print(out)
             return Output(success=True, message=out)
 
         with subprocess.Popen(command, stdout=subprocess.PIPE, text=True) as process:
             if not process.stdout:
-                raise RuntimeError(f'Process {command_argument} does not have an stdout')
+                raise RuntimeError(
+                    f"Process {command_argument} does not have an stdout"
+                )
 
             for line in iter(process.stdout.readline, ""):
                 if line:
                     print(line.rstrip())
                 if process.poll() is not None:
                     break
             success = process.wait() == 0
             if not success:
-                logger.warning(f"Subprocess failed: {process.stderr.read() if process.stderr else 'No stderr output'}")
-
-            return Output(success=success, message='Subprocess executed successfully')
+                logger.warning(
+                    "Subprocess failed" + f" with {process.stderr.read()}"
+                    if process.stderr
+                    else ""
+                )
+                return Output(success=False, message="Subprocess failed")
 
+            return Output(success=True, message="Subprocess executed successfully")
 
     except subprocess.CalledProcessError as exc:
-        logger.warning(f"'{command_argument}': failed with return code: {exc.returncode} err: "
-                       f"{exc.stderr.decode() if exc.stderr else 'No stderr output'}",
-                       exc_info=True)
+        logger.warning(
+            f"'{command_argument}': failed with return code: {exc.returncode} err: "
+            f"{exc.stderr.decode() if exc.stderr else 'No stderr output'}",
+            exc_info=True,
+        )
 
     except FileNotFoundError:
         logger.warning(f"'{command_argument}: file not found", exc_info=True)
 
-    return Output(success=False, message='Subprocess failed')
+    return Output(success=False, message="Subprocess failed")
```

## Comparing `mpyl-1.0.6.dist-info/LICENSE` & `mpyl-1.0.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mpyl-1.0.6.dist-info/METADATA` & `mpyl-1.0.7.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6d70 796c  : 2.1.Name: mpyl
-00000020: 0a56 6572 7369 6f6e 3a20 312e 302e 360a  .Version: 1.0.6.
+00000020: 0a56 6572 7369 6f6e 3a20 312e 302e 370a  .Version: 1.0.7.
 00000030: 5375 6d6d 6172 793a 204d 6f64 756c 6172  Summary: Modular
 00000040: 2050 6970 656c 696e 6520 4c69 6272 6172   Pipeline Librar
 00000050: 790a 486f 6d65 2d70 6167 653a 2068 7474  y.Home-page: htt
 00000060: 7073 3a2f 2f76 616e 6465 6272 6f6e 2e67  ps://vandebron.g
 00000070: 6974 6875 622e 696f 2f6d 7079 6c0a 4175  ithub.io/mpyl.Au
 00000080: 7468 6f72 3a20 5661 6e64 6562 726f 6e20  thor: Vandebron 
 00000090: 456e 6572 6769 6520 4256 0a50 726f 6a65  Energie BV.Proje
@@ -156,217 +156,226 @@
 000009b0: 792d 6c61 6e67 2e6f 7267 2f29 0a5b 215b  y-lang.org/).[![
 000009c0: 6c69 6e74 696e 673a 2070 796c 696e 745d  linting: pylint]
 000009d0: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
 000009e0: 656c 6473 2e69 6f2f 6261 6467 652f 6c69  elds.io/badge/li
 000009f0: 6e74 696e 672d 7079 6c69 6e74 2d79 656c  nting-pylint-yel
 00000a00: 6c6f 7767 7265 656e 295d 2868 7474 7073  lowgreen)](https
 00000a10: 3a2f 2f67 6974 6875 622e 636f 6d2f 5079  ://github.com/Py
-00000a20: 4351 412f 7079 6c69 6e74 290a 0a23 2057  CQA/pylint)..# W
-00000a30: 6861 7420 6973 204d 5079 4c3f 0a0a 4d50  hat is MPyL?..MP
-00000a40: 794c 2073 7461 6e64 7320 666f 7220 4d6f  yL stands for Mo
-00000a50: 6475 6c61 7220 5069 7065 6c69 6e65 204c  dular Pipeline L
-00000a60: 6962 7261 7279 2028 696e 2050 7974 686f  ibrary (in Pytho
-00000a70: 6e29 2e0a 0a54 6869 7320 6c69 6272 6172  n)...This librar
-00000a80: 7920 6973 206c 6f6f 7365 6c79 2062 6173  y is loosely bas
-00000a90: 6564 206f 6e20 7468 6520 7072 696e 6369  ed on the princi
-00000aa0: 706c 6573 2064 6573 6372 6962 6564 2069  ples described i
-00000ab0: 6e20 6874 7470 733a 2f2f 7777 772e 6a65  n https://www.je
-00000ac0: 6e6b 696e 732e 696f 2f62 6c6f 672f 3230  nkins.io/blog/20
-00000ad0: 3139 2f30 312f 3038 2f6d 706c 2d6d 6f64  19/01/08/mpl-mod
-00000ae0: 756c 6172 2d70 6970 656c 696e 652d 6c69  ular-pipeline-li
-00000af0: 6272 6172 792f 0a62 7574 2063 6f6d 706c  brary/.but compl
-00000b00: 6574 656c 7920 696e 6465 7065 6e64 656e  etely independen
-00000b10: 7420 6f66 204a 656e 6b69 6e73 206f 7220  t of Jenkins or 
-00000b20: 616e 7920 6f74 6865 7220 4349 2f43 4420  any other CI/CD 
-00000b30: 706c 6174 666f 726d 2e0a 0a23 2320 f09f  platform...## ..
-00000b40: 9496 2044 6f63 756d 656e 7461 7469 6f6e  .. Documentation
-00000b50: 0a44 6574 6169 6c65 642c 202a 636f 6d70  .Detailed, *comp
-00000b60: 6c65 7465 2a2c 2073 6561 7263 6861 626c  lete*, searchabl
-00000b70: 6520 646f 6375 6d65 6e74 6174 696f 6e20  e documentation 
-00000b80: 6361 6e20 6265 2066 6f75 6e64 2061 7420  can be found at 
-00000b90: 5b68 7474 7073 3a2f 2f76 616e 6465 6272  [https://vandebr
-00000ba0: 6f6e 2e67 6974 6875 622e 696f 2f6d 7079  on.github.io/mpy
-00000bb0: 6c5d 2868 7474 7073 3a2f 2f76 616e 6465  l](https://vande
-00000bc0: 6272 6f6e 2e67 6974 6875 622e 696f 2f6d  bron.github.io/m
-00000bd0: 7079 6c29 0a0a 2323 20f0 9f93 9a20 5072  pyl)..## .... Pr
-00000be0: 696e 6369 706c 6573 0a0a 4d50 794c 2069  inciples..MPyL i
-00000bf0: 7320 6275 696c 7420 7769 7468 2074 6865  s built with the
-00000c00: 2066 6f6c 6c6f 7769 6e67 2070 7269 6e63   following princ
-00000c10: 6970 6c65 7320 696e 206d 696e 642e 0a2d  iples in mind..-
-00000c20: 202a 2a4e 6f74 2061 2070 6c61 7466 6f72   **Not a platfor
-00000c30: 6d2a 2a20 4974 2069 7320 6e6f 7420 7469  m** It is not ti
-00000c40: 6564 2074 6f20 616e 7920 4349 2f43 4420  ed to any CI/CD 
-00000c50: 706c 6174 666f 726d 2e20 4d50 794c 2069  platform. MPyL i
-00000c60: 7320 6120 6c69 6272 6172 792c 206e 6f74  s a library, not
-00000c70: 2061 2066 7261 6d65 776f 726b 2e20 4974   a framework. It
-00000c80: 2069 7320 6e6f 7420 6120 7275 6e6e 6572   is not a runner
-00000c90: 2c0a 2020 6e6f 7420 6120 7363 6865 6475  ,.  not a schedu
-00000ca0: 6c65 722c 2061 6e64 2069 7420 646f 6573  ler, and it does
-00000cb0: 6e27 7420 6861 7665 2061 2047 5549 2e20  n't have a GUI. 
-00000cc0: 4974 2063 616e 2062 6520 706c 7567 6765  It can be plugge
-00000cd0: 6420 696e 746f 2061 6e79 2043 492f 4344  d into any CI/CD
-00000ce0: 2070 6c61 7466 6f72 6d2e 2045 7865 6375   platform. Execu
-00000cf0: 7469 6f6e 2066 6c6f 7773 2066 6f72 0a20  tion flows for. 
-00000d00: 204a 656e 6b69 6e73 206f 7220 4461 6773   Jenkins or Dags
-00000d10: 7465 7220 6172 6520 696e 636c 7564 6564  ter are included
-00000d20: 2061 7320 616e 2065 7861 6d70 6c65 2e0a   as an example..
-00000d30: 2d20 2a2a 4d69 6e69 6d61 6c20 666f 6f74  - **Minimal foot
-00000d40: 7072 696e 742a 2a3a 2049 7420 6973 2073  print**: It is s
-00000d50: 656c 662d 636f 6e74 6169 6e65 6420 616e  elf-contained an
-00000d60: 6420 6861 7320 7665 7279 2066 6577 2065  d has very few e
-00000d70: 7874 6572 6e61 6c20 6465 7065 6e64 656e  xternal dependen
-00000d80: 6369 6573 2028 652e 672e 2047 6974 2c20  cies (e.g. Git, 
-00000d90: 446f 636b 6572 206f 7220 4845 4c4d 292e  Docker or HELM).
-00000da0: 0a20 2049 7420 6361 6e20 6265 2072 756e  .  It can be run
-00000db0: 2061 6e79 7768 6572 652c 2061 6c73 6f20   anywhere, also 
-00000dc0: 6f6e 2079 6f75 7220 6c6f 6361 6c20 6d61  on your local ma
-00000dd0: 6368 696e 652e 0a2d 202a 2a41 6363 6573  chine..- **Acces
-00000de0: 7369 626c 6520 616e 6420 6d61 696e 7461  sible and mainta
-00000df0: 696e 6162 6c65 2a2a 0a20 2020 202d 2057  inable**.    - W
-00000e00: 7269 7474 656e 2069 6e20 5079 7468 6f6e  ritten in Python
-00000e10: 2c20 7468 6520 6d6f 7374 2077 6964 656c  , the most widel
-00000e20: 7920 6164 6f70 7465 6420 7363 7269 7074  y adopted script
-00000e30: 696e 6720 6c61 6e67 7561 6765 2077 6974  ing language wit
-00000e40: 6820 616e 2065 7874 656e 7369 7665 2061  h an extensive a
-00000e50: 6d6f 756e 7420 6f66 2063 6c69 656e 7420  mount of client 
-00000e60: 6c69 6272 6172 6965 7320 7265 6c65 7661  libraries releva
-00000e70: 6e74 2074 6f20 4349 2f43 442e 0a20 2020  nt to CI/CD..   
-00000e80: 202d 2053 7472 6f6e 676c 7920 7479 7065   - Strongly type
-00000e90: 643a 2060 4d79 5079 6020 7479 7065 2068  d: `MyPy` type h
-00000ea0: 696e 7473 2061 6e64 2073 6368 656d 6173  ints and schemas
-00000eb0: 2066 6f72 2061 6c6c 2060 5941 4d4c 6020   for all `YAML` 
-00000ec0: 6669 6c65 732e 2043 6c65 6172 6c79 2064  files. Clearly d
-00000ed0: 6566 696e 6564 2069 6e74 6572 6661 6365  efined interface
-00000ee0: 7320 666f 7220 696e 7075 7473 0a20 2020  s for inputs.   
-00000ef0: 2020 2061 6e64 206f 7574 7075 7473 206f     and outputs o
-00000f00: 6620 7374 6570 732e 0a20 2020 202d 2046  f steps..    - F
-00000f10: 6f63 7573 206f 6e20 7368 6f72 7420 6665  ocus on short fe
-00000f20: 6564 6261 636b 206c 6f6f 702e 2055 6e69  edback loop. Uni
-00000f30: 7420 7465 7374 6162 6c65 2061 6e64 2065  t testable and e
-00000f40: 7665 7279 7468 696e 6720 6361 6e20 6265  verything can be
-00000f50: 2072 756e 206c 6f63 616c 6c79 2e0a 2d20   run locally..- 
-00000f60: 2a2a 5365 6c66 2064 6f63 756d 656e 7465  **Self documente
-00000f70: 642a 2a20 6279 205b 646f 6373 7472 696e  d** by [docstrin
-00000f80: 6773 5d28 6874 7470 733a 2f2f 7661 6e64  gs](https://vand
-00000f90: 6562 726f 6e2e 6769 7468 7562 2e69 6f2f  ebron.github.io/
-00000fa0: 6d70 796c 2920 696e 2074 6865 2063 6f64  mpyl) in the cod
-00000fb0: 652c 2064 6573 6372 6970 7469 6f6e 7320  e, descriptions 
-00000fc0: 696e 2074 6865 2073 6368 656d 6173 0a20  in the schemas. 
-00000fd0: 2061 6e64 2065 7870 6c61 6e61 7469 6f6e   and explanation
-00000fe0: 7320 696e 2074 6865 2043 4c49 2e0a 2d20  s in the CLI..- 
-00000ff0: 2a2a 5079 7468 6f6e 2061 7320 5941 4d4c  **Python as YAML
-00001000: 2074 656d 706c 6174 696e 6720 656e 6769   templating engi
-00001010: 6e65 2a2a 2041 7474 656d 7074 7320 746f  ne** Attempts to
-00001020: 206d 6978 206d 6172 6b75 7020 616e 6420   mix markup and 
-00001030: 6c6f 6769 6320 7465 6e64 2074 6f20 6861  logic tend to ha
-00001040: 7665 2061 0a20 205b 776f 7273 7420 6f66  ve a.  [worst of
-00001050: 2062 6f74 6820 776f 726c 6473 5d28 6874   both worlds](ht
-00001060: 7470 733a 2f2f 616e 7468 6f6e 7968 6177  tps://anthonyhaw
-00001070: 6b69 6e73 2e6d 6564 6975 6d2e 636f 6d2f  kins.medium.com/
-00001080: 6973 2d70 7974 686f 6e2d 7468 652d 7065  is-python-the-pe
-00001090: 7266 6563 742d 6a73 6f6e 2d79 616d 6c2d  rfect-json-yaml-
-000010a0: 7465 6d70 6c61 7469 6e67 2d65 6e67 696e  templating-engin
-000010b0: 652d 6335 6331 6233 3234 3138 6636 290a  e-c5c1b32418f6).
-000010c0: 2020 6f75 7463 6f6d 652e 204d 5079 4c20    outcome. MPyL 
-000010d0: 7573 6573 2060 5941 4d4c 6020 7374 7269  uses `YAML` stri
-000010e0: 6374 6c79 2066 6f72 2063 6f6e 6669 6775  ctly for configu
-000010f0: 7261 7469 6f6e 2e20 5768 6572 6520 6059  ration. Where `Y
-00001100: 414d 4c60 206e 6565 6473 2074 6f20 7072  AML` needs to pr
-00001110: 6f64 7563 6564 2064 796e 616d 6963 616c  oduced dynamical
-00001120: 6c79 2c20 6c69 6b65 2066 6f72 2043 5244  ly, like for CRD
-00001130: 7320 7669 610a 2020 4845 4c4d 2063 6861  s via.  HELM cha
-00001140: 7274 732c 2069 7420 6973 2067 656e 6572  rts, it is gener
-00001150: 6174 6564 2062 7920 5079 7468 6f6e 2063  ated by Python c
-00001160: 6f64 652e 2054 6520 7072 6f64 7563 6564  ode. Te produced
-00001170: 2060 5941 4d4c 6020 6973 2076 616c 6964   `YAML` is valid
-00001180: 6174 6564 2061 6761 696e 7374 2074 6865  ated against the
-00001190: 2063 6f72 7265 7370 6f6e 6469 6e67 2073   corresponding s
-000011a0: 6368 656d 6173 2e0a 2d20 2a2a 4578 7465  chemas..- **Exte
-000011b0: 6e73 6962 6c65 2a2a 2053 7570 706f 7274  nsible** Support
-000011c0: 2066 6f72 2074 6865 206d 6f73 7420 636f   for the most co
-000011d0: 6d6d 6f6e 2075 7365 2063 6173 6573 2028  mmon use cases (
-000011e0: 652e 672e 2044 6f63 6b65 722c 2048 656c  e.g. Docker, Hel
-000011f0: 6d2c 204b 7562 6572 6e65 7465 732c 2041  m, Kubernetes, A
-00001200: 5753 2c20 6574 632e 2920 6973 2062 7569  WS, etc.) is bui
-00001210: 6c74 2d69 6e2e 0a20 2042 7574 2069 7420  lt-in..  But it 
-00001220: 6973 2065 6173 7920 746f 2065 7874 656e  is easy to exten
-00001230: 6420 7769 7468 2079 6f75 7220 6f77 6e20  d with your own 
-00001240: 606d 7079 6c2e 7374 6570 7360 2e0a 0a23  `mpyl.steps`...#
-00001250: 2320 f09f 92bb 2054 6563 686e 6f6c 6f67  # .... Technolog
-00001260: 6965 730a 0a23 2323 2052 6571 7569 7265  ies..### Require
-00001270: 6d65 6e74 730a 5468 6520 666f 6c6c 6f77  ments.The follow
-00001280: 696e 6720 7465 6368 6e6f 6c6f 6769 6573  ing technologies
-00001290: 2061 7265 2065 7870 6563 7465 6420 746f   are expected to
-000012a0: 2062 6520 7072 6573 656e 7420 6f6e 2074   be present on t
-000012b0: 6865 206c 6f63 616c 204f 533a 0a2d 205b  he local OS:.- [
-000012c0: 5079 7468 6f6e 5d28 6874 7470 733a 2f2f  Python](https://
-000012d0: 7777 772e 7079 7468 6f6e 2e6f 7267 2f29  www.python.org/)
-000012e0: 203e 3d20 332e 390a 2d20 5b50 6970 5d28   >= 3.9.- [Pip](
-000012f0: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
-00001300: 2f70 726f 6a65 6374 2f70 6970 2f29 203e  /project/pip/) >
-00001310: 3d20 3233 2e30 2e31 0a2d 205b 446f 636b  = 23.0.1.- [Dock
-00001320: 6572 5d28 6874 7470 733a 2f2f 7777 772e  er](https://www.
-00001330: 646f 636b 6572 2e63 6f6d 2f29 203e 2032  docker.com/) > 2
-00001340: 300a 2d20 5b44 6f63 6b65 7220 636f 6d70  0.- [Docker comp
-00001350: 6f73 655d 2868 7474 7073 3a2f 2f64 6f63  ose](https://doc
-00001360: 732e 646f 636b 6572 2e63 6f6d 2f63 6f6d  s.docker.com/com
-00001370: 706f 7365 2f69 6e73 7461 6c6c 2f6c 696e  pose/install/lin
-00001380: 7578 2f29 0a20 2069 6e73 7461 6c6c 6564  ux/).  installed
-00001390: 2061 7320 706c 7567 696e 2028 6064 6f63   as plugin (`doc
-000013a0: 6b65 7220 636f 6d70 6f73 6520 7665 7273  ker compose vers
-000013b0: 696f 6e60 2920 3e3d 2076 322e 322e 330a  ion`) >= v2.2.3.
-000013c0: 2d20 5b47 6974 5d28 6874 7470 733a 2f2f  - [Git](https://
-000013d0: 6769 742d 7363 6d2e 636f 6d2f 2920 5343  git-scm.com/) SC
-000013e0: 4d0a 0a23 2323 2042 756e 646c 6564 0a4d  M..### Bundled.M
-000013f0: 5079 4c20 6973 2065 7874 656e 7369 626c  PyL is extensibl
-00001400: 6520 616e 6420 6861 7320 6120 6d69 6e69  e and has a mini
-00001410: 6d61 6c20 666f 6f74 7072 696e 742e 2048  mal footprint. H
-00001420: 6176 696e 6720 7361 6964 2074 6861 742c  aving said that,
-00001430: 2062 6174 7465 7269 6573 2066 6f72 2074   batteries for t
-00001440: 6865 2066 6f6c 6c6f 7769 6e67 2074 6563  he following tec
-00001450: 686e 6f6c 6f67 6965 7320 6172 6520 696e  hnologies are in
-00001460: 636c 7564 6564 2e0a 0a23 2323 2323 2043  cluded...##### C
-00001470: 492f 4344 0a23 2323 2323 2320 4275 696c  I/CD.###### Buil
-00001480: 640a 2d20 5b44 6f63 6b65 725d 2868 7474  d.- [Docker](htt
-00001490: 7073 3a2f 2f77 7777 2e64 6f63 6b65 722e  ps://www.docker.
-000014a0: 636f 6d2f 2920 606d 7079 6c2e 7374 6570  com/) `mpyl.step
-000014b0: 732e 6275 696c 642e 646f 636b 6572 6275  s.build.dockerbu
-000014c0: 696c 6460 0a2d 205b 5363 616c 6120 2853  ild`.- [Scala (S
-000014d0: 4254 295d 2868 7474 7073 3a2f 2f77 7777  BT)](https://www
-000014e0: 2e73 6361 6c61 2d73 6274 2e6f 7267 2f29  .scala-sbt.org/)
-000014f0: 2060 6d70 796c 2e73 7465 7073 2e62 7569   `mpyl.steps.bui
-00001500: 6c64 2e73 6274 600a 2d20 5b4a 656e 6b69  ld.sbt`.- [Jenki
-00001510: 6e73 5d28 6874 7470 733a 2f2f 7777 772e  ns](https://www.
-00001520: 6a65 6e6b 696e 732e 696f 2f29 2020 606d  jenkins.io/)  `m
-00001530: 7079 6c2e 636c 692e 636f 6d6d 616e 6473  pyl.cli.commands
-00001540: 2e62 7569 6c64 2e6a 656e 6b69 6e73 6020  .build.jenkins` 
-00001550: 616e 640a 2020 606d 7079 6c2e 7574 696c  and.  `mpyl.util
-00001560: 6974 6965 732e 6a65 6e6b 696e 732e 7275  ities.jenkins.ru
-00001570: 6e6e 6572 2e4a 656e 6b69 6e73 5275 6e6e  nner.JenkinsRunn
-00001580: 6572 600a 0a23 2323 2323 2320 5465 7374  er`..###### Test
-00001590: 696e 670a 2d20 5b4a 756e 6974 5d28 6874  ing.- [Junit](ht
-000015a0: 7470 733a 2f2f 6a75 6e69 742e 6f72 672f  tps://junit.org/
-000015b0: 2920 606d 7079 6c2e 7374 6570 732e 6d6f  ) `mpyl.steps.mo
-000015c0: 6465 6c73 2e41 7274 6966 6163 7454 7970  dels.ArtifactTyp
-000015d0: 652e 4a55 4e49 545f 5445 5354 5360 0a0a  e.JUNIT_TESTS`..
-000015e0: 2323 2323 2323 2044 6570 6c6f 796d 656e  ###### Deploymen
-000015f0: 740a 2d20 5b4b 3853 5d28 6874 7470 733a  t.- [K8S](https:
-00001600: 2f2f 6b75 6265 726e 6574 6573 2e69 6f2f  //kubernetes.io/
-00001610: 2920 606d 7079 6c2e 7374 6570 732e 6465  ) `mpyl.steps.de
-00001620: 706c 6f79 2e6b 7562 6572 6e65 7465 7360  ploy.kubernetes`
-00001630: 0a2d 205b 4865 6c6d 5d28 6874 7470 733a  .- [Helm](https:
-00001640: 2f2f 6865 6c6d 2e73 682f 2920 606d 7079  //helm.sh/) `mpy
-00001650: 6c2e 7374 6570 732e 6465 706c 6f79 2e6b  l.steps.deploy.k
-00001660: 3873 2e68 656c 6d60 0a0a 2323 2323 2320  8s.helm`..##### 
-00001670: 5265 706f 7274 696e 670a 2d20 5b4a 6972  Reporting.- [Jir
-00001680: 615d 2868 7474 7073 3a2f 2f77 7777 2e61  a](https://www.a
-00001690: 746c 6173 7369 616e 2e63 6f6d 2920 606d  tlassian.com) `m
-000016a0: 7079 6c2e 7265 706f 7274 696e 672e 7461  pyl.reporting.ta
-000016b0: 7267 6574 732e 6a69 7261 600a 2d20 5b47  rgets.jira`.- [G
-000016c0: 6974 6875 625d 2868 7474 7073 3a2f 2f67  ithub](https://g
-000016d0: 6974 6875 622e 636f 6d2f 2920 606d 7079  ithub.com/) `mpy
-000016e0: 6c2e 7265 706f 7274 696e 672e 7461 7267  l.reporting.targ
-000016f0: 6574 732e 6769 7468 7562 600a 2d20 5b53  ets.github`.- [S
-00001700: 6c61 636b 5d28 6874 7470 733a 2f2f 736c  lack](https://sl
-00001710: 6163 6b2e 636f 6d2f 2920 606d 7079 6c2e  ack.com/) `mpyl.
-00001720: 7265 706f 7274 696e 672e 7461 7267 6574  reporting.target
-00001730: 732e 736c 6163 6b60 0a                   s.slack`.
+00000a20: 4351 412f 7079 6c69 6e74 290a 3c61 2068  CQA/pylint).<a h
+00000a30: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
+00000a40: 6875 622e 636f 6d2f 7073 662f 626c 6163  hub.com/psf/blac
+00000a50: 6b22 3e3c 696d 6720 616c 743d 2243 6f64  k"><img alt="Cod
+00000a60: 6520 7374 796c 653a 2062 6c61 636b 2220  e style: black" 
+00000a70: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
+00000a80: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
+00000a90: 652f 636f 6465 2532 3073 7479 6c65 2d62  e/code%20style-b
+00000aa0: 6c61 636b 2d30 3030 3030 302e 7376 6722  lack-000000.svg"
+00000ab0: 3e3c 2f61 3e0a 0a23 2057 6861 7420 6973  ></a>..# What is
+00000ac0: 204d 5079 4c3f 0a0a 4d50 794c 2073 7461   MPyL?..MPyL sta
+00000ad0: 6e64 7320 666f 7220 4d6f 6475 6c61 7220  nds for Modular 
+00000ae0: 5069 7065 6c69 6e65 204c 6962 7261 7279  Pipeline Library
+00000af0: 2028 696e 2050 7974 686f 6e29 2e0a 0a54   (in Python)...T
+00000b00: 6869 7320 6c69 6272 6172 7920 6973 206c  his library is l
+00000b10: 6f6f 7365 6c79 2062 6173 6564 206f 6e20  oosely based on 
+00000b20: 7468 6520 7072 696e 6369 706c 6573 2064  the principles d
+00000b30: 6573 6372 6962 6564 2069 6e20 6874 7470  escribed in http
+00000b40: 733a 2f2f 7777 772e 6a65 6e6b 696e 732e  s://www.jenkins.
+00000b50: 696f 2f62 6c6f 672f 3230 3139 2f30 312f  io/blog/2019/01/
+00000b60: 3038 2f6d 706c 2d6d 6f64 756c 6172 2d70  08/mpl-modular-p
+00000b70: 6970 656c 696e 652d 6c69 6272 6172 792f  ipeline-library/
+00000b80: 0a62 7574 2063 6f6d 706c 6574 656c 7920  .but completely 
+00000b90: 696e 6465 7065 6e64 656e 7420 6f66 204a  independent of J
+00000ba0: 656e 6b69 6e73 206f 7220 616e 7920 6f74  enkins or any ot
+00000bb0: 6865 7220 4349 2f43 4420 706c 6174 666f  her CI/CD platfo
+00000bc0: 726d 2e0a 0a23 2320 f09f 9496 2044 6f63  rm...## .... Doc
+00000bd0: 756d 656e 7461 7469 6f6e 0a44 6574 6169  umentation.Detai
+00000be0: 6c65 642c 202a 636f 6d70 6c65 7465 2a2c  led, *complete*,
+00000bf0: 2073 6561 7263 6861 626c 6520 646f 6375   searchable docu
+00000c00: 6d65 6e74 6174 696f 6e20 6361 6e20 6265  mentation can be
+00000c10: 2066 6f75 6e64 2061 7420 5b68 7474 7073   found at [https
+00000c20: 3a2f 2f76 616e 6465 6272 6f6e 2e67 6974  ://vandebron.git
+00000c30: 6875 622e 696f 2f6d 7079 6c5d 2868 7474  hub.io/mpyl](htt
+00000c40: 7073 3a2f 2f76 616e 6465 6272 6f6e 2e67  ps://vandebron.g
+00000c50: 6974 6875 622e 696f 2f6d 7079 6c29 0a0a  ithub.io/mpyl)..
+00000c60: 2323 20f0 9f93 9a20 5072 696e 6369 706c  ## .... Principl
+00000c70: 6573 0a0a 4d50 794c 2069 7320 6275 696c  es..MPyL is buil
+00000c80: 7420 7769 7468 2074 6865 2066 6f6c 6c6f  t with the follo
+00000c90: 7769 6e67 2070 7269 6e63 6970 6c65 7320  wing principles 
+00000ca0: 696e 206d 696e 642e 0a2d 202a 2a4e 6f74  in mind..- **Not
+00000cb0: 2061 2070 6c61 7466 6f72 6d2a 2a20 4974   a platform** It
+00000cc0: 2069 7320 6e6f 7420 7469 6564 2074 6f20   is not tied to 
+00000cd0: 616e 7920 4349 2f43 4420 706c 6174 666f  any CI/CD platfo
+00000ce0: 726d 2e20 4d50 794c 2069 7320 6120 6c69  rm. MPyL is a li
+00000cf0: 6272 6172 792c 206e 6f74 2061 2066 7261  brary, not a fra
+00000d00: 6d65 776f 726b 2e20 4974 2069 7320 6e6f  mework. It is no
+00000d10: 7420 6120 7275 6e6e 6572 2c0a 2020 6e6f  t a runner,.  no
+00000d20: 7420 6120 7363 6865 6475 6c65 722c 2061  t a scheduler, a
+00000d30: 6e64 2069 7420 646f 6573 6e27 7420 6861  nd it doesn't ha
+00000d40: 7665 2061 2047 5549 2e20 4974 2063 616e  ve a GUI. It can
+00000d50: 2062 6520 706c 7567 6765 6420 696e 746f   be plugged into
+00000d60: 2061 6e79 2043 492f 4344 2070 6c61 7466   any CI/CD platf
+00000d70: 6f72 6d2e 2045 7865 6375 7469 6f6e 2066  orm. Execution f
+00000d80: 6c6f 7773 2066 6f72 0a20 204a 656e 6b69  lows for.  Jenki
+00000d90: 6e73 206f 7220 4461 6773 7465 7220 6172  ns or Dagster ar
+00000da0: 6520 696e 636c 7564 6564 2061 7320 616e  e included as an
+00000db0: 2065 7861 6d70 6c65 2e0a 2d20 2a2a 4d69   example..- **Mi
+00000dc0: 6e69 6d61 6c20 666f 6f74 7072 696e 742a  nimal footprint*
+00000dd0: 2a3a 2049 7420 6973 2073 656c 662d 636f  *: It is self-co
+00000de0: 6e74 6169 6e65 6420 616e 6420 6861 7320  ntained and has 
+00000df0: 7665 7279 2066 6577 2065 7874 6572 6e61  very few externa
+00000e00: 6c20 6465 7065 6e64 656e 6369 6573 2028  l dependencies (
+00000e10: 652e 672e 2047 6974 2c20 446f 636b 6572  e.g. Git, Docker
+00000e20: 206f 7220 4845 4c4d 292e 0a20 2049 7420   or HELM)..  It 
+00000e30: 6361 6e20 6265 2072 756e 2061 6e79 7768  can be run anywh
+00000e40: 6572 652c 2061 6c73 6f20 6f6e 2079 6f75  ere, also on you
+00000e50: 7220 6c6f 6361 6c20 6d61 6368 696e 652e  r local machine.
+00000e60: 0a2d 202a 2a41 6363 6573 7369 626c 6520  .- **Accessible 
+00000e70: 616e 6420 6d61 696e 7461 696e 6162 6c65  and maintainable
+00000e80: 2a2a 0a20 2020 202d 2057 7269 7474 656e  **.    - Written
+00000e90: 2069 6e20 5079 7468 6f6e 2c20 7468 6520   in Python, the 
+00000ea0: 6d6f 7374 2077 6964 656c 7920 6164 6f70  most widely adop
+00000eb0: 7465 6420 7363 7269 7074 696e 6720 6c61  ted scripting la
+00000ec0: 6e67 7561 6765 2077 6974 6820 616e 2065  nguage with an e
+00000ed0: 7874 656e 7369 7665 2061 6d6f 756e 7420  xtensive amount 
+00000ee0: 6f66 2063 6c69 656e 7420 6c69 6272 6172  of client librar
+00000ef0: 6965 7320 7265 6c65 7661 6e74 2074 6f20  ies relevant to 
+00000f00: 4349 2f43 442e 0a20 2020 202d 2053 7472  CI/CD..    - Str
+00000f10: 6f6e 676c 7920 7479 7065 643a 2060 4d79  ongly typed: `My
+00000f20: 5079 6020 7479 7065 2068 696e 7473 2061  Py` type hints a
+00000f30: 6e64 2073 6368 656d 6173 2066 6f72 2061  nd schemas for a
+00000f40: 6c6c 2060 5941 4d4c 6020 6669 6c65 732e  ll `YAML` files.
+00000f50: 2043 6c65 6172 6c79 2064 6566 696e 6564   Clearly defined
+00000f60: 2069 6e74 6572 6661 6365 7320 666f 7220   interfaces for 
+00000f70: 696e 7075 7473 0a20 2020 2020 2061 6e64  inputs.      and
+00000f80: 206f 7574 7075 7473 206f 6620 7374 6570   outputs of step
+00000f90: 732e 0a20 2020 202d 2046 6f63 7573 206f  s..    - Focus o
+00000fa0: 6e20 7368 6f72 7420 6665 6564 6261 636b  n short feedback
+00000fb0: 206c 6f6f 702e 2055 6e69 7420 7465 7374   loop. Unit test
+00000fc0: 6162 6c65 2061 6e64 2065 7665 7279 7468  able and everyth
+00000fd0: 696e 6720 6361 6e20 6265 2072 756e 206c  ing can be run l
+00000fe0: 6f63 616c 6c79 2e0a 2d20 2a2a 5365 6c66  ocally..- **Self
+00000ff0: 2064 6f63 756d 656e 7465 642a 2a20 6279   documented** by
+00001000: 205b 646f 6373 7472 696e 6773 5d28 6874   [docstrings](ht
+00001010: 7470 733a 2f2f 7661 6e64 6562 726f 6e2e  tps://vandebron.
+00001020: 6769 7468 7562 2e69 6f2f 6d70 796c 2920  github.io/mpyl) 
+00001030: 696e 2074 6865 2063 6f64 652c 2064 6573  in the code, des
+00001040: 6372 6970 7469 6f6e 7320 696e 2074 6865  criptions in the
+00001050: 2073 6368 656d 6173 0a20 2061 6e64 2065   schemas.  and e
+00001060: 7870 6c61 6e61 7469 6f6e 7320 696e 2074  xplanations in t
+00001070: 6865 2043 4c49 2e0a 2d20 2a2a 5079 7468  he CLI..- **Pyth
+00001080: 6f6e 2061 7320 5941 4d4c 2074 656d 706c  on as YAML templ
+00001090: 6174 696e 6720 656e 6769 6e65 2a2a 2041  ating engine** A
+000010a0: 7474 656d 7074 7320 746f 206d 6978 206d  ttempts to mix m
+000010b0: 6172 6b75 7020 616e 6420 6c6f 6769 6320  arkup and logic 
+000010c0: 7465 6e64 2074 6f20 6861 7665 2061 0a20  tend to have a. 
+000010d0: 205b 776f 7273 7420 6f66 2062 6f74 6820   [worst of both 
+000010e0: 776f 726c 6473 5d28 6874 7470 733a 2f2f  worlds](https://
+000010f0: 616e 7468 6f6e 7968 6177 6b69 6e73 2e6d  anthonyhawkins.m
+00001100: 6564 6975 6d2e 636f 6d2f 6973 2d70 7974  edium.com/is-pyt
+00001110: 686f 6e2d 7468 652d 7065 7266 6563 742d  hon-the-perfect-
+00001120: 6a73 6f6e 2d79 616d 6c2d 7465 6d70 6c61  json-yaml-templa
+00001130: 7469 6e67 2d65 6e67 696e 652d 6335 6331  ting-engine-c5c1
+00001140: 6233 3234 3138 6636 290a 2020 6f75 7463  b32418f6).  outc
+00001150: 6f6d 652e 204d 5079 4c20 7573 6573 2060  ome. MPyL uses `
+00001160: 5941 4d4c 6020 7374 7269 6374 6c79 2066  YAML` strictly f
+00001170: 6f72 2063 6f6e 6669 6775 7261 7469 6f6e  or configuration
+00001180: 2e20 5768 6572 6520 6059 414d 4c60 206e  . Where `YAML` n
+00001190: 6565 6473 2074 6f20 7072 6f64 7563 6564  eeds to produced
+000011a0: 2064 796e 616d 6963 616c 6c79 2c20 6c69   dynamically, li
+000011b0: 6b65 2066 6f72 2043 5244 7320 7669 610a  ke for CRDs via.
+000011c0: 2020 4845 4c4d 2063 6861 7274 732c 2069    HELM charts, i
+000011d0: 7420 6973 2067 656e 6572 6174 6564 2062  t is generated b
+000011e0: 7920 5079 7468 6f6e 2063 6f64 652e 2054  y Python code. T
+000011f0: 6520 7072 6f64 7563 6564 2060 5941 4d4c  e produced `YAML
+00001200: 6020 6973 2076 616c 6964 6174 6564 2061  ` is validated a
+00001210: 6761 696e 7374 2074 6865 2063 6f72 7265  gainst the corre
+00001220: 7370 6f6e 6469 6e67 2073 6368 656d 6173  sponding schemas
+00001230: 2e0a 2d20 2a2a 4578 7465 6e73 6962 6c65  ..- **Extensible
+00001240: 2a2a 2053 7570 706f 7274 2066 6f72 2074  ** Support for t
+00001250: 6865 206d 6f73 7420 636f 6d6d 6f6e 2075  he most common u
+00001260: 7365 2063 6173 6573 2028 652e 672e 2044  se cases (e.g. D
+00001270: 6f63 6b65 722c 2048 656c 6d2c 204b 7562  ocker, Helm, Kub
+00001280: 6572 6e65 7465 732c 2041 5753 2c20 6574  ernetes, AWS, et
+00001290: 632e 2920 6973 2062 7569 6c74 2d69 6e2e  c.) is built-in.
+000012a0: 0a20 2042 7574 2069 7420 6973 2065 6173  .  But it is eas
+000012b0: 7920 746f 2065 7874 656e 6420 7769 7468  y to extend with
+000012c0: 2079 6f75 7220 6f77 6e20 606d 7079 6c2e   your own `mpyl.
+000012d0: 7374 6570 7360 2e0a 0a23 2320 f09f 92bb  steps`...## ....
+000012e0: 2054 6563 686e 6f6c 6f67 6965 730a 0a23   Technologies..#
+000012f0: 2323 2052 6571 7569 7265 6d65 6e74 730a  ## Requirements.
+00001300: 5468 6520 666f 6c6c 6f77 696e 6720 7465  The following te
+00001310: 6368 6e6f 6c6f 6769 6573 2061 7265 2065  chnologies are e
+00001320: 7870 6563 7465 6420 746f 2062 6520 7072  xpected to be pr
+00001330: 6573 656e 7420 6f6e 2074 6865 206c 6f63  esent on the loc
+00001340: 616c 204f 533a 0a2d 205b 5079 7468 6f6e  al OS:.- [Python
+00001350: 5d28 6874 7470 733a 2f2f 7777 772e 7079  ](https://www.py
+00001360: 7468 6f6e 2e6f 7267 2f29 203e 3d20 332e  thon.org/) >= 3.
+00001370: 390a 2d20 5b50 6970 5d28 6874 7470 733a  9.- [Pip](https:
+00001380: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
+00001390: 6374 2f70 6970 2f29 203e 3d20 3233 2e30  ct/pip/) >= 23.0
+000013a0: 2e31 0a2d 205b 446f 636b 6572 5d28 6874  .1.- [Docker](ht
+000013b0: 7470 733a 2f2f 7777 772e 646f 636b 6572  tps://www.docker
+000013c0: 2e63 6f6d 2f29 203e 2032 300a 2d20 5b44  .com/) > 20.- [D
+000013d0: 6f63 6b65 7220 636f 6d70 6f73 655d 2868  ocker compose](h
+000013e0: 7474 7073 3a2f 2f64 6f63 732e 646f 636b  ttps://docs.dock
+000013f0: 6572 2e63 6f6d 2f63 6f6d 706f 7365 2f69  er.com/compose/i
+00001400: 6e73 7461 6c6c 2f6c 696e 7578 2f29 0a20  nstall/linux/). 
+00001410: 2069 6e73 7461 6c6c 6564 2061 7320 706c   installed as pl
+00001420: 7567 696e 2028 6064 6f63 6b65 7220 636f  ugin (`docker co
+00001430: 6d70 6f73 6520 7665 7273 696f 6e60 2920  mpose version`) 
+00001440: 3e3d 2076 322e 322e 330a 2d20 5b47 6974  >= v2.2.3.- [Git
+00001450: 5d28 6874 7470 733a 2f2f 6769 742d 7363  ](https://git-sc
+00001460: 6d2e 636f 6d2f 2920 5343 4d0a 0a23 2323  m.com/) SCM..###
+00001470: 2042 756e 646c 6564 0a4d 5079 4c20 6973   Bundled.MPyL is
+00001480: 2065 7874 656e 7369 626c 6520 616e 6420   extensible and 
+00001490: 6861 7320 6120 6d69 6e69 6d61 6c20 666f  has a minimal fo
+000014a0: 6f74 7072 696e 742e 2048 6176 696e 6720  otprint. Having 
+000014b0: 7361 6964 2074 6861 742c 2062 6174 7465  said that, batte
+000014c0: 7269 6573 2066 6f72 2074 6865 2066 6f6c  ries for the fol
+000014d0: 6c6f 7769 6e67 2074 6563 686e 6f6c 6f67  lowing technolog
+000014e0: 6965 7320 6172 6520 696e 636c 7564 6564  ies are included
+000014f0: 2e0a 0a23 2323 2323 2043 492f 4344 0a23  ...##### CI/CD.#
+00001500: 2323 2323 2320 4275 696c 640a 2d20 5b44  ##### Build.- [D
+00001510: 6f63 6b65 725d 2868 7474 7073 3a2f 2f77  ocker](https://w
+00001520: 7777 2e64 6f63 6b65 722e 636f 6d2f 2920  ww.docker.com/) 
+00001530: 606d 7079 6c2e 7374 6570 732e 6275 696c  `mpyl.steps.buil
+00001540: 642e 646f 636b 6572 6275 696c 6460 0a2d  d.dockerbuild`.-
+00001550: 205b 5363 616c 6120 2853 4254 295d 2868   [Scala (SBT)](h
+00001560: 7474 7073 3a2f 2f77 7777 2e73 6361 6c61  ttps://www.scala
+00001570: 2d73 6274 2e6f 7267 2f29 2060 6d70 796c  -sbt.org/) `mpyl
+00001580: 2e73 7465 7073 2e62 7569 6c64 2e73 6274  .steps.build.sbt
+00001590: 600a 2d20 5b4a 656e 6b69 6e73 5d28 6874  `.- [Jenkins](ht
+000015a0: 7470 733a 2f2f 7777 772e 6a65 6e6b 696e  tps://www.jenkin
+000015b0: 732e 696f 2f29 2020 606d 7079 6c2e 636c  s.io/)  `mpyl.cl
+000015c0: 692e 636f 6d6d 616e 6473 2e62 7569 6c64  i.commands.build
+000015d0: 2e6a 656e 6b69 6e73 6020 616e 640a 2020  .jenkins` and.  
+000015e0: 606d 7079 6c2e 7574 696c 6974 6965 732e  `mpyl.utilities.
+000015f0: 6a65 6e6b 696e 732e 7275 6e6e 6572 2e4a  jenkins.runner.J
+00001600: 656e 6b69 6e73 5275 6e6e 6572 600a 0a23  enkinsRunner`..#
+00001610: 2323 2323 2320 5465 7374 696e 670a 2d20  ##### Testing.- 
+00001620: 5b4a 756e 6974 5d28 6874 7470 733a 2f2f  [Junit](https://
+00001630: 6a75 6e69 742e 6f72 672f 2920 606d 7079  junit.org/) `mpy
+00001640: 6c2e 7374 6570 732e 6d6f 6465 6c73 2e41  l.steps.models.A
+00001650: 7274 6966 6163 7454 7970 652e 4a55 4e49  rtifactType.JUNI
+00001660: 545f 5445 5354 5360 0a0a 2323 2323 2323  T_TESTS`..######
+00001670: 2044 6570 6c6f 796d 656e 740a 2d20 5b4b   Deployment.- [K
+00001680: 3853 5d28 6874 7470 733a 2f2f 6b75 6265  8S](https://kube
+00001690: 726e 6574 6573 2e69 6f2f 2920 606d 7079  rnetes.io/) `mpy
+000016a0: 6c2e 7374 6570 732e 6465 706c 6f79 2e6b  l.steps.deploy.k
+000016b0: 7562 6572 6e65 7465 7360 0a2d 205b 4865  ubernetes`.- [He
+000016c0: 6c6d 5d28 6874 7470 733a 2f2f 6865 6c6d  lm](https://helm
+000016d0: 2e73 682f 2920 606d 7079 6c2e 7374 6570  .sh/) `mpyl.step
+000016e0: 732e 6465 706c 6f79 2e6b 3873 2e68 656c  s.deploy.k8s.hel
+000016f0: 6d60 0a0a 2323 2323 2320 5265 706f 7274  m`..##### Report
+00001700: 696e 670a 2d20 5b4a 6972 615d 2868 7474  ing.- [Jira](htt
+00001710: 7073 3a2f 2f77 7777 2e61 746c 6173 7369  ps://www.atlassi
+00001720: 616e 2e63 6f6d 2920 606d 7079 6c2e 7265  an.com) `mpyl.re
+00001730: 706f 7274 696e 672e 7461 7267 6574 732e  porting.targets.
+00001740: 6a69 7261 600a 2d20 5b47 6974 6875 625d  jira`.- [Github]
+00001750: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00001760: 636f 6d2f 2920 606d 7079 6c2e 7265 706f  com/) `mpyl.repo
+00001770: 7274 696e 672e 7461 7267 6574 732e 6769  rting.targets.gi
+00001780: 7468 7562 600a 2d20 5b53 6c61 636b 5d28  thub`.- [Slack](
+00001790: 6874 7470 733a 2f2f 736c 6163 6b2e 636f  https://slack.co
+000017a0: 6d2f 2920 606d 7079 6c2e 7265 706f 7274  m/) `mpyl.report
+000017b0: 696e 672e 7461 7267 6574 732e 736c 6163  ing.targets.slac
+000017c0: 6b60 0a                                  k`.
```

## Comparing `mpyl-1.0.6.dist-info/RECORD` & `mpyl-1.0.7.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,88 +1,89 @@
-mpyl/__init__.py,sha256=sLR4OPN49X7SpQiYro_GrizAvJo_CI7nXiZh662D7OE,766
-mpyl/__main__.py,sha256=S7WS_61OT3kRc5RJq3vz4AI6N4YRU5h2KG1kBeQKK6I,215
-mpyl/constants.py,sha256=mr9QfGfl56MCHthSyWkFQfDTHrxMuxLW-1xy6TtHKKQ,162
-mpyl/project.py,sha256=91aqusKKQUnB29kem8cxs7GVuqyCgEAAC2YkSLqLYW4,13526
-mpyl/validation.py,sha256=EMbkceP3w805916gdoKqGeD1SPONu3FEb2cJld5V05E,1708
-mpyl/cli/__init__.py,sha256=3sN-_zD8pS3JdHh49qC77aFdwIGTXEV2nGxZbc5Ijx8,2163
-mpyl/cli/build.py,sha256=UWttK-sNbY3tU7HYl763005yTMjcd_mN_FhvlhRT_1Q,10619
-mpyl/cli/health.py,sha256=ny37_DVoqXp8IxGQt9KeBZdrbvtd2WGxXtANXPDiENo,341
-mpyl/cli/meta_info.py,sha256=MJhWR8GxSL1Anx7Cs_6c0QU6_tYP_pNxaazGV8JoO60,2170
-mpyl/cli/projects.py,sha256=m6AYs8cn-TGTgobktzKd2MW7xj9D8Sm5GEkMXYVj1vA,3915
+mpyl/__init__.py,sha256=0A89yKV9DB7xfO0JBHPL_oBVPvLIIkMvUqmzkjtFVt4,766
+mpyl/__main__.py,sha256=2c9boQJDUA6b8p2umOych7HHlwmBdmsIQDLZcE_pBdo,215
+mpyl/constants.py,sha256=QjtU24q52cowD4mLr54Xa0XeclFZ_Bx-7BV7GzpUhyg,162
+mpyl/project.py,sha256=KZGpjTTiu7QiPiv1yCLRJrH-LW_X5INWwcaKv_XwQEE,13948
+mpyl/validation.py,sha256=kcYjYZQx2UmeMRf_OXCrO5tkzrV6SlIDkFbSx5oBPHs,1710
+mpyl/cli/__init__.py,sha256=6J4nIg4-Zo2OCrMBZE-RzLyS7v81G3HtWXpX5Cx0quI,2789
+mpyl/cli/build.py,sha256=Byp-Nq2hVxvM_MszwliznGSqReL2My48MqLy5jFUGe4,11043
+mpyl/cli/health.py,sha256=2MMSEcw8ehtOWQYh1XnNMbJjOqnyKA7DZqH3a-9CdCM,341
+mpyl/cli/meta_info.py,sha256=TWSjF-wk4Strn8xaSgULUUhKBETuSvzQDuunex5FbJE,2170
+mpyl/cli/projects.py,sha256=Mp3CXic59ifTCiIVAevgwPPUMwASsWRFh6USff1EHfI,3853
 mpyl/cli/commands/__init__.py,sha256=DaL5q4ibFJT7EMlgcQBSpAaaQNiBqnSJZ2WIKtPzLJk,34
 mpyl/cli/commands/build/__init__.py,sha256=Ox0F68re6bNGLBC4KEBLmXXSRf5OIJZ8N2Vens3rgEk,439
 mpyl/cli/commands/build/jenkins.py,sha256=GYXj4N0GLIm23Lx8hTIEhlGTxgUhyhYVnnhLD1LCfXQ,3923
-mpyl/cli/commands/build/mpyl.py,sha256=S03ZF4XamZAIgxm81xYXu7Pwwnhk7-ManCaa_bizTVc,5814
+mpyl/cli/commands/build/mpyl.py,sha256=Zyu_nPYpQR4GrprwmOExACTSvC2cZJIl-UfvpMUuUic,5901
 mpyl/cli/commands/health/__init__.py,sha256=Bx6QcWIN-EadbpSe1XAXs1aYCD7Ad8_t3lWRlGDsIr0,38
-mpyl/cli/commands/health/checks.py,sha256=-GEUCE8Jrj-rhOv5hKEPQsNtB_TGqmsKVA59ysw8CqQ,5200
+mpyl/cli/commands/health/checks.py,sha256=rhRKiJrO1vTKojnH04HqW4r3uPIc2wkiFYnw-W7M6Uw,5535
 mpyl/cli/commands/projects/__init__.py,sha256=YoVobAUCYwqc23p-iAuQnpJQYpdri5ljtj8l_XKYOr0,46
-mpyl/cli/commands/projects/formatting.py,sha256=bhoLOUunClIPmSM6eZzJqHgTsdy6fidtz455IlV4xEU,1039
+mpyl/cli/commands/projects/formatting.py,sha256=qpKokiaZdZ2ZezXuGy3Q3e3Fq9DKMq7gvruE779l9TA,1061
 mpyl/projects/__init__.py,sha256=31HPF5jDZK5UkQT8Zw0V0QSJLqzp8f2zFiWd-QkDjRE,620
-mpyl/projects/find.py,sha256=iUA1_8Tz3tZs-GvEQyvru3g9o3erSt5yxCHXLm96h4k,1993
+mpyl/projects/find.py,sha256=qAaYA1V2tNXAM_tq1-HwQV4fvCdwyPGa5InY0RZetm4,2202
 mpyl/reporting/__init__.py,sha256=vRvt_67opWXCfe_zYZChT-YhjoPOahAjLagoaVzOcFM,92
 mpyl/reporting/formatting/__init__.py,sha256=GAvYJpHT2SMQxjiLCSqFy57PNWsGI_Ow2bFnA8cX08k,76
-mpyl/reporting/formatting/markdown.py,sha256=PGPbgYMcr9xEmKQZWc_QUbNjl_lQ1yaRydSLbr2-3FE,4909
-mpyl/reporting/formatting/text.py,sha256=zgRnXSvnwi69mCbAsmcJgiU0PITe9uD8cBgPat4l6t8,1413
-mpyl/reporting/targets/__init__.py,sha256=ePSvaZMALkukb0ovhKRGkyIcwavI_VZi7GUeRuLMeEo,1096
-mpyl/reporting/targets/github.py,sha256=en1ph8y_cVh4jaDeoZLsTPngZW6oxWu4DM6v2Md3p3g,7939
-mpyl/reporting/targets/jira.py,sha256=cc6ndmj3F1w7Y9wZTycMrlz_nCZXurq9aT7u5bCeCMU,9004
-mpyl/reporting/targets/slack.py,sha256=vzMlhHCN1Ldbv6Ssg6SZt2cF5s14H4NNeKkyZZadrqg,7366
+mpyl/reporting/formatting/markdown.py,sha256=dSArxUA0qiN6MzFlqSzIGcjDGY2iFhlZNXMuRwAGwDQ,5213
+mpyl/reporting/formatting/text.py,sha256=oihlYM4XVEjzYz5wq8uUViTypcR4yZ-Aw_ujnr396fE,1411
+mpyl/reporting/targets/__init__.py,sha256=31UWFweqJqvlE3WZBb2CMBIAnmJJRZpVBwpW-ma4MzA,1139
+mpyl/reporting/targets/github.py,sha256=J9lYoib_tLDPgQslzBgeYymk78g4yLMFWDLdlMSyMFs,8453
+mpyl/reporting/targets/jira.py,sha256=8D4LPBhIdYiH_oTgSd7d3nNjnacGEn2Qf4AC7RiFGJU,9331
+mpyl/reporting/targets/slack.py,sha256=gTD8MNNJchCFPwK4k0Rs7eNkUzpyKjnkjB6DwKRmu2I,7997
 mpyl/schema/mpyl_config.schema.yml,sha256=f7j-04KI0Im1CoOZZ-Dale-Sw4RSnX0fdzsJ72FGKU8,8433
 mpyl/schema/project.schema.yml,sha256=Pn31oWBvupNXOVuUwykJv-P7C28eoELz5YwCJcKnntI,25500
-mpyl/schema/run_properties.schema.yml,sha256=A5T0m0_6JQ2D6yPHA6GyNNOggID9iWSnwWcfWCG6Fwk,2787
+mpyl/schema/run_properties.schema.yml,sha256=mIPDvvwi_u3cQZW0FShFY1ZMdqT9AcCwg9Y3MA0xsSw,2914
 mpyl/stages/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mpyl/stages/discovery.py,sha256=5u0QHC9RNjcu855Y0DqGKq2XP_1n42_H4sV-v0MDaqU,3506
-mpyl/steps/__init__.py,sha256=jpcKUPNLQm_8LngC7mbwYUzaoiisgyJy4R8u0qOkmAU,6135
-mpyl/steps/models.py,sha256=5IVLMwPf5AjRgod6W6ATWjMpNcSNACqtq-g92LnBs7k,5977
-mpyl/steps/run.py,sha256=ZzyljvUxkD6Qrwd9QXAFqXLxVFwyf7ZKUcZECkvbB6U,3429
-mpyl/steps/steps.py,sha256=QkT8S600vhPf9QQ_N2vq-iYjBE3__I55cckS1kZl6I4,8405
+mpyl/stages/discovery.py,sha256=HCiWshRKL9Rtgu-HzdR5U5St4hYOlCwFul3CASFcTE0,3698
+mpyl/steps/__init__.py,sha256=utJ4jkk9PP27FVsjDz7awvKAUJdII5GMT5SUM8tAwbw,6437
+mpyl/steps/collection.py,sha256=4VBv34RR261w7aGRFiyq9gkMuqRrDCctnD96wFMTvpM,1442
+mpyl/steps/models.py,sha256=VEeQ_XTC2aC1u_hXthFC1Y-HSR8ndS8NBltEO9pD-ZI,6085
+mpyl/steps/run.py,sha256=kp1Qm3WM3FoIpXTwQ3ddlptyQ_kvC6gtP90-eIW39mc,3505
+mpyl/steps/steps.py,sha256=mUEhy78h3KFXfd5s0DBO3nXIbwcXhlXkR5Cya10wlbU,7278
 mpyl/steps/build/__init__.py,sha256=EyPUNNDMQfJK-RVjYM9WvPhEDITbu2n4fx9mxhGLlDs,59
 mpyl/steps/build/docker_after_build.py,sha256=nok2HRrH66e9FBvfwEKnalJhX3io__PQZaq_fR0S8BI,2093
 mpyl/steps/build/dockerbuild.py,sha256=6lqVqiuGYk8ISuzTterTFdcIWqUkvSOUCOCDmjHkM2s,2865
-mpyl/steps/build/echo.py,sha256=on6n-zYs55z6_CouMrSTRIV_JDSTVdQ53raTt3im1qU,765
+mpyl/steps/build/echo.py,sha256=EwOHLpyD--1joICl7kNnh6p_JfguCSQX4WirA_5BNn8,996
 mpyl/steps/build/sbt.py,sha256=rvJzIVgsx6KrX5HW_jqEhu6yV2QAttEXQRJ3A7XJJ-k,2402
 mpyl/steps/deploy/__init__.py,sha256=14PYgOvt7YEO2Zw4kEeZxWUNBR7Lz91nSoJZpvJHqzE,60
-mpyl/steps/deploy/cloudfront_kubernetes_deploy.py,sha256=4rE6n_Vh3QAl8QyA3Gv1elMcP3amrOUMkGbhVYfGCsU,2496
-mpyl/steps/deploy/echo.py,sha256=f43TQmiY96Da_OLZcjkQx-RjCvlo09Dclpezv9RoMlo,1001
-mpyl/steps/deploy/ephemeral_docker_deploy.py,sha256=NySUtyGl7xOjsgDK48AxorVik_iljcifWcRhJZADFs8,1310
-mpyl/steps/deploy/kubernetes.py,sha256=UAUqQ9EcsT87RNH014TBnx7shcgqsvxP3e__RitC8eA,3415
-mpyl/steps/deploy/kubernetes_job.py,sha256=ME3O5PEnNGDdJHDp-iIWp5i1nFxgOyo7QMn2Axjec1U,1412
-mpyl/steps/deploy/kubernetes_spark_job.py,sha256=XHE_PrEMHGfualvdApAZJr7h0qwPDV9e5Lq2UCZSVDA,1380
-mpyl/steps/deploy/k8s/__init__.py,sha256=JcPfCITgl6JrHb-Enxe2dR1bk8mQ-SD2pIrKsjD80a8,3390
-mpyl/steps/deploy/k8s/chart.py,sha256=uTklf6xJRS1NCSlF_Z6uq2csw3fLlWWSCND07fKpV0Y,18819
-mpyl/steps/deploy/k8s/helm.py,sha256=0ZAMhuTMYyPDHfaUVNJDci3pZtGc3jyOXCaauznJf5U,2856
-mpyl/steps/deploy/k8s/rancher.py,sha256=TNxEcniLqvNif0ymqW2QvY1XPBiKXeh5o12EMNxTx-Y,1685
-mpyl/steps/deploy/k8s/resources/__init__.py,sha256=eSHp1ERR8FPPujHDiyLp8SchAza6TicPgx96zvSq4uQ,4467
-mpyl/steps/deploy/k8s/resources/sealed_secret.py,sha256=4q1POq2Z35putRlQ6cNWDBoTtRbFDDI2rr7JElCIzbM,591
-mpyl/steps/deploy/k8s/resources/spark.py,sha256=GT2lb66Xejb9uSdGE77ItaFBHh1K0IpJDX95RVHUxKQ,6143
-mpyl/steps/deploy/k8s/resources/traefik.py,sha256=uI8xE1KjywZ84OktNMPAB58JIu7tN4OT2V3iZO8tI7o,1948
+mpyl/steps/deploy/cloudfront_kubernetes_deploy.py,sha256=Fcq2555DwX2dUrBcuqLCb5-2lJ_PGqYkiP-NJwglvGY,2767
+mpyl/steps/deploy/echo.py,sha256=pB63Cox_7Bn0wbhlP5Aj9dGh1E8aUGY7pv0HDdIOqao,1196
+mpyl/steps/deploy/ephemeral_docker_deploy.py,sha256=3YUqRWlFD3YVlNR8s5Shfa1KTdQg8vsWZ_omdMY_8b4,1472
+mpyl/steps/deploy/kubernetes.py,sha256=-VjRR5Hk_3MH5xQX7CTbvWpBkT-WbFJX1kECTcy1WP8,3896
+mpyl/steps/deploy/kubernetes_job.py,sha256=tFhY8RASKQ6OSEbxQgMYbcd9--83ibyPNivKxOfbFpY,1588
+mpyl/steps/deploy/kubernetes_spark_job.py,sha256=deKKaX-Ktrll47d_h-Pw1nda-5DfT96LupvWdKdLPSI,1571
+mpyl/steps/deploy/k8s/__init__.py,sha256=VRGBw1VFGB06UVYnMUk_ObK67GOfVx7EhVCO0LpYwfM,3518
+mpyl/steps/deploy/k8s/chart.py,sha256=Lfi30_1s5dshqvZkSlabp3xJpXPpTXj-Ebl6nUmdZKY,20536
+mpyl/steps/deploy/k8s/helm.py,sha256=GHDQjdsFuL54l__gP47REVJWZPr9Acbh20b75fQsEEI,2989
+mpyl/steps/deploy/k8s/rancher.py,sha256=m40g7kGc-09OML4NMtOpnrM8mkZxSIJzx24gc4GqUfk,1732
+mpyl/steps/deploy/k8s/resources/__init__.py,sha256=c2ZTt4SwsExUnF1Bu1N1kjxDNd6zTsYGX2G5btTMdNE,4719
+mpyl/steps/deploy/k8s/resources/sealed_secret.py,sha256=af8zae2HVCnT51aEq_3kKVHp86gf8UpzDWM87jSQoJ4,616
+mpyl/steps/deploy/k8s/resources/spark.py,sha256=GQUHogCmFl3GHAg54pyFlv1bAZAtk68c5vzRQwaWLDk,5850
+mpyl/steps/deploy/k8s/resources/traefik.py,sha256=COJ9ekK8EKtbABE2IWRRIfKCIbOl8DC9Tr_NAuUblCk,2287
 mpyl/steps/deploy/k8s/resources/schema/sparkoperator.k8s.io_scheduledsparkapplications.schema.yml,sha256=jTo3LZklRCZ1L7JZbUdcmhDWhk3VDJhrDz_OTHNUm58,168371
 mpyl/steps/deploy/k8s/resources/schema/sparkoperator.k8s.io_sparkapplications.schema.yml,sha256=s1rMobinpB3aXI1ONcuTMGLMIRRQ_qZrZtQTYZHcDFU,151469
 mpyl/steps/deploy/k8s/resources/schema/traefik.ingress.schema.yml,sha256=3Oc1awM23acMS36kqpbfqwx6D8Sft4FnL8abNLgcwBI,11703
 mpyl/steps/deploy/k8s/resources/schema/traefik.middleware.schema.yml,sha256=6QCi1F9LJ3cgmwaPBV8dWFvbXb2B5huKvfp4Pa1hoBw,42950
 mpyl/steps/postdeploy/__init__.py,sha256=cUDlHPzcW5zGGPxr9T77pATS5lwKnP9Ge8JroAGSvBg,64
-mpyl/steps/postdeploy/cypress_test.py,sha256=qVTaWKfUiL7ui3WLGa1hngD701mDXfEUMKTdMV8m4wU,6004
+mpyl/steps/postdeploy/cypress_test.py,sha256=aZ_fmMsqq7eEsz4GzFS-DTEcdSl0rgOhPC4KLyYmlCA,6496
 mpyl/steps/test/__init__.py,sha256=XL1gSbIMJYSFcy4Vf8YRbZM9yAs3Fzvq2tfX9xTDZX8,58
-mpyl/steps/test/after_test.py,sha256=bKTBVFm88s4Kzr6JypxLAbKTlbRsha7gff3RjSr3ip0,1428
-mpyl/steps/test/before_test.py,sha256=IOUvAa3lKox8IKS28aGmmWJMNWcQWv9yGnTydVBvM14,2453
-mpyl/steps/test/dockertest.py,sha256=upna6Q5tHkyZUpclaeYe7H7Y02JlMVvo2xxWWPlrdMg,3609
-mpyl/steps/test/echo.py,sha256=ShYQNzlCrhU10UKQSbmWm-GPZ9hEt6wE31bDfgxsBRU,1789
-mpyl/steps/test/sbt.py,sha256=4_tZrgyzBoCNWm6sV6XPM7qbUrlx50vVT-qv9UJP-ac,5013
+mpyl/steps/test/after_test.py,sha256=TVRsdWxVRNagi5Ajqa1caP9EySnBmoSJP_j1in7GA30,1560
+mpyl/steps/test/before_test.py,sha256=agBmlSSoHJyK2truhSaVb_0K2trYeIAamDwxQ1ZLh50,2596
+mpyl/steps/test/dockertest.py,sha256=4ESQDmWflOKapVZux7VYDpjlCqv7QXmehFdiJaL39to,3886
+mpyl/steps/test/echo.py,sha256=5xfmhn7xbPCHQ7H_X49idHDv-FZK556kqFRqsUktJnI,1929
+mpyl/steps/test/sbt.py,sha256=26pkmwOvJRegrBRr6KzT3wHbuY-yFIqJ99FQEwCDiac,5075
 mpyl/utilities/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mpyl/utilities/cypress/__init__.py,sha256=cKSYzS1CfQgIClUX7Sj8EF5YlJ-34uck6rjyMJsBkFc,749
-mpyl/utilities/docker/__init__.py,sha256=djMUvAeU2AUV6bRj13yLsuChoKW4L2DnAULzAfotO5o,6470
-mpyl/utilities/github/__init__.py,sha256=EnkcxQ5UQ08ZZOfShr3LFodu4pmzED9wMoHakIRbYO4,1739
-mpyl/utilities/jenkins/__init__.py,sha256=sX-ZO6NnG0i0LOo_0AMdVMmOluG1zUFxwuHip31TDLE,1533
-mpyl/utilities/jenkins/runner.py,sha256=BnndcXKTlwLXFja3nGa_81Jx5frbnMenr0aBVoNdLgU,7627
-mpyl/utilities/junit/__init__.py,sha256=zxWSjvglZJPQPxCSB9TtX-Gaw5i8M0f-IzM3DQQczRY,1382
+mpyl/utilities/cypress/__init__.py,sha256=-31jEaaANvamp7AjocY4D68esOWCxA6rIaz2j8-MOos,768
+mpyl/utilities/docker/__init__.py,sha256=7vk98Y8Obc6UOSq_4qAWSVpa_j7uyuGrF46AiMwZANI,6693
+mpyl/utilities/github/__init__.py,sha256=IPvxPLObUcqwVsWq46Yp6C6MNYFYALtxYTW6gu4F6II,1781
+mpyl/utilities/jenkins/__init__.py,sha256=850w2rxbeSGmYieBQ5VHuSM3pV6FG9Vbdf41Lwpi0_g,1551
+mpyl/utilities/jenkins/runner.py,sha256=ObgHVxZRxiFXUD6v-O55IH7Oh7GpKXqXKSxhg3RCF74,7903
+mpyl/utilities/junit/__init__.py,sha256=lybqA7y8gmOg7HFKdqZYdUf80Z-fCix-yhbjG8OKM4U,1431
 mpyl/utilities/logging/__init__.py,sha256=dlVErHdOt6YQ9LV91_7e1-XMTa4fagC-xl-GROppD5c,254
-mpyl/utilities/pyaml_env/__init__.py,sha256=vrWacRoipXG4SEVOG6ECvp1JwaukhHJhL3xKxVc1mKg,847
-mpyl/utilities/repo/__init__.py,sha256=YGPBcXNARtRWdwG2U01x2lfhlEalTHStpTvcB4OGFVM,6568
-mpyl/utilities/s3/__init__.py,sha256=u7NBYcHgXBeSSsqGSFVQs3FLvK-3M4wPC2-Vsc0AQz8,4622
-mpyl/utilities/sbt/__init__.py,sha256=FQOMPPgmiU7HMgMoioM5T0fSk0LwGti-k8l3f75Cuqw,1551
-mpyl/utilities/subprocess/__init__.py,sha256=_NehZ65pzu_qxsQQ_Q9t_-zX-FBGeiiaNsjuuPJsgVc,2110
-mpyl-1.0.6.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-mpyl-1.0.6.dist-info/METADATA,sha256=9emFgyRk_z3arF92XB4tMroDze6YErwk6_nGNWS4mtA,5945
-mpyl-1.0.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-mpyl-1.0.6.dist-info/entry_points.txt,sha256=Jf4zjGLsiokFbaQ2dfX9AC5Bu3kp7zxrBOAzErmAYs8,35
-mpyl-1.0.6.dist-info/top_level.txt,sha256=xVSrrk0ECDxKYaW8mAyGy02yY8KhKlUSyzHaq9UDVNs,5
-mpyl-1.0.6.dist-info/RECORD,,
+mpyl/utilities/pyaml_env/__init__.py,sha256=Wa-KUCJy8hTFOAYXiZcOKo3_EXmnyD9AzeUuDqeLw24,880
+mpyl/utilities/repo/__init__.py,sha256=dGe6c4hATQqGQkpig7bn9iWkoknLEbBdsjdjDdaSJrQ,7098
+mpyl/utilities/s3/__init__.py,sha256=Czr2nAMwU9eCqEvymGecNhxnYLwYSdHz9Yw13FwPY-A,4764
+mpyl/utilities/sbt/__init__.py,sha256=nM8iUUL92luMGoMQUPnJm2tJkAta0ct601dMj0oFDsg,1612
+mpyl/utilities/subprocess/__init__.py,sha256=KYzwKeOh-myUE2VSEL7NWVpiz-WsoTwRIgU8Y03Fo5I,2326
+mpyl-1.0.7.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+mpyl-1.0.7.dist-info/METADATA,sha256=_GkVO_9gSq4wvvwK0Y6XIoiXuYGpHUI_7boN6HmGejo,6083
+mpyl-1.0.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+mpyl-1.0.7.dist-info/entry_points.txt,sha256=Jf4zjGLsiokFbaQ2dfX9AC5Bu3kp7zxrBOAzErmAYs8,35
+mpyl-1.0.7.dist-info/top_level.txt,sha256=xVSrrk0ECDxKYaW8mAyGy02yY8KhKlUSyzHaq9UDVNs,5
+mpyl-1.0.7.dist-info/RECORD,,
```

