# Comparing `tmp/mapdata-2.8.3.tar.gz` & `tmp/mapdata-2.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapdata-2.8.3.tar", last modified: Fri Jun 30 14:48:03 2023, max compression
+gzip compressed data, was "mapdata-2.8.6.tar", last modified: Mon Jul  3 18:55:12 2023, max compression
```

## Comparing `mapdata-2.8.3.tar` & `mapdata-2.8.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-06-30 14:48:03.360272 mapdata-2.8.3/
--rw-------   0 dreas     (1000) dreas     (1000)      614 2023-05-10 02:52:31.000000 mapdata-2.8.3/LICENSE.txt
--rw-------   0 dreas     (1000) dreas     (1000)       88 2022-01-15 18:16:09.000000 mapdata-2.8.3/MANIFEST.in
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     4115 2023-06-30 14:48:03.360272 mapdata-2.8.3/PKG-INFO
--rw-r--r--   0 dreas     (1000) dreas     (1000)     2870 2023-06-28 13:59:57.000000 mapdata-2.8.3/README.md
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-06-30 14:48:03.360272 mapdata-2.8.3/mapdata/
--rwxrwxr-x   0 dreas     (1000) dreas     (1000)   336291 2023-06-30 14:41:41.000000 mapdata-2.8.3/mapdata/mapdata.py
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-06-30 14:48:03.360272 mapdata-2.8.3/mapdata.egg-info/
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     4115 2023-06-30 14:48:03.000000 mapdata-2.8.3/mapdata.egg-info/PKG-INFO
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      185 2023-06-30 14:48:03.000000 mapdata-2.8.3/mapdata.egg-info/SOURCES.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-06-30 14:48:03.000000 mapdata-2.8.3/mapdata.egg-info/dependency_links.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-06-30 14:48:03.000000 mapdata-2.8.3/mapdata.egg-info/top_level.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)       38 2023-06-30 14:48:03.360272 mapdata-2.8.3/setup.cfg
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     1366 2023-06-30 14:45:27.000000 mapdata-2.8.3/setup.py
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-07-03 18:55:12.982781 mapdata-2.8.6/
+-rw-------   0 dreas     (1000) dreas     (1000)      614 2023-05-10 02:52:31.000000 mapdata-2.8.6/LICENSE.txt
+-rw-------   0 dreas     (1000) dreas     (1000)       88 2022-01-15 18:16:09.000000 mapdata-2.8.6/MANIFEST.in
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     4115 2023-07-03 18:55:12.982781 mapdata-2.8.6/PKG-INFO
+-rw-r--r--   0 dreas     (1000) dreas     (1000)     2870 2023-06-28 13:59:57.000000 mapdata-2.8.6/README.md
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-07-03 18:55:12.982781 mapdata-2.8.6/mapdata/
+-rwxrwxr-x   0 dreas     (1000) dreas     (1000)   339131 2023-07-03 18:22:21.000000 mapdata-2.8.6/mapdata/mapdata.py
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-07-03 18:55:12.982781 mapdata-2.8.6/mapdata.egg-info/
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     4115 2023-07-03 18:55:12.000000 mapdata-2.8.6/mapdata.egg-info/PKG-INFO
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      185 2023-07-03 18:55:12.000000 mapdata-2.8.6/mapdata.egg-info/SOURCES.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-07-03 18:55:12.000000 mapdata-2.8.6/mapdata.egg-info/dependency_links.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-07-03 18:55:12.000000 mapdata-2.8.6/mapdata.egg-info/top_level.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)       38 2023-07-03 18:55:12.982781 mapdata-2.8.6/setup.cfg
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     1366 2023-07-03 12:55:05.000000 mapdata-2.8.6/setup.py
```

### Comparing `mapdata-2.8.3/LICENSE.txt` & `mapdata-2.8.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mapdata-2.8.3/PKG-INFO` & `mapdata-2.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapdata
-Version: 2.8.3
+Version: 2.8.6
 Summary: An interactive map and table explorer for geographic coordinates in a spreadsheet, CSV file, or database
 Home-page: https://osdn.net/project/mapdata/
 Author: Dreas Nielsen
 Author-email: dreas.nielsen@gmail.com
 License: GPL
 Keywords: Map,Locations,CRS,CSV,Spreadsheet,Database,PNG,JPG,Postscript
 Platform: UNKNOWN
```

### Comparing `mapdata-2.8.3/README.md` & `mapdata-2.8.6/README.md`

 * *Files identical despite different names*

### Comparing `mapdata-2.8.3/mapdata/mapdata.py` & `mapdata-2.8.6/mapdata/mapdata.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 # 	The GNU General Public License is available at <http://www.gnu.org/licenses/>
 #
 # AUTHOR
 #	Dreas Nielsen (RDN)
 #
 # ==================================================================
 
-version = "2.8.3"
-vdate = "2023-06-30"
+version = "2.8.6"
+vdate = "2023-07-03"
 
 copyright = "2023"
 
 
 import sys
 import os.path
 import io
@@ -202,14 +202,22 @@
 	'diamond': """#define diamond_width 16
 #define diamond_height 16
 static unsigned char diamond_bits[] = {
    0x80, 0x01, 0xc0, 0x03, 0xe0, 0x07, 0xf0, 0x0f, 0xf8, 0x1f, 0xfc, 0x3f,
    0xfe, 0x7f, 0xff, 0xff, 0xff, 0xff, 0xfe, 0x7f, 0xfc, 0x3f, 0xf8, 0x1f,
    0xf0, 0x0f, 0xe0, 0x07, 0xc0, 0x03, 0x80, 0x01};""",
 
+   'drop': """,
+#define drop.xbm_width 16
+#define drop.xbm_height 16
+static unsigned char drop.xbm_bits[] = {
+   0x80, 0x01, 0x80, 0x01, 0xc0, 0x03, 0xc0, 0x03, 0xe0, 0x07, 0xe0, 0x07,
+   0xf8, 0x1f, 0xf8, 0x1f, 0xfc, 0x3f, 0xfc, 0x3f, 0xfc, 0x3f, 0xfc, 0x3f,
+   0xfc, 0x3f, 0xf0, 0x1f, 0xf0, 0x0f, 0xc0, 0x03};""",
+
    'fish': """#define fish_width 16
 #define fish_height 16
 static unsigned char fish.xbm_bits[] = {
    0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x01, 0x00, 0x03, 0x01, 0x0f,
    0xe3, 0x7f, 0xf7, 0x78, 0x3e, 0xea, 0x9e, 0xfb, 0x73, 0x84, 0xc1, 0x63,
    0x01, 0x3e, 0x00, 0x18, 0x00, 0x18, 0x00, 0x08};""",
 
@@ -679,15 +687,15 @@
 					return 'timestamp'
 				else:
 					return "string"
 		else:
 			return "string"
 
 
-def set_data_types(headers, rows, q):
+def set_data_types_core(headers, rows):
 	# Column-by-column processing is slightly faster than row-by-row processing.
 	coltypes = []
 	for i, colname in enumerate(headers):
 		datavals = [row[i] for row in rows]
 		dt = None
 		for d in datavals:
 			ndt = data_type(d)
@@ -695,15 +703,18 @@
 				dt = priority_data_type(ndt, dt)
 				if dt == "string":
 					break
 		non_null = [d for d in datavals if d is not None and not (type(d) is str and d.strip() == '')]
 		nullcount = len(datavals) - len(non_null)
 		uniquevals = len(set(non_null))
 		coltypes.append((colname, dt, nullcount, uniquevals))
-	q.put(coltypes)
+	return coltypes
+
+def set_data_types(headers, rows, q):
+	q.put(set_data_types_core(headers, rows))
 
 
 # Translations to SQLite type affinity names
 sqlite_type_x = {'int': 'INTEGER', 'float': 'REAL', 'string': 'TEXT', 'timestamptz': 'TEXT',
 		'timestamp': 'TEXT', 'date': 'TEXT', 'boolean': 'INTEGER'}
 
 def center_window(win, x_offset=0, y_offset=0):
@@ -735,72 +746,30 @@
 class MapUI(object):
 	def __init__(self, src_name, message, lat_col, lon_col, crs=4326, sheet=None,
 			label_col=None, symbol_col=None, color_col=None,
 			map_export_file=None, export_time_sec=10):
 		self.win = tk.Tk()
 		self.win.withdraw()
 		self.loading_dlg = LoadingDialog(self.win)
-		if src_name is None:
-			sdsd = SelDataSrcDialog(parent=self.win, mapui=self)
-			src_name, label_col, lat_col, lon_col, crs, symbol_col, color_col, message, headers, rows = sdsd.select()
-			if src_name is None:
-				self.cancel()
-		else:
-			# src_name is a filename, either CSV or spreadsheet
-			self.loading_dlg.display("Loading data")
-			fn, ext = os.path.splitext(src_name)
-			if ext.lower() == ".csv":
-				try:
-					headers, rows = file_data(src_name, 0)
-				except:
-					self.loading_dlg.hide_all()
-					fatal_error("Could not read data from %s" % src_data, kwargs={'parent': self.win})
-			else:
-				if sheet is None:
-					self.loading_dlg.hide_all()
-					fatal_error("A sheet name must be specified for spreadsheets", kwargs={'parent': self.win})
-				try:
-					if ext.lower() == '.ods':
-						headers, rows = ods_data(src_name, sheet, 0)
-					else:
-						headers, rows = xls_data(src_name, sheet, 0)
-				except:
-					self.loading_dlg.hide_all()
-					fatal_error("Could not read table from %s, sheet %s" % (src_name, sheet), kwargs={'parent': self.win})
-			self.loading_dlg.hide()
-		self.win.deiconify()
+		self.loading_dlg.display("Preparing map")
 
 		# Size and position window.
 		self.win.geometry("1200x1000")
-		self.win.update_idletasks()
-		m = re.match(r"(\d+)x(\d+)\+(-?\d+)\+(-?\d+)", self.win.geometry())
-		if m is not None:
-			wwd = int(m.group(1))
-			wht = int(m.group(2))
-			swd = self.win.winfo_screenwidth()
-			sht = self.win.winfo_screenheight()
-			xpos = (swd/2) - (wwd/2)
-			ypos = (sht/2) - (wht/2)
-			self.win.geometry("%dx%d+%d+%d" % (wwd, wht, xpos, ypos))
-
-		self.loading_dlg.display("Preparing map")
+		center_window(self.win)
 
 		self.win.protocol("WM_DELETE_WINDOW", self.cancel)
 		self.data_src_name = src_name
 		self.win.title("Map of %s" % src_name)
 		# Patch ImageTk.PhotoImage.__del__ 
 		ImageTk.PhotoImage.__del__ = new_img_del
 		# Set the font
 		self.mapfont = self.makefont()
 		# Set the application window icon
 		#win_icon = tk.BitmapImage(data=win_icon_xbm, foreground="black", background="tan")
 		#self.win.iconbitmap(win_icon)
-		# Source and possibly un-projected crs
-		self.src_crs = crs
-		self.crs = crs
 		# The markers for all the locations in the data table
 		self.loc_map_markers = []
 		# The markers for the selected location(s)
 		self.sel_map_markers = []
 		# The number of table rows without coordinates
 		self.missing_latlon = 0
 		# Map bounds
@@ -894,20 +863,62 @@
 		mapframe.rowconfigure(0, weight=1)
 		mapframe.columnconfigure(0, weight=1)
 		self.map_widget = tkmv.TkinterMapView(mapframe, height=600, width=600, corner_radius=0)
 		if initial_basemap != "OpenMapServer":
 			tileserver = self.tile_url(initial_basemap)
 			self.map_widget.set_tile_server(tileserver)
 		self.map_widget.grid(row=0, column=0, sticky=tk.NSEW)
+
+		# Remove the splash screen message and show the main UI.
+		self.loading_dlg.hide()
+		# Re-setting the size is necessary on Windows in at least some environments.
+		self.win.geometry("1200x1000")
+		self.win.deiconify()
+
+		# Get data if not provided as arguments
+		if src_name is None:
+			sdsd = SelDataSrcDialog(parent=self.win, mapui=self)
+			src_name, label_col, lat_col, lon_col, crs, symbol_col, color_col, message, headers, rows = sdsd.select()
+			if src_name is None:
+				self.cancel()
+		else:
+			# src_name is a filename, either CSV or spreadsheet
+			self.loading_dlg.display("Loading data")
+			fn, ext = os.path.splitext(src_name)
+			if ext.lower() == ".csv":
+				try:
+					headers, rows = file_data(src_name, 0)
+				except:
+					self.loading_dlg.hide_all()
+					fatal_error("Could not read data from %s" % src_data, kwargs={'parent': self.win})
+			else:
+				if sheet is None:
+					self.loading_dlg.hide_all()
+					fatal_error("A sheet name must be specified for spreadsheets", kwargs={'parent': self.win})
+				try:
+					if ext.lower() == '.ods':
+						headers, rows = ods_data(src_name, sheet, 0)
+					else:
+						headers, rows = xls_data(src_name, sheet, 0)
+				except:
+					self.loading_dlg.hide_all()
+					fatal_error("Could not read table from %s, sheet %s" % (src_name, sheet), kwargs={'parent': self.win})
+			self.loading_dlg.hide()
+
+		self.msg_label.config(text=message)
+
+		# Source and possibly un-projected crs
+		self.src_crs = crs
+		self.crs = crs
+
 		# Populate the table frame
 		self.tblframe.rowconfigure(0, weight=1)
 		self.tblframe.columnconfigure(0, weight=1)
 		try:
-			self.tableframe, self.tbl = self.add_data(rows, headers, lat_col, lon_col, label_col,
-					symbol_col, color_col)
+			self.tableframe, self.tbl = self.add_data(rows, headers, lat_col, lon_col, label_col, symbol_col, color_col)
 		except:
 			self.loading_dlg.hide_all()
 			fatal_error("Cannot load data.  Check latitude, longitude, and CRS values.", kwargs={'parent': self.win})
 		self.tableframe.grid(column=0, row=0, sticky=tk.NSEW)
 		self.set_tbl_selectmode()
 		self.set_status()
 		# Add menu
@@ -1093,20 +1104,20 @@
 		self.color_index = headers.index(color_col) if color_col is not None and color_col != '' else None
 
 		if self.crs != 4326:
 			try:
 				from pyproj import CRS, Transformer
 			except:
 				self.loading_dlg.hide_all()
-				fatal_error("The pyproj library is required to re-project spatial coordinates")
+				fatal_error("The pyproj library is required to re-project spatial coordinates", kwargs={})
 			try:
 				crs_proj = CRS(self.crs)
 			except:
 				self.loading_dlg.hide_all()
-				fatal_error("Invalid CRS (%s)" % self.crs)
+				fatal_error("Invalid CRS (%s)" % self.crs, kwargs={})
 			if self.lat_4326_col is None:
 				for colname in ('lat_4326', 'latitude_4326', 'y_4326', 'unprojected_lat'):
 					if colname not in headers:
 						self.lat_4326_col = colname
 						headers.append(colname)
 						break
 			if self.lon_4326_col is None:
@@ -1177,17 +1188,20 @@
 		cur.executemany("insert into mapdata values (%s)" % params, tbldata)
 		cur.close()
 		# Initial value for user-entered WHERE clause
 		self.whereclause = ""
 
 		# Determe data types for use in table statistics display and in column selection for plotting
 		self.data_types = None
-		self.data_types_queue = multiprocessing.Queue()
-		self.data_types_process = multiprocessing.Process(target=set_data_types, args=(headers, rows, self.data_types_queue))
-		self.data_types_process.start()
+		if os.name == 'posix':
+			self.data_types_queue = multiprocessing.Queue()
+			self.data_types_process = multiprocessing.Process(target=set_data_types, args=(headers, rows, self.data_types_queue))
+			self.data_types_process.start()
+		else:
+			self.data_types = set_data_types_core(headers, rows)
 
 		# Return frame and data table
 		return tframe, tdata
 	def remove_data(self):
 		while len(self.sel_map_markers) > 0:
 			self.sel_map_markers.pop().delete()
 		while len(self.loc_map_markers) > 0:
@@ -1401,15 +1415,15 @@
 		new_crs = crsdlg.get_crs()
 		if new_crs is not None:
 			if new_crs != self.crs:
 				try:
 					from pyproj import CRS, Transformer
 				except:
 					self.loading_dlg.hide_all()
-					fatal_error("The pyproj library is required to re-project spatial coordinates")
+					fatal_error("The pyproj library is required to re-project spatial coordinates", kwargs={})
 				try:
 					crs_proj = CRS(new_crs)
 				except:
 					warning("Invalid CRS (%s)" % new_crs, kwargs={})
 				else:
 					if self.lat_4326_col is None:
 						for colname in ('lat_4326', 'latitude_4326', 'y_4326', 'unprojected_lat'):
@@ -1546,16 +1560,16 @@
 			if mkr is not None:
 				if mkr != location_marker or clr != location_color or datamkr != use_data_marker or \
 						dataclr != use_data_color or column != self.label_col or ffam != label_font or \
 						fsize != label_size or fbold != label_bold or pos != label_position:
 							fontchanged = ffam != label_font or fsize != label_size or fbold != label_bold
 							location_marker = mkr
 							location_color = clr
-							use_data_marker = datamkr
-							use_data_color = dataclr
+							use_data_marker = datamkr == '1'
+							use_data_color = dataclr == '1'
 							self.label_col = column if column != '' else None
 							label_font = ffam
 							label_size = fsize
 							label_bold = fbold
 							label_position = pos
 							if fontchanged:
 								self.mapfont = self.makefont()
@@ -1652,50 +1666,55 @@
 		def show_data_types():
 			if self.data_types is None:
 				self.loading_dlg.display("Evaluating data types")
 				self.data_types = self.data_types_queue.get()
 				self.data_types_process.join()
 				self.data_types_process.close()
 				self.loading_dlg.hide()
-			dlg = MsgDialog("Data Types", "Data types, data completeness, and number of unique non-missing values for columns of the data table:", can_resize=True)
+			dlg = MsgDialog2("Data Types", "Data types, data completeness, and number of unique non-missing values for columns of the data table:", can_resize=True)
 			tframe, tdata = treeview_table(dlg.content_frame, self.data_types, ["Column", "Type", "Missing", "Unique"], "browse")
 			tframe.grid(row=0, column=0, sticky=tk.NSEW)
 			dlg.show()
 		def run_query():
 			dlg = QueryDialog(self.headers, self.db, self.whereclause)
 			whereclause, action = dlg.get_where()
 			if whereclause is not None:
+				self.whereclause = whereclause
 				sqlcmd = "SELECT treeviewid FROM mapdata WHERE %s" % whereclause
 				cur = self.db.cursor()
 				try:
 					result = cur.execute(sqlcmd)
 					id_list = [r[0] for r in result.fetchall()]
 				except:
 					cur.close()
 					warning("Invalid data selection expression: %s" % whereclause, kwargs={})
 				else:
 					cur.close()
-					self.whereclause = whereclause
 					# Enable multiselect
 					global multiselect
 					multiselect = "1"
 					self.multiselect_var.set("1")
 					self.tbl.configure(selectmode = tk.EXTENDED)
 					if action == "Replace":
-						# Remove any existing selections
 						self.unselect_map()
 						self.tbl.selection_set(list(id_list))
-					elif action == "Add":
-						# Add new selections
+					elif action == "Union":
 						all_selections = tuple(set(self.tbl.selection()) | set(id_list))
 						self.tbl.selection_set(all_selections)
-					else:
-						# Remove
+					elif action == "Intersection":
+						int_selections = tuple(set(self.tbl.selection()) & set(id_list))
+						self.tbl.selection_set(int_selections)
+					elif action == "Difference O-N":
+						# Old - New
 						diff_selections = tuple(set(self.tbl.selection()) - set(id_list))
 						self.tbl.selection_set(diff_selections)
+					else:
+						# New - Old
+						diff_selections = tuple(set(id_list) - set(self.tbl.selection()))
+						self.tbl.selection_set(diff_selections)
 					self.mark_map(None)
 					self.set_status()
 		def invert_selections():
 			selected = self.tbl.selection()
 			new_selections = []
 			for iid in self.tbl.get_children():
 				if not iid in selected:
@@ -1726,19 +1745,19 @@
 						msg = msg + "\n\n"
 				if len(config_files_user) > 0:
 					msg = msg + "Configuration files read after startup, in sequence:\n   %s" % "\n   ".join(config_files_user)
 			dlg = MsgDialog("Config files", msg)
 			dlg.show()
 		def show_about():
 			message="""
-               mapdata.py
+                     mapdata.py
 
-     version: %s, %s
-Copyright %s, R Dreas Nielsen
-         License: GNU GPL3""" % (version, vdate, copyright)
+           version: %s, %s
+      Copyright %s, R Dreas Nielsen
+               License: GNU GPL3""" % (version, vdate, copyright)
 			dlg = MsgDialog("About", message)
 			dlg.show()
 
 		file_menu.add_command(label="Open CSV", command = self.new_data_file, underline=5)
 		file_menu.add_command(label="Open spreadsheet", command = self.new_spreadsheet_file, underline=5)
 		file_menu.add_command(label="Open database", command = self.new_db_table, underline=5)
 		file_menu.add_command(label="Import symbol", command = import_symbol_file, underline=0)
@@ -2565,15 +2584,15 @@
 		prompt_frame = tk.Frame(self.dlg)
 		prompt_frame.grid(row=0, column=0, sticky=tk.NSEW, padx=(3,3), pady=(3,3))
 		prompt_frame.columnconfigure(0, weight=1)
 		query_frame = tk.Frame(self.dlg)
 		query_frame.grid(row=1, column=0, sticky=tk.NSEW, padx=(3,3), pady=(3,3))
 		query_frame.rowconfigure(0, weight=1)
 		query_frame.columnconfigure(0, weight=1)
-		query_frame.columnconfigure(1, weight=1)
+		query_frame.columnconfigure(1, weight=3)
 		sql_frame = tk.Frame(query_frame)
 		sql_frame.grid(row=0, column=0, sticky=tk.NSEW, padx=(3,3), pady=(3,3))
 		sql_frame.rowconfigure(0, weight=1)
 		sql_frame.columnconfigure(0, weight=1)
 		col_frame = tk.Frame(query_frame)
 		col_frame.grid(row=0, column=1, rowspan=2, sticky=tk.NS, padx=(3,3), pady=(3,3))
 		col_frame.rowconfigure(0, weight=1)
@@ -2585,16 +2604,18 @@
 		# Prompt
 		prompt_lbl = ttk.Label(prompt_frame, wraplength=300, justify=tk.LEFT, text="Enter an expression below to identify the data rows that you want to select.  The syntax of this expression should correspond to a SQL 'WHERE' clause.  Column names with non-alphanumeric characters should be double-quoted.  String literals should be single-quoted.  The '%' character is a wildcard.  Ctrl-Enter completes entry.")
 		prompt_lbl.grid(row=0, column=0, sticky=tk.EW, padx=(3,3))
 		def wrap_prompt(event):
 			prompt_lbl.configure(wraplength=event.width - 5)
 		prompt_lbl.bind("<Configure>", wrap_prompt)
 		# SQL entry
-		self.sql = None
+		self.sql = init_sql
 		self.sql_text = tk.Text(sql_frame, width=60, height=10)
+		if init_sql is not None and init_sql != "":
+			self.sql_text.insert(tk.END, init_sql)
 		self.sql_text.grid(row=0, column=0, sticky=tk.NSEW, padx=(3,0), pady=(3,3))
 		self.sql_text.bind("<KeyRelease>", self.check_enable)
 		sbar = tk.Scrollbar(sql_frame)
 		sbar.grid(row=0, column=1, sticky=tk.NS, padx=(0,3), pady=(3,3))
 		sbar.config(command=self.sql_text.yview)
 		self.sql_text.config(yscrollcommand = sbar.set)
 		# Column values
@@ -2629,15 +2650,15 @@
 			curs.close()
 			self.tv_tbl.bind("<Double-1>", colval_to_sql)
 		colsel.bind("<<ComboboxSelected>>", list_col_vals)
 		# Action selection
 		self.act_var = tk.StringVar(act_frame, "Replace")
 		act_lbl = ttk.Label(act_frame, text="Action:")
 		act_lbl.grid(row=0, column=0, sticky=tk.E, padx=(6,3))
-		act_sel = ttk.Combobox(act_frame, state="readonly", textvariable=self.act_var, values=["Replace", "Add", "Remove"], width=8)
+		act_sel = ttk.Combobox(act_frame, state="readonly", textvariable=self.act_var, values=["Replace", "Union", "Intersection", "Difference O-N", "Difference N-O"], width=15)
 		act_sel.grid(row=0, column=1, sticky=tk.W, padx=(3,6))
 		# Buttons
 		self.canceled = False
 		help_btn = ttk.Button(btn_frame, text="Help", command=self.do_help, underline=0)
 		help_btn.grid(row=0, column=0, sticky=tk.W, padx=(6,3))
 		self.dlg.bind("<Alt-h>", self.do_help)
 		self.ok_btn = ttk.Button(btn_frame, text="OK", command=self.do_select, underline=0)
@@ -2802,30 +2823,30 @@
 
 	def do_help(self, *args):
 		webbrowser.open("https://mapdata.osdn.io/dialogs.html#plot-dialog", new=2, autoraise=True)
 
 	def show_data(self, *args):
 		# Show data that have been collected for plotting, but not summarized as needed for a particular plot type.
 		if self.dataset is not None:
-			dlg = MsgDialog("Source Data", "Original data:")
+			dlg = MsgDialog2("Source Data", "Original data:")
 			variables = len(self.dataset)
 			rowwise_data = []
 			for i in range(len(self.dataset[0])):
 				row = []
 				for j in range(variables):
 					row.append(self.dataset[j][i])
 				rowwise_data.append(row)
 			tframe, tdata = treeview_table(dlg.content_frame, rowwise_data, self.data_labels)
 			tframe.grid(row=0, column=0, sticky=tk.NSEW)
 			dlg.show()
 
 	def show_plot_data(self, *args):
 		# Show data as summarized for a particular plot type.
 		if self.plot_data is not None:
-			dlg = MsgDialog("Data for Plotting", "Data to be plotted:")
+			dlg = MsgDialog2("Data for Plotting", "Data to be plotted:")
 			variables = len(self.plot_data)
 			rowwise_data = []
 			max_data_len = max([len(self.plot_data[i]) for i in range(variables)])
 			for i in range(max_data_len):
 				row = []
 				for j in range(variables):
 					try:
@@ -2869,15 +2890,15 @@
 		self.plot_data = None
 		self.plot_data_labels = None
 		self.data_btn["state"] = "disabled"
 		self.plot_data_btn["state"] = "disabled"
 		categ_columns = [c[0] for c in self.column_specs if c[1] in ("string", "boolean")]
 		categ_columns.sort()
 		# quant_columns includes date and timestamp columns
-		quant_columns = [c[0] for c in self.column_specs if c[1] not in ("string", "boolean")]
+		quant_columns = [c[0] for c in self.column_specs if c[1] in ("int", "float", "date", "timestamp", "timestamptz")]
 		quant_columns.sort()
 		numeric_columns = [c[0] for c in self.column_specs if c[1] in ("int", "float")]
 		numeric_columns.sort()
 		date_columns = [c[0] for c in self.column_specs if c[1] in ("date", "timestamp", "timestamptz")]
 		date_columns.sort()
 		self.x_var.set('')
 		self.y_var.set('')
@@ -3135,14 +3156,62 @@
 		if parent is not None:
 			self.dlg = tk.Toplevel(parent)
 		else:
 			self.dlg = tk.Toplevel()
 		if bgcolor is not None:
 			self.dlg.configure(bg=bgcolor)
 		self.dlg.title(title)
+		self.dlg.rowconfigure(0, weight=1)
+		self.dlg.columnconfigure(0, weight=2)
+		prompt_frame = tk.Frame(self.dlg)
+		prompt_frame.grid(row=0, column=0, sticky=tk.EW, padx=(6,6), pady=(6,6))
+		prompt_frame.rowconfigure(0, weight=1)
+		prompt_frame.columnconfigure(0, weight=2)
+		msg_lbl = ttk.Label(prompt_frame, wraplength=100, text=message)
+		msg_lbl.grid(row=0, column=0, sticky=tk.EW, padx=(6,6), pady=(3,3))
+		def wrap_msg(event):
+			msg_lbl.configure(wraplength=event.width - 5)
+		msg_lbl.bind("<Configure>", wrap_msg)
+		btn_frame = tk.Frame(self.dlg, borderwidth=3, relief=tk.RIDGE)
+		btn_frame.columnconfigure(0, weight=2)
+		btn_frame.grid(row=1, column=0, sticky=tk.EW, pady=(0,0))
+		btn_frame.columnconfigure(0, weight=1)
+		# Buttons
+		self.canceled = False
+		ok_btn = ttk.Button(btn_frame, text="Close", command=self.do_select, underline=0)
+		ok_btn.grid(row=0, column=0, sticky=tk.E, padx=(12,6))
+		self.dlg.bind("<Alt-c>", self.do_select)
+		self.dlg.bind("<Return>", self.do_select)
+		self.dlg.bind("<Escape>", self.do_select)
+		self.dlg.resizable(can_resize, can_resize)
+		self.dlg.minsize(width=300, height=50)
+		ok_btn.focus()
+	def do_select(self, *args):
+		self.dlg.destroy()
+	def show(self, grab=False):
+		if grab:
+			self.dlg.grab_set()
+		center_window(self.dlg)
+		raise_window(self.dlg)
+		self.dlg.attributes('-topmost', 'true')
+		self.dlg.attributes('-topmost', 'false')
+		self.dlg.wait_window(self.dlg)
+
+
+class MsgDialog2(object):
+	# With an extra content frame.
+	def __init__(self, title, message, parent=None, bgcolor=None, can_resize=True):
+		if parent is not None:
+			self.dlg = tk.Toplevel(parent)
+		else:
+			self.dlg = tk.Toplevel()
+		if bgcolor is not None:
+			self.dlg.configure(bg=bgcolor)
+		self.dlg.title(title)
+		#self.dlg.rowconfigure(0, weight=1)
 		self.dlg.columnconfigure(0, weight=1)
 		prompt_frame = tk.Frame(self.dlg)
 		prompt_frame.grid(row=0, column=0, sticky=tk.EW, padx=(6,6), pady=(6,6))
 		prompt_frame.columnconfigure(0, weight=1)
 		msg_lbl = ttk.Label(prompt_frame, wraplength=80, text=message)
 		msg_lbl.grid(row=0, column=0, sticky=tk.EW, padx=(6,6), pady=(3,3))
 		def wrap_msg(event):
@@ -3161,24 +3230,26 @@
 		self.canceled = False
 		ok_btn = ttk.Button(btn_frame, text="Close", command=self.do_select, underline=0)
 		ok_btn.grid(row=0, column=0, sticky=tk.E, padx=(12,6))
 		self.dlg.bind("<Alt-c>", self.do_select)
 		self.dlg.bind("<Return>", self.do_select)
 		self.dlg.bind("<Escape>", self.do_select)
 		self.dlg.resizable(can_resize, can_resize)
-		self.dlg.minsize(width=300, height=200)
+		self.dlg.minsize(width=300, height=50)
 		#self.dlg.maxsize(width=1600, height=1000)
 		ok_btn.focus()
 	def do_select(self, *args):
 		self.dlg.destroy()
-	def show(self):
-		self.dlg.grab_set()
+	def show(self, grab=False):
+		if grab:
+			self.dlg.grab_set()
 		center_window(self.dlg)
 		raise_window(self.dlg)
 		self.dlg.attributes('-topmost', 'true')
+		self.dlg.attributes('-topmost', 'false')
 		self.dlg.wait_window(self.dlg)
 
 
 class OneEntryDialog(object):
 	def __init__(self, parent, title, prompt):
 		self.dlg = tk.Toplevel(parent)
 		self.dlg.title(title)
@@ -3405,14 +3476,15 @@
 		self.canceled = True
 		self.dlg.destroy()
 	def select(self):
 		self.dlg.grab_set()
 		center_window(self.dlg)
 		raise_window(self.dlg)
 		self.dlg.resizable(False, False)
+		self.dlg.focus()
 		self.dlg.wait_window(self.dlg)
 		return self.rv
 
 
 class EncodedFile(object):
 	# A class providing an open method for an encoded file, allowing reading
 	# and writing using unicode, without explicit decoding or encoding.
@@ -4229,15 +4301,15 @@
 		try:
 			datestr = str(datestr)
 		except:
 			return None
 	dt = None
 	for i, f in enumerate(dt_fmts):
 		try:
-			dt = datetime.datetime.strptime(data, f)
+			dt = datetime.datetime.strptime(datestr, f)
 		except:
 			continue
 		break
 	if i:
 		del dt_fmts[i]
 		dt_fmts.appendleft(f)
 	return dt
@@ -4844,15 +4916,15 @@
 
 class SqlServerDatabase(Database):
 	def __init__(self, server_name, db_name, user_name, need_passwd=False, port=1433, encoding='latin1', password=None):
 		global pyodbc
 		try:
 			import pyodbc
 		except:
-			fatal_error(u"The pyodbc module is required.  See http://github.com/mkleehammer/pyodbc")
+			fatal_error(u"The pyodbc module is required.  See http://github.com/mkleehammer/pyodbc", kwargs={})
 		self.type = dbt_sqlserver
 		self.server_name = server_name
 		self.db_name = db_name
 		self.user = user_name
 		self.need_passwd = need_passwd
 		self.password = password
 		self.port = port if port else 1433
@@ -4917,15 +4989,15 @@
 
 class PostgresDatabase(Database):
 	def __init__(self, server_name, db_name, user_name, need_passwd=False, port=5432, new_db=False, encoding='UTF8', password=None):
 		global psycopg2
 		try:
 			import psycopg2
 		except:
-			fatal_error(u"The psycopg2 module is required to connect to PostgreSQL.")
+			fatal_error(u"The psycopg2 module is required to connect to PostgreSQL.", kwargs={})
 		self.type = dbt_postgres
 		self.server_name = server_name
 		self.db_name = db_name
 		self.user = user_name
 		self.need_passwd = need_passwd
 		self.password = password
 		self.port = port if port else 5432
@@ -5022,15 +5094,15 @@
 
 class OracleDatabase(Database):
 	def __init__(self, server_name, db_name, user_name, need_passwd=False, port=5432, encoding='UTF8', password=None):
 		global cx_Oracle
 		try:
 			import cx_Oracle
 		except:
-			fatal_error(u"The cx-Oracle module is required to connect to Oracle.   See https://pypi.org/project/cx-Oracle/")
+			fatal_error(u"The cx-Oracle module is required to connect to Oracle.   See https://pypi.org/project/cx-Oracle/", kwargs={})
 		self.type = dbt_oracle
 		self.server_name = server_name
 		self.db_name = db_name
 		self.user = user_name
 		self.need_passwd = need_passwd
 		self.password = password
 		self.port = port if port else 1521
@@ -5147,18 +5219,14 @@
 	def paramsubs(self, paramcount):
 		return ",".join(":"+str(d) for d in range(1, paramcount+1))
 
 
 class SQLiteDatabase(Database):
 	def __init__(self, SQLite_fn):
 		global sqlite3
-		try:
-			import sqlite3
-		except:
-			fatal_error(u"The sqlite3 module is required.")
 		self.type = dbt_sqlite
 		self.server_name = None
 		self.db_name = SQLite_fn
 		self.user = None
 		self.need_passwd = False
 		self.encoding = 'UTF-8'
 		self.encode_commands = False
@@ -5231,15 +5299,15 @@
 
 class DuckDBDatabase(Database):
 	def __init__(self, DuckDB_fn):
 		global duckdb
 		try:
 			import duckdb
 		except:
-			fatal_error(u"The duckdb module is required.")
+			fatal_error(u"The duckdb module is required.", kwargs={})
 		self.type = dbt_duckdb
 		self.server_name = None
 		self.db_name = DuckDB_fn
 		self.catalog_name = os.path.splitext(DuckDB_fn)[0]
 		self.user = None
 		self.need_passwd = False
 		self.encoding = 'UTF-8'
@@ -5287,15 +5355,15 @@
 
 class MySQLDatabase(Database):
 	def __init__(self, server_name, db_name, user_name, need_passwd=False, port=3306, encoding='latin1', password=None):
 		global mysql_lib
 		try:
 			import pymysql as mysql_lib
 		except:
-			fatal_error(u"The pymysql module is required to connect to MySQL.   See https://pypi.python.org/pypi/PyMySQL")
+			fatal_error(u"The pymysql module is required to connect to MySQL.   See https://pypi.python.org/pypi/PyMySQL", kwargs={})
 		self.type = dbt_mysql
 		self.server_name = str(server_name)
 		self.db_name = str(db_name)
 		self.user = str(user_name)
 		self.need_passwd = need_passwd
 		self.password = password
 		self.port = 3306 if not port else port
@@ -5339,15 +5407,15 @@
 
 class FirebirdDatabase(Database):
 	def __init__(self, server_name, db_name, user_name, need_passwd=False, port=3050, encoding='latin1', password=None):
 		global firebird_lib
 		try:
 			import fdb as firebird_lib
 		except:
-			fatal_error(u"The fdb module is required to connect to MySQL.   See https://pypi.python.org/pypi/fdb/")
+			fatal_error(u"The fdb module is required to connect to MySQL.   See https://pypi.python.org/pypi/fdb/", kwargs={})
 		self.type = dbt_firebird
 		self.server_name = str(server_name)
 		self.db_name = str(db_name)
 		self.user = str(user_name)
 		self.need_passwd = need_passwd
 		self.password = password
 		self.port = 3050 if not port else port
@@ -6072,15 +6140,15 @@
 		if self.cmdptr > len(self.cmdlist) - 1:
 			return None
 		return self.cmdlist[self.cmdptr]
 	def check_iflevels(self):
 		if_excess = len(if_stack.if_levels) - self.init_if_level
 		if if_excess > 0:
 			sources = if_stack.script_lines(if_excess)
-			src_msg = ", ".join(["%s line %s" % src for src in sources])
+			src_msg = ", ".join(["input line %s" % src for src in sources])
 			raise ErrInfo(type="error", other_msg="IF level mismatch at beginning and end of script; origin at or after: %s." % src_msg)
 	def run_and_increment(self):
 		global last_command
 		global loop_nest_level
 		cmditem = self.cmdlist[self.cmdptr]
 		if compiling_loop:
 			# Don't run this command, but save it or complete the loop and add the loop's set of commands to the stack.
@@ -7712,18 +7780,19 @@
 	global cmds_run
 	global script_errors
 	dbs.add('mapdata_connection', db)
 	subvars.add_substitution("$CURRENT_DBMS", db.type.dbms_id)
 	subvars.add_substitution("$CURRENT_DATABASE", db.name())
 	process_sql(sql_text.splitlines())
 	if len(script_errors) > 0:
-		dlg = MsgDialog("Warnings", "The following unexpected conditions were encountered while parsing the SQL script.", can_resize=True)
+		dlg = MsgDialog2("Warnings", "The following unexpected conditions were encountered while parsing the SQL script.", can_resize=True)
 		hdrs = ["Warning message", "Line no"]
 		tframe, tdata = treeview_table(dlg.content_frame, script_errors, hdrs)
 		tframe.grid(row=0, column=0, sticky=tk.NSEW)
+		dlg.show(grab=True)
 	script_errors = []
 	while len(commandliststack) > 0:
 		current_cmds = commandliststack[-1]
 		set_system_vars()
 		try:
 			current_cmds.run_next()
 		except StopIteration:
@@ -7732,18 +7801,19 @@
 			commandliststack.pop()
 			raise
 		except:
 			commandliststack.pop()
 			raise ErrInfo(type="exception", exception_msg=exception_desc())
 		cmds_run += 1
 	if len(script_errors) > 0:
-		dlg = MsgDialog("Warnings", "The following unexpected conditions were encountered while running the SQL script.", can_resize=True)
+		dlg = MsgDialog2("Warnings", "The following unexpected conditions were encountered while running the SQL script.", can_resize=True)
 		hdrs = ["Warning message", "Line no"]
 		tframe, tdata = treeview_table(dlg.content_frame, script_errors, hdrs)
 		tframe.grid(row=0, column=0, sticky=tk.NSEW)
+		dlg.show(grab=True)
 
 
 #***************************************************************************************************
 #***************************  End of SQL Scripting Extensions  *************************************
 #***************************************************************************************************
 
 
@@ -8545,15 +8615,15 @@
 		fn = lat_col = lon_col = id_col = sym_col = col_col = crs = sheet = msg = headers = rows = imagefile = None
 		imagewait = 12
 	else:
 		fn = args.file
 		if not os.path.exists(fn):
 			win = tk.Tk()
 			win.withdraw()
-			fatal_error("File %s does not exist" % fn)
+			fatal_error("File %s does not exist" % fn, kwargs={})
 		sheet = args.sheet
 		lat_col = args.lat
 		lon_col = args.lon
 		id_col = args.id
 		sym_col = args.symbol
 		col_col = args.color
 		crs = args.projection
```

### Comparing `mapdata-2.8.3/mapdata.egg-info/PKG-INFO` & `mapdata-2.8.6/mapdata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapdata
-Version: 2.8.3
+Version: 2.8.6
 Summary: An interactive map and table explorer for geographic coordinates in a spreadsheet, CSV file, or database
 Home-page: https://osdn.net/project/mapdata/
 Author: Dreas Nielsen
 Author-email: dreas.nielsen@gmail.com
 License: GPL
 Keywords: Map,Locations,CRS,CSV,Spreadsheet,Database,PNG,JPG,Postscript
 Platform: UNKNOWN
```

### Comparing `mapdata-2.8.3/setup.py` & `mapdata-2.8.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 import io
 
 with io.open('README.md', encoding='utf-8') as f:
 	long_description = f.read()
 
 setuptools.setup(name='mapdata',
-	version='2.8.3',
+	version='2.8.6',
 	description="An interactive map and table explorer for geographic coordinates in a spreadsheet, CSV file, or database",
 	author='Dreas Nielsen',
 	author_email='dreas.nielsen@gmail.com',
     url='https://osdn.net/project/mapdata/',
 	scripts=['mapdata/mapdata.py'],
     license='GPL',
 	requires=['tkintermapview', 'pyproj', 'odfpy', 'openpyxl', 'xlrd', 'matplotlib'],
```

