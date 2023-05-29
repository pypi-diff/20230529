# Comparing `tmp/aksharify-2.5.3.tar.gz` & `tmp/aksharify-2.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aksharify-2.5.3.tar", last modified: Sun May 28 07:13:50 2023, max compression
+gzip compressed data, was "aksharify-2.5.5.tar", max compression
```

## Comparing `aksharify-2.5.3.tar` & `aksharify-2.5.5.tar`

### file list

```diff
@@ -1,15 +1,5 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 07:13:50.484324 aksharify-2.5.3/
--rw-rw-rw-   0        0        0     1094 2023-05-26 09:00:50.000000 aksharify-2.5.3/LICENSE.md
--rw-rw-rw-   0        0        0     4874 2023-05-28 07:13:50.479965 aksharify-2.5.3/PKG-INFO
--rw-rw-rw-   0        0        0     4358 2023-05-26 09:00:50.000000 aksharify-2.5.3/README.md
--rw-rw-rw-   0        0        0      634 2023-05-28 07:12:56.000000 aksharify-2.5.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-28 07:13:50.484324 aksharify-2.5.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-28 07:13:50.436069 aksharify-2.5.3/src/
--rw-rw-rw-   0        0        0        0 2023-05-26 09:00:50.000000 aksharify-2.5.3/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 07:13:50.475727 aksharify-2.5.3/src/aksharify.egg-info/
--rw-rw-rw-   0        0        0     4874 2023-05-28 07:13:50.000000 aksharify-2.5.3/src/aksharify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-05-28 07:13:50.000000 aksharify-2.5.3/src/aksharify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 07:13:50.000000 aksharify-2.5.3/src/aksharify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-28 07:13:50.000000 aksharify-2.5.3/src/aksharify.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-28 07:13:50.000000 aksharify-2.5.3/src/aksharify.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5573 2023-05-28 07:12:30.000000 aksharify-2.5.3/src/aksharify.py
+-rw-r--r--   0        0        0       24 2023-05-29 15:23:03.528860 aksharify-2.5.5/aksharify/__init__.py
+-rw-r--r--   0        0        0     6793 2023-05-29 15:26:23.653035 aksharify-2.5.5/aksharify/aksharify.py
+-rw-r--r--   0        0        0      901 2023-05-29 15:55:21.776703 aksharify-2.5.5/pyproject.toml
+-rw-r--r--   0        0        0     4358 2023-05-29 15:59:45.530987 aksharify-2.5.5/README.md
+-rw-r--r--   0        0        0     5132 1970-01-01 00:00:00.000000 aksharify-2.5.5/PKG-INFO
```

### Comparing `aksharify-2.5.3/PKG-INFO` & `aksharify-2.5.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: aksharify
-Version: 2.5.3
-Summary: Ascii art module
-Author-email: Prime Patel <primespatel@gmail.com>
-Project-URL: Homepage, https://github.com/primepatel/aksharify
-Project-URL: Bug Tracker, https://github.com/primepatel/aksharify/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 <a name="readme-top"></a>
 
 # __Aksharify__
 
 [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url]
 [![Stargazers][stars-shield]][stars-url]
@@ -130,8 +116,8 @@
 [stars-url]: https://github.com/primepatel/Aksharify/stargazers
 [issues-shield]: https://img.shields.io/github/issues/primepatel/Aksharify.svg?style=for-the-badge
 [issues-url]: https://github.com/primepatel/Aksharify/issues
 [license-shield]: https://img.shields.io/github/license/primepatel/Aksharify.svg?style=for-the-badge
 [license-url]: https://github.com/primepatel/Aksharify/blob/master/LICENSE.txt
 [linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
 [linkedin-url]: https://linkedin.com/in/primepatel
-[Downloads-shield]: https://img.shields.io/pypi/dm/aksharify?style=for-the-badge
+[Downloads-shield]: https://img.shields.io/pypi/dm/aksharify?style=for-the-badge
```

#### html2text {}

```diff
@@ -1,20 +1,12 @@
-Metadata-Version: 2.1 Name: aksharify Version: 2.5.3 Summary: Ascii art module
-Author-email: Prime Patel
-gmail.com> Project-URL: Homepage, https://github.com/primepatel/aksharify
-Project-URL: Bug Tracker, https://github.com/primepatel/aksharify/issues
-Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
-Approved :: MIT License Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
-LICENSE.md  # __Aksharify__ [![Contributors][contributors-shield]]
-[contributors-url] [![Forks][forks-shield]][forks-url] [![Stargazers][stars-
-shield]][stars-url] [![Issues][issues-shield]][issues-url] [![MIT License]
-[license-shield]][license-url] [![LinkedIn][linkedin-shield]][linkedin-url] [!
-[PyPI - Downloads][Downloads-shield]](https://pypistats.org/packages/aksharify)
-
+ # __Aksharify__ [![Contributors][contributors-shield]][contributors-url] [!
+[Forks][forks-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [!
+[Issues][issues-shield]][issues-url] [![MIT License][license-shield]][license-
+url] [![LinkedIn][linkedin-shield]][linkedin-url] [![PyPI - Downloads]
+[Downloads-shield]](https://pypistats.org/packages/aksharify)
  ## About the module The inspiration for this module came from a Numberphile
 video called "The Trinity Hall Prime," which I first saw in high school days.
 It motivated me to explore the possibilities of such a prime number. I created
 a Python module that uses a predetermined character set to turn photos into
 ASCII art. It manipulates images using the PIL package, transforming them to
 grayscale before mapping pixel values to ASCII letters. Users can change the
 character set to get different effects.  ## Getting Started Before we begin,
```

### Comparing `aksharify-2.5.3/src/aksharify.egg-info/PKG-INFO` & `aksharify-2.5.5/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,137 +1,146 @@
-Metadata-Version: 2.1
-Name: aksharify
-Version: 2.5.3
-Summary: Ascii art module
-Author-email: Prime Patel <primespatel@gmail.com>
-Project-URL: Homepage, https://github.com/primepatel/aksharify
-Project-URL: Bug Tracker, https://github.com/primepatel/aksharify/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
-<a name="readme-top"></a>
-
-# __Aksharify__
-
-[![Contributors][contributors-shield]][contributors-url]
-[![Forks][forks-shield]][forks-url]
-[![Stargazers][stars-shield]][stars-url]
-[![Issues][issues-shield]][issues-url]
-[![MIT License][license-shield]][license-url]
-[![LinkedIn][linkedin-shield]][linkedin-url]
-[![PyPI - Downloads][Downloads-shield]](https://pypistats.org/packages/aksharify)
-
-<br />
-
-<!-- ABOUT THE PROJECT -->
-## About the module
-
-The inspiration for this module came from a Numberphile video called "The Trinity Hall Prime," which I first saw in high school days. It motivated me to explore the possibilities of such a prime number. I created a Python module that uses a predetermined character set to turn photos into ASCII art. It manipulates images using the PIL package, transforming them to grayscale before mapping pixel values to ASCII letters. Users can change the character set to get different effects.
-
-<!-- GETTING STARTED -->
-## Getting Started
-
-Before we begin, make sure you have one of recent versions of Python installed on your computer.
-
-### Installation
-
-```sh
-python -m pip install aksharify
-```
-
-## Usage
-
-```python
-from aksharify import TextArt
-
-# input image file
-art = TextArt("Julia.png")
-
-# see image
-art.image.show()
-
-# set dimension of output text
-art.set_dim(80)
-
-# genetate text
-art.asciify()
-
-# output into .txt file
-art.text_output("output")
-
-# generate colored text using html
-art.colorify()
-
-# output into .html file
-art.color_output("output")
-```
-
-_For examples from user community, please refer to the [primepatel.github.io/aksharify](https://primepatel.github.io/aksharify)_
-
-
-<!-- ROADMAP -->
-## Roadmap
-
-- [x] NumberiFy
-- [-] Predifined order of characters
-- [-] Getting images from URL
-- [-] EmojiFy
-
-See the [open issues](https://github.com/github_username/repo_name/issues) for a full list of proposed features (and known issues).
-
-<!-- CONTRIBUTING -->
-## Contributing
-
-Contributions are what make the open source community such a wonderful place to learn, be inspired, and create. Any contributions you make are `appreciated greatly`.
-
-If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
-Don't forget to give the project a star! Thanks again!
-
-1. Fork the Project
-2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
-3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
-4. Push to the Branch (`git push origin feature/AmazingFeature`)
-5. Open a Pull Request
-
-<!-- LICENSE -->
-## License
-
-Distributed under the MIT License. See `LICENSE.txt` for more information.
-
-<!-- CONTACT -->
-## Contact
-
-Prime Patel - [@primepatel](https://twitter.com/primespatel) - primespatel@gmail.com
-
-Project Link: [https://github.com/primepatel/aksharify](https://github.com/primepatel/aksharify)
-
-
-<!-- ACKNOWLEDGMENTS -->
-<!-- ## Acknowledgments
-
-* []()
-* []()
-* []() -->
-
-<p align="right">(<a href="#readme-top">back to top</a>)</p>
-
-
-
-<!-- MARKDOWN LINKS & IMAGES -->
-<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
-[contributors-shield]: https://img.shields.io/github/contributors/primepatel/Aksharify.svg?style=for-the-badge
-[contributors-url]: https://github.com/primepatel/Aksharify/graphs/contributors
-[forks-shield]: https://img.shields.io/github/forks/primepatel/Aksharify.svg?style=for-the-badge
-[forks-url]: https://github.com/primepatel/Aksharify/network/members
-[stars-shield]: https://img.shields.io/github/stars/primepatel/Aksharify.svg?style=for-the-badge
-[stars-url]: https://github.com/primepatel/Aksharify/stargazers
-[issues-shield]: https://img.shields.io/github/issues/primepatel/Aksharify.svg?style=for-the-badge
-[issues-url]: https://github.com/primepatel/Aksharify/issues
-[license-shield]: https://img.shields.io/github/license/primepatel/Aksharify.svg?style=for-the-badge
-[license-url]: https://github.com/primepatel/Aksharify/blob/master/LICENSE.txt
-[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
-[linkedin-url]: https://linkedin.com/in/primepatel
-[Downloads-shield]: https://img.shields.io/pypi/dm/aksharify?style=for-the-badge
+Metadata-Version: 2.1
+Name: aksharify
+Version: 2.5.5
+Summary: Python Ascii + Emoji Art Module
+Home-page: https://primepatel.github.io/aksharify-docs/
+License: MIT
+Keywords: Ascii Art,Emoji Art,Prime Patel,primepatel
+Author: Prime Patel
+Author-email: primespatel@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: pillow (>=9.5.0,<10.0.0)
+Project-URL: Repository, https://github.com/primepatel/aksharify
+Description-Content-Type: text/markdown
+
+<a name="readme-top"></a>
+
+# __Aksharify__
+
+[![Contributors][contributors-shield]][contributors-url]
+[![Forks][forks-shield]][forks-url]
+[![Stargazers][stars-shield]][stars-url]
+[![Issues][issues-shield]][issues-url]
+[![MIT License][license-shield]][license-url]
+[![LinkedIn][linkedin-shield]][linkedin-url]
+[![PyPI - Downloads][Downloads-shield]](https://pypistats.org/packages/aksharify)
+
+<br />
+
+<!-- ABOUT THE PROJECT -->
+## About the module
+
+The inspiration for this module came from a Numberphile video called "The Trinity Hall Prime," which I first saw in high school days. It motivated me to explore the possibilities of such a prime number. I created a Python module that uses a predetermined character set to turn photos into ASCII art. It manipulates images using the PIL package, transforming them to grayscale before mapping pixel values to ASCII letters. Users can change the character set to get different effects.
+
+<!-- GETTING STARTED -->
+## Getting Started
+
+Before we begin, make sure you have one of recent versions of Python installed on your computer.
+
+### Installation
+
+```sh
+python -m pip install aksharify
+```
+
+## Usage
+
+```python
+from aksharify import TextArt
+
+# input image file
+art = TextArt("Julia.png")
+
+# see image
+art.image.show()
+
+# set dimension of output text
+art.set_dim(80)
+
+# genetate text
+art.asciify()
+
+# output into .txt file
+art.text_output("output")
+
+# generate colored text using html
+art.colorify()
+
+# output into .html file
+art.color_output("output")
+```
+
+_For examples from user community, please refer to the [primepatel.github.io/aksharify](https://primepatel.github.io/aksharify)_
+
+
+<!-- ROADMAP -->
+## Roadmap
+
+- [x] NumberiFy
+- [-] Predifined order of characters
+- [-] Getting images from URL
+- [-] EmojiFy
+
+See the [open issues](https://github.com/github_username/repo_name/issues) for a full list of proposed features (and known issues).
+
+<!-- CONTRIBUTING -->
+## Contributing
+
+Contributions are what make the open source community such a wonderful place to learn, be inspired, and create. Any contributions you make are `appreciated greatly`.
+
+If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
+Don't forget to give the project a star! Thanks again!
+
+1. Fork the Project
+2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
+3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
+4. Push to the Branch (`git push origin feature/AmazingFeature`)
+5. Open a Pull Request
+
+<!-- LICENSE -->
+## License
+
+Distributed under the MIT License. See `LICENSE.txt` for more information.
+
+<!-- CONTACT -->
+## Contact
+
+Prime Patel - [@primepatel](https://twitter.com/primespatel) - primespatel@gmail.com
+
+Project Link: [https://github.com/primepatel/aksharify](https://github.com/primepatel/aksharify)
+
+
+<!-- ACKNOWLEDGMENTS -->
+<!-- ## Acknowledgments
+
+* []()
+* []()
+* []() -->
+
+<p align="right">(<a href="#readme-top">back to top</a>)</p>
+
+
+
+<!-- MARKDOWN LINKS & IMAGES -->
+<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
+[contributors-shield]: https://img.shields.io/github/contributors/primepatel/Aksharify.svg?style=for-the-badge
+[contributors-url]: https://github.com/primepatel/Aksharify/graphs/contributors
+[forks-shield]: https://img.shields.io/github/forks/primepatel/Aksharify.svg?style=for-the-badge
+[forks-url]: https://github.com/primepatel/Aksharify/network/members
+[stars-shield]: https://img.shields.io/github/stars/primepatel/Aksharify.svg?style=for-the-badge
+[stars-url]: https://github.com/primepatel/Aksharify/stargazers
+[issues-shield]: https://img.shields.io/github/issues/primepatel/Aksharify.svg?style=for-the-badge
+[issues-url]: https://github.com/primepatel/Aksharify/issues
+[license-shield]: https://img.shields.io/github/license/primepatel/Aksharify.svg?style=for-the-badge
+[license-url]: https://github.com/primepatel/Aksharify/blob/master/LICENSE.txt
+[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
+[linkedin-url]: https://linkedin.com/in/primepatel
+[Downloads-shield]: https://img.shields.io/pypi/dm/aksharify?style=for-the-badge
```

#### html2text {}

```diff
@@ -1,20 +1,24 @@
-Metadata-Version: 2.1 Name: aksharify Version: 2.5.3 Summary: Ascii art module
-Author-email: Prime Patel
-gmail.com> Project-URL: Homepage, https://github.com/primepatel/aksharify
-Project-URL: Bug Tracker, https://github.com/primepatel/aksharify/issues
-Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
-Approved :: MIT License Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
-LICENSE.md  # __Aksharify__ [![Contributors][contributors-shield]]
-[contributors-url] [![Forks][forks-shield]][forks-url] [![Stargazers][stars-
-shield]][stars-url] [![Issues][issues-shield]][issues-url] [![MIT License]
-[license-shield]][license-url] [![LinkedIn][linkedin-shield]][linkedin-url] [!
-[PyPI - Downloads][Downloads-shield]](https://pypistats.org/packages/aksharify)
-
+Metadata-Version: 2.1 Name: aksharify Version: 2.5.5 Summary: Python Ascii +
+Emoji Art Module Home-page: https://primepatel.github.io/aksharify-docs/
+License: MIT Keywords: Ascii Art,Emoji Art,Prime Patel,primepatel Author: Prime
+Patel Author-email: primespatel@gmail.com Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Programming Language :: Python :: 3.6 Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Requires-Dist:
+pillow (>=9.5.0,<10.0.0) Project-URL: Repository, https://github.com/
+primepatel/aksharify Description-Content-Type: text/markdown  # __Aksharify__
+[![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
+shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-
+shield]][issues-url] [![MIT License][license-shield]][license-url] [![LinkedIn]
+[linkedin-shield]][linkedin-url] [![PyPI - Downloads][Downloads-shield]](https:
+//pypistats.org/packages/aksharify)
  ## About the module The inspiration for this module came from a Numberphile
 video called "The Trinity Hall Prime," which I first saw in high school days.
 It motivated me to explore the possibilities of such a prime number. I created
 a Python module that uses a predetermined character set to turn photos into
 ASCII art. It manipulates images using the PIL package, transforming them to
 grayscale before mapping pixel values to ASCII letters. Users can change the
 character set to get different effects.  ## Getting Started Before we begin,
```

