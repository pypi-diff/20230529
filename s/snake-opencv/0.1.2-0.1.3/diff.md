# Comparing `tmp/snake_opencv-0.1.2.tar.gz` & `tmp/snake_opencv-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snake_opencv-0.1.2.tar", max compression
+gzip compressed data, was "snake_opencv-0.1.3.tar", max compression
```

## Comparing `snake_opencv-0.1.2.tar` & `snake_opencv-0.1.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    11358 2023-05-25 16:59:10.585531 snake_opencv-0.1.2/LICENSE
--rw-r--r--   0        0        0      460 2023-05-25 16:59:10.585668 snake_opencv-0.1.2/README.md
--rw-r--r--   0        0        0      686 2023-05-25 16:59:35.011367 snake_opencv-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      161 2023-05-25 16:59:10.586673 snake_opencv-0.1.2/snake_opencv/__init__.py
--rw-r--r--   0        0        0       44 2023-05-25 16:59:10.586848 snake_opencv-0.1.2/snake_opencv/core/__init__.py
--rw-r--r--   0        0        0    12427 2023-05-25 16:59:10.587037 snake_opencv-0.1.2/snake_opencv/core/binding.py
--rw-r--r--   0        0        0    24344 2023-05-25 16:59:10.587329 snake_opencv-0.1.2/snake_opencv/core/const.py
--rw-r--r--   0        0        0       44 2023-05-25 16:59:10.587539 snake_opencv-0.1.2/snake_opencv/dnn/__init__.py
--rw-r--r--   0        0        0     3607 2023-05-25 16:59:10.587684 snake_opencv-0.1.2/snake_opencv/dnn/binding.py
--rw-r--r--   0        0        0     1379 2023-05-25 16:59:10.587804 snake_opencv-0.1.2/snake_opencv/dnn/const.py
--rw-r--r--   0        0        0       44 2023-05-25 16:59:10.587974 snake_opencv-0.1.2/snake_opencv/highgui/__init__.py
--rw-r--r--   0        0        0     4949 2023-05-25 16:59:10.588127 snake_opencv-0.1.2/snake_opencv/highgui/binding.py
--rw-r--r--   0        0        0     2912 2023-05-25 16:59:10.588256 snake_opencv-0.1.2/snake_opencv/highgui/const.py
--rw-r--r--   0        0        0       44 2023-05-25 16:59:10.588441 snake_opencv-0.1.2/snake_opencv/imgcodecs/__init__.py
--rw-r--r--   0        0        0     5211 2023-05-25 16:59:10.588616 snake_opencv-0.1.2/snake_opencv/imgcodecs/binding.py
--rw-r--r--   0        0        0     1496 2023-05-25 16:59:10.588731 snake_opencv-0.1.2/snake_opencv/imgcodecs/const.py
--rw-r--r--   0        0        0       44 2023-05-25 16:59:10.588907 snake_opencv-0.1.2/snake_opencv/imgproc/__init__.py
--rw-r--r--   0        0        0    37011 2023-05-25 17:52:22.840887 snake_opencv-0.1.2/snake_opencv/imgproc/binding.py
--rw-r--r--   0        0        0    35343 2023-05-25 16:59:10.589626 snake_opencv-0.1.2/snake_opencv/imgproc/const.py
--rw-r--r--   0        0        0       44 2023-05-25 16:59:10.589821 snake_opencv-0.1.2/snake_opencv/photo/__init__.py
--rw-r--r--   0        0        0     3620 2023-05-25 16:59:10.589960 snake_opencv-0.1.2/snake_opencv/photo/binding.py
--rw-r--r--   0        0        0      854 2023-05-25 16:59:10.590090 snake_opencv-0.1.2/snake_opencv/photo/const.py
--rw-r--r--   0        0        0        0 2023-05-25 17:50:01.610033 snake_opencv-0.1.2/snake_opencv/py.typed
--rw-r--r--   0        0        0       44 2023-05-25 16:59:10.590279 snake_opencv-0.1.2/snake_opencv/videoio/__init__.py
--rw-r--r--   0        0        0     7240 2023-05-25 16:59:10.590449 snake_opencv-0.1.2/snake_opencv/videoio/binding.py
--rw-r--r--   0        0        0    29523 2023-05-25 16:59:10.590750 snake_opencv-0.1.2/snake_opencv/videoio/const.py
--rw-r--r--   0        0        0     1194 1970-01-01 00:00:00.000000 snake_opencv-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-05-25 16:59:10.585531 snake_opencv-0.1.3/LICENSE
+-rw-r--r--   0        0        0      346 2023-05-28 23:17:20.546476 snake_opencv-0.1.3/README.md
+-rw-r--r--   0        0        0      686 2023-05-25 18:09:05.544570 snake_opencv-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      161 2023-05-25 16:59:10.586673 snake_opencv-0.1.3/snake_opencv/__init__.py
+-rw-r--r--   0        0        0       44 2023-05-25 16:59:10.586848 snake_opencv-0.1.3/snake_opencv/core/__init__.py
+-rw-r--r--   0        0        0    12427 2023-05-25 16:59:10.587037 snake_opencv-0.1.3/snake_opencv/core/binding.py
+-rw-r--r--   0        0        0    24344 2023-05-25 16:59:10.587329 snake_opencv-0.1.3/snake_opencv/core/const.py
+-rw-r--r--   0        0        0       44 2023-05-25 16:59:10.587539 snake_opencv-0.1.3/snake_opencv/dnn/__init__.py
+-rw-r--r--   0        0        0     3649 2023-05-28 23:04:14.326704 snake_opencv-0.1.3/snake_opencv/dnn/binding.py
+-rw-r--r--   0        0        0     1379 2023-05-25 16:59:10.587804 snake_opencv-0.1.3/snake_opencv/dnn/const.py
+-rw-r--r--   0        0        0       44 2023-05-25 16:59:10.587974 snake_opencv-0.1.3/snake_opencv/highgui/__init__.py
+-rw-r--r--   0        0        0     4949 2023-05-25 16:59:10.588127 snake_opencv-0.1.3/snake_opencv/highgui/binding.py
+-rw-r--r--   0        0        0     2912 2023-05-25 16:59:10.588256 snake_opencv-0.1.3/snake_opencv/highgui/const.py
+-rw-r--r--   0        0        0       44 2023-05-25 16:59:10.588441 snake_opencv-0.1.3/snake_opencv/imgcodecs/__init__.py
+-rw-r--r--   0        0        0     5211 2023-05-25 16:59:10.588616 snake_opencv-0.1.3/snake_opencv/imgcodecs/binding.py
+-rw-r--r--   0        0        0     1496 2023-05-25 16:59:10.588731 snake_opencv-0.1.3/snake_opencv/imgcodecs/const.py
+-rw-r--r--   0        0        0       44 2023-05-25 16:59:10.588907 snake_opencv-0.1.3/snake_opencv/imgproc/__init__.py
+-rw-r--r--   0        0        0    42748 2023-05-28 23:54:03.339666 snake_opencv-0.1.3/snake_opencv/imgproc/binding.py
+-rw-r--r--   0        0        0    35343 2023-05-25 16:59:10.589626 snake_opencv-0.1.3/snake_opencv/imgproc/const.py
+-rw-r--r--   0        0        0       44 2023-05-25 16:59:10.589821 snake_opencv-0.1.3/snake_opencv/photo/__init__.py
+-rw-r--r--   0        0        0     3620 2023-05-25 16:59:10.589960 snake_opencv-0.1.3/snake_opencv/photo/binding.py
+-rw-r--r--   0        0        0      854 2023-05-25 16:59:10.590090 snake_opencv-0.1.3/snake_opencv/photo/const.py
+-rw-r--r--   0        0        0        0 2023-05-25 17:50:01.610033 snake_opencv-0.1.3/snake_opencv/py.typed
+-rw-r--r--   0        0        0       44 2023-05-25 16:59:10.590279 snake_opencv-0.1.3/snake_opencv/videoio/__init__.py
+-rw-r--r--   0        0        0     7320 2023-05-28 22:54:24.723745 snake_opencv-0.1.3/snake_opencv/videoio/binding.py
+-rw-r--r--   0        0        0    29523 2023-05-25 16:59:10.590750 snake_opencv-0.1.3/snake_opencv/videoio/const.py
+-rw-r--r--   0        0        0     1080 1970-01-01 00:00:00.000000 snake_opencv-0.1.3/PKG-INFO
```

### Comparing `snake_opencv-0.1.2/LICENSE` & `snake_opencv-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.2/pyproject.toml` & `snake_opencv-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "snake-opencv"
-version = "0.1.2"
+version = "0.1.3"
 repository = "https://github.com/cospectrum/snake-opencv"
 description = "Snake case opencv with type annotations"
 license = "Apache-2.0"
 authors = ["cospectrum <severinalexeyv@gmail.com>"]
 readme = "README.md"
 packages = [{include = "snake_opencv"}]
```

### Comparing `snake_opencv-0.1.2/snake_opencv/core/binding.py` & `snake_opencv-0.1.3/snake_opencv/core/binding.py`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.2/snake_opencv/core/const.py` & `snake_opencv-0.1.3/snake_opencv/core/const.py`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.2/snake_opencv/dnn/binding.py` & `snake_opencv-0.1.3/snake_opencv/dnn/binding.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,18 +9,22 @@
 
 __all__ = [
     'blob_from_image',
     'blob_from_images',
 ]
 
 
+W = int
+H = int
+
+
 def blob_from_image(
     image: np.ndarray,
     scalefactor: float = 1.0,
-    size: Optional[Tuple[int, int]] = None,
+    size: Optional[Tuple[W, H]] = None,
     mean: Optional[Tuple[float, ...]] = None,
     swap_rb: bool = False,
     crop: bool = False,
     ddepth: int = CV_32F,
 ) -> np.ndarray:
     """Creates 4-dimensional blob from image. Optionally resizes and crops
     image from center, subtract mean values, scales values by scalefactor,
@@ -46,29 +50,29 @@
             corresponding dimension in size and another one is equal or
             larger. Then, crop from the center is performed. If crop is false,
             direct resize without cropping and preserving aspect ratio is
             performed.
 
     Returns: 4-dimensional np.array with NCHW dimensions order.
     """
-    return cv2.dnn.blobFromImage(
+    return cv2.dnn.blobFromImage(  # type: ignore
         image,
         scalefactor,
         size,
         mean=mean,
         swapRB=swap_rb,
         crop=crop,
         ddepth=ddepth,
     )
 
 
 def blob_from_images(
     images: List[np.ndarray],
     scalefactor: float = 1.0,
-    size: Optional[Tuple[int, int]] = None,
+    size: Optional[Tuple[W, H]] = None,
     mean: Optional[Tuple[float, ...]] = None,
     swap_rb: bool = False,
     crop: bool = False,
     ddepth: int = CV_32F,
 ) -> np.ndarray:
     """Creates 4-dimensional blob from image. Optionally resizes and crops
     image from center, subtract mean values, scales values by scalefactor,
@@ -94,15 +98,15 @@
             corresponding dimension in size and another one is equal or
             larger. Then, crop from the center is performed. If crop is false,
             direct resize without cropping and preserving aspect ratio is
             performed.
 
     Returns: 4-dimensional np.array with NCHW dimensions order.
     """
-    return cv2.dnn.blobFromImages(
+    return cv2.dnn.blobFromImages(  # type: ignore
         images,
         scalefactor,
         size,
         mean=mean,
         swapRB=swap_rb,
         crop=crop,
         ddepth=ddepth,
```

### Comparing `snake_opencv-0.1.2/snake_opencv/dnn/const.py` & `snake_opencv-0.1.3/snake_opencv/dnn/const.py`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.2/snake_opencv/highgui/binding.py` & `snake_opencv-0.1.3/snake_opencv/highgui/binding.py`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.2/snake_opencv/highgui/const.py` & `snake_opencv-0.1.3/snake_opencv/highgui/const.py`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.2/snake_opencv/imgcodecs/binding.py` & `snake_opencv-0.1.3/snake_opencv/imgcodecs/binding.py`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.2/snake_opencv/imgcodecs/const.py` & `snake_opencv-0.1.3/snake_opencv/imgcodecs/const.py`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.2/snake_opencv/imgproc/binding.py` & `snake_opencv-0.1.3/snake_opencv/imgproc/binding.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,14 +36,18 @@
     'laplacian',
     'threshold',
     'connected_components_with_stats',
     'connected_components',
     'match_template',
     'warp_affine',
     'get_affine_transform',
+    'get_rotation_matrix_2d',
+    'median_blur',
+    'blur',
+    'bilateral_filter',
 ]
 
 
 LineType = Literal[-1, 4, 8, 16]
 
 
 Width = int
@@ -1024,7 +1028,167 @@
     Args:
         src: Coordinates of triangle vertices in the source image.
         dst:
             Coordinates of the corresponding triangle vertices in the
             destination image.
     """
     return cv2.getAffineTransform(src, dst=dst)  # type: ignore
+
+
+Point2f = Tuple[float, float]
+
+
+def get_rotation_matrix_2d(
+    center: Point2f,
+    angle: float,
+    scale: float,
+) -> np.ndarray:
+    """Calculates an affine matrix of 2D rotation.
+
+    The function calculates the following matrix:
+
+        [ α   β   (1 − α)⋅𝚌𝚎𝚗𝚝𝚎𝚛.𝚡 − β⋅𝚌𝚎𝚗𝚝𝚎𝚛.𝚢]
+        [-β   α   β⋅𝚌𝚎𝚗𝚝𝚎𝚛.𝚡 + (1 − α)⋅𝚌𝚎𝚗𝚝𝚎𝚛.𝚢]
+
+    where
+        α = 𝚜𝚌𝚊𝚕𝚎⋅cos(𝚊𝚗𝚐𝚕𝚎),
+        β = 𝚜𝚌𝚊𝚕𝚎⋅sin(𝚊𝚗𝚐𝚕𝚎)
+
+    The transformation maps the rotation center to itself. If this is not the
+    target, adjust the shift.
+
+    Args:
+        center: Center of the rotation in the source image.
+        angle:
+            Rotation angle in degrees. Positive values mean counter-clockwise
+            rotation (the coordinate origin is assumed to be the top-left
+            corner).
+        scale: Isotropic scale factor.
+    """
+    return cv2.getRotationMatrix2D(center, angle, scale=scale)  # type: ignore
+
+
+def median_blur(
+    src: np.ndarray,
+    ksize: int,
+    dst: Optional[np.ndarray] = None,
+) -> np.ndarray:
+    """Blurs an image using the median filter.
+
+    The function smoothes an image using the median filter with the
+    𝚔𝚜𝚒𝚣𝚎×𝚔𝚜𝚒𝚣𝚎 aperture. Each channel of a multi-channel image is processed
+    independently. In-place operation is supported.
+
+    Args:
+        src:
+            input 1-, 3-, or 4-channel image; when ksize is 3 or 5, the image
+            depth should be CV_8U, CV_16U, or CV_32F, for larger aperture
+            sizes, it can only be CV_8U.
+        dst: destination array of the same size and type as src.
+        ksize:
+            aperture linear size; it must be odd and greater than 1, for
+            example: 3, 5, 7 ...
+    """
+    return cv2.medianBlur(src, ksize=ksize, dst=dst)  # type: ignore
+
+
+def blur(
+    src: np.ndarray,
+    ksize: Tuple[int, int],
+    dst: Optional[np.ndarray] = None,
+    anchor: Tuple[int, int] = (-1, -1),
+    border_type: int = BORDER_DEFAULT,
+) -> np.ndarray:
+    """Blurs an image using the normalized box filter.
+
+    The function smooths an image using the kernel:
+
+        K = (1 / (ksize.width * ksize.height)) * J,
+
+    where
+
+        J = [1 1 1 ... 1 1]
+            [1 1 1 ... 1 1]
+            [...          ]
+            [1 1 1 ... 1 1]
+
+    The call blur(src, dst, ksize, anchor, borderType) is equivalent to
+    boxFilter(src, dst, src.type(), ksize, anchor, true, borderType).
+
+    Args:
+        src:
+            input image; it can have any number of channels, which are
+            processed independently, but the depth should be CV_8U, CV_16U,
+            CV_16S, CV_32F or CV_64F.
+        dst: output image of the same size and type as src.
+        ksize: blurring kernel size.
+        anchor:
+            anchor point; default value Point(-1,-1) means that the anchor is
+            at the kernel center.
+        border_type:
+            border mode used to extrapolate pixels outside of the image, see
+            BorderTypes. BORDER_WRAP is not supported.
+    """
+    return cv2.blur(  # type: ignore
+        src,
+        ksize,
+        dst=dst,
+        anchor=anchor,
+        borderType=border_type,
+    )
+
+
+def bilateral_filter(
+    src: np.ndarray,
+    d: int,
+    sigma_color: float,
+    sigma_space: float,
+    dst: Optional[np.ndarray] = None,
+    border_type: int = BORDER_DEFAULT,
+) -> np.ndarray:
+    """Applies the bilateral filter to an image.
+
+    The function applies bilateral filtering to the input image, as described
+    in http://www.dai.ed.ac.uk/CVonline/LOCAL_COPIES/MANDUCHI1/Bilateral_Filtering.html
+    bilateralFilter can reduce unwanted noise very well while keeping edges
+    fairly sharp. However, it is very slow compared to most filters.
+
+    Sigma values: For simplicity, you can set the 2 sigma values to be the
+    same. If they are small (< 10), the filter will not have much effect,
+    whereas if they are large (> 150), they will have a very strong effect,
+    making the image look "cartoonish".
+
+    Filter size: Large filters (d > 5) are very slow, so it is recommended to
+    use d=5 for real-time applications, and perhaps d=9 for offline
+    applications that need heavy noise filtering.
+
+    This filter does not work inplace.
+
+    Args:
+        src: Source 8-bit or floating-point, 1-channel or 3-channel image.
+        dst: Destination image of the same size and type as src.
+        d:
+            Diameter of each pixel neighborhood that is used during filtering.
+            If it is non-positive, it is computed from sigmaSpace.
+        sigma_color:
+            Filter sigma in the color space. A larger value of the parameter
+            means that farther colors within the pixel neighborhood
+            (see sigmaSpace) will be mixed together, resulting in larger areas
+            of semi-equal color.
+        sigma_space:
+            Filter sigma in the coordinate space. A larger value of the
+            parameter means that farther pixels will influence each other as
+            long as their colors are close enough (see sigmaColor). When d > 0,
+            it specifies the neighborhood size regardless of sigmaSpace.
+            Otherwise, d is proportional to sigmaSpace.
+        border_type:
+            border mode used to extrapolate pixels outside of the image, see
+            BorderTypes
+    """
+    return cv2.bilateralFilter(  # type: ignore
+        src,
+        d=d,
+        sigmaColor=sigma_color,
+        sigmaSpace=sigma_space,
+        dst=dst,
+        borderType=border_type,
+    )
```

### Comparing `snake_opencv-0.1.2/snake_opencv/imgproc/const.py` & `snake_opencv-0.1.3/snake_opencv/imgproc/const.py`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.2/snake_opencv/photo/binding.py` & `snake_opencv-0.1.3/snake_opencv/photo/binding.py`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.2/snake_opencv/photo/const.py` & `snake_opencv-0.1.3/snake_opencv/photo/const.py`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.2/snake_opencv/videoio/binding.py` & `snake_opencv-0.1.3/snake_opencv/videoio/binding.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 __all__ = [
     'VideoCapture',
     'VideoWriter',
 ]
 
 
 class VideoCapture:
-    _reader: cv2.VideoCapture
+    _reader: cv2.VideoCapture  # type: ignore
 
     def __init__(
         self,
         filename: Union[str, int],
         api_preference: int = CAP_ANY,
         params: Optional[List[int]] = None,
     ) -> None:
@@ -31,15 +31,15 @@
         video capturing with API Preference and parameters.
 
         This is an overloaded member function, provided for convenience. It
         differs from the above function only in what argument(s) it accepts.
         The params parameter allows to specify extra parameters encoded as
         pairs (paramId_1, paramValue_1, paramId_2, paramValue_2, ...).
         """
-        self._reader = cv2.VideoCapture(filename, api_preference, params)
+        self._reader = cv2.VideoCapture(filename, api_preference, params)  # type: ignore
 
     def is_opened(self) -> bool:
         """Returns True if video capturing has been initialized already."""
         return self._reader.isOpened()
 
     def read(self) -> Tuple[bool, np.ndarray]:
         """Grabs, decodes and returns the next video frame."""
@@ -120,15 +120,15 @@
 
 
 Width = int
 Height = int
 
 
 class VideoWriter:
-    _writer: cv2.VideoWriter
+    _writer: cv2.VideoWriter  # type: ignore
 
     def __init__(
         self,
         filename: str,
         fourcc: int,
         fps: float,
         frame_size: Tuple[Width, Height],
@@ -146,15 +146,15 @@
                 FFMPEG backend with MP4 container natively uses other values
                 as fourcc code: see http://mp4ra.org/#/codecs, so you may
                 receive a warning message from OpenCV about fourcc code
                 conversion.
             fps: Framerate of the created video stream.
             frame_size: Size (width, height) of the video frames
         """
-        self._writer = cv2.VideoWriter(
+        self._writer = cv2.VideoWriter(  # type: ignore
             filename,
             fourcc,
             fps,
             frame_size,
         )
 
     def write(self, image: np.ndarray) -> None:
@@ -183,15 +183,15 @@
         """Concatenates 4 chars to a fourcc code.
 
         This static method constructs the fourcc code of the codec to be used
         in the VideoWriter constructor.
 
         Returns: a fourcc code
         """
-        return cv2.VideoWriter.fourcc(c1, c2, c3, c4)
+        return cv2.VideoWriter.fourcc(c1, c2, c3, c4)  # type: ignore
 
     def get_backend_name(self) -> str:
         """Returns used backend API name.
         Note:
             Stream should be opened.
         """
         return self._writer.getBackendName()
```

### Comparing `snake_opencv-0.1.2/snake_opencv/videoio/const.py` & `snake_opencv-0.1.3/snake_opencv/videoio/const.py`

 * *Files identical despite different names*

### Comparing `snake_opencv-0.1.2/PKG-INFO` & `snake_opencv-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snake-opencv
-Version: 0.1.2
+Version: 0.1.3
 Summary: Snake case opencv with type annotations
 Home-page: https://github.com/cospectrum/snake-opencv
 License: Apache-2.0
 Author: cospectrum
 Author-email: severinalexeyv@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -20,29 +20,23 @@
 # Snake-OpenCV
 Snake case OpenCV with type annotations for Python.
 
 Note: still in early development
 
 ## Install
 
-Stable version
 ```sh
 pip install snake-opencv
 ```
 
-Latest version from git
-```sh
-pip install git+https://github.com/cospectrum/snake-opencv.git
-```
-
 ## Usage
 ```py
 import snake_opencv as cv
 
-path = '...'
+path = '..'
 image = cv.imread(path)
 assert image is not None
 gray_image = cv.cvt_color(image, cv.COLOR_BGR2GRAY)
 
 cv.imshow(window_name, gray_image) 
 ```
```

