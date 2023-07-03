# Comparing `tmp/melon_scheduler-0.1.7.tar.gz` & `tmp/melon_scheduler-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "melon_scheduler-0.1.7.tar", max compression
+gzip compressed data, was "melon_scheduler-0.1.8.tar", max compression
```

## Comparing `melon_scheduler-0.1.7.tar` & `melon_scheduler-0.1.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     2421 2023-07-02 14:15:03.534105 melon_scheduler-0.1.7/README.md
--rw-r--r--   0        0        0       77 2023-06-22 13:22:24.450031 melon_scheduler-0.1.7/melon/__init__.py
--rw-r--r--   0        0        0     4581 2023-06-30 17:27:21.260501 melon_scheduler-0.1.7/melon/calendar.py
--rw-r--r--   0        0        0      681 2023-07-02 11:05:41.555029 melon_scheduler-0.1.7/melon/config.py
--rw-r--r--   0        0        0     8584 2023-07-02 20:50:00.705171 melon_scheduler-0.1.7/melon/melon.py
--rw-r--r--   0        0        0       91 2023-07-01 17:20:32.719529 melon_scheduler-0.1.7/melon/scheduler/__init__.py
--rw-r--r--   0        0        0     3895 2023-07-02 19:12:32.132011 melon_scheduler-0.1.7/melon/scheduler/base.py
--rw-r--r--   0        0        0     1111 2023-07-02 16:04:48.097289 melon_scheduler-0.1.7/melon/scheduler/cpp.py
--rw-r--r--   0        0        0     4715 2023-07-02 19:15:13.039550 melon_scheduler-0.1.7/melon/scheduler/libcppscheduler.cpp
--rw-r--r--   0        0        0      451 2023-07-02 15:31:25.333156 melon_scheduler-0.1.7/melon/scheduler/libcppscheduler.pyi
--rwxr-xr-x   0        0        0   130504 2023-07-02 21:44:39.558368 melon_scheduler-0.1.7/melon/scheduler/libcppscheduler.so
--rw-r--r--   0        0        0      451 2023-07-02 15:35:21.503677 melon_scheduler-0.1.7/melon/scheduler/libscheduler.pyi
--rw-r--r--   0        0        0     4328 2023-07-02 19:15:07.335567 melon_scheduler-0.1.7/melon/scheduler/libscheduler.rs
--rwxr-xr-x   0        0        0  4377312 2023-07-02 21:44:39.554368 melon_scheduler-0.1.7/melon/scheduler/libscheduler.so
--rw-r--r--   0        0        0     5304 2023-07-02 19:17:20.331169 melon_scheduler-0.1.7/melon/scheduler/numba.py
--rw-r--r--   0        0        0     6450 2023-07-02 16:48:15.160006 melon_scheduler-0.1.7/melon/scheduler/purepython.py
--rw-r--r--   0        0        0     1114 2023-07-02 16:04:48.085290 melon_scheduler-0.1.7/melon/scheduler/rust.py
--rw-r--r--   0        0        0     7173 2023-07-02 15:23:32.496858 melon_scheduler-0.1.7/melon/todo.py
--rw-r--r--   0        0        0     2258 2023-07-02 17:03:15.137772 melon_scheduler-0.1.7/melon/visualise.py
--rw-r--r--   0        0        0      404 2023-06-30 13:41:03.809990 melon_scheduler-0.1.7/melongui/__init__.py
--rw-r--r--   0        0        0     1956 2023-06-17 21:27:46.117936 melon_scheduler-0.1.7/melongui/assets/complete.png
--rw-r--r--   0        0        0     1784 2023-06-17 21:25:13.617891 melon_scheduler-0.1.7/melongui/assets/complete.svg
--rw-r--r--   0        0        0     2047 2023-06-25 23:18:21.448400 melon_scheduler-0.1.7/melongui/calendarlist.py
--rw-r--r--   0        0        0      535 2023-07-02 17:13:51.295628 melon_scheduler-0.1.7/melongui/main.py
--rw-r--r--   0        0        0     4778 2023-07-02 20:47:21.583975 melon_scheduler-0.1.7/melongui/mainwindow.py
--rw-r--r--   0        0        0     5948 2023-07-02 11:46:31.918816 melon_scheduler-0.1.7/melongui/taskitemdelegate.py
--rw-r--r--   0        0        0     5793 2023-07-02 11:46:43.370796 melon_scheduler-0.1.7/melongui/tasklist.py
--rw-r--r--   0        0        0     2152 2023-06-30 13:42:12.081810 melon_scheduler-0.1.7/melongui/taskwidgets.py
--rw-r--r--   0        0        0     1505 2023-07-02 21:45:48.201596 melon_scheduler-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     3179 1970-01-01 00:00:00.000000 melon_scheduler-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     3542 2023-07-03 03:25:39.978642 melon_scheduler-0.1.8/README.md
+-rw-r--r--   0        0        0       77 2023-06-22 13:22:24.450031 melon_scheduler-0.1.8/melon/__init__.py
+-rw-r--r--   0        0        0     4581 2023-06-30 17:27:21.260501 melon_scheduler-0.1.8/melon/calendar.py
+-rw-r--r--   0        0        0      681 2023-07-02 11:05:41.555029 melon_scheduler-0.1.8/melon/config.py
+-rw-r--r--   0        0        0     8584 2023-07-02 20:50:00.705171 melon_scheduler-0.1.8/melon/melon.py
+-rw-r--r--   0        0        0       91 2023-07-01 17:20:32.719529 melon_scheduler-0.1.8/melon/scheduler/__init__.py
+-rw-r--r--   0        0        0     3895 2023-07-02 19:12:32.132011 melon_scheduler-0.1.8/melon/scheduler/base.py
+-rw-r--r--   0        0        0     1111 2023-07-02 16:04:48.097289 melon_scheduler-0.1.8/melon/scheduler/cpp.py
+-rw-r--r--   0        0        0     4715 2023-07-02 19:15:13.039550 melon_scheduler-0.1.8/melon/scheduler/libcppscheduler.cpp
+-rw-r--r--   0        0        0      451 2023-07-02 15:31:25.333156 melon_scheduler-0.1.8/melon/scheduler/libcppscheduler.pyi
+-rwxr-xr-x   0        0        0   130504 2023-07-02 21:44:39.558368 melon_scheduler-0.1.8/melon/scheduler/libcppscheduler.so
+-rw-r--r--   0        0        0      451 2023-07-02 15:35:21.503677 melon_scheduler-0.1.8/melon/scheduler/libscheduler.pyi
+-rw-r--r--   0        0        0     4328 2023-07-02 22:38:02.314459 melon_scheduler-0.1.8/melon/scheduler/libscheduler.rs
+-rwxr-xr-x   0        0        0  4377312 2023-07-02 21:44:39.554368 melon_scheduler-0.1.8/melon/scheduler/libscheduler.so
+-rw-r--r--   0        0        0     5304 2023-07-02 22:38:25.250393 melon_scheduler-0.1.8/melon/scheduler/numba.py
+-rw-r--r--   0        0        0     6453 2023-07-02 22:27:48.315286 melon_scheduler-0.1.8/melon/scheduler/purepython.py
+-rw-r--r--   0        0        0     1114 2023-07-02 16:04:48.085290 melon_scheduler-0.1.8/melon/scheduler/rust.py
+-rw-r--r--   0        0        0     7173 2023-07-02 15:23:32.496858 melon_scheduler-0.1.8/melon/todo.py
+-rw-r--r--   0        0        0     2258 2023-07-02 17:03:15.137772 melon_scheduler-0.1.8/melon/visualise.py
+-rw-r--r--   0        0        0      404 2023-06-30 13:41:03.809990 melon_scheduler-0.1.8/melongui/__init__.py
+-rw-r--r--   0        0        0     1956 2023-06-17 21:27:46.117936 melon_scheduler-0.1.8/melongui/assets/complete.png
+-rw-r--r--   0        0        0     1784 2023-06-17 21:25:13.617891 melon_scheduler-0.1.8/melongui/assets/complete.svg
+-rw-r--r--   0        0        0     2047 2023-06-25 23:18:21.448400 melon_scheduler-0.1.8/melongui/calendarlist.py
+-rw-r--r--   0        0        0      535 2023-07-02 17:13:51.295628 melon_scheduler-0.1.8/melongui/main.py
+-rw-r--r--   0        0        0     4778 2023-07-02 20:47:21.583975 melon_scheduler-0.1.8/melongui/mainwindow.py
+-rw-r--r--   0        0        0     5948 2023-07-02 11:46:31.918816 melon_scheduler-0.1.8/melongui/taskitemdelegate.py
+-rw-r--r--   0        0        0     5793 2023-07-02 11:46:43.370796 melon_scheduler-0.1.8/melongui/tasklist.py
+-rw-r--r--   0        0        0     2152 2023-06-30 13:42:12.081810 melon_scheduler-0.1.8/melongui/taskwidgets.py
+-rw-r--r--   0        0        0     1505 2023-07-03 03:26:33.262411 melon_scheduler-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     4300 1970-01-01 00:00:00.000000 melon_scheduler-0.1.8/PKG-INFO
```

### Comparing `melon_scheduler-0.1.7/melon/calendar.py` & `melon_scheduler-0.1.8/melon/calendar.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.7/melon/config.py` & `melon_scheduler-0.1.8/melon/config.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.7/melon/melon.py` & `melon_scheduler-0.1.8/melon/melon.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.7/melon/scheduler/base.py` & `melon_scheduler-0.1.8/melon/scheduler/base.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.7/melon/scheduler/cpp.py` & `melon_scheduler-0.1.8/melon/scheduler/cpp.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.7/melon/scheduler/libcppscheduler.cpp` & `melon_scheduler-0.1.8/melon/scheduler/libcppscheduler.cpp`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.7/melon/scheduler/libcppscheduler.so` & `melon_scheduler-0.1.8/melon/scheduler/libcppscheduler.so`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.7/melon/scheduler/libscheduler.rs` & `melon_scheduler-0.1.8/melon/scheduler/libscheduler.rs`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
   }
   return state;
 }
 
 fn schedule(tasks: &Vec<Task>) -> Vec<(String, TimeSlot)> {
   let n = tasks.len();
   let mut state = (0..n).collect();
-  for k in 1..11 {
+  for k in 1..16 {
     state = mcmc_sweep(&tasks, state, INITIAL_TEMPERATURE * (k as f64).powf(-1.0));
   }
   return spread_tasks(&tasks, &state);
 }
 
 fn py_schedule(_py: Python, tasks: Vec<(String, f32, u32, u32, f32)>) -> PyResult<Vec<(String, f32, f32)>> {
   let my_tasks: Vec<Task> = tasks
```

### Comparing `melon_scheduler-0.1.7/melon/scheduler/libscheduler.so` & `melon_scheduler-0.1.8/melon/scheduler/libscheduler.so`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.7/melon/scheduler/numba.py` & `melon_scheduler-0.1.8/melon/scheduler/numba.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,15 @@
     Args:
         tasks (Sequence[tuple[str, float, int, int, float]]): vector of tasks (uid, duration, priority, location, due)
 
     Returns:
         Sequence[tuple[str, float, float]]: vector of allocated timeslots (uid, timestamp, duration)
     """
     state = list(range(len(tasks)))
-    for k in range(1, 11):
+    for k in range(1, 16):
         temperature = INITIAL_TEMPERATURE * k**SWEEP_EXPONENT
         state = mcmcSweep(tasks, state, temperature)
     return spreadTasks([tasks[i] for i in state])
 
 
 class NumbaMCMCScheduler(AbstractScheduler):
     """Markov Chain Monte-Carlo Task Scheduler, implemented in Python with numba speed-up."""
```

### Comparing `melon_scheduler-0.1.7/melon/scheduler/purepython.py` & `melon_scheduler-0.1.8/melon/scheduler/purepython.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,9 +147,9 @@
 
         Returns:
             Mapping[str, TimeSlot]: the resulting map of Tasks to TimeSlots
         """
         for k in range(1, 16):
             self.temperature = INITIAL_TEMPERATURE * k**self.sweepExponent
             self.mcmcSweep()
-        logging.info("Final State of the MCMC simulation", self.state)
+        logging.info(f"Final State of the MCMC simulation {self.state}.")
         return dict(self.availability.spreadTasks(self.tasks[i] for i in self.state))
```

### Comparing `melon_scheduler-0.1.7/melon/scheduler/rust.py` & `melon_scheduler-0.1.8/melon/scheduler/rust.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.7/melon/todo.py` & `melon_scheduler-0.1.8/melon/todo.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.7/melon/visualise.py` & `melon_scheduler-0.1.8/melon/visualise.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.7/melongui/assets/complete.png` & `melon_scheduler-0.1.8/melongui/assets/complete.png`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.7/melongui/assets/complete.svg` & `melon_scheduler-0.1.8/melongui/assets/complete.svg`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.7/melongui/calendarlist.py` & `melon_scheduler-0.1.8/melongui/calendarlist.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.7/melongui/main.py` & `melon_scheduler-0.1.8/melongui/main.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.7/melongui/mainwindow.py` & `melon_scheduler-0.1.8/melongui/mainwindow.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.7/melongui/taskitemdelegate.py` & `melon_scheduler-0.1.8/melongui/taskitemdelegate.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.7/melongui/tasklist.py` & `melon_scheduler-0.1.8/melongui/tasklist.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.7/melongui/taskwidgets.py` & `melon_scheduler-0.1.8/melongui/taskwidgets.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.7/pyproject.toml` & `melon_scheduler-0.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "melon-scheduler"
-version = "0.1.7"
+version = "0.1.8"
 description = "Schedules Todos into your Calendar"
 authors = ["redacted"]
 readme = "README.md"
 packages = [{ include = "melon" }, { include = "melongui" }]
 include = ["melon/scheduler/libscheduler.so", "melon/scheduler/libcppscheduler.so"]
 
 [tool.poetry.dependencies]
```

### Comparing `melon_scheduler-0.1.7/PKG-INFO` & `melon_scheduler-0.1.8/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: melon-scheduler
-Version: 0.1.7
+Version: 0.1.8
 Summary: Schedules Todos into your Calendar
 Author: redacted
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: gui
@@ -20,14 +20,54 @@
 Description-Content-Type: text/markdown
 
 # Melon Task Scheduler + UI
 
 A CalDav Todo-List (/ Task-Scheduling) Application that uses Markov chain Monte-Carlo to optimise a task schedule.
 It also features a User Interface written with Qt6.
 
+To start the GUI:
+
+```python
+from melongui.main import main
+main() # to start the GUI
+```
+
+which launches a User Interface such as the one depicted in Figure 1.
+To load todos from a remote calendar, as specified in the configuration file, and
+schedule them, use the following code-snippet:
+
+```python
+from melon.melon import Melon
+from melon.scheduler.rust import RustyMCMCScheduler
+melon = Melon()
+melon.autoInit()
+melon.scheduleAllAndExport("task-schedule.ics", Scheduler=RustyMCMCScheduler)
+```
+
+In order to run the scheduler on demonstration data, please run
+
+```python
+from melon.scheduler.rust import RustyMCMCScheduler
+tasks = generateManyDemoTasks(N=80)
+scheduler = RustyMCMCScheduler(tasks)
+result = scheduler.schedule()
+```
+
+If not specified in the initialiser, Melon loads a configuration file located in the user’s
+home configuration directory, so on Linux `~/.config/melon/config.toml`. The
+file uses Tom’s Obvious, Minimal Language (TOML) format and has the following
+contents:
+
+```toml
+[client]
+url = "https://my-caldav-server.org:2023/dav/user/calendars/"
+username = "user"
+password = "password"
+```
+
 Melon is a Python package on a Markov chain Monte-Carlo (MCMC), using Metropolis-Hastings with Simulated Annealing, optimisation of task scheduling.
 The idea would be to automatically schedule a set of tasks into a calendar based on due date, duration estimate (perhaps dynamically updated), task priority, associated project affiliation and most importantly, location.
 State permutations would be generated randomly according to a probability distribution, starting from a good initial guess of ordering tasks by due date and priority.
 
 One can then define multiple optimisation metrics, based on the number of performed tasks weighted by priority and the need to switch locations.
 So in some sense, reducing the need for commute to e.g. work and scheduling hybrid / on-site tasks according to that (resembling the travelling-salesman problem).
 One could also make that very context dependent using project affiliations or certain keywords, automating the process.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

