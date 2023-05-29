# Comparing `tmp/vid2info-1.98.tar.gz` & `tmp/vid2info-1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vid2info-1.98.tar", last modified: Mon Feb 27 11:49:39 2023, max compression
+gzip compressed data, was "vid2info-1.99.tar", last modified: Mon Feb 27 12:29:46 2023, max compression
```

## Comparing `vid2info-1.98.tar` & `vid2info-1.99.tar`

### file list

```diff
@@ -1,345 +1,345 @@
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:39.612662 vid2info-1.98/
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:36.350314 vid2info-1.98/ByteTrack/
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:36.283627 vid2info-1.98/ByteTrack/deploy/
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:36.374446 vid2info-1.98/ByteTrack/deploy/ONNXRuntime/
--rw-rw-rw-   0        0        0     5855 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/deploy/ONNXRuntime/onnx_inference.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:36.288412 vid2info-1.98/ByteTrack/exps/
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:36.447745 vid2info-1.98/ByteTrack/exps/default/
--rw-rw-rw-   0        0        0     1359 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/exps/default/nano.py
--rw-rw-rw-   0        0        0     3095 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/exps/default/yolov3.py
--rw-rw-rw-   0        0        0      370 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/exps/default/yolox_l.py
--rw-rw-rw-   0        0        0      372 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/exps/default/yolox_m.py
--rw-rw-rw-   0        0        0      372 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/exps/default/yolox_s.py
--rw-rw-rw-   0        0        0      515 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/exps/default/yolox_tiny.py
--rw-rw-rw-   0        0        0      372 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/exps/default/yolox_x.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:36.288412 vid2info-1.98/ByteTrack/exps/example/
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:36.614877 vid2info-1.98/ByteTrack/exps/example/mot/
--rw-rw-rw-   0        0        0     4490 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/exps/example/mot/yolox_l_mix_det.py
--rw-rw-rw-   0        0        0     4492 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/exps/example/mot/yolox_m_mix_det.py
--rw-rw-rw-   0        0        0     5347 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/exps/example/mot/yolox_nano_mix_det.py
--rw-rw-rw-   0        0        0     4492 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/exps/example/mot/yolox_s_mix_det.py
--rw-rw-rw-   0        0        0     4526 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/exps/example/mot/yolox_tiny_mix_det.py
--rw-rw-rw-   0        0        0     4496 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/exps/example/mot/yolox_x_ablation.py
--rw-rw-rw-   0        0        0     4492 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/exps/example/mot/yolox_x_ch.py
--rw-rw-rw-   0        0        0     4594 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/exps/example/mot/yolox_x_mix_det.py
--rw-rw-rw-   0        0        0     4637 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/exps/example/mot/yolox_x_mix_mot20_ch.py
--rw-rw-rw-   0        0        0     4494 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/exps/example/mot/yolox_x_mot17_half.py
--rw-rw-rw-   0        0        0     1740 2022-07-13 17:53:10.000000 vid2info-1.98/ByteTrack/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:36.290789 vid2info-1.98/ByteTrack/src/
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:36.630992 vid2info-1.98/ByteTrack/src/cython-bbox/
--rw-rw-rw-   0        0        0     1350 2022-08-05 22:30:19.000000 vid2info-1.98/ByteTrack/src/cython-bbox/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:36.964009 vid2info-1.98/ByteTrack/tools/
--rw-rw-rw-   0        0        0     2541 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tools/convert_cityperson_to_coco.py
--rw-rw-rw-   0        0        0     2337 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tools/convert_crowdhuman_to_coco.py
--rw-rw-rw-   0        0        0     2527 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tools/convert_ethz_to_coco.py
--rw-rw-rw-   0        0        0     6889 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tools/convert_mot17_to_coco.py
--rw-rw-rw-   0        0        0     6821 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tools/convert_mot20_to_coco.py
--rw-rw-rw-   0        0        0      884 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tools/convert_video.py
--rw-rw-rw-   0        0        0    13970 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tools/demo_track.py
--rw-rw-rw-   0        0        0     3150 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tools/export_onnx.py
--rw-rw-rw-   0        0        0     5732 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tools/interpolation.py
--rw-rw-rw-   0        0        0     2569 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tools/mix_data_ablation.py
--rw-rw-rw-   0        0        0     4070 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tools/mix_data_test_mot17.py
--rw-rw-rw-   0        0        0     2520 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tools/mix_data_test_mot20.py
--rw-rw-rw-   0        0        0     3498 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tools/mota.py
--rw-rw-rw-   0        0        0    10667 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tools/track.py
--rw-rw-rw-   0        0        0    10657 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tools/track_deepsort.py
--rw-rw-rw-   0        0        0    10681 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tools/track_motdt.py
--rw-rw-rw-   0        0        0    10467 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tools/track_sort.py
--rw-rw-rw-   0        0        0     3559 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tools/train.py
--rw-rw-rw-   0        0        0     2217 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tools/trt.py
--rw-rw-rw-   0        0        0     7405 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tools/txt2video.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:36.302322 vid2info-1.98/ByteTrack/tutorials/
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:37.013938 vid2info-1.98/ByteTrack/tutorials/centertrack/
--rw-rw-rw-   0        0        0    13599 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tutorials/centertrack/byte_tracker.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:37.047134 vid2info-1.98/ByteTrack/tutorials/centertrack/mot_online/
--rw-rw-rw-   0        0        0     1003 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tutorials/centertrack/mot_online/basetrack.py
--rw-rw-rw-   0        0        0     9816 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tutorials/centertrack/mot_online/kalman_filter.py
--rw-rw-rw-   0        0        0     7746 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tutorials/centertrack/mot_online/matching.py
--rw-rw-rw-   0        0        0    21716 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tutorials/centertrack/opts.py
--rw-rw-rw-   0        0        0     9103 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tutorials/centertrack/tracker.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:37.089506 vid2info-1.98/ByteTrack/tutorials/cstrack/
--rw-rw-rw-   0        0        0    21156 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tutorials/cstrack/byte_tracker.py
--rw-rw-rw-   0        0        0    23301 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tutorials/cstrack/tracker.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:37.147251 vid2info-1.98/ByteTrack/tutorials/ctracker/
--rw-rw-rw-   0        0        0    12165 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tutorials/ctracker/byte_tracker.py
--rw-rw-rw-   0        0        0     5318 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tutorials/ctracker/eval_motchallenge.py
--rw-rw-rw-   0        0        0     1615 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tutorials/ctracker/generate_half_csv.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:37.164349 vid2info-1.98/ByteTrack/tutorials/ctracker/mot_online/
--rw-rw-rw-   0        0        0     1003 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tutorials/ctracker/mot_online/basetrack.py
--rw-rw-rw-   0        0        0     9816 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tutorials/ctracker/mot_online/kalman_filter.py
--rw-rw-rw-   0        0        0     7746 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tutorials/ctracker/mot_online/matching.py
--rw-rw-rw-   0        0        0    12268 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tutorials/ctracker/test.py
--rw-rw-rw-   0        0        0     6109 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tutorials/ctracker/test_byte.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:37.197938 vid2info-1.98/ByteTrack/tutorials/fairmot/
--rw-rw-rw-   0        0        0    15246 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tutorials/fairmot/byte_tracker.py
--rw-rw-rw-   0        0        0    18050 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tutorials/fairmot/tracker.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:37.266596 vid2info-1.98/ByteTrack/tutorials/jde/
--rw-rw-rw-   0        0        0    15527 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tutorials/jde/byte_tracker.py
--rw-rw-rw-   0        0        0     3698 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tutorials/jde/evaluation.py
--rw-rw-rw-   0        0        0     9076 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tutorials/jde/track_half.py
--rw-rw-rw-   0        0        0    17846 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tutorials/jde/tracker.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:37.380448 vid2info-1.98/ByteTrack/tutorials/motr/
--rw-rw-rw-   0        0        0    12066 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tutorials/motr/byte_tracker.py
--rw-rw-rw-   0        0        0    19720 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tutorials/motr/eval.py
--rw-rw-rw-   0        0        0     7705 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tutorials/motr/evaluation.py
--rw-rw-rw-   0        0        0    12162 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tutorials/motr/joint.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:37.397183 vid2info-1.98/ByteTrack/tutorials/motr/mot_online/
--rw-rw-rw-   0        0        0     1003 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tutorials/motr/mot_online/basetrack.py
--rw-rw-rw-   0        0        0     9782 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tutorials/motr/mot_online/kalman_filter.py
--rw-rw-rw-   0        0        0     7742 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tutorials/motr/mot_online/matching.py
--rw-rw-rw-   0        0        0    33632 2022-08-05 22:30:19.000000 vid2info-1.98/ByteTrack/tutorials/motr/motr.py
--rw-rw-rw-   0        0        0    33693 2022-08-05 22:30:19.000000 vid2info-1.98/ByteTrack/tutorials/motr/motr_det.py
--rw-rw-rw-   0        0        0    22324 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tutorials/motr/transforms.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:37.439619 vid2info-1.98/ByteTrack/tutorials/qdtrack/
--rw-rw-rw-   0        0        0    12720 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tutorials/qdtrack/byte_tracker.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:37.463960 vid2info-1.98/ByteTrack/tutorials/qdtrack/mot_online/
--rw-rw-rw-   0        0        0     1003 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tutorials/qdtrack/mot_online/basetrack.py
--rw-rw-rw-   0        0        0     9816 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tutorials/qdtrack/mot_online/kalman_filter.py
--rw-rw-rw-   0        0        0     7746 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tutorials/qdtrack/mot_online/matching.py
--rw-rw-rw-   0        0        0     6169 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tutorials/qdtrack/qdtrack.py
--rw-rw-rw-   0        0        0    14737 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tutorials/qdtrack/tracker_reid_motion.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:37.497669 vid2info-1.98/ByteTrack/tutorials/trades/
--rw-rw-rw-   0        0        0    13321 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tutorials/trades/byte_tracker.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:37.529763 vid2info-1.98/ByteTrack/tutorials/trades/mot_online/
--rw-rw-rw-   0        0        0     1003 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tutorials/trades/mot_online/basetrack.py
--rw-rw-rw-   0        0        0     9782 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tutorials/trades/mot_online/kalman_filter.py
--rw-rw-rw-   0        0        0     7742 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tutorials/trades/mot_online/matching.py
--rw-rw-rw-   0        0        0    23334 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tutorials/trades/opts.py
--rw-rw-rw-   0        0        0    14902 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tutorials/trades/tracker.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:37.591585 vid2info-1.98/ByteTrack/tutorials/transtrack/
--rw-rw-rw-   0        0        0    12497 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tutorials/transtrack/engine_track.py
--rw-rw-rw-   0        0        0    18928 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tutorials/transtrack/main_track.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:37.647653 vid2info-1.98/ByteTrack/tutorials/transtrack/mot_online/
--rw-rw-rw-   0        0        0     1001 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tutorials/transtrack/mot_online/basetrack.py
--rw-rw-rw-   0        0        0    12950 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tutorials/transtrack/mot_online/byte_tracker.py
--rw-rw-rw-   0        0        0     9816 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tutorials/transtrack/mot_online/kalman_filter.py
--rw-rw-rw-   0        0        0     5486 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tutorials/transtrack/mot_online/matching.py
--rw-rw-rw-   0        0        0     1954 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tutorials/transtrack/save_track.py
--rw-rw-rw-   0        0        0     7685 2022-07-13 17:44:25.000000 vid2info-1.98/ByteTrack/tutorials/transtrack/tracker.py
--rw-rw-rw-   0        0        0    35823 2022-08-04 07:27:36.000000 vid2info-1.98/LICENSE
--rw-rw-rw-   0        0        0     1017 2023-02-27 11:49:39.614118 vid2info-1.98/PKG-INFO
--rw-rw-rw-   0        0        0      163 2022-08-29 23:06:12.000000 vid2info-1.98/README.md
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:37.697094 vid2info-1.98/models/
--rw-rw-rw-   0        0        0    84376 2022-08-27 11:30:35.000000 vid2info-1.98/models/common.py
--rw-rw-rw-   0        0        0    10287 2022-08-27 11:30:49.000000 vid2info-1.98/models/experimental.py
--rw-rw-rw-   0        0        0    40052 2022-08-27 11:31:12.000000 vid2info-1.98/models/yolo.py
--rw-rw-rw-   0        0        0      111 2023-02-27 11:49:39.615120 vid2info-1.98/setup.cfg
--rw-rw-rw-   0        0        0     1321 2023-02-27 11:49:31.000000 vid2info-1.98/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:36.304209 vid2info-1.98/third_party/
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:37.757433 vid2info-1.98/third_party/pidnet/
--rw-rw-rw-   0        0        0    17118 2022-07-23 14:51:56.000000 vid2info-1.98/third_party/pidnet/model_utils.py
--rw-rw-rw-   0        0        0    11938 2022-07-30 12:58:40.000000 vid2info-1.98/third_party/pidnet/pidnet.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:37.773584 vid2info-1.98/training_tools/
--rw-rw-rw-   0        0        0      392 2022-07-22 17:05:37.000000 vid2info-1.98/training_tools/config.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:37.801354 vid2info-1.98/training_tools/dataset_generation/
--rw-rw-rw-   0        0        0      158 2022-07-24 20:53:38.000000 vid2info-1.98/training_tools/dataset_generation/config.py
--rw-rw-rw-   0        0        0     3508 2022-08-05 22:30:19.000000 vid2info-1.98/training_tools/dataset_generation/video_extractor.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:37.947147 vid2info-1.98/utils/
--rw-rw-rw-   0        0        0     2248 2022-08-23 00:27:01.000000 vid2info-1.98/utils/activations.py
--rw-rw-rw-   0        0        0     5616 2022-08-23 00:27:01.000000 vid2info-1.98/utils/add_nms.py
--rw-rw-rw-   0        0        0     7147 2022-08-23 00:27:01.000000 vid2info-1.98/utils/autoanchor.py
--rw-rw-rw-   0        0        0    56073 2022-08-27 11:11:53.000000 vid2info-1.98/utils/datasets.py
--rw-rw-rw-   0        0        0    36821 2022-08-27 11:11:53.000000 vid2info-1.98/utils/general.py
--rw-rw-rw-   0        0        0     4877 2022-08-27 11:01:12.000000 vid2info-1.98/utils/google_utils.py
--rw-rw-rw-   0        0        0    74944 2022-08-23 00:27:01.000000 vid2info-1.98/utils/loss.py
--rw-rw-rw-   0        0        0     8969 2022-08-23 00:27:01.000000 vid2info-1.98/utils/metrics.py
--rw-rw-rw-   0        0        0    20921 2022-08-27 11:11:53.000000 vid2info-1.98/utils/plots.py
--rw-rw-rw-   0        0        0    15467 2022-08-23 00:27:01.000000 vid2info-1.98/utils/torch_utils.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:37.947147 vid2info-1.98/vid2info/
--rw-rw-rw-   0        0        0        0 2022-08-24 13:19:17.000000 vid2info-1.98/vid2info/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:38.014229 vid2info-1.98/vid2info/inference/
--rw-rw-rw-   0        0        0        0 2022-08-27 10:53:11.000000 vid2info-1.98/vid2info/inference/__init__.py
--rw-rw-rw-   0        0        0      515 2022-08-05 22:30:19.000000 vid2info-1.98/vid2info/inference/config.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:38.030578 vid2info-1.98/vid2info/inference/detection/
--rw-rw-rw-   0        0        0        0 2022-08-27 11:06:40.000000 vid2info-1.98/vid2info/inference/detection/__init__.py
--rw-rw-rw-   0        0        0    13801 2023-02-17 17:26:27.000000 vid2info-1.98/vid2info/inference/detection/__yolo_detector.py
--rw-rw-rw-   0        0        0      569 2022-08-29 23:12:12.000000 vid2info-1.98/vid2info/inference/detection/config.py
--rw-rw-rw-   0        0        0     3956 2023-02-17 17:26:27.000000 vid2info-1.98/vid2info/inference/detection/yolov6_detector.py
--rw-rw-rw-   0        0        0     4367 2023-02-17 17:26:28.000000 vid2info-1.98/vid2info/inference/detection/yolov7_detector.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:36.309383 vid2info-1.98/vid2info/inference/models/
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:38.048269 vid2info-1.98/vid2info/inference/models/finite_state_machine_configs/
--rw-rw-rw-   0        0        0     1004 2023-02-17 17:26:27.000000 vid2info-1.98/vid2info/inference/models/finite_state_machine_configs/dummy_finite_state_config.py
--rw-rw-rw-   0        0        0    13020 2023-02-27 10:06:54.000000 vid2info-1.98/vid2info/inference/pipeline.py
--rw-rw-rw-   0        0        0    11130 2023-02-27 10:06:54.000000 vid2info-1.98/vid2info/inference/pipeline_background.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:38.064244 vid2info-1.98/vid2info/inference/segmentation/
--rw-rw-rw-   0        0        0        0 2022-08-27 11:06:40.000000 vid2info-1.98/vid2info/inference/segmentation/__init__.py
--rw-rw-rw-   0        0        0      379 2022-08-29 23:24:48.000000 vid2info-1.98/vid2info/inference/segmentation/config.py
--rw-rw-rw-   0        0        0    13193 2023-02-17 17:26:27.000000 vid2info-1.98/vid2info/inference/segmentation/pidnet_segmenter.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:38.081124 vid2info-1.98/vid2info/inference/tracking/
--rw-rw-rw-   0        0        0        0 2022-08-27 11:06:40.000000 vid2info-1.98/vid2info/inference/tracking/__init__.py
--rw-rw-rw-   0        0        0      168 2022-08-05 17:43:54.000000 vid2info-1.98/vid2info/inference/tracking/config.py
--rw-rw-rw-   0        0        0     7378 2023-02-17 18:05:16.000000 vid2info-1.98/vid2info/inference/tracking/tracker.py
--rw-rw-rw-   0        0        0     7932 2023-02-17 17:26:27.000000 vid2info-1.98/vid2info/inference/utils.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:38.097757 vid2info-1.98/vid2info/state/
--rw-rw-rw-   0        0        0        0 2022-08-11 07:28:01.000000 vid2info-1.98/vid2info/state/__init__.py
--rw-rw-rw-   0        0        0      570 2022-09-11 20:42:48.000000 vid2info-1.98/vid2info/state/config.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:38.107699 vid2info-1.98/vid2info/state/element_state/
--rw-rw-rw-   0        0        0        0 2023-02-27 09:52:37.000000 vid2info-1.98/vid2info/state/element_state/__init__.py
--rw-rw-rw-   0        0        0      124 2023-02-27 11:23:16.000000 vid2info-1.98/vid2info/state/element_state/constants.py
--rw-rw-rw-   0        0        0     7913 2023-02-27 11:46:04.000000 vid2info-1.98/vid2info/state/element_state/element_movement.py
--rw-rw-rw-   0        0        0     5688 2023-02-27 10:06:54.000000 vid2info-1.98/vid2info/state/element_state/element_state.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:38.130447 vid2info-1.98/vid2info/state/finite_state_machine/
--rw-rw-rw-   0        0        0        0 2022-08-16 10:53:01.000000 vid2info-1.98/vid2info/state/finite_state_machine/__init__.py
--rw-rw-rw-   0        0        0      339 2022-08-24 10:08:23.000000 vid2info-1.98/vid2info/state/finite_state_machine/config_keys.py
--rw-rw-rw-   0        0        0     4874 2023-02-17 17:42:16.000000 vid2info-1.98/vid2info/state/finite_state_machine/element_finite_state_machine.py
--rw-rw-rw-   0        0        0    16940 2023-02-17 17:42:16.000000 vid2info-1.98/vid2info/state/finite_state_machine/track_recoverer.py
--rw-rw-rw-   0        0        0     6349 2023-02-27 10:06:54.000000 vid2info-1.98/vid2info/state/scene_state.py
--rw-rw-rw-   0        0        0    17298 2023-02-27 10:06:54.000000 vid2info-1.98/vid2info/state/state_buffer.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:38.147174 vid2info-1.98/vid2info/utils/
--rw-rw-rw-   0        0        0        0 2022-08-27 11:06:40.000000 vid2info-1.98/vid2info/utils/__init__.py
--rw-rw-rw-   0        0        0       59 2022-08-25 14:27:21.000000 vid2info-1.98/vid2info/utils/config.py
--rw-rw-rw-   0        0        0     3465 2023-02-17 17:26:27.000000 vid2info-1.98/vid2info/utils/general.py
--rw-rw-rw-   0        0        0      942 2023-02-17 17:26:27.000000 vid2info-1.98/vid2info/utils/user_interaction.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:38.170221 vid2info-1.98/vid2info/video/
--rw-rw-rw-   0        0        0        0 2022-08-27 11:06:40.000000 vid2info-1.98/vid2info/video/__init__.py
--rw-rw-rw-   0        0        0     3772 2023-02-17 17:26:27.000000 vid2info-1.98/vid2info/video/_video_reader_multithread.py
--rw-rw-rw-   0        0        0     1385 2023-02-17 17:26:28.000000 vid2info-1.98/vid2info/video/_webcam_reader_multithread.py
--rw-rw-rw-   0        0        0       63 2023-01-12 21:33:48.000000 vid2info-1.98/vid2info/video/config.py
--rw-rw-rw-   0        0        0     1109 2023-02-17 17:26:27.000000 vid2info-1.98/vid2info/video/utils.py
--rw-rw-rw-   0        0        0    10499 2023-02-17 17:26:27.000000 vid2info-1.98/vid2info/video/video_reader.py
--rw-rw-rw-   0        0        0     5991 2023-02-17 17:26:28.000000 vid2info-1.98/vid2info/video/webcam_reader.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:38.180563 vid2info-1.98/vid2info/visualization/
--rw-rw-rw-   0        0        0        0 2022-08-27 11:06:40.000000 vid2info-1.98/vid2info/visualization/__init__.py
--rw-rw-rw-   0        0        0     1542 2022-08-25 11:57:24.000000 vid2info-1.98/vid2info/visualization/config.py
--rw-rw-rw-   0        0        0     1658 2023-02-17 17:26:27.000000 vid2info-1.98/vid2info/visualization/general_utils.py
--rw-rw-rw-   0        0        0    21538 2023-02-27 10:06:54.000000 vid2info-1.98/vid2info/visualization/overlay_utils.py
--rw-rw-rw-   0        0        0     7565 2023-02-17 17:26:27.000000 vid2info-1.98/vid2info/visualization/stream_visualization.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:37.997466 vid2info-1.98/vid2info.egg-info/
--rw-rw-rw-   0        0        0     1017 2023-02-27 11:49:36.000000 vid2info-1.98/vid2info.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     9214 2023-02-27 11:49:36.000000 vid2info-1.98/vid2info.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       63 2023-02-27 11:49:36.000000 vid2info-1.98/vid2info.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-02-27 11:49:36.000000 vid2info-1.98/vid2info.egg-info/requires.txt
--rw-rw-rw-   0        0        0       87 2023-02-27 11:49:36.000000 vid2info-1.98/vid2info.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:36.319423 vid2info-1.98/yolov6/
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:38.213981 vid2info-1.98/yolov6/core/
--rw-rw-rw-   0        0        0    12380 2022-07-09 14:36:48.000000 vid2info-1.98/yolov6/core/engine.py
--rw-rw-rw-   0        0        0    11129 2022-07-09 14:36:48.000000 vid2info-1.98/yolov6/core/evaler.py
--rw-rw-rw-   0        0        0     9349 2022-07-09 14:36:48.000000 vid2info-1.98/yolov6/core/inferer.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:38.280519 vid2info-1.98/yolov6/data/
--rw-rw-rw-   0        0        0     8049 2022-07-09 14:36:48.000000 vid2info-1.98/yolov6/data/data_augment.py
--rw-rw-rw-   0        0        0     2890 2022-07-09 14:36:48.000000 vid2info-1.98/yolov6/data/data_load.py
--rw-rw-rw-   0        0        0    21160 2022-07-09 21:27:33.000000 vid2info-1.98/yolov6/data/datasets.py
--rw-rw-rw-   0        0        0     2347 2022-07-09 14:36:48.000000 vid2info-1.98/yolov6/data/vis_dataset.py
--rw-rw-rw-   0        0        0     4106 2022-07-09 14:36:48.000000 vid2info-1.98/yolov6/data/voc2yolo.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:38.306177 vid2info-1.98/yolov6/layers/
--rw-rw-rw-   0        0        0    21559 2022-07-09 14:36:48.000000 vid2info-1.98/yolov6/layers/common.py
--rw-rw-rw-   0        0        0     1963 2022-07-09 14:36:48.000000 vid2info-1.98/yolov6/layers/dbb_transforms.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:38.366504 vid2info-1.98/yolov6/models/
--rw-rw-rw-   0        0        0     2890 2022-07-09 14:36:48.000000 vid2info-1.98/yolov6/models/efficientrep.py
--rw-rw-rw-   0        0        0     7335 2022-07-17 14:32:31.000000 vid2info-1.98/yolov6/models/effidehead.py
--rw-rw-rw-   0        0        0     6380 2022-07-09 14:36:48.000000 vid2info-1.98/yolov6/models/end2end.py
--rw-rw-rw-   0        0        0    16754 2022-07-17 14:32:31.000000 vid2info-1.98/yolov6/models/loss.py
--rw-rw-rw-   0        0        0     3162 2022-07-09 14:36:48.000000 vid2info-1.98/yolov6/models/reppan.py
--rw-rw-rw-   0        0        0     3012 2022-07-09 21:27:33.000000 vid2info-1.98/yolov6/models/yolo.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:38.380633 vid2info-1.98/yolov6/solver/
--rw-rw-rw-   0        0        0     1543 2022-07-09 14:36:48.000000 vid2info-1.98/yolov6/solver/build.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:38.497064 vid2info-1.98/yolov6/utils/
--rw-rw-rw-   0        0        0     2267 2022-07-17 14:33:20.000000 vid2info-1.98/yolov6/utils/checkpoint.py
--rw-rw-rw-   0        0        0     3165 2022-07-09 14:36:48.000000 vid2info-1.98/yolov6/utils/config.py
--rw-rw-rw-   0        0        0     2434 2022-07-09 14:36:48.000000 vid2info-1.98/yolov6/utils/ema.py
--rw-rw-rw-   0        0        0     1576 2022-07-09 14:36:48.000000 vid2info-1.98/yolov6/utils/envs.py
--rw-rw-rw-   0        0        0     1335 2022-07-10 17:16:57.000000 vid2info-1.98/yolov6/utils/events.py
--rw-rw-rw-   0        0        0     5096 2022-07-09 14:36:48.000000 vid2info-1.98/yolov6/utils/figure_iou.py
--rw-rw-rw-   0        0        0      765 2022-07-09 14:36:48.000000 vid2info-1.98/yolov6/utils/general.py
--rw-rw-rw-   0        0        0     5121 2022-08-02 07:10:46.000000 vid2info-1.98/yolov6/utils/nms.py
--rw-rw-rw-   0        0        0     3483 2022-07-09 14:36:48.000000 vid2info-1.98/yolov6/utils/torch_utils.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:36.319423 vid2info-1.98/yolov7/
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:38.531357 vid2info-1.98/yolov7/models/
--rw-rw-rw-   0        0        0    84376 2022-08-27 11:29:05.000000 vid2info-1.98/yolov7/models/common.py
--rw-rw-rw-   0        0        0    10287 2022-08-27 11:29:05.000000 vid2info-1.98/yolov7/models/experimental.py
--rw-rw-rw-   0        0        0    40038 2022-08-27 11:29:15.000000 vid2info-1.98/yolov7/models/yolo.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:38.664294 vid2info-1.98/yolov7/utils/
--rw-rw-rw-   0        0        0     2248 2022-08-23 00:27:01.000000 vid2info-1.98/yolov7/utils/activations.py
--rw-rw-rw-   0        0        0     5616 2022-08-23 00:27:01.000000 vid2info-1.98/yolov7/utils/add_nms.py
--rw-rw-rw-   0        0        0     7154 2022-08-27 11:31:22.000000 vid2info-1.98/yolov7/utils/autoanchor.py
--rw-rw-rw-   0        0        0    56087 2022-08-27 11:29:32.000000 vid2info-1.98/yolov7/utils/datasets.py
--rw-rw-rw-   0        0        0    36842 2022-08-27 11:29:42.000000 vid2info-1.98/yolov7/utils/general.py
--rw-rw-rw-   0        0        0     4877 2022-08-27 11:01:12.000000 vid2info-1.98/yolov7/utils/google_utils.py
--rw-rw-rw-   0        0        0    74958 2022-08-27 11:31:34.000000 vid2info-1.98/yolov7/utils/loss.py
--rw-rw-rw-   0        0        0     8969 2022-08-23 00:27:01.000000 vid2info-1.98/yolov7/utils/metrics.py
--rw-rw-rw-   0        0        0    20935 2022-08-27 11:30:08.000000 vid2info-1.98/yolov7/utils/plots.py
--rw-rw-rw-   0        0        0    15340 2022-08-29 23:17:20.000000 vid2info-1.98/yolov7/utils/torch_utils.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:38.682010 vid2info-1.98/yolox/
--rw-rw-rw-   0        0        0      134 2022-08-27 11:06:45.000000 vid2info-1.98/yolox/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:38.731211 vid2info-1.98/yolox/core/
--rw-rw-rw-   0        0        0      158 2022-07-13 17:44:25.000000 vid2info-1.98/yolox/core/__init__.py
--rw-rw-rw-   0        0        0     7257 2022-07-13 17:44:25.000000 vid2info-1.98/yolox/core/launch.py
--rw-rw-rw-   0        0        0    11334 2022-07-13 17:44:25.000000 vid2info-1.98/yolox/core/trainer.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:38.831861 vid2info-1.98/yolox/data/
--rw-rw-rw-   0        0        0      339 2022-07-13 17:44:25.000000 vid2info-1.98/yolox/data/__init__.py
--rw-rw-rw-   0        0        0     9677 2022-07-13 17:44:25.000000 vid2info-1.98/yolox/data/data_augment.py
--rw-rw-rw-   0        0        0     2375 2022-07-13 17:44:25.000000 vid2info-1.98/yolox/data/data_prefetcher.py
--rw-rw-rw-   0        0        0     6409 2022-07-13 17:44:25.000000 vid2info-1.98/yolox/data/dataloading.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:38.909335 vid2info-1.98/yolox/data/datasets/
--rw-rw-rw-   0        0        0      247 2022-07-13 17:44:25.000000 vid2info-1.98/yolox/data/datasets/__init__.py
--rw-rw-rw-   0        0        0     4378 2022-07-13 17:44:25.000000 vid2info-1.98/yolox/data/datasets/datasets_wrapper.py
--rw-rw-rw-   0        0        0    10438 2022-07-13 17:44:25.000000 vid2info-1.98/yolox/data/datasets/mosaicdetection.py
--rw-rw-rw-   0        0        0     4596 2022-07-13 17:44:25.000000 vid2info-1.98/yolox/data/datasets/mot.py
--rw-rw-rw-   0        0        0     3451 2022-07-13 17:44:25.000000 vid2info-1.98/yolox/data/samplers.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:39.017762 vid2info-1.98/yolox/deepsort_tracker/
--rw-rw-rw-   0        0        0        0 2022-07-13 17:52:59.000000 vid2info-1.98/yolox/deepsort_tracker/__init__.py
--rw-rw-rw-   0        0        0    11343 2022-07-13 17:44:25.000000 vid2info-1.98/yolox/deepsort_tracker/deepsort.py
--rw-rw-rw-   0        0        0     1474 2022-07-13 17:44:25.000000 vid2info-1.98/yolox/deepsort_tracker/detection.py
--rw-rw-rw-   0        0        0     2932 2022-07-13 17:44:25.000000 vid2info-1.98/yolox/deepsort_tracker/iou_matching.py
--rw-rw-rw-   0        0        0     7972 2022-07-13 17:44:25.000000 vid2info-1.98/yolox/deepsort_tracker/kalman_filter.py
--rw-rw-rw-   0        0        0     8059 2022-07-13 17:44:25.000000 vid2info-1.98/yolox/deepsort_tracker/linear_assignment.py
--rw-rw-rw-   0        0        0     4889 2022-07-13 17:44:25.000000 vid2info-1.98/yolox/deepsort_tracker/reid_model.py
--rw-rw-rw-   0        0        0     5222 2022-07-13 17:44:25.000000 vid2info-1.98/yolox/deepsort_tracker/track.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:39.080735 vid2info-1.98/yolox/evaluators/
--rw-rw-rw-   0        0        0      184 2022-07-13 17:44:25.000000 vid2info-1.98/yolox/evaluators/__init__.py
--rw-rw-rw-   0        0        0     7700 2022-07-13 17:44:25.000000 vid2info-1.98/yolox/evaluators/coco_evaluator.py
--rw-rw-rw-   0        0        0     6761 2022-07-13 17:44:25.000000 vid2info-1.98/yolox/evaluators/evaluation.py
--rw-rw-rw-   0        0        0    25910 2022-07-13 17:44:25.000000 vid2info-1.98/yolox/evaluators/mot_evaluator.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:39.132056 vid2info-1.98/yolox/exp/
--rw-rw-rw-   0        0        0      198 2022-07-13 17:44:25.000000 vid2info-1.98/yolox/exp/__init__.py
--rw-rw-rw-   0        0        0     2079 2022-07-13 17:44:25.000000 vid2info-1.98/yolox/exp/base_exp.py
--rw-rw-rw-   0        0        0     1546 2022-07-13 17:44:25.000000 vid2info-1.98/yolox/exp/build.py
--rw-rw-rw-   0        0        0     8475 2022-07-13 17:44:25.000000 vid2info-1.98/yolox/exp/yolox_base.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:39.164481 vid2info-1.98/yolox/layers/
--rw-rw-rw-   0        0        0      156 2022-07-13 17:44:25.000000 vid2info-1.98/yolox/layers/__init__.py
--rw-rw-rw-   0        0        0     5907 2022-08-21 10:28:39.000000 vid2info-1.98/yolox/layers/fast_coco_eval_api.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:39.299152 vid2info-1.98/yolox/models/
--rw-rw-rw-   0        0        0      307 2022-07-13 17:44:25.000000 vid2info-1.98/yolox/models/__init__.py
--rw-rw-rw-   0        0        0     6207 2022-07-13 17:44:25.000000 vid2info-1.98/yolox/models/darknet.py
--rw-rw-rw-   0        0        0     2980 2022-07-13 17:44:25.000000 vid2info-1.98/yolox/models/losses.py
--rw-rw-rw-   0        0        0     6312 2022-07-13 17:44:25.000000 vid2info-1.98/yolox/models/network_blocks.py
--rw-rw-rw-   0        0        0     2570 2022-07-13 17:44:25.000000 vid2info-1.98/yolox/models/yolo_fpn.py
--rw-rw-rw-   0        0        0    24776 2022-07-17 14:32:31.000000 vid2info-1.98/yolox/models/yolo_head.py
--rw-rw-rw-   0        0        0     3656 2022-07-13 17:44:25.000000 vid2info-1.98/yolox/models/yolo_pafpn.py
--rw-rw-rw-   0        0        0     1422 2022-07-13 17:44:25.000000 vid2info-1.98/yolox/models/yolox.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:39.380811 vid2info-1.98/yolox/motdt_tracker/
--rw-rw-rw-   0        0        0        0 2022-07-13 17:52:59.000000 vid2info-1.98/yolox/motdt_tracker/__init__.py
--rw-rw-rw-   0        0        0     1095 2022-07-13 17:44:25.000000 vid2info-1.98/yolox/motdt_tracker/basetrack.py
--rw-rw-rw-   0        0        0     9816 2022-07-13 17:44:25.000000 vid2info-1.98/yolox/motdt_tracker/kalman_filter.py
--rw-rw-rw-   0        0        0     3882 2022-07-13 17:44:25.000000 vid2info-1.98/yolox/motdt_tracker/matching.py
--rw-rw-rw-   0        0        0    13713 2022-07-13 17:44:25.000000 vid2info-1.98/yolox/motdt_tracker/motdt_tracker.py
--rw-rw-rw-   0        0        0     8679 2022-08-21 10:28:50.000000 vid2info-1.98/yolox/motdt_tracker/reid_model.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:39.397554 vid2info-1.98/yolox/sort_tracker/
--rw-rw-rw-   0        0        0        0 2022-07-13 17:52:59.000000 vid2info-1.98/yolox/sort_tracker/__init__.py
--rw-rw-rw-   0        0        0     8921 2022-07-13 17:44:25.000000 vid2info-1.98/yolox/sort_tracker/sort.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:39.432693 vid2info-1.98/yolox/tracker/
--rw-rw-rw-   0        0        0        0 2022-07-13 17:52:59.000000 vid2info-1.98/yolox/tracker/__init__.py
--rw-rw-rw-   0        0        0     1003 2022-07-13 17:44:25.000000 vid2info-1.98/yolox/tracker/basetrack.py
--rw-rw-rw-   0        0        0    12633 2022-07-17 14:10:35.000000 vid2info-1.98/yolox/tracker/byte_tracker.py
--rw-rw-rw-   0        0        0     9816 2022-07-13 17:44:25.000000 vid2info-1.98/yolox/tracker/kalman_filter.py
--rw-rw-rw-   0        0        0     6380 2022-07-13 17:44:25.000000 vid2info-1.98/yolox/tracker/matching.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:39.464071 vid2info-1.98/yolox/tracking_utils/
--rw-rw-rw-   0        0        0        0 2022-07-13 17:52:59.000000 vid2info-1.98/yolox/tracking_utils/__init__.py
--rw-rw-rw-   0        0        0     4162 2022-07-13 17:44:25.000000 vid2info-1.98/yolox/tracking_utils/evaluation.py
--rw-rw-rw-   0        0        0     3742 2022-07-13 17:44:25.000000 vid2info-1.98/yolox/tracking_utils/io.py
--rw-rw-rw-   0        0        0      994 2022-07-13 17:44:25.000000 vid2info-1.98/yolox/tracking_utils/timer.py
-drwxrwxrwx   0        0        0        0 2023-02-27 11:49:39.605013 vid2info-1.98/yolox/utils/
--rw-rw-rw-   0        0        0      466 2022-07-13 17:44:26.000000 vid2info-1.98/yolox/utils/__init__.py
--rw-rw-rw-   0        0        0     2948 2022-07-13 17:44:26.000000 vid2info-1.98/yolox/utils/allreduce_norm.py
--rw-rw-rw-   0        0        0     4601 2022-07-13 17:44:26.000000 vid2info-1.98/yolox/utils/boxes.py
--rw-rw-rw-   0        0        0     1375 2022-07-13 17:44:26.000000 vid2info-1.98/yolox/utils/checkpoint.py
--rw-rw-rw-   0        0        0     2902 2022-07-13 17:44:26.000000 vid2info-1.98/yolox/utils/demo_utils.py
--rw-rw-rw-   0        0        0     7321 2022-07-13 17:44:26.000000 vid2info-1.98/yolox/utils/dist.py
--rw-rw-rw-   0        0        0     2605 2022-07-13 17:44:26.000000 vid2info-1.98/yolox/utils/ema.py
--rw-rw-rw-   0        0        0     2847 2022-07-13 17:44:26.000000 vid2info-1.98/yolox/utils/logger.py
--rw-rw-rw-   0        0        0     6766 2022-07-13 17:44:26.000000 vid2info-1.98/yolox/utils/lr_scheduler.py
--rw-rw-rw-   0        0        0     3217 2022-07-13 17:44:26.000000 vid2info-1.98/yolox/utils/metric.py
--rw-rw-rw-   0        0        0     3375 2022-07-13 17:44:26.000000 vid2info-1.98/yolox/utils/model_utils.py
--rw-rw-rw-   0        0        0     1625 2022-07-13 17:44:26.000000 vid2info-1.98/yolox/utils/setup_env.py
--rw-rw-rw-   0        0        0     5124 2022-07-13 17:44:26.000000 vid2info-1.98/yolox/utils/visualize.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:46.016862 vid2info-1.99/
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.449560 vid2info-1.99/ByteTrack/
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.382251 vid2info-1.99/ByteTrack/deploy/
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.449560 vid2info-1.99/ByteTrack/deploy/ONNXRuntime/
+-rw-rw-rw-   0        0        0     5855 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/deploy/ONNXRuntime/onnx_inference.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.382916 vid2info-1.99/ByteTrack/exps/
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.466256 vid2info-1.99/ByteTrack/exps/default/
+-rw-rw-rw-   0        0        0     1359 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/exps/default/nano.py
+-rw-rw-rw-   0        0        0     3095 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/exps/default/yolov3.py
+-rw-rw-rw-   0        0        0      370 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/exps/default/yolox_l.py
+-rw-rw-rw-   0        0        0      372 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/exps/default/yolox_m.py
+-rw-rw-rw-   0        0        0      372 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/exps/default/yolox_s.py
+-rw-rw-rw-   0        0        0      515 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/exps/default/yolox_tiny.py
+-rw-rw-rw-   0        0        0      372 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/exps/default/yolox_x.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.382916 vid2info-1.99/ByteTrack/exps/example/
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.500129 vid2info-1.99/ByteTrack/exps/example/mot/
+-rw-rw-rw-   0        0        0     4490 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/exps/example/mot/yolox_l_mix_det.py
+-rw-rw-rw-   0        0        0     4492 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/exps/example/mot/yolox_m_mix_det.py
+-rw-rw-rw-   0        0        0     5347 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/exps/example/mot/yolox_nano_mix_det.py
+-rw-rw-rw-   0        0        0     4492 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/exps/example/mot/yolox_s_mix_det.py
+-rw-rw-rw-   0        0        0     4526 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/exps/example/mot/yolox_tiny_mix_det.py
+-rw-rw-rw-   0        0        0     4496 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/exps/example/mot/yolox_x_ablation.py
+-rw-rw-rw-   0        0        0     4492 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/exps/example/mot/yolox_x_ch.py
+-rw-rw-rw-   0        0        0     4594 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/exps/example/mot/yolox_x_mix_det.py
+-rw-rw-rw-   0        0        0     4637 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/exps/example/mot/yolox_x_mix_mot20_ch.py
+-rw-rw-rw-   0        0        0     4494 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/exps/example/mot/yolox_x_mot17_half.py
+-rw-rw-rw-   0        0        0     1740 2022-07-13 17:53:10.000000 vid2info-1.99/ByteTrack/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.382916 vid2info-1.99/ByteTrack/src/
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.502645 vid2info-1.99/ByteTrack/src/cython-bbox/
+-rw-rw-rw-   0        0        0     1350 2022-08-05 22:30:19.000000 vid2info-1.99/ByteTrack/src/cython-bbox/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.533301 vid2info-1.99/ByteTrack/tools/
+-rw-rw-rw-   0        0        0     2541 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tools/convert_cityperson_to_coco.py
+-rw-rw-rw-   0        0        0     2337 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tools/convert_crowdhuman_to_coco.py
+-rw-rw-rw-   0        0        0     2527 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tools/convert_ethz_to_coco.py
+-rw-rw-rw-   0        0        0     6889 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tools/convert_mot17_to_coco.py
+-rw-rw-rw-   0        0        0     6821 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tools/convert_mot20_to_coco.py
+-rw-rw-rw-   0        0        0      884 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tools/convert_video.py
+-rw-rw-rw-   0        0        0    13970 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tools/demo_track.py
+-rw-rw-rw-   0        0        0     3150 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tools/export_onnx.py
+-rw-rw-rw-   0        0        0     5732 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tools/interpolation.py
+-rw-rw-rw-   0        0        0     2569 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tools/mix_data_ablation.py
+-rw-rw-rw-   0        0        0     4070 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tools/mix_data_test_mot17.py
+-rw-rw-rw-   0        0        0     2520 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tools/mix_data_test_mot20.py
+-rw-rw-rw-   0        0        0     3498 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tools/mota.py
+-rw-rw-rw-   0        0        0    10667 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tools/track.py
+-rw-rw-rw-   0        0        0    10657 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tools/track_deepsort.py
+-rw-rw-rw-   0        0        0    10681 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tools/track_motdt.py
+-rw-rw-rw-   0        0        0    10467 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tools/track_sort.py
+-rw-rw-rw-   0        0        0     3559 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tools/train.py
+-rw-rw-rw-   0        0        0     2217 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tools/trt.py
+-rw-rw-rw-   0        0        0     7405 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tools/txt2video.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.402530 vid2info-1.99/ByteTrack/tutorials/
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.549627 vid2info-1.99/ByteTrack/tutorials/centertrack/
+-rw-rw-rw-   0        0        0    13599 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tutorials/centertrack/byte_tracker.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.549627 vid2info-1.99/ByteTrack/tutorials/centertrack/mot_online/
+-rw-rw-rw-   0        0        0     1003 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tutorials/centertrack/mot_online/basetrack.py
+-rw-rw-rw-   0        0        0     9816 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tutorials/centertrack/mot_online/kalman_filter.py
+-rw-rw-rw-   0        0        0     7746 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tutorials/centertrack/mot_online/matching.py
+-rw-rw-rw-   0        0        0    21716 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tutorials/centertrack/opts.py
+-rw-rw-rw-   0        0        0     9103 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tutorials/centertrack/tracker.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.566081 vid2info-1.99/ByteTrack/tutorials/cstrack/
+-rw-rw-rw-   0        0        0    21156 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tutorials/cstrack/byte_tracker.py
+-rw-rw-rw-   0        0        0    23301 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tutorials/cstrack/tracker.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.566081 vid2info-1.99/ByteTrack/tutorials/ctracker/
+-rw-rw-rw-   0        0        0    12165 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tutorials/ctracker/byte_tracker.py
+-rw-rw-rw-   0        0        0     5318 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tutorials/ctracker/eval_motchallenge.py
+-rw-rw-rw-   0        0        0     1615 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tutorials/ctracker/generate_half_csv.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.581783 vid2info-1.99/ByteTrack/tutorials/ctracker/mot_online/
+-rw-rw-rw-   0        0        0     1003 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tutorials/ctracker/mot_online/basetrack.py
+-rw-rw-rw-   0        0        0     9816 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tutorials/ctracker/mot_online/kalman_filter.py
+-rw-rw-rw-   0        0        0     7746 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tutorials/ctracker/mot_online/matching.py
+-rw-rw-rw-   0        0        0    12268 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tutorials/ctracker/test.py
+-rw-rw-rw-   0        0        0     6109 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tutorials/ctracker/test_byte.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.582756 vid2info-1.99/ByteTrack/tutorials/fairmot/
+-rw-rw-rw-   0        0        0    15246 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tutorials/fairmot/byte_tracker.py
+-rw-rw-rw-   0        0        0    18050 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tutorials/fairmot/tracker.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.582756 vid2info-1.99/ByteTrack/tutorials/jde/
+-rw-rw-rw-   0        0        0    15527 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tutorials/jde/byte_tracker.py
+-rw-rw-rw-   0        0        0     3698 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tutorials/jde/evaluation.py
+-rw-rw-rw-   0        0        0     9076 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tutorials/jde/track_half.py
+-rw-rw-rw-   0        0        0    17846 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tutorials/jde/tracker.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.602546 vid2info-1.99/ByteTrack/tutorials/motr/
+-rw-rw-rw-   0        0        0    12066 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tutorials/motr/byte_tracker.py
+-rw-rw-rw-   0        0        0    19720 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tutorials/motr/eval.py
+-rw-rw-rw-   0        0        0     7705 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tutorials/motr/evaluation.py
+-rw-rw-rw-   0        0        0    12162 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tutorials/motr/joint.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.615298 vid2info-1.99/ByteTrack/tutorials/motr/mot_online/
+-rw-rw-rw-   0        0        0     1003 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tutorials/motr/mot_online/basetrack.py
+-rw-rw-rw-   0        0        0     9782 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tutorials/motr/mot_online/kalman_filter.py
+-rw-rw-rw-   0        0        0     7742 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tutorials/motr/mot_online/matching.py
+-rw-rw-rw-   0        0        0    33632 2022-08-05 22:30:19.000000 vid2info-1.99/ByteTrack/tutorials/motr/motr.py
+-rw-rw-rw-   0        0        0    33693 2022-08-05 22:30:19.000000 vid2info-1.99/ByteTrack/tutorials/motr/motr_det.py
+-rw-rw-rw-   0        0        0    22324 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tutorials/motr/transforms.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.615950 vid2info-1.99/ByteTrack/tutorials/qdtrack/
+-rw-rw-rw-   0        0        0    12720 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tutorials/qdtrack/byte_tracker.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.615950 vid2info-1.99/ByteTrack/tutorials/qdtrack/mot_online/
+-rw-rw-rw-   0        0        0     1003 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tutorials/qdtrack/mot_online/basetrack.py
+-rw-rw-rw-   0        0        0     9816 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tutorials/qdtrack/mot_online/kalman_filter.py
+-rw-rw-rw-   0        0        0     7746 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tutorials/qdtrack/mot_online/matching.py
+-rw-rw-rw-   0        0        0     6169 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tutorials/qdtrack/qdtrack.py
+-rw-rw-rw-   0        0        0    14737 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tutorials/qdtrack/tracker_reid_motion.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.632867 vid2info-1.99/ByteTrack/tutorials/trades/
+-rw-rw-rw-   0        0        0    13321 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tutorials/trades/byte_tracker.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.632867 vid2info-1.99/ByteTrack/tutorials/trades/mot_online/
+-rw-rw-rw-   0        0        0     1003 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tutorials/trades/mot_online/basetrack.py
+-rw-rw-rw-   0        0        0     9782 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tutorials/trades/mot_online/kalman_filter.py
+-rw-rw-rw-   0        0        0     7742 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tutorials/trades/mot_online/matching.py
+-rw-rw-rw-   0        0        0    23334 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tutorials/trades/opts.py
+-rw-rw-rw-   0        0        0    14902 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tutorials/trades/tracker.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.632867 vid2info-1.99/ByteTrack/tutorials/transtrack/
+-rw-rw-rw-   0        0        0    12497 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tutorials/transtrack/engine_track.py
+-rw-rw-rw-   0        0        0    18928 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tutorials/transtrack/main_track.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.649015 vid2info-1.99/ByteTrack/tutorials/transtrack/mot_online/
+-rw-rw-rw-   0        0        0     1001 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tutorials/transtrack/mot_online/basetrack.py
+-rw-rw-rw-   0        0        0    12950 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tutorials/transtrack/mot_online/byte_tracker.py
+-rw-rw-rw-   0        0        0     9816 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tutorials/transtrack/mot_online/kalman_filter.py
+-rw-rw-rw-   0        0        0     5486 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tutorials/transtrack/mot_online/matching.py
+-rw-rw-rw-   0        0        0     1954 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tutorials/transtrack/save_track.py
+-rw-rw-rw-   0        0        0     7685 2022-07-13 17:44:25.000000 vid2info-1.99/ByteTrack/tutorials/transtrack/tracker.py
+-rw-rw-rw-   0        0        0    35823 2022-08-04 07:27:36.000000 vid2info-1.99/LICENSE
+-rw-rw-rw-   0        0        0     1017 2023-02-27 12:29:46.016862 vid2info-1.99/PKG-INFO
+-rw-rw-rw-   0        0        0      163 2022-08-29 23:06:12.000000 vid2info-1.99/README.md
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.649015 vid2info-1.99/models/
+-rw-rw-rw-   0        0        0    84376 2022-08-27 11:30:35.000000 vid2info-1.99/models/common.py
+-rw-rw-rw-   0        0        0    10287 2022-08-27 11:30:49.000000 vid2info-1.99/models/experimental.py
+-rw-rw-rw-   0        0        0    40052 2022-08-27 11:31:12.000000 vid2info-1.99/models/yolo.py
+-rw-rw-rw-   0        0        0      111 2023-02-27 12:29:46.032672 vid2info-1.99/setup.cfg
+-rw-rw-rw-   0        0        0     1321 2023-02-27 12:29:40.000000 vid2info-1.99/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.402530 vid2info-1.99/third_party/
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.649015 vid2info-1.99/third_party/pidnet/
+-rw-rw-rw-   0        0        0    17118 2022-07-23 14:51:56.000000 vid2info-1.99/third_party/pidnet/model_utils.py
+-rw-rw-rw-   0        0        0    11938 2022-07-30 12:58:40.000000 vid2info-1.99/third_party/pidnet/pidnet.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.665165 vid2info-1.99/training_tools/
+-rw-rw-rw-   0        0        0      392 2022-07-22 17:05:37.000000 vid2info-1.99/training_tools/config.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.666305 vid2info-1.99/training_tools/dataset_generation/
+-rw-rw-rw-   0        0        0      158 2022-07-24 20:53:38.000000 vid2info-1.99/training_tools/dataset_generation/config.py
+-rw-rw-rw-   0        0        0     3508 2022-08-05 22:30:19.000000 vid2info-1.99/training_tools/dataset_generation/video_extractor.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.682649 vid2info-1.99/utils/
+-rw-rw-rw-   0        0        0     2248 2022-08-23 00:27:01.000000 vid2info-1.99/utils/activations.py
+-rw-rw-rw-   0        0        0     5616 2022-08-23 00:27:01.000000 vid2info-1.99/utils/add_nms.py
+-rw-rw-rw-   0        0        0     7147 2022-08-23 00:27:01.000000 vid2info-1.99/utils/autoanchor.py
+-rw-rw-rw-   0        0        0    56073 2022-08-27 11:11:53.000000 vid2info-1.99/utils/datasets.py
+-rw-rw-rw-   0        0        0    36821 2022-08-27 11:11:53.000000 vid2info-1.99/utils/general.py
+-rw-rw-rw-   0        0        0     4877 2022-08-27 11:01:12.000000 vid2info-1.99/utils/google_utils.py
+-rw-rw-rw-   0        0        0    74944 2022-08-23 00:27:01.000000 vid2info-1.99/utils/loss.py
+-rw-rw-rw-   0        0        0     8969 2022-08-23 00:27:01.000000 vid2info-1.99/utils/metrics.py
+-rw-rw-rw-   0        0        0    20921 2022-08-27 11:11:53.000000 vid2info-1.99/utils/plots.py
+-rw-rw-rw-   0        0        0    15467 2022-08-23 00:27:01.000000 vid2info-1.99/utils/torch_utils.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.682649 vid2info-1.99/vid2info/
+-rw-rw-rw-   0        0        0        0 2022-08-24 13:19:17.000000 vid2info-1.99/vid2info/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.716403 vid2info-1.99/vid2info/inference/
+-rw-rw-rw-   0        0        0        0 2022-08-27 10:53:11.000000 vid2info-1.99/vid2info/inference/__init__.py
+-rw-rw-rw-   0        0        0      515 2022-08-05 22:30:19.000000 vid2info-1.99/vid2info/inference/config.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.736211 vid2info-1.99/vid2info/inference/detection/
+-rw-rw-rw-   0        0        0        0 2022-08-27 11:06:40.000000 vid2info-1.99/vid2info/inference/detection/__init__.py
+-rw-rw-rw-   0        0        0    13801 2023-02-17 17:26:27.000000 vid2info-1.99/vid2info/inference/detection/__yolo_detector.py
+-rw-rw-rw-   0        0        0      569 2022-08-29 23:12:12.000000 vid2info-1.99/vid2info/inference/detection/config.py
+-rw-rw-rw-   0        0        0     3956 2023-02-17 17:26:27.000000 vid2info-1.99/vid2info/inference/detection/yolov6_detector.py
+-rw-rw-rw-   0        0        0     4367 2023-02-17 17:26:28.000000 vid2info-1.99/vid2info/inference/detection/yolov7_detector.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.416002 vid2info-1.99/vid2info/inference/models/
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.736211 vid2info-1.99/vid2info/inference/models/finite_state_machine_configs/
+-rw-rw-rw-   0        0        0     1004 2023-02-17 17:26:27.000000 vid2info-1.99/vid2info/inference/models/finite_state_machine_configs/dummy_finite_state_config.py
+-rw-rw-rw-   0        0        0    13020 2023-02-27 10:06:54.000000 vid2info-1.99/vid2info/inference/pipeline.py
+-rw-rw-rw-   0        0        0    11130 2023-02-27 10:06:54.000000 vid2info-1.99/vid2info/inference/pipeline_background.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.736211 vid2info-1.99/vid2info/inference/segmentation/
+-rw-rw-rw-   0        0        0        0 2022-08-27 11:06:40.000000 vid2info-1.99/vid2info/inference/segmentation/__init__.py
+-rw-rw-rw-   0        0        0      379 2022-08-29 23:24:48.000000 vid2info-1.99/vid2info/inference/segmentation/config.py
+-rw-rw-rw-   0        0        0    13193 2023-02-17 17:26:27.000000 vid2info-1.99/vid2info/inference/segmentation/pidnet_segmenter.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.749424 vid2info-1.99/vid2info/inference/tracking/
+-rw-rw-rw-   0        0        0        0 2022-08-27 11:06:40.000000 vid2info-1.99/vid2info/inference/tracking/__init__.py
+-rw-rw-rw-   0        0        0      168 2022-08-05 17:43:54.000000 vid2info-1.99/vid2info/inference/tracking/config.py
+-rw-rw-rw-   0        0        0     7378 2023-02-17 18:05:16.000000 vid2info-1.99/vid2info/inference/tracking/tracker.py
+-rw-rw-rw-   0        0        0     7932 2023-02-17 17:26:27.000000 vid2info-1.99/vid2info/inference/utils.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.749424 vid2info-1.99/vid2info/state/
+-rw-rw-rw-   0        0        0        0 2022-08-11 07:28:01.000000 vid2info-1.99/vid2info/state/__init__.py
+-rw-rw-rw-   0        0        0      570 2022-09-11 20:42:48.000000 vid2info-1.99/vid2info/state/config.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.766752 vid2info-1.99/vid2info/state/element_state/
+-rw-rw-rw-   0        0        0        0 2023-02-27 09:52:37.000000 vid2info-1.99/vid2info/state/element_state/__init__.py
+-rw-rw-rw-   0        0        0      124 2023-02-27 11:23:16.000000 vid2info-1.99/vid2info/state/element_state/constants.py
+-rw-rw-rw-   0        0        0     7922 2023-02-27 12:29:40.000000 vid2info-1.99/vid2info/state/element_state/element_movement.py
+-rw-rw-rw-   0        0        0     5697 2023-02-27 12:29:40.000000 vid2info-1.99/vid2info/state/element_state/element_state.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.766752 vid2info-1.99/vid2info/state/finite_state_machine/
+-rw-rw-rw-   0        0        0        0 2022-08-16 10:53:01.000000 vid2info-1.99/vid2info/state/finite_state_machine/__init__.py
+-rw-rw-rw-   0        0        0      339 2022-08-24 10:08:23.000000 vid2info-1.99/vid2info/state/finite_state_machine/config_keys.py
+-rw-rw-rw-   0        0        0     4874 2023-02-17 17:42:16.000000 vid2info-1.99/vid2info/state/finite_state_machine/element_finite_state_machine.py
+-rw-rw-rw-   0        0        0    16940 2023-02-17 17:42:16.000000 vid2info-1.99/vid2info/state/finite_state_machine/track_recoverer.py
+-rw-rw-rw-   0        0        0     6349 2023-02-27 10:06:54.000000 vid2info-1.99/vid2info/state/scene_state.py
+-rw-rw-rw-   0        0        0    17298 2023-02-27 10:06:54.000000 vid2info-1.99/vid2info/state/state_buffer.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.782515 vid2info-1.99/vid2info/utils/
+-rw-rw-rw-   0        0        0        0 2022-08-27 11:06:40.000000 vid2info-1.99/vid2info/utils/__init__.py
+-rw-rw-rw-   0        0        0       59 2022-08-25 14:27:21.000000 vid2info-1.99/vid2info/utils/config.py
+-rw-rw-rw-   0        0        0     3465 2023-02-17 17:26:27.000000 vid2info-1.99/vid2info/utils/general.py
+-rw-rw-rw-   0        0        0      942 2023-02-17 17:26:27.000000 vid2info-1.99/vid2info/utils/user_interaction.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.782515 vid2info-1.99/vid2info/video/
+-rw-rw-rw-   0        0        0        0 2022-08-27 11:06:40.000000 vid2info-1.99/vid2info/video/__init__.py
+-rw-rw-rw-   0        0        0     3772 2023-02-17 17:26:27.000000 vid2info-1.99/vid2info/video/_video_reader_multithread.py
+-rw-rw-rw-   0        0        0     1385 2023-02-17 17:26:28.000000 vid2info-1.99/vid2info/video/_webcam_reader_multithread.py
+-rw-rw-rw-   0        0        0       63 2023-01-12 21:33:48.000000 vid2info-1.99/vid2info/video/config.py
+-rw-rw-rw-   0        0        0     1109 2023-02-17 17:26:27.000000 vid2info-1.99/vid2info/video/utils.py
+-rw-rw-rw-   0        0        0    10499 2023-02-17 17:26:27.000000 vid2info-1.99/vid2info/video/video_reader.py
+-rw-rw-rw-   0        0        0     5991 2023-02-17 17:26:28.000000 vid2info-1.99/vid2info/video/webcam_reader.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.802693 vid2info-1.99/vid2info/visualization/
+-rw-rw-rw-   0        0        0        0 2022-08-27 11:06:40.000000 vid2info-1.99/vid2info/visualization/__init__.py
+-rw-rw-rw-   0        0        0     1542 2022-08-25 11:57:24.000000 vid2info-1.99/vid2info/visualization/config.py
+-rw-rw-rw-   0        0        0     1658 2023-02-17 17:26:27.000000 vid2info-1.99/vid2info/visualization/general_utils.py
+-rw-rw-rw-   0        0        0    21538 2023-02-27 10:06:54.000000 vid2info-1.99/vid2info/visualization/overlay_utils.py
+-rw-rw-rw-   0        0        0     7565 2023-02-17 17:26:27.000000 vid2info-1.99/vid2info/visualization/stream_visualization.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.716403 vid2info-1.99/vid2info.egg-info/
+-rw-rw-rw-   0        0        0     1017 2023-02-27 12:29:45.000000 vid2info-1.99/vid2info.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     9214 2023-02-27 12:29:45.000000 vid2info-1.99/vid2info.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       63 2023-02-27 12:29:45.000000 vid2info-1.99/vid2info.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-02-27 12:29:45.000000 vid2info-1.99/vid2info.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       87 2023-02-27 12:29:45.000000 vid2info-1.99/vid2info.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.433388 vid2info-1.99/yolov6/
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.802693 vid2info-1.99/yolov6/core/
+-rw-rw-rw-   0        0        0    12380 2022-07-09 14:36:48.000000 vid2info-1.99/yolov6/core/engine.py
+-rw-rw-rw-   0        0        0    11129 2022-07-09 14:36:48.000000 vid2info-1.99/yolov6/core/evaler.py
+-rw-rw-rw-   0        0        0     9349 2022-07-09 14:36:48.000000 vid2info-1.99/yolov6/core/inferer.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.816115 vid2info-1.99/yolov6/data/
+-rw-rw-rw-   0        0        0     8049 2022-07-09 14:36:48.000000 vid2info-1.99/yolov6/data/data_augment.py
+-rw-rw-rw-   0        0        0     2890 2022-07-09 14:36:48.000000 vid2info-1.99/yolov6/data/data_load.py
+-rw-rw-rw-   0        0        0    21160 2022-07-09 21:27:33.000000 vid2info-1.99/yolov6/data/datasets.py
+-rw-rw-rw-   0        0        0     2347 2022-07-09 14:36:48.000000 vid2info-1.99/yolov6/data/vis_dataset.py
+-rw-rw-rw-   0        0        0     4106 2022-07-09 14:36:48.000000 vid2info-1.99/yolov6/data/voc2yolo.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.816115 vid2info-1.99/yolov6/layers/
+-rw-rw-rw-   0        0        0    21559 2022-07-09 14:36:48.000000 vid2info-1.99/yolov6/layers/common.py
+-rw-rw-rw-   0        0        0     1963 2022-07-09 14:36:48.000000 vid2info-1.99/yolov6/layers/dbb_transforms.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.833274 vid2info-1.99/yolov6/models/
+-rw-rw-rw-   0        0        0     2890 2022-07-09 14:36:48.000000 vid2info-1.99/yolov6/models/efficientrep.py
+-rw-rw-rw-   0        0        0     7335 2022-07-17 14:32:31.000000 vid2info-1.99/yolov6/models/effidehead.py
+-rw-rw-rw-   0        0        0     6380 2022-07-09 14:36:48.000000 vid2info-1.99/yolov6/models/end2end.py
+-rw-rw-rw-   0        0        0    16754 2022-07-17 14:32:31.000000 vid2info-1.99/yolov6/models/loss.py
+-rw-rw-rw-   0        0        0     3162 2022-07-09 14:36:48.000000 vid2info-1.99/yolov6/models/reppan.py
+-rw-rw-rw-   0        0        0     3012 2022-07-09 21:27:33.000000 vid2info-1.99/yolov6/models/yolo.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.833274 vid2info-1.99/yolov6/solver/
+-rw-rw-rw-   0        0        0     1543 2022-07-09 14:36:48.000000 vid2info-1.99/yolov6/solver/build.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.865194 vid2info-1.99/yolov6/utils/
+-rw-rw-rw-   0        0        0     2267 2022-07-17 14:33:20.000000 vid2info-1.99/yolov6/utils/checkpoint.py
+-rw-rw-rw-   0        0        0     3165 2022-07-09 14:36:48.000000 vid2info-1.99/yolov6/utils/config.py
+-rw-rw-rw-   0        0        0     2434 2022-07-09 14:36:48.000000 vid2info-1.99/yolov6/utils/ema.py
+-rw-rw-rw-   0        0        0     1576 2022-07-09 14:36:48.000000 vid2info-1.99/yolov6/utils/envs.py
+-rw-rw-rw-   0        0        0     1335 2022-07-10 17:16:57.000000 vid2info-1.99/yolov6/utils/events.py
+-rw-rw-rw-   0        0        0     5096 2022-07-09 14:36:48.000000 vid2info-1.99/yolov6/utils/figure_iou.py
+-rw-rw-rw-   0        0        0      765 2022-07-09 14:36:48.000000 vid2info-1.99/yolov6/utils/general.py
+-rw-rw-rw-   0        0        0     5121 2022-08-02 07:10:46.000000 vid2info-1.99/yolov6/utils/nms.py
+-rw-rw-rw-   0        0        0     3483 2022-07-09 14:36:48.000000 vid2info-1.99/yolov6/utils/torch_utils.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.433388 vid2info-1.99/yolov7/
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.867335 vid2info-1.99/yolov7/models/
+-rw-rw-rw-   0        0        0    84376 2022-08-27 11:29:05.000000 vid2info-1.99/yolov7/models/common.py
+-rw-rw-rw-   0        0        0    10287 2022-08-27 11:29:05.000000 vid2info-1.99/yolov7/models/experimental.py
+-rw-rw-rw-   0        0        0    40038 2022-08-27 11:29:15.000000 vid2info-1.99/yolov7/models/yolo.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.882411 vid2info-1.99/yolov7/utils/
+-rw-rw-rw-   0        0        0     2248 2022-08-23 00:27:01.000000 vid2info-1.99/yolov7/utils/activations.py
+-rw-rw-rw-   0        0        0     5616 2022-08-23 00:27:01.000000 vid2info-1.99/yolov7/utils/add_nms.py
+-rw-rw-rw-   0        0        0     7154 2022-08-27 11:31:22.000000 vid2info-1.99/yolov7/utils/autoanchor.py
+-rw-rw-rw-   0        0        0    56087 2022-08-27 11:29:32.000000 vid2info-1.99/yolov7/utils/datasets.py
+-rw-rw-rw-   0        0        0    36842 2022-08-27 11:29:42.000000 vid2info-1.99/yolov7/utils/general.py
+-rw-rw-rw-   0        0        0     4877 2022-08-27 11:01:12.000000 vid2info-1.99/yolov7/utils/google_utils.py
+-rw-rw-rw-   0        0        0    74958 2022-08-27 11:31:34.000000 vid2info-1.99/yolov7/utils/loss.py
+-rw-rw-rw-   0        0        0     8969 2022-08-23 00:27:01.000000 vid2info-1.99/yolov7/utils/metrics.py
+-rw-rw-rw-   0        0        0    20935 2022-08-27 11:30:08.000000 vid2info-1.99/yolov7/utils/plots.py
+-rw-rw-rw-   0        0        0    15340 2022-08-29 23:17:20.000000 vid2info-1.99/yolov7/utils/torch_utils.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.882411 vid2info-1.99/yolox/
+-rw-rw-rw-   0        0        0      134 2022-08-27 11:06:45.000000 vid2info-1.99/yolox/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.900445 vid2info-1.99/yolox/core/
+-rw-rw-rw-   0        0        0      158 2022-07-13 17:44:25.000000 vid2info-1.99/yolox/core/__init__.py
+-rw-rw-rw-   0        0        0     7257 2022-07-13 17:44:25.000000 vid2info-1.99/yolox/core/launch.py
+-rw-rw-rw-   0        0        0    11334 2022-07-13 17:44:25.000000 vid2info-1.99/yolox/core/trainer.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.902962 vid2info-1.99/yolox/data/
+-rw-rw-rw-   0        0        0      339 2022-07-13 17:44:25.000000 vid2info-1.99/yolox/data/__init__.py
+-rw-rw-rw-   0        0        0     9677 2022-07-13 17:44:25.000000 vid2info-1.99/yolox/data/data_augment.py
+-rw-rw-rw-   0        0        0     2375 2022-07-13 17:44:25.000000 vid2info-1.99/yolox/data/data_prefetcher.py
+-rw-rw-rw-   0        0        0     6409 2022-07-13 17:44:25.000000 vid2info-1.99/yolox/data/dataloading.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.916294 vid2info-1.99/yolox/data/datasets/
+-rw-rw-rw-   0        0        0      247 2022-07-13 17:44:25.000000 vid2info-1.99/yolox/data/datasets/__init__.py
+-rw-rw-rw-   0        0        0     4378 2022-07-13 17:44:25.000000 vid2info-1.99/yolox/data/datasets/datasets_wrapper.py
+-rw-rw-rw-   0        0        0    10438 2022-07-13 17:44:25.000000 vid2info-1.99/yolox/data/datasets/mosaicdetection.py
+-rw-rw-rw-   0        0        0     4596 2022-07-13 17:44:25.000000 vid2info-1.99/yolox/data/datasets/mot.py
+-rw-rw-rw-   0        0        0     3451 2022-07-13 17:44:25.000000 vid2info-1.99/yolox/data/samplers.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.932604 vid2info-1.99/yolox/deepsort_tracker/
+-rw-rw-rw-   0        0        0        0 2022-07-13 17:52:59.000000 vid2info-1.99/yolox/deepsort_tracker/__init__.py
+-rw-rw-rw-   0        0        0    11343 2022-07-13 17:44:25.000000 vid2info-1.99/yolox/deepsort_tracker/deepsort.py
+-rw-rw-rw-   0        0        0     1474 2022-07-13 17:44:25.000000 vid2info-1.99/yolox/deepsort_tracker/detection.py
+-rw-rw-rw-   0        0        0     2932 2022-07-13 17:44:25.000000 vid2info-1.99/yolox/deepsort_tracker/iou_matching.py
+-rw-rw-rw-   0        0        0     7972 2022-07-13 17:44:25.000000 vid2info-1.99/yolox/deepsort_tracker/kalman_filter.py
+-rw-rw-rw-   0        0        0     8059 2022-07-13 17:44:25.000000 vid2info-1.99/yolox/deepsort_tracker/linear_assignment.py
+-rw-rw-rw-   0        0        0     4889 2022-07-13 17:44:25.000000 vid2info-1.99/yolox/deepsort_tracker/reid_model.py
+-rw-rw-rw-   0        0        0     5222 2022-07-13 17:44:25.000000 vid2info-1.99/yolox/deepsort_tracker/track.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.932604 vid2info-1.99/yolox/evaluators/
+-rw-rw-rw-   0        0        0      184 2022-07-13 17:44:25.000000 vid2info-1.99/yolox/evaluators/__init__.py
+-rw-rw-rw-   0        0        0     7700 2022-07-13 17:44:25.000000 vid2info-1.99/yolox/evaluators/coco_evaluator.py
+-rw-rw-rw-   0        0        0     6761 2022-07-13 17:44:25.000000 vid2info-1.99/yolox/evaluators/evaluation.py
+-rw-rw-rw-   0        0        0    25910 2022-07-13 17:44:25.000000 vid2info-1.99/yolox/evaluators/mot_evaluator.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.949510 vid2info-1.99/yolox/exp/
+-rw-rw-rw-   0        0        0      198 2022-07-13 17:44:25.000000 vid2info-1.99/yolox/exp/__init__.py
+-rw-rw-rw-   0        0        0     2079 2022-07-13 17:44:25.000000 vid2info-1.99/yolox/exp/base_exp.py
+-rw-rw-rw-   0        0        0     1546 2022-07-13 17:44:25.000000 vid2info-1.99/yolox/exp/build.py
+-rw-rw-rw-   0        0        0     8475 2022-07-13 17:44:25.000000 vid2info-1.99/yolox/exp/yolox_base.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.949510 vid2info-1.99/yolox/layers/
+-rw-rw-rw-   0        0        0      156 2022-07-13 17:44:25.000000 vid2info-1.99/yolox/layers/__init__.py
+-rw-rw-rw-   0        0        0     5907 2022-08-21 10:28:39.000000 vid2info-1.99/yolox/layers/fast_coco_eval_api.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.966104 vid2info-1.99/yolox/models/
+-rw-rw-rw-   0        0        0      307 2022-07-13 17:44:25.000000 vid2info-1.99/yolox/models/__init__.py
+-rw-rw-rw-   0        0        0     6207 2022-07-13 17:44:25.000000 vid2info-1.99/yolox/models/darknet.py
+-rw-rw-rw-   0        0        0     2980 2022-07-13 17:44:25.000000 vid2info-1.99/yolox/models/losses.py
+-rw-rw-rw-   0        0        0     6312 2022-07-13 17:44:25.000000 vid2info-1.99/yolox/models/network_blocks.py
+-rw-rw-rw-   0        0        0     2570 2022-07-13 17:44:25.000000 vid2info-1.99/yolox/models/yolo_fpn.py
+-rw-rw-rw-   0        0        0    24776 2022-07-17 14:32:31.000000 vid2info-1.99/yolox/models/yolo_head.py
+-rw-rw-rw-   0        0        0     3656 2022-07-13 17:44:25.000000 vid2info-1.99/yolox/models/yolo_pafpn.py
+-rw-rw-rw-   0        0        0     1422 2022-07-13 17:44:25.000000 vid2info-1.99/yolox/models/yolox.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.982759 vid2info-1.99/yolox/motdt_tracker/
+-rw-rw-rw-   0        0        0        0 2022-07-13 17:52:59.000000 vid2info-1.99/yolox/motdt_tracker/__init__.py
+-rw-rw-rw-   0        0        0     1095 2022-07-13 17:44:25.000000 vid2info-1.99/yolox/motdt_tracker/basetrack.py
+-rw-rw-rw-   0        0        0     9816 2022-07-13 17:44:25.000000 vid2info-1.99/yolox/motdt_tracker/kalman_filter.py
+-rw-rw-rw-   0        0        0     3882 2022-07-13 17:44:25.000000 vid2info-1.99/yolox/motdt_tracker/matching.py
+-rw-rw-rw-   0        0        0    13713 2022-07-13 17:44:25.000000 vid2info-1.99/yolox/motdt_tracker/motdt_tracker.py
+-rw-rw-rw-   0        0        0     8679 2022-08-21 10:28:50.000000 vid2info-1.99/yolox/motdt_tracker/reid_model.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.984687 vid2info-1.99/yolox/sort_tracker/
+-rw-rw-rw-   0        0        0        0 2022-07-13 17:52:59.000000 vid2info-1.99/yolox/sort_tracker/__init__.py
+-rw-rw-rw-   0        0        0     8921 2022-07-13 17:44:25.000000 vid2info-1.99/yolox/sort_tracker/sort.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:45.984687 vid2info-1.99/yolox/tracker/
+-rw-rw-rw-   0        0        0        0 2022-07-13 17:52:59.000000 vid2info-1.99/yolox/tracker/__init__.py
+-rw-rw-rw-   0        0        0     1003 2022-07-13 17:44:25.000000 vid2info-1.99/yolox/tracker/basetrack.py
+-rw-rw-rw-   0        0        0    12633 2022-07-17 14:10:35.000000 vid2info-1.99/yolox/tracker/byte_tracker.py
+-rw-rw-rw-   0        0        0     9816 2022-07-13 17:44:25.000000 vid2info-1.99/yolox/tracker/kalman_filter.py
+-rw-rw-rw-   0        0        0     6380 2022-07-13 17:44:25.000000 vid2info-1.99/yolox/tracker/matching.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:46.003101 vid2info-1.99/yolox/tracking_utils/
+-rw-rw-rw-   0        0        0        0 2022-07-13 17:52:59.000000 vid2info-1.99/yolox/tracking_utils/__init__.py
+-rw-rw-rw-   0        0        0     4162 2022-07-13 17:44:25.000000 vid2info-1.99/yolox/tracking_utils/evaluation.py
+-rw-rw-rw-   0        0        0     3742 2022-07-13 17:44:25.000000 vid2info-1.99/yolox/tracking_utils/io.py
+-rw-rw-rw-   0        0        0      994 2022-07-13 17:44:25.000000 vid2info-1.99/yolox/tracking_utils/timer.py
+drwxrwxrwx   0        0        0        0 2023-02-27 12:29:46.016862 vid2info-1.99/yolox/utils/
+-rw-rw-rw-   0        0        0      466 2022-07-13 17:44:26.000000 vid2info-1.99/yolox/utils/__init__.py
+-rw-rw-rw-   0        0        0     2948 2022-07-13 17:44:26.000000 vid2info-1.99/yolox/utils/allreduce_norm.py
+-rw-rw-rw-   0        0        0     4601 2022-07-13 17:44:26.000000 vid2info-1.99/yolox/utils/boxes.py
+-rw-rw-rw-   0        0        0     1375 2022-07-13 17:44:26.000000 vid2info-1.99/yolox/utils/checkpoint.py
+-rw-rw-rw-   0        0        0     2902 2022-07-13 17:44:26.000000 vid2info-1.99/yolox/utils/demo_utils.py
+-rw-rw-rw-   0        0        0     7321 2022-07-13 17:44:26.000000 vid2info-1.99/yolox/utils/dist.py
+-rw-rw-rw-   0        0        0     2605 2022-07-13 17:44:26.000000 vid2info-1.99/yolox/utils/ema.py
+-rw-rw-rw-   0        0        0     2847 2022-07-13 17:44:26.000000 vid2info-1.99/yolox/utils/logger.py
+-rw-rw-rw-   0        0        0     6766 2022-07-13 17:44:26.000000 vid2info-1.99/yolox/utils/lr_scheduler.py
+-rw-rw-rw-   0        0        0     3217 2022-07-13 17:44:26.000000 vid2info-1.99/yolox/utils/metric.py
+-rw-rw-rw-   0        0        0     3375 2022-07-13 17:44:26.000000 vid2info-1.99/yolox/utils/model_utils.py
+-rw-rw-rw-   0        0        0     1625 2022-07-13 17:44:26.000000 vid2info-1.99/yolox/utils/setup_env.py
+-rw-rw-rw-   0        0        0     5124 2022-07-13 17:44:26.000000 vid2info-1.99/yolox/utils/visualize.py
```

### Comparing `vid2info-1.98/ByteTrack/deploy/ONNXRuntime/onnx_inference.py` & `vid2info-1.99/ByteTrack/deploy/ONNXRuntime/onnx_inference.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/exps/default/nano.py` & `vid2info-1.99/ByteTrack/exps/default/nano.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/exps/default/yolov3.py` & `vid2info-1.99/ByteTrack/exps/default/yolov3.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/exps/default/yolox_tiny.py` & `vid2info-1.99/ByteTrack/exps/default/yolox_tiny.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/exps/example/mot/yolox_l_mix_det.py` & `vid2info-1.99/ByteTrack/exps/example/mot/yolox_l_mix_det.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/exps/example/mot/yolox_m_mix_det.py` & `vid2info-1.99/ByteTrack/exps/example/mot/yolox_m_mix_det.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/exps/example/mot/yolox_nano_mix_det.py` & `vid2info-1.99/ByteTrack/exps/example/mot/yolox_nano_mix_det.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/exps/example/mot/yolox_s_mix_det.py` & `vid2info-1.99/ByteTrack/exps/example/mot/yolox_s_mix_det.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/exps/example/mot/yolox_tiny_mix_det.py` & `vid2info-1.99/ByteTrack/exps/example/mot/yolox_tiny_mix_det.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/exps/example/mot/yolox_x_ablation.py` & `vid2info-1.99/ByteTrack/exps/example/mot/yolox_x_ablation.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/exps/example/mot/yolox_x_ch.py` & `vid2info-1.99/ByteTrack/exps/example/mot/yolox_x_ch.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/exps/example/mot/yolox_x_mix_det.py` & `vid2info-1.99/ByteTrack/exps/example/mot/yolox_x_mix_det.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/exps/example/mot/yolox_x_mix_mot20_ch.py` & `vid2info-1.99/ByteTrack/exps/example/mot/yolox_x_mix_mot20_ch.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/exps/example/mot/yolox_x_mot17_half.py` & `vid2info-1.99/ByteTrack/exps/example/mot/yolox_x_mot17_half.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/setup.py` & `vid2info-1.99/ByteTrack/setup.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/src/cython-bbox/setup.py` & `vid2info-1.99/ByteTrack/src/cython-bbox/setup.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tools/convert_cityperson_to_coco.py` & `vid2info-1.99/ByteTrack/tools/convert_cityperson_to_coco.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tools/convert_crowdhuman_to_coco.py` & `vid2info-1.99/ByteTrack/tools/convert_crowdhuman_to_coco.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tools/convert_ethz_to_coco.py` & `vid2info-1.99/ByteTrack/tools/convert_ethz_to_coco.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tools/convert_mot17_to_coco.py` & `vid2info-1.99/ByteTrack/tools/convert_mot17_to_coco.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tools/convert_mot20_to_coco.py` & `vid2info-1.99/ByteTrack/tools/convert_mot20_to_coco.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tools/convert_video.py` & `vid2info-1.99/ByteTrack/tools/convert_video.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tools/demo_track.py` & `vid2info-1.99/ByteTrack/tools/demo_track.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tools/export_onnx.py` & `vid2info-1.99/ByteTrack/tools/export_onnx.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tools/interpolation.py` & `vid2info-1.99/ByteTrack/tools/interpolation.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tools/mix_data_ablation.py` & `vid2info-1.99/ByteTrack/tools/mix_data_ablation.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tools/mix_data_test_mot17.py` & `vid2info-1.99/ByteTrack/tools/mix_data_test_mot17.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tools/mix_data_test_mot20.py` & `vid2info-1.99/ByteTrack/tools/mix_data_test_mot20.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tools/mota.py` & `vid2info-1.99/ByteTrack/tools/mota.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tools/track.py` & `vid2info-1.99/ByteTrack/tools/track.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tools/track_deepsort.py` & `vid2info-1.99/ByteTrack/tools/track_deepsort.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tools/track_motdt.py` & `vid2info-1.99/ByteTrack/tools/track_motdt.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tools/track_sort.py` & `vid2info-1.99/ByteTrack/tools/track_sort.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tools/train.py` & `vid2info-1.99/ByteTrack/tools/train.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tools/trt.py` & `vid2info-1.99/ByteTrack/tools/trt.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tools/txt2video.py` & `vid2info-1.99/ByteTrack/tools/txt2video.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/centertrack/byte_tracker.py` & `vid2info-1.99/ByteTrack/tutorials/centertrack/byte_tracker.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/centertrack/mot_online/basetrack.py` & `vid2info-1.99/ByteTrack/tutorials/centertrack/mot_online/basetrack.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/centertrack/mot_online/kalman_filter.py` & `vid2info-1.99/ByteTrack/tutorials/centertrack/mot_online/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/centertrack/mot_online/matching.py` & `vid2info-1.99/ByteTrack/tutorials/centertrack/mot_online/matching.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/centertrack/opts.py` & `vid2info-1.99/ByteTrack/tutorials/centertrack/opts.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/centertrack/tracker.py` & `vid2info-1.99/ByteTrack/tutorials/centertrack/tracker.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/cstrack/byte_tracker.py` & `vid2info-1.99/ByteTrack/tutorials/cstrack/byte_tracker.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/cstrack/tracker.py` & `vid2info-1.99/ByteTrack/tutorials/cstrack/tracker.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/ctracker/byte_tracker.py` & `vid2info-1.99/ByteTrack/tutorials/ctracker/byte_tracker.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/ctracker/eval_motchallenge.py` & `vid2info-1.99/ByteTrack/tutorials/ctracker/eval_motchallenge.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/ctracker/generate_half_csv.py` & `vid2info-1.99/ByteTrack/tutorials/ctracker/generate_half_csv.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/ctracker/mot_online/basetrack.py` & `vid2info-1.99/ByteTrack/tutorials/ctracker/mot_online/basetrack.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/ctracker/mot_online/kalman_filter.py` & `vid2info-1.99/ByteTrack/tutorials/ctracker/mot_online/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/ctracker/mot_online/matching.py` & `vid2info-1.99/ByteTrack/tutorials/ctracker/mot_online/matching.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/ctracker/test.py` & `vid2info-1.99/ByteTrack/tutorials/ctracker/test.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/ctracker/test_byte.py` & `vid2info-1.99/ByteTrack/tutorials/ctracker/test_byte.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/fairmot/byte_tracker.py` & `vid2info-1.99/ByteTrack/tutorials/fairmot/byte_tracker.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/fairmot/tracker.py` & `vid2info-1.99/ByteTrack/tutorials/fairmot/tracker.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/jde/byte_tracker.py` & `vid2info-1.99/ByteTrack/tutorials/jde/byte_tracker.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/jde/evaluation.py` & `vid2info-1.99/ByteTrack/tutorials/jde/evaluation.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/jde/track_half.py` & `vid2info-1.99/ByteTrack/tutorials/jde/track_half.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/jde/tracker.py` & `vid2info-1.99/ByteTrack/tutorials/jde/tracker.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/motr/byte_tracker.py` & `vid2info-1.99/ByteTrack/tutorials/motr/byte_tracker.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/motr/eval.py` & `vid2info-1.99/ByteTrack/tutorials/motr/eval.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/motr/evaluation.py` & `vid2info-1.99/ByteTrack/tutorials/motr/evaluation.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/motr/joint.py` & `vid2info-1.99/ByteTrack/tutorials/motr/joint.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/motr/mot_online/basetrack.py` & `vid2info-1.99/ByteTrack/tutorials/motr/mot_online/basetrack.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/motr/mot_online/kalman_filter.py` & `vid2info-1.99/ByteTrack/tutorials/motr/mot_online/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/motr/mot_online/matching.py` & `vid2info-1.99/ByteTrack/tutorials/motr/mot_online/matching.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/motr/motr.py` & `vid2info-1.99/ByteTrack/tutorials/motr/motr.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/motr/motr_det.py` & `vid2info-1.99/ByteTrack/tutorials/motr/motr_det.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/motr/transforms.py` & `vid2info-1.99/ByteTrack/tutorials/motr/transforms.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/qdtrack/byte_tracker.py` & `vid2info-1.99/ByteTrack/tutorials/qdtrack/byte_tracker.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/qdtrack/mot_online/basetrack.py` & `vid2info-1.99/ByteTrack/tutorials/qdtrack/mot_online/basetrack.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/qdtrack/mot_online/kalman_filter.py` & `vid2info-1.99/ByteTrack/tutorials/qdtrack/mot_online/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/qdtrack/mot_online/matching.py` & `vid2info-1.99/ByteTrack/tutorials/qdtrack/mot_online/matching.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/qdtrack/qdtrack.py` & `vid2info-1.99/ByteTrack/tutorials/qdtrack/qdtrack.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/qdtrack/tracker_reid_motion.py` & `vid2info-1.99/ByteTrack/tutorials/qdtrack/tracker_reid_motion.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/trades/byte_tracker.py` & `vid2info-1.99/ByteTrack/tutorials/trades/byte_tracker.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/trades/mot_online/basetrack.py` & `vid2info-1.99/ByteTrack/tutorials/trades/mot_online/basetrack.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/trades/mot_online/kalman_filter.py` & `vid2info-1.99/ByteTrack/tutorials/trades/mot_online/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/trades/mot_online/matching.py` & `vid2info-1.99/ByteTrack/tutorials/trades/mot_online/matching.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/trades/opts.py` & `vid2info-1.99/ByteTrack/tutorials/trades/opts.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/trades/tracker.py` & `vid2info-1.99/ByteTrack/tutorials/trades/tracker.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/transtrack/engine_track.py` & `vid2info-1.99/ByteTrack/tutorials/transtrack/engine_track.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/transtrack/main_track.py` & `vid2info-1.99/ByteTrack/tutorials/transtrack/main_track.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/transtrack/mot_online/basetrack.py` & `vid2info-1.99/ByteTrack/tutorials/transtrack/mot_online/basetrack.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/transtrack/mot_online/byte_tracker.py` & `vid2info-1.99/ByteTrack/tutorials/transtrack/mot_online/byte_tracker.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/transtrack/mot_online/kalman_filter.py` & `vid2info-1.99/ByteTrack/tutorials/transtrack/mot_online/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/transtrack/mot_online/matching.py` & `vid2info-1.99/ByteTrack/tutorials/transtrack/mot_online/matching.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/transtrack/save_track.py` & `vid2info-1.99/ByteTrack/tutorials/transtrack/save_track.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/ByteTrack/tutorials/transtrack/tracker.py` & `vid2info-1.99/ByteTrack/tutorials/transtrack/tracker.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/LICENSE` & `vid2info-1.99/LICENSE`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/PKG-INFO` & `vid2info-1.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vid2info
-Version: 1.98
+Version: 1.99
 Summary: Vid2Info is an easy-to-use Computer Vision pipeline that implements Detection, Tracking and, optionally, Segmentation.
 Home-page: https://github.com/Eric-Canas/vid2info
 Author: Eric Canas
 Author-email: elcorreodeharu@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `vid2info-1.98/models/common.py` & `vid2info-1.99/models/common.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/models/experimental.py` & `vid2info-1.99/models/experimental.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/models/yolo.py` & `vid2info-1.99/models/yolo.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/setup.py` & `vid2info-1.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name='vid2info',
-    version='1.98',
+    version='1.99',
     packages=find_namespace_packages(),
     package_dir={'vid2info': 'vid2info'},
     url='https://github.com/Eric-Canas/vid2info',
     license='MIT',
     author='Eric Canas',
     author_email='elcorreodeharu@gmail.com',
     description='Vid2Info is an easy-to-use Computer Vision pipeline that implements Detection, Tracking and, '
```

### Comparing `vid2info-1.98/third_party/pidnet/model_utils.py` & `vid2info-1.99/third_party/pidnet/model_utils.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/third_party/pidnet/pidnet.py` & `vid2info-1.99/third_party/pidnet/pidnet.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/training_tools/dataset_generation/video_extractor.py` & `vid2info-1.99/training_tools/dataset_generation/video_extractor.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/utils/activations.py` & `vid2info-1.99/utils/activations.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/utils/add_nms.py` & `vid2info-1.99/utils/add_nms.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/utils/autoanchor.py` & `vid2info-1.99/utils/autoanchor.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/utils/datasets.py` & `vid2info-1.99/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/utils/general.py` & `vid2info-1.99/utils/general.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/utils/google_utils.py` & `vid2info-1.99/utils/google_utils.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/utils/loss.py` & `vid2info-1.99/utils/loss.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/utils/metrics.py` & `vid2info-1.99/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/utils/plots.py` & `vid2info-1.99/utils/plots.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/utils/torch_utils.py` & `vid2info-1.99/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/vid2info/inference/config.py` & `vid2info-1.99/vid2info/inference/config.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/vid2info/inference/detection/__yolo_detector.py` & `vid2info-1.99/vid2info/inference/detection/__yolo_detector.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/vid2info/inference/detection/config.py` & `vid2info-1.99/vid2info/inference/detection/config.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/vid2info/inference/detection/yolov6_detector.py` & `vid2info-1.99/vid2info/inference/detection/yolov6_detector.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/vid2info/inference/detection/yolov7_detector.py` & `vid2info-1.99/vid2info/inference/detection/yolov7_detector.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/vid2info/inference/models/finite_state_machine_configs/dummy_finite_state_config.py` & `vid2info-1.99/vid2info/inference/models/finite_state_machine_configs/dummy_finite_state_config.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/vid2info/inference/pipeline.py` & `vid2info-1.99/vid2info/inference/pipeline.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/vid2info/inference/pipeline_background.py` & `vid2info-1.99/vid2info/inference/pipeline_background.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/vid2info/inference/segmentation/pidnet_segmenter.py` & `vid2info-1.99/vid2info/inference/segmentation/pidnet_segmenter.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/vid2info/inference/tracking/tracker.py` & `vid2info-1.99/vid2info/inference/tracking/tracker.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/vid2info/inference/utils.py` & `vid2info-1.99/vid2info/inference/utils.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/vid2info/state/config.py` & `vid2info-1.99/vid2info/state/config.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/vid2info/state/element_state/element_movement.py` & `vid2info-1.99/vid2info/state/element_state/element_movement.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from __future__ import annotations
 
 from collections import deque
 import itertools
 import numpy as np
 
-from state.element_state.constants import STD_OUTLIER_DEVIATION, MIN_POINTS_TO_CALCULATE_OUTLIERS, \
+from vid2info.state.element_state.constants import STD_OUTLIER_DEVIATION, MIN_POINTS_TO_CALCULATE_OUTLIERS, \
     TOP, RIGHT, BOTTOM, LEFT
 
 
 class ElementMovement:
     def __init__(self, element_state: 'ElementState', element_buffer: deque):
         """
         Initialize the ElementMovement calculator.
```

### Comparing `vid2info-1.98/vid2info/state/element_state/element_state.py` & `vid2info-1.99/vid2info/state/element_state/element_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Github: https://github.com/Eric-Canas
 Email: eric@ericcanas.com
 Date: 17-07-2022
 """
 from __future__ import annotations
 from collections import deque
 
-from state.element_state.element_movement import ElementMovement
+from vid2info.state.element_state.element_movement import ElementMovement
 from vid2info.state.finite_state_machine.element_finite_state_machine import ElementFiniteStateMachine
 from vid2info.inference.config import CONFIDENCE, CLASS_ID, CLASS_NAME, BBOX_XYXY, SEGMENTATION_MASK, CLASS_NAMES_LIST, \
     BACKGROUND_CLASS_IDX
 from vid2info.inference.tracking.tracker import TRACK_LENGTH
 
 from time import time
 import numpy as np
```

### Comparing `vid2info-1.98/vid2info/state/finite_state_machine/element_finite_state_machine.py` & `vid2info-1.99/vid2info/state/finite_state_machine/element_finite_state_machine.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/vid2info/state/finite_state_machine/track_recoverer.py` & `vid2info-1.99/vid2info/state/finite_state_machine/track_recoverer.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/vid2info/state/scene_state.py` & `vid2info-1.99/vid2info/state/scene_state.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/vid2info/state/state_buffer.py` & `vid2info-1.99/vid2info/state/state_buffer.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/vid2info/utils/general.py` & `vid2info-1.99/vid2info/utils/general.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/vid2info/utils/user_interaction.py` & `vid2info-1.99/vid2info/utils/user_interaction.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/vid2info/video/_video_reader_multithread.py` & `vid2info-1.99/vid2info/video/_video_reader_multithread.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/vid2info/video/_webcam_reader_multithread.py` & `vid2info-1.99/vid2info/video/_webcam_reader_multithread.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/vid2info/video/utils.py` & `vid2info-1.99/vid2info/video/utils.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/vid2info/video/video_reader.py` & `vid2info-1.99/vid2info/video/video_reader.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/vid2info/video/webcam_reader.py` & `vid2info-1.99/vid2info/video/webcam_reader.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/vid2info/visualization/config.py` & `vid2info-1.99/vid2info/visualization/config.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/vid2info/visualization/general_utils.py` & `vid2info-1.99/vid2info/visualization/general_utils.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/vid2info/visualization/overlay_utils.py` & `vid2info-1.99/vid2info/visualization/overlay_utils.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/vid2info/visualization/stream_visualization.py` & `vid2info-1.99/vid2info/visualization/stream_visualization.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/vid2info.egg-info/PKG-INFO` & `vid2info-1.99/vid2info.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vid2info
-Version: 1.98
+Version: 1.99
 Summary: Vid2Info is an easy-to-use Computer Vision pipeline that implements Detection, Tracking and, optionally, Segmentation.
 Home-page: https://github.com/Eric-Canas/vid2info
 Author: Eric Canas
 Author-email: elcorreodeharu@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `vid2info-1.98/vid2info.egg-info/SOURCES.txt` & `vid2info-1.99/vid2info.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolov6/core/engine.py` & `vid2info-1.99/yolov6/core/engine.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolov6/core/evaler.py` & `vid2info-1.99/yolov6/core/evaler.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolov6/core/inferer.py` & `vid2info-1.99/yolov6/core/inferer.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolov6/data/data_augment.py` & `vid2info-1.99/yolov6/data/data_augment.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolov6/data/data_load.py` & `vid2info-1.99/yolov6/data/data_load.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolov6/data/datasets.py` & `vid2info-1.99/yolov6/data/datasets.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolov6/data/vis_dataset.py` & `vid2info-1.99/yolov6/data/vis_dataset.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolov6/data/voc2yolo.py` & `vid2info-1.99/yolov6/data/voc2yolo.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolov6/layers/common.py` & `vid2info-1.99/yolov6/layers/common.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolov6/layers/dbb_transforms.py` & `vid2info-1.99/yolov6/layers/dbb_transforms.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolov6/models/efficientrep.py` & `vid2info-1.99/yolov6/models/efficientrep.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolov6/models/effidehead.py` & `vid2info-1.99/yolov6/models/effidehead.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolov6/models/end2end.py` & `vid2info-1.99/yolov6/models/end2end.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolov6/models/loss.py` & `vid2info-1.99/yolov6/models/loss.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolov6/models/reppan.py` & `vid2info-1.99/yolov6/models/reppan.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolov6/models/yolo.py` & `vid2info-1.99/yolov6/models/yolo.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolov6/solver/build.py` & `vid2info-1.99/yolov6/solver/build.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolov6/utils/checkpoint.py` & `vid2info-1.99/yolov6/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolov6/utils/config.py` & `vid2info-1.99/yolov6/utils/config.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolov6/utils/ema.py` & `vid2info-1.99/yolov6/utils/ema.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolov6/utils/envs.py` & `vid2info-1.99/yolov6/utils/envs.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolov6/utils/events.py` & `vid2info-1.99/yolov6/utils/events.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolov6/utils/figure_iou.py` & `vid2info-1.99/yolov6/utils/figure_iou.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolov6/utils/general.py` & `vid2info-1.99/yolov6/utils/general.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolov6/utils/nms.py` & `vid2info-1.99/yolov6/utils/nms.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolov6/utils/torch_utils.py` & `vid2info-1.99/yolov6/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolov7/models/common.py` & `vid2info-1.99/yolov7/models/common.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolov7/models/experimental.py` & `vid2info-1.99/yolov7/models/experimental.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolov7/models/yolo.py` & `vid2info-1.99/yolov7/models/yolo.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolov7/utils/activations.py` & `vid2info-1.99/yolov7/utils/activations.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolov7/utils/add_nms.py` & `vid2info-1.99/yolov7/utils/add_nms.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolov7/utils/autoanchor.py` & `vid2info-1.99/yolov7/utils/autoanchor.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolov7/utils/datasets.py` & `vid2info-1.99/yolov7/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolov7/utils/general.py` & `vid2info-1.99/yolov7/utils/general.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolov7/utils/google_utils.py` & `vid2info-1.99/yolov7/utils/google_utils.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolov7/utils/loss.py` & `vid2info-1.99/yolov7/utils/loss.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolov7/utils/metrics.py` & `vid2info-1.99/yolov7/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolov7/utils/plots.py` & `vid2info-1.99/yolov7/utils/plots.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolov7/utils/torch_utils.py` & `vid2info-1.99/yolov7/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/core/launch.py` & `vid2info-1.99/yolox/core/launch.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/core/trainer.py` & `vid2info-1.99/yolox/core/trainer.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/data/data_augment.py` & `vid2info-1.99/yolox/data/data_augment.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/data/data_prefetcher.py` & `vid2info-1.99/yolox/data/data_prefetcher.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/data/dataloading.py` & `vid2info-1.99/yolox/data/dataloading.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/data/datasets/datasets_wrapper.py` & `vid2info-1.99/yolox/data/datasets/datasets_wrapper.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/data/datasets/mosaicdetection.py` & `vid2info-1.99/yolox/data/datasets/mosaicdetection.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/data/datasets/mot.py` & `vid2info-1.99/yolox/data/datasets/mot.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/data/samplers.py` & `vid2info-1.99/yolox/data/samplers.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/deepsort_tracker/deepsort.py` & `vid2info-1.99/yolox/deepsort_tracker/deepsort.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/deepsort_tracker/detection.py` & `vid2info-1.99/yolox/deepsort_tracker/detection.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/deepsort_tracker/iou_matching.py` & `vid2info-1.99/yolox/deepsort_tracker/iou_matching.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/deepsort_tracker/kalman_filter.py` & `vid2info-1.99/yolox/deepsort_tracker/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/deepsort_tracker/linear_assignment.py` & `vid2info-1.99/yolox/deepsort_tracker/linear_assignment.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/deepsort_tracker/reid_model.py` & `vid2info-1.99/yolox/deepsort_tracker/reid_model.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/deepsort_tracker/track.py` & `vid2info-1.99/yolox/deepsort_tracker/track.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/evaluators/coco_evaluator.py` & `vid2info-1.99/yolox/evaluators/coco_evaluator.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/evaluators/evaluation.py` & `vid2info-1.99/yolox/evaluators/evaluation.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/evaluators/mot_evaluator.py` & `vid2info-1.99/yolox/evaluators/mot_evaluator.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/exp/base_exp.py` & `vid2info-1.99/yolox/exp/base_exp.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/exp/build.py` & `vid2info-1.99/yolox/exp/build.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/exp/yolox_base.py` & `vid2info-1.99/yolox/exp/yolox_base.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/layers/fast_coco_eval_api.py` & `vid2info-1.99/yolox/layers/fast_coco_eval_api.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/models/darknet.py` & `vid2info-1.99/yolox/models/darknet.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/models/losses.py` & `vid2info-1.99/yolox/models/losses.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/models/network_blocks.py` & `vid2info-1.99/yolox/models/network_blocks.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/models/yolo_fpn.py` & `vid2info-1.99/yolox/models/yolo_fpn.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/models/yolo_head.py` & `vid2info-1.99/yolox/models/yolo_head.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/models/yolo_pafpn.py` & `vid2info-1.99/yolox/models/yolo_pafpn.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/models/yolox.py` & `vid2info-1.99/yolox/models/yolox.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/motdt_tracker/basetrack.py` & `vid2info-1.99/yolox/motdt_tracker/basetrack.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/motdt_tracker/kalman_filter.py` & `vid2info-1.99/yolox/motdt_tracker/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/motdt_tracker/matching.py` & `vid2info-1.99/yolox/motdt_tracker/matching.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/motdt_tracker/motdt_tracker.py` & `vid2info-1.99/yolox/motdt_tracker/motdt_tracker.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/motdt_tracker/reid_model.py` & `vid2info-1.99/yolox/motdt_tracker/reid_model.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/sort_tracker/sort.py` & `vid2info-1.99/yolox/sort_tracker/sort.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/tracker/basetrack.py` & `vid2info-1.99/yolox/tracker/basetrack.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/tracker/byte_tracker.py` & `vid2info-1.99/yolox/tracker/byte_tracker.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/tracker/kalman_filter.py` & `vid2info-1.99/yolox/tracker/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/tracker/matching.py` & `vid2info-1.99/yolox/tracker/matching.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/tracking_utils/evaluation.py` & `vid2info-1.99/yolox/tracking_utils/evaluation.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/tracking_utils/io.py` & `vid2info-1.99/yolox/tracking_utils/io.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/tracking_utils/timer.py` & `vid2info-1.99/yolox/tracking_utils/timer.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/utils/allreduce_norm.py` & `vid2info-1.99/yolox/utils/allreduce_norm.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/utils/boxes.py` & `vid2info-1.99/yolox/utils/boxes.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/utils/checkpoint.py` & `vid2info-1.99/yolox/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/utils/demo_utils.py` & `vid2info-1.99/yolox/utils/demo_utils.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/utils/dist.py` & `vid2info-1.99/yolox/utils/dist.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/utils/ema.py` & `vid2info-1.99/yolox/utils/ema.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/utils/logger.py` & `vid2info-1.99/yolox/utils/logger.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/utils/lr_scheduler.py` & `vid2info-1.99/yolox/utils/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/utils/metric.py` & `vid2info-1.99/yolox/utils/metric.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/utils/model_utils.py` & `vid2info-1.99/yolox/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/utils/setup_env.py` & `vid2info-1.99/yolox/utils/setup_env.py`

 * *Files identical despite different names*

### Comparing `vid2info-1.98/yolox/utils/visualize.py` & `vid2info-1.99/yolox/utils/visualize.py`

 * *Files identical despite different names*

