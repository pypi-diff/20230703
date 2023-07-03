# Comparing `tmp/windeklar-0.2.2.tar.gz` & `tmp/windeklar-0.2.3.tar.gz`

## Comparing `windeklar-0.2.2.tar` & `windeklar-0.2.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 windeklar-0.2.2/requirements.txt
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 windeklar-0.2.2/setup.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 windeklar-0.2.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 windeklar-0.2.2/.idea/.gitignore
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 windeklar-0.2.2/.idea/.name
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 windeklar-0.2.2/.idea/WinDeklar.iml
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 windeklar-0.2.2/.idea/misc.xml
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 windeklar-0.2.2/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 windeklar-0.2.2/.idea/vcs.xml
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 windeklar-0.2.2/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 windeklar-0.2.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.2.2/src/__init__.py
--rwxr-xr-x   0        0        0    16032 2020-02-02 00:00:00.000000 windeklar-0.2.2/src/WinDeklar/QTAux.py
--rw-r--r--   0        0        0    44876 2020-02-02 00:00:00.000000 windeklar-0.2.2/src/WinDeklar/WindowForm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.2.2/src/WinDeklar/__init__.py
--rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 windeklar-0.2.2/src/WinDeklar/graph_aux.py
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 windeklar-0.2.2/src/WinDeklar/points_box.py
--rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 windeklar-0.2.2/src/WinDeklar/record.py
--rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 windeklar-0.2.2/src/WinDeklar/signal_aux.py
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 windeklar-0.2.2/src/WinDeklar/test_animation.py
--rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 windeklar-0.2.2/src/WinDeklar/test_pyqt.py
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 windeklar-0.2.2/src/WinDeklar/view_animation.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 windeklar-0.2.2/src/WinDeklar/view_animation.yaml
--rw-r--r--   0        0        0     6938 2020-02-02 00:00:00.000000 windeklar-0.2.2/src/WinDeklar/view_example.py
--rw-r--r--   0        0        0     4547 2020-02-02 00:00:00.000000 windeklar-0.2.2/src/WinDeklar/view_example.yaml
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 windeklar-0.2.2/src/WinDeklar/view_simple_graph.py
--rwxr-xr-x   0        0        0     6638 2020-02-02 00:00:00.000000 windeklar-0.2.2/src/WinDeklar/yaml_functions.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 windeklar-0.2.2/LICENSE
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 windeklar-0.2.2/README.md
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 windeklar-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 windeklar-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 windeklar-0.2.3/requirements.txt
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 windeklar-0.2.3/setup.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 windeklar-0.2.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 windeklar-0.2.3/.idea/.gitignore
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 windeklar-0.2.3/.idea/.name
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 windeklar-0.2.3/.idea/WinDeklar.iml
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 windeklar-0.2.3/.idea/misc.xml
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 windeklar-0.2.3/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 windeklar-0.2.3/.idea/vcs.xml
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 windeklar-0.2.3/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 windeklar-0.2.3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.2.3/src/__init__.py
+-rwxr-xr-x   0        0        0    16032 2020-02-02 00:00:00.000000 windeklar-0.2.3/src/WinDeklar/QTAux.py
+-rw-r--r--   0        0        0    45855 2020-02-02 00:00:00.000000 windeklar-0.2.3/src/WinDeklar/WindowForm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.2.3/src/WinDeklar/__init__.py
+-rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 windeklar-0.2.3/src/WinDeklar/graph_aux.py
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 windeklar-0.2.3/src/WinDeklar/points_box.py
+-rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 windeklar-0.2.3/src/WinDeklar/record.py
+-rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 windeklar-0.2.3/src/WinDeklar/signal_aux.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 windeklar-0.2.3/src/WinDeklar/test_animation.py
+-rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 windeklar-0.2.3/src/WinDeklar/test_pyqt.py
+-rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 windeklar-0.2.3/src/WinDeklar/view_animation.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 windeklar-0.2.3/src/WinDeklar/view_animation.yaml
+-rw-r--r--   0        0        0     6956 2020-02-02 00:00:00.000000 windeklar-0.2.3/src/WinDeklar/view_example.py
+-rw-r--r--   0        0        0     4547 2020-02-02 00:00:00.000000 windeklar-0.2.3/src/WinDeklar/view_example.yaml
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 windeklar-0.2.3/src/WinDeklar/view_simple_graph.py
+-rwxr-xr-x   0        0        0     6638 2020-02-02 00:00:00.000000 windeklar-0.2.3/src/WinDeklar/yaml_functions.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 windeklar-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 windeklar-0.2.3/README.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 windeklar-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 windeklar-0.2.3/PKG-INFO
```

### Comparing `windeklar-0.2.2/.github/workflows/python-publish.yml` & `windeklar-0.2.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.2/.idea/inspectionProfiles/Project_Default.xml` & `windeklar-0.2.3/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.2/src/WinDeklar/QTAux.py` & `windeklar-0.2.3/src/WinDeklar/QTAux.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.2/src/WinDeklar/WindowForm.py` & `windeklar-0.2.3/src/WinDeklar/WindowForm.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,29 +55,32 @@
 
         # menu bar
         menu_bar = create_menu_bar(self.win_config, self, self.provider)
         if menu_bar is not None:
             self.setMenuBar(menu_bar)
 
         # toolbar
-        toolbar = create_toolbar(self.win_config, self, self.provider, self.controls)
+        toolbar, toolbar_controls = create_toolbar(self.win_config, self, self.provider)
         if toolbar is not None:
+            self.controls.extend(toolbar_controls)
             self.addToolBar(toolbar)
 
         # Define the geometry of the main window
         size = self.win_config.get('size', [300, 300, 300, 300])
         QTAux.set_window(self, get_title(self.win_config, self.provider), size)
 
         # Create FRAME
         self.FRAME = QtWidgets.QFrame(self)
         if 'back_color' in self.win_config:
             [c1, c2, c3, c4] = self.win_config['back_color']
             self.FRAME.setStyleSheet("QWidget { background-color: %s }" % QtGui.QColor(c1, c2, c3, c4).name())
         self.LAYOUT   = QtWidgets.QGridLayout()
-        self.fig_views, self.controls = set_layout(self.LAYOUT, self.win_config.get('layout', []), self, row_col=[0, 0])
+        self.fig_views, layout_controls = set_layout(self.LAYOUT, self.win_config.get('layout', []), self,
+                                                     row_col=[0, 0])
+        self.controls.extend(layout_controls)
         self.FRAME.setLayout(self.LAYOUT)
         self.setCentralWidget(self.FRAME)
 
         self.provider.initialize()
         self.refresh()
         self.show()
 
@@ -130,14 +133,26 @@
 
     def get_control_by_name(self, control_name):
         for control in self.controls:
             if control.name == control_name:
                 return control
         return None
 
+    def anim_is_running(self):
+        for figure in self.fig_views:
+            if figure.anim_is_running:
+                return True
+        return False
+
+    def start_animations(self):
+        [figure.start_animation() for figure in self.fig_views]
+
+    def stop_animations(self):
+        [figure.stop_animation() for figure in self.fig_views]
+
     def show_status_bar_msg(self, msg):
         if self.statusbar is None:
             print('No status bar defined')
             return
         self.statusbar.showMessage(msg)
 
 
@@ -205,15 +220,15 @@
         self.graph_lines   = None  # set to None to signal graph are not initialized yet
         self.data_provider = None
         self.graph_bounds  = None
         self.points_in_graph = 0
         self.anim_is_running = False
         if self.subtype == self.animation_key:
             interval, self.points_in_graph, self.graph_bounds, self.data_provider = \
-                self.parent.provider.get_data_provider()
+                self.parent.provider.get_data_provider(self)
             if self.data_provider is None:
                 raise Exception(
                     'Figure is defined as "animation" but not data provider is given, implement get_data_provider() '
                     'in provider ')
             self.anim = animation.FuncAnimation(self.figure, self.update_frame, frames=None, interval=interval,
                                                 blit=False)
 
@@ -246,15 +261,15 @@
         # assigning ' ' is a quick fix to assure y values fit in the figure
         self.axes.set_ylabel(ylabel_name)
         if self.x_axis_name is not None:
             self.axes.set_xlabel(self.x_axis_name)
 
     def update_figure(self):
         self.clear()
-        self.parent.provider.update_view(self.name, self.axes)
+        self.parent.provider.update_view(self, self.axes)
         self.parent.provider.apply_zoom()
         self.draw()
 
     # Events
     def onclick(self, event):
         self.parent.provider.on_mouse_click(event, self.axes, self)
         self.set_axis()
@@ -623,19 +638,19 @@
 
     def show_status_bar_msg(self, msg):
         if self.main_window is None:
             print('no main window defined yet')
             return
         self.main_window.show_status_bar_msg(msg)
 
-    def update_view(self, name, ax):
+    def update_view(self, figure, ax):
         """
         Update view of a given Figure
         Abstract method
-        :param name: name of the Figure
+        :param figure: name of the Figure
         :param ax:   axis of the Figure
         :return:
         """
         pass
 
     # Zoom management
     def zoom_active(self):
@@ -730,36 +745,51 @@
         print('File %s saved' % r.get_full_file_name())
 
     def get_info_to_save(self):
         # abstract method
         return {}
 
     # animation methods
-    def get_data_provider(self, interval=100, min_x=0.0, max_x=10.0, data_provider=None):
+    def get_data_provider(self, figure, interval=100, min_x=0.0, max_x=10.0, data_provider=None):
         """
         Abstract method
+        :param figure:   :type FigureView
         :param interval: time at which show new data (in milliseconds)
         :param max_x:    max value in the x-axis, values greater than this will cause the graph to scroll left
         :param min_x:    start value for the x-axis
         :param data_provider:  subclass of RealTimeDataProvider (can be None)
         :return: interval (milliseconds), number of points to show, x axis bounds (ex: [-1, 100]), subclass of
                  RealTimeDataProvider (can be None)
         """
         dt            = interval/1000  # seconds
         max_points    = int(max_x/dt) + 1
         return interval, max_points, (min_x, max_x), data_provider
 
+    def start_stop_animation(self):
+        """
+        Logit to start/stop the graph with only one button (who changes its title depending on the graph is
+        running or not_
+        :return:
+        """
+        if self.anim_is_running():
+            self.stop_animation()
+            is_running = False
+        else:
+            self.start_animation()
+            is_running = True
+        return is_running
+
     def anim_is_running(self):
-        return self.main_window.fig_view.anim_is_running
+        return self.main_window.anim_is_running()
 
     def stop_animation(self):
-        self.main_window.fig_view.stop_animation()
+        self.main_window.stop_animations()
 
     def start_animation(self):
-        self.main_window.fig_view.start_animation()
+        self.main_window.start_animations()
 
 
 class PropertiesHost(HostModel):
     """
     HostModel specialized for editing a set of properties (defined as a dict)
     """
 
@@ -972,18 +1002,20 @@
                                                            function_name=sub_item.get('action', None)))
                 # action = QTAux.MenuItem('1', sub_item['title'], self.provider, sub_item.get('action', None),
                 #                        None, self)
                 main_menu.addAction(action)
     return menu_bar
 
 
-def create_toolbar(config, main_window, provider, controls, key='toolbar', icon_key='icon', tooltip_key='tooltip',
+def create_toolbar(config, main_window, provider, key='toolbar', icon_key='icon', tooltip_key='tooltip',
                    combo_key='Combo', check_key='Check', type_key='type', label_key='Label', action_key='Action'):
+    controls = []
     if key not in config:
-        return None
+        return None, controls
+
     toolbar        = QtWidgets.QToolBar()
     toolbar_config = config[key]
     for item1 in toolbar_config:
         item      = item1['item']
         title     = item.get('title', '')
         name      = item.get('name', 'NoName')
         item_type = item.get(type_key, 'Action')
@@ -1003,15 +1035,15 @@
             action.qt_action.triggered.connect(functools.partial(exec_action, provider,
                                                                  function_name=item.get('action', None)))
             toolbar.addAction(action.qt_action)
             controls.append(action)
         else:
             raise Exception('%s is not implemented in Toolbar' % item_type)
 
-    return toolbar
+    return toolbar, controls
 
 
 def create_status_bar(win_config, main_window, status_key='status_bar'):
     if not win_config.get(status_key, True):  # create a statusbar unless is explicitly forbidden
         return None
     statusbar = QtWidgets.QStatusBar(main_window)
     main_window.setStatusBar(statusbar)
```

### Comparing `windeklar-0.2.2/src/WinDeklar/graph_aux.py` & `windeklar-0.2.3/src/WinDeklar/graph_aux.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.2/src/WinDeklar/points_box.py` & `windeklar-0.2.3/src/WinDeklar/points_box.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.2/src/WinDeklar/record.py` & `windeklar-0.2.3/src/WinDeklar/record.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.2/src/WinDeklar/signal_aux.py` & `windeklar-0.2.3/src/WinDeklar/signal_aux.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.2/src/WinDeklar/test_animation.py` & `windeklar-0.2.3/src/WinDeklar/test_animation.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.2/src/WinDeklar/test_pyqt.py` & `windeklar-0.2.3/src/WinDeklar/test_pyqt.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.2/src/WinDeklar/view_animation.py` & `windeklar-0.2.3/src/WinDeklar/view_animation.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,57 +9,68 @@
 
 
 class ExampleHost(WinForm.HostModel):
     """
     Shows tentacles
     """
 
-    def __init__(self, function=np.sin, color='Blue', y_bounds=(-1.2, 1.2)):
+    def __init__(self, function1=np.sin, function2=np.cos, color='Blue', y_bounds=(-1.2, 1.2)):
         # keys (names used in the yaml definition file)
         self.start_stop_key        = 'start_stop'
         self.start_stop_action_key = 'start_stop_action'
+        self.graph1_key = 'graph1'
+        self.graph2_key = 'graph2'
 
         # particular data
-        self.function = function
+        self.function1 = function1
+        self.function2 = function2
         self.color    = color
         self.y_bounds = y_bounds
 
         initial_values = {}
         super(ExampleHost, self).__init__(initial_values=initial_values)
 
-    def get_data_provider(self, interval=100, min_x=0.0, max_x=10.0, data_provider=None):
+    def get_data_provider(self, figure, interval=100, min_x=0.0, max_x=10.0, data_provider=None):
         """
         Returns the basic setup of the graph, most important one is the data provider
+        :param figure:
         :param interval:       time in milliseconds to show each point in the graph
         :param min_x:          start value in the x-axis
         :param max_x:          max value in the x-axis, after that it starts to scroll left
         :param data_provider:  subclass of RealTimeDataProvider
         :return:
         """
+        if figure.name == self.graph1_key:
+            function = self.function1
+        elif figure.name == self.graph2_key:
+            function = self.function2
+        else:
+            raise Exception('"%s" graph name not implemented (valids are %s and %s)' %
+                            (figure.name, self.graph1_key, self.graph2_key))
+
         dt             = interval/1000  # seconds
         max_points     = int(max_x/dt) + 1
         x_bounds       = [min_x, max_x]
         data_provider1 = [ga.RealTimeFunctionDataProvider(dt=dt, min_y=self.y_bounds[0], max_y=self.y_bounds[1],
-                                                          function=self.function, color=self.color)]
+                                                          function=function, color=self.color)]
         return interval, max_points, x_bounds, data_provider1
 
-    def start_stop_animation(self):
+    def start_stop(self):
         """
         Logit to start/stop the graph with only one button (who changes its title depending on the graph is
         running or not_
         :return:
         """
-        if self.anim_is_running():
-            self.stop_animation()
-            self.set_control_title(self.start_stop_key, 'Restart Animation')
-            self.set_control_title(self.start_stop_action_key, 'Restart Animation')
-        else:
-            self.start_animation()
+        is_running = self.start_stop_animation()
+        if is_running:
             self.set_control_title(self.start_stop_key, 'Pause Animation')
             self.set_control_title(self.start_stop_action_key, 'Pause Animation')
+        else:
+            self.set_control_title(self.start_stop_key, 'Restart Animation')
+            self.set_control_title(self.start_stop_action_key, 'Restart Animation')
 
 
 if __name__ == '__main__':
     app = QTAux.def_app()
     provider = ExampleHost()        # class to handle the WinForm logic
     WinForm.run_winform(__file__, provider)
     sys.exit(app.exec_())
```

### Comparing `windeklar-0.2.2/src/WinDeklar/view_example.py` & `windeklar-0.2.3/src/WinDeklar/view_example.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,32 +47,32 @@
         :param name:
         :param value:
         :return:
         """
         if name == self.type_key:
             self.show_status_bar_msg('%s graph type chosen' % value)
 
-    def update_view(self, name, ax):
+    def update_view(self, figure, ax):
         """
         Update the figure
         Notes:
             - This method is called when any property changes or refresh() is used
             - All form variables are in dict self.state
-        :param name:
+        :param figure:
         :param ax:
         :return:
         """
-        if name == self.graph1_key:
+        if figure.name == self.graph1_key:
             function_name = self.state.get(self.type_key, 'None')
             points        = self.get_graph_points(function_name)
             show_axis     = [True, True] if self.state.get(self.axis_key, True) else [False, False]
             ga.graph_points(ax, points, x_visible=show_axis[0], y_visible=show_axis[1],
                             line_width=self.state.get(self.width_key, 1.0))
             self.resize_figure(ax, points)
-        elif name == self.graph2_key:
+        elif figure.name == self.graph2_key:
             number_of_points = int(self.state.get(self.points_key, 10))
             p1 = [number_of_points, number_of_points]
             p2 = [0, 0]
             show_arrow(ax, p1, p2)
             self.resize_figure(ax, [p1, p2])
 
     def redraw(self):
```

### Comparing `windeklar-0.2.2/src/WinDeklar/view_example.yaml` & `windeklar-0.2.3/src/WinDeklar/view_example.yaml`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.2/src/WinDeklar/view_simple_graph.py` & `windeklar-0.2.3/src/WinDeklar/view_simple_graph.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.2/src/WinDeklar/yaml_functions.py` & `windeklar-0.2.3/src/WinDeklar/yaml_functions.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.2/LICENSE` & `windeklar-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.2/README.md` & `windeklar-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.2/pyproject.toml` & `windeklar-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name    = "WinDeklar"
-version = "0.2.2"
+version = "0.2.3"
 authors = [
   { name="Nicolas Jodal", email="jnj@genexus.com" },
 ]
 description = "Create winforms in an easy, declarative way. Specially suited for Robotics applications"
 readme      = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `windeklar-0.2.2/PKG-INFO` & `windeklar-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WinDeklar
-Version: 0.2.2
+Version: 0.2.3
 Summary: Create winforms in an easy, declarative way. Specially suited for Robotics applications
 Project-URL: Homepage, https://github.com/njodal/WinDeklar
 Project-URL: Bug Tracker, https://github.com/njodal/WinDeklar/issues
 Author-email: Nicolas Jodal <jnj@genexus.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

