# Comparing `tmp/eArsivPortal-0.0.5.tar.gz` & `tmp/eArsivPortal-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eArsivPortal-0.0.5.tar", last modified: Sun May 28 14:48:04 2023, max compression
+gzip compressed data, was "eArsivPortal-0.0.6.tar", last modified: Mon May 29 12:09:53 2023, max compression
```

## Comparing `eArsivPortal-0.0.5.tar` & `eArsivPortal-0.0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:48:04.260117 eArsivPortal-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-28 14:47:32.000000 eArsivPortal-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-28 14:47:32.000000 eArsivPortal-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6206 2023-05-28 14:48:04.260117 eArsivPortal-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-05-28 14:47:32.000000 eArsivPortal-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:48:04.256117 eArsivPortal-0.0.5/eArsivPortal/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:48:04.260117 eArsivPortal-0.0.5/eArsivPortal/Core/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-28 14:47:32.000000 eArsivPortal-0.0.5/eArsivPortal/Core/Hatalar.py
--rw-r--r--   0 runner    (1001) docker     (123)     6179 2023-05-28 14:47:32.000000 eArsivPortal-0.0.5/eArsivPortal/Core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:48:04.260117 eArsivPortal-0.0.5/eArsivPortal/Libs/
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-05-28 14:47:32.000000 eArsivPortal-0.0.5/eArsivPortal/Libs/FaturaVer.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-28 14:47:32.000000 eArsivPortal-0.0.5/eArsivPortal/Libs/Oturum.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-28 14:47:32.000000 eArsivPortal-0.0.5/eArsivPortal/Libs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:48:04.260117 eArsivPortal-0.0.5/eArsivPortal/Models/
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-05-28 14:47:32.000000 eArsivPortal-0.0.5/eArsivPortal/Models/Komutlar.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-28 14:47:32.000000 eArsivPortal-0.0.5/eArsivPortal/Models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-28 14:47:32.000000 eArsivPortal-0.0.5/eArsivPortal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:48:04.260117 eArsivPortal-0.0.5/eArsivPortal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6206 2023-05-28 14:48:04.000000 eArsivPortal-0.0.5/eArsivPortal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-28 14:48:04.000000 eArsivPortal-0.0.5/eArsivPortal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 14:48:04.000000 eArsivPortal-0.0.5/eArsivPortal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-28 14:48:04.000000 eArsivPortal-0.0.5/eArsivPortal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-28 14:48:04.000000 eArsivPortal-0.0.5/eArsivPortal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 14:48:04.260117 eArsivPortal-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-28 14:47:32.000000 eArsivPortal-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:09:53.432963 eArsivPortal-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-29 12:08:54.000000 eArsivPortal-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-29 12:08:54.000000 eArsivPortal-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6604 2023-05-29 12:09:53.432963 eArsivPortal-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-05-29 12:08:54.000000 eArsivPortal-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:09:53.432963 eArsivPortal-0.0.6/eArsivPortal/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:09:53.432963 eArsivPortal-0.0.6/eArsivPortal/Core/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-29 12:08:54.000000 eArsivPortal-0.0.6/eArsivPortal/Core/Hatalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8311 2023-05-29 12:08:54.000000 eArsivPortal-0.0.6/eArsivPortal/Core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:09:53.432963 eArsivPortal-0.0.6/eArsivPortal/Libs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-05-29 12:08:54.000000 eArsivPortal-0.0.6/eArsivPortal/Libs/FaturaVer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-29 12:08:54.000000 eArsivPortal-0.0.6/eArsivPortal/Libs/Oturum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-29 12:08:54.000000 eArsivPortal-0.0.6/eArsivPortal/Libs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:09:53.432963 eArsivPortal-0.0.6/eArsivPortal/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-29 12:08:54.000000 eArsivPortal-0.0.6/eArsivPortal/Models/Komutlar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-29 12:08:54.000000 eArsivPortal-0.0.6/eArsivPortal/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-29 12:08:54.000000 eArsivPortal-0.0.6/eArsivPortal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:09:53.432963 eArsivPortal-0.0.6/eArsivPortal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6604 2023-05-29 12:09:53.000000 eArsivPortal-0.0.6/eArsivPortal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-29 12:09:53.000000 eArsivPortal-0.0.6/eArsivPortal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 12:09:53.000000 eArsivPortal-0.0.6/eArsivPortal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-29 12:09:53.000000 eArsivPortal-0.0.6/eArsivPortal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-29 12:09:53.000000 eArsivPortal-0.0.6/eArsivPortal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 12:09:53.432963 eArsivPortal-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-29 12:08:54.000000 eArsivPortal-0.0.6/setup.py
```

### Comparing `eArsivPortal-0.0.5/LICENSE` & `eArsivPortal-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `eArsivPortal-0.0.5/PKG-INFO` & `eArsivPortal-0.0.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eArsivPortal
-Version: 0.0.5
+Version: 0.0.6
 Summary: GİB e-Arşiv Portal e-Fatura, e-SMM, e-Müstahsil Oluşturucu
 Home-page: https://github.com/keyiflerolsun/eArsivPortal
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: eArsivPortal,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
@@ -112,15 +112,15 @@
     unvan:str         = "",
     vergi_dairesi:str = "",
     urun_adi:str      = "Python Yazılım Hizmeti",
     fiyat:int | float = 100,
     fatura_notu:str   = "— QNB Finansbank —\nTR70 0011 1000 0000 0118 5102 59\nÖmer Faruk Sancak"
 )
 #--------------------------------------------------------------#
-True
+{"ettn": "b40c16ae-8509-434e-bd6f-894459372134"}
 ```
 
 ```python
 faturalar = portal.faturalari_getir(
     baslangic_tarihi = "01/05/2023",
     bitis_tarihi     = "28/05/2023"
 )
@@ -153,14 +153,32 @@
     onay_durumu = faturalar[0].get("onayDurumu")
 )
 
 with open(f"{faturalar[0].get("aliciUnvanAdSoyad")}.html", "w", encoding="utf-8") as dosya:
     dosya.write(html_fatura)
 ```
 
+```python
+portal.fatura_sil(
+    faturalar = [faturalar[0], faturalar[1]]
+    aciklama  = "Fatura silindi."
+)
+#--------------------------------------------------------------#
+2 fatura başarıyla silindi.
+```
+
+```python
+oid = portal.gib_imza()
+portal.gib_sms_onay(faturalar[3], oid, input("SMS Doğrulama Kodu: "))
+```
+
+```python
+portal.cikis_yap()
+```
+
 ## 🌐 Telif Hakkı ve Lisans
 
 * *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/keyiflerolsun) ❤️️
 * [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/eArsivPortal/blob/master/LICENSE) *Koşullarına göre lisanslanmıştır..*
 
 ## ♻️ İletişim
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: eArsivPortal Version: 0.0.5 Summary: GÄ°B e-ArÅiv
+Metadata-Version: 2.1 Name: eArsivPortal Version: 0.0.6 Summary: GÄ°B e-ArÅiv
 Portal e-Fatura, e-SMM, e-MÃ¼stahsil OluÅturucu Home-page: https://github.com/
 keyiflerolsun/eArsivPortal Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 eArsivPortal,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
@@ -51,28 +51,33 @@
 -------------# { "unvan":"HOSAM ALDEEN ABUSHAWER TÄ°CARÄ° GÄ°RÄ°ÅÄ°MÄ°",
 "adi":"", "soyadi":"", "vergiDairesi":"kars" } ``` ```python
 portal.fatura_olustur( tarih:str = "07/10/1995", saat:str = "14:28:37",
 vkn_veya_tckn:str = "11111111111", ad:str = "Ãmer Faruk", soyad:str =
 "Sancak", unvan:str = "", vergi_dairesi:str = "", urun_adi:str = "Python
 YazÄ±lÄ±m Hizmeti", fiyat:int | float = 100, fatura_notu:str = "â QNB
 Finansbank â\nTR70 0011 1000 0000 0118 5102 59\nÃmer Faruk Sancak" ) #------
---------------------------------------------------------# True ``` ```python
-faturalar = portal.faturalari_getir( baslangic_tarihi = "01/05/2023",
-bitis_tarihi = "28/05/2023" ) #------------------------------------------------
---------------# [ { 'belgeNumarasi': 'GIB2023000002672', 'aliciVknTckn':
-'16045751784', 'aliciUnvanAdSoyad': 'Sercan AYDIN', 'belgeTarihi': '28-05-
-2023', 'belgeTuru': 'FATURA', 'onayDurumu': 'OnaylanmadÄ±', 'ettn': '0c111c74-
-fcd4-11ed-8026-3ae56703837b' }, { 'belgeNumarasi': 'GIB2023000002673',
-'aliciVknTckn': '16045751784', 'aliciUnvanAdSoyad': 'Sercan AYDIN',
-'belgeTarihi': '28-05-2023', 'belgeTuru': 'FATURA', 'onayDurumu': 'SilinmiÅ',
-'ettn': '234baa8e-fcd5-11ed-827f-3ae56703837b' } ] ``` ```python html_fatura =
-portal.fatura_html( ettn = faturalar[0].get("ettn") onay_durumu = faturalar
-[0].get("onayDurumu") ) with open(f"{faturalar[0].get
-("aliciUnvanAdSoyad")}.html", "w", encoding="utf-8") as dosya: dosya.write
-(html_fatura) ``` ## ð Telif HakkÄ± ve Lisans * *Copyright (C) 2023 by*
-[keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL
-PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/
-eArsivPortal/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ##
-â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek isterseniz, **Telegram**'dan
-mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ##
-ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)**
-*** > **[@KekikAkademi](https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
+--------------------------------------------------------# {"ettn": "b40c16ae-
+8509-434e-bd6f-894459372134"} ``` ```python faturalar = portal.faturalari_getir
+( baslangic_tarihi = "01/05/2023", bitis_tarihi = "28/05/2023" ) #-------------
+-------------------------------------------------# [ { 'belgeNumarasi':
+'GIB2023000002672', 'aliciVknTckn': '16045751784', 'aliciUnvanAdSoyad': 'Sercan
+AYDIN', 'belgeTarihi': '28-05-2023', 'belgeTuru': 'FATURA', 'onayDurumu':
+'OnaylanmadÄ±', 'ettn': '0c111c74-fcd4-11ed-8026-3ae56703837b' },
+{ 'belgeNumarasi': 'GIB2023000002673', 'aliciVknTckn': '16045751784',
+'aliciUnvanAdSoyad': 'Sercan AYDIN', 'belgeTarihi': '28-05-2023', 'belgeTuru':
+'FATURA', 'onayDurumu': 'SilinmiÅ', 'ettn': '234baa8e-fcd5-11ed-827f-
+3ae56703837b' } ] ``` ```python html_fatura = portal.fatura_html( ettn =
+faturalar[0].get("ettn") onay_durumu = faturalar[0].get("onayDurumu") ) with
+open(f"{faturalar[0].get("aliciUnvanAdSoyad")}.html", "w", encoding="utf-8") as
+dosya: dosya.write(html_fatura) ``` ```python portal.fatura_sil( faturalar =
+[faturalar[0], faturalar[1]] aciklama = "Fatura silindi." ) #------------------
+--------------------------------------------# 2 fatura baÅarÄ±yla silindi. ```
+```python oid = portal.gib_imza() portal.gib_sms_onay(faturalar[3], oid, input
+("SMS DoÄrulama Kodu: ")) ``` ```python portal.cikis_yap() ``` ## ð Telif
+HakkÄ± ve Lisans * *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/
+keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007]
+(https://github.com/keyiflerolsun/eArsivPortal/blob/master/LICENSE)
+*KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ## â»ï¸ Ä°letiÅim *Benimle
+iletiÅime geÃ§mek isterseniz, **Telegram**'dan mesaj gÃ¶ndermekten
+Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ## ð¸ BaÄÄ±Å Yap **
+[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)** *** > **
+[@KekikAkademi](https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
```

### Comparing `eArsivPortal-0.0.5/README.md` & `eArsivPortal-0.0.6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     unvan:str         = "",
     vergi_dairesi:str = "",
     urun_adi:str      = "Python Yazılım Hizmeti",
     fiyat:int | float = 100,
     fatura_notu:str   = "— QNB Finansbank —\nTR70 0011 1000 0000 0118 5102 59\nÖmer Faruk Sancak"
 )
 #--------------------------------------------------------------#
-True
+{"ettn": "b40c16ae-8509-434e-bd6f-894459372134"}
 ```
 
 ```python
 faturalar = portal.faturalari_getir(
     baslangic_tarihi = "01/05/2023",
     bitis_tarihi     = "28/05/2023"
 )
@@ -137,14 +137,32 @@
     onay_durumu = faturalar[0].get("onayDurumu")
 )
 
 with open(f"{faturalar[0].get("aliciUnvanAdSoyad")}.html", "w", encoding="utf-8") as dosya:
     dosya.write(html_fatura)
 ```
 
+```python
+portal.fatura_sil(
+    faturalar = [faturalar[0], faturalar[1]]
+    aciklama  = "Fatura silindi."
+)
+#--------------------------------------------------------------#
+2 fatura başarıyla silindi.
+```
+
+```python
+oid = portal.gib_imza()
+portal.gib_sms_onay(faturalar[3], oid, input("SMS Doğrulama Kodu: "))
+```
+
+```python
+portal.cikis_yap()
+```
+
 ## 🌐 Telif Hakkı ve Lisans
 
 * *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/keyiflerolsun) ❤️️
 * [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/eArsivPortal/blob/master/LICENSE) *Koşullarına göre lisanslanmıştır..*
 
 ## ♻️ İletişim
```

#### html2text {}

```diff
@@ -43,28 +43,33 @@
 -------------# { "unvan":"HOSAM ALDEEN ABUSHAWER TÄ°CARÄ° GÄ°RÄ°ÅÄ°MÄ°",
 "adi":"", "soyadi":"", "vergiDairesi":"kars" } ``` ```python
 portal.fatura_olustur( tarih:str = "07/10/1995", saat:str = "14:28:37",
 vkn_veya_tckn:str = "11111111111", ad:str = "Ãmer Faruk", soyad:str =
 "Sancak", unvan:str = "", vergi_dairesi:str = "", urun_adi:str = "Python
 YazÄ±lÄ±m Hizmeti", fiyat:int | float = 100, fatura_notu:str = "â QNB
 Finansbank â\nTR70 0011 1000 0000 0118 5102 59\nÃmer Faruk Sancak" ) #------
---------------------------------------------------------# True ``` ```python
-faturalar = portal.faturalari_getir( baslangic_tarihi = "01/05/2023",
-bitis_tarihi = "28/05/2023" ) #------------------------------------------------
---------------# [ { 'belgeNumarasi': 'GIB2023000002672', 'aliciVknTckn':
-'16045751784', 'aliciUnvanAdSoyad': 'Sercan AYDIN', 'belgeTarihi': '28-05-
-2023', 'belgeTuru': 'FATURA', 'onayDurumu': 'OnaylanmadÄ±', 'ettn': '0c111c74-
-fcd4-11ed-8026-3ae56703837b' }, { 'belgeNumarasi': 'GIB2023000002673',
-'aliciVknTckn': '16045751784', 'aliciUnvanAdSoyad': 'Sercan AYDIN',
-'belgeTarihi': '28-05-2023', 'belgeTuru': 'FATURA', 'onayDurumu': 'SilinmiÅ',
-'ettn': '234baa8e-fcd5-11ed-827f-3ae56703837b' } ] ``` ```python html_fatura =
-portal.fatura_html( ettn = faturalar[0].get("ettn") onay_durumu = faturalar
-[0].get("onayDurumu") ) with open(f"{faturalar[0].get
-("aliciUnvanAdSoyad")}.html", "w", encoding="utf-8") as dosya: dosya.write
-(html_fatura) ``` ## ð Telif HakkÄ± ve Lisans * *Copyright (C) 2023 by*
-[keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL
-PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/
-eArsivPortal/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ##
-â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek isterseniz, **Telegram**'dan
-mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ##
-ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)**
-*** > **[@KekikAkademi](https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
+--------------------------------------------------------# {"ettn": "b40c16ae-
+8509-434e-bd6f-894459372134"} ``` ```python faturalar = portal.faturalari_getir
+( baslangic_tarihi = "01/05/2023", bitis_tarihi = "28/05/2023" ) #-------------
+-------------------------------------------------# [ { 'belgeNumarasi':
+'GIB2023000002672', 'aliciVknTckn': '16045751784', 'aliciUnvanAdSoyad': 'Sercan
+AYDIN', 'belgeTarihi': '28-05-2023', 'belgeTuru': 'FATURA', 'onayDurumu':
+'OnaylanmadÄ±', 'ettn': '0c111c74-fcd4-11ed-8026-3ae56703837b' },
+{ 'belgeNumarasi': 'GIB2023000002673', 'aliciVknTckn': '16045751784',
+'aliciUnvanAdSoyad': 'Sercan AYDIN', 'belgeTarihi': '28-05-2023', 'belgeTuru':
+'FATURA', 'onayDurumu': 'SilinmiÅ', 'ettn': '234baa8e-fcd5-11ed-827f-
+3ae56703837b' } ] ``` ```python html_fatura = portal.fatura_html( ettn =
+faturalar[0].get("ettn") onay_durumu = faturalar[0].get("onayDurumu") ) with
+open(f"{faturalar[0].get("aliciUnvanAdSoyad")}.html", "w", encoding="utf-8") as
+dosya: dosya.write(html_fatura) ``` ```python portal.fatura_sil( faturalar =
+[faturalar[0], faturalar[1]] aciklama = "Fatura silindi." ) #------------------
+--------------------------------------------# 2 fatura baÅarÄ±yla silindi. ```
+```python oid = portal.gib_imza() portal.gib_sms_onay(faturalar[3], oid, input
+("SMS DoÄrulama Kodu: ")) ``` ```python portal.cikis_yap() ``` ## ð Telif
+HakkÄ± ve Lisans * *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/
+keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007]
+(https://github.com/keyiflerolsun/eArsivPortal/blob/master/LICENSE)
+*KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ## â»ï¸ Ä°letiÅim *Benimle
+iletiÅime geÃ§mek isterseniz, **Telegram**'dan mesaj gÃ¶ndermekten
+Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ## ð¸ BaÄÄ±Å Yap **
+[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)** *** > **
+[@KekikAkademi](https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
```

### Comparing `eArsivPortal-0.0.5/eArsivPortal/Core/__init__.py` & `eArsivPortal-0.0.6/eArsivPortal/Core/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from parsel   import Selector
 from .Hatalar import GirisYapilmadi, OturumSuresiDoldu, eArsivPortalHatasi
 
 from datetime import datetime
 from pytz     import timezone
 
 class eArsivPortal:
-    def __init__(self, kullanici_kodu:str="33333301", sifre:str="1", test_modu:bool=True):
+    def __init__(self, kullanici_kodu:str="33333315", sifre:str="1", test_modu:bool=True):
 
         self.kullanici_kodu = kullanici_kodu
         self.sifre          = sifre
         self.test_modu      = test_modu
 
         apiler = {
             "YAYIN" : "https://earsivportal.efatura.gov.tr",     # * https://earsivportal.efatura.gov.tr/intragiris.html
@@ -26,54 +26,71 @@
         self.oturum   = legacy_session()
         self.komutlar = Komutlar()
 
         self.oturum.headers.update({
             "User-Agent" : "https://github.com/keyiflerolsun/eArsivPortal"
         })
 
-        self.__giris_yap(kullanici_kodu, sifre)
+        self.token = None
+        self.giris_yap()
 
     def __istek_ayristir(self, istek:Response, veri:dict) -> dict | Exception:
         if istek.status_code != 200 or veri.get("error"):
-            try:
-                hata_metni = veri["messages"][0]["text"]
-            except TypeError:
-                hata_metni = veri["messages"][0]
+            veri_mesaj = veri["messages"][0]
+            hata_metni = veri_mesaj["text"] if isinstance(veri_mesaj, dict) else veri_mesaj
 
             if "Oturum zamanaşımına uğradı" in hata_metni:
                 raise OturumSuresiDoldu(hata_metni)
 
             raise eArsivPortalHatasi(hata_metni)
 
         return veri
 
-    def __giris_yap(self, kullanici_kodu:str, sifre:str) -> bool | eArsivPortalHatasi:
+    def giris_yap(self) -> bool | eArsivPortalHatasi:
         istek = self.oturum.post(
-            url     = f"{self.url}/earsiv-services/assos-login",
-            data    = {
+            url  = f"{self.url}/earsiv-services/assos-login",
+            data = {
                 "assoscmd" : "login" if self.test_modu else "anologin",
                 "rtype"    : "json",
-                "userid"   : kullanici_kodu,
-                "sifre"    : sifre,
-                "sifre2"   : sifre,
+                "userid"   : self.kullanici_kodu,
+                "sifre"    : self.sifre,
+                "sifre2"   : self.sifre,
                 "parola"   : "1"
             }
         )
         veri = istek.json()
         self.token = self.__istek_ayristir(istek, veri)["token"]
         return self.token is not None
 
+    def cikis_yap(self) -> bool | eArsivPortalHatasi:
+        if not self.token:
+            raise GirisYapilmadi("Giriş yapmadan çıkış yapamazsınız!")
+
+        istek = self.oturum.post(
+            url  = f"{self.url}/earsiv-services/assos-login",
+            data = {
+                "assoscmd" : "logout",
+                "rtype"    : "json",
+                "token"    : self.token
+            }
+        )
+        if istek.status_code != 200:
+            return False
+
+        self.token = None
+        return True
+
     def __kod_calistir(self, komut:Komut, jp:dict):
         if not self.token:
-            raise GirisYapilmadi("Giriş yapmadan fatura oluşturamazsınız!")
+            raise GirisYapilmadi("Giriş yapmadan işlem yapamazsınız!")
 
         try:
             istek = self.oturum.post(
-                url     = f"{self.url}/earsiv-services/dispatch",
-                data    = {
+                url  = f"{self.url}/earsiv-services/dispatch",
+                data = {
                     "cmd"      : komut.cmd,
                     "callid"   : f"{uuid4()}",
                     "pageName" : komut.sayfa,
                     "token"    : self.token,
                     "jp"       : dumps(jp)
                 }
             )
@@ -81,92 +98,144 @@
 
             return self.__istek_ayristir(istek, veri)
         except OturumSuresiDoldu:
             self.__giris_yap(self.kullanici_kodu, self.sifre)
             return self.__kod_calistir(komut, jp)
 
     def bilgilerim(self) -> dict:
-        veri = self.__kod_calistir(
+        istek = self.__kod_calistir(
             komut = self.komutlar.KULLANICI_BILGILERI_GETIR,
             jp    = {}
         )
 
-        return veri.get("data")
+        return istek.get("data")
 
-    def kisi_getir(self, vkn_veya_tckn:str):
-        veri = self.__kod_calistir(
-            komut = self.komutlar.MERNISTEN_BILGILERI_GETIR,
-            jp    = {
-                "vknTckn" : vkn_veya_tckn
-            }
-        )
+    def kisi_getir(self, vkn_veya_tckn:str) -> dict:
+        try:
+            istek = self.__kod_calistir(
+                komut = self.komutlar.MERNISTEN_BILGILERI_GETIR,
+                jp    = {
+                    "vknTckn" : vkn_veya_tckn
+                }
+            )
+        except Exception:
+            return {}
 
-        return veri.get("data")
+        return istek.get("data")
 
     def fatura_olustur(
         self,
         tarih:str         = "07/10/1995",
         saat:str          = "14:28:37",
         vkn_veya_tckn:str = "11111111111",
         ad:str            = "Ömer Faruk",
         soyad:str         = "Sancak",
         unvan:str         = "",
         vergi_dairesi:str = "",
         urun_adi:str      = "Python Yazılım Hizmeti",
         fiyat:int | float = 100,
         fatura_notu:str   = "— QNB Finansbank —\nTR70 0011 1000 0000 0118 5102 59\nÖmer Faruk Sancak"
-    ) -> bool:
+    ) -> dict[str, str | None]:
         kisi_bilgi = self.kisi_getir(vkn_veya_tckn)
 
-        veri = self.__kod_calistir(
+        fatura = fatura_ver(
+            tarih         = tarih or datetime.now(timezone("Turkey")).strftime("%d/%m/%Y"),
+            saat          = saat,
+            vkn_veya_tckn = vkn_veya_tckn,
+            ad            = kisi_bilgi.get("adi") or ad,
+            soyad         = kisi_bilgi.get("soyadi") or soyad,
+            unvan         = kisi_bilgi.get("unvan") or unvan,
+            vergi_dairesi = kisi_bilgi.get("vergiDairesi") or vergi_dairesi,
+            urun_adi      = urun_adi,
+            fiyat         = fiyat,
+            fatura_notu   = fatura_notu
+        )
+
+        istek = self.__kod_calistir(
             komut = self.komutlar.FATURA_OLUSTUR,
-            jp    = fatura_ver(
-                tarih         = tarih or datetime.now(timezone("Turkey")).strftime("%d/%m/%Y"),
-                saat          = saat,
-                vkn_veya_tckn = vkn_veya_tckn,
-                ad            = kisi_bilgi.get("adi") or ad,
-                soyad         = kisi_bilgi.get("soyadi") or soyad,
-                unvan         = kisi_bilgi.get("unvan") or unvan,
-                vergi_dairesi = kisi_bilgi.get("vergiDairesi") or vergi_dairesi,
-                urun_adi      = urun_adi,
-                fiyat         = fiyat,
-                fatura_notu   = fatura_notu
-            )
+            jp    = fatura
         )
 
-        return "Faturanız başarıyla oluşturulmuştur." in veri.get("data")
+        if "Faturanız başarıyla oluşturulmuştur." in istek.get("data"):
+            return {"ettn": fatura.get("faturaUuid")}
+
+        return {"ettn": None}
 
     def faturalari_getir(self, baslangic_tarihi:str="01/05/2023", bitis_tarihi:str="28/05/2023") -> list[dict]:
-        veri = self.__kod_calistir(
+        istek = self.__kod_calistir(
             komut = self.komutlar.TASLAKLARI_GETIR,
-            jp    =     {
-                "baslangic" : baslangic_tarihi,
+            jp    = {
+                "baslangic" : baslangic_tarihi or datetime.now(timezone("Turkey")).strftime("%d/%m/%Y"),
                 "bitis"     : bitis_tarihi or datetime.now(timezone("Turkey")).strftime("%d/%m/%Y"),
                 "hangiTip"  :"5000/30000",
                 "table"     : []
             }
         )
 
-        return veri.get("data")
+        return istek.get("data")
 
     def fatura_html(self, ettn:str, onay_durumu:str) -> str:
-        veri = self.__kod_calistir(
+        istek = self.__kod_calistir(
             komut = self.komutlar.FATURA_GOSTER,
             jp    = {
                 "ettn"       : ettn,
                 "onayDurumu" : onay_durumu
             }
         )
 
-        secici = Selector(veri.get("data"))
+        secici = Selector(istek.get("data"))
 
         for tr in secici.xpath("//tr"):
             bos_tdler = tr.xpath(".//td[normalize-space(.)='\xa0']")
 
             if len(bos_tdler) == len(tr.xpath(".//td")):
                 tr_element = tr.root
                 tr_element.getparent().remove(tr_element)
 
         return secici.extract()
 
+    def fatura_sil(self, faturalar:list[dict] | dict, aciklama:str):
+        istek = self.__kod_calistir(
+            komut = self.komutlar.FATURA_SIL,
+            jp    = {
+                "silinecekler" : [faturalar] if isinstance(faturalar, dict) else faturalar,
+                "aciklama"     : aciklama
+            }
+        )
+
+        return istek.get("data")
+
+    def gib_imza(self) -> dict[str, str | None]:
+        telefon_istek = self.__kod_calistir(
+            komut = self.komutlar.TELEFONNO_SORGULA,
+            jp    = {}
+        )
+        telefon_veri = telefon_istek.get("data")
+        telefon_no   = telefon_veri.get("telefon")
+        if not telefon_no:
+            return {"oid": None}
+
+        sms_gonder = self.__kod_calistir(
+            komut = self.komutlar.SMSSIFRE_GONDER,
+            jp    = {
+                "CEPTEL"  : telefon_no,
+                "KCEPTEL" : False,
+                "TIP"     : ""
+            }
+        )
+
+        return sms_gonder.get("data")
+
+    def gib_sms_onay(self, faturalar:list[dict] | dict, oid:str, sifre:str):
+        istek = self.__kod_calistir(
+            komut = self.komutlar.SMSSIFRE_DOGRULA,
+            jp    = {
+                "SIFRE" : sifre,
+                "OID"   : oid,
+                "OPR"   : 1,
+                "DATA"  : [faturalar] if isinstance(faturalar, dict) else faturalar,
+            }
+        )
+
+        return istek.get("data")
 
     # TODO: https://github.com/mlevent/fatura 'dan faydalanarak geri kalan fonksiyonlar yazılacaktır..
```

### Comparing `eArsivPortal-0.0.5/eArsivPortal/Libs/FaturaVer.py` & `eArsivPortal-0.0.6/eArsivPortal/Libs/FaturaVer.py`

 * *Files identical despite different names*

### Comparing `eArsivPortal-0.0.5/eArsivPortal/Libs/Oturum.py` & `eArsivPortal-0.0.6/eArsivPortal/Libs/Oturum.py`

 * *Files identical despite different names*

### Comparing `eArsivPortal-0.0.5/eArsivPortal/Models/Komutlar.py` & `eArsivPortal-0.0.6/eArsivPortal/Models/Komutlar.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,59 +3,43 @@
 from pydantic import BaseModel, Field
 
 class Komut(BaseModel):
     cmd:str   = Field(..., description="Komut Adı")
     sayfa:str = Field(..., description="Sayfa Adı")
 
 class Komutlar(BaseModel):
+    KULLANICI_BILGILERI_GETIR:Komut      = Komut(
+        cmd   = "EARSIV_PORTAL_KULLANICI_BILGILERI_GETIR",
+        sayfa = "RG_KULLANICI"
+    )
+    MERNISTEN_BILGILERI_GETIR:Komut      = Komut(
+        cmd   = "SICIL_VEYA_MERNISTEN_BILGILERI_GETIR",
+        sayfa = "RG_BASITFATURA"
+    )
     FATURA_OLUSTUR:Komut                 = Komut(
         cmd   = "EARSIV_PORTAL_FATURA_OLUSTUR",
         sayfa = "RG_BASITFATURA"
     )
     TASLAKLARI_GETIR:Komut               = Komut(
         cmd   = "EARSIV_PORTAL_TASLAKLARI_GETIR",
         sayfa = "RG_BASITTASLAKLAR"
     )
-    ADIMA_KESILEN_BELGELERI_GETIR:Komut  = Komut(
-        cmd   = "EARSIV_PORTAL_ADIMA_KESILEN_BELGELERI_GETIR",
-        sayfa = "RG_ALICI_TASLAKLAR"
-    )
-    FATURA_HSM_CIHAZI_ILE_IMZALA:Komut   = Komut(
-        cmd   = "EARSIV_PORTAL_FATURA_HSM_CIHAZI_ILE_IMZALA",
-        sayfa = "RG_BASITTASLAKLAR"
-    )
     FATURA_GOSTER:Komut                  = Komut(
         cmd   = "EARSIV_PORTAL_FATURA_GOSTER",
         sayfa = "RG_BASITTASLAKLAR"
     )
     FATURA_SIL:Komut                     = Komut(
         cmd   = "EARSIV_PORTAL_FATURA_SIL",
         sayfa = "RG_BASITTASLAKLAR"
     )
-    MERNISTEN_BILGILERI_GETIR:Komut      = Komut(
-        cmd   = "SICIL_VEYA_MERNISTEN_BILGILERI_GETIR",
-        sayfa = "RG_BASITFATURA"
+    TELEFONNO_SORGULA:Komut                = Komut(
+        cmd   = "EARSIV_PORTAL_TELEFONNO_SORGULA",
+        sayfa = "RG_SMSONAY"
     )
     SMSSIFRE_GONDER:Komut                = Komut(
         cmd   = "EARSIV_PORTAL_SMSSIFRE_GONDER",
         sayfa = "RG_SMSONAY"
     )
     SMSSIFRE_DOGRULA:Komut               = Komut(
-        cmd   = "EARSIV_PORTAL_SMSSIFRE_DOGRULA",
+        cmd   = "0lhozfib5410mp",
         sayfa = "RG_SMSONAY"
-    )
-    KULLANICI_BILGILERI_GETIR:Komut      = Komut(
-        cmd   = "EARSIV_PORTAL_KULLANICI_BILGILERI_GETIR",
-        sayfa = "RG_KULLANICI"
-    )
-    KULLANICI_BILGILERI_KAYDET:Komut     = Komut(
-        cmd   = "EARSIV_PORTAL_KULLANICI_BILGILERI_KAYDET",
-        sayfa = "RG_KULLANICI"
-    )
-    MUSTAHSIL_OLUSTUR:Komut              = Komut(
-        cmd   = "EARSIV_PORTAL_MUSTAHSIL_OLUSTUR",
-        sayfa = "RG_MUSTAHSIL"
-    )
-    SERBEST_MESLEK_MAKBUZU_OLUSTUR:Komut = Komut(
-        cmd   = "EARSIV_PORTAL_SERBEST_MESLEK_MAKBUZU_OLUSTUR",
-        sayfa = "RG_SERBEST"
     )
```

### Comparing `eArsivPortal-0.0.5/eArsivPortal.egg-info/PKG-INFO` & `eArsivPortal-0.0.6/eArsivPortal.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eArsivPortal
-Version: 0.0.5
+Version: 0.0.6
 Summary: GİB e-Arşiv Portal e-Fatura, e-SMM, e-Müstahsil Oluşturucu
 Home-page: https://github.com/keyiflerolsun/eArsivPortal
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: eArsivPortal,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
@@ -112,15 +112,15 @@
     unvan:str         = "",
     vergi_dairesi:str = "",
     urun_adi:str      = "Python Yazılım Hizmeti",
     fiyat:int | float = 100,
     fatura_notu:str   = "— QNB Finansbank —\nTR70 0011 1000 0000 0118 5102 59\nÖmer Faruk Sancak"
 )
 #--------------------------------------------------------------#
-True
+{"ettn": "b40c16ae-8509-434e-bd6f-894459372134"}
 ```
 
 ```python
 faturalar = portal.faturalari_getir(
     baslangic_tarihi = "01/05/2023",
     bitis_tarihi     = "28/05/2023"
 )
@@ -153,14 +153,32 @@
     onay_durumu = faturalar[0].get("onayDurumu")
 )
 
 with open(f"{faturalar[0].get("aliciUnvanAdSoyad")}.html", "w", encoding="utf-8") as dosya:
     dosya.write(html_fatura)
 ```
 
+```python
+portal.fatura_sil(
+    faturalar = [faturalar[0], faturalar[1]]
+    aciklama  = "Fatura silindi."
+)
+#--------------------------------------------------------------#
+2 fatura başarıyla silindi.
+```
+
+```python
+oid = portal.gib_imza()
+portal.gib_sms_onay(faturalar[3], oid, input("SMS Doğrulama Kodu: "))
+```
+
+```python
+portal.cikis_yap()
+```
+
 ## 🌐 Telif Hakkı ve Lisans
 
 * *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/keyiflerolsun) ❤️️
 * [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/eArsivPortal/blob/master/LICENSE) *Koşullarına göre lisanslanmıştır..*
 
 ## ♻️ İletişim
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: eArsivPortal Version: 0.0.5 Summary: GÄ°B e-ArÅiv
+Metadata-Version: 2.1 Name: eArsivPortal Version: 0.0.6 Summary: GÄ°B e-ArÅiv
 Portal e-Fatura, e-SMM, e-MÃ¼stahsil OluÅturucu Home-page: https://github.com/
 keyiflerolsun/eArsivPortal Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 eArsivPortal,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
@@ -51,28 +51,33 @@
 -------------# { "unvan":"HOSAM ALDEEN ABUSHAWER TÄ°CARÄ° GÄ°RÄ°ÅÄ°MÄ°",
 "adi":"", "soyadi":"", "vergiDairesi":"kars" } ``` ```python
 portal.fatura_olustur( tarih:str = "07/10/1995", saat:str = "14:28:37",
 vkn_veya_tckn:str = "11111111111", ad:str = "Ãmer Faruk", soyad:str =
 "Sancak", unvan:str = "", vergi_dairesi:str = "", urun_adi:str = "Python
 YazÄ±lÄ±m Hizmeti", fiyat:int | float = 100, fatura_notu:str = "â QNB
 Finansbank â\nTR70 0011 1000 0000 0118 5102 59\nÃmer Faruk Sancak" ) #------
---------------------------------------------------------# True ``` ```python
-faturalar = portal.faturalari_getir( baslangic_tarihi = "01/05/2023",
-bitis_tarihi = "28/05/2023" ) #------------------------------------------------
---------------# [ { 'belgeNumarasi': 'GIB2023000002672', 'aliciVknTckn':
-'16045751784', 'aliciUnvanAdSoyad': 'Sercan AYDIN', 'belgeTarihi': '28-05-
-2023', 'belgeTuru': 'FATURA', 'onayDurumu': 'OnaylanmadÄ±', 'ettn': '0c111c74-
-fcd4-11ed-8026-3ae56703837b' }, { 'belgeNumarasi': 'GIB2023000002673',
-'aliciVknTckn': '16045751784', 'aliciUnvanAdSoyad': 'Sercan AYDIN',
-'belgeTarihi': '28-05-2023', 'belgeTuru': 'FATURA', 'onayDurumu': 'SilinmiÅ',
-'ettn': '234baa8e-fcd5-11ed-827f-3ae56703837b' } ] ``` ```python html_fatura =
-portal.fatura_html( ettn = faturalar[0].get("ettn") onay_durumu = faturalar
-[0].get("onayDurumu") ) with open(f"{faturalar[0].get
-("aliciUnvanAdSoyad")}.html", "w", encoding="utf-8") as dosya: dosya.write
-(html_fatura) ``` ## ð Telif HakkÄ± ve Lisans * *Copyright (C) 2023 by*
-[keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL
-PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/
-eArsivPortal/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ##
-â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek isterseniz, **Telegram**'dan
-mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ##
-ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)**
-*** > **[@KekikAkademi](https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
+--------------------------------------------------------# {"ettn": "b40c16ae-
+8509-434e-bd6f-894459372134"} ``` ```python faturalar = portal.faturalari_getir
+( baslangic_tarihi = "01/05/2023", bitis_tarihi = "28/05/2023" ) #-------------
+-------------------------------------------------# [ { 'belgeNumarasi':
+'GIB2023000002672', 'aliciVknTckn': '16045751784', 'aliciUnvanAdSoyad': 'Sercan
+AYDIN', 'belgeTarihi': '28-05-2023', 'belgeTuru': 'FATURA', 'onayDurumu':
+'OnaylanmadÄ±', 'ettn': '0c111c74-fcd4-11ed-8026-3ae56703837b' },
+{ 'belgeNumarasi': 'GIB2023000002673', 'aliciVknTckn': '16045751784',
+'aliciUnvanAdSoyad': 'Sercan AYDIN', 'belgeTarihi': '28-05-2023', 'belgeTuru':
+'FATURA', 'onayDurumu': 'SilinmiÅ', 'ettn': '234baa8e-fcd5-11ed-827f-
+3ae56703837b' } ] ``` ```python html_fatura = portal.fatura_html( ettn =
+faturalar[0].get("ettn") onay_durumu = faturalar[0].get("onayDurumu") ) with
+open(f"{faturalar[0].get("aliciUnvanAdSoyad")}.html", "w", encoding="utf-8") as
+dosya: dosya.write(html_fatura) ``` ```python portal.fatura_sil( faturalar =
+[faturalar[0], faturalar[1]] aciklama = "Fatura silindi." ) #------------------
+--------------------------------------------# 2 fatura baÅarÄ±yla silindi. ```
+```python oid = portal.gib_imza() portal.gib_sms_onay(faturalar[3], oid, input
+("SMS DoÄrulama Kodu: ")) ``` ```python portal.cikis_yap() ``` ## ð Telif
+HakkÄ± ve Lisans * *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/
+keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007]
+(https://github.com/keyiflerolsun/eArsivPortal/blob/master/LICENSE)
+*KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ## â»ï¸ Ä°letiÅim *Benimle
+iletiÅime geÃ§mek isterseniz, **Telegram**'dan mesaj gÃ¶ndermekten
+Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ## ð¸ BaÄÄ±Å Yap **
+[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)** *** > **
+[@KekikAkademi](https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
```

### Comparing `eArsivPortal-0.0.5/setup.py` & `eArsivPortal-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 from io         import open
 
 setup(
     # ? Genel Bilgiler
     name         = "eArsivPortal",
-    version      = "0.0.5",
+    version      = "0.0.6",
     url          = "https://github.com/keyiflerolsun/eArsivPortal",
     description  = "GİB e-Arşiv Portal e-Fatura, e-SMM, e-Müstahsil Oluşturucu",
     keywords     = ["eArsivPortal", "KekikAkademi", "keyiflerolsun"],
 
     author       = "keyiflerolsun",
     author_email = "keyiflerolsun@gmail.com",
```

