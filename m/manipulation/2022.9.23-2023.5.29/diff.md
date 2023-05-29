# Comparing `tmp/manipulation-2022.9.23.tar.gz` & `tmp/manipulation-2023.5.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manipulation-2022.9.23.tar", last modified: Sat Sep 24 01:11:05 2022, max compression
+gzip compressed data, was "manipulation-2023.5.29.tar", last modified: Mon May 29 21:26:51 2023, max compression
```

## Comparing `manipulation-2022.9.23.tar` & `manipulation-2023.5.29.tar`

### file list

```diff
@@ -1,93 +1,116 @@
-drwxr-xr-x   0 russt      (504) staff       (20)        0 2022-09-24 01:11:05.166964 manipulation-2022.9.23/
--rw-r--r--   0 russt      (504) staff       (20)     1561 2022-07-31 19:35:30.000000 manipulation-2022.9.23/LICENSE.TXT
--rw-r--r--   0 russt      (504) staff       (20)       91 2022-01-04 11:46:53.000000 manipulation-2022.9.23/MANIFEST.in
--rw-r--r--   0 russt      (504) staff       (20)      971 2022-09-24 01:11:05.167165 manipulation-2022.9.23/PKG-INFO
--rw-r--r--   0 russt      (504) staff       (20)      466 2022-07-31 19:35:30.000000 manipulation-2022.9.23/README.md
-drwxr-xr-x   0 russt      (504) staff       (20)        0 2022-09-24 01:11:05.146342 manipulation-2022.9.23/manipulation/
--rw-r--r--   0 russt      (504) staff       (20)      142 2022-02-27 02:09:05.000000 manipulation-2022.9.23/manipulation/__init__.py
--rw-r--r--   0 russt      (504) staff       (20)    11087 2022-01-04 12:29:33.000000 manipulation-2022.9.23/manipulation/drake_gym.py
-drwxr-xr-x   0 russt      (504) staff       (20)        0 2022-09-24 01:11:05.147496 manipulation-2022.9.23/manipulation/envs/
--rw-r--r--   0 russt      (504) staff       (20)     9661 2022-06-13 23:12:21.000000 manipulation-2022.9.23/manipulation/envs/box_flipup.py
-drwxr-xr-x   0 russt      (504) staff       (20)        0 2022-09-24 01:11:05.147806 manipulation-2022.9.23/manipulation/exercises/
-drwxr-xr-x   0 russt      (504) staff       (20)        0 2022-09-24 01:11:05.148751 manipulation-2022.9.23/manipulation/exercises/clutter/
--rw-r--r--   0 russt      (504) staff       (20)     1707 2021-12-11 10:12:32.000000 manipulation-2022.9.23/manipulation/exercises/clutter/test_analytic_grasp.py
--rw-r--r--   0 russt      (504) staff       (20)     6413 2022-09-21 09:42:38.000000 manipulation-2022.9.23/manipulation/exercises/clutter/test_grasp_candidate.py
--rw-r--r--   0 russt      (504) staff       (20)     1740 2022-09-21 09:42:38.000000 manipulation-2022.9.23/manipulation/exercises/clutter/test_normal.py
-drwxr-xr-x   0 russt      (504) staff       (20)        0 2022-09-24 01:11:05.149006 manipulation-2022.9.23/manipulation/exercises/force/
--rw-r--r--   0 russt      (504) staff       (20)     1536 2022-06-12 12:50:14.000000 manipulation-2022.9.23/manipulation/exercises/force/test_hybrid.py
--rw-r--r--   0 russt      (504) staff       (20)     4827 2022-02-25 20:04:09.000000 manipulation-2022.9.23/manipulation/exercises/grader.py
-drwxr-xr-x   0 russt      (504) staff       (20)        0 2022-09-24 01:11:05.150436 manipulation-2022.9.23/manipulation/exercises/pick/
--rw-r--r--   0 russt      (504) staff       (20)     1185 2021-12-11 10:12:32.000000 manipulation-2022.9.23/manipulation/exercises/pick/plot_planar_manipulator.py
--rw-r--r--   0 russt      (504) staff       (20)    16008 2021-12-11 10:12:32.000000 manipulation-2022.9.23/manipulation/exercises/pick/test_differential_ik.py
--rw-r--r--   0 russt      (504) staff       (20)     3571 2021-12-11 10:12:32.000000 manipulation-2022.9.23/manipulation/exercises/pick/test_planar_manipulator.py
--rw-r--r--   0 russt      (504) staff       (20)     2957 2021-12-11 10:12:32.000000 manipulation-2022.9.23/manipulation/exercises/pick/test_rigid_transforms.py
--rw-r--r--   0 russt      (504) staff       (20)     2030 2021-12-11 10:12:32.000000 manipulation-2022.9.23/manipulation/exercises/pick/test_robot_painter.py
--rw-r--r--   0 russt      (504) staff       (20)     1019 2021-12-11 10:12:32.000000 manipulation-2022.9.23/manipulation/exercises/pick/test_simple_qp.py
-drwxr-xr-x   0 russt      (504) staff       (20)        0 2022-09-24 01:11:05.151055 manipulation-2022.9.23/manipulation/exercises/pose/
--rw-r--r--   0 russt      (504) staff       (20)     3501 2022-09-21 09:42:38.000000 manipulation-2022.9.23/manipulation/exercises/pose/test_icp.py
--rw-r--r--   0 russt      (504) staff       (20)     2447 2022-09-21 09:42:38.000000 manipulation-2022.9.23/manipulation/exercises/pose/test_pose_estimation.py
--rw-r--r--   0 russt      (504) staff       (20)     3177 2022-09-21 09:42:38.000000 manipulation-2022.9.23/manipulation/exercises/pose/test_ransac.py
-drwxr-xr-x   0 russt      (504) staff       (20)        0 2022-09-24 01:11:05.151574 manipulation-2022.9.23/manipulation/exercises/rl/
--rw-r--r--   0 russt      (504) staff       (20)     3647 2021-12-11 10:12:32.000000 manipulation-2022.9.23/manipulation/exercises/rl/test_stochastic_optimization.py
--rw-r--r--   0 russt      (504) staff       (20)     3053 2021-12-11 10:12:32.000000 manipulation-2022.9.23/manipulation/exercises/rl/test_vpg.py
-drwxr-xr-x   0 russt      (504) staff       (20)        0 2022-09-24 01:11:05.152646 manipulation-2022.9.23/manipulation/exercises/robot/
--rw-r--r--   0 russt      (504) staff       (20)      954 2022-09-09 01:18:42.000000 manipulation-2022.9.23/manipulation/exercises/robot/test_direct_joint_control.py
--rw-r--r--   0 russt      (504) staff       (20)     1150 2022-09-09 01:37:26.000000 manipulation-2022.9.23/manipulation/exercises/robot/test_manipulation_io.py
--rw-r--r--   0 russt      (504) staff       (20)     2359 2021-12-11 10:12:32.000000 manipulation-2022.9.23/manipulation/exercises/robot/test_reflected_inertia.py
--rw-r--r--   0 russt      (504) staff       (20)      693 2021-12-11 10:12:32.000000 manipulation-2022.9.23/manipulation/exercises/robot/test_survey.py
-drwxr-xr-x   0 russt      (504) staff       (20)        0 2022-09-24 01:11:05.153023 manipulation-2022.9.23/manipulation/exercises/segmentation/
--rw-r--r--   0 russt      (504) staff       (20)     1410 2021-12-11 10:12:32.000000 manipulation-2022.9.23/manipulation/exercises/segmentation/test_mask.py
--rw-r--r--   0 russt      (504) staff       (20)     2126 2021-12-11 10:12:32.000000 manipulation-2022.9.23/manipulation/exercises/segmentation/test_segmentation_and_grasp.py
-drwxr-xr-x   0 russt      (504) staff       (20)        0 2022-09-24 01:11:05.153576 manipulation-2022.9.23/manipulation/exercises/trajectories/
-drwxr-xr-x   0 russt      (504) staff       (20)        0 2022-09-24 01:11:05.155212 manipulation-2022.9.23/manipulation/exercises/trajectories/rrt_planner/
--rw-r--r--   0 russt      (504) staff       (20)        0 2021-12-11 10:12:32.000000 manipulation-2022.9.23/manipulation/exercises/trajectories/rrt_planner/__init__.py
--rw-r--r--   0 russt      (504) staff       (20)    23494 2021-12-11 10:12:32.000000 manipulation-2022.9.23/manipulation/exercises/trajectories/rrt_planner/geometry.py
--rw-r--r--   0 russt      (504) staff       (20)     3754 2021-12-11 10:12:32.000000 manipulation-2022.9.23/manipulation/exercises/trajectories/rrt_planner/iiwa_rrt_problem.py
--rw-r--r--   0 russt      (504) staff       (20)     6317 2021-12-11 10:12:32.000000 manipulation-2022.9.23/manipulation/exercises/trajectories/rrt_planner/robot.py
--rw-r--r--   0 russt      (504) staff       (20)    14619 2021-12-11 10:12:32.000000 manipulation-2022.9.23/manipulation/exercises/trajectories/rrt_planner/rrt_planning.py
--rw-r--r--   0 russt      (504) staff       (20)     1491 2021-12-11 10:12:32.000000 manipulation-2022.9.23/manipulation/exercises/trajectories/test_door_opening.py
--rw-r--r--   0 russt      (504) staff       (20)     2546 2021-12-11 10:12:32.000000 manipulation-2022.9.23/manipulation/exercises/trajectories/test_rrt_planning.py
--rw-r--r--   0 russt      (504) staff       (20)     2655 2022-09-21 09:42:38.000000 manipulation-2022.9.23/manipulation/icp.py
--rw-r--r--   0 russt      (504) staff       (20)      246 2022-08-29 09:35:58.000000 manipulation-2022.9.23/manipulation/meshcat_cpp_utils.py
--rw-r--r--   0 russt      (504) staff       (20)    17455 2022-09-22 10:44:05.000000 manipulation-2022.9.23/manipulation/meshcat_utils.py
-drwxr-xr-x   0 russt      (504) staff       (20)        0 2022-09-24 01:11:05.162854 manipulation-2022.9.23/manipulation/models/
--rw-r--r--   0 russt      (504) staff       (20)     5938 2022-04-29 11:59:11.000000 manipulation-2022.9.23/manipulation/models/061_foam_brick_w_visual_contact_spheres.sdf
-drwxr-xr-x   0 russt      (504) staff       (20)        0 2022-09-24 01:11:05.163236 manipulation-2022.9.23/manipulation/models/bunny/
--rw-r--r--   0 russt      (504) staff       (20)   658744 2021-12-11 10:12:32.000000 manipulation-2022.9.23/manipulation/models/bunny/bun_zipper_res2.ply
--rw-r--r--   0 russt      (504) staff       (20)     1496 2021-12-11 10:12:32.000000 manipulation-2022.9.23/manipulation/models/camera_box.sdf
--rw-r--r--   0 russt      (504) staff       (20)      151 2022-09-08 13:14:02.000000 manipulation-2022.9.23/manipulation/models/clutter.dmd.yaml
--rw-r--r--   0 russt      (504) staff       (20)      446 2022-03-05 18:32:17.000000 manipulation-2022.9.23/manipulation/models/clutter_mustard.yaml
--rw-r--r--   0 russt      (504) staff       (20)      175 2021-12-11 10:12:32.000000 manipulation-2022.9.23/manipulation/models/clutter_planning.yaml
--rw-r--r--   0 russt      (504) staff       (20)      161 2022-09-08 13:14:02.000000 manipulation-2022.9.23/manipulation/models/clutter_w_cameras.dmd.yaml
--rw-r--r--   0 russt      (504) staff       (20)     2485 2021-12-11 10:12:32.000000 manipulation-2022.9.23/manipulation/models/double_pendulum.urdf
--rw-r--r--   0 russt      (504) staff       (20)      688 2022-09-08 13:14:02.000000 manipulation-2022.9.23/manipulation/models/iiwa_and_wsg.dmd.yaml
--rw-r--r--   0 russt      (504) staff       (20)     1662 2022-03-05 18:32:17.000000 manipulation-2022.9.23/manipulation/models/mustard_w_cameras.yaml
--rw-r--r--   0 russt      (504) staff       (20)     2004 2021-12-11 10:12:32.000000 manipulation-2022.9.23/manipulation/models/planar_bin.sdf
--rw-r--r--   0 russt      (504) staff       (20)     3716 2022-05-25 00:46:59.000000 manipulation-2022.9.23/manipulation/models/planar_foam_brick_collision_as_visual.sdf
--rw-r--r--   0 russt      (504) staff       (20)     3002 2022-06-26 10:43:13.000000 manipulation-2022.9.23/manipulation/models/schunk_wsg_50_welded_fingers.sdf
--rw-r--r--   0 russt      (504) staff       (20)      111 2021-12-11 10:12:32.000000 manipulation-2022.9.23/manipulation/models/schunk_wsg_50_welded_fingers.yaml
--rw-r--r--   0 russt      (504) staff       (20)     2350 2022-03-05 18:32:17.000000 manipulation-2022.9.23/manipulation/models/segmentation_and_grasp_scene.yaml
--rw-r--r--   0 russt      (504) staff       (20)     2784 2021-12-11 10:12:32.000000 manipulation-2022.9.23/manipulation/models/shelves.sdf
--rw-r--r--   0 russt      (504) staff       (20)      686 2021-12-20 14:34:17.000000 manipulation-2022.9.23/manipulation/models/two_bins.sdf
--rw-r--r--   0 russt      (504) staff       (20)      653 2021-12-11 10:12:32.000000 manipulation-2022.9.23/manipulation/models/two_bins.yaml
--rw-r--r--   0 russt      (504) staff       (20)     2459 2021-12-20 14:34:17.000000 manipulation-2022.9.23/manipulation/models/two_bins_w_cameras.sdf
--rw-r--r--   0 russt      (504) staff       (20)     1911 2021-12-11 10:12:32.000000 manipulation-2022.9.23/manipulation/models/two_bins_w_cameras.yaml
--rw-r--r--   0 russt      (504) staff       (20)    16421 2022-03-05 18:32:17.000000 manipulation-2022.9.23/manipulation/models/two_link_iiwa14.urdf
--rw-r--r--   0 russt      (504) staff       (20)     2346 2022-09-21 09:42:38.000000 manipulation-2022.9.23/manipulation/mustard_depth_camera_example.py
--rw-r--r--   0 russt      (504) staff       (20)     2559 2022-09-21 09:42:38.000000 manipulation-2022.9.23/manipulation/open3d_utils.py
--rw-r--r--   0 russt      (504) staff       (20)    27941 2022-09-21 10:07:07.000000 manipulation-2022.9.23/manipulation/scenarios.py
-drwxr-xr-x   0 russt      (504) staff       (20)        0 2022-09-24 01:11:05.166117 manipulation-2022.9.23/manipulation/test/
--rw-r--r--   0 russt      (504) staff       (20)     2559 2022-06-13 23:12:21.000000 manipulation-2022.9.23/manipulation/test/test_gym.py
--rw-r--r--   0 russt      (504) staff       (20)      425 2022-08-29 09:17:32.000000 manipulation-2022.9.23/manipulation/test/test_meshcat_utils.py
--rw-r--r--   0 russt      (504) staff       (20)      675 2022-05-14 20:52:13.000000 manipulation-2022.9.23/manipulation/test/test_model_directives.py
--rw-r--r--   0 russt      (504) staff       (20)     1152 2022-09-21 09:42:38.000000 manipulation-2022.9.23/manipulation/test/test_open3d_utils.py
--rw-r--r--   0 russt      (504) staff       (20)      158 2021-12-20 14:34:17.000000 manipulation-2022.9.23/manipulation/test/test_utils.py
--rw-r--r--   0 russt      (504) staff       (20)     7752 2022-05-14 20:35:45.000000 manipulation-2022.9.23/manipulation/utils.py
-drwxr-xr-x   0 russt      (504) staff       (20)        0 2022-09-24 01:11:05.147335 manipulation-2022.9.23/manipulation.egg-info/
--rw-r--r--   0 russt      (504) staff       (20)      971 2022-09-24 01:11:05.000000 manipulation-2022.9.23/manipulation.egg-info/PKG-INFO
--rw-r--r--   0 russt      (504) staff       (20)     3156 2022-09-24 01:11:05.000000 manipulation-2022.9.23/manipulation.egg-info/SOURCES.txt
--rw-r--r--   0 russt      (504) staff       (20)        1 2022-09-24 01:11:05.000000 manipulation-2022.9.23/manipulation.egg-info/dependency_links.txt
--rw-r--r--   0 russt      (504) staff       (20)       94 2022-09-24 01:11:05.000000 manipulation-2022.9.23/manipulation.egg-info/requires.txt
--rw-r--r--   0 russt      (504) staff       (20)       13 2022-09-24 01:11:05.000000 manipulation-2022.9.23/manipulation.egg-info/top_level.txt
--rw-r--r--   0 russt      (504) staff       (20)      103 2022-01-04 11:46:53.000000 manipulation-2022.9.23/pyproject.toml
--rw-r--r--   0 russt      (504) staff       (20)     3156 2022-09-24 01:11:05.168079 manipulation-2022.9.23/setup.cfg
+drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-05-29 21:26:51.370219 manipulation-2023.5.29/
+-rw-r--r--   0 russt      (504) staff       (20)     1561 2022-07-31 19:35:30.000000 manipulation-2023.5.29/LICENSE.TXT
+-rw-r--r--   0 russt      (504) staff       (20)      977 2023-05-29 21:26:51.370321 manipulation-2023.5.29/PKG-INFO
+-rw-r--r--   0 russt      (504) staff       (20)      472 2022-11-10 11:04:31.000000 manipulation-2023.5.29/README.md
+drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-05-29 21:26:51.338221 manipulation-2023.5.29/manipulation/
+-rw-r--r--   0 russt      (504) staff       (20)     2390 2022-11-15 14:27:42.000000 manipulation-2023.5.29/manipulation/BUILD.bazel
+-rw-r--r--   0 russt      (504) staff       (20)      167 2023-03-12 00:55:50.000000 manipulation-2023.5.29/manipulation/__init__.py
+-rw-r--r--   0 russt      (504) staff       (20)     6496 2023-03-12 00:55:50.000000 manipulation-2023.5.29/manipulation/clutter.py
+-rw-r--r--   0 russt      (504) staff       (20)    13232 2023-03-12 00:55:50.000000 manipulation-2023.5.29/manipulation/drake_gym.py
+drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-05-29 21:26:51.339365 manipulation-2023.5.29/manipulation/envs/
+-rw-r--r--   0 russt      (504) staff       (20)      551 2022-07-31 19:35:30.000000 manipulation-2023.5.29/manipulation/envs/BUILD.bazel
+-rw-r--r--   0 russt      (504) staff       (20)    10475 2023-03-12 00:55:50.000000 manipulation-2023.5.29/manipulation/envs/box_flipup.py
+drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-05-29 21:26:51.339939 manipulation-2023.5.29/manipulation/exercises/
+-rw-r--r--   0 russt      (504) staff       (20)      345 2022-07-31 19:35:30.000000 manipulation-2023.5.29/manipulation/exercises/BUILD.bazel
+drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-05-29 21:26:51.341943 manipulation-2023.5.29/manipulation/exercises/clutter/
+-rw-r--r--   0 russt      (504) staff       (20)      798 2022-10-14 12:15:23.000000 manipulation-2023.5.29/manipulation/exercises/clutter/BUILD.bazel
+-rw-r--r--   0 russt      (504) staff       (20)    32464 2021-12-11 10:12:32.000000 manipulation-2023.5.29/manipulation/exercises/clutter/normal_solution.npy
+-rw-r--r--   0 russt      (504) staff       (20)     1723 2023-03-12 00:55:50.000000 manipulation-2023.5.29/manipulation/exercises/clutter/test_analytic_grasp.py
+-rw-r--r--   0 russt      (504) staff       (20)     6180 2023-03-12 00:55:50.000000 manipulation-2023.5.29/manipulation/exercises/clutter/test_grasp_candidate.py
+-rw-r--r--   0 russt      (504) staff       (20)     1788 2023-03-12 00:55:50.000000 manipulation-2023.5.29/manipulation/exercises/clutter/test_normal.py
+-rw-r--r--   0 russt      (504) staff       (20)     9803 2023-03-12 00:55:50.000000 manipulation-2023.5.29/manipulation/exercises/clutter/test_simulation_tuning.py
+drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-05-29 21:26:51.342449 manipulation-2023.5.29/manipulation/exercises/deep_perception/
+-rw-r--r--   0 russt      (504) staff       (20)      365 2022-10-21 02:52:37.000000 manipulation-2023.5.29/manipulation/exercises/deep_perception/BUILD.bazel
+-rw-r--r--   0 russt      (504) staff       (20)     3633 2023-03-12 00:55:50.000000 manipulation-2023.5.29/manipulation/exercises/deep_perception/test_contrastive.py
+drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-05-29 21:26:51.343082 manipulation-2023.5.29/manipulation/exercises/force/
+-rw-r--r--   0 russt      (504) staff       (20)      355 2022-07-31 19:35:30.000000 manipulation-2023.5.29/manipulation/exercises/force/BUILD.bazel
+-rw-r--r--   0 russt      (504) staff       (20)     1602 2023-05-29 15:59:44.000000 manipulation-2023.5.29/manipulation/exercises/force/test_hybrid.py
+-rw-r--r--   0 russt      (504) staff       (20)     4951 2023-03-12 00:55:50.000000 manipulation-2023.5.29/manipulation/exercises/grader.py
+drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-05-29 21:26:51.345202 manipulation-2023.5.29/manipulation/exercises/pick/
+-rw-r--r--   0 russt      (504) staff       (20)     1046 2022-07-31 19:35:30.000000 manipulation-2023.5.29/manipulation/exercises/pick/BUILD.bazel
+-rw-r--r--   0 russt      (504) staff       (20)     1188 2023-03-12 00:55:50.000000 manipulation-2023.5.29/manipulation/exercises/pick/plot_planar_manipulator.py
+-rw-r--r--   0 russt      (504) staff       (20)    26805 2023-03-12 00:55:50.000000 manipulation-2023.5.29/manipulation/exercises/pick/test_differential_ik.py
+-rw-r--r--   0 russt      (504) staff       (20)     3584 2023-03-12 00:55:50.000000 manipulation-2023.5.29/manipulation/exercises/pick/test_planar_manipulator.py
+-rw-r--r--   0 russt      (504) staff       (20)     2886 2023-03-12 00:55:50.000000 manipulation-2023.5.29/manipulation/exercises/pick/test_rigid_transforms.py
+-rw-r--r--   0 russt      (504) staff       (20)     1962 2023-03-12 00:55:50.000000 manipulation-2023.5.29/manipulation/exercises/pick/test_robot_painter.py
+-rw-r--r--   0 russt      (504) staff       (20)     1138 2023-03-12 00:55:50.000000 manipulation-2023.5.29/manipulation/exercises/pick/test_simple_qp.py
+drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-05-29 21:26:51.347239 manipulation-2023.5.29/manipulation/exercises/pose/
+-rw-r--r--   0 russt      (504) staff       (20)      665 2022-07-31 19:35:30.000000 manipulation-2023.5.29/manipulation/exercises/pose/BUILD.bazel
+-rw-r--r--   0 russt      (504) staff       (20)   116432 2021-12-11 10:12:32.000000 manipulation-2023.5.29/manipulation/exercises/pose/pcl_filtered.npy
+-rw-r--r--   0 russt      (504) staff       (20)     3737 2023-03-12 00:55:50.000000 manipulation-2023.5.29/manipulation/exercises/pose/test_icp.py
+-rw-r--r--   0 russt      (504) staff       (20)     1291 2023-03-12 00:55:50.000000 manipulation-2023.5.29/manipulation/exercises/pose/test_pose_estimation.py
+-rw-r--r--   0 russt      (504) staff       (20)     3261 2023-03-12 00:55:50.000000 manipulation-2023.5.29/manipulation/exercises/pose/test_ransac.py
+drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-05-29 21:26:51.347986 manipulation-2023.5.29/manipulation/exercises/rl/
+-rw-r--r--   0 russt      (504) staff       (20)      500 2022-07-31 19:35:30.000000 manipulation-2023.5.29/manipulation/exercises/rl/BUILD.bazel
+-rw-r--r--   0 russt      (504) staff       (20)     3379 2023-03-12 00:55:50.000000 manipulation-2023.5.29/manipulation/exercises/rl/test_stochastic_optimization.py
+-rw-r--r--   0 russt      (504) staff       (20)     2890 2023-03-12 00:55:50.000000 manipulation-2023.5.29/manipulation/exercises/rl/test_vpg.py
+drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-05-29 21:26:51.349352 manipulation-2023.5.29/manipulation/exercises/robot/
+-rw-r--r--   0 russt      (504) staff       (20)      774 2022-09-09 01:21:28.000000 manipulation-2023.5.29/manipulation/exercises/robot/BUILD.bazel
+-rw-r--r--   0 russt      (504) staff       (20)      981 2023-03-12 00:55:50.000000 manipulation-2023.5.29/manipulation/exercises/robot/test_direct_joint_control.py
+-rw-r--r--   0 russt      (504) staff       (20)     1180 2023-03-12 00:55:50.000000 manipulation-2023.5.29/manipulation/exercises/robot/test_manipulation_io.py
+-rw-r--r--   0 russt      (504) staff       (20)     2167 2023-03-12 00:55:50.000000 manipulation-2023.5.29/manipulation/exercises/robot/test_reflected_inertia.py
+-rw-r--r--   0 russt      (504) staff       (20)      671 2023-03-12 00:55:50.000000 manipulation-2023.5.29/manipulation/exercises/robot/test_survey.py
+drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-05-29 21:26:51.350118 manipulation-2023.5.29/manipulation/exercises/segmentation/
+-rw-r--r--   0 russt      (504) staff       (20)      499 2022-10-21 02:51:30.000000 manipulation-2023.5.29/manipulation/exercises/segmentation/BUILD.bazel
+-rw-r--r--   0 russt      (504) staff       (20)     1394 2023-03-12 00:55:50.000000 manipulation-2023.5.29/manipulation/exercises/segmentation/test_mask.py
+-rw-r--r--   0 russt      (504) staff       (20)     2291 2023-03-12 00:55:50.000000 manipulation-2023.5.29/manipulation/exercises/segmentation/test_segmentation_and_grasp.py
+drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-05-29 21:26:51.351029 manipulation-2023.5.29/manipulation/exercises/trajectories/
+-rw-r--r--   0 russt      (504) staff       (20)      629 2022-10-28 00:13:17.000000 manipulation-2023.5.29/manipulation/exercises/trajectories/BUILD.bazel
+drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-05-29 21:26:51.353257 manipulation-2023.5.29/manipulation/exercises/trajectories/rrt_planner/
+-rw-r--r--   0 russt      (504) staff       (20)      490 2022-07-31 19:35:30.000000 manipulation-2023.5.29/manipulation/exercises/trajectories/rrt_planner/BUILD.bazel
+-rw-r--r--   0 russt      (504) staff       (20)        0 2021-12-11 10:12:32.000000 manipulation-2023.5.29/manipulation/exercises/trajectories/rrt_planner/__init__.py
+-rw-r--r--   0 russt      (504) staff       (20)    23490 2023-03-12 00:55:50.000000 manipulation-2023.5.29/manipulation/exercises/trajectories/rrt_planner/geometry.py
+-rw-r--r--   0 russt      (504) staff       (20)     3781 2023-03-12 00:55:50.000000 manipulation-2023.5.29/manipulation/exercises/trajectories/rrt_planner/iiwa_rrt_problem.py
+-rw-r--r--   0 russt      (504) staff       (20)     6308 2023-03-12 00:55:50.000000 manipulation-2023.5.29/manipulation/exercises/trajectories/rrt_planner/robot.py
+-rw-r--r--   0 russt      (504) staff       (20)    14619 2021-12-11 10:12:32.000000 manipulation-2023.5.29/manipulation/exercises/trajectories/rrt_planner/rrt_planning.py
+-rw-r--r--   0 russt      (504) staff       (20)     1463 2023-03-12 00:55:50.000000 manipulation-2023.5.29/manipulation/exercises/trajectories/test_door_opening.py
+-rw-r--r--   0 russt      (504) staff       (20)     2402 2023-03-12 00:55:50.000000 manipulation-2023.5.29/manipulation/exercises/trajectories/test_rrt_planning.py
+-rw-r--r--   0 russt      (504) staff       (20)     5576 2023-03-12 00:55:50.000000 manipulation-2023.5.29/manipulation/exercises/trajectories/test_taskspace_iris.py
+-rw-r--r--   0 russt      (504) staff       (20)     3764 2023-03-12 00:55:50.000000 manipulation-2023.5.29/manipulation/icp.py
+-rw-r--r--   0 russt      (504) staff       (20)      256 2023-03-12 00:55:50.000000 manipulation-2023.5.29/manipulation/meshcat_cpp_utils.py
+-rw-r--r--   0 russt      (504) staff       (20)    15686 2023-03-12 00:55:50.000000 manipulation-2023.5.29/manipulation/meshcat_utils.py
+drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-05-29 21:26:51.366299 manipulation-2023.5.29/manipulation/models/
+-rw-r--r--   0 russt      (504) staff       (20)     5938 2022-04-29 11:59:11.000000 manipulation-2023.5.29/manipulation/models/061_foam_brick_w_visual_contact_spheres.sdf
+-rw-r--r--   0 russt      (504) staff       (20)      466 2022-07-31 19:35:30.000000 manipulation-2023.5.29/manipulation/models/BUILD.bazel
+drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-05-29 21:26:51.368878 manipulation-2023.5.29/manipulation/models/bunny/
+-rw-r--r--   0 russt      (504) staff       (20)      299 2022-09-21 09:42:38.000000 manipulation-2023.5.29/manipulation/models/bunny/BUILD.bazel
+-rw-r--r--   0 russt      (504) staff       (20)     1280 2022-09-21 09:42:38.000000 manipulation-2023.5.29/manipulation/models/bunny/README
+-rw-r--r--   0 russt      (504) staff       (20)   658744 2021-12-11 10:12:32.000000 manipulation-2023.5.29/manipulation/models/bunny/bun_zipper_res2.ply
+-rw-r--r--   0 russt      (504) staff       (20)   196232 2022-09-21 09:42:38.000000 manipulation-2023.5.29/manipulation/models/bunny/bunny.npy
+-rw-r--r--   0 russt      (504) staff       (20)     1496 2021-12-11 10:12:32.000000 manipulation-2023.5.29/manipulation/models/camera_box.sdf
+-rw-r--r--   0 russt      (504) staff       (20)      155 2022-10-09 15:39:01.000000 manipulation-2023.5.29/manipulation/models/clutter.dmd.yaml
+-rw-r--r--   0 russt      (504) staff       (20)      450 2022-10-09 15:38:50.000000 manipulation-2023.5.29/manipulation/models/clutter_mustard.dmd.yaml
+-rw-r--r--   0 russt      (504) staff       (20)      183 2022-10-09 15:38:57.000000 manipulation-2023.5.29/manipulation/models/clutter_planning.dmd.yaml
+-rw-r--r--   0 russt      (504) staff       (20)      165 2022-10-09 15:39:00.000000 manipulation-2023.5.29/manipulation/models/clutter_w_cameras.dmd.yaml
+-rw-r--r--   0 russt      (504) staff       (20)     2485 2021-12-11 10:12:32.000000 manipulation-2023.5.29/manipulation/models/double_pendulum.urdf
+-rw-r--r--   0 russt      (504) staff       (20)     1407 2022-10-12 00:43:20.000000 manipulation-2023.5.29/manipulation/models/floor.sdf
+-rw-r--r--   0 russt      (504) staff       (20)      688 2022-09-08 13:14:02.000000 manipulation-2023.5.29/manipulation/models/iiwa_and_wsg.dmd.yaml
+-rw-r--r--   0 russt      (504) staff       (20)     1925 2022-11-10 11:04:31.000000 manipulation-2023.5.29/manipulation/models/manipulation_station_with_cupboard.dmd.yaml
+-rw-r--r--   0 russt      (504) staff       (20)     1662 2022-03-05 18:32:17.000000 manipulation-2023.5.29/manipulation/models/mustard_w_cameras.dmd.yaml
+-rw-r--r--   0 russt      (504) staff       (20)      374 2021-12-11 10:12:32.000000 manipulation-2023.5.29/manipulation/models/package.xml
+-rw-r--r--   0 russt      (504) staff       (20)     2004 2021-12-11 10:12:32.000000 manipulation-2023.5.29/manipulation/models/planar_bin.sdf
+-rw-r--r--   0 russt      (504) staff       (20)     3716 2022-05-25 00:46:59.000000 manipulation-2023.5.29/manipulation/models/planar_foam_brick_collision_as_visual.sdf
+-rw-r--r--   0 russt      (504) staff       (20)     1109 2022-11-10 11:04:31.000000 manipulation-2023.5.29/manipulation/models/planar_manipulation_station.dmd.yaml
+-rw-r--r--   0 russt      (504) staff       (20)    49209 2022-11-20 11:50:02.000000 manipulation-2023.5.29/manipulation/models/rubiks_cube.sdf
+-rw-r--r--   0 russt      (504) staff       (20)    15864 2022-11-20 10:08:31.000000 manipulation-2023.5.29/manipulation/models/rubiks_cube_2_by_2.sdf
+-rw-r--r--   0 russt      (504) staff       (20)      111 2021-12-11 10:12:32.000000 manipulation-2023.5.29/manipulation/models/schunk_wsg_50_welded_fingers.dmd.yaml
+-rw-r--r--   0 russt      (504) staff       (20)     2963 2023-03-12 00:55:50.000000 manipulation-2023.5.29/manipulation/models/schunk_wsg_50_welded_fingers.sdf
+-rw-r--r--   0 russt      (504) staff       (20)     2660 2023-03-12 00:55:50.000000 manipulation-2023.5.29/manipulation/models/schunk_wsg_50_welded_fingers_sphere.sdf
+-rw-r--r--   0 russt      (504) staff       (20)     2350 2022-03-05 18:32:17.000000 manipulation-2023.5.29/manipulation/models/segmentation_and_grasp_scene.dmd.yaml
+-rw-r--r--   0 russt      (504) staff       (20)     2784 2021-12-11 10:12:32.000000 manipulation-2023.5.29/manipulation/models/shelves.sdf
+-rw-r--r--   0 russt      (504) staff       (20)     2876 2022-10-25 10:48:24.000000 manipulation-2023.5.29/manipulation/models/shelves_w_ellipsoid_collision.sdf
+-rw-r--r--   0 russt      (504) staff       (20)      822 2022-10-12 00:43:20.000000 manipulation-2023.5.29/manipulation/models/two_bins.dmd.yaml
+-rw-r--r--   0 russt      (504) staff       (20)      686 2021-12-20 14:34:17.000000 manipulation-2023.5.29/manipulation/models/two_bins.sdf
+-rw-r--r--   0 russt      (504) staff       (20)     1915 2022-10-09 15:39:03.000000 manipulation-2023.5.29/manipulation/models/two_bins_w_cameras.dmd.yaml
+-rw-r--r--   0 russt      (504) staff       (20)     2459 2021-12-20 14:34:17.000000 manipulation-2023.5.29/manipulation/models/two_bins_w_cameras.sdf
+-rw-r--r--   0 russt      (504) staff       (20)    16331 2023-04-12 10:28:51.000000 manipulation-2023.5.29/manipulation/models/two_link_iiwa14.urdf
+-rw-r--r--   0 russt      (504) staff       (20)     2184 2023-03-12 00:55:50.000000 manipulation-2023.5.29/manipulation/mustard_depth_camera_example.py
+-rw-r--r--   0 russt      (504) staff       (20)     4225 2023-03-12 00:55:50.000000 manipulation-2023.5.29/manipulation/pick.py
+-rw-r--r--   0 russt      (504) staff       (20)    29849 2023-03-12 00:55:50.000000 manipulation-2023.5.29/manipulation/scenarios.py
+-rw-r--r--   0 russt      (504) staff       (20)     8109 2023-04-22 12:50:13.000000 manipulation-2023.5.29/manipulation/utils.py
+drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-05-29 21:26:51.370090 manipulation-2023.5.29/manipulation.egg-info/
+-rw-r--r--   0 russt      (504) staff       (20)     4185 2023-05-29 21:26:51.000000 manipulation-2023.5.29/manipulation.egg-info/SOURCES.txt
+-rw-r--r--   0 russt      (504) staff       (20)      528 2023-03-12 00:55:50.000000 manipulation-2023.5.29/pyproject.toml
+drwxr-xr-x   0 russt      (504) staff       (20)        0 2023-05-29 21:26:51.369693 manipulation-2023.5.29/rl/
+-rw-r--r--   0 russt      (504) staff       (20)     1873 2023-03-12 00:55:50.000000 manipulation-2023.5.29/rl/train_boxflipup.py
+-rw-r--r--   0 russt      (504) staff       (20)     3167 2023-05-29 21:26:51.371506 manipulation-2023.5.29/setup.cfg
```

### Comparing `manipulation-2022.9.23/LICENSE.TXT` & `manipulation-2023.5.29/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `manipulation-2022.9.23/PKG-INFO` & `manipulation-2023.5.29/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: manipulation
-Version: 2022.9.23
+Version: 2023.5.29
 Summary: MIT 6.4210 - Robotic Manipulation
 Home-page: https://manipulation.mit.edu
 Author: Russ Tedrake
 Author-email: russt@mit.edu
 Project-URL: Bug Tracker, https://github.com/RussTedrake/manipulation/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.TXT
 
 <!-- Remember, this produces the front page on github, dockerhub, and pypi. -->
 
-# Robot Manipulation
+# Robotic Manipulation
 
 *Perception, Planning, and Control*
 
 This is the companion software for the textbook available at:
-http://manipulation.mit.edu/
+https://manipulation.mit.edu/
 
 To cite this software (or the corresponding textbook), please use:
 
-Russ Tedrake. _Robot Manipulation: Perception, Planning, and Control (Course
-Notes for MIT 6.4210/6.4212)._ Downloaded on [date] from <http://manipulation.mit.edu/>.
+Russ Tedrake. _Robotic Manipulation: Perception, Planning, and Control (Course
+Notes for MIT 6.4210/6.4212)._ Downloaded on [date] from <https://manipulation.mit.edu/>.
```

### Comparing `manipulation-2022.9.23/manipulation/drake_gym.py` & `manipulation-2023.5.29/manipulation/drake_gym.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,87 +1,103 @@
-# Note: My goal is to move this to it's own repo: See Drake issue #15508.
+from typing import Callable, Optional, Union
+import warnings
 
 import gym
 import numpy as np
-from typing import Callable, Union
-import warnings
 
 from pydrake.common import RandomGenerator
-from pydrake.systems.sensors import ImageRgba8U
+from pydrake.systems.analysis import Simulator, SimulatorStatus
 from pydrake.systems.framework import (
     Context,
     InputPort,
     InputPortIndex,
-    OutputPort,
     OutputPortIndex,
     PortDataType,
     System,
 )
-from pydrake.systems.analysis import Simulator, SimulatorStatus
+from pydrake.systems.sensors import ImageRgba8U
 
 
 class DrakeGymEnv(gym.Env):
     """
     DrakeGymEnv provides a gym.Env interface for a Drake System (often a
     Diagram) using a Simulator.
     """
 
-    def __init__(self,
-                 simulator: Union[Simulator, Callable[[RandomGenerator],
-                                                      Simulator]],
-                 time_step: float,
-                 action_space: gym.spaces.space,
-                 observation_space: gym.spaces.space,
-                 reward: Union[Callable[[System, Context], float],
-                               OutputPortIndex, str],
-                 action_port_id: Union[InputPort, InputPortIndex, str] = None,
-                 observation_port_id: Union[OutputPortIndex, str] = None,
-                 render_rgb_port_id: Union[OutputPortIndex, str] = None):
+    def __init__(
+        self,
+        simulator: Union[Simulator, Callable[[RandomGenerator], Simulator]],
+        time_step: float,
+        action_space: gym.spaces.space,
+        observation_space: gym.spaces.space,
+        reward: Union[
+            Callable[[System, Context], float], OutputPortIndex, str
+        ],
+        action_port_id: Union[InputPort, InputPortIndex, str] = None,
+        observation_port_id: Union[OutputPortIndex, str] = None,
+        render_rgb_port_id: Union[OutputPortIndex, str] = None,
+        set_home: Callable[[Simulator, Context], None] = None,
+        hardware: bool = False,
+    ):
         """
         Args:
-            system: A Drake System
+            simulator: Either:
+                * A drake.systems.analysis.Simulator, or
+                * A function that produces a (randomized) Simulator.
             time_step: Each call to step() will advance the simulator by
                 `time_step` seconds.
             reward: The reward can be specified in one of two
                 ways: (1) by passing a callable with the signature
                 `value = reward(context)` or (2) by passing a scalar
-                vector-valued output port of `system`.
-            action_port: An input port of `system` compatible with the
-                action_space.  Each Env *must* have an action port; passing
-                `None` defaults to using the *first* input port (inspired by
+                vector-valued output port of `simulator`'s system.
+            action_port_id: The ID of an input port of `simulator`'s system
+                compatible with the action_space.  Each Env *must* have an
+                action port; passing `None` defaults to using the *first*
+                input port (inspired by
                 `InputPortSelection.kUseFirstInputIfItExists`).
             action_space: Defines the `gym.spaces.space` for the actions.  If
-                action_port is vector-valued, then passing `None` defaults to a
-                gym.spaces.Box of the correct dimension with bounds at negative
-                and positive infinity.  Note: Stable Baselines 3 strongly
-                encourages normalizing the action_space to [-1, 1].
-            observation_port: An output port of `system` compatible with the
-                observation_space. Each Env *must* have an observation port (it
-                seems that gym doesn't support empty observation spaces /
-                open-loop policies); passing `None` defaults to using the
-                *first* input port (inspired by
+                the action port is vector-valued, then passing `None` defaults
+                to a gym.spaces.Box of the correct dimension with bounds at
+                negative and positive infinity.  Note: Stable Baselines 3
+                strongly encourages normalizing the action_space to [-1, 1].
+            observation_port_id: An output port of `simulator`'s system
+                compatible with the observation_space. Each Env *must* have
+                an observation port (it seems that gym doesn't support empty
+                observation spaces / open-loop policies); passing `None`
+                defaults to using the *first* input port (inspired by
                 `OutputPortSelection.kUseFirstOutputIfItExists`).
             observation_space: Defines the gym.spaces.space for the
-                observations.  If observation_port is vector-valued, then
+                observations.  If the observation port is vector-valued, then
                 passing `None` defaults to a gym.spaces.Box of the correct
                 dimension with bounds at negative and positive infinity.
-            render_rgb_port: An optional output port of `system` that returns
-                an `ImageRgba8U`; often the `color_image` port of Drake's
-                `RgbdSensor`.  When not `None`, this enables the environment
-                `render_mode` `rgb_array`.
+            render_rgb_port: An optional output port of `simulator`'s system
+                that returns  an `ImageRgba8U`; often the `color_image` port
+                of a Drake `RgbdSensor`.  When not `None`, this enables the
+                environment `render_mode` `rgb_array`.
+            set_home: A function that sets the home state (plant, and/or env.)
+                at reset(). The reset state can be specified in one of
+                the two ways:
+                (1) setting random context using a Drake random_generator
+                (e.g. joint.set_random_pose_distribution()),
+                (2) parssing a function set_home().
+            hardware: If True, it prevents from setting random context at
+                reset() when using random_generator, but it does execute
+                set_home() if given.
+
 
         Notes (using `env` as an instance of this class):
         - You may set simulator/integrator preferences by using `env.simulator`
           directly.
         - The `done` condition returned by `step()` is always False by
           default.  Use `env.simulator.set_monitor()` to use Drake's monitor
           functionality for specifying termination conditions.
         - You may additionally wish to directly set `env.reward_range` and/or
           `env.spec`.  See the docs for gym.Env for more details.
         """
+        super().__init__()
         if isinstance(simulator, Simulator):
             self.simulator = simulator
             self.make_simulator = None
         elif callable(simulator):
             self.simulator = None
             self.make_simulator = simulator
         else:
@@ -113,69 +129,81 @@
 
         if observation_port_id:
             assert isinstance(observation_port_id, (OutputPortIndex, str))
             self.observation_port_id = observation_port_id
         else:
             self.observation_port_id = OutputPortIndex(0)
 
-        self.metadata['render.modes'] = ['human', 'ascii']
+        self.metadata["render.modes"] = ["human", "ascii"]
 
         # (Maybe) setup rendering
         if render_rgb_port_id:
             assert isinstance(render_rgb_port_id, (OutputPortIndex, str))
-            self.metadata['render.modes'].append('rgb_array')
+            self.metadata["render.modes"].append("rgb_array")
         self.render_rgb_port_id = render_rgb_port_id
 
         self.generator = RandomGenerator()
 
+        if set_home is None or callable(set_home):
+            self.set_home = set_home
+        else:
+            raise ValueError("Invalid set_home argument")
+
+        self.hardware = hardware
+
         if self.simulator:
             self._setup()
 
     def _setup(self):
         """Completes the setup once we have a self.simulator."""
         system = self.simulator.get_system()
 
         # Setup action port
         if self.action_port_id:
             if isinstance(self.action_port_id, InputPortIndex):
                 self.action_port = system.get_input_port(self.action_port_id)
             else:
                 self.action_port = system.GetInputPort(self.action_port_id)
         if self.action_port.get_data_type() == PortDataType.kVectorValued:
-            assert np.array_equal(self.action_space.shape,
-                                  [self.action_port.size()])
+            assert np.array_equal(
+                self.action_space.shape, [self.action_port.size()]
+            )
 
         def get_output_port(id):
             if isinstance(id, OutputPortIndex):
                 return system.get_output_port(id)
             return system.GetOutputPort(id)
 
         # Setup observation port
         if self.observation_port_id:
             self.observation_port = get_output_port(self.observation_port_id)
         if self.observation_port.get_data_type() == PortDataType.kVectorValued:
-            assert np.array_equal(self.observation_space.shape,
-                                  [self.observation_port.size()])
+            assert np.array_equal(
+                self.observation_space.shape, [self.observation_port.size()]
+            )
 
         # Note: We require that there is no direct feedthrough action_port to
         # observation_port.  Unfortunately, HasDirectFeedthrough returns false
         # positives, and would produce noisy warnings.
 
         # Setup reward
         if self.reward_port_id:
             reward_port = get_output_port(self.reward_port_id)
             self.reward = lambda system, context: reward_port.Eval(context)[0]
 
         # (Maybe) setup rendering port
         if self.render_rgb_port_id:
             self.render_rgb_port = get_output_port(self.render_rgb_port_id)
-            assert self.render_rgb_port.get_data_type() == \
-                PortDataType.kAbstractValued
-            assert isinstance(self.render_rgb_port.Allocate().get_value(),
-                              ImageRgba8U)
+            assert (
+                self.render_rgb_port.get_data_type()
+                == PortDataType.kAbstractValued
+            )
+            assert isinstance(
+                self.render_rgb_port.Allocate().get_value(), ImageRgba8U
+            )
 
     def step(self, action):
         """
         Implements gym.Env.step to advance the simulation forward by one
         `self.time_step`.
 
         Args:
@@ -183,76 +211,111 @@
         """
         assert self.simulator, "You must call reset() first"
 
         context = self.simulator.get_context()
         time = context.get_time()
 
         self.action_port.FixValue(context, action)
-        catch = False
+        truncated = False
         try:
             status = self.simulator.AdvanceTo(time + self.time_step)
         except RuntimeError as e:
-            if "MultibodyPlant's discrete update solver failed to converge" \
-                    not in e.args[0]:
+            if (
+                "MultibodyPlant's discrete update solver failed to converge"
+                not in e.args[0]
+            ):
                 raise
             warnings.warn("Calling Done after catching RuntimeError:")
             warnings.warn(e.args[0])
-            catch = True
+            truncated = True
+            status = e.args[0]
 
         observation = self.observation_port.Eval(context)
         reward = self.reward(self.simulator.get_system(), context)
-        done = catch or status.reason() == \
+        reached_term = (
             SimulatorStatus.ReturnReason.kReachedTerminationCondition
+        )
+        terminated = not truncated and (status.reason() == reached_term)
         info = dict()
 
-        return observation, reward, done, info
-
-    def reset(self):
+        # TODO(ggould) This interface is in flux and lags its documentation;
+        # when gym is next upgraded it will begin to generate warnings.  At
+        # that time replace `(terminated or truncated)`
+        # with `terminated, truncated`.
+        return observation, reward, (terminated or truncated), info
+
+    def reset(
+        self,
+        *,
+        seed: Optional[int] = None,
+        return_info: bool = False,
+        options: Optional[dict] = None
+    ):
         """
         If a callable "simulator factory" was passed to the constructor, then a
         new simulator is created.  Otherwise this method simply resets the
         `simulator` and its Context.
         """
+        assert options is None  # No options supported yet.
+
+        if seed is not None:
+            # TODO(ggould) This should not reset the generator if it was
+            # already explicitly seeded (see API spec), but we have no way to
+            # check that at the moment.
+            self.generator = RandomGenerator(seed)
+
         if self.make_simulator:
             self.simulator = self.make_simulator(self.generator)
             self._setup()
 
         context = self.simulator.get_mutable_context()
         context.SetTime(0)
-        self.simulator.get_system().SetRandomContext(context, self.generator)
         self.simulator.Initialize()
-        # Note: The output port will be evaluated without fixing the input port.
+        if self.set_home is not None:
+            self.simulator.get_system().SetDefaultContext(context)
+            self.set_home(self.simulator, context, seed)
+        else:
+            if not self.hardware:
+                self.simulator.get_system().SetRandomContext(
+                    context, self.generator
+                )
+        # Note: The output port will be evaluated without fixing the input
+        # port.
         observations = self.observation_port.Eval(context)
-        return observations
+        return observations if not return_info else (observations, dict())
 
-    def render(self, mode='human'):
+    def render(self, mode="human"):
         """
         Rendering in `human` mode is accomplished by calling Publish on
         `system`.  This should cause visualizers inside the System (e.g.
         MeshcatVisualizer, PlanarSceneGraphVisualizer, etc.) to draw their
         outputs.  To be fully compliant, those visualizers should set their
         default publishing period to `np.inf` (do not publish periodically).
 
         Rendering in `ascii` mode calls __repr__ on the system Context.
 
         Rendering in `rgb_array` mode is enabled by passing a compatible
         `render_rgb_port` to the class constructor.
         """
         assert self.simulator, "You must call reset() first"
 
-        if mode == 'human':
-            self.simulator.get_system().Publish(self.simulator.get_context())
+        if mode == "human":
+            self.simulator.get_system().ForcedPublish(
+                self.simulator.get_context()
+            )
             return
-        elif mode == 'ansi':
+        elif mode == "ansi":
             return __repr__(self.simulator.get_context())
-        elif mode == 'rgb_array':
-            assert self.render_rgb_port, \
-                "You must set render_rgb_port in the constructor"
+        elif mode == "rgb_array":
+            assert (
+                self.render_rgb_port
+            ), "You must set render_rgb_port in the constructor"
             return self.render_rgb_port.Eval(
-                self.simulator.get_context()).data[:, :, :3]
+                self.simulator.get_context()
+            ).data[:, :, :3]
         else:
             super(DrakeGymEnv, self).render(mode=mode)
 
     def seed(self, seed=None):
         """Implements gym.Env.seed using Drake's RandomGenerator."""
         if seed:
             self.generator = RandomGenerator(seed)
```

### Comparing `manipulation-2022.9.23/manipulation/envs/box_flipup.py` & `manipulation-2023.5.29/manipulation/envs/box_flipup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import gym
 import numpy as np
-
 from pydrake.all import (
     AddMultibodyPlantSceneGraph,
     Box,
     ConstantVectorSource,
     ContactVisualizer,
     ContactVisualizerParams,
     DiagramBuilder,
@@ -18,192 +17,245 @@
     MultibodyPositionToGeometryPose,
     Multiplexer,
     Parser,
     PassThrough,
     PlanarJoint,
     PrismaticJoint,
     RandomGenerator,
-    Rgba,
     RigidTransform,
     RotationMatrix,
     SceneGraph,
     Simulator,
     SpatialInertia,
     Sphere,
     UnitInertia,
     Variable,
 )
 
 from manipulation.drake_gym import DrakeGymEnv
 from manipulation.scenarios import AddShape, SetColor, SetTransparency
-from manipulation.utils import FindResource
+from manipulation.utils import ConfigureParser
 
 
-def AddPlanarBinAndSimpleBox(plant,
-                             mass=1.0,
-                             mu=1.0,
-                             width=0.2,
-                             depth=0.05,
-                             height=0.3):
+def AddPlanarBinAndSimpleBox(
+    plant, mass=1.0, mu=1.0, width=0.2, depth=0.05, height=0.3
+):
     parser = Parser(plant)
-    bin = parser.AddModelFromFile(FindResource("models/planar_bin.sdf"))
+    ConfigureParser(parser)
+    sdf_location = "package://manipulation/planar_bin.sdf"
+    bin = parser.AddModelsFromUrl(sdf_location)[0]
     plant.WeldFrames(
-        plant.world_frame(), plant.GetFrameByName("bin_base", bin),
-        RigidTransform(RotationMatrix.MakeZRotation(np.pi / 2.0),
-                       [0, 0, -0.015]))
+        plant.world_frame(),
+        plant.GetFrameByName("bin_base", bin),
+        RigidTransform(
+            RotationMatrix.MakeZRotation(np.pi / 2.0), [0, 0, -0.015]
+        ),
+    )
 
     planar_joint_frame = plant.AddFrame(
         FixedOffsetFrame(
-            "planar_joint_frame", plant.world_frame(),
-            RigidTransform(RotationMatrix.MakeXRotation(np.pi / 2))))
+            "planar_joint_frame",
+            plant.world_frame(),
+            RigidTransform(RotationMatrix.MakeXRotation(np.pi / 2)),
+        )
+    )
 
     # TODO(russt): make this a *random* box?
     # TODO(russt): move random box to a shared py file.
     box_instance = AddShape(plant, Box(width, depth, height), "box", mass, mu)
     box_joint = plant.AddJoint(
-        PlanarJoint("box", planar_joint_frame,
-                    plant.GetFrameByName("box", box_instance)))
-    box_joint.set_position_limits([-.5, -.1, -np.pi], [.5, .3, np.pi])
+        PlanarJoint(
+            "box",
+            planar_joint_frame,
+            plant.GetFrameByName("box", box_instance),
+        )
+    )
+    box_joint.set_position_limits([-0.5, -0.1, -np.pi], [0.5, 0.3, np.pi])
     box_joint.set_velocity_limits([-2, -2, -2], [2, 2, 2])
     box_joint.set_default_translation([0, depth / 2.0])
     return box_instance
 
 
 def AddPointFinger(plant):
-    finger = AddShape(plant, Sphere(0.01), "finger", color=[.9, .5, .5, 1.0])
+    finger = AddShape(
+        plant, Sphere(0.01), "finger", color=[0.9, 0.5, 0.5, 1.0]
+    )
     false_body1 = plant.AddRigidBody(
-        "false_body1", finger, SpatialInertia(0, [0, 0, 0],
-                                              UnitInertia(0, 0, 0)))
+        "false_body1",
+        finger,
+        SpatialInertia(0, [0, 0, 0], UnitInertia(0, 0, 0)),
+    )
     finger_x = plant.AddJoint(
-        PrismaticJoint("finger_x", plant.world_frame(),
-                       plant.GetFrameByName("false_body1"), [1, 0, 0], -.3, .3))
-    finger_x.set_position_limits([-.5], [.5])
+        PrismaticJoint(
+            "finger_x",
+            plant.world_frame(),
+            plant.GetFrameByName("false_body1"),
+            [1, 0, 0],
+            -0.3,
+            0.3,
+        )
+    )
+    finger_x.set_position_limits([-0.5], [0.5])
     finger_x.set_velocity_limits([-2], [2])
     plant.AddJointActuator("finger_x", finger_x)
     finger_z = plant.AddJoint(
-        PrismaticJoint("finger_z", plant.GetFrameByName("false_body1"),
-                       plant.GetFrameByName("finger"), [0, 0, 1], 0.0, 0.5))
+        PrismaticJoint(
+            "finger_z",
+            plant.GetFrameByName("false_body1"),
+            plant.GetFrameByName("finger"),
+            [0, 0, 1],
+            0.0,
+            0.5,
+        )
+    )
     finger_z.set_default_translation(0.25)
-    finger_z.set_position_limits([-.1], [.3])
+    finger_z.set_position_limits([-0.1], [0.3])
     finger_z.set_velocity_limits([-2], [2])
     plant.AddJointActuator("finger_z", finger_z)
 
     return finger
 
 
-def make_box_flipup(generator,
-                    observations="state",
-                    meshcat=None,
-                    time_limit=10):
+def make_box_flipup(
+    generator, observations="state", meshcat=None, time_limit=10
+):
     builder = DiagramBuilder()
     plant, scene_graph = AddMultibodyPlantSceneGraph(builder, time_step=0.001)
+
+    # TODO(russt): Re-enable Sap pending resolution of
+    # https://github.com/RobotLocomotion/drake/issues/18338
+    # plant.set_discrete_contact_solver(DiscreteContactSolver.kSap)
+
     # TODO(russt): randomize parameters.
+
     box = AddPlanarBinAndSimpleBox(plant)
     finger = AddPointFinger(plant)
     plant.Finalize()
     plant.set_name("plant")
     SetTransparency(scene_graph, alpha=0.5, source_id=plant.get_source_id())
     controller_plant = MultibodyPlant(time_step=0.005)
     AddPointFinger(controller_plant)
 
     if meshcat:
         MeshcatVisualizer.AddToBuilder(builder, scene_graph, meshcat)
-        meshcat.Set2dRenderMode(xmin=-.35, xmax=.35, ymin=-0.1, ymax=0.3)
+        meshcat.Set2dRenderMode(xmin=-0.35, xmax=0.35, ymin=-0.1, ymax=0.3)
         ContactVisualizer.AddToBuilder(
-            builder, plant, meshcat,
-            ContactVisualizerParams(radius=0.005, newtons_per_meter=40.0))
+            builder,
+            plant,
+            meshcat,
+            ContactVisualizerParams(radius=0.005, newtons_per_meter=40.0),
+        )
 
         # Use the controller plant to visualize the set point geometry.
         controller_scene_graph = builder.AddSystem(SceneGraph())
         controller_plant.RegisterAsSourceForSceneGraph(controller_scene_graph)
-        SetColor(controller_scene_graph,
-                 color=[1.0, 165.0 / 255, 0.0, 1.0],
-                 source_id=controller_plant.get_source_id())
+        SetColor(
+            controller_scene_graph,
+            color=[1.0, 165.0 / 255, 0.0, 1.0],
+            source_id=controller_plant.get_source_id(),
+        )
         controller_vis = MeshcatVisualizer.AddToBuilder(
-            builder, controller_scene_graph, meshcat,
-            MeshcatVisualizerParams(prefix="controller"))
+            builder,
+            controller_scene_graph,
+            meshcat,
+            MeshcatVisualizerParams(prefix="controller"),
+        )
         controller_vis.set_name("controller meshcat")
 
     controller_plant.Finalize()
 
     # Stiffness control.  (For a point finger with unit mass, the
     # InverseDynamicsController is identical)
     N = controller_plant.num_positions()
     kp = [100] * N
     ki = [1] * N
     kd = [2 * np.sqrt(kp[0])] * N
     controller = builder.AddSystem(
-        InverseDynamicsController(controller_plant, kp, ki, kd, False))
-    builder.Connect(plant.get_state_output_port(finger),
-                    controller.get_input_port_estimated_state())
+        InverseDynamicsController(controller_plant, kp, ki, kd, False)
+    )
+    builder.Connect(
+        plant.get_state_output_port(finger),
+        controller.get_input_port_estimated_state(),
+    )
 
     actions = builder.AddSystem(PassThrough(N))
     positions_to_state = builder.AddSystem(Multiplexer([N, N]))
-    builder.Connect(actions.get_output_port(),
-                    positions_to_state.get_input_port(0))
+    builder.Connect(
+        actions.get_output_port(), positions_to_state.get_input_port(0)
+    )
     zeros = builder.AddSystem(ConstantVectorSource([0] * N))
-    builder.Connect(zeros.get_output_port(),
-                    positions_to_state.get_input_port(1))
-    builder.Connect(positions_to_state.get_output_port(),
-                    controller.get_input_port_desired_state())
-    builder.Connect(controller.get_output_port(),
-                    plant.get_actuation_input_port())
+    builder.Connect(
+        zeros.get_output_port(), positions_to_state.get_input_port(1)
+    )
+    builder.Connect(
+        positions_to_state.get_output_port(),
+        controller.get_input_port_desired_state(),
+    )
+    builder.Connect(
+        controller.get_output_port(), plant.get_actuation_input_port()
+    )
     if meshcat:
         positions_to_poses = builder.AddSystem(
-            MultibodyPositionToGeometryPose(controller_plant))
+            MultibodyPositionToGeometryPose(controller_plant)
+        )
         builder.Connect(
             positions_to_poses.get_output_port(),
             controller_scene_graph.get_source_pose_port(
-                controller_plant.get_source_id()))
+                controller_plant.get_source_id()
+            ),
+        )
 
     builder.ExportInput(actions.get_input_port(), "actions")
     if observations == "state":
         builder.ExportOutput(plant.get_state_output_port(), "observations")
     # TODO(russt): Add 'time', and 'keypoints'
     else:
         raise ValueError("observations must be one of ['state']")
 
     class RewardSystem(LeafSystem):
-
         def __init__(self):
             LeafSystem.__init__(self)
             self.DeclareVectorInputPort("box_state", 6)
             self.DeclareVectorInputPort("finger_state", 4)
             self.DeclareVectorInputPort("actions", 2)
             self.DeclareVectorOutputPort("reward", 1, self.CalcReward)
 
         def CalcReward(self, context, output):
             box_state = self.get_input_port(0).Eval(context)
             finger_state = self.get_input_port(1).Eval(context)
             actions = self.get_input_port(2).Eval(context)
 
             angle_from_vertical = (box_state[2] % np.pi) - np.pi / 2
             cost = 2 * angle_from_vertical**2  # box angle
-            cost += 0.1 * box_state[5]**2  # box velocity
+            cost += 0.1 * box_state[5] ** 2  # box velocity
             effort = actions - finger_state[:2]
             cost += 0.1 * effort.dot(effort)  # effort
             # finger velocity
             cost += 0.1 * finger_state[2:].dot(finger_state[2:])
             # Add 10 to make rewards positive (to avoid rewarding simulator
             # crashes).
             output[0] = 10 - cost
 
     reward = builder.AddSystem(RewardSystem())
     builder.Connect(plant.get_state_output_port(box), reward.get_input_port(0))
-    builder.Connect(plant.get_state_output_port(finger),
-                    reward.get_input_port(1))
+    builder.Connect(
+        plant.get_state_output_port(finger), reward.get_input_port(1)
+    )
     builder.Connect(actions.get_output_port(), reward.get_input_port(2))
     builder.ExportOutput(reward.get_output_port(), "reward")
 
     # Set random state distributions.
-    uniform_random = Variable(name="uniform_random",
-                              type=Variable.Type.RANDOM_UNIFORM)
+    uniform_random = Variable(
+        name="uniform_random", type=Variable.Type.RANDOM_UNIFORM
+    )
     box_joint = plant.GetJointByName("box")
     x, y = box_joint.get_default_translation()
-    box_joint.set_random_pose_distribution([.2 * uniform_random - .1 + x, y], 0)
+    box_joint.set_random_pose_distribution(
+        [0.2 * uniform_random - 0.1 + x, y], 0
+    )
 
     diagram = builder.Build()
     simulator = Simulator(diagram)
 
     # Termination conditions:
     def monitor(context):
         if context.get_time() > time_limit:
@@ -211,33 +263,51 @@
         return EventStatus.Succeeded()
 
     simulator.set_monitor(monitor)
     return simulator
 
 
 def BoxFlipUpEnv(observations="state", meshcat=None, time_limit=10):
-    simulator = make_box_flipup(RandomGenerator(),
-                                observations,
-                                meshcat=meshcat,
-                                time_limit=time_limit)
-    action_space = gym.spaces.Box(low=np.array([-.5, -0.1], dtype="float32"),
-                                  high=np.array([.5, 0.6], dtype="float32"))
+    simulator = make_box_flipup(
+        RandomGenerator(), observations, meshcat=meshcat, time_limit=time_limit
+    )
+    action_space = gym.spaces.Box(
+        low=np.array([-0.5, -0.1]), high=np.array([0.5, 0.6]), dtype=np.float64
+    )
 
     plant = simulator.get_system().GetSubsystemByName("plant")
 
+    # It is unsound to use raw MBP dof limits as observation bounds, because
+    # most simulations will violate those limits in practice (in collision, or
+    # due to gravity, or in general because no constraint force is incurred
+    # except in violation).  However we don't have any other better limits
+    # here.  So we broaden the limits by a fixed offset and hope for the best.
+    NUM_DOFS = 5
+    POSITION_LIMIT_TOLERANCE = np.full((NUM_DOFS,), 0.1)
+    VELOCITY_LIMIT_TOLERANCE = np.full((NUM_DOFS,), 0.5)
     if observations == "state":
         low = np.concatenate(
-            (plant.GetPositionLowerLimits(), plant.GetVelocityLowerLimits()))
+            (
+                plant.GetPositionLowerLimits() - POSITION_LIMIT_TOLERANCE,
+                plant.GetVelocityLowerLimits() - VELOCITY_LIMIT_TOLERANCE,
+            )
+        )
         high = np.concatenate(
-            (plant.GetPositionUpperLimits(), plant.GetVelocityUpperLimits()))
-        observation_space = gym.spaces.Box(low=np.asarray(low, dtype="float32"),
-                                           high=np.asarray(high,
-                                                           dtype="float32"))
-
-    env = DrakeGymEnv(simulator=simulator,
-                      time_step=0.1,
-                      action_space=action_space,
-                      observation_space=observation_space,
-                      reward="reward",
-                      action_port_id="actions",
-                      observation_port_id="observations")
+            (
+                plant.GetPositionUpperLimits() + POSITION_LIMIT_TOLERANCE,
+                plant.GetVelocityUpperLimits() + VELOCITY_LIMIT_TOLERANCE,
+            )
+        )
+        observation_space = gym.spaces.Box(
+            low=np.asarray(low), high=np.asarray(high), dtype=np.float64
+        )
+
+    env = DrakeGymEnv(
+        simulator=simulator,
+        time_step=0.1,
+        action_space=action_space,
+        observation_space=observation_space,
+        reward="reward",
+        action_port_id="actions",
+        observation_port_id="observations",
+    )
     return env
```

### Comparing `manipulation-2022.9.23/manipulation/exercises/clutter/test_analytic_grasp.py` & `manipulation-2023.5.29/manipulation/exercises/clutter/test_analytic_grasp.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,55 +1,57 @@
 import unittest
 import timeout_decorator
 from gradescope_utils.autograder_utils.decorators import weight
 import numpy as np
-import os
 
 
 class TestAnalyticGrasp(unittest.TestCase):
-
     def __init__(self, test_name, notebook_locals):
         super().__init__(test_name)
         self.notebook_locals = notebook_locals
 
     @weight(4)
-    @timeout_decorator.timeout(10.)
+    @timeout_decorator.timeout(10.0)
     def test_antipodal_points(self):
         """Test find_antipodal_pts"""
         shape = self.notebook_locals["shape"]
         f = self.notebook_locals["find_antipodal_pts"]
 
         # Use a seed that can test for different Hessians
         np.random.seed(45)
 
         result_lst = []
         H_eig_lst = []
 
         for i in range(4):
             result, H_eig = f(shape)
             result_lst.append(result)
-            H_eig_lst.append(H_eig)
+            H_eig_lst.append(np.sort(H_eig)[::-1])
 
         result_lst_eval = np.array(result_lst)
         H_eig_lst_eval = np.array(H_eig_lst)
 
         # yapf: disable
         result_lst_target = np.array([  # noqa
             [6.276351, 3.497493],
             [3.948776, 1.636278],
             [6.104002, 4.219046],
             [3.223685, 0.710411]])
 
         H_eig_lst_target = np.array([  # noqa
-            [29612.82676, 35855.23483],
+            [35855.23483, 29612.82676],
             [-1025.65590, -1312.08498],
-            [-643.00117, 6819.32722],
-            [-1249.67350, 27654.86062]])
+            [6819.32722, -643.00117],
+            [27654.86062, -1249.67350]])
         # yapf: enable
 
         self.assertLessEqual(
-            np.linalg.norm(result_lst_target - result_lst_eval), 1e-4,
-            "The optimal values are not returned correctly.")
+            np.linalg.norm(result_lst_target - result_lst_eval),
+            1e-4,
+            "The optimal values are not returned correctly.",
+        )
 
-        self.assertLessEqual(np.linalg.norm(H_eig_lst_target - H_eig_lst_eval),
-                             1e-4,
-                             "The Hessian values are not returned correctly.")
+        self.assertLessEqual(
+            np.linalg.norm(H_eig_lst_target - H_eig_lst_eval),
+            1e-4,
+            "The Hessian values are not returned correctly.",
+        )
```

### Comparing `manipulation-2022.9.23/manipulation/exercises/clutter/test_grasp_candidate.py` & `manipulation-2023.5.29/manipulation/exercises/clutter/test_grasp_candidate.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,75 +23,72 @@
      [-0.26262784, -0.22653088, +0.93792874, +0.04541413]]])
 # yapf: enable
 
 test_indices = [10137, 21584, 7259, 32081]
 
 
 class TestGraspCandidate(unittest.TestCase):
-
     def __init__(self, test_name, notebook_locals):
         super().__init__(test_name)
         self.notebook_locals = notebook_locals
 
     @weight(4)
-    @timeout_decorator.timeout(10.)
+    @timeout_decorator.timeout(10.0)
     def test_darboux_frame(self):
         """Test compute_darboux_frame"""
         pcd = self.notebook_locals["pcd"]
         kdtree = KDTree(pcd.xyzs().T)
         f = self.notebook_locals["compute_darboux_frame"]
 
-        X_lst_eval = []
-
-        np.random.seed(11)
         for i in range(4):
             index = test_indices[i]
             RT = f(index, pcd, kdtree)
-            X_lst_eval.append(RT.GetAsMatrix34())
-
-        X_lst_eval = np.asarray(X_lst_eval)
-
-        self.assertLessEqual(np.linalg.norm(X_lst_target - X_lst_eval), 1e-4,
-                             "The Darboux frame is not correct")
+            RT_desired = RigidTransform(X_lst_target[i])
+            self.assertTrue(
+                RT.IsNearlyEqualTo(RT_desired, 0.1),
+                "Your transform doesn't match the expected transform",
+            )
 
         index = 5
         RT = f(index, pcd, kdtree)
 
-        X_lst_order_eval = RT.GetAsMatrix34()
-
         # yapf: disable
-        X_lst_order_target = np.array([  # noqa
+        RT_desired = RigidTransform(np.array([  # noqa
             [+0.03674694, -0.88056642, -0.47249594, +0.00884530],
             [+0.93758428, +0.19399482, -0.28862041, -0.00240727],
-            [+0.34581122, -0.43239886, +0.83273393, +0.19118717]])
+            [+0.34581122, -0.43239886, +0.83273393, +0.19118717]]))
         # yapf: enable
 
-        self.assertLessEqual(
-            np.linalg.norm(X_lst_order_eval - X_lst_order_target), 1e-4,
+        self.assertTrue(
+            RT.IsNearlyEqualTo(RT_desired, 0.01),
             "Did you forget to sort the eigenvalues, "
-            "or handle improper rotations?")
+            "or handle improper rotations?",
+        )
 
     @weight(4)
-    @timeout_decorator.timeout(10.)
+    @timeout_decorator.timeout(10.0)
     def test_minimum_distance(self):
         """Test find_minimum_distance"""
         pcd = self.notebook_locals["pcd"]
         f = self.notebook_locals["find_minimum_distance"]
 
         # The following should return nan
         for i in [0, 2]:
             dist, X_new = f(pcd, RigidTransform(X_lst_target[i]))
             self.assertTrue(
-                np.isnan(dist), "There is no value of y that results in "
-                "no collision in the grid, but dist is not nan")
+                np.isnan(dist),
+                "There is no value of y that results in "
+                "no collision in the grid, but dist is not nan",
+            )
             self.assertTrue(
                 isinstance(X_new, type(None)),
                 "There is no value of y that results in "
                 "no collision in the grid, but X_WGnew is"
-                "not None.")
+                "not None.",
+            )
 
         # yapf: disable
         dist_new_target = np.array([  # noqa
             0.0035799752,
             0.0008069168])
 
         X_new_target = np.array([  # noqa
@@ -107,56 +104,63 @@
         X_new_eval = []
         # The following should return numbers.
         for i in [1, 3]:
             dist, X_new = f(pcd, RigidTransform(X_lst_target[i]))
             self.assertTrue(
                 not np.isnan(dist),
                 "There is a valid value of y that results in "
-                "no collision in the grid, but dist is nan")
+                "no collision in the grid, but dist is nan",
+            )
             self.assertTrue(
                 not isinstance(X_new, type(None)),
                 "There is a valid value of y that results in no "
-                "collision in the grid, but X_WGnew is None.")
+                "collision in the grid, but X_WGnew is None.",
+            )
             dist_new_eval.append(dist)
             X_new_eval.append(X_new.GetAsMatrix34())
 
         dist_new_eval = np.array(dist_new_eval)
         X_new_eval = np.array(X_new_eval)
 
-        self.assertLessEqual(np.linalg.norm(dist_new_target - dist_new_eval),
-                             1e-5, "The returned distance is not correct.")
-        self.assertLessEqual(np.linalg.norm(X_new_target - X_new_eval), 1e-4,
-                             "The returned transform is not correct.")
+        self.assertLessEqual(
+            np.linalg.norm(dist_new_target - dist_new_eval),
+            1e-5,
+            "The returned distance is not correct.",
+        )
+        self.assertLessEqual(
+            np.linalg.norm(X_new_target - X_new_eval),
+            1e-4,
+            "The returned transform is not correct.",
+        )
 
     @weight(4)
-    @timeout_decorator.timeout(60.)
+    @timeout_decorator.timeout(60.0)
     def test_candidate_grasps(self):
         """Test compute_candidate_grasps"""
         pcd = self.notebook_locals["pcd_downsampled"]
-        f = self.notebook_locals["compute_candidate_grasps"]
-
-        # yapf: disable
-        X_lst_target = np.array([  # noqa
-            [[+0.00385728, -0.99714784, -0.07537471, +0.06982844],
-             [+0.99269683, -0.00527015, +0.12052071, -0.00385548],
-             [-0.12057423, -0.07528912, +0.98984516, +0.02492355]],
-            [[-0.82320983, +0.55645203, +0.11263515, -0.05386203],
-             [+0.55569232, +0.74907938, +0.36067459, -0.05987444],
-             [+0.11632545, +0.35950136, -0.92586565, -0.01982360]],
-            [[-0.37491799, +0.92414904, +0.07338335, -0.07043153],
-             [-0.85535209, -0.37535911, +0.35704106, +0.03011875],
-             [+0.35750425, +0.07109251, +0.93120170, +0.05676402]]])
-        # yapf: enable
-
-        grasp_candidates = f(pcd, candidate_num=3, random_seed=5)
+        compute_candidate_grasps = self.notebook_locals[
+            "compute_candidate_grasps"
+        ]
+        find_minimum_distance = self.notebook_locals["find_minimum_distance"]
+        check_collision = self.notebook_locals["check_collision"]
+        check_nonempty = self.notebook_locals["check_nonempty"]
+
+        grasp_candidates = compute_candidate_grasps(
+            pcd, candidate_num=3, random_seed=5
+        )
 
         self.assertTrue(
             len(grasp_candidates) == 3,
-            "Length of returned array is not correct.")
-
-        X_lst_eval = []
-        for i in range(len(grasp_candidates)):
-            X_lst_eval.append(grasp_candidates[i].GetAsMatrix34())
-        X_lst_eval = np.array(X_lst_eval)
+            "Length of returned array is not correct.",
+        )
 
-        self.assertLessEqual(np.linalg.norm(X_lst_target - X_lst_eval), 1e-4,
-                             "The returned grasp candidates are not correct.")
+        for X_WP in grasp_candidates:
+            distance, X_WP_new = find_minimum_distance(pcd, X_WP)
+            self.assertLessEqual(
+                distance, 1e-2
+            ), "The returned grasp candidates are not minimum distance"
+            self.assertTrue(
+                check_collision(pcd, X_WP)
+            ), "The returned grasp candidates have collisions"
+            self.assertTrue(
+                check_nonempty(pcd, X_WP)
+            ), "The returned grasp candidates are not empty"
```

### Comparing `manipulation-2022.9.23/manipulation/exercises/clutter/test_normal.py` & `manipulation-2023.5.29/manipulation/exercises/clutter/test_normal.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,43 +2,47 @@
 import timeout_decorator
 from gradescope_utils.autograder_utils.decorators import weight
 import numpy as np
 from manipulation.utils import FindResource
 
 
 class TestNormal(unittest.TestCase):
-
     def __init__(self, test_name, notebook_locals):
         super().__init__(test_name)
         self.notebook_locals = notebook_locals
 
     @weight(4)
     @timeout_decorator.timeout(60.0)
     def test_normal(self):
         """Testing the normal vectors"""
-        env = self.notebook_locals['env']
-        f = self.notebook_locals['estimate_normal_by_nearest_pixels']
-        pC = self.notebook_locals['pC']
+        env = self.notebook_locals["env"]
+        f = self.notebook_locals["estimate_normal_by_nearest_pixels"]
+        pC = self.notebook_locals["pC"]
 
         student_sol = f(env.X_WC, pC, uv_step=10)
         reference_sol = np.load(
-            FindResource("exercises/clutter/normal_solution.npy"))
+            FindResource("exercises/clutter/normal_solution.npy")
+        )
 
         self.assertTrue(
             len(student_sol) == len(reference_sol),
-            'the number of the normals is incorrect')
+            "the number of the normals is incorrect",
+        )
 
         for X, X_sol in zip(student_sol, reference_sol):
             # check only points within the bounding box
             pos_x, pos_y, pos_z = X_sol[0:3, 3]
             if abs(pos_x) < 1.0 and abs(pos_y) < 1.0:
                 sol_v = X_sol[0:3, 2]
                 # check only the normal vector, not the entire frame
                 student_v = X.GetAsMatrix4()[0:3, 2]
                 # normalize the vector in case it is not normalized
                 student_v = student_v / np.linalg.norm(student_v)
                 test = np.dot(student_v, sol_v)
                 self.assertTrue(
-                    test > 0.7, 'error at the point: \n {} \
+                    test > 0.7,
+                    "error at the point: \n {} \
                     \n normal is: {} \
-                    \n solution normal is: {}'.format([pos_x, pos_y, pos_z],
-                                                      student_v, sol_v))
+                    \n solution normal is: {}".format(
+                        [pos_x, pos_y, pos_z], student_v, sol_v
+                    ),
+                )
```

### Comparing `manipulation-2022.9.23/manipulation/exercises/force/test_hybrid.py` & `manipulation-2023.5.29/manipulation/exercises/force/test_hybrid.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,55 @@
 import unittest
 import timeout_decorator
 from gradescope_utils.autograder_utils.decorators import weight
 import numpy as np
-import os
 
 
 class TestHybrid(unittest.TestCase):
-
     def __init__(self, test_name, notebook_locals):
         super().__init__(test_name)
         self.notebook_locals = notebook_locals
 
     @weight(4)
-    @timeout_decorator.timeout(30.)
+    @timeout_decorator.timeout(30.0)
     def test_antipodal_points(self):
         """Test compute_ctrl"""
         log = self.notebook_locals["log"]
         plant = self.notebook_locals["plant"]
         plant_context = self.notebook_locals["plant_context"]
 
         # Get final pose of the book.
-        X_WB = plant.GetFreeBodyPose(plant_context,
-                                     plant.GetBodyByName("book_body"))
+        X_WB = plant.GetFreeBodyPose(
+            plant_context, plant.GetBodyByName("book_body")
+        )
 
         p_WB = X_WB.translation()
 
         # 1. Check upper bound on book pose.
         self.assertLessEqual(
-            p_WB[0], 0.55, "Edge of the book is not between the gap. "
-            "It is too far.")
+            p_WB[0],
+            0.55,
+            "Edge of the book is not between the gap. " "It is too far.",
+        )
 
         # 2. Check lower bound on book pose.
         self.assertLessEqual(
-            -p_WB[0], -0.5, "Edge of the book is not betwee the gap. "
-            "It is too close.")
+            -p_WB[0],
+            -0.5,
+            "Edge of the book is not between the gap. " "It is too close.",
+        )
 
         time = log.sample_times()
         traj = log.data()
 
         finger_length = 0.12
 
         p_x = traj[1, :] - finger_length * np.sin(traj[0, :])
         p_y = traj[2, :] - finger_length * np.cos(traj[0, :])
 
         for t in range(len(time)):
             self.assertLessEqual(
-                -p_y[t], -0.045, "The gripper tip cannot be lower than the "
-                "surface of the book.")
+                -p_y[t],
+                -0.045,
+                "The gripper tip cannot be lower than the "
+                "surface of the book.",
+            )
```

### Comparing `manipulation-2022.9.23/manipulation/exercises/grader.py` & `manipulation-2023.5.29/manipulation/exercises/grader.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,121 +11,139 @@
 
 def set_grader_throws(val):
     global grader_throws
     grader_throws = val
 
 
 class Grader:
-
     def __init__(self):
         pass
 
     @staticmethod
-    def grade_from_notebooks(test_cases_list, notebook_ipynb_list,
-                             results_json):
+    def grade_from_notebooks(
+        test_cases_list, notebook_ipynb_list, results_json
+    ):
         """
         Running notebooks in notebook_ipynb_list and evaluating
         them on test_cases_list. Result is written into results_json
         """
         try:
             notebook_locals_list = []
             for notebook_ipynb in notebook_ipynb_list:
                 notebook_locals_list.append(
-                    Grader.locals_from_notebook(notebook_ipynb))
+                    Grader.locals_from_notebook(notebook_ipynb)
+                )
         except Exception as e:
             Grader.global_fail_with_error_message(
-                "Exception when running file: " + notebook_ipynb + ', '
-                + str(e), results_json)
+                "Exception when running file: "
+                + notebook_ipynb
+                + ", "
+                + str(e),
+                results_json,
+            )
             raise
 
         # Grade notebook_locals_list on test_cases_list
-        Grader.grade_output(test_cases_list, notebook_locals_list, results_json)
+        Grader.grade_output(
+            test_cases_list, notebook_locals_list, results_json
+        )
 
     @staticmethod
     def grade_output(test_case_list, notebook_locals_list, results_json):
         """Grading the notebook_locals with the provided test_cases"""
         # setup test suite for gradescope
         suite = unittest.TestSuite()
-        for test_case, notebook_locals in zip(test_case_list,
-                                              notebook_locals_list):
+        for test_case, notebook_locals in zip(
+            test_case_list, notebook_locals_list
+        ):
             test_case_names = unittest.defaultTestLoader.getTestCaseNames(
-                test_case)
+                test_case
+            )
             for test_case_name in test_case_names:
                 suite.addTest(test_case(test_case_name, notebook_locals))
 
         # run all the tests in the suite
-        with open(results_json, 'w') as fh:
+        with open(results_json, "w") as fh:
             JSONTestRunner(stream=fh).run(suite)
 
     @staticmethod
     def locals_from_notebook(notebook_ipynb):
         """Read, run, return locals of notebook"""
-        banned_commands = ['HTML']
+        banned_commands = ["HTML"]
 
         ipynb = json.load(open(notebook_ipynb))
 
-        for cell in ipynb['cells']:
+        for cell in ipynb["cells"]:
             # clearOutput as an output type is not supported
             # by nbformat.reads(). Therefore, filter out
             # any output cells with the clearOutput warning
-            if ('outputs' in cell.keys()):
-                if any('clearOutput' in line['output_type']
-                       for line in cell['outputs']):
-                    cell['outputs'] = []
+            if "outputs" in cell.keys():
+                if any(
+                    "clearOutput" in line["output_type"]
+                    for line in cell["outputs"]
+                ):
+                    cell["outputs"] = []
 
             # erase test cells, this is optional and useful for debugging
             # to avoid recursions when developing
-            if any('## TEST ##' in line for line in cell['source']):
-                cell['source'] = []
+            if any("## TEST ##" in line for line in cell["source"]):
+                cell["source"] = []
             # filter out all the lines with banned commands
             if banned_commands is not None:
-                cell['source'] = [
-                    line for line in cell['source']
+                cell["source"] = [
+                    line
+                    for line in cell["source"]
                     if not any(command in line for command in banned_commands)
                 ]
 
         exporter = PythonExporter()
         source, meta = exporter.from_notebook_node(
-            nbformat.reads(json.dumps(ipynb), nbformat.NO_CONVERT))
-        with open('./cleaned_notebook.py', 'w') as fh:
+            nbformat.reads(json.dumps(ipynb), nbformat.NO_CONVERT)
+        )
+        with open("./cleaned_notebook.py", "w") as fh:
             fh.write(source)
 
-        notebook_locals = run_module('cleaned_notebook')
-        os.system('rm cleaned_notebook.py')
+        notebook_locals = run_module("cleaned_notebook")
+        os.system("rm cleaned_notebook.py")
         return notebook_locals
 
     @staticmethod
     def global_fail_with_error_message(msg, results_json):
         """Error message if no specific"""
         results = {"score": 0.0, "output": msg}
 
-        with open(results_json, 'w') as f:
+        with open(results_json, "w") as f:
             f.write(
-                json.dumps(results,
-                           indent=4,
-                           sort_keys=True,
-                           separators=(',', ': '),
-                           ensure_ascii=True))
+                json.dumps(
+                    results,
+                    indent=4,
+                    sort_keys=True,
+                    separators=(",", ": "),
+                    ensure_ascii=True,
+                )
+            )
 
     @staticmethod
     def print_test_results(results_json):
         """Printing the results.json"""
         # open the json file for reading
-        with open(results_json, 'r') as fh:
+        with open(results_json, "r") as fh:
             result = json.load(fh)
 
         # print total score
-        max_score = sum(test['max_score'] for test in result['tests'])
-        print('Total score is {}/{}.'.format(int(result['score']), max_score))
-
-        if grader_throws and int(result['score']) != max_score:
-            raise RuntimeError("Grader did not award full points.")
+        max_score = sum(test["max_score"] for test in result["tests"])
+        print("Total score is {}/{}.".format(int(result["score"]), max_score))
 
         # print partial scores
-        for test in result['tests']:
-            print('\nScore for {} is {}/{}.'.format(test['name'],
-                                                    int(test['score']),
-                                                    test['max_score']))
+        for test in result["tests"]:
+            print(
+                "\nScore for {} is {}/{}.".format(
+                    test["name"], int(test["score"]), test["max_score"]
+                )
+            )
 
             # print error message if any
-            if 'output' in test:
-                print('- ' + test['output'])
+            if "output" in test:
+                print("- " + test["output"])
+
+        if grader_throws and int(result["score"]) != max_score:
+            raise RuntimeError("Grader did not award full points.")
```

### Comparing `manipulation-2022.9.23/manipulation/exercises/pick/plot_planar_manipulator.py` & `manipulation-2023.5.29/manipulation/exercises/pick/plot_planar_manipulator.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,32 +11,32 @@
 
       - plot_planar_manipulator(q, forward_kinematics(q))
       - plot_planar_manipulator(inverse_kinematics(p), p)
 
     which helps verify the correctness of the implementations.
 
     """
-    base = [0., 0.]
+    base = [0.0, 0.0]
     p_AB = [np.cos(q[0]), np.sin(q[0])]
     p_AC = [
         np.cos(q[0]) + np.cos(q[0] + q[1]),
-        np.sin(q[0]) + np.sin(q[0] + q[1])
+        np.sin(q[0]) + np.sin(q[0] + q[1]),
     ]
 
     plt.figure()
 
     # Plot first link
-    plt.plot([base[0], p_AB[0]], [base[1], p_AB[1]], 'k-', linewidth=2)
+    plt.plot([base[0], p_AB[0]], [base[1], p_AB[1]], "k-", linewidth=2)
     # Plot second link
-    plt.plot([p_AB[0], p_AC[0]], [p_AB[1], p_AC[1]], 'k-', linewidth=2)
+    plt.plot([p_AB[0], p_AC[0]], [p_AB[1], p_AC[1]], "k-", linewidth=2)
     # Plot joint locations
-    plt.plot(base[0], base[1], 'go')
-    plt.plot(p_AB[0], p_AB[1], 'bo')
-    plt.plot(p_AC[0], p_AC[1], 'ro')
+    plt.plot(base[0], base[1], "go")
+    plt.plot(p_AB[0], p_AB[1], "bo")
+    plt.plot(p_AC[0], p_AC[1], "ro")
 
     # Plot user provided position
-    plt.plot(p_ACplot[0], p_ACplot[1], 'kx', markersize=15)
+    plt.plot(p_ACplot[0], p_ACplot[1], "kx", markersize=15)
 
     # Set settings so things visualize nicely
     plt.xlim([-2.2, 2.2])
     plt.ylim([-2.2, 2.2])
-    plt.gca().set_aspect('equal', adjustable='box')
+    plt.gca().set_aspect("equal", adjustable="box")
```

### Comparing `manipulation-2022.9.23/manipulation/exercises/pick/test_planar_manipulator.py` & `manipulation-2023.5.29/manipulation/exercises/pick/test_planar_manipulator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import unittest
 import timeout_decorator
 from gradescope_utils.autograder_utils.decorators import weight
-import pydrake.symbolic as ps
 import numpy as np
 
 
 class TestPlanarManipulator(unittest.TestCase):
-
     def __init__(self, test_name, notebook_locals):
         super().__init__(test_name)
         self.notebook_locals = notebook_locals
 
     @weight(2)
-    @timeout_decorator.timeout(1.)
+    @timeout_decorator.timeout(1.0)
     def test_forward_kinematics(self):
         """Test forward kinematics"""
         f = self.notebook_locals["forward_kinematics"]
 
         # yapf: disable
         f_target = np.array(  # noqa
             [[1.50622542e+00, -3.24106720e-01],
@@ -41,25 +39,27 @@
              [-3.16654300e-01, -1.25453082e+00]])
         # yapf: enable
 
         np.random.seed(7)
         n_rands = 20
         f_eval = []
         for i in range(n_rands):
-            q = 2. * np.pi * np.random.rand(2)
+            q = 2.0 * np.pi * np.random.rand(2)
             f_eval.append(f(q))
 
         f_eval = np.array(f_eval).squeeze()
 
         self.assertLessEqual(
-            np.linalg.norm(f_target - np.stack(f_eval)), 1e-6,
-            'The forward kinematics implementation is not correct')
+            np.linalg.norm(f_target - np.stack(f_eval)),
+            1e-6,
+            "The forward kinematics implementation is not correct",
+        )
 
     @weight(2)
-    @timeout_decorator.timeout(1.)
+    @timeout_decorator.timeout(1.0)
     def test_jacobian(self):
         """Test jacobian"""
         f = self.notebook_locals["Jacobian"]
 
         # yapf: disable
         f_target = np.array(  # noqa
             [[[3.24106720e-01, 7.85406073e-01],
@@ -84,14 +84,17 @@
               [1.87023541e+00, 9.62207961e-01]]])
         # yapf: enable
 
         np.random.seed(7)
         n_rands = 10
         f_eval = []
         for i in range(n_rands):
-            q = 2. * np.pi * np.random.rand(2)
+            q = 2.0 * np.pi * np.random.rand(2)
             f_eval.append(f(q))
 
         f_eval = np.array(f_eval).squeeze()
 
-        self.assertLessEqual(np.linalg.norm(f_target - np.stack(f_eval)), 1e-6,
-                             'The Jacobian implementation is not correct')
+        self.assertLessEqual(
+            np.linalg.norm(f_target - np.stack(f_eval)),
+            1e-6,
+            "The Jacobian implementation is not correct",
+        )
```

### Comparing `manipulation-2022.9.23/manipulation/exercises/pick/test_rigid_transforms.py` & `manipulation-2023.5.29/manipulation/exercises/pick/test_rigid_transforms.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import unittest
 import timeout_decorator
 from gradescope_utils.autograder_utils.decorators import weight
 import numpy as np
-from pydrake.all import (PiecewiseQuaternionSlerp, PiecewisePolynomial,
-                         RigidTransform, RotationMatrix)
+from pydrake.all import (
+    RigidTransform,
+    RotationMatrix,
+)
 
 
 class TestRigidTransforms(unittest.TestCase):
-
     def __init__(self, test_name, notebook_locals):
         super().__init__(test_name)
         self.notebook_locals = notebook_locals
 
     @weight(1)
-    @timeout_decorator.timeout(1.)
+    @timeout_decorator.timeout(1.0)
     def test_X_WB(self):
         """Testing X_WB"""
-        f = self.notebook_locals['compute_X_WB']
+        f = self.notebook_locals["compute_X_WB"]
 
         # construct a test case
         theta1, theta2, theta3 = np.pi / 3.0, np.pi / 6.0, np.pi / 4.0
         R_WA = RotationMatrix.MakeXRotation(theta1)
         R_AB = RotationMatrix.MakeZRotation(theta2)
         R_CB = RotationMatrix.MakeYRotation(theta3)
 
@@ -32,18 +33,18 @@
         true_X_WB = X_WA.multiply(X_AB)
 
         test_result = test_X_WB.multiply(true_X_WB.inverse())
         test_result = test_result.GetAsMatrix4()
         self.assertTrue(np.allclose(test_result, np.eye(4)))
 
     @weight(1)
-    @timeout_decorator.timeout(1.)
+    @timeout_decorator.timeout(1.0)
     def test_X_CW(self):
         """Testing X_CW"""
-        f = self.notebook_locals['compute_X_CW']
+        f = self.notebook_locals["compute_X_CW"]
 
         # construct a test case
         theta1, theta2, theta3 = np.pi / 3.0, np.pi / 6.0, np.pi / 4.0
         R_WA = RotationMatrix.MakeXRotation(theta1)
         R_AB = RotationMatrix.MakeZRotation(theta2)
         R_CB = RotationMatrix.MakeYRotation(theta3)
 
@@ -57,28 +58,28 @@
         test_X_CW = f(X_WA, X_AB, X_CB)
 
         test_result = true_X_CW.multiply(test_X_CW.inverse())
         test_result = test_result.GetAsMatrix4()
         self.assertTrue(np.allclose(test_result, np.eye(4)))
 
     @weight(2)
-    @timeout_decorator.timeout(1.)
+    @timeout_decorator.timeout(1.0)
     def test_grasp_pose(self):
         """Testing grasp pose"""
-        f = self.notebook_locals['design_grasp_pose']
-        X_WO = self.notebook_locals['X_WO']
+        f = self.notebook_locals["design_grasp_pose"]
+        X_WO = self.notebook_locals["X_WO"]
 
         test_X_OG, test_X_WG = f(X_WO)
 
         R_OG = RotationMatrix(np.array([[0, 0, 1], [1, 0, 0], [0, 1, 0]]).T)
         p_OG = [-0.02, 0, 0]
         X_OG = RigidTransform(R_OG, p_OG)
         X_WG = X_WO.multiply(X_OG)
 
-        test_X_CW = f(X_WO)
+        f(X_WO)
 
         test_result = test_X_OG.multiply(X_OG.inverse())
         test_result = test_result.GetAsMatrix4()
         self.assertTrue(np.allclose(test_result, np.eye(4)))
 
         test_result = test_X_WG.multiply(X_WG.inverse())
         test_result = test_result.GetAsMatrix4()
```

### Comparing `manipulation-2022.9.23/manipulation/exercises/pick/test_robot_painter.py` & `manipulation-2023.5.29/manipulation/exercises/pick/test_robot_painter.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,47 +1,50 @@
 import unittest
 import timeout_decorator
 from gradescope_utils.autograder_utils.decorators import weight
 import numpy as np
-from pydrake.all import (PiecewiseQuaternionSlerp, PiecewisePolynomial,
-                         ToleranceType)
 
 
 class TestRobotPainter(unittest.TestCase):
-
     def __init__(self, test_name, notebook_locals):
         super().__init__(test_name)
         self.notebook_locals = notebook_locals
 
     @weight(4)
-    @timeout_decorator.timeout(1.)
+    @timeout_decorator.timeout(1.0)
     def test_key_frames(self):
         """compose_circualr_key_frames"""
-        f = self.notebook_locals['compose_circular_key_frames']
-        X_WC = self.notebook_locals['X_WorldCenter']
-        X_WG = self.notebook_locals['X_WG']
-        radius = self.notebook_locals['radius']
-        thetas = self.notebook_locals['thetas']
+        f = self.notebook_locals["compose_circular_key_frames"]
+        X_WC = self.notebook_locals["X_WorldCenter"]
+        X_WG = self.notebook_locals["X_WG"]
+        radius = self.notebook_locals["radius"]
+        thetas = self.notebook_locals["thetas"]
         # carry out computation
         output_frames = f(thetas, X_WC, X_WG)
 
         # test all key positions match radius
         for i, frame_i in enumerate(output_frames):
             if i == 0:
                 # check if the first frame is the gripper's current frame
-                dist = np.linalg.norm(frame_i.translation()
-                                      - X_WG.translation())
-                self.assertLessEqual(dist, 1e-6,
-                                     'first key frame position incorrenct!')
+                dist = np.linalg.norm(
+                    frame_i.translation() - X_WG.translation()
+                )
+                self.assertLessEqual(
+                    dist, 1e-6, "first key frame position incorrenct!"
+                )
             else:
                 # check if the radius is correct
                 pos_cur = frame_i.translation()
                 r_cur = np.linalg.norm(pos_cur - X_WC.translation())
-                self.assertLessEqual(abs(radius - r_cur), 1e-6,
-                                     'key frame positions incorrenct!')
+                self.assertLessEqual(
+                    abs(radius - r_cur),
+                    1e-6,
+                    "key frame positions incorrenct!",
+                )
 
                 # check if +z of each frame points toward the center
                 z_cur = frame_i.rotation().matrix()[0:3, 2]
                 test_center = z_cur * radius + pos_cur
                 center_err = np.linalg.norm(test_center - X_WC.translation())
-                self.assertLessEqual(center_err, 1e-6,
-                                     'key frame orientations incorrect!')
+                self.assertLessEqual(
+                    center_err, 1e-6, "key frame orientations incorrect!"
+                )
```

### Comparing `manipulation-2022.9.23/manipulation/exercises/pick/test_simple_qp.py` & `manipulation-2023.5.29/manipulation/exercises/pick/test_simple_qp.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,41 @@
 import unittest
 import timeout_decorator
 from gradescope_utils.autograder_utils.decorators import weight
-import pydrake.symbolic as ps
 import numpy as np
 
 
 class TestSimpleQP(unittest.TestCase):
-
     def __init__(self, test_name, notebook_locals):
         super().__init__(test_name)
         self.notebook_locals = notebook_locals
 
     @weight(4)
-    @timeout_decorator.timeout(1.)
+    @timeout_decorator.timeout(1.0)
     def test_simple_qp(self):
         """Test Simple QP problem"""
         f = self.notebook_locals["result_submission"]
 
         # To test, prepare a random matrix so that we don't show the
         # answers directly.
         np.random.seed(7)
         crypt_mat = np.random.rand(8, 3)
         f_eval = crypt_mat.dot(f).squeeze()
 
-        f_target = np.array([
-            0.0868976, 0.19919438, 0.1619166, 0.28836804, 0.1513985, 0.27334388,
-            0.3473831, 0.31146061
-        ])
-
-        self.assertLessEqual(np.linalg.norm(f_target - np.stack(f_eval)), 1e-6,
-                             'The answer to the QP is not correct.')
+        f_target = np.array(
+            [
+                0.0868976,
+                0.19919438,
+                0.1619166,
+                0.28836804,
+                0.1513985,
+                0.27334388,
+                0.3473831,
+                0.31146061,
+            ]
+        )
+
+        self.assertLessEqual(
+            np.linalg.norm(f_target - np.stack(f_eval)),
+            1e-6,
+            "The answer to the QP is not correct.",
+        )
```

### Comparing `manipulation-2022.9.23/manipulation/exercises/pose/test_icp.py` & `manipulation-2023.5.29/manipulation/exercises/pose/test_icp.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import unittest
+
+import numpy as np
 import timeout_decorator
 from gradescope_utils.autograder_utils.decorators import weight
-import numpy as np
-from pydrake.all import (RigidTransform, RotationMatrix, RandomGenerator,
-                         UniformlyRandomRotationMatrix)
+from pydrake.all import (
+    RigidTransform,
+    RollPitchYaw,
+    RotationMatrix,
+)
 
 
 def least_squares_transform(scene, model):
     X_BA = RigidTransform()
     mu_m = np.mean(model, axis=1)
     mu_s = np.mean(scene, axis=1)
 
@@ -23,79 +27,93 @@
 
     X_BA.set_rotation(RotationMatrix(R_star))
     X_BA.set_translation(t_star)
 
     return X_BA
 
 
-def generate_random_transform(seed_num):
-    generator = RandomGenerator(seed_num)
-    R_BA = UniformlyRandomRotationMatrix(generator)
-    p_BA = np.random.RandomState(generator()).rand(3)
+def generate_arbitrary_transform(seed):
+    R_BA = RollPitchYaw(seed * 7.363, seed * 1.35, seed * 5.47)
+    p_BA = np.mod([seed * 2.13, seed * 3.3, seed * 5.225], 0.1) - 0.05
     X_BA = RigidTransform(R_BA, p_BA)
     return X_BA
 
 
 class TestICP(unittest.TestCase):
-
     def __init__(self, test_name, notebook_locals):
         super().__init__(test_name)
         self.notebook_locals = notebook_locals
 
         self.model = self.notebook_locals["pointcloud_model"]
 
     @weight(3)
-    @timeout_decorator.timeout(5.)
+    @timeout_decorator.timeout(5.0)
     def test_least_square(self):
         """Test least square transform"""
         f = self.notebook_locals["least_squares_transform"]
         nearest_neighbors = self.notebook_locals["nearest_neighbors"]
 
-        # Run a batter of tests determinisitcally, making sure the test cases
-        # include an impropoer rotation case.
+        # Run a battery of tests deterministically, making sure that the
+        # condition number of the data matrix (the singular values of W) are
+        # not too small.
         for i in range(10):
-            X_BA = generate_random_transform(i)
+            X_BA = generate_arbitrary_transform(i)
             self.scene = X_BA.multiply(self.model)
             distances, indices = nearest_neighbors(self.scene, self.model)
 
             X_BA_test = f(self.scene, self.model[:, indices])
-            X_BA_true = least_squares_transform(self.scene, self.model[:,
-                                                                       indices])
+            X_BA_true = least_squares_transform(
+                self.scene, self.model[:, indices]
+            )
 
             # check answer
             result = X_BA_true.inverse().multiply(X_BA_test)
 
-            self.assertTrue(np.allclose(result.GetAsMatrix4(), np.eye(4)),
-                            'least square transform is incorrect')
+            self.assertTrue(
+                np.allclose(result.GetAsMatrix4(), np.eye(4)),
+                "least square transform is incorrect",
+            )
+
+        # Test improper matrix
+        result = f(self.model, np.diag([1, 1, -1]) @ self.model)
+        self.assertTrue(
+            result.rotation().IsValid(),
+            "Your method returned an improper rotation matrix",
+        )
 
     @weight(3)
-    @timeout_decorator.timeout(5.)
+    @timeout_decorator.timeout(10.0)
     def test_icp(self):
         """Test icp implementation"""
         f = self.notebook_locals["icp"]
         nearest_neighbors = self.notebook_locals["nearest_neighbors"]
 
         # It should be sufficient to test only one for ICP.
-        X_BA = generate_random_transform(7)
+        X_BA = generate_arbitrary_transform(7)
         self.scene = X_BA.multiply(self.model)
         X_BA_test, mean_error_test, num_iters_test = f(self.scene, self.model)
         num_iters = 0
         mean_error = 0.0
         max_iterations = 20
         tolerance = 1e-3
         prev_error = 0
         X_BA = RigidTransform()
 
         while True:
             num_iters += 1
-            distances, indices = nearest_neighbors(self.scene,
-                                                   X_BA.multiply(self.model))
+            distances, indices = nearest_neighbors(
+                self.scene, X_BA.multiply(self.model)
+            )
             X_BA = least_squares_transform(self.scene, self.model[:, indices])
             mean_error = np.mean(distances)
-            if abs(mean_error
-                   - prev_error) < tolerance or num_iters >= max_iterations:
+            if (
+                abs(mean_error - prev_error) < tolerance
+                or num_iters >= max_iterations
+            ):
                 break
             prev_error = mean_error
 
         result = X_BA.multiply(X_BA_test.inverse())
-        self.assertTrue(np.allclose(result.GetAsMatrix4(), np.eye(4)),
-                        'icp implementation is incorrect')
+        self.assertTrue(
+            np.allclose(result.GetAsMatrix4(), np.eye(4)),
+            "icp implementation is incorrect",
+        )
```

### Comparing `manipulation-2022.9.23/manipulation/exercises/pose/test_ransac.py` & `manipulation-2023.5.29/manipulation/exercises/pose/test_ransac.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import unittest
 import timeout_decorator
 from gradescope_utils.autograder_utils.decorators import weight
 import numpy as np
-from pydrake.all import (RigidTransform, RotationMatrix, RandomGenerator)
 from copy import deepcopy
 
 
-def ransac_solution(point_cloud,
-                    model_fit_func,
-                    tolerance=1e-3,
-                    max_iterations=500):
+def ransac_solution(
+    point_cloud, model_fit_func, rng, tolerance=1e-3, max_iterations=500
+):
     """
     Args:
       point_cloud is (3, N) numpy array
       tolerance is a float
+      rng is a random number generator
       max_iterations is a (small) integer
       model_fit_func: the function to fit the model (point clouds)
 
     Returns:
       (4,) numpy array
     """
     best_ic = 0  # inlier count
@@ -25,64 +24,80 @@
     N = point_cloud.shape[1]  # number of points
 
     sample_size = 3
 
     point_cloud_1 = np.ones((N, 4))
     point_cloud_1[:, :3] = point_cloud.T
     for i in range(max_iterations):
-        s = point_cloud[:, np.random.randint(N, size=sample_size)]
+        s = point_cloud[:, rng.integers(0, N - 1, size=sample_size)]
         m = model_fit_func(s)
         abs_distances = np.abs(np.dot(m, point_cloud_1.T))  # 1 x N
         inliner_count = np.sum(abs_distances < tolerance)
 
         if inliner_count > best_ic:
             best_ic = inliner_count
             best_model = m
 
     return best_ic, best_model
 
 
 class TestRANSAC(unittest.TestCase):
-
     def __init__(self, test_name, notebook_locals):
         super().__init__(test_name)
         self.notebook_locals = notebook_locals
-        self.ransac_student = self.notebook_locals['ransac']
-        self.fit_plane = self.notebook_locals['fit_plane']
+        self.ransac_student = self.notebook_locals["ransac"]
+        self.fit_plane = self.notebook_locals["fit_plane"]
 
     @weight(4)
     @timeout_decorator.timeout(2.0)
     def test_ransac(self):
         """Test ransac method"""
-        simple_cloud = np.array([[0, 1, 0], [0, 0, 0], [1, 0, 0], [1, 1, 0],
-                                 [0.2, 0.5, 0], [2, 4, 1]]).T
-
-        _, plane_student = self.ransac_student(simple_cloud, self.fit_plane,
-                                               1e-5, 100)
-        _, plane_solution = ransac_solution(simple_cloud, self.fit_plane, 1e-5,
-                                            100)
-        self.assertTrue(np.array_equal(plane_solution, plane_student),
-                        "ransac implementation incorrect")
+        simple_cloud = np.array(
+            [
+                [0, 1, 0],
+                [0, 0, 0],
+                [1, 0, 0],
+                [1, 1, 0],
+                [0.2, 0.5, 0],
+                [2, 4, 1],
+            ]
+        ).T
+
+        rng = np.random.default_rng(135)
+        _, plane_student = self.ransac_student(
+            simple_cloud, self.fit_plane, rng, 1e-5, 100
+        )
+        rng = np.random.default_rng(135)
+        _, plane_solution = ransac_solution(
+            simple_cloud, self.fit_plane, rng, 1e-5, 100
+        )
+        self.assertTrue(
+            np.array_equal(plane_solution, plane_student),
+            "ransac implementation incorrect",
+        )
 
     @weight(2)
-    @timeout_decorator.timeout(2.0)
+    @timeout_decorator.timeout(8.0)
     def test_outlier_removal(self):
         """Test outlier removal"""
         # check whether outlier is in student's answer
-        remove_plane = self.notebook_locals['remove_plane']
-        bunny_w_plane = self.notebook_locals['bunny_w_plane']
+        remove_plane = self.notebook_locals["remove_plane"]
+        bunny_w_plane = self.notebook_locals["bunny_w_plane"]
         bunny_w_plane_copy = deepcopy(bunny_w_plane)
 
-        student_answer = remove_plane(bunny_w_plane,
-                                      self.ransac_student,
-                                      tol=1e-4)
+        rng = np.random.default_rng(135)
+        student_answer = remove_plane(
+            bunny_w_plane, self.ransac_student, rng, tol=1e-4
+        )
 
         outliers = []
         plane_equation = np.array([0.0, 0.0, 1.0, 0.0])
         dst = plane_equation[:3].dot(bunny_w_plane_copy) + plane_equation[3]
         for i in range(len(dst)):
             if abs(dst[i]) < 1e-6:
                 outliers.append(bunny_w_plane_copy[:, i])
         outliers = np.asarray(outliers)
         for pnt in student_answer.T:
-            self.assertTrue(not (pnt in outliers),
-                            "found unremoved points on the planar surface")
+            self.assertTrue(
+                not (pnt in outliers),
+                "found unremoved points on the planar surface",
+            )
```

### Comparing `manipulation-2022.9.23/manipulation/exercises/rl/test_stochastic_optimization.py` & `manipulation-2023.5.29/manipulation/exercises/rl/test_stochastic_optimization.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,89 +1,104 @@
 import unittest
 import timeout_decorator
 from gradescope_utils.autograder_utils.decorators import weight
 import numpy as np
-import os
 
 
 class TestStochasticOptimization(unittest.TestCase):
-
     def __init__(self, test_name, notebook_locals):
         super().__init__(test_name)
         self.notebook_locals = notebook_locals
         self.gradient_descent = self.notebook_locals["gradient_descent"]
 
     @weight(2)
-    @timeout_decorator.timeout(15.)
+    @timeout_decorator.timeout(15.0)
     def test_exact_gradient(self):
         """Test exact gradient function"""
         np.random.seed(7)
         exact_gradient = self.notebook_locals["exact_gradient"]
-        f_eval = self.gradient_descent(0.1,
-                                       exact_gradient,
-                                       initial_x=np.array([2., 2.]),
-                                       iter=5)
+        f_eval = self.gradient_descent(
+            0.1, exact_gradient, initial_x=np.array([2.0, 2.0]), iter=5
+        )
         f_eval = np.array(f_eval)
 
-        f_target = np.array([[2.000000, 2.000000, 2.466667],
-                             [1.790000, 1.850000, 1.961246],
-                             [1.707546, 1.712750, 1.723588],
-                             [1.653825, 1.584424, 1.539064],
-                             [1.614487, 1.463857, 1.384269],
-                             [1.584082, 1.350302, 1.250706]])
+        f_target = np.array(
+            [
+                [2.000000, 2.000000, 2.466667],
+                [1.790000, 1.850000, 1.961246],
+                [1.707546, 1.712750, 1.723588],
+                [1.653825, 1.584424, 1.539064],
+                [1.614487, 1.463857, 1.384269],
+                [1.584082, 1.350302, 1.250706],
+            ]
+        )
 
-        self.assertLessEqual(np.linalg.norm(f_target - f_eval), 1e-2,
-                             'You have wrong exact gradients.')
+        self.assertLessEqual(
+            np.linalg.norm(f_target - f_eval),
+            1e-2,
+            "You have wrong exact gradients.",
+        )
 
     @weight(2)
-    @timeout_decorator.timeout(15.)
+    @timeout_decorator.timeout(15.0)
     def test_approximated_gradient(self):
         """Test approximated gradient function"""
         np.random.seed(7)
         approximated_gradient = self.notebook_locals["approximated_gradient"]
-        f_eval = self.gradient_descent(0.1,
-                                       approximated_gradient,
-                                       initial_x=np.array([2., 2.]),
-                                       iter=5)
+        f_eval = self.gradient_descent(
+            0.1, approximated_gradient, initial_x=np.array([2.0, 2.0]), iter=5
+        )
         f_eval = np.array(f_eval)
 
-        f_target = np.array([[2.000000, 2.000000, 2.466667],
-                             [1.279693, 2.198529, 2.209571],
-                             [1.279187, 2.192247, 2.200421],
-                             [1.268846, 2.192274, 2.195393],
-                             [1.268799, 2.100353, 2.067566],
-                             [1.232492, 2.078929, 2.020906]])
+        f_target = np.array(
+            [
+                [2.000000, 2.000000, 2.466667],
+                [1.279693, 2.198529, 2.209571],
+                [1.279187, 2.192247, 2.200421],
+                [1.268846, 2.192274, 2.195393],
+                [1.268799, 2.100353, 2.067566],
+                [1.232492, 2.078929, 2.020906],
+            ]
+        )
 
-        self.assertLessEqual(np.linalg.norm(f_target - f_eval), 1e-2,
-                             'You have wrong approximated gradients.')
+        self.assertLessEqual(
+            np.linalg.norm(f_target - f_eval),
+            1e-2,
+            "You have wrong approximated gradients.",
+        )
 
     @weight(1)
-    @timeout_decorator.timeout(15.)
+    @timeout_decorator.timeout(15.0)
     def test_approximated_gradient_with_baseline(self):
         """Test approximated gradient with baseline function"""
         np.random.seed(7)
         approximated_gradient_with_baseline = self.notebook_locals[
-            "approximated_gradient_with_baseline"]
+            "approximated_gradient_with_baseline"
+        ]
 
         def baseline(x):
             return 5
 
         def reduced_function(x, rate):
             return approximated_gradient_with_baseline(x, rate, baseline)
 
-        f_eval = self.gradient_descent(0.1,
-                                       reduced_function,
-                                       initial_x=np.array([2., 2.]),
-                                       iter=5)
+        f_eval = self.gradient_descent(
+            0.1, reduced_function, initial_x=np.array([2.0, 2.0]), iter=5
+        )
         f_eval = np.array(f_eval)
 
-        f_target = np.array([[2.000000, 2.000000, 2.466667],
-                             [1.493827, 2.139510, 2.214994],
-                             [1.497885, 2.189906, 2.289990],
-                             [1.383463, 2.190205, 2.244283],
-                             [1.383293, 1.854385, 1.788513],
-                             [1.509619, 1.928927, 1.927494]])
+        f_target = np.array(
+            [
+                [2.000000, 2.000000, 2.466667],
+                [1.493827, 2.139510, 2.214994],
+                [1.497885, 2.189906, 2.289990],
+                [1.383463, 2.190205, 2.244283],
+                [1.383293, 1.854385, 1.788513],
+                [1.509619, 1.928927, 1.927494],
+            ]
+        )
 
         self.assertLessEqual(
-            np.linalg.norm(f_target - f_eval), 1e-2,
-            'You have wrong approixmated gradients'
-            'with baseline')
+            np.linalg.norm(f_target - f_eval),
+            1e-2,
+            "You have wrong approixmated gradients" "with baseline",
+        )
```

### Comparing `manipulation-2022.9.23/manipulation/exercises/rl/test_vpg.py` & `manipulation-2023.5.29/manipulation/exercises/rl/test_vpg.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,76 +2,81 @@
 import timeout_decorator
 from gradescope_utils.autograder_utils.decorators import weight
 import torch
 from torch.nn.functional import l1_loss
 
 
 class TestVPG(unittest.TestCase):
-
     def __init__(self, test_name, notebook_locals):
         super().__init__(test_name)
         self.notebook_locals = notebook_locals
 
     @weight(2)
     @timeout_decorator.timeout(60.0)
     def test_policy_loss(self):
         """Testing the policy loss"""
-        PolicyEstimator = self.notebook_locals['PolicyEstimator']
-        student_policy_loss = self.notebook_locals['util_compute_policy_loss']
+        PolicyEstimator = self.notebook_locals["PolicyEstimator"]
+        student_policy_loss = self.notebook_locals["util_compute_policy_loss"]
         obs = torch.ones(3, 2) * 2.0
         actions = torch.ones(3, 1) * 3.0
         returns = torch.arange(3, 6).float()
-        policy_f = PolicyEstimator(num_hidden=1,
-                                   hidden_dim=2,
-                                   obs_dim=2,
-                                   action_dim=1)
+        policy_f = PolicyEstimator(
+            num_hidden=1, hidden_dim=2, obs_dim=2, action_dim=1
+        )
         # initialize to constant values
         for p in policy_f.parameters():
             torch.nn.init.ones_(p)
         loss_student = student_policy_loss(policy_f, obs, actions, returns)
         self.assertTrue(
             torch.abs(loss_student - 7.6758) < 0.1,
-            'The policy loss computation is incorrect')
+            "The policy loss computation is incorrect",
+        )
 
     @weight(2)
     @timeout_decorator.timeout(60.0)
     def test_value_loss(self):
         """Testing the value loss"""
-        ValueEstimator = self.notebook_locals['ValueEstimator']
-        value_f = ValueEstimator(num_hidden=1,
-                                 hidden_dim=2,
-                                 obs_dim=2,
-                                 action_dim=1)
-        student_value_loss = self.notebook_locals['util_compute_value_loss']
+        ValueEstimator = self.notebook_locals["ValueEstimator"]
+        value_f = ValueEstimator(
+            num_hidden=1, hidden_dim=2, obs_dim=2, action_dim=1
+        )
+        student_value_loss = self.notebook_locals["util_compute_value_loss"]
         # initialize to constant values
         for p in value_f.parameters():
             torch.nn.init.ones_(p)
 
         # test tensors
         obs = torch.ones(3, 2) * 2.0
         returns = torch.arange(3, 6).float()
 
         loss_student = student_value_loss(value_f, obs, returns)
         self.assertTrue(
             torch.abs(loss_student - 2.0317) < 0.1,
-            'The value loss computation is incorrect')
+            "The value loss computation is incorrect",
+        )
 
     @weight(4)
     @timeout_decorator.timeout(60.0)
     def test_advantage_function(self):
         """Testing advantage function"""
-        compute_advantages = self.notebook_locals['compute_advantages']
+        compute_advantages = self.notebook_locals["compute_advantages"]
         discount = 0.99
         gae_lambda = 1.0
         max_episode_length = 2
         baselines = torch.FloatTensor([[1, 2, 3], [2, 1, 1]])
         rewards = torch.FloatTensor([[9, 8, 5], [6, 6, 6]])
-        student_sol = compute_advantages(discount, gae_lambda,
-                                         max_episode_length, baselines, rewards)
-        reference_sol = torch.FloatTensor([[20.8205, 10.9500, 0.0000],
-                                           [15.8206, 10.9400, 0.0000]])
-
-        l1_error = l1_loss(input=student_sol[:, :-1],
-                           target=reference_sol[:, :-1])
+        student_sol = compute_advantages(
+            discount, gae_lambda, max_episode_length, baselines, rewards
+        )
+        reference_sol = torch.FloatTensor(
+            [[20.8205, 10.9500, 0.0000], [15.8206, 10.9400, 0.0000]]
+        )
+
+        l1_error = l1_loss(
+            input=student_sol[:, :-1], target=reference_sol[:, :-1]
+        )
         print(l1_error)
-        self.assertLess(l1_error, 5.0, 'computation of the advantage '
-                        'function is incorrect')
+        self.assertLess(
+            l1_error,
+            5.0,
+            "computation of the advantage " "function is incorrect",
+        )
```

### Comparing `manipulation-2022.9.23/manipulation/exercises/robot/test_direct_joint_control.py` & `manipulation-2023.5.29/manipulation/exercises/robot/test_direct_joint_control.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 import unittest
 import timeout_decorator
 from gradescope_utils.autograder_utils.decorators import weight
 import numpy as np
 
 
 class TestDirectJointControl(unittest.TestCase):
-
     def __init__(self, test_name, notebook_locals):
         super().__init__(test_name)
         self.notebook_locals = notebook_locals
 
     @weight(5)
-    @timeout_decorator.timeout(1.)
+    @timeout_decorator.timeout(1.0)
     def test_position(self):
         """Test iiwa_position_measured"""
-        f = self.notebook_locals['teleop_2d_direct']
+        f = self.notebook_locals["teleop_2d_direct"]
 
         q_cmd = np.array([0.1, 0.2, 0.3])
         station, context = f(interactive=False, q_cmd=q_cmd)
-        self.assertIsNotNone(context, 'Incorrect context')
+        self.assertIsNotNone(context, "Incorrect context")
 
         station_context = station.GetMyContextFromRoot(context)
         commanded_pos = station.GetOutputPort("iiwa_position_commanded").Eval(
-            station_context)
+            station_context
+        )
 
-        self.assertLessEqual(np.linalg.norm(commanded_pos - q_cmd), 1e-3,
-                             'wrong commanded position')
+        self.assertLessEqual(
+            np.linalg.norm(commanded_pos - q_cmd),
+            1e-3,
+            "wrong commanded position",
+        )
```

### Comparing `manipulation-2022.9.23/manipulation/exercises/robot/test_manipulation_io.py` & `manipulation-2023.5.29/manipulation/exercises/robot/test_manipulation_io.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 import unittest
 import timeout_decorator
 from gradescope_utils.autograder_utils.decorators import weight
 import numpy as np
 
 
 class TestManipulationIO(unittest.TestCase):
-
     def __init__(self, test_name, notebook_locals):
         super().__init__(test_name)
         self.notebook_locals = notebook_locals
 
     @weight(5)
-    @timeout_decorator.timeout(1.)
+    @timeout_decorator.timeout(1.0)
     def test_dynamics(self):
         """Test get_velocity implementation"""
-        f = self.notebook_locals['get_velocity']
-        station = self.notebook_locals['station']
-        station_context = self.notebook_locals['station_context']
-        plant = self.notebook_locals['plant']
-        plant_context = self.notebook_locals['plant_context']
+        f = self.notebook_locals["get_velocity"]
+        station = self.notebook_locals["station"]
+        station_context = self.notebook_locals["station_context"]
+        plant = self.notebook_locals["plant"]
+        plant_context = self.notebook_locals["plant_context"]
         iiwa = plant.GetModelInstanceByName("iiwa")
 
         np.random.seed(7)
         for i in range(10):
             test_vel = np.random.rand(7)  # draw 7 random numbers
             plant.SetVelocities(plant_context, iiwa, test_vel)
             eval_vel = f(station, station_context)
-            self.assertLessEqual(np.linalg.norm(test_vel - eval_vel), 1e-6,
-                                 'get_velocity implementation is not correct!')
+            self.assertLessEqual(
+                np.linalg.norm(test_vel - eval_vel),
+                1e-6,
+                "get_velocity implementation is not correct!",
+            )
```

### Comparing `manipulation-2022.9.23/manipulation/exercises/robot/test_reflected_inertia.py` & `manipulation-2023.5.29/manipulation/exercises/robot/test_reflected_inertia.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,55 +2,60 @@
 import timeout_decorator
 from gradescope_utils.autograder_utils.decorators import weight
 import pydrake.symbolic as ps
 import numpy as np
 
 
 class TestSimplePendulumWithGearbox(unittest.TestCase):
-
     def __init__(self, test_name, notebook_locals):
         super().__init__(test_name)
         self.notebook_locals = notebook_locals
 
     @weight(5)
-    @timeout_decorator.timeout(1.)
+    @timeout_decorator.timeout(1.0)
     def test_dynamics(self):
         """Test state space dynamics"""
-        f = self.notebook_locals['pendulum_with_motor_dynamics']
+        f = self.notebook_locals["pendulum_with_motor_dynamics"]
 
         # Don't use local p since students might have different params.
         p = {"m": 1.0, "l": 0.5, "g": 9.81, "N": 160, "I": 3.46e-4}
 
-        f_target = np.array([[7.79918792e-01, 7.66080504e+00],
-                             [9.77989512e-01, 9.10363857e+00],
-                             [7.20511334e-02, 4.45713832e+00],
-                             [6.79229996e-01, 1.38617385e+01],
-                             [6.59363469e-02, 4.86183460e+00],
-                             [2.13385354e-01, 7.51773706e+00],
-                             [2.48992276e-02, 1.01181812e+01],
-                             [2.30302879e-01, 9.19761678e+00],
-                             [1.33169446e-01, 8.77027126e+00],
-                             [6.69013241e-01, 7.85009758e+00],
-                             [4.90765889e-01, 6.43240569e+00],
-                             [3.65890386e-01, 1.44728761e+01],
-                             [3.13994677e-01, 9.68534802e+00],
-                             [4.52842933e-01, 6.05424583e+00],
-                             [3.70351083e-01, 7.73613524e+00],
-                             [4.12991829e-01, 1.55689682e+01],
-                             [7.41118873e-01, 7.32350209e+00],
-                             [6.34379869e-01, 8.96351019e+00],
-                             [1.42688056e-03, 1.40375517e+00],
-                             [5.24345597e-01, 1.18791650e+01]])
+        f_target = np.array(
+            [
+                [7.79918792e-01, 7.66080504e00],
+                [9.77989512e-01, 9.10363857e00],
+                [7.20511334e-02, 4.45713832e00],
+                [6.79229996e-01, 1.38617385e01],
+                [6.59363469e-02, 4.86183460e00],
+                [2.13385354e-01, 7.51773706e00],
+                [2.48992276e-02, 1.01181812e01],
+                [2.30302879e-01, 9.19761678e00],
+                [1.33169446e-01, 8.77027126e00],
+                [6.69013241e-01, 7.85009758e00],
+                [4.90765889e-01, 6.43240569e00],
+                [3.65890386e-01, 1.44728761e01],
+                [3.13994677e-01, 9.68534802e00],
+                [4.52842933e-01, 6.05424583e00],
+                [3.70351083e-01, 7.73613524e00],
+                [4.12991829e-01, 1.55689682e01],
+                [7.41118873e-01, 7.32350209e00],
+                [6.34379869e-01, 8.96351019e00],
+                [1.42688056e-03, 1.40375517e00],
+                [5.24345597e-01, 1.18791650e01],
+            ]
+        )
 
         np.random.seed(7)
         n_rands = 20
         f_eval = []
         for i in range(n_rands):
             x = np.random.rand(2)
             u = np.random.rand(1)
             f_eval.append(ps.Evaluate(f(x, u, p)))
 
         f_eval = np.array(f_eval).squeeze()
 
         self.assertLessEqual(
-            np.linalg.norm(f_target - np.stack(f_eval)), 1e-6,
-            'The pendulum with motor dynamics are not corret.')
+            np.linalg.norm(f_target - np.stack(f_eval)),
+            1e-6,
+            "The pendulum with motor dynamics are not corret.",
+        )
```

### Comparing `manipulation-2022.9.23/manipulation/exercises/robot/test_survey.py` & `manipulation-2023.5.29/manipulation/exercises/robot/test_survey.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import unittest
 import timeout_decorator
 from gradescope_utils.autograder_utils.decorators import weight
-import numpy as np
 import hashlib
 
 
 class TestSurvey(unittest.TestCase):
-
     def __init__(self, test_name, notebook_locals):
         super().__init__(test_name)
         self.notebook_locals = notebook_locals
 
     @weight(1)
-    @timeout_decorator.timeout(1.)
+    @timeout_decorator.timeout(1.0)
     def test_dynamics(self):
         """Test Survey Code"""
-        survey_code = self.notebook_locals['survey_code']
-        m = hashlib.sha1(survey_code.encode('utf-8'))
-        self.assertEqual(m.hexdigest(),
-                         "415133a1dd0d559a2fbe766054892d0a6b16fee9",
-                         'wrong survey code!')
+        survey_code = self.notebook_locals["survey_code"]
+        m = hashlib.sha1(survey_code.encode("utf-8"))
+        self.assertEqual(
+            m.hexdigest(),
+            "415133a1dd0d559a2fbe766054892d0a6b16fee9",
+            "wrong survey code!",
+        )
```

### Comparing `manipulation-2022.9.23/manipulation/exercises/segmentation/test_mask.py` & `manipulation-2023.5.29/manipulation/exercises/segmentation/test_mask.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 import unittest
+
+import numpy as np
 import timeout_decorator
 from gradescope_utils.autograder_utils.decorators import weight
-import numpy as np
-from manipulation import FindResource
 
 
 def normalize(arr):
     rng = arr.max() - arr.min()
     amin = arr.min()
     return (arr - amin) * 255 / rng
 
 
 class TestMask(unittest.TestCase):
-
     def __init__(self, test_name, notebook_locals):
         super().__init__(test_name)
         self.notebook_locals = notebook_locals
 
     @weight(3)
     @timeout_decorator.timeout(60.0)
     def test_mask(self):
         """Testing deproject_pW_to_image"""
-        env = self.notebook_locals['env']
+        env = self.notebook_locals["env"]
 
         # compute the student solution
         cx, cy, fx, fy = env.get_intrinsics()
-        f = self.notebook_locals['deproject_pW_to_image']
-        p_W_mustard = self.notebook_locals['p_W_mustard']
-        X_WC = self.notebook_locals['X_WC']
+        f = self.notebook_locals["deproject_pW_to_image"]
+        p_W_mustard = self.notebook_locals["p_W_mustard"]
+        X_WC = self.notebook_locals["X_WC"]
         mask_student = f(p_W_mustard, cx, cy, fx, fy, X_WC)
         mask_sol = env.mask
 
-        self.assertTrue(mask_student.shape == mask_sol.shape,
-                        'the shape of the generated mask is incorrect')
+        self.assertTrue(
+            mask_student.shape == mask_sol.shape,
+            "the shape of the generated mask is incorrect",
+        )
 
         # normalize student's mask
         mask_student = normalize(mask_student)
-        mask_sol = normalize(mask_student)
+        mask_sol = normalize(mask_sol.astype(np.uint8))
         # quantify image difference
         difference = np.sum(np.abs(mask_student - mask_sol))
-        self.assertTrue(difference < 0.1 * 480 * 640,
-                        'Computed mask is incorrect')
+        self.assertTrue(
+            difference < 0.1 * 480 * 640, "Computed mask is incorrect"
+        )
```

### Comparing `manipulation-2022.9.23/manipulation/exercises/segmentation/test_segmentation_and_grasp.py` & `manipulation-2023.5.29/manipulation/exercises/segmentation/test_segmentation_and_grasp.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,67 @@
 import unittest
 import timeout_decorator
 from gradescope_utils.autograder_utils.decorators import weight
 import numpy as np
 from manipulation.utils import LoadDataResource
 
 
-class TestSegmentationAndGrasp(unittest.TestCase):
+def chamfer_dist(pc_a, pc_b):
+    """
+    pc_a of Size(N, 3)
+    pc_b of Size(M, 3)
+    """
+    diff = np.linalg.norm(pc_a[:, None] - pc_b[None], axis=2) ** 2
+    dist = np.mean(np.min(diff, axis=0)) + np.mean(np.min(diff, axis=1))
+    return dist
+
 
+class TestSegmentationAndGrasp(unittest.TestCase):
     def __init__(self, test_name, notebook_locals):
         super().__init__(test_name)
         self.notebook_locals = notebook_locals
 
     @weight(4)
-    @timeout_decorator.timeout(10.)
+    @timeout_decorator.timeout(10.0)
     def test_get_merged_masked_pcd(self):
         """Test find_antipodal_pts"""
         predictions = self.notebook_locals["predictions"]
         cameras = self.notebook_locals["cameras"]
         get_merged_masked_pcd = self.notebook_locals["get_merged_masked_pcd"]
 
         rgb_ims = [c.rgb_im for c in cameras]
         depth_ims = [c.depth_im for c in cameras]
         project_depth_to_pC_funcs = [c.project_depth_to_pC for c in cameras]
         X_WCs = [c.X_WC for c in cameras]
 
-        pcd_eval = get_merged_masked_pcd(predictions, rgb_ims, depth_ims, project_depth_to_pC_funcs, X_WCs)
-        pcd_pts_eval = np.asarray(pcd_eval.points)
-        pcd_colors_eval = np.asarray(pcd_eval.colors)
+        pcd_eval = get_merged_masked_pcd(
+            predictions, rgb_ims, depth_ims, project_depth_to_pC_funcs, X_WCs
+        )
+        pcd_pts_eval = np.asarray(pcd_eval.xyzs()[:])
+        pcd_colors_eval = np.asarray(pcd_eval.rgbs()[:])
+        pcd_pts_eval = pcd_pts_eval.T
         num_points_eval = pcd_pts_eval.shape[0]
 
         data_target = np.load(
-            LoadDataResource("segmentation_and_grasp_soln.npz"))
-        pcd_pts_target = data_target['points']
-        pcd_colors_target = data_target['colors']
+            LoadDataResource("segmentation_and_grasp_soln.npz")
+        )
+        pcd_pts_target = data_target["points"]
+        data_target["colors"]
         num_points_target = pcd_pts_target.shape[0]
 
         # Allow some deviation in the number of points
         self.assertLessEqual(
-            np.linalg.norm(num_points_target - num_points_eval), 200,
-            "Wrong number of points returned.")
+            np.linalg.norm(num_points_target - num_points_eval),
+            200,
+            "Wrong number of points returned.",
+        )
 
         # Make sure the sizes match
         min_num_pts = min(num_points_eval, num_points_target)
 
         self.assertLessEqual(
-            np.linalg.norm(pcd_pts_target[:min_num_pts,:] - pcd_pts_eval[:min_num_pts,:]), 1e-4,
-            "Point cloud points are not close enough to the solution values.")
-
-        self.assertLessEqual(
-            np.linalg.norm(pcd_colors_target[:min_num_pts,:] - pcd_colors_eval[:min_num_pts,:]), 1e-4,
-            "Point cloud colors are not close enough to the solution values.")
+            chamfer_dist(
+                pcd_pts_target[:min_num_pts, :], pcd_pts_eval[:min_num_pts, :]
+            ),
+            1e-4,
+            "Point cloud points are not close enough to the solution values.",
+        )
```

### Comparing `manipulation-2022.9.23/manipulation/exercises/trajectories/rrt_planner/geometry.py` & `manipulation-2023.5.29/manipulation/exercises/trajectories/rrt_planner/geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Written by Caelan Garrett, modified a bit by Tomas Lozano-Perez
 # yapf: disable
-from math import sqrt, cos, sin, atan2, pi
+from math import sqrt, cos, sin, atan2
 
 # Some utilities used in the class definitions, notably Polygon,
 
 
 # is exp near zero?
 def within(exp, threshold=.001):
     return abs(exp) < threshold
```

### Comparing `manipulation-2022.9.23/manipulation/exercises/trajectories/rrt_planner/iiwa_rrt_problem.py` & `manipulation-2023.5.29/manipulation/exercises/trajectories/rrt_planner/iiwa_rrt_problem.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 # %%
 import numpy as np
-from rrt_planner.manipulation_station_collision_checker import \
-    ManipulationStationCollisionChecker
+from rrt_planner.manipulation_station_collision_checker import (
+    ManipulationStationCollisionChecker,
+)
 from rrt_planner.robot import Range, ConfigurationSpace
 from rrt_planner.rrt_planning import Problem
 
 
 class IiwaProblem(Problem):
-
-    def __init__(self,
-                 q_start: np.array,
-                 q_goal: np.array,
-                 gripper_setpoint: float,
-                 left_door_angle: float,
-                 right_door_angle: float,
-                 is_visualizing=False):
+    def __init__(
+        self,
+        q_start: np.array,
+        q_goal: np.array,
+        gripper_setpoint: float,
+        left_door_angle: float,
+        right_door_angle: float,
+        is_visualizing=False,
+    ):
         self.gripper_setpoint = gripper_setpoint
         self.left_door_angle = left_door_angle
         self.right_door_angle = right_door_angle
         self.is_visualizing = is_visualizing
 
         self.collision_checker = ManipulationStationCollisionChecker(
-            is_visualizing=is_visualizing)
+            is_visualizing=is_visualizing
+        )
 
         # Construct configuration space for IIWA.
         plant = self.collision_checker.plant
         nq = 7
         joint_limits = np.zeros((nq, 2))
         for i in range(nq):
             joint = plant.GetJointByName("iiwa_joint_%i" % (i + 1))
@@ -50,56 +53,70 @@
             self,
             x=10,  # not used.
             y=10,  # not used.
             robot=None,  # not used.
             obstacles=None,  # not used.
             start=tuple(q_start),
             goal=tuple(q_goal),
-            cspace=cspace_iiwa)
+            cspace=cspace_iiwa,
+        )
 
     def collide(self, configuration):
         q = np.array(configuration)
-        return self.collision_checker.ExistsCollision(q, self.gripper_setpoint,
-                                                      self.left_door_angle,
-                                                      self.right_door_angle)
+        return self.collision_checker.ExistsCollision(
+            q,
+            self.gripper_setpoint,
+            self.left_door_angle,
+            self.right_door_angle,
+        )
 
     def run_planner(self, method: str):
         path = None
-        if method == 'rrt':
+        if method == "rrt":
             path = self.rrt_planning()
-        elif method == 'birrt':
+        elif method == "birrt":
             path = self.bidirectional_rrt_planning()
         else:
             raise NotImplementedError
 
         if path is None:
-            print('No path found')
+            print("No path found")
             return None
         else:
             print(
-                'Path found with ' + str(len(path) - 1)
-                + ' movements of distance ', self.path_distance(path))
+                "Path found with "
+                + str(len(path) - 1)
+                + " movements of distance ",
+                self.path_distance(path),
+            )
             smooth_path = self.smooth_path(path)
             print(
-                'Smoothed path found with ' + str(len(smooth_path) - 1)
-                + ' movements of distance ', self.path_distance(smooth_path))
+                "Smoothed path found with "
+                + str(len(smooth_path) - 1)
+                + " movements of distance ",
+                self.path_distance(smooth_path),
+            )
             # interpolated smooth path
             spath = []
             for i in range(1, len(smooth_path)):
                 spath.extend(
-                    self.cspace.path(smooth_path[i - 1], smooth_path[i]))
+                    self.cspace.path(smooth_path[i - 1], smooth_path[i])
+                )
 
             # make sure path is collision free
             if any([self.collide(c) for c in spath]):
-                print('Collision in smoothed path')
+                print("Collision in smoothed path")
                 return None
 
             return spath
 
     def visualize_path(self, path):
         # show path in meshcat
         for q in path:
             q = np.array(q)
-            self.collision_checker.DrawStation(q, self.gripper_setpoint,
-                                               self.left_door_angle,
-                                               self.right_door_angle)
+            self.collision_checker.DrawStation(
+                q,
+                self.gripper_setpoint,
+                self.left_door_angle,
+                self.right_door_angle,
+            )
             input("next?")
```

### Comparing `manipulation-2022.9.23/manipulation/exercises/trajectories/rrt_planner/robot.py` & `manipulation-2023.5.29/manipulation/exercises/trajectories/rrt_planner/robot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # yapf: disable
-from .geometry import Point, Pose, Polygon, Object
+from .geometry import Point, Pose, Object
 import random
 from math import ceil, sqrt
 
 
 class Robot:
     """A Robot is a set of convex polygons."""
```

### Comparing `manipulation-2022.9.23/manipulation/exercises/trajectories/rrt_planner/rrt_planning.py` & `manipulation-2023.5.29/manipulation/exercises/trajectories/rrt_planner/rrt_planning.py`

 * *Files identical despite different names*

### Comparing `manipulation-2022.9.23/manipulation/exercises/trajectories/test_door_opening.py` & `manipulation-2023.5.29/manipulation/exercises/trajectories/test_door_opening.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 import unittest
 import timeout_decorator
 from gradescope_utils.autograder_utils.decorators import weight
 import numpy as np
-import os
 
 
 class TestDoorOpening(unittest.TestCase):
-
     def __init__(self, test_name, notebook_locals):
         super().__init__(test_name)
         self.notebook_locals = notebook_locals
 
         simulator = self.notebook_locals["simulator"]
         station_plant = self.notebook_locals["station_plant"]
 
         context = simulator.get_context()
         door_angle = station_plant.GetPositions(
             station_plant.GetMyContextFromRoot(context),
-            station_plant.GetModelInstanceByName("cupboard"))
+            station_plant.GetModelInstanceByName("cupboard"),
+        )
 
         self.door_angle_deg = np.rad2deg(door_angle[1])
 
     @weight(2)
-    @timeout_decorator.timeout(15.)
+    @timeout_decorator.timeout(15.0)
     def test_ten_bound(self):
         """Test 10 degree bound for door angle"""
-        self.assertGreaterEqual(self.door_angle_deg, 10,
-                                "Door is not opened more than 10 degs.")
+        self.assertGreaterEqual(
+            self.door_angle_deg, 10, "Door is not opened more than 10 degs."
+        )
 
     @weight(2)
-    @timeout_decorator.timeout(15.)
+    @timeout_decorator.timeout(15.0)
     def test_forty_bound(self):
         """Test 40 degree bound for door angle"""
-        self.assertGreaterEqual(self.door_angle_deg, 40,
-                                "Door is not opened more than 40 degs.")
+        self.assertGreaterEqual(
+            self.door_angle_deg, 40, "Door is not opened more than 40 degs."
+        )
 
     @weight(1)
-    @timeout_decorator.timeout(15.)
+    @timeout_decorator.timeout(15.0)
     def test_seventy_bound(self):
         """Test 70 degree bound for door angle"""
-        self.assertGreaterEqual(self.door_angle_deg, 70,
-                                "Door is not opened more than 70 degs.")
+        self.assertGreaterEqual(
+            self.door_angle_deg, 70, "Door is not opened more than 70 degs."
+        )
```

### Comparing `manipulation-2022.9.23/manipulation/exercises/trajectories/test_rrt_planning.py` & `manipulation-2023.5.29/manipulation/exercises/trajectories/test_rrt_planning.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,59 +1,68 @@
 import unittest
 import timeout_decorator
 from gradescope_utils.autograder_utils.decorators import weight
 import numpy as np
 
 
 class TestRRT(unittest.TestCase):
-
     def __init__(self, test_name, notebook_locals):
         super().__init__(test_name)
         self.notebook_locals = notebook_locals
 
     @weight(5)
-    @timeout_decorator.timeout(60.)
+    @timeout_decorator.timeout(60.0)
     def test_rrt(self):
         """Test RRT Planner"""
         # construct a new problem
-        IKSolver = self.notebook_locals['IKSolver']
-        IiwaProblem = self.notebook_locals['IiwaProblem']
-        env = self.notebook_locals['env']
+        self.notebook_locals["IKSolver"]
+        IiwaProblem = self.notebook_locals["IiwaProblem"]
+        env = self.notebook_locals["env"]
 
         np.random.seed(0)
         q_init = env.q0
-        q_goal = self.notebook_locals['q_goal']
+        q_goal = self.notebook_locals["q_goal"]
 
         gripper_setpoint = 0.1
         left_door_angle = -np.pi / 2
         right_door_angle = np.pi / 2
 
-        iiwa_problem_test = IiwaProblem(q_start=q_init,
-                                        q_goal=q_goal,
-                                        gripper_setpoint=gripper_setpoint,
-                                        left_door_angle=left_door_angle,
-                                        right_door_angle=right_door_angle,
-                                        is_visualizing=False)
-        print('Constructed problem object')
+        iiwa_problem_test = IiwaProblem(
+            q_start=q_init,
+            q_goal=q_goal,
+            gripper_setpoint=gripper_setpoint,
+            left_door_angle=left_door_angle,
+            right_door_angle=right_door_angle,
+            is_visualizing=False,
+        )
+        print("Constructed problem object")
         # load student RRT method
-        student_rrt = self.notebook_locals['rrt_planning']
+        student_rrt = self.notebook_locals["rrt_planning"]
         student_path = None
-        print('Started to solve the problem using RRT planner ...')
+        print("Started to solve the problem using RRT planner ...")
         for i in range(3):  # allow 3 attempts
             student_path = student_rrt(iiwa_problem_test, 500, 0.5)
             if student_path is not None:
-                print('run 1 found a solution')
+                print("run 1 found a solution")
                 break
-            print('run {} fails to find a solution'.format(i))
-        self.assertTrue(expr=(student_path is not None),
-                        msg='computed path is None. This may imply that '
-                        'the RRT planner failse to find a solution '
-                        'out of 3 attempts.')
-        self.assertTrue(isinstance(student_path[-1], tuple),
-                        msg='please use tuple to store configurations.'
-                        'The computed path should be a list of tuples')
-        self.assertTrue(student_path[-1] == iiwa_problem_test.goal,
-                        msg='the last configuration of the path '
-                        'does not equal to goal.')
-        self.assertTrue(student_path[0] == iiwa_problem_test.start,
-                        msg='the first configuration of the path '
-                        'does not match start configuration')
+            print("run {} fails to find a solution".format(i))
+        self.assertTrue(
+            expr=(student_path is not None),
+            msg="computed path is None. This may imply that "
+            "the RRT planner failse to find a solution "
+            "out of 3 attempts.",
+        )
+        self.assertTrue(
+            isinstance(student_path[-1], tuple),
+            msg="please use tuple to store configurations."
+            "The computed path should be a list of tuples",
+        )
+        self.assertTrue(
+            student_path[-1] == iiwa_problem_test.goal,
+            msg="the last configuration of the path "
+            "does not equal to goal.",
+        )
+        self.assertTrue(
+            student_path[0] == iiwa_problem_test.start,
+            msg="the first configuration of the path "
+            "does not match start configuration",
+        )
```

### Comparing `manipulation-2022.9.23/manipulation/icp.py` & `manipulation-2023.5.29/manipulation/icp.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from pydrake.all import RigidTransform, RotationMatrix
+from pydrake.all import PointCloud, Rgba, RigidTransform, RotationMatrix
 from scipy.spatial import KDTree
 
 
 def PoseEstimationGivenCorrespondences(p_Om, p_s, chat):
     """Returns optimal X_O given the correspondences"""
     # Apply correspondences, and transpose data to support numpy broadcasting
     p_Omc = p_Om[:, chat].T
@@ -28,28 +28,27 @@
 
     # Compute p
     p = p_sbar - np.matmul(R, p_Ombar)
 
     return RigidTransform(RotationMatrix(R), p)
 
 
-def FindClosestPoints(point_cloud_A, point_cloud_B):
+def FindClosestPoints(kdtree_A, point_cloud_B):
     """
-    Finds the nearest (Euclidean) neighbor in point_cloud_B for each
-    point in point_cloud_A.
-    @param point_cloud_A A 3xN numpy array of points.
+    Finds the nearest (Euclidean) neighbor in kdtree_A for each
+    point in point_cloud_B.
+    @param kdtree_A A scipy KDTree containing point cloud A
     @param point_cloud_B A 3xN numpy array of points.
-    @return indices An (N, ) numpy array of the indices in point_cloud_B of each
-        point_cloud_A point's nearest neighbor.
+    @return indices An (N, ) numpy array of the indices in point_cloud_A of each
+        point_cloud_B point's nearest neighbor.
     """
-    indices = np.empty(point_cloud_A.shape[1], dtype=int)
+    indices = np.empty(point_cloud_B.shape[1], dtype=int)
 
-    kdtree = KDTree(point_cloud_B.T, copy_data=True)
-    for i in range(point_cloud_A.shape[1]):
-        distance, indices[i] = kdtree.query(point_cloud_A[:, i], k=1)
+    for i in range(point_cloud_B.shape[1]):
+        distance, indices[i] = kdtree_A.query(point_cloud_B[:, i], k=1)
 
     return indices
 
 
 def PrintResults(X_O, Xhat_O):
     p = X_O.translation()
     aa = X_O.rotation().ToAngleAxis()
@@ -57,31 +56,60 @@
     print(f"True orientation: {aa}")
     p = Xhat_O.translation()
     aa = Xhat_O.rotation().ToAngleAxis()
     print(f"Estimated position: {p}")
     print(f"Estimated orientation: {aa}")
 
 
-def IterativeClosestPoint(p_Om,
-                          p_s,
-                          X_O=None,
-                          meshcat=None,
-                          meshcat_scene_path=None):
-    Xhat = RigidTransform()
-    Nm = p_s.shape[1]
-    chat_previous = np.zeros(
-        Nm) - 1  # Set chat to a value that FindClosePoints will never return.
+def IterativeClosestPoint(
+    p_Om,
+    p_Ws,
+    X_Ohat=RigidTransform(),
+    X_O=None,
+    meshcat=None,
+    meshcat_scene_path=None,
+    max_iterations=None,
+):
+    """
+    Implements the vanilla ICP algorithm corresponding all scene points to a
+    model point.
+    @param p_Om A 3xN numpy array of "model" points in the model/object frame.
+    @param p_Ws A 3xN numpy array of "scene" points in the world frame.
+    @param X_Ohat An RigidTransform() containing the initial guess for X_O.
+    @param X_O The true, known, X_O; if provided, then the method will print a
+               comparison of the results.
+    @param meshcat a Meshcat instance for visualizing the point clouds.
+    @param meshcat_scene_path A string under which the point clouds will be
+                              published.
+    @return X_WOhat The estimated pose of the model in the world frame.
+    @return chat The indices of correspondences (and index into the model
+                 points) for each scene point.
+    """
+    Nm = p_Ws.shape[1]
+    # Set chat to a value that FindClosestPoints will never return.
+    chat_previous = np.zeros(Nm) - 1
+
+    kdtree_Om = KDTree(p_Om.T, copy_data=True)
+
+    if meshcat_scene_path:
+        cloud = PointCloud(p_Om.shape[1])
+        cloud.mutable_xyzs()[:] = p_Om
+        meshcat.SetObject(meshcat_scene_path, cloud, rgba=Rgba(0, 0, 1, 1))
 
+    iterations = 0
     while True:
-        chat = FindClosestPoints(p_s, Xhat.multiply(p_Om))
+        chat = FindClosestPoints(kdtree_Om, X_Ohat.inverse() @ p_Ws)
         if np.array_equal(chat, chat_previous):
             # Then I've converged.
             break
         chat_previous = chat
-        Xhat = PoseEstimationGivenCorrespondences(p_Om, p_s, chat)
+        X_Ohat = PoseEstimationGivenCorrespondences(p_Om, p_Ws, chat)
         if meshcat_scene_path:
-            meshcat.SetTransform(meshcat_scene_path, Xhat.inverse())
+            meshcat.SetTransform(meshcat_scene_path, X_Ohat)
+        iterations += 1
+        if max_iterations and iterations >= max_iterations:
+            break
 
     if X_O:
-        PrintResults(X_O, Xhat)
+        PrintResults(X_O, X_Ohat)
 
-    return Xhat, chat
+    return X_Ohat, chat
```

### Comparing `manipulation-2022.9.23/manipulation/meshcat_utils.py` & `manipulation-2023.5.29/manipulation/meshcat_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,24 @@
-import os
-import sys
 import time
 from collections import namedtuple
 from functools import partial
 
 import numpy as np
-from IPython.display import HTML, Javascript, display
 from pydrake.common.value import AbstractValue
-from pydrake.geometry import (Cylinder, MeshcatVisualizer,
-                              MeshcatVisualizerParams, Rgba, Role, Sphere)
+from pydrake.geometry import (
+    Cylinder,
+    Rgba,
+    Sphere,
+)
 from pydrake.math import RigidTransform, RollPitchYaw, RotationMatrix
-from pydrake.multibody.meshcat import JointSliders
-from pydrake.multibody.parsing import Parser
-from pydrake.multibody.plant import AddMultibodyPlantSceneGraph
-from pydrake.multibody.tree import BodyIndex, JointIndex
-from pydrake.perception import BaseField, Fields, PointCloud
-from pydrake.solvers.mathematicalprogram import BoundingBoxConstraint
-from pydrake.systems.framework import (DiagramBuilder, EventStatus, LeafSystem,
-                                       PublishEvent, VectorSystem)
+from pydrake.solvers import BoundingBoxConstraint
+from pydrake.systems.framework import (
+    EventStatus,
+    LeafSystem,
+)
 
 from manipulation import running_as_notebook
 
 # Some GUI code that will be moved into Drake.
 
 
 class MeshcatSliders(LeafSystem):
@@ -48,16 +45,18 @@
         """
         LeafSystem.__init__(self)
 
         self._meshcat = meshcat
         self._sliders = slider_names
         for i, slider_iterable in enumerate(self._sliders):
             port = self.DeclareVectorOutputPort(
-                f"slider_group_{i}", len(slider_iterable),
-                partial(self.DoCalcOutput, port_index=i))
+                f"slider_group_{i}",
+                len(slider_iterable),
+                partial(self.DoCalcOutput, port_index=i),
+            )
             port.disable_caching_by_default()
 
     def DoCalcOutput(self, context, output, port_index):
         for i, slider in enumerate(self._sliders[port_index]):
             output[i] = self._meshcat.GetSliderValue(slider)
 
 
@@ -75,41 +74,58 @@
         output_ports:
         - pose
 
     The optional `pose` input port is used ONLY at initialization; it can be
     used to set the initial pose e.g. from the current pose of a MultibodyPlant
     frame.
     """
+
     # TODO(russt): Use namedtuple defaults parameter once we are Python >= 3.7.
     Visible = namedtuple("Visible", ("roll", "pitch", "yaw", "x", "y", "z"))
     Visible.__new__.__defaults__ = (True, True, True, True, True, True)
     MinRange = namedtuple("MinRange", ("roll", "pitch", "yaw", "x", "y", "z"))
     MinRange.__new__.__defaults__ = (-np.pi, -np.pi, -np.pi, -1.0, -1.0, -1.0)
     MaxRange = namedtuple("MaxRange", ("roll", "pitch", "yaw", "x", "y", "z"))
     MaxRange.__new__.__defaults__ = (np.pi, np.pi, np.pi, 1.0, 1.0, 1.0)
     Value = namedtuple("Value", ("roll", "pitch", "yaw", "x", "y", "z"))
     Value.__new__.__defaults__ = (0.0, 0.0, 0.0, 0.0, 0.0, 0.0)
-    DecrementKey = namedtuple("DecrementKey",
-                              ("roll", "pitch", "yaw", "x", "y", "z"))
-    DecrementKey.__new__.__defaults__ = ("KeyQ", "KeyW", "KeyA", "KeyJ", "KeyI",
-                                         "KeyO")
-    IncrementKey = namedtuple("IncrementKey",
-                              ("roll", "pitch", "yaw", "x", "y", "z"))
-    IncrementKey.__new__.__defaults__ = ("KeyE", "KeyS", "KeyD", "KeyL", "KeyK",
-                                         "KeyU")
-
-    def __init__(self,
-                 meshcat,
-                 visible=Visible(),
-                 min_range=MinRange(),
-                 max_range=MaxRange(),
-                 value=Value(),
-                 decrement_keycode=DecrementKey(),
-                 increment_keycode=IncrementKey(),
-                 body_index=None):
+    DecrementKey = namedtuple(
+        "DecrementKey", ("roll", "pitch", "yaw", "x", "y", "z")
+    )
+    DecrementKey.__new__.__defaults__ = (
+        "KeyQ",
+        "KeyW",
+        "KeyA",
+        "KeyJ",
+        "KeyI",
+        "KeyO",
+    )
+    IncrementKey = namedtuple(
+        "IncrementKey", ("roll", "pitch", "yaw", "x", "y", "z")
+    )
+    IncrementKey.__new__.__defaults__ = (
+        "KeyE",
+        "KeyS",
+        "KeyD",
+        "KeyL",
+        "KeyK",
+        "KeyU",
+    )
+
+    def __init__(
+        self,
+        meshcat,
+        visible=Visible(),
+        min_range=MinRange(),
+        max_range=MaxRange(),
+        value=Value(),
+        decrement_keycode=DecrementKey(),
+        increment_keycode=IncrementKey(),
+        body_index=None,
+    ):
         """
         Args:
             meshcat: A Meshcat instance.
             visible: An object with boolean elements for 'roll', 'pitch',
                      'yaw', 'x', 'y', 'z'; the intention is for this to be the
                      PoseSliders.Visible() namedtuple.  Defaults to all true.
             min_range, max_range, value: Objects with float values for 'roll',
@@ -118,19 +134,22 @@
                       Value namedtuples.  See those tuples for default values.
             body_index: if the body_poses input port is connected, then this
                         index determine which pose is used to set the initial
                         slider positions during the Initialization event.
         """
         LeafSystem.__init__(self)
         port = self.DeclareAbstractOutputPort(
-            "pose", lambda: AbstractValue.Make(RigidTransform()),
-            self.DoCalcOutput)
-
-        self.DeclareAbstractInputPort("body_poses",
-                                      AbstractValue.Make([RigidTransform()]))
+            "pose",
+            lambda: AbstractValue.Make(RigidTransform()),
+            self.DoCalcOutput,
+        )
+
+        self.DeclareAbstractInputPort(
+            "body_poses", AbstractValue.Make([RigidTransform()])
+        )
         self.DeclareInitializationDiscreteUpdateEvent(self.Initialize)
 
         # The widgets themselves have undeclared state.  For now, we accept it,
         # and simply disable caching on the output port.
         # TODO(russt): consider implementing the more elaborate methods seen
         # in, e.g., LcmMessageSubscriber.
         port.disable_caching_by_default()
@@ -139,27 +158,29 @@
         self._visible = visible
         self._value = list(value)
         self._body_index = body_index
 
         print("Keyboard Controls:")
         for i in range(6):
             if visible[i]:
-                meshcat.AddSlider(min=min_range[i],
-                                  max=max_range[i],
-                                  value=value[i],
-                                  step=0.02,
-                                  name=value._fields[i],
-                                  decrement_keycode=decrement_keycode[i],
-                                  increment_keycode=increment_keycode[i])
+                meshcat.AddSlider(
+                    min=min_range[i],
+                    max=max_range[i],
+                    value=value[i],
+                    step=0.02,
+                    name=value._fields[i],
+                    decrement_keycode=decrement_keycode[i],
+                    increment_keycode=increment_keycode[i],
+                )
                 print(
                     f"{value._fields[i]} : {decrement_keycode[i]} / {increment_keycode[i]}"  # noqa
                 )
 
     def __del__(self):
-        for s in ['roll', 'pitch', 'yaw', 'x', 'y', 'z']:
+        for s in ["roll", "pitch", "yaw", "x", "y", "z"]:
             if visible[s]:
                 self._meshcat.DeleteSlider(s)
 
     def SetPose(self, pose):
         """
         Sets the current value of the sliders.
 
@@ -179,86 +200,92 @@
             rpy: An instance of drake.math.RollPitchYaw
         """
         self._value[0] = rpy.roll_angle()
         self._value[1] = rpy.pitch_angle()
         self._value[2] = rpy.yaw_angle()
         for i in range(3):
             if self._visible[i]:
-                self._meshcat.SetSliderValue(self._visible._fields[i],
-                                             self._value[i])
+                self._meshcat.SetSliderValue(
+                    self._visible._fields[i], self._value[i]
+                )
 
     def SetXyz(self, xyz):
         """
         Sets the current value of the sliders for x, y, and z.
 
         Args:
             xyz: A 3 element iterable object with x, y, z.
         """
         self._value[3:] = xyz
         for i in range(3, 6):
             if self._visible[i]:
-                self._meshcat.SetSliderValue(self._visible._fields[i],
-                                             self._value[i])
+                self._meshcat.SetSliderValue(
+                    self._visible._fields[i], self._value[i]
+                )
 
     def _update_values(self):
         changed = False
         for i in range(6):
             if self._visible[i]:
                 old_value = self._value[i]
                 self._value[i] = self._meshcat.GetSliderValue(
-                    self._visible._fields[i])
+                    self._visible._fields[i]
+                )
                 changed = changed or self._value[i] != old_value
         return changed
 
     def _get_transform(self):
         return RigidTransform(
             RollPitchYaw(self._value[0], self._value[1], self._value[2]),
-            self._value[3:])
+            self._value[3:],
+        )
 
     def DoCalcOutput(self, context, output):
         """Constructs the output values from the sliders."""
         self._update_values()
         output.set_value(self._get_transform())
 
     def Initialize(self, context, discrete_state):
         if self.get_input_port().HasValue(context):
             if self._body_index is None:
                 raise RuntimeError(
                     "If the `body_poses` input port is connected, then you "
-                    "must also pass a `body_index` to the constructor.")
+                    "must also pass a `body_index` to the constructor."
+                )
             self.SetPose(self.get_input_port().Eval(context)[self._body_index])
             return EventStatus.Succeeded()
         return EventStatus.DidNothing()
 
     def Run(self, publishing_system, root_context, callback):
-        # Calls callback(root_context, pose), then publishing_system.Publish()
-        # each time the sliders change value.
+        # Calls callback(root_context, pose), then
+        # publishing_system.ForcedPublish() each time the sliders change value.
         if not running_as_notebook:
             return
 
         publishing_context = publishing_system.GetMyContextFromRoot(
-            root_context)
+            root_context
+        )
 
         print("Press the 'Stop PoseSliders' button in Meshcat to continue.")
-        self._meshcat.AddButton("Stop PoseSliders")
+        self._meshcat.AddButton("Stop PoseSliders", "Escape")
         while self._meshcat.GetButtonClicks("Stop PoseSliders") < 1:
             if self._update_values():
                 callback(root_context, self._get_transform())
-                publishing_system.Publish(publishing_context)
-            time.sleep(.1)
+                publishing_system.ForcedPublish(publishing_context)
+            time.sleep(0.1)
 
         self._meshcat.DeleteButton("Stop PoseSliders")
 
 
 class WsgButton(LeafSystem):
-
     def __init__(self, meshcat):
         LeafSystem.__init__(self)
-        port = self.DeclareVectorOutputPort("wsg_position", 1,
-                                            self.DoCalcOutput)
+        port = self.DeclareVectorOutputPort(
+            "wsg_position", 1, self.DoCalcOutput
+        )
         port.disable_caching_by_default()
         self._meshcat = meshcat
         self._button = "Open/Close Gripper"
         meshcat.AddButton(self._button, "Space")
         print("Press Space to open/close the gripper")
 
     def __del__(self):
@@ -267,53 +294,57 @@
     def DoCalcOutput(self, context, output):
         position = 0.107  # open
         if (self._meshcat.GetButtonClicks(self._button) % 2) == 1:
             position = 0.002  # close
         output.SetAtIndex(0, position)
 
 
-def AddMeshcatTriad(meshcat,
-                    path,
-                    length=.25,
-                    radius=0.01,
-                    opacity=1.,
-                    X_PT=RigidTransform()):
+def AddMeshcatTriad(
+    meshcat, path, length=0.25, radius=0.01, opacity=1.0, X_PT=RigidTransform()
+):
     meshcat.SetTransform(path, X_PT)
     # x-axis
-    X_TG = RigidTransform(RotationMatrix.MakeYRotation(np.pi / 2),
-                          [length / 2., 0, 0])
+    X_TG = RigidTransform(
+        RotationMatrix.MakeYRotation(np.pi / 2), [length / 2.0, 0, 0]
+    )
     meshcat.SetTransform(path + "/x-axis", X_TG)
-    meshcat.SetObject(path + "/x-axis", Cylinder(radius, length),
-                      Rgba(1, 0, 0, opacity))
+    meshcat.SetObject(
+        path + "/x-axis", Cylinder(radius, length), Rgba(1, 0, 0, opacity)
+    )
 
     # y-axis
-    X_TG = RigidTransform(RotationMatrix.MakeXRotation(np.pi / 2),
-                          [0, length / 2., 0])
+    X_TG = RigidTransform(
+        RotationMatrix.MakeXRotation(np.pi / 2), [0, length / 2.0, 0]
+    )
     meshcat.SetTransform(path + "/y-axis", X_TG)
-    meshcat.SetObject(path + "/y-axis", Cylinder(radius, length),
-                      Rgba(0, 1, 0, opacity))
+    meshcat.SetObject(
+        path + "/y-axis", Cylinder(radius, length), Rgba(0, 1, 0, opacity)
+    )
 
     # z-axis
-    X_TG = RigidTransform([0, 0, length / 2.])
+    X_TG = RigidTransform([0, 0, length / 2.0])
     meshcat.SetTransform(path + "/z-axis", X_TG)
-    meshcat.SetObject(path + "/z-axis", Cylinder(radius, length),
-                      Rgba(0, 0, 1, opacity))
+    meshcat.SetObject(
+        path + "/z-axis", Cylinder(radius, length), Rgba(0, 0, 1, opacity)
+    )
 
 
-def plot_surface(meshcat,
-                 path,
-                 X,
-                 Y,
-                 Z,
-                 rgba=Rgba(.87, .6, .6, 1.0),
-                 wireframe=False,
-                 wireframe_line_width=1.0):
+def plot_surface(
+    meshcat,
+    path,
+    X,
+    Y,
+    Z,
+    rgba=Rgba(0.87, 0.6, 0.6, 1.0),
+    wireframe=False,
+    wireframe_line_width=1.0,
+):
     (rows, cols) = Z.shape
-    assert (np.array_equal(X.shape, Y.shape))
-    assert (np.array_equal(X.shape, Z.shape))
+    assert np.array_equal(X.shape, Y.shape)
+    assert np.array_equal(X.shape, Z.shape)
 
     vertices = np.empty((rows * cols, 3), dtype=np.float32)
     vertices[:, 0] = X.reshape((-1))
     vertices[:, 1] = Y.reshape((-1))
     vertices[:, 2] = Z.reshape((-1))
 
     # Vectorized faces code from https://stackoverflow.com/questions/44934631/making-grid-triangular-mesh-quickly-with-numpy  # noqa
@@ -323,29 +354,26 @@
     faces[:, :, 1, 0] = r[:-1, 1:]
     faces[:, :, 0, 1] = r[:-1, 1:]
     faces[:, :, 1, 1] = r[1:, 1:]
     faces[:, :, :, 2] = r[1:, :-1, None]
     faces.shape = (-1, 3)
 
     # TODO(Russ): support per vertex / Colormap colors.
-    meshcat.SetTriangleMesh(path, vertices.T, faces.T, rgba, wireframe,
-                            wireframe_line_width)
+    meshcat.SetTriangleMesh(
+        path, vertices.T, faces.T, rgba, wireframe, wireframe_line_width
+    )
 
 
-def plot_mathematical_program(meshcat,
-                              path,
-                              prog,
-                              X,
-                              Y,
-                              result=None,
-                              point_size=0.05):
+def plot_mathematical_program(
+    meshcat, path, prog, X, Y, result=None, point_size=0.05
+):
     assert prog.num_vars() == 2
     assert X.size == Y.size
 
-    N = X.size
+    X.size
     values = np.vstack((X.reshape(-1), Y.reshape(-1)))
     costs = prog.GetAllCosts()
 
     # Vectorized multiply for the quadratic form.
     # Z = (D*np.matmul(Q,D)).sum(0).reshape(nx, ny)
 
     if costs:
@@ -358,91 +386,90 @@
         if isinstance(binding.evaluator(), BoundingBoxConstraint):
             c = binding.evaluator()
             var_indices = [
                 int(prog.decision_variable_index()[v.get_id()])
                 for v in binding.variables()
             ]
             satisfied = np.array(
-                c.CheckSatisfiedVectorized(values[var_indices, :],
-                                           0.001)).reshape(1, -1)
+                c.CheckSatisfiedVectorized(values[var_indices, :], 0.001)
+            ).reshape(1, -1)
             if costs:
                 Z[~satisfied] = np.nan
 
             v = f"{cv}/{type(c).__name__}"
             Zc = np.zeros(Z.shape)
             Zc[satisfied] = np.nan
-            plot_surface(meshcat,
-                         v,
-                         X,
-                         Y,
-                         Zc.reshape(X.shape),
-                         rgba=Rgba(1.0, .2, .2, 1.0),
-                         wireframe=True)
+            plot_surface(
+                meshcat,
+                v,
+                X,
+                Y,
+                Zc.reshape(X.shape),
+                rgba=Rgba(1.0, 0.2, 0.2, 1.0),
+                wireframe=True,
+            )
         else:
             Zc = prog.EvalBindingVectorized(binding, values)
             evaluator = binding.evaluator()
             low = evaluator.lower_bound()
             up = evaluator.upper_bound()
             cvb = f"{cv}/{type(evaluator).__name__}"
             for index in range(Zc.shape[0]):
                 # TODO(russt): Plot infeasible points in a different color.
-                infeasible = np.logical_or(Zc[index, :] < low[index],
-                                           Zc[index, :] > up[index])
-                plot_surface(meshcat,
-                             f"{cvb}/{index}",
-                             X,
-                             Y,
-                             Zc[index, :].reshape(X.shape),
-                             rgba=Rgba(1.0, .3, 1.0, 1.0),
-                             wireframe=True)
+                infeasible = np.logical_or(
+                    Zc[index, :] < low[index], Zc[index, :] > up[index]
+                )
+                plot_surface(
+                    meshcat,
+                    f"{cvb}/{index}",
+                    X,
+                    Y,
+                    Zc[index, :].reshape(X.shape),
+                    rgba=Rgba(1.0, 0.3, 1.0, 1.0),
+                    wireframe=True,
+                )
 
     if costs:
-        plot_surface(meshcat,
-                     f"{path}/objective",
-                     X,
-                     Y,
-                     Z.reshape(X.shape),
-                     rgba=Rgba(.3, 1.0, .3, 1.0),
-                     wireframe=True)
+        plot_surface(
+            meshcat,
+            f"{path}/objective",
+            X,
+            Y,
+            Z.reshape(X.shape),
+            rgba=Rgba(0.3, 1.0, 0.3, 1.0),
+            wireframe=True,
+        )
 
     if result:
         v = f"{path}/solution"
-        meshcat.SetObject(v, Sphere(point_size), Rgba(.3, 1.0, .3, 1.0))
+        meshcat.SetObject(v, Sphere(point_size), Rgba(0.3, 1.0, 0.3, 1.0))
         x_solution = result.get_x_val()
         meshcat.SetTransform(
             v,
             RigidTransform(
-                [x_solution[0], x_solution[1],
-                 result.get_optimal_cost()]))
+                [x_solution[0], x_solution[1], result.get_optimal_cost()]
+            ),
+        )
+
+
+def PublishPositionTrajectory(
+    trajectory, root_context, plant, visualizer, time_step=1.0 / 33.0
+):
+    """
+    Args:
+        trajectory: A Trajectory instance.
+    """
+    plant_context = plant.GetMyContextFromRoot(root_context)
+    visualizer_context = visualizer.GetMyContextFromRoot(root_context)
+
+    visualizer.StartRecording(False)
 
+    for t in np.append(
+        np.arange(trajectory.start_time(), trajectory.end_time(), time_step),
+        trajectory.end_time(),
+    ):
+        root_context.SetTime(t)
+        plant.SetPositions(plant_context, trajectory.value(t))
+        visualizer.ForcedPublish(visualizer_context)
 
-# TODO(russt): Use the one true Drake version once this lands:
-# https://github.com/RobotLocomotion/drake/issues/17689
-def model_inspector(meshcat, filename):
-    builder = DiagramBuilder()
-
-    # Note: the time_step here is chosen arbitrarily.
-    plant, scene_graph = AddMultibodyPlantSceneGraph(builder, time_step=0.001)
-
-    # Load the file into the plant/scene_graph.
-    parser = Parser(plant)
-    parser.AddModelFromFile(filename)
-    plant.Finalize()
-
-    # Add two visualizers, one to publish the "visual" geometry, and one to
-    # publish the "collision" geometry.
-    visual = MeshcatVisualizer.AddToBuilder(
-        builder, scene_graph, meshcat,
-        MeshcatVisualizerParams(role=Role.kPerception, prefix="visual"))
-    collision = MeshcatVisualizer.AddToBuilder(
-        builder, scene_graph, meshcat,
-        MeshcatVisualizerParams(role=Role.kProximity, prefix="collision"))
-    # Disable the collision geometry at the start; it can be enabled by the
-    # checkbox in the meshcat controls.
-    meshcat.SetProperty("collision", "visible", False)
-
-    # Set the timeout to a small number in test mode. Otherwise, JointSliders
-    # will run until "Stop JointSliders" button is clicked.
-    default_interactive_timeout = None if running_as_notebook else 1.0
-    sliders = builder.AddSystem(JointSliders(meshcat, plant))
-    diagram = builder.Build()
-    sliders.Run(diagram, default_interactive_timeout)
+    visualizer.StopRecording()
+    visualizer.PublishRecording()
```

### Comparing `manipulation-2022.9.23/manipulation/models/061_foam_brick_w_visual_contact_spheres.sdf` & `manipulation-2023.5.29/manipulation/models/061_foam_brick_w_visual_contact_spheres.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2022.9.23/manipulation/models/bunny/bun_zipper_res2.ply` & `manipulation-2023.5.29/manipulation/models/bunny/bun_zipper_res2.ply`

 * *Files identical despite different names*

### Comparing `manipulation-2022.9.23/manipulation/models/camera_box.sdf` & `manipulation-2023.5.29/manipulation/models/camera_box.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2022.9.23/manipulation/models/double_pendulum.urdf` & `manipulation-2023.5.29/manipulation/models/double_pendulum.urdf`

 * *Files identical despite different names*

### Comparing `manipulation-2022.9.23/manipulation/models/iiwa_and_wsg.dmd.yaml` & `manipulation-2023.5.29/manipulation/models/iiwa_and_wsg.dmd.yaml`

 * *Files identical despite different names*

### Comparing `manipulation-2022.9.23/manipulation/models/mustard_w_cameras.yaml` & `manipulation-2023.5.29/manipulation/models/mustard_w_cameras.dmd.yaml`

 * *Files identical despite different names*

### Comparing `manipulation-2022.9.23/manipulation/models/planar_bin.sdf` & `manipulation-2023.5.29/manipulation/models/planar_bin.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2022.9.23/manipulation/models/planar_foam_brick_collision_as_visual.sdf` & `manipulation-2023.5.29/manipulation/models/planar_foam_brick_collision_as_visual.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2022.9.23/manipulation/models/schunk_wsg_50_welded_fingers.sdf` & `manipulation-2023.5.29/manipulation/models/schunk_wsg_50_welded_fingers.sdf`

 * *Files 4% similar despite different names*

#### Comparing `manipulation-2022.9.23/manipulation/models/schunk_wsg_50_welded_fingers.sdf` & `manipulation-2023.5.29/manipulation/models/schunk_wsg_50_welded_fingers.sdf`

```diff
@@ -15,15 +15,15 @@
           <izz>0.164814</izz>
         </inertia>
       </inertial>
       <visual name="visual">
         <geometry>
           <mesh>
             <scale>1 1 1</scale>
-            <uri>package://drake/manipulation/models/wsg_50_description/meshes/wsg_body.obj</uri>
+            <uri>package://drake_models/wsg_50_description/meshes/wsg_body.obj</uri>
           </mesh>
         </geometry>
         <material>
           <diffuse>0.7 0.7 0.7 1</diffuse>
         </material>
       </visual>
       <collision name="collision">
@@ -50,15 +50,15 @@
           <izz>0.16</izz>
         </inertia>
       </inertial>
       <visual name="visual">
         <geometry>
           <mesh>
             <scale>1 1 1</scale>
-            <uri>package://drake/manipulation/models/wsg_50_description/meshes/finger_without_tip.obj</uri>
+            <uri>package://drake_models/wsg_50_description/meshes/finger_without_tip.obj</uri>
           </mesh>
         </geometry>
         <material>
           <diffuse>0.2 0.2 0.2 1</diffuse>
         </material>
       </visual>
       <collision name="collision">
@@ -82,15 +82,15 @@
           <izz>0.16</izz>
         </inertia>
       </inertial>
       <visual name="visual">
         <geometry>
           <mesh>
             <scale>1 1 1</scale>
-            <uri>package://drake/manipulation/models/wsg_50_description/meshes/finger_without_tip.obj</uri>
+            <uri>package://drake_models/wsg_50_description/meshes/finger_without_tip.obj</uri>
           </mesh>
         </geometry>
         <material>
           <diffuse>0.2 0.2 0.2 1</diffuse>
         </material>
       </visual>
       <collision name="collision">
```

### Comparing `manipulation-2022.9.23/manipulation/models/segmentation_and_grasp_scene.yaml` & `manipulation-2023.5.29/manipulation/models/segmentation_and_grasp_scene.dmd.yaml`

 * *Files identical despite different names*

### Comparing `manipulation-2022.9.23/manipulation/models/shelves.sdf` & `manipulation-2023.5.29/manipulation/models/shelves.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2022.9.23/manipulation/models/two_bins.sdf` & `manipulation-2023.5.29/manipulation/models/two_bins.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2022.9.23/manipulation/models/two_bins.yaml` & `manipulation-2023.5.29/manipulation/models/two_bins.dmd.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -25,7 +25,17 @@
 - add_model:
     name: bin1
     file: package://drake/examples/manipulation_station/models/bin.sdf
 
 - add_weld:
     parent: bin1_origin
     child: bin1::bin_base
+
+- add_model:
+    name: floor
+    file: package://manipulation/floor.sdf
+
+- add_weld:
+    parent: world
+    child: floor::box
+    X_PC:
+        translation: [0, 0, -.5]
```

### Comparing `manipulation-2022.9.23/manipulation/models/two_bins_w_cameras.sdf` & `manipulation-2023.5.29/manipulation/models/two_bins_w_cameras.sdf`

 * *Files identical despite different names*

### Comparing `manipulation-2022.9.23/manipulation/models/two_bins_w_cameras.yaml` & `manipulation-2023.5.29/manipulation/models/two_bins_w_cameras.dmd.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 directives:
 - add_directives:
-    file: package://manipulation/two_bins.yaml
+    file: package://manipulation/two_bins.dmd.yaml
 
 - add_frame:
     name: camera0_origin
     X_PF:
         base_frame: world
         rotation: !Rpy { deg: [-130.0, 0, 90.0]}
         translation: [.25, -.5, .4]
```

### Comparing `manipulation-2022.9.23/manipulation/models/two_link_iiwa14.urdf` & `manipulation-2023.5.29/manipulation/models/two_link_iiwa14.urdf`

 * *Files 3% similar despite different names*

#### Comparing `manipulation-2022.9.23/manipulation/models/two_link_iiwa14.urdf` & `manipulation-2023.5.29/manipulation/models/two_link_iiwa14.urdf`

```diff
@@ -27,15 +27,15 @@
       <origin rpy="0 0 0" xyz="-0.1 0 0.07"/>
       <mass value="5"/>
       <inertia ixx="0.05" ixy="0" ixz="0" iyy="0.06" iyz="0" izz="0.03"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/manipulation/models/iiwa_description/meshes/visual/link_0.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_0.obj"/>
       </geometry>
       <material name="Grey"/>
     </visual>
     <collision>
       <origin rpy="0 0 0" xyz="-0.015 0 0.07"/>
       <geometry>
         <cylinder length="0.17" radius="0.139"/>
@@ -60,15 +60,15 @@
       <origin rpy="0 0 0" xyz="0 -0.03 0.12"/>
       <mass value="5.76"/>
       <inertia ixx="0.033" ixy="0" ixz="0" iyy="0.0333" iyz="0" izz="0.0123"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/manipulation/models/iiwa_description/meshes/visual/link_1.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_1.obj"/>
       </geometry>
       <material name="Grey"/>
     </visual>
     <collision>
       <origin rpy="0 0 0" xyz="0 -0.03344534434 0.1974815417"/>
       <geometry>
         <sphere radius="0.07959901601"/>
@@ -93,22 +93,22 @@
       <!-- 3.95 kuka CAD value-->
       <!--4 Original Drake URDF value-->
       <inertia ixx="0.0305" ixy="0" ixz="0" iyy="0.0304" iyz="0" izz="0.011"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/manipulation/models/iiwa_description/meshes/visual/link_2_orange.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_2_orange.obj"/>
       </geometry>
       <material name="Orange"/>
     </visual>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/manipulation/models/iiwa_description/meshes/visual/link_2_grey.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_2_grey.obj"/>
       </geometry>
       <material name="Grey"/>
     </visual>
     <collision>
       <origin rpy="0 0 0" xyz="-2.488800594e-017 0.203225991 -0.002065464272"/>
       <geometry>
         <sphere radius="0.06602481863"/>
@@ -136,29 +136,29 @@
       <!--3.18 kuka CAD value-->
       <!--3 Original Drake URDF value-->
       <inertia ixx="0.025" ixy="0" ixz="0" iyy="0.0238" iyz="0" izz="0.0076"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/manipulation/models/iiwa_description/meshes/visual/link_3.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_3.obj"/>
       </geometry>
       <material name="Grey"/>
     </visual>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/manipulation/models/iiwa_description/meshes/visual/band.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/band.obj"/>
       </geometry>
       <material name="Silver"/>
     </visual>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/manipulation/models/iiwa_description/meshes/visual/kuka.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/kuka.obj"/>
       </geometry>
       <material name="Black"/>
     </visual>
     <collision>
       <origin rpy="0 0 0" xyz="0 0 0.0355"/>
       <geometry>
         <sphere radius="0.075"/>
@@ -239,22 +239,22 @@
       <!--2.74 kuka CAD value-->
       <!--2.7 Original Drake URDF value-->
       <inertia ixx="0.017" ixy="0" ixz="0" iyy="0.0164" iyz="0" izz="0.006"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/manipulation/models/iiwa_description/meshes/visual/link_4_orange.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_4_orange.obj"/>
       </geometry>
       <material name="Orange"/>
     </visual>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/manipulation/models/iiwa_description/meshes/visual/link_4_grey.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_4_grey.obj"/>
       </geometry>
       <material name="Grey"/>
     </visual>
     <collision>
       <origin rpy="0 0 0" xyz="0 0.01 0.046"/>
       <geometry>
         <sphere radius="0.078"/>
@@ -310,29 +310,29 @@
       <!--1.69 kuka CAD value-->
       <!--1.7 Original Drake URDF value-->
       <inertia ixx="0.01" ixy="0" ixz="0" iyy="0.0087" iyz="0" izz="0.00449"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/manipulation/models/iiwa_description/meshes/visual/link_5.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_5.obj"/>
       </geometry>
       <material name="Grey"/>
     </visual>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/manipulation/models/iiwa_description/meshes/visual/band.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/band.obj"/>
       </geometry>
       <material name="Silver"/>
     </visual>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/manipulation/models/iiwa_description/meshes/visual/kuka.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/kuka.obj"/>
       </geometry>
       <material name="Black"/>
     </visual>
   </link>
   <!-- joint between link_5 and link_6 -->
   <joint name="iiwa_joint_6" type="fixed">
     <parent link="iiwa_link_5"/>
@@ -346,22 +346,22 @@
       <!--1.8 kuka CAD value-->
       <!--1.8 Original Drake URDF value-->
       <inertia ixx="0.0049" ixy="0" ixz="0" iyy="0.0047" iyz="0" izz="0.0036"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/manipulation/models/iiwa_description/meshes/visual/link_6_orange.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_6_orange.obj"/>
       </geometry>
       <material name="Orange"/>
     </visual>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/manipulation/models/iiwa_description/meshes/visual/link_6_grey.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_6_grey.obj"/>
       </geometry>
       <material name="Grey"/>
     </visual>
     <collision>
       <origin rpy="0 0 0" xyz="0 0 -0.059"/>
       <geometry>
         <sphere radius="0.055"/>
@@ -389,15 +389,15 @@
       <!--0.31 kuka CAD value-->
       <!--0.3 Original Drake URDF value-->
       <inertia ixx="0.001" ixy="0" ixz="0" iyy="0.001" iyz="0" izz="0.001"/>
     </inertial>
     <visual>
       <origin rpy="0 0 0" xyz="0 0 0"/>
       <geometry>
-        <mesh filename="package://drake/manipulation/models/iiwa_description/meshes/visual/link_7.obj"/>
+        <mesh filename="package://drake_models/iiwa_description/meshes/iiwa14/visual/link_7.obj"/>
       </geometry>
       <material name="Grey"/>
     </visual>
     <collision>
       <origin rpy="0 0 0" xyz="0 0 0.001"/>
       <geometry>
         <sphere radius="0.06"/>
```

### Comparing `manipulation-2022.9.23/manipulation/mustard_depth_camera_example.py` & `manipulation-2023.5.29/manipulation/mustard_depth_camera_example.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from pydrake.multibody.parsing import (Parser, ProcessModelDirectives,
-                                       LoadModelDirectives)
+from pydrake.multibody.parsing import Parser
 from pydrake.multibody.plant import AddMultibodyPlantSceneGraph
 from pydrake.perception import Concatenate
 from pydrake.systems.framework import DiagramBuilder
 
 from manipulation.scenarios import AddRgbdSensors
-from manipulation.utils import FindResource, AddPackagePaths
+from manipulation.utils import ConfigureParser
 
 
 def MustardExampleSystem():
     builder = DiagramBuilder()
 
     # Create the physics engine + scene graph.
     plant, scene_graph = AddMultibodyPlantSceneGraph(builder, time_step=0.0)
     parser = Parser(plant)
-    AddPackagePaths(parser)
-    ProcessModelDirectives(
-        LoadModelDirectives(FindResource("models/mustard_w_cameras.yaml")),
-        plant, parser)
-
+    ConfigureParser(parser)
+    parser.AddModelsFromUrl(
+        "package://manipulation/mustard_w_cameras.dmd.yaml"
+    )
     plant.Finalize()
 
     # Add a visualizer just to help us see the object.
     use_meshcat = False
     if use_meshcat:
         meshcat = builder.AddSystem(MeshcatVisualizer(scene_graph))
-        builder.Connect(scene_graph.get_query_output_port(),
-                        meshcat.get_geometry_query_input_port())
+        builder.Connect(
+            scene_graph.get_query_output_port(),
+            meshcat.get_geometry_query_input_port(),
+        )
 
     AddRgbdSensors(builder, plant, scene_graph)
 
     diagram = builder.Build()
     diagram.set_name("depth_camera_demo_system")
     return diagram
 
@@ -42,16 +42,17 @@
     plant_context = plant.GetMyMutableContextFromRoot(context)
 
     pcd = []
     for i in range(3):
         cloud = system.GetOutputPort(f"camera{i}_point_cloud").Eval(context)
 
         # Crop to region of interest.
-        pcd.append(cloud.Crop(lower_xyz=[-.3, -.3, -.3], upper_xyz=[.3, .3,
-                                                                    .3]))
+        pcd.append(
+            cloud.Crop(lower_xyz=[-0.3, -0.3, -0.3], upper_xyz=[0.3, 0.3, 0.3])
+        )
 
         if normals:
             pcd[i].EstimateNormals(radius=0.1, num_closest=30)
 
             camera = plant.GetModelInstanceByName(f"camera{i}")
             body = plant.GetBodyByName("base", camera)
             X_C = plant.EvalBodyPoseInWorld(plant_context, body)
```

### Comparing `manipulation-2022.9.23/manipulation/scenarios.py` & `manipulation-2023.5.29/manipulation/scenarios.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,44 +4,75 @@
 """
 import os
 import sys
 import warnings
 
 import numpy as np
 from pydrake.all import (
-    AbstractValue, Adder, AddMultibodyPlantSceneGraph, BallRpyJoint, BaseField,
-    Box, CameraInfo, ClippingRange, CoulombFriction, Cylinder, Demultiplexer,
-    DepthImageToPointCloud, DepthRange, DepthRenderCamera, DiagramBuilder,
-    FindResourceOrThrow, GeometryInstance, InverseDynamicsController,
-    LeafSystem, LoadModelDirectives, LoadModelDirectivesFromString,
-    MakeMultibodyStateToWsgStateSystem, MakePhongIllustrationProperties,
-    MakeRenderEngineVtk, ModelInstanceIndex, MultibodyPlant, Parser,
-    PassThrough, PrismaticJoint, ProcessModelDirectives, RenderCameraCore,
-    RenderEngineVtkParams, RevoluteJoint, Rgba, RgbdSensor, RigidTransform,
-    RollPitchYaw, RotationMatrix, SchunkWsgPositionController, SpatialInertia,
-    Sphere, StateInterpolatorWithDiscreteDerivative, UnitInertia)
-from pydrake.manipulation.planner import (
+    AbstractValue,
+    Adder,
+    AddMultibodyPlantSceneGraph,
+    BallRpyJoint,
+    BaseField,
+    Box,
+    CameraInfo,
+    Capsule,
+    ClippingRange,
+    CoulombFriction,
+    Cylinder,
+    Demultiplexer,
+    DepthImageToPointCloud,
+    DepthRange,
+    DepthRenderCamera,
+    DiagramBuilder,
     DifferentialInverseKinematicsIntegrator,
-    DifferentialInverseKinematicsParameters)
+    DifferentialInverseKinematicsParameters,
+    GeometryInstance,
+    InverseDynamicsController,
+    LeafSystem,
+    MakeMultibodyStateToWsgStateSystem,
+    MakePhongIllustrationProperties,
+    MakeRenderEngineVtk,
+    ModelInstanceIndex,
+    MultibodyPlant,
+    Parser,
+    PassThrough,
+    PrismaticJoint,
+    RenderCameraCore,
+    RenderEngineVtkParams,
+    RevoluteJoint,
+    Rgba,
+    RgbdSensor,
+    RigidTransform,
+    RollPitchYaw,
+    RotationMatrix,
+    SchunkWsgPositionController,
+    SpatialInertia,
+    Sphere,
+    StateInterpolatorWithDiscreteDerivative,
+    UnitInertia,
+)
 
-from manipulation.utils import AddPackagePaths, FindResource
+from manipulation.utils import ConfigureParser
 
 ycb = [
-    "003_cracker_box.sdf", "004_sugar_box.sdf", "005_tomato_soup_can.sdf",
-    "006_mustard_bottle.sdf", "009_gelatin_box.sdf", "010_potted_meat_can.sdf"
+    "003_cracker_box.sdf",
+    "004_sugar_box.sdf",
+    "005_tomato_soup_can.sdf",
+    "006_mustard_bottle.sdf",
+    "009_gelatin_box.sdf",
+    "010_potted_meat_can.sdf",
 ]
 
 
 def AddIiwa(plant, collision_model="no_collision"):
-    sdf_path = FindResourceOrThrow(
-        "drake/manipulation/models/iiwa_description/iiwa7/"
-        f"iiwa7_{collision_model}.sdf")
-
     parser = Parser(plant)
-    iiwa = parser.AddModelFromFile(sdf_path)
+    iiwa = parser.AddModelsFromUrl(
+        f"package://drake/manipulation/models/iiwa_description/iiwa7/iiwa7_{collision_model}.sdf"
+    )[0]
     plant.WeldFrames(plant.world_frame(), plant.GetFrameByName("iiwa_link_0"))
 
     # Set default positions:
     q0 = [0.0, 0.1, 0, -1.2, 0, 1.6, 0]
     index = 0
     for joint_index in plant.GetJointIndices(iiwa):
         joint = plant.get_mutable_joint(joint_index)
@@ -49,20 +80,18 @@
             joint.set_default_angle(q0[index])
             index += 1
 
     return iiwa
 
 
 def AddPlanarIiwa(plant):
-    urdf = FindResourceOrThrow(
-        "drake/manipulation/models/iiwa_description/urdf/"
-        "planar_iiwa14_spheres_dense_elbow_collision.urdf")
+    urdf = "package://drake/manipulation/models/iiwa_description/urdf/planar_iiwa14_spheres_dense_elbow_collision.urdf"
 
     parser = Parser(plant)
-    iiwa = parser.AddModelFromFile(urdf)
+    iiwa = parser.AddModelsFromUrl(urdf)[0]
     plant.WeldFrames(plant.world_frame(), plant.GetFrameByName("iiwa_link_0"))
 
     # Set default positions:
     q0 = [0.1, -1.2, 1.6]
     index = 0
     for joint_index in plant.GetJointIndices(iiwa):
         joint = plant.get_mutable_joint(joint_index)
@@ -70,276 +99,380 @@
             joint.set_default_angle(q0[index])
             index += 1
 
     return iiwa
 
 
 def AddTwoLinkIiwa(plant, q0=[0.1, -1.2]):
-    urdf = FindResource("models/two_link_iiwa14.urdf")
-
     parser = Parser(plant)
-    iiwa = parser.AddModelFromFile(urdf)
+    ConfigureParser(parser)
+    iiwa = parser.AddModelsFromUrl(
+        "package://manipulation/two_link_iiwa14.urdf"
+    )[0]
     plant.WeldFrames(plant.world_frame(), plant.GetFrameByName("iiwa_link_0"))
 
     # Set default positions:
     index = 0
     for joint_index in plant.GetJointIndices(iiwa):
         joint = plant.get_mutable_joint(joint_index)
         if isinstance(joint, RevoluteJoint):
             joint.set_default_angle(q0[index])
             index += 1
 
     return iiwa
 
 
 # TODO: take argument for whether we want the welded fingers version or not
-def AddWsg(plant, iiwa_model_instance, roll=np.pi / 2.0, welded=False):
+def AddWsg(
+    plant, iiwa_model_instance, roll=np.pi / 2.0, welded=False, sphere=False
+):
     parser = Parser(plant)
+    ConfigureParser(parser)
     if welded:
-        gripper = parser.AddModelFromFile(
-            FindResource("models/schunk_wsg_50_welded_fingers.sdf"), "gripper")
+        if sphere:
+            file = "package://manipulation/schunk_wsg_50_welded_fingers_sphere.sdf"
+        else:
+            file = "package://manipulation/schunk_wsg_50_welded_fingers.sdf"
     else:
-        gripper = parser.AddModelFromFile(
-            FindResourceOrThrow(
-                "drake/manipulation/models/"
-                "wsg_50_description/sdf/schunk_wsg_50_with_tip.sdf"))
+        file = "package://drake/manipulation/models/wsg_50_description/sdf/schunk_wsg_50_with_tip.sdf"
+
+    directives = f"""
+directives:
+- add_model:
+    name: gripper
+    file: {file}
+"""
+    gripper = parser.AddModelsFromString(directives, ".dmd.yaml")[0]
 
     X_7G = RigidTransform(RollPitchYaw(np.pi / 2.0, 0, roll), [0, 0, 0.09])
-    plant.WeldFrames(plant.GetFrameByName("iiwa_link_7", iiwa_model_instance),
-                     plant.GetFrameByName("body", gripper), X_7G)
+    plant.WeldFrames(
+        plant.GetFrameByName("iiwa_link_7", iiwa_model_instance),
+        plant.GetFrameByName("body", gripper),
+        X_7G,
+    )
     return gripper
 
 
-def AddFloatingRpyJoint(plant, frame, instance):
+def AddFloatingXyzJoint(plant, frame, instance, actuators=False):
     inertia = UnitInertia.SolidSphere(1.0)
     x_body = plant.AddRigidBody(
-        "x", instance,
-        SpatialInertia(mass=0, p_PScm_E=[0., 0., 0.], G_SP_E=inertia))
-    plant.AddJoint(
-        PrismaticJoint("x", plant.world_frame(), x_body.body_frame(),
-                       [1, 0, 0]))
+        "x",
+        instance,
+        SpatialInertia(mass=0, p_PScm_E=[0.0, 0.0, 0.0], G_SP_E=inertia),
+    )
+    x_joint = plant.AddJoint(
+        PrismaticJoint(
+            "x", plant.world_frame(), x_body.body_frame(), [1, 0, 0]
+        )
+    )
+    if actuators:
+        plant.AddJointActuator("x", x_joint)
     y_body = plant.AddRigidBody(
-        "y", instance,
-        SpatialInertia(mass=0, p_PScm_E=[0., 0., 0.], G_SP_E=inertia))
-    plant.AddJoint(
-        PrismaticJoint("y", x_body.body_frame(), y_body.body_frame(),
-                       [0, 1, 0]))
+        "y",
+        instance,
+        SpatialInertia(mass=0, p_PScm_E=[0.0, 0.0, 0.0], G_SP_E=inertia),
+    )
+    y_joint = plant.AddJoint(
+        PrismaticJoint(
+            "y", x_body.body_frame(), y_body.body_frame(), [0, 1, 0]
+        )
+    )
+    if actuators:
+        plant.AddJointActuator("y", y_joint)
+    z_joint = plant.AddJoint(
+        PrismaticJoint("z", y_body.body_frame(), frame, [0, 0, 1])
+    )
+    if actuators:
+        plant.AddJointActuator("z", z_joint)
+
+
+def AddFloatingRpyJoint(plant, frame, instance):
+    inertia = UnitInertia.SolidSphere(1.0)
     z_body = plant.AddRigidBody(
-        "z", instance,
-        SpatialInertia(mass=0, p_PScm_E=[0., 0., 0.], G_SP_E=inertia))
-    plant.AddJoint(
-        PrismaticJoint("z", y_body.body_frame(), z_body.body_frame(),
-                       [0, 0, 1]))
+        "z",
+        instance,
+        SpatialInertia(mass=0, p_PScm_E=[0.0, 0.0, 0.0], G_SP_E=inertia),
+    )
+    AddFloatingXyzJoint(plant, z_body.body_frame(), instance)
     plant.AddJoint(BallRpyJoint("ball", z_body.body_frame(), frame))
 
 
-def AddShape(plant, shape, name, mass=1, mu=1, color=[.5, .5, .9, 1.0]):
+def AddShape(plant, shape, name, mass=1, mu=1, color=[0.5, 0.5, 0.9, 1.0]):
     instance = plant.AddModelInstance(name)
     # TODO: Add a method to UnitInertia that accepts a geometry shape (unless
     # that dependency is somehow gross) and does this.
     if isinstance(shape, Box):
-        inertia = UnitInertia.SolidBox(shape.width(), shape.depth(),
-                                       shape.height())
+        inertia = UnitInertia.SolidBox(
+            shape.width(), shape.depth(), shape.height()
+        )
     elif isinstance(shape, Cylinder):
         inertia = UnitInertia.SolidCylinder(shape.radius(), shape.length())
     elif isinstance(shape, Sphere):
         inertia = UnitInertia.SolidSphere(shape.radius())
+    elif isinstance(shape, Capsule):
+        # TODO(russt): Add python bindings for SolidCapsule.
+        inertia = UnitInertia.SolidCylinder(shape.radius(), shape.length())
     else:
-        raise RunTimeError(
-            f"need to write the unit inertia for shapes of type {shape}")
+        raise RuntimeError(
+            f"need to write the unit inertia for shapes of type {shape}"
+        )
     body = plant.AddRigidBody(
-        name, instance,
-        SpatialInertia(mass=mass,
-                       p_PScm_E=np.array([0., 0., 0.]),
-                       G_SP_E=inertia))
+        name,
+        instance,
+        SpatialInertia(
+            mass=mass, p_PScm_E=np.array([0.0, 0.0, 0.0]), G_SP_E=inertia
+        ),
+    )
     if plant.geometry_source_is_registered():
         if isinstance(shape, Box):
             plant.RegisterCollisionGeometry(
-                body, RigidTransform(),
-                Box(shape.width() - 0.001,
+                body,
+                RigidTransform(),
+                Box(
+                    shape.width() - 0.001,
                     shape.depth() - 0.001,
-                    shape.height() - 0.001), name, CoulombFriction(mu, mu))
+                    shape.height() - 0.001,
+                ),
+                name,
+                CoulombFriction(mu, mu),
+            )
             i = 0
             for x in [-shape.width() / 2.0, shape.width() / 2.0]:
                 for y in [-shape.depth() / 2.0, shape.depth() / 2.0]:
                     for z in [-shape.height() / 2.0, shape.height() / 2.0]:
                         plant.RegisterCollisionGeometry(
-                            body, RigidTransform([x, y, z]),
-                            Sphere(radius=1e-7), f"contact_sphere{i}",
-                            CoulombFriction(mu, mu))
+                            body,
+                            RigidTransform([x, y, z]),
+                            Sphere(radius=1e-7),
+                            f"contact_sphere{i}",
+                            CoulombFriction(mu, mu),
+                        )
                         i += 1
         else:
-            plant.RegisterCollisionGeometry(body, RigidTransform(), shape, name,
-                                            CoulombFriction(mu, mu))
+            plant.RegisterCollisionGeometry(
+                body, RigidTransform(), shape, name, CoulombFriction(mu, mu)
+            )
 
-        plant.RegisterVisualGeometry(body, RigidTransform(), shape, name, color)
+        plant.RegisterVisualGeometry(
+            body, RigidTransform(), shape, name, color
+        )
 
     return instance
 
 
 # Add the camera_box.sdf.
 def AddCameraBox(plant, X_WC, name="camera0", parent_frame=None):
     # TODO(russt): could be smarter and increment the default camera name (by
     # checking with the plant).
     if not parent_frame:
         parent_frame = plant.world_frame()
-    camera = Parser(plant).AddModelFromFile(
-        FindResource("models/camera_box.sdf"), name)
+    parser = Plant(parser)
+    ConfigureParser(parser)
+    directives = f"""
+directives:
+- add_model:
+    name: {name}
+    file: package://manipulation/camera_box.sdf
+"""
+    camera = parser.AddModelsFromString(directives, ".dmd.yaml")
     plant.WeldFrames(parent_frame, plant.GetFrameByName("base", camera), X_WC)
 
 
 def AddCamera(builder, scene_graph, X_WC, depth_camera=None, renderer=None):
-    warnings.warn("Please use AddRgbdSensor instead.",
-                  warnings.DeprecationWarning)
+    warnings.warn(
+        "Please use AddRgbdSensor instead.", warnings.DeprecationWarning
+    )
     return AddRgbdSensor(builder, scene_graph, X_WC, depth_camera, renderer)
 
 
-def AddRgbdSensor(builder,
-                  scene_graph,
-                  X_PC,
-                  depth_camera=None,
-                  renderer=None,
-                  parent_frame_id=None):
+def AddRgbdSensor(
+    builder,
+    scene_graph,
+    X_PC,
+    depth_camera=None,
+    renderer=None,
+    parent_frame_id=None,
+):
     """
     Adds a RgbdSensor to to the scene_graph at (fixed) pose X_PC relative to
     the parent_frame.  If depth_camera is None, then a default camera info will
     be used.  If renderer is None, then we will assume the name 'my_renderer',
     and create a VTK renderer if a renderer of that name doesn't exist.  If
     parent_frame is None, then the world frame is used.
     """
     if sys.platform == "linux" and os.getenv("DISPLAY") is None:
         from pyvirtualdisplay import Display
+
         virtual_display = Display(visible=0, size=(1400, 900))
         virtual_display.start()
 
     if not renderer:
         renderer = "my_renderer"
 
     if not parent_frame_id:
         parent_frame_id = scene_graph.world_frame_id()
 
     if not scene_graph.HasRenderer(renderer):
-        scene_graph.AddRenderer(renderer,
-                                MakeRenderEngineVtk(RenderEngineVtkParams()))
+        scene_graph.AddRenderer(
+            renderer, MakeRenderEngineVtk(RenderEngineVtkParams())
+        )
 
     if not depth_camera:
         depth_camera = DepthRenderCamera(
             RenderCameraCore(
-                renderer, CameraInfo(width=640, height=480, fov_y=np.pi / 4.0),
-                ClippingRange(near=0.1, far=10.0), RigidTransform()),
-            DepthRange(0.1, 10.0))
+                renderer,
+                CameraInfo(width=640, height=480, fov_y=np.pi / 4.0),
+                ClippingRange(near=0.1, far=10.0),
+                RigidTransform(),
+            ),
+            DepthRange(0.1, 10.0),
+        )
 
     rgbd = builder.AddSystem(
-        RgbdSensor(parent_id=parent_frame_id,
-                   X_PB=X_PC,
-                   depth_camera=depth_camera,
-                   show_window=False))
-
-    builder.Connect(scene_graph.get_query_output_port(),
-                    rgbd.query_object_input_port())
+        RgbdSensor(
+            parent_id=parent_frame_id,
+            X_PB=X_PC,
+            depth_camera=depth_camera,
+            show_window=False,
+        )
+    )
+
+    builder.Connect(
+        scene_graph.get_query_output_port(), rgbd.query_object_input_port()
+    )
 
     return rgbd
 
 
-def AddRgbdSensors(builder,
-                   plant,
-                   scene_graph,
-                   also_add_point_clouds=True,
-                   model_instance_prefix="camera",
-                   depth_camera=None,
-                   renderer=None):
+def AddRgbdSensors(
+    builder,
+    plant,
+    scene_graph,
+    also_add_point_clouds=True,
+    model_instance_prefix="camera",
+    depth_camera=None,
+    renderer=None,
+):
     """
     Adds a RgbdSensor to the first body in the plant for every model instance
     with a name starting with model_instance_prefix.  If depth_camera is None,
     then a default camera info will be used.  If renderer is None, then we will
     assume the name 'my_renderer', and create a VTK renderer if a renderer of
     that name doesn't exist.
     """
     if sys.platform == "linux" and os.getenv("DISPLAY") is None:
         from pyvirtualdisplay import Display
+
         virtual_display = Display(visible=0, size=(1400, 900))
         virtual_display.start()
 
     if not renderer:
         renderer = "my_renderer"
 
     if not scene_graph.HasRenderer(renderer):
-        scene_graph.AddRenderer(renderer,
-                                MakeRenderEngineVtk(RenderEngineVtkParams()))
+        scene_graph.AddRenderer(
+            renderer, MakeRenderEngineVtk(RenderEngineVtkParams())
+        )
 
     if not depth_camera:
         depth_camera = DepthRenderCamera(
             RenderCameraCore(
-                renderer, CameraInfo(width=640, height=480, fov_y=np.pi / 4.0),
-                ClippingRange(near=0.1, far=10.0), RigidTransform()),
-            DepthRange(0.1, 10.0))
+                renderer,
+                CameraInfo(width=640, height=480, fov_y=np.pi / 4.0),
+                ClippingRange(near=0.1, far=10.0),
+                RigidTransform(),
+            ),
+            DepthRange(0.1, 10.0),
+        )
 
     for index in range(plant.num_model_instances()):
         model_instance_index = ModelInstanceIndex(index)
         model_name = plant.GetModelInstanceName(model_instance_index)
 
         if model_name.startswith(model_instance_prefix):
             body_index = plant.GetBodyIndices(model_instance_index)[0]
             rgbd = builder.AddSystem(
-                RgbdSensor(parent_id=plant.GetBodyFrameIdOrThrow(body_index),
-                           X_PB=RigidTransform(),
-                           depth_camera=depth_camera,
-                           show_window=False))
+                RgbdSensor(
+                    parent_id=plant.GetBodyFrameIdOrThrow(body_index),
+                    X_PB=RigidTransform(),
+                    depth_camera=depth_camera,
+                    show_window=False,
+                )
+            )
             rgbd.set_name(model_name)
 
-            builder.Connect(scene_graph.get_query_output_port(),
-                            rgbd.query_object_input_port())
+            builder.Connect(
+                scene_graph.get_query_output_port(),
+                rgbd.query_object_input_port(),
+            )
 
             # Export the camera outputs
-            builder.ExportOutput(rgbd.color_image_output_port(),
-                                 f"{model_name}_rgb_image")
-            builder.ExportOutput(rgbd.depth_image_32F_output_port(),
-                                 f"{model_name}_depth_image")
-            builder.ExportOutput(rgbd.label_image_output_port(),
-                                 f"{model_name}_label_image")
+            builder.ExportOutput(
+                rgbd.color_image_output_port(), f"{model_name}_rgb_image"
+            )
+            builder.ExportOutput(
+                rgbd.depth_image_32F_output_port(), f"{model_name}_depth_image"
+            )
+            builder.ExportOutput(
+                rgbd.label_image_output_port(), f"{model_name}_label_image"
+            )
 
             if also_add_point_clouds:
                 # Add a system to convert the camera output into a point cloud
                 to_point_cloud = builder.AddSystem(
-                    DepthImageToPointCloud(camera_info=rgbd.depth_camera_info(),
-                                           fields=BaseField.kXYZs
-                                           | BaseField.kRGBs))
-                builder.Connect(rgbd.depth_image_32F_output_port(),
-                                to_point_cloud.depth_image_input_port())
-                builder.Connect(rgbd.color_image_output_port(),
-                                to_point_cloud.color_image_input_port())
+                    DepthImageToPointCloud(
+                        camera_info=rgbd.depth_camera_info(),
+                        fields=BaseField.kXYZs | BaseField.kRGBs,
+                    )
+                )
+                builder.Connect(
+                    rgbd.depth_image_32F_output_port(),
+                    to_point_cloud.depth_image_input_port(),
+                )
+                builder.Connect(
+                    rgbd.color_image_output_port(),
+                    to_point_cloud.color_image_input_port(),
+                )
 
                 class ExtractBodyPose(LeafSystem):
-
                     def __init__(self, body_index):
                         LeafSystem.__init__(self)
                         self.body_index = body_index
                         self.DeclareAbstractInputPort(
                             "poses",
-                            plant.get_body_poses_output_port().Allocate())
+                            plant.get_body_poses_output_port().Allocate(),
+                        )
                         self.DeclareAbstractOutputPort(
                             "pose",
                             lambda: AbstractValue.Make(RigidTransform()),
-                            self.CalcOutput)
+                            self.CalcOutput,
+                        )
 
                     def CalcOutput(self, context, output):
                         poses = self.EvalAbstractInput(context, 0).get_value()
                         pose = poses[int(self.body_index)]
-                        output.get_mutable_value().set(pose.rotation(),
-                                                       pose.translation())
+                        output.get_mutable_value().set(
+                            pose.rotation(), pose.translation()
+                        )
 
                 camera_pose = builder.AddSystem(ExtractBodyPose(body_index))
-                builder.Connect(plant.get_body_poses_output_port(),
-                                camera_pose.get_input_port())
-                builder.Connect(camera_pose.get_output_port(),
-                                to_point_cloud.GetInputPort("camera_pose"))
+                builder.Connect(
+                    plant.get_body_poses_output_port(),
+                    camera_pose.get_input_port(),
+                )
+                builder.Connect(
+                    camera_pose.get_output_port(),
+                    to_point_cloud.GetInputPort("camera_pose"),
+                )
 
                 # Export the point cloud output.
-                builder.ExportOutput(to_point_cloud.point_cloud_output_port(),
-                                     f"{model_name}_point_cloud")
+                builder.ExportOutput(
+                    to_point_cloud.point_cloud_output_port(),
+                    f"{model_name}_point_cloud",
+                )
 
 
 def SetTransparency(scene_graph, alpha, source_id, geometry_ids=None):
     inspector = scene_graph.model_inspector()
     if not geometry_ids:
         geometry_ids = inspector.GetAllGeometryIds()
 
@@ -366,22 +499,24 @@
         props = inspector.GetIllustrationProperties(gid)
         if props is None or not props.HasProperty("phong", "diffuse"):
             continue
         new_color = Rgba(color[0], color[1], color[2], color[3])
         props.UpdateProperty("phong", "diffuse", new_color)
 
 
-def AddTriad(source_id,
-             frame_id,
-             scene_graph,
-             length=.25,
-             radius=0.01,
-             opacity=1.,
-             X_FT=RigidTransform(),
-             name="frame"):
+def AddTriad(
+    source_id,
+    frame_id,
+    scene_graph,
+    length=0.25,
+    radius=0.01,
+    opacity=1.0,
+    X_FT=RigidTransform(),
+    name="frame",
+):
     """
     Adds illustration geometry representing the coordinate frame, with the
     x-axis drawn in red, the y-axis in green and the z-axis in blue. The axes
     point in +x, +y and +z directions, respectively.
 
     Args:
       source_id: The source registered with SceneGraph.
@@ -390,80 +525,116 @@
       length: the length of each axis in meters.
       radius: the radius of each axis in meters.
       opacity: the opacity of the coordinate axes, between 0 and 1.
       X_FT: a RigidTransform from the triad frame T to the frame_id frame F
       name: the added geometry will have names name + " x-axis", etc.
     """
     # x-axis
-    X_TG = RigidTransform(RotationMatrix.MakeYRotation(np.pi / 2),
-                          [length / 2., 0, 0])
-    geom = GeometryInstance(X_FT.multiply(X_TG), Cylinder(radius, length),
-                            name + " x-axis")
+    X_TG = RigidTransform(
+        RotationMatrix.MakeYRotation(np.pi / 2), [length / 2.0, 0, 0]
+    )
+    geom = GeometryInstance(
+        X_FT.multiply(X_TG), Cylinder(radius, length), name + " x-axis"
+    )
     geom.set_illustration_properties(
-        MakePhongIllustrationProperties([1, 0, 0, opacity]))
+        MakePhongIllustrationProperties([1, 0, 0, opacity])
+    )
     scene_graph.RegisterGeometry(source_id, frame_id, geom)
 
     # y-axis
-    X_TG = RigidTransform(RotationMatrix.MakeXRotation(np.pi / 2),
-                          [0, length / 2., 0])
-    geom = GeometryInstance(X_FT.multiply(X_TG), Cylinder(radius, length),
-                            name + " y-axis")
+    X_TG = RigidTransform(
+        RotationMatrix.MakeXRotation(np.pi / 2), [0, length / 2.0, 0]
+    )
+    geom = GeometryInstance(
+        X_FT.multiply(X_TG), Cylinder(radius, length), name + " y-axis"
+    )
     geom.set_illustration_properties(
-        MakePhongIllustrationProperties([0, 1, 0, opacity]))
+        MakePhongIllustrationProperties([0, 1, 0, opacity])
+    )
     scene_graph.RegisterGeometry(source_id, frame_id, geom)
 
     # z-axis
-    X_TG = RigidTransform([0, 0, length / 2.])
-    geom = GeometryInstance(X_FT.multiply(X_TG), Cylinder(radius, length),
-                            name + " z-axis")
+    X_TG = RigidTransform([0, 0, length / 2.0])
+    geom = GeometryInstance(
+        X_FT.multiply(X_TG), Cylinder(radius, length), name + " z-axis"
+    )
     geom.set_illustration_properties(
-        MakePhongIllustrationProperties([0, 0, 1, opacity]))
+        MakePhongIllustrationProperties([0, 0, 1, opacity])
+    )
     scene_graph.RegisterGeometry(source_id, frame_id, geom)
 
 
-def AddMultibodyTriad(frame, scene_graph, length=.25, radius=0.01, opacity=1.):
+def AddMultibodyTriad(
+    frame, scene_graph, length=0.25, radius=0.01, opacity=1.0
+):
     plant = frame.GetParentPlant()
-    AddTriad(plant.get_source_id(),
-             plant.GetBodyFrameIdOrThrow(frame.body().index()), scene_graph,
-             length, radius, opacity, frame.GetFixedPoseInBodyFrame())
+    AddTriad(
+        plant.get_source_id(),
+        plant.GetBodyFrameIdOrThrow(frame.body().index()),
+        scene_graph,
+        length,
+        radius,
+        opacity,
+        frame.GetFixedPoseInBodyFrame(),
+    )
 
 
 def AddIiwaDifferentialIK(builder, plant, frame=None):
-    params = DifferentialInverseKinematicsParameters(plant.num_positions(),
-                                                     plant.num_velocities())
+    params = DifferentialInverseKinematicsParameters(
+        plant.num_positions(), plant.num_velocities()
+    )
     time_step = plant.time_step()
-    params.set_timestep(time_step)  # Not actually required.
     q0 = plant.GetPositions(plant.CreateDefaultContext())
     params.set_nominal_joint_position(q0)
+    params.set_end_effector_angular_speed_limit(2)
+    params.set_end_effector_translational_velocity_limits(
+        [-2, -2, -2], [2, 2, 2]
+    )
     if plant.num_positions() == 3:  # planar iiwa
         iiwa14_velocity_limits = np.array([1.4, 1.3, 2.3])
         params.set_joint_velocity_limits(
-            (-iiwa14_velocity_limits, iiwa14_velocity_limits))
-        # These constants are in body frame.
-        params.set_end_effector_velocity_gain([.1, 0, 0, 0, .1, .1])
+            (-iiwa14_velocity_limits, iiwa14_velocity_limits)
+        )
+        # These constants are in body frame
+        assert (
+            frame.name() == "iiwa_link_7"
+        ), "Still need to generalize the remaining planar diff IK params for different frames"  # noqa
+        params.set_end_effector_velocity_flag(
+            [True, False, False, True, False, True]
+        )
     else:
         iiwa14_velocity_limits = np.array([1.4, 1.4, 1.7, 1.3, 2.2, 2.3, 2.3])
         params.set_joint_velocity_limits(
-            (-iiwa14_velocity_limits, iiwa14_velocity_limits))
-        params.set_end_effector_velocity_gain([.1] * 6)
+            (-iiwa14_velocity_limits, iiwa14_velocity_limits)
+        )
+        params.set_joint_centering_gain(10 * np.eye(7))
     if frame is None:
         frame = plant.GetFrameByName("body")
     differential_ik = builder.AddSystem(
-        DifferentialInverseKinematicsIntegrator(plant, frame, time_step,
-                                                params))
+        DifferentialInverseKinematicsIntegrator(
+            plant,
+            frame,
+            time_step,
+            params,
+            log_only_when_result_state_changes=True,
+        )
+    )
     return differential_ik
 
 
-def MakeManipulationStation(model_directives=None,
-                            filename=None,
-                            time_step=0.002,
-                            iiwa_prefix="iiwa",
-                            wsg_prefix="wsg",
-                            camera_prefix="camera",
-                            package_xmls=[]):
+def MakeManipulationStation(
+    model_directives=None,
+    filename=None,
+    time_step=0.002,
+    iiwa_prefix="iiwa",
+    wsg_prefix="wsg",
+    camera_prefix="camera",
+    prefinalize_callback=None,
+    package_xmls=[],
+):
     """
     Creates a manipulation station system, which is a sub-diagram containing:
       - A MultibodyPlant with populated via the Parser from the
         `model_directives` argument AND the `filename` argument.
       - A SceneGraph
       - For each model instance starting with `iiwa_prefix`, we add an
         additional iiwa controller system
@@ -487,153 +658,212 @@
         wsg_prefix: Any model instance starting with `wsg_prefix` will get a
         schunk controller
 
         camera_prefix: Any bodies in the plant (created during the
         plant_setup_callback) starting with this prefix will get a camera
         attached.
 
+        prefinalize_callback: A function, setup(plant), that will be called
+        with the multibody plant before calling finalize.  This can be useful
+        for e.g. adding additional bodies/models to the simulation.
+
         package_xmls: A list of filenames to be passed to
         PackageMap.AddPackageXml().  This is useful if you need to add more
         models to your path (e.g. from your current working directory).
     """
     builder = DiagramBuilder()
 
     # Add (only) the iiwa, WSG, and cameras to the scene.
-    plant, scene_graph = AddMultibodyPlantSceneGraph(builder,
-                                                     time_step=time_step)
+    plant, scene_graph = AddMultibodyPlantSceneGraph(
+        builder, time_step=time_step
+    )
     parser = Parser(plant)
     for p in package_xmls:
         parser.package_map().AddPackageXml(p)
-    AddPackagePaths(parser)
+    ConfigureParser(parser)
     if model_directives:
-        directives = LoadModelDirectivesFromString(model_directives)
-        ProcessModelDirectives(directives, parser)
+        parser.AddModelsFromString(model_directives, ".dmd.yaml")
     if filename:
-        directives = LoadModelDirectives(filename)
-        ProcessModelDirectives(directives, parser)
+        parser.AddModelsFromUrl(filename)
+    if prefinalize_callback:
+        prefinalize_callback(plant)
     plant.Finalize()
 
     for i in range(plant.num_model_instances()):
         model_instance = ModelInstanceIndex(i)
         model_instance_name = plant.GetModelInstanceName(model_instance)
 
         if model_instance_name.startswith(iiwa_prefix):
             num_iiwa_positions = plant.num_positions(model_instance)
 
             # I need a PassThrough system so that I can export the input port.
             iiwa_position = builder.AddSystem(PassThrough(num_iiwa_positions))
-            builder.ExportInput(iiwa_position.get_input_port(),
-                                model_instance_name + "_position")
-            builder.ExportOutput(iiwa_position.get_output_port(),
-                                 model_instance_name + "_position_commanded")
+            builder.ExportInput(
+                iiwa_position.get_input_port(),
+                model_instance_name + "_position",
+            )
+            builder.ExportOutput(
+                iiwa_position.get_output_port(),
+                model_instance_name + "_position_commanded",
+            )
 
             # Export the iiwa "state" outputs.
             demux = builder.AddSystem(
-                Demultiplexer(2 * num_iiwa_positions, num_iiwa_positions))
-            builder.Connect(plant.get_state_output_port(model_instance),
-                            demux.get_input_port())
-            builder.ExportOutput(demux.get_output_port(0),
-                                 model_instance_name + "_position_measured")
-            builder.ExportOutput(demux.get_output_port(1),
-                                 model_instance_name + "_velocity_estimated")
-            builder.ExportOutput(plant.get_state_output_port(model_instance),
-                                 model_instance_name + "_state_estimated")
+                Demultiplexer(2 * num_iiwa_positions, num_iiwa_positions)
+            )
+            builder.Connect(
+                plant.get_state_output_port(model_instance),
+                demux.get_input_port(),
+            )
+            builder.ExportOutput(
+                demux.get_output_port(0),
+                model_instance_name + "_position_measured",
+            )
+            builder.ExportOutput(
+                demux.get_output_port(1),
+                model_instance_name + "_velocity_estimated",
+            )
+            builder.ExportOutput(
+                plant.get_state_output_port(model_instance),
+                model_instance_name + "_state_estimated",
+            )
 
             # Make the plant for the iiwa controller to use.
             controller_plant = MultibodyPlant(time_step=time_step)
             # TODO: Add the correct IIWA model (introspected from MBP)
             if plant.num_positions(model_instance) == 3:
                 controller_iiwa = AddPlanarIiwa(controller_plant)
             else:
                 controller_iiwa = AddIiwa(controller_plant)
             AddWsg(controller_plant, controller_iiwa, welded=True)
             controller_plant.Finalize()
 
             # Add the iiwa controller
             iiwa_controller = builder.AddSystem(
-                InverseDynamicsController(controller_plant,
-                                          kp=[100] * num_iiwa_positions,
-                                          ki=[1] * num_iiwa_positions,
-                                          kd=[20] * num_iiwa_positions,
-                                          has_reference_acceleration=False))
+                InverseDynamicsController(
+                    controller_plant,
+                    kp=[100] * num_iiwa_positions,
+                    ki=[1] * num_iiwa_positions,
+                    kd=[20] * num_iiwa_positions,
+                    has_reference_acceleration=False,
+                )
+            )
             iiwa_controller.set_name(model_instance_name + "_controller")
-            builder.Connect(plant.get_state_output_port(model_instance),
-                            iiwa_controller.get_input_port_estimated_state())
+            builder.Connect(
+                plant.get_state_output_port(model_instance),
+                iiwa_controller.get_input_port_estimated_state(),
+            )
 
             # Add in the feed-forward torque
             adder = builder.AddSystem(Adder(2, num_iiwa_positions))
-            builder.Connect(iiwa_controller.get_output_port_control(),
-                            adder.get_input_port(0))
+            builder.Connect(
+                iiwa_controller.get_output_port_control(),
+                adder.get_input_port(0),
+            )
             # Use a PassThrough to make the port optional (it will provide zero
             # values if not connected).
             torque_passthrough = builder.AddSystem(
-                PassThrough([0] * num_iiwa_positions))
-            builder.Connect(torque_passthrough.get_output_port(),
-                            adder.get_input_port(1))
-            builder.ExportInput(torque_passthrough.get_input_port(),
-                                model_instance_name + "_feedforward_torque")
-            builder.Connect(adder.get_output_port(),
-                            plant.get_actuation_input_port(model_instance))
+                PassThrough([0] * num_iiwa_positions)
+            )
+            builder.Connect(
+                torque_passthrough.get_output_port(), adder.get_input_port(1)
+            )
+            builder.ExportInput(
+                torque_passthrough.get_input_port(),
+                model_instance_name + "_feedforward_torque",
+            )
+            builder.Connect(
+                adder.get_output_port(),
+                plant.get_actuation_input_port(model_instance),
+            )
 
             # Add discrete derivative to command velocities.
             desired_state_from_position = builder.AddSystem(
                 StateInterpolatorWithDiscreteDerivative(
                     num_iiwa_positions,
                     time_step,
-                    suppress_initial_transient=True))
+                    suppress_initial_transient=True,
+                )
+            )
             desired_state_from_position.set_name(
-                model_instance_name + "_desired_state_from_position")
-            builder.Connect(desired_state_from_position.get_output_port(),
-                            iiwa_controller.get_input_port_desired_state())
-            builder.Connect(iiwa_position.get_output_port(),
-                            desired_state_from_position.get_input_port())
+                model_instance_name + "_desired_state_from_position"
+            )
+            builder.Connect(
+                desired_state_from_position.get_output_port(),
+                iiwa_controller.get_input_port_desired_state(),
+            )
+            builder.Connect(
+                iiwa_position.get_output_port(),
+                desired_state_from_position.get_input_port(),
+            )
 
             # Export commanded torques.
-            builder.ExportOutput(adder.get_output_port(),
-                                 model_instance_name + "_torque_commanded")
-            builder.ExportOutput(adder.get_output_port(),
-                                 model_instance_name + "_torque_measured")
+            builder.ExportOutput(
+                adder.get_output_port(),
+                model_instance_name + "_torque_commanded",
+            )
+            builder.ExportOutput(
+                adder.get_output_port(),
+                model_instance_name + "_torque_measured",
+            )
 
             builder.ExportOutput(
                 plant.get_generalized_contact_forces_output_port(
-                    model_instance), model_instance_name + "_torque_external")
+                    model_instance
+                ),
+                model_instance_name + "_torque_external",
+            )
 
         elif model_instance_name.startswith(wsg_prefix):
-
             # Wsg controller.
             wsg_controller = builder.AddSystem(SchunkWsgPositionController())
             wsg_controller.set_name(model_instance_name + "_controller")
-            builder.Connect(wsg_controller.get_generalized_force_output_port(),
-                            plant.get_actuation_input_port(model_instance))
-            builder.Connect(plant.get_state_output_port(model_instance),
-                            wsg_controller.get_state_input_port())
+            builder.Connect(
+                wsg_controller.get_generalized_force_output_port(),
+                plant.get_actuation_input_port(model_instance),
+            )
+            builder.Connect(
+                plant.get_state_output_port(model_instance),
+                wsg_controller.get_state_input_port(),
+            )
             builder.ExportInput(
                 wsg_controller.get_desired_position_input_port(),
-                model_instance_name + "_position")
-            builder.ExportInput(wsg_controller.get_force_limit_input_port(),
-                                model_instance_name + "_force_limit")
+                model_instance_name + "_position",
+            )
+            builder.ExportInput(
+                wsg_controller.get_force_limit_input_port(),
+                model_instance_name + "_force_limit",
+            )
             wsg_mbp_state_to_wsg_state = builder.AddSystem(
-                MakeMultibodyStateToWsgStateSystem())
-            builder.Connect(plant.get_state_output_port(model_instance),
-                            wsg_mbp_state_to_wsg_state.get_input_port())
-            builder.ExportOutput(wsg_mbp_state_to_wsg_state.get_output_port(),
-                                 model_instance_name + "_state_measured")
-            builder.ExportOutput(wsg_controller.get_grip_force_output_port(),
-                                 model_instance_name + "_force_measured")
+                MakeMultibodyStateToWsgStateSystem()
+            )
+            builder.Connect(
+                plant.get_state_output_port(model_instance),
+                wsg_mbp_state_to_wsg_state.get_input_port(),
+            )
+            builder.ExportOutput(
+                wsg_mbp_state_to_wsg_state.get_output_port(),
+                model_instance_name + "_state_measured",
+            )
+            builder.ExportOutput(
+                wsg_controller.get_grip_force_output_port(),
+                model_instance_name + "_force_measured",
+            )
 
     # Cameras.
-    AddRgbdSensors(builder,
-                   plant,
-                   scene_graph,
-                   model_instance_prefix=camera_prefix)
+    AddRgbdSensors(
+        builder, plant, scene_graph, model_instance_prefix=camera_prefix
+    )
 
     # Export "cheat" ports.
     builder.ExportOutput(scene_graph.get_query_output_port(), "query_object")
-    builder.ExportOutput(plant.get_contact_results_output_port(),
-                         "contact_results")
-    builder.ExportOutput(plant.get_state_output_port(),
-                         "plant_continuous_state")
+    builder.ExportOutput(
+        plant.get_contact_results_output_port(), "contact_results"
+    )
+    builder.ExportOutput(
+        plant.get_state_output_port(), "plant_continuous_state"
+    )
     builder.ExportOutput(plant.get_body_poses_output_port(), "body_poses")
 
     diagram = builder.Build()
     diagram.set_name("ManipulationStation")
     return diagram
```

### Comparing `manipulation-2022.9.23/manipulation/utils.py` & `manipulation-2023.5.29/manipulation/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,93 +1,115 @@
-import numpy as np
 import os
 import sys
 from urllib.request import urlretrieve
-from IPython import get_ipython
 
-import pydrake.all
-
-from pydrake.multibody.tree import JointIndex
+import numpy as np
+from IPython import get_ipython
+from pydrake.common import GetDrakePath
 from pydrake.common.containers import namedview
+from pydrake.geometry import RenderLabel
+from pydrake.multibody.tree import JointIndex
 
 # Use a global variable here because some calls to IPython will actually case an
 # interpreter to be created.  This file needs to be imported BEFORE that
 # happens.
-running_as_notebook = "COLAB_TESTING" not in os.environ and get_ipython(
-) and hasattr(get_ipython(), 'kernel')
+running_as_notebook = (
+    "COLAB_TESTING" not in os.environ
+    and get_ipython()
+    and hasattr(get_ipython(), "kernel")
+)
 
 running_as_test = False
 
 
 def set_running_as_test(value):
     global running_as_test
     running_as_test = value
 
 
 def pyplot_is_interactive():
     # import needs to happen after the backend is set.
     import matplotlib.pyplot as plt
     from matplotlib.rcsetup import interactive_bk
+
     return plt.get_backend() in interactive_bk
 
 
 def FindResource(filename):
     return os.path.join(os.path.dirname(__file__), filename)
 
 
 # A filename from the data directory.  Will download if necessary.
 def LoadDataResource(filename):
     data = os.path.join(os.path.dirname(os.path.dirname(__file__)), "data")
     if not os.path.exists(data):
         os.makedirs(data)
     path = os.path.join(data, filename)
     if not os.path.exists(path):
-        urlretrieve(f"https://manipulation.csail.mit.edu/data/{filename}", path)
+        print(f"{path} was not found locally; downloading it now...")
+        urlretrieve(
+            f"https://manipulation.csail.mit.edu/data/{filename}", path
+        )
     return path
 
 
+def ConfigureParser(parser):
+    """Add the manipulation/package.xml index to the given Parser."""
+    package_xml = os.path.join(os.path.dirname(__file__), "models/package.xml")
+    parser.package_map().AddPackageXml(filename=package_xml)
+    AddPackagePaths(parser)
+
+
 def AddPackagePaths(parser):
     # Remove once https://github.com/RobotLocomotion/drake/issues/10531 lands.
     parser.package_map().PopulateFromFolder(FindResource(""))
     parser.package_map().Add(
         "manipulation_station",
-        os.path.join(pydrake.common.GetDrakePath(),
-                     "examples/manipulation_station/models"))
+        os.path.join(
+            GetDrakePath(),
+            "examples/manipulation_station/models",
+        ),
+    )
     parser.package_map().Add(
         "ycb",
-        os.path.join(pydrake.common.GetDrakePath(), "manipulation/models/ycb"))
+        os.path.join(GetDrakePath(), "manipulation/models/ycb"),
+    )
     parser.package_map().Add(
         "wsg_50_description",
-        os.path.join(pydrake.common.GetDrakePath(),
-                     "manipulation/models/wsg_50_description"))
+        os.path.join(
+            GetDrakePath(),
+            "manipulation/models/wsg_50_description",
+        ),
+    )
 
 
 reserved_labels = [
-    pydrake.geometry.render.RenderLabel.kDoNotRender,
-    pydrake.geometry.render.RenderLabel.kDontCare,
-    pydrake.geometry.render.RenderLabel.kEmpty,
-    pydrake.geometry.render.RenderLabel.kUnspecified,
+    RenderLabel.kDoNotRender,
+    RenderLabel.kDontCare,
+    RenderLabel.kEmpty,
+    RenderLabel.kUnspecified,
 ]
 
 
 def colorize_labels(image):
     # import needs to happen after backend is set up.
-    import matplotlib.pyplot as plt
     import matplotlib as mpl
+    import matplotlib.pyplot as plt
+
     """Colorizes labels."""
     # TODO(eric.cousineau): Revive and use Kuni's palette.
     cc = mpl.colors.ColorConverter()
     color_cycle = plt.rcParams["axes.prop_cycle"]
     colors = np.array([cc.to_rgb(c["color"]) for c in color_cycle])
     bg_color = [0, 0, 0]
     image = np.squeeze(image)
     background = np.zeros(image.shape[:2], dtype=bool)
     for label in reserved_labels:
         background |= image == int(label)
-    foreground = image[np.logical_not(background)]
+    image[np.logical_not(background)]
     color_image = colors[image % len(colors)]
     color_image[background] = bg_color
     return color_image
 
 
 def SetupMatplotlibBackend(wishlist=["notebook"]):
     """
@@ -103,15 +125,15 @@
     # To find available backends, one can access the lists:
     # matplotlib.rcsetup.interactive_bk
     # matplotlib.rcsetup.non_interactive_bk
     # matplotlib.rcsetup.all_backends
     if running_as_notebook:
         ipython = get_ipython()
         # Short-circuit for google colab.
-        if 'google.colab' in sys.modules:
+        if "google.colab" in sys.modules:
             ipython.run_line_magic("matplotlib", "inline")
             return False
         # TODO: Find a way to detect vscode, and use inline instead of notebook
         for backend in wishlist:
             try:
                 ipython.run_line_magic("matplotlib", backend)
                 return pyplot_is_interactive()
@@ -120,51 +142,57 @@
         ipython.run_line_magic("matplotlib", "inline")
     return False
 
 
 # TODO(russt): promote these to drake (and make a version with model_instance)
 
 
-def MakeNamedViewPositions(mbp, view_name, add_suffix_if_single_position=False):
+def MakeNamedViewPositions(
+    mbp, view_name, add_suffix_if_single_position=False
+):
     names = [None] * mbp.num_positions()
     for ind in range(mbp.num_joints()):
         joint = mbp.get_joint(JointIndex(ind))
         if joint.num_positions() == 1 and not add_suffix_if_single_position:
             names[joint.position_start()] = joint.name()
         else:
             for i in range(joint.num_positions()):
-                names[joint.position_start() + i] = \
-                    f"{joint.name()}_{joint.position_suffix(i)}"
+                names[
+                    joint.position_start() + i
+                ] = f"{joint.name()}_{joint.position_suffix(i)}"
     for ind in mbp.GetFloatingBaseBodies():
         body = mbp.get_body(ind)
         start = body.floating_positions_start()
         for i in range(7):
-            names[start
-                  + i] = f"{body.name()}_{body.floating_position_suffix(i)}"
+            names[
+                start + i
+            ] = f"{body.name()}_{body.floating_position_suffix(i)}"
     return namedview(view_name, names)
 
 
-def MakeNamedViewVelocities(mbp,
-                            view_name,
-                            add_suffix_if_single_velocity=False):
+def MakeNamedViewVelocities(
+    mbp, view_name, add_suffix_if_single_velocity=False
+):
     names = [None] * mbp.num_velocities()
     for ind in range(mbp.num_joints()):
         joint = mbp.get_joint(JointIndex(ind))
         if joint.num_velocities() == 1 and not add_suffix_if_single_velocity:
             names[joint.velocity_start()] = joint.name()
         else:
             for i in range(joint.num_velocities()):
-                names[joint.velocity_start() + i] = \
-                    f"{joint.name()}_{joint.velocity_suffix(i)}"
+                names[
+                    joint.velocity_start() + i
+                ] = f"{joint.name()}_{joint.velocity_suffix(i)}"
     for ind in mbp.GetFloatingBaseBodies():
         body = mbp.get_body(ind)
         start = body.floating_velocities_start() - mbp.num_positions()
         for i in range(6):
-            names[start
-                  + i] = f"{body.name()}_{body.floating_velocity_suffix(i)}"
+            names[
+                start + i
+            ] = f"{body.name()}_{body.floating_velocity_suffix(i)}"
     return namedview(view_name, names)
 
 
 def MakeNamedViewState(mbp, view_name):
     # TODO: this could become a nested named view, pending
     # https://github.com/RobotLocomotion/drake/pull/14973
     pview = MakeNamedViewPositions(mbp, f"{view_name}_pos", True)
@@ -174,29 +202,32 @@
 
 # Adapted from Drake's system_doxygen.py.  Just make an html rendering of the
 # system block with its name and input/output ports (even if it is a Diagram).
 def SystemHtml(system):
     input_port_html = ""
     for p in range(system.num_input_ports()):
         input_port_html += (
-            f'<tr><td align=right style=\"padding:5px 0px 5px 0px\">'
-            f'{system.get_input_port(p).get_name()} &rarr;</td></tr>')
+            f'<tr><td align=right style="padding:5px 0px 5px 0px">'
+            f"{system.get_input_port(p).get_name()} &rarr;</td></tr>"
+        )
     output_port_html = ""
     for p in range(system.num_output_ports()):
         output_port_html += (
-            '<tr><td align=left style=\"padding:5px 0px 5px 0px\">'
-            f'&rarr; {system.get_output_port(p).get_name()}</td></tr>')
+            '<tr><td align=left style="padding:5px 0px 5px 0px">'
+            f"&rarr; {system.get_output_port(p).get_name()}</td></tr>"
+        )
     # Note: keeping this on a single line avoids having to handle comment line
     # markers (e.g. * or ///)
     html = (
-        f'<table align=center cellpadding=0 cellspacing=0><tr align=center>'
-        f'<td style=\"vertical-align:middle\">'
-        f'<table cellspacing=0 cellpadding=0>{input_port_html}</table>'
-        f'</td>'
-        f'<td align=center style=\"border:2px solid black;padding-left:20px;'
-        f'padding-right:20px;vertical-align:middle\" bgcolor=#F0F0F0>'
-        f'{system.get_name()}</td>'
-        f'<td style=\"vertical-align:middle\">'
-        f'<table cellspacing=0 cellpadding=0>{output_port_html}</table>'
-        f'</td></tr></table>')
+        f"<table align=center cellpadding=0 cellspacing=0><tr align=center>"
+        f'<td style="vertical-align:middle">'
+        f"<table cellspacing=0 cellpadding=0>{input_port_html}</table>"
+        f"</td>"
+        f'<td align=center style="border:2px solid black;padding-left:20px;'
+        f'padding-right:20px;vertical-align:middle" bgcolor=#F0F0F0>'
+        f"{system.get_name()}</td>"
+        f'<td style="vertical-align:middle">'
+        f"<table cellspacing=0 cellpadding=0>{output_port_html}</table>"
+        f"</td></tr></table>"
+    )
 
     return html
```

### Comparing `manipulation-2022.9.23/manipulation.egg-info/SOURCES.txt` & `manipulation-2023.5.29/manipulation.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,75 +1,97 @@
 LICENSE.TXT
-MANIFEST.in
+LICENSE.txt
 README.md
 pyproject.toml
 setup.cfg
+manipulation/BUILD.bazel
 manipulation/__init__.py
+manipulation/clutter.py
 manipulation/drake_gym.py
 manipulation/icp.py
 manipulation/meshcat_cpp_utils.py
 manipulation/meshcat_utils.py
 manipulation/mustard_depth_camera_example.py
-manipulation/open3d_utils.py
+manipulation/pick.py
 manipulation/scenarios.py
 manipulation/utils.py
-manipulation.egg-info/PKG-INFO
-manipulation.egg-info/SOURCES.txt
-manipulation.egg-info/dependency_links.txt
-manipulation.egg-info/requires.txt
-manipulation.egg-info/top_level.txt
+manipulation/envs/BUILD.bazel
 manipulation/envs/box_flipup.py
+manipulation/exercises/BUILD.bazel
 manipulation/exercises/grader.py
+manipulation/exercises/clutter/BUILD.bazel
+manipulation/exercises/clutter/normal_solution.npy
 manipulation/exercises/clutter/test_analytic_grasp.py
 manipulation/exercises/clutter/test_grasp_candidate.py
 manipulation/exercises/clutter/test_normal.py
+manipulation/exercises/clutter/test_simulation_tuning.py
+manipulation/exercises/deep_perception/BUILD.bazel
+manipulation/exercises/deep_perception/test_contrastive.py
+manipulation/exercises/force/BUILD.bazel
 manipulation/exercises/force/test_hybrid.py
+manipulation/exercises/pick/BUILD.bazel
 manipulation/exercises/pick/plot_planar_manipulator.py
 manipulation/exercises/pick/test_differential_ik.py
 manipulation/exercises/pick/test_planar_manipulator.py
 manipulation/exercises/pick/test_rigid_transforms.py
 manipulation/exercises/pick/test_robot_painter.py
 manipulation/exercises/pick/test_simple_qp.py
+manipulation/exercises/pose/BUILD.bazel
+manipulation/exercises/pose/pcl_filtered.npy
 manipulation/exercises/pose/test_icp.py
 manipulation/exercises/pose/test_pose_estimation.py
 manipulation/exercises/pose/test_ransac.py
+manipulation/exercises/rl/BUILD.bazel
 manipulation/exercises/rl/test_stochastic_optimization.py
 manipulation/exercises/rl/test_vpg.py
+manipulation/exercises/robot/BUILD.bazel
 manipulation/exercises/robot/test_direct_joint_control.py
 manipulation/exercises/robot/test_manipulation_io.py
 manipulation/exercises/robot/test_reflected_inertia.py
 manipulation/exercises/robot/test_survey.py
+manipulation/exercises/segmentation/BUILD.bazel
 manipulation/exercises/segmentation/test_mask.py
 manipulation/exercises/segmentation/test_segmentation_and_grasp.py
+manipulation/exercises/trajectories/BUILD.bazel
 manipulation/exercises/trajectories/test_door_opening.py
 manipulation/exercises/trajectories/test_rrt_planning.py
+manipulation/exercises/trajectories/test_taskspace_iris.py
+manipulation/exercises/trajectories/rrt_planner/BUILD.bazel
 manipulation/exercises/trajectories/rrt_planner/__init__.py
 manipulation/exercises/trajectories/rrt_planner/geometry.py
 manipulation/exercises/trajectories/rrt_planner/iiwa_rrt_problem.py
 manipulation/exercises/trajectories/rrt_planner/robot.py
 manipulation/exercises/trajectories/rrt_planner/rrt_planning.py
 manipulation/models/061_foam_brick_w_visual_contact_spheres.sdf
+manipulation/models/BUILD.bazel
 manipulation/models/camera_box.sdf
 manipulation/models/clutter.dmd.yaml
-manipulation/models/clutter_mustard.yaml
-manipulation/models/clutter_planning.yaml
+manipulation/models/clutter_mustard.dmd.yaml
+manipulation/models/clutter_planning.dmd.yaml
 manipulation/models/clutter_w_cameras.dmd.yaml
 manipulation/models/double_pendulum.urdf
+manipulation/models/floor.sdf
 manipulation/models/iiwa_and_wsg.dmd.yaml
-manipulation/models/mustard_w_cameras.yaml
+manipulation/models/manipulation_station_with_cupboard.dmd.yaml
+manipulation/models/mustard_w_cameras.dmd.yaml
+manipulation/models/package.xml
 manipulation/models/planar_bin.sdf
 manipulation/models/planar_foam_brick_collision_as_visual.sdf
+manipulation/models/planar_manipulation_station.dmd.yaml
+manipulation/models/rubiks_cube.sdf
+manipulation/models/rubiks_cube_2_by_2.sdf
+manipulation/models/schunk_wsg_50_welded_fingers.dmd.yaml
 manipulation/models/schunk_wsg_50_welded_fingers.sdf
-manipulation/models/schunk_wsg_50_welded_fingers.yaml
-manipulation/models/segmentation_and_grasp_scene.yaml
+manipulation/models/schunk_wsg_50_welded_fingers_sphere.sdf
+manipulation/models/segmentation_and_grasp_scene.dmd.yaml
 manipulation/models/shelves.sdf
+manipulation/models/shelves_w_ellipsoid_collision.sdf
+manipulation/models/two_bins.dmd.yaml
 manipulation/models/two_bins.sdf
-manipulation/models/two_bins.yaml
+manipulation/models/two_bins_w_cameras.dmd.yaml
 manipulation/models/two_bins_w_cameras.sdf
-manipulation/models/two_bins_w_cameras.yaml
 manipulation/models/two_link_iiwa14.urdf
+manipulation/models/bunny/BUILD.bazel
+manipulation/models/bunny/README
 manipulation/models/bunny/bun_zipper_res2.ply
-manipulation/test/test_gym.py
-manipulation/test/test_meshcat_utils.py
-manipulation/test/test_model_directives.py
-manipulation/test/test_open3d_utils.py
-manipulation/test/test_utils.py
+manipulation/models/bunny/bunny.npy
+rl/train_boxflipup.py
```

### Comparing `manipulation-2022.9.23/setup.cfg` & `manipulation-2023.5.29/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = manipulation
-version = 2022.09.23
+version = 2023.05.29
 author = Russ Tedrake
 author_email = russt@mit.edu
 description = MIT 6.4210 - Robotic Manipulation
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://manipulation.mit.edu
 project_urls = 
@@ -13,19 +13,19 @@
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: BSD License
 	Operating System :: POSIX :: Linux
 
 [options]
 package_dir = 
 include_package_data = True
-packages = find:
+packages = find_namespace:
 python_requires = >=3.8
 install_requires = 
 	cloudpickle>=1.6.0
-	drake>=1.8.0
+	drake>=1.17.0
 	gradescope-utils>=0.4.0
 	mpld3>=0.5.1
 	timeout-decorator>=0.4.1
 
 [pycodestyle]
 exclude = .git
 filename = *.py
```

