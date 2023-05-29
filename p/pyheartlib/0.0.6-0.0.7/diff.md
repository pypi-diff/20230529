# Comparing `tmp/pyheartlib-0.0.6.tar.gz` & `tmp/pyheartlib-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyheartlib-0.0.6.tar", max compression
+gzip compressed data, was "pyheartlib-0.0.7.tar", max compression
```

## Comparing `pyheartlib-0.0.6.tar` & `pyheartlib-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       59 2023-05-25 08:38:53.575999 pyheartlib-0.0.6/LICENSE
--rw-r--r--   0        0        0     2438 2023-05-25 08:38:53.575999 pyheartlib-0.0.6/README.md
--rw-r--r--   0        0        0     1412 2023-05-25 08:40:33.947862 pyheartlib-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      112 2023-05-25 08:38:53.583999 pyheartlib-0.0.6/src/pyheartlib/__init__.py
--rw-r--r--   0        0        0       54 2023-05-25 08:38:53.583999 pyheartlib-0.0.6/src/pyheartlib/archs/__init__.py
--rw-r--r--   0        0        0    18725 2023-05-25 08:38:53.583999 pyheartlib-0.0.6/src/pyheartlib/beat_info.py
--rw-r--r--   0        0        0     1160 2023-05-25 08:38:53.583999 pyheartlib-0.0.6/src/pyheartlib/config.yaml
--rw-r--r--   0        0        0     5349 2023-05-25 08:38:53.583999 pyheartlib-0.0.6/src/pyheartlib/data.py
--rw-r--r--   0        0        0     9295 2023-05-25 08:38:53.583999 pyheartlib-0.0.6/src/pyheartlib/data_arrhythmia.py
--rw-r--r--   0        0        0    22880 2023-05-25 08:38:53.583999 pyheartlib-0.0.6/src/pyheartlib/data_beat.py
--rw-r--r--   0        0        0     9605 2023-05-25 08:38:53.583999 pyheartlib-0.0.6/src/pyheartlib/data_rpeak.py
--rw-r--r--   0        0        0       39 2023-05-25 08:38:53.583999 pyheartlib-0.0.6/src/pyheartlib/extra/__init__.py
--rw-r--r--   0        0        0     4176 2023-05-25 08:38:53.583999 pyheartlib-0.0.6/src/pyheartlib/extra/pqrst.py
--rw-r--r--   0        0        0     2827 2023-05-25 08:38:53.583999 pyheartlib-0.0.6/src/pyheartlib/extra/report.py
--rw-r--r--   0        0        0     5887 2023-05-25 08:38:53.583999 pyheartlib-0.0.6/src/pyheartlib/extra/utils.py
--rw-r--r--   0        0        0     5866 2023-05-25 08:38:53.583999 pyheartlib-0.0.6/src/pyheartlib/features.py
--rw-r--r--   0        0        0     2579 2023-05-25 08:38:53.583999 pyheartlib-0.0.6/src/pyheartlib/io.py
--rw-r--r--   0        0        0     8796 2023-05-25 08:38:53.583999 pyheartlib-0.0.6/src/pyheartlib/processing.py
--rw-r--r--   0        0        0     3088 1970-01-01 00:00:00.000000 pyheartlib-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       59 2023-05-29 09:26:57.636241 pyheartlib-0.0.7/LICENSE
+-rw-r--r--   0        0        0     2438 2023-05-29 09:26:57.636241 pyheartlib-0.0.7/README.md
+-rw-r--r--   0        0        0     1429 2023-05-29 09:28:47.204727 pyheartlib-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      112 2023-05-29 09:26:57.644241 pyheartlib-0.0.7/src/pyheartlib/__init__.py
+-rw-r--r--   0        0        0       54 2023-05-29 09:26:57.644241 pyheartlib-0.0.7/src/pyheartlib/archs/__init__.py
+-rw-r--r--   0        0        0    17957 2023-05-29 09:26:57.644241 pyheartlib-0.0.7/src/pyheartlib/beat_info.py
+-rw-r--r--   0        0        0     1160 2023-05-29 09:26:57.644241 pyheartlib-0.0.7/src/pyheartlib/config.yaml
+-rw-r--r--   0        0        0     5429 2023-05-29 09:26:57.644241 pyheartlib-0.0.7/src/pyheartlib/data.py
+-rw-r--r--   0        0        0     9295 2023-05-29 09:26:57.644241 pyheartlib-0.0.7/src/pyheartlib/data_arrhythmia.py
+-rw-r--r--   0        0        0    23957 2023-05-29 09:26:57.644241 pyheartlib-0.0.7/src/pyheartlib/data_beat.py
+-rw-r--r--   0        0        0     9605 2023-05-29 09:26:57.644241 pyheartlib-0.0.7/src/pyheartlib/data_rpeak.py
+-rw-r--r--   0        0        0       39 2023-05-29 09:26:57.644241 pyheartlib-0.0.7/src/pyheartlib/extra/__init__.py
+-rw-r--r--   0        0        0     4176 2023-05-29 09:26:57.644241 pyheartlib-0.0.7/src/pyheartlib/extra/pqrst.py
+-rw-r--r--   0        0        0     2827 2023-05-29 09:26:57.644241 pyheartlib-0.0.7/src/pyheartlib/extra/report.py
+-rw-r--r--   0        0        0     5887 2023-05-29 09:26:57.644241 pyheartlib-0.0.7/src/pyheartlib/extra/utils.py
+-rw-r--r--   0        0        0     6150 2023-05-29 09:26:57.644241 pyheartlib-0.0.7/src/pyheartlib/features.py
+-rw-r--r--   0        0        0     2579 2023-05-29 09:26:57.644241 pyheartlib-0.0.7/src/pyheartlib/io.py
+-rw-r--r--   0        0        0     5773 2023-05-29 09:26:57.644241 pyheartlib-0.0.7/src/pyheartlib/processing.py
+-rw-r--r--   0        0        0     3118 1970-01-01 00:00:00.000000 pyheartlib-0.0.7/PKG-INFO
```

### Comparing `pyheartlib-0.0.6/README.md` & `pyheartlib-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pyheartlib-0.0.6/pyproject.toml` & `pyheartlib-0.0.7/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "pyheartlib"
-version = "0.0.6"
+version = "0.0.7"
 description = "A Python package for processing and modeling electrocardiogram signals"
 authors = ["Sadegh Mohammadi"]
 license = "Proprietary"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 numpy = ">=1.22.0"
 wfdb = ">=4.0.0"
 pandas = ">=1.4.0"
 tqdm = ">=4.63.0"
 scikit-learn = ">=1.1.0"
 tensorflow = ">=2.8.0"
+pyyaml = ">=6.0"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 pytest-cov = "^4.1.0"
 black = "^23.3.0"
```

### Comparing `pyheartlib-0.0.6/src/pyheartlib/beat_info.py` & `pyheartlib-0.0.7/src/pyheartlib/beat_info.py`

 * *Files 18% similar despite different names*

```diff
@@ -142,14 +142,15 @@
             # if the feature function returns multiple values as a dict
             elif isinstance(ret, dict):
                 feature_dict.update(ret)
         return feature_dict
 
     def get_beat_waveform(self, win=[-0.35, 0.65]):
         """Segment beat waveform according to the pre and post RR intervals."""
+
         try:
             beat_rpeak_idx = self.rpeaks[self.beat_loc]
             prerri = self.rri_smpl[self.beat_loc - 1]
             postrri = self.rri_smpl[self.beat_loc]
             beat_onset_org = int(beat_rpeak_idx + win[0] * prerri)
             beat_offset_org = int(beat_rpeak_idx + win[1] * postrri)
 
@@ -228,159 +229,160 @@
         sdrri = list(np.diff(np.asarray(self.rri)))
         return sdrri
 
     # ============================================================
     # RRI features
     # ============================================================
     def F_post_rri(self):
+        """Post RR interval."""
         return self.rri[self.beat_loc]
 
     def F_pre_rri(self):
+        """Pre RR interval."""
         return self.rri[self.beat_loc - 1]
 
     def F_ratio_post_pre(self):
+        """Ratio of post and pre RR intervals."""
         post = self.F_post_rri()
         pre = self.F_pre_rri()
         return post / pre
 
     def F_diff_post_pre(self):
+        """Difference of post and pre RR intervals."""
         post = self.F_post_rri()
         pre = self.F_pre_rri()
         return post - pre
 
     def F_diff_post_pre_nr(self):
+        """Normalized difference of post and pre RR intervals."""
         post = self.F_post_rri()
         pre = self.F_pre_rri()
         return (post - pre) / self.F_rms_rri()
 
     def F_median_rri(self):
-        # median of rri
+        """Median of RR intervals."""
         return np.median(self.rri)
 
     def F_mean_pre_rri(self):
-        # average of pre-rri
+        """Mean of pre RR intervals."""
         pre_rri = self.rri[: self.beat_loc]
         return np.mean(pre_rri)
 
     def F_rms_rri(self):
-        # rms of rri
+        """RMS of RR intervals."""
         rri = np.asarray(self.rri)
         rms = np.sqrt(np.mean(rri**2))
         return rms
 
     def F_std_rri(self):
-        # std of RR intervals
+        """STD of RR intervals."""
         return np.std(self.rri)
 
     def F_ratio_pre_rms(self):
-        # ratio of pre-rr interval to rms
+        """Ratio of pre RR interval to RMS of RR intervals."""
         return self.F_pre_rri() / self.F_rms_rri()
 
     def F_ratio_post_rms(self):
-        # ratio of post-rr interval to rms
+        """Ratio of post RR interval to RMS of RR intervals."""
         return self.F_post_rri() / self.F_rms_rri()
 
     def F_diff_pre_avg_nr(self):
-        # diff of pre-rr interval to local rr average
+        """Difference of pre RR interval and median of RR intervals, normalized by their RMS."""
         return (self.F_pre_rri() - self.F_median_rri()) / self.F_rms_rri()
 
     def F_diff_post_avg_nr(self):
-        # diff of post-rr interval to local rr average
+        """Difference of post RR interval and median of RR intervals, normalized by their RMS."""
         return (self.F_post_rri() - self.F_median_rri()) / self.F_rms_rri()
 
     def F_compensate_ratio(self):
+        """Compensation ratio."""
         postpre = self.F_post_rri() + self.F_pre_rri()
         _2t2ndpre = 2 * self.rri[self.beat_loc - 2]  # 2 times second pre rri
         return postpre / _2t2ndpre
 
     def F_compensate_diff_nr(self):
+        """Compensation diff normalized by RMS."""
         postpre = self.F_post_rri() + self.F_pre_rri()
         _2t2ndpre = 2 * self.rri[self.beat_loc - 2]  # 2 times second pre rri
         return (postpre - _2t2ndpre) / self.F_rms_rri()
 
     def F_heart_rate(self):
+        """Heart rate."""
         pre_rri = (
             self.rpeaks[self.beat_loc] - self.rpeaks[self.beat_loc - 1]
         ) / self.fs
         hr = 60 / pre_rri
         return hr
 
     # ============================================================
     # SDRRI features
     # ============================================================
-    def F_post_sdrri(self):
-        try:
-            return self.sdrri[self.beat_loc]
-        except:
-            return None
-
-    def F_onbeat_sdrri(self):
-        # on beat(postrri-prerri)
-        return self.sdrri[self.beat_loc - 1]
-
-    def F_pre_sdrri(self):
-        # pre beat
-        return self.sdrri[self.beat_loc - 2]
-
     def F_mean_sdrri(self):
-        # average of sdrri
+        """Mean of successive RRI differences."""
         return np.mean(self.sdrri)
 
     def F_absmean_sdrri(self):
-        # abs average of sdrri
+        """Mean of absolute successive RRI differences."""
         return np.mean(np.abs(self.sdrri))
 
     def F_mean_pre_sdrri(self):
-        # average of pre-rri
+        """Mean of pre successive RRI differences."""
         pre_sdrri = self.sdrri[: self.beat_loc - 1]
         return np.mean(pre_sdrri)
 
     def F_rms_sdrri(self):
-        # rms of rri
+        """RMS of successive RRI differences."""
         sdrri = np.asarray(self.sdrri)
-        rms = np.sqrt(np.mean(sdrri**2))
-        return rms
+        return np.sqrt(np.mean(sdrri**2))
 
     def F_std_sdrri(self):
-        # std of sdrri
+        """STD of successive RRI differences."""
         return np.std(self.sdrri)
 
     # ============================================================
     # Waveform features
     # ============================================================
     def reported_rpeak(self):
         return self.rpeaks[self.beat_loc] - self.wfpts["beat_onset_org"]
 
     def F_beat_max(self):
+        """Max value of heartbeat waveform."""
         return max(self.bwaveform)
 
     def F_beat_min(self):
+        """Min value of heartbeat waveform."""
         return min(self.bwaveform)
 
     def F_maxmin_diff(self):
+        """Difference of max and min values of heartbeat waveform."""
         return self.F_beat_max() - self.F_beat_min()
 
     def F_maxmin_diff_norm(self):
+        """Difference of max and min values of heartbeat waveform normalized by waveform RMS"""
         return self.F_maxmin_diff() / self.F_beat_rms()
 
     def F_beat_mean(self):
+        """Mean of heartbeat waveform."""
         return np.mean(self.bwaveform)
 
     def F_beat_std(self):
+        """STD of heartbeat waveform."""
         return np.std(self.bwaveform)
 
     def F_beat_skewness(self):
+        """Skewness of heartbeat waveform."""
         return stats.skew(self.bwaveform)
 
     def F_beat_kurtosis(self):
+        """Kurtosis of heartbeat waveform."""
         return stats.kurtosis(self.bwaveform)
 
     def F_beat_rms(self):
-        rms = np.sqrt(np.mean(self.bwaveform**2))
-        return rms
+        """RMS of heartbeat waveform."""
+        return np.sqrt(np.mean(self.bwaveform**2))
 
     def pqrst(self):
         # 120ms <Normal_PR< 220ms.
         # 75ms  <Normal_QRS< 120ms
         # QRS region estimate 160ms.
         # Compute: QRS width,Q,R,S amplitudes.
 
@@ -390,65 +392,14 @@
         q = beat_pqrst.qwave
         r = beat_pqrst.rwave
         s = beat_pqrst.swave
         pr = beat_pqrst.pr_interval
         qs = beat_pqrst.qs_interval
         return {"p": p, "q": q, "r": r, "s": s, "pr": pr, "qs": qs}
 
-    def pqrst_segs(self):
-        # splits the beat waveform into 3-segments using q and s points in the middle
-        pqrst = self.pqrst_dict
-        points = [0, pqrst["q"][0], pqrst["s"][0], len(self.bwaveform)]
-
-        lmax = []
-        lmin = []
-        lmean = []
-        lmedian = []
-        std = []
-        lskewness = []
-        lkurtosis = []
-        lrms = []
-
-        try:
-            for i in range(3):
-                s_ix = int(points[i])
-                e_ix = int(points[i + 1])
-                seg = self.bwaveform[s_ix:e_ix]
-                lmax.append(max(seg))
-                lmin.append(min(seg))
-                lmean.append(np.mean(seg))
-                lmedian.append(np.median(seg))
-                std.append(np.std(seg))
-                lskewness.append(stats.skew(seg))
-                lkurtosis.append(stats.kurtosis(seg))
-                lrms.append(np.sqrt(np.mean(seg**2)))
-
-            res = [lmax, lmin, lmean, lmedian, std, lskewness, lkurtosis, lrms]
-
-            # agg results
-            mean_res = []
-            std_res = []
-            rms_res = []
-            for mtrc in res:
-                mtrc = np.asarray(mtrc)
-                mean_res.append(np.mean(mtrc))
-                std_res.append(np.std(mtrc))
-                rms_res.append(np.sqrt(np.mean(mtrc**2)))
-
-            aggs = [mean_res, std_res, rms_res]
-            return res, aggs
-        except ValueError:
-            # print('pqrst segs error!')
-            # print('rec_id={}, sindex={}'.format(
-            # 					self.data['rec_id'],
-            # 					self.data['start_idx']))
-            res = [[np.nan] * 3] * 8
-            aggs = [[np.nan] * 8] * 3
-            return res, aggs
-
     def pr_interval(self):
         # pr interval in ms
         pr = self.pqrst_dict["pr"]
         return pr
 
     def qs_interval(self):
         # qs interval in ms
@@ -456,22 +407,27 @@
         return qs
 
     def qs_interval_nr(self):
         # qs interval (normalized)
         qs = self.pqrst_dict["qs"]
         return qs / self.rms_rri()
 
-    def pflag(self):
-        if self.label == "N":
-            return 1
-        else:
-            return 0
+    def nsampels(self, n_samples=10):
+        """Gives equally spaced samples of the trimmed heartbeat waveform.
+
+        Parameters
+        ----------
+        n_samples : int, optional
+            Number of samples, by default 10
 
-    def nsampels(self, n_samples=50):
-        # get samples of the waveform
+        Returns
+        -------
+        list
+            Waveform sample values.
+        """
         dt = int(len(self.bwaveform) / n_samples)
         samples = []
         for i in range(n_samples):
             samples.append(self.bwaveform[int(i * dt)])
         return samples
 
     def sub_segs(self, n_subsegs=10):
@@ -513,29 +469,33 @@
         aggs = [mean_res, std_res, rms_res]
         return res, aggs
 
     # ============================================================
     # Spectral features of the beat waveform
     # ============================================================
     def fft_features(self):
-        # return fft of each beat bwaveform as a list.
+        """Returns FFT of each heartbeat trimmed waveform.
+
+        Returns
+        -------
+        list
+        """
+
         sig = self.bwaveform
-        num_samples = sig.size
+        # num_samples = sig.size
         # xf = rfftfreq(num_samples, 1 / self.fs)
         yf = np.abs(rfft(sig))
-
         return list(yf)
 
     # ============================================================
     # helper functions
     # ============================================================
     def plot_wf(self):
         from matplotlib import figure
 
-        # fig = figure.Figure()
         fig = figure.Figure(figsize=(8, 4), dpi=170)
         ax = fig.add_subplot(111)
         ax.plot(self.whole_waveform)
         # plt.plot(bwaveform)
         beat_rpeak_idx = self.rpeaks[self.beat_loc]
         beat_onset = self.wfpts["beat_onset"]
         beat_offset = self.wfpts["beat_offset"]
```

### Comparing `pyheartlib-0.0.6/src/pyheartlib/config.yaml` & `pyheartlib-0.0.7/src/pyheartlib/config.yaml`

 * *Files identical despite different names*

### Comparing `pyheartlib-0.0.6/src/pyheartlib/data.py` & `pyheartlib-0.0.7/src/pyheartlib/data.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,21 +5,14 @@
 from pyheartlib.io import get_data, save_data
 from pyheartlib.processing import Processing
 
 
 class Data:
     """Parent of other data classes.
 
-    Attributes
-    ----------
-    config : dict
-        Dataset config loaded from config.yaml file.
-    data_path : str
-        Path of the data directory.
-
     Parameters
     ----------
     base_path : str, optional
         Path of the main directory for loading and saving data, by default None
     remove_bl : bool, optional
         If True, the baseline is removed from the raw signals before extracting
         beat excerpts, by default False
@@ -27,14 +20,22 @@
         Whether to apply low pass filtering to the raw signals, by default False
     sampling_rate : int, optional
         Sampling rate of the signals, by default 360
     cutoff : int, optional
         Parameter of the low pass filter, by default 45
     order : int, optional
         Parameter of the low pass filter, by default 15
+
+    Attributes
+    ----------
+    config : dict
+        Dataset config loaded from config.yaml file.
+    data_path : str
+        Path of the data directory.
+
     """
 
     def __init__(
         self,
         base_path=None,
         remove_bl=False,
         lowpass=False,
@@ -62,21 +63,22 @@
         """Loads a record and returns its components.
 
         Parameters
         ----------
         record_id : str
             Record id.
         return_dict : bool
-            If True returns a dictionary, otherwise returns a pandas dataframe.
+            If True the method returns a dictionary, otherwise returns a pandas dataframe.
 
         Returns
         -------
         dict or dataframe
             If return_dict is True, it returns a dictionary
-            with keys: 'signal', 'r_locations', 'r_labels', 'rhythms', 'rhythms_locations'.
+            with keys: *signal*, *r_locations*, *r_labels*, *rhythms*,
+            *rhythms_locations*.
 
             If return_dict is False, it returns a dataframe containing the time, raw signal, and
             a list of equal size to the raw signal with None values except at annotations locations.
         """
         record_path = os.path.join(self.data_path, str(record_id))
         data_dict = get_data(record_path, self.config, return_dict=True)
         data_dict["signal"] = Processing.denoise_signal(
@@ -107,15 +109,16 @@
         rec_list : list
             List of records.
 
         Returns
         -------
         list
             A list containing a dict for each record. [rec1,rec2,....].
-            Each rec is a dict with keys: 'signal', 'r_locations', 'r_labels', 'rhythms', 'rhythms_locations', 'full_ann'.
+            Each rec is a dictionary with keys: *signal*, *r_locations*,
+            *r_labels*, *rhythms*, *rhythms_locations*, *full_ann*.
         """
 
         all_recs = []
         for rec_id in tqdm(rec_list, disable=DataSeq.progress_bar):
             rec_dict = self.get_ecg_record(record_id=rec_id)
             rec_dict["full_ann"] = self.full_annotate(rec_dict)[
                 1
@@ -141,17 +144,20 @@
             Windows size
         stride : int, optional
             Stride of the moving windows, by default 36
 
         Returns
         -------
         list
-            The list contains two elements. First element is a list containing a dict for each record, [rec1,rec2,....].
-            Each rec is a dict with keys: 'signal','r_locations','r_labels','rhythms','rhythms_locations', 'full_ann'. Second element is
-            a list of lists. Each inner list is like [record_no, start_win, end_win, label]. E.g. : [[10,500,800,'AFIB'], [10,700,900,'(N'], ...].
+            The list contains two elements. First element is a list containing
+            a dict for each record, [rec1,rec2,....].
+            Each rec is a dict with keys: *signal*, *r_locations*, *r_labels*,
+            *rhythms*, *rhythms_locations*, *full_ann*. Second element is a nested list.
+            Each inner list is like [record_no, start_win, end_win, label].
+            E.g. : [[10,500,800,'AFIB'], [10,700,900,'(N'], ...].
         """
 
         annotated_records = self.get_all_annotated_records(rec_list)
         samples_info = self.make_samples_info(annotated_records, win_size, stride)
         data = [annotated_records, samples_info]
         file_path = os.path.join(self.base_path, file_name)
         save_data(data, file_path=file_path)
```

### Comparing `pyheartlib-0.0.6/src/pyheartlib/data_arrhythmia.py` & `pyheartlib-0.0.7/src/pyheartlib/data_arrhythmia.py`

 * *Files identical despite different names*

### Comparing `pyheartlib-0.0.6/src/pyheartlib/data_beat.py` & `pyheartlib-0.0.7/src/pyheartlib/data_beat.py`

 * *Files 3% similar despite different names*

```diff
@@ -138,27 +138,27 @@
     def make_dataset(self, records, beatinfo_obj=None):
         """Creates a dataset from the provided records.
 
         Parameters
         ----------
         records : list
             A list containing records ids.
-        beatinfo_obj : instance of BeatInfo
-            An instance of BeatInfo.
+        beatinfo_obj : instance of BeatInfo.
 
         Returns
         -------
         dict
-            A dictionary containing:
-                'waveforms' : numpy.ndarray
-                    2D array of beat waveforms.
-                'beat_feats' : pd.DataFrame
-                    DataFrame of beats' features.
-                'labels' : numpy.ndarray
-                    1D array of beats' labels.
+            Dictionary with keys:
+
+            'waveforms' : numpy.ndarray
+                2D array of beat waveforms.
+            'beat_feats' : pd.DataFrame
+                DataFrame of beats' features.
+            'labels' : numpy.ndarray
+                1D array of beats' labels.
         """
         xds = []
         yds = []
         rds = []
         start_idxs = []
         rec_ids_list = []  # debug
         for i in tqdm(range(len(records)), disable=self.progress_bar):
@@ -199,22 +199,29 @@
 
     def beat_info_feat(self, data, beatinfo_obj):
         """Provides the computed features for all the beats.
 
         Parameters
         ----------
         data : dict
-            A dictionary containing:
-                'waveform' : list of waveforms
-                'rpeak_locs' : list of rpeak locations
-                'rec_ids' : list of record ids
-                'start_idxs' : list of start_idxs of waveforms on the raw signal
-                'labels' : list of beat labels
-        beatinfo_obj : instance of BeatInfo
-            An instance of BeatInfo.
+
+            Dictionary with keys:
+
+            'waveform' : list
+                List of waveforms.
+            'rpeak_locs' : list
+                List of rpeak locations.
+            'rec_ids' : list
+                List of record ids.
+            'start_idxs' : list
+                List of start_idxs of waveforms on the raw signal.
+            'labels' : list
+                List of beat labels.
+        beatinfo_obj : Instance of BeatInfo
+
         Returns
         -------
         Tuple
             features : list
                 Contains feature dictionaries for all the beats.
             labels : list
                 Contains corresponding beat labels.
@@ -241,226 +248,58 @@
             features.append(beat_features_dict)
             # only append labels for beats that are correct
             labels.append(beatinfo_obj.label)
             # import time
             # time.sleep(0.3)
         return features, labels
 
-    def clean_irrelevant_data(self, ds):
-        """Removes data with irrelevant labels (symbols) which are not in the symbols list.
-
-        Parameters
-        ----------
-        ds : dict
-            Dataset as a dictionary containing waveforms, beat features, and labels.
-
-        Returns
-        -------
-        dict
-            Cleaned dataset
-        """
-
-        yds = ds["labels"]
-        xds = ds["waveforms"]
-        rds = ds["beat_feats"]
-        indexes_rm = [i for i, item in enumerate(yds) if item not in self.syms]
-        # indexes_rm = np.where(np.invert(np.isin(yds, self.syms)))[0]
-        xds = np.delete(xds, indexes_rm, axis=0)
-        rds = np.delete(rds, indexes_rm, axis=0)
-        yds = np.delete(yds, indexes_rm, axis=0)
-        # ydsc = [it for ind,it in enumerate(yds) if ind not in indexes_rm]
-        return {"waveforms": xds, "beat_feats": rds, "labels": yds}
-
-    def search_label(self, inp, sym="N"):
-        """Searches the provided data and returns the indexes for a patricular label.
-
-        Parameters
-        ----------
-        inp : dict or numpy.ndarray
-            Input can be a dictionary having a 'labels' key, or a 1D numpy array.
-        sym : str, optional
-            The label to be searched for in the dataset, by default 'N'
-
-        Returns
-        -------
-        list
-            A list of indexes corresponding to the searched label.
-
-        Raises
-        ------
-        TypeError
-            Input data must be a dictionary or a numpy array.
-        """
-
-        if isinstance(inp, dict):
-            yds = list(inp["labels"])
-        elif isinstance(inp, np.ndarray):
-            yds = inp
-        else:
-            raise TypeError("input must be a dictionary or a numpy array!")
-        indexes = [i for i, item in enumerate(yds) if item == sym]
-        return indexes
-
-    def report_stats(self, yds_list):
-        """Counts the number of samples for each label type in the data.
-
-        Parameters
-        ----------
-        yds_list : list
-            List containing several label data sets. e.g train,val,test.
-
-        Returns
-        -------
-        list
-            A list of dictionaries. One dictionary per one data set.
-            Keys are labels types(symbols) and values are the counts of each specific symbol.
-        """
-        res_list = []
-        for yds in yds_list:
-            res = {}
-            for sym in self.syms:
-                indexes = [i for i, item in enumerate(yds) if item == sym]
-                res[sym] = len(indexes)
-            res_list.append(res)
-        return res_list
-
-    def report_stats_table(self, yds_list, name_list=[]):
-        """Returns the number of samples for each label type in the data.
-
-        Parameters
-        ----------
-        yds_list : list
-            List containing several label data. e.g train,val,test.
-        name_list : list, optional
-            A list of strings as the name of label data e.g. train,val,test, by default []
-
-        Returns
-        -------
-        pandas.dataframe
-            A dataframe containing symbols and their counts.
-        """
-        if len(name_list) == len(yds_list):
-            indx = name_list
-        else:
-            indx = None
-        res_list = self.report_stats(yds_list)
-        df = pd.DataFrame(res_list, index=indx)
-        return df
-
-    def save_dataset_inter(self, records, beatinfo_obj, file=None, clean=True):
+    def save_dataset_inter(self, records, beatinfo_obj, file=None):
         """Makes dataset and saves it in a file.
 
         Parameters
         ----------
         records : list
             A list containing records ids.
         beatinfo_obj : instance of BeatInfo
-            An instance of BeatInfo.
         file : str
             Name of the file to be saved.
-        clean : bool, optional
-            If True removes irrelevant label types, by default True
-
-        Raises
-        ------
-        ValueError
-            File path is not provided.
         """
 
         if file is None:
             raise ValueError("Save file path is not provided!")
         ds = self.make_dataset(records, beatinfo_obj)
-        if clean == True:
-            ds = self.clean_irrelevant_data(ds)
         save_data(ds, file_path=os.path.join(self.base_path, file))
 
-    def save_dataset_single(
-        self, record, beatinfo_obj, clean=True, split_ratio=0.3, file=None
-    ):
-        """Saves the signal fragments and their labels into a file for a single record.
-
-        Parameters
-        ----------
-        record : str
-            Record id.
-        beatinfo_obj : instance of BeatInfo
-            An instance of BeatInfo.
-        clean : bool, optional
-            If True does not include irrelevant label classes, by default True
-        split_ratio : float, optional
-            Ratio of test set, by default 0.3
-        file : str, optional
-            Name of the file to be saved, by default None
-        """
-        ds = self.make_dataset([record], beatinfo_obj)
-        if clean is True:
-            ds = self.clean_irrelevant_data(ds)
-
-        # slice the dataset based on the split_ratio
-        xarr = ds["waveforms"]
-        farr = ds["beat_feats"]
-        yarr = ds["labels"]
-        print(xarr.shape[0])
-        print(len(xarr))
-        split_idx = int(split_ratio * xarr.shape[0])
-        xarr_train = xarr[:split_idx]
-        xarr_test = xarr[split_idx:]
-        farr_train = farr[:split_idx]
-        farr_test = farr[split_idx:]
-        yarr_train = yarr[:split_idx]
-        yarr_test = yarr[split_idx:]
-
-        ds_train = {
-            "waveforms": xarr_train,
-            "beat_feats": farr_train,
-            "labels": yarr_train,
-        }
-        ds_test = {"waveforms": xarr_test, "beat_feats": farr_test, "labels": yarr_test}
-        if file is None:
-            file_train = str(record) + "_train" + ".beat"
-            file_test = str(record) + "_test" + ".beat"
-        else:
-            file_train = file + "_train" + ".beat"
-            file_test = file + "_test" + ".beat"
-        save_data(ds_train, file_path=os.path.join(self.base_path, file_train))
-        save_data(ds_test, file_path=os.path.join(self.base_path, file_test))
-
     def save_dataset_intra(
         self,
         records,
         beatinfo_obj,
-        clean=True,
         split_ratio=0.3,
         file_prefix="intra",
     ):
         """Makes and saves the dataset in intra way.
 
         Parameters
         ----------
         records : list, optional
             A list of record ids.
         beatinfo_obj : instance of BeatInfo
-            An instance of BeatInfo.
-        clean : bool, optional
-            If True does not include irrelevant label classes, by default True
         split_ratio : float, optional
             Ratio of test set, by default 0.3
         file_prefix : str, optional
             Prefix for the file names to be saved, by default 'intra'
         """
         xdata_train = []
         fdata_train = pd.DataFrame()
         ydata_train = []
         xdata_test = []
         fdata_test = pd.DataFrame()
         ydata_test = []
         for record in records:
             ds = self.make_dataset([record], beatinfo_obj)
-            if clean is True:
-                ds = self.clean_irrelevant_data(ds)
 
             # slice the dataset based on the split_ratio
             xarr = ds["waveforms"]
             farr = ds["beat_feats"]
             yarr = ds["labels"]
 
             split_idx = int(split_ratio * xarr.shape[0])
@@ -496,31 +335,68 @@
 
         file_train = file_prefix + "_train" + ".beat"
         save_data(ds_train, file_path=os.path.join(self.base_path, file_train))
 
         file_test = file_prefix + "_test" + ".beat"
         save_data(ds_test, file_path=os.path.join(self.base_path, file_test))
 
+    def save_dataset_single(self, record, beatinfo_obj, split_ratio=0.3, file=None):
+        """Saves the signal fragments and their labels into a file for a single record.
+
+        Parameters
+        ----------
+        record : str
+            Record id.
+        beatinfo_obj : instance of BeatInfo
+        split_ratio : float, optional
+            Ratio of test set, by default 0.3
+        file : str, optional
+            Name of the file to be saved, by default None
+        """
+        ds = self.make_dataset([record], beatinfo_obj)
+
+        # slice the dataset based on the split_ratio
+        xarr = ds["waveforms"]
+        farr = ds["beat_feats"]
+        yarr = ds["labels"]
+        split_idx = int(split_ratio * xarr.shape[0])
+        xarr_train = xarr[:split_idx]
+        xarr_test = xarr[split_idx:]
+        farr_train = farr[:split_idx]
+        farr_test = farr[split_idx:]
+        yarr_train = yarr[:split_idx]
+        yarr_test = yarr[split_idx:]
+
+        ds_train = {
+            "waveforms": xarr_train,
+            "beat_feats": farr_train,
+            "labels": yarr_train,
+        }
+        ds_test = {"waveforms": xarr_test, "beat_feats": farr_test, "labels": yarr_test}
+        if file is None:
+            file_train = str(record) + "_train" + ".beat"
+            file_test = str(record) + "_test" + ".beat"
+        else:
+            file_train = file + "_train" + ".beat"
+            file_test = file + "_test" + ".beat"
+        save_data(ds_train, file_path=os.path.join(self.base_path, file_train))
+        save_data(ds_test, file_path=os.path.join(self.base_path, file_test))
+
     def load_data(self, file_name):
         """Loads a file containing a dataframe.
 
         Parameters
         ----------
         file_name : str
             File name. The final final path is the join of base path and file name.
 
         Returns
         -------
         pandas.dataframe
             Dataset as a dataframe. Keys are "waveforms", "beat_feats", and "labels".
-
-        Raises
-        ------
-        ValueError
-            File name is not provided.
         """
 
         if file_name is None:
             raise ValueError("Load file name is not provided!")
         ds = load_data(file_path=os.path.join(self.base_path, file_name))
         for k, v in ds.items():
             print(
@@ -528,14 +404,60 @@
                     k, v.shape, v.shape[0]
                 )
             )
         print(self.report_stats_table([ds["labels"]], [file_name]))
         print()
         return ds
 
+    def report_stats(self, yds_list):
+        """Counts the number of samples for each label type in the data.
+
+        Parameters
+        ----------
+        yds_list : list
+            List containing several label data sets. e.g train,val,test.
+
+        Returns
+        -------
+        list
+            A list of dictionaries. One dictionary per one data set.
+            Keys are labels types(symbols) and values are the counts of each specific symbol.
+        """
+        res_list = []
+        for yds in yds_list:
+            res = {}
+            for sym in self.syms:
+                indexes = [i for i, item in enumerate(yds) if item == sym]
+                res[sym] = len(indexes)
+            res_list.append(res)
+        return res_list
+
+    def report_stats_table(self, yds_list, name_list=[]):
+        """Returns the number of samples for each label type in the data.
+
+        Parameters
+        ----------
+        yds_list : list
+            List containing several label data. e.g train,val,test.
+        name_list : list, optional
+            A list of strings as the name of label data e.g. train,val,test, by default []
+
+        Returns
+        -------
+        pandas.dataframe
+            A dataframe containing symbols and their counts.
+        """
+        if len(name_list) == len(yds_list):
+            indx = name_list
+        else:
+            indx = None
+        res_list = self.report_stats(yds_list)
+        df = pd.DataFrame(res_list, index=indx)
+        return df
+
     def per_record_stats(self, rec_ids_list=None, cols=None):
         """Returns a dataframe containing the number of each type in each record.
 
         Parameters
         ----------
         rec_ids_list : list, optional
             List of record ids, by default None
@@ -560,41 +482,67 @@
         df.fillna(0, inplace=True)
         df = df.astype("int32")
         df = df[list(set(cols) & set(df.columns))]
         return df
 
     def slice_data(self, ds, labels_list):
         """Only holds the data that their annotation is in the labels_list"""
+
         sliced_x = ds["waveforms"]
         sliced_r = ds["beat_feats"]
         sliced_y = ds["labels"]
         indexes_keep = []
         for sym in labels_list:
             inds = [i for i, item in enumerate(sliced_y) if item == sym]
             indexes_keep.extend(inds)
         sliced_x = sliced_x[indexes_keep]
         sliced_r = sliced_r[indexes_keep]
         sliced_y = sliced_y[indexes_keep]
         return {"waveforms": sliced_x, "beat_feats": sliced_r, "labels": sliced_y}
 
-    def search_type(self, x, y, sym="N"):
-        """Search for a signal excerpt with a patricular type"""
-        indexes = [i for i, item in enumerate(y) if item == sym]
-        return x[indexes], indexes
+    def search_label(self, inp, sym="N"):
+        """Searches the provided data and returns the indexes for a patricular label.
+
+        Parameters
+        ----------
+        inp : dict or numpy.ndarray
+            Input can be a dictionary having a 'labels' key, or a 1D numpy array.
+        sym : str, optional
+            The label to be searched for in the dataset, by default 'N'
+
+        Returns
+        -------
+        list
+            A list of indexes corresponding to the searched label.
+
+        Raises
+        ------
+        TypeError
+            Input data must be a dictionary or a numpy array.
+        """
+
+        if isinstance(inp, dict):
+            yds = list(inp["labels"])
+        elif isinstance(inp, np.ndarray):
+            yds = inp
+        else:
+            raise TypeError("input must be a dictionary or a 1D numpy array!")
+        indexes = [i for i, item in enumerate(yds) if item == sym]
+        return indexes
 
     def aug_decrease(self, ds, label="N", desired_size=21000):
         """Simple data augmentation to decrease a particular type in the dataset."""
         import random
         import copy
 
         ds = copy.deepcopy(ds)
         xx = ds["waveforms"]
         rr = ds["beat_feats"]
         yy = ds["labels"]
-        _, ind = self.search_type(xx, yy, sym=label)
+        ind = self.search_label(ds, sym=label)
         random.shuffle(ind)
         nn = len(ind) - desired_size
         ind_remove = ind[0:nn]
         x_train_aug = np.delete(xx, ind_remove, axis=0)
         r_train_aug = np.delete(rr, ind_remove, axis=0)
         y_train_aug = np.delete(yy, ind_remove)
         print(x_train_aug.shape, y_train_aug.shape)
@@ -609,15 +557,15 @@
         import copy
 
         x_aug = ds["waveforms"]
         r_aug = ds["beat_feats"]
         y_aug = ds["labels"].tolist()
         for sym in self.config["BEAT_TYPES"]:
             try:
-                _, ind_minor = self.search_type(ds["waveforms"], ds["labels"], sym=sym)
+                ind_minor = self.search_label(ds, sym=sym)
                 minority = np.take(ds["waveforms"], ind_minor, axis=0)
                 minority_r = np.take(ds["beat_feats"], ind_minor, axis=0)
                 minority_labels = [sym] * len(minority)
                 if len(minority) > 0 and len(ind_minor) < desired_size:
                     times = desired_size // len(minority)
                     if times > 0:
                         arr = copy.deepcopy(minority)
@@ -632,15 +580,117 @@
                         y_aug = y_aug + list_appnd
                     else:
                         print(sym)
             except:
                 print("label zero")
         return {"waveforms": x_aug, "beat_feats": r_aug, "labels": np.array(y_aug)}
 
-    def stndr(self, arr, mean, std):
-        X = arr.copy()
-        X = (X - np.mean(X)) / np.std(X)
-        return X
-
-    def binarize_labels(self, labels_list, positive_label, pos=1, neg=-1):
-        new_y = [pos if item == positive_label else neg for item in labels_list]
-        return new_y
+    def clean_inf_nan(self, ds):
+        """Cleans the dataset by removing samples with inf and nan in computed features.
+
+        Parameters
+        ----------
+        ds : dict
+            Dataset as a dictionary.
+
+        Returns
+        -------
+        dict
+            Cleaned dataset.
+        """
+
+        yds = ds["labels"]
+        xds = ds["waveforms"]
+        fds = ds["beat_feats"]
+        indexes = []
+        # cleans feature array
+        indexes.extend(np.where(np.isinf(fds))[0])
+        indexes.extend(np.where(np.isnan(fds))[0])
+        fds.drop(indexes, axis=0, inplace=True)
+        xds = np.delete(xds, indexes, axis=0)
+        yds = np.delete(yds, indexes, axis=0)
+        return {"waveforms": xds, "beat_feats": fds, "labels": yds}
+
+    def clean_IQR(self, ds, factor=1.5, return_indexes=False):
+        """Cleans the dataset by removing outliers using IQR method.
+
+        Parameters
+        ----------
+        ds : dict
+            Dataset.
+        factor : float, optional
+            Parameter of IQR method, by default 1.5
+        return_indexes : bool, optional
+            If True returns indexes of outliers, otherwise returns cleaned dataset, by default False
+
+        Returns
+        -------
+        dict
+            Cleaned dataset.
+        """
+        yds = ds["labels"]
+        xds = ds["waveforms"]
+        fds = ds["beat_feats"]
+        # cleans a 2d array. Each column is a features, rows are samples. Only fds.
+        ind_outliers = []
+        for i in range(fds.shape[1]):
+            x = fds[:, i]
+            Q1 = np.quantile(x, 0.25, axis=0)
+            Q3 = np.quantile(x, 0.75, axis=0)
+            IQR = Q3 - Q1
+            inds = np.where((x > (Q3 + factor * IQR)) | (x < (Q1 - factor * IQR)))[0]
+            ind_outliers.extend(inds)
+        fds.drop(ind_outliers, axis=0, inplace=True)
+        xds = np.delete(xds, ind_outliers, axis=0)
+        yds = np.delete(yds, ind_outliers, axis=0)
+        if return_indexes is False:
+            return {"waveforms": xds, "beat_feats": fds, "labels": yds}
+        else:
+            return ind_outliers
+
+    def append_ds(self, ds1, ds2):
+        """Appends two datasets together.
+
+        Parameters
+        ----------
+        ds1 : dict
+            Dataset one.
+        ds2 : dict
+            Dataset two.
+
+        Returns
+        -------
+        dict
+            Final dataset.
+        """
+        dss = dict()
+        dss["waveforms"] = np.vstack((ds1["waveforms"], ds2["waveforms"]))
+        # dss["beat_feats"] = np.vstack((ds1["beat_feats"], ds2["beat_feats"]))
+        dss["beat_feats"] = pd.concat([ds1["beat_feats"], ds2["beat_feats"]])
+        dss["labels"] = np.vstack(
+            (ds1["labels"].reshape(-1, 1), ds2["labels"].reshape(-1, 1))
+        ).flatten()
+        return dss
+
+    def clean_IQR_class(self, ds, factor=1.5):
+        """Cleans dataset by IQR method for every class separately.
+
+        Parameters
+        ----------
+        ds : dict
+            Dataset.
+        factor : float, optional
+            Parameter of IQR method, by default 1.5
+
+        Returns
+        -------
+        dict
+            Cleaned dataset.
+        """
+        for label in list(np.unique(ds["labels"])):
+            sliced = self.slice_data(ds, [label])
+            cleaned = self.clean_IQR(sliced, factor=factor)
+            try:
+                ds_all = append_ds(ds_all, cleaned)
+            except NameError:
+                ds_all = cleaned
+        return ds_all
```

### Comparing `pyheartlib-0.0.6/src/pyheartlib/data_rpeak.py` & `pyheartlib-0.0.7/src/pyheartlib/data_rpeak.py`

 * *Files identical despite different names*

### Comparing `pyheartlib-0.0.6/src/pyheartlib/extra/pqrst.py` & `pyheartlib-0.0.7/src/pyheartlib/extra/pqrst.py`

 * *Files identical despite different names*

### Comparing `pyheartlib-0.0.6/src/pyheartlib/extra/report.py` & `pyheartlib-0.0.7/src/pyheartlib/extra/report.py`

 * *Files identical despite different names*

### Comparing `pyheartlib-0.0.6/src/pyheartlib/extra/utils.py` & `pyheartlib-0.0.7/src/pyheartlib/extra/utils.py`

 * *Files identical despite different names*

### Comparing `pyheartlib-0.0.6/src/pyheartlib/features.py` & `pyheartlib-0.0.7/src/pyheartlib/features.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,16 +65,16 @@
 def get_hrv_features(rri, features="all"):
     """
     Computes hrv features for the input samples.
 
     Parameters
     ----------
     rri : numpy.array
-        A 2D numpy array with shape (#samples,len_series).
-        Series are rr intervals in milliseconds(ms)
+        A 2D numpy array with shape (#samples, len_series).
+        Series are rr intervals in milliseconds(ms).
     features : list
         A list of features to be computed.
 
     Returns
     -------
     features_arr : numpy.array
         A 2D numpy array with the shape (#samples, #features).
@@ -177,17 +177,29 @@
         ix = flist.index("sdhr")
         features_arr[:, ix] = np.std(hr, axis=1)
 
     return features_arr
 
 
 def get_wf_feats(sig, interval):
-    """Computes features for the signal waveform
+    """Computes features for the signal waveform.
 
     The input signal is segmented into sub-signals based on the given interval parameter.
+
+    Parameters
+    ----------
+    sig : numpy.array
+        A 1D numpy array.
+    interval : int
+        Length of subsegments.
+
+    Returns
+    -------
+    features_arr : numpy.array
+        A 2D numpy array with the shape (#subsegments, #features).
     """
     b = int(len(sig) / interval)
     subseqs = []
     for i in range(b):
         subseq = sig[i * interval : (i + 1) * interval]
         subseqs.append(subseq)
     subseqs = np.array(subseqs)  # interval=36---> (300,36)
@@ -202,9 +214,11 @@
     f8 = np.amax(sqr, axis=1)
     f9 = np.amin(sqr, axis=1)
     f10 = np.mean(sqr, axis=1)
     f11 = np.std(sqr, axis=1)
     f12 = np.median(sqr, axis=1)
     f13 = stats.skew(sqr, axis=1)
     f14 = stats.kurtosis(sqr, axis=1)
-    feats = np.vstack((f1, f2, f3, f4, f5, f6, f7, f8, f9, f10, f11, f12, f13, f14))
-    return feats.T
+    features_arr = np.vstack(
+        (f1, f2, f3, f4, f5, f6, f7, f8, f9, f10, f11, f12, f13, f14)
+    )
+    return features_arr.T
```

### Comparing `pyheartlib-0.0.6/src/pyheartlib/io.py` & `pyheartlib-0.0.7/src/pyheartlib/io.py`

 * *Files identical despite different names*

### Comparing `pyheartlib-0.0.6/PKG-INFO` & `pyheartlib-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: pyheartlib
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Python package for processing and modeling electrocardiogram signals
 License: Proprietary
 Author: Sadegh Mohammadi
 Requires-Python: >=3.10,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.22.0)
 Requires-Dist: pandas (>=1.4.0)
+Requires-Dist: pyyaml (>=6.0)
 Requires-Dist: scikit-learn (>=1.1.0)
 Requires-Dist: tensorflow (>=2.8.0)
 Requires-Dist: tqdm (>=4.63.0)
 Requires-Dist: wfdb (>=4.0.0)
 Description-Content-Type: text/markdown
 
 # pyheartlib
```

