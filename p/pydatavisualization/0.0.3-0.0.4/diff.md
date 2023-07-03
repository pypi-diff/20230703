# Comparing `tmp/pydatavisualization-0.0.3.tar.gz` & `tmp/pydatavisualization-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydatavisualization-0.0.3.tar", last modified: Mon Jun 26 15:28:40 2023, max compression
+gzip compressed data, was "pydatavisualization-0.0.4.tar", last modified: Mon Jul  3 12:17:47 2023, max compression
```

## Comparing `pydatavisualization-0.0.3.tar` & `pydatavisualization-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 15:28:40.920090 pydatavisualization-0.0.3/
--rw-rw-rw-   0        0        0     1088 2023-06-19 08:30:04.000000 pydatavisualization-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     1278 2023-06-26 15:28:40.920090 pydatavisualization-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      755 2023-06-26 15:26:20.000000 pydatavisualization-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 15:28:40.920090 pydatavisualization-0.0.3/descriptive/
--rw-rw-rw-   0        0        0        2 2023-06-26 14:41:05.000000 pydatavisualization-0.0.3/descriptive/__init__.py
--rw-rw-rw-   0        0        0    49657 2023-06-26 09:15:43.000000 pydatavisualization-0.0.3/descriptive/pyeda.py
-drwxrwxrwx   0        0        0        0 2023-06-26 15:28:40.920090 pydatavisualization-0.0.3/pydatavisualization.egg-info/
--rw-rw-rw-   0        0        0     1278 2023-06-26 15:28:40.000000 pydatavisualization-0.0.3/pydatavisualization.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-06-26 15:28:40.000000 pydatavisualization-0.0.3/pydatavisualization.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 15:28:40.000000 pydatavisualization-0.0.3/pydatavisualization.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-06-26 15:28:40.000000 pydatavisualization-0.0.3/pydatavisualization.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-26 15:28:40.000000 pydatavisualization-0.0.3/pydatavisualization.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-26 15:28:40.935705 pydatavisualization-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1109 2023-06-26 14:41:05.000000 pydatavisualization-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 12:17:47.880552 pydatavisualization-0.0.4/
+-rw-rw-rw-   0        0        0     1088 2023-06-19 08:30:04.000000 pydatavisualization-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1278 2023-07-03 12:17:47.879550 pydatavisualization-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      755 2023-06-26 15:26:20.000000 pydatavisualization-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 12:17:47.870908 pydatavisualization-0.0.4/descriptive/
+-rw-rw-rw-   0        0        0        2 2023-07-03 10:52:24.000000 pydatavisualization-0.0.4/descriptive/__init__.py
+-rw-rw-rw-   0        0        0    51071 2023-07-03 10:35:19.000000 pydatavisualization-0.0.4/descriptive/pyeda.py
+drwxrwxrwx   0        0        0        0 2023-07-03 12:17:47.877546 pydatavisualization-0.0.4/pydatavisualization.egg-info/
+-rw-rw-rw-   0        0        0     1278 2023-07-03 12:17:47.000000 pydatavisualization-0.0.4/pydatavisualization.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-07-03 12:17:47.000000 pydatavisualization-0.0.4/pydatavisualization.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 12:17:47.000000 pydatavisualization-0.0.4/pydatavisualization.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-03 12:17:47.000000 pydatavisualization-0.0.4/pydatavisualization.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-03 12:17:47.000000 pydatavisualization-0.0.4/pydatavisualization.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 12:17:47.880552 pydatavisualization-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1098 2023-07-03 10:52:03.000000 pydatavisualization-0.0.4/setup.py
```

### Comparing `pydatavisualization-0.0.3/LICENSE` & `pydatavisualization-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pydatavisualization-0.0.3/PKG-INFO` & `pydatavisualization-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydatavisualization
-Version: 0.0.3
+Version: 0.0.4
 Summary: Data Visualization Functions
 Author: Tamer Samara
 Author-email: tamer.samara@gmail.com
 License: MIT
 Keywords: python,data+science,eda,data+preprocessing,data+analysis,machine+learning
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `pydatavisualization-0.0.3/README.md` & `pydatavisualization-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pydatavisualization-0.0.3/descriptive/pyeda.py` & `pydatavisualization-0.0.4/descriptive/pyeda.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 import matplotlib.pyplot as plt
 import seaborn as sns
 from statsmodels.graphics.gofplots import qqplot
 import numpy as np
 import warnings
 
 __all__ = ["import_dataset", "read_dataset", "display_dataset_info", "display_dataset_detail", "display_summary_data",
-           "display_columns", "select_numeric_variables", "select_categorical_variables",
+           "display_column_types", "select_numeric_variables", "select_categorical_variables",
            "visualize_distribution_of_numeric_col", "visualize_distribution_of_categorical_col", "visualize_boxplot",
            "visualize_frequency_distribution_horizontally", "visualize_frequency_distribution",
            "visualize_basic_scatter_plot", "visualize_advanced_scatter_plot", "visualize_stack_bar",
-           "visualize_advanced_stack_bar", "visualize_pie_chart", "pivot_tabel", "visualize_point_plot",
+           "vis_advanced_stack_bar", "visualize_pie_chart", "pivot_tabel", "visualize_point_plot",
            "visualize_average_bar_plot", "visualize_advanced_bar_plot", "visualize_barplot_for_categorical_col",
-           "visualize_heatmap", "visualize_linear_regression", "visualize_causation", "save_data_to_csv_file",
+           "vis_heatmap", "visualize_linear_regression", "visualize_causation", "save_data_to_csv_file",
            "visualize_time_relationship", "visualize_time_relationship_by_categorical_variable",
-           "visualize_highest_percentage_datapoints", "visualize_lowest_percentage_datapoints",
-           "visualize_top_ten_values", "visualize_top_highest_average"]
+           "vis_highest_percentage_datapoints", "vis_lowest_percentage_datapoints",
+           "vis_top_ten_values", "vis_top_highest_average", "vis_pie_chart"]
 
 # --- Create List of Color Palettes ---
 red_grad = ['#FF0000', '#BF0000', '#800000', '#400000', '#000000']
 pink_grad = ['#8A0030', '#BA1141', '#FF5C8A', '#FF99B9', '#FFDEEB']
 purple_grad = ['#4C0028', '#7F0043', '#8E004C', '#A80059', '#C10067']
 color_mix = ['#F38BB2', '#FFB9CF', '#FFD7D7', '#F17881', '#E7525B', "#FFCDCD", "#FFBCBC", "#FF9090"]
 black_grad = ['#100C07', 'dimgray', '#6D6A6A', '#9B9A9C', '#CAC9CD']
@@ -29,31 +29,32 @@
 #             ----------------  Libraries Settings  ---------------
 
 pd.set_option("display.max_columns", None)
 sns.set_style(style="whitegrid")
 plt.rcParams["figure.dpi"] = 100
 warnings.filterwarnings("ignore")
 
+
 #             ----------------  EDA Methods  ---------------
 
 
 def show_values(axs, orient="v", space=.01):
     def _single(axes2):
         if orient == "v":
             for p in axes2.patches:
                 _x = p.get_x() + p.get_width() / 2
                 _y = p.get_y() + p.get_height() + (p.get_height()*0.01)
-                value = '{:.3f}'.format(p.get_height())
-                axes2.text(_x, _y, value, ha="center")
+                value = '{:.2f}'.format(p.get_height())
+                axes2.text(_x, _y, value, ha="center", color=colors[0])
         elif orient == "h":
             for p in axes2.patches:
                 _x = p.get_x() + p.get_width() + float(space)
                 _y = p.get_y() + p.get_height() - (p.get_height()*0.5)
-                value = '{:.3f}'.format(p.get_width())
-                axes2.text(_x, _y, value, ha="left")
+                value = '{:.2f}'.format(p.get_width())
+                axes2.text(_x, _y, value, ha="left", color=colors[0])
 
     if isinstance(axs, np.ndarray):
         for idx, ax in np.ndenumerate(axs):
             _single(ax)
     else:
         _single(axs)
 
@@ -71,26 +72,26 @@
         df = pd.read_csv(file_name, parse_dates=True, header=0)
         return df
     except FileNotFoundError:
         print("No such File, upload your dataset CSV file to the project")
 
 
 def read_dataset(data):
-    """"
+    """
     Reading data from a variable.
 
     :param data: variable
 
     :return: data
 
     """
     return data.head()
 
 
-def display_dataset_info(data):
+def display_dataset_info(data) -> None:
     """
     Print dataset info.
 
     :param data: variable
 
     :return: total rows and columns
     """
@@ -126,27 +127,27 @@
     
     - Null Percentage.
     
     - DataType.
     
     :param data: variable
     
-    :return: Summarize columns dataframe
+    :return: Summarize columns
     
     """
     summary_tabel = pd.DataFrame({"Unique": data.nunique(),
                                   "Null": data.isna().sum(),
                                   "NullPercent": data.isna().sum() / len(data),
                                   "Types": data.dtypes.values})
     print(summary_tabel)
 
 
-def display_columns(data):
+def display_column_types(data):
     """
-    Separate numerical features and categorical features.
+    Separate numerical columns and categorical columns.
     
     :param data: variable
     
     :return: list of numerical and categorical feature names
     
     """
     numeric_variable_lst = data.select_dtypes(include=["int64", "float64"]).columns.tolist()
@@ -175,15 +176,15 @@
     
     :return: all categorical features in a dataset
     """
     categorical_variable_lst = data.select_dtypes(include=["object", "category"])
     return list(categorical_variable_lst)
 
 
-def visualize_distribution_of_numeric_col(data_frame, column_name: str, bins: int):
+def visualize_distribution_of_numeric_col(data_frame, column_name: str, bins: int) -> None:
     """
     Visualize numerical column.
 
     :param data_frame: variable
     
     :param column_name: str
 
@@ -253,71 +254,69 @@
     fig = plt.figure(figsize=(10, 6))
     fig.suptitle(f"{column_name.title()} Distribution", fontweight="heavy", x=0.069, y=0.98, ha="left", fontsize="16",
                  fontfamily="sans-serif",
                  color=black_grad[0])
     # Pie Chart
     plt.subplot(1, 2, 1)
     plt.title("Pie Chart", fontweight="bold", fontsize=14, fontfamily="sans-serif", color=colors[0])
-    plt.pie(data_frame[column_name].value_counts(), colors=pastel, pctdistance=0.7, autopct="%.2f%%",
-            wedgeprops=dict(alpha=0.8, edgecolor=black_grad[1]), textprops={"fontsize": 12})
-    centre = plt.Circle((0, 0), 0.45, fc="white", edgecolor=black_grad[1])
+    labels = data_frame[column_name].unique()
+    plt.pie(data_frame[column_name].value_counts(), colors=pastel, pctdistance=0.7, autopct="%.2f%%", labels=labels,
+            wedgeprops=dict(alpha=0.8, edgecolor=colors[0]), textprops={"fontsize": 12}, startangle=90)
+    centre = plt.Circle((0, 0), 0.45, fc="white", edgecolor=colors[0])
     plt.gcf().gca().add_artist(centre)
 
     # Histogram
     plt.subplot(1, 2, 2)
     plt.title("Histogram", fontweight="bold", fontsize=14, fontfamily="sans-serif", color=colors[0])
     ax = sns.countplot(x=column_name, data=data_frame, palette=pastel, order=order, edgecolor=black_grad[2],
                        alpha=0.85)
-    for rect in ax.patches:
-        ax.text(rect.get_x() + rect.get_width()/2, rect.get_height()+4.25, rect.get_height(),
-                horizontalalignment="center", fontsize=10, bbox=dict(facecolor="none", edgecolor=black_grad[0],
-                                                                     linewidth=0.25, boxstyle="round"))
-
+    show_values(ax, "v")
     plt.xlabel(column_name.capitalize(), fontweight="bold", fontsize=11, fontfamily="sans-serif",
                color=black_grad[1])
     plt.ylabel("Total", fontweight="bold", fontsize=11, fontfamily="sans-serif", color=black_grad[1])
     plt.xticks(rotation=45)
     plt.tight_layout(rect=[0, 0.04, 1, 1.025])
-    plt.grid(axis="y", alpha=0.4)
+    plt.grid(axis="y", alpha=0)
     plt.grid(axis="x", alpha=0)
+    ax.set(frame_on=False)
     plt.show()
 
 
-def visualize_boxplot(data_frame, numeric_column: str, categorical_column: str,
+def visualize_boxplot(data, numeric_column: str, categorical_column: str,
                       subtitle: str = "Explain ur data viz by subtitle"):
     """
     Visualize numeric column medians by a categorical column.
 
     Add new subtitle content to the third parameter.
 
-    :param data_frame: variable
+    :param data: variable
 
     :param numeric_column: str
 
     :param categorical_column: str
 
     :param subtitle: str
 
     :return: boxplot chart
 
     """
-    if not data_frame[numeric_column].dtype in ["int64", "float64"]:
+    if not data[numeric_column].dtype in ["int64", "float64"]:
         raise TypeError(f"{numeric_column} Is not a Numeric Column. Only Numeric Column is Allowed")
     fig = plt.figure(figsize=(10, 6))
     fig.suptitle(f"Distribution of {numeric_column.title()} Grouped By {categorical_column.title()}",
                  fontweight="heavy", x=0.060, y=0.98, ha="left", fontsize="16",
                  fontfamily="sans-serif",
                  color=black_grad[0])
     plt.title(subtitle.capitalize(),
               fontweight="heavy", fontsize="12", fontfamily="sans-serif", color=colors[0], loc="left", pad=12)
 
-    medians = data_frame.groupby([categorical_column])[numeric_column].median().round(3).sort_values()
+    medians = data.groupby([categorical_column])[numeric_column].median().round(3).sort_values()
 
-    vertical_offset = data_frame[numeric_column].median() * 0.05
-    box_plot = sns.boxplot(data=data_frame, x=categorical_column, y=numeric_column,
+    vertical_offset = data[numeric_column].median() * 0.05
+    box_plot = sns.boxplot(data=data, x=categorical_column, y=numeric_column,
                            medianprops={"color": "coral"}, order=medians.index, palette=color_mix[0:8])
 
     for xtick in box_plot.get_xticks():
         box_plot.text(xtick, medians[xtick] + vertical_offset, medians[xtick], horizontalalignment="center",
                       size=12, color=colors[1], weight="bold")
 
     plt.tight_layout(rect=[0, 0.04, 1, 1.025])
@@ -336,17 +335,17 @@
 
     Add new subtitle content to the third parameter.
 
     :param data: variable
 
     :param first_column: str
 
-    :param target_column:str
+    :param target_column: str
 
-    :param subtitle:str
+    :param subtitle: str
 
     :return: Horizontal bar chart
 
     """
     _, ax = plt.subplots(figsize=(11.5, 7))
     plt.suptitle(f"{first_column.title()} Distribution Based On {target_column.title()}",
                  fontweight="heavy", x=0.069, y=0.98, ha="left", fontsize="16",
@@ -413,111 +412,120 @@
     ax.set(frame_on=False)
     plt.xticks(rotation=45)
     plt.xlabel(first_column, fontweight="bold", fontsize=11, fontfamily="sans-serif", color=black_grad[1])
     plt.tight_layout(rect=[0, 0.04, 1, 1.025])
     plt.show()
 
 
-def visualize_basic_scatter_plot(data, first_column: str, second_column: str):
+def visualize_basic_scatter_plot(data, first_column: str, second_column: str,
+                                 subtitle: str = "Explain ur data viz by subtitle"):
     """
     Visualize relationship between two numeric column.
     
     :param data: variable
     
     :param first_column: str
     
     :param second_column: str
+
+    :param subtitle: str
     
     :return: Basic scatter plot
     
     """
 
     plt.figure(figsize=(10, 6))
     plt.suptitle(f"Relationship Between {second_column.title()} and {first_column.title()} Column",
                  fontweight="heavy", x=0.059, y=0.98, ha="left", fontsize="16",
                  fontfamily="sans-serif",
                  color=black_grad[0]
                  )
-    plt.title("explain ur data viz by subtitle",
+    plt.title(subtitle,
               fontweight="heavy", fontsize="12", fontfamily="sans-serif", color=colors[0], loc="left", pad=10)
     ax = sns.scatterplot(data=data, x=first_column, y=second_column, legend="full")
 
     plt.xlabel(first_column, fontweight="bold", fontsize=11, fontfamily="sans-serif", color=black_grad[1])
     plt.ylabel(second_column, fontweight="bold", fontsize=11, fontfamily="sans-serif", color=black_grad[1])
     plt.ticklabel_format(style="plain", axis="both")
     plt.grid(axis="both", alpha=0.4, lw=0.5)
     ax.set(frame_on=False)
     plt.tight_layout(rect=[0, 0.04, 1, 1.025])
     plt.show()
 
 
-def visualize_advanced_scatter_plot(data, first_column: str, second_column: str, by_third_column: str):
+def visualize_advanced_scatter_plot(data, first_numeric: str, second_numeric: str, categorical_col: str,
+                                    subtitle: str = "Explain ur data viz by subtitle"):
     """
     Vis the relationship between two numeric variable's by a third categorical variable,
     to dictate the color of data point's.
 
-    :param: data: Data frame variable
 
-    :param: first_column:str
+    :param data: Data frame variable
 
-    :param: second_column: str
+    :param first_numeric: str
 
-    :param: by_third_column :str
+    :param second_numeric: str
+
+    :param categorical_col: str
+
+    :param subtitle: str
 
     :return: Advanced scatter plot
     """
+
     plt.figure(figsize=(10, 6))
-    plt.suptitle(f"Relationship Between {second_column.title()} per {first_column.title()} as "
-                 f"{by_third_column.title()}",
+    plt.suptitle(f"Relationship Between {second_numeric.title()} per {first_numeric.title()} as "
+                 f"{categorical_col.title()}",
                  fontweight="heavy", x=0.058, y=0.98, ha="left", fontsize="16",
                  fontfamily="sans-serif",
                  color=black_grad[0]
                  )
-    plt.title("explain ur data viz by subtitle",
+    plt.title(subtitle,
               fontweight="heavy", fontsize=12, fontfamily="sans-serif", color=colors[0], loc="left", pad=10)
 
-    ax = sns.scatterplot(data=data, x=first_column, y=second_column, hue=by_third_column, palette=pastel,
+    ax = sns.scatterplot(data=data, x=first_numeric, y=second_numeric, hue=categorical_col, palette=pastel,
                          legend="full")
 
-    plt.xlabel(first_column, fontweight="bold", fontsize=11, fontfamily="sans-serif", color=black_grad[1])
-    plt.ylabel(second_column, fontweight="bold", fontsize=11, fontfamily="sans-serif", color=black_grad[1])
+    plt.xlabel(first_numeric, fontweight="bold", fontsize=11, fontfamily="sans-serif", color=black_grad[1])
+    plt.ylabel(second_numeric, fontweight="bold", fontsize=11, fontfamily="sans-serif", color=black_grad[1])
     plt.ticklabel_format(style="plain", axis="both")
     plt.grid(axis="both", alpha=0.4, lw=0.5)
-    ax.legend(title=by_third_column.title(), bbox_to_anchor=(0.98, 0.90), loc="upper left", frameon=True)
+    ax.legend(title=categorical_col.title(), bbox_to_anchor=(0.98, 0.90), loc="upper left", frameon=True)
     ax.set(frame_on=False)
+    plt.grid(axis="x", alpha=0)
     plt.tight_layout(rect=[0, 0.04, 1, 1.025])
     plt.show()
 
 
-def visualize_stack_bar(data, first_column: str, second_column: str,
+def visualize_stack_bar(data, first_categorical: str, second_categorical: str,
                         subtitle: str = "explain ur data viz by subtitle"):
     """
     Visualize percentage relationship using two categorical variables.
 
     Add new subtitle content to the third parameter.
 
-    :param: data: Data fame variable
+    :param data: Data fame variable
 
-    :param: first_column: str
+    :param first_categorical: str
 
-    :param: second_column: str
+    :param second_categorical: str
 
-    :param: subtitle: str
+    :param subtitle: str
 
     :return: stacked bar plot
 
     """
     df = (data
-          .groupby(first_column)[second_column]
+          .groupby(first_categorical)[second_categorical]
           .value_counts(normalize=True)
           .mul(100)
           .round(2)
           .unstack())
     fig, ax = plt.subplots(figsize=(12, 6))
-    plt.suptitle(f"Percentage of {second_column.title()} by {first_column.title()}",
+    plt.suptitle(f"Percentage of {second_categorical.title()} by {first_categorical.title()}",
                  fontweight="heavy", x=0.059, y=0.98, ha="left", fontsize="16",
                  fontfamily="sans-serif",
                  color=black_grad[0]
                  )
     plt.title(subtitle.capitalize(),
               fontweight="heavy", fontsize=12, fontfamily="sans-serif", color=colors[0], loc="left", pad=15)
     # Plot
@@ -532,49 +540,50 @@
                      color=colors[0],
                      size=12)  # add a container object "c" as first argument
     # Removing spines
     for s in ["top", "right"]:
         ax.spines[s].set_visible(False)
 
     # Adding tick and axes labels
-    ax.legend(title=second_column.title(), bbox_to_anchor=(0.98, 0.90), loc="upper left")
+    ax.legend(title=second_categorical.title(), bbox_to_anchor=(0.98, 0.90), loc="upper left")
     ax.grid(axis="both", alpha=0.4, lw=0.5)
     ax.set(frame_on=False, xlabel=None)
     ax.tick_params(labelsize=12, labelrotation=0)
     ax.set_ylabel("Percentage", size=14, color=colors[0])
     plt.tight_layout(rect=[0, 0.04, 1, 1.025])
     plt.show()
 
 
-def visualize_advanced_stack_bar(data, first_column: str, second_column: str, third_column: str,
-                                 subtitle: str = "explain ur data viz by subtitle"):
+def vis_advanced_stack_bar(data, first_categorical: str, second_categorical: str, third_categorical: str,
+                           subtitle: str = "explain ur data viz by subtitle"):
 
     """
     Visualize percentage relationship using three categorical variables.
 
     Add new subtitle content to the third parameter.
 
     :param data: variable
 
-    :param first_column: str
+    :param first_categorical: str
 
-    :param second_column: str
+    :param second_categorical: str
 
-    :param third_column: str
+    :param third_categorical: str
 
     :param subtitle: str
 
     :return: stacked bar plot
 
     """
-    df = data.groupby([first_column, second_column])[third_column].value_counts(normalize=True)\
+    df = data.groupby([first_categorical, second_categorical])[third_categorical].value_counts(normalize=True)\
         .mul(100).round(2).unstack()
     _, ax = plt.subplots(figsize=(11, 6))
-    plt.suptitle(f"Percentage of {third_column.title()} by {first_column.title()} and {second_column.title()}",
-                 fontweight="heavy", x=0.26, y=0.98,  fontsize="16",
+    plt.suptitle(f"Percentage of {third_categorical.title()} by {first_categorical.title()} and "
+                 f"{second_categorical.title()}",
+                 fontweight="heavy", x=0.26, y=0.98, fontsize="16",
                  fontfamily="sans-serif",
                  color=black_grad[0]
                  )
     plt.title(subtitle.capitalize(),
               fontweight="heavy", fontsize="12", fontfamily="sans-serif", color=black_grad[1], loc="left", pad=15)
     df.plot(kind="bar", stacked=True, width=0.4, ax=ax, color=pastel)
 
@@ -586,43 +595,43 @@
                      labels=labels,
                      color=colors[0],
                      size=10)  # add a container object "c" as first argument
     # Removing spines
     for s in ["top", "right"]:
         ax.spines[s].set_visible(False)
 
-    ax.legend(title=third_column.title(), bbox_to_anchor=(0.98, 0.90), loc="upper left", frameon=True)
+    ax.legend(title=third_categorical.title(), bbox_to_anchor=(0.98, 0.90), loc="upper left", frameon=True)
     plt.grid(axis="both", alpha=0.4, lw=0.5)
     ax.set(frame_on=False, xlabel=None)
     plt.xticks(rotation=45)
     plt.tight_layout(rect=[0, 0.04, 1, 1.025])
     plt.show()
 
 
 def visualize_pie_chart(data, categorical_col: str, numerical_col: str,
                         subtitle: str = "explain ur data viz by subtitle"):
     """
     Visualize pie chart.
 
     Add new subtitle content to the third parameter.
 
-    :param data:
-    :param categorical_col:
-    :param numerical_col:
-    :param subtitle:
+    :param data: variable
+    :param categorical_col: str
+    :param numerical_col: str
+    :param subtitle: str
     :return: pie chart
     """
     _, ax = plt.subplots(figsize=(10, 6))
     plt.suptitle(f"Comparison {numerical_col.title()} per {categorical_col.title()}",
-                 fontweight="heavy", x=0.15, y=0.99, fontsize="16", ha="left",
+                 fontweight="heavy", x=0.24, y=0.99, fontsize="16", ha="left",
                  fontfamily="sans-serif",
                  color=black_grad[0]
                  )
     plt.title(subtitle.capitalize(),
-              fontweight="heavy", fontsize="12", fontfamily="sans-serif", color="dimgray", loc="left")
+              fontweight="heavy", fontsize="12", fontfamily="sans-serif", color="dimgray", loc="left", pad=10)
     labels = data[categorical_col].unique()
     df = data.groupby(categorical_col)[numerical_col].sum()
     plt.pie(df, colors=pastel, pctdistance=0.7, autopct="%.2f%%", labels=labels,
             wedgeprops=dict(alpha=0.8, edgecolor="floralwhite"), textprops={"fontsize": 12})
     centre = plt.Circle((0, 0), 0.45, fc="white", edgecolor="aliceblue")
     plt.gcf().gca().add_artist(centre)
     ax.legend(title=categorical_col.title(), bbox_to_anchor=(1.2, 0.90), loc="upper left", frameon=True, shadow=True)
@@ -713,66 +722,66 @@
               fontweight="heavy", fontsize=12, fontfamily="sans-serif", color=colors[0], loc="left", pad=15)
     order = data.groupby([categorical_col])[numerical_col].mean().round().sort_values(ascending=False).index
     ax = sns.barplot(data=data, y=categorical_col, x=numerical_col, ci=None, palette=pastel, order=order)
 
     show_values(ax, "h", space=0)
 
     plt.xlabel(f"Average", fontweight="bold", fontsize=11, fontfamily="sans-serif", color=black_grad[1])
-    plt.ylabel(f"{categorical_col}", fontweight="bold", fontsize=11, fontfamily="sans-serif",
+    plt.ylabel(f"{categorical_col.title()}", fontweight="bold", fontsize=11, fontfamily="sans-serif",
                color=black_grad[1])
-    plt.grid(axis="x", alpha=0.4)
+    plt.grid(axis="x", alpha=0)
     plt.tight_layout(rect=[0, 0.04, 1, 1.025])
     ax.set(frame_on=False)
     plt.show()
 
 
-def visualize_advanced_bar_plot(data, categorical_column: str, numerical_column: str, second_categorical_column: str,
+def visualize_advanced_bar_plot(data, categorical_col: str, numerical_col: str, second_categorical_col: str,
                                 subtitle: str = "Explain ur data viz by subtitle "):
     """
     Summarize two categorical columns by numerical column .
 
     Add new subtitle content to the third parameter.
 
     :param data: variable
 
-    :param categorical_column: str
+    :param categorical_col: str
 
-    :param numerical_column: str
+    :param numerical_col: str
 
-    :param second_categorical_column: str
+    :param second_categorical_col: str
 
     :param subtitle: str
 
     :return: bar chart
     """
 
     _, ax = plt.subplots(figsize=(11.5, 6))
-    plt.suptitle(f"The Number of {numerical_column.title()} by {categorical_column.title()} per "
-                 f"{second_categorical_column.title()}", fontweight="heavy", x=0.060, y=0.990, ha="left", fontsize="16",
+    plt.suptitle(f"The Number of {numerical_col.title()} by {categorical_col.title()} per "
+                 f"{second_categorical_col.title()}", fontweight="heavy", x=0.060, y=0.990, ha="left", fontsize="16",
                  fontfamily="sans-serif",
                  color=black_grad[0]
                  )
     plt.title(subtitle,
               fontweight="heavy", fontsize="12", fontfamily="sans-serif", color=colors[0], loc="left", pad=10)
-    df = data.groupby([categorical_column, second_categorical_column])[numerical_column].count().reset_index()\
-        .sort_values(numerical_column, ascending=False)
-    ax = sns.barplot(data=df, x=numerical_column, y=categorical_column, hue=second_categorical_column, palette=pastel,
+    df = data.groupby([categorical_col, second_categorical_col])[numerical_col].count().reset_index()\
+        .sort_values(numerical_col, ascending=False)
+    ax = sns.barplot(data=df, x=numerical_col, y=categorical_col, hue=second_categorical_col, palette=pastel,
                      errwidth=0)
     for rect in ax.containers:
         ax.bar_label(rect, color=colors[0])
 
     ax.set(frame_on=False)
 
-    plt.xlabel(f"{numerical_column}", labelpad=15, fontweight="bold", fontsize=16,
+    plt.xlabel(f"{numerical_col}", labelpad=15, fontweight="bold", fontsize=16,
                fontfamily="sans-serif",
                color=black_grad[1])
-    plt.ylabel(f"{categorical_column}", labelpad=15, fontweight="bold", fontsize=16,
+    plt.ylabel(f"{categorical_col}", labelpad=15, fontweight="bold", fontsize=16,
                fontfamily="sans-serif",
                color=black_grad[1])
-    ax.legend(title=f"{second_categorical_column.title()}",
+    ax.legend(title=f"{second_categorical_col.title()}",
               bbox_to_anchor=(1.2, 1), shadow=True, title_fontsize="x-large")
     plt.tight_layout(rect=[0, 0.04, 1, 1.025])
     plt.grid(axis="x", alpha=0.2)
     plt.show()
 
 
 def visualize_barplot_for_categorical_col(data, first_categorical_col: str, second_categorical_col: str,
@@ -817,15 +826,15 @@
     plt.tight_layout()
     plt.xlabel(f"{first_categorical_col}", labelpad=10, fontweight="bold", fontsize=16,
                fontfamily="sans-serif",
                color=black_grad[1])
     plt.show()
 
 
-def visualize_heatmap(data):
+def vis_heatmap(data):
     """
     Visualize the correlation between multiple numeric column.
     
     :param data: variable
     
     :return: heatmap
     
@@ -842,88 +851,88 @@
 
     sns.heatmap(numeric_features.corr(), cmap="Reds", annot=True, linewidths=0.1)
 
     plt.tight_layout(rect=[0, 0.04, 1, 1.025])
     plt.show()
 
 
-def visualize_linear_regression(data, numerical_column: str, numerical_col: str,
+def visualize_linear_regression(data, first_numeric: str, second_numeric: str,
                                 subtitle: str = "explain ur data viz by subtitle "):
     """
     Visualize the relationship between two numeric column.
 
     Add new subtitle content to the third parameter.
 
     :param data: variable
     
-    :param numerical_column: str
+    :param first_numeric: str
     
-    :param numerical_col: str
+    :param second_numeric: str
 
     :param subtitle: str
 
     :return: regression plot
     """
-    corr = data[numerical_column].corr(data[numerical_col])
+    corr = data[first_numeric].corr(data[second_numeric])
     print("*" * 25)
-    print("Correlation between ", numerical_column.title(), " and ", numerical_col.title(), " is ",
+    print("Correlation between ", first_numeric.title(), " and ", second_numeric.title(), " is ",
           round(corr, 2))
     print("*" * 25)
     _, ax = plt.subplots(figsize=(10, 6))
-    sns.regplot(x=numerical_column, y=numerical_col, data=data, line_kws={"color": "red"}, ax=ax)
+    sns.regplot(x=first_numeric, y=second_numeric, data=data, line_kws={"color": "red"}, ax=ax)
 
-    plt.suptitle(f"Correlation Between {numerical_column.title()} and {numerical_col.title()}",
+    plt.suptitle(f"Correlation Between {first_numeric.title()} and {second_numeric.title()}",
                  fontweight="heavy", x=0.058, y=0.98, ha="left", fontsize="16",
                  fontfamily="sans-serif",
                  color=black_grad[0]
                  )
     plt.title(subtitle,
               fontweight="heavy", fontsize="10", fontfamily="sans-serif", color=black_grad[1], loc="left", pad=38)
-    plt.xlabel(numerical_column.upper(), fontweight="regular", fontsize=11, fontfamily="sans-serif",
+    plt.xlabel(first_numeric.upper(), fontweight="regular", fontsize=11, fontfamily="sans-serif",
                color=black_grad[1])
-    plt.ylabel(numerical_col.upper(), fontweight="regular", fontsize=11, fontfamily="sans-serif", color=black_grad[1])
+    plt.ylabel(second_numeric.upper(), fontweight="regular", fontsize=11, fontfamily="sans-serif", color=black_grad[1])
     plt.tight_layout(rect=[0, 0.04, 1, 1.025])
     plt.grid(axis="x", alpha=0)
     plt.grid(axis="y", alpha=0.4)
     plt.show()
 
 
-def visualize_causation(data, numerical_column: str, numerical_col: str, categorical: str,
+def visualize_causation(data, first_numeric: str, second_numeric: str, category_col: str,
                         subtitle: str = "explain ur data viz by subtitle "):
     """
     Visualize the relationship between two numeric column by a categorical column.
 
     Add new subtitle content to the third parameter.
 
     :param data: variable
 
-    :param numerical_column: str
+    :param first_numeric: str
 
-    :param numerical_col: str
+    :param second_numeric: str
 
-    :param categorical: str
+    :param category_col: str
 
-    :param subtitle:str
+    :param subtitle: str
 
     :return: regression plot
     """
 
-    sns.lmplot(x=numerical_column, y=numerical_col, hue=categorical, data=data, palette=pastel, legend=False, height=6,
+    sns.lmplot(x=first_numeric, y=second_numeric, hue=category_col, data=data, palette=pastel, legend=False, height=6,
                aspect=1.5)
-    plt.suptitle(f"Correlation Between {numerical_column.title()} and {numerical_col.title()}",
+    plt.suptitle(f"Correlation Between {first_numeric.title()} and {second_numeric.title()}",
                  fontweight="heavy", x=0.065, y=0.98, ha="left", fontsize="16",
                  fontfamily="sans-serif",
                  color=black_grad[0]
                  )
     plt.title(subtitle,
               fontweight="heavy", fontsize="10", fontfamily="sans-serif", color=black_grad[1], loc="left", pad=40)
-    plt.xlabel(numerical_column.upper(), fontweight="regular", fontsize=11, fontfamily="sans-serif",
+    plt.xlabel(first_numeric.upper(), fontweight="regular", fontsize=11, fontfamily="sans-serif",
                color=black_grad[1])
-    plt.ylabel(numerical_col.upper(), fontweight="regular", fontsize=11, fontfamily="sans-serif", color=black_grad[1])
-    plt.legend(title=categorical.title(), bbox_to_anchor=(1, 1.02), loc="upper left")
+    plt.ylabel(second_numeric.upper(), fontweight="regular", fontsize=11, fontfamily="sans-serif", color=black_grad[1])
+    plt.legend(title=category_col.title(), bbox_to_anchor=(1, 1.02), loc="upper left")
     plt.tight_layout(rect=[0, 0.04, 1, 1.025])
     plt.grid(axis="x", alpha=0)
     plt.grid(axis="y", alpha=0.4)
     plt.show()
 
 
 def save_data_to_csv_file(data, filename: str):
@@ -947,19 +956,24 @@
 
     - Year
 
     - Month
 
     - Day
 
-    :param data:
-    :param date_colum:
-    :param numerical_column:
-    :param filter_by:
-    :param subtitle:
+    :param data: variable
+
+    :param date_colum: str
+
+    :param numerical_column: str
+
+    :param filter_by: str
+
+    :param subtitle: str
+
     :return: Line Chart
     """
     fig, ax = plt.subplots(figsize=(10, 6))
     if filter_by.lower() == "month":
         data[date_colum] = pd.to_datetime(data[date_colum])
         data[filter_by] = data[date_colum].dt.month
         sns.lineplot(data=data, x=filter_by, y=numerical_column, linewidth=1, estimator="sum", errorbar=None, ax=ax)
@@ -986,33 +1000,40 @@
     plt.grid(axis="x", alpha=0)
     plt.grid(axis="y", alpha=0.4)
     ax.locator_params(integer=True)
     plt.show()
 
 
 def visualize_time_relationship_by_categorical_variable(data, date_colum: str, numerical_col: str,
-                                                        categorical_colum, filter_by: str,
+                                                        categorical_colum: str, filter_by: str,
                                                         subtitle: str = "explain ur data viz by subtitle "):
     """
-        Visualize the sum between date column and continues column with categorical column, filter by :
+    Visualize the sum between date column and continues column with categorical column, filter by :
+
+    - Year
 
-        - Year
+    - Month
 
-        - Month
+    - Day
 
-        - Day
+    :param data: variable
+
+    :param date_colum: str
+
+    :param numerical_col: str
+
+    :param filter_by: str
+
+    :param categorical_colum: str
+
+    :param subtitle: str
+
+    :return: Line Chart
+    """
 
-        :param data:
-        :param date_colum:
-        :param numerical_col:
-        :param filter_by:
-        :param categorical_colum:
-        :param subtitle:
-        :return: Line Chart
-        """
     fig, ax = plt.subplots(figsize=(10, 6))
     if filter_by.lower() == "month":
         data[date_colum] = pd.to_datetime(data[date_colum])
         data[filter_by] = data[date_colum].dt.month
         sns.lineplot(data=data, x=filter_by, y=numerical_col, hue=categorical_colum, linewidth=2, estimator="sum",
                      errorbar=None, color=pastel, ax=ax)
     elif filter_by.lower() == "year":
@@ -1042,16 +1063,16 @@
     plt.grid(axis="y", alpha=0.4)
     ax.locator_params(integer=True)
     plt.legend(title=categorical_colum.title(), bbox_to_anchor=(1, 1.02), loc="upper left", shadow=True)
     plt.tight_layout(rect=[0, 0.04, 1, 1.025])
     plt.show()
 
 
-def visualize_highest_percentage_datapoints(data, first_categorical_col: str, second_categorical_col: str,
-                                            subtitle: str = "explain ur data viz by subtitle "):
+def vis_highest_percentage_datapoints(data, first_categorical_col: str, second_categorical_col: str,
+                                      subtitle: str = "explain ur data viz by subtitle "):
     """
     Visualize the highest percentage of datapoint values,
 
     for categorical variable grouped by second categorical variable.
 
     Add new subtitle content to the third parameter.
 
@@ -1095,158 +1116,194 @@
     plt.tight_layout()
     plt.xlabel(f"{first_categorical_col}", labelpad=10, fontweight="bold", fontsize=16,
                fontfamily="sans-serif",
                color=black_grad[1])
     plt.show()
 
 
-def visualize_lowest_percentage_datapoints(data, first_categorical_col: str, second_categorical_col: str,
-                                           subtitle: str = "explain ur data viz by subtitle "):
+def vis_lowest_percentage_datapoints(data, first_categorical: str, second_categorical: str,
+                                     subtitle: str = "explain ur data viz by subtitle "):
     """
     Visualize the lowest percentage of datapoint values,
 
     for categorical variable grouped by second categorical variable.
 
     Add new subtitle content to the third parameter.
 
     :param data: variable
 
-    :param first_categorical_col: str
+    :param first_categorical: str
 
-    :param second_categorical_col: str
+    :param second_categorical: str
 
     :param subtitle: str
 
     :return: count plot
     """
     _, ax = plt.subplots(figsize=(10, 6))
-    plt.suptitle(f"{first_categorical_col.title()} Lowest Percentage per {second_categorical_col.title()}",
+    plt.suptitle(f"{first_categorical.title()} Lowest Percentage per {second_categorical.title()}",
                  fontweight="heavy", x=0.044, y=0.98, ha="left", fontsize="16",
                  fontfamily="sans-serif",
                  color=black_grad[0]
                  )
     plt.title(subtitle.capitalize(),
               fontweight="heavy", fontsize="12", fontfamily="sans-serif", color=black_grad[1], loc="left", pad=40)
 
-    ax = sns.countplot(x=first_categorical_col, hue=second_categorical_col, data=data,
+    ax = sns.countplot(x=first_categorical, hue=second_categorical, data=data,
                        color="aquamarine", saturation=0.5)
 
     for c in ax.containers:
         # custom label calculates percent and add an empty string so 0 value bars don't have a number
-        labels = [f'{h / data[second_categorical_col].count() * 100:0.1f}%' if (h := v.get_height()) > 0 else '' for v
+        labels = [f'{h / data[second_categorical].count() * 100:0.1f}%' if (h := v.get_height()) > 0 else '' for v
                   in c]
         ax.bar_label(c, labels=labels, label_type='edge', fontsize=10, color=colors[0])
 
     # Lowest value
     patch_h = [patch.get_height() for patch in ax.patches]
     idx_tallest = np.argmin(patch_h)
     ax.patches[idx_tallest].set_facecolor("tomato")
 
-    ax.set(xlabel=first_categorical_col, frame_on=False, ylabel=None)
-    ax.legend(title=second_categorical_col.title(), bbox_to_anchor=(1, 1.02), loc="upper left")
+    ax.set(xlabel=first_categorical, frame_on=False, ylabel=None)
+    ax.legend(title=second_categorical.title(), bbox_to_anchor=(1, 1.02), loc="upper left")
     plt.tight_layout()
-    plt.xlabel(f"{first_categorical_col}", labelpad=10, fontweight="bold", fontsize=16,
+    plt.xlabel(f"{first_categorical}", labelpad=10, fontweight="bold", fontsize=16,
                fontfamily="sans-serif",
                color=black_grad[1])
     plt.show()
 
 
-def visualize_top_ten_values(data_frame, first_column: str, second_column: str, limit_number: int,
-                             subtitle: str = "Explain ur data viz by subtitle "):
+def vis_top_ten_values(data_frame, first_categorical: str, second_categorical: str, limit_number: int,
+                       subtitle: str = "Explain ur data viz by subtitle "):
     """
     Visualize the top 10  values from two  categorical columns limit the number to determine which bars to color.
 
     Add new subtitle content to the third parameter.
 
     :param data_frame: variable
 
-    :param second_column: str
+    :param second_categorical: str
 
-    :param first_column: str
+    :param first_categorical: str
 
     :param limit_number: int
 
     :param subtitle: str
 
     :return: bar chart
     """
 
     _, ax = plt.subplots(figsize=(10, 6))
 
-    grouped_data = data_frame.groupby(first_column)[second_column].count().sort_values(ascending=False).head(10)
+    grouped_data = data_frame.groupby(first_categorical)[second_categorical].count()\
+        .sort_values(ascending=False).head(10)
 
-    plt.suptitle(f"{first_column.title()} with the most {second_column.title()} ",
+    plt.suptitle(f"{first_categorical.title()} with the most {second_categorical.title()} ",
                  fontweight="heavy", x=0.069, y=0.98, ha="left", fontsize="16",
                  fontfamily="sans-serif",
                  color=black_grad[0]
                  )
     plt.title(subtitle,
               fontweight="heavy", fontsize="12", fontfamily="sans-serif", color=black_grad[1], loc="left", pad=10)
 
     set_colors = [colors[0] if x < limit_number else colors[1] for x in grouped_data.values]
     fig = sns.barplot(data=pd.DataFrame(grouped_data).transpose(), orient="h", palette=set_colors)
-    fig.set_ylabel(first_column, fontsize=12)
-    fig.set_xlabel(f"\nCount of {second_column.title()}", fontsize=12)
+    fig.set_ylabel(first_categorical, fontsize=12)
+    fig.set_xlabel(f"\nCount of {second_categorical.title()}", fontsize=12)
     fig.set_yticklabels(fig.get_yticklabels(), rotation=0)
 
     for p in fig.patches:
         width = p.get_width()
         if width < limit_number:
             clr = colors[2]
         else:
             clr = colors[3]
         plt.text(-30 + p.get_width(), p.get_y()+0.45*p.get_height(), "{:.0f}".format(width), color=clr,
                  ha="center", va="center", fontsize="large")
     sns.despine(right=True, top=True, left=True)
+    ax.set(frame_on=False)
     plt.tight_layout()
     plt.show()
 
 
-def visualize_top_highest_average(data_frame, categorical_column: str, numerical_column: str, avg_numbers: list,
-                                  subtitle: str = "Explain ur data viz by subtitle "):
+def vis_top_highest_average(data_frame, categorical_column: str, numerical_column: str, avg_numbers: list,
+                            subtitle: str = "Explain ur data viz by subtitle "):
     """
     Visualize the highest average values.
 
     add avg_numbers to determine which bars to be colored.
 
     Add new subtitle content to the third parameter.
 
-    :param data_frame:
-    :param categorical_column:
-    :param numerical_column:
-    :param avg_numbers:
-    :param subtitle:
+    :param data_frame: variable
+
+    :param categorical_column: str
+
+    :param numerical_column: str
+
+    :param avg_numbers: list
+
+    :param subtitle: str
+
     :return: bar chart
     """
 
-    df_cat = data_frame.loc[data_frame[categorical_column].isin(data_frame[categorical_column].value_counts().head(10)
-                                                                .index)]
+    df_cat = data_frame.loc[data_frame[categorical_column].isin(data_frame[categorical_column]
+                                                                .value_counts().head(10).index)]
 
-    numer = df_cat.groupby(categorical_column)[numerical_column].mean().round(3)\
-        .astype("float64").sort_values(ascending=False)
+    numer = df_cat.groupby(categorical_column)[numerical_column].mean().round(2)\
+        .astype("float64").sort_values(ascending=False).head(10)
     _, ax = plt.subplots(figsize=(10, 6))
-    plt.suptitle(f"Average {numerical_column.title()} per {categorical_column.title()} ",
+    plt.suptitle(f"The Highest Average {numerical_column.title()} per {categorical_column.title()} ",
                  fontweight="heavy", x=0.069, y=0.98, ha="left", fontsize="16",
                  fontfamily="sans-serif",
                  color=black_grad[0]
                  )
     plt.title(subtitle,
               fontweight="heavy", fontsize="12", fontfamily="sans-serif", color=black_grad[1], loc="left", pad=15)
 
     set_colors = [colors[1] if x in avg_numbers else colors[0] for x in numer.values]
     fig = sns.barplot(data=pd.DataFrame(numer).transpose(), orient="h", palette=set_colors)
-    fig.set_ylabel(categorical_column, fontsize=12)
-    fig.set_xlabel(f"\nMean {numerical_column.title()}", fontsize=12)
+    fig.set_ylabel(categorical_column.title(), fontsize=12)
+    fig.set_xlabel(f"\nAverage {numerical_column.title()}", fontsize=12)
     fig.set_yticklabels(fig.get_yticklabels(), rotation=0)
 
-    for p in fig.patches:
-        width = p.get_width()
-        if width in avg_numbers:
-            clr = colors[2]
-        else:
-            clr = colors[3]
-        plt.text(-25 + p.get_width(), p.get_y() + 0.50 * p.get_height(), "{:.0f}".format(width), color=clr,
-                 ha="center", va="center", fontsize="medium")
-    sns.despine(right=True, top=True, left=True)
     show_values(fig, "h")
+    plt.grid(axis="y", alpha=0)
+    plt.grid(axis="x", alpha=0)
+    ax.set(frame_on=False)
+    plt.tight_layout()
+    plt.show()
+
+
+def vis_pie_chart(data, categorical_col: str, numerical_col: str,
+                  subtitle: str = "explain ur data viz by subtitle"):
+    """
+    Visualize the highest label in pie chart.
+
+    Add new subtitle content to the third parameter.
+
+    :param data: variable
+    :param categorical_col: str
+    :param numerical_col: str
+    :param subtitle: str
+    :return: pie chart
+    """
+
+    _, ax = plt.subplots(figsize=(10, 6))
+    plt.suptitle(f"Comparison {numerical_col.title()} per {categorical_col.title()}",
+                 fontweight="heavy", x=0.30, y=0.99, fontsize="16", ha="left",
+                 fontfamily="sans-serif",
+                 color=black_grad[0]
+                 )
+    plt.title(subtitle.capitalize(),
+              fontweight="heavy", fontsize="10", fontfamily="sans-serif", color="dimgray", loc="left", pad=8)
+    labels = data[categorical_col].unique()
+    df = data.groupby(categorical_col)[numerical_col].mean()
+    clrs = [colors[0] if (x < max(df.values)) else colors[1] for x in df.values]
+    plt.pie(df, colors=clrs, pctdistance=0.7, autopct="%.2f%%", labels=labels, labeldistance=1.1,
+            wedgeprops=dict(alpha=0.8, edgecolor="floralwhite"), textprops={"fontsize": 10})
+    centre = plt.Circle((0, 0), 0.45, fc="white", edgecolor=colors[0])
+    plt.gcf().gca().add_artist(centre)
+    ax.legend(title=categorical_col.title(), bbox_to_anchor=(0.5, -0.04), ncol=4, loc="upper center",
+              frameon=True, shadow=True)
     plt.tight_layout()
     plt.show()
```

### Comparing `pydatavisualization-0.0.3/pydatavisualization.egg-info/PKG-INFO` & `pydatavisualization-0.0.4/pydatavisualization.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydatavisualization
-Version: 0.0.3
+Version: 0.0.4
 Summary: Data Visualization Functions
 Author: Tamer Samara
 Author-email: tamer.samara@gmail.com
 License: MIT
 Keywords: python,data+science,eda,data+preprocessing,data+analysis,machine+learning
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `pydatavisualization-0.0.3/setup.py` & `pydatavisualization-0.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import setuptools
 from setuptools import setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'Data Visualization Functions'
-LONG_DESCRIPTION = 'The modules include functions that might be useful in general cases for data analysis ' \
+LONG_DESCRIPTION = 'The module include functions that might be useful in general cases for data analysis ' \
                    'and data visualization. '
 
 # Setting up
 setup(
     name="pydatavisualization",
     version=VERSION,
     license="MIT",
     author="Tamer Samara",
     author_email="tamer.samara@gmail.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=setuptools.find_packages(),
-    install_requires=["Pandas", "Statsmodels", "Seaborn", "Matplotlib", "SciPy", "NumPy", "Scikit-learn"],
+    install_requires=["Pandas", "Statsmodels", "Seaborn", "Matplotlib","NumPy", "Scikit-learn"],
     keywords=['python', 'data+science', 'eda', 'data+preprocessing', 'data+analysis', 'machine+learning'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
```

