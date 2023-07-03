# Comparing `tmp/genetic-algo-0.0.4.tar.gz` & `tmp/genetic-algo-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genetic-algo-0.0.4.tar", last modified: Sat Jul  1 09:06:03 2023, max compression
+gzip compressed data, was "genetic-algo-0.0.5.tar", last modified: Mon Jul  3 14:17:48 2023, max compression
```

## Comparing `genetic-algo-0.0.4.tar` & `genetic-algo-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 09:06:03.698225 genetic-algo-0.0.4/
--rw-rw-rw-   0        0        0      115 2023-07-01 09:06:03.000000 genetic-algo-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     2040 2023-07-01 09:06:03.698225 genetic-algo-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1229 2023-07-01 09:05:38.000000 genetic-algo-0.0.4/README.md
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 genetic-algo-0.0.4/build.py
-drwxrwxrwx   0        0        0        0 2023-07-01 09:06:03.688228 genetic-algo-0.0.4/genetic_algo/
--rw-rw-rw-   0        0        0     8934 2023-06-20 16:13:53.000000 genetic-algo-0.0.4/genetic_algo/attributes.py
--rw-rw-rw-   0        0        0     5955 2023-06-03 06:57:31.000000 genetic-algo-0.0.4/genetic_algo/driver.py
--rw-rw-rw-   0        0        0    15381 2023-06-18 09:15:27.000000 genetic-algo-0.0.4/genetic_algo/environment.py
--rw-rw-rw-   0        0        0     4841 2023-06-20 18:47:51.000000 genetic-algo-0.0.4/genetic_algo/solution.py
-drwxrwxrwx   0        0        0        0 2023-07-01 09:06:03.697224 genetic-algo-0.0.4/genetic_algo.egg-info/
--rw-rw-rw-   0        0        0     2040 2023-07-01 09:06:03.000000 genetic-algo-0.0.4/genetic_algo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      382 2023-07-01 09:06:03.000000 genetic-algo-0.0.4/genetic_algo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 09:06:03.000000 genetic-algo-0.0.4/genetic_algo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-07-01 09:06:03.000000 genetic-algo-0.0.4/genetic_algo.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-01 09:06:03.000000 genetic-algo-0.0.4/genetic_algo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      645 2023-07-01 09:06:03.000000 genetic-algo-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       38 2023-06-18 08:47:03.000000 genetic-algo-0.0.4/requirements-dev.txt
--rw-rw-rw-   0        0        0       29 2023-06-18 08:47:03.000000 genetic-algo-0.0.4/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-01 09:06:03.699241 genetic-algo-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1601 2023-07-01 09:05:58.000000 genetic-algo-0.0.4/setup.py
--rw-rw-rw-   0        0        0     2645 2023-06-03 07:02:29.000000 genetic-algo-0.0.4/test.py
+drwxrwxrwx   0        0        0        0 2023-07-03 14:17:48.094955 genetic-algo-0.0.5/
+-rw-rw-rw-   0        0        0      115 2023-07-03 14:17:47.000000 genetic-algo-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     2040 2023-07-03 14:17:48.093960 genetic-algo-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1229 2023-07-01 09:05:38.000000 genetic-algo-0.0.5/README.md
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 genetic-algo-0.0.5/build.py
+drwxrwxrwx   0        0        0        0 2023-07-03 14:17:48.078955 genetic-algo-0.0.5/genetic_algo/
+-rw-rw-rw-   0        0        0     8921 2023-07-03 14:16:05.000000 genetic-algo-0.0.5/genetic_algo/attributes.py
+-rw-rw-rw-   0        0        0     5957 2023-07-03 14:16:25.000000 genetic-algo-0.0.5/genetic_algo/driver.py
+-rw-rw-rw-   0        0        0    15386 2023-07-03 14:16:58.000000 genetic-algo-0.0.5/genetic_algo/environment.py
+-rw-rw-rw-   0        0        0     4843 2023-07-03 14:17:21.000000 genetic-algo-0.0.5/genetic_algo/solution.py
+drwxrwxrwx   0        0        0        0 2023-07-03 14:17:48.092983 genetic-algo-0.0.5/genetic_algo.egg-info/
+-rw-rw-rw-   0        0        0     2040 2023-07-03 14:17:48.000000 genetic-algo-0.0.5/genetic_algo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      382 2023-07-03 14:17:48.000000 genetic-algo-0.0.5/genetic_algo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 14:17:48.000000 genetic-algo-0.0.5/genetic_algo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 14:17:48.000000 genetic-algo-0.0.5/genetic_algo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-03 14:17:48.000000 genetic-algo-0.0.5/genetic_algo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      645 2023-07-03 14:17:47.000000 genetic-algo-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       38 2023-06-18 08:47:03.000000 genetic-algo-0.0.5/requirements-dev.txt
+-rw-rw-rw-   0        0        0       29 2023-06-18 08:47:03.000000 genetic-algo-0.0.5/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 14:17:48.094955 genetic-algo-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1601 2023-07-03 14:17:45.000000 genetic-algo-0.0.5/setup.py
+-rw-rw-rw-   0        0        0     2645 2023-06-03 07:02:29.000000 genetic-algo-0.0.5/test.py
```

### Comparing `genetic-algo-0.0.4/PKG-INFO` & `genetic-algo-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genetic-algo
-Version: 0.0.4
+Version: 0.0.5
 Summary: A framework for developing Genetic-Algorithm programs to solve problems dynamically and explicitly.
 Home-page: https://github.com/Shahaf-F-S/auto-screener
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `genetic-algo-0.0.4/README.md` & `genetic-algo-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `genetic-algo-0.0.4/build.py` & `genetic-algo-0.0.5/build.py`

 * *Files identical despite different names*

### Comparing `genetic-algo-0.0.4/genetic_algo/attributes.py` & `genetic-algo-0.0.5/genetic_algo/attributes.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,26 +4,27 @@
     Self, Iterable, Any, Optional,
     Type, Union, Generic, TypeVar
 )
 import string
 import random
 from abc import ABCMeta
 
-from represent import BaseModel, Modifiers
+from represent import represent, Modifiers
 
 __all__ = [
     "Arguments",
     "Attribute",
     "NumericAttribute",
     "StringAttribute",
     "IntegerAttribute",
     "FloatAttribute"
 ]
 
-class Arguments(BaseModel):
+@represent
+class Arguments:
     """A class to represent a fitness function."""
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         """
         Calls the fitness function on the solution.
 
         :param args: Any positional arguments.
@@ -57,26 +58,26 @@
 
         return Arguments(*self.args, **self.kwargs)
     # end copy
 # end Arguments
 
 _V = TypeVar("_V")
 
-class Attribute(BaseModel, Generic[_V], metaclass=ABCMeta):
+@represent
+class Attribute(Generic[_V], metaclass=ABCMeta):
     """A class to represent an attribute of a solution."""
 
     NAME: Optional[str] = None
 
     EXCLUDED: Iterable[Any] = []
 
     arguments = Arguments()
 
-    modifiers = Modifiers(**BaseModel.modifiers)
-
-    modifiers.properties = True
+    __modifiers__ = Modifiers()
+    __modifiers__.properties = True
 
     def __init__(self, value: _V, name: Optional[str] = None) -> None:
         """
         Defines the class attributes.
 
         :param value: The value of the attribute.
         :param name: The name of the attribute.
```

### Comparing `genetic-algo-0.0.4/genetic_algo/driver.py` & `genetic-algo-0.0.5/genetic_algo/driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # driver.py
 
 from typing import Self, Optional, List
 from collections.abc import Iterator
 
-from represent import BaseModel
+from represent import represent
 
 from genetic_algo.environment import scale, Environment, Generation
 
 __all__ = [
     "Driver",
     "DriverDefinition"
 ]
 
-class DriverDefinition(BaseModel):
+@represent
+class DriverDefinition:
     """A class to contain the definition values of a driver object."""
 
     def __init__(
             self,
             fitness_limit: float,
             max_generations: int,
             min_improvement: float,
@@ -55,15 +56,16 @@
             fitness_limit=self.fitness_limit,
             max_generations=self.max_generations,
             min_improvement=self.min_improvement
         )
     # end copy
 # end DriverDefinition
 
-class Driver(BaseModel):
+@represent
+class Driver:
     """A class to represent a driver for genetic algorithm environments."""
 
     def __init__(
             self,
             definition: DriverDefinition,
             environment: Environment
     ) -> None:
```

### Comparing `genetic-algo-0.0.4/genetic_algo/environment.py` & `genetic-algo-0.0.5/genetic_algo/environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     Self, Iterable, Optional,
     Type, List, Dict, Union
 )
 import random
 from itertools import combinations
 from abc import abstractmethod
 
-from represent import BaseModel
+from represent import represent
 
 from multithreading import Caller, multi_threaded_call
 
 from genetic_algo.attributes import Attribute
 from genetic_algo.solution import Solution, Template, eliminate_repetitions
 
 __all__ = [
@@ -20,15 +20,16 @@
     "EnvironmentDefinition",
     "Fitness",
     "History",
     "Environment",
     "scale"
 ]
 
-class Generation(BaseModel):
+@represent
+class Generation:
     """A class to represent a generation of solutions."""
 
     def __init__(self, solutions: Iterable[Solution]) -> None:
         """
         Defines the class attributes.
 
         :param solutions: The solutions of the generation.
@@ -100,15 +101,16 @@
             f"relative {f'value {name}' or 'value'} of type {int} "
             f"must be in the range between {0} and {1}, "
             f"but {value} was given."
         )
     # end if
 # end scale
 
-class EnvironmentDefinition(BaseModel):
+@represent
+class EnvironmentDefinition:
     """A class to define the attributes of an environment."""
 
     def __init__(
             self,
             size: int,
             ascending: bool,
             successors: Optional[Union[int, float]] = None,
@@ -162,15 +164,16 @@
             successors=self.successors,
             continuers=self.continuers,
             mutations=self.mutations,
         )
     # end copy
 # end EnvironmentDefinition
 
-class Fitness(BaseModel):
+@represent
+class Fitness:
     """A class to represent a fitness function."""
 
     def __call__(self, solution: Solution) -> float:
         """
         Calls the fitness function on the solution.
 
         :param solution: The solution object.
@@ -189,15 +192,16 @@
         :param solution: The solution object.
 
         :return: The fitness value.
         """
     # end call
 # end Fitness
 
-class History(BaseModel):
+@represent
+class History:
     """A class to represent an environment history."""
 
     def __init__(self, generations: Optional[Iterable[Generation]] = None) -> None:
         """
         Defines the class attributes.
 
         :param generations: The generations to add to the history.
@@ -213,15 +217,16 @@
         :param generation: The generation to add to the history.
         """
 
         self.generations.append(generation)
     # end add
 # end History
 
-class Environment(BaseModel):
+@represent
+class Environment:
     """A class to represent an environment."""
 
     OPTIMIZE = False
 
     def __init__(
             self,
             definition: EnvironmentDefinition,
```

### Comparing `genetic-algo-0.0.4/genetic_algo/solution.py` & `genetic-algo-0.0.5/genetic_algo/solution.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # solution.py
 
 from typing import (
     Self, Iterable, Optional, Type,
     List, Union, Generic, TypeVar
 )
 
-from represent import BaseModel
+from represent import represent
 
 from genetic_algo.attributes import Attribute
 
 __all__ = [
     "Solution",
     "Template",
     "eliminate_repetitions",
     "same_solution"
 ]
 
-class Solution(BaseModel):
+@represent
+class Solution:
     """A class to represent a solution of a problem."""
 
     def __init__(self, attributes: Iterable[Attribute]) -> None:
         """
         Defines the class attributes.
 
         :param attributes: The attributes of the solution.
@@ -118,15 +119,16 @@
 Attributes = List[
     Union[
         Union[Attribute, Type[Attribute]],
         Iterable[Union[Attribute, Type[Attribute]]]
     ]
 ]
 
-class Template(BaseModel, Generic[_S]):
+@represent
+class Template(Generic[_S]):
     """A class to represent a template for solution attributes."""
 
     SOLUTION: _S = Solution
     ATTRIBUTES: Attributes = []
 
     def __init__(
             self,
```

### Comparing `genetic-algo-0.0.4/genetic_algo.egg-info/PKG-INFO` & `genetic-algo-0.0.5/genetic_algo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genetic-algo
-Version: 0.0.4
+Version: 0.0.5
 Summary: A framework for developing Genetic-Algorithm programs to solve problems dynamically and explicitly.
 Home-page: https://github.com/Shahaf-F-S/auto-screener
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `genetic-algo-0.0.4/pyproject.toml` & `genetic-algo-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'genetic-algo'
-version = '0.0.4'
+version = '0.0.5'
 description = 'A framework for developing Genetic-Algorithm programs to solve problems dynamically and explicitly.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `genetic-algo-0.0.4/setup.py` & `genetic-algo-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "test.py"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='genetic-algo',
-        version='0.0.4',
+        version='0.0.5',
         description=(
             "A framework for developing Genetic-Algorithm "
             "programs to solve problems dynamically and explicitly."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
         author_email='shahaffrs@gmail.com',
```

### Comparing `genetic-algo-0.0.4/test.py` & `genetic-algo-0.0.5/test.py`

 * *Files identical despite different names*

