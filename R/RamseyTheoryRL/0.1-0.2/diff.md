# Comparing `tmp/RamseyTheoryRL-0.1.tar.gz` & `tmp/RamseyTheoryRL-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RamseyTheoryRL-0.1.tar", last modified: Mon Jul  3 02:55:15 2023, max compression
+gzip compressed data, was "RamseyTheoryRL-0.2.tar", last modified: Mon Jul  3 03:06:15 2023, max compression
```

## Comparing `RamseyTheoryRL-0.1.tar` & `RamseyTheoryRL-0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 02:55:15.770269 RamseyTheoryRL-0.1/
--rw-r--r--   0 stevevott   (501) staff       (20)     1071 2023-07-03 02:47:52.000000 RamseyTheoryRL-0.1/LICENSE.txt
--rw-r--r--   0 stevevott   (501) staff       (20)     2743 2023-07-03 02:55:15.770165 RamseyTheoryRL-0.1/PKG-INFO
--rw-r--r--   0 stevevott   (501) staff       (20)     2096 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.1/README.md
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 02:55:15.770004 RamseyTheoryRL-0.1/RamseyTheoryRL.egg-info/
--rw-r--r--   0 stevevott   (501) staff       (20)     2743 2023-07-03 02:55:15.000000 RamseyTheoryRL-0.1/RamseyTheoryRL.egg-info/PKG-INFO
--rw-r--r--   0 stevevott   (501) staff       (20)      182 2023-07-03 02:55:15.000000 RamseyTheoryRL-0.1/RamseyTheoryRL.egg-info/SOURCES.txt
--rw-r--r--   0 stevevott   (501) staff       (20)        1 2023-07-03 02:55:15.000000 RamseyTheoryRL-0.1/RamseyTheoryRL.egg-info/dependency_links.txt
--rw-r--r--   0 stevevott   (501) staff       (20)        1 2023-07-03 02:55:15.000000 RamseyTheoryRL-0.1/RamseyTheoryRL.egg-info/top_level.txt
--rw-r--r--   0 stevevott   (501) staff       (20)       38 2023-07-03 02:55:15.770310 RamseyTheoryRL-0.1/setup.cfg
--rw-r--r--   0 stevevott   (501) staff       (20)      778 2023-07-03 02:55:10.000000 RamseyTheoryRL-0.1/setup.py
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:06:15.647801 RamseyTheoryRL-0.2/
+-rw-r--r--   0 stevevott   (501) staff       (20)     1071 2023-07-03 02:47:52.000000 RamseyTheoryRL-0.2/LICENSE.txt
+-rw-r--r--   0 stevevott   (501) staff       (20)     2760 2023-07-03 03:06:15.647696 RamseyTheoryRL-0.2/PKG-INFO
+-rw-r--r--   0 stevevott   (501) staff       (20)     2096 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.2/README.md
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-03 03:06:15.647531 RamseyTheoryRL-0.2/RamseyTheoryRL.egg-info/
+-rw-r--r--   0 stevevott   (501) staff       (20)     2760 2023-07-03 03:06:15.000000 RamseyTheoryRL-0.2/RamseyTheoryRL.egg-info/PKG-INFO
+-rw-r--r--   0 stevevott   (501) staff       (20)      182 2023-07-03 03:06:15.000000 RamseyTheoryRL-0.2/RamseyTheoryRL.egg-info/SOURCES.txt
+-rw-r--r--   0 stevevott   (501) staff       (20)        1 2023-07-03 03:06:15.000000 RamseyTheoryRL-0.2/RamseyTheoryRL.egg-info/dependency_links.txt
+-rw-r--r--   0 stevevott   (501) staff       (20)        1 2023-07-03 03:06:15.000000 RamseyTheoryRL-0.2/RamseyTheoryRL.egg-info/top_level.txt
+-rw-r--r--   0 stevevott   (501) staff       (20)       38 2023-07-03 03:06:15.647844 RamseyTheoryRL-0.2/setup.cfg
+-rw-r--r--   0 stevevott   (501) staff       (20)      795 2023-07-03 03:05:45.000000 RamseyTheoryRL-0.2/setup.py
```

### Comparing `RamseyTheoryRL-0.1/LICENSE.txt` & `RamseyTheoryRL-0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.1/PKG-INFO` & `RamseyTheoryRL-0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: RamseyTheoryRL
-Version: 0.1
+Version: 0.2
 Summary: Ramsey Number Explorer
 Home-page: https://github.com/aLehav/RamseyTheoryRL
 Author: Adam Lehavi, Steve Vott
-Author-email: svott03@gmail.com
+Author-email: svott03@gmail.com, alehavi@usc.edu
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,35 +1,36 @@
-Metadata-Version: 2.1 Name: RamseyTheoryRL Version: 0.1 Summary: Ramsey Number
+Metadata-Version: 2.1 Name: RamseyTheoryRL Version: 0.2 Summary: Ramsey Number
 Explorer Home-page: https://github.com/aLehav/RamseyTheoryRL Author: Adam
-Lehavi, Steve Vott Author-email: svott03@gmail.com License: MIT Platform:
-UNKNOWN Classifier: License :: OSI Approved :: MIT License Classifier:
-Programming Language :: Python Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Description-Content-Type:
-text/markdown License-File: LICENSE.txt # Ramsey Theory RL Exploration This is
-a small project that uses logistic regression with hybrid parameters and grid
-search to train or compare RL models for developing counterexamples for Ramsey
-Theory values. ## Structure - All runnable code inside src/ramsey_checker - Set
-environment variables, hyperparameters and data paths then run `python test.py`
-## Purpose The purpose of this project is to develop a model that can find a
-graph disproving a lower bound of R(r,k) using RL models and logistic
-regression with hybrid parameters. This will be accomplished through the
-following steps: 1. Define the problem and requirements: Clearly define the
-problem and the requirements for the model to be developed. 2. Gather data:
-Gather the data needed to train and test the model. This will involve
-collecting data on graphs and their properties. 3. Preprocess data: Preprocess
-the data to make it suitable for use with the model. This may involve cleaning
-the data, transforming it into a suitable format, or encoding it in a way that
-can be used by the model. 4. Train and test the model: Train and test the model
-using logistic regression with hybrid parameters and grid search to find the
-best hyperparameters. This will involve using RL models to develop
-counterexamples for Ramsey Theory values and evaluating the model's
-performance. 5. Evaluate and compare results: Evaluate the performance of the
-model and compare it to other RL models. This will involve comparing the
-accuracy, precision, and recall of the model to other models and analyzing the
-results. ## Progress - [x] Define the problem and requirements - [ ] Gather
-data - [ ] Preprocess data - [ ] Train and test the model - [ ] Evaluate and
-compare results As of now, the problem and requirements for the model have been
-defined. The next steps will be to gather and preprocess the data, train and
-test the model, and evaluate and compare the results. # Contributors [https://
-contrib.rocks/image?repo=aLehav/RamseyTheoryRL]
+Lehavi, Steve Vott Author-email: svott03@gmail.com, alehavi@usc.edu License:
+MIT Platform: UNKNOWN Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Description-
+Content-Type: text/markdown License-File: LICENSE.txt # Ramsey Theory RL
+Exploration This is a small project that uses logistic regression with hybrid
+parameters and grid search to train or compare RL models for developing
+counterexamples for Ramsey Theory values. ## Structure - All runnable code
+inside src/ramsey_checker - Set environment variables, hyperparameters and data
+paths then run `python test.py` ## Purpose The purpose of this project is to
+develop a model that can find a graph disproving a lower bound of R(r,k) using
+RL models and logistic regression with hybrid parameters. This will be
+accomplished through the following steps: 1. Define the problem and
+requirements: Clearly define the problem and the requirements for the model to
+be developed. 2. Gather data: Gather the data needed to train and test the
+model. This will involve collecting data on graphs and their properties. 3.
+Preprocess data: Preprocess the data to make it suitable for use with the
+model. This may involve cleaning the data, transforming it into a suitable
+format, or encoding it in a way that can be used by the model. 4. Train and
+test the model: Train and test the model using logistic regression with hybrid
+parameters and grid search to find the best hyperparameters. This will involve
+using RL models to develop counterexamples for Ramsey Theory values and
+evaluating the model's performance. 5. Evaluate and compare results: Evaluate
+the performance of the model and compare it to other RL models. This will
+involve comparing the accuracy, precision, and recall of the model to other
+models and analyzing the results. ## Progress - [x] Define the problem and
+requirements - [ ] Gather data - [ ] Preprocess data - [ ] Train and test the
+model - [ ] Evaluate and compare results As of now, the problem and
+requirements for the model have been defined. The next steps will be to gather
+and preprocess the data, train and test the model, and evaluate and compare the
+results. # Contributors [https://contrib.rocks/image?repo=aLehav/
+RamseyTheoryRL]
```

### Comparing `RamseyTheoryRL-0.1/README.md` & `RamseyTheoryRL-0.2/README.md`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.1/RamseyTheoryRL.egg-info/PKG-INFO` & `RamseyTheoryRL-0.2/RamseyTheoryRL.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: RamseyTheoryRL
-Version: 0.1
+Version: 0.2
 Summary: Ramsey Number Explorer
 Home-page: https://github.com/aLehav/RamseyTheoryRL
 Author: Adam Lehavi, Steve Vott
-Author-email: svott03@gmail.com
+Author-email: svott03@gmail.com, alehavi@usc.edu
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,35 +1,36 @@
-Metadata-Version: 2.1 Name: RamseyTheoryRL Version: 0.1 Summary: Ramsey Number
+Metadata-Version: 2.1 Name: RamseyTheoryRL Version: 0.2 Summary: Ramsey Number
 Explorer Home-page: https://github.com/aLehav/RamseyTheoryRL Author: Adam
-Lehavi, Steve Vott Author-email: svott03@gmail.com License: MIT Platform:
-UNKNOWN Classifier: License :: OSI Approved :: MIT License Classifier:
-Programming Language :: Python Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Description-Content-Type:
-text/markdown License-File: LICENSE.txt # Ramsey Theory RL Exploration This is
-a small project that uses logistic regression with hybrid parameters and grid
-search to train or compare RL models for developing counterexamples for Ramsey
-Theory values. ## Structure - All runnable code inside src/ramsey_checker - Set
-environment variables, hyperparameters and data paths then run `python test.py`
-## Purpose The purpose of this project is to develop a model that can find a
-graph disproving a lower bound of R(r,k) using RL models and logistic
-regression with hybrid parameters. This will be accomplished through the
-following steps: 1. Define the problem and requirements: Clearly define the
-problem and the requirements for the model to be developed. 2. Gather data:
-Gather the data needed to train and test the model. This will involve
-collecting data on graphs and their properties. 3. Preprocess data: Preprocess
-the data to make it suitable for use with the model. This may involve cleaning
-the data, transforming it into a suitable format, or encoding it in a way that
-can be used by the model. 4. Train and test the model: Train and test the model
-using logistic regression with hybrid parameters and grid search to find the
-best hyperparameters. This will involve using RL models to develop
-counterexamples for Ramsey Theory values and evaluating the model's
-performance. 5. Evaluate and compare results: Evaluate the performance of the
-model and compare it to other RL models. This will involve comparing the
-accuracy, precision, and recall of the model to other models and analyzing the
-results. ## Progress - [x] Define the problem and requirements - [ ] Gather
-data - [ ] Preprocess data - [ ] Train and test the model - [ ] Evaluate and
-compare results As of now, the problem and requirements for the model have been
-defined. The next steps will be to gather and preprocess the data, train and
-test the model, and evaluate and compare the results. # Contributors [https://
-contrib.rocks/image?repo=aLehav/RamseyTheoryRL]
+Lehavi, Steve Vott Author-email: svott03@gmail.com, alehavi@usc.edu License:
+MIT Platform: UNKNOWN Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Description-
+Content-Type: text/markdown License-File: LICENSE.txt # Ramsey Theory RL
+Exploration This is a small project that uses logistic regression with hybrid
+parameters and grid search to train or compare RL models for developing
+counterexamples for Ramsey Theory values. ## Structure - All runnable code
+inside src/ramsey_checker - Set environment variables, hyperparameters and data
+paths then run `python test.py` ## Purpose The purpose of this project is to
+develop a model that can find a graph disproving a lower bound of R(r,k) using
+RL models and logistic regression with hybrid parameters. This will be
+accomplished through the following steps: 1. Define the problem and
+requirements: Clearly define the problem and the requirements for the model to
+be developed. 2. Gather data: Gather the data needed to train and test the
+model. This will involve collecting data on graphs and their properties. 3.
+Preprocess data: Preprocess the data to make it suitable for use with the
+model. This may involve cleaning the data, transforming it into a suitable
+format, or encoding it in a way that can be used by the model. 4. Train and
+test the model: Train and test the model using logistic regression with hybrid
+parameters and grid search to find the best hyperparameters. This will involve
+using RL models to develop counterexamples for Ramsey Theory values and
+evaluating the model's performance. 5. Evaluate and compare results: Evaluate
+the performance of the model and compare it to other RL models. This will
+involve comparing the accuracy, precision, and recall of the model to other
+models and analyzing the results. ## Progress - [x] Define the problem and
+requirements - [ ] Gather data - [ ] Preprocess data - [ ] Train and test the
+model - [ ] Evaluate and compare results As of now, the problem and
+requirements for the model have been defined. The next steps will be to gather
+and preprocess the data, train and test the model, and evaluate and compare the
+results. # Contributors [https://contrib.rocks/image?repo=aLehav/
+RamseyTheoryRL]
```

### Comparing `RamseyTheoryRL-0.1/setup.py` & `RamseyTheoryRL-0.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name="RamseyTheoryRL",
-    version="0.1",
+    version="0.2",
     packages=find_packages(),
     author="Adam Lehavi, Steve Vott",
-    author_email="svott03@gmail.com",
+    author_email="svott03@gmail.com, alehavi@usc.edu",
     description="Ramsey Number Explorer",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     license="MIT",
     url="https://github.com/aLehav/RamseyTheoryRL",
     classifiers=[
         "License :: OSI Approved :: MIT License",
```

