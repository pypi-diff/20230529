# Comparing `tmp/fluvio-0.9.6b2.tar.gz` & `tmp/fluvio-0.9.6b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluvio-0.9.6b2.tar", last modified: Thu Sep 23 18:46:02 2021, max compression
+gzip compressed data, was "fluvio-0.9.6b3.tar", last modified: Fri Oct  1 00:20:07 2021, max compression
```

## Comparing `fluvio-0.9.6b2.tar` & `fluvio-0.9.6b3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 18:46:02.765005 fluvio-0.9.6b2/
--rw-r--r--   0 runner    (1001) docker     (121)    45177 2021-09-23 18:41:04.000000 fluvio-0.9.6b2/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (121)      431 2021-09-23 18:41:04.000000 fluvio-0.9.6b2/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-09-23 18:41:04.000000 fluvio-0.9.6b2/LICENSE-APACHE
--rw-r--r--   0 runner    (1001) docker     (121)       97 2021-09-23 18:41:04.000000 fluvio-0.9.6b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3626 2021-09-23 18:46:02.765005 fluvio-0.9.6b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2715 2021-09-23 18:41:04.000000 fluvio-0.9.6b2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      578 2021-09-23 18:41:04.000000 fluvio-0.9.6b2/build.rs
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 18:46:02.761005 fluvio-0.9.6b2/fluvio/
--rw-r--r--   0 runner    (1001) docker     (121)     7089 2021-09-23 18:41:04.000000 fluvio-0.9.6b2/fluvio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 18:46:02.765005 fluvio-0.9.6b2/fluvio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3626 2021-09-23 18:46:02.000000 fluvio-0.9.6b2/fluvio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      285 2021-09-23 18:46:02.000000 fluvio-0.9.6b2/fluvio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-23 18:46:02.000000 fluvio-0.9.6b2/fluvio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-23 18:46:02.000000 fluvio-0.9.6b2/fluvio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-09-23 18:46:02.000000 fluvio-0.9.6b2/fluvio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       69 2021-09-23 18:41:04.000000 fluvio-0.9.6b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-23 18:46:02.765005 fluvio-0.9.6b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1814 2021-09-23 18:41:04.000000 fluvio-0.9.6b2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-23 18:46:02.765005 fluvio-0.9.6b2/src/
--rw-r--r--   0 runner    (1001) docker     (121)     4819 2021-09-23 18:41:04.000000 fluvio-0.9.6b2/src/glue.rs.in
--rw-r--r--   0 runner    (1001) docker     (121)       83 2021-09-23 18:41:04.000000 fluvio-0.9.6b2/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-01 00:20:07.854752 fluvio-0.9.6b3/
+-rw-r--r--   0 runner    (1001) docker     (121)    44934 2021-10-01 00:16:27.000000 fluvio-0.9.6b3/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (121)      431 2021-10-01 00:16:27.000000 fluvio-0.9.6b3/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-10-01 00:16:27.000000 fluvio-0.9.6b3/LICENSE-APACHE
+-rw-r--r--   0 runner    (1001) docker     (121)       97 2021-10-01 00:16:27.000000 fluvio-0.9.6b3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     3611 2021-10-01 00:20:07.854752 fluvio-0.9.6b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2700 2021-10-01 00:16:27.000000 fluvio-0.9.6b3/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      578 2021-10-01 00:16:27.000000 fluvio-0.9.6b3/build.rs
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-01 00:20:07.854752 fluvio-0.9.6b3/fluvio/
+-rw-r--r--   0 runner    (1001) docker     (121)     7089 2021-10-01 00:16:27.000000 fluvio-0.9.6b3/fluvio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-01 00:20:07.854752 fluvio-0.9.6b3/fluvio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3611 2021-10-01 00:20:07.000000 fluvio-0.9.6b3/fluvio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2021-10-01 00:20:07.000000 fluvio-0.9.6b3/fluvio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-01 00:20:07.000000 fluvio-0.9.6b3/fluvio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-01 00:20:07.000000 fluvio-0.9.6b3/fluvio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-10-01 00:20:07.000000 fluvio-0.9.6b3/fluvio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2021-10-01 00:16:27.000000 fluvio-0.9.6b3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-01 00:20:07.854752 fluvio-0.9.6b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1814 2021-10-01 00:16:27.000000 fluvio-0.9.6b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-01 00:20:07.854752 fluvio-0.9.6b3/src/
+-rw-r--r--   0 runner    (1001) docker     (121)     4819 2021-10-01 00:16:27.000000 fluvio-0.9.6b3/src/glue.rs.in
+-rw-r--r--   0 runner    (1001) docker     (121)       83 2021-10-01 00:16:27.000000 fluvio-0.9.6b3/src/lib.rs
```

### Comparing `fluvio-0.9.6b2/Cargo.lock` & `fluvio-0.9.6b3/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -116,17 +116,17 @@
  "async-io",
  "blocking",
  "futures-lite",
 ]
 
 [[package]]
 name = "async-process"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a8f38756dd9ac84671c428afbf7c9f7495feff9ec5b0710f17100098e5b354ac"
+checksum = "b21b63ab5a0db0369deb913540af2892750e42d949faacc7a61495ac418a1692"
 dependencies = [
  "async-io",
  "blocking",
  "cfg-if",
  "event-listener",
  "futures-lite",
  "libc",
@@ -143,17 +143,17 @@
 dependencies = [
  "async-mutex",
  "event-listener",
 ]
 
 [[package]]
 name = "async-std"
-version = "1.9.0"
+version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d9f06685bad74e0570f5213741bea82158279a4103d988e57bfada11ad230341"
+checksum = "f8056f1455169ab86dd47b47391e4ab0cbd25410a70e9fe675544f49bafaf952"
 dependencies = [
  "async-channel",
  "async-global-executor",
  "async-io",
  "async-lock",
  "async-process",
  "crossbeam-utils",
@@ -228,17 +228,17 @@
 name = "base64"
 version = "0.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "904dfeac50f3cdaba28fc6f57fdcddb75f49ed61346676a78c4ffe55877802fd"
 
 [[package]]
 name = "bitflags"
-version = "1.2.1"
+version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cf1de2fe8c75bc145a2f577add951f8134889b4795d47466a54a5c846d691693"
+checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "blocking"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c5e170dbede1f740736619b776d7251cb1b9095c435c34d8ca9f57fcd2f335e9"
 dependencies = [
@@ -248,35 +248,35 @@
  "fastrand",
  "futures-lite",
  "once_cell",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.7.0"
+version = "3.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c59e7af012c713f529e7a3ee57ce9b31ddd858d4b512923602f74608b009631"
+checksum = "d9df67f7bf9ef8498769f994239c45613ef0c5899415fb58e9add412d2c1a538"
 
 [[package]]
 name = "bytes"
-version = "1.0.1"
+version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b700ce4376041dcd0a327fd0097c41095743c4c8af8887265942faf1100bd040"
+checksum = "c4872d67bab6358e59559027aa3b9157c53d9358c51423c17554809a8858e0f8"
 
 [[package]]
 name = "cache-padded"
 version = "1.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "631ae5198c9be5e753e5cc215e1bd73c2b466a3565173db433f52bb9d3e66dba"
 
 [[package]]
 name = "cc"
-version = "1.0.69"
+version = "1.0.70"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e70cc2f62c6ce1868963827bd677764c62d07c3d9a3e1fb1177ee1a9ab199eb2"
+checksum = "d26a6ce4b6a484fa3edb70f7efa6fc430fd2b87285fe8b84304fd0936faa0dc0"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
@@ -333,17 +333,17 @@
 dependencies = [
  "cfg-if",
  "lazy_static",
 ]
 
 [[package]]
 name = "ctor"
-version = "0.1.20"
+version = "0.1.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5e98e2ad1a782e33928b96fc3948e7c355e5af34ba4de7670fe8bac2a3b2006d"
+checksum = "ccc0a48a9b826acdf4028595adc9db92caea352f7af011a3034acd172a52a0aa"
 dependencies = [
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "darling"
@@ -494,29 +494,29 @@
  "strum",
  "syn",
  "which",
 ]
 
 [[package]]
 name = "flate2"
-version = "1.0.20"
+version = "1.0.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cd3aec53de10fe96d7d8c565eb17f2c687bb5518a2ec453b5b1252964526abe0"
+checksum = "1e6988e897c1c9c485f43b47a529cef42fde0547f9d8d41a7062518f1d8fc53f"
 dependencies = [
  "cfg-if",
  "crc32fast",
  "libc",
  "miniz_oxide",
 ]
 
 [[package]]
 name = "fluvio"
-version = "0.9.5"
+version = "0.9.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a3dddf55be8c05c09d39fa5abcdc0e3b92795a4903cd2e745c2b51ed855526b7"
+checksum = "e1451c6936f2bc13589737124216c4ee3a8da86c590482ca9ef00c8ab8bf53cb"
 dependencies = [
  "async-channel",
  "async-lock",
  "async-rwlock",
  "base64",
  "bytes",
  "cfg-if",
@@ -542,34 +542,34 @@
  "toml",
  "tracing",
  "tracing-futures",
 ]
 
 [[package]]
 name = "fluvio-controlplane-metadata"
-version = "0.11.1"
+version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ee403ac0924dfc8ea1ede654f2d0fff38a12781f63e935b8b96073dd7c28ac8f"
+checksum = "6ff2dce7b8031680af08f3c92fa8223e368213e35eced383a12f4ac62d0e655d"
 dependencies = [
  "async-trait",
  "fluvio-dataplane-protocol",
  "fluvio-future",
  "fluvio-protocol",
  "fluvio-stream-model",
  "fluvio-types",
  "flv-util",
  "log",
  "tracing",
 ]
 
 [[package]]
 name = "fluvio-dataplane-protocol"
-version = "0.6.0"
+version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1b437151cfcdc56c8d15de4b700a1026d18cc28a128af76aab34063134e16a5"
+checksum = "11f6b2407acc8bc8ad7a01cb8b5de00e074ef68c72c700b06788c714fc3db83d"
 dependencies = [
  "bytes",
  "cfg-if",
  "content_inspector",
  "crc32c",
  "eyre",
  "fluvio-future",
@@ -612,26 +612,26 @@
 checksum = "2c82ffee969c32ce6b5a596c6c8b3a9d5412c1b9ebb355a1ded7a5efcb0d72af"
 dependencies = [
  "bytes",
  "fluvio-future",
  "fluvio-protocol-api",
  "fluvio-protocol-codec",
  "fluvio-protocol-core",
- "fluvio-protocol-derive 0.3.0",
+ "fluvio-protocol-derive",
  "tracing",
 ]
 
 [[package]]
 name = "fluvio-protocol-api"
-version = "0.4.0"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "073574e905be69f14a3a1962d90cf3e353d02d2242985a453d78ea67d839f08a"
+checksum = "d68c561e8999df089915271ae25f5861fd9b4e571c9d8a58ef6e05bba7e157bd"
 dependencies = [
  "fluvio-protocol-core",
- "fluvio-protocol-derive 0.2.1",
+ "fluvio-protocol-derive",
  "flv-util",
  "tracing",
 ]
 
 [[package]]
 name = "fluvio-protocol-codec"
 version = "0.3.1"
@@ -642,67 +642,55 @@
  "fluvio-protocol-core",
  "log",
  "tokio-util",
 ]
 
 [[package]]
 name = "fluvio-protocol-core"
-version = "0.3.1"
+version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "197b15a522fe85abdfbe0f925d3293de32358c7b5f27f934e2acdfadc2632c2c"
+checksum = "690ec99ef681001bd0d692b59788f21c1caacf68b6d11730424f23f567dc6779"
 dependencies = [
  "bytes",
  "log",
 ]
 
 [[package]]
 name = "fluvio-protocol-derive"
-version = "0.2.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c7a5d62992277733fed40e8c9166f3c4843e9df35023dd74b644f3a6354b0212"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn",
- "tracing",
-]
-
-[[package]]
-name = "fluvio-protocol-derive"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8da35db64755c1becbfa015259f25b3dbb69fe012645154094cbe4febe2f803d"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
  "tracing",
 ]
 
 [[package]]
 name = "fluvio-sc-schema"
-version = "0.9.4"
+version = "0.10.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e9536d844d9107d8700b944e24eeeb4c0909055d6bb007dad1a3146d7f252947"
+checksum = "f3d266575533dbf90b66ae05edcba44edd9f870260cf623401501c66d44be240"
 dependencies = [
  "fluvio-controlplane-metadata",
  "fluvio-dataplane-protocol",
  "fluvio-protocol",
  "fluvio-types",
  "log",
  "static_assertions",
  "thiserror",
  "tracing",
 ]
 
 [[package]]
 name = "fluvio-socket"
-version = "0.10.0"
+version = "0.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "989a67e12af05201442cc10783cadd5b3ac0b657a1643422e8a99e5fada1c3a3"
+checksum = "4bd0d32c36b781d58beb33e05f914ea2fbec9cf5c12a7138fa8d68e417bb02c5"
 dependencies = [
  "async-channel",
  "async-lock",
  "async-trait",
  "bytes",
  "cfg-if",
  "event-listener",
@@ -715,48 +703,50 @@
  "tokio",
  "tokio-util",
  "tracing",
 ]
 
 [[package]]
 name = "fluvio-spu-schema"
-version = "0.8.1"
+version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6e52061ce95fdd7c06988f2ed83af813d303a159b91f7d8fd0834ce8ae999c12"
+checksum = "98e2470bfd7a3b71aef8536a648e08a4a2769d8c2f79aafedc766bdf8c3fc86d"
 dependencies = [
  "bytes",
  "flate2",
  "fluvio-dataplane-protocol",
  "fluvio-protocol",
  "log",
  "serde",
  "static_assertions",
  "tracing",
 ]
 
 [[package]]
 name = "fluvio-stream-model"
-version = "0.5.1"
+version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2ad47fd2cd14d75ea98228f049185732a676aa1390e38d9ad858b7b12b9dd610"
+checksum = "f727e6d2d57ededa529d78f57cfb7df104fc957932640134b8a729c2fffff468"
 dependencies = [
  "async-rwlock",
  "event-listener",
  "once_cell",
  "tracing",
 ]
 
 [[package]]
 name = "fluvio-types"
-version = "0.2.2"
+version = "0.2.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "591ae978fa5451502e6065fbc717ef92a334d9281ec8179caf21fe2c7c8adf34"
+checksum = "b586fdd7eb83f446294838e8a1f1021921b8d003bc5251e845f143f9a22d2f3c"
 dependencies = [
  "event-listener",
+ "thiserror",
  "tracing",
+ "tracing-futures",
 ]
 
 [[package]]
 name = "fluvio-wasm-timer"
 version = "0.2.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b768c170dc045fa587a8f948c91f9bcfb87f774930477c6215addf54317f137f"
@@ -817,59 +807,59 @@
 name = "foreign-types-shared"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "00b0228411908ca8685dba7fc2cdd70ec9990a6e753e89b6ac91a84c40fbaf4b"
 
 [[package]]
 name = "futures"
-version = "0.3.16"
+version = "0.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1adc00f486adfc9ce99f77d717836f0c5aa84965eb0b4f051f4e83f7cab53f8b"
+checksum = "a12aa0eb539080d55c3f2d45a67c3b58b6b0773c1a3ca2dfec66d58c97fd66ca"
 dependencies = [
  "futures-channel",
  "futures-core",
  "futures-executor",
  "futures-io",
  "futures-sink",
  "futures-task",
  "futures-util",
 ]
 
 [[package]]
 name = "futures-channel"
-version = "0.3.16"
+version = "0.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "74ed2411805f6e4e3d9bc904c95d5d423b89b3b25dc0250aa74729de20629ff9"
+checksum = "5da6ba8c3bb3c165d3c7319fc1cc8304facf1fb8db99c5de877183c08a273888"
 dependencies = [
  "futures-core",
  "futures-sink",
 ]
 
 [[package]]
 name = "futures-core"
-version = "0.3.16"
+version = "0.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af51b1b4a7fdff033703db39de8802c673eb91855f2e0d47dcf3bf2c0ef01f99"
+checksum = "88d1c26957f23603395cd326b0ffe64124b818f4449552f960d815cfba83a53d"
 
 [[package]]
 name = "futures-executor"
-version = "0.3.16"
+version = "0.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4d0d535a57b87e1ae31437b892713aee90cd2d7b0ee48727cd11fc72ef54761c"
+checksum = "45025be030969d763025784f7f355043dc6bc74093e4ecc5000ca4dc50d8745c"
 dependencies = [
  "futures-core",
  "futures-task",
  "futures-util",
 ]
 
 [[package]]
 name = "futures-io"
-version = "0.3.16"
+version = "0.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0b0e06c393068f3a6ef246c75cdca793d6a46347e75286933e5e75fd2fd11582"
+checksum = "522de2a0fe3e380f1bc577ba0474108faf3f6b18321dbf60b3b9c39a75073377"
 
 [[package]]
 name = "futures-lite"
 version = "1.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7694489acd39452c77daa48516b894c153f192c3578d5a839b62c58099fcbf48"
 dependencies = [
@@ -880,42 +870,42 @@
  "parking",
  "pin-project-lite",
  "waker-fn",
 ]
 
 [[package]]
 name = "futures-macro"
-version = "0.3.16"
+version = "0.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c54913bae956fb8df7f4dc6fc90362aa72e69148e3f39041fbe8742d21e0ac57"
+checksum = "18e4a4b95cea4b4ccbcf1c5675ca7c4ee4e9e75eb79944d07defde18068f79bb"
 dependencies = [
  "autocfg",
  "proc-macro-hack",
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "futures-sink"
-version = "0.3.16"
+version = "0.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c0f30aaa67363d119812743aa5f33c201a7a66329f97d1a887022971feea4b53"
+checksum = "36ea153c13024fe480590b3e3d4cad89a0cfacecc24577b68f86c6ced9c2bc11"
 
 [[package]]
 name = "futures-task"
-version = "0.3.16"
+version = "0.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bbe54a98670017f3be909561f6ad13e810d9a51f3f061b902062ca3da80799f2"
+checksum = "1d3d00f4eddb73e498a54394f228cd55853bdf059259e8e7bc6e69d408892e99"
 
 [[package]]
 name = "futures-util"
-version = "0.3.16"
+version = "0.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "67eb846bfd58e44a8481a00049e82c43e0ccb5d61f8dc071057cb19249dd4d78"
+checksum = "36568465210a3a6ee45e1f165136d68671471a501e632e9a98d96872222b5481"
 dependencies = [
  "autocfg",
  "futures-channel",
  "futures-core",
  "futures-io",
  "futures-macro",
  "futures-sink",
@@ -1002,35 +992,35 @@
 dependencies = [
  "autocfg",
  "hashbrown",
 ]
 
 [[package]]
 name = "instant"
-version = "0.1.10"
+version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bee0328b1209d157ef001c94dd85b4f8f64139adb0eac2659f4b08382b2f474d"
+checksum = "716d3d89f35ac6a34fd0eed635395f4c3b76fa889338a4632e5231a8684216bd"
 dependencies = [
  "cfg-if",
  "js-sys",
  "wasm-bindgen",
  "web-sys",
 ]
 
 [[package]]
 name = "itoa"
-version = "0.4.7"
+version = "0.4.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd25036021b0de88a0aff6b850051563c6516d0bf53f8638938edbb9de732736"
+checksum = "b71991ff56294aa922b450139ee08b3bfc70982c6b2c7562771375cf73542dd4"
 
 [[package]]
 name = "js-sys"
-version = "0.3.52"
+version = "0.3.55"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ce791b7ca6638aae45be056e068fc756d871eb3b3b10b8efa62d1c9cec616752"
+checksum = "7cc9ffccd38c451a86bf13657df244e9c3f37493cce8e5e21e940963777acc84"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "kv-log-macro"
 version = "1.0.7"
@@ -1044,23 +1034,23 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.98"
+version = "0.2.103"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "320cfe77175da3a483efed4bc0adc1968ca050b098ce4f2f1c13a56626128790"
+checksum = "dd8f7255a17a627354f321ef0055d63b898c6fb27eff628af4d1b66b7331edf6"
 
 [[package]]
 name = "lock_api"
-version = "0.4.4"
+version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0382880606dff6d15c9476c416d18690b72742aa7b605bb6dd6ec9030fbf07eb"
+checksum = "712a4d093c9976e24e7dbca41db895dabcbac38eb5f4045393d17a95bdfb1109"
 dependencies = [
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
 version = "0.4.14"
@@ -1069,17 +1059,17 @@
 dependencies = [
  "cfg-if",
  "value-bag",
 ]
 
 [[package]]
 name = "memchr"
-version = "2.4.0"
+version = "2.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b16bd47d9e329435e309c58469fe0791c2d0d1ba96ec0954152a5ae2b04387dc"
+checksum = "308cc39be01b73d0d18f82a0e7b2a3df85245f84af96fdddc5d202d27e47b86a"
 
 [[package]]
 name = "miniz_oxide"
 version = "0.4.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a92518e98c078586bc6c934028adcca4c92a53d6a958196de835170a01d84e4b"
 dependencies = [
@@ -1110,40 +1100,40 @@
 name = "once_cell"
 version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "692fcb63b64b1758029e0a96ee63e049ce8c5948587f2f7208df04625e5f6b56"
 
 [[package]]
 name = "openssl"
-version = "0.10.35"
+version = "0.10.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "549430950c79ae24e6d02e0b7404534ecf311d94cc9f861e9e4020187d13d885"
+checksum = "8d9facdb76fec0b73c406f125d44d86fdad818d66fef0531eec9233ca425ff4a"
 dependencies = [
  "bitflags",
  "cfg-if",
  "foreign-types",
  "libc",
  "once_cell",
  "openssl-sys",
 ]
 
 [[package]]
 name = "openssl-src"
-version = "111.15.0+1.1.1k"
+version = "111.16.0+1.1.1l"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1a5f6ae2ac04393b217ea9f700cd04fa9bf3d93fae2872069f3d15d908af70a"
+checksum = "7ab2173f69416cf3ec12debb5823d244127d23a9b127d5a5189aa97c5fa2859f"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "openssl-sys"
-version = "0.9.65"
+version = "0.9.67"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7a7907e3bfa08bb85105209cdfcb6c63d109f8f6c1ed6ca318fff5c1853fbc1d"
+checksum = "69df2d8dfc6ce3aaf44b40dec6f487d5a886516cf6879c49e98e0710f310a058"
 dependencies = [
  "autocfg",
  "cc",
  "libc",
  "openssl-src",
  "pkg-config",
  "vcpkg",
@@ -1153,28 +1143,28 @@
 name = "parking"
 version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "427c3892f9e783d91cc128285287e70a59e206ca452770ece88a76f7a3eddd72"
 
 [[package]]
 name = "parking_lot"
-version = "0.11.1"
+version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6d7744ac029df22dca6284efe4e898991d28e3085c706c972bcd7da4a27a15eb"
+checksum = "7d17b78036a60663b797adeaee46f5c9dfebb86948d1255007a1d6be0271ff99"
 dependencies = [
  "instant",
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.8.3"
+version = "0.8.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fa7a782938e745763fe6907fc6ba86946d72f49fe7e21de074e08128a99fb018"
+checksum = "d76e8e1493bcac0d2766c42737f34458f1c8c50c0d23bcb24ea953affb273216"
 dependencies = [
  "cfg-if",
  "instant",
  "libc",
  "redox_syscall",
  "smallvec",
  "winapi",
@@ -1245,17 +1235,17 @@
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
 [[package]]
 name = "pkg-config"
-version = "0.3.19"
+version = "0.3.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3831453b3449ceb48b6d9c7ad7c96d5ea673e9b470a1dc578c2ce6521230884c"
+checksum = "7c9b1041b4387893b91ee6746cddfc28516aff326a3519fb2adf820932c5e6cb"
 
 [[package]]
 name = "polling"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "92341d779fa34ea8437ef4d82d440d5e1ce3f3ff7f824aa64424cd481f9a1f25"
 dependencies = [
@@ -1276,17 +1266,17 @@
 name = "proc-macro-nested"
 version = "0.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bc881b2c22681370c6a780e47af9840ef841837bc98118431d4e1868bd0c1086"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.28"
+version = "1.0.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5c7ed8b8c7b886ea3ed7dde405212185f423ab44682667c8c6dd14aa1d9f6612"
+checksum = "b9f5105d4fdaab20335ca9565e106a5d9b82b6219b5ba735731124ac6711d23d"
 dependencies = [
  "unicode-xid",
 ]
 
 [[package]]
 name = "python3-sys"
 version = "0.6.0"
@@ -1304,17 +1294,17 @@
 checksum = "c3d0b9745dc2debf507c8422de05d7226cc1f0644216dfdfead988f9b1ab32a7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.2.9"
+version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5ab49abadf3f9e1c4bc499e8845e152ad87d2ad2d30371841171169e9d75feee"
+checksum = "8383f39639269cde97d255a32bdb68c047337295414940c68bdd30c2e13203ff"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "redox_users"
 version = "0.4.0"
@@ -1406,48 +1396,48 @@
 name = "send_wrapper"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "930c0acf610d3fdb5e2ab6213019aaa04e227ebe9547b0649ba599b16d788bd7"
 
 [[package]]
 name = "serde"
-version = "1.0.127"
+version = "1.0.130"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f03b9878abf6d14e6779d3f24f07b2cfa90352cfec4acc5aab8f1ac7f146fae8"
+checksum = "f12d06de37cf59146fbdecab66aa99f9fe4f78722e3607577a5375d66bd0c913"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.127"
+version = "1.0.130"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a024926d3432516606328597e0f224a51355a493b49fdd67e9209187cbe55ecc"
+checksum = "d7bc1a1ab1961464eae040d96713baa5a724a8152c1222492465b54322ec508b"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.66"
+version = "1.0.68"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "336b10da19a12ad094b59d870ebde26a45402e5b470add4b5fd03c5048a32127"
+checksum = "0f690853975602e1bfe1ccbf50504d67174e3bcf340f23b5ea9992e0587a52d8"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "signal-hook"
-version = "0.3.9"
+version = "0.3.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "470c5a6397076fae0094aaf06a08e6ba6f37acb77d3b1b91ea92b4d6c8650c39"
+checksum = "9c98891d737e271a2954825ef19e46bd16bdb98e2746f2eec4f7a4ef7946efd1"
 dependencies = [
  "libc",
  "signal-hook-registry",
 ]
 
 [[package]]
 name = "signal-hook-registry"
@@ -1456,41 +1446,41 @@
 checksum = "e51e73328dc4ac0c7ccbda3a494dfa03df1de2f46018127f60c693f2648455b0"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "siphasher"
-version = "0.3.6"
+version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "729a25c17d72b06c68cb47955d44fda88ad2d3e7d77e025663fdd69b93dd71a1"
+checksum = "533494a8f9b724d33625ab53c6c4800f7cc445895924a8ef649222dcb76e938b"
 
 [[package]]
 name = "slab"
-version = "0.4.3"
+version = "0.4.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f173ac3d1a7e3b28003f40de0b5ce7fe2710f9b9dc3fc38664cebee46b3b6527"
+checksum = "c307a32c1c5c437f38c7fd45d753050587732ba8628319fbdf12a7e289ccc590"
 
 [[package]]
 name = "smallvec"
-version = "1.6.1"
+version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fe0f37c9e8f3c5a4a66ad655a93c74daac4ad00c441533bf5c6e7990bb42604e"
+checksum = "1ecab6c735a6bb4139c0caafd0cc3635748bbb3acf4550e8138122099251f309"
 
 [[package]]
 name = "smol_str"
 version = "0.1.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b203e79e90905594272c1c97c7af701533d42adaab0beb3859018e477d54a3b0"
 
 [[package]]
 name = "socket2"
-version = "0.4.1"
+version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "765f090f0e423d2b55843402a07915add955e7d60657db13707a159727326cad"
+checksum = "5dc90fe6c7be1a323296982db1836d1ea9e47b6839496dde9a541bc496df3516"
 dependencies = [
  "libc",
  "winapi",
 ]
 
 [[package]]
 name = "static_assertions"
@@ -1523,17 +1513,17 @@
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "syn"
-version = "1.0.74"
+version = "1.0.77"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1873d832550d4588c3dbc20f01361ab00bfe741048f71e3fecf145a7cc18b29c"
+checksum = "5239bc68e0fef57495900cfea4e8dc75596d9a319d7e16b1e0a440d24e6fe0a0"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-xid",
 ]
 
 [[package]]
@@ -1543,59 +1533,59 @@
 checksum = "2dfed899f0eb03f32ee8c6a0aabdb8a7949659e3466561fc0adf54e26d88c5f4"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.26"
+version = "1.0.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "93119e4feac1cbe6c798c34d3a53ea0026b0b1de6a120deef895137c0529bfe2"
+checksum = "602eca064b2d83369e2b2f34b09c70b605402801927c65c11071ac911d299b88"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.26"
+version = "1.0.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "060d69a0afe7796bf42e9e2ff91f5ee691fb15c53d38b4b62a9a53eb23164745"
+checksum = "bad553cc2c78e8de258400763a647e80e6d1b31ee237275d756f6836d204494c"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "tokio"
-version = "1.9.0"
+version = "1.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4b7b349f11a7047e6d1276853e612d152f5e8a352c61917887cc2169e2366b4c"
+checksum = "c2c2416fdedca8443ae44b4527de1ea633af61d8f7169ffa6e72c5b53d24efcc"
 dependencies = [
  "autocfg",
  "pin-project-lite",
  "tokio-macros",
 ]
 
 [[package]]
 name = "tokio-macros"
-version = "1.3.0"
+version = "1.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "54473be61f4ebe4efd09cec9bd5d16fa51d70ea0192213d754d2d500457db110"
+checksum = "154794c8f499c2619acd19e839294703e9e32e7630ef5f46ea80d4ef0fbee5eb"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "tokio-util"
-version = "0.6.7"
+version = "0.6.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1caa0b0c8d94a049db56b5acf8cba99dc0623aab1b26d5b5f5e2d945846b3592"
+checksum = "08d3725d3efa29485e87311c5b699de63cde14b00ed4d256b8318aa30ca452cd"
 dependencies = [
  "bytes",
  "futures-core",
  "futures-io",
  "futures-sink",
  "log",
  "pin-project-lite",
@@ -1609,40 +1599,40 @@
 checksum = "a31142970826733df8241ef35dc040ef98c679ab14d7c3e54d827099b3acecaa"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "tracing"
-version = "0.1.26"
+version = "0.1.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "09adeb8c97449311ccd28a427f96fb563e7fd31aabf994189879d9da2394b89d"
+checksum = "84f96e095c0c82419687c20ddf5cb3eadb61f4e1405923c9dc8e53a1adacbda8"
 dependencies = [
  "cfg-if",
  "pin-project-lite",
  "tracing-attributes",
  "tracing-core",
 ]
 
 [[package]]
 name = "tracing-attributes"
-version = "0.1.15"
+version = "0.1.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c42e6fa53307c8a17e4ccd4dc81cf5ec38db9209f59b222210375b54ee40d1e2"
+checksum = "98863d0dd09fa59a1b79c6750ad80dbda6b75f4e71c437a6a1a8cb91a8bcbd77"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "tracing-core"
-version = "0.1.18"
+version = "0.1.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a9ff14f98b1a4b289c6248a023c1c2fa1491062964e9fed67ab29c4e4da4a052"
+checksum = "46125608c26121c81b0c6d693eab5a420e416da7e43c426d2e8f7df8da8a3acf"
 dependencies = [
  "lazy_static",
 ]
 
 [[package]]
 name = "tracing-futures"
 version = "0.2.5"
@@ -1703,83 +1693,83 @@
 name = "wasi"
 version = "0.10.2+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fd6fbd9a79829dd1ad0cc20627bf1ed606756a7f77edff7b66b7064f9cb327c6"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.75"
+version = "0.2.78"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b608ecc8f4198fe8680e2ed18eccab5f0cd4caaf3d83516fa5fb2e927fda2586"
+checksum = "632f73e236b219150ea279196e54e610f5dbafa5d61786303d4da54f84e47fce"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.75"
+version = "0.2.78"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "580aa3a91a63d23aac5b6b267e2d13cb4f363e31dce6c352fca4752ae12e479f"
+checksum = "a317bf8f9fba2476b4b2c85ef4c4af8ff39c3c7f0cdfeed4f82c34a880aa837b"
 dependencies = [
  "bumpalo",
  "lazy_static",
  "log",
  "proc-macro2",
  "quote",
  "syn",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
-version = "0.4.25"
+version = "0.4.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "16646b21c3add8e13fdb8f20172f8a28c3dbf62f45406bcff0233188226cfe0c"
+checksum = "8e8d7523cb1f2a4c96c1317ca690031b714a51cc14e05f712446691f413f5d39"
 dependencies = [
  "cfg-if",
  "js-sys",
  "wasm-bindgen",
  "web-sys",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.75"
+version = "0.2.78"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "171ebf0ed9e1458810dfcb31f2e766ad6b3a89dbda42d8901f2b268277e5f09c"
+checksum = "d56146e7c495528bf6587663bea13a8eb588d39b36b679d83972e1a2dbbdacf9"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.75"
+version = "0.2.78"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6c2657dd393f03aa2a659c25c6ae18a13a4048cebd220e147933ea837efc589f"
+checksum = "7803e0eea25835f8abdc585cd3021b3deb11543c6fe226dcd30b228857c5c5ab"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.75"
+version = "0.2.78"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2e0c4a743a309662d45f4ede961d7afa4ba4131a59a639f29b0069c3798bbcc2"
+checksum = "0237232789cf037d5480773fe568aac745bfe2afbc11a863e97901780a6b47cc"
 
 [[package]]
 name = "web-sys"
-version = "0.3.52"
+version = "0.3.55"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "01c70a82d842c9979078c772d4a1344685045f1a5628f677c2b2eab4dd7d2696"
+checksum = "38eb105f1c59d9eaa6b5cdc92b859d85b926e82cb2e0945cd0c9259faa6fe9fb"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "wepoll-ffi"
```

### Comparing `fluvio-0.9.6b2/LICENSE-APACHE` & `fluvio-0.9.6b3/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `fluvio-0.9.6b2/PKG-INFO` & `fluvio-0.9.6b3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluvio
-Version: 0.9.6b2
+Version: 0.9.6b3
 Summary: Python client library for Fluvio
 Home-page: https://www.fluvio.io/
 Author: Fluvio Contributors
 Author-email: team@fluvio.io
 License: APACHE
 Project-URL: Bug Reports, https://github.com/infinyon/fluvio-client-python/issues
 Project-URL: Source, https://github.com/infinyon/fluvio-client-python
@@ -34,22 +34,21 @@
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/infinyon/fluvio-client-python/blob/master/LICENSE-APACHE)
 [![PyPi](https://img.shields.io/pypi/v/fluvio.svg)](https://img.shields.io/pypi/v/fluvio.svg)
 
 ## Documentation
 
 Fluvio client uses [pdoc](https://github.com/mitmproxy/pdoc) to generate the client API [documentation](https://infinyon.github.io/fluvio-client-python/fluvio.html).
 
-## Non-prebuilt installation
+## Installation
 
-We publish to pypi with wheels but we don't publish for every os/architecture
-out there. To build from source, do:
 ```
-pip install git+https://github.com/infinyon/fluvio-client-python
+pip install fluvio
 ```
-You will need the rust compiler and maybe some operating system sources.
+
+This will get the wheel for the os/architecture of the installation system if available, otherwise it will try to build from source. If building from source, you will need the rust compiler and maybe some operating system sources.
 
 # Example Usage
 
 ## Producer
 ```python
 from fluvio import Fluvio
 fluvio = Fluvio.connect()
```

### Comparing `fluvio-0.9.6b2/README.md` & `fluvio-0.9.6b3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -10,22 +10,21 @@
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/infinyon/fluvio-client-python/blob/master/LICENSE-APACHE)
 [![PyPi](https://img.shields.io/pypi/v/fluvio.svg)](https://img.shields.io/pypi/v/fluvio.svg)
 
 ## Documentation
 
 Fluvio client uses [pdoc](https://github.com/mitmproxy/pdoc) to generate the client API [documentation](https://infinyon.github.io/fluvio-client-python/fluvio.html).
 
-## Non-prebuilt installation
+## Installation
 
-We publish to pypi with wheels but we don't publish for every os/architecture
-out there. To build from source, do:
 ```
-pip install git+https://github.com/infinyon/fluvio-client-python
+pip install fluvio
 ```
-You will need the rust compiler and maybe some operating system sources.
+
+This will get the wheel for the os/architecture of the installation system if available, otherwise it will try to build from source. If building from source, you will need the rust compiler and maybe some operating system sources.
 
 # Example Usage
 
 ## Producer
 ```python
 from fluvio import Fluvio
 fluvio = Fluvio.connect()
```

### Comparing `fluvio-0.9.6b2/build.rs` & `fluvio-0.9.6b3/build.rs`

 * *Files identical despite different names*

### Comparing `fluvio-0.9.6b2/fluvio/__init__.py` & `fluvio-0.9.6b3/fluvio/__init__.py`

 * *Files identical despite different names*

### Comparing `fluvio-0.9.6b2/fluvio.egg-info/PKG-INFO` & `fluvio-0.9.6b3/fluvio.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluvio
-Version: 0.9.6b2
+Version: 0.9.6b3
 Summary: Python client library for Fluvio
 Home-page: https://www.fluvio.io/
 Author: Fluvio Contributors
 Author-email: team@fluvio.io
 License: APACHE
 Project-URL: Bug Reports, https://github.com/infinyon/fluvio-client-python/issues
 Project-URL: Source, https://github.com/infinyon/fluvio-client-python
@@ -34,22 +34,21 @@
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/infinyon/fluvio-client-python/blob/master/LICENSE-APACHE)
 [![PyPi](https://img.shields.io/pypi/v/fluvio.svg)](https://img.shields.io/pypi/v/fluvio.svg)
 
 ## Documentation
 
 Fluvio client uses [pdoc](https://github.com/mitmproxy/pdoc) to generate the client API [documentation](https://infinyon.github.io/fluvio-client-python/fluvio.html).
 
-## Non-prebuilt installation
+## Installation
 
-We publish to pypi with wheels but we don't publish for every os/architecture
-out there. To build from source, do:
 ```
-pip install git+https://github.com/infinyon/fluvio-client-python
+pip install fluvio
 ```
-You will need the rust compiler and maybe some operating system sources.
+
+This will get the wheel for the os/architecture of the installation system if available, otherwise it will try to build from source. If building from source, you will need the rust compiler and maybe some operating system sources.
 
 # Example Usage
 
 ## Producer
 ```python
 from fluvio import Fluvio
 fluvio = Fluvio.connect()
```

### Comparing `fluvio-0.9.6b2/setup.py` & `fluvio-0.9.6b3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_namespace_packages
 from setuptools_rust import Binding, RustExtension, Strip
 
 setup(
     name='fluvio',
-    version="0.9.6-beta-2",
+    version="0.9.6-beta-3",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author = "Fluvio Contributors",
     description='Python client library for Fluvio',
     python_requires='>=3.6',
     url='https://www.fluvio.io/',
     keywords=['fluvio', 'streaming', 'stream'],
```

### Comparing `fluvio-0.9.6b2/src/glue.rs.in` & `fluvio-0.9.6b3/src/glue.rs.in`

 * *Files identical despite different names*

