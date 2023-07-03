# Comparing `tmp/Simba-UW-tf-dev-1.63.7.tar.gz` & `tmp/Simba-UW-tf-dev-1.63.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Simba-UW-tf-dev-1.63.7.tar", last modified: Thu Jun 29 19:37:39 2023, max compression
+gzip compressed data, was "dist/Simba-UW-tf-dev-1.63.8.tar", last modified: Mon Jul  3 16:33:46 2023, max compression
```

## Comparing `Simba-UW-tf-dev-1.63.7.tar` & `Simba-UW-tf-dev-1.63.8.tar`

### file list

```diff
@@ -1,581 +1,583 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:38.000000 Simba-UW-tf-dev-1.63.7/simba/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/ui/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.63.7/simba/ui/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/
--rw-r--r--   0 simon      (501) staff       (20)     9020 2023-06-29 01:16:45.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/mutual_exclusivity_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/csv_2_parquet_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2343 2023-05-17 20:47:45.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/quick_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/batch_preprocess_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8342 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/heatmap_location_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/clf_probability_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:42.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/movement_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9471 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/clf_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    15950 2023-05-20 12:10:35.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1150 2023-05-25 18:21:39.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/remove_roi_features_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5814 2023-06-15 20:06:37.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/roi_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5977 2023-05-31 12:58:14.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/outlier_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/gantt_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/clf_validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7721 2023-05-24 15:18:33.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/severity_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/fsttc_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4052 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/kleinberg_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7288 2023-05-29 20:14:50.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5425 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/pose_reorganizer_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/clf_by_timebins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8673 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/heatmap_clf_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/data_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7860 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/roi_features_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/pup_retrieval_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/about_simba_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3605 2023-05-25 18:54:56.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6353 2023-05-24 15:31:12.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    42478 2023-04-29 18:56:08.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/video_processing_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7535 2023-05-15 13:09:04.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/clf_by_roi_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/make_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/archive_files_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4087 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/pose_bp_drop_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    10695 2023-05-31 16:42:04.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/distance_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3599 2023-06-29 19:35:48.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    12869 2023-05-23 12:47:59.000000 Simba-UW-tf-dev-1.63.7/simba/ui/video_info_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     6019 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.63.7/simba/ui/user_defined_pose_creator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/ui/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    12879 2023-06-18 20:27:37.000000 Simba-UW-tf-dev-1.63.7/simba/ui/create_project_ui.py
--rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.63.7/simba/ui/tkinter_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    35431 2023-06-13 17:24:57.000000 Simba-UW-tf-dev-1.63.7/simba/ui/machine_model_settings_ui.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/blob_storage/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.63.7/simba/blob_storage/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/labelling/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.63.7/simba/labelling/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21667 2023-06-20 18:30:00.000000 Simba-UW-tf-dev-1.63.7/simba/labelling/labelling_interface_old.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/labelling/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    20914 2023-06-22 13:26:28.000000 Simba-UW-tf-dev-1.63.7/simba/labelling/labelling_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     3568 2023-05-19 11:18:49.000000 Simba-UW-tf-dev-1.63.7/simba/labelling/extract_labelled_frames.py
--rw-r--r--   0 simon      (501) staff       (20)    26943 2023-06-20 19:04:35.000000 Simba-UW-tf-dev-1.63.7/simba/labelling/labelling_advanced_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     6629 2023-05-13 17:45:08.000000 Simba-UW-tf-dev-1.63.7/simba/labelling/play_annotation_video.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)    11877 2023-05-17 14:59:39.000000 Simba-UW-tf-dev-1.63.7/simba/unsupervised/dbcv_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.63.7/simba/unsupervised/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-13 17:25:39.000000 Simba-UW-tf-dev-1.63.7/simba/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     8141 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.63.7/simba/unsupervised/dataset_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     5636 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.63.7/simba/unsupervised/grid_search_visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)     7310 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.63.7/simba/unsupervised/data_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     9846 2023-06-06 18:27:30.000000 Simba-UW-tf-dev-1.63.7/simba/unsupervised/ui.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/unsupervised/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     9851 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.63.7/simba/unsupervised/umap_embedder.py
--rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.63.7/simba/unsupervised/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)     2931 2023-05-17 14:54:38.000000 Simba-UW-tf-dev-1.63.7/simba/unsupervised/bout_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)    20846 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.63.7/simba/unsupervised/cluster_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.63.7/simba/unsupervised/data_map.yaml
--rw-r--r--   0 simon      (501) staff       (20)    10287 2023-06-06 17:50:12.000000 Simba-UW-tf-dev-1.63.7/simba/unsupervised/hdbscan_clusterer.py
--rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.63.7/simba/unsupervised/tsne.py
--rw-r--r--   0 simon      (501) staff       (20)     6656 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.63.7/simba/unsupervised/cluster_visualizer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/bounding_box_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.63.7/simba/bounding_box_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/bounding_box_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7031 2023-05-14 18:13:04.000000 Simba-UW-tf-dev-1.63.7/simba/bounding_box_tools/agg_boundary_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    23566 2023-05-14 18:29:41.000000 Simba-UW-tf-dev-1.63.7/simba/bounding_box_tools/boundary_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     8497 2023-05-14 18:22:39.000000 Simba-UW-tf-dev-1.63.7/simba/bounding_box_tools/boundary_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     6376 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.7/simba/bounding_box_tools/find_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    11381 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.7/simba/bounding_box_tools/visualize_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    49156 2023-06-26 17:54:54.000000 Simba-UW-tf-dev-1.63.7/simba/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)    42512 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/feature_extractor_14bp.py
--rw-r--r--   0 simon      (501) staff       (20)    21482 2023-05-14 23:55:56.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/feature_extractor_7bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/
--rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/peaks.py
--rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     7127 2023-05-28 19:41:35.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-07 20:28:11.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     8943 2023-06-05 18:15:28.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/shap_log_mp_2.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     8580 2023-05-31 20:02:32.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/shap_log_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)    30764 2023-06-13 17:23:34.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
--rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/time_stamp_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     4279 2023-06-01 12:49:14.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/read_files_mp_2.py
--rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:44:29.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
--rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)    27995 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/feature_extractor_8bps_2_animals.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3864 2023-05-19 19:41:40.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/perimeter_jit.py
--rw-r--r--   0 simon      (501) staff       (20)    16349 2023-06-29 19:29:12.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/feature_subsets.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8244 2023-05-21 16:28:49.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/feature_extractor_user_defined.py
--rw-r--r--   0 simon      (501) staff       (20)    46461 2023-05-15 00:03:36.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/feature_extractor_16bp.py
--rw-r--r--   0 simon      (501) staff       (20)    28259 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/feature_extractor_9bp.py
--rw-r--r--   0 simon      (501) staff       (20)    23976 2023-05-15 00:01:21.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/feature_extractor_8bp.py
--rw-r--r--   0 simon      (501) staff       (20)    16880 2023-05-14 23:53:59.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/feature_extractor_4bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/.idea/features_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/.idea/.gitignore
--rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/.idea/.name
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/feature_extractors/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    15434 2023-05-20 18:29:53.000000 Simba-UW-tf-dev-1.63.7/simba/requirements.txt
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/mixins/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.63.7/simba/mixins/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43029 2023-06-05 17:40:09.000000 Simba-UW-tf-dev-1.63.7/simba/mixins/pop_up_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    38224 2023-06-15 15:41:52.000000 Simba-UW-tf-dev-1.63.7/simba/mixins/config_reader.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/mixins/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18616 2023-05-17 19:39:33.000000 Simba-UW-tf-dev-1.63.7/simba/mixins/pose_importer_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/mixins/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-06-01 18:12:36.000000 Simba-UW-tf-dev-1.63.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.63.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     2090 2023-06-01 14:35:51.000000 Simba-UW-tf-dev-1.63.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    82442 2023-06-01 18:12:36.000000 Simba-UW-tf-dev-1.63.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    51809 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.63.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    14391 2023-06-01 14:35:51.000000 Simba-UW-tf-dev-1.63.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.2.nbc
--rw-r--r--   0 simon      (501) staff       (20)    14188 2023-05-21 00:18:56.000000 Simba-UW-tf-dev-1.63.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    37135 2023-06-02 12:12:15.000000 Simba-UW-tf-dev-1.63.7/simba/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    61873 2023-05-19 21:14:46.000000 Simba-UW-tf-dev-1.63.7/simba/mixins/plotting_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     9145 2023-06-13 18:36:10.000000 Simba-UW-tf-dev-1.63.7/simba/mixins/unsupervised_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    73291 2023-06-19 20:46:57.000000 Simba-UW-tf-dev-1.63.7/simba/mixins/train_model_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/third_party_label_appenders/
--rw-r--r--   0 simon      (501) staff       (20)     6094 2023-05-21 17:39:19.000000 Simba-UW-tf-dev-1.63.7/simba/third_party_label_appenders/deepethogram_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    10759 2023-06-08 22:23:03.000000 Simba-UW-tf-dev-1.63.7/simba/third_party_label_appenders/BORIS_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8998 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.63.7/simba/third_party_label_appenders/observer_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.63.7/simba/third_party_label_appenders/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    18417 2023-06-18 19:01:16.000000 Simba-UW-tf-dev-1.63.7/simba/third_party_label_appenders/tools.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.63.7/simba/third_party_label_appenders/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18934 2023-06-18 19:03:04.000000 Simba-UW-tf-dev-1.63.7/simba/third_party_label_appenders/third_party_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8181 2023-05-21 17:19:25.000000 Simba-UW-tf-dev-1.63.7/simba/third_party_label_appenders/ethovision_import.py
--rw-r--r--   0 simon      (501) staff       (20)     6988 2023-05-21 17:31:04.000000 Simba-UW-tf-dev-1.63.7/simba/third_party_label_appenders/BENTO_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     5239 2023-05-21 18:07:18.000000 Simba-UW-tf-dev-1.63.7/simba/third_party_label_appenders/solomon_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/cue_light_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.63.7/simba/cue_light_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7652 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.7/simba/cue_light_tools/cue_light_clf_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    12207 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.7/simba/cue_light_tools/cue_light_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    16690 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.7/simba/cue_light_tools/cue_light_menues.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/cue_light_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1879 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.7/simba/cue_light_tools/cue_light_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    15212 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.63.7/simba/cue_light_tools/cue_light_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12650 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.7/simba/cue_light_tools/cue_light_movement_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/utils/
--rw-r--r--   0 simon      (501) staff       (20)    11876 2023-06-18 20:21:39.000000 Simba-UW-tf-dev-1.63.7/simba/utils/config_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    21103 2023-06-20 12:58:32.000000 Simba-UW-tf-dev-1.63.7/simba/utils/enums.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.63.7/simba/utils/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7601 2023-06-18 18:58:51.000000 Simba-UW-tf-dev-1.63.7/simba/utils/warnings.py
--rw-r--r--   0 simon      (501) staff       (20)     8807 2023-05-25 13:24:45.000000 Simba-UW-tf-dev-1.63.7/simba/utils/checks.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/utils/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    43313 2023-06-27 15:38:38.000000 Simba-UW-tf-dev-1.63.7/simba/utils/read_write.py
--rw-r--r--   0 simon      (501) staff       (20)     9841 2023-06-19 23:24:08.000000 Simba-UW-tf-dev-1.63.7/simba/utils/lookups.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/utils/cli/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/utils/cli/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6017 2023-05-28 13:41:20.000000 Simba-UW-tf-dev-1.63.7/simba/utils/cli/cli_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    14666 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.63.7/simba/utils/errors.py
--rw-r--r--   0 simon      (501) staff       (20)    19250 2023-06-13 13:46:20.000000 Simba-UW-tf-dev-1.63.7/simba/utils/data.py
--rw-r--r--   0 simon      (501) staff       (20)     1615 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.63.7/simba/utils/printing.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/st/
--rw-r--r--   0 simon      (501) staff       (20)      282 2023-06-16 17:26:25.000000 Simba-UW-tf-dev-1.63.7/simba/st/enums.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-16 13:55:39.000000 Simba-UW-tf-dev-1.63.7/simba/st/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2102 2023-06-19 19:54:19.000000 Simba-UW-tf-dev-1.63.7/simba/st/select_groups_pg.py
--rw-r--r--   0 simon      (501) staff       (20)     2325 2023-06-19 19:54:19.000000 Simba-UW-tf-dev-1.63.7/simba/st/aggregate_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     1485 2023-06-16 18:20:31.000000 Simba-UW-tf-dev-1.63.7/simba/st/app.py
--rw-r--r--   0 simon      (501) staff       (20)      249 2023-06-16 18:20:19.000000 Simba-UW-tf-dev-1.63.7/simba/st/welcome_page.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/pose_processors/
--rw-r--r--   0 simon      (501) staff       (20)     8256 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.63.7/simba/pose_processors/reorganize_keypoint.py
--rw-r--r--   0 simon      (501) staff       (20)     5167 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.63.7/simba/pose_processors/remove_keypoints.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.63.7/simba/pose_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/pose_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2656 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.63.7/simba/pose_processors/pose_reset.py
--rw-r--r--   0 simon      (501) staff       (20)     5618 2023-06-13 18:36:10.000000 Simba-UW-tf-dev-1.63.7/simba/pose_processors/reverse_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     9114 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/gantt_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/tools/
--rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/tools/tkinter_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    13008 2023-05-24 15:32:44.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    14568 2023-05-15 18:41:17.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/shap_agg_stats_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    10105 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/gantt_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15730 2023-05-15 17:49:01.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/heat_mapper_clf_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8731 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/probability_plot_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    12484 2023-05-23 14:52:24.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/plot_clf_results.py
--rw-r--r--   0 simon      (501) staff       (20)    14056 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/plot_clf_results_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    16031 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/ROI_feature_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12770 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/heat_mapper_location.py
--rw-r--r--   0 simon      (501) staff       (20)    10100 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/probability_plot_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     4881 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/interactive_probability_grapher.py
--rw-r--r--   0 simon      (501) staff       (20)    14029 2023-06-04 11:55:47.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/single_run_model_validation_video.py
--rw-r--r--   0 simon      (501) staff       (20)    12790 2023-05-16 16:20:20.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/frame_mergerer_ffmpeg.py
--rw-r--r--   0 simon      (501) staff       (20)     7660 2023-06-20 12:45:11.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/pose_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     7891 2023-05-29 21:41:05.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/Directing_animals_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11219 2023-05-17 12:58:17.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/clf_validator.py
--rw-r--r--   0 simon      (501) staff       (20)    15745 2023-05-20 12:16:06.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/path_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11203 2023-05-24 15:35:24.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/ROI_feature_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8933 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/data_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13471 2023-05-20 12:15:46.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/path_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     6494 2023-05-17 20:55:17.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/ez_lineplot.py
--rw-r--r--   0 simon      (501) staff       (20)    11519 2023-05-31 16:42:04.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/distance_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15794 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13163 2023-05-16 16:42:03.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/heat_mapper_clf.py
--rw-r--r--   0 simon      (501) staff       (20)     9385 2023-05-31 16:46:49.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     9526 2023-06-04 12:03:25.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/single_run_model_validation_video_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    10005 2023-05-29 21:36:37.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/Directing_animals_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    16320 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.63.7/simba/plotting/heat_mapper_location_mp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/dash_app/
--rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/dash_app/SimBA_dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/dash_app/run_dash_tkinter.py
--rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/dash_app/dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-16 12:50:41.000000 Simba-UW-tf-dev-1.63.7/simba/dash_app/plotly_dash.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/data_processors/
--rw-r--r--   0 simon      (501) staff       (20)     7248 2023-05-25 19:01:00.000000 Simba-UW-tf-dev-1.63.7/simba/data_processors/agg_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.63.7/simba/data_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    11196 2023-05-28 19:50:35.000000 Simba-UW-tf-dev-1.63.7/simba/data_processors/severity_bout_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    16285 2023-06-13 13:57:45.000000 Simba-UW-tf-dev-1.63.7/simba/data_processors/interpolation_smoothing.py
--rw-r--r--   0 simon      (501) staff       (20)     8127 2023-05-25 13:57:19.000000 Simba-UW-tf-dev-1.63.7/simba/data_processors/timebins_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    13451 2023-06-19 20:47:55.000000 Simba-UW-tf-dev-1.63.7/simba/data_processors/fsttc_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/data_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6306 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.63.7/simba/data_processors/interpolate_pose.py
--rw-r--r--   0 simon      (501) staff       (20)     9646 2023-05-14 19:19:14.000000 Simba-UW-tf-dev-1.63.7/simba/data_processors/directing_other_animals_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8624 2023-05-25 14:07:56.000000 Simba-UW-tf-dev-1.63.7/simba/data_processors/timebins_movement_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     4799 2023-05-17 17:23:16.000000 Simba-UW-tf-dev-1.63.7/simba/data_processors/severity_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    16980 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.63.7/simba/data_processors/pup_retrieval_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-13 17:23:00.000000 Simba-UW-tf-dev-1.63.7/simba/data_processors/pybursts_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    11533 2023-05-28 19:50:34.000000 Simba-UW-tf-dev-1.63.7/simba/data_processors/severity_frame_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     6087 2023-06-28 20:32:32.000000 Simba-UW-tf-dev-1.63.7/simba/data_processors/mutual_exclusivity_corrector.py
--rw-r--r--   0 simon      (501) staff       (20)     9656 2023-05-25 13:32:25.000000 Simba-UW-tf-dev-1.63.7/simba/data_processors/kleinberg_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8131 2023-05-25 14:37:36.000000 Simba-UW-tf-dev-1.63.7/simba/data_processors/movement_calculator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:38.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/model/
--rw-r--r--   0 simon      (501) staff       (20)    20086 2023-06-05 20:43:28.000000 Simba-UW-tf-dev-1.63.7/simba/model/train_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.63.7/simba/model/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3315 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.63.7/simba/model/inference_batch.py
--rw-r--r--   0 simon      (501) staff       (20)    20849 2023-06-05 18:44:40.000000 Simba-UW-tf-dev-1.63.7/simba/model/grid_search_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3363 2023-05-19 11:12:45.000000 Simba-UW-tf-dev-1.63.7/simba/model/inference_validation.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/roi_tools/
--rw-r--r--   0 simon      (501) staff       (20)     5858 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_time_bin_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     1687 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.63.7/simba/roi_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43194 2023-06-22 13:51:00.000000 Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_define.py
--rw-r--r--   0 simon      (501) staff       (20)     4024 2023-05-16 13:21:43.000000 Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_reset.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/roi_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    20174 2023-06-12 15:28:58.000000 Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    11608 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_feature_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_multiply.py
--rw-r--r--   0 simon      (501) staff       (20)     2290 2023-06-12 16:21:03.000000 Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_size_calculations.py
--rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_zoom.py
--rw-r--r--   0 simon      (501) staff       (20)    11474 2023-06-12 19:37:22.000000 Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_directing_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_move_shape.py
--rw-r--r--   0 simon      (501) staff       (20)     5080 2023-06-22 13:37:25.000000 Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    13742 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_image.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)     8115 2023-05-14 18:03:14.000000 Simba-UW-tf-dev-1.63.7/simba/pose_importers/sleap_csv_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/pose_importers/misc/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:42:38.000000 Simba-UW-tf-dev-1.63.7/simba/pose_importers/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.63.7/simba/pose_importers/misc/apt_trk_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.63.7/simba/pose_importers/read_DANNCE_mat.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.63.7/simba/pose_importers/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    12549 2023-05-17 20:32:56.000000 Simba-UW-tf-dev-1.63.7/simba/pose_importers/sleap_h5_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7322 2023-05-16 16:55:05.000000 Simba-UW-tf-dev-1.63.7/simba/pose_importers/madlc_importer.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/pose_importers/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    12141 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.63.7/simba/pose_importers/sleap_slp_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7931 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.63.7/simba/pose_importers/import_mars.py
--rw-r--r--   0 simon      (501) staff       (20)     6978 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.7/simba/pose_importers/dlc_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.63.7/simba/pose_importers/trk_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-05-14 23:57:00.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations/schematics/
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/pose_configurations/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:38.000000 Simba-UW-tf-dev-1.63.7/simba/three_dimensions/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/three_dimensions/ui/
--rw-r--r--   0 simon      (501) staff       (20)     1747 2023-06-25 18:18:01.000000 Simba-UW-tf-dev-1.63.7/simba/three_dimensions/ui/define_px_to_mm_ui.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/three_dimensions/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)     6777 2023-06-26 17:04:03.000000 Simba-UW-tf-dev-1.63.7/simba/three_dimensions/feature_extractors/generic_feature_extractor.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/three_dimensions/mixins/
--rw-r--r--   0 simon      (501) staff       (20)    38820 2023-06-23 01:28:48.000000 Simba-UW-tf-dev-1.63.7/simba/three_dimensions/mixins/config_reader.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/three_dimensions/mixins/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)    51001 2023-06-26 13:52:31.000000 Simba-UW-tf-dev-1.63.7/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    50997 2023-06-25 19:59:06.000000 Simba-UW-tf-dev-1.63.7/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1380 2023-06-26 13:52:31.000000 Simba-UW-tf-dev-1.63.7/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     1379 2023-06-25 19:59:06.000000 Simba-UW-tf-dev-1.63.7/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     3758 2023-06-26 13:45:44.000000 Simba-UW-tf-dev-1.63.7/simba/three_dimensions/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     3953 2023-06-25 18:18:01.000000 Simba-UW-tf-dev-1.63.7/simba/three_dimensions/mixins/plotting_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/three_dimensions/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     3192 2023-06-25 18:21:24.000000 Simba-UW-tf-dev-1.63.7/simba/three_dimensions/plotting/plot_pose_in_dir.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/three_dimensions/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)     3445 2023-06-22 22:21:05.000000 Simba-UW-tf-dev-1.63.7/simba/three_dimensions/pose_importers/anipose_csv_import.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/three_dimensions/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     5832 2023-06-23 13:06:19.000000 Simba-UW-tf-dev-1.63.7/simba/three_dimensions/outlier_tools/outlier_corrector_movement.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/video_processors/
--rw-r--r--   0 simon      (501) staff       (20)    45563 2023-06-09 13:51:45.000000 Simba-UW-tf-dev-1.63.7/simba/video_processors/video_processing.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-06-17 18:48:42.000000 Simba-UW-tf-dev-1.63.7/simba/video_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.63.7/simba/video_processors/px_to_mm.py
--rw-r--r--   0 simon      (501) staff       (20)    24648 2023-05-16 16:42:04.000000 Simba-UW-tf-dev-1.63.7/simba/video_processors/batch_process_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     7333 2023-05-16 12:54:28.000000 Simba-UW-tf-dev-1.63.7/simba/video_processors/multi_cropper.py
--rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.63.7/simba/video_processors/extract_frames.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/video_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8266 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.63.7/simba/video_processors/calculate_px_dist.py
--rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.63.7/simba/video_processors/extract_seqframes.py
--rw-r--r--   0 simon      (501) staff       (20)    11087 2023-05-14 16:24:59.000000 Simba-UW-tf-dev-1.63.7/simba/video_processors/batch_process_create_ffmpeg_commands.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6535 2023-05-25 14:24:01.000000 Simba-UW-tf-dev-1.63.7/simba/outlier_tools/outlier_corrector_movement.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:37.000000 Simba-UW-tf-dev-1.63.7/simba/outlier_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/outlier_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8168 2023-06-01 12:38:34.000000 Simba-UW-tf-dev-1.63.7/simba/outlier_tools/outlier_corrector_location.py
--rw-r--r--   0 simon      (501) staff       (20)     2668 2023-05-25 14:26:49.000000 Simba-UW-tf-dev-1.63.7/simba/outlier_tools/skip_outlier_correction.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/outlier_tools/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/outlier_tools/.idea/outlier_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/outlier_tools/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/outlier_tools/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/outlier_tools/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/outlier_tools/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/outlier_tools/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/outlier_tools/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/outlier_tools/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    66068 2023-06-20 18:58:45.000000 Simba-UW-tf-dev-1.63.7/simba/SimBA.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:38.000000 Simba-UW-tf-dev-1.63.7/simba/assets/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/simba/assets/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/unsupervised/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/unsupervised/features.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:38.000000 Simba-UW-tf-dev-1.63.7/simba/assets/shap/
--rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/shap/down_arrow.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/shap/intruder_shape.jpg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:38.000000 Simba-UW-tf-dev-1.63.7/simba/assets/shap/feature_categories/
--rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
--rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/shap/feature_categories/shap_feature_categories.csv
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-06-15 21:18:05.000000 Simba-UW-tf-dev-1.63.7/simba/assets/shap/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/shap/resident_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/shap/resident_intruder_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/shap/animal_distances.jpg
--rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/shap/baseline_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/shap/ubuntu.regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/shap/side_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/shap/UbuntuMono-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/shap/side_scale_5.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/shap/intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/shap/resident_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/shap/color_bar.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/shap/resident_intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)    16388 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.63.7/simba/assets/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:38.000000 Simba-UW-tf-dev-1.63.7/simba/assets/lookups/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/lookups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/lookups/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.63.7/simba/assets/lookups/feature_extraction_headers.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/lookups/features.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/lookups/unsupervised_example_x.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:38.000000 Simba-UW-tf-dev-1.63.7/simba/assets/stl/
--rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/stl/operant_tray.stl
--rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/stl/operant_lever.stl
--rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/stl/operant_walls.stl
--rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/stl/grid_floor.stl
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:38.000000 Simba-UW-tf-dev-1.63.7/simba/assets/img/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.63.7/simba/assets/img/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/img/about_me.png
--rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.63.7/simba/assets/img/splash.mp4
--rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.63.7/simba/assets/img/bg_2.png
--rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/img/splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.63.7/simba/assets/img/bg.png
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/UbuntuMono-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:38.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/
--rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/factory.png
--rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/cluster.png
--rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/load.png
--rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/gif.png
--rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/pose.png
--rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/features.png
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/.DS_Store
--rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/settings.png
--rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/stopwatch.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/link.png
--rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/dash_simba.css
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/documentation.png
--rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/fps.png
--rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/dimensionality_reduction.png
--rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/roi.png
--rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/superimpose.png
--rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/label.png
--rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/change.png
--rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/crop.png
--rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/rotate.png
--rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/path.png
--rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/clip.png
--rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/restart.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/calipher.png
--rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/add_on.png
--rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/create.png
--rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/SimBA_logo.ico
--rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/print.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/clf.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:38.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/concat_icons/
--rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/concat_icons/mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/concat_icons/vertical.png
--rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/concat_icons/horizontal.png
--rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/concat_icons/mixed_mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/merge.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/clean.png
--rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/clf_2.png
--rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/visualize.png
--rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/concat.png
--rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/boris.png
--rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/frames.png
--rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/video.png
--rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/sample.png
--rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/metrics.png
--rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/grey.png
--rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/exit.png
--rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/outlier.png
--rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/clahe.png
--rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/trash.png
--rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/about.png
--rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/convert.png
--rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/SimBA_logo.icns
--rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/reorganize.png
--rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/browse.png
--rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/SimBA_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/ethovision.png
--rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.63.7/simba/assets/icons/close.png
--rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/dash_simba_base.css
--rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.7/simba/assets/TheGoldenLab.PNG
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:38.000000 Simba-UW-tf-dev-1.63.7/Simba_UW_tf_dev.egg-info/
--rw-rw-r--   0 simon      (501) staff       (20)      579 2023-06-29 19:37:38.000000 Simba-UW-tf-dev-1.63.7/Simba_UW_tf_dev.egg-info/PKG-INFO
--rw-rw-r--   0 simon      (501) staff       (20)    21589 2023-06-29 19:37:38.000000 Simba-UW-tf-dev-1.63.7/Simba_UW_tf_dev.egg-info/SOURCES.txt
--rw-rw-r--   0 simon      (501) staff       (20)       44 2023-06-29 19:37:38.000000 Simba-UW-tf-dev-1.63.7/Simba_UW_tf_dev.egg-info/entry_points.txt
--rw-rw-r--   0 simon      (501) staff       (20)      639 2023-06-29 19:37:38.000000 Simba-UW-tf-dev-1.63.7/Simba_UW_tf_dev.egg-info/requires.txt
--rw-rw-r--   0 simon      (501) staff       (20)       12 2023-06-29 19:37:38.000000 Simba-UW-tf-dev-1.63.7/Simba_UW_tf_dev.egg-info/top_level.txt
--rw-rw-r--   0 simon      (501) staff       (20)        1 2023-06-29 19:37:38.000000 Simba-UW-tf-dev-1.63.7/Simba_UW_tf_dev.egg-info/dependency_links.txt
--rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.63.7/LICENSE.md
--rw-r--r--   0 simon      (501) staff       (20)       89 2023-05-20 17:55:56.000000 Simba-UW-tf-dev-1.63.7/pyproject.toml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/tests/
--rw-r--r--   0 simon      (501) staff       (20)     5209 2023-05-28 14:15:24.000000 Simba-UW-tf-dev-1.63.7/tests/test_data_processors.py
--rw-r--r--   0 simon      (501) staff       (20)     5317 2023-05-31 19:40:16.000000 Simba-UW-tf-dev-1.63.7/tests/test_distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-13 13:57:45.000000 Simba-UW-tf-dev-1.63.7/tests/test_interpolation_smoothing.py
--rw-r--r--   0 simon      (501) staff       (20)    12374 2023-06-07 20:44:17.000000 Simba-UW-tf-dev-1.63.7/tests/test_train_model_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     2470 2023-06-12 20:51:29.000000 Simba-UW-tf-dev-1.63.7/tests/test_pose_importers.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.7/tests/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6757 2023-06-02 12:11:53.000000 Simba-UW-tf-dev-1.63.7/tests/test_feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-12 20:53:51.000000 Simba-UW-tf-dev-1.63.7/tests/test_pose_processors.py
--rw-r--r--   0 simon      (501) staff       (20)     1774 2023-06-13 19:27:04.000000 Simba-UW-tf-dev-1.63.7/tests/test_utils_data.py
--rw-r--r--   0 simon      (501) staff       (20)     8984 2023-06-07 20:11:11.000000 Simba-UW-tf-dev-1.63.7/tests/test_config_reader_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     1528 2023-05-25 14:26:19.000000 Simba-UW-tf-dev-1.63.7/tests/test_outlier_correctors.py
--rw-r--r--   0 simon      (501) staff       (20)     4356 2023-05-29 20:59:49.000000 Simba-UW-tf-dev-1.63.7/tests/test_visualize_directing_animals.py
--rw-r--r--   0 simon      (501) staff       (20)     1859 2023-05-21 16:40:19.000000 Simba-UW-tf-dev-1.63.7/tests/test_featurizers.py
--rw-r--r--   0 simon      (501) staff       (20)     8736 2023-06-13 13:49:50.000000 Simba-UW-tf-dev-1.63.7/tests/test_video_processors.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/tests/data/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.7/tests/data/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/two_c57/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/two_c57/video_processing/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/two_c57/video_processing/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/two_c57/video_processing/test_imgs/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/two_c57/video_processing/test_imgs/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/two_c57/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/two_c57/models/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/two_c57/models/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/two_c57/expected_animal_bp_dict/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/two_c57/expected_animal_bp_dict/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/mouse_open_field/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/mouse_open_field/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/zebrafish/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/zebrafish/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/zebrafish/models/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/zebrafish/models/generated_models/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/zebrafish/models/generated_models/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/zebrafish/models/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/zebrafish/models/validations/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/zebrafish/models/validations/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/zebrafish/project_folder/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/zebrafish/project_folder/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/zebrafish/project_folder/videos/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/zebrafish/project_folder/videos/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/zebrafish/project_folder/logs/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/zebrafish/project_folder/logs/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/zebrafish/project_folder/logs/measures/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/zebrafish/project_folder/logs/measures/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/zebrafish/feature_file/
--rw-rw-r--   0 simon      (501) staff       (20)        0 2020-08-11 16:11:18.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/zebrafish/feature_file/__init__.py
--rw-rw-r--   0 simon      (501) staff       (20)    14128 2022-04-11 08:07:36.000000 Simba-UW-tf-dev-1.63.7/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py
--rw-r--r--   0 simon      (501) staff       (20)     3971 2023-05-28 17:20:18.000000 Simba-UW-tf-dev-1.63.7/tests/test_thirdparty_appenders.py
--rw-r--r--   0 simon      (501) staff       (20)     3090 2023-05-31 15:49:24.000000 Simba-UW-tf-dev-1.63.7/tests/test_validation_clips.py
--rw-r--r--   0 simon      (501) staff       (20)     4463 2023-06-12 18:41:18.000000 Simba-UW-tf-dev-1.63.7/tests/test_roi_tools.py
--rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.63.7/MANIFEST.in
--rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.63.7/README.md
--rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-06-29 19:37:32.000000 Simba-UW-tf-dev-1.63.7/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-06-29 19:37:39.000000 Simba-UW-tf-dev-1.63.7/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/ui/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-07-03 15:11:10.000000 Simba-UW-tf-dev-1.63.8/simba/ui/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/
+-rw-r--r--   0 simon      (501) staff       (20)     9015 2023-06-29 20:55:17.000000 Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/mutual_exclusivity_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/csv_2_parquet_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2343 2023-05-17 20:47:45.000000 Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/quick_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/batch_preprocess_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8342 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/heatmap_location_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/clf_probability_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:42.000000 Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/movement_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9471 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/clf_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    15950 2023-05-20 12:10:35.000000 Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1150 2023-05-25 18:21:39.000000 Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/remove_roi_features_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5814 2023-06-15 20:06:37.000000 Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/roi_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5977 2023-05-31 12:58:14.000000 Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/outlier_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/gantt_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/clf_validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7721 2023-05-24 15:18:33.000000 Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/severity_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/fsttc_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4052 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/kleinberg_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7288 2023-05-29 20:14:50.000000 Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5425 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/pose_reorganizer_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/clf_by_timebins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8673 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/heatmap_clf_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/data_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7860 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/roi_features_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/pup_retrieval_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/about_simba_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3605 2023-05-25 18:54:56.000000 Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6353 2023-05-24 15:31:12.000000 Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    42791 2023-07-03 16:15:16.000000 Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/video_processing_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7535 2023-05-15 13:09:04.000000 Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/clf_by_roi_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/make_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/archive_files_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4087 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/pose_bp_drop_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    10695 2023-05-31 16:42:04.000000 Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/distance_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3601 2023-07-03 00:19:12.000000 Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    12869 2023-05-23 12:47:59.000000 Simba-UW-tf-dev-1.63.8/simba/ui/video_info_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     6019 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.63.8/simba/ui/user_defined_pose_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/ui/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    12879 2023-06-18 20:27:37.000000 Simba-UW-tf-dev-1.63.8/simba/ui/create_project_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.63.8/simba/ui/tkinter_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    35431 2023-06-13 17:24:57.000000 Simba-UW-tf-dev-1.63.8/simba/ui/machine_model_settings_ui.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/blob_storage/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.63.8/simba/blob_storage/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/labelling/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.63.8/simba/labelling/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21667 2023-06-20 18:30:00.000000 Simba-UW-tf-dev-1.63.8/simba/labelling/labelling_interface_old.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/labelling/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    20914 2023-06-22 13:26:28.000000 Simba-UW-tf-dev-1.63.8/simba/labelling/labelling_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     3568 2023-05-19 11:18:49.000000 Simba-UW-tf-dev-1.63.8/simba/labelling/extract_labelled_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)    26943 2023-06-20 19:04:35.000000 Simba-UW-tf-dev-1.63.8/simba/labelling/labelling_advanced_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     6629 2023-05-13 17:45:08.000000 Simba-UW-tf-dev-1.63.8/simba/labelling/play_annotation_video.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)    11877 2023-05-17 14:59:39.000000 Simba-UW-tf-dev-1.63.8/simba/unsupervised/dbcv_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.63.8/simba/unsupervised/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-13 17:25:39.000000 Simba-UW-tf-dev-1.63.8/simba/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     8141 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.63.8/simba/unsupervised/dataset_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5636 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.63.8/simba/unsupervised/grid_search_visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     7310 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.63.8/simba/unsupervised/data_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     9846 2023-06-06 18:27:30.000000 Simba-UW-tf-dev-1.63.8/simba/unsupervised/ui.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/unsupervised/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     9851 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.63.8/simba/unsupervised/umap_embedder.py
+-rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.63.8/simba/unsupervised/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)     2931 2023-05-17 14:54:38.000000 Simba-UW-tf-dev-1.63.8/simba/unsupervised/bout_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20846 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.63.8/simba/unsupervised/cluster_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.63.8/simba/unsupervised/data_map.yaml
+-rw-r--r--   0 simon      (501) staff       (20)    10287 2023-06-06 17:50:12.000000 Simba-UW-tf-dev-1.63.8/simba/unsupervised/hdbscan_clusterer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.63.8/simba/unsupervised/tsne.py
+-rw-r--r--   0 simon      (501) staff       (20)     6656 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.63.8/simba/unsupervised/cluster_visualizer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/bounding_box_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.63.8/simba/bounding_box_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/bounding_box_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7031 2023-05-14 18:13:04.000000 Simba-UW-tf-dev-1.63.8/simba/bounding_box_tools/agg_boundary_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    23566 2023-05-14 18:29:41.000000 Simba-UW-tf-dev-1.63.8/simba/bounding_box_tools/boundary_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     8497 2023-05-14 18:22:39.000000 Simba-UW-tf-dev-1.63.8/simba/bounding_box_tools/boundary_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     6376 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.8/simba/bounding_box_tools/find_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    11381 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.8/simba/bounding_box_tools/visualize_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    49156 2023-07-03 15:11:15.000000 Simba-UW-tf-dev-1.63.8/simba/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)    42512 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/feature_extractor_14bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21482 2023-05-14 23:55:56.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/feature_extractor_7bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     7127 2023-05-28 19:41:35.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-07 20:28:11.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     8943 2023-06-05 18:15:28.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/shap_log_mp_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8580 2023-05-31 20:02:32.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/shap_log_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)    30764 2023-06-13 17:23:34.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
+-rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/time_stamp_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     4279 2023-06-01 12:49:14.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/read_files_mp_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:44:29.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    27995 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/feature_extractor_8bps_2_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-06-29 20:33:26.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3864 2023-05-19 19:41:40.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/perimeter_jit.py
+-rw-r--r--   0 simon      (501) staff       (20)    17857 2023-07-03 15:15:20.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/feature_subsets.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8244 2023-05-21 16:28:49.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/feature_extractor_user_defined.py
+-rw-r--r--   0 simon      (501) staff       (20)    46461 2023-05-15 00:03:36.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/feature_extractor_16bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    28259 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/feature_extractor_9bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    23976 2023-05-15 00:01:21.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/feature_extractor_8bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16880 2023-05-14 23:53:59.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/feature_extractor_4bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/.idea/features_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/.idea/.gitignore
+-rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/.idea/.name
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/feature_extractors/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    15434 2023-05-20 18:29:53.000000 Simba-UW-tf-dev-1.63.8/simba/requirements.txt
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-07-02 23:47:13.000000 Simba-UW-tf-dev-1.63.8/simba/mixins/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43029 2023-06-05 17:40:09.000000 Simba-UW-tf-dev-1.63.8/simba/mixins/pop_up_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    38224 2023-06-15 15:41:52.000000 Simba-UW-tf-dev-1.63.8/simba/mixins/config_reader.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/mixins/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18616 2023-05-17 19:39:33.000000 Simba-UW-tf-dev-1.63.8/simba/mixins/pose_importer_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     2938 2023-07-02 20:03:29.000000 Simba-UW-tf-dev-1.63.8/simba/mixins/video_processing_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/mixins/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-06-01 18:12:36.000000 Simba-UW-tf-dev-1.63.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.63.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2023-06-01 14:35:51.000000 Simba-UW-tf-dev-1.63.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    82442 2023-06-01 18:12:36.000000 Simba-UW-tf-dev-1.63.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    51809 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.63.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    14391 2023-06-01 14:35:51.000000 Simba-UW-tf-dev-1.63.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.2.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    14188 2023-05-21 00:18:56.000000 Simba-UW-tf-dev-1.63.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    37135 2023-06-02 12:12:15.000000 Simba-UW-tf-dev-1.63.8/simba/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    61873 2023-05-19 21:14:46.000000 Simba-UW-tf-dev-1.63.8/simba/mixins/plotting_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     9145 2023-06-13 18:36:10.000000 Simba-UW-tf-dev-1.63.8/simba/mixins/unsupervised_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    73291 2023-06-19 20:46:57.000000 Simba-UW-tf-dev-1.63.8/simba/mixins/train_model_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/third_party_label_appenders/
+-rw-r--r--   0 simon      (501) staff       (20)     6094 2023-05-21 17:39:19.000000 Simba-UW-tf-dev-1.63.8/simba/third_party_label_appenders/deepethogram_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10759 2023-06-08 22:23:03.000000 Simba-UW-tf-dev-1.63.8/simba/third_party_label_appenders/BORIS_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8998 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.63.8/simba/third_party_label_appenders/observer_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.63.8/simba/third_party_label_appenders/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    18417 2023-06-18 19:01:16.000000 Simba-UW-tf-dev-1.63.8/simba/third_party_label_appenders/tools.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.63.8/simba/third_party_label_appenders/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18934 2023-06-18 19:03:04.000000 Simba-UW-tf-dev-1.63.8/simba/third_party_label_appenders/third_party_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8181 2023-05-21 17:19:25.000000 Simba-UW-tf-dev-1.63.8/simba/third_party_label_appenders/ethovision_import.py
+-rw-r--r--   0 simon      (501) staff       (20)     6988 2023-05-21 17:31:04.000000 Simba-UW-tf-dev-1.63.8/simba/third_party_label_appenders/BENTO_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     5239 2023-05-21 18:07:18.000000 Simba-UW-tf-dev-1.63.8/simba/third_party_label_appenders/solomon_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/cue_light_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.63.8/simba/cue_light_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7652 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.8/simba/cue_light_tools/cue_light_clf_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    12207 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.8/simba/cue_light_tools/cue_light_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16690 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.8/simba/cue_light_tools/cue_light_menues.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/cue_light_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1879 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.8/simba/cue_light_tools/cue_light_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    15212 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.63.8/simba/cue_light_tools/cue_light_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12650 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.8/simba/cue_light_tools/cue_light_movement_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/utils/
+-rw-r--r--   0 simon      (501) staff       (20)    11876 2023-06-18 20:21:39.000000 Simba-UW-tf-dev-1.63.8/simba/utils/config_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    21103 2023-06-20 12:58:32.000000 Simba-UW-tf-dev-1.63.8/simba/utils/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.63.8/simba/utils/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7698 2023-07-03 16:08:55.000000 Simba-UW-tf-dev-1.63.8/simba/utils/warnings.py
+-rw-r--r--   0 simon      (501) staff       (20)     8807 2023-05-25 13:24:45.000000 Simba-UW-tf-dev-1.63.8/simba/utils/checks.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/utils/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    43313 2023-06-27 15:38:38.000000 Simba-UW-tf-dev-1.63.8/simba/utils/read_write.py
+-rw-r--r--   0 simon      (501) staff       (20)     9841 2023-06-19 23:24:08.000000 Simba-UW-tf-dev-1.63.8/simba/utils/lookups.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/utils/cli/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/utils/cli/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6017 2023-05-28 13:41:20.000000 Simba-UW-tf-dev-1.63.8/simba/utils/cli/cli_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    14886 2023-07-03 16:08:55.000000 Simba-UW-tf-dev-1.63.8/simba/utils/errors.py
+-rw-r--r--   0 simon      (501) staff       (20)    19250 2023-06-13 13:46:20.000000 Simba-UW-tf-dev-1.63.8/simba/utils/data.py
+-rw-r--r--   0 simon      (501) staff       (20)     1615 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.63.8/simba/utils/printing.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/st/
+-rw-r--r--   0 simon      (501) staff       (20)      282 2023-06-16 17:26:25.000000 Simba-UW-tf-dev-1.63.8/simba/st/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-16 13:55:39.000000 Simba-UW-tf-dev-1.63.8/simba/st/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2102 2023-06-19 19:54:19.000000 Simba-UW-tf-dev-1.63.8/simba/st/select_groups_pg.py
+-rw-r--r--   0 simon      (501) staff       (20)     2325 2023-06-19 19:54:19.000000 Simba-UW-tf-dev-1.63.8/simba/st/aggregate_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     1485 2023-06-16 18:20:31.000000 Simba-UW-tf-dev-1.63.8/simba/st/app.py
+-rw-r--r--   0 simon      (501) staff       (20)      249 2023-06-16 18:20:19.000000 Simba-UW-tf-dev-1.63.8/simba/st/welcome_page.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/pose_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     8256 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.63.8/simba/pose_processors/reorganize_keypoint.py
+-rw-r--r--   0 simon      (501) staff       (20)     5167 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.63.8/simba/pose_processors/remove_keypoints.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.63.8/simba/pose_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/pose_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2656 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.63.8/simba/pose_processors/pose_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)     5618 2023-06-13 18:36:10.000000 Simba-UW-tf-dev-1.63.8/simba/pose_processors/reverse_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     9114 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.63.8/simba/plotting/gantt_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/plotting/tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.63.8/simba/plotting/tools/tkinter_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    13008 2023-05-24 15:32:44.000000 Simba-UW-tf-dev-1.63.8/simba/plotting/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.63.8/simba/plotting/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    14568 2023-05-15 18:41:17.000000 Simba-UW-tf-dev-1.63.8/simba/plotting/shap_agg_stats_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10105 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.63.8/simba/plotting/gantt_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15730 2023-05-15 17:49:01.000000 Simba-UW-tf-dev-1.63.8/simba/plotting/heat_mapper_clf_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8731 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.63.8/simba/plotting/probability_plot_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12484 2023-05-23 14:52:24.000000 Simba-UW-tf-dev-1.63.8/simba/plotting/plot_clf_results.py
+-rw-r--r--   0 simon      (501) staff       (20)    14056 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.63.8/simba/plotting/plot_clf_results_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16031 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.63.8/simba/plotting/ROI_feature_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12770 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.63.8/simba/plotting/heat_mapper_location.py
+-rw-r--r--   0 simon      (501) staff       (20)    10100 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.63.8/simba/plotting/probability_plot_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/plotting/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     4881 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.63.8/simba/plotting/interactive_probability_grapher.py
+-rw-r--r--   0 simon      (501) staff       (20)    14029 2023-06-04 11:55:47.000000 Simba-UW-tf-dev-1.63.8/simba/plotting/single_run_model_validation_video.py
+-rw-r--r--   0 simon      (501) staff       (20)    12790 2023-05-16 16:20:20.000000 Simba-UW-tf-dev-1.63.8/simba/plotting/frame_mergerer_ffmpeg.py
+-rw-r--r--   0 simon      (501) staff       (20)     7660 2023-06-20 12:45:11.000000 Simba-UW-tf-dev-1.63.8/simba/plotting/pose_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     7891 2023-05-29 21:41:05.000000 Simba-UW-tf-dev-1.63.8/simba/plotting/Directing_animals_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11219 2023-05-17 12:58:17.000000 Simba-UW-tf-dev-1.63.8/simba/plotting/clf_validator.py
+-rw-r--r--   0 simon      (501) staff       (20)    15745 2023-05-20 12:16:06.000000 Simba-UW-tf-dev-1.63.8/simba/plotting/path_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11203 2023-05-24 15:35:24.000000 Simba-UW-tf-dev-1.63.8/simba/plotting/ROI_feature_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8933 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.63.8/simba/plotting/data_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13471 2023-05-20 12:15:46.000000 Simba-UW-tf-dev-1.63.8/simba/plotting/path_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     6494 2023-05-17 20:55:17.000000 Simba-UW-tf-dev-1.63.8/simba/plotting/ez_lineplot.py
+-rw-r--r--   0 simon      (501) staff       (20)    11519 2023-05-31 16:42:04.000000 Simba-UW-tf-dev-1.63.8/simba/plotting/distance_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15794 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.63.8/simba/plotting/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13163 2023-05-16 16:42:03.000000 Simba-UW-tf-dev-1.63.8/simba/plotting/heat_mapper_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)     9385 2023-05-31 16:46:49.000000 Simba-UW-tf-dev-1.63.8/simba/plotting/distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     9526 2023-06-04 12:03:25.000000 Simba-UW-tf-dev-1.63.8/simba/plotting/single_run_model_validation_video_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    10005 2023-05-29 21:36:37.000000 Simba-UW-tf-dev-1.63.8/simba/plotting/Directing_animals_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16320 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.63.8/simba/plotting/heat_mapper_location_mp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/dash_app/
+-rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/dash_app/SimBA_dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/dash_app/run_dash_tkinter.py
+-rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/dash_app/dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-16 12:50:41.000000 Simba-UW-tf-dev-1.63.8/simba/dash_app/plotly_dash.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/data_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     7248 2023-05-25 19:01:00.000000 Simba-UW-tf-dev-1.63.8/simba/data_processors/agg_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.63.8/simba/data_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    11196 2023-05-28 19:50:35.000000 Simba-UW-tf-dev-1.63.8/simba/data_processors/severity_bout_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16285 2023-06-13 13:57:45.000000 Simba-UW-tf-dev-1.63.8/simba/data_processors/interpolation_smoothing.py
+-rw-r--r--   0 simon      (501) staff       (20)     8127 2023-05-25 13:57:19.000000 Simba-UW-tf-dev-1.63.8/simba/data_processors/timebins_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    13451 2023-06-19 20:47:55.000000 Simba-UW-tf-dev-1.63.8/simba/data_processors/fsttc_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/data_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6306 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.63.8/simba/data_processors/interpolate_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)     9646 2023-05-14 19:19:14.000000 Simba-UW-tf-dev-1.63.8/simba/data_processors/directing_other_animals_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8624 2023-05-25 14:07:56.000000 Simba-UW-tf-dev-1.63.8/simba/data_processors/timebins_movement_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4799 2023-05-17 17:23:16.000000 Simba-UW-tf-dev-1.63.8/simba/data_processors/severity_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16980 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.63.8/simba/data_processors/pup_retrieval_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-13 17:23:00.000000 Simba-UW-tf-dev-1.63.8/simba/data_processors/pybursts_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    11533 2023-05-28 19:50:34.000000 Simba-UW-tf-dev-1.63.8/simba/data_processors/severity_frame_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     6087 2023-06-28 20:32:32.000000 Simba-UW-tf-dev-1.63.8/simba/data_processors/mutual_exclusivity_corrector.py
+-rw-r--r--   0 simon      (501) staff       (20)     9656 2023-05-25 13:32:25.000000 Simba-UW-tf-dev-1.63.8/simba/data_processors/kleinberg_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8131 2023-05-25 14:37:36.000000 Simba-UW-tf-dev-1.63.8/simba/data_processors/movement_calculator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:45.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations_archive/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations_archive/pose_configurations_archive_1/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/model/
+-rw-r--r--   0 simon      (501) staff       (20)    20086 2023-06-05 20:43:28.000000 Simba-UW-tf-dev-1.63.8/simba/model/train_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.63.8/simba/model/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3315 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.63.8/simba/model/inference_batch.py
+-rw-r--r--   0 simon      (501) staff       (20)    20849 2023-06-05 18:44:40.000000 Simba-UW-tf-dev-1.63.8/simba/model/grid_search_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3363 2023-05-19 11:12:45.000000 Simba-UW-tf-dev-1.63.8/simba/model/inference_validation.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/roi_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5858 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.63.8/simba/roi_tools/ROI_time_bin_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1687 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.63.8/simba/roi_tools/ROI_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.63.8/simba/roi_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43194 2023-06-22 13:51:00.000000 Simba-UW-tf-dev-1.63.8/simba/roi_tools/ROI_define.py
+-rw-r--r--   0 simon      (501) staff       (20)     4024 2023-05-16 13:21:43.000000 Simba-UW-tf-dev-1.63.8/simba/roi_tools/ROI_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/roi_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    20174 2023-06-12 15:28:58.000000 Simba-UW-tf-dev-1.63.8/simba/roi_tools/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11608 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.63.8/simba/roi_tools/ROI_feature_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.63.8/simba/roi_tools/ROI_multiply.py
+-rw-r--r--   0 simon      (501) staff       (20)     2290 2023-06-12 16:21:03.000000 Simba-UW-tf-dev-1.63.8/simba/roi_tools/ROI_size_calculations.py
+-rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/roi_tools/ROI_zoom.py
+-rw-r--r--   0 simon      (501) staff       (20)    11474 2023-06-12 19:37:22.000000 Simba-UW-tf-dev-1.63.8/simba/roi_tools/ROI_directing_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/roi_tools/ROI_move_shape.py
+-rw-r--r--   0 simon      (501) staff       (20)     5080 2023-06-22 13:37:25.000000 Simba-UW-tf-dev-1.63.8/simba/roi_tools/ROI_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    13742 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.63.8/simba/roi_tools/ROI_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.63.8/simba/roi_tools/ROI_image.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)     8115 2023-05-14 18:03:14.000000 Simba-UW-tf-dev-1.63.8/simba/pose_importers/sleap_csv_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/pose_importers/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:42:38.000000 Simba-UW-tf-dev-1.63.8/simba/pose_importers/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.63.8/simba/pose_importers/misc/apt_trk_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.63.8/simba/pose_importers/read_DANNCE_mat.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.63.8/simba/pose_importers/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    12549 2023-05-17 20:32:56.000000 Simba-UW-tf-dev-1.63.8/simba/pose_importers/sleap_h5_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7322 2023-05-16 16:55:05.000000 Simba-UW-tf-dev-1.63.8/simba/pose_importers/madlc_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/pose_importers/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    12141 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.63.8/simba/pose_importers/sleap_slp_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7931 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.63.8/simba/pose_importers/import_mars.py
+-rw-r--r--   0 simon      (501) staff       (20)     6978 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.63.8/simba/pose_importers/dlc_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.63.8/simba/pose_importers/trk_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-05-14 23:57:00.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/pose_configurations/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:45.000000 Simba-UW-tf-dev-1.63.8/simba/three_dimensions/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/three_dimensions/ui/
+-rw-r--r--   0 simon      (501) staff       (20)     1747 2023-06-25 18:18:01.000000 Simba-UW-tf-dev-1.63.8/simba/three_dimensions/ui/define_px_to_mm_ui.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/three_dimensions/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)     6777 2023-06-26 17:04:03.000000 Simba-UW-tf-dev-1.63.8/simba/three_dimensions/feature_extractors/generic_feature_extractor.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/three_dimensions/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)    38820 2023-06-23 01:28:48.000000 Simba-UW-tf-dev-1.63.8/simba/three_dimensions/mixins/config_reader.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/three_dimensions/mixins/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)    51001 2023-06-26 13:52:31.000000 Simba-UW-tf-dev-1.63.8/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    50997 2023-06-25 19:59:06.000000 Simba-UW-tf-dev-1.63.8/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1380 2023-06-26 13:52:31.000000 Simba-UW-tf-dev-1.63.8/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     1379 2023-06-25 19:59:06.000000 Simba-UW-tf-dev-1.63.8/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     3758 2023-06-26 13:45:44.000000 Simba-UW-tf-dev-1.63.8/simba/three_dimensions/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     3953 2023-06-25 18:18:01.000000 Simba-UW-tf-dev-1.63.8/simba/three_dimensions/mixins/plotting_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/three_dimensions/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     3192 2023-06-25 18:21:24.000000 Simba-UW-tf-dev-1.63.8/simba/three_dimensions/plotting/plot_pose_in_dir.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/three_dimensions/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)     3445 2023-06-22 22:21:05.000000 Simba-UW-tf-dev-1.63.8/simba/three_dimensions/pose_importers/anipose_csv_import.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/three_dimensions/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5832 2023-06-23 13:06:19.000000 Simba-UW-tf-dev-1.63.8/simba/three_dimensions/outlier_tools/outlier_corrector_movement.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/video_processors/
+-rw-r--r--   0 simon      (501) staff       (20)    47201 2023-07-03 16:33:39.000000 Simba-UW-tf-dev-1.63.8/simba/video_processors/video_processing.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-06-17 18:48:42.000000 Simba-UW-tf-dev-1.63.8/simba/video_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.63.8/simba/video_processors/px_to_mm.py
+-rw-r--r--   0 simon      (501) staff       (20)    24648 2023-05-16 16:42:04.000000 Simba-UW-tf-dev-1.63.8/simba/video_processors/batch_process_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     3748 2023-07-02 21:12:43.000000 Simba-UW-tf-dev-1.63.8/simba/video_processors/video_processing_new.py
+-rw-r--r--   0 simon      (501) staff       (20)     7333 2023-05-16 12:54:28.000000 Simba-UW-tf-dev-1.63.8/simba/video_processors/multi_cropper.py
+-rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.63.8/simba/video_processors/extract_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/video_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8266 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.63.8/simba/video_processors/calculate_px_dist.py
+-rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.63.8/simba/video_processors/extract_seqframes.py
+-rw-r--r--   0 simon      (501) staff       (20)    11087 2023-05-14 16:24:59.000000 Simba-UW-tf-dev-1.63.8/simba/video_processors/batch_process_create_ffmpeg_commands.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6535 2023-05-25 14:24:01.000000 Simba-UW-tf-dev-1.63.8/simba/outlier_tools/outlier_corrector_movement.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:37.000000 Simba-UW-tf-dev-1.63.8/simba/outlier_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/outlier_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8168 2023-06-01 12:38:34.000000 Simba-UW-tf-dev-1.63.8/simba/outlier_tools/outlier_corrector_location.py
+-rw-r--r--   0 simon      (501) staff       (20)     2668 2023-05-25 14:26:49.000000 Simba-UW-tf-dev-1.63.8/simba/outlier_tools/skip_outlier_correction.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/outlier_tools/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/outlier_tools/.idea/outlier_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/outlier_tools/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/outlier_tools/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/outlier_tools/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/outlier_tools/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/outlier_tools/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/outlier_tools/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/outlier_tools/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    66374 2023-06-29 20:30:38.000000 Simba-UW-tf-dev-1.63.8/simba/SimBA.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/assets/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/assets/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/assets/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/assets/unsupervised/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/assets/unsupervised/features.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/assets/shap/
+-rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/assets/shap/down_arrow.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/assets/shap/intruder_shape.jpg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/assets/shap/feature_categories/
+-rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
+-rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/assets/shap/feature_categories/shap_feature_categories.csv
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-06-15 21:18:05.000000 Simba-UW-tf-dev-1.63.8/simba/assets/shap/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/assets/shap/resident_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/assets/shap/resident_intruder_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/assets/shap/animal_distances.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/assets/shap/baseline_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/assets/shap/ubuntu.regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/assets/shap/side_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/assets/shap/UbuntuMono-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/assets/shap/side_scale_5.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/assets/shap/intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/assets/shap/resident_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/assets/shap/color_bar.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/assets/shap/resident_intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)    16388 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.63.8/simba/assets/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/assets/lookups/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/assets/lookups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/assets/lookups/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.63.8/simba/assets/lookups/feature_extraction_headers.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/assets/lookups/features.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/assets/lookups/unsupervised_example_x.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/assets/stl/
+-rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/assets/stl/operant_tray.stl
+-rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/assets/stl/operant_lever.stl
+-rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/assets/stl/operant_walls.stl
+-rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/assets/stl/grid_floor.stl
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/assets/img/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.63.8/simba/assets/img/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/assets/img/about_me.png
+-rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.63.8/simba/assets/img/splash.mp4
+-rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.63.8/simba/assets/img/bg_2.png
+-rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/assets/img/splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.63.8/simba/assets/img/bg.png
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/assets/UbuntuMono-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/
+-rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/factory.png
+-rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/cluster.png
+-rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/load.png
+-rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/gif.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/pose.png
+-rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/features.png
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/.DS_Store
+-rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/settings.png
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/stopwatch.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/link.png
+-rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/dash_simba.css
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/documentation.png
+-rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/fps.png
+-rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/dimensionality_reduction.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/roi.png
+-rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/superimpose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/label.png
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/change.png
+-rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/crop.png
+-rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/rotate.png
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/path.png
+-rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/clip.png
+-rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/restart.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/calipher.png
+-rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/add_on.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/create.png
+-rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/SimBA_logo.ico
+-rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/print.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/clf.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/concat_icons/
+-rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/concat_icons/mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/concat_icons/vertical.png
+-rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/concat_icons/horizontal.png
+-rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/concat_icons/mixed_mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/merge.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/clean.png
+-rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/clf_2.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/visualize.png
+-rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/concat.png
+-rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/boris.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/frames.png
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/video.png
+-rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/sample.png
+-rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/metrics.png
+-rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/grey.png
+-rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/exit.png
+-rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/outlier.png
+-rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/clahe.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/trash.png
+-rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/about.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/convert.png
+-rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/SimBA_logo.icns
+-rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/reorganize.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/browse.png
+-rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/SimBA_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/ethovision.png
+-rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.63.8/simba/assets/icons/close.png
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/assets/dash_simba_base.css
+-rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.63.8/simba/assets/TheGoldenLab.PNG
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/Simba_UW_tf_dev.egg-info/
+-rw-rw-r--   0 simon      (501) staff       (20)      579 2023-07-03 16:33:45.000000 Simba-UW-tf-dev-1.63.8/Simba_UW_tf_dev.egg-info/PKG-INFO
+-rw-rw-r--   0 simon      (501) staff       (20)    21675 2023-07-03 16:33:45.000000 Simba-UW-tf-dev-1.63.8/Simba_UW_tf_dev.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       44 2023-07-03 16:33:45.000000 Simba-UW-tf-dev-1.63.8/Simba_UW_tf_dev.egg-info/entry_points.txt
+-rw-rw-r--   0 simon      (501) staff       (20)      639 2023-07-03 16:33:45.000000 Simba-UW-tf-dev-1.63.8/Simba_UW_tf_dev.egg-info/requires.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       12 2023-07-03 16:33:45.000000 Simba-UW-tf-dev-1.63.8/Simba_UW_tf_dev.egg-info/top_level.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        1 2023-07-03 16:33:45.000000 Simba-UW-tf-dev-1.63.8/Simba_UW_tf_dev.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.63.8/LICENSE.md
+-rw-r--r--   0 simon      (501) staff       (20)       89 2023-05-20 17:55:56.000000 Simba-UW-tf-dev-1.63.8/pyproject.toml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/tests/
+-rw-r--r--   0 simon      (501) staff       (20)     5209 2023-05-28 14:15:24.000000 Simba-UW-tf-dev-1.63.8/tests/test_data_processors.py
+-rw-r--r--   0 simon      (501) staff       (20)     5317 2023-05-31 19:40:16.000000 Simba-UW-tf-dev-1.63.8/tests/test_distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-13 13:57:45.000000 Simba-UW-tf-dev-1.63.8/tests/test_interpolation_smoothing.py
+-rw-r--r--   0 simon      (501) staff       (20)    12374 2023-06-07 20:44:17.000000 Simba-UW-tf-dev-1.63.8/tests/test_train_model_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     2470 2023-06-12 20:51:29.000000 Simba-UW-tf-dev-1.63.8/tests/test_pose_importers.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.8/tests/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6757 2023-06-02 12:11:53.000000 Simba-UW-tf-dev-1.63.8/tests/test_feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-12 20:53:51.000000 Simba-UW-tf-dev-1.63.8/tests/test_pose_processors.py
+-rw-r--r--   0 simon      (501) staff       (20)     1774 2023-06-13 19:27:04.000000 Simba-UW-tf-dev-1.63.8/tests/test_utils_data.py
+-rw-r--r--   0 simon      (501) staff       (20)     8984 2023-06-07 20:11:11.000000 Simba-UW-tf-dev-1.63.8/tests/test_config_reader_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     1528 2023-05-25 14:26:19.000000 Simba-UW-tf-dev-1.63.8/tests/test_outlier_correctors.py
+-rw-r--r--   0 simon      (501) staff       (20)     4356 2023-05-29 20:59:49.000000 Simba-UW-tf-dev-1.63.8/tests/test_visualize_directing_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)     1859 2023-05-21 16:40:19.000000 Simba-UW-tf-dev-1.63.8/tests/test_featurizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     8736 2023-06-13 13:49:50.000000 Simba-UW-tf-dev-1.63.8/tests/test_video_processors.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/tests/data/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.8/tests/data/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/tests/data/test_projects/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/tests/data/test_projects/two_c57/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/tests/data/test_projects/two_c57/video_processing/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.8/tests/data/test_projects/two_c57/video_processing/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/tests/data/test_projects/two_c57/video_processing/test_imgs/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.8/tests/data/test_projects/two_c57/video_processing/test_imgs/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.8/tests/data/test_projects/two_c57/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/tests/data/test_projects/two_c57/models/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.8/tests/data/test_projects/two_c57/models/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/tests/data/test_projects/two_c57/expected_animal_bp_dict/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.8/tests/data/test_projects/two_c57/expected_animal_bp_dict/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.8/tests/data/test_projects/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/tests/data/test_projects/mouse_open_field/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.8/tests/data/test_projects/mouse_open_field/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/tests/data/test_projects/zebrafish/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.8/tests/data/test_projects/zebrafish/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/tests/data/test_projects/zebrafish/models/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/tests/data/test_projects/zebrafish/models/generated_models/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.8/tests/data/test_projects/zebrafish/models/generated_models/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.8/tests/data/test_projects/zebrafish/models/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/tests/data/test_projects/zebrafish/models/validations/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.8/tests/data/test_projects/zebrafish/models/validations/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/tests/data/test_projects/zebrafish/project_folder/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.8/tests/data/test_projects/zebrafish/project_folder/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/tests/data/test_projects/zebrafish/project_folder/videos/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.8/tests/data/test_projects/zebrafish/project_folder/videos/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/tests/data/test_projects/zebrafish/project_folder/logs/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.8/tests/data/test_projects/zebrafish/project_folder/logs/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/tests/data/test_projects/zebrafish/project_folder/logs/measures/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.63.8/tests/data/test_projects/zebrafish/project_folder/logs/measures/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/tests/data/test_projects/zebrafish/feature_file/
+-rw-rw-r--   0 simon      (501) staff       (20)        0 2020-08-11 16:11:18.000000 Simba-UW-tf-dev-1.63.8/tests/data/test_projects/zebrafish/feature_file/__init__.py
+-rw-rw-r--   0 simon      (501) staff       (20)    14128 2022-04-11 08:07:36.000000 Simba-UW-tf-dev-1.63.8/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py
+-rw-r--r--   0 simon      (501) staff       (20)     3971 2023-05-28 17:20:18.000000 Simba-UW-tf-dev-1.63.8/tests/test_thirdparty_appenders.py
+-rw-r--r--   0 simon      (501) staff       (20)     3090 2023-05-31 15:49:24.000000 Simba-UW-tf-dev-1.63.8/tests/test_validation_clips.py
+-rw-r--r--   0 simon      (501) staff       (20)     4463 2023-06-12 18:41:18.000000 Simba-UW-tf-dev-1.63.8/tests/test_roi_tools.py
+-rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.63.8/MANIFEST.in
+-rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.63.8/README.md
+-rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-07-03 16:33:39.000000 Simba-UW-tf-dev-1.63.8/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-07-03 16:33:46.000000 Simba-UW-tf-dev-1.63.8/setup.cfg
```

### Comparing `Simba-UW-tf-dev-1.63.7/PKG-INFO` & `Simba-UW-tf-dev-1.63.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.63.7
+Version: 1.63.8
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/.DS_Store` & `Simba-UW-tf-dev-1.63.8/simba/ui/.DS_Store`

 * *Files 6% similar despite different names*

```diff
@@ -278,15 +278,15 @@
 00001150: 6261 7208 0809 0809 5f10 197b 7b33 3534  bar....._..{{354
 00001160: 2c20 3132 347d 2c20 7b31 3037 362c 2036  , 124}, {1076, 6
 00001170: 3231 7d7d 0908 1725 313d 4960 6d79 7a7b  21}}...%1=I`myz{
 00001180: 7c7d 7e9a 0000 0000 0000 0101 0000 0000  |}~.............
 00001190: 0000 000f 0000 0000 0000 0000 0000 0000  ................
 000011a0: 0000 009b 0000 0007 0070 006f 0070 005f  .........p.o.p._
 000011b0: 0075 0070 0073 6c67 3153 636f 6d70 0000  .u.p.slg1Scomp..
-000011c0: 0000 000d a80a 0000 0007 0070 006f 0070  ...........p.o.p
+000011c0: 0000 000d e875 0000 0007 0070 006f 0070  .....u.....p.o.p
 000011d0: 005f 0075 0070 0073 6c73 7643 626c 6f62  ._.u.p.slsvCblob
 000011e0: 0000 02b8 6270 6c69 7374 3030 da01 0203  ....bplist00....
 000011f0: 0405 0607 0809 0a0b 0c0d 1848 4948 4a0c  ...........HIHJ.
 00001200: 4c5f 1012 7669 6577 4f70 7469 6f6e 7356  L_..viewOptionsV
 00001210: 6572 7369 6f6e 5f10 0f73 686f 7749 636f  ersion_..showIco
 00001220: 6e50 7265 7669 6577 5763 6f6c 756d 6e73  nPreviewWcolumns
 00001230: 5f10 1163 616c 6375 6c61 7465 416c 6c53  _..calculateAllS
@@ -369,20 +369,20 @@
 00001700: 7b01 7c01 7e01 8701 8801 8a01 8b01 8d01  {.|.~...........
 00001710: 9601 9701 9901 9a01 9c01 a501 a601 a801  ................
 00001720: a901 ab01 b401 b501 b801 b901 bb01 bc01  ................
 00001730: c501 ce01 db01 dc00 0000 0000 0002 0100  ................
 00001740: 0000 0000 0000 4c00 0000 0000 0000 0000  ......L.........
 00001750: 0000 0000 0001 e500 0000 0700 7000 6f00  ............p.o.
 00001760: 7000 5f00 7500 7000 736d 6f44 4462 6c6f  p._.u.p.smoDDblo
-00001770: 6200 0000 08f5 31c6 66d3 1dc5 4100 0000  b.....1.f...A...
+00001770: 6200 0000 0820 7622 c025 29c5 4100 0000  b.... v".%).A...
 00001780: 0700 7000 6f00 7000 5f00 7500 7000 736d  ..p.o.p._.u.p.sm
-00001790: 6f64 4462 6c6f 6200 0000 08f5 31c6 66d3  odDblob.....1.f.
-000017a0: 1dc5 4100 0000 0700 7000 6f00 7000 5f00  ..A.....p.o.p._.
+00001790: 6f64 4462 6c6f 6200 0000 089f 9551 d210  odDblob......Q..
+000017a0: 27c5 4100 0000 0700 7000 6f00 7000 5f00  '.A.....p.o.p._.
 000017b0: 7500 7000 7370 6831 5363 6f6d 7000 0000  u.p.sph1Scomp...
-000017c0: 0000 1300 0000 0000 0700 7000 6f00 7000  ..........p.o.p.
+000017c0: 0000 1350 0000 0000 0700 7000 6f00 7000  ...P......p.o.p.
 000017d0: 5f00 7500 7000 7376 5372 6e6c 6f6e 6700  _.u.p.svSrnlong.
 000017e0: 0000 0100 0000 0000 0000 0000 0000 0000  ................
 000017f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001800: 0000 0000 0000 0003 0000 0000 0000 180b  ................
 00001810: 0000 0045 0000 100b 0000 0000 0000 0000  ...E............
 00001820: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001830: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -497,17 +497,17 @@
 00001f00: 7b01 7c01 7e01 8701 8801 8a01 8b01 8d01  {.|.~...........
 00001f10: 9601 9701 9901 9a01 9c01 a501 a601 a801  ................
 00001f20: a901 ab01 b401 b501 b801 b901 bb01 bc01  ................
 00001f30: c501 ce01 db01 dc00 0000 0000 0002 0100  ................
 00001f40: 0000 0000 0000 4c00 0000 0000 0000 0000  ......L.........
 00001f50: 0000 0000 0001 e500 0000 0700 7000 6f00  ............p.o.
 00001f60: 7000 5f00 7500 7000 736d 6f44 4462 6c6f  p._.u.p.smoDDblo
-00001f70: 6200 0000 08f5 31c6 66d3 1dc5 4100 0000  b.....1.f...A...
+00001f70: 6200 0000 0820 7622 c025 29c5 4100 0000  b.... v".%).A...
 00001f80: 0700 7000 6f00 7000 5f00 7500 7000 736d  ..p.o.p._.u.p.sm
-00001f90: 6f64 4462 6c6f 6200 0000 08f5 31c6 66d3  odDblob.....1.f.
-00001fa0: 1dc5 4100 0000 0700 7000 6f00 7000 5f00  ..A.....p.o.p._.
+00001f90: 6f64 4462 6c6f 6200 0000 089f 9551 d210  odDblob......Q..
+00001fa0: 27c5 4100 0000 0700 7000 6f00 7000 5f00  '.A.....p.o.p._.
 00001fb0: 7500 7000 7370 6831 5363 6f6d 7000 0000  u.p.sph1Scomp...
-00001fc0: 0000 1300 0000 0000 0700 7000 6f00 7000  ..........p.o.p.
+00001fc0: 0000 1350 0000 0000 0700 7000 6f00 7000  ...P......p.o.p.
 00001fd0: 5f00 7500 7000 7376 5372 6e6c 6f6e 6700  _.u.p.svSrnlong.
 00001fe0: 0000 0100 0000 0000 0000 0000 0000 0000  ................
 00001ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002000: 0000 0000                                ....
```

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/mutual_exclusivity_pop_up.py` & `Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/mutual_exclusivity_pop_up.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         if hasattr(self, 'rule_definitions_frame'):
             self.rule_definitions_frame.destroy()
         self.rule_definitions_frame = LabelFrame(self.main_frm, text='RULE DEFINITIONS', font=Formats.LABELFRAME_HEADER_FORMAT.value, pady=5, padx=5)
         self.rule_definitions_frame.grid(row=1, column=0, sticky='NW')
         Label(self.rule_definitions_frame, text='RULE #').grid(row=0, column=0, sticky=NW)
         for cnt, clf_name in enumerate(self.clf_names):
             Label(self.rule_definitions_frame, text=clf_name).grid(row=0, column=cnt+1, sticky=NW)
-        Label(self.rule_definitions_frame, text='DETERMINATOR').grid(row=0, column=self.clf_cnt + 1, sticky=NW)
+        Label(self.rule_definitions_frame, text='WINNER').grid(row=0, column=self.clf_cnt + 1, sticky=NW)
         Label(self.rule_definitions_frame, text='THRESHOLD').grid(row=0, column=self.clf_cnt + 2, sticky=NW)
         Label(self.rule_definitions_frame, text='HIGHEST PROBABILITY').grid(row=0, column=self.clf_cnt + 3, sticky=NW)
         Label(self.rule_definitions_frame, text='TIE BREAK').grid(row=0, column=self.clf_cnt + 4, sticky=NW)
         Label(self.rule_definitions_frame, text='SKIP ON EQUAL').grid(row=0, column=self.clf_cnt + 5, sticky=NW)
 
         self.rules_dict = {}
         for rule_cnt in range(1, rules_cnt+1):
@@ -125,9 +125,9 @@
                     InvalidInputError(msg=f'Less than two classifiers ticked for rule #{rule_cnt}')
                 if rule_data['winner_dropdown'].getChoices() not in rules[rule_cnt]['subordinates']:
                     InvalidInputError(msg=f'For rule {rule_cnt}, the winner ({rule_data["winner_dropdown"].getChoices()}) is not one of the checked classifiers.')
                 else:
                     rules[rule_cnt]['winner'] = rule_data['winner_dropdown'].getChoices()
 
 
-test = MutualExclusivityPupUp(config_path='/Users/simon/Desktop/envs/troubleshooting/anipose/project_folder/project_config.ini')
+#test = MutualExclusivityPupUp(config_path='/Users/simon/Desktop/envs/troubleshooting/anipose/project_folder/project_config.ini')
```

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/csv_2_parquet_pop_up.py` & `Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/csv_2_parquet_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/quick_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/quick_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/batch_preprocess_pop_up.py` & `Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/batch_preprocess_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/heatmap_location_pop_up.py` & `Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/heatmap_location_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/clf_probability_plot_pop_up.py` & `Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/clf_probability_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/.DS_Store` & `Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/movement_analysis_pop_up.py` & `Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/movement_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py` & `Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/clf_plot_pop_up.py` & `Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/clf_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/path_plot_pop_up.py` & `Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/remove_roi_features_pop_up.py` & `Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/remove_roi_features_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/smoothing_interpolation_pop_up.py` & `Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/smoothing_interpolation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py` & `Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/roi_analysis_pop_up.py` & `Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/roi_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/outlier_settings_pop_up.py` & `Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/outlier_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/gantt_pop_up.py` & `Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/gantt_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/clf_validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/clf_validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/severity_analysis_pop_up.py` & `Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/severity_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/fsttc_pop_up.py` & `Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/fsttc_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/kleinberg_pop_up.py` & `Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/kleinberg_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py` & `Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/pose_reorganizer_pop_up.py` & `Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/pose_reorganizer_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/append_roi_features_animals_pop_up.py` & `Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/append_roi_features_animals_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/clf_by_timebins_pop_up.py` & `Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/clf_by_timebins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/heatmap_clf_pop_up.py` & `Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/heatmap_clf_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/data_plot_pop_up.py` & `Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/data_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/roi_features_plot_pop_up.py` & `Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/roi_features_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/pup_retrieval_pop_up.py` & `Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/pup_retrieval_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/about_simba_pop_up.py` & `Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/about_simba_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py` & `Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/roi_tracking_plot_pop_up.py` & `Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/roi_tracking_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py` & `Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/clf_add_remove_print_pop_up.py` & `Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/clf_add_remove_print_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/video_processing_pop_up.py` & `Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/video_processing_pop_up.py`

 * *Files 0% similar despite different names*

```diff
@@ -422,28 +422,32 @@
         PopUpMixin.__init__(self, title="CONCATENATE VIDEOS", size=(300, 300))
         settings_frm = CreateLabelFrameWithIcon(parent=self.main_frm, header='SETTINGS', icon_name=Keys.DOCUMENTATION.value, icon_link=Links.VIDEO_TOOLS.value)
         video_path_1 = FileSelect(settings_frm, "First video path: ", title='Select a video file', lblwidth=15)
         video_path_2 = FileSelect(settings_frm, "Second video path: ", title='Select a video file', lblwidth=15)
         resolutions = ['Video 1', 'Video 2', 320, 640, 720, 1280, 1980]
         resolution_dropdown = DropDownMenu(settings_frm, 'Resolution:', resolutions, '15')
         resolution_dropdown.setChoices(resolutions[0])
+        use_gpu_var = BooleanVar(value=False)
         horizontal = BooleanVar(value=False)
         horizontal_radio_btn = Radiobutton(settings_frm, text="Horizontal concatenation", variable=horizontal, value=True)
+        use_gpu_cb = Checkbutton(settings_frm, text='Use GPU (potentially faster)', variable=use_gpu_var)
         vertical_radio_btn = Radiobutton(settings_frm, text="Vertical concatenation", variable=horizontal, value=False)
         run_btn = Button(self.main_frm, text='RUN', font=('Helvetica', 12, 'bold'), command=lambda: video_concatenator(video_one_path=video_path_1.file_path,
                                                                                       video_two_path=video_path_2.file_path,
                                                                                       resolution=resolution_dropdown.getChoices(),
-                                                                                      horizontal=horizontal.get()))
+                                                                                      horizontal=horizontal.get(),
+                                                                                      gpu=use_gpu_var.get()))
 
         settings_frm.grid(row=0, column=0, sticky=NW)
         video_path_1.grid(row=0, column=0, sticky=NW)
         video_path_2.grid(row=1, column=0, sticky=NW)
         resolution_dropdown.grid(row=2,column=0,sticky=NW)
-        horizontal_radio_btn.grid(row=3,column=0,sticky=NW)
-        vertical_radio_btn.grid(row=4, column=0, sticky=NW)
+        use_gpu_cb.grid(row=3, column=0, sticky=NW)
+        horizontal_radio_btn.grid(row=4,column=0,sticky=NW)
+        vertical_radio_btn.grid(row=5, column=0, sticky=NW)
         run_btn.grid(row=1, column=0, sticky=NW)
 
 class ConcatenatorPopUp(PopUpMixin, ConfigReader):
     def __init__(self,
                  config_path: str or None):
 
         PopUpMixin.__init__(self, title='MERGE (CONCATENATE) VIDEOS')
```

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/clf_by_roi_pop_up.py` & `Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/clf_by_roi_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/make_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/make_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py` & `Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/archive_files_pop_up.py` & `Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/archive_files_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/pose_bp_drop_pop_up.py` & `Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/pose_bp_drop_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/distance_plot_pop_up.py` & `Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/distance_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/subset_feature_extractor_pop_up.py` & `Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/subset_feature_extractor_pop_up.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,13 +44,13 @@
         #self.main_frm.mainloop()
 
     def run(self):
         check_if_dir_exists(in_dir=self.save_dir.folder_path)
         feature_extractor = FeatureSubsetsCalculator(config_path=self.config_path,
                                                      feature_family=self.feature_family_dropdown.getChoices(),
                                                      save_dir=self.save_dir.folder_path,
-                                                     append_to_features_extracted=self.append_to_targets_inserted_var.get(),
+                                                     append_to_features_extracted=self.append_to_features_extracted_var.get(),
                                                      append_to_targets_inserted=self.append_to_targets_inserted_var.get())
         feature_extractor.run()
 
 
 #FeatureSubsetExtractorPopUp(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini')
```

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py` & `Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.63.8/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/video_info_ui.py` & `Simba-UW-tf-dev-1.63.8/simba/ui/video_info_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/user_defined_pose_creator.py` & `Simba-UW-tf-dev-1.63.8/simba/ui/user_defined_pose_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/create_project_ui.py` & `Simba-UW-tf-dev-1.63.8/simba/ui/create_project_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/tkinter_functions.py` & `Simba-UW-tf-dev-1.63.8/simba/ui/tkinter_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/ui/machine_model_settings_ui.py` & `Simba-UW-tf-dev-1.63.8/simba/ui/machine_model_settings_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/blob_storage/.DS_Store` & `Simba-UW-tf-dev-1.63.8/simba/blob_storage/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/labelling/.DS_Store` & `Simba-UW-tf-dev-1.63.8/simba/labelling/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/labelling/labelling_interface_old.py` & `Simba-UW-tf-dev-1.63.8/simba/labelling/labelling_interface_old.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/labelling/labelling_interface.py` & `Simba-UW-tf-dev-1.63.8/simba/labelling/labelling_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/labelling/extract_labelled_frames.py` & `Simba-UW-tf-dev-1.63.8/simba/labelling/extract_labelled_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/labelling/labelling_advanced_interface.py` & `Simba-UW-tf-dev-1.63.8/simba/labelling/labelling_advanced_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/labelling/play_annotation_video.py` & `Simba-UW-tf-dev-1.63.8/simba/labelling/play_annotation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/unsupervised/dbcv_calculator.py` & `Simba-UW-tf-dev-1.63.8/simba/unsupervised/dbcv_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/unsupervised/enums.py` & `Simba-UW-tf-dev-1.63.8/simba/unsupervised/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.63.8/simba/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/unsupervised/dataset_creator.py` & `Simba-UW-tf-dev-1.63.8/simba/unsupervised/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/unsupervised/grid_search_visualizers.py` & `Simba-UW-tf-dev-1.63.8/simba/unsupervised/grid_search_visualizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/unsupervised/data_extractor.py` & `Simba-UW-tf-dev-1.63.8/simba/unsupervised/data_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/unsupervised/ui.py` & `Simba-UW-tf-dev-1.63.8/simba/unsupervised/ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/unsupervised/umap_embedder.py` & `Simba-UW-tf-dev-1.63.8/simba/unsupervised/umap_embedder.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/unsupervised/pop_up_classes.py` & `Simba-UW-tf-dev-1.63.8/simba/unsupervised/pop_up_classes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/unsupervised/bout_aggregator.py` & `Simba-UW-tf-dev-1.63.8/simba/unsupervised/bout_aggregator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/unsupervised/cluster_statistics.py` & `Simba-UW-tf-dev-1.63.8/simba/unsupervised/cluster_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/unsupervised/data_map.yaml` & `Simba-UW-tf-dev-1.63.8/simba/unsupervised/data_map.yaml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/unsupervised/hdbscan_clusterer.py` & `Simba-UW-tf-dev-1.63.8/simba/unsupervised/hdbscan_clusterer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/unsupervised/tsne.py` & `Simba-UW-tf-dev-1.63.8/simba/unsupervised/tsne.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/unsupervised/cluster_visualizer.py` & `Simba-UW-tf-dev-1.63.8/simba/unsupervised/cluster_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/bounding_box_tools/.DS_Store` & `Simba-UW-tf-dev-1.63.8/simba/bounding_box_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/bounding_box_tools/agg_boundary_stats.py` & `Simba-UW-tf-dev-1.63.8/simba/bounding_box_tools/agg_boundary_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/bounding_box_tools/boundary_menus.py` & `Simba-UW-tf-dev-1.63.8/simba/bounding_box_tools/boundary_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/bounding_box_tools/boundary_statistics.py` & `Simba-UW-tf-dev-1.63.8/simba/bounding_box_tools/boundary_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/bounding_box_tools/find_boundaries.py` & `Simba-UW-tf-dev-1.63.8/simba/bounding_box_tools/find_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/bounding_box_tools/visualize_boundaries.py` & `Simba-UW-tf-dev-1.63.8/simba/bounding_box_tools/visualize_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/.DS_Store` & `Simba-UW-tf-dev-1.63.8/simba/.DS_Store`

 * *Files 1% similar despite different names*

```diff
@@ -876,15 +876,15 @@
 000036b0: 0000 0000 0000 000f 0000 0000 0000 0000  ................
 000036c0: 0000 0000 0000 009a 0000 0010 0076 0069  .............v.i
 000036d0: 0064 0065 006f 005f 0070 0072 006f 0063  .d.e.o._.p.r.o.c
 000036e0: 0065 0073 0073 006f 0072 0073 6473 636c  .e.s.s.o.r.sdscl
 000036f0: 626f 6f6c 0000 0000 1000 7600 6900 6400  bool......v.i.d.
 00003700: 6500 6f00 5f00 7000 7200 6f00 6300 6500  e.o._.p.r.o.c.e.
 00003710: 7300 7300 6f00 7200 736c 6731 5363 6f6d  s.s.o.r.slg1Scom
-00003720: 7000 0000 0000 05a8 1400 0000 1000 7600  p.............v.
+00003720: 7000 0000 0000 05b6 ca00 0000 1000 7600  p.............v.
 00003730: 6900 6400 6500 6f00 5f00 7000 7200 6f00  i.d.e.o._.p.r.o.
 00003740: 6300 6500 7300 7300 6f00 7200 736c 7376  c.e.s.s.o.r.slsv
 00003750: 4362 6c6f 6200 0002 9762 706c 6973 7430  Cblob....bplist0
 00003760: 30d8 0102 0304 0506 0708 090a 0b19 494a  0.............IJ
 00003770: 0a4c 5869 636f 6e53 697a 655f 100f 7368  .LXiconSize_..sh
 00003780: 6f77 4963 6f6e 5072 6576 6965 7757 636f  owIconPreviewWco
 00003790: 6c75 6d6e 735f 1011 6361 6c63 756c 6174  lumns_..calculat
@@ -964,23 +964,23 @@
 00003c30: 0161 016a 016b 016d 016e 0170 0179 017a  .a.j.k.m.n.p.y.z
 00003c40: 017c 017d 017f 0188 0189 018c 018d 018f  .|.}............
 00003c50: 0198 0199 019a 019c 019d 01a6 01ab 0000  ................
 00003c60: 0000 0000 0201 0000 0000 0000 0049 0000  .............I..
 00003c70: 0000 0000 0000 0000 0000 0000 01ac 0000  ................
 00003c80: 0010 0076 0069 0064 0065 006f 005f 0070  ...v.i.d.e.o._.p
 00003c90: 0072 006f 0063 0065 0073 0073 006f 0072  .r.o.c.e.s.s.o.r
-00003ca0: 0073 6d6f 4444 626c 6f62 0000 0008 c1a2  .smoDDblob......
-00003cb0: e9f8 b219 c541 0000 0010 0076 0069 0064  .....A.....v.i.d
+00003ca0: 0073 6d6f 4444 626c 6f62 0000 0008 0295  .smoDDblob......
+00003cb0: 8be5 0f29 c541 0000 0010 0076 0069 0064  ...).A.....v.i.d
 00003cc0: 0065 006f 005f 0070 0072 006f 0063 0065  .e.o._.p.r.o.c.e
 00003cd0: 0073 0073 006f 0072 0073 6d6f 6444 626c  .s.s.o.r.smodDbl
-00003ce0: 6f62 0000 0008 c1a2 e9f8 b219 c541 0000  ob...........A..
+00003ce0: 6f62 0000 0008 586d 22f8 6428 c541 0000  ob....Xm".d(.A..
 00003cf0: 0010 0076 0069 0064 0065 006f 005f 0070  ...v.i.d.e.o._.p
 00003d00: 0072 006f 0063 0065 0073 0073 006f 0072  .r.o.c.e.s.s.o.r
 00003d10: 0073 7068 3153 636f 6d70 0000 0000 0007  .sph1Scomp......
-00003d20: 0000 0000 0010 0076 0069 0064 0065 006f  .......v.i.d.e.o
+00003d20: 1000 0000 0010 0076 0069 0064 0065 006f  .......v.i.d.e.o
 00003d30: 005f 0070 0072 006f 0063 0065 0073 0073  ._.p.r.o.c.e.s.s
 00003d40: 006f 0072 0073 7653 726e 6c6f 6e67 0000  .o.r.svSrnlong..
 00003d50: 0001 0000 0000 0000 0000 0000 0000 0000  ................
 00003d60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003d70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003d80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003d90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -1035,17 +1035,17 @@
 000040a0: 0073 0069 006d 0062 0061 002f 0000 000b  .s.i.m.b.a./....
 000040b0: 005f 005f 0069 006e 0069 0074 005f 005f  ._._.i.n.i.t._._
 000040c0: 002e 0070 0079 7074 624e 7573 7472 0000  ...p.yptbNustr..
 000040d0: 000b 005f 005f 0069 006e 0069 0074 005f  ..._._.i.n.i.t._
 000040e0: 005f 002e 0070 0079 0000 000b 005f 005f  ._...p.y....._._
 000040f0: 0070 0079 0063 0061 0063 0068 0065 005f  .p.y.c.a.c.h.e._
 00004100: 005f 6c67 3153 636f 6d70 0000 0000 0002  ._lg1Scomp......
-00004110: 5c68 0000 000b 005f 005f 0070 0079 0063  \h....._._.p.y.c
+00004110: 5d82 0000 000b 005f 005f 0070 0079 0063  ]......_._.p.y.c
 00004120: 0061 0063 0068 0065 005f 005f 6d6f 4444  .a.c.h.e._._moDD
-00004130: 626c 6f62 0000 0008 fef2 7934 1721 c541  blob......y4.!.A
+00004130: 626c 6f62 0000 0008 e2d6 95d5 1027 c541  blob.........'.A
 00004140: 0000 000b 005f 005f 0070 0079 0063 0061  ....._._.p.y.c.a
 00004150: 0063 0068 0065 005f 005f 6d6f 6444 626c  .c.h.e._._modDbl
 00004160: 6f62 0000 0008 fef2 7934 1721 c541 0000  ob......y4.!.A..
 00004170: 000b 005f 005f 0070 0079 0063 0061 0063  ..._._.p.y.c.a.c
 00004180: 0068 0065 005f 005f 7068 3153 636f 6d70  .h.e._._ph1Scomp
 00004190: 0000 0000 0002 a000 0000 0006 0061 0073  .............a.s
 000041a0: 0073 0065 0074 0073 6277 7370 626c 6f62  .s.e.t.sbwspblob
@@ -1370,15 +1370,15 @@
 00005590: 0100 0000 0000 0000 0f00 0000 0000 0000  ................
 000055a0: 0000 0000 0000 0000 9b00 0000 0f00 6400  ..............d.
 000055b0: 6100 7400 6100 5f00 7000 7200 6f00 6300  a.t.a._.p.r.o.c.
 000055c0: 6500 7300 7300 6f00 7200 7364 7363 6c62  e.s.s.o.r.sdsclb
 000055d0: 6f6f 6c00 0000 000f 0064 0061 0074 0061  ool......d.a.t.a
 000055e0: 005f 0070 0072 006f 0063 0065 0073 0073  ._.p.r.o.c.e.s.s
 000055f0: 006f 0072 0073 6c67 3153 636f 6d70 0000  .o.r.slg1Scomp..
-00005600: 0000 0006 9ad9 0000 000f 0064 0061 0074  ...........d.a.t
+00005600: 0000 0006 b2a0 0000 000f 0064 0061 0074  ...........d.a.t
 00005610: 0061 005f 0070 0072 006f 0063 0065 0073  .a._.p.r.o.c.e.s
 00005620: 0073 006f 0072 0073 6c73 7643 626c 6f62  .s.o.r.slsvCblob
 00005630: 0000 0281 6270 6c69 7374 3030 d801 0203  ....bplist00....
 00005640: 0405 0607 0809 0a0b 1646 4748 0a5f 1012  .........FGH._..
 00005650: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
 00005660: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
 00005670: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
@@ -1457,22 +1457,22 @@
 00005b00: 6301 6501 6e01 6f01 7101 7201 7401 7d01  c.e.n.o.q.r.t.}.
 00005b10: 7e01 8001 8101 8301 8c01 8d01 9001 9101  ~...............
 00005b20: 9301 9401 9d01 aa01 b300 0000 0000 0002  ................
 00005b30: 0100 0000 0000 0000 4900 0000 0000 0000  ........I.......
 00005b40: 0000 0000 0000 0001 b400 0000 0f00 6400  ..............d.
 00005b50: 6100 7400 6100 5f00 7000 7200 6f00 6300  a.t.a._.p.r.o.c.
 00005b60: 6500 7300 7300 6f00 7200 736d 6f44 4462  e.s.s.o.r.smoDDb
-00005b70: 6c6f 6200 0000 089a 4682 3d7b 20c5 4100  lob.....F.={ .A.
+00005b70: 6c6f 6200 0000 083b e05c 3068 26c5 4100  lob....;.\0h&.A.
 00005b80: 0000 0f00 6400 6100 7400 6100 5f00 7000  ....d.a.t.a._.p.
 00005b90: 7200 6f00 6300 6500 7300 7300 6f00 7200  r.o.c.e.s.s.o.r.
-00005ba0: 736d 6f64 4462 6c6f 6200 0000 089a 4682  smodDblob.....F.
-00005bb0: 3d7b 20c5 4100 0000 0f00 6400 6100 7400  ={ .A.....d.a.t.
+00005ba0: 736d 6f64 4462 6c6f 6200 0000 083b e05c  smodDblob....;.\
+00005bb0: 3068 26c5 4100 0000 0f00 6400 6100 7400  0h&.A.....d.a.t.
 00005bc0: 6100 5f00 7000 7200 6f00 6300 6500 7300  a._.p.r.o.c.e.s.
 00005bd0: 7300 6f00 7200 7370 6831 5363 6f6d 7000  s.o.r.sph1Scomp.
-00005be0: 0000 0000 0880 0000 0000 0f00 6400 6100  ............d.a.
+00005be0: 0000 0000 08a0 0000 0000 0f00 6400 6100  ............d.a.
 00005bf0: 7400 6100 5f00 7000 7200 6f00 6300 6500  t.a._.p.r.o.c.e.
 00005c00: 7300 7300 6f00 7200 7376 5372 6e6c 6f6e  s.s.o.r.svSrnlon
 00005c10: 6700 0000 0100 0000 1200 6600 6500 6100  g.........f.e.a.
 00005c20: 7400 7500 7200 6500 5f00 6500 7800 7400  t.u.r.e._.e.x.t.
 00005c30: 7200 6100 6300 7400 6f00 7200 7362 7773  r.a.c.t.o.r.sbws
 00005c40: 7062 6c6f 6200 0000 c962 706c 6973 7430  pblob....bplist0
 00005c50: 30d7 0102 0304 0506 0708 080a 080a 0d0a  0...............
@@ -1489,15 +1489,15 @@
 00005d00: 000f 0000 0000 0000 0000 0000 0000 0000  ................
 00005d10: 009a 0000 0012 0066 0065 0061 0074 0075  .......f.e.a.t.u
 00005d20: 0072 0065 005f 0065 0078 0074 0072 0061  .r.e._.e.x.t.r.a
 00005d30: 0063 0074 006f 0072 0073 6473 636c 626f  .c.t.o.r.sdsclbo
 00005d40: 6f6c 0000 0000 1200 6600 6500 6100 7400  ol......f.e.a.t.
 00005d50: 7500 7200 6500 5f00 6500 7800 7400 7200  u.r.e._.e.x.t.r.
 00005d60: 6100 6300 7400 6f00 7200 736c 6731 5363  a.c.t.o.r.slg1Sc
-00005d70: 6f6d 7000 0000 0000 0b3d ba10 c808 5e64  omp......=....^d
+00005d70: 6f6d 7000 0000 0000 0b53 c910 c808 5e64  omp......S....^d
 00005d80: 6174 654c 6173 744f 7065 6e65 64d4 0d0e  ateLastOpened...
 00005d90: 0f10 161c 1644 0808 5964 6174 6541 6464  .....D..YdateAdd
 00005da0: 6564 0823 4028 0000 0000 0000 546e 616d  ed.#@(......Tnam
 00005db0: 6523 4030 0000 0000 0000 0900 0800 1900  e#@0............
 00005dc0: 2e00 4000 4800 5c00 6500 7000 7900 8c00  ..@.H.\.e.p.y...
 00005dd0: 8e00 8f00 9b00 a400 ac00 b200 bc00 c700  ................
 00005de0: c800 cb00 cc00 d100 da00 db00 dd00 de00  ................
@@ -1579,22 +1579,22 @@
 000062a0: a501 ae01 b001 b201 b301 b401 bd01 bf01  ................
 000062b0: c201 c301 c401 c501 ce01 d701 e400 0000  ................
 000062c0: 0000 0002 0100 0000 0000 0000 4c00 0000  ............L...
 000062d0: 0000 0000 0000 0000 0000 0001 e500 0000  ................
 000062e0: 1200 6600 6500 6100 7400 7500 7200 6500  ..f.e.a.t.u.r.e.
 000062f0: 5f00 6500 7800 7400 7200 6100 6300 7400  _.e.x.t.r.a.c.t.
 00006300: 6f00 7200 736d 6f44 4462 6c6f 6200 0000  o.r.smoDDblob...
-00006310: 0869 3ef0 203f 0dc5 4100 0000 1200 6600  .i>. ?..A.....f.
+00006310: 08da 0969 fb83 29c5 4100 0000 1200 6600  ...i..).A.....f.
 00006320: 6500 6100 7400 7500 7200 6500 5f00 6500  e.a.t.u.r.e._.e.
 00006330: 7800 7400 7200 6100 6300 7400 6f00 7200  x.t.r.a.c.t.o.r.
-00006340: 736d 6f64 4462 6c6f 6200 0000 0869 3ef0  smodDblob....i>.
-00006350: 203f 0dc5 4100 0000 1200 6600 6500 6100   ?..A.....f.e.a.
+00006340: 736d 6f64 4462 6c6f 6200 0000 08da 0969  smodDblob......i
+00006350: fb83 29c5 4100 0000 1200 6600 6500 6100  ..).A.....f.e.a.
 00006360: 7400 7500 7200 6500 5f00 6500 7800 7400  t.u.r.e._.e.x.t.
 00006370: 7200 6100 6300 7400 6f00 7200 7370 6831  r.a.c.t.o.r.sph1
-00006380: 5363 6f6d 7000 0000 0000 0db0 0000 0000  Scomp...........
+00006380: 5363 6f6d 7000 0000 0000 0dd0 0000 0000  Scomp...........
 00006390: 1200 6600 6500 6100 7400 7500 7200 6500  ..f.e.a.t.u.r.e.
 000063a0: 5f00 6500 7800 7400 7200 6100 6300 7400  _.e.x.t.r.a.c.t.
 000063b0: 6f00 7200 7376 5372 6e6c 6f6e 6700 0000  o.r.svSrnlong...
 000063c0: 0100 0000 0900 6c00 6100 6200 6500 6c00  ......l.a.b.e.l.
 000063d0: 6c00 6900 6e00 6762 7773 7062 6c6f 6200  l.i.n.gbwspblob.
 000063e0: 0000 b862 706c 6973 7430 30d6 0102 0304  ...bplist00.....
 000063f0: 0506 0708 0708 0b08 5d53 686f 7753 7461  ........]ShowSta
@@ -1713,15 +1713,15 @@
 00006b00: 735b 5368 6f77 5369 6465 6261 7208 0809  s[ShowSidebar...
 00006b10: 0809 5f10 177b 7b30 2c20 3130 357d 2c20  .._..{{0, 105}, 
 00006b20: 7b31 3139 392c 2037 3639 7d7d 0908 1725  {1199, 769}}...%
 00006b30: 313d 4960 6d79 7a7b 7c7d 7e98 0000 0000  1=I`myz{|}~.....
 00006b40: 0000 0101 0000 0000 0000 000f 0000 0000  ................
 00006b50: 0000 0000 0000 0000 0000 0099 0000 0006  ................
 00006b60: 006d 0069 0078 0069 006e 0073 6c67 3153  .m.i.x.i.n.slg1S
-00006b70: 636f 6d70 0000 0000 0010 4dd8 0000 0006  comp......M.....
+00006b70: 636f 6d70 0000 0000 0010 6607 0000 0006  comp......f.....
 00006b80: 006d 0069 0078 0069 006e 0073 6c73 7643  .m.i.x.i.n.slsvC
 00006b90: 626c 6f62 0000 0281 6270 6c69 7374 3030  blob....bplist00
 00006ba0: d801 0203 0405 0607 0809 0a0b 1646 4748  .............FGH
 00006bb0: 0a5f 1012 7669 6577 4f70 7469 6f6e 7356  ._..viewOptionsV
 00006bc0: 6572 7369 6f6e 5f10 0f73 686f 7749 636f  ersion_..showIco
 00006bd0: 6e50 7265 7669 6577 5763 6f6c 756d 6e73  nPreviewWcolumns
 00006be0: 5f10 1163 616c 6375 6c61 7465 416c 6c53  _..calculateAllS
@@ -1788,20 +1788,20 @@
 00006fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007000: 0000 0000 0000 0000 0000 0016 0000 0006  ................
 00007010: 006d 0069 0078 0069 006e 0073 6d6f 4444  .m.i.x.i.n.smoDD
-00007020: 626c 6f62 0000 0008 1c97 c920 7b20 c541  blob....... { .A
+00007020: 626c 6f62 0000 0008 e4a6 81c8 0729 c541  blob.........).A
 00007030: 0000 0006 006d 0069 0078 0069 006e 0073  .....m.i.x.i.n.s
-00007040: 6d6f 6444 626c 6f62 0000 0008 1c97 c920  modDblob....... 
-00007050: 7b20 c541 0000 0006 006d 0069 0078 0069  { .A.....m.i.x.i
+00007040: 6d6f 6444 626c 6f62 0000 0008 71b7 5521  modDblob....q.U!
+00007050: fd28 c541 0000 0006 006d 0069 0078 0069  .(.A.....m.i.x.i
 00007060: 006e 0073 7068 3153 636f 6d70 0000 0000  .n.sph1Scomp....
-00007070: 0011 a000 0000 0006 006d 0069 0078 0069  .........m.i.x.i
+00007070: 0011 c000 0000 0006 006d 0069 0078 0069  .........m.i.x.i
 00007080: 006e 0073 7653 726e 6c6f 6e67 0000 0001  .n.svSrnlong....
 00007090: 0000 0005 006d 006f 0064 0065 006c 6277  .....m.o.d.e.lbw
 000070a0: 7370 626c 6f62 0000 00c9 6270 6c69 7374  spblob....bplist
 000070b0: 3030 d701 0203 0405 0607 0808 0a08 0a0d  00..............
 000070c0: 0a5d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
 000070d0: 5368 6f77 5061 7468 6261 725b 5368 6f77  ShowPathbar[Show
 000070e0: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
@@ -2485,15 +2485,15 @@
 00009b40: 6562 6172 0808 0908 095f 1019 7b7b 3233  ebar....._..{{23
 00009b50: 322c 2031 3931 7d2c 207b 3133 3032 2c20  2, 191}, {1302, 
 00009b60: 3731 347d 7d09 0817 2531 3d49 606d 797a  714}}...%1=I`myz
 00009b70: 7b7c 7d7e 9a00 0000 0000 0001 0100 0000  {|}~............
 00009b80: 0000 0000 0f00 0000 0000 0000 0000 0000  ................
 00009b90: 0000 0000 9b00 0000 0900 7200 6f00 6900  ..........r.o.i.
 00009ba0: 5f00 7400 6f00 6f00 6c00 736c 6731 5363  _.t.o.o.l.slg1Sc
-00009bb0: 6f6d 7000 0000 0000 079d 0800 0000 0900  omp.............
+00009bb0: 6f6d 7000 0000 0000 079c b900 0000 0900  omp.............
 00009bc0: 7200 6f00 6900 5f00 7400 6f00 6f00 6c00  r.o.i._.t.o.o.l.
 00009bd0: 736c 7376 4362 6c6f 6200 0002 7962 706c  slsvCblob...ybpl
 00009be0: 6973 7430 30d8 0102 0304 0506 0708 090a  ist00...........
 00009bf0: 0b16 4647 480a 5f10 1276 6965 774f 7074  ..FGH._..viewOpt
 00009c00: 696f 6e73 5665 7273 696f 6e5f 100f 7368  ionsVersion_..sh
 00009c10: 6f77 4963 6f6e 5072 6576 6965 7757 636f  owIconPreviewWco
 00009c20: 6c75 6d6e 735f 1011 6361 6c63 756c 6174  lumns_..calculat
@@ -2700,15 +2700,15 @@
 0000a8b0: 0530 0000 0000 1b00 7400 6800 6900 7200  .0......t.h.i.r.
 0000a8c0: 6400 5f00 7000 6100 7200 7400 7900 5f00  d._.p.a.r.t.y._.
 0000a8d0: 6c00 6100 6200 6500 6c00 5f00 6100 7000  l.a.b.e.l._.a.p.
 0000a8e0: 7000 6500 6e00 6400 6500 7200 7376 5372  p.e.n.d.e.r.svSr
 0000a8f0: 6e6c 6f6e 6700 0000 0100 0000 1000 7400  nlong.........t.
 0000a900: 6800 7200 6500 6500 5f00 6400 6900 6d00  h.r.e.e._.d.i.m.
 0000a910: 6500 6e00 7300 6900 6f00 6e00 736c 6731  e.n.s.i.o.n.slg1
-0000a920: 5363 6f6d 7000 0000 0000 0332 ac00 0000  Scomp......2....
+0000a920: 5363 6f6d 7000 0000 0000 033c cc00 0000  Scomp......<....
 0000a930: 1000 7400 6800 7200 6500 6500 5f00 6400  ..t.h.r.e.e._.d.
 0000a940: 6900 6d00 6500 6e00 7300 6900 6f00 6e00  i.m.e.n.s.i.o.n.
 0000a950: 736d 6f44 4462 6c6f 6200 0000 08f6 8857  smoDDblob......W
 0000a960: d65e 24c5 4100 0000 1000 7400 6800 7200  .^$.A.....t.h.r.
 0000a970: 6500 6500 5f00 6400 6900 6d00 6500 6e00  e.e._.d.i.m.e.n.
 0000a980: 7300 6900 6f00 6e00 736d 6f64 4462 6c6f  s.i.o.n.smodDblo
 0000a990: 6200 0000 08f6 8857 d65e 24c5 4100 0000  b......W.^$.A...
@@ -2727,15 +2727,15 @@
 0000aa60: 0908 095f 1019 7b7b 3335 342c 2031 3234  ..._..{{354, 124
 0000aa70: 7d2c 207b 3130 3736 2c20 3632 317d 7d09  }, {1076, 621}}.
 0000aa80: 0817 2531 3d49 606d 797a 7b7c 7d7e 9a00  ..%1=I`myz{|}~..
 0000aa90: 0000 0000 0001 0100 0000 0000 0000 0f00  ................
 0000aaa0: 0000 0000 0000 0000 0000 0000 0000 9b00  ................
 0000aab0: 0000 0200 7500 6964 7363 6c62 6f6f 6c00  ....u.idsclbool.
 0000aac0: 0000 0002 0075 0069 6c67 3153 636f 6d70  .....u.ilg1Scomp
-0000aad0: 0000 0000 0011 9d6c 0000 0002 0075 0069  .......l.....u.i
+0000aad0: 0000 0000 0011 ddd7 0000 0002 0075 0069  .............u.i
 0000aae0: 6c73 7643 626c 6f62 0000 0279 6270 6c69  lsvCblob...ybpli
 0000aaf0: 7374 3030 d801 0203 0405 0607 0809 0a0b  st00............
 0000ab00: 1846 4748 0a5f 1012 7669 6577 4f70 7469  .FGH._..viewOpti
 0000ab10: 6f6e 7356 6572 7369 6f6e 5f10 0f73 686f  onsVersion_..sho
 0000ab20: 7749 636f 6e50 7265 7669 6577 5763 6f6c  wIconPreviewWcol
 0000ab30: 756d 6e73 5f10 1163 616c 6375 6c61 7465  umns_..calculate
 0000ab40: 416c 6c53 697a 6573 5874 6578 7453 697a  AllSizesXtextSiz
@@ -2812,15 +2812,15 @@
 0000afb0: 9401 9d01 a201 ab00 0000 0000 0002 0100  ................
 0000afc0: 0000 0000 0000 4900 0000 0000 0000 0000  ......I.........
 0000afd0: 0000 0000 0001 ac00 0000 0200 7500 696d  ............u.im
 0000afe0: 6f44 4462 6c6f 6200 0000 087e abce 1cd0  oDDblob....~....
 0000aff0: 1fc5 4100 0000 0000 0000 0000 0000 0000  ..A.............
 0000b000: 0000 0000 0000 0000 0000 000c 0000 0002  ................
 0000b010: 0075 0069 7068 3153 636f 6d70 0000 0000  .u.iph1Scomp....
-0000b020: 0017 c000 0000 0002 0075 0069 7653 726e  .........u.ivSrn
+0000b020: 0018 1000 0000 0002 0075 0069 7653 726e  .........u.ivSrn
 0000b030: 6c6f 6e67 0000 0001 0000 000c 0075 006e  long.........u.n
 0000b040: 0073 0075 0070 0065 0072 0076 0069 0073  .s.u.p.e.r.v.i.s
 0000b050: 0065 0064 6277 7370 626c 6f62 0000 00ca  .e.dbwspblob....
 0000b060: 6270 6c69 7374 3030 d701 0203 0405 0607  bplist00........
 0000b070: 0808 0a08 0a0d 0a5d 5368 6f77 5374 6174  .......]ShowStat
 0000b080: 7573 4261 725b 5368 6f77 5061 7468 6261  usBar[ShowPathba
 0000b090: 725b 5368 6f77 546f 6f6c 6261 725b 5368  r[ShowToolbar[Sh
@@ -2956,15 +2956,15 @@
 0000b8b0: 0530 0000 0000 1b00 7400 6800 6900 7200  .0......t.h.i.r.
 0000b8c0: 6400 5f00 7000 6100 7200 7400 7900 5f00  d._.p.a.r.t.y._.
 0000b8d0: 6c00 6100 6200 6500 6c00 5f00 6100 7000  l.a.b.e.l._.a.p.
 0000b8e0: 7000 6500 6e00 6400 6500 7200 7376 5372  p.e.n.d.e.r.svSr
 0000b8f0: 6e6c 6f6e 6700 0000 0100 0000 1000 7400  nlong.........t.
 0000b900: 6800 7200 6500 6500 5f00 6400 6900 6d00  h.r.e.e._.d.i.m.
 0000b910: 6500 6e00 7300 6900 6f00 6e00 736c 6731  e.n.s.i.o.n.slg1
-0000b920: 5363 6f6d 7000 0000 0000 0332 ac00 0000  Scomp......2....
+0000b920: 5363 6f6d 7000 0000 0000 033c cc00 0000  Scomp......<....
 0000b930: 1000 7400 6800 7200 6500 6500 5f00 6400  ..t.h.r.e.e._.d.
 0000b940: 6900 6d00 6500 6e00 7300 6900 6f00 6e00  i.m.e.n.s.i.o.n.
 0000b950: 736d 6f44 4462 6c6f 6200 0000 08f6 8857  smoDDblob......W
 0000b960: d65e 24c5 4100 0000 1000 7400 6800 7200  .^$.A.....t.h.r.
 0000b970: 6500 6500 5f00 6400 6900 6d00 6500 6e00  e.e._.d.i.m.e.n.
 0000b980: 7300 6900 6f00 6e00 736d 6f64 4462 6c6f  s.i.o.n.smodDblo
 0000b990: 6200 0000 08f6 8857 d65e 24c5 4100 0000  b......W.^$.A...
@@ -2983,15 +2983,15 @@
 0000ba60: 0908 095f 1019 7b7b 3335 342c 2031 3234  ..._..{{354, 124
 0000ba70: 7d2c 207b 3130 3736 2c20 3632 317d 7d09  }, {1076, 621}}.
 0000ba80: 0817 2531 3d49 606d 797a 7b7c 7d7e 9a00  ..%1=I`myz{|}~..
 0000ba90: 0000 0000 0001 0100 0000 0000 0000 0f00  ................
 0000baa0: 0000 0000 0000 0000 0000 0000 0000 9b00  ................
 0000bab0: 0000 0200 7500 6964 7363 6c62 6f6f 6c00  ....u.idsclbool.
 0000bac0: 0000 0002 0075 0069 6c67 3153 636f 6d70  .....u.ilg1Scomp
-0000bad0: 0000 0000 0011 9d6c 0000 0002 0075 0069  .......l.....u.i
+0000bad0: 0000 0000 0011 ddd7 0000 0002 0075 0069  .............u.i
 0000bae0: 6c73 7643 626c 6f62 0000 0279 6270 6c69  lsvCblob...ybpli
 0000baf0: 7374 3030 d801 0203 0405 0607 0809 0a0b  st00............
 0000bb00: 1846 4748 0a5f 1012 7669 6577 4f70 7469  .FGH._..viewOpti
 0000bb10: 6f6e 7356 6572 7369 6f6e 5f10 0f73 686f  onsVersion_..sho
 0000bb20: 7749 636f 6e50 7265 7669 6577 5763 6f6c  wIconPreviewWcol
 0000bb30: 756d 6e73 5f10 1163 616c 6375 6c61 7465  umns_..calculate
 0000bb40: 416c 6c53 697a 6573 5874 6578 7453 697a  AllSizesXtextSiz
```

### Comparing `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/feature_extractor_14bp.py` & `Simba-UW-tf-dev-1.63.8/simba/feature_extractors/feature_extractor_14bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/feature_extractor_7bp.py` & `Simba-UW-tf-dev-1.63.8/simba/feature_extractors/feature_extractor_7bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/doctests.py` & `Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/read_in_mp.py` & `Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/peaks.py` & `Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/peaks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/.DS_Store` & `Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/count_values_in_range.py` & `Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/graph_creator.py` & `Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/termite_rois.csv` & `Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/mutual_exclusive.py` & `Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/video_color.py` & `Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/shap_log_mp_2.py` & `Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/shap_log_mp_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/video_rotator.py` & `Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/shap_log_mp.py` & `Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/shap_log_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/make_splash.py` & `Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py` & `Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/time_stamp_calculator.py` & `Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/time_stamp_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/video_rotator_mp.py` & `Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/read_files_mp_2.py` & `Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/read_files_mp_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py` & `Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/misc/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.63.8/simba/feature_extractors/misc/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/feature_extractor_8bps_2_animals.py` & `Simba-UW-tf-dev-1.63.8/simba/feature_extractors/feature_extractor_8bps_2_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/.DS_Store` & `Simba-UW-tf-dev-1.63.8/simba/feature_extractors/.DS_Store`

 * *Files 4% similar despite different names*

```diff
@@ -276,23 +276,23 @@
 00001130: 5f10 197b 7b34 3732 2c20 3134 327d 2c20  _..{{472, 142}, 
 00001140: 7b31 3037 362c 2036 3231 7d7d 0908 1725  {1076, 621}}...%
 00001150: 313d 4960 6d79 7a7b 7c7d 7e9a 0000 0000  1=I`myz{|}~.....
 00001160: 0000 0101 0000 0000 0000 000f 0000 0000  ................
 00001170: 0000 0000 0000 0000 0000 009b 0000 000b  ................
 00001180: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00001190: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-000011a0: 0000 0004 3e87 0000 000b 005f 005f 0070  ....>......_._.p
+000011a0: 0000 0004 43ec 0000 000b 005f 005f 0070  ....C......_._.p
 000011b0: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-000011c0: 6d6f 4444 626c 6f62 0000 0008 ea13 b999  moDDblob........
-000011d0: 8d20 c541 0000 000b 005f 005f 0070 0079  . .A....._._.p.y
+000011c0: 6d6f 4444 626c 6f62 0000 0008 2dea ae91  moDDblob....-...
+000011d0: 0927 c541 0000 000b 005f 005f 0070 0079  .'.A....._._.p.y
 000011e0: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-000011f0: 6444 626c 6f62 0000 0008 ea13 b999 8d20  dDblob......... 
+000011f0: 6444 626c 6f62 0000 0008 2dea ae91 0927  dDblob....-....'
 00001200: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 00001210: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-00001220: 636f 6d70 0000 0000 0004 f000 0000 000b  comp............
+00001220: 636f 6d70 0000 0000 0005 0000 0000 000b  comp............
 00001230: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00001240: 0065 005f 005f 7653 726e 6c6f 6e67 0000  .e._._vSrnlong..
 00001250: 0001 0000 0004 006d 0069 0073 0063 6277  .......m.i.s.cbw
 00001260: 7370 626c 6f62 0000 00c9 6270 6c69 7374  spblob....bplist
 00001270: 3030 d701 0203 0405 0607 0808 0a08 0a0d  00..............
 00001280: 0a5d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
 00001290: 5368 6f77 5061 7468 6261 725b 5368 6f77  ShowPathbar[Show
```

### Comparing `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/perimeter_jit.py` & `Simba-UW-tf-dev-1.63.8/simba/feature_extractors/perimeter_jit.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/feature_subsets.py` & `Simba-UW-tf-dev-1.63.8/simba/feature_extractors/feature_subsets.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from simba.feature_extractors.perimeter_jit import jitted_hull
 from simba.utils.enums import Formats, Options
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.feature_extraction_mixin import FeatureExtractionMixin
 from simba.utils.checks import check_if_filepath_list_is_empty, check_file_exist_and_readable
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.read_write import get_fn_ext, read_df, write_df
-from simba.utils.errors import CountError
+from simba.utils.errors import CountError, DataHeaderError
 
 
 class FeatureSubsetsCalculator(ConfigReader, FeatureExtractionMixin):
     """
     Computes a subset of features from pose for non-ML downstream purposes.
     E.g., returns the size of animal convex hull in each frame.
 
@@ -115,15 +115,15 @@
             self.__save()
             self.video_timer.stop_timer()
             print(
                 f"Video {self.video_name} complete (elapsed time {self.video_timer.elapsed_time_str}s)..."
             )
         self.timer.stop_timer()
         stdout_success(
-            msg=f"{self.feature_family} for {str(len(self.outlier_corrected_paths))} videos saved in {self.save_dir}",
+            msg=f"{self.feature_family} for {str(len(self.outlier_corrected_paths))} video(s) saved in {self.save_dir}",
             elapsed_time=self.timer.elapsed_time_str,
         )
 
     def calc_distances(self):
         for c in self.two_point_combs:
             col_names = list(sum([(x + "_x", y + "_y") for (x, y) in zip(c, c)], ()))
 
@@ -279,41 +279,54 @@
                                 f"{animal} {bp} inside polygon {shape_name} (Boolean)"
                             ] = self.framewise_inside_polygon_roi(
                                 bp_location=bp_arr, roi_coords=shape_data
                             )
 
     def __save(self):
         if self.append_to_features:
+            prior_appending_features_data_folder = os.path.join(self.features_dir, f'Prior_to_third_subset_features_{self.datetime}')
+            if not os.path.isdir(prior_appending_features_data_folder):
+                os.makedirs(prior_appending_features_data_folder)
             file_path = os.path.join(self.features_dir, f"{self.video_name}.csv")
             check_file_exist_and_readable(file_path=file_path)
             features_df = read_df(file_path=file_path, file_type=self.file_type)
             if len(features_df) != len(self.results):
                 raise CountError(f'Cannot append feature subsets to features file. The file used to create the feature subsets ({self.current_file_path}) contains data for {len(self.results)} frames, while the file representing the same video in features extracted folder ({file_path}) contains data for {len(features_df)} frames. Make sure the two files has an equal number of rows.')
             new_features_df = pd.concat([features_df, self.results.round(2)], axis=1)
+            duplicate_cols = new_features_df.columns[new_features_df.columns.duplicated()]
+            if len(duplicate_cols) > 0:
+                raise DataHeaderError(msg=f'Attempted to append feature data to file {file_path}. However the new features (e.g., {duplicate_cols[0]}) already exist in the file.')
+            write_df(df=features_df, file_type=self.file_type, save_path=os.path.join(prior_appending_features_data_folder, os.path.basename(file_path)))
             write_df(df=new_features_df, file_type=self.file_type, save_path=file_path)
             del new_features_df
             print(f'New features for video {self.video_name} saved in project_folder/csv/features_extracted directory...')
 
         if self.append_to_targets:
+            prior_appending_features_data_folder = os.path.join(self.targets_folder,f'Prior_to_third_subset_features_{self.datetime}')
+            if not os.path.isdir(prior_appending_features_data_folder):
+                os.makedirs(prior_appending_features_data_folder)
             file_path = os.path.join(self.targets_folder, f"{self.video_name}.csv")
             check_file_exist_and_readable(file_path=file_path)
             targets_df = read_df(file_path=file_path, file_type=self.file_type)
             targets_clf_df = pd.DataFrame()
-
             for clf in self.clf_names:
                 if clf in targets_df.columns:
                     targets_clf_df[clf] = targets_df[clf]
                     targets_df.drop(clf, axis=1, inplace=True)
 
             new_targets_df = pd.concat([targets_df, self.results.round(2), targets_clf_df], axis=1)
-            write_df(df=new_targets_df, file_type=self.file_type, save_path=file_path)
-            del new_targets_df
-            print(f'New targets file for video {self.video_name} saved in project_folder/csv/targets_inserted directory...')
+            duplicate_cols = new_targets_df.columns[new_targets_df.columns.duplicated()]
+            if len(duplicate_cols) > 0:
+                raise DataHeaderError(msg=f'Attempted to append feature data to file {file_path}. However the new features (e.g., {duplicate_cols[0]}) already exist in the file.')
 
 
+            write_df(df=targets_df, file_type=self.file_type, save_path=os.path.join(prior_appending_features_data_folder, os.path.basename(file_path)))
+            write_df(df=new_targets_df, file_type=self.file_type, save_path=file_path)
+            del new_targets_df; del targets_df
+            print(f'New targets file for video {self.video_name} saved in project_folder/csv/targets_inserted directory...')
 
         save_path = os.path.join(self.save_dir, f"{self.video_name}.csv")
         write_df(df=self.results.round(2), file_type=Formats.CSV.value, save_path=save_path)
 
 
 # test = FeatureSubsetsCalculator(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
 #                                 feature_family='Frame-by-frame body-parts inside ROIs (Boolean)',
@@ -322,14 +335,14 @@
 
 
 # test = FeatureSubsetsCalculator(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
 #                                 feature_family='Frame-by-frame body-part movements (mm)',
 #                                 save_dir='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/data')
 # test.run()
 
-
+#
 # test = FeatureSubsetsCalculator(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
 #                                 feature_family='Frame-by-frame body-parts inside ROIs (Boolean)',
 #                                 save_dir='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/data',
-#                                 append_to_features_extracted=True,
+#                                 append_to_features_extracted=False,
 #                                 append_to_targets_inserted=True)
 # test.run()
```

### Comparing `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/feature_extractor_user_defined.py` & `Simba-UW-tf-dev-1.63.8/simba/feature_extractors/feature_extractor_user_defined.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/feature_extractor_16bp.py` & `Simba-UW-tf-dev-1.63.8/simba/feature_extractors/feature_extractor_16bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/feature_extractor_9bp.py` & `Simba-UW-tf-dev-1.63.8/simba/feature_extractors/feature_extractor_9bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/feature_extractor_8bp.py` & `Simba-UW-tf-dev-1.63.8/simba/feature_extractors/feature_extractor_8bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/feature_extractor_4bp.py` & `Simba-UW-tf-dev-1.63.8/simba/feature_extractors/feature_extractor_4bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/.idea/features_scripts.iml` & `Simba-UW-tf-dev-1.63.8/simba/feature_extractors/.idea/features_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.63.8/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/feature_extractors/.idea/workspace.xml` & `Simba-UW-tf-dev-1.63.8/simba/feature_extractors/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/requirements.txt` & `Simba-UW-tf-dev-1.63.8/simba/requirements.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/mixins/.DS_Store` & `Simba-UW-tf-dev-1.63.8/simba/pose_processors/.DS_Store`

 * *Files 6% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000100: 0000 0000 0000 0000 0000 0004 0000 000b  ................
 00000110: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00000120: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00000130: 0000 000b eaf3 0000 000b 005f 005f 0070  ..........._._.p
+00000130: 0000 0000 a209 0000 000b 005f 005f 0070  ..........._._.p
 00000140: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00000150: 6d6f 4444 626c 6f62 0000 0008 f1c6 1c64  moDDblob.......d
-00000160: 4422 c541 0000 000b 005f 005f 0070 0079  D".A....._._.p.y
+00000150: 6d6f 4444 626c 6f62 0000 0008 beac 8729  moDDblob.......)
+00000160: 7b20 c541 0000 000b 005f 005f 0070 0079  { .A....._._.p.y
 00000170: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00000180: 6444 626c 6f62 0000 0008 f1c6 1c64 4422  dDblob.......dD"
+00000180: 6444 626c 6f62 0000 0008 beac 8729 7b20  dDblob.......){ 
 00000190: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000001a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000001b0: 636f 6d70 0000 0000 000c f000 0000 0000  comp............
+000001b0: 636f 6d70 0000 0000 0001 4000 0000 0000  comp......@.....
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `Simba-UW-tf-dev-1.63.7/simba/mixins/pop_up_mixin.py` & `Simba-UW-tf-dev-1.63.8/simba/mixins/pop_up_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/mixins/config_reader.py` & `Simba-UW-tf-dev-1.63.8/simba/mixins/config_reader.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/mixins/pose_importer_mixin.py` & `Simba-UW-tf-dev-1.63.8/simba/mixins/pose_importer_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.nbi` & `Simba-UW-tf-dev-1.63.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi` & `Simba-UW-tf-dev-1.63.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi` & `Simba-UW-tf-dev-1.63.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.1.nbc` & `Simba-UW-tf-dev-1.63.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc` & `Simba-UW-tf-dev-1.63.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.2.nbc` & `Simba-UW-tf-dev-1.63.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.2.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc` & `Simba-UW-tf-dev-1.63.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.63.8/simba/mixins/feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/mixins/plotting_mixin.py` & `Simba-UW-tf-dev-1.63.8/simba/mixins/plotting_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/mixins/unsupervised_mixin.py` & `Simba-UW-tf-dev-1.63.8/simba/mixins/unsupervised_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/mixins/train_model_mixin.py` & `Simba-UW-tf-dev-1.63.8/simba/mixins/train_model_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/third_party_label_appenders/deepethogram_importer.py` & `Simba-UW-tf-dev-1.63.8/simba/third_party_label_appenders/deepethogram_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/third_party_label_appenders/BORIS_appender.py` & `Simba-UW-tf-dev-1.63.8/simba/third_party_label_appenders/BORIS_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/third_party_label_appenders/observer_importer.py` & `Simba-UW-tf-dev-1.63.8/simba/third_party_label_appenders/observer_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/third_party_label_appenders/.DS_Store` & `Simba-UW-tf-dev-1.63.8/simba/third_party_label_appenders/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/third_party_label_appenders/tools.py` & `Simba-UW-tf-dev-1.63.8/simba/third_party_label_appenders/tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/third_party_label_appenders/third_party_appender.py` & `Simba-UW-tf-dev-1.63.8/simba/third_party_label_appenders/third_party_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/third_party_label_appenders/ethovision_import.py` & `Simba-UW-tf-dev-1.63.8/simba/third_party_label_appenders/ethovision_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/third_party_label_appenders/BENTO_appender.py` & `Simba-UW-tf-dev-1.63.8/simba/third_party_label_appenders/BENTO_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/third_party_label_appenders/solomon_importer.py` & `Simba-UW-tf-dev-1.63.8/simba/third_party_label_appenders/solomon_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/cue_light_tools/.DS_Store` & `Simba-UW-tf-dev-1.63.8/simba/cue_light_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/cue_light_tools/cue_light_clf_statistics.py` & `Simba-UW-tf-dev-1.63.8/simba/cue_light_tools/cue_light_clf_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/cue_light_tools/cue_light_analyzer.py` & `Simba-UW-tf-dev-1.63.8/simba/cue_light_tools/cue_light_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/cue_light_tools/cue_light_menues.py` & `Simba-UW-tf-dev-1.63.8/simba/cue_light_tools/cue_light_menues.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/cue_light_tools/cue_light_tools.py` & `Simba-UW-tf-dev-1.63.8/simba/cue_light_tools/cue_light_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/cue_light_tools/cue_light_visualizer.py` & `Simba-UW-tf-dev-1.63.8/simba/cue_light_tools/cue_light_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/cue_light_tools/cue_light_movement_statistics.py` & `Simba-UW-tf-dev-1.63.8/simba/cue_light_tools/cue_light_movement_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/utils/config_creator.py` & `Simba-UW-tf-dev-1.63.8/simba/utils/config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/utils/enums.py` & `Simba-UW-tf-dev-1.63.8/simba/utils/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/utils/.DS_Store` & `Simba-UW-tf-dev-1.63.8/simba/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/utils/warnings.py` & `Simba-UW-tf-dev-1.63.8/simba/utils/warnings.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,8 +124,12 @@
 def MultiProcessingFailedWarning(msg: str):
     stdout_warning(msg=f'SIMBA MULTI-PROCESSING WARNING: {msg}')
 
 def PythonVersionWarning(msg: str):
     stdout_warning(msg=f'SIMBA PYTHON VERSION WARNING: {msg}')
 
 def BorisPointEventsWarning(msg: str):
-    stdout_warning(msg=f'SIMBA BORIS POINT EVENT WARNING: {msg}')
+    stdout_warning(msg=f'SIMBA BORIS POINT EVENT WARNING: {msg}')
+
+
+def FFMpegCodecWarning(msg: str):
+    stdout_warning(msg=f'SIMBA FFMPEG CODEC WARNING: {msg}')
```

### Comparing `Simba-UW-tf-dev-1.63.7/simba/utils/checks.py` & `Simba-UW-tf-dev-1.63.8/simba/utils/checks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/utils/read_write.py` & `Simba-UW-tf-dev-1.63.8/simba/utils/read_write.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/utils/lookups.py` & `Simba-UW-tf-dev-1.63.8/simba/utils/lookups.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/utils/cli/cli_tools.py` & `Simba-UW-tf-dev-1.63.8/simba/utils/cli/cli_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/utils/errors.py` & `Simba-UW-tf-dev-1.63.8/simba/utils/errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -297,8 +297,13 @@
                 f'However, in BORIS, you have annotated {clf_name} to happen at frame number {str(first_error_frm)}. '
                 f'These ambiguous annotations occur in {str(ambiguous_cnt)} different frames for video {video_name} that SimBA will **remove** by default. '
                 f'Please make sure you imported the same video as you annotated in BORIS into SimBA and the video is registered with the correct frame rate.')
         else:
             msg = f'SIMBA THIRD-PARTY ANNOTATION WARNING: The annotations for video {video_name} contain data for {str(annotation_frms)} frames. The pose-estimation features for the same video contain data for {str(frm_cnt)} frames.'
 
         super().__init__(msg=msg, show_window=show_window)
-        self.print_msg(msg=msg)
+        self.print_msg(msg=msg)
+
+class FFMPEGCodecError(SimbaError):
+    def __init__(self, msg: str, show_window: bool = False):
+        super().__init__(msg=msg, show_window=show_window)
+        self.print_msg(msg=f'SIMBA FFMPEG CODEC ERROR: {msg}')
```

### Comparing `Simba-UW-tf-dev-1.63.7/simba/utils/data.py` & `Simba-UW-tf-dev-1.63.8/simba/utils/data.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/utils/printing.py` & `Simba-UW-tf-dev-1.63.8/simba/utils/printing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/st/select_groups_pg.py` & `Simba-UW-tf-dev-1.63.8/simba/st/select_groups_pg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/st/aggregate_statistics.py` & `Simba-UW-tf-dev-1.63.8/simba/st/aggregate_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/st/app.py` & `Simba-UW-tf-dev-1.63.8/simba/st/app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_processors/reorganize_keypoint.py` & `Simba-UW-tf-dev-1.63.8/simba/pose_processors/reorganize_keypoint.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_processors/remove_keypoints.py` & `Simba-UW-tf-dev-1.63.8/simba/pose_processors/remove_keypoints.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_processors/.DS_Store` & `Simba-UW-tf-dev-1.63.8/simba/mixins/.DS_Store`

 * *Files 5% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000100: 0000 0000 0000 0000 0000 0004 0000 000b  ................
 00000110: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00000120: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00000130: 0000 0000 a209 0000 000b 005f 005f 0070  ..........._._.p
+00000130: 0000 000b f7a8 0000 000b 005f 005f 0070  ..........._._.p
 00000140: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00000150: 6d6f 4444 626c 6f62 0000 0008 beac 8729  moDDblob.......)
-00000160: 7b20 c541 0000 000b 005f 005f 0070 0079  { .A....._._.p.y
+00000150: 6d6f 4444 626c 6f62 0000 0008 61f9 77e8  moDDblob....a.w.
+00000160: 2129 c541 0000 000b 005f 005f 0070 0079  !).A....._._.p.y
 00000170: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00000180: 6444 626c 6f62 0000 0008 beac 8729 7b20  dDblob.......){ 
+00000180: 6444 626c 6f62 0000 0008 c0be a523 fd28  dDblob.......#.(
 00000190: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000001a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000001b0: 636f 6d70 0000 0000 0001 4000 0000 0000  comp......@.....
+000001b0: 636f 6d70 0000 0000 000d 0000 0000 0000  comp............
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_processors/pose_reset.py` & `Simba-UW-tf-dev-1.63.8/simba/pose_processors/pose_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_processors/reverse_pose.py` & `Simba-UW-tf-dev-1.63.8/simba/pose_processors/reverse_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/plotting/gantt_creator.py` & `Simba-UW-tf-dev-1.63.8/simba/plotting/gantt_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/plotting/tools/tkinter_tools.py` & `Simba-UW-tf-dev-1.63.8/simba/plotting/tools/tkinter_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/plotting/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.63.8/simba/plotting/ROI_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/plotting/.DS_Store` & `Simba-UW-tf-dev-1.63.8/simba/plotting/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/plotting/shap_agg_stats_visualizer.py` & `Simba-UW-tf-dev-1.63.8/simba/plotting/shap_agg_stats_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/plotting/gantt_creator_mp.py` & `Simba-UW-tf-dev-1.63.8/simba/plotting/gantt_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/plotting/heat_mapper_clf_mp.py` & `Simba-UW-tf-dev-1.63.8/simba/plotting/heat_mapper_clf_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/plotting/probability_plot_creator.py` & `Simba-UW-tf-dev-1.63.8/simba/plotting/probability_plot_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/plotting/plot_clf_results.py` & `Simba-UW-tf-dev-1.63.8/simba/plotting/plot_clf_results.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/plotting/plot_clf_results_mp.py` & `Simba-UW-tf-dev-1.63.8/simba/plotting/plot_clf_results_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/plotting/ROI_feature_visualizer.py` & `Simba-UW-tf-dev-1.63.8/simba/plotting/ROI_feature_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/plotting/heat_mapper_location.py` & `Simba-UW-tf-dev-1.63.8/simba/plotting/heat_mapper_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/plotting/probability_plot_creator_mp.py` & `Simba-UW-tf-dev-1.63.8/simba/plotting/probability_plot_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/plotting/interactive_probability_grapher.py` & `Simba-UW-tf-dev-1.63.8/simba/plotting/interactive_probability_grapher.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/plotting/single_run_model_validation_video.py` & `Simba-UW-tf-dev-1.63.8/simba/plotting/single_run_model_validation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/plotting/frame_mergerer_ffmpeg.py` & `Simba-UW-tf-dev-1.63.8/simba/plotting/frame_mergerer_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/plotting/pose_plotter_mp.py` & `Simba-UW-tf-dev-1.63.8/simba/plotting/pose_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/plotting/Directing_animals_visualizer_mp.py` & `Simba-UW-tf-dev-1.63.8/simba/plotting/Directing_animals_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/plotting/clf_validator.py` & `Simba-UW-tf-dev-1.63.8/simba/plotting/clf_validator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/plotting/path_plotter_mp.py` & `Simba-UW-tf-dev-1.63.8/simba/plotting/path_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/plotting/ROI_feature_visualizer_mp.py` & `Simba-UW-tf-dev-1.63.8/simba/plotting/ROI_feature_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/plotting/data_plotter.py` & `Simba-UW-tf-dev-1.63.8/simba/plotting/data_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/plotting/path_plotter.py` & `Simba-UW-tf-dev-1.63.8/simba/plotting/path_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/plotting/ez_lineplot.py` & `Simba-UW-tf-dev-1.63.8/simba/plotting/ez_lineplot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/plotting/distance_plotter_mp.py` & `Simba-UW-tf-dev-1.63.8/simba/plotting/distance_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/plotting/ROI_plotter.py` & `Simba-UW-tf-dev-1.63.8/simba/plotting/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/plotting/heat_mapper_clf.py` & `Simba-UW-tf-dev-1.63.8/simba/plotting/heat_mapper_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/plotting/distance_plotter.py` & `Simba-UW-tf-dev-1.63.8/simba/plotting/distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/plotting/single_run_model_validation_video_mp.py` & `Simba-UW-tf-dev-1.63.8/simba/plotting/single_run_model_validation_video_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/plotting/Directing_animals_visualizer.py` & `Simba-UW-tf-dev-1.63.8/simba/plotting/Directing_animals_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/plotting/heat_mapper_location_mp.py` & `Simba-UW-tf-dev-1.63.8/simba/plotting/heat_mapper_location_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/dash_app/SimBA_dash_app.py` & `Simba-UW-tf-dev-1.63.8/simba/dash_app/SimBA_dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/dash_app/run_dash_tkinter.py` & `Simba-UW-tf-dev-1.63.8/simba/dash_app/run_dash_tkinter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/dash_app/dash_app.py` & `Simba-UW-tf-dev-1.63.8/simba/dash_app/dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/data_processors/agg_clf_calculator.py` & `Simba-UW-tf-dev-1.63.8/simba/data_processors/agg_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/data_processors/.DS_Store` & `Simba-UW-tf-dev-1.63.8/simba/data_processors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/data_processors/severity_bout_based_calculator.py` & `Simba-UW-tf-dev-1.63.8/simba/data_processors/severity_bout_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/data_processors/interpolation_smoothing.py` & `Simba-UW-tf-dev-1.63.8/simba/data_processors/interpolation_smoothing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/data_processors/timebins_clf_calculator.py` & `Simba-UW-tf-dev-1.63.8/simba/data_processors/timebins_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/data_processors/fsttc_calculator.py` & `Simba-UW-tf-dev-1.63.8/simba/data_processors/fsttc_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/data_processors/interpolate_pose.py` & `Simba-UW-tf-dev-1.63.8/simba/data_processors/interpolate_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/data_processors/directing_other_animals_calculator.py` & `Simba-UW-tf-dev-1.63.8/simba/data_processors/directing_other_animals_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/data_processors/timebins_movement_calculator.py` & `Simba-UW-tf-dev-1.63.8/simba/data_processors/timebins_movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/data_processors/severity_calculator.py` & `Simba-UW-tf-dev-1.63.8/simba/data_processors/severity_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/data_processors/pup_retrieval_calculator.py` & `Simba-UW-tf-dev-1.63.8/simba/data_processors/pup_retrieval_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/data_processors/pybursts_calculator.py` & `Simba-UW-tf-dev-1.63.8/simba/data_processors/pybursts_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/data_processors/severity_frame_based_calculator.py` & `Simba-UW-tf-dev-1.63.8/simba/data_processors/severity_frame_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/data_processors/mutual_exclusivity_corrector.py` & `Simba-UW-tf-dev-1.63.8/simba/data_processors/mutual_exclusivity_corrector.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/data_processors/kleinberg_calculator.py` & `Simba-UW-tf-dev-1.63.8/simba/data_processors/kleinberg_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/data_processors/movement_calculator.py` & `Simba-UW-tf-dev-1.63.8/simba/data_processors/movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store` & `Simba-UW-tf-dev-1.63.8/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.63.8/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.63.8/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.63.8/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.63.8/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store` & `Simba-UW-tf-dev-1.63.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png` & `Simba-UW-tf-dev-1.63.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png` & `Simba-UW-tf-dev-1.63.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png` & `Simba-UW-tf-dev-1.63.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png` & `Simba-UW-tf-dev-1.63.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png` & `Simba-UW-tf-dev-1.63.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png` & `Simba-UW-tf-dev-1.63.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png` & `Simba-UW-tf-dev-1.63.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png` & `Simba-UW-tf-dev-1.63.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png` & `Simba-UW-tf-dev-1.63.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png` & `Simba-UW-tf-dev-1.63.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png` & `Simba-UW-tf-dev-1.63.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png` & `Simba-UW-tf-dev-1.63.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png` & `Simba-UW-tf-dev-1.63.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/model/train_rf.py` & `Simba-UW-tf-dev-1.63.8/simba/model/train_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/model/.DS_Store` & `Simba-UW-tf-dev-1.63.8/simba/model/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/model/inference_batch.py` & `Simba-UW-tf-dev-1.63.8/simba/model/inference_batch.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/model/grid_search_rf.py` & `Simba-UW-tf-dev-1.63.8/simba/model/grid_search_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/model/inference_validation.py` & `Simba-UW-tf-dev-1.63.8/simba/model/inference_validation.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_time_bin_calculator.py` & `Simba-UW-tf-dev-1.63.8/simba/roi_tools/ROI_time_bin_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_movement_analyzer.py` & `Simba-UW-tf-dev-1.63.8/simba/roi_tools/ROI_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/roi_tools/.DS_Store` & `Simba-UW-tf-dev-1.63.8/simba/roi_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_define.py` & `Simba-UW-tf-dev-1.63.8/simba/roi_tools/ROI_define.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_reset.py` & `Simba-UW-tf-dev-1.63.8/simba/roi_tools/ROI_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_analyzer.py` & `Simba-UW-tf-dev-1.63.8/simba/roi_tools/ROI_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_feature_analyzer.py` & `Simba-UW-tf-dev-1.63.8/simba/roi_tools/ROI_feature_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_multiply.py` & `Simba-UW-tf-dev-1.63.8/simba/roi_tools/ROI_multiply.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_size_calculations.py` & `Simba-UW-tf-dev-1.63.8/simba/roi_tools/ROI_size_calculations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_zoom.py` & `Simba-UW-tf-dev-1.63.8/simba/roi_tools/ROI_zoom.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_directing_analyzer.py` & `Simba-UW-tf-dev-1.63.8/simba/roi_tools/ROI_directing_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_move_shape.py` & `Simba-UW-tf-dev-1.63.8/simba/roi_tools/ROI_move_shape.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_menus.py` & `Simba-UW-tf-dev-1.63.8/simba/roi_tools/ROI_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_clf_calculator.py` & `Simba-UW-tf-dev-1.63.8/simba/roi_tools/ROI_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/roi_tools/ROI_image.py` & `Simba-UW-tf-dev-1.63.8/simba/roi_tools/ROI_image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_importers/sleap_csv_importer.py` & `Simba-UW-tf-dev-1.63.8/simba/pose_importers/sleap_csv_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_importers/misc/.DS_Store` & `Simba-UW-tf-dev-1.63.8/simba/pose_importers/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_importers/misc/apt_trk_importer.py` & `Simba-UW-tf-dev-1.63.8/simba/pose_importers/misc/apt_trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_importers/read_DANNCE_mat.py` & `Simba-UW-tf-dev-1.63.8/simba/pose_importers/read_DANNCE_mat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_importers/.DS_Store` & `Simba-UW-tf-dev-1.63.8/simba/pose_importers/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_importers/sleap_h5_importer.py` & `Simba-UW-tf-dev-1.63.8/simba/pose_importers/sleap_h5_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_importers/madlc_importer.py` & `Simba-UW-tf-dev-1.63.8/simba/pose_importers/madlc_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_importers/sleap_slp_importer.py` & `Simba-UW-tf-dev-1.63.8/simba/pose_importers/sleap_slp_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_importers/import_mars.py` & `Simba-UW-tf-dev-1.63.8/simba/pose_importers/import_mars.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_importers/dlc_importer_csv.py` & `Simba-UW-tf-dev-1.63.8/simba/pose_importers/dlc_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_importers/trk_importer.py` & `Simba-UW-tf-dev-1.63.8/simba/pose_importers/trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_configurations/.DS_Store` & `Simba-UW-tf-dev-1.63.8/simba/pose_configurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_configurations/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.63.8/simba/pose_configurations/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_configurations/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.63.8/simba/pose_configurations/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_configurations/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.63.8/simba/pose_configurations/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_configurations/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.63.8/simba/pose_configurations/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_configurations/schematics/8.png` & `Simba-UW-tf-dev-1.63.8/simba/pose_configurations/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_configurations/schematics/9.png` & `Simba-UW-tf-dev-1.63.8/simba/pose_configurations/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_configurations/schematics/12.png` & `Simba-UW-tf-dev-1.63.8/simba/pose_configurations/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_configurations/schematics/11.png` & `Simba-UW-tf-dev-1.63.8/simba/pose_configurations/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_configurations/schematics/10.png` & `Simba-UW-tf-dev-1.63.8/simba/pose_configurations/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_configurations/schematics/4.png` & `Simba-UW-tf-dev-1.63.8/simba/pose_configurations/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_configurations/schematics/5.png` & `Simba-UW-tf-dev-1.63.8/simba/pose_configurations/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_configurations/schematics/7.png` & `Simba-UW-tf-dev-1.63.8/simba/pose_configurations/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_configurations/schematics/6.png` & `Simba-UW-tf-dev-1.63.8/simba/pose_configurations/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_configurations/schematics/2.png` & `Simba-UW-tf-dev-1.63.8/simba/pose_configurations/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_configurations/schematics/3.png` & `Simba-UW-tf-dev-1.63.8/simba/pose_configurations/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/pose_configurations/schematics/1.png` & `Simba-UW-tf-dev-1.63.8/simba/pose_configurations/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/three_dimensions/ui/define_px_to_mm_ui.py` & `Simba-UW-tf-dev-1.63.8/simba/three_dimensions/ui/define_px_to_mm_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/three_dimensions/feature_extractors/generic_feature_extractor.py` & `Simba-UW-tf-dev-1.63.8/simba/three_dimensions/feature_extractors/generic_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/three_dimensions/mixins/config_reader.py` & `Simba-UW-tf-dev-1.63.8/simba/three_dimensions/mixins/config_reader.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.1.nbc` & `Simba-UW-tf-dev-1.63.8/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.1.nbc` & `Simba-UW-tf-dev-1.63.8/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.nbi` & `Simba-UW-tf-dev-1.63.8/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.nbi` & `Simba-UW-tf-dev-1.63.8/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/three_dimensions/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.63.8/simba/three_dimensions/mixins/feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/three_dimensions/mixins/plotting_mixin.py` & `Simba-UW-tf-dev-1.63.8/simba/three_dimensions/mixins/plotting_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/three_dimensions/plotting/plot_pose_in_dir.py` & `Simba-UW-tf-dev-1.63.8/simba/three_dimensions/plotting/plot_pose_in_dir.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/three_dimensions/pose_importers/anipose_csv_import.py` & `Simba-UW-tf-dev-1.63.8/simba/three_dimensions/pose_importers/anipose_csv_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/three_dimensions/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.63.8/simba/three_dimensions/outlier_tools/outlier_corrector_movement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/video_processors/video_processing.py` & `Simba-UW-tf-dev-1.63.8/simba/video_processors/video_processing.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import simba
 from simba.mixins.config_reader import ConfigReader
 from tkinter import *
 from datetime import datetime
 import time
 from PIL import Image, ImageTk
 import multiprocessing
-from typing import List, Union
+from typing import List, Union, Optional
 
 from simba.utils.checks import (check_file_exist_and_readable, check_int, check_if_filepath_list_is_empty)
 from simba.utils.read_write import (get_fn_ext,
                                     get_video_meta_data,
                                     find_all_videos_in_directory,
                                     find_core_cnt,
                                     read_config_entry,
@@ -28,15 +28,16 @@
 from simba.utils.enums import Formats, Paths, ConfigKey
 
 from simba.utils.errors import (NotDirectoryError,
                                 NoFilesFoundError,
                                 FileExistError,
                                 CountError,
                                 InvalidInputError,
-                                DirectoryExistError)
+                                DirectoryExistError,
+                                FFMPEGCodecError)
 from simba.utils.warnings import (SameInputAndOutputWarning,
                                   FileExistWarning)
 
 
 MAX_FRM_SIZE = 1080, 650
 
 def change_img_format(directory: Union[str, os.PathLike],
@@ -158,15 +159,15 @@
     video_meta_data = get_video_meta_data(video_path=file_path)
     dir_name, file_name, ext = get_fn_ext(filepath=file_path)
     if int(fps) == int(video_meta_data['fps']):
         SameInputAndOutputWarning(msg=f'The new fps is the same as the input fps for video {file_name} ({str(fps)})')
     save_path = os.path.join(dir_name, file_name + '_fps_{}{}'.format(str(fps), str(ext)))
     if os.path.isfile(save_path):
         FileExistWarning(msg=f'Overwriting existing file at {save_path}')
-    command = str('ffmpeg -i ') + '"' + str(file_path) + '"' + ' -filter:v fps=fps=' + str(fps) + ' ' + '"' + save_path + '"'
+        command = str('ffmpeg -i ') + '"' + str(file_path) + '"' + ' -filter:v fps=fps=' + str(fps) + ' ' + '"' + save_path + '"'
     subprocess.call(command, shell=True)
     stdout_success(msg=f'SIMBA COMPLETE: FPS of video {file_name} changed from {str(video_meta_data["fps"])} to {str(fps)} and saved in directory {save_path}')
 
 def change_fps_of_multiple_videos(directory: Union[str, os.PathLike],
                                   fps: int) -> None:
     """
     Change the fps of all video files in a folder. Results are stored in the same directory as in the input files with
@@ -237,15 +238,14 @@
     if os.path.isfile(save_name):
         raise FileExistError(msg='SIMBA ERROR: The outfile file already exist: {}.'.format(save_name))
     command = (str('ffmpeg -i ') + '"' + str(file_path) + '"' + ' ' + '"' + save_name + '"')
     print('Converting to mp4... ')
     subprocess.call(command, shell=True, stdout=subprocess.PIPE)
     stdout_success(msg=f'SIMBA COMPLETE: Video converted! {save_name} generated!')
 
-
 def video_to_greyscale(file_path: Union[str, os.PathLike]) -> None:
     """
     Convert a video file to greyscale mp4 format. The result is stored in the same directory as the
     input file with the ``_grayscale.mp4`` suffix.
 
     :parameter Union[str, os.PathLike] file_path: Path to video file.
 
@@ -411,15 +411,15 @@
     stored in the same directory as the input files.
 
     :parameter Union[str, os.PathLike] directory: Path to video file directory.
     :parameter str input_format: Format of the input files (e.g., avi).
     :parameter str output_format: Format of the output files (e.g., mp4).
 
     :example:
-    >>> _ = gif_creator(directory='project_folder/videos', input_format='avi', output_format='mp4')
+    >>> _ = batch_convert_video_format(directory='project_folder/videos', input_format='avi', output_format='mp4')
     """
 
     if not os.path.isdir(directory):
         raise NotDirectoryError(msg='SIMBA ERROR: {} is not a valid directory'.format(directory))
     video_paths = []
     file_paths_in_folder = [f for f in glob.glob(directory + '/*') if os.path.isfile(f)]
     for file_path in file_paths_in_folder:
@@ -649,29 +649,29 @@
     subprocess.call(command, shell=True)
     stdout_success(msg=f'Video created at {save_path}')
 
 
 def video_concatenator(video_one_path: Union[str, os.PathLike],
                        video_two_path: Union[str, os.PathLike],
                        resolution: Union[int, str],
-                       horizontal: bool) -> None:
+                       horizontal: bool,
+                       gpu: Optional[bool] = False) -> None:
 
     """
     Concatenate two videos to a single video
 
     :param str video_one_path: Path to the first video in the concatenated video
     :param str video_two_path: Path to the second video in the concatenated video
     :param int or str resolution: If str, then the name of the video which resolution you want to retain. E.g., `Video_1`. Else int, representing the video width (if vertical concat) or height (if horizontal concat). Aspect raio will be retained.
     :param horizontal: If true, then horizontal concatenation. Else vertical concatenation.
 
     :example:
     >>> video_concatenator(video_one_path='project_folder/videos/Video_1.mp4', video_two_path='project_folder/videos/Video_2.mp4', resolution=800, horizontal=True)
     """
-
-
+    timer = SimbaTimer(start=True)
     for file_path in [video_one_path, video_two_path]:
         check_file_exist_and_readable(file_path=file_path)
         _ = get_video_meta_data(file_path)
     if type(resolution) is int:
         video_meta_data = {}
         if horizontal:
             video_meta_data['height'] = resolution
@@ -679,23 +679,39 @@
             video_meta_data['width'] = resolution
     elif resolution is 'Video 1':
         video_meta_data = get_video_meta_data(video_one_path)
     else:
         video_meta_data = get_video_meta_data(video_one_path)
     dir, file_name_1, _ = get_fn_ext(video_one_path)
     _, file_name_2, _ = get_fn_ext(video_two_path)
-    print('Concatenating videos...')
+    print(f'Concatenating videos {file_name_1} and {file_name_2}...')
     save_path = os.path.join(dir, file_name_1 + file_name_2 + '_concat.mp4')
     if horizontal:
-        command = 'ffmpeg -y -i "{}" -i "{}" -filter_complex "[0:v]scale=-1:{}[v0];[v0][1:v]hstack=inputs=2" "{}"'.format(video_one_path, video_two_path, video_meta_data['height'], save_path)
+        if gpu:
+            command = f'ffmpeg -y -hwaccel cuvid -c:v h264_cuvid -i "{video_one_path}" -hwaccel cuvid -c:v h264_cuvid -i "{video_two_path}" -filter_complex "[0:v]scale=-1:<height>[v0];[v0][1:v]hstack=inputs=2" -c:v h264_nvenc "{save_path}"'
+        else:
+            command = 'ffmpeg -y -i "{}" -i "{}" -filter_complex "[0:v]scale=-1:{}[v0];[v0][1:v]hstack=inputs=2" "{}"'.format(video_one_path, video_two_path, video_meta_data['height'], save_path)
     else:
-        command = 'ffmpeg -y -i "{}" -i "{}" -filter_complex "[0:v]scale={}:-1[v0];[v0][1:v]vstack=inputs=2" "{}"'.format(video_one_path, video_two_path, video_meta_data['width'], save_path)
-    subprocess.call(command, shell=True, stdout=subprocess.PIPE)
-    stdout_success(msg=f'Videos concatenated and saved at {save_path}')
+        if gpu:
+            command = f'ffmpeg -y -hwaccel cuvid -c:v h264_cuvid -i "{video_one_path}" -hwaccel cuvid -c:v h264_cuvid -i "{video_two_path}" -filter_complex "[0:v]scale=<width>:-1[v0];[v0][1:v]vstack=inputs=2" -c:v h264_nvenc "{save_path}"'
+        else:
+            command = 'ffmpeg -y -i "{}" -i "{}" -filter_complex "[0:v]scale={}:-1[v0];[v0][1:v]vstack=inputs=2" "{}"'.format(video_one_path, video_two_path, video_meta_data['width'], save_path)
 
+    if gpu:
+        process = subprocess.Popen(command.split(' '), stdout = subprocess.PIPE, stderr = subprocess.PIPE)
+        output, error = process.communicate()
+        if process.returncode != 0:
+            #if 'Unknown decoder' in str(error.split(b'\n')[-2]):
+            raise FFMPEGCodecError(msg='GPU codec not found: reverting to CPU. Properly configure FFMpeg and ensure you have GPU available or use CPU.')
+        else:
+            pass
+    else:
+       subprocess.call(command, shell=True)
+    timer.stop_timer()
+    stdout_success(msg=f'Videos concatenated and saved at {save_path}', elapsed_time=timer.elapsed_time_str)
 
 class VideoRotator(ConfigReader):
     """
     GUI Tool for rotating video. Rotated video is saved with the ``_rotated_DATETIME.mp4`` suffix.
 
     :parameter str input_path: Path to video to rotate.
     :parameter str output_dir: Directory where to save the rotated video.
@@ -848,15 +864,14 @@
 
     :parameter str config_path: path to SimBA project config file in Configparser format.
     :parameter str source: path to image folder outside SimBA project.
 
     :example:
     >>> copy_img_folder(config_path='MySimBAprojectConfig', source='/DirectoryWithVideos/')
 
-
     """
     timer = SimbaTimer(start=True)
     if not os.path.isdir(source):
         raise NotDirectoryError(msg=f'SIMBA ERROR: source {source} is not a directory.')
     if len(glob.glob(source + '/*.png')) == 0:
         raise NoFilesFoundError(msg=f'SIMBA ERROR: source {source} does not contain any .png files.')
     input_basename = os.path.basename(source)
@@ -879,8 +894,12 @@
 
 # video_concatenator(video_one_path='/Users/simon/Desktop/troubleshooting/Open_field_5/project_folder/frames/output/gantt_plots/SI_DAY3_308_CD1_PRESENT_2.mp4',
 #                    video_two_path= '/Users/simon/Desktop/troubleshooting/Open_field_5/project_folder/frames/output/gantt_plots/SI_DAY3_308_CD1_PRESENT.mp4',
 #                    resolution='Video 1',
 #                    horizontal=False)
 
 
-
+# video_concatenator(video_one_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/videos/Together_1.avi',
+#                    video_two_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/videos/Together_1.avi',
+#                    resolution='Video_1',
+#                    horizontal=True,
+#                    gpu=False)
```

### Comparing `Simba-UW-tf-dev-1.63.7/simba/video_processors/.DS_Store` & `Simba-UW-tf-dev-1.63.8/simba/video_processors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/video_processors/px_to_mm.py` & `Simba-UW-tf-dev-1.63.8/simba/video_processors/px_to_mm.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/video_processors/batch_process_menus.py` & `Simba-UW-tf-dev-1.63.8/simba/video_processors/batch_process_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/video_processors/multi_cropper.py` & `Simba-UW-tf-dev-1.63.8/simba/video_processors/multi_cropper.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/video_processors/extract_frames.py` & `Simba-UW-tf-dev-1.63.8/simba/video_processors/extract_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/video_processors/calculate_px_dist.py` & `Simba-UW-tf-dev-1.63.8/simba/video_processors/calculate_px_dist.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/video_processors/extract_seqframes.py` & `Simba-UW-tf-dev-1.63.8/simba/video_processors/extract_seqframes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/video_processors/batch_process_create_ffmpeg_commands.py` & `Simba-UW-tf-dev-1.63.8/simba/video_processors/batch_process_create_ffmpeg_commands.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.63.8/simba/outlier_tools/outlier_corrector_movement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/outlier_tools/.DS_Store` & `Simba-UW-tf-dev-1.63.8/simba/outlier_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/outlier_tools/outlier_corrector_location.py` & `Simba-UW-tf-dev-1.63.8/simba/outlier_tools/outlier_corrector_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/outlier_tools/skip_outlier_correction.py` & `Simba-UW-tf-dev-1.63.8/simba/outlier_tools/skip_outlier_correction.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/outlier_tools/.idea/outlier_scripts.iml` & `Simba-UW-tf-dev-1.63.8/simba/outlier_tools/.idea/outlier_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.63.8/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/outlier_tools/.idea/workspace.xml` & `Simba-UW-tf-dev-1.63.8/simba/outlier_tools/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/SimBA.py` & `Simba-UW-tf-dev-1.63.8/simba/SimBA.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 from simba.ui.pop_ups.roi_analysis_pop_up import ROIAnalysisPopUp
 from simba.ui.pop_ups.append_roi_features_animals_pop_up import AppendROIFeaturesByAnimalPopUp
 from simba.ui.pop_ups.movement_analysis_time_bins_pop_up import MovementAnalysisTimeBinsPopUp
 from simba.ui.pop_ups.heatmap_location_pop_up import HeatmapLocationPopup
 from simba.ui.pop_ups.quick_path_plot_pop_up import QuickLineplotPopup
 from simba.ui.pop_ups.clf_by_roi_pop_up import ClfByROIPopUp
 from simba.ui.pop_ups.fsttc_pop_up import FSTTCPopUp
+from simba.ui.pop_ups.mutual_exclusivity_pop_up import MutualExclusivityPupUp
 from simba.ui.pop_ups.kleinberg_pop_up import KleinbergPopUp
 from simba.ui.pop_ups.clf_by_timebins_pop_up import TimeBinsClfPopUp
 from simba.ui.pop_ups.clf_descriptive_statistics_pop_up import ClfDescriptiveStatsPopUp
 from simba.ui.pop_ups.visualize_pose_in_dir_pop_up import VisualizePoseInFolderPopUp
 from simba.ui.pop_ups.gantt_pop_up import GanttPlotPopUp
 from simba.ui.pop_ups.path_plot_pop_up import PathPlotPopUp
 from simba.ui.pop_ups.distance_plot_pop_up import DistancePlotterPopUp
@@ -382,14 +383,15 @@
         button_run_rfmodelsettings.image = self.btn_icons['settings']['img']
 
         button_runmachinemodel = Button(label_runmachinemodel,text='RUN MODELS', fg='green', compound='left', image=self.btn_icons['clf']['img'], command=self.runrfmodel)
         button_runmachinemodel.image = self.btn_icons['clf']['img']
 
         kleinberg_button = Button(label_runmachinemodel,text='KLEINBERG SMOOTHING', fg='green', command=lambda: KleinbergPopUp(config_path=self.config_path))
         fsttc_button = Button(label_runmachinemodel,text='FSTTC', fg='green', command=lambda:FSTTCPopUp(config_path=self.config_path))
+        mutual_exclusivity = Button(label_runmachinemodel, text='MUTUAL EXCLUSIVITY CORRECTION', fg='green', command=lambda: MutualExclusivityPupUp(config_path=self.config_path))
 
         label_machineresults = CreateLabelFrameWithIcon(parent=tab9, header='ANALYZE MACHINE RESULTS', icon_name=Keys.DOCUMENTATION.value, icon_link=Links.ANALYZE_ML_RESULTS.value)
         button_process_datalog = Button(label_machineresults, text='ANALYZE MACHINE PREDICTIONS: AGGREGATES', fg='blue', command=lambda: ClfDescriptiveStatsPopUp(config_path=self.config_path))
         button_process_movement = Button(label_machineresults, text='ANALYZE DISTANCES/VELOCITY: AGGREGATES', fg='blue', command=lambda: MovementAnalysisPopUp(config_path=self.config_path))
         button_movebins = Button(label_machineresults, text='ANALYZE DISTANCES/VELOCITY: TIME BINS', fg='blue', command=lambda: MovementAnalysisTimeBinsPopUp(config_path=self.config_path))
         button_classifierbins = Button(label_machineresults,text='ANALYZE MACHINE PREDICTIONS: TIME-BINS', fg='blue', command=lambda: TimeBinsClfPopUp(config_path=self.config_path))
         button_classifier_ROI = Button(label_machineresults, text='ANALYZE MACHINE PREDICTION: BY ROI', fg='blue', command=lambda: ClfByROIPopUp(config_path=self.config_path))
@@ -522,14 +524,15 @@
         button_validate_model.grid(row=6, sticky=W)
 
         label_runmachinemodel.grid(row=8,sticky=NW)
         button_run_rfmodelsettings.grid(row=0,sticky=NW)
         button_runmachinemodel.grid(row=1,sticky=NW)
         kleinberg_button.grid(row=2,sticky=NW)
         fsttc_button.grid(row=3,sticky=NW)
+        mutual_exclusivity.grid(row=4,sticky=NW)
 
         label_machineresults.grid(row=9,sticky=W,pady=5)
         button_process_datalog.grid(row=2,column=0,sticky=W,padx=3)
         button_process_movement.grid(row=2,column=1,sticky=W,padx=3)
         button_movebins.grid(row=3,column=1,sticky=W,padx=3)
         button_classifierbins.grid(row=3,column=0,sticky=W,padx=3)
         button_classifier_ROI.grid(row=4, column=0, sticky=W, padx=3)
```

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.63.8/simba/assets/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/unsupervised/model_names.parquet` & `Simba-UW-tf-dev-1.63.8/simba/assets/unsupervised/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/unsupervised/features.csv` & `Simba-UW-tf-dev-1.63.8/simba/assets/unsupervised/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/shap/down_arrow.jpg` & `Simba-UW-tf-dev-1.63.8/simba/assets/shap/down_arrow.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/shap/intruder_shape.jpg` & `Simba-UW-tf-dev-1.63.8/simba/assets/shap/intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/shap/feature_categories/shap_feature_categories.csv` & `Simba-UW-tf-dev-1.63.8/simba/assets/shap/feature_categories/shap_feature_categories.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/shap/.DS_Store` & `Simba-UW-tf-dev-1.63.8/simba/assets/shap/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/shap/resident_shape.jpg` & `Simba-UW-tf-dev-1.63.8/simba/assets/shap/resident_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/shap/resident_intruder_shape.jpg` & `Simba-UW-tf-dev-1.63.8/simba/assets/shap/resident_intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/shap/animal_distances.jpg` & `Simba-UW-tf-dev-1.63.8/simba/assets/shap/animal_distances.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/shap/baseline_scale.jpg` & `Simba-UW-tf-dev-1.63.8/simba/assets/shap/baseline_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/shap/ubuntu.regular.ttf` & `Simba-UW-tf-dev-1.63.8/simba/assets/shap/ubuntu.regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/shap/side_scale.jpg` & `Simba-UW-tf-dev-1.63.8/simba/assets/shap/side_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/shap/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.63.8/simba/assets/shap/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/shap/side_scale_5.jpg` & `Simba-UW-tf-dev-1.63.8/simba/assets/shap/side_scale_5.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/shap/intruder_movement.jpg` & `Simba-UW-tf-dev-1.63.8/simba/assets/shap/intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/shap/resident_movement.jpg` & `Simba-UW-tf-dev-1.63.8/simba/assets/shap/resident_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/shap/color_bar.jpg` & `Simba-UW-tf-dev-1.63.8/simba/assets/shap/color_bar.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/shap/resident_intruder_movement.jpg` & `Simba-UW-tf-dev-1.63.8/simba/assets/shap/resident_intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/.DS_Store` & `Simba-UW-tf-dev-1.63.8/simba/assets/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/lookups/.DS_Store` & `Simba-UW-tf-dev-1.63.8/simba/assets/lookups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/lookups/model_names.parquet` & `Simba-UW-tf-dev-1.63.8/simba/assets/lookups/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/lookups/feature_extraction_headers.csv` & `Simba-UW-tf-dev-1.63.8/simba/assets/lookups/feature_extraction_headers.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/lookups/features.csv` & `Simba-UW-tf-dev-1.63.8/simba/assets/lookups/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/lookups/unsupervised_example_x.csv` & `Simba-UW-tf-dev-1.63.8/simba/assets/lookups/unsupervised_example_x.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/stl/operant_tray.stl` & `Simba-UW-tf-dev-1.63.8/simba/assets/stl/operant_tray.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/stl/operant_lever.stl` & `Simba-UW-tf-dev-1.63.8/simba/assets/stl/operant_lever.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/stl/operant_walls.stl` & `Simba-UW-tf-dev-1.63.8/simba/assets/stl/operant_walls.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/stl/grid_floor.stl` & `Simba-UW-tf-dev-1.63.8/simba/assets/stl/grid_floor.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/img/.DS_Store` & `Simba-UW-tf-dev-1.63.8/simba/assets/img/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/img/about_me.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/img/about_me.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/img/splash.mp4` & `Simba-UW-tf-dev-1.63.8/simba/assets/img/splash.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/img/bg_2.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/img/bg_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/img/splash.pptx` & `Simba-UW-tf-dev-1.63.8/simba/assets/img/splash.pptx`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/img/bg.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.63.8/simba/assets/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/factory.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/factory.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/cluster.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/cluster.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/load.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/load.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/gif.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/gif.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/pose.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/pose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/features.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/features.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/.DS_Store` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/settings.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/stopwatch.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/stopwatch.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/link.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/link.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/dash_simba.css` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/dash_simba.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/documentation.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/fps.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/fps.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/dimensionality_reduction.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/dimensionality_reduction.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/roi.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/superimpose.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/superimpose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/label.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/label.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/change.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/change.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/crop.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/crop.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/rotate.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/path.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/path.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/clip.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/clip.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/restart.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/restart.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/calipher.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/calipher.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/add_on.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/add_on.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/create.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/create.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/SimBA_logo.ico` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/print.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/print.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/clf.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/clf.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/concat_icons/mosaic.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/concat_icons/mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/concat_icons/vertical.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/concat_icons/vertical.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/concat_icons/horizontal.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/concat_icons/horizontal.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/concat_icons/mixed_mosaic.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/concat_icons/mixed_mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/merge.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/clean.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/clean.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/clf_2.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/clf_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/visualize.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/visualize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/concat.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/concat.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/boris.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/boris.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/frames.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/frames.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/video.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/video.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/sample.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/sample.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/metrics.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/metrics.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/grey.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/grey.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/exit.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/exit.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/outlier.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/outlier.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/clahe.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/clahe.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/trash.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/trash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/about.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/about.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/convert.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/convert.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/SimBA_logo.icns` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/SimBA_logo.icns`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/reorganize.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/reorganize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/browse.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/browse.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/SimBA_logo.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/SimBA_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/ethovision.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/ethovision.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/icons/close.png` & `Simba-UW-tf-dev-1.63.8/simba/assets/icons/close.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/dash_simba_base.css` & `Simba-UW-tf-dev-1.63.8/simba/assets/dash_simba_base.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/simba/assets/TheGoldenLab.PNG` & `Simba-UW-tf-dev-1.63.8/simba/assets/TheGoldenLab.PNG`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/Simba_UW_tf_dev.egg-info/PKG-INFO` & `Simba-UW-tf-dev-1.63.8/Simba_UW_tf_dev.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.63.7
+Version: 1.63.8
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.63.7/Simba_UW_tf_dev.egg-info/SOURCES.txt` & `Simba-UW-tf-dev-1.63.8/Simba_UW_tf_dev.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -206,14 +206,15 @@
 simba/mixins/config_reader.py
 simba/mixins/feature_extraction_mixin.py
 simba/mixins/plotting_mixin.py
 simba/mixins/pop_up_mixin.py
 simba/mixins/pose_importer_mixin.py
 simba/mixins/train_model_mixin.py
 simba/mixins/unsupervised_mixin.py
+simba/mixins/video_processing_mixin.py
 simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc
 simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.2.nbc
 simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi
 simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc
 simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi
 simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.1.nbc
 simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.nbi
@@ -459,14 +460,15 @@
 simba/video_processors/batch_process_menus.py
 simba/video_processors/calculate_px_dist.py
 simba/video_processors/extract_frames.py
 simba/video_processors/extract_seqframes.py
 simba/video_processors/multi_cropper.py
 simba/video_processors/px_to_mm.py
 simba/video_processors/video_processing.py
+simba/video_processors/video_processing_new.py
 tests/__init__.py
 tests/test_config_reader_mixin.py
 tests/test_data_processors.py
 tests/test_distance_plotter.py
 tests/test_feature_extraction_mixin.py
 tests/test_featurizers.py
 tests/test_interpolation_smoothing.py
```

### Comparing `Simba-UW-tf-dev-1.63.7/Simba_UW_tf_dev.egg-info/requires.txt` & `Simba-UW-tf-dev-1.63.8/Simba_UW_tf_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/LICENSE.md` & `Simba-UW-tf-dev-1.63.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/tests/test_data_processors.py` & `Simba-UW-tf-dev-1.63.8/tests/test_data_processors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/tests/test_distance_plotter.py` & `Simba-UW-tf-dev-1.63.8/tests/test_distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/tests/test_train_model_mixin.py` & `Simba-UW-tf-dev-1.63.8/tests/test_train_model_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/tests/test_pose_importers.py` & `Simba-UW-tf-dev-1.63.8/tests/test_pose_importers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/tests/test_feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.63.8/tests/test_feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/tests/test_utils_data.py` & `Simba-UW-tf-dev-1.63.8/tests/test_utils_data.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/tests/test_config_reader_mixin.py` & `Simba-UW-tf-dev-1.63.8/tests/test_config_reader_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/tests/test_outlier_correctors.py` & `Simba-UW-tf-dev-1.63.8/tests/test_outlier_correctors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/tests/test_visualize_directing_animals.py` & `Simba-UW-tf-dev-1.63.8/tests/test_visualize_directing_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/tests/test_featurizers.py` & `Simba-UW-tf-dev-1.63.8/tests/test_featurizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/tests/test_video_processors.py` & `Simba-UW-tf-dev-1.63.8/tests/test_video_processors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py` & `Simba-UW-tf-dev-1.63.8/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/tests/test_thirdparty_appenders.py` & `Simba-UW-tf-dev-1.63.8/tests/test_thirdparty_appenders.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/tests/test_validation_clips.py` & `Simba-UW-tf-dev-1.63.8/tests/test_validation_clips.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/tests/test_roi_tools.py` & `Simba-UW-tf-dev-1.63.8/tests/test_roi_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/README.md` & `Simba-UW-tf-dev-1.63.8/README.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.63.7/setup.py` & `Simba-UW-tf-dev-1.63.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Licensed under GNU Lesser General Public License v3.0
 """
 
 import setuptools
 
 setuptools.setup(
     name="Simba-UW-tf-dev",
-    version="1.63.7",
+    version="1.63.8",
     author="Simon Nilsson, Jia Jie Choong, Sophia Hwang",
     author_email="sronilsson@gmail.com",
     description="Toolkit for computer classification of complex social behaviors in experimental animals",
     url="https://github.com/sgoldenlab/simba",
     install_requires=['Pillow == 5.4.1', 'pyyaml == 5.3.1','shapely == 1.7','wxpython == 4.0.4',
               'dtreeviz == 0.8.1','eli5 == 0.10.1','graphviz == 0.11',
               'imblearn == 0.0','imgaug == 0.4.0','imutils == 0.5.2','matplotlib == 3.0.3', 'numpy == 1.18.1',
```

