# Comparing `tmp/adam_sim-1.0.0.tar.gz` & `tmp/adam_sim-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adam_sim-1.0.0.tar", last modified: Sat Apr 22 21:29:04 2023, max compression
+gzip compressed data, was "adam_sim-1.0.1.tar", last modified: Mon May 29 15:40:50 2023, max compression
```

## Comparing `adam_sim-1.0.0.tar` & `adam_sim-1.0.1.tar`

### file list

```diff
@@ -1,173 +1,176 @@
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.543120 adam_sim-1.0.0/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     1063 2023-04-12 06:42:52.000000 adam_sim-1.0.0/LICENSE
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     3532 2023-04-22 21:29:04.543120 adam_sim-1.0.0/PKG-INFO
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     2887 2023-04-14 09:53:02.000000 adam_sim-1.0.0/README.md
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.507122 adam_sim-1.0.0/adam_sim/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)       40 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/__init__.py
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.507122 adam_sim-1.0.0/adam_sim/core/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)      815 2023-04-17 10:50:13.000000 adam_sim-1.0.0/adam_sim/core/topics.yaml
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.507122 adam_sim-1.0.0/adam_sim/entities/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)      353 2023-04-13 11:45:34.000000 adam_sim-1.0.0/adam_sim/entities/__init__.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     3134 2023-04-13 11:45:06.000000 adam_sim-1.0.0/adam_sim/entities/acceleration.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     6411 2023-04-19 11:37:53.000000 adam_sim-1.0.0/adam_sim/entities/configuration.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     3065 2023-04-19 07:31:45.000000 adam_sim-1.0.0/adam_sim/entities/point.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     2351 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/entities/system.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     1665 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/entities/vector.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     2782 2023-04-13 11:36:34.000000 adam_sim-1.0.0/adam_sim/entities/velocity.py
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.507122 adam_sim-1.0.0/adam_sim/features/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)      121 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/__init__.py
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.507122 adam_sim-1.0.0/adam_sim/features/adam/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)       23 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/adam/__init__.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     7765 2023-04-20 13:03:37.000000 adam_sim-1.0.0/adam_sim/features/adam/adam.py
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.507122 adam_sim-1.0.0/adam_sim/features/adam/communication/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)       57 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/__init__.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)      352 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/adam_repository_factory.py
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.507122 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)      116 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/__init__.py
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.507122 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/real_adam_repository/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)       53 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/real_adam_repository/__init__.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)      929 2023-04-20 13:05:27.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/real_adam_repository/real_adam_repository.py
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.507122 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)       63 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/__init__.py
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.507122 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.511122 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     1225 2023-04-12 10:28:03.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/actuators.xml
--rw-rw-r--   0 vistor    (1000) vistor    (1000)      853 2023-04-12 10:53:15.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/adam.xml
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     2491 2023-04-12 10:28:03.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/assets.xml
--rw-rw-r--   0 vistor    (1000) vistor    (1000)      952 2023-04-12 10:28:03.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/defaults.xml
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     5817 2023-04-12 10:29:53.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/left_manipulator.xml
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     5832 2023-04-12 10:30:17.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/right_manipulator.xml
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.539121 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)   306784 2023-04-12 10:28:03.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/base.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)    64184 2023-04-12 10:28:03.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/body.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     6084 2023-04-12 10:28:03.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/body1.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     1484 2023-04-12 10:28:03.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/body2.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     6284 2023-04-12 10:28:03.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/body3.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)    48684 2023-04-12 10:28:03.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/body4.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)   234684 2023-04-12 10:28:03.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/end_effector_body.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)    41484 2023-04-12 10:28:03.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/end_effector_rubber.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)   514984 2023-04-12 10:28:03.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_body.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)   983584 2023-04-12 10:28:03.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_body_2.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)  1147584 2023-04-12 10:28:03.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_cap.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)   307884 2023-04-12 10:28:03.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_link_body.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)    41484 2023-04-12 10:28:03.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_rubber.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)    41484 2023-04-12 10:28:03.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_rubber_2.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)   953184 2023-04-12 10:28:03.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/shoulder_body.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)  3570434 2023-04-12 10:28:03.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/shoulder_cap.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)    41884 2023-04-12 10:28:03.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/shoulder_rubber.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)   174484 2023-04-12 10:28:03.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/shoulder_screws.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)   953184 2023-04-12 10:28:03.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_body.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)  3570434 2023-04-12 10:28:03.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_cap.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)   461284 2023-04-12 10:28:04.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_link_body.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)    41884 2023-04-12 10:28:04.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_rubber.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)    41484 2023-04-12 10:28:04.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_rubber_2.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)    41484 2023-04-12 10:28:04.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_rubber_3.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)   174484 2023-04-12 10:28:04.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_screws.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)   483484 2023-04-12 10:28:04.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_1_body.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)  1619484 2023-04-12 10:28:04.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_1_cap.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)    41484 2023-04-12 10:28:04.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_1_rubber.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)   483484 2023-04-12 10:28:04.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_2_body.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)  1619484 2023-04-12 10:28:04.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_2_cap.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)    41484 2023-04-12 10:28:04.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_2_rubber.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)   483484 2023-04-12 10:28:04.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_3_body.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)  1619484 2023-04-12 10:28:04.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_3_cap.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)    41484 2023-04-12 10:28:04.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_3_rubber.stl
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     1043 2023-04-12 10:28:04.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/scene.xml
--rw-rw-r--   0 vistor    (1000) vistor    (1000)      442 2023-04-20 13:08:10.000000 adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/simulated_adam_repository.py
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.539121 adam_sim-1.0.0/adam_sim/features/adam/entities/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)       32 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/adam/entities/__init__.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)      703 2023-04-18 10:04:19.000000 adam_sim-1.0.0/adam_sim/features/adam/entities/adam_info.py
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.539121 adam_sim-1.0.0/adam_sim/features/adam/repository/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)       44 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/adam/repository/__init__.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)      352 2023-04-20 13:04:57.000000 adam_sim-1.0.0/adam_sim/features/adam/repository/adam_repository.py
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.539121 adam_sim-1.0.0/adam_sim/features/adam/use_cases/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)       27 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/adam/use_cases/__init__.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     1384 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/adam/use_cases/viewer.py
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.539121 adam_sim-1.0.0/adam_sim/features/base/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)       23 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/base/__init__.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)      427 2023-04-19 09:57:15.000000 adam_sim-1.0.0/adam_sim/features/base/base.py
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.539121 adam_sim-1.0.0/adam_sim/features/base/communication/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)       57 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/base/communication/__init__.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)      352 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/base/communication/base_repository_factory.py
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.539121 adam_sim-1.0.0/adam_sim/features/base/communication/implementations/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)      116 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/base/communication/implementations/__init__.py
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.539121 adam_sim-1.0.0/adam_sim/features/base/communication/implementations/real_base_repository/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)       53 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/base/communication/implementations/real_base_repository/__init__.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)      666 2023-04-20 13:11:50.000000 adam_sim-1.0.0/adam_sim/features/base/communication/implementations/real_base_repository/real_base_repository.py
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.539121 adam_sim-1.0.0/adam_sim/features/base/communication/implementations/simulated_base_repository/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)       63 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/base/communication/implementations/simulated_base_repository/__init__.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)      640 2023-04-20 13:12:00.000000 adam_sim-1.0.0/adam_sim/features/base/communication/implementations/simulated_base_repository/simulated_base_repository.py
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.539121 adam_sim-1.0.0/adam_sim/features/base/entities/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)       32 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/base/entities/__init__.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)      475 2023-04-13 12:23:56.000000 adam_sim-1.0.0/adam_sim/features/base/entities/base_info.py
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.539121 adam_sim-1.0.0/adam_sim/features/base/repository/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)       44 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/base/repository/__init__.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)      403 2023-04-20 13:08:40.000000 adam_sim-1.0.0/adam_sim/features/base/repository/base_repository.py
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.539121 adam_sim-1.0.0/adam_sim/features/data_manager/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)       38 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/data_manager/__init__.py
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.539121 adam_sim-1.0.0/adam_sim/features/data_manager/data/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)    20048 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/data_manager/data/configurations_test.csv
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     5901 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/data_manager/data/end_effector_positions_test.csv
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     3330 2023-04-19 07:32:30.000000 adam_sim-1.0.0/adam_sim/features/data_manager/data_manager.py
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.539121 adam_sim-1.0.0/adam_sim/features/manipulator/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)       37 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/manipulator/__init__.py
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.539121 adam_sim-1.0.0/adam_sim/features/manipulator/communication/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)       71 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/manipulator/communication/__init__.py
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.539121 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)      328 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/__init__.py
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.539121 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/real_left_manipulator_repository/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)       76 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/real_left_manipulator_repository/__init__.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     2010 2023-04-20 13:01:18.000000 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/real_left_manipulator_repository/real_left_manipulator_repository.py
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.543120 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/real_left_manipulator_repository/use_cases/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)       31 2023-04-18 07:57:00.000000 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/real_left_manipulator_repository/use_cases/__init__.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     1947 2023-04-22 11:00:16.000000 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/real_left_manipulator_repository/use_cases/client.py
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.543120 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/real_right_manipulator_repository/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)       78 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/real_right_manipulator_repository/__init__.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     2011 2023-04-22 10:57:14.000000 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/real_right_manipulator_repository/real_right_manipulator_repository.py
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.543120 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/real_right_manipulator_repository/use_cases/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)       31 2023-04-22 10:57:33.000000 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/real_right_manipulator_repository/use_cases/__init__.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     1949 2023-04-22 10:59:24.000000 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/real_right_manipulator_repository/use_cases/client.py
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.543120 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/simulated_left_manipulator_repository/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)       86 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/simulated_left_manipulator_repository/__init__.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     3634 2023-04-20 13:00:00.000000 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/simulated_left_manipulator_repository/simulated_left_manipulator_repository.py
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.543120 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/simulated_left_manipulator_repository/use_cases/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)       48 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/simulated_left_manipulator_repository/use_cases/__init__.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     4434 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/simulated_left_manipulator_repository/use_cases/collision_checker.py
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.543120 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/simulated_right_manipulator_repository/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)       88 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/simulated_right_manipulator_repository/__init__.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     3643 2023-04-20 13:00:17.000000 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/simulated_right_manipulator_repository/simulated_right_manipulator_repository.py
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.543120 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/simulated_right_manipulator_repository/use_cases/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)       48 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/simulated_right_manipulator_repository/use_cases/__init__.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     4439 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/simulated_right_manipulator_repository/use_cases/collision_checker.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)      667 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/manipulator/communication/manipulator_repository_factory.py
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.543120 adam_sim-1.0.0/adam_sim/features/manipulator/entities/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)       79 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/manipulator/entities/__init__.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     1698 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/manipulator/entities/collision.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     1008 2023-04-13 11:47:19.000000 adam_sim-1.0.0/adam_sim/features/manipulator/entities/manipulator_info.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     2528 2023-04-19 09:56:54.000000 adam_sim-1.0.0/adam_sim/features/manipulator/manipulator.py
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.543120 adam_sim-1.0.0/adam_sim/features/manipulator/repository/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)       58 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/manipulator/repository/__init__.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     1103 2023-04-20 12:59:27.000000 adam_sim-1.0.0/adam_sim/features/manipulator/repository/manipulator_repository.py
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.543120 adam_sim-1.0.0/adam_sim/features/manipulator/use_cases/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)       73 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/manipulator/use_cases/__init__.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     3761 2023-04-12 06:42:52.000000 adam_sim-1.0.0/adam_sim/features/manipulator/use_cases/control_visualizer.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     5109 2023-04-12 10:03:03.000000 adam_sim-1.0.0/adam_sim/features/manipulator/use_cases/farm.py
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.507122 adam_sim-1.0.0/adam_sim.egg-info/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     3532 2023-04-22 21:29:04.000000 adam_sim-1.0.0/adam_sim.egg-info/PKG-INFO
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     9827 2023-04-22 21:29:04.000000 adam_sim-1.0.0/adam_sim.egg-info/SOURCES.txt
--rw-rw-r--   0 vistor    (1000) vistor    (1000)        1 2023-04-22 21:29:04.000000 adam_sim-1.0.0/adam_sim.egg-info/dependency_links.txt
--rw-rw-r--   0 vistor    (1000) vistor    (1000)       75 2023-04-22 21:29:04.000000 adam_sim-1.0.0/adam_sim.egg-info/requires.txt
--rw-rw-r--   0 vistor    (1000) vistor    (1000)        9 2023-04-22 21:29:04.000000 adam_sim-1.0.0/adam_sim.egg-info/top_level.txt
--rw-rw-r--   0 vistor    (1000) vistor    (1000)      921 2023-04-22 21:28:41.000000 adam_sim-1.0.0/pyproject.toml
--rw-rw-r--   0 vistor    (1000) vistor    (1000)       38 2023-04-22 21:29:04.543120 adam_sim-1.0.0/setup.cfg
-drwxrwxr-x   0 vistor    (1000) vistor    (1000)        0 2023-04-22 21:29:04.543120 adam_sim-1.0.0/tests/
--rw-rw-r--   0 vistor    (1000) vistor    (1000)      743 2023-04-13 10:35:02.000000 adam_sim-1.0.0/tests/test_basic_usage.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     1541 2023-04-13 11:22:46.000000 adam_sim-1.0.0/tests/test_collisions.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)      494 2023-04-19 11:02:01.000000 adam_sim-1.0.0/tests/test_configuration.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)      344 2023-04-13 10:42:23.000000 adam_sim-1.0.0/tests/test_control.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)     1021 2023-04-19 08:23:30.000000 adam_sim-1.0.0/tests/test_data_manager.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)      116 2023-04-13 11:20:44.000000 adam_sim-1.0.0/tests/test_export_scene.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)      752 2023-04-13 11:07:55.000000 adam_sim-1.0.0/tests/test_farm.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)      604 2023-04-20 14:31:17.000000 adam_sim-1.0.0/tests/test_real_communication.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)      854 2023-04-13 11:59:15.000000 adam_sim-1.0.0/tests/test_returning_info.py
--rw-rw-r--   0 vistor    (1000) vistor    (1000)      533 2023-04-13 12:17:49.000000 adam_sim-1.0.0/tests/test_velocity.py
+drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.095546 adam_sim-1.0.1/
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)     1063 2023-05-29 15:34:07.000000 adam_sim-1.0.1/LICENSE
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)     3532 2023-05-29 15:40:50.095546 adam_sim-1.0.1/PKG-INFO
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)     2887 2023-05-29 15:34:07.000000 adam_sim-1.0.1/README.md
+drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.075654 adam_sim-1.0.1/adam_sim/
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)       40 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/__init__.py
+drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.075654 adam_sim-1.0.1/adam_sim/core/
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)      815 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/core/topics.yaml
+drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.079632 adam_sim-1.0.1/adam_sim/entities/
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)      353 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/entities/__init__.py
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)     3134 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/entities/acceleration.py
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)     6411 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/entities/configuration.py
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)     3065 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/entities/point.py
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)     2351 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/entities/system.py
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)     1665 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/entities/vector.py
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)     2782 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/entities/velocity.py
+drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.079632 adam_sim-1.0.1/adam_sim/features/
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)      121 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/__init__.py
+drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.079632 adam_sim-1.0.1/adam_sim/features/adam/
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)       23 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/__init__.py
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)     7765 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/adam.py
+drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.079632 adam_sim-1.0.1/adam_sim/features/adam/communication/
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)       57 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/__init__.py
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)      352 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/adam_repository_factory.py
+drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.079632 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)      116 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/__init__.py
+drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.079632 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/real_adam_repository/
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)       53 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/real_adam_repository/__init__.py
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)      929 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/real_adam_repository/real_adam_repository.py
+drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.079632 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)       63 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/__init__.py
+drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.079632 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/
+drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.079632 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)     1225 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/actuators.xml
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)      853 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/adam.xml
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)     2491 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/assets.xml
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)      952 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/defaults.xml
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)     5817 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/left_manipulator.xml
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)     5832 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/right_manipulator.xml
+drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)   306784 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/base.stl
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)    64184 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/body.stl
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)     6084 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/body1.stl
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)     1484 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/body2.stl
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)     6284 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/body3.stl
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)    48684 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/body4.stl
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)   234684 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/end_effector_body.stl
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)    41484 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/end_effector_rubber.stl
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)   514984 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_body.stl
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)   983584 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_body_2.stl
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)  1147584 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_cap.stl
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)   307884 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_link_body.stl
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)    41484 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_rubber.stl
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)    41484 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_rubber_2.stl
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)   953184 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/shoulder_body.stl
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)  3570434 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/shoulder_cap.stl
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)    41884 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/shoulder_rubber.stl
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)   174484 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/shoulder_screws.stl
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)   953184 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_body.stl
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)  3570434 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_cap.stl
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)   461284 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_link_body.stl
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)    41884 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_rubber.stl
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)    41484 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_rubber_2.stl
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)    41484 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_rubber_3.stl
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)   174484 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_screws.stl
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)   483484 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_1_body.stl
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)  1619484 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_1_cap.stl
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)    41484 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_1_rubber.stl
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)   483484 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_2_body.stl
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)  1619484 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_2_cap.stl
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)    41484 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_2_rubber.stl
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)   483484 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_3_body.stl
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)  1619484 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_3_cap.stl
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)    41484 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_3_rubber.stl
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)     1043 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/scene.xml
+drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/textures/
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)    73373 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/textures/light-gray-floor-tile.png
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)   196878 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/textures/metal.png
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)      442 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/simulated_adam_repository.py
+drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/adam/entities/
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)       32 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/entities/__init__.py
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)      703 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/entities/adam_info.py
+drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/adam/repository/
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)       44 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/repository/__init__.py
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)      352 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/repository/adam_repository.py
+drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/adam/use_cases/
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)       27 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/use_cases/__init__.py
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)     1384 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/adam/use_cases/viewer.py
+drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/base/
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)       23 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/base/__init__.py
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)      427 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/base/base.py
+drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/base/communication/
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)       57 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/base/communication/__init__.py
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)      352 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/base/communication/base_repository_factory.py
+drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/base/communication/implementations/
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)      116 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/base/communication/implementations/__init__.py
+drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/base/communication/implementations/real_base_repository/
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)       53 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/base/communication/implementations/real_base_repository/__init__.py
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)      666 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/base/communication/implementations/real_base_repository/real_base_repository.py
+drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/base/communication/implementations/simulated_base_repository/
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)       63 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/base/communication/implementations/simulated_base_repository/__init__.py
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)      640 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/base/communication/implementations/simulated_base_repository/simulated_base_repository.py
+drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/base/entities/
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)       32 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/base/entities/__init__.py
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)      475 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/base/entities/base_info.py
+drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/base/repository/
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)       44 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/base/repository/__init__.py
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)      403 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/base/repository/base_repository.py
+drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/data_manager/
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)       38 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/data_manager/__init__.py
+drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/data_manager/data/
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)    20048 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/data_manager/data/configurations_test.csv
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)     5901 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/data_manager/data/end_effector_positions_test.csv
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)     3330 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/data_manager/data_manager.py
+drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/manipulator/
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)       37 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/__init__.py
+drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/manipulator/communication/
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)       71 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/communication/__init__.py
+drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)      328 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/__init__.py
+drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/real_left_manipulator_repository/
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)       76 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/real_left_manipulator_repository/__init__.py
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)     2010 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/real_left_manipulator_repository/real_left_manipulator_repository.py
+drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/real_left_manipulator_repository/use_cases/
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)       31 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/real_left_manipulator_repository/use_cases/__init__.py
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)     1947 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/real_left_manipulator_repository/use_cases/client.py
+drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/real_right_manipulator_repository/
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)       78 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/real_right_manipulator_repository/__init__.py
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)     2011 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/real_right_manipulator_repository/real_right_manipulator_repository.py
+drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/real_right_manipulator_repository/use_cases/
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)       31 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/real_right_manipulator_repository/use_cases/__init__.py
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)     1949 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/real_right_manipulator_repository/use_cases/client.py
+drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/simulated_left_manipulator_repository/
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)       86 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/simulated_left_manipulator_repository/__init__.py
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)     3634 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/simulated_left_manipulator_repository/simulated_left_manipulator_repository.py
+drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/simulated_left_manipulator_repository/use_cases/
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)       48 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/simulated_left_manipulator_repository/use_cases/__init__.py
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)     4434 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/simulated_left_manipulator_repository/use_cases/collision_checker.py
+drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/simulated_right_manipulator_repository/
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)       88 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/simulated_right_manipulator_repository/__init__.py
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)     3643 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/simulated_right_manipulator_repository/simulated_right_manipulator_repository.py
+drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/simulated_right_manipulator_repository/use_cases/
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)       48 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/simulated_right_manipulator_repository/use_cases/__init__.py
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)     4439 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/simulated_right_manipulator_repository/use_cases/collision_checker.py
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)      667 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/communication/manipulator_repository_factory.py
+drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/manipulator/entities/
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)       79 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/entities/__init__.py
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)     1698 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/entities/collision.py
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)     1008 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/entities/manipulator_info.py
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)     2528 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/manipulator.py
+drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/manipulator/repository/
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)       58 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/repository/__init__.py
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)     1103 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/repository/manipulator_repository.py
+drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.091568 adam_sim-1.0.1/adam_sim/features/manipulator/use_cases/
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)       73 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/use_cases/__init__.py
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)     3761 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/use_cases/control_visualizer.py
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)     5109 2023-05-29 15:34:07.000000 adam_sim-1.0.1/adam_sim/features/manipulator/use_cases/farm.py
+drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.075654 adam_sim-1.0.1/adam_sim.egg-info/
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)     3532 2023-05-29 15:40:50.000000 adam_sim-1.0.1/adam_sim.egg-info/PKG-INFO
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)    10053 2023-05-29 15:40:50.000000 adam_sim-1.0.1/adam_sim.egg-info/SOURCES.txt
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)        1 2023-05-29 15:40:50.000000 adam_sim-1.0.1/adam_sim.egg-info/dependency_links.txt
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)       75 2023-05-29 15:40:50.000000 adam_sim-1.0.1/adam_sim.egg-info/requires.txt
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)        9 2023-05-29 15:40:50.000000 adam_sim-1.0.1/adam_sim.egg-info/top_level.txt
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)      930 2023-05-29 15:40:24.000000 adam_sim-1.0.1/pyproject.toml
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)       38 2023-05-29 15:40:50.095546 adam_sim-1.0.1/setup.cfg
+drwxrwxr-x   0 vistor    (1001) vistor    (1001)        0 2023-05-29 15:40:50.095546 adam_sim-1.0.1/tests/
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)      743 2023-05-29 15:34:07.000000 adam_sim-1.0.1/tests/test_basic_usage.py
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)     1541 2023-05-29 15:34:07.000000 adam_sim-1.0.1/tests/test_collisions.py
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)      494 2023-05-29 15:34:07.000000 adam_sim-1.0.1/tests/test_configuration.py
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)      344 2023-05-29 15:34:07.000000 adam_sim-1.0.1/tests/test_control.py
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)     1021 2023-05-29 15:34:07.000000 adam_sim-1.0.1/tests/test_data_manager.py
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)      116 2023-05-29 15:34:07.000000 adam_sim-1.0.1/tests/test_export_scene.py
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)      752 2023-05-29 15:34:07.000000 adam_sim-1.0.1/tests/test_farm.py
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)      604 2023-05-29 15:34:07.000000 adam_sim-1.0.1/tests/test_real_communication.py
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)      854 2023-05-29 15:34:07.000000 adam_sim-1.0.1/tests/test_returning_info.py
+-rw-rw-r--   0 vistor    (1001) vistor    (1001)      533 2023-05-29 15:34:07.000000 adam_sim-1.0.1/tests/test_velocity.py
```

### Comparing `adam_sim-1.0.0/LICENSE` & `adam_sim-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/PKG-INFO` & `adam_sim-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adam_sim
-Version: 1.0.0
+Version: 1.0.1
 Summary: A simulator of ADAM (Autonomous Domestic Ambidextrous Manipulator), a mobile robot manipulator consisting of a base with two Degrees of Freedom (DoF) and two Universal Robots UR3 of 6 DoF each.
 Author: Vistor
 Project-URL: Homepage, https://github.com/vistormu/adam_simulator
 Project-URL: Bug Tracker, https://github.com/vistormu/adam_simulator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: adam_sim Version: 1.0.0 Summary: A simulator of
+Metadata-Version: 2.1 Name: adam_sim Version: 1.0.1 Summary: A simulator of
 ADAM (Autonomous Domestic Ambidextrous Manipulator), a mobile robot manipulator
 consisting of a base with two Degrees of Freedom (DoF) and two Universal Robots
 UR3 of 6 DoF each. Author: Vistor Project-URL: Homepage, https://github.com/
 vistormu/adam_simulator Project-URL: Bug Tracker, https://github.com/vistormu/
 adam_simulator/issues Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.10 Description-Content-Type: text/
```

### Comparing `adam_sim-1.0.0/README.md` & `adam_sim-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/core/topics.yaml` & `adam_sim-1.0.1/adam_sim/core/topics.yaml`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/entities/acceleration.py` & `adam_sim-1.0.1/adam_sim/entities/acceleration.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/entities/configuration.py` & `adam_sim-1.0.1/adam_sim/entities/configuration.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/entities/point.py` & `adam_sim-1.0.1/adam_sim/entities/point.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/entities/system.py` & `adam_sim-1.0.1/adam_sim/entities/system.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/entities/vector.py` & `adam_sim-1.0.1/adam_sim/entities/vector.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/entities/velocity.py` & `adam_sim-1.0.1/adam_sim/entities/velocity.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/adam/adam.py` & `adam_sim-1.0.1/adam_sim/features/adam/adam.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/real_adam_repository/real_adam_repository.py` & `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/real_adam_repository/real_adam_repository.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/actuators.xml` & `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/actuators.xml`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/adam.xml` & `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/adam.xml`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/assets.xml` & `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/assets.xml`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/defaults.xml` & `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/defaults.xml`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/left_manipulator.xml` & `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/left_manipulator.xml`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/right_manipulator.xml` & `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/adam/right_manipulator.xml`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/base.stl` & `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/base.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/body.stl` & `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/body.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/body1.stl` & `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/body1.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/body2.stl` & `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/body2.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/body3.stl` & `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/body3.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/body4.stl` & `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/body4.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/end_effector_body.stl` & `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/end_effector_body.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/end_effector_rubber.stl` & `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/end_effector_rubber.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_body.stl` & `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_body.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_body_2.stl` & `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_body_2.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_cap.stl` & `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_cap.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_link_body.stl` & `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_link_body.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_rubber.stl` & `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_rubber.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_rubber_2.stl` & `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/forearm_rubber_2.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/shoulder_body.stl` & `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/shoulder_body.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/shoulder_cap.stl` & `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/shoulder_cap.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/shoulder_rubber.stl` & `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/shoulder_rubber.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/shoulder_screws.stl` & `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/shoulder_screws.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_body.stl` & `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_body.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_cap.stl` & `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_cap.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_link_body.stl` & `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_link_body.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_rubber.stl` & `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_rubber.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_rubber_2.stl` & `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_rubber_2.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_rubber_3.stl` & `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_rubber_3.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_screws.stl` & `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/upperarm_screws.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_1_body.stl` & `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_1_body.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_1_cap.stl` & `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_1_cap.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_1_rubber.stl` & `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_1_rubber.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_2_body.stl` & `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_2_body.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_2_cap.stl` & `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_2_cap.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_2_rubber.stl` & `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_2_rubber.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_3_body.stl` & `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_3_body.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_3_cap.stl` & `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_3_cap.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_3_rubber.stl` & `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_3_rubber.stl`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/scene.xml` & `adam_sim-1.0.1/adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/scene.xml`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/adam/entities/adam_info.py` & `adam_sim-1.0.1/adam_sim/features/adam/entities/adam_info.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/adam/use_cases/viewer.py` & `adam_sim-1.0.1/adam_sim/features/adam/use_cases/viewer.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/base/communication/implementations/real_base_repository/real_base_repository.py` & `adam_sim-1.0.1/adam_sim/features/base/communication/implementations/real_base_repository/real_base_repository.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/base/communication/implementations/simulated_base_repository/simulated_base_repository.py` & `adam_sim-1.0.1/adam_sim/features/base/communication/implementations/simulated_base_repository/simulated_base_repository.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/data_manager/data/configurations_test.csv` & `adam_sim-1.0.1/adam_sim/features/data_manager/data/configurations_test.csv`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/data_manager/data/end_effector_positions_test.csv` & `adam_sim-1.0.1/adam_sim/features/data_manager/data/end_effector_positions_test.csv`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/data_manager/data_manager.py` & `adam_sim-1.0.1/adam_sim/features/data_manager/data_manager.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/real_left_manipulator_repository/real_left_manipulator_repository.py` & `adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/real_left_manipulator_repository/real_left_manipulator_repository.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/real_left_manipulator_repository/use_cases/client.py` & `adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/real_left_manipulator_repository/use_cases/client.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/real_right_manipulator_repository/real_right_manipulator_repository.py` & `adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/real_right_manipulator_repository/real_right_manipulator_repository.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/real_right_manipulator_repository/use_cases/client.py` & `adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/real_right_manipulator_repository/use_cases/client.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/simulated_left_manipulator_repository/simulated_left_manipulator_repository.py` & `adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/simulated_left_manipulator_repository/simulated_left_manipulator_repository.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/simulated_left_manipulator_repository/use_cases/collision_checker.py` & `adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/simulated_left_manipulator_repository/use_cases/collision_checker.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/simulated_right_manipulator_repository/simulated_right_manipulator_repository.py` & `adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/simulated_right_manipulator_repository/simulated_right_manipulator_repository.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/manipulator/communication/implementations/simulated_right_manipulator_repository/use_cases/collision_checker.py` & `adam_sim-1.0.1/adam_sim/features/manipulator/communication/implementations/simulated_right_manipulator_repository/use_cases/collision_checker.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/manipulator/communication/manipulator_repository_factory.py` & `adam_sim-1.0.1/adam_sim/features/manipulator/communication/manipulator_repository_factory.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/manipulator/entities/collision.py` & `adam_sim-1.0.1/adam_sim/features/manipulator/entities/collision.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/manipulator/entities/manipulator_info.py` & `adam_sim-1.0.1/adam_sim/features/manipulator/entities/manipulator_info.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/manipulator/manipulator.py` & `adam_sim-1.0.1/adam_sim/features/manipulator/manipulator.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/manipulator/repository/manipulator_repository.py` & `adam_sim-1.0.1/adam_sim/features/manipulator/repository/manipulator_repository.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/manipulator/use_cases/control_visualizer.py` & `adam_sim-1.0.1/adam_sim/features/manipulator/use_cases/control_visualizer.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim/features/manipulator/use_cases/farm.py` & `adam_sim-1.0.1/adam_sim/features/manipulator/use_cases/farm.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/adam_sim.egg-info/PKG-INFO` & `adam_sim-1.0.1/adam_sim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adam-sim
-Version: 1.0.0
+Version: 1.0.1
 Summary: A simulator of ADAM (Autonomous Domestic Ambidextrous Manipulator), a mobile robot manipulator consisting of a base with two Degrees of Freedom (DoF) and two Universal Robots UR3 of 6 DoF each.
 Author: Vistor
 Project-URL: Homepage, https://github.com/vistormu/adam_simulator
 Project-URL: Bug Tracker, https://github.com/vistormu/adam_simulator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: adam-sim Version: 1.0.0 Summary: A simulator of
+Metadata-Version: 2.1 Name: adam-sim Version: 1.0.1 Summary: A simulator of
 ADAM (Autonomous Domestic Ambidextrous Manipulator), a mobile robot manipulator
 consisting of a base with two Degrees of Freedom (DoF) and two Universal Robots
 UR3 of 6 DoF each. Author: Vistor Project-URL: Homepage, https://github.com/
 vistormu/adam_simulator Project-URL: Bug Tracker, https://github.com/vistormu/
 adam_simulator/issues Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.10 Description-Content-Type: text/
```

### Comparing `adam_sim-1.0.0/adam_sim.egg-info/SOURCES.txt` & `adam_sim-1.0.1/adam_sim.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,16 @@
 adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_1_rubber.stl
 adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_2_body.stl
 adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_2_cap.stl
 adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_2_rubber.stl
 adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_3_body.stl
 adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_3_cap.stl
 adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/meshes/wrist_3_rubber.stl
+adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/textures/light-gray-floor-tile.png
+adam_sim/features/adam/communication/implementations/simulated_adam_repository/assets/textures/metal.png
 adam_sim/features/adam/entities/__init__.py
 adam_sim/features/adam/entities/adam_info.py
 adam_sim/features/adam/repository/__init__.py
 adam_sim/features/adam/repository/adam_repository.py
 adam_sim/features/adam/use_cases/__init__.py
 adam_sim/features/adam/use_cases/viewer.py
 adam_sim/features/base/__init__.py
```

### Comparing `adam_sim-1.0.0/pyproject.toml` & `adam_sim-1.0.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "adam_sim"
-version = "1.0.0"
+version = "1.0.1"
 authors = [{ name = "Vistor" }]
 description = "A simulator of ADAM (Autonomous Domestic Ambidextrous Manipulator), a mobile robot manipulator consisting of a base with two Degrees of Freedom (DoF) and two Universal Robots UR3 of 6 DoF each."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
@@ -22,12 +22,12 @@
   "pandas",
   "matplotlib",
   "paho-mqtt",
   "vclog",  
 ]
 
 [tool.setuptools.package-data]
-"*" = ["*.csv", "*.stl", "*.xml", "*.yaml"]
+"*" = ["*.csv", "*.stl", "*.xml", "*.yaml", "*.png"]
 
 [project.urls]
 "Homepage" = "https://github.com/vistormu/adam_simulator"
 "Bug Tracker" = "https://github.com/vistormu/adam_simulator/issues"
```

### Comparing `adam_sim-1.0.0/tests/test_basic_usage.py` & `adam_sim-1.0.1/tests/test_basic_usage.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/tests/test_collisions.py` & `adam_sim-1.0.1/tests/test_collisions.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/tests/test_data_manager.py` & `adam_sim-1.0.1/tests/test_data_manager.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/tests/test_farm.py` & `adam_sim-1.0.1/tests/test_farm.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/tests/test_real_communication.py` & `adam_sim-1.0.1/tests/test_real_communication.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/tests/test_returning_info.py` & `adam_sim-1.0.1/tests/test_returning_info.py`

 * *Files identical despite different names*

### Comparing `adam_sim-1.0.0/tests/test_velocity.py` & `adam_sim-1.0.1/tests/test_velocity.py`

 * *Files identical despite different names*

