# Comparing `tmp/yapairwise_testing-0.1.tar.gz` & `tmp/yapairwise_testing-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yapairwise_testing-0.1.tar", last modified: Mon Jul  3 19:35:42 2023, max compression
+gzip compressed data, was "yapairwise_testing-0.2.tar", last modified: Mon Jul  3 20:04:45 2023, max compression
```

## Comparing `yapairwise_testing-0.1.tar` & `yapairwise_testing-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 clayton   (1000) clayton   (1000)        0 2023-07-03 19:35:42.098853 yapairwise_testing-0.1/
--rw-rw-r--   0 clayton   (1000) clayton   (1000)     1124 2023-07-03 18:53:42.000000 yapairwise_testing-0.1/LICENSE.txt
--rw-rw-r--   0 clayton   (1000) clayton   (1000)     8788 2023-07-03 19:35:42.098853 yapairwise_testing-0.1/PKG-INFO
--rw-rw-r--   0 clayton   (1000) clayton   (1000)     8322 2023-07-03 19:17:28.000000 yapairwise_testing-0.1/README.md
--rw-rw-r--   0 clayton   (1000) clayton   (1000)       38 2023-07-03 19:35:42.098853 yapairwise_testing-0.1/setup.cfg
--rw-rw-r--   0 clayton   (1000) clayton   (1000)      631 2023-07-03 19:35:35.000000 yapairwise_testing-0.1/setup.py
-drwxrwxr-x   0 clayton   (1000) clayton   (1000)        0 2023-07-03 19:35:42.098853 yapairwise_testing-0.1/yapairwise_testing/
--rw-rw-r--   0 clayton   (1000) clayton   (1000)       62 2023-07-03 18:57:31.000000 yapairwise_testing-0.1/yapairwise_testing/__init__.py
--rw-rw-r--   0 clayton   (1000) clayton   (1000)      900 2023-07-03 19:01:17.000000 yapairwise_testing-0.1/yapairwise_testing/pairwise_testing.py
-drwxrwxr-x   0 clayton   (1000) clayton   (1000)        0 2023-07-03 19:35:42.098853 yapairwise_testing-0.1/yapairwise_testing.egg-info/
--rw-rw-r--   0 clayton   (1000) clayton   (1000)     8788 2023-07-03 19:35:42.000000 yapairwise_testing-0.1/yapairwise_testing.egg-info/PKG-INFO
--rw-rw-r--   0 clayton   (1000) clayton   (1000)      268 2023-07-03 19:35:42.000000 yapairwise_testing-0.1/yapairwise_testing.egg-info/SOURCES.txt
--rw-rw-r--   0 clayton   (1000) clayton   (1000)        1 2023-07-03 19:35:42.000000 yapairwise_testing-0.1/yapairwise_testing.egg-info/dependency_links.txt
--rw-rw-r--   0 clayton   (1000) clayton   (1000)       19 2023-07-03 19:35:42.000000 yapairwise_testing-0.1/yapairwise_testing.egg-info/top_level.txt
+drwxrwxr-x   0 clayton   (1000) clayton   (1000)        0 2023-07-03 20:04:45.063300 yapairwise_testing-0.2/
+-rw-rw-r--   0 clayton   (1000) clayton   (1000)     1124 2023-07-03 18:53:42.000000 yapairwise_testing-0.2/LICENSE.txt
+-rw-rw-r--   0 clayton   (1000) clayton   (1000)     9489 2023-07-03 20:04:45.063300 yapairwise_testing-0.2/PKG-INFO
+-rw-rw-r--   0 clayton   (1000) clayton   (1000)     9023 2023-07-03 20:03:00.000000 yapairwise_testing-0.2/README.md
+-rw-rw-r--   0 clayton   (1000) clayton   (1000)       38 2023-07-03 20:04:45.063300 yapairwise_testing-0.2/setup.cfg
+-rw-rw-r--   0 clayton   (1000) clayton   (1000)      631 2023-07-03 20:04:39.000000 yapairwise_testing-0.2/setup.py
+drwxrwxr-x   0 clayton   (1000) clayton   (1000)        0 2023-07-03 20:04:45.059300 yapairwise_testing-0.2/yapairwise_testing/
+-rw-rw-r--   0 clayton   (1000) clayton   (1000)       62 2023-07-03 18:57:31.000000 yapairwise_testing-0.2/yapairwise_testing/__init__.py
+-rw-rw-r--   0 clayton   (1000) clayton   (1000)      900 2023-07-03 19:01:17.000000 yapairwise_testing-0.2/yapairwise_testing/pairwise_testing.py
+drwxrwxr-x   0 clayton   (1000) clayton   (1000)        0 2023-07-03 20:04:45.059300 yapairwise_testing-0.2/yapairwise_testing.egg-info/
+-rw-rw-r--   0 clayton   (1000) clayton   (1000)     9489 2023-07-03 20:04:45.000000 yapairwise_testing-0.2/yapairwise_testing.egg-info/PKG-INFO
+-rw-rw-r--   0 clayton   (1000) clayton   (1000)      268 2023-07-03 20:04:45.000000 yapairwise_testing-0.2/yapairwise_testing.egg-info/SOURCES.txt
+-rw-rw-r--   0 clayton   (1000) clayton   (1000)        1 2023-07-03 20:04:45.000000 yapairwise_testing-0.2/yapairwise_testing.egg-info/dependency_links.txt
+-rw-rw-r--   0 clayton   (1000) clayton   (1000)       19 2023-07-03 20:04:45.000000 yapairwise_testing-0.2/yapairwise_testing.egg-info/top_level.txt
```

### Comparing `yapairwise_testing-0.1/LICENSE.txt` & `yapairwise_testing-0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `yapairwise_testing-0.1/PKG-INFO` & `yapairwise_testing-0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Metadata-Version: 2.1
 Name: yapairwise_testing
-Version: 0.1
+Version: 0.2
 Summary: A library for pairwise testing package
 Home-page: https://github.com/claytonfraga/yapairwise_testing
 Author: Clayton Vieira Fraga Filho
 Author-email: claytonfraga@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
+## Visão geral
+
+A Análise de Par de Combinações, também conhecida como Pairwise Testing, é uma técnica de teste de software que busca reduzir a quantidade de cenários de testes por meio da exploração da interação efetiva entre pares de variáveis de entrada. Esta abordagem baseia-se no princípio empírico de que a maioria dos defeitos do software é causada pela interação de apenas dois fatores. Portanto, ao invés de testar todas as combinações possíveis de entradas (que pode ser impraticável para sistemas complexos), a técnica Pairwise Testing testa todas as possíveis combinações de pares de entradas, reduzindo significativamente a quantidade de testes necessários.
+
 ## Uso
 
 Para usar a função `pairwise_testing`, importe-a da seguinte maneira:
 
 from pairwise_testing import pairwise_testing
 
 A função pairwise_testing recebe três argumentos:
```

### Comparing `yapairwise_testing-0.1/README.md` & `yapairwise_testing-0.2/yapairwise_testing.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: yapairwise-testing
+Version: 0.2
+Summary: A library for pairwise testing package
+Home-page: https://github.com/claytonfraga/yapairwise_testing
+Author: Clayton Vieira Fraga Filho
+Author-email: claytonfraga@gmail.com
+License: MIT
+Platform: UNKNOWN
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+## Visão geral
+
+A Análise de Par de Combinações, também conhecida como Pairwise Testing, é uma técnica de teste de software que busca reduzir a quantidade de cenários de testes por meio da exploração da interação efetiva entre pares de variáveis de entrada. Esta abordagem baseia-se no princípio empírico de que a maioria dos defeitos do software é causada pela interação de apenas dois fatores. Portanto, ao invés de testar todas as combinações possíveis de entradas (que pode ser impraticável para sistemas complexos), a técnica Pairwise Testing testa todas as possíveis combinações de pares de entradas, reduzindo significativamente a quantidade de testes necessários.
+
 ## Uso
 
 Para usar a função `pairwise_testing`, importe-a da seguinte maneira:
 
 from pairwise_testing import pairwise_testing
 
 A função pairwise_testing recebe três argumentos:
@@ -198,7 +217,9 @@
     "Desconto Categoria": discount_customer_category,
     "Desconto Idade": discount_customer_age,
     "Desconto Total": total_discount
 }
 
 # Chamando a função
 pairwise_testing(variables, results_rules, 'test_cases.csv')
+
+
```

### Comparing `yapairwise_testing-0.1/setup.py` & `yapairwise_testing-0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='yapairwise_testing',
-    version='0.1',
+    version='0.2',
     packages=find_packages(),
     description='A library for pairwise testing package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',  # Linha nova    
     url='https://github.com/claytonfraga/yapairwise_testing',
     author='Clayton Vieira Fraga Filho',
     author_email='claytonfraga@gmail.com',
```

### Comparing `yapairwise_testing-0.1/yapairwise_testing/pairwise_testing.py` & `yapairwise_testing-0.2/yapairwise_testing/pairwise_testing.py`

 * *Files identical despite different names*

### Comparing `yapairwise_testing-0.1/yapairwise_testing.egg-info/PKG-INFO` & `yapairwise_testing-0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,10 @@
-Metadata-Version: 2.1
-Name: yapairwise-testing
-Version: 0.1
-Summary: A library for pairwise testing package
-Home-page: https://github.com/claytonfraga/yapairwise_testing
-Author: Clayton Vieira Fraga Filho
-Author-email: claytonfraga@gmail.com
-License: MIT
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
+## Visão geral
+
+A Análise de Par de Combinações, também conhecida como Pairwise Testing, é uma técnica de teste de software que busca reduzir a quantidade de cenários de testes por meio da exploração da interação efetiva entre pares de variáveis de entrada. Esta abordagem baseia-se no princípio empírico de que a maioria dos defeitos do software é causada pela interação de apenas dois fatores. Portanto, ao invés de testar todas as combinações possíveis de entradas (que pode ser impraticável para sistemas complexos), a técnica Pairwise Testing testa todas as possíveis combinações de pares de entradas, reduzindo significativamente a quantidade de testes necessários.
 
 ## Uso
 
 Para usar a função `pairwise_testing`, importe-a da seguinte maneira:
 
 from pairwise_testing import pairwise_testing
 
@@ -213,9 +202,7 @@
     "Desconto Categoria": discount_customer_category,
     "Desconto Idade": discount_customer_age,
     "Desconto Total": total_discount
 }
 
 # Chamando a função
 pairwise_testing(variables, results_rules, 'test_cases.csv')
-
-
```

