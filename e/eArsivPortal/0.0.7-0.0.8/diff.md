# Comparing `tmp/eArsivPortal-0.0.7.tar.gz` & `tmp/eArsivPortal-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eArsivPortal-0.0.7.tar", last modified: Mon May 29 12:24:18 2023, max compression
+gzip compressed data, was "eArsivPortal-0.0.8.tar", last modified: Mon May 29 16:00:46 2023, max compression
```

## Comparing `eArsivPortal-0.0.7.tar` & `eArsivPortal-0.0.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:24:18.150122 eArsivPortal-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-29 12:23:49.000000 eArsivPortal-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-29 12:23:49.000000 eArsivPortal-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-05-29 12:24:18.150122 eArsivPortal-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-05-29 12:23:49.000000 eArsivPortal-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:24:18.150122 eArsivPortal-0.0.7/eArsivPortal/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:24:18.150122 eArsivPortal-0.0.7/eArsivPortal/Core/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-29 12:23:49.000000 eArsivPortal-0.0.7/eArsivPortal/Core/Hatalar.py
--rw-r--r--   0 runner    (1001) docker     (123)     8311 2023-05-29 12:23:49.000000 eArsivPortal-0.0.7/eArsivPortal/Core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:24:18.150122 eArsivPortal-0.0.7/eArsivPortal/Libs/
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-05-29 12:23:49.000000 eArsivPortal-0.0.7/eArsivPortal/Libs/FaturaVer.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-29 12:23:49.000000 eArsivPortal-0.0.7/eArsivPortal/Libs/Oturum.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-29 12:23:49.000000 eArsivPortal-0.0.7/eArsivPortal/Libs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:24:18.150122 eArsivPortal-0.0.7/eArsivPortal/Models/
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-29 12:23:49.000000 eArsivPortal-0.0.7/eArsivPortal/Models/Komutlar.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-29 12:23:49.000000 eArsivPortal-0.0.7/eArsivPortal/Models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-29 12:23:49.000000 eArsivPortal-0.0.7/eArsivPortal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:24:18.150122 eArsivPortal-0.0.7/eArsivPortal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-05-29 12:24:18.000000 eArsivPortal-0.0.7/eArsivPortal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-29 12:24:18.000000 eArsivPortal-0.0.7/eArsivPortal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 12:24:18.000000 eArsivPortal-0.0.7/eArsivPortal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-29 12:24:18.000000 eArsivPortal-0.0.7/eArsivPortal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-29 12:24:18.000000 eArsivPortal-0.0.7/eArsivPortal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 12:24:18.150122 eArsivPortal-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-29 12:23:49.000000 eArsivPortal-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:00:46.276864 eArsivPortal-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-29 16:00:14.000000 eArsivPortal-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-29 16:00:14.000000 eArsivPortal-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-05-29 16:00:46.272863 eArsivPortal-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-05-29 16:00:14.000000 eArsivPortal-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:00:46.272863 eArsivPortal-0.0.8/eArsivPortal/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:00:46.272863 eArsivPortal-0.0.8/eArsivPortal/Core/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-29 16:00:14.000000 eArsivPortal-0.0.8/eArsivPortal/Core/Hatalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-05-29 16:00:14.000000 eArsivPortal-0.0.8/eArsivPortal/Core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:00:46.272863 eArsivPortal-0.0.8/eArsivPortal/Libs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-05-29 16:00:14.000000 eArsivPortal-0.0.8/eArsivPortal/Libs/FaturaVer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-29 16:00:14.000000 eArsivPortal-0.0.8/eArsivPortal/Libs/Oturum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-29 16:00:14.000000 eArsivPortal-0.0.8/eArsivPortal/Libs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:00:46.272863 eArsivPortal-0.0.8/eArsivPortal/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-29 16:00:14.000000 eArsivPortal-0.0.8/eArsivPortal/Models/Komutlar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-29 16:00:14.000000 eArsivPortal-0.0.8/eArsivPortal/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-29 16:00:14.000000 eArsivPortal-0.0.8/eArsivPortal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:00:46.272863 eArsivPortal-0.0.8/eArsivPortal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-05-29 16:00:46.000000 eArsivPortal-0.0.8/eArsivPortal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-29 16:00:46.000000 eArsivPortal-0.0.8/eArsivPortal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 16:00:46.000000 eArsivPortal-0.0.8/eArsivPortal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-29 16:00:46.000000 eArsivPortal-0.0.8/eArsivPortal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-29 16:00:46.000000 eArsivPortal-0.0.8/eArsivPortal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 16:00:46.276864 eArsivPortal-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-29 16:00:14.000000 eArsivPortal-0.0.8/setup.py
```

### Comparing `eArsivPortal-0.0.7/LICENSE` & `eArsivPortal-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `eArsivPortal-0.0.7/PKG-INFO` & `eArsivPortal-0.0.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eArsivPortal
-Version: 0.0.7
+Version: 0.0.8
 Summary: GİB e-Arşiv Portal e-Fatura Oluşturucu
 Home-page: https://github.com/keyiflerolsun/eArsivPortal
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: eArsivPortal,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
@@ -61,49 +61,53 @@
     sifre          = "1",
     test_modu      = True
 )
 ```
 
 ```python
 portal.bilgilerim()
+
 #--------------------------------------------------------------#
-{
-    "vknTckn": "3333333301",
-    "unvan": "HOSAM ALDEEN ABUSHAWER TİCARİ GİRİŞİMİ",
-    "ad": "",
-    "soyad": "",
-    "cadde": "şehit yusuf bey",
-    "apartmanAdi": "yıldız",
-    "apartmanNo": "8",
-    "kapiNo": "2",
-    "kasaba": "ortakapı",
-    "ilce": "Merkez",
-    "il": "Kars",
-    "postaKodu": "36000",
-    "ulke": "Türkiye",
-    "telNo": "05524775288",
-    "faksNo": "",
-    "ePostaAdresi": "",
-    "webSitesiAdresi": "",
-    "vergiDairesi": "kars",
-    "sicilNo": "8729",
-    "isMerkezi": "",
-    "mersisNo": "9962438036000001"
-}
+
+Bilgilerim(
+    vknTckn='3333333315',
+    unvan='XYZ Yaz',
+    ad='',
+    soyad='',
+    cadde='Sahil yolu',
+    apartmanAdi='Dali çıtır pide',
+    apartmanNo='12',
+    kapiNo='3',
+    kasaba='adana',
+    ilce='GEMLİK',
+    il='Antalya',
+    postaKodu='16000',
+    ulke='Türkiye',
+    telNo='053982456665',
+    faksNo='',
+    ePostaAdresi='info@vekamp.com',
+    webSitesiAdresi='',
+    vergiDairesi='orhangazi vergi dairesi',
+    sicilNo='00000000000000',
+    isMerkezi='',
+    mersisNo=''
+)
 ```
 
 ```python
 portal.kisi_getir(vkn_veya_tckn="3333333301")
+
 #--------------------------------------------------------------#
-{
-    "unvan":"HOSAM ALDEEN ABUSHAWER TİCARİ GİRİŞİMİ",
-    "adi":"",
-    "soyadi":"",
-    "vergiDairesi":"kars"
-}
+
+Kisi(
+    unvan='XYZ Yaz',
+    adi='',
+    soyadi='',
+    vergiDairesi='orhangazi vergi dairesi'
+)
 ```
 
 ```python
 portal.fatura_olustur(
     tarih:str         = "07/10/1995",
     saat:str          = "14:28:37",
     vkn_veya_tckn:str = "11111111111",
@@ -111,68 +115,87 @@
     soyad:str         = "Sancak",
     unvan:str         = "",
     vergi_dairesi:str = "",
     urun_adi:str      = "Python Yazılım Hizmeti",
     fiyat:int | float = 100,
     fatura_notu:str   = "— QNB Finansbank —\nTR70 0011 1000 0000 0118 5102 59\nÖmer Faruk Sancak"
 )
+
 #--------------------------------------------------------------#
-{"ettn": "b40c16ae-8509-434e-bd6f-894459372134"}
+
+FaturaOlustur(ettn='8cb401e3-ca6d-442a-8389-894459372134')
 ```
 
 ```python
 faturalar = portal.faturalari_getir(
     baslangic_tarihi = "01/05/2023",
     bitis_tarihi     = "28/05/2023"
 )
+
 #--------------------------------------------------------------#
+
 [
-    {
-        'belgeNumarasi': 'GIB2023000002672',
-        'aliciVknTckn': '16045751784',
-        'aliciUnvanAdSoyad': 'Sercan AYDIN',
-        'belgeTarihi': '28-05-2023',
-        'belgeTuru': 'FATURA',
-        'onayDurumu': 'Onaylanmadı',
-        'ettn': '0c111c74-fcd4-11ed-8026-3ae56703837b'
-    },
-    {
-        'belgeNumarasi': 'GIB2023000002673',
-        'aliciVknTckn': '16045751784',
-        'aliciUnvanAdSoyad': 'Sercan AYDIN',
-        'belgeTarihi': '28-05-2023',
-        'belgeTuru': 'FATURA',
-        'onayDurumu': 'Silinmiş',
-        'ettn': '234baa8e-fcd5-11ed-827f-3ae56703837b'
-    }
+    Fatura(
+        belgeNumarasi='GIB2023000002672',
+        aliciVknTckn='16045751784',
+        aliciUnvanAdSoyad='Sercan AYDIN',
+        belgeTarihi='29-05-2023',
+        belgeTuru='FATURA',
+        onayDurumu='Silinmiş',
+        ettn='7386c1dc-8a23-4d46-9c8d-de3512b630b4'
+    ),
+    Fatura(
+        belgeNumarasi='GIB2023000001918',
+        aliciVknTckn='16045751784',
+        aliciUnvanAdSoyad='Sercan AYDIN',
+        belgeTarihi='29-05-2023',
+        belgeTuru='FATURA',
+        onayDurumu='Onaylanmadı',
+        ettn='2ef98bfa-8787-4429-a1fa-a0514560e7eb'
+    ),
+    Fatura(
+        belgeNumarasi='GIB2023000001919',
+        aliciVknTckn='16045751784',
+        aliciUnvanAdSoyad='Sercan AYDIN',
+        belgeTarihi='29-05-2023',
+        belgeTuru='FATURA',
+        onayDurumu='Onaylandı',
+        ettn='8cb401e3-ca6d-442a-8389-c4d87c9eb67c'
+    )
 ]
 ```
 
 ```python
 html_fatura = portal.fatura_html(
-    ettn        = faturalar[0].get("ettn")
-    onay_durumu = faturalar[0].get("onayDurumu")
+    ettn        = faturalar[0].ettn
+    onay_durumu = faturalar[0].onayDurumu
 )
 
-with open(f"{faturalar[0].get("aliciUnvanAdSoyad")}.html", "w", encoding="utf-8") as dosya:
+with open(f"{faturalar[0].aliciUnvanAdSoyad}.html", "w", encoding="utf-8") as dosya:
     dosya.write(html_fatura)
 ```
 
 ```python
 portal.fatura_sil(
     faturalar = [faturalar[0], faturalar[1]]
     aciklama  = "Fatura silindi."
 )
+
 #--------------------------------------------------------------#
-2 fatura başarıyla silindi.
+
+FaturaSil(mesaj='2 fatura başarıyla silindi.')
 ```
 
 ```python
-oid = portal.gib_imza()
-portal.gib_sms_onay(faturalar[3], oid, input("SMS Doğrulama Kodu: "))
+imza = portal.gib_imza()
+portal.gib_sms_onay(faturalar[3], imza.oid, input("SMS Doğrulama Kodu: "))
+
+#--------------------------------------------------------------#
+
+GibSMSOnay(mesaj='SMS şifreniz doğrulandı, işlem başarılı.')
 ```
 
 ```python
 portal.cikis_yap()
 ```
 
 ## 🌐 Telif Hakkı ve Lisans
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: eArsivPortal Version: 0.0.7 Summary: GÄ°B e-ArÅiv
+Metadata-Version: 2.1 Name: eArsivPortal Version: 0.0.8 Summary: GÄ°B e-ArÅiv
 Portal e-Fatura OluÅturucu Home-page: https://github.com/keyiflerolsun/
 eArsivPortal Author: keyiflerolsun Author-email: keyiflerolsun@gmail.com
 License: GPLv3+ Keywords: eArsivPortal,KekikAkademi,keyiflerolsun Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: GNU General Public License v3 or later (GPLv3+) Classifier: Programming
 Language :: Python :: 3 Requires-Python: >=3.10 Description-Content-Type: text/
 markdown License-File: LICENSE # ð§¾ eArsivPortal [![Boyut](https://
@@ -34,48 +34,52 @@
 keyiflerolsun/) ## ð Kurulum ### [https://raw.githubusercontent.com/
 keyiflerolsun/eArsivPortal/main/.github/icons/pypi.svg] PyPI ```bash #
 YÃ¼klemek pip install eArsivPortal # GÃ¼ncellemek pip install -U eArsivPortal
 ``` ## ð KullanÄ±m ### [https://raw.githubusercontent.com/keyiflerolsun/
 eArsivPortal/main/.github/icons/python.svg] Lib ```python from eArsivPortal
 import eArsivPortal portal = eArsivPortal( kullanici_kodu = "33333301", sifre =
 "1", test_modu = True ) ``` ```python portal.bilgilerim() #--------------------
-------------------------------------------# { "vknTckn": "3333333301", "unvan":
-"HOSAM ALDEEN ABUSHAWER TÄ°CARÄ° GÄ°RÄ°ÅÄ°MÄ°", "ad": "", "soyad": "",
-"cadde": "Åehit yusuf bey", "apartmanAdi": "yÄ±ldÄ±z", "apartmanNo": "8",
-"kapiNo": "2", "kasaba": "ortakapÄ±", "ilce": "Merkez", "il": "Kars",
-"postaKodu": "36000", "ulke": "TÃ¼rkiye", "telNo": "05524775288", "faksNo": "",
-"ePostaAdresi": "", "webSitesiAdresi": "", "vergiDairesi": "kars", "sicilNo":
-"8729", "isMerkezi": "", "mersisNo": "9962438036000001" } ``` ```python
-portal.kisi_getir(vkn_veya_tckn="3333333301") #--------------------------------
-------------------------------# { "unvan":"HOSAM ALDEEN ABUSHAWER TÄ°CARÄ°
-GÄ°RÄ°ÅÄ°MÄ°", "adi":"", "soyadi":"", "vergiDairesi":"kars" } ``` ```python
+------------------------------------------# Bilgilerim( vknTckn='3333333315',
+unvan='XYZ Yaz', ad='', soyad='', cadde='Sahil yolu', apartmanAdi='Dali
+Ã§Ä±tÄ±r pide', apartmanNo='12', kapiNo='3', kasaba='adana', ilce='GEMLÄ°K',
+il='Antalya', postaKodu='16000', ulke='TÃ¼rkiye', telNo='053982456665',
+faksNo='', ePostaAdresi='info@vekamp.com', webSitesiAdresi='',
+vergiDairesi='orhangazi vergi dairesi', sicilNo='00000000000000', isMerkezi='',
+mersisNo='' ) ``` ```python portal.kisi_getir(vkn_veya_tckn="3333333301") #----
+----------------------------------------------------------# Kisi( unvan='XYZ
+Yaz', adi='', soyadi='', vergiDairesi='orhangazi vergi dairesi' ) ``` ```python
 portal.fatura_olustur( tarih:str = "07/10/1995", saat:str = "14:28:37",
 vkn_veya_tckn:str = "11111111111", ad:str = "Ãmer Faruk", soyad:str =
 "Sancak", unvan:str = "", vergi_dairesi:str = "", urun_adi:str = "Python
 YazÄ±lÄ±m Hizmeti", fiyat:int | float = 100, fatura_notu:str = "â QNB
 Finansbank â\nTR70 0011 1000 0000 0118 5102 59\nÃmer Faruk Sancak" ) #------
---------------------------------------------------------# {"ettn": "b40c16ae-
-8509-434e-bd6f-894459372134"} ``` ```python faturalar = portal.faturalari_getir
-( baslangic_tarihi = "01/05/2023", bitis_tarihi = "28/05/2023" ) #-------------
--------------------------------------------------# [ { 'belgeNumarasi':
-'GIB2023000002672', 'aliciVknTckn': '16045751784', 'aliciUnvanAdSoyad': 'Sercan
-AYDIN', 'belgeTarihi': '28-05-2023', 'belgeTuru': 'FATURA', 'onayDurumu':
-'OnaylanmadÄ±', 'ettn': '0c111c74-fcd4-11ed-8026-3ae56703837b' },
-{ 'belgeNumarasi': 'GIB2023000002673', 'aliciVknTckn': '16045751784',
-'aliciUnvanAdSoyad': 'Sercan AYDIN', 'belgeTarihi': '28-05-2023', 'belgeTuru':
-'FATURA', 'onayDurumu': 'SilinmiÅ', 'ettn': '234baa8e-fcd5-11ed-827f-
-3ae56703837b' } ] ``` ```python html_fatura = portal.fatura_html( ettn =
-faturalar[0].get("ettn") onay_durumu = faturalar[0].get("onayDurumu") ) with
-open(f"{faturalar[0].get("aliciUnvanAdSoyad")}.html", "w", encoding="utf-8") as
-dosya: dosya.write(html_fatura) ``` ```python portal.fatura_sil( faturalar =
-[faturalar[0], faturalar[1]] aciklama = "Fatura silindi." ) #------------------
---------------------------------------------# 2 fatura baÅarÄ±yla silindi. ```
-```python oid = portal.gib_imza() portal.gib_sms_onay(faturalar[3], oid, input
-("SMS DoÄrulama Kodu: ")) ``` ```python portal.cikis_yap() ``` ## ð Telif
-HakkÄ± ve Lisans * *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/
+--------------------------------------------------------# FaturaOlustur
+(ettn='8cb401e3-ca6d-442a-8389-894459372134') ``` ```python faturalar =
+portal.faturalari_getir( baslangic_tarihi = "01/05/2023", bitis_tarihi = "28/
+05/2023" ) #--------------------------------------------------------------#
+[ Fatura( belgeNumarasi='GIB2023000002672', aliciVknTckn='16045751784',
+aliciUnvanAdSoyad='Sercan AYDIN', belgeTarihi='29-05-2023', belgeTuru='FATURA',
+onayDurumu='SilinmiÅ', ettn='7386c1dc-8a23-4d46-9c8d-de3512b630b4' ), Fatura
+( belgeNumarasi='GIB2023000001918', aliciVknTckn='16045751784',
+aliciUnvanAdSoyad='Sercan AYDIN', belgeTarihi='29-05-2023', belgeTuru='FATURA',
+onayDurumu='OnaylanmadÄ±', ettn='2ef98bfa-8787-4429-a1fa-a0514560e7eb' ),
+Fatura( belgeNumarasi='GIB2023000001919', aliciVknTckn='16045751784',
+aliciUnvanAdSoyad='Sercan AYDIN', belgeTarihi='29-05-2023', belgeTuru='FATURA',
+onayDurumu='OnaylandÄ±', ettn='8cb401e3-ca6d-442a-8389-c4d87c9eb67c' ) ] ```
+```python html_fatura = portal.fatura_html( ettn = faturalar[0].ettn
+onay_durumu = faturalar[0].onayDurumu ) with open(f"{faturalar
+[0].aliciUnvanAdSoyad}.html", "w", encoding="utf-8") as dosya: dosya.write
+(html_fatura) ``` ```python portal.fatura_sil( faturalar = [faturalar[0],
+faturalar[1]] aciklama = "Fatura silindi." ) #---------------------------------
+-----------------------------# FaturaSil(mesaj='2 fatura baÅarÄ±yla silindi.')
+``` ```python imza = portal.gib_imza() portal.gib_sms_onay(faturalar[3],
+imza.oid, input("SMS DoÄrulama Kodu: ")) #------------------------------------
+--------------------------# GibSMSOnay(mesaj='SMS Åifreniz doÄrulandÄ±,
+iÅlem baÅarÄ±lÄ±.') ``` ```python portal.cikis_yap() ``` ## ð Telif HakkÄ±
+ve Lisans * *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/
 keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007]
 (https://github.com/keyiflerolsun/eArsivPortal/blob/master/LICENSE)
 *KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ## â»ï¸ Ä°letiÅim *Benimle
 iletiÅime geÃ§mek isterseniz, **Telegram**'dan mesaj gÃ¶ndermekten
 Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ## ð¸ BaÄÄ±Å Yap **
 [âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)** *** > **
 [@KekikAkademi](https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
```

### Comparing `eArsivPortal-0.0.7/README.md` & `eArsivPortal-0.0.8/eArsivPortal.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: eArsivPortal
+Version: 0.0.8
+Summary: GİB e-Arşiv Portal e-Fatura Oluşturucu
+Home-page: https://github.com/keyiflerolsun/eArsivPortal
+Author: keyiflerolsun
+Author-email: keyiflerolsun@gmail.com
+License: GPLv3+
+Keywords: eArsivPortal,KekikAkademi,keyiflerolsun
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # 🧾 eArsivPortal
 
 [![Boyut](https://img.shields.io/github/repo-size/keyiflerolsun/eArsivPortal?logo=git&logoColor=white&label=Boyut)](#)
 [![Görüntülenme](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/keyiflerolsun/eArsivPortal&title=Görüntülenme)](#)
 <a href="https://KekikAkademi.org/Kahve" target="_blank"><img src="https://img.shields.io/badge/☕️-Kahve Ismarla-ffdd00" title="☕️ Kahve Ismarla" style="padding-left:5px;"></a>
 
 [![PyPI Yükleyici](https://img.shields.io/github/actions/workflow/status/keyiflerolsun/eArsivPortal/PyPI.yml?label=PyPI%20Y%C3%BCkleyici&logo=github)](https://github.com/keyiflerolsun/eArsivPortal/actions/workflows/PyPI.yml)
@@ -45,49 +61,53 @@
     sifre          = "1",
     test_modu      = True
 )
 ```
 
 ```python
 portal.bilgilerim()
+
 #--------------------------------------------------------------#
-{
-    "vknTckn": "3333333301",
-    "unvan": "HOSAM ALDEEN ABUSHAWER TİCARİ GİRİŞİMİ",
-    "ad": "",
-    "soyad": "",
-    "cadde": "şehit yusuf bey",
-    "apartmanAdi": "yıldız",
-    "apartmanNo": "8",
-    "kapiNo": "2",
-    "kasaba": "ortakapı",
-    "ilce": "Merkez",
-    "il": "Kars",
-    "postaKodu": "36000",
-    "ulke": "Türkiye",
-    "telNo": "05524775288",
-    "faksNo": "",
-    "ePostaAdresi": "",
-    "webSitesiAdresi": "",
-    "vergiDairesi": "kars",
-    "sicilNo": "8729",
-    "isMerkezi": "",
-    "mersisNo": "9962438036000001"
-}
+
+Bilgilerim(
+    vknTckn='3333333315',
+    unvan='XYZ Yaz',
+    ad='',
+    soyad='',
+    cadde='Sahil yolu',
+    apartmanAdi='Dali çıtır pide',
+    apartmanNo='12',
+    kapiNo='3',
+    kasaba='adana',
+    ilce='GEMLİK',
+    il='Antalya',
+    postaKodu='16000',
+    ulke='Türkiye',
+    telNo='053982456665',
+    faksNo='',
+    ePostaAdresi='info@vekamp.com',
+    webSitesiAdresi='',
+    vergiDairesi='orhangazi vergi dairesi',
+    sicilNo='00000000000000',
+    isMerkezi='',
+    mersisNo=''
+)
 ```
 
 ```python
 portal.kisi_getir(vkn_veya_tckn="3333333301")
+
 #--------------------------------------------------------------#
-{
-    "unvan":"HOSAM ALDEEN ABUSHAWER TİCARİ GİRİŞİMİ",
-    "adi":"",
-    "soyadi":"",
-    "vergiDairesi":"kars"
-}
+
+Kisi(
+    unvan='XYZ Yaz',
+    adi='',
+    soyadi='',
+    vergiDairesi='orhangazi vergi dairesi'
+)
 ```
 
 ```python
 portal.fatura_olustur(
     tarih:str         = "07/10/1995",
     saat:str          = "14:28:37",
     vkn_veya_tckn:str = "11111111111",
@@ -95,68 +115,87 @@
     soyad:str         = "Sancak",
     unvan:str         = "",
     vergi_dairesi:str = "",
     urun_adi:str      = "Python Yazılım Hizmeti",
     fiyat:int | float = 100,
     fatura_notu:str   = "— QNB Finansbank —\nTR70 0011 1000 0000 0118 5102 59\nÖmer Faruk Sancak"
 )
+
 #--------------------------------------------------------------#
-{"ettn": "b40c16ae-8509-434e-bd6f-894459372134"}
+
+FaturaOlustur(ettn='8cb401e3-ca6d-442a-8389-894459372134')
 ```
 
 ```python
 faturalar = portal.faturalari_getir(
     baslangic_tarihi = "01/05/2023",
     bitis_tarihi     = "28/05/2023"
 )
+
 #--------------------------------------------------------------#
+
 [
-    {
-        'belgeNumarasi': 'GIB2023000002672',
-        'aliciVknTckn': '16045751784',
-        'aliciUnvanAdSoyad': 'Sercan AYDIN',
-        'belgeTarihi': '28-05-2023',
-        'belgeTuru': 'FATURA',
-        'onayDurumu': 'Onaylanmadı',
-        'ettn': '0c111c74-fcd4-11ed-8026-3ae56703837b'
-    },
-    {
-        'belgeNumarasi': 'GIB2023000002673',
-        'aliciVknTckn': '16045751784',
-        'aliciUnvanAdSoyad': 'Sercan AYDIN',
-        'belgeTarihi': '28-05-2023',
-        'belgeTuru': 'FATURA',
-        'onayDurumu': 'Silinmiş',
-        'ettn': '234baa8e-fcd5-11ed-827f-3ae56703837b'
-    }
+    Fatura(
+        belgeNumarasi='GIB2023000002672',
+        aliciVknTckn='16045751784',
+        aliciUnvanAdSoyad='Sercan AYDIN',
+        belgeTarihi='29-05-2023',
+        belgeTuru='FATURA',
+        onayDurumu='Silinmiş',
+        ettn='7386c1dc-8a23-4d46-9c8d-de3512b630b4'
+    ),
+    Fatura(
+        belgeNumarasi='GIB2023000001918',
+        aliciVknTckn='16045751784',
+        aliciUnvanAdSoyad='Sercan AYDIN',
+        belgeTarihi='29-05-2023',
+        belgeTuru='FATURA',
+        onayDurumu='Onaylanmadı',
+        ettn='2ef98bfa-8787-4429-a1fa-a0514560e7eb'
+    ),
+    Fatura(
+        belgeNumarasi='GIB2023000001919',
+        aliciVknTckn='16045751784',
+        aliciUnvanAdSoyad='Sercan AYDIN',
+        belgeTarihi='29-05-2023',
+        belgeTuru='FATURA',
+        onayDurumu='Onaylandı',
+        ettn='8cb401e3-ca6d-442a-8389-c4d87c9eb67c'
+    )
 ]
 ```
 
 ```python
 html_fatura = portal.fatura_html(
-    ettn        = faturalar[0].get("ettn")
-    onay_durumu = faturalar[0].get("onayDurumu")
+    ettn        = faturalar[0].ettn
+    onay_durumu = faturalar[0].onayDurumu
 )
 
-with open(f"{faturalar[0].get("aliciUnvanAdSoyad")}.html", "w", encoding="utf-8") as dosya:
+with open(f"{faturalar[0].aliciUnvanAdSoyad}.html", "w", encoding="utf-8") as dosya:
     dosya.write(html_fatura)
 ```
 
 ```python
 portal.fatura_sil(
     faturalar = [faturalar[0], faturalar[1]]
     aciklama  = "Fatura silindi."
 )
+
 #--------------------------------------------------------------#
-2 fatura başarıyla silindi.
+
+FaturaSil(mesaj='2 fatura başarıyla silindi.')
 ```
 
 ```python
-oid = portal.gib_imza()
-portal.gib_sms_onay(faturalar[3], oid, input("SMS Doğrulama Kodu: "))
+imza = portal.gib_imza()
+portal.gib_sms_onay(faturalar[3], imza.oid, input("SMS Doğrulama Kodu: "))
+
+#--------------------------------------------------------------#
+
+GibSMSOnay(mesaj='SMS şifreniz doğrulandı, işlem başarılı.')
 ```
 
 ```python
 portal.cikis_yap()
 ```
 
 ## 🌐 Telif Hakkı ve Lisans
@@ -170,8 +209,8 @@
 
 ## 💸 Bağış Yap
 
 **[☕️ Kahve Ismarla](https://KekikAkademi.org/Kahve)**
 
 ***
 
-> **[@KekikAkademi](https://t.me/KekikAkademi)** *için yazılmıştır..*
+> **[@KekikAkademi](https://t.me/KekikAkademi)** *için yazılmıştır..*
```

#### html2text {}

```diff
@@ -1,14 +1,21 @@
-# ð§¾ eArsivPortal [![Boyut](https://img.shields.io/github/repo-size/
-keyiflerolsun/eArsivPortal?logo=git&logoColor=white&label=Boyut)](#) [!
-[GÃ¶rÃ¼ntÃ¼lenme](https://hits.seeyoufarm.com/api/count/incr/
-badge.svg?url=https://github.com/keyiflerolsun/
-eArsivPortal&title=GÃ¶rÃ¼ntÃ¼lenme)](#) [https://img.shields.io/badge/âï¸-
-Kahve_Ismarla-ffdd00] [![PyPI YÃ¼kleyici](https://img.shields.io/github/
-actions/workflow/status/keyiflerolsun/eArsivPortal/
+Metadata-Version: 2.1 Name: eArsivPortal Version: 0.0.8 Summary: GÄ°B e-ArÅiv
+Portal e-Fatura OluÅturucu Home-page: https://github.com/keyiflerolsun/
+eArsivPortal Author: keyiflerolsun Author-email: keyiflerolsun@gmail.com
+License: GPLv3+ Keywords: eArsivPortal,KekikAkademi,keyiflerolsun Classifier:
+Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
+:: GNU General Public License v3 or later (GPLv3+) Classifier: Programming
+Language :: Python :: 3 Requires-Python: >=3.10 Description-Content-Type: text/
+markdown License-File: LICENSE # ð§¾ eArsivPortal [![Boyut](https://
+img.shields.io/github/repo-size/keyiflerolsun/
+eArsivPortal?logo=git&logoColor=white&label=Boyut)](#) [![GÃ¶rÃ¼ntÃ¼lenme]
+(https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/
+keyiflerolsun/eArsivPortal&title=GÃ¶rÃ¼ntÃ¼lenme)](#) [https://img.shields.io/
+badge/âï¸-Kahve_Ismarla-ffdd00] [![PyPI YÃ¼kleyici](https://img.shields.io/
+github/actions/workflow/status/keyiflerolsun/eArsivPortal/
 PyPI.yml?label=PyPI%20Y%C3%BCkleyici&logo=github)](https://github.com/
 keyiflerolsun/eArsivPortal/actions/workflows/PyPI.yml) [![PyPI](https://
 img.shields.io/pypi/v/eArsivPortal?logo=pypi&logoColor=white&label=PyPI)]
 (https://pypi.org/project/eArsivPortal) [![PyPI - YÃ¼klenme](https://
 img.shields.io/pypi/dm/eArsivPortal?logo=pypi&logoColor=white&label=YÃ¼klenme)]
 (https://pypi.org/project/eArsivPortal) [![PyPI - Wheel](https://
 img.shields.io/pypi/wheel/eArsivPortal?logo=pypi&logoColor=white&label=Wheel)]
@@ -27,48 +34,52 @@
 keyiflerolsun/) ## ð Kurulum ### [https://raw.githubusercontent.com/
 keyiflerolsun/eArsivPortal/main/.github/icons/pypi.svg] PyPI ```bash #
 YÃ¼klemek pip install eArsivPortal # GÃ¼ncellemek pip install -U eArsivPortal
 ``` ## ð KullanÄ±m ### [https://raw.githubusercontent.com/keyiflerolsun/
 eArsivPortal/main/.github/icons/python.svg] Lib ```python from eArsivPortal
 import eArsivPortal portal = eArsivPortal( kullanici_kodu = "33333301", sifre =
 "1", test_modu = True ) ``` ```python portal.bilgilerim() #--------------------
-------------------------------------------# { "vknTckn": "3333333301", "unvan":
-"HOSAM ALDEEN ABUSHAWER TÄ°CARÄ° GÄ°RÄ°ÅÄ°MÄ°", "ad": "", "soyad": "",
-"cadde": "Åehit yusuf bey", "apartmanAdi": "yÄ±ldÄ±z", "apartmanNo": "8",
-"kapiNo": "2", "kasaba": "ortakapÄ±", "ilce": "Merkez", "il": "Kars",
-"postaKodu": "36000", "ulke": "TÃ¼rkiye", "telNo": "05524775288", "faksNo": "",
-"ePostaAdresi": "", "webSitesiAdresi": "", "vergiDairesi": "kars", "sicilNo":
-"8729", "isMerkezi": "", "mersisNo": "9962438036000001" } ``` ```python
-portal.kisi_getir(vkn_veya_tckn="3333333301") #--------------------------------
-------------------------------# { "unvan":"HOSAM ALDEEN ABUSHAWER TÄ°CARÄ°
-GÄ°RÄ°ÅÄ°MÄ°", "adi":"", "soyadi":"", "vergiDairesi":"kars" } ``` ```python
+------------------------------------------# Bilgilerim( vknTckn='3333333315',
+unvan='XYZ Yaz', ad='', soyad='', cadde='Sahil yolu', apartmanAdi='Dali
+Ã§Ä±tÄ±r pide', apartmanNo='12', kapiNo='3', kasaba='adana', ilce='GEMLÄ°K',
+il='Antalya', postaKodu='16000', ulke='TÃ¼rkiye', telNo='053982456665',
+faksNo='', ePostaAdresi='info@vekamp.com', webSitesiAdresi='',
+vergiDairesi='orhangazi vergi dairesi', sicilNo='00000000000000', isMerkezi='',
+mersisNo='' ) ``` ```python portal.kisi_getir(vkn_veya_tckn="3333333301") #----
+----------------------------------------------------------# Kisi( unvan='XYZ
+Yaz', adi='', soyadi='', vergiDairesi='orhangazi vergi dairesi' ) ``` ```python
 portal.fatura_olustur( tarih:str = "07/10/1995", saat:str = "14:28:37",
 vkn_veya_tckn:str = "11111111111", ad:str = "Ãmer Faruk", soyad:str =
 "Sancak", unvan:str = "", vergi_dairesi:str = "", urun_adi:str = "Python
 YazÄ±lÄ±m Hizmeti", fiyat:int | float = 100, fatura_notu:str = "â QNB
 Finansbank â\nTR70 0011 1000 0000 0118 5102 59\nÃmer Faruk Sancak" ) #------
---------------------------------------------------------# {"ettn": "b40c16ae-
-8509-434e-bd6f-894459372134"} ``` ```python faturalar = portal.faturalari_getir
-( baslangic_tarihi = "01/05/2023", bitis_tarihi = "28/05/2023" ) #-------------
--------------------------------------------------# [ { 'belgeNumarasi':
-'GIB2023000002672', 'aliciVknTckn': '16045751784', 'aliciUnvanAdSoyad': 'Sercan
-AYDIN', 'belgeTarihi': '28-05-2023', 'belgeTuru': 'FATURA', 'onayDurumu':
-'OnaylanmadÄ±', 'ettn': '0c111c74-fcd4-11ed-8026-3ae56703837b' },
-{ 'belgeNumarasi': 'GIB2023000002673', 'aliciVknTckn': '16045751784',
-'aliciUnvanAdSoyad': 'Sercan AYDIN', 'belgeTarihi': '28-05-2023', 'belgeTuru':
-'FATURA', 'onayDurumu': 'SilinmiÅ', 'ettn': '234baa8e-fcd5-11ed-827f-
-3ae56703837b' } ] ``` ```python html_fatura = portal.fatura_html( ettn =
-faturalar[0].get("ettn") onay_durumu = faturalar[0].get("onayDurumu") ) with
-open(f"{faturalar[0].get("aliciUnvanAdSoyad")}.html", "w", encoding="utf-8") as
-dosya: dosya.write(html_fatura) ``` ```python portal.fatura_sil( faturalar =
-[faturalar[0], faturalar[1]] aciklama = "Fatura silindi." ) #------------------
---------------------------------------------# 2 fatura baÅarÄ±yla silindi. ```
-```python oid = portal.gib_imza() portal.gib_sms_onay(faturalar[3], oid, input
-("SMS DoÄrulama Kodu: ")) ``` ```python portal.cikis_yap() ``` ## ð Telif
-HakkÄ± ve Lisans * *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/
+--------------------------------------------------------# FaturaOlustur
+(ettn='8cb401e3-ca6d-442a-8389-894459372134') ``` ```python faturalar =
+portal.faturalari_getir( baslangic_tarihi = "01/05/2023", bitis_tarihi = "28/
+05/2023" ) #--------------------------------------------------------------#
+[ Fatura( belgeNumarasi='GIB2023000002672', aliciVknTckn='16045751784',
+aliciUnvanAdSoyad='Sercan AYDIN', belgeTarihi='29-05-2023', belgeTuru='FATURA',
+onayDurumu='SilinmiÅ', ettn='7386c1dc-8a23-4d46-9c8d-de3512b630b4' ), Fatura
+( belgeNumarasi='GIB2023000001918', aliciVknTckn='16045751784',
+aliciUnvanAdSoyad='Sercan AYDIN', belgeTarihi='29-05-2023', belgeTuru='FATURA',
+onayDurumu='OnaylanmadÄ±', ettn='2ef98bfa-8787-4429-a1fa-a0514560e7eb' ),
+Fatura( belgeNumarasi='GIB2023000001919', aliciVknTckn='16045751784',
+aliciUnvanAdSoyad='Sercan AYDIN', belgeTarihi='29-05-2023', belgeTuru='FATURA',
+onayDurumu='OnaylandÄ±', ettn='8cb401e3-ca6d-442a-8389-c4d87c9eb67c' ) ] ```
+```python html_fatura = portal.fatura_html( ettn = faturalar[0].ettn
+onay_durumu = faturalar[0].onayDurumu ) with open(f"{faturalar
+[0].aliciUnvanAdSoyad}.html", "w", encoding="utf-8") as dosya: dosya.write
+(html_fatura) ``` ```python portal.fatura_sil( faturalar = [faturalar[0],
+faturalar[1]] aciklama = "Fatura silindi." ) #---------------------------------
+-----------------------------# FaturaSil(mesaj='2 fatura baÅarÄ±yla silindi.')
+``` ```python imza = portal.gib_imza() portal.gib_sms_onay(faturalar[3],
+imza.oid, input("SMS DoÄrulama Kodu: ")) #------------------------------------
+--------------------------# GibSMSOnay(mesaj='SMS Åifreniz doÄrulandÄ±,
+iÅlem baÅarÄ±lÄ±.') ``` ```python portal.cikis_yap() ``` ## ð Telif HakkÄ±
+ve Lisans * *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/
 keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007]
 (https://github.com/keyiflerolsun/eArsivPortal/blob/master/LICENSE)
 *KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ## â»ï¸ Ä°letiÅim *Benimle
 iletiÅime geÃ§mek isterseniz, **Telegram**'dan mesaj gÃ¶ndermekten
 Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ## ð¸ BaÄÄ±Å Yap **
 [âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)** *** > **
 [@KekikAkademi](https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
```

### Comparing `eArsivPortal-0.0.7/eArsivPortal/Core/__init__.py` & `eArsivPortal-0.0.8/eArsivPortal/Core/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from uuid     import uuid4
 from parsel   import Selector
 from .Hatalar import GirisYapilmadi, OturumSuresiDoldu, eArsivPortalHatasi
 
 from datetime import datetime
 from pytz     import timezone
 
+from pydantic import create_model, BaseModel
+
 class eArsivPortal:
     def __init__(self, kullanici_kodu:str="33333315", sifre:str="1", test_modu:bool=True):
 
         self.kullanici_kodu = kullanici_kodu
         self.sifre          = sifre
         self.test_modu      = test_modu
 
@@ -29,15 +31,20 @@
         self.oturum.headers.update({
             "User-Agent" : "https://github.com/keyiflerolsun/eArsivPortal"
         })
 
         self.token = None
         self.giris_yap()
 
-    def __istek_ayristir(self, istek:Response, veri:dict) -> dict | Exception:
+    def __nesne_ver(self, isim, veri) -> BaseModel:
+        __nesne = create_model(isim, **veri)
+
+        return __nesne(**veri)
+
+    def __istek_ayristir(self, istek:Response, veri:dict) -> dict | str | Exception:
         if istek.status_code != 200 or veri.get("error"):
             veri_mesaj = veri["messages"][0]
             hata_metni = veri_mesaj["text"] if isinstance(veri_mesaj, dict) else veri_mesaj
 
             if "Oturum zamanaşımına uğradı" in hata_metni:
                 raise OturumSuresiDoldu(hata_metni)
 
@@ -97,145 +104,166 @@
             veri = istek.json()
 
             return self.__istek_ayristir(istek, veri)
         except OturumSuresiDoldu:
             self.__giris_yap(self.kullanici_kodu, self.sifre)
             return self.__kod_calistir(komut, jp)
 
-    def bilgilerim(self) -> dict:
+    def bilgilerim(self) -> BaseModel:
         istek = self.__kod_calistir(
             komut = self.komutlar.KULLANICI_BILGILERI_GETIR,
             jp    = {}
         )
+        veri  = istek.get("data")
 
-        return istek.get("data")
+        return self.__nesne_ver("Bilgilerim", veri)
 
-    def kisi_getir(self, vkn_veya_tckn:str) -> dict:
+    def kisi_getir(self, vkn_veya_tckn:str) -> BaseModel:
         try:
             istek = self.__kod_calistir(
                 komut = self.komutlar.MERNISTEN_BILGILERI_GETIR,
                 jp    = {
-                    "vknTckn" : vkn_veya_tckn
+                    "vknTcknn" : vkn_veya_tckn
                 }
             )
+            veri  = istek.get("data")
         except Exception:
-            return {}
+            veri  = {"unvan": None, "adi": None, "soyadi": None, "vergiDairesi": None}
 
-        return istek.get("data")
+        return self.__nesne_ver("Kisi", veri)
 
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
-    ) -> dict[str, str | None]:
+    ) -> BaseModel:
         kisi_bilgi = self.kisi_getir(vkn_veya_tckn)
 
         fatura = fatura_ver(
             tarih         = tarih or datetime.now(timezone("Turkey")).strftime("%d/%m/%Y"),
             saat          = saat,
             vkn_veya_tckn = vkn_veya_tckn,
-            ad            = kisi_bilgi.get("adi") or ad,
-            soyad         = kisi_bilgi.get("soyadi") or soyad,
-            unvan         = kisi_bilgi.get("unvan") or unvan,
-            vergi_dairesi = kisi_bilgi.get("vergiDairesi") or vergi_dairesi,
+            ad            = kisi_bilgi.adi or ad,
+            soyad         = kisi_bilgi.soyadi or soyad,
+            unvan         = kisi_bilgi.unvan or unvan,
+            vergi_dairesi = kisi_bilgi.vergiDairesi or vergi_dairesi,
             urun_adi      = urun_adi,
             fiyat         = fiyat,
             fatura_notu   = fatura_notu
         )
 
         istek = self.__kod_calistir(
             komut = self.komutlar.FATURA_OLUSTUR,
             jp    = fatura
         )
 
+        ettn = None
         if "Faturanız başarıyla oluşturulmuştur." in istek.get("data"):
-            return {"ettn": fatura.get("faturaUuid")}
+            ettn = fatura.get("faturaUuid")
 
-        return {"ettn": None}
+        return self.__nesne_ver("FaturaOlustur", {"ettn": ettn})
 
-    def faturalari_getir(self, baslangic_tarihi:str="01/05/2023", bitis_tarihi:str="28/05/2023") -> list[dict]:
+    def faturalari_getir(self, baslangic_tarihi:str="01/05/2023", bitis_tarihi:str="28/05/2023") -> list[BaseModel]:
         istek = self.__kod_calistir(
             komut = self.komutlar.TASLAKLARI_GETIR,
             jp    = {
                 "baslangic" : baslangic_tarihi or datetime.now(timezone("Turkey")).strftime("%d/%m/%Y"),
                 "bitis"     : bitis_tarihi or datetime.now(timezone("Turkey")).strftime("%d/%m/%Y"),
                 "hangiTip"  :"5000/30000",
                 "table"     : []
             }
         )
+        veri  = istek.get("data")
 
-        return istek.get("data")
+        return [self.__nesne_ver("Fatura", fatura) for fatura in veri]
 
     def fatura_html(self, ettn:str, onay_durumu:str) -> str:
         istek = self.__kod_calistir(
             komut = self.komutlar.FATURA_GOSTER,
             jp    = {
                 "ettn"       : ettn,
                 "onayDurumu" : onay_durumu
             }
         )
+        veri  = istek.get("data")
 
-        secici = Selector(istek.get("data"))
+        secici = Selector(veri)
 
         for tr in secici.xpath("//tr"):
             bos_tdler = tr.xpath(".//td[normalize-space(.)='\xa0']")
 
             if len(bos_tdler) == len(tr.xpath(".//td")):
                 tr_element = tr.root
                 tr_element.getparent().remove(tr_element)
 
         return secici.extract()
 
-    def fatura_sil(self, faturalar:list[dict] | dict, aciklama:str):
+    def __fatura_ver(self, faturalar) -> list[dict] | Exception:
+        if not isinstance(faturalar, list):
+            faturalar = [faturalar]
+
+        payload = []
+        for fatura in faturalar:
+            if isinstance(fatura, dict):
+                payload.append(fatura)
+            elif isinstance(fatura, list):
+                payload.extend(fatura)
+            else:
+                payload.append(fatura.dict())
+
+        return payload
+
+    def fatura_sil(self, faturalar:list[dict] | dict, aciklama:str) -> BaseModel:
         istek = self.__kod_calistir(
             komut = self.komutlar.FATURA_SIL,
             jp    = {
-                "silinecekler" : [faturalar] if isinstance(faturalar, dict) else faturalar,
+                "silinecekler" : self.__fatura_ver(faturalar),
                 "aciklama"     : aciklama
             }
         )
 
-        return istek.get("data")
+        return self.__nesne_ver("FaturaSil", {"mesaj": istek.get("data")})
 
-    def gib_imza(self) -> dict[str, str | None]:
+    def gib_imza(self) -> BaseModel:
         telefon_istek = self.__kod_calistir(
             komut = self.komutlar.TELEFONNO_SORGULA,
             jp    = {}
         )
         telefon_veri = telefon_istek.get("data")
         telefon_no   = telefon_veri.get("telefon")
         if not telefon_no:
-            return {"oid": None}
+            return self.__nesne_ver("GibImza", {"oid": None})
 
         sms_gonder = self.__kod_calistir(
             komut = self.komutlar.SMSSIFRE_GONDER,
             jp    = {
                 "CEPTEL"  : telefon_no,
                 "KCEPTEL" : False,
                 "TIP"     : ""
             }
         )
 
-        return sms_gonder.get("data")
+        return self.__nesne_ver("GibImza", sms_gonder.get("data"))
 
-    def gib_sms_onay(self, faturalar:list[dict] | dict, oid:str, sifre:str):
+    def gib_sms_onay(self, faturalar:list[dict] | dict, oid:str, sifre:str) -> BaseModel:
         istek = self.__kod_calistir(
             komut = self.komutlar.SMSSIFRE_DOGRULA,
             jp    = {
                 "SIFRE" : sifre,
                 "OID"   : oid,
                 "OPR"   : 1,
-                "DATA"  : [faturalar] if isinstance(faturalar, dict) else faturalar,
+                "DATA"  : self.__fatura_ver(faturalar),
             }
         )
+        veri  = istek.get("data")
 
-        return istek.get("data")
+        return self.__nesne_ver("GibSMSOnay", {"mesaj": veri.get("msg")})
 
     # TODO: https://github.com/mlevent/fatura 'dan faydalanarak geri kalan fonksiyonlar yazılacaktır..
```

### Comparing `eArsivPortal-0.0.7/eArsivPortal/Libs/FaturaVer.py` & `eArsivPortal-0.0.8/eArsivPortal/Libs/FaturaVer.py`

 * *Files identical despite different names*

### Comparing `eArsivPortal-0.0.7/eArsivPortal/Libs/Oturum.py` & `eArsivPortal-0.0.8/eArsivPortal/Libs/Oturum.py`

 * *Files identical despite different names*

### Comparing `eArsivPortal-0.0.7/eArsivPortal/Models/Komutlar.py` & `eArsivPortal-0.0.8/eArsivPortal/Models/Komutlar.py`

 * *Files identical despite different names*

### Comparing `eArsivPortal-0.0.7/eArsivPortal.egg-info/PKG-INFO` & `eArsivPortal-0.0.8/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: eArsivPortal
-Version: 0.0.7
-Summary: GİB e-Arşiv Portal e-Fatura Oluşturucu
-Home-page: https://github.com/keyiflerolsun/eArsivPortal
-Author: keyiflerolsun
-Author-email: keyiflerolsun@gmail.com
-License: GPLv3+
-Keywords: eArsivPortal,KekikAkademi,keyiflerolsun
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # 🧾 eArsivPortal
 
 [![Boyut](https://img.shields.io/github/repo-size/keyiflerolsun/eArsivPortal?logo=git&logoColor=white&label=Boyut)](#)
 [![Görüntülenme](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/keyiflerolsun/eArsivPortal&title=Görüntülenme)](#)
 <a href="https://KekikAkademi.org/Kahve" target="_blank"><img src="https://img.shields.io/badge/☕️-Kahve Ismarla-ffdd00" title="☕️ Kahve Ismarla" style="padding-left:5px;"></a>
 
 [![PyPI Yükleyici](https://img.shields.io/github/actions/workflow/status/keyiflerolsun/eArsivPortal/PyPI.yml?label=PyPI%20Y%C3%BCkleyici&logo=github)](https://github.com/keyiflerolsun/eArsivPortal/actions/workflows/PyPI.yml)
@@ -61,49 +45,53 @@
     sifre          = "1",
     test_modu      = True
 )
 ```
 
 ```python
 portal.bilgilerim()
+
 #--------------------------------------------------------------#
-{
-    "vknTckn": "3333333301",
-    "unvan": "HOSAM ALDEEN ABUSHAWER TİCARİ GİRİŞİMİ",
-    "ad": "",
-    "soyad": "",
-    "cadde": "şehit yusuf bey",
-    "apartmanAdi": "yıldız",
-    "apartmanNo": "8",
-    "kapiNo": "2",
-    "kasaba": "ortakapı",
-    "ilce": "Merkez",
-    "il": "Kars",
-    "postaKodu": "36000",
-    "ulke": "Türkiye",
-    "telNo": "05524775288",
-    "faksNo": "",
-    "ePostaAdresi": "",
-    "webSitesiAdresi": "",
-    "vergiDairesi": "kars",
-    "sicilNo": "8729",
-    "isMerkezi": "",
-    "mersisNo": "9962438036000001"
-}
+
+Bilgilerim(
+    vknTckn='3333333315',
+    unvan='XYZ Yaz',
+    ad='',
+    soyad='',
+    cadde='Sahil yolu',
+    apartmanAdi='Dali çıtır pide',
+    apartmanNo='12',
+    kapiNo='3',
+    kasaba='adana',
+    ilce='GEMLİK',
+    il='Antalya',
+    postaKodu='16000',
+    ulke='Türkiye',
+    telNo='053982456665',
+    faksNo='',
+    ePostaAdresi='info@vekamp.com',
+    webSitesiAdresi='',
+    vergiDairesi='orhangazi vergi dairesi',
+    sicilNo='00000000000000',
+    isMerkezi='',
+    mersisNo=''
+)
 ```
 
 ```python
 portal.kisi_getir(vkn_veya_tckn="3333333301")
+
 #--------------------------------------------------------------#
-{
-    "unvan":"HOSAM ALDEEN ABUSHAWER TİCARİ GİRİŞİMİ",
-    "adi":"",
-    "soyadi":"",
-    "vergiDairesi":"kars"
-}
+
+Kisi(
+    unvan='XYZ Yaz',
+    adi='',
+    soyadi='',
+    vergiDairesi='orhangazi vergi dairesi'
+)
 ```
 
 ```python
 portal.fatura_olustur(
     tarih:str         = "07/10/1995",
     saat:str          = "14:28:37",
     vkn_veya_tckn:str = "11111111111",
@@ -111,68 +99,87 @@
     soyad:str         = "Sancak",
     unvan:str         = "",
     vergi_dairesi:str = "",
     urun_adi:str      = "Python Yazılım Hizmeti",
     fiyat:int | float = 100,
     fatura_notu:str   = "— QNB Finansbank —\nTR70 0011 1000 0000 0118 5102 59\nÖmer Faruk Sancak"
 )
+
 #--------------------------------------------------------------#
-{"ettn": "b40c16ae-8509-434e-bd6f-894459372134"}
+
+FaturaOlustur(ettn='8cb401e3-ca6d-442a-8389-894459372134')
 ```
 
 ```python
 faturalar = portal.faturalari_getir(
     baslangic_tarihi = "01/05/2023",
     bitis_tarihi     = "28/05/2023"
 )
+
 #--------------------------------------------------------------#
+
 [
-    {
-        'belgeNumarasi': 'GIB2023000002672',
-        'aliciVknTckn': '16045751784',
-        'aliciUnvanAdSoyad': 'Sercan AYDIN',
-        'belgeTarihi': '28-05-2023',
-        'belgeTuru': 'FATURA',
-        'onayDurumu': 'Onaylanmadı',
-        'ettn': '0c111c74-fcd4-11ed-8026-3ae56703837b'
-    },
-    {
-        'belgeNumarasi': 'GIB2023000002673',
-        'aliciVknTckn': '16045751784',
-        'aliciUnvanAdSoyad': 'Sercan AYDIN',
-        'belgeTarihi': '28-05-2023',
-        'belgeTuru': 'FATURA',
-        'onayDurumu': 'Silinmiş',
-        'ettn': '234baa8e-fcd5-11ed-827f-3ae56703837b'
-    }
+    Fatura(
+        belgeNumarasi='GIB2023000002672',
+        aliciVknTckn='16045751784',
+        aliciUnvanAdSoyad='Sercan AYDIN',
+        belgeTarihi='29-05-2023',
+        belgeTuru='FATURA',
+        onayDurumu='Silinmiş',
+        ettn='7386c1dc-8a23-4d46-9c8d-de3512b630b4'
+    ),
+    Fatura(
+        belgeNumarasi='GIB2023000001918',
+        aliciVknTckn='16045751784',
+        aliciUnvanAdSoyad='Sercan AYDIN',
+        belgeTarihi='29-05-2023',
+        belgeTuru='FATURA',
+        onayDurumu='Onaylanmadı',
+        ettn='2ef98bfa-8787-4429-a1fa-a0514560e7eb'
+    ),
+    Fatura(
+        belgeNumarasi='GIB2023000001919',
+        aliciVknTckn='16045751784',
+        aliciUnvanAdSoyad='Sercan AYDIN',
+        belgeTarihi='29-05-2023',
+        belgeTuru='FATURA',
+        onayDurumu='Onaylandı',
+        ettn='8cb401e3-ca6d-442a-8389-c4d87c9eb67c'
+    )
 ]
 ```
 
 ```python
 html_fatura = portal.fatura_html(
-    ettn        = faturalar[0].get("ettn")
-    onay_durumu = faturalar[0].get("onayDurumu")
+    ettn        = faturalar[0].ettn
+    onay_durumu = faturalar[0].onayDurumu
 )
 
-with open(f"{faturalar[0].get("aliciUnvanAdSoyad")}.html", "w", encoding="utf-8") as dosya:
+with open(f"{faturalar[0].aliciUnvanAdSoyad}.html", "w", encoding="utf-8") as dosya:
     dosya.write(html_fatura)
 ```
 
 ```python
 portal.fatura_sil(
     faturalar = [faturalar[0], faturalar[1]]
     aciklama  = "Fatura silindi."
 )
+
 #--------------------------------------------------------------#
-2 fatura başarıyla silindi.
+
+FaturaSil(mesaj='2 fatura başarıyla silindi.')
 ```
 
 ```python
-oid = portal.gib_imza()
-portal.gib_sms_onay(faturalar[3], oid, input("SMS Doğrulama Kodu: "))
+imza = portal.gib_imza()
+portal.gib_sms_onay(faturalar[3], imza.oid, input("SMS Doğrulama Kodu: "))
+
+#--------------------------------------------------------------#
+
+GibSMSOnay(mesaj='SMS şifreniz doğrulandı, işlem başarılı.')
 ```
 
 ```python
 portal.cikis_yap()
 ```
 
 ## 🌐 Telif Hakkı ve Lisans
@@ -186,8 +193,8 @@
 
 ## 💸 Bağış Yap
 
 **[☕️ Kahve Ismarla](https://KekikAkademi.org/Kahve)**
 
 ***
 
-> **[@KekikAkademi](https://t.me/KekikAkademi)** *için yazılmıştır..*
+> **[@KekikAkademi](https://t.me/KekikAkademi)** *için yazılmıştır..*
```

#### html2text {}

```diff
@@ -1,21 +1,14 @@
-Metadata-Version: 2.1 Name: eArsivPortal Version: 0.0.7 Summary: GÄ°B e-ArÅiv
-Portal e-Fatura OluÅturucu Home-page: https://github.com/keyiflerolsun/
-eArsivPortal Author: keyiflerolsun Author-email: keyiflerolsun@gmail.com
-License: GPLv3+ Keywords: eArsivPortal,KekikAkademi,keyiflerolsun Classifier:
-Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
-:: GNU General Public License v3 or later (GPLv3+) Classifier: Programming
-Language :: Python :: 3 Requires-Python: >=3.10 Description-Content-Type: text/
-markdown License-File: LICENSE # ð§¾ eArsivPortal [![Boyut](https://
-img.shields.io/github/repo-size/keyiflerolsun/
-eArsivPortal?logo=git&logoColor=white&label=Boyut)](#) [![GÃ¶rÃ¼ntÃ¼lenme]
-(https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/
-keyiflerolsun/eArsivPortal&title=GÃ¶rÃ¼ntÃ¼lenme)](#) [https://img.shields.io/
-badge/âï¸-Kahve_Ismarla-ffdd00] [![PyPI YÃ¼kleyici](https://img.shields.io/
-github/actions/workflow/status/keyiflerolsun/eArsivPortal/
+# ð§¾ eArsivPortal [![Boyut](https://img.shields.io/github/repo-size/
+keyiflerolsun/eArsivPortal?logo=git&logoColor=white&label=Boyut)](#) [!
+[GÃ¶rÃ¼ntÃ¼lenme](https://hits.seeyoufarm.com/api/count/incr/
+badge.svg?url=https://github.com/keyiflerolsun/
+eArsivPortal&title=GÃ¶rÃ¼ntÃ¼lenme)](#) [https://img.shields.io/badge/âï¸-
+Kahve_Ismarla-ffdd00] [![PyPI YÃ¼kleyici](https://img.shields.io/github/
+actions/workflow/status/keyiflerolsun/eArsivPortal/
 PyPI.yml?label=PyPI%20Y%C3%BCkleyici&logo=github)](https://github.com/
 keyiflerolsun/eArsivPortal/actions/workflows/PyPI.yml) [![PyPI](https://
 img.shields.io/pypi/v/eArsivPortal?logo=pypi&logoColor=white&label=PyPI)]
 (https://pypi.org/project/eArsivPortal) [![PyPI - YÃ¼klenme](https://
 img.shields.io/pypi/dm/eArsivPortal?logo=pypi&logoColor=white&label=YÃ¼klenme)]
 (https://pypi.org/project/eArsivPortal) [![PyPI - Wheel](https://
 img.shields.io/pypi/wheel/eArsivPortal?logo=pypi&logoColor=white&label=Wheel)]
@@ -34,48 +27,52 @@
 keyiflerolsun/) ## ð Kurulum ### [https://raw.githubusercontent.com/
 keyiflerolsun/eArsivPortal/main/.github/icons/pypi.svg] PyPI ```bash #
 YÃ¼klemek pip install eArsivPortal # GÃ¼ncellemek pip install -U eArsivPortal
 ``` ## ð KullanÄ±m ### [https://raw.githubusercontent.com/keyiflerolsun/
 eArsivPortal/main/.github/icons/python.svg] Lib ```python from eArsivPortal
 import eArsivPortal portal = eArsivPortal( kullanici_kodu = "33333301", sifre =
 "1", test_modu = True ) ``` ```python portal.bilgilerim() #--------------------
-------------------------------------------# { "vknTckn": "3333333301", "unvan":
-"HOSAM ALDEEN ABUSHAWER TÄ°CARÄ° GÄ°RÄ°ÅÄ°MÄ°", "ad": "", "soyad": "",
-"cadde": "Åehit yusuf bey", "apartmanAdi": "yÄ±ldÄ±z", "apartmanNo": "8",
-"kapiNo": "2", "kasaba": "ortakapÄ±", "ilce": "Merkez", "il": "Kars",
-"postaKodu": "36000", "ulke": "TÃ¼rkiye", "telNo": "05524775288", "faksNo": "",
-"ePostaAdresi": "", "webSitesiAdresi": "", "vergiDairesi": "kars", "sicilNo":
-"8729", "isMerkezi": "", "mersisNo": "9962438036000001" } ``` ```python
-portal.kisi_getir(vkn_veya_tckn="3333333301") #--------------------------------
-------------------------------# { "unvan":"HOSAM ALDEEN ABUSHAWER TÄ°CARÄ°
-GÄ°RÄ°ÅÄ°MÄ°", "adi":"", "soyadi":"", "vergiDairesi":"kars" } ``` ```python
+------------------------------------------# Bilgilerim( vknTckn='3333333315',
+unvan='XYZ Yaz', ad='', soyad='', cadde='Sahil yolu', apartmanAdi='Dali
+Ã§Ä±tÄ±r pide', apartmanNo='12', kapiNo='3', kasaba='adana', ilce='GEMLÄ°K',
+il='Antalya', postaKodu='16000', ulke='TÃ¼rkiye', telNo='053982456665',
+faksNo='', ePostaAdresi='info@vekamp.com', webSitesiAdresi='',
+vergiDairesi='orhangazi vergi dairesi', sicilNo='00000000000000', isMerkezi='',
+mersisNo='' ) ``` ```python portal.kisi_getir(vkn_veya_tckn="3333333301") #----
+----------------------------------------------------------# Kisi( unvan='XYZ
+Yaz', adi='', soyadi='', vergiDairesi='orhangazi vergi dairesi' ) ``` ```python
 portal.fatura_olustur( tarih:str = "07/10/1995", saat:str = "14:28:37",
 vkn_veya_tckn:str = "11111111111", ad:str = "Ãmer Faruk", soyad:str =
 "Sancak", unvan:str = "", vergi_dairesi:str = "", urun_adi:str = "Python
 YazÄ±lÄ±m Hizmeti", fiyat:int | float = 100, fatura_notu:str = "â QNB
 Finansbank â\nTR70 0011 1000 0000 0118 5102 59\nÃmer Faruk Sancak" ) #------
---------------------------------------------------------# {"ettn": "b40c16ae-
-8509-434e-bd6f-894459372134"} ``` ```python faturalar = portal.faturalari_getir
-( baslangic_tarihi = "01/05/2023", bitis_tarihi = "28/05/2023" ) #-------------
--------------------------------------------------# [ { 'belgeNumarasi':
-'GIB2023000002672', 'aliciVknTckn': '16045751784', 'aliciUnvanAdSoyad': 'Sercan
-AYDIN', 'belgeTarihi': '28-05-2023', 'belgeTuru': 'FATURA', 'onayDurumu':
-'OnaylanmadÄ±', 'ettn': '0c111c74-fcd4-11ed-8026-3ae56703837b' },
-{ 'belgeNumarasi': 'GIB2023000002673', 'aliciVknTckn': '16045751784',
-'aliciUnvanAdSoyad': 'Sercan AYDIN', 'belgeTarihi': '28-05-2023', 'belgeTuru':
-'FATURA', 'onayDurumu': 'SilinmiÅ', 'ettn': '234baa8e-fcd5-11ed-827f-
-3ae56703837b' } ] ``` ```python html_fatura = portal.fatura_html( ettn =
-faturalar[0].get("ettn") onay_durumu = faturalar[0].get("onayDurumu") ) with
-open(f"{faturalar[0].get("aliciUnvanAdSoyad")}.html", "w", encoding="utf-8") as
-dosya: dosya.write(html_fatura) ``` ```python portal.fatura_sil( faturalar =
-[faturalar[0], faturalar[1]] aciklama = "Fatura silindi." ) #------------------
---------------------------------------------# 2 fatura baÅarÄ±yla silindi. ```
-```python oid = portal.gib_imza() portal.gib_sms_onay(faturalar[3], oid, input
-("SMS DoÄrulama Kodu: ")) ``` ```python portal.cikis_yap() ``` ## ð Telif
-HakkÄ± ve Lisans * *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/
+--------------------------------------------------------# FaturaOlustur
+(ettn='8cb401e3-ca6d-442a-8389-894459372134') ``` ```python faturalar =
+portal.faturalari_getir( baslangic_tarihi = "01/05/2023", bitis_tarihi = "28/
+05/2023" ) #--------------------------------------------------------------#
+[ Fatura( belgeNumarasi='GIB2023000002672', aliciVknTckn='16045751784',
+aliciUnvanAdSoyad='Sercan AYDIN', belgeTarihi='29-05-2023', belgeTuru='FATURA',
+onayDurumu='SilinmiÅ', ettn='7386c1dc-8a23-4d46-9c8d-de3512b630b4' ), Fatura
+( belgeNumarasi='GIB2023000001918', aliciVknTckn='16045751784',
+aliciUnvanAdSoyad='Sercan AYDIN', belgeTarihi='29-05-2023', belgeTuru='FATURA',
+onayDurumu='OnaylanmadÄ±', ettn='2ef98bfa-8787-4429-a1fa-a0514560e7eb' ),
+Fatura( belgeNumarasi='GIB2023000001919', aliciVknTckn='16045751784',
+aliciUnvanAdSoyad='Sercan AYDIN', belgeTarihi='29-05-2023', belgeTuru='FATURA',
+onayDurumu='OnaylandÄ±', ettn='8cb401e3-ca6d-442a-8389-c4d87c9eb67c' ) ] ```
+```python html_fatura = portal.fatura_html( ettn = faturalar[0].ettn
+onay_durumu = faturalar[0].onayDurumu ) with open(f"{faturalar
+[0].aliciUnvanAdSoyad}.html", "w", encoding="utf-8") as dosya: dosya.write
+(html_fatura) ``` ```python portal.fatura_sil( faturalar = [faturalar[0],
+faturalar[1]] aciklama = "Fatura silindi." ) #---------------------------------
+-----------------------------# FaturaSil(mesaj='2 fatura baÅarÄ±yla silindi.')
+``` ```python imza = portal.gib_imza() portal.gib_sms_onay(faturalar[3],
+imza.oid, input("SMS DoÄrulama Kodu: ")) #------------------------------------
+--------------------------# GibSMSOnay(mesaj='SMS Åifreniz doÄrulandÄ±,
+iÅlem baÅarÄ±lÄ±.') ``` ```python portal.cikis_yap() ``` ## ð Telif HakkÄ±
+ve Lisans * *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/
 keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007]
 (https://github.com/keyiflerolsun/eArsivPortal/blob/master/LICENSE)
 *KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ## â»ï¸ Ä°letiÅim *Benimle
 iletiÅime geÃ§mek isterseniz, **Telegram**'dan mesaj gÃ¶ndermekten
 Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ## ð¸ BaÄÄ±Å Yap **
 [âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)** *** > **
 [@KekikAkademi](https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
```

### Comparing `eArsivPortal-0.0.7/setup.py` & `eArsivPortal-0.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 from io         import open
 
 setup(
     # ? Genel Bilgiler
     name         = "eArsivPortal",
-    version      = "0.0.7",
+    version      = "0.0.8",
     url          = "https://github.com/keyiflerolsun/eArsivPortal",
     description  = "GİB e-Arşiv Portal e-Fatura Oluşturucu",
     keywords     = ["eArsivPortal", "KekikAkademi", "keyiflerolsun"],
 
     author       = "keyiflerolsun",
     author_email = "keyiflerolsun@gmail.com",
```

