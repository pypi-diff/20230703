# Comparing `tmp/orchestrator_core-1.1.1rc4.tar.gz` & `tmp/orchestrator_core-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orchestrator_core-1.1.1rc4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "orchestrator_core-1.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `orchestrator_core-1.1.1rc4.tar` & `orchestrator_core-1.2.0.tar`

### file list

```diff
@@ -1,386 +1,403 @@
--rw-r--r--   0        0        0      342 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/.bumpversion.cfg
--rw-r--r--   0        0        0       33 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/.coveragerc
--rw-r--r--   0        0        0     2620 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/.github/workflows/README.md
--rw-r--r--   0        0        0     1851 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/.github/workflows/build-push-container.yml
--rw-r--r--   0        0        0      291 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/.github/workflows/changelog.yml
--rw-r--r--   0        0        0     2341 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0      371 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/.github/workflows/gh-pages.yml
--rw-r--r--   0        0        0      550 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/.github/workflows/publish-package.yml
--rw-r--r--   0        0        0     1163 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/.github/workflows/run-linting-tests.yml
--rw-r--r--   0        0        0     2113 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/.github/workflows/run-unit-tests.yml
--rw-r--r--   0        0        0     1985 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/.github/workflows/scheduled-build.yml
--rw-r--r--   0        0        0     1809 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/.gitignore
--rw-r--r--   0        0        0     2099 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1150 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/.stignore
--rw-r--r--   0        0        0    29970 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/CHANGELOG.md
--rw-r--r--   0        0        0      333 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/Dockerfile
--rw-r--r--   0        0        0    11409 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/LICENSE
--rw-r--r--   0        0        0      150 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/NOTICE
--rw-r--r--   0        0        0     4965 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/README.md
--rw-r--r--   0        0        0       76 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/codecov.yml
--rw-r--r--   0        0        0       45 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/docs/architecture/application/api.md
--rw-r--r--   0        0        0    16572 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/docs/architecture/application/cli.md
--rw-r--r--   0        0        0    10741 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/docs/architecture/application/domainmodels.md
--rw-r--r--   0        0        0    13931 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/docs/architecture/application/forms.md
--rw-r--r--   0        0        0    48867 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/docs/architecture/application/openapi.json
--rw-r--r--   0        0        0     1565 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/docs/architecture/application/python.md
--rw-r--r--   0        0        0     5585 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/docs/architecture/application/scaling.md
--rw-r--r--   0        0        0     5514 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/docs/architecture/application/tasks.md
--rw-r--r--   0        0        0     2371 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/docs/architecture/application/websockets.md
--rw-r--r--   0        0        0    11465 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/docs/architecture/application/workflow.md
--rw-r--r--   0        0        0        0 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/docs/architecture/orchestration/philosophy.md
--rw-r--r--   0        0        0     2080 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/docs/architecture/tldr.md
--rw-r--r--   0        0        0     1694 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/docs/contributing/guidelines.md
--rw-r--r--   0        0        0    10000 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/docs/contributing/testing.md
--rw-r--r--   0        0        0      452 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/docs/css/custom.css
--rw-r--r--   0        0        0     2165 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/docs/css/termynal.css
--rw-r--r--   0        0        0     2135 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/docs/getting-started/base.md
--rw-r--r--   0        0        0      928 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/docs/getting-started/development.md
--rw-r--r--   0        0        0     2367 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/docs/index.md
--rw-r--r--   0        0        0     3897 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/docs/js/custom.js
--rw-r--r--   0        0        0     9540 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/docs/js/termynal.js
--rw-r--r--   0        0        0     8925 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/docs/workshops/advanced/circuit-workflow.md
--rw-r--r--   0        0        0      254 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/docs/workshops/advanced/database-migration.md
--rw-r--r--   0        0        0     3776 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/docs/workshops/advanced/docker-installation.md
--rw-r--r--   0        0        0     2563 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/docs/workshops/advanced/domain-models.md
--rw-r--r--   0        0        0     4126 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/docs/workshops/advanced/node-workflow.md
--rw-r--r--   0        0        0     3079 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/docs/workshops/advanced/overview.md
--rw-r--r--   0        0        0     1750 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/docs/workshops/advanced/scenario.md
--rw-r--r--   0        0        0     4369 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/docs/workshops/advanced/workflow-introduction.md
--rw-r--r--   0        0        0     5605 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/docs/workshops/beginner/create-user-group.md
--rw-r--r--   0        0        0     4438 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/docs/workshops/beginner/create-user.md
--rw-r--r--   0        0        0     7471 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/docs/workshops/beginner/database-migration.md
--rw-r--r--   0        0        0     3700 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/docs/workshops/beginner/debian.md
--rw-r--r--   0        0        0     3063 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/docs/workshops/beginner/docker.md
--rw-r--r--   0        0        0     6106 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/docs/workshops/beginner/domain-models.md
--rw-r--r--   0        0        0     1952 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/docs/workshops/beginner/explore.md
--rw-r--r--   0        0        0     3996 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/docs/workshops/beginner/input-forms.md
--rw-r--r--   0        0        0     3595 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/docs/workshops/beginner/macos.md
--rw-r--r--   0        0        0     3411 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/docs/workshops/beginner/modify-user-group.md
--rw-r--r--   0        0        0     2143 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/docs/workshops/beginner/modify-user.md
--rw-r--r--   0        0        0     2885 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/docs/workshops/beginner/overview.md
--rw-r--r--   0        0        0     4547 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/docs/workshops/beginner/register-workflows.md
--rw-r--r--   0        0        0      786 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/docs/workshops/beginner/scenario.md
--rw-r--r--   0        0        0     1013 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/docs/workshops/beginner/start-applications.md
--rw-r--r--   0        0        0     2988 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/docs/workshops/beginner/terminate-user-group.md
--rw-r--r--   0        0        0     1332 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/docs/workshops/beginner/terminate-user.md
--rw-r--r--   0        0        0     3637 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/docs/workshops/beginner/workflow-introduction.md
--rw-r--r--   0        0        0    46296 2023-06-27 11:40:53.964177 orchestrator_core-1.1.1rc4/docs/workshops/images/metadata_products.png
--rw-r--r--   0        0        0   983304 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/docs/workshops/images/netbox_devices_active.png
--rw-r--r--   0        0        0      771 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/examples/basic/basic_orchestrator.py
--rw-r--r--   0        0        0     4214 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/mkdocs.yml
--rw-r--r--   0        0        0     1267 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/mutmut_config.py
--rw-r--r--   0        0        0        0 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/.stignore
--rw-r--r--   0        0        0     1098 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/__init__.py
--rw-r--r--   0        0        0      571 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/api/__init__.py
--rw-r--r--   0        0        0      571 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/api/api_v1/__init__.py
--rw-r--r--   0        0        0     2967 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/api/api_v1/api.py
--rw-r--r--   0        0        0      571 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/api/api_v1/endpoints/__init__.py
--rw-r--r--   0        0        0     2841 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/api/api_v1/endpoints/fixed_input.py
--rw-r--r--   0        0        0     1236 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/api/api_v1/endpoints/health.py
--rw-r--r--   0        0        0    12993 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/api/api_v1/endpoints/processes.py
--rw-r--r--   0        0        0     2703 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/api/api_v1/endpoints/product_blocks.py
--rw-r--r--   0        0        0     3331 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/api/api_v1/endpoints/products.py
--rw-r--r--   0        0        0     2552 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/api/api_v1/endpoints/resource_types.py
--rw-r--r--   0        0        0     5803 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/api/api_v1/endpoints/settings.py
--rw-r--r--   0        0        0     2866 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py
--rw-r--r--   0        0        0    11740 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/api/api_v1/endpoints/subscriptions.py
--rw-r--r--   0        0        0      994 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/api/api_v1/endpoints/translations.py
--rw-r--r--   0        0        0     1833 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/api/api_v1/endpoints/user.py
--rw-r--r--   0        0        0     1961 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/api/api_v1/endpoints/workflows.py
--rw-r--r--   0        0        0     1543 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/api/error_handling.py
--rw-r--r--   0        0        0    11705 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/api/helpers.py
--rw-r--r--   0        0        0     5636 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/api/models.py
--rw-r--r--   0        0        0     7681 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/app.py
--rw-r--r--   0        0        0      571 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/cli/__init__.py
--rw-r--r--   0        0        0    13831 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/cli/database.py
--rw-r--r--   0        0        0        0 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/cli/domain_gen_helpers/__init__.py
--rw-r--r--   0        0        0     6853 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py
--rw-r--r--   0        0        0     1953 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/cli/domain_gen_helpers/helpers.py
--rw-r--r--   0        0        0    10653 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/cli/domain_gen_helpers/product_block_helpers.py
--rw-r--r--   0        0        0     9423 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/cli/domain_gen_helpers/product_helpers.py
--rw-r--r--   0        0        0    24095 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py
--rw-r--r--   0        0        0     1439 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/cli/domain_gen_helpers/types.py
--rw-r--r--   0        0        0     2371 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/cli/generate.md
--rw-r--r--   0        0        0     5168 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/cli/generate.py
--rw-r--r--   0        0        0        0 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/cli/generator/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/cli/generator/generator/__init__.py
--rw-r--r--   0        0        0     1758 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/cli/generator/generator/fixed_input.py
--rw-r--r--   0        0        0     2626 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/cli/generator/generator/helpers.py
--rw-r--r--   0        0        0     2607 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/cli/generator/generator/migration.py
--rw-r--r--   0        0        0     2152 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/cli/generator/generator/product.py
--rw-r--r--   0        0        0     5811 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/cli/generator/generator/product_block.py
--rw-r--r--   0        0        0     1400 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/cli/generator/generator/settings.py
--rw-r--r--   0        0        0     1794 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/cli/generator/generator/translations.py
--rw-r--r--   0        0        0     4234 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/cli/generator/generator/unittest.py
--rw-r--r--   0        0        0     1957 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/cli/generator/generator/validations.py
--rw-r--r--   0        0        0     6543 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/cli/generator/generator/workflow.py
--rw-r--r--   0        0        0      779 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/cli/generator/products/workshop/circuit.yaml
--rw-r--r--   0        0        0      557 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/cli/generator/products/workshop/node.yaml
--rw-r--r--   0        0        0      553 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/cli/generator/products/workshop/user.yaml
--rw-r--r--   0        0        0      380 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/cli/generator/products/workshop/user_group.yaml
--rw-r--r--   0        0        0      289 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/cli/generator/templates/constrained_int_definitions.j2
--rw-r--r--   0        0        0     4196 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/cli/generator/templates/create_product.j2
--rw-r--r--   0        0        0      337 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/cli/generator/templates/list_definitions.j2
--rw-r--r--   0        0        0      520 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/cli/generator/templates/macros.j2
--rw-r--r--   0        0        0     4405 2023-06-27 11:40:53.972176 orchestrator_core-1.1.1rc4/orchestrator/cli/generator/templates/modify_product.j2
--rw-r--r--   0        0        0     2639 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/cli/generator/templates/new_product_migration.j2
--rw-r--r--   0        0        0     1675 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/cli/generator/templates/product.j2
--rw-r--r--   0        0        0     2275 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/cli/generator/templates/product_block.j2
--rw-r--r--   0        0        0      514 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/cli/generator/templates/shared_forms.j2
--rw-r--r--   0        0        0     2808 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/cli/generator/templates/terminate_product.j2
--rw-r--r--   0        0        0     1764 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/cli/generator/templates/test_create_workflow.j2
--rw-r--r--   0        0        0     1689 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/cli/generator/templates/test_modify_workflow.j2
--rw-r--r--   0        0        0     1860 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/cli/generator/templates/test_product_type.j2
--rw-r--r--   0        0        0     1518 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/cli/generator/templates/test_terminate_workflow.j2
--rw-r--r--   0        0        0      984 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/cli/generator/templates/test_validate_workflow.j2
--rw-r--r--   0        0        0     2391 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/cli/generator/templates/validate_product.j2
--rw-r--r--   0        0        0      571 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/cli/helpers/__init__.py
--rw-r--r--   0        0        0     1165 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/cli/helpers/input_helpers.py
--rw-r--r--   0        0        0      830 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/cli/helpers/print_helpers.py
--rw-r--r--   0        0        0      983 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/cli/main.py
--rwxr-xr-x   0        0        0    20183 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/cli/migrate_domain_models.py
--rwxr-xr-x   0        0        0     8943 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/cli/migrate_workflows.py
--rw-r--r--   0        0        0     4113 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/cli/migration_helpers.py
--rw-r--r--   0        0        0     1896 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/cli/scheduler.py
--rw-r--r--   0        0        0      571 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/config/__init__.py
--rw-r--r--   0        0        0      770 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/config/assignee.py
--rw-r--r--   0        0        0     2984 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/db/__init__.py
--rw-r--r--   0        0        0    10288 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/db/database.py
--rw-r--r--   0        0        0      303 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/db/filters/__init__.py
--rw-r--r--   0        0        0     3618 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/db/filters/filters.py
--rw-r--r--   0        0        0      774 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/db/filters/generic_filters/__init__.py
--rw-r--r--   0        0        0      992 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/db/filters/generic_filters/bool_filter.py
--rw-r--r--   0        0        0      952 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/db/filters/generic_filters/is_like_filter.py
--rw-r--r--   0        0        0     2542 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/db/filters/generic_filters/range_filter.py
--rw-r--r--   0        0        0      993 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/db/filters/generic_filters/values_in_column_filter.py
--rw-r--r--   0        0        0     3592 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/db/filters/process.py
--rw-r--r--   0        0        0     1251 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/db/filters/product.py
--rw-r--r--   0        0        0     3203 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/db/filters/subscription.py
--rw-r--r--   0        0        0    23630 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/db/models.py
--rw-r--r--   0        0        0      104 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/db/range/__init__.py
--rw-r--r--   0        0        0     1439 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/db/range/range.py
--rw-r--r--   0        0        0      419 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/db/sorting/__init__.py
--rw-r--r--   0        0        0      603 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/db/sorting/process.py
--rw-r--r--   0        0        0      418 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/db/sorting/product.py
--rw-r--r--   0        0        0     4427 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/db/sorting/sorting.py
--rw-r--r--   0        0        0      606 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/db/sorting/subscription.py
--rw-r--r--   0        0        0        0 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/devtools/__init__.py
--rw-r--r--   0        0        0    16866 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/devtools/populator.py
--rw-r--r--   0        0        0     2508 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/distlock/__init__.py
--rw-r--r--   0        0        0     2533 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/distlock/distlock_manager.py
--rw-r--r--   0        0        0      571 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/distlock/managers/__init__.py
--rw-r--r--   0        0        0     3062 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/distlock/managers/memory_distlock_manager.py
--rw-r--r--   0        0        0     3329 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/distlock/managers/redis_distlock_manager.py
--rw-r--r--   0        0        0      924 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/domain/__init__.py
--rw-r--r--   0        0        0    62796 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/domain/base.py
--rw-r--r--   0        0        0     2694 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/domain/lifecycle.py
--rw-r--r--   0        0        0     2977 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/exception_handlers.py
--rw-r--r--   0        0        0     5434 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/forms/__init__.py
--rw-r--r--   0        0        0     2145 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/forms/network_type_validators.py
--rw-r--r--   0        0        0    11483 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/forms/validators.py
--rw-r--r--   0        0        0     5373 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/graphql/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/graphql/extensions/__init__.py
--rw-r--r--   0        0        0     4325 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/graphql/extensions/deprecation_checker_extension.py
--rw-r--r--   0        0        0     1777 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/graphql/extensions/error_collector_extension.py
--rw-r--r--   0        0        0     2334 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/graphql/pagination.py
--rw-r--r--   0        0        0      420 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/graphql/resolvers/__init__.py
--rw-r--r--   0        0        0     3674 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/graphql/resolvers/process.py
--rw-r--r--   0        0        0     2154 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/graphql/resolvers/product.py
--rw-r--r--   0        0        0     3727 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/graphql/resolvers/settings.py
--rw-r--r--   0        0        0     2907 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/graphql/resolvers/subscription.py
--rw-r--r--   0        0        0      203 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/graphql/schemas/errors.py
--rw-r--r--   0        0        0      513 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/graphql/schemas/fixed_input.py
--rw-r--r--   0        0        0     3674 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/graphql/schemas/process.py
--rw-r--r--   0        0        0     1776 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/graphql/schemas/product.py
--rw-r--r--   0        0        0      530 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/graphql/schemas/product_block.py
--rw-r--r--   0        0        0      305 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/graphql/schemas/resource_type.py
--rw-r--r--   0        0        0      980 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/graphql/schemas/settings.py
--rw-r--r--   0        0        0     7736 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/graphql/schemas/subscription.py
--rw-r--r--   0        0        0      172 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/graphql/schemas/workflow.py
--rw-r--r--   0        0        0     1789 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/graphql/types.py
--rw-r--r--   0        0        0      114 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/graphql/utils/__init__.py
--rw-r--r--   0        0        0     1071 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/graphql/utils/create_resolver_error_handler.py
--rw-r--r--   0        0        0      992 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/graphql/utils/get_selected_fields.py
--rw-r--r--   0        0        0       39 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/migrations/README
--rw-r--r--   0        0        0      873 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/migrations/alembic.ini
--rwxr-xr-x   0        0        0     3365 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/migrations/env.py
--rw-r--r--   0        0        0    40397 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/migrations/helpers.py
--rw-r--r--   0        0        0      510 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/migrations/script.py.mako
--rw-r--r--   0        0        0      905 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/migrations/templates/alembic.ini.j2
--rwxr-xr-x   0        0        0     2821 2023-06-27 11:40:53.976176 orchestrator_core-1.1.1rc4/orchestrator/migrations/templates/env.py.j2
--rw-r--r--   0        0        0       98 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/migrations/templates/helpers.py.j2
--rw-r--r--   0        0        0     2641 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py
--rw-r--r--   0        0        0     1266 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py
--rw-r--r--   0        0        0    38591 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py
--rw-r--r--   0        0        0      951 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py
--rw-r--r--   0        0        0     1213 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py
--rw-r--r--   0        0        0     1556 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py
--rw-r--r--   0        0        0     5105 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py
--rw-r--r--   0        0        0     7723 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py
--rw-r--r--   0        0        0      989 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/migrations/versions/schema/2023-05-25_b1970225392d_add_subscription_metadata_workflow.py
--rw-r--r--   0        0        0        0 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/py.typed
--rw-r--r--   0        0        0     1090 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/schedules/__init__.py
--rw-r--r--   0        0        0      832 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/schedules/resume_workflows.py
--rw-r--r--   0        0        0     1535 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/schedules/scheduling.py
--rw-r--r--   0        0        0      821 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/schedules/task_vacuum.py
--rw-r--r--   0        0        0     1053 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/schedules/validate_products.py
--rw-r--r--   0        0        0     2131 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/schedules/validate_subscriptions.py
--rw-r--r--   0        0        0     2631 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/schemas/__init__.py
--rw-r--r--   0        0        0      886 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/schemas/base.py
--rw-r--r--   0        0        0     1293 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/schemas/engine_settings.py
--rw-r--r--   0        0        0     1346 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/schemas/fixed_input.py
--rw-r--r--   0        0        0      842 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/schemas/problem_detail.py
--rw-r--r--   0        0        0     3390 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/schemas/process.py
--rw-r--r--   0        0        0     1670 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/schemas/product.py
--rw-r--r--   0        0        0     1735 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/schemas/product_block.py
--rw-r--r--   0        0        0      951 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/schemas/resource_type.py
--rw-r--r--   0        0        0     3180 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/schemas/subscription.py
--rw-r--r--   0        0        0     1013 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/schemas/subscription_descriptions.py
--rw-r--r--   0        0        0     1803 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/schemas/workflow.py
--rw-r--r--   0        0        0     1797 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/security.py
--rw-r--r--   0        0        0      571 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/services/__init__.py
--rw-r--r--   0        0        0     3586 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/services/celery.py
--rw-r--r--   0        0        0    22589 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/services/processes.py
--rw-r--r--   0        0        0     1530 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/services/products.py
--rw-r--r--   0        0        0     3879 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/services/settings.py
--rw-r--r--   0        0        0    24525 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/services/subscriptions.py
--rw-r--r--   0        0        0     5708 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/services/tasks.py
--rw-r--r--   0        0        0     1719 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/services/translations.py
--rw-r--r--   0        0        0     3708 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/settings.py
--rw-r--r--   0        0        0      766 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/targets.py
--rw-r--r--   0        0        0     9449 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/types.py
--rw-r--r--   0        0        0      571 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/utils/__init__.py
--rw-r--r--   0        0        0     5593 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/utils/crypt.py
--rw-r--r--   0        0        0     1477 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/utils/datetime.py
--rw-r--r--   0        0        0     6207 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/utils/docs.py
--rw-r--r--   0        0        0     3839 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/utils/errors.py
--rw-r--r--   0        0        0     8079 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/utils/functional.py
--rw-r--r--   0        0        0     2785 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/utils/helpers.py
--rw-r--r--   0        0        0     8512 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/utils/json.py
--rw-r--r--   0        0        0     3376 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/utils/redis.py
--rw-r--r--   0        0        0     2972 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/utils/show_process.py
--rw-r--r--   0        0        0     2395 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/utils/speed.py
--rw-r--r--   0        0        0    13148 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/utils/state.py
--rw-r--r--   0        0        0     1077 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/utils/strings.py
--rw-r--r--   0        0        0     7231 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/utils/vlans.py
--rw-r--r--   0        0        0     1323 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/version.py
--rw-r--r--   0        0        0     4476 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/websocket/__init__.py
--rw-r--r--   0        0        0     3535 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/websocket/managers/broadcast_websocket_manager.py
--rw-r--r--   0        0        0     3312 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/websocket/managers/memory_websocket_manager.py
--rw-r--r--   0        0        0     2900 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/websocket/websocket_manager.py
--rw-r--r--   0        0        0    33615 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/workflow.py
--rw-r--r--   0        0        0     4085 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/workflows/__init__.py
--rw-r--r--   0        0        0     2135 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/workflows/modify_note.py
--rw-r--r--   0        0        0      909 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/workflows/removed_workflow.py
--rw-r--r--   0        0        0     9188 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/workflows/steps.py
--rw-r--r--   0        0        0      571 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/workflows/tasks/__init__.py
--rw-r--r--   0        0        0     1510 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/workflows/tasks/cleanup_tasks_log.py
--rw-r--r--   0        0        0     2120 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/workflows/tasks/resume_workflows.py
--rw-r--r--   0        0        0     8335 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/workflows/tasks/validate_products.py
--rw-r--r--   0        0        0      684 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/workflows/translations/en-GB.json
--rw-r--r--   0        0        0    12830 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/orchestrator/workflows/utils.py
--rw-r--r--   0        0        0     4617 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/pyproject.toml
--rw-r--r--   0        0        0     2413 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/setup.cfg
--rw-r--r--   0        0        0      665 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/setup.py
--rw-r--r--   0        0        0        0 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/test/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/test/acceptance_tests/__init__.py
--rw-r--r--   0        0        0     3199 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/test/acceptance_tests/conftest.py
--rw-r--r--   0        0        0        0 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/test/acceptance_tests/fixtures/test_orchestrator/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/__init__.py
--rw-r--r--   0        0        0     1855 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py
--rw-r--r--   0        0        0     1544 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/test/acceptance_tests/fixtures/test_orchestrator/main.py
--rw-r--r--   0        0        0        0 2023-06-27 11:40:53.980176 orchestrator_core-1.1.1rc4/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/__init__.py
--rw-r--r--   0        0        0     1608 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py
--rw-r--r--   0        0        0        0 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/acceptance_tests/fixtures/test_orchestrator/products/__init__.py
--rw-r--r--   0        0        0     1211 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py
--rw-r--r--   0        0        0        0 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/acceptance_tests/fixtures/test_orchestrator/workflows/__init__.py
--rw-r--r--   0        0        0     2828 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py
--rw-r--r--   0        0        0      588 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/acceptance_tests/test_test_product.py
--rw-r--r--   0        0        0        0 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/api/__init__.py
--rw-r--r--   0        0        0     5159 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/api/test_caching.py
--rw-r--r--   0        0        0     1578 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/api/test_fixed_inputs.py
--rw-r--r--   0        0        0     1192 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/api/test_health.py
--rw-r--r--   0        0        0     3049 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/api/test_helpers.py
--rw-r--r--   0        0        0     1747 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/api/test_models.py
--rw-r--r--   0        0        0    19964 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/api/test_processes.py
--rw-r--r--   0        0        0    15454 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/api/test_processes_ws.py
--rw-r--r--   0        0        0     3742 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/api/test_product_blocks.py
--rw-r--r--   0        0        0     7942 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/api/test_products.py
--rw-r--r--   0        0        0     2486 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/api/test_resource_types.py
--rw-r--r--   0        0        0     1772 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/api/test_settings.py
--rw-r--r--   0        0        0     2985 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/api/test_subscription_customer_descriptions.py
--rw-r--r--   0        0        0    37706 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/api/test_subscriptions.py
--rw-r--r--   0        0        0     2367 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/api/test_workflows.py
--rw-r--r--   0        0        0    25724 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/cli/test_migrate_domain_models_with_instances.py
--rw-r--r--   0        0        0    27170 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/cli/test_migrate_domain_models_without_instances.py
--rw-r--r--   0        0        0      511 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/config.py
--rw-r--r--   0        0        0    22649 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/conftest.py
--rw-r--r--   0        0        0        0 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/domain/__init__.py
--rw-r--r--   0        0        0    50537 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/domain/test_base.py
--rw-r--r--   0        0        0     8092 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/domain/test_base_with_list_union.py
--rw-r--r--   0        0        0     4493 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/domain/test_base_with_union.py
--rw-r--r--   0        0        0     2824 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/fixtures/__init__.py
--rw-r--r--   0        0        0     7530 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/fixtures/processes.py
--rw-r--r--   0        0        0        0 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/fixtures/products/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/fixtures/products/product_blocks/__init__.py
--rw-r--r--   0        0        0     1683 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py
--rw-r--r--   0        0        0     2569 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/fixtures/products/product_blocks/product_block_one.py
--rw-r--r--   0        0        0     1609 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py
--rw-r--r--   0        0        0     2642 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py
--rw-r--r--   0        0        0     2590 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py
--rw-r--r--   0        0        0     1232 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py
--rw-r--r--   0        0        0     1055 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py
--rw-r--r--   0        0        0        0 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/fixtures/products/product_types/__init__.py
--rw-r--r--   0        0        0     2372 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py
--rw-r--r--   0        0        0     2262 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/fixtures/products/product_types/product_type_list_union.py
--rw-r--r--   0        0        0     4191 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py
--rw-r--r--   0        0        0     3240 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/fixtures/products/product_types/product_type_one.py
--rw-r--r--   0        0        0     2341 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py
--rw-r--r--   0        0        0     2977 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py
--rw-r--r--   0        0        0     2298 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py
--rw-r--r--   0        0        0     2282 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py
--rw-r--r--   0        0        0     1671 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py
--rw-r--r--   0        0        0     1898 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/fixtures/products/product_types/product_type_union.py
--rw-r--r--   0        0        0      527 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/fixtures/products/resource_types.py
--rw-r--r--   0        0        0        0 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/forms/__init__.py
--rw-r--r--   0        0        0     1462 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/forms/shared.py
--rw-r--r--   0        0        0    25426 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/forms/test_generic_validators.py
--rw-r--r--   0        0        0     7644 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/forms/test_network_validators.py
--rw-r--r--   0        0        0     6626 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/forms/test_post_process.py
--rw-r--r--   0        0        0    11107 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/graphql/test_processes.py
--rw-r--r--   0        0        0     7301 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/graphql/test_product.py
--rw-r--r--   0        0        0     5174 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/graphql/test_settings.py
--rw-r--r--   0        0        0    23655 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/graphql/test_subscriptions.py
--rw-r--r--   0        0        0        0 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/schedules/__init__.py
--rw-r--r--   0        0        0      807 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/schedules/test_scheduling.py
--rw-r--r--   0        0        0        0 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/services/__init__.py
--rw-r--r--   0        0        0    26695 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/services/test_processes.py
--rw-r--r--   0        0        0     1083 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/services/test_products.py
--rw-r--r--   0        0        0     5830 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/services/test_subscriptions.py
--rw-r--r--   0        0        0     2100 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/services/test_translations.py
--rw-r--r--   0        0        0     7353 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/test_db.py
--rw-r--r--   0        0        0      385 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/test_types.py
--rw-r--r--   0        0        0    12048 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/test_workflow.py
--rw-r--r--   0        0        0        0 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/utils/__init__.py
--rw-r--r--   0        0        0      163 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/utils/test_datetime.py
--rw-r--r--   0        0        0     1871 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/utils/test_errors.py
--rw-r--r--   0        0        0     3517 2023-06-27 11:40:53.984176 orchestrator_core-1.1.1rc4/test/unit_tests/utils/test_functional.py
--rw-r--r--   0        0        0     3052 2023-06-27 11:40:53.988176 orchestrator_core-1.1.1rc4/test/unit_tests/utils/test_json.py
--rw-r--r--   0        0        0     1144 2023-06-27 11:40:53.988176 orchestrator_core-1.1.1rc4/test/unit_tests/utils/test_speed.py
--rw-r--r--   0        0        0    11501 2023-06-27 11:40:53.988176 orchestrator_core-1.1.1rc4/test/unit_tests/utils/test_state.py
--rw-r--r--   0        0        0      192 2023-06-27 11:40:53.988176 orchestrator_core-1.1.1rc4/test/unit_tests/utils/test_strings.py
--rw-r--r--   0        0        0     8339 2023-06-27 11:40:53.988176 orchestrator_core-1.1.1rc4/test/unit_tests/utils/test_vlans.py
--rw-r--r--   0        0        0    12492 2023-06-27 11:40:53.988176 orchestrator_core-1.1.1rc4/test/unit_tests/workflows/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 11:40:53.988176 orchestrator_core-1.1.1rc4/test/unit_tests/workflows/conftest.py
--rw-r--r--   0        0        0        0 2023-06-27 11:40:53.988176 orchestrator_core-1.1.1rc4/test/unit_tests/workflows/shared/__init__.py
--rw-r--r--   0        0        0     2091 2023-06-27 11:40:53.988176 orchestrator_core-1.1.1rc4/test/unit_tests/workflows/shared/test_validate_subscriptions.py
--rw-r--r--   0        0        0        0 2023-06-27 11:40:53.988176 orchestrator_core-1.1.1rc4/test/unit_tests/workflows/tasks/__init__.py
--rw-r--r--   0        0        0     2039 2023-06-27 11:40:53.988176 orchestrator_core-1.1.1rc4/test/unit_tests/workflows/tasks/test_clean_up_task_log.py
--rw-r--r--   0        0        0     2584 2023-06-27 11:40:53.988176 orchestrator_core-1.1.1rc4/test/unit_tests/workflows/tasks/test_resume_workflows.py
--rw-r--r--   0        0        0      288 2023-06-27 11:40:53.988176 orchestrator_core-1.1.1rc4/test/unit_tests/workflows/tasks/test_validate_products.py
--rw-r--r--   0        0        0     3390 2023-06-27 11:40:53.988176 orchestrator_core-1.1.1rc4/test/unit_tests/workflows/test_config_db_code.py
--rw-r--r--   0        0        0     1877 2023-06-27 11:40:53.988176 orchestrator_core-1.1.1rc4/test/unit_tests/workflows/test_generic_workflow_steps.py
--rw-r--r--   0        0        0      987 2023-06-27 11:40:53.988176 orchestrator_core-1.1.1rc4/test/unit_tests/workflows/test_modify_note.py
--rw-r--r--   0        0        0     5363 1970-01-01 00:00:00.000000 orchestrator_core-1.1.1rc4/PKG-INFO
+-rw-r--r--   0        0        0      339 2023-07-03 10:05:15.849169 orchestrator_core-1.2.0/.bumpversion.cfg
+-rw-r--r--   0        0        0       33 2023-07-03 10:05:15.849169 orchestrator_core-1.2.0/.coveragerc
+-rw-r--r--   0        0        0     2620 2023-07-03 10:05:15.849169 orchestrator_core-1.2.0/.github/workflows/README.md
+-rw-r--r--   0        0        0     1851 2023-07-03 10:05:15.849169 orchestrator_core-1.2.0/.github/workflows/build-push-container.yml
+-rw-r--r--   0        0        0      291 2023-07-03 10:05:15.849169 orchestrator_core-1.2.0/.github/workflows/changelog.yml
+-rw-r--r--   0        0        0     2341 2023-07-03 10:05:15.849169 orchestrator_core-1.2.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0      371 2023-07-03 10:05:15.849169 orchestrator_core-1.2.0/.github/workflows/gh-pages.yml
+-rw-r--r--   0        0        0      550 2023-07-03 10:05:15.849169 orchestrator_core-1.2.0/.github/workflows/publish-package.yml
+-rw-r--r--   0        0        0     1138 2023-07-03 10:05:15.849169 orchestrator_core-1.2.0/.github/workflows/run-linting-tests.yml
+-rw-r--r--   0        0        0     2113 2023-07-03 10:05:15.849169 orchestrator_core-1.2.0/.github/workflows/run-unit-tests.yml
+-rw-r--r--   0        0        0     1985 2023-07-03 10:05:15.849169 orchestrator_core-1.2.0/.github/workflows/scheduled-build.yml
+-rw-r--r--   0        0        0     1809 2023-07-03 10:05:15.849169 orchestrator_core-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1592 2023-07-03 10:05:15.849169 orchestrator_core-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1150 2023-07-03 10:05:15.849169 orchestrator_core-1.2.0/.stignore
+-rw-r--r--   0        0        0    30087 2023-07-03 10:05:15.849169 orchestrator_core-1.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0      333 2023-07-03 10:05:15.849169 orchestrator_core-1.2.0/Dockerfile
+-rw-r--r--   0        0        0    11409 2023-07-03 10:05:15.849169 orchestrator_core-1.2.0/LICENSE
+-rw-r--r--   0        0        0      150 2023-07-03 10:05:15.849169 orchestrator_core-1.2.0/NOTICE
+-rw-r--r--   0        0        0     4965 2023-07-03 10:05:15.849169 orchestrator_core-1.2.0/README.md
+-rw-r--r--   0        0        0       76 2023-07-03 10:05:15.849169 orchestrator_core-1.2.0/codecov.yml
+-rw-r--r--   0        0        0       45 2023-07-03 10:05:15.849169 orchestrator_core-1.2.0/docs/architecture/application/api.md
+-rw-r--r--   0        0        0    16572 2023-07-03 10:05:15.849169 orchestrator_core-1.2.0/docs/architecture/application/cli.md
+-rw-r--r--   0        0        0    10741 2023-07-03 10:05:15.849169 orchestrator_core-1.2.0/docs/architecture/application/domainmodels.md
+-rw-r--r--   0        0        0    13931 2023-07-03 10:05:15.849169 orchestrator_core-1.2.0/docs/architecture/application/forms.md
+-rw-r--r--   0        0        0    48867 2023-07-03 10:05:15.849169 orchestrator_core-1.2.0/docs/architecture/application/openapi.json
+-rw-r--r--   0        0        0     1565 2023-07-03 10:05:15.849169 orchestrator_core-1.2.0/docs/architecture/application/python.md
+-rw-r--r--   0        0        0     5585 2023-07-03 10:05:15.849169 orchestrator_core-1.2.0/docs/architecture/application/scaling.md
+-rw-r--r--   0        0        0     5514 2023-07-03 10:05:15.849169 orchestrator_core-1.2.0/docs/architecture/application/tasks.md
+-rw-r--r--   0        0        0     2371 2023-07-03 10:05:15.849169 orchestrator_core-1.2.0/docs/architecture/application/websockets.md
+-rw-r--r--   0        0        0    11465 2023-07-03 10:05:15.849169 orchestrator_core-1.2.0/docs/architecture/application/workflow.md
+-rw-r--r--   0        0        0        0 2023-07-03 10:05:15.849169 orchestrator_core-1.2.0/docs/architecture/orchestration/philosophy.md
+-rw-r--r--   0        0        0      668 2023-07-03 10:05:15.849169 orchestrator_core-1.2.0/docs/architecture/product_modelling/context.md
+-rw-r--r--   0        0        0      802 2023-07-03 10:05:15.849169 orchestrator_core-1.2.0/docs/architecture/product_modelling/introduction.md
+-rw-r--r--   0        0        0     1671 2023-07-03 10:05:15.849169 orchestrator_core-1.2.0/docs/architecture/product_modelling/ip_static.md
+-rw-r--r--   0        0        0    84576 2023-07-03 10:05:15.849169 orchestrator_core-1.2.0/docs/architecture/product_modelling/ip_static.png
+-rw-r--r--   0        0        0     1310 2023-07-03 10:05:15.849169 orchestrator_core-1.2.0/docs/architecture/product_modelling/l2_point_to_point.md
+-rw-r--r--   0        0        0    55937 2023-07-03 10:05:15.849169 orchestrator_core-1.2.0/docs/architecture/product_modelling/l2_point_to_point.png
+-rw-r--r--   0        0        0      854 2023-07-03 10:05:15.849169 orchestrator_core-1.2.0/docs/architecture/product_modelling/l2_vpn.md
+-rw-r--r--   0        0        0    29551 2023-07-03 10:05:15.849169 orchestrator_core-1.2.0/docs/architecture/product_modelling/l2_vpn.png
+-rw-r--r--   0        0        0     1397 2023-07-03 10:05:15.849169 orchestrator_core-1.2.0/docs/architecture/product_modelling/modelling.md
+-rw-r--r--   0        0        0     1137 2023-07-03 10:05:15.849169 orchestrator_core-1.2.0/docs/architecture/product_modelling/node.md
+-rw-r--r--   0        0        0    23110 2023-07-03 10:05:15.853169 orchestrator_core-1.2.0/docs/architecture/product_modelling/node.png
+-rw-r--r--   0        0        0     1147 2023-07-03 10:05:15.853169 orchestrator_core-1.2.0/docs/architecture/product_modelling/port.md
+-rw-r--r--   0        0        0    37248 2023-07-03 10:05:15.853169 orchestrator_core-1.2.0/docs/architecture/product_modelling/port.png
+-rw-r--r--   0        0        0     1694 2023-07-03 10:05:15.853169 orchestrator_core-1.2.0/docs/architecture/product_modelling/product_block_graph.md
+-rw-r--r--   0        0        0    78824 2023-07-03 10:05:15.853169 orchestrator_core-1.2.0/docs/architecture/product_modelling/product_block_graph.png
+-rw-r--r--   0        0        0      989 2023-07-03 10:05:15.853169 orchestrator_core-1.2.0/docs/architecture/product_modelling/standards.md
+-rw-r--r--   0        0        0     1114 2023-07-03 10:05:15.853169 orchestrator_core-1.2.0/docs/architecture/product_modelling/terminology.md
+-rw-r--r--   0        0        0     2080 2023-07-03 10:05:15.853169 orchestrator_core-1.2.0/docs/architecture/tldr.md
+-rw-r--r--   0        0        0     1694 2023-07-03 10:05:15.853169 orchestrator_core-1.2.0/docs/contributing/guidelines.md
+-rw-r--r--   0        0        0    10000 2023-07-03 10:05:15.853169 orchestrator_core-1.2.0/docs/contributing/testing.md
+-rw-r--r--   0        0        0      452 2023-07-03 10:05:15.853169 orchestrator_core-1.2.0/docs/css/custom.css
+-rw-r--r--   0        0        0     2165 2023-07-03 10:05:15.853169 orchestrator_core-1.2.0/docs/css/termynal.css
+-rw-r--r--   0        0        0     2135 2023-07-03 10:05:15.853169 orchestrator_core-1.2.0/docs/getting-started/base.md
+-rw-r--r--   0        0        0      928 2023-07-03 10:05:15.853169 orchestrator_core-1.2.0/docs/getting-started/development.md
+-rw-r--r--   0        0        0     2367 2023-07-03 10:05:15.853169 orchestrator_core-1.2.0/docs/index.md
+-rw-r--r--   0        0        0     3897 2023-07-03 10:05:15.853169 orchestrator_core-1.2.0/docs/js/custom.js
+-rw-r--r--   0        0        0     9540 2023-07-03 10:05:15.853169 orchestrator_core-1.2.0/docs/js/termynal.js
+-rw-r--r--   0        0        0     8925 2023-07-03 10:05:15.853169 orchestrator_core-1.2.0/docs/workshops/advanced/circuit-workflow.md
+-rw-r--r--   0        0        0      254 2023-07-03 10:05:15.853169 orchestrator_core-1.2.0/docs/workshops/advanced/database-migration.md
+-rw-r--r--   0        0        0     3776 2023-07-03 10:05:15.853169 orchestrator_core-1.2.0/docs/workshops/advanced/docker-installation.md
+-rw-r--r--   0        0        0     2563 2023-07-03 10:05:15.853169 orchestrator_core-1.2.0/docs/workshops/advanced/domain-models.md
+-rw-r--r--   0        0        0     4126 2023-07-03 10:05:15.853169 orchestrator_core-1.2.0/docs/workshops/advanced/node-workflow.md
+-rw-r--r--   0        0        0     3079 2023-07-03 10:05:15.853169 orchestrator_core-1.2.0/docs/workshops/advanced/overview.md
+-rw-r--r--   0        0        0     1750 2023-07-03 10:05:15.853169 orchestrator_core-1.2.0/docs/workshops/advanced/scenario.md
+-rw-r--r--   0        0        0     4369 2023-07-03 10:05:15.853169 orchestrator_core-1.2.0/docs/workshops/advanced/workflow-introduction.md
+-rw-r--r--   0        0        0     5605 2023-07-03 10:05:15.853169 orchestrator_core-1.2.0/docs/workshops/beginner/create-user-group.md
+-rw-r--r--   0        0        0     4438 2023-07-03 10:05:15.853169 orchestrator_core-1.2.0/docs/workshops/beginner/create-user.md
+-rw-r--r--   0        0        0     7471 2023-07-03 10:05:15.853169 orchestrator_core-1.2.0/docs/workshops/beginner/database-migration.md
+-rw-r--r--   0        0        0     3700 2023-07-03 10:05:15.853169 orchestrator_core-1.2.0/docs/workshops/beginner/debian.md
+-rw-r--r--   0        0        0     3063 2023-07-03 10:05:15.853169 orchestrator_core-1.2.0/docs/workshops/beginner/docker.md
+-rw-r--r--   0        0        0     6106 2023-07-03 10:05:15.853169 orchestrator_core-1.2.0/docs/workshops/beginner/domain-models.md
+-rw-r--r--   0        0        0     1952 2023-07-03 10:05:15.853169 orchestrator_core-1.2.0/docs/workshops/beginner/explore.md
+-rw-r--r--   0        0        0     3996 2023-07-03 10:05:15.853169 orchestrator_core-1.2.0/docs/workshops/beginner/input-forms.md
+-rw-r--r--   0        0        0     3595 2023-07-03 10:05:15.853169 orchestrator_core-1.2.0/docs/workshops/beginner/macos.md
+-rw-r--r--   0        0        0     3411 2023-07-03 10:05:15.853169 orchestrator_core-1.2.0/docs/workshops/beginner/modify-user-group.md
+-rw-r--r--   0        0        0     2143 2023-07-03 10:05:15.853169 orchestrator_core-1.2.0/docs/workshops/beginner/modify-user.md
+-rw-r--r--   0        0        0     2885 2023-07-03 10:05:15.853169 orchestrator_core-1.2.0/docs/workshops/beginner/overview.md
+-rw-r--r--   0        0        0     4547 2023-07-03 10:05:15.853169 orchestrator_core-1.2.0/docs/workshops/beginner/register-workflows.md
+-rw-r--r--   0        0        0      786 2023-07-03 10:05:15.853169 orchestrator_core-1.2.0/docs/workshops/beginner/scenario.md
+-rw-r--r--   0        0        0     1013 2023-07-03 10:05:15.853169 orchestrator_core-1.2.0/docs/workshops/beginner/start-applications.md
+-rw-r--r--   0        0        0     2988 2023-07-03 10:05:15.853169 orchestrator_core-1.2.0/docs/workshops/beginner/terminate-user-group.md
+-rw-r--r--   0        0        0     1332 2023-07-03 10:05:15.853169 orchestrator_core-1.2.0/docs/workshops/beginner/terminate-user.md
+-rw-r--r--   0        0        0     3637 2023-07-03 10:05:15.853169 orchestrator_core-1.2.0/docs/workshops/beginner/workflow-introduction.md
+-rw-r--r--   0        0        0    46296 2023-07-03 10:05:15.853169 orchestrator_core-1.2.0/docs/workshops/images/metadata_products.png
+-rw-r--r--   0        0        0   983304 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/docs/workshops/images/netbox_devices_active.png
+-rw-r--r--   0        0        0      771 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/examples/basic/basic_orchestrator.py
+-rw-r--r--   0        0        0     4990 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/mkdocs.yml
+-rw-r--r--   0        0        0     1262 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/mutmut_config.py
+-rw-r--r--   0        0        0        0 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/.stignore
+-rw-r--r--   0        0        0     1095 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/__init__.py
+-rw-r--r--   0        0        0      571 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/api/__init__.py
+-rw-r--r--   0        0        0      571 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/api/api_v1/__init__.py
+-rw-r--r--   0        0        0     2967 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/api/api_v1/api.py
+-rw-r--r--   0        0        0      571 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/api/api_v1/endpoints/__init__.py
+-rw-r--r--   0        0        0     2855 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/api/api_v1/endpoints/fixed_input.py
+-rw-r--r--   0        0        0     1236 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/api/api_v1/endpoints/health.py
+-rw-r--r--   0        0        0    12981 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/api/api_v1/endpoints/processes.py
+-rw-r--r--   0        0        0     2703 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/api/api_v1/endpoints/product_blocks.py
+-rw-r--r--   0        0        0     3331 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/api/api_v1/endpoints/products.py
+-rw-r--r--   0        0        0     2552 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/api/api_v1/endpoints/resource_types.py
+-rw-r--r--   0        0        0     5801 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/api/api_v1/endpoints/settings.py
+-rw-r--r--   0        0        0     2866 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py
+-rw-r--r--   0        0        0    11648 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/api/api_v1/endpoints/subscriptions.py
+-rw-r--r--   0        0        0      961 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/api/api_v1/endpoints/translations.py
+-rw-r--r--   0        0        0     1833 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/api/api_v1/endpoints/user.py
+-rw-r--r--   0        0        0     1961 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/api/api_v1/endpoints/workflows.py
+-rw-r--r--   0        0        0     1543 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/api/error_handling.py
+-rw-r--r--   0        0        0    11719 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/api/helpers.py
+-rw-r--r--   0        0        0     5617 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/api/models.py
+-rw-r--r--   0        0        0     6969 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/app.py
+-rw-r--r--   0        0        0      571 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/__init__.py
+-rw-r--r--   0        0        0    13845 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/database.py
+-rw-r--r--   0        0        0        0 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/domain_gen_helpers/__init__.py
+-rw-r--r--   0        0        0     6837 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py
+-rw-r--r--   0        0        0     1953 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/domain_gen_helpers/helpers.py
+-rw-r--r--   0        0        0    10635 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/domain_gen_helpers/product_block_helpers.py
+-rw-r--r--   0        0        0     9409 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/domain_gen_helpers/product_helpers.py
+-rw-r--r--   0        0        0    24055 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py
+-rw-r--r--   0        0        0     1435 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/domain_gen_helpers/types.py
+-rw-r--r--   0        0        0     2371 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/generate.md
+-rw-r--r--   0        0        0     5168 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/generate.py
+-rw-r--r--   0        0        0        0 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/generator/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/generator/generator/__init__.py
+-rw-r--r--   0        0        0     1744 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/generator/generator/fixed_input.py
+-rw-r--r--   0        0        0     2626 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/generator/generator/helpers.py
+-rw-r--r--   0        0        0     2607 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/generator/generator/migration.py
+-rw-r--r--   0        0        0     2152 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/generator/generator/product.py
+-rw-r--r--   0        0        0     5793 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/generator/generator/product_block.py
+-rw-r--r--   0        0        0     1400 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/generator/generator/settings.py
+-rw-r--r--   0        0        0     1794 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/generator/generator/translations.py
+-rw-r--r--   0        0        0     4234 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/generator/generator/unittest.py
+-rw-r--r--   0        0        0     1957 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/generator/generator/validations.py
+-rw-r--r--   0        0        0     6535 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/generator/generator/workflow.py
+-rw-r--r--   0        0        0      779 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/generator/products/workshop/circuit.yaml
+-rw-r--r--   0        0        0      557 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/generator/products/workshop/node.yaml
+-rw-r--r--   0        0        0      553 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/generator/products/workshop/user.yaml
+-rw-r--r--   0        0        0      380 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/generator/products/workshop/user_group.yaml
+-rw-r--r--   0        0        0      289 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/generator/templates/constrained_int_definitions.j2
+-rw-r--r--   0        0        0     4196 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/generator/templates/create_product.j2
+-rw-r--r--   0        0        0      337 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/generator/templates/list_definitions.j2
+-rw-r--r--   0        0        0      520 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/generator/templates/macros.j2
+-rw-r--r--   0        0        0     4405 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/generator/templates/modify_product.j2
+-rw-r--r--   0        0        0     2639 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/generator/templates/new_product_migration.j2
+-rw-r--r--   0        0        0     1675 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/generator/templates/product.j2
+-rw-r--r--   0        0        0     2275 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/generator/templates/product_block.j2
+-rw-r--r--   0        0        0      514 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/generator/templates/shared_forms.j2
+-rw-r--r--   0        0        0     2808 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/generator/templates/terminate_product.j2
+-rw-r--r--   0        0        0     1764 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/generator/templates/test_create_workflow.j2
+-rw-r--r--   0        0        0     1689 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/generator/templates/test_modify_workflow.j2
+-rw-r--r--   0        0        0     1860 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/generator/templates/test_product_type.j2
+-rw-r--r--   0        0        0     1518 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/generator/templates/test_terminate_workflow.j2
+-rw-r--r--   0        0        0      984 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/generator/templates/test_validate_workflow.j2
+-rw-r--r--   0        0        0     2391 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/generator/templates/validate_product.j2
+-rw-r--r--   0        0        0      571 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/helpers/__init__.py
+-rw-r--r--   0        0        0     1165 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/helpers/input_helpers.py
+-rw-r--r--   0        0        0      830 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/helpers/print_helpers.py
+-rw-r--r--   0        0        0      983 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/main.py
+-rwxr-xr-x   0        0        0    20258 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/migrate_domain_models.py
+-rwxr-xr-x   0        0        0     8929 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/migrate_workflows.py
+-rw-r--r--   0        0        0     4093 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/migration_helpers.py
+-rw-r--r--   0        0        0     1896 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/cli/scheduler.py
+-rw-r--r--   0        0        0      571 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/config/__init__.py
+-rw-r--r--   0        0        0      770 2023-07-03 10:05:15.861169 orchestrator_core-1.2.0/orchestrator/config/assignee.py
+-rw-r--r--   0        0        0     2981 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/db/__init__.py
+-rw-r--r--   0        0        0    10201 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/db/database.py
+-rw-r--r--   0        0        0      303 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/db/filters/__init__.py
+-rw-r--r--   0        0        0     3618 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/db/filters/filters.py
+-rw-r--r--   0        0        0      774 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/db/filters/generic_filters/__init__.py
+-rw-r--r--   0        0        0      992 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/db/filters/generic_filters/bool_filter.py
+-rw-r--r--   0        0        0      952 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/db/filters/generic_filters/is_like_filter.py
+-rw-r--r--   0        0        0     2542 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/db/filters/generic_filters/range_filter.py
+-rw-r--r--   0        0        0      993 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/db/filters/generic_filters/values_in_column_filter.py
+-rw-r--r--   0        0        0     3592 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/db/filters/process.py
+-rw-r--r--   0        0        0     1251 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/db/filters/product.py
+-rw-r--r--   0        0        0     3203 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/db/filters/subscription.py
+-rw-r--r--   0        0        0    23604 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/db/models.py
+-rw-r--r--   0        0        0      104 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/db/range/__init__.py
+-rw-r--r--   0        0        0     1433 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/db/range/range.py
+-rw-r--r--   0        0        0      419 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/db/sorting/__init__.py
+-rw-r--r--   0        0        0      603 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/db/sorting/process.py
+-rw-r--r--   0        0        0      418 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/db/sorting/product.py
+-rw-r--r--   0        0        0     4367 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/db/sorting/sorting.py
+-rw-r--r--   0        0        0      606 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/db/sorting/subscription.py
+-rw-r--r--   0        0        0        0 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/devtools/__init__.py
+-rw-r--r--   0        0        0    16814 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/devtools/populator.py
+-rw-r--r--   0        0        0     2513 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/distlock/__init__.py
+-rw-r--r--   0        0        0     2533 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/distlock/distlock_manager.py
+-rw-r--r--   0        0        0      571 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/distlock/managers/__init__.py
+-rw-r--r--   0        0        0     3062 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/distlock/managers/memory_distlock_manager.py
+-rw-r--r--   0        0        0     3298 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/distlock/managers/redis_distlock_manager.py
+-rw-r--r--   0        0        0      924 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/domain/__init__.py
+-rw-r--r--   0        0        0    62898 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/domain/base.py
+-rw-r--r--   0        0        0     2694 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/domain/lifecycle.py
+-rw-r--r--   0        0        0     2908 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/exception_handlers.py
+-rw-r--r--   0        0        0     5418 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/forms/__init__.py
+-rw-r--r--   0        0        0     2145 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/forms/network_type_validators.py
+-rw-r--r--   0        0        0    11483 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/forms/validators.py
+-rw-r--r--   0        0        0     5373 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/graphql/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/graphql/extensions/__init__.py
+-rw-r--r--   0        0        0     4311 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/graphql/extensions/deprecation_checker_extension.py
+-rw-r--r--   0        0        0     1777 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/graphql/extensions/error_collector_extension.py
+-rw-r--r--   0        0        0     2334 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/graphql/pagination.py
+-rw-r--r--   0        0        0      420 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/graphql/resolvers/__init__.py
+-rw-r--r--   0        0        0     3674 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/graphql/resolvers/process.py
+-rw-r--r--   0        0        0     2154 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/graphql/resolvers/product.py
+-rw-r--r--   0        0        0     3727 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/graphql/resolvers/settings.py
+-rw-r--r--   0        0        0     2907 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/graphql/resolvers/subscription.py
+-rw-r--r--   0        0        0      203 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/graphql/schemas/errors.py
+-rw-r--r--   0        0        0      513 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/graphql/schemas/fixed_input.py
+-rw-r--r--   0        0        0     3674 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/graphql/schemas/process.py
+-rw-r--r--   0        0        0     1776 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/graphql/schemas/product.py
+-rw-r--r--   0        0        0      530 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/graphql/schemas/product_block.py
+-rw-r--r--   0        0        0      305 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/graphql/schemas/resource_type.py
+-rw-r--r--   0        0        0      980 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/graphql/schemas/settings.py
+-rw-r--r--   0        0        0     7736 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/graphql/schemas/subscription.py
+-rw-r--r--   0        0        0      172 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/graphql/schemas/workflow.py
+-rw-r--r--   0        0        0     1789 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/graphql/types.py
+-rw-r--r--   0        0        0      114 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/graphql/utils/__init__.py
+-rw-r--r--   0        0        0     1071 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/graphql/utils/create_resolver_error_handler.py
+-rw-r--r--   0        0        0      990 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/graphql/utils/get_selected_fields.py
+-rw-r--r--   0        0        0       39 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/migrations/README
+-rw-r--r--   0        0        0      873 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/migrations/alembic.ini
+-rwxr-xr-x   0        0        0     3365 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/migrations/env.py
+-rw-r--r--   0        0        0    40411 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/migrations/helpers.py
+-rw-r--r--   0        0        0      510 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/migrations/script.py.mako
+-rw-r--r--   0        0        0      905 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/migrations/templates/alembic.ini.j2
+-rwxr-xr-x   0        0        0     2821 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/migrations/templates/env.py.j2
+-rw-r--r--   0        0        0       98 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/migrations/templates/helpers.py.j2
+-rw-r--r--   0        0        0     2641 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py
+-rw-r--r--   0        0        0     1266 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py
+-rw-r--r--   0        0        0    38591 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py
+-rw-r--r--   0        0        0      951 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py
+-rw-r--r--   0        0        0     1213 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py
+-rw-r--r--   0        0        0     1556 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py
+-rw-r--r--   0        0        0     5105 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py
+-rw-r--r--   0        0        0     7723 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py
+-rw-r--r--   0        0        0      989 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/migrations/versions/schema/2023-05-25_b1970225392d_add_subscription_metadata_workflow.py
+-rw-r--r--   0        0        0        0 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/py.typed
+-rw-r--r--   0        0        0     1090 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/schedules/__init__.py
+-rw-r--r--   0        0        0      832 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/schedules/resume_workflows.py
+-rw-r--r--   0        0        0     1535 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/schedules/scheduling.py
+-rw-r--r--   0        0        0      821 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/schedules/task_vacuum.py
+-rw-r--r--   0        0        0     1053 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/schedules/validate_products.py
+-rw-r--r--   0        0        0     2131 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/schedules/validate_subscriptions.py
+-rw-r--r--   0        0        0     2631 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/schemas/__init__.py
+-rw-r--r--   0        0        0      886 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/schemas/base.py
+-rw-r--r--   0        0        0     1293 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/schemas/engine_settings.py
+-rw-r--r--   0        0        0     1346 2023-07-03 10:05:15.865169 orchestrator_core-1.2.0/orchestrator/schemas/fixed_input.py
+-rw-r--r--   0        0        0      842 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/orchestrator/schemas/problem_detail.py
+-rw-r--r--   0        0        0     3404 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/orchestrator/schemas/process.py
+-rw-r--r--   0        0        0     1670 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/orchestrator/schemas/product.py
+-rw-r--r--   0        0        0     1735 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/orchestrator/schemas/product_block.py
+-rw-r--r--   0        0        0      951 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/orchestrator/schemas/resource_type.py
+-rw-r--r--   0        0        0     3180 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/orchestrator/schemas/subscription.py
+-rw-r--r--   0        0        0     1013 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/orchestrator/schemas/subscription_descriptions.py
+-rw-r--r--   0        0        0     1803 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/orchestrator/schemas/workflow.py
+-rw-r--r--   0        0        0     1797 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/orchestrator/security.py
+-rw-r--r--   0        0        0      571 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/orchestrator/services/__init__.py
+-rw-r--r--   0        0        0     3586 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/orchestrator/services/celery.py
+-rw-r--r--   0        0        0    22606 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/orchestrator/services/processes.py
+-rw-r--r--   0        0        0     1525 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/orchestrator/services/products.py
+-rw-r--r--   0        0        0     3927 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/orchestrator/services/settings.py
+-rw-r--r--   0        0        0    24397 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/orchestrator/services/subscriptions.py
+-rw-r--r--   0        0        0     5716 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/orchestrator/services/tasks.py
+-rw-r--r--   0        0        0     1719 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/orchestrator/services/translations.py
+-rw-r--r--   0        0        0     3190 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/orchestrator/settings.py
+-rw-r--r--   0        0        0      766 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/orchestrator/targets.py
+-rw-r--r--   0        0        0     9427 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/orchestrator/types.py
+-rw-r--r--   0        0        0      571 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/orchestrator/utils/__init__.py
+-rw-r--r--   0        0        0     5593 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/orchestrator/utils/crypt.py
+-rw-r--r--   0        0        0     1477 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/orchestrator/utils/datetime.py
+-rw-r--r--   0        0        0     6206 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/orchestrator/utils/docs.py
+-rw-r--r--   0        0        0     4324 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/orchestrator/utils/errors.py
+-rw-r--r--   0        0        0     8079 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/orchestrator/utils/functional.py
+-rw-r--r--   0        0        0     2751 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/orchestrator/utils/helpers.py
+-rw-r--r--   0        0        0     8489 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/orchestrator/utils/json.py
+-rw-r--r--   0        0        0     3340 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/orchestrator/utils/redis.py
+-rw-r--r--   0        0        0     2972 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/orchestrator/utils/show_process.py
+-rw-r--r--   0        0        0     2395 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/orchestrator/utils/speed.py
+-rw-r--r--   0        0        0    13057 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/orchestrator/utils/state.py
+-rw-r--r--   0        0        0     1077 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/orchestrator/utils/strings.py
+-rw-r--r--   0        0        0     7240 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/orchestrator/utils/vlans.py
+-rw-r--r--   0        0        0     1318 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/orchestrator/version.py
+-rw-r--r--   0        0        0     4476 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/orchestrator/websocket/__init__.py
+-rw-r--r--   0        0        0     3535 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/orchestrator/websocket/managers/broadcast_websocket_manager.py
+-rw-r--r--   0        0        0     3312 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/orchestrator/websocket/managers/memory_websocket_manager.py
+-rw-r--r--   0        0        0     2900 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/orchestrator/websocket/websocket_manager.py
+-rw-r--r--   0        0        0    33502 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/orchestrator/workflow.py
+-rw-r--r--   0        0        0     4085 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/orchestrator/workflows/__init__.py
+-rw-r--r--   0        0        0     2135 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/orchestrator/workflows/modify_note.py
+-rw-r--r--   0        0        0      909 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/orchestrator/workflows/removed_workflow.py
+-rw-r--r--   0        0        0     9185 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/orchestrator/workflows/steps.py
+-rw-r--r--   0        0        0      571 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/orchestrator/workflows/tasks/__init__.py
+-rw-r--r--   0        0        0     1510 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/orchestrator/workflows/tasks/cleanup_tasks_log.py
+-rw-r--r--   0        0        0     2120 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/orchestrator/workflows/tasks/resume_workflows.py
+-rw-r--r--   0        0        0     8375 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/orchestrator/workflows/tasks/validate_products.py
+-rw-r--r--   0        0        0      684 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/orchestrator/workflows/translations/en-GB.json
+-rw-r--r--   0        0        0    12830 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/orchestrator/workflows/utils.py
+-rw-r--r--   0        0        0     4873 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1940 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/setup.cfg
+-rw-r--r--   0        0        0      665 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/setup.py
+-rw-r--r--   0        0        0        0 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/test/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/test/acceptance_tests/__init__.py
+-rw-r--r--   0        0        0     3199 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/test/acceptance_tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/test/acceptance_tests/fixtures/test_orchestrator/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/__init__.py
+-rw-r--r--   0        0        0     1855 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py
+-rw-r--r--   0        0        0     1544 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/test/acceptance_tests/fixtures/test_orchestrator/main.py
+-rw-r--r--   0        0        0        0 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/__init__.py
+-rw-r--r--   0        0        0     1608 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py
+-rw-r--r--   0        0        0        0 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/test/acceptance_tests/fixtures/test_orchestrator/products/__init__.py
+-rw-r--r--   0        0        0     1210 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py
+-rw-r--r--   0        0        0        0 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/test/acceptance_tests/fixtures/test_orchestrator/workflows/__init__.py
+-rw-r--r--   0        0        0     2828 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py
+-rw-r--r--   0        0        0      588 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/test/acceptance_tests/test_test_product.py
+-rw-r--r--   0        0        0        0 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/test/unit_tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/test/unit_tests/api/__init__.py
+-rw-r--r--   0        0        0     5159 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/test/unit_tests/api/test_caching.py
+-rw-r--r--   0        0        0     1578 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/test/unit_tests/api/test_fixed_inputs.py
+-rw-r--r--   0        0        0     1192 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/test/unit_tests/api/test_health.py
+-rw-r--r--   0        0        0     3049 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/test/unit_tests/api/test_helpers.py
+-rw-r--r--   0        0        0     1747 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/test/unit_tests/api/test_models.py
+-rw-r--r--   0        0        0    19964 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/test/unit_tests/api/test_processes.py
+-rw-r--r--   0        0        0    15454 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/test/unit_tests/api/test_processes_ws.py
+-rw-r--r--   0        0        0     3742 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/test/unit_tests/api/test_product_blocks.py
+-rw-r--r--   0        0        0     7942 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/test/unit_tests/api/test_products.py
+-rw-r--r--   0        0        0     2486 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/test/unit_tests/api/test_resource_types.py
+-rw-r--r--   0        0        0     1772 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/test/unit_tests/api/test_settings.py
+-rw-r--r--   0        0        0     2985 2023-07-03 10:05:15.869169 orchestrator_core-1.2.0/test/unit_tests/api/test_subscription_customer_descriptions.py
+-rw-r--r--   0        0        0    37706 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/api/test_subscriptions.py
+-rw-r--r--   0        0        0     2367 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/api/test_workflows.py
+-rw-r--r--   0        0        0    25724 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/cli/test_migrate_domain_models_with_instances.py
+-rw-r--r--   0        0        0    27170 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/cli/test_migrate_domain_models_without_instances.py
+-rw-r--r--   0        0        0      511 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/config.py
+-rw-r--r--   0        0        0    22634 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/domain/__init__.py
+-rw-r--r--   0        0        0    50537 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/domain/test_base.py
+-rw-r--r--   0        0        0     8092 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/domain/test_base_with_list_union.py
+-rw-r--r--   0        0        0     4493 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/domain/test_base_with_union.py
+-rw-r--r--   0        0        0     2845 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/fixtures/__init__.py
+-rw-r--r--   0        0        0     7530 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/fixtures/processes.py
+-rw-r--r--   0        0        0        0 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/fixtures/products/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/fixtures/products/product_blocks/__init__.py
+-rw-r--r--   0        0        0     1683 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py
+-rw-r--r--   0        0        0     2569 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/fixtures/products/product_blocks/product_block_one.py
+-rw-r--r--   0        0        0     1609 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py
+-rw-r--r--   0        0        0     2642 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py
+-rw-r--r--   0        0        0     2590 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py
+-rw-r--r--   0        0        0     1232 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py
+-rw-r--r--   0        0        0     1055 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py
+-rw-r--r--   0        0        0        0 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/fixtures/products/product_types/__init__.py
+-rw-r--r--   0        0        0     2372 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py
+-rw-r--r--   0        0        0     2262 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/fixtures/products/product_types/product_type_list_union.py
+-rw-r--r--   0        0        0     4191 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py
+-rw-r--r--   0        0        0     3240 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/fixtures/products/product_types/product_type_one.py
+-rw-r--r--   0        0        0     2341 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py
+-rw-r--r--   0        0        0     2977 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py
+-rw-r--r--   0        0        0     2298 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py
+-rw-r--r--   0        0        0     2282 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py
+-rw-r--r--   0        0        0     1671 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py
+-rw-r--r--   0        0        0     1898 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/fixtures/products/product_types/product_type_union.py
+-rw-r--r--   0        0        0      527 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/fixtures/products/resource_types.py
+-rw-r--r--   0        0        0        0 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/forms/__init__.py
+-rw-r--r--   0        0        0     1462 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/forms/shared.py
+-rw-r--r--   0        0        0    25426 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/forms/test_generic_validators.py
+-rw-r--r--   0        0        0     7644 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/forms/test_network_validators.py
+-rw-r--r--   0        0        0     6626 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/forms/test_post_process.py
+-rw-r--r--   0        0        0    11107 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/graphql/test_processes.py
+-rw-r--r--   0        0        0     7301 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/graphql/test_product.py
+-rw-r--r--   0        0        0     5174 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/graphql/test_settings.py
+-rw-r--r--   0        0        0    23655 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/graphql/test_subscriptions.py
+-rw-r--r--   0        0        0        0 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/schedules/__init__.py
+-rw-r--r--   0        0        0      807 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/schedules/test_scheduling.py
+-rw-r--r--   0        0        0        0 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/services/__init__.py
+-rw-r--r--   0        0        0    26695 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/services/test_processes.py
+-rw-r--r--   0        0        0     1083 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/services/test_products.py
+-rw-r--r--   0        0        0     5830 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/services/test_subscriptions.py
+-rw-r--r--   0        0        0     2100 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/services/test_translations.py
+-rw-r--r--   0        0        0     7353 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/test_db.py
+-rw-r--r--   0        0        0      385 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/test_types.py
+-rw-r--r--   0        0        0    12029 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/test_workflow.py
+-rw-r--r--   0        0        0        0 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/utils/__init__.py
+-rw-r--r--   0        0        0      163 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/utils/test_datetime.py
+-rw-r--r--   0        0        0     1891 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/utils/test_errors.py
+-rw-r--r--   0        0        0     3517 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/utils/test_functional.py
+-rw-r--r--   0        0        0     3052 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/utils/test_json.py
+-rw-r--r--   0        0        0     1144 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/utils/test_speed.py
+-rw-r--r--   0        0        0    11501 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/utils/test_state.py
+-rw-r--r--   0        0        0      192 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/utils/test_strings.py
+-rw-r--r--   0        0        0     8339 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/utils/test_vlans.py
+-rw-r--r--   0        0        0    12493 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/workflows/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/workflows/conftest.py
+-rw-r--r--   0        0        0        0 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/workflows/shared/__init__.py
+-rw-r--r--   0        0        0     2091 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/workflows/shared/test_validate_subscriptions.py
+-rw-r--r--   0        0        0        0 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/workflows/tasks/__init__.py
+-rw-r--r--   0        0        0     2039 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/workflows/tasks/test_clean_up_task_log.py
+-rw-r--r--   0        0        0     2584 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/workflows/tasks/test_resume_workflows.py
+-rw-r--r--   0        0        0      288 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/workflows/tasks/test_validate_products.py
+-rw-r--r--   0        0        0     3390 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/workflows/test_config_db_code.py
+-rw-r--r--   0        0        0     1877 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/workflows/test_generic_workflow_steps.py
+-rw-r--r--   0        0        0      987 2023-07-03 10:05:15.873169 orchestrator_core-1.2.0/test/unit_tests/workflows/test_modify_note.py
+-rw-r--r--   0        0        0     4350 1970-01-01 00:00:00.000000 orchestrator_core-1.2.0/PKG-INFO
```

### Comparing `orchestrator_core-1.1.1rc4/.github/workflows/README.md` & `orchestrator_core-1.2.0/.github/workflows/README.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/.github/workflows/build-push-container.yml` & `orchestrator_core-1.2.0/.github/workflows/build-push-container.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/.github/workflows/codeql-analysis.yml` & `orchestrator_core-1.2.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/.github/workflows/publish-package.yml` & `orchestrator_core-1.2.0/.github/workflows/publish-package.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/.github/workflows/run-linting-tests.yml` & `orchestrator_core-1.2.0/.github/workflows/run-linting-tests.yml`

 * *Files 19% similar despite different names*

```diff
@@ -27,16 +27,15 @@
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install flit
           flit install --deps develop --symlink
       - name: Check formatting
         run: |
-          isort -c .
           black --check .
-      - name: Lint with flake8
+      - name: Lint with ruff
         run: |
           # stop the build if there are Python syntax errors or undefined names
-          flake8 .
+          ruff .
       - name: Check with mypy
         run: |
           mypy .
```

### Comparing `orchestrator_core-1.1.1rc4/.github/workflows/run-unit-tests.yml` & `orchestrator_core-1.2.0/.github/workflows/run-unit-tests.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/.github/workflows/scheduled-build.yml` & `orchestrator_core-1.2.0/.github/workflows/scheduled-build.yml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/.gitignore` & `orchestrator_core-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/.pre-commit-config.yaml` & `orchestrator_core-1.2.0/.pre-commit-config.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 default_language_version:
   python: python3
 repos:
-  - repo: https://github.com/timothycrosley/isort
-    rev: 5.12.0
-    hooks:
-      - id: isort
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/asottile/blacken-docs
     rev: 1.13.0
     hooks:
@@ -21,29 +17,14 @@
       - id: end-of-file-fixer
       - id: check-docstring-first
       - id: check-json
       - id: check-yaml
       - id: debug-statements
       - id: requirements-txt-fixer
       - id: detect-private-key
-  - repo: https://github.com/PyCQA/flake8
-    rev: 6.0.0
-    hooks:
-      - id: flake8
-        additional_dependencies:
-          - flake8-bandit
-          - flake8-bugbear
-          - flake8-comprehensions
-          - flake8-docstrings
-          - flake8-logging-format
-          - flake8-pep3101
-          - flake8-print
-          - flake8-rst
-          - flake8-rst-docstrings
-          - flake8-tidy-imports
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: v1.2.0
     hooks:
       - id: mypy
         additional_dependencies:
           - pydantic
           - types-toml
```

### Comparing `orchestrator_core-1.1.1rc4/.stignore` & `orchestrator_core-1.2.0/.stignore`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/CHANGELOG.md` & `orchestrator_core-1.2.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Changelog
 
-## [1.1.0rc2]
+## [1.2.0]
+ - Removed the opentelemetry dependancy and added warnings to function calls
+ - Renamed an error classes and added warnings
 
-- Add support for subscription metadata [\#266](https://github.com/workfloworchestrator/orchestrator-core/issues/266)
-
-
-## [1.1.0rc1]
+## [1.1.0]
 
 ### Breaking change
  - Changed `settings.CACHE_HOST` and `settings.CACHE_PORT` to `settings.CACHE_URI` 
+ - Add support for subscription metadata [\#266](https://github.com/workfloworchestrator/orchestrator-core/issues/266)
 
 ## [1.0.2]
 
 - Allow user to extend the default translation set, instead of overwriting everything
 - Return worker status information in the `/api/settings/worker-status` endpoint
 
 ## [0.4.0-rc1](https://github.com/workfloworchestrator/orchestrator-core/tree/0.4.0-rc1) (2022-03-08)
```

### Comparing `orchestrator_core-1.1.1rc4/LICENSE` & `orchestrator_core-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/README.md` & `orchestrator_core-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/docs/architecture/application/cli.md` & `orchestrator_core-1.2.0/docs/architecture/application/cli.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/docs/architecture/application/domainmodels.md` & `orchestrator_core-1.2.0/docs/architecture/application/domainmodels.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/docs/architecture/application/forms.md` & `orchestrator_core-1.2.0/docs/architecture/application/forms.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/docs/architecture/application/openapi.json` & `orchestrator_core-1.2.0/docs/architecture/application/openapi.json`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/docs/architecture/application/python.md` & `orchestrator_core-1.2.0/docs/architecture/application/python.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/docs/architecture/application/scaling.md` & `orchestrator_core-1.2.0/docs/architecture/application/scaling.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/docs/architecture/application/tasks.md` & `orchestrator_core-1.2.0/docs/architecture/application/tasks.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/docs/architecture/application/websockets.md` & `orchestrator_core-1.2.0/docs/architecture/application/websockets.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/docs/architecture/application/workflow.md` & `orchestrator_core-1.2.0/docs/architecture/application/workflow.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/docs/architecture/tldr.md` & `orchestrator_core-1.2.0/docs/architecture/tldr.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/docs/contributing/guidelines.md` & `orchestrator_core-1.2.0/docs/contributing/guidelines.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/docs/contributing/testing.md` & `orchestrator_core-1.2.0/docs/contributing/testing.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/docs/css/termynal.css` & `orchestrator_core-1.2.0/docs/css/termynal.css`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/docs/getting-started/base.md` & `orchestrator_core-1.2.0/docs/getting-started/base.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/docs/getting-started/development.md` & `orchestrator_core-1.2.0/docs/getting-started/development.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/docs/index.md` & `orchestrator_core-1.2.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/docs/js/custom.js` & `orchestrator_core-1.2.0/docs/js/custom.js`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/docs/js/termynal.js` & `orchestrator_core-1.2.0/docs/js/termynal.js`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/docs/workshops/advanced/circuit-workflow.md` & `orchestrator_core-1.2.0/docs/workshops/advanced/circuit-workflow.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/docs/workshops/advanced/docker-installation.md` & `orchestrator_core-1.2.0/docs/workshops/advanced/docker-installation.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/docs/workshops/advanced/domain-models.md` & `orchestrator_core-1.2.0/docs/workshops/advanced/domain-models.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/docs/workshops/advanced/node-workflow.md` & `orchestrator_core-1.2.0/docs/workshops/advanced/node-workflow.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/docs/workshops/advanced/overview.md` & `orchestrator_core-1.2.0/docs/workshops/advanced/overview.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/docs/workshops/advanced/scenario.md` & `orchestrator_core-1.2.0/docs/workshops/advanced/scenario.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/docs/workshops/advanced/workflow-introduction.md` & `orchestrator_core-1.2.0/docs/workshops/advanced/workflow-introduction.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/docs/workshops/beginner/create-user-group.md` & `orchestrator_core-1.2.0/docs/workshops/beginner/create-user-group.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/docs/workshops/beginner/create-user.md` & `orchestrator_core-1.2.0/docs/workshops/beginner/create-user.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/docs/workshops/beginner/database-migration.md` & `orchestrator_core-1.2.0/docs/workshops/beginner/database-migration.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/docs/workshops/beginner/debian.md` & `orchestrator_core-1.2.0/docs/workshops/beginner/debian.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/docs/workshops/beginner/docker.md` & `orchestrator_core-1.2.0/docs/workshops/beginner/docker.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/docs/workshops/beginner/domain-models.md` & `orchestrator_core-1.2.0/docs/workshops/beginner/domain-models.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/docs/workshops/beginner/explore.md` & `orchestrator_core-1.2.0/docs/workshops/beginner/explore.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/docs/workshops/beginner/input-forms.md` & `orchestrator_core-1.2.0/docs/workshops/beginner/input-forms.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/docs/workshops/beginner/macos.md` & `orchestrator_core-1.2.0/docs/workshops/beginner/macos.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/docs/workshops/beginner/modify-user-group.md` & `orchestrator_core-1.2.0/docs/workshops/beginner/modify-user-group.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/docs/workshops/beginner/modify-user.md` & `orchestrator_core-1.2.0/docs/workshops/beginner/modify-user.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/docs/workshops/beginner/overview.md` & `orchestrator_core-1.2.0/docs/workshops/beginner/overview.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/docs/workshops/beginner/register-workflows.md` & `orchestrator_core-1.2.0/docs/workshops/beginner/register-workflows.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/docs/workshops/beginner/scenario.md` & `orchestrator_core-1.2.0/docs/workshops/beginner/scenario.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/docs/workshops/beginner/start-applications.md` & `orchestrator_core-1.2.0/docs/workshops/beginner/start-applications.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/docs/workshops/beginner/terminate-user-group.md` & `orchestrator_core-1.2.0/docs/workshops/beginner/terminate-user-group.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/docs/workshops/beginner/terminate-user.md` & `orchestrator_core-1.2.0/docs/workshops/beginner/terminate-user.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/docs/workshops/beginner/workflow-introduction.md` & `orchestrator_core-1.2.0/docs/workshops/beginner/workflow-introduction.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/docs/workshops/images/metadata_products.png` & `orchestrator_core-1.2.0/docs/workshops/images/metadata_products.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/docs/workshops/images/netbox_devices_active.png` & `orchestrator_core-1.2.0/docs/workshops/images/netbox_devices_active.png`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/examples/basic/basic_orchestrator.py` & `orchestrator_core-1.2.0/examples/basic/basic_orchestrator.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/mkdocs.yml` & `orchestrator_core-1.2.0/mkdocs.yml`

 * *Files 26% similar despite different names*

```diff
@@ -61,14 +61,27 @@
   - Orchestrator Core: index.md
   - Getting Started:
     - Base Application: getting-started/base.md
     - Development setup: getting-started/development.md
   - Architecture:
     - Architecture; TLDR: architecture/tldr.md
     - Orchestration Philosophy: architecture/orchestration/philosophy.md
+    - Product modelling:
+      - Introduction: architecture/product_modelling/introduction.md
+      - Standards: architecture/product_modelling/standards.md
+      - Modelling: architecture/product_modelling/modelling.md
+      - Context: architecture/product_modelling/context.md
+      - Terminology: architecture/product_modelling/terminology.md
+      - Example Product Models:
+        - Node: architecture/product_modelling/node.md
+        - Port: architecture/product_modelling/port.md
+        - L2 Point-to-Point: architecture/product_modelling/l2_point_to_point.md
+        - L2 VPN: architecture/product_modelling/l2_vpn.md
+        - IP Static: architecture/product_modelling/ip_static.md
+      - Product Block Graph: architecture/product_modelling/product_block_graph.md
     - Internals:
       - How do Workflows work?: architecture/application/workflow.md
       - What are tasks?: architecture/application/tasks.md
       - Validating input through forms: architecture/application/forms.md
       - Domain Models: architecture/application/domainmodels.md
     - Documentation:
       - Command Line Interface: architecture/application/cli.md
```

### Comparing `orchestrator_core-1.1.1rc4/mutmut_config.py` & `orchestrator_core-1.2.0/mutmut_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 def pre_mutation(context):
-    """
-    Prepare mutmut context.
+    """Prepare mutmut context.
 
     This helps skipping needless mutations.
     """
     line = context.current_source_line.strip()
     if context.current_line_index != 0:
         prev_line = context.source_by_line_number[context.current_line_index - 1].strip()
     else:
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/__init__.py` & `orchestrator_core-1.2.0/orchestrator/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """This is the orchestrator workflow engine."""
 
-__version__ = "1.1.1rc4"
+__version__ = "1.2.0"
 
 from orchestrator.app import OrchestratorCore
 from orchestrator.settings import app_settings, oauth2_settings
 from orchestrator.workflow import begin, conditional, done, focussteps, inputstep, retrystep, step, steplens, workflow
 
 __all__ = [
     "OrchestratorCore",
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/api/__init__.py` & `orchestrator_core-1.2.0/orchestrator/api/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/api/api_v1/__init__.py` & `orchestrator_core-1.2.0/orchestrator/api/api_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/api/api_v1/api.py` & `orchestrator_core-1.2.0/orchestrator/api/api_v1/api.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/api/api_v1/endpoints/__init__.py` & `orchestrator_core-1.2.0/orchestrator/api/api_v1/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/api/api_v1/endpoints/fixed_input.py` & `orchestrator_core-1.2.0/orchestrator/api/api_v1/endpoints/fixed_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 router = APIRouter()
 
 logger = structlog.get_logger(__name__)
 
 
 @router.get("/configuration", response_model=FixedInputConfigurationSchema)
-def fi_configuration() -> Dict[str, Any]:
+def fi_configuration() -> Dict[str, Any]:  # noqa: C901
     product_tags = products.get_tags()
 
     data: dict = {"fixed_inputs": [], "by_tag": {}}
     for tag in product_tags:
         data["by_tag"][tag] = []
 
     for product_name, model in SUBSCRIPTION_MODEL_REGISTRY.items():
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/api/api_v1/endpoints/health.py` & `orchestrator_core-1.2.0/orchestrator/api/api_v1/endpoints/health.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/api/api_v1/endpoints/processes.py` & `orchestrator_core-1.2.0/orchestrator/api/api_v1/endpoints/processes.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,15 +164,15 @@
 def abort_process_endpoint(pid: UUID, request: Request, user: Optional[OIDCUserModel] = Depends(oidc_user)) -> None:
     process = _get_process(pid)
 
     user_name = user.user_name if user else SYSTEM_USER
     broadcast_func = api_broadcast_process_data(request)
     try:
         abort_process(process, user_name, broadcast_func=broadcast_func)
-        return None
+        return
     except Exception as e:
         raise_status(HTTPStatus.INTERNAL_SERVER_ERROR, str(e))
 
 
 @router.get(
     "/process-subscriptions-by-subscription-id/{subscription_id}", response_model=List[ProcessSubscriptionSchema]
 )
@@ -188,16 +188,15 @@
 
 @router.get("/process-subscriptions-by-pid/{pid}", response_model=List[ProcessSubscriptionBaseSchema])
 def process_subscriptions_by_process_pid(pid: UUID) -> List[ProcessSubscriptionTable]:
     return ProcessSubscriptionTable.query.filter_by(pid=pid).all()
 
 
 def check_global_lock() -> None:
-    """
-    Check the global lock of the engine.
+    """Check the global lock of the engine.
 
     Returns:
         None or raises an exception
 
     """
     engine_settings = EngineSettingsTable.query.one()
     if engine_settings.global_lock:
@@ -234,25 +233,24 @@
 
 
 @router.get("/{pid}", response_model=ProcessSchema)
 def show(pid: UUID) -> Dict[str, Any]:
     process = _get_process(pid)
     p = load_process(process)
 
-    data = show_process(process, p)
-    return data
+    return show_process(process, p)
 
 
 def handle_process_error(message: str, **kwargs: Any) -> None:
     logger.debug(message, **kwargs)
     raise_status(HTTPStatus.BAD_REQUEST, message)
 
 
 @router.get("/", response_model=List[ProcessListItemSchema])
-def processes_filterable(
+def processes_filterable(  # noqa: C901
     response: Response,
     range: Optional[str] = None,
     sort: Optional[str] = None,
     filter: Optional[str] = None,
     if_none_match: Optional[str] = Header(None),
 ) -> List[Dict[str, Any]]:
     _range: Union[List[int], None] = list(map(int, range.split(","))) if range else None
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/api/api_v1/endpoints/product_blocks.py` & `orchestrator_core-1.2.0/orchestrator/api/api_v1/endpoints/product_blocks.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/api/api_v1/endpoints/products.py` & `orchestrator_core-1.2.0/orchestrator/api/api_v1/endpoints/products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/api/api_v1/endpoints/resource_types.py` & `orchestrator_core-1.2.0/orchestrator/api/api_v1/endpoints/resource_types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/api/api_v1/endpoints/settings.py` & `orchestrator_core-1.2.0/orchestrator/api/api_v1/endpoints/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,19 +54,19 @@
     return CACHE_FLUSH_OPTIONS
 
 
 @router.put("/status", response_model=EngineSettingsSchema)
 async def set_global_status(
     body: EngineSettingsBaseSchema, user: Optional[OIDCUserModel] = Depends(oidc_user)
 ) -> EngineSettingsSchema:
-    """
-    Update the global status of the engine to a new state.
+    """Update the global status of the engine to a new state.
 
     Args:
         body: The GlobalStatus object
+        user: The OIDCUser model
 
     Returns:
         The updated global status object
 
     """
 
     engine_settings = EngineSettingsTable.query.with_for_update().one()
@@ -90,36 +90,33 @@
         )
 
     return status_response
 
 
 @router.get("/worker-status", response_model=WorkerStatus)
 def get_worker_status() -> WorkerStatus:
-    """
-    Return data on job workers and queues.
+    """Return data on job workers and queues.
 
     Returns:
     - The number of queued jobs
     - The number of workers
     - The number of running jobs
     - The number of successful and unsuccessful jobs
     """
 
     if app_settings.EXECUTOR == ExecutorType.WORKER:
         from orchestrator.services.tasks import CeleryJobWorkerStatus
 
         return CeleryJobWorkerStatus()
-    else:
-        return ThreadPoolWorkerStatus()
+    return ThreadPoolWorkerStatus()
 
 
 @router.get("/status", response_model=EngineSettingsSchema)
 def get_global_status() -> EngineSettingsSchema:
-    """
-    Retrieve the global status object.
+    """Retrieve the global status object.
 
     Returns:
         The global status of the engine
 
     """
     engine_settings = EngineSettingsTable.query.one()
     return generate_engine_status_response(engine_settings)
@@ -143,30 +140,30 @@
         channel = WS_CHANNELS.ENGINE_SETTINGS
         await websocket_manager.connect(websocket, channel)
 
 
 def generate_engine_status_response(
     engine_settings: EngineSettingsTable,
 ) -> EngineSettingsSchema:
-    """
-    Generate the correct engine status response.
+    """Generate the correct engine status response.
 
     Args:
         engine_settings: Engine settings database object
 
     Returns:
         Engine StatusEnum
 
     """
 
     if engine_settings.global_lock and engine_settings.running_processes > 0:
         result = EngineSettingsSchema.from_orm(engine_settings)
         result.global_status = GlobalStatusEnum.PAUSING
         return result
-    elif engine_settings.global_lock and engine_settings.running_processes == 0:
+
+    if engine_settings.global_lock and engine_settings.running_processes == 0:
         result = EngineSettingsSchema.from_orm(engine_settings)
         result.global_status = GlobalStatusEnum.PAUSED
         return result
 
     result = EngineSettingsSchema.from_orm(engine_settings)
     result.global_status = GlobalStatusEnum.RUNNING
     return result
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py` & `orchestrator_core-1.2.0/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/api/api_v1/endpoints/subscriptions.py` & `orchestrator_core-1.2.0/orchestrator/api/api_v1/endpoints/subscriptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,16 +72,15 @@
         ProcessStepTable.query.filter(ProcessStepTable.pid == pid).delete()
         ProcessTable.query.filter(ProcessTable.pid == pid).delete()
         subscription = SubscriptionTable.query.filter(SubscriptionTable.subscription_id == subscription_id).first()
         _delete_subscription_tree(subscription)
 
 
 def _filter_statuses(filter_statuses: Optional[str] = None) -> List[str]:
-    """
-    Check valid filter statuses.
+    """Check valid filter statuses.
 
     Args:
         filter_statuses: the filters.
 
     Returns:
         list of filters
 
@@ -133,30 +132,28 @@
 
 
 @router.delete("/{subscription_id}", response_model=None)
 def delete_subscription(subscription_id: UUID) -> None:
     all_process_subscriptions = ProcessSubscriptionTable.query.filter_by(subscription_id=subscription_id).all()
     if len(all_process_subscriptions) > 0:
         _delete_process_subscriptions(all_process_subscriptions)
-        return None
-    else:
-        subscription = SubscriptionTable.query.filter(SubscriptionTable.subscription_id == subscription_id).first()
-        if not subscription:
-            raise_status(HTTPStatus.NOT_FOUND)
+        return
+    subscription = SubscriptionTable.query.filter(SubscriptionTable.subscription_id == subscription_id).first()
+    if not subscription:
+        raise_status(HTTPStatus.NOT_FOUND)
 
-        _delete_subscription_tree(subscription)
-        return None
+    _delete_subscription_tree(subscription)
+    return
 
 
 @router.get("/in_use_by/{subscription_id}", response_model=List[SubscriptionSchema])
 def in_use_by_subscriptions(
     subscription_id: UUID, filter_statuses: List[str] = Depends(_filter_statuses)
 ) -> List[SubscriptionTable]:
-    """
-    Retrieve subscriptions that are in use by this subscription.
+    """Retrieve subscriptions that are in use by this subscription.
 
     Args:
         subscription_id: Subscription to query
         filter_statuses: List of filters
 
     Returns:
         list of subscriptions
@@ -182,16 +179,15 @@
 
 
 @router.get("/depends_on/{subscription_id}", response_model=List[SubscriptionSchema])
 def depends_on_subscriptions(
     subscription_id: UUID,
     filter_statuses: List[str] = Depends(_filter_statuses),
 ) -> List[SubscriptionTable]:
-    """
-    Retrieve dependant subscriptions.
+    """Retrieve dependant subscriptions.
 
     Args:
         subscription_id: The subscription id
         filter_statuses: the status of dependant subscriptions
 
     Returns:
         List of dependant subscriptions.
@@ -200,16 +196,15 @@
     return query_depends_on_subscriptions(subscription_id, filter_statuses).all()
 
 
 @router.get("/", response_model=List[SubscriptionSchema])
 def subscriptions_filterable(
     response: Response, range: Optional[str] = None, sort: Optional[str] = None, filter: Optional[str] = None
 ) -> List[SubscriptionTable]:
-    """
-    Get subscriptions filtered.
+    """Get subscriptions filtered.
 
     Args:
         response: Fastapi Response object
         range: Range
         sort: Sort
         filter: Filter
 
@@ -220,16 +215,15 @@
     _range: Union[List[int], None] = list(map(int, range.split(","))) if range else None
     _sort: Union[List[str], None] = sort.split(",") if sort else None
     _filter: Union[List[str], None] = filter.split(",") if filter else None
     logger.info("subscriptions_filterable() called", range=_range, sort=_sort, filter=_filter)
     query = SubscriptionTable.query.join(SubscriptionTable.product).options(
         contains_eager(SubscriptionTable.product), defer("product_id")
     )
-    query_result = _query_with_filters(response, query, _range, _sort, _filter)
-    return query_result
+    return _query_with_filters(response, query, _range, _sort, _filter)
 
 
 @router.get(
     "/workflows/{subscription_id}", response_model=SubscriptionWorkflowListsSchema, response_model_exclude_none=True
 )
 def subscription_workflows_by_id(subscription_id: UUID) -> Dict[str, List[Dict[str, Union[List[Any], str]]]]:
     subscription = SubscriptionTable.query.options(joinedload("product"), joinedload("product.workflows")).get(
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/api/api_v1/endpoints/translations.py` & `orchestrator_core-1.2.0/orchestrator/api/api_v1/endpoints/translations.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,10 +21,8 @@
 
 
 router = APIRouter()
 
 
 @router.get("/{language}", response_model=dict)
 def get_translations(language: str = Path(..., regex="^[a-z]+-[A-Z]+$")) -> dict:
-    translations = generate_translations(language)
-
-    return translations
+    return generate_translations(language)
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/api/api_v1/endpoints/user.py` & `orchestrator_core-1.2.0/orchestrator/api/api_v1/endpoints/user.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/api/api_v1/endpoints/workflows.py` & `orchestrator_core-1.2.0/orchestrator/api/api_v1/endpoints/workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/api/error_handling.py` & `orchestrator_core-1.2.0/orchestrator/api/error_handling.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/api/helpers.py` & `orchestrator_core-1.2.0/orchestrator/api/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     try:
         return " ".join([_quote_if_kv_pair(token) for token in lex])
     except ValueError:
         logger.debug("Error parsing text query.")
         return q
 
 
-def _query_with_filters(
+def _query_with_filters(  # noqa: C901
     response: Response,
     query: Query,
     range: Optional[List[int]] = None,
     sort: Optional[List[str]] = None,
     filters: Optional[List[str]] = None,
 ) -> List:
     if filters is not None:
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/api/models.py` & `orchestrator_core-1.2.0/orchestrator/api/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,17 +90,16 @@
 
 
 def delete(cls: Type, primary_key: UUID) -> None:
     pk = list({k: v for k, v in cls.__table__.columns._collection if v.primary_key}.keys())[0]
     row_count = cls.query.filter(cls.__dict__[pk] == primary_key).delete()
     db.session.commit()
     if row_count > 0:
-        return None
-    else:
-        raise_status(HTTPStatus.NOT_FOUND)
+        return
+    raise_status(HTTPStatus.NOT_FOUND)
 
 
 deserialization_mapping = {
     "steps": ProcessStepTable,
     "subscriptions": ProcessSubscriptionTable,
     "product_blocks": ProductBlockTable,
     "fixed_inputs": FixedInputTable,
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/app.py` & `orchestrator_core-1.2.0/orchestrator/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,44 +13,39 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Any, Callable, Dict, Optional, Type
 
 import sentry_sdk
 import structlog
 import typer
+from deprecated import deprecated
 from fastapi.applications import FastAPI
 from fastapi_etag.dependency import add_exception_handler
-from nwastdlib.logging import ClearStructlogContextASGIMiddleware, initialise_logging
-from opentelemetry import trace
-from opentelemetry.instrumentation.fastapi import FastAPIInstrumentor
-from opentelemetry.instrumentation.httpx import HTTPXClientInstrumentor
-from opentelemetry.instrumentation.psycopg2 import Psycopg2Instrumentor
-from opentelemetry.instrumentation.redis import RedisInstrumentor
-from opentelemetry.instrumentation.sqlalchemy import SQLAlchemyInstrumentor
 from pydantic.json import ENCODERS_BY_TYPE
 from sentry_sdk.integrations.fastapi import FastApiIntegration
 from sentry_sdk.integrations.redis import RedisIntegration
 from sentry_sdk.integrations.sqlalchemy import SqlalchemyIntegration
 from starlette.middleware.cors import CORSMiddleware
 from starlette.middleware.sessions import SessionMiddleware
 from starlette.responses import JSONResponse, Response
 
+from nwastdlib.logging import ClearStructlogContextASGIMiddleware, initialise_logging
 from orchestrator import __version__
 from orchestrator.api.api_v1.api import api_router
 from orchestrator.api.error_handling import ProblemDetailException
 from orchestrator.cli.main import app as cli_app
 from orchestrator.db import db, init_database
 from orchestrator.db.database import DBSessionMiddleware
 from orchestrator.distlock import init_distlock_manager
 from orchestrator.domain import SUBSCRIPTION_MODEL_REGISTRY, SubscriptionModel
 from orchestrator.exception_handlers import form_error_handler, problem_detail_handler
-from orchestrator.forms import FormException
+from orchestrator.forms import FormError
 from orchestrator.graphql import graphql_router
 from orchestrator.services.processes import ProcessDataBroadcastThread
-from orchestrator.settings import AppSettings, app_settings, tracer_provider
+from orchestrator.settings import AppSettings, app_settings
 from orchestrator.utils.vlans import VlanRanges
 from orchestrator.version import GIT_COMMIT_HASH
 from orchestrator.websocket import init_websocket_manager
 
 logger = structlog.get_logger(__name__)
 
 
@@ -110,30 +105,25 @@
             CORSMiddleware,
             allow_origins=origins,
             allow_methods=base_settings.CORS_ALLOW_METHODS,
             allow_headers=base_settings.CORS_ALLOW_HEADERS,
             expose_headers=base_settings.CORS_EXPOSE_HEADERS,
         )
 
-        self.add_exception_handler(FormException, form_error_handler)
+        self.add_exception_handler(FormError, form_error_handler)
         self.add_exception_handler(ProblemDetailException, problem_detail_handler)
         add_exception_handler(self)
 
         @self.router.get("/", response_model=str, response_class=JSONResponse, include_in_schema=False)
         def _index() -> str:
             return "Orchestrator orchestrator"
 
+    @deprecated("Not using Opentelemetry from version 1.2.0, removing after version 1.3.0")
     def instrument_app(self) -> None:
-        logger.info("Activating Opentelemetry tracing to app", app=self.title)
-        trace.set_tracer_provider(tracer_provider)
-        FastAPIInstrumentor.instrument_app(self)
-        HTTPXClientInstrumentor().instrument()
-        RedisInstrumentor().instrument()
-        Psycopg2Instrumentor().instrument()
-        SQLAlchemyInstrumentor().instrument(engine=db.engine, tracer_provider=tracer_provider)
+        pass
 
     def add_sentry(
         self,
         sentry_dsn: str,
         trace_sample_rate: float,
         server_name: str,
         environment: str,
@@ -142,23 +132,22 @@
         logger.info("Adding Sentry middleware to app", app=self.title)
         sentry_sdk.init(
             dsn=sentry_dsn,
             traces_sample_rate=trace_sample_rate,
             server_name=server_name,
             environment=environment,
             release=f"orchestrator@{release}",
-            integrations=[SqlalchemyIntegration(), RedisIntegration(), FastApiIntegration(transaction_style="url")],
+            integrations=[SqlalchemyIntegration(), RedisIntegration(), FastApiIntegration()],
             propagate_traces=True,
             profiles_sample_rate=trace_sample_rate,
         )
 
     @staticmethod
     def register_subscription_models(product_to_subscription_model_mapping: Dict[str, Type[SubscriptionModel]]) -> None:
-        """
-        Register your subscription models.
+        """Register your subscription models.
 
         This method is needed to register your subscription models inside the orchestrator core.
 
         Args:
             product_to_subscription_model_mapping: The dictionary should contain a mapping of products to SubscriptionModels.
                 The selection will be done depending on the name of the product.
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/cli/__init__.py` & `orchestrator_core-1.2.0/orchestrator/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/cli/database.py` & `orchestrator_core-1.2.0/orchestrator/cli/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,16 +54,15 @@
     return cfg
 
 
 @app.command(
     help="Initialize an empty migrations environment. This command will throw an exception when it detects conflicting files and directories."
 )
 def init() -> None:
-    """
-    Initialize the migrations directory.
+    """Initialize the migrations directory.
 
     This command will initialize a migration directory for the orchestrator core application and setup a correct
     migration environment.
 
     Returns:
         None
 
@@ -114,47 +113,44 @@
 @app.command(help="Merge database revisions.")
 def merge(
     revisions: Optional[List[str]] = typer.Argument(
         None, help="Add the revision you would like to merge to this command."
     ),
     message: str = typer.Option(None, "--message", "-m", help="The revision message"),
 ) -> None:
-    """
-    Merge database revisions.
+    """Merge database revisions.
 
     Args:
         revisions: List of revisions to merge
         message: Optional message for the revision.
 
     Returns:
         None
 
     """
     command.merge(alembic_cfg(), revisions, message=message)
 
 
 @app.command()
 def upgrade(revision: Optional[str] = typer.Argument(None, help="Rev id to upgrade to")) -> None:
-    """
-    Upgrade the database.
+    """Upgrade the database.
 
     Args:
         revision: Optional argument to indicate where to upgrade to.
 
     Returns:
         None
 
     """
     command.upgrade(alembic_cfg(), revision)
 
 
 @app.command()
 def downgrade(revision: Optional[str] = typer.Argument("-1", help="Rev id to upgrade to")) -> None:
-    """
-    Downgrade the database.
+    """Downgrade the database.
 
     Args:
         revision: Optional argument to indicate where to downgrade to.
 
     Returns:
         None
 
@@ -165,16 +161,15 @@
 @app.command()
 def revision(
     message: str = typer.Option(None, "--message", "-m", help="The revision message"),
     version_path: str = typer.Option(None, "--version-path", help="Specify specific path from config for version file"),
     autogenerate: bool = typer.Option(False, help="Detect schema changes and add migrations"),
     head: str = typer.Option(None, help="Determine the head you need to add your migration to."),
 ) -> None:
-    """
-    Create a new revision file.
+    """Create a new revision file.
 
     Args:
         message: The revision message
         version_path: Specify specific path from config for version file
         autogenerate: Whether to detect schema changes.
         head: To which head the migration applies
 
@@ -186,16 +181,15 @@
 
 
 @app.command()
 def history(
     verbose: bool = typer.Option(False, "--verbose", "-v", help="Verbose output"),
     indicate_current: bool = typer.Option(False, "--current", "-c", help="Indicate current revision"),
 ) -> None:
-    """
-    List changeset scripts in chronological order.
+    """List changeset scripts in chronological order.
 
     Args:
         verbose: Verbose output
         indicate_current: Indicate current revision
 
     Returns:
         None
@@ -213,32 +207,32 @@
 ) -> Union[Tuple[List[str], List[str]], None]:
     """Create migration file based on SubscriptionModel.diff_product_in_database. BACKUP DATABASE BEFORE USING THE MIGRATION!.
 
     You will be prompted with inputs for new models and resource type updates.
     Resource type updates are only handled when it's renamed in all product blocks.
 
     Args:
-    - `message`: Message/description of the generated migration.
-    - `--test`: Optional boolean if you don't want to generate a migration file.
-    - `--inputs`: stringified dict to prefill inputs.
-        The inputs and updates argument is mostly used for testing, prefilling the given inputs, here examples:
-        - new product: `inputs = { "new_product_name": { "description": "add description", "product_type": "add_type", "tag": "add_tag" }}`
-        - new product fixed input: `inputs = { "new_product_name": { "new_fixed_input_name": "value" }}`
-        - new product block: `inputs = { "new_product_block_name": { "description": "add description", "tag": "add_tag" } }`
-        - new resource type: `inputs = { "new_resource_type_name": { "description": "add description", "value": "add default value", "new_product_block_name": "add default value for block" }}`
-            - `new_product_block_name` prop inserts value specifically for that block.
-            - `value` prop is inserted as default for all existing instances it is added to.
-
-    - `--updates`: stringified dict to prefill inputs.
-        - renaming a fixed input:
-            - `updates = { "fixed_inputs": { "product_name": { "old_fixed_input_name": "new_fixed_input_name" } } }`
-        - renaming a resource type to a new resource type:
-            - `inputs = { "new_resource_type_name": { "description": "add description" }}`
-            - `updates = { "resource_types": { "old_resource_type_name": "new_resource_type_name" } }`
-        - renaming a resource type to existing resource type: `updates = { "resource_types": { "old_resource_type_name": "new_resource_type_name" } }`
+        message: Message/description of the generated migration.
+        test: Optional boolean if you don't want to generate a migration file.
+        inputs: stringified dict to prefill inputs.
+            The inputs and updates argument is mostly used for testing, prefilling the given inputs, here examples:
+            - new product: `inputs = { "new_product_name": { "description": "add description", "product_type": "add_type", "tag": "add_tag" }}`
+            - new product fixed input: `inputs = { "new_product_name": { "new_fixed_input_name": "value" }}`
+            - new product block: `inputs = { "new_product_block_name": { "description": "add description", "tag": "add_tag" } }`
+            - new resource type: `inputs = { "new_resource_type_name": { "description": "add description", "value": "add default value", "new_product_block_name": "add default value for block" }}`
+                - `new_product_block_name` prop inserts value specifically for that block.
+                - `value` prop is inserted as default for all existing instances it is added to.
+
+        updates: stringified dict to prefill inputs.
+            - renaming a fixed input:
+                - `updates = { "fixed_inputs": { "product_name": { "old_fixed_input_name": "new_fixed_input_name" } } }`
+            - renaming a resource type to a new resource type:
+                - `inputs = { "new_resource_type_name": { "description": "add description" }}`
+                - `updates = { "resource_types": { "old_resource_type_name": "new_resource_type_name" } }`
+            - renaming a resource type to existing resource type: `updates = { "resource_types": { "old_resource_type_name": "new_resource_type_name" } }`
 
     Returns None unless `--test` is used, in which case it returns:
         - tuple:
             - list of upgrade SQL statements in string format.
             - list of downgrade SQL statements in string format.
     """
     if not app_settings.TESTING:
@@ -276,16 +270,16 @@
 ) -> Union[Tuple[List[dict], List[dict]], None]:
     """Create a migration file based on the difference between workflows in the database and registered WorkflowInstances. BACKUP DATABASE BEFORE USING THE MIGRATION!.
 
     You will be prompted with inputs for new models and resource type updates.
     Resource type updates are only handled when it's renamed in all product blocks.
 
     Args:
-    - `message`: Message/description of the generated migration.
-    - `--test`: Optional boolean if you don't want to generate a migration file.
+        message: Message/description of the generated migration.
+        test: Optional boolean if you don't want to generate a migration file.
 
     Returns None unless `--test` is used, in which case it returns:
         - tuple:
             - list of upgrade SQL statements in string format.
             - list of downgrade SQL statements in string format.
     """
     if not app_settings.TESTING:
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py` & `orchestrator_core-1.2.0/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 from orchestrator.db.models import FixedInputTable
 
 
 def map_update_fixed_inputs(product_diffs: Dict[str, Dict[str, Set[str]]]) -> Dict[str, Dict[str, str]]:
     """Map fixed inputs to update.
 
     Args:
-        - product_diffs: Dict with product differences.
+        product_diffs: Dict with product differences.
             - key: product name
             - value: Dict with differences between model and database.
                 - key: difference name, 'missing_fixed_inputs_in_model' and 'missing_fixed_inputs_in_db' are used to check if a fixed input can be renamed.
                 - value: Set of fixed input names.
 
     Returns: Dict with updated fixed inputs mapped by product.
-        - key: product name.
-        - value: Dict with updated fixed inputs.
+        key: product name.
+        value: Dict with updated fixed inputs.
             - key: old fixed input name.
             - value: new fixed input name.
     """
     print_fmt("\nUpdate fixed inputs", flags=[COLOR.BOLD, COLOR.UNDERLINE])
 
     def rename_map(product_name: str, product_diff: Dict[str, Set[str]]) -> Dict[str, str]:
         db_props = list(product_diff.get("missing_fixed_inputs_in_model", []))
@@ -61,23 +61,23 @@
 
 def generate_create_fixed_inputs_sql(
     fixed_inputs: Dict[str, Set[str]], inputs: Dict[str, Dict[str, str]], revert: bool = False
 ) -> List[str]:
     """Generate SQL to create fixed inputs.
 
     Args:
-        - fixed_inputs: Dict with product names by fixed input.
+        fixed_inputs: Dict with product names by fixed input.
             - key: fixed input value.
             - value: product names.
-        - inputs: Optional Dict to prefill fixed input 'value' per product.
+        inputs: Optional Dict to prefill fixed input 'value' per product.
             - key: fixed input name.
             - value: Dict with prefilled value.
                 - key: 'value' as key.
                 - value: prefilled value.
-        - revert: boolean to create SQL string with value filled by the database.
+        revert: boolean to create SQL string with value filled by the database.
 
     Returns: List of SQL to create fixed inputs.
     """
     print_fmt("\nCreate fixed inputs", flags=[COLOR.BOLD, COLOR.UNDERLINE])
 
     def create_fixed_input(fixed_input: str, product_names: Set[str]) -> str:
         def create_product_insert_dict(product_name: str) -> Dict[str, Union[str, ScalarSelect]]:
@@ -111,15 +111,15 @@
     return [create_fixed_input(*item) for item in fixed_inputs.items()]
 
 
 def generate_delete_fixed_inputs_sql(fixed_inputs: Dict[str, Set[str]]) -> List[str]:
     """Generate SQL to delete fixed inputs.
 
     Args:
-        - fixed_inputs: Dict with product names by fixed input.
+        fixed_inputs: Dict with product names by fixed input.
             - key: fixed input value.
             - value: product names.
 
     Returns: List of SQL strings to delete fixed inputs.
     """
 
     def delete_fixed_input(fixed_input: str, product_names: Set[str]) -> str:
@@ -136,15 +136,15 @@
     return [delete_fixed_input(*item) for item in fixed_inputs.items()]
 
 
 def generate_update_fixed_inputs_sql(product_fixed_inputs: Dict[str, Dict[str, str]]) -> List[str]:
     """Generate SQL to update fixed inputs.
 
     Args:
-        - product_fixed_inputs: Dict with product names by fixed input.
+        product_fixed_inputs: Dict with product names by fixed input.
             - key: fixed input value.
             - value: product names.
 
     Returns: List of SQL strings to update fixed inputs.
     """
 
     def update_fixed_inputs(product_name: str, fixed_inputs: Dict[str, str]) -> List[str]:
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/cli/domain_gen_helpers/helpers.py` & `orchestrator_core-1.2.0/orchestrator/cli/domain_gen_helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/cli/domain_gen_helpers/product_block_helpers.py` & `orchestrator_core-1.2.0/orchestrator/cli/domain_gen_helpers/product_block_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,44 +42,44 @@
     )
 
 
 def map_create_product_blocks(product_blocks: Dict[str, Type[ProductBlockModel]]) -> Dict[str, Type[ProductBlockModel]]:
     """Map product blocks to create.
 
     Args:
-        - product_blocks: Dict of product blocks mapped by product block name.
+        product_blocks: Dict of product blocks mapped by product block name.
 
     Returns: Dict of product blocks by product block name to create.
     """
     _existing_product_blocks = ProductBlockTable.query.with_entities(ProductBlockTable.name).all()
     existing_product_blocks = {block_name[0] for block_name in _existing_product_blocks}
     return {
         block_name: block for block_name, block in product_blocks.items() if block_name not in existing_product_blocks
     }
 
 
 def map_delete_product_blocks(product_blocks: Dict[str, Type[ProductBlockModel]]) -> Set[str]:
     """Map product blocks to delete.
 
     Args:
-        - product_blocks: Dict of product blocks mapped by product block name.
+        product_blocks: Dict of product blocks mapped by product block name.
 
     Returns: List of product block names to delete.
     """
     existing_product_blocks = ProductBlockTable.query.with_entities(ProductBlockTable.name).all()
     return {name[0] for name in existing_product_blocks if name[0] not in product_blocks}
 
 
 def map_product_block_additional_relations(changes: DomainModelChanges) -> DomainModelChanges:
     """Map additional relations for created product blocks.
 
     Adds resource type and product block relations.
 
     Args:
-        - changes: DomainModelChanges class with all changes.
+        changes: DomainModelChanges class with all changes.
 
     Returns: Updated DomainModelChanges.
     """
 
     for block_name, block_class in changes.create_product_blocks.items():
         for field_name in block_class._non_product_block_fields_.keys():
             changes.create_resource_type_relations.setdefault(field_name, set()).add(block_name)
@@ -93,16 +93,16 @@
 
 def generate_create_product_blocks_sql(
     create_product_blocks: Dict[str, Any], inputs: Dict[str, Dict[str, str]]
 ) -> List[str]:
     """Generate SQL to create product blocks.
 
     Args:
-        - create_product_blocks: List of product block names.
-        - inputs: Optional Dict to prefill 'description' and 'tag' per product block.
+        create_product_blocks: List of product block names.
+        inputs: Optional Dict to prefill 'description' and 'tag' per product block.
             - key: product block name.
             - value: Dict with 'description' and 'tag'.
                 - key: product block property.
                 - value: value for the property.
 
     Returns: List of SQL to create product blocks.
     """
@@ -127,15 +127,15 @@
     return [create_product_block(name) for name in create_product_blocks]
 
 
 def generate_delete_product_blocks_sql(delete_product_blocks: Set[str]) -> List[str]:
     """Generate SQL to delete product blocks.
 
     Args:
-        - delete_product_blocks: List of product block names.
+        delete_product_blocks: List of product block names.
 
     Returns: List of SQL to delete product blocks.
     """
 
     if not delete_product_blocks:
         return []
     return [
@@ -148,15 +148,15 @@
     ]
 
 
 def generate_create_product_block_relations_sql(create_block_relations: Dict[str, Set[str]]) -> List[str]:
     """Generate SQL to create product block to product block relations.
 
     Args:
-        - create_block_relations: Dict with product blocks by product block
+        create_block_relations: Dict with product blocks by product block
             - key: product block name.
             - value: Set of product block names to relate with.
 
     Returns: List of SQL to create relation between product blocks.
     """
 
     def create_block_relation(depends_block_name: str, block_names: Set[str]) -> str:
@@ -172,15 +172,15 @@
     return [create_block_relation(*item) for item in create_block_relations.items()]
 
 
 def generate_create_product_block_instance_relations_sql(product_block_relations: Dict[str, Set[str]]) -> List[str]:
     """Generate SQL to create resource type instance values for existing instances.
 
     Args:
-        - product_block_relations: Dict with product blocks by resource type
+        product_block_relations: Dict with product blocks by resource type
             - key: product block name.
             - value: Set of product block names to relate to.
 
     Returns: .
     """
 
     def create_subscription_instance_relations(
@@ -231,15 +231,15 @@
     )
 
 
 def generate_delete_product_block_relations_sql(delete_block_relations: Dict[str, Set[str]]) -> List[str]:
     """Generate SQL to delete product block to product blocks relations.
 
     Args:
-        - delete_block_relations: Dict with product blocks by product block
+        delete_block_relations: Dict with product blocks by product block
             - key: Product block name.
             - value: Set of product block names to relate with.
 
     Returns: List of SQL to delete relations between product blocks.
     """
 
     def delete_block_relation(delete_block_name: str, block_names: Set[str]) -> str:
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/cli/domain_gen_helpers/product_helpers.py` & `orchestrator_core-1.2.0/orchestrator/cli/domain_gen_helpers/product_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 def map_product_additional_relations(changes: DomainModelChanges) -> DomainModelChanges:
     """Map additional relations for created products.
 
     Adds resource type and product block relations.
 
     Args:
-        - changes: DomainModelChanges class with all changes.
+        changes: DomainModelChanges class with all changes.
 
     Returns: Updated DomainModelChanges.
     """
 
     for product_name, product_class in changes.create_products.items():
         for field_name in product_class._non_product_block_fields_.keys():
             changes.create_product_fixed_inputs.setdefault(field_name, set()).add(product_name)
@@ -56,18 +56,18 @@
 
 def generate_create_products_sql(
     create_products: Dict[str, Type[SubscriptionModel]], inputs: Dict[str, Dict[str, str]]
 ) -> List[str]:
     """Generate SQL to create products.
 
     Args:
-        - create_products: Dict of SubscriptionModels by product name.
+        create_products: Dict of SubscriptionModels by product name.
             - key: product name.
             - value: SubscriptionModel
-        - inputs: Optional Dict to add prefilled values for 'description', 'product_type' and 'tag' per product.
+        inputs: Optional Dict to add prefilled values for 'description', 'product_type' and 'tag' per product.
             - key: product name.
             - value: Dict with 'description', 'product_type' and 'tag'.
                 - key: product property.
                 - value: value for the property.
 
     Returns: List of SQL strings to create products.
     """
@@ -95,15 +95,15 @@
     ]
 
 
 def generate_delete_products_sql(delete_products: Set[str]) -> List[str]:
     """Generate SQL to delete products.
 
     Args:
-        - delete_products: List of product names.
+        delete_products: List of product names.
 
     Returns: List of SQL strings to delete products.
     """
     if not delete_products:
         return []
 
     def delete_product_relations_sql(product_names: Set[str]) -> List[str]:
@@ -137,15 +137,15 @@
     return sql_deletes
 
 
 def generate_create_product_relations_sql(create_block_relations: Dict[str, Set[str]]) -> List[str]:
     """Generate SQL to create product relations to product blocks.
 
     Args:
-        - create_block_relations: Dict with product names by product block
+        create_block_relations: Dict with product names by product block
             - key: product block name.
             - value: Set of product names to relate with.
 
     Returns: List of SQL strings to create subscription instances.
     """
 
     def create_block_relation(block_name: str, product_names: Set[str]) -> str:
@@ -163,15 +163,15 @@
     return [create_block_relation(*item) for item in create_block_relations.items()]
 
 
 def generate_create_product_instance_relations_sql(product_to_block_relations: Dict[str, Set[str]]) -> List[str]:
     """Generate SQL to create subscription instances for existing subscriptions.
 
     Args:
-        - product_to_block_relations: Dict with product blocks by resource type
+        product_to_block_relations: Dict with product blocks by resource type
             - key: product block name.
             - value: Set of product names to relate with.
 
     Returns: List of SQL strings to create subscription instances.
     """
 
     def create_subscription_instance_relations(block_name: str, product_names: Set[str]) -> Generator[str, None, None]:
@@ -203,15 +203,15 @@
     )
 
 
 def generate_delete_product_relations_sql(delete_block_relations: Dict[str, Set[str]]) -> List[str]:
     """Generate SQL to delete product to product blocks relations.
 
     Args:
-        - delete_block_relations: Dict with product blocks by resource type
+        delete_block_relations: Dict with product blocks by resource type
             - key: product block name.
             - value: Set of product names to relate with.
 
     Returns: List of SQL strings to delete relations between product and product block.
     """
 
     def delete_block_relation(delete_block_name: str, product_names: Set[str]) -> str:
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py` & `orchestrator_core-1.2.0/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,16 +38,16 @@
     )
 
 
 def map_create_resource_types(resource_type_names: Set[str], updated_resource_types: Set[str]) -> Set[str]:
     """Map resource types to create.
 
     Args:
-        - resource_types: List of resource type names.
-        - updated_resource_types: List of resource types that get renamed and don't need to be created.
+        resource_type_names: List of resource type names.
+        updated_resource_types: List of resource types that get renamed and don't need to be created.
 
     Returns: List of resource type names that can be created.
     """
     existing_resource_types = (
         ResourceTypeTable.query.where(ResourceTypeTable.resource_type.in_(resource_type_names))
         .with_entities(ResourceTypeTable.resource_type)
         .all()
@@ -58,16 +58,16 @@
 
 def find_resource_within_blocks(
     resource_type_names: List[str], product_blocks: Dict[str, Type[ProductBlockModel]]
 ) -> Set[str]:
     """Find resource types within product blocks.
 
     Args:
-        - resource_type_names: List of resource type names.
-        - product_blocks: Dict of product blocks mapped by product block name, used to check if the resource type still exists in a product block that hasn't changed.
+        resource_type_names: List of resource type names.
+        product_blocks: Dict of product blocks mapped by product block name, used to check if the resource type still exists in a product block that hasn't changed.
 
     Returns: List of the resource_type_names that are found within product blocks.
     """
     keys = flatten([product_block._non_product_block_fields_.keys() for product_block in product_blocks.values()])
     return {field_name for field_name in keys if field_name in resource_type_names}
 
 
@@ -96,20 +96,20 @@
 def map_rename_resource_types(
     block_diffs: Dict[str, Dict[str, Set[str]]],
     product_blocks: Dict[str, Type[ProductBlockModel]],
 ) -> Dict[str, str]:
     """Map resource types to rename.
 
     Args:
-        - block_diffs: Dict with product block differences.
+        block_diffs: Dict with product block differences.
             - key: product block name
             - value: Dict with differences between model and database.
                 - key: difference name, 'missing_resource_types_in_model' and 'missing_resource_types_in_db' are used to check if a resource type can be renamed.
                 - value: Set of resource type names.
-        - product_blocks: Dict of product blocks mapped by product block name, used to check if the resource type still exists in a product block.
+        product_blocks: Dict of product blocks mapped by product block name, used to check if the resource type still exists in a product block.
 
     Returns: Dict with resource types that can be updated.
         - key: old resource type name.
         - value: new resource type name.
     """
 
     renamed_resource_types: Dict[str, str] = {}
@@ -175,20 +175,20 @@
 def map_update_product_block_resource_types(
     block_diffs: Dict[str, Dict[str, Set[str]]],
     renamed_resource_types: Dict[str, str],
 ) -> Dict[str, Dict[str, str]]:
     """Map resource types to update per product block.
 
     Args:
-        - block_diffs: Dict with product block differences.
+        block_diffs: Dict with product block differences.
             - key: product block name.
             - value: Dict with differences between model and database.
                 - key: difference name, 'missing_resource_types_in_model' and 'missing_resource_types_in_db' are used to check if a resource type can be renamed.
                 - value: Set of resource type names.
-        - renamed_resource_types: Dict of renamed resource types, old name as key and new name as value.
+        renamed_resource_types: Dict of renamed resource types, old name as key and new name as value.
 
     Returns: Dict with resource types per product block that can be updated.
         - key: product block name.
         - value: Dict with resource types to update.
             - key: old resource type name.
             - value: new resource type name.
     """
@@ -218,17 +218,17 @@
     resource_types: Dict[str, Set[str]],
     updated_resource_types: List[str],
     product_blocks: Dict[str, Type[ProductBlockModel]],
 ) -> Set[str]:
     """Map resource types to delete.
 
     Args:
-        - resource_types: List of resource type names.
-        - updated_resource_types: List of resource types that get renamed and shouldn't be deleted.
-        - product_blocks: Dict of product blocks mapped by product block name, used to check if the resource type still exists in a product block.
+        resource_types: List of resource type names.
+        updated_resource_types: List of resource types that get renamed and shouldn't be deleted.
+        product_blocks: Dict of product blocks mapped by product block name, used to check if the resource type still exists in a product block.
 
     Returns: List of resource type names that can be deleted.
     """
     resource_type_names = resource_types.keys()
     existing_resource_types = (
         ResourceTypeTable.query.where(ResourceTypeTable.resource_type.in_(resource_type_names))
         .with_entities(ResourceTypeTable.resource_type)
@@ -261,15 +261,15 @@
 
 def map_create_resource_type_instances(changes: DomainModelChanges) -> Dict[str, Set[str]]:
     """Map resource types that need a default value.
 
     Resource types need a default value when the related product block is used in an existing instance or will be used in an existing instance.
 
     Args:
-        - changes: DomainModelChanges class with all changes.
+        changes: DomainModelChanges class with all changes.
 
     Returns: Dict with resource types that need a default value.
         - key: resource type name.
         - value: set of product block names.
     """
 
     def _has_existing_instances(block_name: str) -> bool:
@@ -292,20 +292,21 @@
 
 def generate_create_resource_types_sql(
     resource_types: Set[str], inputs: Dict[str, Dict[str, str]], revert: bool = False
 ) -> List[str]:
     """Generate SQL to create resource types.
 
     Args:
-        - resource_types: List of resource type names.
-        - inputs: Optional Dict to add default value to the resource type for existing product block instances.
+        resource_types: List of resource type names.
+        inputs: Optional Dict to add default value to the resource type for existing product block instances.
             - key: Resource type name.
             - value: Dict with product block by default value.
                 - key: Product block name.
                 - value: Default value for the resource type.
+        revert: Revert bool
 
     Returns: List of SQL strings to create resource type.
     """
     print_fmt("\nCreate resource types", flags=[COLOR.BOLD, COLOR.UNDERLINE])
 
     def create_resource_type(resource_type: str) -> str:
         if revert:
@@ -326,15 +327,15 @@
     return [create_resource_type(resource_type) for resource_type in resource_types]
 
 
 def generate_rename_resource_types_sql(resource_types: Dict[str, str]) -> List[str]:
     """Generate SQL to update resource types.
 
     Args:
-        - resource_types: Dict with new resource type name by old resource type name.
+        resource_types: Dict with new resource type name by old resource type name.
             - key: old resource type name.
             - value: new resource type name.
 
     Returns: List of SQL strings to update resource types.
     """
 
     def update_resource_type(old_rt_name: str, new_rt_name: str) -> str:
@@ -347,15 +348,15 @@
     return [update_resource_type(*item) for item in resource_types.items()]
 
 
 def generate_delete_resource_types_sql(resource_types: Set[str]) -> List[str]:
     """Generate SQL to delete resource types.
 
     Args:
-        - resource_types: List of resource type names.
+        resource_types: List of resource type names.
 
     Returns: List of SQL strings to delete resource types.
     """
     if not resource_types:
         return []
     return [
         sql_compile(
@@ -367,15 +368,15 @@
     ]
 
 
 def generate_create_resource_type_relations_sql(resource_types: Dict[str, Set[str]]) -> List[str]:
     """Generate SQL to create resource type relations.
 
     Args:
-        - resource_types: Dict with product blocks by resource type
+        resource_types: Dict with product blocks by resource type
             - key: Resource type name.
             - value: Set of product block names to relate with.
 
     Returns: List of SQL strings to create relation between product blocks and resource type.
     """
 
     def create_resource_type_relation(resource_type: str, block_names: Set[str]) -> str:
@@ -393,18 +394,18 @@
 
 def generate_create_resource_type_instance_values_sql(
     resource_types: Dict[str, Set[str]], inputs: Dict[str, Dict[str, str]]
 ) -> List[str]:
     """Generate SQL to create resource type instance values for existing instances.
 
     Args:
-        - resource_types: Dict with product blocks by resource type
+        resource_types: Dict with product blocks by resource type
             - key: Resource type name.
             - value: Set of product block names to relate with.
-        - inputs: Optional Dict to add default value to the resource type for existing product block instances.
+        inputs: Optional Dict to add default value to the resource type for existing product block instances.
             - key: Resource type name.
             - value: Dict with product block by default value.
                 - key: Product block name.
                 - value: Default value for the resource type.
 
     Returns: List of SQL strings to create subscription instance values for existing product block instances.
     """
@@ -437,28 +438,27 @@
                 CROSS JOIN subscription_instance_ids
                 WHERE resource_types.resource_type = '{1}'
         """
         sql_string = query.format(block_name, resource_type, value)
         logger.debug("Generated SQL", sql_string=sql_string)
         return sql_string
 
-    sql_statements = [
+    return [
         sql
         for resource_type, block_names in resource_types.items()
         for block_name in block_names
         if (sql := map_subscription_instance_relations(resource_type, block_name))
     ]
-    return sql_statements
 
 
 def generate_delete_resource_type_relations_sql(delete_resource_types: Dict[str, Set[str]]) -> List[str]:
     """Generate SQL to delete resource type relations and its instance values.
 
     Args:
-        - resource_types: Dict with product blocks by resource type
+        delete_resource_types: Dict with product blocks by resource type
             - key: Resource type name.
             - value: Set of product block names to relate with.
 
     Returns: List of SQL strings to delete relations between product blocks and resource type.
     """
 
     def delete_resource_type_relation(resource_type: str, block_names: Set[str]) -> List[str]:
@@ -487,15 +487,15 @@
     return list(flatten([delete_resource_type_relation(*item) for item in delete_resource_types.items()]))
 
 
 def generate_update_resource_type_block_relations_sql(block_rt_updates: Dict[str, Dict[str, str]]) -> List[str]:
     """Generate SQL to update resource type block relations.
 
     Args:
-        - block_rt_updates: Dict with rt updates per product block.
+        block_rt_updates: Dict with rt updates per product block.
             - key: product block name.
             - value: Dict with new resource type name by old resource type name:
                 - key: old resource type name.
                 - value: new resource type name.
 
     Returns: List of SQL strings to update resource types.
     """
@@ -520,15 +520,15 @@
     return list(flatten([update_block_resource_types(*item) for item in block_rt_updates.items()]))
 
 
 def generate_update_resource_type_instance_values_sql(block_rt_updates: Dict[str, Dict[str, str]]) -> List[str]:
     """Generate SQL to update resource type instance values.
 
     Args:
-        - block_rt_updates: Dict with rt updates per product block.
+        block_rt_updates: Dict with rt updates per product block.
             - key: product block name.
             - value: Dict with new resource type name by old resource type name:
                 - key: old resource type name.
                 - value: new resource type name.
 
     Returns: List of SQL strings to update resource types.
     """
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/cli/domain_gen_helpers/types.py` & `orchestrator_core-1.2.0/orchestrator/cli/domain_gen_helpers/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     update_block_resource_types: Dict[str, Dict[str, str]] = {}
     delete_resource_types: Set[str] = set()
     create_resource_type_relations: Dict[str, Set[str]] = {}
     create_resource_type_instance_relations: Dict[str, Set[str]] = {}
     delete_resource_type_relations: Dict[str, Set[str]] = {}
 
 
-class DuplicateException(Exception):
+class DuplicateError(Exception):
     pass
 
 
 class ModelUpdates(BaseModel):
     fixed_inputs: Dict[str, Dict[str, str]] = {}
     resource_types: Dict[str, str] = {}
     block_resource_types: Dict[str, Dict[str, str]] = {}
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/cli/generate.md` & `orchestrator_core-1.2.0/orchestrator/cli/generate.md`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/cli/generate.py` & `orchestrator_core-1.2.0/orchestrator/cli/generate.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/cli/generator/generator/fixed_input.py` & `orchestrator_core-1.2.0/orchestrator/cli/generator/generator/fixed_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,16 +31,15 @@
 def is_int_enum(fixed_input: dict) -> bool:
     return is_enum_of_type(fixed_input, "int")
 
 
 def convert_enum(fixed_input: dict) -> dict:
     if is_enum(fixed_input):
         return fixed_input | {"type": fixed_input["name"].title()}
-    else:
-        return fixed_input
+    return fixed_input
 
 
 def get_str_enum_fixed_inputs(fixed_inputs: list[dict]) -> list[dict]:
     return [convert_enum(fi) for fi in fixed_inputs if is_str_enum(fi)]
 
 
 def get_int_enum_fixed_inputs(fixed_inputs: list[dict]) -> list[dict]:
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/cli/generator/generator/helpers.py` & `orchestrator_core-1.2.0/orchestrator/cli/generator/generator/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/cli/generator/generator/migration.py` & `orchestrator_core-1.2.0/orchestrator/cli/generator/generator/migration.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/cli/generator/generator/product.py` & `orchestrator_core-1.2.0/orchestrator/cli/generator/generator/product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/cli/generator/generator/product_block.py` & `orchestrator_core-1.2.0/orchestrator/cli/generator/generator/product_block.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,18 +66,19 @@
     return name_spaced_type.split(".")[-1]
 
 
 def get_fields(product_block: dict) -> list[dict]:
     def to_type(field: dict) -> dict:
         if is_constrained_int(field):
             return field | {"type": snake_to_camel(field["name"])}
-        elif is_name_spaced_field_type(field):
+
+        if is_name_spaced_field_type(field):
             return field | {"type": name_space_get_type(field["type"])}
-        else:
-            return field
+
+        return field
 
     return [to_type(field) for field in product_block["fields"]]
 
 
 def get_lists_to_generate(fields: list[dict]) -> list[dict]:
     def should_generate(type: str, list_type: Optional[str] = None, **kwargs: Any) -> bool:
         return type == "list" and list_type not in ["str", "int", "bool", "UUID"]
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/cli/generator/generator/settings.py` & `orchestrator_core-1.2.0/orchestrator/cli/generator/generator/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/cli/generator/generator/translations.py` & `orchestrator_core-1.2.0/orchestrator/cli/generator/generator/translations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/cli/generator/generator/unittest.py` & `orchestrator_core-1.2.0/orchestrator/cli/generator/generator/unittest.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/cli/generator/generator/validations.py` & `orchestrator_core-1.2.0/orchestrator/cli/generator/generator/validations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/cli/generator/generator/workflow.py` & `orchestrator_core-1.2.0/orchestrator/cli/generator/generator/workflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,23 +40,21 @@
                 return {f"{field_name}_path": pb["name"]}
     return {}
 
 
 def add_optional_ims_config(config: dict) -> dict:
     if found := find_field_with_name(config, "ims_circuit_id"):
         return config | found
-    else:
-        return config
+    return config
 
 
 def add_optional_nso_config(config: dict) -> dict:
     if found := find_field_with_name(config, "nso_service_id"):
         return config | found
-    else:
-        return config
+    return config
 
 
 def insert_lazy_workflow_instances(environment: Environment, config: dict, writer: Callable) -> None:
     template = environment.get_template("lazy_workflow_instance.j2")
     content = template.render(product=config)
 
     path = f"{product_generator_settings.WORKFLOWS_PATH}/__init__.py"
@@ -122,14 +120,15 @@
     @wraps(f)
     def wrapper(environment: Environment, config: dict, writer: Callable) -> Any:
         def workflow_enabled() -> bool:
             return all(wf.get("enabled", True) for wf in config.get("workflows", []) if wf["name"] == workflow)
 
         if workflow_enabled():
             return f(environment, config, writer)
+        return None
 
     return wrapper
 
 
 @generate_workflow(workflow="create")
 def generate_create_workflow(environment: Environment, config: dict, writer: Callable) -> None:
     product_block = root_product_block(config)
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/cli/generator/products/workshop/circuit.yaml` & `orchestrator_core-1.2.0/orchestrator/cli/generator/products/workshop/circuit.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/cli/generator/products/workshop/node.yaml` & `orchestrator_core-1.2.0/orchestrator/cli/generator/products/workshop/node.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/cli/generator/products/workshop/user.yaml` & `orchestrator_core-1.2.0/orchestrator/cli/generator/products/workshop/user.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/cli/generator/templates/create_product.j2` & `orchestrator_core-1.2.0/orchestrator/cli/generator/templates/create_product.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/cli/generator/templates/macros.j2` & `orchestrator_core-1.2.0/orchestrator/cli/generator/templates/macros.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/cli/generator/templates/modify_product.j2` & `orchestrator_core-1.2.0/orchestrator/cli/generator/templates/modify_product.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/cli/generator/templates/new_product_migration.j2` & `orchestrator_core-1.2.0/orchestrator/cli/generator/templates/new_product_migration.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/cli/generator/templates/product.j2` & `orchestrator_core-1.2.0/orchestrator/cli/generator/templates/product.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/cli/generator/templates/product_block.j2` & `orchestrator_core-1.2.0/orchestrator/cli/generator/templates/product_block.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/cli/generator/templates/shared_forms.j2` & `orchestrator_core-1.2.0/orchestrator/cli/generator/templates/shared_forms.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/cli/generator/templates/terminate_product.j2` & `orchestrator_core-1.2.0/orchestrator/cli/generator/templates/terminate_product.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/cli/generator/templates/test_create_workflow.j2` & `orchestrator_core-1.2.0/orchestrator/cli/generator/templates/test_create_workflow.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/cli/generator/templates/test_modify_workflow.j2` & `orchestrator_core-1.2.0/orchestrator/cli/generator/templates/test_modify_workflow.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/cli/generator/templates/test_product_type.j2` & `orchestrator_core-1.2.0/orchestrator/cli/generator/templates/test_product_type.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/cli/generator/templates/test_terminate_workflow.j2` & `orchestrator_core-1.2.0/orchestrator/cli/generator/templates/test_terminate_workflow.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/cli/generator/templates/test_validate_workflow.j2` & `orchestrator_core-1.2.0/orchestrator/cli/generator/templates/test_validate_workflow.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/cli/generator/templates/validate_product.j2` & `orchestrator_core-1.2.0/orchestrator/cli/generator/templates/validate_product.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/cli/helpers/__init__.py` & `orchestrator_core-1.2.0/orchestrator/cli/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/cli/helpers/input_helpers.py` & `orchestrator_core-1.2.0/orchestrator/cli/helpers/input_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/cli/helpers/print_helpers.py` & `orchestrator_core-1.2.0/orchestrator/cli/helpers/print_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/cli/main.py` & `orchestrator_core-1.2.0/orchestrator/cli/main.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/cli/migrate_domain_models.py` & `orchestrator_core-1.2.0/orchestrator/cli/migrate_domain_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,16 @@
 def map_product_blocks_in_class(
     model_class: Union[Type[SubscriptionModel], Type[ProductBlockModel]],
     product_blocks: Dict[str, Type[ProductBlockModel]],
 ) -> Dict[str, Type[ProductBlockModel]]:
     """Create mapping of all existing product block models related to a model.
 
     Args:
-        - model_class: a product class (SubscriptionModel) or product block class (ProductBlockModel).
+        model_class: a product class (SubscriptionModel) or product block class (ProductBlockModel).
+        product_blocks: The product blocks the
 
     Returns a Dict with product block models by product block name.
     """
     product_blocks_types_in_model = get_depends_on_product_block_type_list(
         model_class._get_depends_on_product_block_types()
     )
 
@@ -100,15 +101,15 @@
     return {**product_blocks, **blocks_map}
 
 
 def map_product_blocks(product_classes: List[Type[SubscriptionModel]]) -> Dict[str, Type[ProductBlockModel]]:
     """Create mapping of all existing product block models related to products.
 
     Args:
-        - product_classes: List of product classes.
+        product_classes: List of product classes.
 
     Returns a Dict with product block models by product block name.
     """
 
     product_blocks: Dict[str, Type[ProductBlockModel]] = {}
     for product_class in product_classes:
         product_blocks = {**product_blocks, **map_product_blocks_in_class(product_class, product_blocks)}
@@ -117,16 +118,16 @@
 
 def map_differences_unique(
     registered_products: Dict[str, Type[SubscriptionModel]], existing_products: List[Tuple[str, UUID]]
 ) -> Dict[str, Dict[str, Dict[str, Set[str]]]]:
     """Create a unique map for products and product block differences from the database.
 
     Args:
-        - registered_products: Dict with product models by product name.
-        - existing_products: List with tuples of product name and its uuid that exist in the database.
+        registered_products: Dict with product models by product name.
+        existing_products: List with tuples of product name and its uuid that exist in the database.
 
     Returns a dict with product and product block differences from the database without duplicates.
     """
     model_diffs: Dict[str, Dict[str, Dict[str, Set[str]]]] = {"products": {}, "blocks": {}}
 
     for product_name, product_id in existing_products:
         if should_skip(product_name) or product_name not in registered_products:
@@ -184,22 +185,22 @@
     db_product_names: List[str],
     inputs: Dict[str, Dict[str, str]],
     updates: Optional[ModelUpdates],
 ) -> DomainModelChanges:
     """Map changes that need to be made to fix differences between models and database.
 
     Args:
-        - model_diffs: Dict with product and product block differences.
-            - products: Dict with product differences.
-            - blocks: Dict with product block differences.
-        - products: Dict with product model by product name.
-        - product_blocks: Dict with product block model by product name.
-        - db_product_names: Product names out of the database.
-        - inputs: Optional Dict with prefilled values.
-        - updates: Optional Dict.
+        model_diffs: Dict with product and product block differences.
+        products: Dict with product differences.
+        blocks: Dict with product block differences.
+        products: Dict with product model by product name.
+        product_blocks: Dict with product block model by product name.
+        db_product_names: Product names out of the database.
+        inputs: Optional Dict with prefilled values.
+        updates: Optional Dict.
 
     Returns: Mapped changes.
     """
     create_products = {name: model for name, model in products.items() if name not in db_product_names}
     delete_products = {name for name in db_product_names if name not in SUBSCRIPTION_MODEL_REGISTRY}
 
     # updates need to go before create or deletes.
@@ -250,16 +251,16 @@
     return changes
 
 
 def generate_upgrade_sql(changes: DomainModelChanges, inputs: Dict[str, Dict[str, str]]) -> List[str]:
     """Generate upgrade SQL with mapped changes.
 
     Args:
-        - changes: Mapping of model changes.
-        - inputs: Optional Dict with prefilled values.
+        changes: Mapping of model changes.
+        inputs: Optional Dict with prefilled values.
 
     Returns: List of SQL strings to upgrade the database.
     """
     return (
         generate_update_fixed_inputs_sql(changes.update_product_fixed_inputs)
         + generate_rename_resource_types_sql(changes.rename_resource_types)
         + generate_delete_resource_type_relations_sql(changes.delete_resource_type_relations)
@@ -286,15 +287,16 @@
 
 def generate_downgrade_sql(changes: DomainModelChanges) -> List[str]:
     """Generate downgrade SQL with mapped changes.
 
     Does not revert deleted subscription instances and subscription instance values!
 
     Args:
-        - changes: Mapping of model changes.
+        changes: Mapping of model changes.
+
 
     Returns: List of SQL strings to downgrade the database back before upgrade SQL.
     """
     sql_revert_create_fixed_inputs = generate_delete_fixed_inputs_sql(changes.create_product_fixed_inputs)
 
     update_revert_map = {
         name: {new: old for old, new in updates.items()}
@@ -355,19 +357,21 @@
     is_test: bool = False,
 ) -> Tuple[List[str], List[str]]:
     """Create tuple with list for upgrade and downgrade SQL statements based on SubscriptionModel.diff_product_in_database.
 
     You will be prompted with inputs for new models and resource type updates.
 
     Args:
-        - inputs: dict with pre-defined input values
+        inputs: dict with pre-defined input values
+        updates: The model
+        is_test: the bool for if it is test
 
     Returns tuple:
-        - list of upgrade SQL statements in string format.
-        - list of downgrade SQL statements in string format.
+        list of upgrade SQL statements in string format.
+        list of downgrade SQL statements in string format.
     """
     existing_products: List[Tuple[str, UUID]] = list(
         ProductTable.query.with_entities(ProductTable.name, ProductTable.product_id)
     )
     db_product_names: List[str] = [product_name for product_name, _ in existing_products]
 
     products = SUBSCRIPTION_MODEL_REGISTRY
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/cli/migrate_workflows.py` & `orchestrator_core-1.2.0/orchestrator/cli/migrate_workflows.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,16 +110,15 @@
     wf_num = get_user_input("Which workflow do you want to delete? (q to cancel) ", "q")
     if not wf_num.isdigit():
         return state
     wf_index = int(wf_num) - 1
     if 0 <= wf_index < len(items):
         item = dict(zip(keys[1:], items[wf_index]))
         return {**state, "workflows_to_delete": [*state["workflows_to_delete"], item]}
-    else:
-        return state
+    return state
 
 
 def _show_state(state: dict) -> dict:
     print_fmt("\nWorkflows to add:", flags=[COLOR.GREEN])
     print_fmt(
         tabulate(
             state["workflows_to_add"],
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/cli/migration_helpers.py` & `orchestrator_core-1.2.0/orchestrator/cli/migration_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
     with open(migration.path, "w") as f:
         f.write(text)
 
 
 def _insert_preamble(text: str, s: str) -> str:
     lines = text.splitlines(keepends=True)
-    line_num = next((i for i, l in enumerate(lines) if "def upgrade()" in l), None)
+    line_num = next((i for i, line in enumerate(lines) if "def upgrade()" in line), None)
     return "".join(lines[:line_num]) + f"{s}\n\n" + "".join(lines[line_num:]) if line_num else text
 
 
 def create_migration_file(
     alembic_config: Config, sql_upgrade_str: str, sql_downgrade_str: str, message: str, preamble: str = ""
 ) -> None:
     if not (sql_upgrade_str or sql_downgrade_str):
@@ -90,16 +90,15 @@
             "The script directory has multiple heads" in error_str
         ):
             try:
                 migration = command.revision(alembic_config, message, head="data@head")
             except CommandError:
                 if "Branch name 'data'" in error_str and "already used by revision" in error_str:
                     raise CommandError("Database not up to date with latest revision")
-                else:
-                    raise CommandError("Database head 'data' already exists but no revision/migration file found")
+                raise CommandError("Database head 'data' already exists but no revision/migration file found")
         else:
             raise err
 
     with open(migration.path) as f:
         file_data = f.read()
 
     if preamble:
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/cli/scheduler.py` & `orchestrator_core-1.2.0/orchestrator/cli/scheduler.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/config/__init__.py` & `orchestrator_core-1.2.0/orchestrator/config/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/config/assignee.py` & `orchestrator_core-1.2.0/orchestrator/config/assignee.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/db/__init__.py` & `orchestrator_core-1.2.0/orchestrator/db/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     SubscriptionCustomerDescriptionTable,
     SubscriptionInstanceRelationTable,
     SubscriptionInstanceTable,
     SubscriptionInstanceValueTable,
     SubscriptionMetadataTable,
     SubscriptionTable,
     UtcTimestamp,
-    UtcTimestampException,
+    UtcTimestampError,
     WorkflowTable,
 )
 from orchestrator.settings import AppSettings
 
 logger = get_logger(__name__)
 
 
@@ -47,15 +47,15 @@
         self.wrapped_database = wrappee
         logger.warning("Database object configured, all methods referencing `db` should work.")
 
     def __getattr__(self, attr: str) -> Any:
         if not isinstance(self.wrapped_database, Database):
             if "_" in attr:
                 logger.warning("No database configured, but attempting to access class methods")
-                return
+                return None
             raise RuntimeWarning(
                 "No database configured at this time. Please pass database configuration to OrchestratorCore base_settings"
             )
 
         return getattr(self.wrapped_database, attr)
 
 
@@ -84,11 +84,11 @@
     "SubscriptionMetadataTable",
     "ResourceTypeTable",
     "FixedInputTable",
     "EngineSettingsTable",
     "WorkflowTable",
     "SubscriptionCustomerDescriptionTable",
     "UtcTimestamp",
-    "UtcTimestampException",
+    "UtcTimestampError",
     "db",
     "init_database",
 ]
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/db/database.py` & `orchestrator_core-1.2.0/orchestrator/db/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,16 +50,15 @@
     def set_query(self, query: SearchQuery) -> None:
         self._query = query
 
     @property
     def query(self) -> SearchQuery:
         if self._query is not None:
             return self._query
-        else:
-            raise NoSessionError("Cant get session. Please, call BaseModel.set_query() first")
+        raise NoSessionError("Cant get session. Please, call BaseModel.set_query() first")
 
 
 @as_declarative(metaclass=BaseModelMeta)
 class _Base:
     """SQLAlchemy base class."""
 
     __abstract__ = True
@@ -124,16 +123,15 @@
         # sensitive data from JSON representation.
         keys -= exclude
 
         return {key: getattr(self, key) for key in keys}
 
 
 class BaseModel(_Base):
-    """
-    Separate BaseModel class to be able to include mixins and to Fix typing.
+    """Separate BaseModel class to be able to include mixins and to Fix typing.
 
     This should be used instead of Base.
     """
 
     metadata: ClassVar[MetaData]
     query: ClassVar[SearchQuery]
     set_query: ClassVar[Callable[[SearchQuery], None]]
@@ -191,30 +189,29 @@
         self.engine = create_engine(db_url, **ENGINE_ARGUMENTS)
         self.session_factory = sessionmaker(bind=self.engine, **SESSION_ARGUMENTS)
 
         self.scoped_session = scoped_session(self.session_factory, self._scopefunc)
         BaseModel.set_query(cast(SearchQuery, self.scoped_session.query_property()))
 
     def _scopefunc(self) -> Optional[str]:
-        scope_str = self.request_context.get()
-        return scope_str
+        return self.request_context.get()
 
     @property
     def session(self) -> WrappedSession:
         return self.scoped_session()
 
     @contextmanager
     def database_scope(self, **kwargs: Any) -> Generator["Database", None, None]:
         """Create a new database session (scope).
 
         This creates a new database session to handle all the database connection from a single scope (request or workflow).
         This method should typically only been called in request middleware or at the start of workflows.
 
         Args:
-            ``**kwargs``: Optional session kw args for this session
+            kwargs: Optional session kw args for this session
         """
         token = self.request_context.set(str(uuid4()))
         self.scoped_session(**kwargs)
         yield self
         self.scoped_session.remove()
         self.request_context.reset(token)
 
@@ -223,16 +220,15 @@
     def __init__(self, app: ASGIApp, database: Database, commit_on_exit: bool = False):
         super().__init__(app)
         self.commit_on_exit = commit_on_exit
         self.database = database
 
     async def dispatch(self, request: Request, call_next: RequestResponseEndpoint) -> Response:
         with self.database.database_scope():
-            response = await call_next(request)
-        return response
+            return await call_next(request)
 
 
 @contextmanager
 def disable_commit(db: Database, log: BoundLogger) -> Iterator:
     restore = True
     # If `db.session` already has its `commit` method disabled we won't try disabling *and* restoring it again.
     if db.session.info.get("disabled", False):
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/db/filters/filters.py` & `orchestrator_core-1.2.0/orchestrator/db/filters/filters.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/db/filters/generic_filters/__init__.py` & `orchestrator_core-1.2.0/orchestrator/db/filters/generic_filters/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/db/filters/generic_filters/bool_filter.py` & `orchestrator_core-1.2.0/orchestrator/db/filters/generic_filters/bool_filter.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/db/filters/generic_filters/is_like_filter.py` & `orchestrator_core-1.2.0/orchestrator/db/filters/generic_filters/is_like_filter.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/db/filters/generic_filters/range_filter.py` & `orchestrator_core-1.2.0/orchestrator/db/filters/generic_filters/range_filter.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/db/filters/generic_filters/values_in_column_filter.py` & `orchestrator_core-1.2.0/orchestrator/db/filters/generic_filters/values_in_column_filter.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/db/filters/process.py` & `orchestrator_core-1.2.0/orchestrator/db/filters/process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/db/filters/product.py` & `orchestrator_core-1.2.0/orchestrator/db/filters/product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/db/filters/subscription.py` & `orchestrator_core-1.2.0/orchestrator/db/filters/subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/db/models.py` & `orchestrator_core-1.2.0/orchestrator/db/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
 logger = structlog.get_logger(__name__)
 
 TAG_LENGTH = 20
 STATUS_LENGTH = 255
 
 
-class UtcTimestampException(Exception, DontWrapMixin):
+class UtcTimestampError(Exception, DontWrapMixin):
     pass
 
 
 class UtcTimestamp(TypeDecorator):
     """Timestamps in UTC.
 
     This column type always returns timestamps with the UTC timezone, regardless of the database/connection time zone
@@ -69,15 +69,15 @@
     impl = sqlalchemy.types.TIMESTAMP(timezone=True)
     cache_ok = False
     python_type = datetime
 
     def process_bind_param(self, value: Optional[datetime], dialect: Dialect) -> Optional[datetime]:
         if value is not None:
             if value.tzinfo is None:
-                raise UtcTimestampException(f"Expected timestamp with tzinfo. Got naive timestamp {value!r} instead")
+                raise UtcTimestampError(f"Expected timestamp with tzinfo. Got naive timestamp {value!r} instead")
         return value
 
     def process_result_value(self, value: Optional[datetime], dialect: Dialect) -> Optional[datetime]:
         if value is not None:
             return value.astimezone(timezone.utc)
         return value
 
@@ -224,16 +224,15 @@
         return self._subscription_workflow_key(Target.TERMINATE)
 
     def modify_subscription_workflow_key(self, name: str) -> Optional[str]:
         wfs = list(filter(lambda w: w.target == Target.MODIFY and w.name == name, self.workflows))
         return wfs[0].name if len(wfs) > 0 else None
 
     def workflow_by_key(self, name: str) -> Optional[WorkflowTable]:
-        workflow = first_true(self.workflows, None, lambda wf: wf.name == name)
-        return workflow
+        return first_true(self.workflows, None, lambda wf: wf.name == name)  # type: ignore
 
 
 class FixedInputTable(BaseModel):
     __tablename__ = "fixed_inputs"
 
     fixed_input_id = Column(UUIDType, server_default=text("uuid_generate_v4()"), primary_key=True)
     name = Column(String(), nullable=False, unique=UniqueConstraint("name", "product_id"))
@@ -446,16 +445,15 @@
     depends_on: list[SubscriptionInstanceTable] = association_proxy(
         "depends_on_block_relations",
         "depends_on",
         creator=lambda depends_on: SubscriptionInstanceRelationTable(depends_on=depends_on),
     )
 
     def value_for_resource_type(self, name: Optional[str]) -> Optional[SubscriptionInstanceValueTable]:
-        value = first_true(self.values, None, lambda x: x.resource_type.resource_type == name)
-        return value
+        return first_true(self.values, None, lambda x: x.resource_type.resource_type == name)  # type: ignore
 
 
 SubscriptionInstanceTable.parent_relations = SubscriptionInstanceTable.in_use_by_block_relations
 SubscriptionInstanceTable.children_relations = SubscriptionInstanceTable.depends_on_block_relations
 
 subscription_instance_s_pb_ix = Index(
     "subscription_instance_s_pb_ix",
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/db/range/range.py` & `orchestrator_core-1.2.0/orchestrator/db/range/range.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 logger = structlog.get_logger(__name__)
 
 
 def apply_range_to_query(query: SearchQuery, offset: int, limit: int) -> SearchQuery:
     """Apply range to the SearchQuery.
 
     Args:
-        - query: The sql query to add offset and limit to.
-        - offset: the limit item in the list to get.
-        - limit: the amount of items to get with offset as start point.
+        query: The sql query to add offset and limit to.
+        offset: the limit item in the list to get.
+        limit: the amount of items to get with offset as start point.
 
     returns the query with offset and limit applied.
     """
 
     if offset is not None and limit:
         if offset >= offset + limit:
             msg = "range start must be lower than end"
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/db/sorting/process.py` & `orchestrator_core-1.2.0/orchestrator/db/sorting/process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/db/sorting/sorting.py` & `orchestrator_core-1.2.0/orchestrator/db/sorting/sorting.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,17 +43,15 @@
 
 def generic_sorts_validate(
     valid_sort_functions_by_column: ValidSortFunctionsByColumnType,
 ) -> Callable[[list[Sort]], tuple[Iterator[Sort], Iterator[Sort]]]:
     """Create generic validate sort factory that creates a validate function based on the valid sort dict.
 
     Args:
-        - valid_sort_dict: dict of column names by valid sort keys
-            - key: sort key.
-            - value: column name.
+        valid_sort_functions_by_column: The sort functions per column
 
     Returns function that takes sort parameters and returns a list of invalid and valid Sort items.
     """
 
     def validate_sort_items(sort_by: list[Sort]) -> tuple[Iterator[Sort], Iterator[Sort]]:
         def _is_valid_sort(item: Sort) -> bool:
             return item.field in valid_sort_functions_by_column
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/db/sorting/subscription.py` & `orchestrator_core-1.2.0/orchestrator/db/sorting/subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/devtools/populator.py` & `orchestrator_core-1.2.0/orchestrator/devtools/populator.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 from typing import Any, TypedDict, Union
 from uuid import UUID
 
 import jsonref
 import requests
 import structlog
 from more_itertools import first_true
-from nwastdlib.url import URL
 
+from nwastdlib.url import URL
 from orchestrator.types import InputForm as LegacyInputForm
 from orchestrator.types import State
 
 
 class JSONSubSchema(TypedDict, total=False):
     title: str
     type: str
@@ -142,32 +142,30 @@
         """Add extra default value from classes that inherit me.
 
         This method can be overridden to add custom default
         values. Please ensure that you call super().add_default_values() in that case.
         """
 
     def _get_product_by_name(self, product_name: str) -> dict:
-        """
-        Fetch all active products.
+        """Fetch all active products.
 
         Returns: product dict
 
         """
         response = self.session.get(BASE_API_URL / "products/")
         if response.status_code == HTTPStatus.OK:
             for product in response.json():
                 if product["name"] == product_name:
                     self.log.info("Resolved product.", product_id=product["product_id"])
                     return product
         self.log.error("Error product not found.", product=product_name, status_code=response.status_code)
         return {}
 
-    def get_form_data(self, form: JSONSchema) -> dict:
-        """
-        Compiles a dict that can be used as the payload in api request that need human input.
+    def get_form_data(self, form: JSONSchema) -> dict:  # noqa: C901
+        """Compiles a dict that can be used as the payload in api request that need human input.
 
         Note: if you want to populate a boolean field: you have to provide 'False' instead of 'None', as the
         latter is used to determine if one of the ways to populate the input_filed value was already successful.
 
         Args:
             form: a json schema form definition.
 
@@ -263,19 +261,19 @@
                 value = ""
 
             log.debug("Resolved input_field.", value=value)
             data[field_name] = value
         return data
 
     def _start_workflow(self, workflow_name: str, **kwargs: Any) -> UUIDstr:
-        """
-        Start a workflow.
+        """Start a workflow.
 
         Args:
             workflow_name: workflow name
+            kwargs: The kwargs
 
         Returns: the pid of the workflow process
 
         """
         self.log = self.log.bind(pid=None, workflow=workflow_name)
         self.log.info("Starting workflow")
 
@@ -289,16 +287,15 @@
 
         self.pid = pid = response_json["id"]
         self.log = self.log.bind(pid=self.pid)
         self.started = True
         return pid
 
     def start_create_workflow(self, **kwargs: Any) -> UUIDstr:
-        """
-        Start a create workflow.
+        """Start a create workflow.
 
         Args:
             kwargs: values to be used as form input
 
         Returns: the pid of the workflow process
 
         """
@@ -306,16 +303,15 @@
         self.log.info("Started create workflow")
         product_id = self._product.get("product_id")
         return self._start_workflow(self.create_workflow, product=product_id, **kwargs)
 
     def start_modify_workflow(
         self, workflow_name: str, subscription_id: Union[UUIDstr, UUID], **kwargs: Any
     ) -> UUIDstr:
-        """
-        Start a modify workflow for the provided name and subscription_id.
+        """Start a modify workflow for the provided name and subscription_id.
 
         Args:
             workflow_name: workflow name
             subscription_id: uuid of the subscription you want to modify
             kwargs: values to be used as form input
 
         Returns: the pid of the workflow process
@@ -329,32 +325,30 @@
     def start_verify_workflow(self, workflow_name: str, subscription_id: Union[UUIDstr, UUID]) -> UUIDstr:
         subscription_id = str(subscription_id)
         self.log = self.log.bind(subscription_id=subscription_id)
         self.log.info("Started verify workflow")
         return self._start_workflow(workflow_name, subscription_id=subscription_id)
 
     def start_terminate_workflow(self, subscription_id: Union[UUIDstr, UUID], **kwargs: Any) -> UUIDstr:
-        """
-        Start a terminate workflow for the provided subscription_id.
+        """Start a terminate workflow for the provided subscription_id.
 
         Args:
             subscription_id: uuid of the subscription you want to terminate
             kwargs: values to be used as form input
 
         Returns: the pid of the workflow process
 
         """
         subscription_id = str(subscription_id)
         self.log = self.log.bind(pid=None, subscription_id=subscription_id)
         self.log.info("Starting terminate workflow")
         return self._start_workflow(self.terminate_workflow, subscription_id=subscription_id, **kwargs)
 
     def human_input_needed(self) -> bool:
-        """
-        Check whether the workflow process needs human input.
+        """Check whether the workflow process needs human input.
 
         Returns: True or False
 
         """
         response = self.session.get(BASE_API_URL / "processes" / self.pid)
         if response.status_code == HTTPStatus.OK:
             self.last_state = response.json()
@@ -362,28 +356,30 @@
             self.log.error("Cowardly quitting due to response code.", status_code=response.status_code)
             raise Exception("Request failed")
         status = self.last_state["status"] if "status" in self.last_state else self.last_state["last_status"]
         if status == "completed":
             self.log.info("Process is complete.")
             self.done = True
             return False
-        elif status == "suspended":
+
+        if status == "suspended":
             return True
-        elif status in ("created", "running", "resumed"):
+
+        if status in ("created", "running", "resumed"):
             return False
-        elif status in ("failed", "waiting"):
+
+        if status in ("failed", "waiting"):
             if self.retries < 1:
                 self.retries += 1
                 return True
 
             self.log.error("Cowardly quitting due to failed step.", reason=self.last_state["failed_reason"])
             raise Exception(f"Step failed: {self.last_state['failed_reason']}")
-        else:
-            self.log.error("Cowardly quitting due to unknown status", status=self.last_state["status"])
-            raise Exception(f"Unknown status: {status}")
+        self.log.error("Cowardly quitting due to unknown status", status=self.last_state["status"])
+        raise Exception(f"Unknown status: {status}")
 
     def get_current_form(self) -> Union[JSONSchema, None]:
         self.log.info("Current form.", form=self.last_state.get("form"))
         return copy.deepcopy(self.last_state.get("form"))
 
     def provide_user_input(self, method: str, url: URL, form: Union[JSONSchema, None] = None) -> requests.Response:
         """Provide input for steps that normally require a user."""
@@ -407,16 +403,15 @@
         self.last_state = {}
         self.pid = None
 
         # ensure dynamic stuff is also reset
         self.add_default_values()
 
     def run(self, **kwargs: Any) -> UUIDstr:
-        """
-        Responsible for auto-completing the workflow after the process has been started.
+        """Responsible for auto-completing the workflow after the process has been started.
 
         Returns: subscription_id of the created subscription
 
         """
         self.custom_input_values.update(kwargs)
         self.retries = 0
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/distlock/__init__.py` & `orchestrator_core-1.2.0/orchestrator/distlock/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         self.wrapped_distlock_manager = wrappee
         logger.warning("DistLockManager object configured, all methods referencing `distlock_manager` should work.")
 
     def __getattr__(self, attr: str) -> Any:
         if not isinstance(self.wrapped_distlock_manager, DistLockManager):
             if "_" in attr:
                 logger.warning("No DistLockManager configured, but attempting to access class methods")
-                return
+                return None
             raise RuntimeWarning(
                 "No DistLockManager configured at this time. Please set ENABLE_DISTLOCK_MANAGER "
                 "and DISTLOCK_BACKEND in OrchestratorCore base_settings"
             )
         if attr != "enabled" and not self.wrapped_distlock_manager.enabled:
             logger.warning("Distributed Locking is disabled, unable to access class methods")
             return empty_fn
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/distlock/distlock_manager.py` & `orchestrator_core-1.2.0/orchestrator/distlock/distlock_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/distlock/managers/__init__.py` & `orchestrator_core-1.2.0/orchestrator/distlock/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/distlock/managers/memory_distlock_manager.py` & `orchestrator_core-1.2.0/orchestrator/distlock/managers/memory_distlock_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/distlock/managers/redis_distlock_manager.py` & `orchestrator_core-1.2.0/orchestrator/distlock/managers/redis_distlock_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,25 +55,24 @@
                 name=key,
                 timeout=float(expiration_seconds),
                 blocking=False,
                 thread_local=False,
             )
             if await lock.acquire():
                 return lock
-            else:
-                # normal behavior (lock acquired by something else)
-                return None
+            # normal behavior (lock acquired by something else)
+            return None
         except LockError:
             # Unexpected behavior, possibly a problem with Redis
             logger.Exception("Could not acquire lock for resource", resource=key)
             return None
 
     async def release_lock(self, lock: Lock) -> None:
         if not self.redis_conn:
-            return None
+            return
 
         try:
             await lock.release()
         except LockError:
             logger.Exception("Could not release lock for resource", resource=lock.name)
 
     # https://github.com/aio-libs/aioredis-py/issues/1273
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/domain/__init__.py` & `orchestrator_core-1.2.0/orchestrator/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/domain/base.py` & `orchestrator_core-1.2.0/orchestrator/domain/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 )
 from orchestrator.utils.datetime import nowtz
 from orchestrator.utils.docs import make_product_block_docstring, make_subscription_model_docstring
 
 logger = structlog.get_logger(__name__)
 
 
-class ProductNotInRegistryException(Exception):
+class ProductNotInRegistryError(Exception):
     pass
 
 
 class serializable_property(property):
     """Inherit from property class to mark a field in a product block as serializable."""
 
     pass
@@ -99,16 +99,15 @@
     # subclass on typing.List throws exception and there is no good way to test for this
     try:
         is_constrained_list = issubclass(type, ConstrainedList)
     except Exception:
         # Strip generic arguments, it still might be a subclass
         if get_origin(type):
             return _is_constrained_list_type(get_origin(type))  # type: ignore
-        else:
-            return False
+        return False
 
     return is_constrained_list
 
 
 T = TypeVar("T")  # pragma: no mutate
 S = TypeVar("S", bound="SubscriptionModel")  # pragma: no mutate
 B = TypeVar("B", bound="ProductBlockModel")  # pragma: no mutate
@@ -230,23 +229,24 @@
             # We only want fields that are on this class and not on the related product blocks
             if is_product_block_field:
                 cls._product_block_fields_[field_name] = field_type
             else:
                 cls._non_product_block_fields_[field_name] = field_type
 
     @classmethod
-    def _init_instances(
+    def _init_instances(  # noqa: C901
         cls, subscription_id: UUID, skip_keys: Optional[List[str]] = None
     ) -> Dict[str, Union[List["ProductBlockModel"], "ProductBlockModel"]]:
         """Initialize default subscription instances.
 
         When a new domain model is created that is not loaded from an existing subscription.
         We also create all subscription instances for it. This function does that.
 
         Args:
+            subscription_id: The UUID of the subscription
             skip_keys: list of fields on the class to skip when creating dummy instances.
 
         Returns:
             A dict with instances to pass to the new model
 
         """
         if skip_keys is None:
@@ -281,15 +281,15 @@
                 product_block_model = product_block_field_type
                 # Scalar field of a ProductBlockModel expects 1 instance
                 default_value = product_block_model.new(subscription_id=subscription_id)
             instances[product_block_field_name] = default_value
         return instances
 
     @classmethod
-    def _load_instances(
+    def _load_instances(  # noqa: C901
         cls,
         db_instances: List[SubscriptionInstanceTable],
         status: SubscriptionLifecycle,
         match_domain_attr: bool = True,
     ) -> Dict[str, Union[Optional["ProductBlockModel"], List["ProductBlockModel"]]]:
         """Load subscription instances for this domain model.
 
@@ -312,16 +312,15 @@
             return i.product_block.name
 
         sorted_instances = sorted(db_instances, key=keyfunc)
         grouped_instances = {k: list(g) for k, g in groupby(sorted_instances, keyfunc)}
 
         def match_domain_model_attr_if_possible(field_name: str) -> Callable:
             def domain_filter(instance: SubscriptionInstanceTable) -> bool:
-                """
-                Match domain model attributes.
+                """Match domain model attributes.
 
                 This helper is necessary to filter through all relations in a subscription. Not all subscriptions have a
                 domain model attribute that is set as it is not always necessary. However when it is set, it is necessary
                 to filter through instances depending on that attribute.
 
                 Args:
                     instance: depends on subscription instance
@@ -371,15 +370,16 @@
                 )
 
                 instances[product_block_field_name] = product_block_model_list
             else:
                 instance = only(instance_list)
                 if not is_optional_type(product_block_field_type) and instance is None:
                     raise ValueError("Required subscription instance is missing in database")
-                elif is_optional_type(product_block_field_type) and instance is None:
+
+                if is_optional_type(product_block_field_type) and instance is None:
                     instances[product_block_field_name] = None
                 elif instance:
                     assert (  # noqa: S101
                         len(possible_product_block_types) is not None
                     ), "Product block model has not been resolved. Unable to continue"
                     instances[product_block_field_name] = possible_product_block_types[
                         instance.product_block.name
@@ -870,21 +870,21 @@
         return subscription_instance_values
 
     def _set_instance_domain_model_attrs(
         self,
         subscription_instance: SubscriptionInstanceTable,
         subscription_instance_mapping: Dict[str, List[SubscriptionInstanceTable]],
     ) -> None:
-        """
-        Save the domain model attribute to the database.
+        """Save the domain model attribute to the database.
 
         This function iterates through the subscription instances and stores the domain model attribute in the
         hierarchy relationship.
 
         Args:
+            subscription_instance: The subscription instance object.
             subscription_instance_mapping: a mapping of the domain model attribute a underlying instances
 
         Returns:
             None
 
         """
         depends_on_block_relations = []
@@ -1298,15 +1298,15 @@
         if not cls.__base_type__:
             # Import here to prevent cyclic imports
             from orchestrator.domain import SUBSCRIPTION_MODEL_REGISTRY
 
             try:
                 cls = SUBSCRIPTION_MODEL_REGISTRY[subscription.product.name]  # type:ignore
             except KeyError:
-                raise ProductNotInRegistryException(
+                raise ProductNotInRegistryError(
                     f"'{subscription.product.name}' is not found within the SUBSCRIPTION_MODEL_REGISTRY"
                 )
             cls = lookup_specialized_type(cls, status)
         elif not issubclass(cls, lookup_specialized_type(cls, status)):
             raise ValueError(f"{cls} is not valid for lifecycle {status}")
 
         fixed_inputs = {fi.name: fi.value for fi in subscription.product.fixed_inputs}
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/domain/lifecycle.py` & `orchestrator_core-1.2.0/orchestrator/domain/lifecycle.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/exception_handlers.py` & `orchestrator_core-1.2.0/orchestrator/exception_handlers.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from http import HTTPStatus
 
-from nwastdlib.ex import show_ex
 from starlette.requests import Request
 from starlette.responses import JSONResponse
 
+from nwastdlib.ex import show_ex
 from orchestrator.api.error_handling import ProblemDetailException
-from orchestrator.forms import FormException, FormNotCompleteError, FormValidationError
+from orchestrator.forms import FormError, FormNotCompleteError, FormValidationError
 from orchestrator.utils.json import json_dumps, json_loads
 
 PROBLEM_DETAIL_FIELDS = ("title", "type")
 
 
 async def problem_detail_handler(request: Request, exc: ProblemDetailException) -> JSONResponse:
     headers = getattr(exc, "headers", None)
@@ -32,48 +32,47 @@
     for field in PROBLEM_DETAIL_FIELDS:
         value = getattr(exc, field, None)
         if value:
             body[field] = value
 
     if headers:
         return JSONResponse(body, status_code=exc.status_code, headers=headers)
-    else:
-        return JSONResponse(body, status_code=exc.status_code)
+    return JSONResponse(body, status_code=exc.status_code)
 
 
-async def form_error_handler(request: Request, exc: FormException) -> JSONResponse:
+async def form_error_handler(request: Request, exc: FormError) -> JSONResponse:
     if isinstance(exc, FormValidationError):
         return JSONResponse(
             {
                 "type": type(exc).__name__,
                 "detail": str(exc),
                 "traceback": show_ex(exc),
                 "title": "Form not valid",
                 # We need to make sure the is nothing the default json.dumps cannot handle
                 "validation_errors": json_loads(json_dumps(exc.errors)),
                 "status": HTTPStatus.BAD_REQUEST,
             },
             status_code=HTTPStatus.BAD_REQUEST,
         )
-    elif isinstance(exc, FormNotCompleteError):
+
+    if isinstance(exc, FormNotCompleteError):
         return JSONResponse(
             {
                 "type": type(exc).__name__,
                 "detail": str(exc),
                 "traceback": show_ex(exc),
                 # We need to make sure the is nothing the default json.dumps cannot handle
                 "form": json_loads(json_dumps(exc.form)),
                 "title": "Form not complete",
                 "status": HTTPStatus.NOT_EXTENDED,
             },
             status_code=HTTPStatus.NOT_EXTENDED,
         )
-    else:
-        return JSONResponse(
-            {
-                "detail": str(exc),
-                "title": "Internal Server Error",
-                "status": HTTPStatus.INTERNAL_SERVER_ERROR,
-                "type": type(exc).__name__,
-            },
-            status_code=HTTPStatus.INTERNAL_SERVER_ERROR,
-        )
+    return JSONResponse(
+        {
+            "detail": str(exc),
+            "title": "Internal Server Error",
+            "status": HTTPStatus.INTERNAL_SERVER_ERROR,
+            "type": type(exc).__name__,
+        },
+        status_code=HTTPStatus.INTERNAL_SERVER_ERROR,
+    )
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/forms/__init__.py` & `orchestrator_core-1.2.0/orchestrator/forms/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,37 +22,37 @@
 
 from orchestrator.types import JSON, InputForm, State, StateInputFormGenerator
 from orchestrator.utils.json import json_dumps, json_loads
 
 logger = structlog.get_logger(__name__)
 
 
-__all__ = ("generate_form", "post_process", "FormNotCompleteError", "FormValidationError", "FormException")
+__all__ = ("generate_form", "post_process", "FormNotCompleteError", "FormValidationError", "FormError")
 
 
-class FormException(Exception):
+class FormError(Exception):
     pass
 
 
-class FormNotCompleteError(FormException):
+class FormNotCompleteError(FormError):
     form: InputForm
 
     def __init__(self, form: JSON):
         super().__init__(form)
         self.form = form
 
 
 class PydanticErrorDict(TypedDict):
     loc: List[Union[str, int]]
     type: str
     msg: str
     ctx: Dict[str, Any]
 
 
-class FormValidationError(FormException):
+class FormValidationError(FormError):
     validator_name: str
     errors: List[PydanticErrorDict]
 
     def __init__(self, validator_name: str, errors: List[Dict[str, Any]]):
         super().__init__(validator_name, errors)
         self.validator_name = validator_name
         self.errors = cast(List[PydanticErrorDict], errors)
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/forms/network_type_validators.py` & `orchestrator_core-1.2.0/orchestrator/forms/network_type_validators.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/forms/validators.py` & `orchestrator_core-1.2.0/orchestrator/forms/validators.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/graphql/__init__.py` & `orchestrator_core-1.2.0/orchestrator/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/graphql/extensions/deprecation_checker_extension.py` & `orchestrator_core-1.2.0/orchestrator/graphql/extensions/deprecation_checker_extension.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,15 @@
 
 DeprecatedPaths = dict[str, str]
 
 
 def get_path_as_string(path: Path) -> str:
     if path.prev:
         return f"{get_path_as_string(path.prev)}/{path.key}"
-    else:
-        return f"{path.key}"
+    return f"{path.key}"
 
 
 def get_root_path(path: Path) -> Path:
     while path.prev:
         path = path.prev
     return path
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/graphql/extensions/error_collector_extension.py` & `orchestrator_core-1.2.0/orchestrator/graphql/extensions/error_collector_extension.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/graphql/pagination.py` & `orchestrator_core-1.2.0/orchestrator/graphql/pagination.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/graphql/resolvers/process.py` & `orchestrator_core-1.2.0/orchestrator/graphql/resolvers/process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/graphql/resolvers/product.py` & `orchestrator_core-1.2.0/orchestrator/graphql/resolvers/product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/graphql/resolvers/settings.py` & `orchestrator_core-1.2.0/orchestrator/graphql/resolvers/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/graphql/resolvers/subscription.py` & `orchestrator_core-1.2.0/orchestrator/graphql/resolvers/subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/graphql/schemas/fixed_input.py` & `orchestrator_core-1.2.0/orchestrator/graphql/schemas/fixed_input.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/graphql/schemas/process.py` & `orchestrator_core-1.2.0/orchestrator/graphql/schemas/process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/graphql/schemas/product.py` & `orchestrator_core-1.2.0/orchestrator/graphql/schemas/product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/graphql/schemas/product_block.py` & `orchestrator_core-1.2.0/orchestrator/graphql/schemas/product_block.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/graphql/schemas/settings.py` & `orchestrator_core-1.2.0/orchestrator/graphql/schemas/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/graphql/schemas/subscription.py` & `orchestrator_core-1.2.0/orchestrator/graphql/schemas/subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/graphql/types.py` & `orchestrator_core-1.2.0/orchestrator/graphql/types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/graphql/utils/create_resolver_error_handler.py` & `orchestrator_core-1.2.0/orchestrator/graphql/utils/create_resolver_error_handler.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/graphql/utils/get_selected_fields.py` & `orchestrator_core-1.2.0/orchestrator/graphql/utils/get_selected_fields.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 def get_selected_fields(info: CustomInfo) -> list[str]:
     """Get SelectedField names from the requested query (info).
 
     Can be used to get the selected fields of the schema, to only fetch those from the database.
 
     Args:
-        - info: The info class with request information.
+        info: The info class with request information.
 
     returns the names of SelectedFields as a list of strings.
     """
     root_selected = info.selected_fields[0]
 
     def has_field_name(selection: Selection, field_name: str) -> bool:
         return isinstance(selection, SelectedField) and selection.name == field_name
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/migrations/alembic.ini` & `orchestrator_core-1.2.0/orchestrator/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/migrations/env.py` & `orchestrator_core-1.2.0/orchestrator/migrations/env.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/migrations/helpers.py` & `orchestrator_core-1.2.0/orchestrator/migrations/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -460,15 +460,15 @@
             ),
             product_block_name=product_block,
             new_resource_types=tuple(resource_types.keys()),
         )
     return resource_type_ids
 
 
-def create(conn: sa.engine.Connection, new: Dict) -> None:
+def create(conn: sa.engine.Connection, new: Dict) -> None:  # noqa: C901
     """Call other functions in this file based on the schema.
 
     Args:
         conn: DB connection as available in migration main file
         new: a dict with everything you want to make and link
 
     Example:
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/migrations/templates/alembic.ini.j2` & `orchestrator_core-1.2.0/orchestrator/migrations/templates/alembic.ini.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/migrations/templates/env.py.j2` & `orchestrator_core-1.2.0/orchestrator/migrations/templates/env.py.j2`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py` & `orchestrator_core-1.2.0/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py` & `orchestrator_core-1.2.0/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py` & `orchestrator_core-1.2.0/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py` & `orchestrator_core-1.2.0/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py` & `orchestrator_core-1.2.0/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py` & `orchestrator_core-1.2.0/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py` & `orchestrator_core-1.2.0/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py` & `orchestrator_core-1.2.0/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/migrations/versions/schema/2023-05-25_b1970225392d_add_subscription_metadata_workflow.py` & `orchestrator_core-1.2.0/orchestrator/migrations/versions/schema/2023-05-25_b1970225392d_add_subscription_metadata_workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/schedules/__init__.py` & `orchestrator_core-1.2.0/orchestrator/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/schedules/resume_workflows.py` & `orchestrator_core-1.2.0/orchestrator/schedules/resume_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/schedules/scheduling.py` & `orchestrator_core-1.2.0/orchestrator/schedules/scheduling.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/schedules/task_vacuum.py` & `orchestrator_core-1.2.0/orchestrator/schedules/task_vacuum.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/schedules/validate_products.py` & `orchestrator_core-1.2.0/orchestrator/schedules/validate_products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/schedules/validate_subscriptions.py` & `orchestrator_core-1.2.0/orchestrator/schedules/validate_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/schemas/__init__.py` & `orchestrator_core-1.2.0/orchestrator/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/schemas/base.py` & `orchestrator_core-1.2.0/orchestrator/schemas/base.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/schemas/engine_settings.py` & `orchestrator_core-1.2.0/orchestrator/schemas/engine_settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/schemas/fixed_input.py` & `orchestrator_core-1.2.0/orchestrator/schemas/fixed_input.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/schemas/problem_detail.py` & `orchestrator_core-1.2.0/orchestrator/schemas/problem_detail.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/schemas/process.py` & `orchestrator_core-1.2.0/orchestrator/schemas/process.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     id: UUID
 
 
 class ProcessForm(OrchestratorBaseModel):
     title: str
     type: str
     properties: Dict[str, Any]
-    additionalProperties: bool
+    additionalProperties: bool  # noqa: N815
     required: List[str] = []
     definitions: Optional[Dict[str, Any]]
 
 
 class ProcessBaseSchema(OrchestratorBaseModel):
     id: UUID
     workflow_name: str
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/schemas/product.py` & `orchestrator_core-1.2.0/orchestrator/schemas/product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/schemas/product_block.py` & `orchestrator_core-1.2.0/orchestrator/schemas/product_block.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/schemas/resource_type.py` & `orchestrator_core-1.2.0/orchestrator/schemas/resource_type.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/schemas/subscription.py` & `orchestrator_core-1.2.0/orchestrator/schemas/subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/schemas/subscription_descriptions.py` & `orchestrator_core-1.2.0/orchestrator/schemas/subscription_descriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/schemas/workflow.py` & `orchestrator_core-1.2.0/orchestrator/schemas/workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/security.py` & `orchestrator_core-1.2.0/orchestrator/security.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from authlib.integrations.starlette_client import OAuth
-from nwastdlib.url import URL
 from oauth2_lib.fastapi import OIDCUser, opa_decision, opa_graphql_decision
 
+from nwastdlib.url import URL
 from orchestrator.settings import oauth2_settings
 
 oauth_client_credentials = OAuth()
 
 well_known_endpoint = URL(oauth2_settings.OIDC_CONF_WELL_KNOWN_URL)
 
 oauth_client_credentials.register(
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/services/__init__.py` & `orchestrator_core-1.2.0/orchestrator/services/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/services/celery.py` & `orchestrator_core-1.2.0/orchestrator/services/celery.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/services/processes.py` & `orchestrator_core-1.2.0/orchestrator/services/processes.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 from http import HTTPStatus
 from typing import Any, Callable, Dict, List, Literal, Optional, Tuple
 from uuid import UUID, uuid4
 
 import structlog
 from deepmerge import Merger
 from fastapi import Request
-from nwastdlib.ex import show_ex
 from sqlalchemy.orm import joinedload
 
+from nwastdlib.ex import show_ex
 from orchestrator.api.error_handling import raise_status
 from orchestrator.config.assignee import Assignee
 from orchestrator.db import EngineSettingsTable, ProcessStepTable, ProcessSubscriptionTable, ProcessTable, db
 from orchestrator.distlock import distlock_manager
 from orchestrator.forms import FormValidationError, post_process
 from orchestrator.schemas.engine_settings import WorkerStatus
 from orchestrator.settings import ExecutorType, app_settings
@@ -39,17 +39,16 @@
 from orchestrator.websocket import (
     WS_CHANNELS,
     create_process_websocket_data,
     send_process_data_to_websocket,
     websocket_manager,
 )
 from orchestrator.websocket.websocket_manager import WebSocketManager
-from orchestrator.workflow import Failed
+from orchestrator.workflow import Failed, ProcessStat, ProcessStatus, Step, StepList, Success, Workflow, abort_wf, runwf
 from orchestrator.workflow import Process as WFProcess
-from orchestrator.workflow import ProcessStat, ProcessStatus, Step, StepList, Success, Workflow, abort_wf, runwf
 from orchestrator.workflows import get_workflow
 from orchestrator.workflows.removed_workflow import removed_workflow
 
 logger = structlog.get_logger(__name__)
 
 StateMerger = Merger([(dict, ["merge"])], ["override"], ["override"])
 
@@ -61,16 +60,15 @@
 def get_execution_context() -> Dict[str, Callable]:
     from orchestrator.services.celery import CELERY_EXECUTION_CONTEXT
 
     return CELERY_EXECUTION_CONTEXT if app_settings.EXECUTOR == ExecutorType.WORKER else THREADPOOL_EXECUTION_CONTEXT
 
 
 def get_thread_pool() -> ThreadPoolExecutor:
-    """
-    Get and optionally initialise a ThreadPoolExecutor.
+    """Get and optionally initialise a ThreadPoolExecutor.
 
     Returns:
         ThreadPoolExecutor
 
     """
     global _workflow_executor
     if _workflow_executor is None:
@@ -240,16 +238,15 @@
 
         # Try writing the failure, but return the original exception on success
         # on a second failure the exception should be handled higher
         return _db_log_step(stat, step, failure, broadcast_func=broadcast_func)
 
 
 def _db_log_process_ex(pid: UUID, ex: Exception) -> None:
-    """
-    Write the exception to the process or task when everything else has failed.
+    """Write the exception to the process or task when everything else has failed.
 
     Args:
         pid: the pid of the workflow process
         ex: the Exception message
 
     Returns: None, there is no one to listen at this point
 
@@ -289,20 +286,20 @@
         raise_status(HTTPStatus.NOT_FOUND, f"Process with pid {pid} not found")
 
     return process
 
 
 def _run_process_async(pid: UUID, f: Callable) -> UUID:
     def _update_running_processes(method: Literal["+", "-"], *args: Any) -> None:
-        """
-        Update amount of running processes by one.
+        """Update amount of running processes by one.
 
         Args:
             method: Add or subtract by one the amount of running processes
             args: Any args that are still going to be passed. When called as a callback this will be the future.
+
         Returns:
             None
 
         """
         engine_settings = EngineSettingsTable.query.with_for_update().one()
         engine_settings.running_processes += 1 if method == "+" else -1
         if engine_settings.running_processes < 0:
@@ -503,14 +500,15 @@
     broadcast_func: Optional[Callable] = None,
 ) -> bool:
     """Asynchronously resume multiple failed processes.
 
     Args:
         processes: Processes from database
         user_name: User who requested resuming the processes
+        broadcast_func: The broadcast functionality
 
     Returns:
         True if the resume-all operation has been started.
         False if it has not been started because it is already running.
 
     """
     lock_expiration = max(30, len(processes) // 10)
@@ -522,15 +520,15 @@
             for _proc in processes:
                 try:
                     process = _get_process(_proc.pid)
                     if process.last_status == ProcessStatus.RUNNING:
                         # Process has been started by something else in the meantime
                         logger.info("Cannot resume a running process", pid=_proc.pid)
                         continue
-                    elif process.last_status == ProcessStatus.RESUMED:
+                    elif process.last_status == ProcessStatus.RESUMED:  # noqa: RET507
                         # Process has been resumed by something else in the meantime
                         logger.info("Cannot resume a resumed process", pid=_proc.pid)
                         continue
                     resume_process(process, user=user_name, broadcast_func=broadcast_func)
                 except Exception:
                     logger.exception("Failed to resume process", pid=_proc.pid)
             logger.info("Completed resuming processes")
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/services/products.py` & `orchestrator_core-1.2.0/orchestrator/services/products.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,16 +19,15 @@
 from sqlalchemy.orm import joinedload
 
 from orchestrator.db import ProductTable
 from orchestrator.types import UUIDstr
 
 
 def get_product_by_id(product_id: Union[UUID, UUIDstr]) -> ProductTable:
-    """
-    Get product by id.
+    """Get product by id.
 
     Args:
         product_id: ProductTable id uuid
 
     Returns: ProductTable object
 
     """
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/services/settings.py` & `orchestrator_core-1.2.0/orchestrator/services/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,42 +23,41 @@
 from orchestrator.services.processes import SYSTEM_USER, resume_process
 from orchestrator.settings import app_settings
 
 logger = structlog.get_logger(__name__)
 
 
 def post_update_to_slack(engine_status: EngineSettingsSchema, user: str) -> None:
-    """
-    Post engine settings update to slack.
+    """Post engine settings update to slack.
 
     Args:
         engine_status: EngineStatus
+        user: The user who executed the change
 
     Returns:
         None
 
     """
     try:
         if engine_status.global_lock is True:
             action = f"stopped the `{app_settings.ENVIRONMENT}` workflow engine. The orchestrator will pause all running processes."
         else:
             action = f"started the `{app_settings.ENVIRONMENT}` workflow engine. The orchestrator will pick up all pending processes."
 
         message = {"text": f"User `{user}` {action}"}
-        requests.post(app_settings.SLACK_ENGINE_SETTINGS_HOOK_URL, json=message)
+        requests.post(app_settings.SLACK_ENGINE_SETTINGS_HOOK_URL, json=message, timeout=5)
 
     # Catch all Request exceptions and log. Then pass
     except RequestException:
         logger.exception("Post to slack failed.")
         pass
 
 
 def marshall_processes(engine_settings: EngineSettingsTable, new_global_lock: bool) -> Optional[EngineSettingsTable]:
-    """
-    Manage processes depending on the engine status.
+    """Manage processes depending on the engine status.
 
     This function only has to act when in the transitioning fases, i.e Pausing and Starting
 
     Args:
         engine_settings: Engine status containing the lock and status fields
         new_global_lock: The state to which needs to be transitioned
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/services/subscriptions.py` & `orchestrator_core-1.2.0/orchestrator/services/subscriptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,24 +85,22 @@
     try:
         subscription = query.get(subscription_id)
     except SQLAlchemyError as e:
         raise ValueError("Invalid subscription id") from e
 
     if subscription:
         return subscription
-    else:
-        raise ValueError(f"Subscription with {subscription_id} does not exist in the database")
+    raise ValueError(f"Subscription with {subscription_id} does not exist in the database")
 
 
 def get_subscription_metadata(subscription_id: UUIDstr) -> Optional[dict]:
     subscription_metadata = SubscriptionMetadataTable.find_by_subscription_id(subscription_id)
     if subscription_metadata:
         return subscription_metadata.metadata_
-    else:
-        return None
+    return None
 
 
 def update_subscription_status(subscription_id: UUIDstr, status: str) -> SubscriptionTable:
     """Update the subscription status.
 
     Args:
         subscription_id: Id of the subscription to update.
@@ -178,28 +176,28 @@
 
 
 def unsync(subscription_id: UUIDstr, checked: bool = True) -> SubscriptionTable:
     """Unsync subscription by subscription id.
 
     Args:
         subscription_id: Subscription id of the subscription
+        checked: Checked or not
 
     Returns: Updated subscription object
 
     """
     subscription = get_subscription(subscription_id, for_update=True)
     if checked and not subscription.insync:
         raise ValueError("Subscription is already out of sync, cannot continue!")
     subscription.insync = False
     return subscription
 
 
 def resync(subscription_id: UUIDstr) -> SubscriptionTable:
-    """
-    Resync subscription by subscription id.
+    """Resync subscription by subscription id.
 
     Args:
         subscription_id: Subscription id of the subscription
 
     Returns: Updated subscription object
 
     """
@@ -231,16 +229,15 @@
     )
     db.session.add(subscription)
 
     return subscription.subscription_id
 
 
 def update_subscription(subscription_id: str, **attrs: Union[Dict, UUIDstr, str, datetime]) -> SubscriptionTable:
-    """
-    Update the subscription.
+    """Update the subscription.
 
     Args:
         subscription_id: SubscriptionTable id of the subscription
         attrs: Attributes that will be set
 
     Returns: Subscription
 
@@ -251,48 +248,45 @@
     for key, value in attrs.items():
         setattr(subscription, key, value)
 
     return subscription
 
 
 def retrieve_node_subscriptions_by_name(node_name: str) -> List[SubscriptionTable]:
-    node_subscriptions = (
+    return (
         SubscriptionTable.query.join(
             ProductTable, SubscriptionInstanceTable, SubscriptionInstanceValueTable, ResourceTypeTable
         )
         .filter(SubscriptionInstanceValueTable.value == node_name)
         .filter(ResourceTypeTable.resource_type == "nso_device_id")
         .filter(SubscriptionTable.status.in_(["active", "provisioning"]))
         .all()
     )
-    return node_subscriptions
 
 
 def retrieve_subscription_by_subscription_instance_value(
     resource_type: str, value: str, sub_status: Tuple = ("provisioning", "active")
 ) -> Optional[SubscriptionTable]:
-    """
-    Retrieve a Subscriptions by resource_type and value.
+    """Retrieve a Subscriptions by resource_type and value.
 
     Args:
         resource_type: name of the resource type
         value: value of the resource type
         sub_status: status of the subscriptions
 
     Returns: Subscription or None
 
     """
-    subscription = (
+    return (
         SubscriptionTable.query.join(SubscriptionInstanceTable, SubscriptionInstanceValueTable, ResourceTypeTable)
         .filter(SubscriptionInstanceValueTable.value == value)
         .filter(ResourceTypeTable.resource_type == resource_type)
         .filter(SubscriptionTable.status.in_(sub_status))
         .one_or_none()
     )
-    return subscription
 
 
 def find_values_for_resource_types(
     subscription_id: Union[UUID, UUIDstr], resource_types: Sequence[str], strict: bool = True
 ) -> Dict[str, List[str]]:
     """Find values for resource types by subscription ID.
 
@@ -350,16 +344,15 @@
         missing = set(resource_types) - set(rt2v.keys())
         if missing:
             raise ValueError(f"Could not find requested resource types: '{','.join(missing)}'!")
     return rt2v
 
 
 def query_in_use_by_subscriptions(subscription_id: UUID, filter_statuses: Optional[List[str]] = None) -> Query:
-    """
-    Return a query with all subscriptions -in_use_by- that use this subscription with resource_type or direct relation.
+    """Return a query with all subscriptions -in_use_by- that use this subscription with resource_type or direct relation.
 
     The query can be used to add extra filters when/where needed.
     """
     # Find relations through resource types
     resource_type_relations = (
         SubscriptionTable.query.join(SubscriptionInstanceTable)
         .options(joinedload("customer_descriptions"))
@@ -388,16 +381,15 @@
             SubscriptionTable.subscription_id.in_(relation_relations.scalar_subquery()),
         ),
         SubscriptionTable.status.in_(filter_statuses if filter_statuses else SubscriptionLifecycle.values()),
     )
 
 
 def query_depends_on_subscriptions(subscription_id: UUID, filter_statuses: Optional[List[str]] = None) -> Query:
-    """
-    Return a query with all subscriptions -depends_on- that this subscription is dependent on with resource_type or direct relation.
+    """Return a query with all subscriptions -depends_on- that this subscription is dependent on with resource_type or direct relation.
 
     The query can be used to add extra filters when/where needed.
     """
     # Find relations through resource types
     resource_type_relations = (
         SubscriptionInstanceTable.query.join(SubscriptionInstanceValueTable)
         .join(ResourceTypeTable)
@@ -484,16 +476,15 @@
     return result
 
 
 def get_relations(subscription_id: UUIDstr) -> Dict[str, List[UUID]]:
     subscription_table = SubscriptionTable.query.options(joinedload("product"), joinedload("product.workflows")).get(
         subscription_id
     )
-    relations = status_relations(subscription_table)
-    return relations
+    return status_relations(subscription_table)
 
 
 TARGET_DEFAULT_USABLE_MAP: Dict[Target, List[str]] = {
     Target.CREATE: [],
     Target.MODIFY: ["active"],
     Target.TERMINATE: ["active", "provisioning"],
     Target.SYSTEM: ["active"],
@@ -504,16 +495,15 @@
 WF_BLOCKED_BY_PARENTS: Dict[str, bool] = {}
 WF_BLOCKED_BY_IN_USE_BY_SUBSCRIPTIONS: Dict[str, bool] = {}
 
 WF_USABLE_WHILE_OUT_OF_SYNC: List[str] = ["modify_note"]
 
 
 def subscription_workflows(subscription: SubscriptionTable) -> Dict[str, Any]:
-    """
-    Return a dict containing all the workflows a user can start for this subscription.
+    """Return a dict containing all the workflows a user can start for this subscription.
 
     Args:
         subscription: an SqlAlchemy instance of a `db.SubscriptionTable`
 
     Returns:
         A dictionary with the following structure (reason and its related keys are only present when workflows are blocked):
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/services/tasks.py` & `orchestrator_core-1.2.0/orchestrator/services/tasks.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,24 +40,23 @@
 RESUME_TASK = "tasks.resume_task"
 RESUME_WORKFLOW = "tasks.resume_workflow"
 
 
 def get_celery_task(task_name: str) -> Task:
     if _celery:
         return _celery.signature(task_name)
-    else:
-        raise AssertionError("Celery has not been initialised yet")
+    raise AssertionError("Celery has not been initialised yet")
 
 
 def register_custom_serializer() -> None:
     # orchestrator specific serializer to correctly handle more complex classes
     registry.register("orchestrator-json", json_dumps, json_loads, "application/json", "utf-8")
 
 
-def initialise_celery(celery: Celery) -> None:
+def initialise_celery(celery: Celery) -> None:  # noqa: C901
     global _celery
     if _celery:
         raise AssertionError("You can only initialise Celery once")
     _celery = celery
 
     # Different routes/queues so we can assign them priorities
     celery.conf.task_routes = {
@@ -134,11 +133,11 @@
             return
 
         inspection: Inspect = _celery.control.inspect()
         stats = inspection.stats()
         self.number_of_workers_online = len(stats)
 
         def sum_items(d: dict) -> int:
-            return sum(len(l) for _, l in d.items()) if d else 0
+            return sum(len(lines) for _, lines in d.items()) if d else 0
 
         self.number_of_queued_jobs = sum_items(inspection.scheduled()) + sum_items(inspection.reserved())
         self.number_of_running_jobs = sum(len(tasks) for w, tasks in inspection.active().items())
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/services/translations.py` & `orchestrator_core-1.2.0/orchestrator/services/translations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/settings.py` & `orchestrator_core-1.2.0/orchestrator/settings.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,18 +12,14 @@
 # limitations under the License.
 
 import secrets
 import string
 from pathlib import Path
 from typing import List, Optional
 
-from opentelemetry.exporter.otlp.proto.grpc.trace_exporter import OTLPSpanExporter
-from opentelemetry.sdk.resources import SERVICE_NAME, Resource
-from opentelemetry.sdk.trace import TracerProvider
-from opentelemetry.sdk.trace.export import BatchSpanProcessor
 from pydantic import BaseSettings, PostgresDsn, RedisDsn
 
 from orchestrator.types import strEnum
 
 
 class ExecutorType(strEnum):
     WORKER = "celery"
@@ -86,13 +82,7 @@
     OAUTH2_TOKEN_URL: str = ""
     OIDC_CONF_WELL_KNOWN_URL: str = ""
     OPA_URL: str = "http://127.0.0.1:8181/v1/data/automation/authorization/allow"
 
 
 app_settings = AppSettings()
 oauth2_settings = Oauth2Settings()
-
-# Tracer settings
-tracer_provider = TracerProvider(resource=Resource.create({SERVICE_NAME: app_settings.SERVICE_NAME}))
-
-otlp_exporter = OTLPSpanExporter(endpoint=app_settings.TRACE_HOST)
-tracer_provider.add_span_processor(BatchSpanProcessor(otlp_exporter))
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/targets.py` & `orchestrator_core-1.2.0/orchestrator/targets.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/types.py` & `orchestrator_core-1.2.0/orchestrator/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,16 +212,15 @@
         elif issubclass(get_origin(t), list):  # type: ignore
             if test_type and get_args(t):
                 first_arg = get_args(t)[0]
                 # To support a list with union of multiple product blocks.
                 if is_union_type(first_arg) and get_args(first_arg) and not is_union_type(test_type):
                     first_arg = get_args(first_arg)[0]
                 return is_of_type(first_arg, test_type)
-            else:
-                return True
+            return True
 
     return False
 
 
 def is_optional_type(t: Any, test_type: Optional[type] = None) -> bool:
     """Check if `t` is optional type (Union[None, ...]).
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/utils/__init__.py` & `orchestrator_core-1.2.0/orchestrator/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/utils/crypt.py` & `orchestrator_core-1.2.0/orchestrator/utils/crypt.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/utils/datetime.py` & `orchestrator_core-1.2.0/orchestrator/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/utils/docs.py` & `orchestrator_core-1.2.0/orchestrator/utils/docs.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""
-Functions for automatically generating docs for workflows and domain models.
+"""Functions for automatically generating docs for workflows and domain models.
 
 WARNING: When developing on these auto generated docs,
     sphinx does not rebuild the files where these functions are called. To see your changes reflected you need to
     change or ``touch`` the file in question. Or use ``make clean docs``
 
 WARNING2: Since we use the sphinx napoleon extension and the docstrings we generate are parsed by that.
     You cannot use all rst but you need to conform to google style docstring syntax. This also means that
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/utils/errors.py` & `orchestrator_core-1.2.0/orchestrator/utils/errors.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,22 +12,23 @@
 # limitations under the License.
 
 
 from http import HTTPStatus
 from typing import Dict, Optional, cast
 
 import structlog
-from nwastdlib.ex import show_ex
+from deprecated import deprecated
 
+from nwastdlib.ex import show_ex
 from orchestrator.types import JSON, ErrorDict
 
 logger = structlog.get_logger(__name__)
 
 
-class ApiException(Exception):
+class ApiException(Exception):  # noqa: N818
     """Api Exception Class.
 
     This is a copy of what is generated in api_clients. We use this to have consistent error handling for nso to.
     This should conform to what is used in the api clients.
     """
 
     status: Optional[HTTPStatus]
@@ -58,25 +59,39 @@
 
         if self.body:
             error_message += f"HTTP response body: {self.body}\n"
 
         return error_message
 
 
-class ProcessFailure(Exception):
+class ProcessFailureError(Exception):
     message: str
     details: JSON
 
     def __init__(self, message: str, details: JSON = None) -> None:
         super().__init__(message, details)
         self.message = message
         self.details = details
 
 
-class InconsistentData(ProcessFailure):
+@deprecated(
+    "Renamed the error 'ProcessFailure', `from orchestrator.errors import ProcessFailureError` removing in version 1.3.0"
+)
+class ProcessFailure(ProcessFailureError):  # noqa: N818
+    pass
+
+
+class InconsistentDataError(ProcessFailureError):
+    pass
+
+
+@deprecated(
+    "Renamed the error 'InconsistentDataError', `from orchestrator.errors import InconsistentDataError` removing in version 1.3.0"
+)
+class InconsistentDataException(InconsistentDataError):  # noqa: N818
     pass
 
 
 def is_api_exception(ex: Exception) -> bool:
     """Test for swagger-codegen ApiException.
 
     For each API, swagger-codegen generates a new ApiException class. These are not organized into
@@ -98,21 +113,21 @@
 
     Args:
         err: Exception
     Returns:
         An ErrorDict containing the error message a status_code and a traceback if available
 
     """
-    if isinstance(err, ProcessFailure):
+    if isinstance(err, ProcessFailureError):
         return {"class": type(err).__name__, "error": err.message, "traceback": show_ex(err), "details": err.details}
-    elif is_api_exception(err):
+
+    if is_api_exception(err):
         err = cast(ApiException, err)
         return {
             "class": type(err).__name__,
             "error": err.reason,
             "status_code": err.status,
             "body": err.body,
             "headers": "\n".join(f"{k}: {v}" for k, v in err.headers.items()),
             "traceback": show_ex(err),
         }
-    else:
-        return {"class": type(err).__name__, "error": str(err), "traceback": show_ex(err)}
+    return {"class": type(err).__name__, "error": str(err), "traceback": show_ex(err)}
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/utils/functional.py` & `orchestrator_core-1.2.0/orchestrator/utils/functional.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/utils/helpers.py` & `orchestrator_core-1.2.0/orchestrator/utils/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,20 +71,18 @@
         logger.warning("Found unused keys", keys=keys)
 
 
 def map_value(mapping: dict[str, Callable], k: str, v: Any) -> tuple[Any, ...]:
     if f := mapping.get(k):
         if v is None:
             return k, None
-        elif type(v) == dict:
+        if type(v) == dict:
             return result if type(result := f(**v)) is tuple else (k, result)
-        else:
-            return result if type(result := f(v)) is tuple else (k, result)
-    else:
-        return k, v
+        return result if type(result := f(v)) is tuple else (k, result)
+    return k, v
 
 
 def to_camel(s: str) -> str:
     first, *rest = s.split("_")
     return first + "".join(word.title() for word in rest)
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/utils/json.py` & `orchestrator_core-1.2.0/orchestrator/utils/json.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,16 +109,15 @@
         orjson_options |= json.OPT_INDENT_2
     try:
         return json.dumps(obj, default=to_serializable, option=orjson_options).decode("utf8")
     except TypeError as e:
         # When Recursion limit is not configurable in orjson, falling back to the next best lib.
         if str(e) == "default serializer exceeds recursion limit":
             return rjson.dumps(obj, default=to_serializable)
-        else:
-            raise e
+        raise e
 
 
 def to_serializable(o: Any) -> Any:
     """Convert an object into an object that the JSON encode can serialize.
 
     Args:
         o: Object to convert.
@@ -177,16 +176,15 @@
                 timestamp = datetime.fromisoformat(v)
                 assert timestamp.tzinfo is not None, "All timestamps should contain timezone information."  # noqa: S101
                 dct[k] = timestamp
     return dct
 
 
 def non_none_dict(dikt: Sequence[Tuple[str, Any]]) -> Dict[Any, Any]:
-    """
-    Return no `None` values in a Dict.
+    """Return no `None` values in a Dict.
 
     This function may be used in the `asdict()` method as dictionary factory.
 
     Args:
         dikt: Tuple of values where
 
     Returns:
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/utils/redis.py` & `orchestrator_core-1.2.0/orchestrator/utils/redis.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,19 +47,17 @@
 def from_redis(subscription_id: UUID) -> Optional[Tuple[Any, str]]:
     if caching_models_enabled():
         logger.info("Retrieving subscription from cache", subscription=subscription_id)
         obj = cache.get(f"domain:{subscription_id}")
         etag = cache.get(f"domain:etag:{subscription_id}")
         if obj and etag:
             return json_loads(obj), etag.decode("utf-8")
-        else:
-            return None
-    else:
-        logger.warning("Caching disabled, not loading subscription", subscription=subscription_id)
         return None
+    logger.warning("Caching disabled, not loading subscription", subscription=subscription_id)
+    return None
 
 
 def delete_from_redis(subscription_id: UUID) -> None:
     if caching_models_enabled():
         logger.info("Deleting subscription object from cache", subscription_id=subscription_id)
         cache.delete(f"domain:{subscription_id}")
         cache.delete(f"domain:etag:{subscription_id}")
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/utils/show_process.py` & `orchestrator_core-1.2.0/orchestrator/utils/show_process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/utils/speed.py` & `orchestrator_core-1.2.0/orchestrator/utils/speed.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/utils/state.py` & `orchestrator_core-1.2.0/orchestrator/utils/state.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,30 +64,28 @@
     - have a top level key `light_path` with a `str` or `UUID` value for the associated `subscription_id`
     - have a top level key `light_path` with dict representation of the domain model.
 
     In case of the latter, the `subscription_id` is represented by the key `subscription_id` in the dict
     representation of the domain model.
 
     Args:
-        data: the state like dict
-        name: name of the variable representing a domain model
+        val: The value of the subscription id
 
     Returns:
         A UUID if found, None otherwise.
 
     """
     if isinstance(val, dict):
         val = val.get("subscription_id")
     elif isinstance(val, SubscriptionModel):
         raise AssertionError("There should be no SubscriptionModel instances in the state before a step!")
     elif isinstance(val, UUID):
         return val
     try:
-        uuid = UUID(val)
-        return uuid
+        return UUID(val)
     except Exception:
         return None
 
 
 def _save_models(state: State) -> None:
     """Save all domain models found under a key in the state.
 
@@ -133,15 +131,15 @@
         elif isinstance(value, list):
             _save_models({f"{key}.{i}": v for i, v in enumerate(value)})
         elif isinstance(value, dict):
             # traverse entire state, depth first
             _save_models(value)
 
 
-def _build_arguments(func: Union[StepFunc, InputStepFunc], state: State) -> List:
+def _build_arguments(func: Union[StepFunc, InputStepFunc], state: State) -> List:  # noqa: C901
     """Build actual arguments based on step function signature and state.
 
     What the step function requests in its function signature it what this function retrieves from the state or DB.
     Domain models are retrieved from the DB (after `subscription_id` lookup in the state). Everything else is
     retrieved from the state.
 
     For domain models only ``Optional`` and ``List`` are supported as container types. Union, Dict and others are not supported
@@ -328,11 +326,10 @@
 
     else:
         simple_func = cast(SimpleInputFormGenerator, func)
 
         @wraps(simple_func)
         def wrapper(state: State) -> Optional[InputForm]:
             args = _build_arguments(simple_func, state)
-            new_state = simple_func(*args)
-            return new_state
+            return simple_func(*args)
 
     return wrapper
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/utils/strings.py` & `orchestrator_core-1.2.0/orchestrator/utils/strings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/utils/vlans.py` & `orchestrator_core-1.2.0/orchestrator/utils/vlans.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,17 @@
         VlanRanges([[4], [10,12], [11,14]])
         VlanRanges([(4, 4), (10, 14)])
 
     """
 
     _vlan_ranges: Tuple[range, ...]
 
-    def __init__(self, val: Optional[Union[str, int, Iterable[int], Sequence[Sequence[int]]]] = None) -> None:
+    def __init__(  # noqa: C901
+        self, val: Optional[Union[str, int, Iterable[int], Sequence[Sequence[int]]]] = None
+    ) -> None:
         # The idea is to bring all acceptable values to one canonical intermediate format: the `Sequence[Sequence[
         # int]]`. Where the inner sequence is either a one or two element sequence. The one element sequence
         # represents a single VLAN, the two element sequence represents a VLAN range.
         #
         # An example of this intermediate format is::
         #
         #     vlans = [[5], [10, 12]]
@@ -63,15 +65,16 @@
         # This intermediate format happens to be the format as accepted by :func:`expand_ranges`. This function has
         # the advantage of deduplicating overlapping ranges or VLANs specified more than once. In addition its return
         # value can be use as input to the :func:`to_ranges` function.
         vlans: Sequence[Sequence[int]] = []
         if val is None:
             self._vlan_ranges = ()
             return
-        elif isinstance(val, str):
+
+        if isinstance(val, str):
             if val.strip() != "":
                 # This might look complex, but it does handle strings such as `"  3, 4, 6-9, 4, 8 - 10"`
                 try:
                     vlans = list(map(lambda s: list(map(int, s.strip().split("-"))), val.split(",")))
                 except ValueError:
                     raise ValueError(f"{val} could not be converted to a {self.__class__.__name__} object.")
         elif isinstance(val, int):
@@ -149,16 +152,15 @@
         return hash(self._vlan_ranges)
 
     def __sub__(self, other: Union[int, AbstractSet[Any]]) -> VlanRanges:
         if isinstance(other, int):
             new_set = set(self)
             new_set.remove(other)
             return VlanRanges(new_set)
-        else:
-            return VlanRanges(set(self) - set(other))
+        return VlanRanges(set(self) - set(other))
 
     def __and__(self, other: AbstractSet[Any]) -> VlanRanges:
         return VlanRanges(set(self) & set(other))
 
     def __or__(self, other: AbstractSet[Any]) -> VlanRanges:
         return VlanRanges(set(self) | set(other))
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/version.py` & `orchestrator_core-1.2.0/orchestrator/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,15 @@
 
 import structlog
 
 logger = structlog.getLogger(__name__)
 
 
 def __getattr__(name: str) -> Optional[str]:
-    """
-    Return the GIT_COMMIT_HASH.
+    """Return the GIT_COMMIT_HASH.
 
     Usage::
 
         from orchestrator.version import GIT_COMMIT_HASH
         print(GIT_COMMIT_HASH)
 
     Args:
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/websocket/__init__.py` & `orchestrator_core-1.2.0/orchestrator/websocket/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         else:
             logger.warning("WebSocketManager object not configured, ENABLE_WEBSOCKETS is false.")
 
     def __getattr__(self, attr: str) -> Any:
         if not isinstance(self.wrapped_websocket_manager, WebSocketManager):
             if "_" in attr:
                 logger.warning("No WebSocketManager configured, but attempting to access class methods")
-                return
+                return None
             raise RuntimeWarning(
                 "No WebSocketManager configured at this time. Please pass WebSocketManager configuration to OrchestratorCore base_settings"
             )
         if attr != "enabled" and not self.wrapped_websocket_manager.enabled:
             logger.warning("Websockets are disabled, unable to access class methods")
             return empty_fn
 
@@ -89,15 +89,15 @@
 def send_process_data_to_websocket(
     pid: UUID,
     data: Dict,
     broadcast_func: Optional[BroadcastFunc] = None,
 ) -> None:
     """Broadcast data of the current process to connected websocket clients."""
     if not websocket_manager.enabled:
-        return None
+        return
 
     if broadcast_func:
         logger.debug("Broadcast process data through broadcast_func", pid=str(pid))
         broadcast_func(pid, data)
     else:
         logger.debug("Broadcast process data directly to websocket_manager", pid=str(pid))
         loop = new_event_loop()
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/websocket/managers/broadcast_websocket_manager.py` & `orchestrator_core-1.2.0/orchestrator/websocket/managers/broadcast_websocket_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/websocket/managers/memory_websocket_manager.py` & `orchestrator_core-1.2.0/orchestrator/websocket/managers/memory_websocket_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/websocket/websocket_manager.py` & `orchestrator_core-1.2.0/orchestrator/websocket/websocket_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/workflow.py` & `orchestrator_core-1.2.0/orchestrator/workflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,18 +32,18 @@
     overload,
     runtime_checkable,
 )
 from uuid import UUID
 
 import strawberry
 import structlog
-from nwastdlib import const, identity
 from structlog.contextvars import bound_contextvars
 from structlog.stdlib import BoundLogger
 
+from nwastdlib import const, identity
 from orchestrator.config.assignee import Assignee
 from orchestrator.db import EngineSettingsTable, db, transactional
 from orchestrator.forms import FormPage
 from orchestrator.targets import Target
 from orchestrator.types import (
     ErrorDict,
     FormGenerator,
@@ -143,42 +143,43 @@
             # ensure we return a StepList and not a regular list.
             retval = type(self)(retval)
         return retval
 
     def __rshift__(self, other: Union[StepList, Step]) -> StepList:
         if isinstance(other, Step):
             return StepList([*self, other])
-        elif isinstance(other, StepList):
+
+        if isinstance(other, StepList):
             return StepList([*self, *other])
-        elif hasattr(other, "__name__"):  # type:ignore
+
+        if hasattr(other, "__name__"):  # type:ignore
             raise ValueError(
                 f"Expected @step decorated function or type Step or StepList, got {type(other)} with name {other.__name__} instead."
             )
-        else:
-            raise ValueError(f"Expected @step decorated function or type Step or StepList, got {type(other)} instead.")
+        raise ValueError(f"Expected @step decorated function or type Step or StepList, got {type(other)} instead.")
 
     def __str__(self) -> str:
         return f"StepList [{', '.join(x.name for x in self)}]"
 
     def __repr__(self) -> str:
         return f"StepList [{', '.join(repr(x) for x in self)}]"
 
 
 def _handle_simple_input_form_generator(f: StateInputStepFunc) -> StateInputFormGenerator:
     if inspect.isgeneratorfunction(f):
         return cast(StateInputFormGenerator, f)
     if inspect.isgenerator(f):
         raise ValueError("Got a generator object instead of function, this is not correct")
-    else:
-        # If f is a SimpleInputFormGenerator convert to new style generator function
-        def form_generator(state: State) -> FormGenerator:
-            user_input = yield cast(StateSimpleInputFormGenerator, f)(state)
-            return user_input.dict()
 
-        return form_generator
+    # If f is a SimpleInputFormGenerator convert to new style generator function
+    def form_generator(state: State) -> FormGenerator:
+        user_input = yield cast(StateSimpleInputFormGenerator, f)(state)
+        return user_input.dict()
+
+    return form_generator
 
 
 def make_workflow(
     f: Callable,
     description: str,
     initial_input_form: Optional[InputStepFunc],
     target: Optional[Target],
@@ -324,16 +325,15 @@
         def wrapper(state: State) -> Process:
             sub_state = get(state)
 
             result: Process = step(sub_state)
 
             if result.isfailed() or result.iswaiting():
                 return result
-            else:
-                return result.map(set(state))
+            return result.map(set(state))
 
         return make_step_function(wrapper, step.name, step.form, step.assignee)
 
     return wrap
 
 
 def focussteps(key: str) -> Callable[[Union[Step, StepList]], StepList]:
@@ -953,16 +953,15 @@
         >>> Suspend({"a":1}).resume(lambda s: Failed({"error": "Exception!!"}))
         Failed {'error': 'Exception!!'}
         """
 
         next_state = self._fold(Success, Success, Success, Success, Abort, Success, Complete)
 
         if self.issuspend():
-            result = resume_suspend(next_state)  # type: ignore
-            return result
+            return resume_suspend(next_state)  # type: ignore
 
         return next_state  # type: ignore
 
 
 class Success(Process[S]):
     def _fold(
         self,
@@ -1168,16 +1167,15 @@
 
     if not pstat.state.iscomplete():
         abort_func = make_step_function(Abort, "User Aborted")
 
         state = pstat.state.abort()
 
         return logstep(pstat, abort_func, state)
-    else:
-        return pstat.state
+    return pstat.state
 
 
 @_purestep("Start")
 def init(state: State) -> Process:
     """Start of workflow."""
     return Success(state)
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/workflows/__init__.py` & `orchestrator_core-1.2.0/orchestrator/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/workflows/modify_note.py` & `orchestrator_core-1.2.0/orchestrator/workflows/modify_note.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/workflows/removed_workflow.py` & `orchestrator_core-1.2.0/orchestrator/workflows/removed_workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/workflows/steps.py` & `orchestrator_core-1.2.0/orchestrator/workflows/steps.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,16 +35,15 @@
     """Transition a subscription to in sync."""
     subscription.insync = True
     return {"subscription": subscription}
 
 
 @step("Lock subscription")
 def unsync(subscription_id: UUIDstr, __old_subscriptions__: Optional[dict] = None) -> State:
-    """
-    Transition a subscription to out of sync.
+    """Transition a subscription to out of sync.
 
     This step will also create a backup of the current subscription details in the state with the key
     `__old_subscriptions__`
 
     Note:  This step will NOT overwrite any existing data in the state for the `__old_subscriptions__` key. Some
     workflows already change subscription details in the initial form step. This is not a best practice but
     it can be handy/needed for some scenarios. To ensure that you get a correct backup these forms need to create
@@ -136,42 +135,40 @@
     return _set_status
 
 
 @step("Remove domain model from cache")
 def remove_domain_model_from_cache(
     workflow_name: str, subscription: Optional[SubscriptionModel] = None, subscription_id: Optional[UUID] = None
 ) -> State:
-    """
-    Remove the domain model from the cache if it exists.
+    """Remove the domain model from the cache if it exists.
 
     Args:
         workflow_name: The workflow name
         subscription: Subscription Model
         subscription_id: The subscription id
 
     Returns:
         State
 
     """
 
     if not (subscription or subscription_id):
         logger.warning("No subscription found in this workflow", workflow_name=workflow_name)
         return {"deleted_subscription_id": None}
-    elif subscription:
+    if subscription:
         delete_from_redis(subscription.subscription_id)
     elif subscription_id:
         delete_from_redis(subscription_id)
 
     return {"deleted_subscription_id": subscription_id or subscription.subscription_id}  # type: ignore[union-attr]
 
 
 @step("Cache Subscription and related subscriptions")
-def cache_domain_models(workflow_name: str, subscription: Optional[SubscriptionModel] = None) -> State:
-    """
-    Attempt to cache all Subscriptions once they have been touched once.
+def cache_domain_models(workflow_name: str, subscription: Optional[SubscriptionModel] = None) -> State:  # noqa: C901
+    """Attempt to cache all Subscriptions once they have been touched once.
 
     Args:
         workflow_name: The Workflow Name
         subscription:  The Subscription if it exists.
 
     Returns:
         Returns State.
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/workflows/tasks/__init__.py` & `orchestrator_core-1.2.0/orchestrator/workflows/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/workflows/tasks/cleanup_tasks_log.py` & `orchestrator_core-1.2.0/orchestrator/workflows/tasks/cleanup_tasks_log.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/workflows/tasks/resume_workflows.py` & `orchestrator_core-1.2.0/orchestrator/workflows/tasks/resume_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/workflows/tasks/validate_products.py` & `orchestrator_core-1.2.0/orchestrator/workflows/tasks/validate_products.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,28 +25,28 @@
 from orchestrator.api.api_v1.endpoints.fixed_input import fi_configuration
 from orchestrator.db import FixedInputTable, ProductTable, SubscriptionTable, WorkflowTable
 from orchestrator.domain.base import SubscriptionModel
 from orchestrator.services import products
 from orchestrator.services.translations import generate_translations
 from orchestrator.targets import Target
 from orchestrator.types import State
-from orchestrator.utils.errors import ProcessFailure
+from orchestrator.utils.errors import ProcessFailureError
 from orchestrator.workflow import StepList, done, init, step, workflow
 
 # Since these errors are probably programming failures we should not throw AssertionErrors
 
 
 @step("Check all workflows in database")
 def check_all_workflows_are_in_db() -> State:
     all_workflows_in_db = {k.name for k in WorkflowTable.query.all()}
     all_workflows = {k for k in orchestrator.workflows.ALL_WORKFLOWS.keys()}  # noqa: C416
     not_in_db = all_workflows - all_workflows_in_db
     not_in_lwi = all_workflows_in_db - all_workflows
     if not_in_db or not_in_lwi:
-        raise ProcessFailure(
+        raise ProcessFailureError(
             "Found missing workflows in database or implementations",
             {
                 "Workflows not registered in the database": list(not_in_db),
                 "Workflows not registered in a `LazyWorkflowInstance`": list(not_in_lwi),
             },
         )
 
@@ -70,37 +70,37 @@
                     f"Workflow {wf.name}: {wf.target} <=> {db_workflow.target}, "
                     f"{wf.name} <=> {db_workflow.name} and {wf.description} <=> {db_workflow.description}. "
                 )
                 workflow_assertions.append(message)
 
     if workflow_assertions:
         workflow_message = "\n".join(workflow_assertions)
-        raise ProcessFailure("Workflows with none matching targets and descriptions", workflow_message)
+        raise ProcessFailureError("Workflows with none matching targets and descriptions", workflow_message)
 
     # Check translations
     translations = generate_translations("en-GB")["workflow"]
     workflow_assertions = []
     for key in orchestrator.workflows.ALL_WORKFLOWS:
         if key not in translations:
             workflow_assertions.append(key)
 
     if workflow_assertions:
         workflow_message = "\n".join(workflow_assertions)
-        raise ProcessFailure("Workflows with missing translations", workflow_message)
+        raise ProcessFailureError("Workflows with missing translations", workflow_message)
 
     return {"check_workflows_for_matching_targets_and_descriptions": True}
 
 
 @step("Check that all products have at least one workflow")
 def check_that_products_have_at_least_one_workflow() -> State:
     prods_without_wf = list(
         flatten(ProductTable.query.filter(not_(ProductTable.workflows.any())).with_entities(ProductTable.name))
     )
     if prods_without_wf:
-        raise ProcessFailure("Found products that do not have a workflow associated with them", prods_without_wf)
+        raise ProcessFailureError("Found products that do not have a workflow associated with them", prods_without_wf)
 
     return {"check_that_products_have_at_least_one_workflow": True}
 
 
 @step("Check that all products have a create, modify, terminate and validate workflow")
 def check_that_products_have_create_modify_and_terminate_workflows() -> State:
     product_data = ProductTable.query.filter(ProductTable.status == "active")
@@ -125,15 +125,15 @@
 @step("Check that all active products have a modify note")
 def check_that_active_products_have_a_modify_note() -> State:
     modify_workflow = WorkflowTable.query.filter(WorkflowTable.name == "modify_note").first()
 
     product_data = ProductTable.query.filter(ProductTable.status == "active").all()
     result = [product.name for product in product_data if modify_workflow not in product.workflows]
     if result:
-        raise ProcessFailure("Found products that do not have a modify_note workflow", result)
+        raise ProcessFailureError("Found products that do not have a modify_note workflow", result)
 
     return {"check_that_active_products_have_a_modify_note": True}
 
 
 @step("Check the DB fixed input config")
 def check_db_fixed_input_config() -> State:
     fixed_input_configuration = fi_configuration()
@@ -163,15 +163,15 @@
 
         if {fi.name for fi in fi.product.fixed_inputs} - set(tag_data):
             errors.append(fi.product.name)
         if set(tag_data_required) - {fi.name for fi in fi.product.fixed_inputs}:
             errors.append(fi.product.name)
 
     if errors:
-        raise ProcessFailure("Errors in fixed input config", errors)
+        raise ProcessFailureError("Errors in fixed input config", errors)
 
     return {"check_db_fixed_input_config": True}
 
 
 @step("Check subscription models")
 def check_subscription_models() -> State:
     subscriptions = SubscriptionTable.query.all()
@@ -181,15 +181,15 @@
             SubscriptionModel.from_subscription(subscription.subscription_id)
         except ValidationError as e:
             failures[str(subscription.subscription_id)] = e.errors()
         except Exception as e:
             failures[str(subscription.subscription_id)] = str(e)
 
     if failures:
-        raise ProcessFailure("Found subscriptions that could not be loaded", failures)
+        raise ProcessFailureError("Found subscriptions that could not be loaded", failures)
 
     return {"check_subscription_models": True}
 
 
 @workflow("Validate products", target=Target.SYSTEM)
 def task_validate_products() -> StepList:
     return (
```

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/workflows/translations/en-GB.json` & `orchestrator_core-1.2.0/orchestrator/workflows/translations/en-GB.json`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/orchestrator/workflows/utils.py` & `orchestrator_core-1.2.0/orchestrator/workflows/utils.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/pyproject.toml` & `orchestrator_core-1.2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -37,44 +37,37 @@
     "Topic :: Internet :: WWW/HTTP",
 ]
 dependencies = [
     "alembic==1.5.4",
     "anyio>=3.7.0",
     "broadcaster[redis]==0.2.0",
     "click==8.0.3",
+    "deprecated",
     "deepmerge==0.1.0",
-    "fastapi~=0.98.0",
+    "fastapi~=0.99.1",
     "fastapi-etag==0.4.0",
     "more-itertools~=9.0.0",
-    "itsdangerous==2.1.2",
+    "itsdangerous",
     "Jinja2==3.1.2",
-    "opentelemetry-distro",
-    "opentelemetry-exporter-otlp",
-    "opentelemetry-instrumentation-httpx",
-    "opentelemetry-instrumentation-fastapi",
-    "opentelemetry-instrumentation-psycopg2",
-    "opentelemetry-instrumentation-redis",
-    "opentelemetry-instrumentation-sqlalchemy",
     "orjson==3.9.1",
     "psycopg2-binary==2.9.5",
     "pydantic[email]==1.10.9",
     "python-dateutil==2.8.2",
     "python-rapidjson==1.9",
     "pytz==2023.3",
     "redis>=4.5.5,<4.6",
     "schedule==1.1.0",
     "sentry-sdk[fastapi]==1.25.1",
     "SQLAlchemy==1.4.48",
     "SQLAlchemy-Utils==0.40.0",
+    "structlog",
     "typer==0.7.0",
     "uvicorn[standard]~=0.20.0",
     "nwa-stdlib~=1.4.8",
-    "oauth2-lib~=1.2.10",
-    "markupsafe==2.0.1",
-    "bandit==1.7.2",
+    "oauth2-lib~=1.3.1",
     "tabulate==0.9.0",
     "strawberry-graphql==0.171.1"
 ]
 description-file = "README.md"
 requires-python = ">=3.9,<3.12"
 
 [project.urls]
@@ -86,28 +79,15 @@
 ]
 
 test = [
     "apache-license-check",
     "black",
     "blinker",
     "deepdiff",
-    "flake8 < 5.0.0", # Due to https://github.com/tylerwince/flake8-bandit/issues/33
-    "flake8-bandit",
-    "flake8-bugbear",
-    "flake8-comprehensions",
-    "flake8-docstrings",
-    "flake8-junit-report",
-    "flake8-logging-format",
-    "flake8-pep3101",
-    "flake8-print",
-    "flake8-rst",
-    "flake8-rst-docstrings",
-    "flake8-tidy-imports",
-    "isort",
-    "structlog",
+    "ruff",
     "jsonref",
     "mypy",
     "pytest",
     "pytest-cov",
     "pytest-httpx",
     "pytest-xdist",
     "requests-mock",
@@ -171,7 +151,73 @@
     | src
   )/
 )
 '''
 
 [tool.nitpick]
 style="github://workfloworchestrator/nitpick-style@main/nitpick-style-orchestrator-core.toml"
+
+
+[tool.ruff]
+exclude = [
+    ".git",
+    ".cache",
+    ".eggs",
+    "__pycache__",
+    "dist",
+    "src",
+    "crypt.py",
+    "venv",
+    ".venv",
+    "docs",
+]
+ignore = [
+    "C417",
+    "D100",
+    "D101",
+    "D102",
+    "D103",
+    "D104",
+    "D105",
+    "D106",
+    "D107",
+    "D202",
+    "E501",
+    "N806",
+    "B905",
+    "N805",
+    "B904",
+    "N803",
+    "N801",
+    "N815",
+    "N802"
+]
+line-length = 120
+select = [
+    "B",
+    "C",
+    "D",
+    "E",
+    "F",
+    "I",
+    "N",
+    "RET",
+    "S",
+    "T",
+    "W",
+]
+target-version = "py310"
+
+[tool.ruff.flake8-tidy-imports]
+ban-relative-imports = "all"
+
+[tool.ruff.per-file-ignores]
+"orchestrator/api/*" = ["B008"]
+"orchestrator/cli/*" = ["B008"]
+"test/*" = ["S101", "B033", "N816", "N802"]
+
+[tool.ruff.pydocstyle]
+convention = "google"
+
+[tool.ruff.isort]
+known-third-party = ["pynso", "pydantic"]
+known-first-party = ["migrations", "test", "nwastdlib", "oauth2-lib"]
```

### Comparing `orchestrator_core-1.1.1rc4/setup.cfg` & `orchestrator_core-1.2.0/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,10 @@
 [aliases]
 test=pytest
 
-[flake8]
-ignore = D100,D101,D102,D103,D104,D105,D106,D107,D202,E501,RST301,RST304,W503,E203,C417,T202
-exclude = .git,.cache,.eggs,__pycache__,dist,src,crypt.py,venv,.venv,docs
-enable-extensions = G
-select = B,C,D,E,F,G,I,N,S,T,W,B902,B903,R
-max-line-length = 120
-ban-relative-imports = true
-per-file-ignores =
-	# Allow first argument to be cls instead of self for pydantic validators
-	orchestrator/*: B902
-	orchestrator/api/*: B008
-	orchestrator/cli/*: B008
-	test/*: S101
-
 [tool:pytest]
 addopts=--doctest-modules --doctest-ignore-import-errors
 norecursedirs=.git build dist *.egg __pycache__ .cache .* migrations docs
 testpaths=test/unit_tests orchestrator
 junit_suite_name = orchestrator
 filterwarnings=
 	ignore::pytest.PytestCollectionWarning
```

### Comparing `orchestrator_core-1.1.1rc4/setup.py` & `orchestrator_core-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/acceptance_tests/conftest.py` & `orchestrator_core-1.2.0/test/acceptance_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py` & `orchestrator_core-1.2.0/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/acceptance_tests/fixtures/test_orchestrator/main.py` & `orchestrator_core-1.2.0/test/acceptance_tests/fixtures/test_orchestrator/main.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py` & `orchestrator_core-1.2.0/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py` & `orchestrator_core-1.2.0/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,23 +8,22 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
+from orchestrator.domain.base import SubscriptionModel
+from orchestrator.types import SubscriptionLifecycle
 from test_orchestrator.product_blocks.test_product_blocks import (
     TestProductBlock,
     TestProductBlockInactive,
     TestProductBlockProvisioning,
 )
 
-from orchestrator.domain.base import SubscriptionModel
-from orchestrator.types import SubscriptionLifecycle
-
 
 class TestProductInactive(SubscriptionModel, is_base=True):
     testproduct: TestProductBlockInactive
 
 
 class TestProductProvisioning(TestProductInactive, lifecycle=[SubscriptionLifecycle.PROVISIONING]):
     testproduct: TestProductBlockProvisioning
```

### Comparing `orchestrator_core-1.1.1rc4/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py` & `orchestrator_core-1.2.0/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -12,23 +12,23 @@
 # limitations under the License.
 
 
 from ipaddress import IPv4Address, IPv6Address
 from uuid import UUID
 
 from structlog import get_logger
-from test_orchestrator.products.test_product import TestProductInactive
 
 from orchestrator.forms import FormPage
 from orchestrator.forms.validators import OrganisationId
 from orchestrator.targets import Target
 from orchestrator.types import FormGenerator, State, SubscriptionLifecycle, UUIDstr
 from orchestrator.workflow import StepList, begin, done, step, workflow
 from orchestrator.workflows.steps import store_process_subscription
 from orchestrator.workflows.utils import wrap_create_initial_input_form
+from test_orchestrator.products.test_product import TestProductInactive
 
 logger = get_logger(__name__)
 
 
 def initial_input_form_generator(product_name: str, product: UUIDstr) -> FormGenerator:
     class CreateTestProductForm(FormPage):
         class Config:
```

### Comparing `orchestrator_core-1.1.1rc4/test/acceptance_tests/test_test_product.py` & `orchestrator_core-1.2.0/test/acceptance_tests/test_test_product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/api/test_caching.py` & `orchestrator_core-1.2.0/test/unit_tests/api/test_caching.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """(regression)tests in relation to domain model caching."""
 from http import HTTPStatus
 from os import getenv
 
 import pytest
-from nwastdlib.url import URL
 
+from nwastdlib.url import URL
 from orchestrator.domain.base import SubscriptionModel
 from orchestrator.services.subscriptions import build_extended_domain_model
 from orchestrator.utils.redis import to_redis
 
 
 @pytest.mark.skipif(
     not getenv("AIOCACHE_DISABLE", "0") == "0", reason="AIOCACHE must be enabled for this test to do anything"
```

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/api/test_fixed_inputs.py` & `orchestrator_core-1.2.0/test/unit_tests/api/test_fixed_inputs.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/api/test_health.py` & `orchestrator_core-1.2.0/test/unit_tests/api/test_health.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/api/test_helpers.py` & `orchestrator_core-1.2.0/test/unit_tests/api/test_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/api/test_models.py` & `orchestrator_core-1.2.0/test/unit_tests/api/test_models.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/api/test_processes.py` & `orchestrator_core-1.2.0/test/unit_tests/api/test_processes.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/api/test_processes_ws.py` & `orchestrator_core-1.2.0/test/unit_tests/api/test_processes_ws.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/api/test_product_blocks.py` & `orchestrator_core-1.2.0/test/unit_tests/api/test_product_blocks.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/api/test_products.py` & `orchestrator_core-1.2.0/test/unit_tests/api/test_products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/api/test_resource_types.py` & `orchestrator_core-1.2.0/test/unit_tests/api/test_resource_types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/api/test_settings.py` & `orchestrator_core-1.2.0/test/unit_tests/api/test_settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/api/test_subscription_customer_descriptions.py` & `orchestrator_core-1.2.0/test/unit_tests/api/test_subscription_customer_descriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/api/test_subscriptions.py` & `orchestrator_core-1.2.0/test/unit_tests/api/test_subscriptions.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from http import HTTPStatus
 from os import getenv
 from uuid import uuid4
 
 import pytest
-from nwastdlib.url import URL
 from redis import Redis
 
+from nwastdlib.url import URL
 from orchestrator.api.helpers import product_block_paths
 from orchestrator.db import (
     FixedInputTable,
     ProcessSubscriptionTable,
     ProcessTable,
     ProductBlockTable,
     ProductTable,
```

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/api/test_workflows.py` & `orchestrator_core-1.2.0/test/unit_tests/api/test_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/cli/test_migrate_domain_models_with_instances.py` & `orchestrator_core-1.2.0/test/unit_tests/cli/test_migrate_domain_models_with_instances.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/cli/test_migrate_domain_models_without_instances.py` & `orchestrator_core-1.2.0/test/unit_tests/cli/test_migrate_domain_models_without_instances.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/conftest.py` & `orchestrator_core-1.2.0/test/unit_tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,16 +122,15 @@
 
 logger = structlog.getLogger(__name__)
 
 CUSTOMER_ID: UUIDstr = "2f47f65a-0911-e511-80d0-005056956c1a"
 
 
 def run_migrations(db_uri: str) -> None:
-    """
-    Configure the alembic context and run the migrations.
+    """Configure the alembic context and run the migrations.
 
     Each test will start with a clean database. This a heavy operation but ensures that our database is clean and
     tests run within their own context.
 
     Args:
         db_uri: The database uri configuration to run the migration on.
 
@@ -150,16 +149,15 @@
     )
     alembic_cfg.set_main_option("sqlalchemy.url", db_uri)
     command.upgrade(alembic_cfg, "heads")
 
 
 @pytest.fixture(scope="session")
 def db_uri(worker_id):
-    """
-    Ensure each pytest thread has its database.
+    """Ensure each pytest thread has its database.
 
     When running tests with the -j option make sure each test worker is isolated within its own database.
 
     Args:
         worker_id: the worker id
 
     Returns:
@@ -212,16 +210,15 @@
         with closing(engine.connect()) as conn:
             conn.execute("COMMIT;")
             conn.execute(f'DROP DATABASE IF EXISTS "{db_to_create}";')
 
 
 @pytest.fixture(autouse=True)
 def db_session(database):
-    """
-    Ensure tests are run in a transaction with automatic rollback.
+    """Ensure tests are run in a transaction with automatic rollback.
 
     This implementation creates a connection and transaction before yielding to the test function. Any transactions
     started and committed from within the test will be tied to this outer transaction. From the test function's
     perspective it looks like everything will indeed be committed; allowing for queries on the database to be
     performed to see if functions under test have persisted their changes to the database correctly. However once
     the test function returns this fixture will clean everything up by rolling back the outer transaction; leaving the
     database in a known state (=empty with the exception of what migrations have added as the initial state).
```

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/domain/test_base.py` & `orchestrator_core-1.2.0/test/unit_tests/domain/test_base.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/domain/test_base_with_list_union.py` & `orchestrator_core-1.2.0/test/unit_tests/domain/test_base_with_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/domain/test_base_with_union.py` & `orchestrator_core-1.2.0/test/unit_tests/domain/test_base_with_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/fixtures/__init__.py` & `orchestrator_core-1.2.0/test/unit_tests/fixtures/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,24 +17,23 @@
     charset = string.ascii_lowercase + string.digits
     return "".join(random.choice(charset) for _ in range(0, length))  # noqa: S311
 
 
 def create_subscription_for_mapping(
     product: ProductTable, mapping: SubscriptionMapping, values: Dict[str, Any], **kwargs: Any
 ) -> SubscriptionTable:
-    """
-    Create a subscription in the test coredb for the given subscription_mapping and values.
+    """Create a subscription in the test coredb for the given subscription_mapping and values.
 
     This function handles optional resource types starting with a ? in the mapping not supplied in the values array.
 
     Args:
         product: the ProductTable to create a sub for
         mapping: the subscription_mapping belonging to that product
         values: a dictionary of keys from the sub_map and their corresponding test values
-        kwargs:
+        kwargs: The rest of the arguments
 
     Returns: The conforming subscription.
     """
 
     def build_instance(name, value_mapping):
         block = product.find_block_by_name(name)
```

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/fixtures/processes.py` & `orchestrator_core-1.2.0/test/unit_tests/fixtures/processes.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py` & `orchestrator_core-1.2.0/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/fixtures/products/product_blocks/product_block_one.py` & `orchestrator_core-1.2.0/test/unit_tests/fixtures/products/product_blocks/product_block_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py` & `orchestrator_core-1.2.0/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py` & `orchestrator_core-1.2.0/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py` & `orchestrator_core-1.2.0/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py` & `orchestrator_core-1.2.0/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py` & `orchestrator_core-1.2.0/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py` & `orchestrator_core-1.2.0/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/fixtures/products/product_types/product_type_list_union.py` & `orchestrator_core-1.2.0/test/unit_tests/fixtures/products/product_types/product_type_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py` & `orchestrator_core-1.2.0/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/fixtures/products/product_types/product_type_one.py` & `orchestrator_core-1.2.0/test/unit_tests/fixtures/products/product_types/product_type_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py` & `orchestrator_core-1.2.0/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py` & `orchestrator_core-1.2.0/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py` & `orchestrator_core-1.2.0/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py` & `orchestrator_core-1.2.0/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py` & `orchestrator_core-1.2.0/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/fixtures/products/product_types/product_type_union.py` & `orchestrator_core-1.2.0/test/unit_tests/fixtures/products/product_types/product_type_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/fixtures/products/resource_types.py` & `orchestrator_core-1.2.0/test/unit_tests/fixtures/products/resource_types.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/forms/shared.py` & `orchestrator_core-1.2.0/test/unit_tests/forms/shared.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/forms/test_generic_validators.py` & `orchestrator_core-1.2.0/test/unit_tests/forms/test_generic_validators.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/forms/test_network_validators.py` & `orchestrator_core-1.2.0/test/unit_tests/forms/test_network_validators.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/forms/test_post_process.py` & `orchestrator_core-1.2.0/test/unit_tests/forms/test_post_process.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/graphql/test_processes.py` & `orchestrator_core-1.2.0/test/unit_tests/graphql/test_processes.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/graphql/test_product.py` & `orchestrator_core-1.2.0/test/unit_tests/graphql/test_product.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/graphql/test_settings.py` & `orchestrator_core-1.2.0/test/unit_tests/graphql/test_settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/graphql/test_subscriptions.py` & `orchestrator_core-1.2.0/test/unit_tests/graphql/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/schedules/test_scheduling.py` & `orchestrator_core-1.2.0/test/unit_tests/schedules/test_scheduling.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/services/test_processes.py` & `orchestrator_core-1.2.0/test/unit_tests/services/test_processes.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/services/test_products.py` & `orchestrator_core-1.2.0/test/unit_tests/services/test_products.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/services/test_subscriptions.py` & `orchestrator_core-1.2.0/test/unit_tests/services/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/services/test_translations.py` & `orchestrator_core-1.2.0/test/unit_tests/services/test_translations.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/test_db.py` & `orchestrator_core-1.2.0/test/unit_tests/test_db.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/test_workflow.py` & `orchestrator_core-1.2.0/test/unit_tests/test_workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,44 @@
 from copy import deepcopy
 from functools import reduce
 from typing import List, NoReturn, Tuple
 from unittest import mock
 from uuid import UUID, uuid4
 
 import pytest
-from nwastdlib import const
 
+from nwastdlib import const
 from orchestrator.config.assignee import Assignee
 from orchestrator.forms import FormPage
 from orchestrator.services.processes import SYSTEM_USER
 from orchestrator.types import FormGenerator, State, UUIDstr
 from orchestrator.utils.errors import error_state_to_dict
-from orchestrator.workflow import Abort, Failed, Process, ProcessStat, Skipped, Success, Suspend, Waiting
-from orchestrator.workflow import _purestep as purestep
 from orchestrator.workflow import (
+    Abort,
+    Failed,
+    Process,
+    ProcessStat,
+    Skipped,
+    Success,
+    Suspend,
+    Waiting,
     abort,
     abort_wf,
     begin,
     conditional,
     done,
     focussteps,
     init,
     inputstep,
     retrystep,
     runwf,
     step,
     workflow,
 )
+from orchestrator.workflow import _purestep as purestep
 from test.unit_tests.workflows import (
     WorkflowInstanceForTests,
     assert_aborted,
     assert_complete,
     assert_failed,
     assert_state,
     assert_success,
@@ -166,16 +173,15 @@
 def test_resume_waiting_workflow():
     hack = {"error": True}
 
     @retrystep("Waiting step")
     def soft_fail():
         if hack["error"]:
             raise ValueError("error")
-        else:
-            return {"some_key": True}
+        return {"some_key": True}
 
     wf = workflow("Workflow with soft fail")(lambda: begin >> step1 >> soft_fail >> step2)
 
     log = []
 
     state = Waiting({"steps": [1]})
```

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/utils/test_errors.py` & `orchestrator_core-1.2.0/test/unit_tests/utils/test_errors.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from http import HTTPStatus
 
-from orchestrator.utils.errors import ApiException, ProcessFailure, error_state_to_dict
+from orchestrator.utils.errors import ApiException, ProcessFailureError, error_state_to_dict
 
 
 class RESTResponse:  # From openapi-generator generated clients
     def __init__(self, status, reason, data, headers):
         self.status = status
         self.reason = reason
         self.data = data
@@ -41,14 +41,14 @@
         "class": "ApiException",
         "error": "Not Found",
         "headers": "Header: value\nContent-type: bogus",
         "status_code": HTTPStatus.NOT_FOUND,
         "traceback": "ApiException: (404)\nReason: Not Found\nHTTP response headers: {'Header': 'value', 'Content-type': 'bogus'}\nHTTP response body: Body\n\n",
     }
 
-    e = ProcessFailure(message="Something went wrong", details={"foo": "bar"})
+    e = ProcessFailureError(message="Something went wrong", details={"foo": "bar"})
     assert error_state_to_dict(e) == {
-        "class": "ProcessFailure",
+        "class": "ProcessFailureError",
         "details": {"foo": "bar"},
         "error": "Something went wrong",
-        "traceback": "ProcessFailure: ('Something went wrong', {'foo': 'bar'})\n",
+        "traceback": "ProcessFailureError: ('Something went wrong', {'foo': 'bar'})\n",
     }
```

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/utils/test_functional.py` & `orchestrator_core-1.2.0/test/unit_tests/utils/test_functional.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/utils/test_json.py` & `orchestrator_core-1.2.0/test/unit_tests/utils/test_json.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/utils/test_speed.py` & `orchestrator_core-1.2.0/test/unit_tests/utils/test_speed.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/utils/test_state.py` & `orchestrator_core-1.2.0/test/unit_tests/utils/test_state.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # type: ignore
 
 from typing import List, Optional
 from uuid import uuid4
 
 import pytest
-from nwastdlib import const
 
+from nwastdlib import const
 from orchestrator.domain.base import SubscriptionModel
 from orchestrator.forms import FormPage, post_process
 from orchestrator.types import State, SubscriptionLifecycle
 from orchestrator.utils.state import extract, form_inject_args, inject_args
 
 STATE = {"one": 1, "two": 2, "three": 3, "four": 4}
```

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/utils/test_vlans.py` & `orchestrator_core-1.2.0/test/unit_tests/utils/test_vlans.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/workflows/__init__.py` & `orchestrator_core-1.2.0/test/unit_tests/workflows/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -275,14 +275,15 @@
     been ran.
 
     Args:
         form_generator: A form generator
         extra_inputs: Optional list of user input dicts for each page in the generator.
                       If no input is given for a page an empty dict is used.
                       The default value from the form is used as default value for a field.
+
     Returns:
         A list of generated forms and the result state for the whole generator.
 
     Example:
         Given the following form generator:
 
         >>> from orchestrator.forms import FormPage
```

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/workflows/shared/test_validate_subscriptions.py` & `orchestrator_core-1.2.0/test/unit_tests/workflows/shared/test_validate_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/workflows/tasks/test_clean_up_task_log.py` & `orchestrator_core-1.2.0/test/unit_tests/workflows/tasks/test_clean_up_task_log.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/workflows/tasks/test_resume_workflows.py` & `orchestrator_core-1.2.0/test/unit_tests/workflows/tasks/test_resume_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/workflows/test_config_db_code.py` & `orchestrator_core-1.2.0/test/unit_tests/workflows/test_config_db_code.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/workflows/test_generic_workflow_steps.py` & `orchestrator_core-1.2.0/test/unit_tests/workflows/test_generic_workflow_steps.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/test/unit_tests/workflows/test_modify_note.py` & `orchestrator_core-1.2.0/test/unit_tests/workflows/test_modify_note.py`

 * *Files identical despite different names*

### Comparing `orchestrator_core-1.1.1rc4/PKG-INFO` & `orchestrator_core-1.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orchestrator-core
-Version: 1.1.1rc4
+Version: 1.2.0
 Summary: Open source orchestration software for NREN's
 Requires-Python: >=3.9,<3.12
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python
@@ -27,44 +27,37 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Dist: alembic==1.5.4
 Requires-Dist: anyio>=3.7.0
 Requires-Dist: broadcaster[redis]==0.2.0
 Requires-Dist: click==8.0.3
+Requires-Dist: deprecated
 Requires-Dist: deepmerge==0.1.0
-Requires-Dist: fastapi~=0.98.0
+Requires-Dist: fastapi~=0.99.1
 Requires-Dist: fastapi-etag==0.4.0
 Requires-Dist: more-itertools~=9.0.0
-Requires-Dist: itsdangerous==2.1.2
+Requires-Dist: itsdangerous
 Requires-Dist: Jinja2==3.1.2
-Requires-Dist: opentelemetry-distro
-Requires-Dist: opentelemetry-exporter-otlp
-Requires-Dist: opentelemetry-instrumentation-httpx
-Requires-Dist: opentelemetry-instrumentation-fastapi
-Requires-Dist: opentelemetry-instrumentation-psycopg2
-Requires-Dist: opentelemetry-instrumentation-redis
-Requires-Dist: opentelemetry-instrumentation-sqlalchemy
 Requires-Dist: orjson==3.9.1
 Requires-Dist: psycopg2-binary==2.9.5
 Requires-Dist: pydantic[email]==1.10.9
 Requires-Dist: python-dateutil==2.8.2
 Requires-Dist: python-rapidjson==1.9
 Requires-Dist: pytz==2023.3
 Requires-Dist: redis>=4.5.5,<4.6
 Requires-Dist: schedule==1.1.0
 Requires-Dist: sentry-sdk[fastapi]==1.25.1
 Requires-Dist: SQLAlchemy==1.4.48
 Requires-Dist: SQLAlchemy-Utils==0.40.0
+Requires-Dist: structlog
 Requires-Dist: typer==0.7.0
 Requires-Dist: uvicorn[standard]~=0.20.0
 Requires-Dist: nwa-stdlib~=1.4.8
-Requires-Dist: oauth2-lib~=1.2.10
-Requires-Dist: markupsafe==2.0.1
-Requires-Dist: bandit==1.7.2
+Requires-Dist: oauth2-lib~=1.3.1
 Requires-Dist: tabulate==0.9.0
 Requires-Dist: strawberry-graphql==0.171.1
 Requires-Dist: celery~=5.2.7 ; extra == "celery"
 Requires-Dist: toml ; extra == "dev"
 Requires-Dist: bumpversion ; extra == "dev"
 Requires-Dist: mypy_extensions ; extra == "dev"
 Requires-Dist: pre-commit ; extra == "dev"
@@ -75,28 +68,15 @@
 Requires-Dist: mkdocs-material ; extra == "doc"
 Requires-Dist: mkdocs-render-swagger-plugin ; extra == "doc"
 Requires-Dist: mkdocs-include-markdown-plugin ; extra == "doc"
 Requires-Dist: apache-license-check ; extra == "test"
 Requires-Dist: black ; extra == "test"
 Requires-Dist: blinker ; extra == "test"
 Requires-Dist: deepdiff ; extra == "test"
-Requires-Dist: flake8 < 5.0.0 ; extra == "test"
-Requires-Dist: flake8-bandit ; extra == "test"
-Requires-Dist: flake8-bugbear ; extra == "test"
-Requires-Dist: flake8-comprehensions ; extra == "test"
-Requires-Dist: flake8-docstrings ; extra == "test"
-Requires-Dist: flake8-junit-report ; extra == "test"
-Requires-Dist: flake8-logging-format ; extra == "test"
-Requires-Dist: flake8-pep3101 ; extra == "test"
-Requires-Dist: flake8-print ; extra == "test"
-Requires-Dist: flake8-rst ; extra == "test"
-Requires-Dist: flake8-rst-docstrings ; extra == "test"
-Requires-Dist: flake8-tidy-imports ; extra == "test"
-Requires-Dist: isort ; extra == "test"
-Requires-Dist: structlog ; extra == "test"
+Requires-Dist: ruff ; extra == "test"
 Requires-Dist: jsonref ; extra == "test"
 Requires-Dist: mypy ; extra == "test"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: pytest-httpx ; extra == "test"
 Requires-Dist: pytest-xdist ; extra == "test"
 Requires-Dist: requests-mock ; extra == "test"
```

