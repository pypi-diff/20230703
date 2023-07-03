# Comparing `tmp/pyrfuniverse-0.8.5.tar.gz` & `tmp/pyrfuniverse-0.9.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrfuniverse-0.8.5.tar", last modified: Wed Jun 14 03:58:23 2023, max compression
+gzip compressed data, was "pyrfuniverse-0.9.10.tar", last modified: Mon Jul  3 04:47:49 2023, max compression
```

## Comparing `pyrfuniverse-0.8.5.tar` & `pyrfuniverse-0.9.10.tar`

### file list

```diff
@@ -1,174 +1,125 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 03:58:23.639599 pyrfuniverse-0.8.5/
--rw-rw-rw-   0        0        0    11357 2022-08-10 05:19:33.000000 pyrfuniverse-0.8.5/LICENSE
--rw-rw-rw-   0        0        0      263 2023-06-14 03:58:23.639599 pyrfuniverse-0.8.5/PKG-INFO
--rw-rw-rw-   0        0        0     2758 2023-05-28 07:57:50.000000 pyrfuniverse-0.8.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 03:58:22.980572 pyrfuniverse-0.8.5/pyrfuniverse/
--rw-rw-rw-   0        0        0      758 2023-06-02 08:36:48.000000 pyrfuniverse-0.8.5/pyrfuniverse/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:58:23.086829 pyrfuniverse-0.8.5/pyrfuniverse/attributes/
--rw-rw-rw-   0        0        0     1472 2023-06-13 10:32:18.000000 pyrfuniverse-0.8.5/pyrfuniverse/attributes/__init__.py
--rw-rw-rw-   0        0        0     4881 2023-05-28 07:57:51.000000 pyrfuniverse-0.8.5/pyrfuniverse/attributes/activelightsensor_attr.py
--rw-rw-rw-   0        0        0    15090 2023-05-28 07:57:51.000000 pyrfuniverse-0.8.5/pyrfuniverse/attributes/base_attr.py
--rw-rw-rw-   0        0        0    18228 2023-05-28 07:57:51.000000 pyrfuniverse-0.8.5/pyrfuniverse/attributes/camera_attr.py
--rw-rw-rw-   0        0        0      528 2023-05-28 07:57:51.000000 pyrfuniverse-0.8.5/pyrfuniverse/attributes/cloth_attr.py
--rw-rw-rw-   0        0        0     1229 2023-05-28 07:57:51.000000 pyrfuniverse-0.8.5/pyrfuniverse/attributes/collider_attr.py
--rw-rw-rw-   0        0        0    34457 2023-05-30 04:20:58.000000 pyrfuniverse-0.8.5/pyrfuniverse/attributes/controller_attr.py
--rw-rw-rw-   0        0        0     1563 2023-05-28 07:57:51.000000 pyrfuniverse-0.8.5/pyrfuniverse/attributes/custom_attr.py
--rw-rw-rw-   0        0        0     1141 2023-05-28 07:57:51.000000 pyrfuniverse-0.8.5/pyrfuniverse/attributes/digit_attr.py
--rw-rw-rw-   0        0        0     1758 2023-06-02 02:37:47.000000 pyrfuniverse-0.8.5/pyrfuniverse/attributes/fallingcloth_attr.py
--rw-rw-rw-   0        0        0     3655 2023-05-28 07:57:51.000000 pyrfuniverse-0.8.5/pyrfuniverse/attributes/gameobject_attr.py
--rw-rw-rw-   0        0        0     5700 2023-05-28 07:57:51.000000 pyrfuniverse-0.8.5/pyrfuniverse/attributes/graspsim_attr.py
--rw-rw-rw-   0        0        0     8856 2023-05-28 07:57:51.000000 pyrfuniverse-0.8.5/pyrfuniverse/attributes/humanbody_attr.py
--rw-rw-rw-   0        0        0     3591 2023-05-28 07:57:51.000000 pyrfuniverse-0.8.5/pyrfuniverse/attributes/light_attr.py
--rw-rw-rw-   0        0        0     9293 2023-06-13 10:32:18.000000 pyrfuniverse-0.8.5/pyrfuniverse/attributes/omplmanager_attr.py
--rw-rw-rw-   0        0        0     1998 2023-05-28 07:57:51.000000 pyrfuniverse-0.8.5/pyrfuniverse/attributes/pointcloud_attr.py
--rw-rw-rw-   0        0        0     3854 2023-05-28 07:57:51.000000 pyrfuniverse-0.8.5/pyrfuniverse/attributes/rigidbody_attr.py
--rw-rw-rw-   0        0        0      529 2023-05-28 07:57:51.000000 pyrfuniverse-0.8.5/pyrfuniverse/attributes/softbody_attr.py
--rw-rw-rw-   0        0        0    23240 2023-05-28 07:57:51.000000 pyrfuniverse-0.8.5/pyrfuniverse/base_env.py
--rw-rw-rw-   0        0        0     1928 2023-05-28 07:57:51.000000 pyrfuniverse-0.8.5/pyrfuniverse/communicator.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:58:23.240577 pyrfuniverse-0.8.5/pyrfuniverse/communicator_objects/
--rw-rw-rw-   0        0        0      835 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.5/pyrfuniverse/communicator_objects/__init__.py
--rw-rw-rw-   0        0        0     3785 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.5/pyrfuniverse/communicator_objects/agent_action_pb2.py
--rw-rw-rw-   0        0        0     3885 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.5/pyrfuniverse/communicator_objects/agent_info_action_pair_pb2.py
--rw-rw-rw-   0        0        0     5849 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.5/pyrfuniverse/communicator_objects/agent_info_pb2.py
--rw-rw-rw-   0        0        0     8080 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.5/pyrfuniverse/communicator_objects/brain_parameters_pb2.py
--rw-rw-rw-   0        0        0     5258 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.5/pyrfuniverse/communicator_objects/capabilities_pb2.py
--rw-rw-rw-   0        0        0     2073 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.5/pyrfuniverse/communicator_objects/command_pb2.py
--rw-rw-rw-   0        0        0     2134 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.5/pyrfuniverse/communicator_objects/custom_reset_parameters_pb2.py
--rw-rw-rw-   0        0        0     4261 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.5/pyrfuniverse/communicator_objects/demonstration_meta_pb2.py
--rw-rw-rw-   0        0        0     4647 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.5/pyrfuniverse/communicator_objects/engine_configuration_pb2.py
--rw-rw-rw-   0        0        0     2709 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.5/pyrfuniverse/communicator_objects/header_pb2.py
--rw-rw-rw-   0        0        0     9625 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.5/pyrfuniverse/communicator_objects/observation_pb2.py
--rw-rw-rw-   0        0        0     1979 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.5/pyrfuniverse/communicator_objects/space_type_pb2.py
--rw-rw-rw-   0        0        0    12746 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.5/pyrfuniverse/communicator_objects/training_analytics_pb2.py
--rw-rw-rw-   0        0        0     3893 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.5/pyrfuniverse/communicator_objects/unity_input_pb2.py
--rw-rw-rw-   0        0        0     4553 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.5/pyrfuniverse/communicator_objects/unity_message_pb2.py
--rw-rw-rw-   0        0        0     3928 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.5/pyrfuniverse/communicator_objects/unity_output_pb2.py
--rw-rw-rw-   0        0        0     4512 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.5/pyrfuniverse/communicator_objects/unity_rl_initialization_input_pb2.py
--rw-rw-rw-   0        0        0     5963 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.5/pyrfuniverse/communicator_objects/unity_rl_initialization_output_pb2.py
--rw-rw-rw-   0        0        0     8094 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.5/pyrfuniverse/communicator_objects/unity_rl_input_pb2.py
--rw-rw-rw-   0        0        0     7216 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.5/pyrfuniverse/communicator_objects/unity_rl_output_pb2.py
--rw-rw-rw-   0        0        0     2353 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.5/pyrfuniverse/communicator_objects/unity_to_external_pb2.py
--rw-rw-rw-   0        0        0     1775 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.5/pyrfuniverse/communicator_objects/unity_to_external_pb2_grpc.py
--rw-rw-rw-   0        0        0     5302 2023-05-28 07:57:51.000000 pyrfuniverse-0.8.5/pyrfuniverse/env_utils.py
--rw-rw-rw-   0        0        0    22704 2023-05-28 07:57:51.000000 pyrfuniverse-0.8.5/pyrfuniverse/environment.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:58:23.294875 pyrfuniverse-0.8.5/pyrfuniverse/envs/
--rw-rw-rw-   0        0        0    14453 2023-04-07 06:50:32.000000 pyrfuniverse-0.8.5/pyrfuniverse/envs/__init__.py
--rw-rw-rw-   0        0        0     4178 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.5/pyrfuniverse/envs/balance_ball_env.py
--rw-rw-rw-   0        0        0    27872 2023-06-13 10:24:47.000000 pyrfuniverse-0.8.5/pyrfuniverse/envs/base_env.py
--rw-rw-rw-   0        0        0     4564 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.5/pyrfuniverse/envs/bouncer_env.py
--rw-rw-rw-   0        0        0     3982 2023-02-10 17:44:39.000000 pyrfuniverse-0.8.5/pyrfuniverse/envs/franka_grasp_env.py
--rw-rw-rw-   0        0        0     3077 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.5/pyrfuniverse/envs/franka_push_env.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:58:23.329532 pyrfuniverse-0.8.5/pyrfuniverse/envs/gripper_nail/
--rw-rw-rw-   0        0        0      736 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.5/pyrfuniverse/envs/gripper_nail/__init__.py
--rw-rw-rw-   0        0        0     4209 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.5/pyrfuniverse/envs/gripper_nail/nail_can_env.py
--rw-rw-rw-   0        0        0     5750 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.5/pyrfuniverse/envs/gripper_nail/nail_card_env.py
--rw-rw-rw-   0        0        0     3917 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.5/pyrfuniverse/envs/gripper_nail/robotiq85_insert_env.py
--rw-rw-rw-   0        0        0     4149 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.5/pyrfuniverse/envs/gripper_nail/robotiq85_nail_book_env.py
--rw-rw-rw-   0        0        0     4220 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.5/pyrfuniverse/envs/gripper_nail/robotiq85_nail_can_env.py
--rw-rw-rw-   0        0        0     5917 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.5/pyrfuniverse/envs/gripper_nail/robotiq85_nail_card_env.py
--rw-rw-rw-   0        0        0     5696 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.5/pyrfuniverse/envs/gripper_nail/robotiq85_nail_coin_env.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:58:23.341570 pyrfuniverse-0.8.5/pyrfuniverse/envs/multi_agent/
--rw-rw-rw-   0        0        0      172 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.5/pyrfuniverse/envs/multi_agent/__init__.py
--rw-rw-rw-   0        0        0     9111 2023-02-10 17:44:39.000000 pyrfuniverse-0.8.5/pyrfuniverse/envs/multi_agent/cleaner_env.py
--rw-rw-rw-   0        0        0    11818 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.5/pyrfuniverse/envs/multi_agent/navigation_env.py
--rw-rw-rw-   0        0        0     6000 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.5/pyrfuniverse/envs/multi_agent_navigation_env.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:58:23.360150 pyrfuniverse-0.8.5/pyrfuniverse/envs/multi_physics/
--rw-rw-rw-   0        0        0      871 2023-05-28 07:57:51.000000 pyrfuniverse-0.8.5/pyrfuniverse/envs/multi_physics/__init__.py
--rw-rw-rw-   0        0        0    17018 2023-06-02 02:26:31.000000 pyrfuniverse-0.8.5/pyrfuniverse/envs/multi_physics/flexiv_cutting.py
--rw-rw-rw-   0        0        0     8228 2023-06-02 03:13:38.000000 pyrfuniverse-0.8.5/pyrfuniverse/envs/multi_physics/kinova_gen2_catching_cloth_env.py
--rw-rw-rw-   0        0        0    10184 2023-06-02 03:13:38.000000 pyrfuniverse-0.8.5/pyrfuniverse/envs/multi_physics/ur5_water_shooting.py
--rw-rw-rw-   0        0        0      513 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.5/pyrfuniverse/envs/rfuniverse_robot_hub_env.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:58:23.394632 pyrfuniverse-0.8.5/pyrfuniverse/envs/robotics/
--rw-rw-rw-   0        0        0      675 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.5/pyrfuniverse/envs/robotics/__init__.py
--rw-rw-rw-   0        0        0     7357 2022-12-15 06:20:36.000000 pyrfuniverse-0.8.5/pyrfuniverse/envs/robotics/franka_cloth_env.py
--rw-rw-rw-   0        0        0     7455 2022-12-15 06:20:57.000000 pyrfuniverse-0.8.5/pyrfuniverse/envs/robotics/franka_cloth_fold_env.py
--rw-rw-rw-   0        0        0     9747 2023-06-02 03:13:38.000000 pyrfuniverse-0.8.5/pyrfuniverse/envs/robotics/franka_robotics_env.py
--rw-rw-rw-   0        0        0     8041 2022-12-15 06:20:52.000000 pyrfuniverse-0.8.5/pyrfuniverse/envs/robotics/franka_softbody_env.py
--rw-rw-rw-   0        0        0      817 2022-12-15 05:37:19.000000 pyrfuniverse-0.8.5/pyrfuniverse/envs/robotics/pick_and_place_env.py
--rw-rw-rw-   0        0        0      754 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.5/pyrfuniverse/envs/robotics/push_env.py
--rw-rw-rw-   0        0        0      864 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.5/pyrfuniverse/envs/robotics/reach_env.py
--rw-rw-rw-   0        0        0     4463 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.5/pyrfuniverse/envs/roller_env.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:58:23.402651 pyrfuniverse-0.8.5/pyrfuniverse/envs/tobor_robotics/
--rw-rw-rw-   0        0        0      121 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.5/pyrfuniverse/envs/tobor_robotics/__init__.py
--rw-rw-rw-   0        0        0    10897 2022-07-08 02:22:23.000000 pyrfuniverse-0.8.5/pyrfuniverse/envs/tobor_robotics/tobor_push_pull_env.py
--rw-rw-rw-   0        0        0     9736 2023-02-15 08:33:33.000000 pyrfuniverse-0.8.5/pyrfuniverse/envs/tobor_robotiq85_manipulation_env.py
--rw-rw-rw-   0        0        0     8205 2022-11-02 03:34:57.000000 pyrfuniverse-0.8.5/pyrfuniverse/envs/ur5_box_env.py
--rw-rw-rw-   0        0        0     8549 2022-11-02 03:34:57.000000 pyrfuniverse-0.8.5/pyrfuniverse/envs/ur5_drawer_env.py
--rw-rw-rw-   0        0        0     1707 2023-05-28 07:57:51.000000 pyrfuniverse-0.8.5/pyrfuniverse/exception.py
--rw-rw-rw-   0        0        0     1929 2023-05-28 07:57:51.000000 pyrfuniverse-0.8.5/pyrfuniverse/logging_util.py
--rw-rw-rw-   0        0        0     4035 2023-05-28 07:57:51.000000 pyrfuniverse-0.8.5/pyrfuniverse/mock_communicator.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:58:23.423600 pyrfuniverse-0.8.5/pyrfuniverse/registry/
--rw-rw-rw-   0        0        0      114 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.5/pyrfuniverse/registry/__init__.py
--rw-rw-rw-   0        0        0     1855 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.5/pyrfuniverse/registry/base_registry_entry.py
--rw-rw-rw-   0        0        0     8085 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.5/pyrfuniverse/registry/binary_utils.py
--rw-rw-rw-   0        0        0     3256 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.5/pyrfuniverse/registry/remote_registry_entry.py
--rw-rw-rw-   0        0        0     5017 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.5/pyrfuniverse/registry/unity_env_registry.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:58:23.450186 pyrfuniverse-0.8.5/pyrfuniverse/rfuniverse_channel/
--rw-rw-rw-   0        0        0      496 2023-05-28 07:57:51.000000 pyrfuniverse-0.8.5/pyrfuniverse/rfuniverse_channel/__init__.py
--rw-rw-rw-   0        0        0    10422 2023-05-28 07:57:51.000000 pyrfuniverse-0.8.5/pyrfuniverse/rfuniverse_channel/asset_channel.py
--rw-rw-rw-   0        0        0     1317 2023-05-28 07:57:51.000000 pyrfuniverse-0.8.5/pyrfuniverse/rfuniverse_channel/asset_channel_ext.py
--rw-rw-rw-   0        0        0     1738 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.5/pyrfuniverse/rfuniverse_channel/debug_channel.py
--rw-rw-rw-   0        0        0     2244 2023-05-28 07:57:51.000000 pyrfuniverse-0.8.5/pyrfuniverse/rfuniverse_channel/instance_channel.py
--rw-rw-rw-   0        0        0     2198 2022-08-25 10:50:54.000000 pyrfuniverse-0.8.5/pyrfuniverse/rfuniverse_channel/rfuniverse_channel.py
--rw-rw-rw-   0        0        0     6579 2023-05-28 07:57:51.000000 pyrfuniverse-0.8.5/pyrfuniverse/rpc_communicator.py
--rw-rw-rw-   0        0        0    16840 2023-05-28 07:57:51.000000 pyrfuniverse-0.8.5/pyrfuniverse/rpc_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:58:23.490722 pyrfuniverse-0.8.5/pyrfuniverse/side_channel/
--rw-rw-rw-   0        0        0      234 2023-05-28 07:57:51.000000 pyrfuniverse-0.8.5/pyrfuniverse/side_channel/__init__.py
--rw-rw-rw-   0        0        0     4935 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.5/pyrfuniverse/side_channel/engine_configuration_channel.py
--rw-rw-rw-   0        0        0     3872 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.5/pyrfuniverse/side_channel/environment_parameters_channel.py
--rw-rw-rw-   0        0        0     2226 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.5/pyrfuniverse/side_channel/float_properties_channel.py
--rw-rw-rw-   0        0        0     3459 2023-05-28 07:57:51.000000 pyrfuniverse-0.8.5/pyrfuniverse/side_channel/incoming_message.py
--rw-rw-rw-   0        0        0     2026 2023-05-28 07:57:51.000000 pyrfuniverse-0.8.5/pyrfuniverse/side_channel/outgoing_message.py
--rw-rw-rw-   0        0        0     1300 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.5/pyrfuniverse/side_channel/raw_bytes_channel.py
--rw-rw-rw-   0        0        0     1502 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.5/pyrfuniverse/side_channel/side_channel.py
--rw-rw-rw-   0        0        0     3745 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.5/pyrfuniverse/side_channel/side_channel_manager.py
--rw-rw-rw-   0        0        0     1875 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.5/pyrfuniverse/side_channel/stats_side_channel.py
--rw-rw-rw-   0        0        0    12046 2023-05-28 07:57:51.000000 pyrfuniverse-0.8.5/pyrfuniverse/timers.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:58:23.542274 pyrfuniverse-0.8.5/pyrfuniverse/utils/
--rw-rw-rw-   0        0        0      181 2022-10-31 06:20:22.000000 pyrfuniverse-0.8.5/pyrfuniverse/utils/__init__.py
--rw-rw-rw-   0        0        0    13620 2023-02-10 17:44:39.000000 pyrfuniverse-0.8.5/pyrfuniverse/utils/active_depth_generate.py
--rw-rw-rw-   0        0        0     6006 2022-07-13 10:31:45.000000 pyrfuniverse-0.8.5/pyrfuniverse/utils/controller.py
--rw-rw-rw-   0        0        0    11646 2023-05-28 07:57:51.000000 pyrfuniverse-0.8.5/pyrfuniverse/utils/depth_processor.py
--rw-rw-rw-   0        0        0     3218 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.5/pyrfuniverse/utils/interpolate_utils.py
--rw-rw-rw-   0        0        0     4304 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.5/pyrfuniverse/utils/jaco_controller.py
--rw-rw-rw-   0        0        0     4908 2022-10-27 03:27:48.000000 pyrfuniverse-0.8.5/pyrfuniverse/utils/kinova_controller.py
--rw-rw-rw-   0        0        0      755 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.5/pyrfuniverse/utils/os_utils.py
--rw-rw-rw-   0        0        0     3569 2023-05-28 07:57:51.000000 pyrfuniverse-0.8.5/pyrfuniverse/utils/rfuniverse_utility.py
--rw-rw-rw-   0        0        0     5690 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.5/pyrfuniverse/utils/stretch_controller.py
--rw-rw-rw-   0        0        0     6776 2022-08-15 11:02:54.000000 pyrfuniverse-0.8.5/pyrfuniverse/utils/tobor_controller.py
--rw-rw-rw-   0        0        0     4783 2022-06-27 07:07:03.000000 pyrfuniverse-0.8.5/pyrfuniverse/utils/ur5_controller.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:58:22.996141 pyrfuniverse-0.8.5/pyrfuniverse.egg-info/
--rw-rw-rw-   0        0        0      263 2023-06-14 03:58:22.000000 pyrfuniverse-0.8.5/pyrfuniverse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6375 2023-06-14 03:58:22.000000 pyrfuniverse-0.8.5/pyrfuniverse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 03:58:22.000000 pyrfuniverse-0.8.5/pyrfuniverse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 11:32:20.000000 pyrfuniverse-0.8.5/pyrfuniverse.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      120 2023-06-14 03:58:22.000000 pyrfuniverse-0.8.5/pyrfuniverse.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-14 03:58:22.000000 pyrfuniverse-0.8.5/pyrfuniverse.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 03:58:23.639599 pyrfuniverse-0.8.5/setup.cfg
--rw-rw-rw-   0        0        0      755 2023-05-28 18:32:56.000000 pyrfuniverse-0.8.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 03:58:23.638595 pyrfuniverse-0.8.5/test/
--rw-rw-rw-   0        0        0     5651 2023-05-28 07:57:50.000000 pyrfuniverse-0.8.5/test/test_active_depth.py
--rw-rw-rw-   0        0        0      995 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.5/test/test_articulation_ik.py
--rw-rw-rw-   0        0        0      766 2023-05-28 07:57:50.000000 pyrfuniverse-0.8.5/test/test_camera_image.py
--rw-rw-rw-   0        0        0     1143 2023-05-28 07:57:50.000000 pyrfuniverse-0.8.5/test/test_custom_message.py
--rw-rw-rw-   0        0        0     1038 2023-04-06 04:49:14.000000 pyrfuniverse-0.8.5/test/test_debug.py
--rw-rw-rw-   0        0        0      439 2023-04-07 05:04:11.000000 pyrfuniverse-0.8.5/test/test_digit.py
--rw-rw-rw-   0        0        0      827 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.5/test/test_grasp_pose.py
--rw-rw-rw-   0        0        0     2758 2023-05-28 07:57:50.000000 pyrfuniverse-0.8.5/test/test_grasp_sim.py
--rw-rw-rw-   0        0        0      989 2023-04-10 09:39:27.000000 pyrfuniverse-0.8.5/test/test_heat_map.py
--rw-rw-rw-   0        0        0     1426 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.5/test/test_humanbody_ik.py
--rw-rw-rw-   0        0        0     1996 2023-05-28 07:57:50.000000 pyrfuniverse-0.8.5/test/test_label.py
--rw-rw-rw-   0        0        0      702 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.5/test/test_light.py
--rw-rw-rw-   0        0        0      589 2023-06-13 10:33:21.000000 pyrfuniverse-0.8.5/test/test_load_mesh.py
--rw-rw-rw-   0        0        0     1010 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.5/test/test_load_urdf.py
--rw-rw-rw-   0        0        0     1137 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.5/test/test_object_data.py
--rw-rw-rw-   0        0        0     1529 2023-06-13 10:34:48.000000 pyrfuniverse-0.8.5/test/test_ompl.py
--rw-rw-rw-   0        0        0     2149 2023-03-15 04:00:24.000000 pyrfuniverse-0.8.5/test/test_pick_and_place.py
--rw-rw-rw-   0        0        0     2174 2023-03-15 04:05:23.000000 pyrfuniverse-0.8.5/test/test_pick_and_place_flexiv.py
--rw-rw-rw-   0        0        0     1746 2023-05-28 07:57:50.000000 pyrfuniverse-0.8.5/test/test_point_cloud.py
--rw-rw-rw-   0        0        0      441 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.5/test/test_point_cloud_render.py
--rw-rw-rw-   0        0        0     1938 2023-05-28 07:57:50.000000 pyrfuniverse-0.8.5/test/test_point_cloud_with_intrinsic_matrix.py
--rw-rw-rw-   0        0        0      659 2023-04-13 02:37:33.000000 pyrfuniverse-0.8.5/test/test_save_gripper.py
--rw-rw-rw-   0        0        0      380 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.5/test/test_save_obj.py
--rw-rw-rw-   0        0        0     1024 2023-04-06 04:45:20.000000 pyrfuniverse-0.8.5/test/test_scene.py
--rw-rw-rw-   0        0        0      740 2023-04-07 07:58:17.000000 pyrfuniverse-0.8.5/test/test_tobor_move.py
+drwxrwxrwx   0        0        0        0 2023-07-03 04:47:49.577521 pyrfuniverse-0.9.10/
+-rw-rw-rw-   0        0        0    11357 2022-08-10 05:19:33.000000 pyrfuniverse-0.9.10/LICENSE
+-rw-rw-rw-   0        0        0      266 2023-07-03 04:47:49.577521 pyrfuniverse-0.9.10/PKG-INFO
+-rw-rw-rw-   0        0        0     2758 2023-06-21 09:17:40.000000 pyrfuniverse-0.9.10/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 04:47:49.499034 pyrfuniverse-0.9.10/pyrfuniverse/
+-rw-rw-rw-   0        0        0      759 2023-07-03 04:47:38.000000 pyrfuniverse-0.9.10/pyrfuniverse/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 04:47:49.526229 pyrfuniverse-0.9.10/pyrfuniverse/attributes/
+-rw-rw-rw-   0        0        0     1472 2023-06-21 09:17:41.000000 pyrfuniverse-0.9.10/pyrfuniverse/attributes/__init__.py
+-rw-rw-rw-   0        0        0     4555 2023-06-27 09:24:35.000000 pyrfuniverse-0.9.10/pyrfuniverse/attributes/activelightsensor_attr.py
+-rw-rw-rw-   0        0        0     8532 2023-06-26 07:46:59.000000 pyrfuniverse-0.9.10/pyrfuniverse/attributes/base_attr.py
+-rw-rw-rw-   0        0        0     8438 2023-06-27 09:30:40.000000 pyrfuniverse-0.9.10/pyrfuniverse/attributes/camera_attr.py
+-rw-rw-rw-   0        0        0      384 2023-06-26 03:15:33.000000 pyrfuniverse-0.9.10/pyrfuniverse/attributes/cloth_attr.py
+-rw-rw-rw-   0        0        0      601 2023-06-26 02:35:41.000000 pyrfuniverse-0.9.10/pyrfuniverse/attributes/collider_attr.py
+-rw-rw-rw-   0        0        0    15137 2023-07-03 03:38:52.000000 pyrfuniverse-0.9.10/pyrfuniverse/attributes/controller_attr.py
+-rw-rw-rw-   0        0        0      622 2023-06-26 02:41:17.000000 pyrfuniverse-0.9.10/pyrfuniverse/attributes/custom_attr.py
+-rw-rw-rw-   0        0        0      678 2023-06-26 03:18:21.000000 pyrfuniverse-0.9.10/pyrfuniverse/attributes/digit_attr.py
+-rw-rw-rw-   0        0        0      871 2023-06-26 02:43:24.000000 pyrfuniverse-0.9.10/pyrfuniverse/attributes/fallingcloth_attr.py
+-rw-rw-rw-   0        0        0     1533 2023-06-26 07:30:57.000000 pyrfuniverse-0.9.10/pyrfuniverse/attributes/gameobject_attr.py
+-rw-rw-rw-   0        0        0     4038 2023-06-26 06:02:42.000000 pyrfuniverse-0.9.10/pyrfuniverse/attributes/graspsim_attr.py
+-rw-rw-rw-   0        0        0     4520 2023-06-26 07:34:41.000000 pyrfuniverse-0.9.10/pyrfuniverse/attributes/humanbody_attr.py
+-rw-rw-rw-   0        0        0     2643 2023-06-26 07:41:38.000000 pyrfuniverse-0.9.10/pyrfuniverse/attributes/light_attr.py
+-rw-rw-rw-   0        0        0     8924 2023-06-27 09:47:18.000000 pyrfuniverse-0.9.10/pyrfuniverse/attributes/omplmanager_attr.py
+-rw-rw-rw-   0        0        0     1331 2023-06-27 08:46:11.000000 pyrfuniverse-0.9.10/pyrfuniverse/attributes/pointcloud_attr.py
+-rw-rw-rw-   0        0        0     1737 2023-06-26 03:12:07.000000 pyrfuniverse-0.9.10/pyrfuniverse/attributes/rigidbody_attr.py
+-rw-rw-rw-   0        0        0      387 2023-06-26 03:12:19.000000 pyrfuniverse-0.9.10/pyrfuniverse/attributes/softbody_attr.py
+drwxrwxrwx   0        0        0        0 2023-07-03 04:47:49.534245 pyrfuniverse-0.9.10/pyrfuniverse/envs/
+-rw-rw-rw-   0        0        0    14525 2023-06-26 03:42:24.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/__init__.py
+-rw-rw-rw-   0        0        0     4178 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/balance_ball_env.py
+-rw-rw-rw-   0        0        0    24046 2023-07-03 03:53:17.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/base_env.py
+-rw-rw-rw-   0        0        0     4564 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/bouncer_env.py
+-rw-rw-rw-   0        0        0     3982 2023-02-10 17:44:39.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/franka_grasp_env.py
+-rw-rw-rw-   0        0        0     3077 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/franka_push_env.py
+drwxrwxrwx   0        0        0        0 2023-07-03 04:47:49.539932 pyrfuniverse-0.9.10/pyrfuniverse/envs/gripper_nail/
+-rw-rw-rw-   0        0        0      736 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/gripper_nail/__init__.py
+-rw-rw-rw-   0        0        0     4209 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/gripper_nail/nail_can_env.py
+-rw-rw-rw-   0        0        0     5750 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/gripper_nail/nail_card_env.py
+-rw-rw-rw-   0        0        0     3917 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/gripper_nail/robotiq85_insert_env.py
+-rw-rw-rw-   0        0        0     4149 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/gripper_nail/robotiq85_nail_book_env.py
+-rw-rw-rw-   0        0        0     4220 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/gripper_nail/robotiq85_nail_can_env.py
+-rw-rw-rw-   0        0        0     5917 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/gripper_nail/robotiq85_nail_card_env.py
+-rw-rw-rw-   0        0        0     5696 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/gripper_nail/robotiq85_nail_coin_env.py
+-rw-rw-rw-   0        0        0      769 2023-06-26 03:45:35.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/gym_goal_wrapper_env.py
+-rw-rw-rw-   0        0        0      702 2023-06-26 03:45:35.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/gym_wrapper_env.py
+drwxrwxrwx   0        0        0        0 2023-07-03 04:47:49.542004 pyrfuniverse-0.9.10/pyrfuniverse/envs/multi_agent/
+-rw-rw-rw-   0        0        0      172 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/multi_agent/__init__.py
+-rw-rw-rw-   0        0        0     9111 2023-02-10 17:44:39.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/multi_agent/cleaner_env.py
+-rw-rw-rw-   0        0        0    11818 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/multi_agent/navigation_env.py
+-rw-rw-rw-   0        0        0     6000 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/multi_agent_navigation_env.py
+drwxrwxrwx   0        0        0        0 2023-07-03 04:47:49.544004 pyrfuniverse-0.9.10/pyrfuniverse/envs/multi_physics/
+-rw-rw-rw-   0        0        0      871 2023-06-21 09:17:41.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/multi_physics/__init__.py
+-rw-rw-rw-   0        0        0    13868 2023-07-03 04:41:20.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/multi_physics/flexiv_cutting.py
+-rw-rw-rw-   0        0        0     8156 2023-06-28 05:32:14.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/multi_physics/kinova_gen2_catching_cloth_env.py
+-rw-rw-rw-   0        0        0    10075 2023-06-29 05:13:30.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/multi_physics/ur5_water_shooting.py
+-rw-rw-rw-   0        0        0      513 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/rfuniverse_robot_hub_env.py
+drwxrwxrwx   0        0        0        0 2023-07-03 04:47:49.549513 pyrfuniverse-0.9.10/pyrfuniverse/envs/robotics/
+-rw-rw-rw-   0        0        0      675 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/robotics/__init__.py
+-rw-rw-rw-   0        0        0     7276 2023-06-29 05:13:30.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/robotics/franka_cloth_env.py
+-rw-rw-rw-   0        0        0     7476 2023-06-29 05:13:30.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/robotics/franka_cloth_fold_env.py
+-rw-rw-rw-   0        0        0     9654 2023-06-29 05:13:30.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/robotics/franka_robotics_env.py
+-rw-rw-rw-   0        0        0     8014 2023-06-29 05:13:30.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/robotics/franka_softbody_env.py
+-rw-rw-rw-   0        0        0      817 2022-12-15 05:37:19.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/robotics/pick_and_place_env.py
+-rw-rw-rw-   0        0        0      754 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/robotics/push_env.py
+-rw-rw-rw-   0        0        0      864 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/robotics/reach_env.py
+-rw-rw-rw-   0        0        0     4463 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/roller_env.py
+drwxrwxrwx   0        0        0        0 2023-07-03 04:47:49.550512 pyrfuniverse-0.9.10/pyrfuniverse/envs/tobor_robotics/
+-rw-rw-rw-   0        0        0      121 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/tobor_robotics/__init__.py
+-rw-rw-rw-   0        0        0    10897 2022-07-08 02:22:23.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/tobor_robotics/tobor_push_pull_env.py
+-rw-rw-rw-   0        0        0     8629 2023-06-27 11:22:59.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/tobor_robotiq85_manipulation_env.py
+-rw-rw-rw-   0        0        0     8205 2022-11-02 03:34:57.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/ur5_box_env.py
+-rw-rw-rw-   0        0        0     8549 2022-11-02 03:34:57.000000 pyrfuniverse-0.9.10/pyrfuniverse/envs/ur5_drawer_env.py
+drwxrwxrwx   0        0        0        0 2023-07-03 04:47:49.552021 pyrfuniverse-0.9.10/pyrfuniverse/side_channel/
+-rw-rw-rw-   0        0        0      144 2023-06-26 02:33:27.000000 pyrfuniverse-0.9.10/pyrfuniverse/side_channel/__init__.py
+-rw-rw-rw-   0        0        0     3244 2023-06-26 02:33:27.000000 pyrfuniverse-0.9.10/pyrfuniverse/side_channel/incoming_message.py
+-rw-rw-rw-   0        0        0     1536 2023-06-26 02:33:27.000000 pyrfuniverse-0.9.10/pyrfuniverse/side_channel/outgoing_message.py
+drwxrwxrwx   0        0        0        0 2023-07-03 04:47:49.560049 pyrfuniverse-0.9.10/pyrfuniverse/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-03 03:57:44.000000 pyrfuniverse-0.9.10/pyrfuniverse/utils/__init__.py
+-rw-rw-rw-   0        0        0    13620 2023-02-10 17:44:39.000000 pyrfuniverse-0.9.10/pyrfuniverse/utils/active_depth_generate.py
+-rw-rw-rw-   0        0        0     6006 2022-07-13 10:31:45.000000 pyrfuniverse-0.9.10/pyrfuniverse/utils/controller.py
+-rw-rw-rw-   0        0        0    11746 2023-06-27 09:15:30.000000 pyrfuniverse-0.9.10/pyrfuniverse/utils/depth_processor.py
+-rw-rw-rw-   0        0        0     3227 2023-06-28 05:30:44.000000 pyrfuniverse-0.9.10/pyrfuniverse/utils/interpolate_utils.py
+-rw-rw-rw-   0        0        0     4304 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.10/pyrfuniverse/utils/jaco_controller.py
+-rw-rw-rw-   0        0        0     4908 2022-10-27 03:27:48.000000 pyrfuniverse-0.9.10/pyrfuniverse/utils/kinova_controller.py
+-rw-rw-rw-   0        0        0      755 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.10/pyrfuniverse/utils/os_utils.py
+-rw-rw-rw-   0        0        0     9072 2023-07-02 13:36:55.000000 pyrfuniverse-0.9.10/pyrfuniverse/utils/rfuniverse_communicator.py
+-rw-rw-rw-   0        0        0     3569 2023-06-21 09:17:41.000000 pyrfuniverse-0.9.10/pyrfuniverse/utils/rfuniverse_utility.py
+-rw-rw-rw-   0        0        0     5690 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.10/pyrfuniverse/utils/stretch_controller.py
+-rw-rw-rw-   0        0        0     6776 2022-08-15 11:02:54.000000 pyrfuniverse-0.9.10/pyrfuniverse/utils/tobor_controller.py
+-rw-rw-rw-   0        0        0     4783 2022-06-27 07:07:03.000000 pyrfuniverse-0.9.10/pyrfuniverse/utils/ur5_controller.py
+drwxrwxrwx   0        0        0        0 2023-07-03 04:47:49.513716 pyrfuniverse-0.9.10/pyrfuniverse.egg-info/
+-rw-rw-rw-   0        0        0      266 2023-07-03 04:47:49.000000 pyrfuniverse-0.9.10/pyrfuniverse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4088 2023-07-03 04:47:49.000000 pyrfuniverse-0.9.10/pyrfuniverse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 04:47:49.000000 pyrfuniverse-0.9.10/pyrfuniverse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 11:32:20.000000 pyrfuniverse-0.9.10/pyrfuniverse.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       36 2023-07-03 04:47:49.000000 pyrfuniverse-0.9.10/pyrfuniverse.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-03 04:47:49.000000 pyrfuniverse-0.9.10/pyrfuniverse.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 04:47:49.577521 pyrfuniverse-0.9.10/setup.cfg
+-rw-rw-rw-   0        0        0      601 2023-07-03 03:43:45.000000 pyrfuniverse-0.9.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 04:47:49.576521 pyrfuniverse-0.9.10/test/
+-rw-rw-rw-   0        0        0     5924 2023-06-28 08:06:36.000000 pyrfuniverse-0.9.10/test/test_active_depth.py
+-rw-rw-rw-   0        0        0      995 2023-04-06 04:45:20.000000 pyrfuniverse-0.9.10/test/test_articulation_ik.py
+-rw-rw-rw-   0        0        0      943 2023-06-30 10:11:12.000000 pyrfuniverse-0.9.10/test/test_camera_image.py
+-rw-rw-rw-   0        0        0     1939 2023-06-29 07:29:03.000000 pyrfuniverse-0.9.10/test/test_custom_message.py
+-rw-rw-rw-   0        0        0     1038 2023-04-06 04:49:14.000000 pyrfuniverse-0.9.10/test/test_debug.py
+-rw-rw-rw-   0        0        0      439 2023-04-07 05:04:11.000000 pyrfuniverse-0.9.10/test/test_digit.py
+-rw-rw-rw-   0        0        0      827 2023-04-06 04:45:20.000000 pyrfuniverse-0.9.10/test/test_grasp_pose.py
+-rw-rw-rw-   0        0        0     2750 2023-06-28 08:06:36.000000 pyrfuniverse-0.9.10/test/test_grasp_sim.py
+-rw-rw-rw-   0        0        0      989 2023-04-10 09:39:27.000000 pyrfuniverse-0.9.10/test/test_heat_map.py
+-rw-rw-rw-   0        0        0     1426 2023-04-06 04:45:20.000000 pyrfuniverse-0.9.10/test/test_humanbody_ik.py
+-rw-rw-rw-   0        0        0     1087 2023-06-28 08:06:36.000000 pyrfuniverse-0.9.10/test/test_image_stream.py
+-rw-rw-rw-   0        0        0     1984 2023-06-26 02:33:27.000000 pyrfuniverse-0.9.10/test/test_label.py
+-rw-rw-rw-   0        0        0      702 2023-04-06 04:45:20.000000 pyrfuniverse-0.9.10/test/test_light.py
+-rw-rw-rw-   0        0        0      589 2023-06-13 10:33:21.000000 pyrfuniverse-0.9.10/test/test_load_mesh.py
+-rw-rw-rw-   0        0        0     1008 2023-06-27 08:00:59.000000 pyrfuniverse-0.9.10/test/test_load_urdf.py
+-rw-rw-rw-   0        0        0      277 2023-06-26 07:47:27.000000 pyrfuniverse-0.9.10/test/test_load_urdf_akb.py
+-rw-rw-rw-   0        0        0     1980 2023-06-27 08:13:05.000000 pyrfuniverse-0.9.10/test/test_object_data.py
+-rw-rw-rw-   0        0        0     1646 2023-06-28 08:01:52.000000 pyrfuniverse-0.9.10/test/test_ompl.py
+-rw-rw-rw-   0        0        0     2149 2023-03-15 04:00:24.000000 pyrfuniverse-0.9.10/test/test_pick_and_place.py
+-rw-rw-rw-   0        0        0     2174 2023-03-15 04:05:23.000000 pyrfuniverse-0.9.10/test/test_pick_and_place_flexiv.py
+-rw-rw-rw-   0        0        0     1658 2023-06-28 08:06:36.000000 pyrfuniverse-0.9.10/test/test_point_cloud.py
+-rw-rw-rw-   0        0        0      441 2023-04-06 04:45:20.000000 pyrfuniverse-0.9.10/test/test_point_cloud_render.py
+-rw-rw-rw-   0        0        0     1830 2023-06-28 08:06:36.000000 pyrfuniverse-0.9.10/test/test_point_cloud_with_intrinsic_matrix.py
+-rw-rw-rw-   0        0        0      659 2023-04-13 02:37:33.000000 pyrfuniverse-0.9.10/test/test_save_gripper.py
+-rw-rw-rw-   0        0        0      378 2023-06-28 08:06:36.000000 pyrfuniverse-0.9.10/test/test_save_obj.py
+-rw-rw-rw-   0        0        0     1024 2023-04-06 04:45:20.000000 pyrfuniverse-0.9.10/test/test_scene.py
+-rw-rw-rw-   0        0        0      740 2023-04-07 07:58:17.000000 pyrfuniverse-0.9.10/test/test_tobor_move.py
```

### Comparing `pyrfuniverse-0.8.5/LICENSE` & `pyrfuniverse-0.9.10/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.5/README.md` & `pyrfuniverse-0.9.10/README.md`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/__init__.py` & `pyrfuniverse-0.9.10/pyrfuniverse/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Version of the library that will be used to upload to pypi
-__version__ = "0.8.5"
+__version__ = "0.9.10"
 
 import os.path
 import json
 
 def read_config():
     if not os.path.exists(config_path):
         config = {}
```

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/attributes/__init__.py` & `pyrfuniverse-0.9.10/pyrfuniverse/attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/attributes/activelightsensor_attr.py` & `pyrfuniverse-0.9.10/pyrfuniverse/attributes/activelightsensor_attr.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,36 @@
 import base64
 import cv2
 import numpy as np
 import pyrfuniverse.attributes as attr
 import pyrfuniverse.utils.active_depth_generate as active_depth
-from pyrfuniverse.side_channel.side_channel import (
-    IncomingMessage,
-    OutgoingMessage,
-)
 
 
 class ActiveLightSensorAttr(attr.CameraAttr):
     """
     Class of IR-based depth sensor, which can simulate the noise of 
     real-world depth camera and produce depth image in similar pattern.
     """
     def __init__(self, env, id: int, data=None):
         super().__init__(env, id, data)
-        self.main_intrinsic_matrix = np.eye(4)
-        self.ir_intrinsic_matrix = np.eye(4)
+        self.main_intrinsic_matrix = np.eye(3)
+        self.ir_intrinsic_matrix = np.eye(3)
 
-    def parse_message(self, msg: IncomingMessage) -> dict:
+    def parse_message(self, data: dict):
         """
         Parse messages. This function is called by internal function.
 
         Returns:
             Dict: A dict containing useful information of this class.\n
             self.data['active_depth']: IR-based depth, shape = (w,h)
         """
-        super().parse_message(msg)
-        if msg.read_bool() is True:
-            self.data['ir_left'] = base64.b64decode(msg.read_string())
-            self.data['ir_right'] = base64.b64decode(msg.read_string())
+        super().parse_message(data)
+        if 'ir_left' in self.data and 'ir_right' in self.data:
+            self.data['ir_left'] = base64.b64decode(self.data['ir_left'])
+            self.data['ir_right'] = base64.b64decode(self.data['ir_right'])
 
             image_left = np.frombuffer(self.data['ir_left'], dtype=np.uint8)
             image_left = cv2.imdecode(image_left, cv2.IMREAD_COLOR)[..., 2]
             image_right = np.frombuffer(self.data['ir_right'], dtype=np.uint8)
             image_right = cv2.imdecode(image_right, cv2.IMREAD_COLOR)[..., 2]
             left_extrinsic_matrix = np.array(
                 [[0., -1., 0., -0.0175], [0., 0., -1., 0.], [1., 0., 0., 0.], [0., 0., 0., 1.]])
@@ -57,26 +53,19 @@
                                                                                         ndisp=128,
                                                                                         use_census=True,
                                                                                         register_depth=True,
                                                                                         census_wsize=7,
                                                                                         use_noise=False)
             self.data['active_depth'][self.data['active_depth'] > 8.] = 0
             self.data['active_depth'][self.data['active_depth'] < 0.1] = 0
-        return self.data
 
-    def GetActiveDepth(self, main_intrinsic_matrix_local: list, ir_intrinsic_matrix_local: list):
+    def GetActiveDepth(self, main_intrinsic_matrix_local: np.ndarray, ir_intrinsic_matrix_local: np.ndarray):
         """
         Get IR-based depth image.
 
         Args:
-            main_intrinsic_matrix_local: List[float] The intrinsic matrix of main camera.
-            ir_intrinsic_matrix_local: List[float] The intrinsic matrix of IR-based camera.
+            main_intrinsic_matrix_local: np.ndarray The intrinsic matrix of main camera.
+            ir_intrinsic_matrix_local: np.ndarray The intrinsic matrix of IR-based camera.
         """
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('GetActiveDepth')
-        self.main_intrinsic_matrix = np.reshape(main_intrinsic_matrix_local, [3, 3]).T
-        self.ir_intrinsic_matrix = np.reshape(ir_intrinsic_matrix_local, [3, 3]).T
-        msg.write_float32_list(self.ir_intrinsic_matrix.T.reshape([-1]).tolist())
-
-        self.env.instance_channel.send_message(msg)
+        self.main_intrinsic_matrix = main_intrinsic_matrix_local
+        self.ir_intrinsic_matrix = ir_intrinsic_matrix_local
+        self._send_data('GetActiveDepth', self.ir_intrinsic_matrix)
```

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/attributes/cloth_attr.py` & `pyrfuniverse-0.9.10/pyrfuniverse/attributes/collider_attr.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import pyrfuniverse.attributes as attr
-from pyrfuniverse.side_channel.side_channel import (
-    IncomingMessage,
-    OutgoingMessage,
-)
 
 
-class ClothAttr(attr.BaseAttr):
+class ColliderAttr(attr.GameObjectAttr):
     """
-    Obi cloth class.
+    Collider class for objects who have collider in Unity.
     """
-    def parse_message(self, msg: IncomingMessage) -> dict:
+    def parse_message(self, data: dict):
         """
         Parse messages. This function is called by internal function.
 
         Returns:
             Dict: A dict containing useful information of this class.
+        """
+        super().parse_message(data)
 
+    def GenerateVHACDColider(self):
+        """
+        Generate convex colliders using VHACD algorithm.
         """
-        super().parse_message(msg)
-        return self.data
+        self._send_data('GenerateVHACDColider')
```

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/attributes/light_attr.py` & `pyrfuniverse-0.9.10/pyrfuniverse/attributes/light_attr.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,20 @@
 from enum import Enum
-
 import pyrfuniverse.attributes as attr
-from pyrfuniverse.side_channel.side_channel import (
-    IncomingMessage,
-    OutgoingMessage,
-)
 
 
 class LightType(Enum):
     """
     The type of light, keeping same name with LightType (https://docs.unity3d.com/ScriptReference/LightType.html) in Unity.
     """
     Spot = 0
     Directional = 1
     Point = 2
-    Area = 3  # 不可用
-    Disc = 4  # 不可用
+    Area = 3  # unused
+    Disc = 4  # unused
 
 
 class LightShadow(Enum):
     """
     The type of shadow, keeping same name with LightShadows (https://docs.unity3d.com/ScriptReference/LightShadows.html) in Unity.
     """
     NoneShadow = 0
@@ -27,107 +22,72 @@
     Soft = 2
 
 
 class LightAttr(attr.BaseAttr):
     """
     Light attribute class.
     """
-    def parse_message(self, msg: IncomingMessage) -> dict:
+    def parse_message(self, data: dict):
         """
         Parse messages. This function is called by internal function.
 
         Returns:
             Dict: A dict containing useful information of this class.
         """
-        super().parse_message(msg)
-        return self.data
+        super().parse_message(data)
 
     def SetColor(self, color: list):
         """
         Set the color of light.
 
         Args:
             color: A list of length 3, representing the R, G and B channel, in range [0, 1].
         """
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('SetColor')
-        for i in range(3):
-            msg.write_float32(color[i])
+        assert color is not None and len(color) == 3, 'position length must be 3'
+        color = [float(i) for i in color]
 
-        self.env.instance_channel.send_message(msg)
+        self._send_data('SetColor', color)
 
     def SetType(self, light_type: LightType):
         """
         Set the type of light.
 
         Args:
             light_type: LightType, the type of light.
         """
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('SetType')
-        msg.write_int32(light_type.value)
-
-        self.env.instance_channel.send_message(msg)
+        self._send_data('SetType', light_type.value)
 
     def SetShadow(self, light_shadow: LightShadow):
         """
         Set the type of shadow.
 
         Args:
             light_shadow: LightShadow, the type of the shadow.
         """
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('SetShadow')
-        msg.write_float32(light_shadow.value)
-
-        self.env.instance_channel.send_message(msg)
+        self._send_data('SetShadow', light_shadow.value)
 
     def SetIntensity(self, light_intensity: float):
         """
         Set the intensity of light.
 
         Args:
             light_intensity: Float, the intensity of light.
         """
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('SetIntensity')
-        msg.write_float32(light_intensity)
-
-        self.env.instance_channel.send_message(msg)
+        self._send_data('SetIntensity', float(light_intensity))
 
     def SetRange(self, light_range: float):
         """
         Set the range of light. (Only available when the LightType is `LightType.Spot` or `LightType.Point`)
 
         Args:
             light_range: Float, the range of light.
         """
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('SetRange')
-        msg.write_float32(light_range)
-
-        self.env.instance_channel.send_message(msg)
+        self._send_data('SetRange', float(light_range))
 
     def SetSpotAngle(self, spot_angle: float):
         """
         Set the angle of light. (Only available when the LightType is `LightType.Spot`)
 
         Args:
             spot_angle: Float, the angle of light.
         """
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('SetSpotAngle')
-        msg.write_float32(spot_angle)
-
-        self.env.instance_channel.send_message(msg)
+        self._send_data('SetSpotAngle', float(spot_angle))
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/attributes/omplmanager_attr.py` & `pyrfuniverse-0.9.10/pyrfuniverse/attributes/omplmanager_attr.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,19 +6,14 @@
 '''
 
 INTERPOLATE_NUM = 300
 DEFAULT_PLANNING_TIME = 500.0
 
 from ompl import base as ob
 from ompl import geometric as og
-
-from pyrfuniverse.side_channel.side_channel import (
-    IncomingMessage,
-    OutgoingMessage,
-)
 import copy
 import pyrfuniverse.attributes as attr
 
 
 class OmplManagerAttr(attr.BaseAttr):
     """
     To use with rfu_OMPL. You need to construct a instance of this class and pass to PbOMPL.
@@ -33,32 +28,25 @@
         self.is_collision = False
         self.state = None
         self.robot_attr = None
         self.joint_num = 0
         self.joint_lower_limit = []
         self.joint_upper_limit = []
 
-    def parse_message(self, msg: IncomingMessage) -> dict:
-        super().parse_message(msg)
-        self.is_collision = msg.read_bool()
-        return self.data
+    def parse_message(self, data: dict):
+        super().parse_message(data)
+        self.is_collision = data['is_collide']
 
     def modify_robot(self, robot_id: int):
         self.robot_attr = self.env.GetAttr(robot_id)
         self.joint_num = self.robot_attr.data['number_of_moveable_joints']
         self.joint_lower_limit = self.robot_attr.data['joint_lower_limit']
         self.joint_upper_limit = self.robot_attr.data['joint_upper_limit']
 
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('ModifyRobot')
-        msg.write_int32(robot_id)
-
-        self.env.instance_channel.send_message(msg)
+        self._send_data('ModifyRobot', robot_id)
 
     def get_cur_state(self) -> list:
         """
         Get current robot state.
         """
         return copy.deepcopy(self.state)
 
@@ -77,23 +65,21 @@
         Reset robot state
         Args:
             state: list[Float], joint values of robot
         """
         self.state = [0.0] * self.joint_num
         self._set_joint_positions(self.state)
 
-    def _set_joint_positions(self, positions):
+    def _set_joint_positions(self, positions: list):
         self.is_collision = False
 
-        msg = OutgoingMessage()
-        msg.write_int32(self.id)
-        msg.write_string('SetJointState')
-        msg.write_float32_list(positions)
+        self._send_data('SetJointState', positions)
 
-        self.env.instance_channel.send_message(msg)
+    def RestoreRobot(self, robot_id: int):
+        self._send_data('RestoreRobot', robot_id)
 
 
 class RFUStateSpace(ob.RealVectorStateSpace):
     def __init__(self, num_dim) -> None:
         super().__init__(num_dim)
         self.num_dim = num_dim
         self.state_sampler = None
@@ -146,16 +132,15 @@
 
         self.set_planner("InformedRRTstar") # RRT by default
 
     def is_state_valid(self, state):
         # check if a given state will lead a collision
         self.manager.set_state(self.state_to_list(state))
         # self.env.SetNextStepNoTimeConsuming()
-        self.env.step()
-        self.env.step()
+        self.env.step(2)
         return not self.manager.is_collision
 
     def set_planner(self, planner_name):
         """
         Note: Add your planner here!!
         """
         if planner_name == "PRM":
```

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/attributes/pointcloud_attr.py` & `pyrfuniverse-0.9.10/pyrfuniverse/attributes/gameobject_attr.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,62 +1,58 @@
-import numpy as np
-
 import pyrfuniverse.attributes as attr
-from pyrfuniverse.side_channel.side_channel import (
-    IncomingMessage,
-    OutgoingMessage,
-)
 
 
-class PointCloudAttr(attr.BaseAttr):
+class GameObjectAttr(attr.BaseAttr):
     """
-    Point cloud rendering class.
+    Basic game object attribute class.
     """
-    def parse_message(self, msg: IncomingMessage) -> dict:
+    def parse_message(self, data: dict):
         """
         Parse messages. This function is called by internal function.
 
         Returns:
             Dict: A dict containing useful information of this class.
+
+            self.data['3d_bounding_box']: The 3d bounding box of objects.
         """
-        super().parse_message(msg)
-        return self.data
+        super().parse_message(data)
 
-    def ShowPointCloud(self, positions: list = [], colors: list = [], ply_path: str = None, radius: float = 0.01):
+    def SetColor(self, color: list):
         """
-        Display point cloud in Unity.
+        Set object color.
 
         Args:
-            positions: A list of positions of points in a point cloud.
-            colors: A list of colors of points (range [0, 1]) in a point cloud.
-            ply_path: Str, the absolute path of `.ply` file. If this parameter is specified, `positions`
-                and `colors` will be ignored.
-            radius: Float, the radius of the point cloud.
-        """
-        msg = OutgoingMessage()
-
-        msg.write_int32(self.id)
-        msg.write_string('ShowPointCloud')
-        msg.write_bool(ply_path is not None)
-        if ply_path is not None:
-            msg.write_string(ply_path)
-        else:
-            msg.write_float32_list(np.array(positions).reshape(-1).tolist())
-            msg.write_float32_list(np.array(colors).reshape(-1).tolist())
-        msg.write_float32(radius)
+            color: A list of length 4, represenging r, g, b and a. Each float is in range (0, 1).
+        """
+        if color is not None:
+            assert len(color) == 4, 'color length must be 4'
+            color = [float(i) for i in color]
+
+        self._send_data('SetColor', color)
+
+    def EnabledRender(self, enabled: bool):
+        """
+        Enable or disable rendering system.
 
-        self.env.instance_channel.send_message(msg)
+        Args:
+            enabled: Bool, Ture for enable rendering and False for disable rendering.
+        """
+        self._send_data('EnabledRender', enabled)
 
-    def SetRadius(self, radius: float):
+    def SetTexture(self, path: str):
         """
-        Set the radius for points in a point cloud.
+        Set the texture of object.
 
         Args:
-            radius: Float, the radius.
+            path: Str, the absolute path for texture file.
+        """
+        self._send_data('SetTexture', path)
+
+    def Get3DBBox(self):
+        """
+        Get the 3d bounding box of this object.
+        
         """
-        msg = OutgoingMessage()
+        self._send_data('Get3DBBox')
+
 
-        msg.write_int32(self.id)
-        msg.write_string('SetRadius')
-        msg.write_float32(radius)
 
-        self.env.instance_channel.send_message(msg)
```

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/attributes/softbody_attr.py` & `pyrfuniverse-0.9.10/pyrfuniverse/attributes/custom_attr.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import pyrfuniverse.attributes as attr
-from pyrfuniverse.side_channel.side_channel import (
-    IncomingMessage,
-    OutgoingMessage,
-)
 
-class SoftbodyAttr(attr.BaseAttr):
+
+class CustomAttr(attr.BaseAttr):
     """
-    Obi Softbody class
+    This is an example of custom attribute class, without actual functions.
     """
-    def parse_message(self, msg: IncomingMessage) -> dict:
+    def parse_message(self, data: dict):
         """
         Parse messages. This function is called by internal function.
 
         Returns:
             Dict: A dict containing useful information of this class.
+
+            data['custom_message']: A custom message
         """
-        super().parse_message(msg)
-        return self.data
+        super().parse_message(data)
+
+    # An example of new API
+    def CustomMessage(self, message: str):
+        self._send_data('CustomMessage', message)
```

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/base_env.py` & `pyrfuniverse-0.9.10/pyrfuniverse/envs/base_env.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,616 +1,700 @@
-"""
-Python Environment API for the ML-Agents Toolkit
-The aim of this API is to expose Agents evolving in a simulation
-to perform reinforcement learning on.
-This API supports multi-agent scenarios and groups similar Agents (same
-observations, actions spaces and behavior) together. These groups of Agents are
-identified by their BehaviorName.
-For performance reasons, the data of each group of agents is processed in a
-batched manner. Agents are identified by a unique AgentId identifier that
-allows tracking of Agents across simulation steps. Note that there is no
-guarantee that the number or order of the Agents in the state will be
-consistent across simulation steps.
-A simulation steps corresponds to moving the simulation forward until at least
-one agent in the simulation sends its observations to Python again. Since
-Agents can request decisions at different frequencies, a simulation step does
-not necessarily correspond to a fixed simulation time increment.
-"""
-
-from abc import ABC, abstractmethod
-from collections.abc import Mapping
-from typing import (
-    List,
-    NamedTuple,
-    Tuple,
-    Optional,
-    Dict,
-    Iterator,
-    Any,
-    Mapping as MappingType,
-)
-from enum import IntFlag, Enum
+import random
+import subprocess
+from abc import ABC
+import socket
 import numpy as np
+import pyrfuniverse
+import pyrfuniverse.attributes as attr
+from pyrfuniverse.side_channel import IncomingMessage, OutgoingMessage
+from pyrfuniverse.utils.rfuniverse_communicator import RFUniverseCommunicator
+import os
 
-from pyrfuniverse.exception import UnityActionException
 
-AgentId = int
-GroupId = int
-BehaviorName = str
-
-
-class DecisionStep(NamedTuple):
+class RFUniverseBaseEnv(ABC):
     """
-    Contains the data a single Agent collected since the last
-    simulation step.
-     - obs is a list of numpy arrays observations collected by the agent.
-     - reward is a float. Corresponds to the rewards collected by the agent
-     since the last simulation step.
-     - agent_id is an int and an unique identifier for the corresponding Agent.
-     - action_mask is an optional list of one dimensional array of booleans.
-     Only available when using multi-discrete actions.
-     Each array corresponds to an action branch. Each array contains a mask
-     for each action of the branch. If true, the action is not available for
-     the agent during this simulation step.
+    RFUniverse base environment class.
+
+    Args:
+        executable_file: Str, the absolute path of Unity executable file. None for last used executable file; "@editor" for using Unity Editor.
+        scene_file: Str, the absolute path of Unity scene JSON file. All JSON files locate at `StraemingAssets/SceneData` by default.
+        assets: List, the list of pre-load assets. All assets in the list will be pre-loaded in Unity when the environment is initialized, which will save time during instanciating.
+        graphics: Bool, True for showing GUI and False for headless mode.
     """
+    metadata = {'render.modes': ['human', 'rgb_array']}
 
-    obs: List[np.ndarray]
-    reward: float
-    agent_id: AgentId
-    action_mask: Optional[List[np.ndarray]]
-    group_id: int
-    group_reward: float
+    def __init__(
+        self,
+        executable_file: str = None,
+        scene_file: str = None,
+        assets: list = [],
+        graphics: bool = True,
+        port: int = 5004
+    ):
+        # time step
+        self.t = 0
+        self.executable_file = executable_file
+        self.scene_file = scene_file
+        self.pre_load_assets = assets
+        self.graphics = graphics
 
+        self.attrs = {}
+        self.data = {}
+        self.listen_messages = {}
+        self.listen_object = {}
+        self.port = port
 
-class DecisionSteps(Mapping):
-    """
-    Contains the data a batch of similar Agents collected since the last
-    simulation step. Note that all Agents do not necessarily have new
-    information to send at each simulation step. Therefore, the ordering of
-    agents and the batch size of the DecisionSteps are not fixed across
-    simulation steps.
-     - obs is a list of numpy arrays observations collected by the batch of
-     agent. Each obs has one extra dimension compared to DecisionStep: the
-     first dimension of the array corresponds to the batch size of the batch.
-     - reward is a float vector of length batch size. Corresponds to the
-     rewards collected by each agent since the last simulation step.
-     - agent_id is an int vector of length batch size containing unique
-     identifier for the corresponding Agent. This is used to track Agents
-     across simulation steps.
-     - action_mask is an optional list of two dimensional array of booleans.
-     Only available when using multi-discrete actions.
-     Each array corresponds to an action branch. The first dimension of each
-     array is the batch size and the second contains a mask for each action of
-     the branch. If true, the action is not available for the agent during
-     this simulation step.
-    """
+        if self.executable_file is None:
+            self.executable_file = pyrfuniverse.executable_file
 
-    def __init__(self, obs, reward, agent_id, action_mask, group_id, group_reward):
-        self.obs: List[np.ndarray] = obs
-        self.reward: np.ndarray = reward
-        self.agent_id: np.ndarray = agent_id
-        self.action_mask: Optional[List[np.ndarray]] = action_mask
-        self.group_id: np.ndarray = group_id
-        self.group_reward: np.ndarray = group_reward
-        self._agent_id_to_index: Optional[Dict[AgentId, int]] = None
-
-    @property
-    def agent_id_to_index(self) -> Dict[AgentId, int]:
-        """
-        :returns: A Dict that maps agent_id to the index of those agents in
-        this DecisionSteps.
-        """
-        if self._agent_id_to_index is None:
-            self._agent_id_to_index = {}
-            for a_idx, a_id in enumerate(self.agent_id):
-                self._agent_id_to_index[a_id] = a_idx
-        return self._agent_id_to_index
-
-    def __len__(self) -> int:
-        return len(self.agent_id)
-
-    def __getitem__(self, agent_id: AgentId) -> DecisionStep:
-        """
-        returns the DecisionStep for a specific agent.
-        :param agent_id: The id of the agent
-        :returns: The DecisionStep
-        """
-        if agent_id not in self.agent_id_to_index:
-            raise KeyError(f"agent_id {agent_id} is not present in the DecisionSteps")
-        agent_index = self._agent_id_to_index[agent_id]  # type: ignore
-        agent_obs = []
-        for batched_obs in self.obs:
-            agent_obs.append(batched_obs[agent_index])
-        agent_mask = None
-        if self.action_mask is not None:
-            agent_mask = []
-            for mask in self.action_mask:
-                agent_mask.append(mask[agent_index])
-        group_id = self.group_id[agent_index]
-        return DecisionStep(
-            obs=agent_obs,
-            reward=self.reward[agent_index],
-            agent_id=agent_id,
-            action_mask=agent_mask,
-            group_id=group_id,
-            group_reward=self.group_reward[agent_index],
-        )
-
-    def __iter__(self) -> Iterator[Any]:
-        yield from self.agent_id
-
-    @staticmethod
-    def empty(spec: "BehaviorSpec") -> "DecisionSteps":
-        """
-        Returns an empty DecisionSteps.
-        :param spec: The BehaviorSpec for the DecisionSteps
-        """
-        obs: List[np.ndarray] = []
-        for sen_spec in spec.observation_specs:
-            obs += [np.zeros((0,) + sen_spec.shape, dtype=np.float32)]
-        return DecisionSteps(
-            obs=obs,
-            reward=np.zeros(0, dtype=np.float32),
-            agent_id=np.zeros(0, dtype=np.int32),
-            action_mask=None,
-            group_id=np.zeros(0, dtype=np.int32),
-            group_reward=np.zeros(0, dtype=np.float32),
-        )
+        if self.executable_file == '' or self.executable_file == '@editor':
+            print('Waiting for UnityEditor Play...')
+            self.process = None
+        elif os.path.exists(self.executable_file):
+            self.port = self._get_port()
+            self.process = self._start_unity_env(self.executable_file, self.port)
+        else:
+            raise Exception('Executable file not exists')
+        self.communicator = RFUniverseCommunicator(port=self.port, receive_data_callback=self._receive_data)
+        self._send_debug_data('SendVersion', pyrfuniverse.__version__)
+        if len(self.pre_load_assets) > 0:
+            self.PreLoadAssetsAsync(assets, True)
+        if self.scene_file is not None:
+            self.LoadSceneAsync(self.scene_file, True)
 
+    def _get_port(self) -> int:
+        executable_port = 5005
+        s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+        while True:
+            try:
+                s.bind(("localhost", executable_port))
+                s.close()
+                return executable_port
+            except OSError:
+                executable_port += 1
+                continue
 
-class TerminalStep(NamedTuple):
-    """
-    Contains the data a single Agent collected when its episode ended.
-     - obs is a list of numpy arrays observations collected by the agent.
-     - reward is a float. Corresponds to the rewards collected by the agent
-     since the last simulation step.
-     - interrupted is a bool. Is true if the Agent was interrupted since the last
-     decision step. For example, if the Agent reached the maximum number of steps for
-     the episode.
-     - agent_id is an int and an unique identifier for the corresponding Agent.
-    """
+    def _start_unity_env(self, executable_file: str, port: int) -> subprocess.Popen:
+        arg = [executable_file]
+        if not self.graphics:
+            arg.extend(["-nographics", "-batchmode"])
+        arg.append(f'-port:{port}')
+        return subprocess.Popen(arg)
 
-    obs: List[np.ndarray]
-    reward: float
-    interrupted: bool
-    agent_id: AgentId
-    group_id: GroupId
-    group_reward: float
+    def _receive_data(self, objs: list) -> None:
+        type = objs[0]
+        objs = objs[1:]
+        if type == 'Env':
+            self._parse_env_data(objs)
+        elif type == 'Instance':
+            self._parse_instence_data(objs)
+        elif type == 'Debug':
+            self._parse_debug_data(objs)
+        elif type == 'Message':
+            self._parse_message_data(objs)
+        elif type == 'Object':
+            self._parse_object_data(objs)
+        return
+    def _parse_env_data(self, objs: list) -> None:
+        type = objs[0]
+        objs = objs[1:]
+        if type == 'LoadDone':
+            self.data['load_done'] = True
+        elif type == 'PendDone':
+            self.data['pend_done'] = True
+        elif type == 'RFMoveColliders':
+            self.data['colliders'] = objs[0]
+        elif type == 'CurrentCollisionPairs':
+            self.data['collision_pairs'] = objs[0]
+        else:
+            print(f'unknown env data type: {type}')
 
+    def _parse_instence_data(self, objs: list) -> None:
+        this_object_id = objs[0]
+        this_object_type = objs[1]
+        this_object_data = objs[2]
 
-class TerminalSteps(Mapping):
-    """
-    Contains the data a batch of Agents collected when their episode
-    terminated. All Agents present in the TerminalSteps have ended their
-    episode.
-     - obs is a list of numpy arrays observations collected by the batch of
-     agent. Each obs has one extra dimension compared to DecisionStep: the
-     first dimension of the array corresponds to the batch size of the batch.
-     - reward is a float vector of length batch size. Corresponds to the
-     rewards collected by each agent since the last simulation step.
-     - interrupted is an array of booleans of length batch size. Is true if the
-     associated Agent was interrupted since the last decision step. For example, if the
-     Agent reached the maximum number of steps for the episode.
-     - agent_id is an int vector of length batch size containing unique
-     identifier for the corresponding Agent. This is used to track Agents
-     across simulation steps.
-    """
+        attr_type = eval('attr.' + this_object_type)
+        if this_object_id not in self.attrs:
+            self.attrs[this_object_id] = attr_type(self, this_object_id)
+        elif type(self.attrs[this_object_id]) != attr_type:
+            self.attrs[this_object_id] = attr_type(self, this_object_id, self.attrs[this_object_id].data)
 
-    def __init__(self, obs, reward, interrupted, agent_id, group_id, group_reward):
-        self.obs: List[np.ndarray] = obs
-        self.reward: np.ndarray = reward
-        self.interrupted: np.ndarray = interrupted
-        self.agent_id: np.ndarray = agent_id
-        self.group_id: np.ndarray = group_id
-        self.group_reward: np.ndarray = group_reward
-        self._agent_id_to_index: Optional[Dict[AgentId, int]] = None
-
-    @property
-    def agent_id_to_index(self) -> Dict[AgentId, int]:
-        """
-        :returns: A Dict that maps agent_id to the index of those agents in
-        this TerminalSteps.
-        """
-        if self._agent_id_to_index is None:
-            self._agent_id_to_index = {}
-            for a_idx, a_id in enumerate(self.agent_id):
-                self._agent_id_to_index[a_id] = a_idx
-        return self._agent_id_to_index
-
-    def __len__(self) -> int:
-        return len(self.agent_id)
-
-    def __getitem__(self, agent_id: AgentId) -> TerminalStep:
-        """
-        returns the TerminalStep for a specific agent.
-        :param agent_id: The id of the agent
-        :returns: obs, reward, done, agent_id and optional action mask for a
-        specific agent
-        """
-        if agent_id not in self.agent_id_to_index:
-            raise KeyError(f"agent_id {agent_id} is not present in the TerminalSteps")
-        agent_index = self._agent_id_to_index[agent_id]  # type: ignore
-        agent_obs = []
-        for batched_obs in self.obs:
-            agent_obs.append(batched_obs[agent_index])
-        group_id = self.group_id[agent_index]
-        return TerminalStep(
-            obs=agent_obs,
-            reward=self.reward[agent_index],
-            interrupted=self.interrupted[agent_index],
-            agent_id=agent_id,
-            group_id=group_id,
-            group_reward=self.group_reward[agent_index],
-        )
-
-    def __iter__(self) -> Iterator[Any]:
-        yield from self.agent_id
-
-    @staticmethod
-    def empty(spec: "BehaviorSpec") -> "TerminalSteps":
-        """
-        Returns an empty TerminalSteps.
-        :param spec: The BehaviorSpec for the TerminalSteps
-        """
-        obs: List[np.ndarray] = []
-        for sen_spec in spec.observation_specs:
-            obs += [np.zeros((0,) + sen_spec.shape, dtype=np.float32)]
-        return TerminalSteps(
-            obs=obs,
-            reward=np.zeros(0, dtype=np.float32),
-            interrupted=np.zeros(0, dtype=bool),
-            agent_id=np.zeros(0, dtype=np.int32),
-            group_id=np.zeros(0, dtype=np.int32),
-            group_reward=np.zeros(0, dtype=np.float32),
-        )
+        self.data[this_object_id] = self.attrs[this_object_id].parse_message(this_object_data)
 
+    def _parse_debug_data(self, objs: list) -> None:
+        return
 
-class _ActionTupleBase(ABC):
-    """
-    An object whose fields correspond to action data of continuous and discrete
-    spaces. Dimensions are of (n_agents, continuous_size) and (n_agents, discrete_size),
-    respectively. Note, this also holds when continuous or discrete size is
-    zero.
-    """
+    def _parse_message_data(self, objs: list) -> None:
+        msg = objs[0]
+        objs = objs[1:]
+        if msg in self.listen_messages:
+            self.listen_messages[msg](IncomingMessage(objs[0]))
 
-    def __init__(
-        self,
-        continuous: Optional[np.ndarray] = None,
-        discrete: Optional[np.ndarray] = None,
-    ):
-        self._continuous: Optional[np.ndarray] = None
-        self._discrete: Optional[np.ndarray] = None
-        if continuous is not None:
-            self.add_continuous(continuous)
-        if discrete is not None:
-            self.add_discrete(discrete)
-
-    @property
-    def continuous(self) -> np.ndarray:
-        return self._continuous
-
-    @property
-    def discrete(self) -> np.ndarray:
-        return self._discrete
-
-    def add_continuous(self, continuous: np.ndarray) -> None:
-        if continuous.dtype != np.float32:
-            continuous = continuous.astype(np.float32, copy=False)
-        if self._discrete is None:
-            self._discrete = np.zeros(
-                (continuous.shape[0], 0), dtype=self.discrete_dtype
-            )
-        self._continuous = continuous
-
-    def add_discrete(self, discrete: np.ndarray) -> None:
-        if discrete.dtype != self.discrete_dtype:
-            discrete = discrete.astype(self.discrete_dtype, copy=False)
-        if self._continuous is None:
-            self._continuous = np.zeros((discrete.shape[0], 0), dtype=np.float32)
-        self._discrete = discrete
-
-    @property
-    @abstractmethod
-    def discrete_dtype(self) -> np.dtype:
-        pass
+    def _parse_object_data(self, objs: list) -> None:
+        head = objs[0]
+        objs = objs[1:]
+        if head in self.listen_object:
+            self.listen_object[head](objs)
 
+    def _send_env_data(self, *args) -> None:
+        self.communicator.send_object('Env', *args)
 
-class ActionTuple(_ActionTupleBase):
-    """
-    An object whose fields correspond to actions of different types.
-    Continuous and discrete actions are numpy arrays of type float32 and
-    int32, respectively and are type checked on construction.
-    Dimensions are of (n_agents, continuous_size) and (n_agents, discrete_size),
-    respectively. Note, this also holds when continuous or discrete size is
-    zero.
-    """
+    def _send_instance_data(self, *args) -> None:
+        self.communicator.send_object('Instance', *args)
+
+    def _send_debug_data(self, *args) -> None:
+        self.communicator.send_object('Debug', *args)
 
-    @property
-    def discrete_dtype(self) -> np.dtype:
+    def _send_message_data(self, *args) -> None:
+        self.communicator.send_object('Message', *args)
+
+    def _send_object_data(self, *args) -> None:
+        self.communicator.send_object('Object', *args)
+
+    def _step(self):
+        self.communicator.sync_step()
+
+    def step(self, count: int = 1):
+        """
+        Send the messages of called functions to Unity and simulate for a step, then accept the data from Unity.
+
+        Args:
+            count: the number of steps for executing Unity simulation.
         """
-        The dtype of a discrete action.
+        if count < 1:
+            count = 1
+        for _ in range(count):
+            self._step()
+
+    def close(self):
+        """
+        Close the environment
         """
-        return np.int32
+        if self.process is not None:
+            self.process.kill()
 
+    def GetAttr(self, id: int):
+        """
+        Get the attribute instance by object id.
 
-class ActionSpec(NamedTuple):
-    """
-    A NamedTuple containing utility functions and information about the action spaces
-    for a group of Agents under the same behavior.
-    - num_continuous_actions is an int corresponding to the number of floats which
-    constitute the action.
-    - discrete_branch_sizes is a Tuple of int where each int corresponds to
-    the number of discrete actions available to the agent on an independent action branch.
-    """
+        Args:
+            id: Int, object id.
 
-    continuous_size: int
-    discrete_branches: Tuple[int, ...]
+        Returns:
+            pyrfuniverse.attributes.BaseAttr: An instance of attribute.
+        """
+        assert id in self.attrs, 'this ID not exists'
+        return self.attrs[id]
 
-    def __eq__(self, other):
-        return (
-            self.continuous_size == other.continuous_size
-            and self.discrete_branches == other.discrete_branches
-        )
+    #Env API
+    def PreLoadAssetsAsync(self, names: list, auto_wait: bool = False) -> None:
+        """
+        PreLoad the asset.
 
-    def __str__(self):
-        return f"Continuous: {self.continuous_size}, Discrete: {self.discrete_branches}"
+        Args:
+            names: list, the name of assets.
+            auto_wait: Bool, if True, this function will not return until the loading is done.
+        """
+        self._send_env_data('PreLoadAssetsAsync', names)
 
-    # For backwards compatibility
-    def is_discrete(self) -> bool:
+        if auto_wait:
+            self.WaitLoadDone()
+
+    def LoadSceneAsync(self, file: str, auto_wait: bool = False) -> None:
         """
-        Returns true if this Behavior uses discrete actions
+        Load the scene asynchronisely.
+
+        Args:
+            file: Str, the scene JSON file. If it's a relative path, it will load from `StraemingAssets`.
+            auto_wait: Bool, if True, this function will not return until the loading is done.
         """
-        return self.discrete_size > 0 and self.continuous_size == 0
+        self._send_env_data('LoadSceneAsync', file)
 
-    # For backwards compatibility
-    def is_continuous(self) -> bool:
+        if auto_wait:
+            self.WaitLoadDone()
+
+    def SwitchSceneAsync(self, name: str, auto_wait: bool = False) -> None:
         """
-        Returns true if this Behavior uses continuous actions
+        Switch the scene asynchronisely.
+
+        Args:
+            name: Str, the scene name.
+            auto_wait: Bool, if True, this function will not return until the loading is done.
         """
-        return self.discrete_size == 0 and self.continuous_size > 0
+        self._send_env_data('SwitchSceneAsync', name)
+
+        if auto_wait:
+            self.WaitLoadDone()
 
-    @property
-    def discrete_size(self) -> int:
+    def WaitLoadDone(self) -> None:
         """
-        Returns a an int corresponding to the number of discrete branches.
+        Wait for the loading is done.
         """
-        return len(self.discrete_branches)
+        self.data['load_done'] = False
+        while not self.data['load_done']:
+            self._step()
 
-    def empty_action(self, n_agents: int) -> ActionTuple:
+    def Pend(self) -> None:
         """
-        Generates ActionTuple corresponding to an empty action (all zeros)
-        for a number of agents.
-        :param n_agents: The number of agents that will have actions generated
+        Pend the program until the `EndPend` button in `UnityPlayer` is clicked.
+        """
+        self._send_env_data('Pend')
+
+        self.data['pend_done'] = False
+        while not self.data['pend_done']:
+            self._step()
+
+    def SendMessage(self, message: str, *args) -> None:
         """
-        _continuous = np.zeros((n_agents, self.continuous_size), dtype=np.float32)
-        _discrete = np.zeros((n_agents, self.discrete_size), dtype=np.int32)
-        return ActionTuple(continuous=_continuous, discrete=_discrete)
+        Send message to Unity.
 
-    def random_action(self, n_agents: int) -> ActionTuple:
+        Args:
+            message: Str, the message head.
+            *args: List, the list of parameters. We support str, bool, int, float and List[float] types.
         """
-        Generates ActionTuple corresponding to a random action (either discrete
-        or continuous) for a number of agents.
-        :param n_agents: The number of agents that will have actions generated
+        msg = OutgoingMessage()
+        for i in args:
+            if type(i) == str:
+                msg.write_string(i)
+            elif type(i) == bool:
+                msg.write_bool(i)
+            elif type(i) == int:
+                msg.write_int32(i)
+            elif type(i) == float or type(i) == np.float32 or type(i) == np.float64:
+                msg.write_float32(float(i))
+            elif type(i) == list and type(i[0]) == float:
+                msg.write_float32_list(i)
+            else:
+                print(f'dont support this data type:{type(i)}')
+        self._send_message_data(message, msg.buffer)
+
+    def SendObject(self, head: str, *args) -> None:
         """
-        _continuous = np.random.uniform(
-            low=-1.0, high=1.0, size=(n_agents, self.continuous_size)
-        )
-        _discrete = np.zeros((n_agents, self.discrete_size), dtype=np.int32)
-        if self.discrete_size > 0:
-            _discrete = np.column_stack(
-                [
-                    np.random.randint(
-                        0,
-                        self.discrete_branches[i],  # type: ignore
-                        size=(n_agents),
-                        dtype=np.int32,
-                    )
-                    for i in range(self.discrete_size)
-                ]
-            )
-        return ActionTuple(continuous=_continuous, discrete=_discrete)
+        Send object to Unity.
 
-    def _validate_action(
-        self, actions: ActionTuple, n_agents: int, name: str
-    ) -> ActionTuple:
+        Args:
+            head: Str, the message head.
+            *args: List, the list of parameters. We support str, bool, int, float and List[float] types.
         """
-        Validates that action has the correct action dim
-        for the correct number of agents and ensures the type.
+        self._send_object_data(head, *args)
+
+    def AddListener(self, message: str, fun):
         """
-        _expected_shape = (n_agents, self.continuous_size)
-        if actions.continuous.shape != _expected_shape:
-            raise UnityActionException(
-                f"The behavior {name} needs a continuous input of dimension "
-                f"{_expected_shape} for (<number of agents>, <action size>) but "
-                f"received input of dimension {actions.continuous.shape}"
-            )
-        _expected_shape = (n_agents, self.discrete_size)
-        if actions.discrete.shape != _expected_shape:
-            raise UnityActionException(
-                f"The behavior {name} needs a discrete input of dimension "
-                f"{_expected_shape} for (<number of agents>, <action size>) but "
-                f"received input of dimension {actions.discrete.shape}"
-            )
-        return actions
+        Add listener.
 
-    @staticmethod
-    def create_continuous(continuous_size: int) -> "ActionSpec":
+        Args:
+            message: Str, the message head.
+            fun: Callable, the callback function.
         """
-        Creates an ActionSpec that is homogenously continuous
+        self.listen_messages[message] = fun
+
+    def RemoveListener(self, message: str, fun):
         """
-        return ActionSpec(continuous_size, ())
+        Remove listener.
 
-    @staticmethod
-    def create_discrete(discrete_branches: Tuple[int]) -> "ActionSpec":
+        Args:
+            message: Str, the message head.
+            fun: Callable, the callback function.
         """
-        Creates an ActionSpec that is homogenously discrete
+        self.listen_messages.pop(message)
+
+    def AddListenerObject(self, type: str, fun):
         """
-        return ActionSpec(0, discrete_branches)
+        Add object listener.
 
+        Args:
+            type: Str, the message head.
+            fun: Callable, the callback function.
+        """
+        self.listen_object[type] = fun
 
-class DimensionProperty(IntFlag):
-    """
-    The dimension property of a dimension of an observation.
-    """
+    def RemoveListenerObject(self, type: str):
+        """
+        Remove object listener.
 
-    UNSPECIFIED = 0
-    """
-    No properties specified.
-    """
+        Args:
+            type: Str, the message head.
+        """
+        self.listen_object.pop(type)
 
-    NONE = 1
-    """
-    No Property of the observation in that dimension. Observation can be processed with
-    Fully connected networks.
-    """
+    def InstanceObject(self, name: str, id: int = None, attr_type: type = attr.BaseAttr):
+        """
+        Instanciate an object.
 
-    TRANSLATIONAL_EQUIVARIANCE = 2
-    """
-    Means it is suitable to do a convolution in this dimension.
-    """
+        Built-in assets:
+    
+        GameObjectAttr:
+            Basic Objects:
+                "GameObject_Box",
+                "GameObject_Capsule",
+                "GameObject_Cylinder",
+                "GameObject_Sphere",
+                "GameObject_Quad",
+            IGbison Meshes:
+                "Hainesburg_mesh_texture",
+                "Halfway_mesh_texture",
+                "Hallettsville_mesh_texture",
+                "Hambleton_mesh_texture",
+                "Hammon_mesh_texture",
+                "Hatfield_mesh_texture",
+                "Haxtun_mesh_texture",
+                "Haymarket_mesh_texture",
+                "Hendrix_mesh_texture",
+                "Hercules_mesh_texture",
+                "Highspire_mesh_texture",
+                "Hitchland_mesh_texture",
 
-    VARIABLE_SIZE = 4
-    """
-    Means that there can be a variable number of observations in this dimension.
-    The observations are unordered.
-    """
+        ColliderAttr:
+            "Collider_Box",
+            "Collider_ObiBox",
+            "Collider_Capsule",
+            "Collider_Cylinder",
+            "Collider_Sphere",
+            "Collider_Quad",
 
+        RigidbodyAttr:
+            Basic Objects:
+                "Rigidbody_Box",
+                "GameObject_Capsule",
+                "Rigidbody_Cylinder",
+                "Rigidbody_Sphere",
+            YCB dataset: 
+                77 models in YCB dataset. See YCB Object and Model Set for detail: https://rse-lab.cs.washington.edu/projects/posecnn/
 
-class ObservationType(Enum):
-    """
-    An Enum which defines the type of information carried in the observation
-    of the agent.
-    """
+        ControllerAttr:
+            gripper:
+                "allegro_hand_right",
+                "bhand",
+                "svh",
+                "robotiq_arg2f_85_model",
+                "dh_robotics_ag95_gripper",
+            robot:
+                "kinova_gen3",
+                "kinova_gen3_robotiq85",
+                "ur5",
+                "ur5_robotiq85",
+                "franka_panda",
+                "franka_hand",
+                "tobor_robotiq85_robotiq85",
+                "flexivArm",
+                "flexivArm_ag95",
+                "yumi",
 
-    DEFAULT = 0
-    """
-    Observation information is generic.
-    """
+        CameraAttr:
+            "Camera",
 
-    GOAL_SIGNAL = 1
-    """
-    Observation contains goal information for current task.
-    """
+        LightAttr:
+            "Light",
 
+        Args:
+            name: Str, object name. Please check the above `built-in assets` list for names.
+            id: Int, object id.
+            attr_type: type(pyrfuniverse.attributes.BaseAttr), the attribute type.
 
-class ObservationSpec(NamedTuple):
-    """
-    A NamedTuple containing information about the observation of Agents.
-    - shape is a Tuple of int : It corresponds to the shape of
-    an observation's dimensions.
-    - dimension_property is a Tuple of DimensionProperties flag, one flag for each
-    dimension.
-    - observation_type is an enum of ObservationType.
-    """
+        Returns:
+            type(`attr_type`): The object attribute instance.
+        """
+        assert id not in self.attrs, \
+            'this ID exists'
 
-    shape: Tuple[int, ...]
-    dimension_property: Tuple[DimensionProperty, ...]
-    observation_type: ObservationType
+        while id is None or id in self.attrs:
+            id = random.randint(100000, 999999)
 
-    # Optional name. For observations coming from com.unity.ml-agents, this
-    # will be the ISensor name.
-    name: str
+        self._send_env_data('InstanceObject', name, id)
 
+        self.attrs[id] = attr_type(self, id)
+        return self.attrs[id]
 
-class BehaviorSpec(NamedTuple):
-    """
-    A NamedTuple containing information about the observation and action
-    spaces for a group of Agents under the same behavior.
-    - observation_specs is a List of ObservationSpec NamedTuple containing
-    information about the information of the Agent's observations such as their shapes.
-    The order of the ObservationSpec is the same as the order of the observations of an
-    agent.
-    - action_spec is an ActionSpec NamedTuple.
-    """
+    def LoadURDF(self, path: str, id: int = None, native_ik: bool = True, axis: str = 'y') -> attr.ControllerAttr:
+        """
+        Load a model from URDF file.
 
-    observation_specs: List[ObservationSpec]
-    action_spec: ActionSpec
+        Args:
+            path: Str, the URDF file path.
+            id: Int, object id.
+            native_ik: Bool, True for enabling native IK; False for using custom IK.When it is True, through the IKTargetDo*** interface, according to the end pose.When it is False, through the SetJoint*** interface, according to the joint movement.
+            axis: Str, import axis, This can be 'z' or 'y', depending on the URDF file
 
+        Returns:
+            pyrfuniverse.attributes.ControllerAttr: The object attribute intance.
+        """
+        assert id not in self.attrs, 'this ID exists'
 
-class BehaviorMapping(Mapping):
-    def __init__(self, specs: Dict[BehaviorName, BehaviorSpec]):
-        self._dict = specs
+        while id is None or id in self.attrs:
+            id = random.randint(100000, 999999)
 
-    def __len__(self) -> int:
-        return len(self._dict)
+        self._send_env_data('LoadURDF', id, path, native_ik, axis)
 
-    def __getitem__(self, behavior: BehaviorName) -> BehaviorSpec:
-        return self._dict[behavior]
+        self.attrs[id] = attr.ControllerAttr(self, id)
+        return self.attrs[id]
 
-    def __iter__(self) -> Iterator[Any]:
-        yield from self._dict
+    def LoadMesh(self, path: str, id: int = None) -> attr.RigidbodyAttr:
+        """
+        Load a model from Mesh file.
 
+        Args:
+            path: Str, the Mesh file path.
+            id: Int, object id.
 
-class BaseEnv(ABC):
-    @abstractmethod
-    def step(self) -> None:
+        Returns:
+            pyrfuniverse.attributes.RigidbodyAttr: The object attribute intance.
         """
-        Signals the environment that it must move the simulation forward
-        by one step.
+        assert id not in self.attrs, \
+            'this ID exists'
+
+        while id is None or id in self.attrs:
+            id = random.randint(100000, 999999)
+
+        self._send_env_data('LoadMesh', id, path)
+
+        self.attrs[id] = attr.RigidbodyAttr(self, id)
+        return self.attrs[id]
+
+    def IgnoreLayerCollision(self, layer1: int, layer2: int, ignore: bool) -> None:
         """
+        Ignore or enable the collision between two layers.
 
-    @abstractmethod
-    def reset(self) -> None:
+        Args:
+            layer1: Int, the layer number of the first layer.
+            layer2: Int, the layer number of the second layer.
+            ignore: Bool, True for ignoring collision between two layers; False for enabling collision between two layers.
         """
-        Signals the environment that it must reset the simulation.
+        self._send_env_data('IgnoreLayerCollision', layer1, layer2, ignore)
+
+    def GetCurrentCollisionPairs(self) -> None:
         """
+        Get the collision pairs of current collision.
 
-    @abstractmethod
-    def close(self) -> None:
+        Returns:
+            Call this function and `step()`, the collision pairs can be got from env.data['CurrentCollisionPairs'].
         """
-        Signals the environment that it must close.
+        self._send_env_data('GetCurrentCollisionPairs')
+
+    def GetRFMoveColliders(self) -> None:
         """
+        Get the RFMove colliders.
 
-    @property
-    @abstractmethod
-    def behavior_specs(self) -> MappingType[str, BehaviorSpec]:
+        Returns:
+            Call this function and `step()`, the collision pairs can be got from env.data['RFMoveColliders'].
         """
-        Returns a Mapping from behavior names to behavior specs.
-        Agents grouped under the same behavior name have the same action and
-        observation specs, and are expected to behave similarly in the
-        environment.
-        Note that new keys can be added to this mapping as new policies are instantiated.
+        self._send_env_data('GetRFMoveColliders')
+
+    def SetGravity(self, x: float, y: float, z: float) -> None:
         """
+        Set the gravity of environment.
 
-    @abstractmethod
-    def set_actions(self, behavior_name: BehaviorName, action: ActionTuple) -> None:
+        Args:
+            x: Float, gravity on global x-axis (right).
+            y: Float, gravity on global y-axis (up).
+            z: Float, gravity on global z-axis (forward).
         """
-        Sets the action for all of the agents in the simulation for the next
-        step. The Actions must be in the same order as the order received in
-        the DecisionSteps.
-        :param behavior_name: The name of the behavior the agents are part of
-        :param action: ActionTuple tuple of continuous and/or discrete action.
-        Actions are np.arrays with dimensions  (n_agents, continuous_size) and
-        (n_agents, discrete_size), respectively.
+        self._send_env_data('SetGravity', [float(x), float(y), float(z)])
+
+    def SetGroundActive(self, active: bool) -> None:
+        """
+        Set the ground active or inactive.
+
+        Args:
+            active: Bool, active or inactive the ground.
+        """
+        self._send_env_data('GetRFMoveColliders', active)
+
+    def SetGroundPhysicMaterial(self, bounciness: float, dynamic_friction: float, static_friction: float, friction_combine: int, bounce_combine: int) -> None:
+        """
+        Set the physics material of ground in environment.
+
+        Args:
+            bounciness: Float, the bounciness.
+            dynamic_friction: Float, the dynamic friction coefficient (0-1).
+            static_friction: Float, the static friction coefficient (0-1).
+            friction_combine: Int, how friction of two colliding objects is combined. 0 for Average, 1 for Minimum, 2 for Maximum and 3 for Multiply. See https://docs.unity3d.com/Manual/class-PhysicMaterial.html for more details.
+            bounce_combine: Int, how bounciness of two colliding objects is combined. The value representation is the same with `friction_combine`.
+        """
+        self._send_env_data('SetGroundPhysicMaterial', float(bounciness), float(dynamic_friction), float(static_friction), friction_combine, bounce_combine)
+
+    def SetTimeStep(self, delta_time: float) -> None:
+        """
+        Set the time for a step in Unity.
+
+        Args:
+            delta_time: Float, the time for a step in Unity.
+        """
+        self._send_env_data('SetTimeStep', float(delta_time))
+
+    def SetTimeScale(self, time_scale: float) -> None:
+        """
+        Set the time scale in Unity.
+
+        Args:
+            time_scale: Float, the time scale in Unity.
+        """
+        self._send_env_data('SetTimeScale', float(time_scale))
+
+    def SetResolution(self, resolution_x: int, resolution_y: int) -> None:
+        """
+        Set the resolution of windowed GUI.
+
+        Args:
+            resolution_x: Int, window width.
+            resolution_y: Int, window height.
+        """
+        self._send_env_data('SetResolution', resolution_x, resolution_y)
+
+    def ExportOBJ(self, items_id: list, save_path: str) -> None:
+        """
+        Export the specified object list to OBJ file. For native bundle models, the `Read/Write` must be checked in Unity Editor.
+
+        Args:
+            items_id: List, the object ids.
+            save_path: Str, the path to save the OBJ files.
+        """
+        self._send_env_data('ExportOBJ', items_id, save_path)
+
+    def SetShadowDistance(self, distance: float) -> None:
+        """
+        Set the shadow distance for rendering in environment.
+
+        Args:
+            distance: Float, the shadow distance measured in meter.
+        """
+        self._send_env_data('SetShadowDistance', float(distance))
+
+    def SaveScene(self, file: str) -> None:
+        """
+        Save current scene.
+
+        Args:
+            file: Str, the file path to save current scene. Default saving to `StreamingAssets` folder.
+        """
+        self._send_env_data('SaveScene', file)
+
+    def ClearScene(self) -> None:
+        """
+        Clear current scene.
+        """
+        self._send_env_data('ClearScene')
+
+    def AlignCamera(self, camera_id: int) -> None:
         """
+        Align current GUI view to a given camera.
 
-    @abstractmethod
-    def set_action_for_agent(
-        self, behavior_name: BehaviorName, agent_id: AgentId, action: ActionTuple
-    ) -> None:
+        Args:
+            camera_id: Int, camera id.
         """
-        Sets the action for one of the agents in the simulation for the next
-        step.
-        :param behavior_name: The name of the behavior the agent is part of
-        :param agent_id: The id of the agent the action is set for
-        :param action: ActionTuple tuple of continuous and/or discrete action
-        Actions are np.arrays with dimensions  (1, continuous_size) and
-        (1, discrete_size), respectively. Note, this initial dimensions of 1 is because
-        this action is meant for a single agent.
+        self._send_env_data('AlignCamera', camera_id)
+
+    def SetViewTransform(self, position: list = None, rotation: list = None) -> None:
         """
+        Set the GUI view.
 
-    @abstractmethod
-    def get_steps(
-        self, behavior_name: BehaviorName
-    ) -> Tuple[DecisionSteps, TerminalSteps]:
+        Args:
+            position: A list of length 3, representing the position of GUI view.
+            rotation: A list of length 3, representing the rotation of GUI view.
         """
-        Retrieves the steps of the agents that requested a step in the
-        simulation.
-        :param behavior_name: The name of the behavior the agents are part of
-        :return: A tuple containing :
-         - A DecisionSteps NamedTuple containing the observations,
-         the rewards, the agent ids and the action masks for the Agents
-         of the specified behavior. These Agents need an action this step.
-         - A TerminalSteps NamedTuple containing the observations,
-         rewards, agent ids and interrupted flags of the agents that had their
-         episode terminated last step.
+        if position is not None:
+            assert type(position) == list and len(position) == 3, \
+                'Argument position must be a 3-d list.'
+            position = [float(i) for i in position]
+        if rotation is not None:
+            assert type(rotation) == list and len(rotation) == 3, \
+                'Argument rotation must be a 3-d list.'
+            rotation = [float(i) for i in rotation]
+
+        self._send_env_data('SetViewTransform', position, rotation)
+
+    def SetViewBackGround(self, color: list = None) -> None:
         """
+        Set the GUI view.
+
+        Args:
+            color: A list of length 3, background color of GUI view. None : default skybox.
+        """
+        if color is not None:
+            assert type(color) == list and len(color) == 3, 'color length must be 3'
+            color = [float(i) for i in color]
+
+        self._send_env_data('SetViewBackGround', color)
+
+
+    #Dubug API
+    def DebugGraspPoint(self, enabled: bool = True) -> None:
+        """
+        Show or hide end effector of robot arm for debug.
+
+        Args:
+            enabled: Bool, True for showing and False for hiding.
+        """
+        self._send_debug_data('DebugGraspPoint', enabled)
+
+    def DebugObjectPose(self, enabled: bool = True) -> None:
+        """
+        Show or hide object base point for debug.
+
+        Args:
+            enabled: Bool, True for showing and False for hiding.
+        """
+        self._send_debug_data('DebugObjectPose', enabled)
+
+    def DebugCollisionPair(self, enabled: bool = True) -> None:
+        """
+        Show or hide collision pairs for debug.
+
+        Args:
+            enabled: Bool, True for showing and False for hiding.
+        """
+        self._send_debug_data('DebugCollisionPair', enabled)
+    
+    def DebugColliderBound(self, enabled: bool = True) -> None:
+        """
+        Show or hide collider bounding box for debug.
+
+        Args:
+            enabled: Bool, True for showing and False for hiding.
+        """
+        self._send_debug_data('DebugColliderBound', enabled)
+
+    def DebugObjectID(self, enabled: bool = True) -> None:
+        """
+        Show or hide object id for debug.
+
+        Args:
+            enabled: Bool, True for showing and False for hiding.
+        """
+        self._send_debug_data('DebugObjectID', enabled)
+
+    def Debug3DBBox(self, enabled: bool = True) -> None:
+        """
+        Show or hide 3d bounding box of objects for debug.
+
+        Args:
+            enabled: Bool, True for showing and False for hiding.
+        """
+        self._send_debug_data('Debug3DBBox', enabled)
+
+    def Debug2DBBox(self, enabled: bool = True) -> None:
+        """
+        Show or hide 2d bounding box of objects for debug.
+
+        Args:
+            enabled: Bool, True for showing and False for hiding.
+        """
+        self._send_debug_data('Debug2DBBox', enabled)
+
+    def DebugJointLink(self, enabled: bool = True) -> None:
+        """
+        Show or hide joint information of articulation for debug.
+
+        Args:
+            enabled: Bool, True for showing and False for hiding.
+        """
+        self._send_debug_data('DebugJointLink', enabled)
+
+    def SendLog(self, log: str) -> None:
+        """
+        Send log messange and show it on Unity GUI window.
+
+        Args:
+            log: Str, log message.
+        """
+        self._send_debug_data('SendLog', log)
+
```

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/envs/__init__.py` & `pyrfuniverse-0.9.10/pyrfuniverse/envs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,13 @@
-from pyrfuniverse.envs.base_env import RFUniverseBaseEnv
-from pyrfuniverse.envs.base_env import RFUniverseGymWrapper
-from pyrfuniverse.envs.base_env import RFUniverseGymGoalWrapper
+# from pyrfuniverse.envs.base_env import RFUniverseBaseEnv
+# try:
+#     from pyrfuniverse.envs.gym_wrapper_env import RFUniverseGymWrapper
+#     from pyrfuniverse.envs.gym_goal_wrapper import RFUniverseGymGoalWrapper
+# except ImportError:
+#     pass
 # from pyrfuniverse.envs.franka_grasp_env import FrankaGraspEnv
 # from pyrfuniverse.envs.franka_push_env import FrankaPushEnv
 # from pyrfuniverse.envs.balance_ball_env import BalanceBallEnv
 # from pyrfuniverse.envs.balance_ball_env import BalanceBallEnvV0
 # from pyrfuniverse.envs.bouncer_env import BouncerEnv
 # from pyrfuniverse.envs.bouncer_env import BouncerEnvV0
 # from pyrfuniverse.envs.roller_env import RollerEnv
```

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/envs/balance_ball_env.py` & `pyrfuniverse-0.9.10/pyrfuniverse/envs/balance_ball_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/envs/bouncer_env.py` & `pyrfuniverse-0.9.10/pyrfuniverse/envs/bouncer_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/envs/franka_grasp_env.py` & `pyrfuniverse-0.9.10/pyrfuniverse/envs/franka_grasp_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/envs/franka_push_env.py` & `pyrfuniverse-0.9.10/pyrfuniverse/envs/franka_push_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/envs/gripper_nail/__init__.py` & `pyrfuniverse-0.9.10/pyrfuniverse/envs/gripper_nail/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/envs/gripper_nail/nail_can_env.py` & `pyrfuniverse-0.9.10/pyrfuniverse/envs/gripper_nail/nail_can_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/envs/gripper_nail/nail_card_env.py` & `pyrfuniverse-0.9.10/pyrfuniverse/envs/gripper_nail/nail_card_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/envs/gripper_nail/robotiq85_insert_env.py` & `pyrfuniverse-0.9.10/pyrfuniverse/envs/gripper_nail/robotiq85_insert_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/envs/gripper_nail/robotiq85_nail_book_env.py` & `pyrfuniverse-0.9.10/pyrfuniverse/envs/gripper_nail/robotiq85_nail_book_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/envs/gripper_nail/robotiq85_nail_can_env.py` & `pyrfuniverse-0.9.10/pyrfuniverse/envs/gripper_nail/robotiq85_nail_can_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/envs/gripper_nail/robotiq85_nail_card_env.py` & `pyrfuniverse-0.9.10/pyrfuniverse/envs/gripper_nail/robotiq85_nail_card_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/envs/gripper_nail/robotiq85_nail_coin_env.py` & `pyrfuniverse-0.9.10/pyrfuniverse/envs/gripper_nail/robotiq85_nail_coin_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/envs/multi_agent/cleaner_env.py` & `pyrfuniverse-0.9.10/pyrfuniverse/envs/multi_agent/cleaner_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/envs/multi_agent/navigation_env.py` & `pyrfuniverse-0.9.10/pyrfuniverse/envs/multi_agent/navigation_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/envs/multi_agent_navigation_env.py` & `pyrfuniverse-0.9.10/pyrfuniverse/envs/multi_agent_navigation_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/envs/multi_physics/__init__.py` & `pyrfuniverse-0.9.10/pyrfuniverse/envs/multi_physics/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/envs/multi_physics/kinova_gen2_catching_cloth_env.py` & `pyrfuniverse-0.9.10/pyrfuniverse/envs/multi_physics/kinova_gen2_catching_cloth_env.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import math
-from pyrfuniverse.envs import RFUniverseGymWrapper
+from pyrfuniverse.envs.gym_wrapper_env import RFUniverseGymWrapper
 import pyrfuniverse.attributes as attr
 from pyrfuniverse.utils.jaco_controller import RFUniverseJacoController
 import numpy as np
 from gym import spaces
 from gym.utils import seeding
 import pybullet as p
 
@@ -162,33 +162,33 @@
         joint_positions[7] = 50
         joint_positions[8] = 50
         joint_positions[9] = 50
         self.attrs[self.object2id['kinova']].SetJointPositionDirectly(joint_positions=list(joint_positions[0:10]))
         self._step()
 
     def _get_eef_position(self):
-        return np.array(self.instance_channel.data[self.object2id['kinova']]['positions'][15]) / self.scale
+        return np.array(self.attrs[self.object2id['kinova']].data['positions'][15]) / self.scale
 
     def _get_eef_velocity(self):
-        return np.array(self.instance_channel.data[self.object2id['kinova']]['velocities'][15]) / self.scale
+        return np.array(self.attrs[self.object2id['kinova']].data['velocities'][15]) / self.scale
 
     def _get_target_position(self):
-        return np.array(self.instance_channel.data[self.object2id['target']]['position']) / self.scale
+        return np.array(self.attrs[self.object2id['target']].data['position']) / self.scale
 
     def _get_cloth_position(self):
-        return np.array(self.instance_channel.data[self.object2id['cloth']]['avg_position']) / self.scale
+        return np.array(self.attrs[self.object2id['cloth']].data['avg_position']) / self.scale
 
     def _get_cloth_velocity(self):
-        return np.array(self.instance_channel.data[self.object2id['cloth']]['avg_velocity']) / self.scale
+        return np.array(self.attrs[self.object2id['cloth']].data['avg_velocity']) / self.scale
 
     def _get_force_zone_parameters(self):
         return np.array([
-            self.instance_channel.data[self.object2id['cloth']]['force_zone_orientation'] / 180 * math.pi,
-            self.instance_channel.data[self.object2id['cloth']]['force_zone_intensity'],
-            self.instance_channel.data[self.object2id['cloth']]['force_zone_turbulence'],
+            self.attrs[self.object2id['cloth']].data['force_zone_orientation'] / 180 * math.pi,
+            self.attrs[self.object2id['cloth']].data['force_zone_intensity'],
+            self.attrs[self.object2id['cloth']].data['force_zone_turbulence'],
         ])
 
     def _check_fail(self, obs):
         cloth_position = obs[3:6]
         return cloth_position[1] < self.y_bound / self.scale
 
     def _compute_reward(self, obs):
```

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/envs/multi_physics/ur5_water_shooting.py` & `pyrfuniverse-0.9.10/pyrfuniverse/envs/multi_physics/ur5_water_shooting.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pyrfuniverse.envs import RFUniverseGymGoalWrapper
+from pyrfuniverse.envs.gym_goal_wrapper_env import RFUniverseGymGoalWrapper
 from pyrfuniverse.utils.ur5_controller import RFUniverseUR5Controller
 import numpy as np
 import pybullet as p
 from gym import spaces
 from gym.utils import seeding
 import math
 
@@ -173,54 +173,54 @@
         goal = [float(goal_x), 0, float(goal_z)]
         self.attrs[self.object2id['goal']].SetTransform(position=list(goal))
         self._step()
 
         return np.array(goal)
 
     def _reset_liquid(self):
-        self.asset_channel.SendMessage('SetZibraLiquid', False)
+        self.SendMessage('SetZibraLiquid', False)
         self._step()
-        self.asset_channel.SendMessage('SetZibraLiquid', True)
+        self.SendMessage('SetZibraLiquid', True)
         self._step()
 
     def _reset_object(self):
         object_pos = self.np_random.uniform(
             low=self.object_range_low, high=self.object_range_high, size=(3,)
         )
         self.attrs[self.object2id['cube']].SetTransform(position=list(object_pos),
                                                         rotation=[0, 0, 0])
         self._step()
         return object_pos.copy()
 
     def _get_eef_position(self):
-        return np.array(self.instance_channel.data[self.object2id['robotiq85']]['positions'][7])
+        return np.array(self.attrs[self.object2id['robotiq85']].data['positions'][7])
 
     def _get_eef_velocity(self):
-        return np.array(self.instance_channel.data[self.object2id['robotiq85']]['velocities'][7])
+        return np.array(self.attrs[self.object2id['robotiq85']].data['velocities'][7])
 
     def _get_gripper_width(self):
         left_finger_pos = np.array(
-            self.instance_channel.data[self.object2id['left_finger']]['position']
+            self.attrs[self.object2id['left_finger']].data['position']
         )
         right_finger_pos = np.array(
-            self.instance_channel.data[self.object2id['right_finger']]['position']
+            self.attrs[self.object2id['right_finger']].data['position']
         )
         return self._distance(left_finger_pos, right_finger_pos)
 
     def _get_target_pos(self):
-        return np.array(self.instance_channel.data[self.object2id['target']]['position'])
+        return np.array(self.attrs[self.object2id['target']].data['position'])
 
     def _get_cube_pos(self):
-        return np.array(self.instance_channel.data[self.object2id['cube']]['position'])
+        return np.array(self.attrs[self.object2id['cube']].data['position'])
 
     def _get_cube_velocity(self):
-        return np.array(self.instance_channel.data[self.object2id['cube']]['velocity'])
+        return np.array(self.attrs[self.object2id['cube']].data['velocity'])
 
     def _get_cube_rotation(self):
-        return np.array(self.instance_channel.data[self.object2id['cube']]['rotation']) / 180 * math.pi
+        return np.array(self.attrs[self.object2id['cube']].data['rotation']) / 180 * math.pi
 
     def _set_ur5_robotiq85(self, joint_positions):
         self.attrs[self.object2id['ur5']].SetJointPosition(joint_positions=list(joint_positions[:6]))
         self._step()
 
         width = joint_positions[6]
         gripper_angle = self._compute_gripper_angle(width)
@@ -248,15 +248,15 @@
 
     def _set_liquid_parameters(self, gripper_width):
         prop = gripper_width / 0.085
         volume_per_time_step = prop * self.volume_per_time_step_range[1] + \
             (1 - prop) * self.volume_per_time_step_range[0]
         liquid_init_velocity = prop * self.liquid_init_velocity_range[1] + \
             (1 - prop) * self.liquid_init_velocity_range[0]
-        self.asset_channel.SendMessage('SetZibraLiquidEmitter', volume_per_time_step, 0., -liquid_init_velocity, 0.)
+        self.SendMessage('SetZibraLiquidEmitter', volume_per_time_step, 0., -liquid_init_velocity, 0.)
         self._step()
 
     def _check_success(self, achieved_goal, desired_goal):
         distance = abs(achieved_goal - desired_goal)
         return (max(distance[0], distance[2]) < self.tolerance).astype(np.float32)
 
     def _check_fail(self, achieved_goal):
```

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/envs/rfuniverse_robot_hub_env.py` & `pyrfuniverse-0.9.10/pyrfuniverse/envs/rfuniverse_robot_hub_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/envs/robotics/__init__.py` & `pyrfuniverse-0.9.10/pyrfuniverse/envs/robotics/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/envs/robotics/franka_cloth_env.py` & `pyrfuniverse-0.9.10/pyrfuniverse/envs/robotics/franka_cloth_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-from pyrfuniverse.envs import RFUniverseBaseEnv
-from pyrfuniverse.envs import RFUniverseGymGoalWrapper
-# from pyrfuniverse.utils import RFUniverseController
+from pyrfuniverse.envs.gym_goal_wrapper_env import RFUniverseGymGoalWrapper
 import numpy as np
 import math
 import copy
 from gym import spaces
 from gym.utils import seeding
```

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/envs/robotics/franka_cloth_fold_env.py` & `pyrfuniverse-0.9.10/pyrfuniverse/envs/robotics/franka_cloth_fold_env.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pyrfuniverse.envs import RFUniverseGymGoalWrapper
+from pyrfuniverse.envs.gym_goal_wrapper_env import RFUniverseGymGoalWrapper
 # from pyrfuniverse.utils import RFUniverseController
 import numpy as np
 from gym import spaces
 from gym.utils import seeding
 import copy
```

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/envs/robotics/franka_robotics_env.py` & `pyrfuniverse-0.9.10/pyrfuniverse/envs/robotics/franka_robotics_env.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pyrfuniverse.envs import RFUniverseGymGoalWrapper
+from pyrfuniverse.envs.gym_goal_wrapper_env import RFUniverseGymGoalWrapper
 import numpy as np
 from gym import spaces
 from gym.utils import seeding
 import copy
 
 
 class FrankaRoboticsEnv(RFUniverseGymGoalWrapper):
@@ -64,15 +64,15 @@
     def step(self, action: np.ndarray):
         """
         Params:
             action: 4-d numpy array.
         """
         # print(action)
         pos_ctrl = action[:3] * 0.05
-        curr_pos = np.array(self.instance_channel.data[9658740]['positions'][3])
+        curr_pos = np.array(self.attrs[9658740].data['positions'][3])
         # print(curr_pos)
         pos_ctrl = curr_pos + pos_ctrl
 
         # print(pos_ctrl)
         # self.instance_channel.set_action(
         #     "IKTargetDoMove",
         #     id=965874,
@@ -105,15 +105,14 @@
         if self.t == self.max_steps:
             done = True
 
         return obs, reward, done, info
 
     def reset(self):
         super().reset()
-        self.env.reset()
         self.t = 0
         self.goal = self._sample_goal()
         object_pos = None
 
         if self.load_object:
             object_pos = self._reset_object()
 
@@ -149,27 +148,27 @@
         distance = self._compute_goal_distance(achieved_goal, desired_goal)
         if self.reward_type == 'sparse':
             return -(distance > self.tolerance).astype(np.float32)
         else:
             return -distance
 
     def _get_obs(self):
-        gripper_position = np.array(self.instance_channel.data[9658740]['positions'][3])
-        gripper_velocity = np.array(self.instance_channel.data[9658740]['velocities'][3])
+        gripper_position = np.array(self.attrs[9658740].data['positions'][3])
+        gripper_velocity = np.array(self.attrs[9658740].data['velocities'][3])
         gripper_width = self._get_gripper_width()
         # gripper_joint_position = np.array(self.articulation_channel.data[1]['joint_positions'])
         # gripper_joint_velocity = np.array(self.articulation_channel.data[1]['joint_velocities'])
 
         panda_obs = np.concatenate((gripper_position, gripper_velocity, [gripper_width]))
 
         if self.load_object:
-            object_position = np.array(self.instance_channel.data[0]['position'])
-            object_rotation = np.array(self.instance_channel.data[0]['rotation'])
-            object_velocity = np.array(self.instance_channel.data[0]['velocity'])
-            object_angular_vel = np.array(self.instance_channel.data[0]['angular_vel'])
+            object_position = np.array(self.attrs[0].data['position'])
+            object_rotation = np.array(self.attrs[0].data['rotation'])
+            object_velocity = np.array(self.attrs[0].data['velocity'])
+            object_angular_vel = np.array(self.attrs[0].data['angular_vel'])
             # object_rel_pos = object_position - gripper_position
             # object_velocity = object_velocity - gripper_velocity
             achieved_goal = object_position.copy()
         else:
             # object_position = object_rotation = object_velocity = object_angular_vel = object_rel_pos = np.zeros(0)
             object_position = object_rotation = object_velocity = object_angular_vel = np.zeros(0)
             achieved_goal = gripper_position.copy()
@@ -209,15 +208,15 @@
         return random_float
 
     def _set_gripper_width(self, w: float):
         w = w / 2
         self.attrs[9658740].SetJointPosition(joint_positions=[w, w])
 
     def _get_gripper_width(self) -> float:
-        gripper_joint_positions = copy.deepcopy(self.instance_channel.data[9658740]['joint_positions'])
+        gripper_joint_positions = copy.deepcopy(self.attrs[9658740].data['joint_positions'])
         return -1 * (gripper_joint_positions[0] + gripper_joint_positions[1])
 
     def _check_success(self, obs):
         achieved_goal = obs['achieved_goal']
         desired_goal = obs['desired_goal']
         distance = self._compute_goal_distance(achieved_goal, desired_goal)
```

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/envs/robotics/franka_softbody_env.py` & `pyrfuniverse-0.9.10/pyrfuniverse/envs/robotics/franka_softbody_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from pyrfuniverse.envs import RFUniverseBaseEnv
-from pyrfuniverse.envs import RFUniverseGymGoalWrapper
+from pyrfuniverse.envs.gym_goal_wrapper_env import RFUniverseGymGoalWrapper
 # from pyrfuniverse.utils import RFUniverseController
 import numpy as np
 import math
 import copy
 from gym import spaces
 from gym.utils import seeding
```

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/envs/robotics/pick_and_place_env.py` & `pyrfuniverse-0.9.10/pyrfuniverse/envs/robotics/pick_and_place_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/envs/robotics/push_env.py` & `pyrfuniverse-0.9.10/pyrfuniverse/envs/robotics/push_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/envs/robotics/reach_env.py` & `pyrfuniverse-0.9.10/pyrfuniverse/envs/robotics/reach_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/envs/roller_env.py` & `pyrfuniverse-0.9.10/pyrfuniverse/envs/roller_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/envs/tobor_robotics/tobor_push_pull_env.py` & `pyrfuniverse-0.9.10/pyrfuniverse/envs/tobor_robotics/tobor_push_pull_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/envs/tobor_robotiq85_manipulation_env.py` & `pyrfuniverse-0.9.10/pyrfuniverse/envs/tobor_robotiq85_manipulation_env.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,24 +12,16 @@
             only_calculate=False,
             left_init_joint_positions=[0] * 7,
             right_init_joint_positions=[0] * 7
     ):
         super().__init__(
             scene_file=scene_file,
         )
-        self.instance_channel.set_action(
-            'EnabledNativeIK',
-            id=9874610,
-            enabled=False
-        )
-        self.instance_channel.set_action(
-            'EnabledNativeIK',
-            id=9874611,
-            enabled=False
-        )
+        self.GetAttr(9874610).EnabledNativeIK(enabled=False)
+        self.GetAttr(9874611).EnabledNativeIK(enabled=False)
         self._step()
         self.ik_controller = RFUniverseToborController(
             urdf_folder='../URDF/tobor',
             left_hand='robotiq85',
             right_hand='robotiq85',
             left_init_joint_positions=left_init_joint_positions,
             right_init_joint_positions=right_init_joint_positions,
@@ -49,18 +41,18 @@
         self.only_calculate = only_calculate
         #with open(self.record_file, 'w') as f:
             #f.close()
 
     def step(self, mode, position: np.ndarray, orientation=None):
         if mode == 'left':
             # Robotiq85
-            current_position = np.array(self.instance_channel.data[98746100]['positions'][7])
+            current_position = np.array(self.GetAttr(98746100).data['positions'][7])
         else:
             # Robotiq85
-            current_position = np.array(self.instance_channel.data[98746110]['positions'][7])
+            current_position = np.array(self.GetAttr(98746110).data['positions'][7])
 
         distance = position - current_position
         time_steps = int(np.abs(distance / 0.05).max()) + 1
         unit_distance = distance / time_steps
 
         for i in range(time_steps):
             target_position = current_position + unit_distance * (i + 1)
@@ -69,40 +61,36 @@
                 target_position,
                 orientation
             )
 
             if mode == 'left':
                 self.left_joint_positions = joint_positions
                 if not self.only_calculate:
-                    self.instance_channel.set_action(
-                        'SetJointPosition',
-                        id=9874610,
+                    self.GetAttr(9874610).SetJointPosition(
                         joint_positions=list(joint_positions),
                     )
             else:
                 self.right_joint_positions = joint_positions
                 if not self.only_calculate:
-                    self.instance_channel.set_action(
-                        'SetJointPosition',
-                        id=9874611,
+                    self.GetAttr(9874611).SetJointPosition(
                         joint_positions=list(joint_positions),
                     )
 
             for j in range(20):
                 if not self.only_calculate:
                     self._step()
                 self.write()
 
 
     def double_step(self, left_pos, right_pos, left_orn=None, right_orn=None):
-        left_current_pos = np.array(self.instance_channel.data[98746100]['positions'][7])
+        left_current_pos = np.array(self.GetAttr(98746100).data['positions'][7])
         left_distance = left_pos - left_current_pos
         left_time_steps = int(np.abs(left_distance / 0.05).max()) + 1
 
-        right_current_pos = np.array(self.instance_channel.data[98746110]['positions'][7])
+        right_current_pos = np.array(self.GetAttr(98746110).data['positions'][7])
         right_distance = right_pos - right_current_pos
         right_time_steps = int(np.abs(right_distance / 0.05).max()) + 1
 
         time_steps = max(left_time_steps, right_time_steps)
         left_unit_distance = left_distance / time_steps
         right_unit_distance = right_distance / time_steps
 
@@ -119,126 +107,101 @@
                 'right',
                 right_target_position,
                 right_orn
             )
             self.right_joint_positions = right_joint_positions
 
             if not self.only_calculate:
-                self.instance_channel.set_action(
-                    'SetJointPosition',
-                    id=9874610,
+                self.GetAttr(9874610).SetJointPosition(
                     joint_positions=list(left_joint_positions),
                 )
                 self._step()
-                self.instance_channel.set_action(
-                    'SetJointPosition',
-                    id=9874611,
+                self.GetAttr(9874611).SetJointPosition(
                     joint_positions=list(right_joint_positions),
                 )
 
             for j in range(20):
                 if not self.only_calculate:
                     self._step()
                 self.write()
 
     def double_close(self):
         if not self.only_calculate:
-            self.instance_channel.set_action(
-                'SetJointPosition',
-                id=98746100,
-                joint_positions=[50, 50],
+            self.GetAttr(98746100).SetJointPosition(
+                joint_positions=[50, 50]
             )
             self.left_gripper_open = False
             self._step()
-            self.instance_channel.set_action(
-                'SetJointPosition',
-                id=98746110,
-                joint_positions=[50, 50],
+            self.GetAttr(98746110).SetJointPosition(
+                joint_positions=[50, 50]
             )
             self.right_gripper_open = False
             self._step()
 
         for i in range(20):
             if not self.only_calculate:
                 self._step()
             self.write()
 
     def double_open(self):
         if not self.only_calculate:
-            self.instance_channel.set_action(
-                'SetJointPosition',
-                id=98746100,
-                joint_positions=[0, 0],
+            self.GetAttr(98746100).SetJointPosition(
+                joint_positions=[0, 0]
             )
             self.left_gripper_open = True
             self._step()
-            self.instance_channel.set_action(
-                'SetJointPosition',
-                id=98746110,
-                joint_positions=[0, 0],
+            self.GetAttr(98746110).SetJointPosition(
+                joint_positions=[0, 0]
             )
             self.right_gripper_open = True
             self._step()
 
         for i in range(20):
             if not self.only_calculate:
                 self._step()
             self.write()
 
     def reset(self):
-        self.env.reset()
-        self.instance_channel.set_action(
-            'SetJointPositionDirectly',
-            id=9874610,
+        self.GetAttr(9874610).SetJointPositionDirectly(
             joint_positions=self.left_init_joint_positions
         )
         self._step()
-        self.instance_channel.set_action(
-            'SetJointPositionDirectly',
-            id=9874611,
+        self.GetAttr(9874611).SetJointPositionDirectly(
             joint_positions=self.right_init_joint_positions
         )
         self._step()
 
     def close_gripper(self, mode):
         if not self.only_calculate:
             if mode == 'left':
-                self.instance_channel.set_action(
-                    'SetJointPosition',
-                    id=98746100,
-                    joint_positions=[50, 50],
+                self.GetAttr(98746100).SetJointPosition(
+                    joint_positions=[50, 50]
                 )
                 self.left_gripper_open = False
             else:
-                self.instance_channel.set_action(
-                    'SetJointPosition',
-                    id=98746110,
-                    joint_positions=[50, 50],
+                self.GetAttr(98746110).SetJointPosition(
+                    joint_positions=[50, 50]
                 )
                 self.right_gripper_open = False
         for i in range(20):
             if not self.only_calculate:
                 self._step()
             self.write()
 
 
     def open_gripper(self, mode):
         if not self.only_calculate:
             if mode == 'left':
-                self.instance_channel.set_action(
-                    'SetJointPosition',
-                    id=98746100,
-                    joint_positions=[0, 0],
+                self.GetAttr(98746100).SetJointPosition(
+                    joint_positions=[0, 0]
                 )
                 self.left_gripper_open = True
             else:
-                self.instance_channel.set_action(
-                    'SetJointPosition',
-                    id=98746110,
-                    joint_positions=[0, 0],
+                self.GetAttr(98746110).SetJointPosition(
+                    joint_positions=[0, 0]
                 )
                 self.right_gripper_open = True
         for i in range(20):
             if not self.only_calculate:
                 self._step()
             self.write()
 
@@ -274,11 +237,11 @@
 
     def write_raw(self, raw_str):
         with open(self.record_file, 'a+') as f:
             f.write(raw_str)
 
     def get_current_position(self, mode):
         if mode == 'left':
-            return np.array(self.instance_channel.data[98746100]['positions'][7])
+            return np.array(self.GetAttr(98746100).data['positions'][7])
         elif mode == 'right':
-            return np.array(self.instance_channel.data[98746110]['positions'][7])
+            return np.array(self.GetAttr(98746110).data['positions'][7])
```

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/envs/ur5_box_env.py` & `pyrfuniverse-0.9.10/pyrfuniverse/envs/ur5_box_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/envs/ur5_drawer_env.py` & `pyrfuniverse-0.9.10/pyrfuniverse/envs/ur5_drawer_env.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/side_channel/incoming_message.py` & `pyrfuniverse-0.9.10/pyrfuniverse/side_channel/incoming_message.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,43 +20,40 @@
         Read a boolean value from the message buffer.
         :param default_value: Default value to use if the end of the message is reached.
         :return: The value read from the message, or the default value if the end was reached.
         """
         if self._at_end_of_buffer():
             return default_value
 
-        val = struct.unpack_from("<?", self.buffer, self.offset)[0]
         self.offset += 1
-        return val
+        return bool(int.from_bytes(self.buffer[self.offset - 1:self.offset], byteorder='little'))
 
     def read_int32(self, default_value: int = 0) -> int:
         """
         Read an integer value from the message buffer.
         :param default_value: Default value to use if the end of the message is reached.
         :return: The value read from the message, or the default value if the end was reached.
         """
         if self._at_end_of_buffer():
             return default_value
 
-        val = struct.unpack_from("<i", self.buffer, self.offset)[0]
         self.offset += 4
-        return val
+        return int.from_bytes(self.buffer[self.offset - 4:self.offset], byteorder='little')
 
     def read_float32(self, default_value: float = 0.0) -> float:
         """
         Read a float value from the message buffer.
         :param default_value: Default value to use if the end of the message is reached.
         :return: The value read from the message, or the default value if the end was reached.
         """
         if self._at_end_of_buffer():
             return default_value
 
-        val = struct.unpack_from("<f", self.buffer, self.offset)[0]
         self.offset += 4
-        return val
+        return struct.unpack('f', self.buffer[self.offset - 4:self.offset])[0]
 
     def read_float32_list(self, default_value: List[float] = None) -> List[float]:
         """
         Read a list of float values from the message buffer.
         :param default_value: Default value to use if the end of the message is reached.
         :return: The value read from the message, or the default value if the end was reached.
         """
@@ -74,20 +71,13 @@
         Read a string value from the message buffer.
         :param default_value: Default value to use if the end of the message is reached.
         :return: The value read from the message, or the default value if the end was reached.
         """
         if self._at_end_of_buffer():
             return default_value
 
-        encoded_str_len = self.read_int32()
-        val = self.buffer[self.offset : self.offset + encoded_str_len].decode("ascii")
-        self.offset += encoded_str_len
-        return val
-
-    def get_raw_bytes(self) -> bytes:
-        """
-        Get a copy of the internal bytes used by the message.
-        """
-        return bytearray(self.buffer)
+        count = self.read_int32()
+        self.offset += count
+        return self.buffer[self.offset - count:self.offset].decode('utf-8')
 
     def _at_end_of_buffer(self) -> bool:
         return self.offset >= len(self.buffer)
```

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/side_channel/outgoing_message.py` & `pyrfuniverse-0.9.10/pyrfuniverse/side_channel/outgoing_message.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 from typing import List
 import struct
 
-from pyrfuniverse.logging_util import get_logger
-
-logger = get_logger(__name__)
-
 
 class OutgoingMessage:
     """
     Utility class for forming the message that is written to a SideChannel.
     All data is written in little-endian format using the struct module.
     """
 
@@ -18,49 +14,37 @@
         """
         self.buffer = bytearray()
 
     def write_bool(self, b: bool) -> None:
         """
         Append a boolean value.
         """
-        self.buffer += struct.pack("<?", b)
+        self.buffer.extend(int(b).to_bytes(1, byteorder='little'))
 
     def write_int32(self, i: int) -> None:
         """
         Append an integer value.
         """
-        self.buffer += struct.pack("<i", i)
+        self.buffer.extend(i.to_bytes(4, byteorder='little'))
 
     def write_float32(self, f: float) -> None:
         """
         Append a float value. It will be truncated to 32-bit precision.
         """
-        self.buffer += struct.pack("<f", f)
+        self.buffer.extend(struct.pack('f', f))
 
     def write_float32_list(self, float_list: List[float]) -> None:
         """
         Append a list of float values. They will be truncated to 32-bit precision.
         """
         self.write_int32(len(float_list))
         for f in float_list:
             self.write_float32(f)
 
     def write_string(self, s: str) -> None:
         """
         Append a string value. Internally, it will be encoded to ascii, and the
         encoded length will also be written to the message.
         """
-        encoded_key = s.encode("ascii")
-        self.write_int32(len(encoded_key))
-        self.buffer += encoded_key
-
-    def set_raw_bytes(self, buffer: bytearray) -> None:
-        """
-        Set the internal buffer to a new bytearray. This will overwrite any existing data.
-        :param buffer:
-        :return:
-        """
-        if self.buffer:
-            logger.warning(
-                "Called set_raw_bytes but the message already has been written to. This will overwrite data."
-            )
-        self.buffer = bytearray(buffer)
+        s_byte = s.encode('utf-8')
+        self.write_int32(len(s_byte))
+        self.buffer.extend(s_byte)
```

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/utils/active_depth_generate.py` & `pyrfuniverse-0.9.10/pyrfuniverse/utils/active_depth_generate.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/utils/controller.py` & `pyrfuniverse-0.9.10/pyrfuniverse/utils/controller.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/utils/depth_processor.py` & `pyrfuniverse-0.9.10/pyrfuniverse/utils/depth_processor.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 import random
 
 import numpy as np
 import open3d as o3d
 import cv2
 import tempfile
 
-def image_bytes_to_point_cloud(rgb_bytes: bytes, depth_bytes: bytes, fov: float, extrinsic_matrix: np.ndarray):
+def image_bytes_to_point_cloud(rgb_bytes: bytes, depth_bytes: bytes, fov: float, local_to_world_matrix: np.ndarray):
     """
     Use the raw bytes of RGB image and depth image, as well as the camera
     FOV and extrinsic matrix to generate point cloud in global coordinate.
 
     Args:
         rgb_bytes: Bytes, raw bytes of RGB image.
         depth_bytes: Bytes, raw bytes of depth image.
         fov: Float, camera Field Of View (FOV).
-        extrinsic_matrix: Numpy.ndarray, the extrinsic matrix of camera.
+        local_to_world_matrix: Numpy.ndarray, the local_to_world_matrix of camera.
     
     Return:
         open3d.geometry.PointCloud: The point cloud.
     """
     image_rgb = np.frombuffer(rgb_bytes, dtype=np.uint8)
     image_rgb = cv2.imdecode(image_rgb, cv2.IMREAD_COLOR)
     image_rgb = cv2.cvtColor(image_rgb, cv2.COLOR_BGR2RGB)
@@ -31,40 +31,40 @@
     with open(temp_file_path, 'wb') as f:
         f.write(depth_bytes)
     image_depth = cv2.imread(temp_file_path, cv2.IMREAD_UNCHANGED)
     os.remove(temp_file_path)
 
     image_depth = np.transpose(image_depth, [1, 0])
 
-    pcd = image_array_to_point_cloud(image_rgb, image_depth, fov, extrinsic_matrix)
+    pcd = image_array_to_point_cloud(image_rgb, image_depth, fov, local_to_world_matrix)
     return pcd
 
 
-def image_array_to_point_cloud(image_rgb: np.ndarray, image_depth: np.ndarray, fov: float, extrinsic_matrix: np.ndarray):
+def image_array_to_point_cloud(image_rgb: np.ndarray, image_depth: np.ndarray, fov: float, local_to_world_matrix: np.ndarray):
     """
     Use the RGB image and depth image, as well as the camera
     FOV and extrinsic matrix to generate point cloud in global coordinate.
 
     Args:
         image_rgb: Numpy.ndarray, in shape (H,W,3), the RGB image.
         image_depth: Numpy.ndarray, in shape (H,W,3), the depth image.
         fov: Float, camera Field Of View (FOV).
-        extrinsic_matrix: Numpy.ndarray, the extrinsic matrix of camera.
+        local_to_world_matrix: Numpy.ndarray, the local_to_world_matrix of camera.
     
     Return:
         open3d.geometry.PointCloud: The point cloud.
     """
     points = depth_to_point_cloud(image_depth, fov=fov, organized=False)
     pcd = o3d.geometry.PointCloud()
     pcd.points = o3d.utility.Vector3dVector(points)
 
     colors = image_rgb.reshape(-1, 3)
     pcd.colors = o3d.utility.Vector3dVector(colors.astype(np.float32) / 255.0)
 
-    pcd.transform(extrinsic_matrix)
+    pcd.transform(local_to_world_matrix)
 
     return pcd
 
 def depth_to_point_cloud(depth: np.ndarray, fov: float, organized=False):
     """
     Use the depth image and the camera FOV to generate point cloud in
     camera coordinate.
@@ -102,24 +102,24 @@
 
     cloud = np.stack([points_x, -points_y, points_z], axis=-1)
     if not organized:
         cloud = cloud.reshape([-1, 3])
 
     return cloud
 
-def image_bytes_to_point_cloud_intrinsic_matrix(rgb_bytes: bytes, depth_bytes: bytes, intrinsic_matrix: np.ndarray, extrinsic_matrix: np.ndarray):
+def image_bytes_to_point_cloud_intrinsic_matrix(rgb_bytes: bytes, depth_bytes: bytes, intrinsic_matrix: np.ndarray, local_to_world_matrix: np.ndarray):
     """
     Use the raw bytes of RGB image and depth image, as well as the camera
     intrinsic matrix and extrinsic matrix to generate point cloud in global coordinate.
 
     Args:
         rgb_bytes: Bytes, raw bytes of RGB image.
         depth_bytes: Bytes, raw bytes of depth image.
         intrinsic_matrix: Numpy.ndarray, the intrinsic matrix of camera.
-        extrinsic_matrix: Numpy.ndarray, the extrinsic matrix of camera.
+        local_to_world_matrix: Numpy.ndarray, the local_to_world_matrix of camera.
     
     Return:
         open3d.geometry.PointCloud: The point cloud.
     """
     temp_file_path = osp.join(tempfile.gettempdir(), f'temp_img_{int(random.uniform(10000000,99999999))}.png')
     with open(temp_file_path, 'wb') as f:
         f.write(rgb_bytes)
@@ -137,29 +137,29 @@
     depth_png = (depth_exr * 1000).astype(np.uint16)[:, :]
     # foreground_depth_png[~foregound_mask] = 0  # filter the background, only need foreground
     temp_file_path = osp.join(tempfile.gettempdir(), f'temp_img_{int(random.uniform(10000000,99999999))}.png')
     cv2.imwrite(temp_file_path, depth_png)
     depth = o3d.io.read_image(temp_file_path)
     os.remove(temp_file_path)
 
-    pcd = image_open3d_to_point_cloud_intrinsic_matrix(color, depth, intrinsic_matrix, extrinsic_matrix)
+    pcd = image_open3d_to_point_cloud_intrinsic_matrix(color, depth, intrinsic_matrix, local_to_world_matrix)
 
     return pcd
 
 
-def image_array_to_point_cloud_intrinsic_matrix(image_rgb: np.ndarray, image_depth: np.ndarray, intrinsic_matrix: np.ndarray, extrinsic_matrix: np.ndarray):
+def image_array_to_point_cloud_intrinsic_matrix(image_rgb: np.ndarray, image_depth: np.ndarray, intrinsic_matrix: np.ndarray, local_to_world_matrix: np.ndarray):
     """
     Use the RGB image and depth image, as well as the camera
     intrinsic matrix and extrinsic matrix to generate point cloud in global coordinate.
 
     Args:
         image_rgb: Numpy.ndarray, in shape (H,W,3), the RGB image.
         image_depth: Numpy.ndarray, in shape (H,W,3), the depth image.
         intrinsic_matrix: Numpy.ndarray, the intrinsic matrix of camera.
-        extrinsic_matrix: Numpy.ndarray, the extrinsic matrix of camera.
+        local_to_world_matrix: Numpy.ndarray, the local_to_world_matrix of camera.
     
     Return:
         open3d.geometry.PointCloud: The point cloud.
     """
     temp_file_path = osp.join(tempfile.gettempdir(), f'temp_img_{int(random.uniform(10000000,99999999))}.png')
 
     image_rgb = np.transpose(image_rgb, [1, 0, 2])
@@ -171,28 +171,28 @@
     depth_png = (image_depth * 1000).astype(np.uint16)[:, :]
     depth_png = np.transpose(depth_png, [1, 0])
     cv2.imwrite(temp_file_path, depth_png)
     depth = o3d.io.read_image(temp_file_path)
 
     os.remove(temp_file_path)
 
-    pcd = image_open3d_to_point_cloud_intrinsic_matrix(color, depth, intrinsic_matrix, extrinsic_matrix)
+    pcd = image_open3d_to_point_cloud_intrinsic_matrix(color, depth, intrinsic_matrix, local_to_world_matrix)
 
     return pcd
 
-def image_open3d_to_point_cloud_intrinsic_matrix(color: o3d.geometry.Image, depth: o3d.geometry.Image, intrinsic_matrix: np.ndarray, extrinsic_matrix: np.ndarray):
+def image_open3d_to_point_cloud_intrinsic_matrix(color: o3d.geometry.Image, depth: o3d.geometry.Image, intrinsic_matrix: np.ndarray, local_to_world_matrix: np.ndarray):
     """
     Use the RGB image and depth image in open3d.geometry.Image format, as well as the camera
     intrinsic matrix and extrinsic matrix to generate point cloud in global coordinate.
 
     Args:
         color: open3d.geometry.Image, the RGB image.
         depth: open3d.geometry.Image, the depth image.
         intrinsic_matrix: Numpy.ndarray, the intrinsic matrix of camera.
-        extrinsic_matrix: Numpy.ndarray, the extrinsic matrix of camera.
+        local_to_world_matrix: Numpy.ndarray, the local_to_world_matrix of camera.
     
     Return:
         open3d.geometry.PointCloud: The point cloud.
     """
     rgbd_image = o3d.geometry.RGBDImage.create_from_color_and_depth(
         color, depth, depth_trunc=20, convert_rgb_to_intensity=False)
 
@@ -204,15 +204,15 @@
     pcd = o3d.geometry.PointCloud.create_from_rgbd_image(
         rgbd_image, intrinsic_matrix, project_valid_depth_only=False)
 
     # convter to unity space
     pcd.transform([[1, 0, 0, 0], [0, -1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]])
 
     # camera to world in unity space
-    pcd.transform(extrinsic_matrix)
+    pcd.transform(local_to_world_matrix)
 
     return pcd
 
 def mask_point_cloud_with_id_color(pcd: o3d.geometry.PointCloud, image_mask: np.ndarray, color:list):
     """
     Mask the point cloud with given segmentation masks and target color.
```

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/utils/interpolate_utils.py` & `pyrfuniverse-0.9.10/pyrfuniverse/utils/interpolate_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pyrfuniverse.envs import RFUniverseBaseEnv
+from pyrfuniverse.envs.base_env import RFUniverseBaseEnv
 import numpy as np
 import math
 
 
 def average_interpolate_with_max_step_length(start: np.ndarray, terminal: np.ndarray, max_step_length):
     assert start.shape == terminal.shape
     distance = terminal - start
```

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/utils/jaco_controller.py` & `pyrfuniverse-0.9.10/pyrfuniverse/utils/jaco_controller.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/utils/kinova_controller.py` & `pyrfuniverse-0.9.10/pyrfuniverse/utils/kinova_controller.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/utils/os_utils.py` & `pyrfuniverse-0.9.10/pyrfuniverse/utils/os_utils.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/utils/rfuniverse_utility.py` & `pyrfuniverse-0.9.10/pyrfuniverse/utils/rfuniverse_utility.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/utils/stretch_controller.py` & `pyrfuniverse-0.9.10/pyrfuniverse/utils/stretch_controller.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/utils/tobor_controller.py` & `pyrfuniverse-0.9.10/pyrfuniverse/utils/tobor_controller.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.5/pyrfuniverse/utils/ur5_controller.py` & `pyrfuniverse-0.9.10/pyrfuniverse/utils/ur5_controller.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.5/test/test_active_depth.py` & `pyrfuniverse-0.9.10/test/test_active_depth.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,102 +1,106 @@
 import os
 os.environ["OPENCV_IO_ENABLE_OPENEXR"] = "1"
 import cv2
 import numpy as np
 try:
     import open3d as o3d
 except ImportError:
-    print('This feature requires open3d, please install with `pip install open3d`')
-    raise
+    raise Exception('This feature requires open3d, please install with `pip install open3d`')
 import pyrfuniverse.utils.rfuniverse_utility as utility
 import pyrfuniverse.utils.depth_processor as dp
 from pyrfuniverse.envs.base_env import RFUniverseBaseEnv
 
-env = RFUniverseBaseEnv(scene_file='ActiveDepth.json')
-
-active_light_sensor_1 = env.GetAttr(789789)
 
-main_intrinsic_matrix = [600, 0, 0, 0, 600, 0, 240, 240, 1]
-ir_intrinsic_matrix = [480, 0, 0, 0, 480, 0, 240, 240, 1]
+nd_main_intrinsic_matrix = np.array([[600, 0, 240],
+                                     [0, 600, 240],
+                                     [0, 0, 1]])
+nd_ir_intrinsic_matrix = np.array([[480, 0, 240],
+                                   [0, 480, 240],
+                                   [0, 0, 1]])
 
-nd_main_intrinsic_matrix = np.reshape(main_intrinsic_matrix, [3, 3]).T
+env = RFUniverseBaseEnv(scene_file='ActiveDepth.json')
+active_light_sensor_1 = env.GetAttr(789789)
 
-active_light_sensor_1.GetRGB(intrinsic_matrix=main_intrinsic_matrix)
+active_light_sensor_1.GetRGB(intrinsic_matrix=nd_main_intrinsic_matrix)
 env.step()
 image_byte = active_light_sensor_1.data['rgb']
 image_rgb = np.frombuffer(image_byte, dtype=np.uint8)
 image_rgb = cv2.imdecode(image_rgb, cv2.IMREAD_COLOR)
 image_rgb = cv2.cvtColor(image_rgb, cv2.COLOR_BGR2RGB)
 image_rgb = np.transpose(image_rgb, [1, 0, 2])
 
-active_light_sensor_1.GetID(intrinsic_matrix=main_intrinsic_matrix)
+active_light_sensor_1.GetID(intrinsic_matrix=nd_main_intrinsic_matrix)
 env.step()
 image_id = active_light_sensor_1.data['id_map']
 image_id = np.frombuffer(image_id, dtype=np.uint8)
 image_id = cv2.imdecode(image_id, cv2.IMREAD_COLOR)
 image_id = cv2.cvtColor(image_id, cv2.COLOR_BGR2RGB)
 
-active_light_sensor_1.GetDepthEXR(intrinsic_matrix=main_intrinsic_matrix)
+active_light_sensor_1.GetDepthEXR(intrinsic_matrix=nd_main_intrinsic_matrix)
 env.step()
 image_depth_exr = active_light_sensor_1.data['depth_exr']
 
-active_light_sensor_1.GetActiveDepth(main_intrinsic_matrix_local = main_intrinsic_matrix, ir_intrinsic_matrix_local = ir_intrinsic_matrix)
+active_light_sensor_1.GetActiveDepth(main_intrinsic_matrix_local=nd_main_intrinsic_matrix,
+                                     ir_intrinsic_matrix_local=nd_ir_intrinsic_matrix)
 env.step()
 image_active_depth = active_light_sensor_1.data['active_depth']
 image_active_depth = np.transpose(image_active_depth, [1, 0])
 
 local_to_world_matrix = active_light_sensor_1.data['local_to_world_matrix']
-local_to_world_matrix = np.reshape(local_to_world_matrix, [4, 4]).T
+# local_to_world_matrix = np.reshape(local_to_world_matrix, [4, 4]).T
 
 # point = dp.image_array_to_point_cloud(image_rgb, image_active_depth, 45, local_to_world_matrix)
 
 color = utility.EncodeIDAsColor(568451)[0:3]
 real_point_cloud1 = dp.image_bytes_to_point_cloud_intrinsic_matrix(image_byte, image_depth_exr, nd_main_intrinsic_matrix, local_to_world_matrix)
 real_point_cloud1 = dp.mask_point_cloud_with_id_color(real_point_cloud1, image_id, color)
 active_point_cloud1 = dp.image_array_to_point_cloud_intrinsic_matrix(image_rgb, image_active_depth, nd_main_intrinsic_matrix, local_to_world_matrix)
 active_point_cloud1 = dp.mask_point_cloud_with_id_color(active_point_cloud1, image_id, color)
 filtered_point_cloud1 = dp.filter_active_depth_point_cloud_with_exact_depth_point_cloud(active_point_cloud1, real_point_cloud1)
 
 ##################################################
 
 active_light_sensor_2 = env.GetAttr(123123)
 
-active_light_sensor_2.GetRGB(intrinsic_matrix=main_intrinsic_matrix)
+active_light_sensor_2.GetRGB(intrinsic_matrix=nd_main_intrinsic_matrix)
 env.step()
 image_byte = active_light_sensor_2.data['rgb']
 image_rgb = np.frombuffer(image_byte, dtype=np.uint8)
 image_rgb = cv2.imdecode(image_rgb, cv2.IMREAD_COLOR)
 image_rgb = cv2.cvtColor(image_rgb, cv2.COLOR_BGR2RGB)
 image_rgb = np.transpose(image_rgb, [1, 0, 2])
 
-active_light_sensor_2.GetID(intrinsic_matrix=main_intrinsic_matrix)
+active_light_sensor_2.GetID(intrinsic_matrix=nd_main_intrinsic_matrix)
 env.step()
 image_id = active_light_sensor_2.data['id_map']
 image_id = np.frombuffer(image_id, dtype=np.uint8)
 image_id = cv2.imdecode(image_id, cv2.IMREAD_COLOR)
 image_id = cv2.cvtColor(image_id, cv2.COLOR_BGR2RGB)
 
-active_light_sensor_2.GetDepthEXR(intrinsic_matrix=main_intrinsic_matrix)
+active_light_sensor_2.GetDepthEXR(intrinsic_matrix=nd_main_intrinsic_matrix)
 env.step()
-image_depth_exr = env.instance_channel.data[123123]['depth_exr']
+image_depth_exr = active_light_sensor_2.data['depth_exr']
 
-active_light_sensor_2.GetActiveDepth(main_intrinsic_matrix_local = main_intrinsic_matrix, ir_intrinsic_matrix_local = ir_intrinsic_matrix)
+active_light_sensor_2.GetActiveDepth(main_intrinsic_matrix_local=nd_main_intrinsic_matrix,
+                                     ir_intrinsic_matrix_local=nd_ir_intrinsic_matrix)
 env.step()
 image_active_depth = active_light_sensor_2.data['active_depth']
 image_active_depth = np.transpose(image_active_depth, [1, 0])
 
 local_to_world_matrix = active_light_sensor_2.data['local_to_world_matrix']
-local_to_world_matrix = np.reshape(local_to_world_matrix, [4, 4]).T
 
 env.close()
 
 # point = dp.image_array_to_point_cloud(image_rgb, image_active_depth, 45, local_to_world_matrix)
-real_point_cloud2 = dp.image_bytes_to_point_cloud_intrinsic_matrix(image_byte, image_depth_exr, nd_main_intrinsic_matrix, local_to_world_matrix)
+real_point_cloud2 = dp.image_bytes_to_point_cloud_intrinsic_matrix(image_byte, image_depth_exr,
+                                                                   nd_main_intrinsic_matrix, local_to_world_matrix)
 real_point_cloud2 = dp.mask_point_cloud_with_id_color(real_point_cloud2, image_id, color)
-active_point_cloud2 = dp.image_array_to_point_cloud_intrinsic_matrix(image_rgb, image_active_depth, nd_main_intrinsic_matrix, local_to_world_matrix)
+active_point_cloud2 = dp.image_array_to_point_cloud_intrinsic_matrix(image_rgb, image_active_depth,
+                                                                     nd_main_intrinsic_matrix, local_to_world_matrix)
 active_point_cloud2 = dp.mask_point_cloud_with_id_color(active_point_cloud2, image_id, color)
 filtered_point_cloud2 = dp.filter_active_depth_point_cloud_with_exact_depth_point_cloud(active_point_cloud2, real_point_cloud2)
 
 # unity space to open3d space and show
 real_point_cloud1.transform([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]])
 real_point_cloud2.transform([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]])
 active_point_cloud1.transform([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]])
```

### Comparing `pyrfuniverse-0.8.5/test/test_articulation_ik.py` & `pyrfuniverse-0.9.10/test/test_articulation_ik.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.5/test/test_camera_image.py` & `pyrfuniverse-0.9.10/test/test_camera_image.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from pyrfuniverse.envs.base_env import RFUniverseBaseEnv
 import pyrfuniverse.attributes as attr
 import cv2
 import numpy as np
 
-env = RFUniverseBaseEnv(assets=['Camera'])
+env = RFUniverseBaseEnv(assets=['Camera', 'GameObject_Box'])
 
 camera = env.InstanceObject(name='Camera', id=123456, attr_type=attr.CameraAttr)
+box = env.InstanceObject(name='GameObject_Box', attr_type=attr.GameObjectAttr)
+box.SetTransform(position=[0, 0.05, 0.5], scale=[0.1, 0.1, 0.1])
+box.SetColor([1, 0, 0, 1])
 camera.SetTransform(position=[0, 0.25, 0], rotation=[30, 0, 0])
 camera.GetDepth(width=512, height=512, zero_dis=1, one_dis=5)
 camera.GetDepthEXR(width=512, height=512)
 camera.GetRGB(width=512, height=512)
 env.step()
 print(camera.data['depth'])
 print(camera.data['depth_exr'])
 print(camera.data['rgb'])
-image_np = np.frombuffer(camera.data['rgb'], dtype=np.uint8)
-image_np = cv2.imdecode(image_np, cv2.IMREAD_COLOR)
-print(image_np.shape)
+image = np.frombuffer(camera.data['rgb'], dtype=np.uint8)
+image = cv2.imdecode(image, cv2.IMREAD_COLOR)
+print(image.shape)
 env.close()
-cv2.imshow("rgb", image_np)
+cv2.imshow("rgb", image)
 cv2.waitKey(0)
```

### Comparing `pyrfuniverse-0.8.5/test/test_debug.py` & `pyrfuniverse-0.9.10/test/test_debug.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.5/test/test_grasp_pose.py` & `pyrfuniverse-0.9.10/test/test_grasp_pose.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.5/test/test_grasp_sim.py` & `pyrfuniverse-0.9.10/test/test_grasp_sim.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 import os
 import numpy as np
-
 try:
     import pandas as pd
 except ImportError:
-    print('This feature requires pandas, please install with `pip install pandas`')
-    raise
+    raise Exception('This feature requires pandas, please install with `pip install pandas`')
 try:
     import open3d as o3d
 except ImportError:
-    print('This feature requires open3d, please install with `pip install open3d`')
-    raise
+    raise Exception('This feature requires open3d, please install with `pip install open3d`')
 from pyrfuniverse.envs.base_env import RFUniverseBaseEnv
 import pyrfuniverse.attributes as attr
 
 
 def get_grasp_pose(file: str, points_count, scale: float = 1):
     mesh = o3d.io.read_triangle_mesh(file)
     mesh.scale(scale, np.array([0, 0, 0]))
@@ -60,15 +57,17 @@
 
 points = grasp_sim.data['points']
 points = np.array(points).reshape([-1, 3])
 quaternions = grasp_sim.data['quaternions']
 quaternions = np.array(quaternions).reshape([-1, 4])
 width = grasp_sim.data['width']
 width = np.array(width).reshape([-1, 1])
-print(points.shape)
+
+env.close()
+
 data = np.concatenate((points, quaternions, width), axis=1)
 csv = pd.DataFrame(data, columns=['x', 'y', 'z', 'qx', 'qy', 'qz', 'qw', 'width'])
 
 csv_path = os.path.join(os.path.dirname(mesh_path), 'grasps_rfu.csv')
 csv.to_csv(csv_path, index=True, header=True)
 
 env.Pend()
```

### Comparing `pyrfuniverse-0.8.5/test/test_heat_map.py` & `pyrfuniverse-0.9.10/test/test_heat_map.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.5/test/test_humanbody_ik.py` & `pyrfuniverse-0.9.10/test/test_humanbody_ik.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.5/test/test_label.py` & `pyrfuniverse-0.9.10/test/test_label.py`

 * *Files 22% similar despite different names*

```diff
@@ -47,18 +47,18 @@
 id_map = np.frombuffer(camera.data['id_map'], dtype=np.uint8)
 id_map = cv2.imdecode(id_map, cv2.IMREAD_COLOR)
 
 print('2d_bounding_box:')
 for i in camera.data['2d_bounding_box']:
     print(i)
     print(camera.data['2d_bounding_box'][i])
-    position = camera.data['2d_bounding_box'][i]['position']
-    size = camera.data['2d_bounding_box'][i]['size']
-    tl_point = (int(position[0] + size[0]/2), int(512 - position[1] + size[1]/2))
-    br_point = (int(position[0] - size[0]/2), int(512 - position[1] - size[1]/2))
+    center = camera.data['2d_bounding_box'][i][0:2]
+    size = camera.data['2d_bounding_box'][i][2:4]
+    tl_point = (int(center[0] + size[0] / 2), int(512 - center[1] + size[1] / 2))
+    br_point = (int(center[0] - size[0] / 2), int(512 - center[1] - size[1] / 2))
     cv2.rectangle(id_map, tl_point, br_point, (255, 255, 255), 1)
 
 #3d_bounding_box
 print('3d_bounding_box:')
 for i in camera.data['3d_bounding_box']:
     print(i)
     print(camera.data['3d_bounding_box'][i])
```

### Comparing `pyrfuniverse-0.8.5/test/test_light.py` & `pyrfuniverse-0.9.10/test/test_light.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.5/test/test_load_mesh.py` & `pyrfuniverse-0.9.10/test/test_load_mesh.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.5/test/test_load_urdf.py` & `pyrfuniverse-0.9.10/test/test_load_urdf.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 
 ur5 = env.LoadURDF(path=os.path.abspath('../URDF/UR5/ur5_robot.urdf'), native_ik=True)
 ur5.SetTransform(position=[1, 0, 0])
 yumi = env.LoadURDF(path=os.path.abspath('../URDF/yumi_description/urdf/yumi.urdf'), native_ik=False)
 yumi.SetTransform(position=[2, 0, 0])
 kinova = env.LoadURDF(path=os.path.abspath('../URDF/kinova_gen3/GEN3_URDF_V12.urdf'), native_ik=False)
 kinova.SetTransform(position=[3, 0, 0])
+env.step()
 
 ur5.IKTargetDoMove(position=[0, 0.5, 0], duration=0.1, relative=True)
 env.step()
 ur5.WaitDo()
 ur5.IKTargetDoMove(position=[0, 0, -0.5], duration=0.1, relative=True)
 env.step()
 ur5.WaitDo()
 ur5.IKTargetDoMove(position=[0, -0.2, 0.3], duration=0.1, relative=True)
 ur5.IKTargetDoRotateQuaternion(quaternion=utility.UnityEularToQuaternion([0, 90, 0]), duration=30, relative=True)
 env.step()
 ur5.WaitDo()
 
-while 1:
-    env.step()
+env.Pend()
```

### Comparing `pyrfuniverse-0.8.5/test/test_ompl.py` & `pyrfuniverse-0.9.10/test/test_ompl.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from pyrfuniverse.envs.base_env import RFUniverseBaseEnv
 import pyrfuniverse.attributes as attr
-import pyrfuniverse.attributes.omplmanager_attr as rfu_ompl
+try:
+    import pyrfuniverse.attributes.omplmanager_attr as rfu_ompl
+except ImportError:
+    raise Exception('This feature requires ompl, see: https://github.com/ompl/ompl')
 
 env = RFUniverseBaseEnv(assets=['franka_panda', 'Collider_Box', 'OmplManager'])
 
 robot = env.InstanceObject(name='franka_panda', id=123456, attr_type=attr.ControllerAttr)
 robot.EnabledNativeIK(False)
 box1 = env.InstanceObject(name='Collider_Box', id=111111, attr_type=attr.ColliderAttr)
 box1.SetTransform(position=[-0.5, 0.5, 0], scale=[0.2, 1, 0.2])
```

### Comparing `pyrfuniverse-0.8.5/test/test_pick_and_place.py` & `pyrfuniverse-0.9.10/test/test_pick_and_place.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.5/test/test_pick_and_place_flexiv.py` & `pyrfuniverse-0.9.10/test/test_pick_and_place_flexiv.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.5/test/test_point_cloud.py` & `pyrfuniverse-0.9.10/test/test_point_cloud.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,43 +1,40 @@
 import os
 os.environ["OPENCV_IO_ENABLE_OPENEXR"] = "1"
 from pyrfuniverse.envs.base_env import RFUniverseBaseEnv
 import pyrfuniverse.utils.depth_processor as dp
-import numpy as np
 try:
     import open3d as o3d
 except ImportError:
-    print('This feature requires open3d, please install with `pip install open3d`')
-    raise
+    raise Exception('This feature requires open3d, please install with `pip install open3d`')
 
 env = RFUniverseBaseEnv(scene_file='PointCloud.json')
 camera1 = env.GetAttr(698548)
 camera1.GetDepthEXR(width=1920, height=1080)
 camera1.GetRGB(width=1920, height=1080)
 camera1.GetID(width=1920, height=1080)
 env.step()
 
 image_rgb = camera1.data['rgb']
 image_depth_exr = camera1.data['depth_exr']
 fov = camera1.data['fov']
 local_to_world_matrix = camera1.data['local_to_world_matrix']
-local_to_world_matrix = np.reshape(local_to_world_matrix, [4, 4]).T
 point1 = dp.image_bytes_to_point_cloud(image_rgb, image_depth_exr, fov, local_to_world_matrix)
 
 camera2 = env.GetAttr(698550)
 camera2.GetDepthEXR(width=1920, height=1080)
 camera2.GetRGB(width=1920, height=1080)
 camera2.GetID(width=1920, height=1080)
 env.step()
 
 image_rgb = camera2.data['rgb']
 image_depth_exr = camera2.data['depth_exr']
 fov = camera2.data['fov']
 local_to_world_matrix = camera2.data['local_to_world_matrix']
-local_to_world_matrix = np.reshape(local_to_world_matrix, [4, 4]).T
+# local_to_world_matrix = np.reshape(local_to_world_matrix, [4, 4]).T
 point2 = dp.image_bytes_to_point_cloud(image_rgb, image_depth_exr, fov, local_to_world_matrix)
 
 env.close()
 
 # unity space to open3d space and show
 point1.transform([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]])
 point2.transform([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]])
```

### Comparing `pyrfuniverse-0.8.5/test/test_point_cloud_with_intrinsic_matrix.py` & `pyrfuniverse-0.9.10/test/test_point_cloud_with_intrinsic_matrix.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,44 +2,41 @@
 os.environ["OPENCV_IO_ENABLE_OPENEXR"] = "1"
 from pyrfuniverse.envs.base_env import RFUniverseBaseEnv
 import pyrfuniverse.utils.depth_processor as dp
 import numpy as np
 try:
     import open3d as o3d
 except ImportError:
-    print('This feature requires open3d, please install with `pip install open3d`')
-    raise
+    raise Exception('This feature requires open3d, please install with `pip install open3d`')
 
 env = RFUniverseBaseEnv(scene_file='PointCloud.json')
 
-intrinsic_matrix = [960, 0, 0, 0, 960, 0, 960, 540, 1]
-nd_intrinsic_matrix = np.reshape(intrinsic_matrix, [3, 3]).T
-
+nd_intrinsic_matrix = np.array([[960, 0, 960],
+                            [0, 960, 540],
+                            [0, 0, 1]])
 camera1 = env.GetAttr(698548)
-camera1.GetDepthEXR(intrinsic_matrix=intrinsic_matrix)
-camera1.GetRGB(intrinsic_matrix=intrinsic_matrix)
-camera1.GetID(intrinsic_matrix=intrinsic_matrix)
+camera1.GetDepthEXR(intrinsic_matrix=nd_intrinsic_matrix)
+camera1.GetRGB(intrinsic_matrix=nd_intrinsic_matrix)
+camera1.GetID(intrinsic_matrix=nd_intrinsic_matrix)
 env.step()
 
 image_rgb = camera1.data['rgb']
 image_depth_exr = camera1.data['depth_exr']
 local_to_world_matrix = camera1.data['local_to_world_matrix']
-local_to_world_matrix = np.reshape(local_to_world_matrix, [4, 4]).T
 point1 = dp.image_bytes_to_point_cloud_intrinsic_matrix(image_rgb, image_depth_exr, nd_intrinsic_matrix, local_to_world_matrix)
 
 camera2 = env.GetAttr(698550)
-camera2.GetDepthEXR(intrinsic_matrix=intrinsic_matrix)
-camera2.GetRGB(intrinsic_matrix=intrinsic_matrix)
-camera2.GetID(intrinsic_matrix=intrinsic_matrix)
+camera2.GetDepthEXR(intrinsic_matrix=nd_intrinsic_matrix)
+camera2.GetRGB(intrinsic_matrix=nd_intrinsic_matrix)
+camera2.GetID(intrinsic_matrix=nd_intrinsic_matrix)
 env.step()
 
 image_rgb = camera2.data['rgb']
 image_depth_exr = camera2.data['depth_exr']
 local_to_world_matrix = camera2.data['local_to_world_matrix']
-local_to_world_matrix = np.reshape(local_to_world_matrix, [4, 4]).T
 point2 = dp.image_bytes_to_point_cloud_intrinsic_matrix(image_rgb, image_depth_exr, nd_intrinsic_matrix, local_to_world_matrix)
 env.close()
 
 # unity space to open3d space and show
 point1.transform([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]])
 point2.transform([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]])
 coorninate = o3d.geometry.TriangleMesh.create_coordinate_frame()
```

### Comparing `pyrfuniverse-0.8.5/test/test_save_gripper.py` & `pyrfuniverse-0.9.10/test/test_save_gripper.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.5/test/test_scene.py` & `pyrfuniverse-0.9.10/test/test_scene.py`

 * *Files identical despite different names*

### Comparing `pyrfuniverse-0.8.5/test/test_tobor_move.py` & `pyrfuniverse-0.9.10/test/test_tobor_move.py`

 * *Files identical despite different names*

