# Comparing `tmp/vitya-0.14.0.tar.gz` & `tmp/vitya-0.15.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vitya-0.14.0.tar", last modified: Thu Apr 27 10:02:51 2023, max compression
+gzip compressed data, was "dist/vitya-0.15.0.tar", last modified: Mon May 29 15:13:12 2023, max compression
```

## Comparing `vitya-0.14.0.tar` & `vitya-0.15.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:02:51.000000 vitya-0.14.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-27 10:02:48.000000 vitya-0.14.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-27 10:02:51.000000 vitya-0.14.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-27 10:02:48.000000 vitya-0.14.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-27 10:02:48.000000 vitya-0.14.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 10:02:51.000000 vitya-0.14.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-27 10:02:48.000000 vitya-0.14.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:02:51.000000 vitya-0.14.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8405 2023-04-27 10:02:48.000000 vitya-0.14.0/tests/test_vitya.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:02:51.000000 vitya-0.14.0/vitya/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-27 10:02:48.000000 vitya-0.14.0/vitya/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-04-27 10:02:48.000000 vitya-0.14.0/vitya/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-27 10:02:48.000000 vitya-0.14.0/vitya/errors_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:02:51.000000 vitya-0.14.0/vitya/payment_order/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 10:02:48.000000 vitya-0.14.0/vitya/payment_order/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-27 10:02:48.000000 vitya-0.14.0/vitya/payment_order/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    28380 2023-04-27 10:02:48.000000 vitya-0.14.0/vitya/payment_order/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-27 10:02:48.000000 vitya-0.14.0/vitya/payment_order/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:02:51.000000 vitya-0.14.0/vitya/payment_order/payments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 10:02:48.000000 vitya-0.14.0/vitya/payment_order/payments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8970 2023-04-27 10:02:48.000000 vitya-0.14.0/vitya/payment_order/payments/checkers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12986 2023-04-27 10:02:48.000000 vitya-0.14.0/vitya/payment_order/payments/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-27 10:02:48.000000 vitya-0.14.0/vitya/payment_order/payments/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-04-27 10:02:48.000000 vitya-0.14.0/vitya/payment_order/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 10:02:48.000000 vitya-0.14.0/vitya/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-27 10:02:48.000000 vitya-0.14.0/vitya/pydantic_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-04-27 10:02:48.000000 vitya-0.14.0/vitya/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:02:51.000000 vitya-0.14.0/vitya.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-27 10:02:51.000000 vitya-0.14.0/vitya.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-27 10:02:51.000000 vitya-0.14.0/vitya.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 10:02:51.000000 vitya-0.14.0/vitya.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-27 10:02:51.000000 vitya-0.14.0/vitya.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:13:12.000000 vitya-0.15.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-29 15:13:09.000000 vitya-0.15.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-29 15:13:12.000000 vitya-0.15.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-29 15:13:09.000000 vitya-0.15.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-29 15:13:09.000000 vitya-0.15.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 15:13:12.000000 vitya-0.15.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-29 15:13:09.000000 vitya-0.15.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:13:12.000000 vitya-0.15.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8405 2023-05-29 15:13:09.000000 vitya-0.15.0/tests/test_vitya.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:13:12.000000 vitya-0.15.0/vitya/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-29 15:13:09.000000 vitya-0.15.0/vitya/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-05-29 15:13:09.000000 vitya-0.15.0/vitya/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-29 15:13:09.000000 vitya-0.15.0/vitya/errors_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:13:12.000000 vitya-0.15.0/vitya/payment_order/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 15:13:09.000000 vitya-0.15.0/vitya/payment_order/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-29 15:13:09.000000 vitya-0.15.0/vitya/payment_order/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28762 2023-05-29 15:13:09.000000 vitya-0.15.0/vitya/payment_order/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-29 15:13:09.000000 vitya-0.15.0/vitya/payment_order/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:13:12.000000 vitya-0.15.0/vitya/payment_order/payments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 15:13:09.000000 vitya-0.15.0/vitya/payment_order/payments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9229 2023-05-29 15:13:09.000000 vitya-0.15.0/vitya/payment_order/payments/checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13485 2023-05-29 15:13:09.000000 vitya-0.15.0/vitya/payment_order/payments/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-29 15:13:09.000000 vitya-0.15.0/vitya/payment_order/payments/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-29 15:13:09.000000 vitya-0.15.0/vitya/payment_order/payments/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-05-29 15:13:09.000000 vitya-0.15.0/vitya/payment_order/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 15:13:09.000000 vitya-0.15.0/vitya/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-05-29 15:13:09.000000 vitya-0.15.0/vitya/pydantic_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-05-29 15:13:09.000000 vitya-0.15.0/vitya/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:13:12.000000 vitya-0.15.0/vitya.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-29 15:13:12.000000 vitya-0.15.0/vitya.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-29 15:13:12.000000 vitya-0.15.0/vitya.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 15:13:12.000000 vitya-0.15.0/vitya.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-29 15:13:12.000000 vitya-0.15.0/vitya.egg-info/top_level.txt
```

### Comparing `vitya-0.14.0/LICENSE` & `vitya-0.15.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vitya-0.14.0/PKG-INFO` & `vitya-0.15.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vitya
-Version: 0.14.0
+Version: 0.15.0
 Summary: Validators for different russian banking values
 Home-page: https://github.com/hicebank/vitya
 Author: hicebank.ru
 Author-email: inyutin@hicebank.ru
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `vitya-0.14.0/README.md` & `vitya-0.15.0/README.md`

 * *Files identical despite different names*

### Comparing `vitya-0.14.0/setup.py` & `vitya-0.15.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='vitya',
-    version='0.14.0',
+    version='0.15.0',
     author='hicebank.ru',
     author_email='inyutin@hicebank.ru',
     description='Validators for different russian banking values',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/hicebank/vitya',
     packages=setuptools.find_packages(),
```

### Comparing `vitya-0.14.0/tests/test_vitya.py` & `vitya-0.15.0/tests/test_vitya.py`

 * *Files identical despite different names*

### Comparing `vitya-0.14.0/vitya/errors.py` & `vitya-0.15.0/vitya/errors.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 
 
 class OKTMOValidationTypeError(OKTMOValidationError, PydanticTypeError):
     description = 'must be str'
     description_ru = 'должен быть строкой'
 
 
-class OKTMOValidationValueLenError(PydanticValueError):
+class OKTMOValidationValueLenError(OKTMOValidationError):
     description = 'must be match 8 or 11 digits'
     description_ru = 'должен состоять из 8 или 11 цифр'
 
 
-class OKTMOValidationValueError(PydanticValueError):
+class OKTMOValidationValueError(OKTMOValidationError):
     description = 'must be match as ([0-9]{11}|[0-9]{8})'
     description_ru = 'должен матчиться с ([0-9]{11}|[0-9]{8})'
 
 
 class INNValidationError(VityaDescribedError, PydanticValueError):
     target = 'inn'
     target_ru = 'ИНН'
```

### Comparing `vitya-0.14.0/vitya/payment_order/errors.py` & `vitya-0.15.0/vitya/payment_order/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,19 @@
 
 
 class AmountValidationLessOrEqualZeroError(AmountValidationError):
     description = 'cannot be less than or equal to 0.0'
     description_ru = 'не может быть меньше или равно 0.0'
 
 
+class AmountNotANumber(AmountValidationError):
+    description = 'require to be a number'
+    description_ru = 'должно быть числом'
+
+
 class CustomerValidationError(VityaDescribedError, PydanticValueError):
     target = 'customer'
     target_ru = 'плательщик или получатель'
     description = 'base error'
     description_ru = 'базовая ошибка'
 
 
@@ -173,25 +178,14 @@
 
 
 class UINValidationBOLenError(UINValidationLenError):
     description = 'len uin for bo payment must be 4, 20 or 25 len'
     description_ru = 'длина для платежей с типом иные должна быть 4, 30 или 25'
 
 
-class UINValidationBOValueError(UINValidationError):
-    description = (
-        'for bo payment with payee account start with '
-        "('03212', '03222', '03232', '03242', '03252', '03262', '03272') uin must be non zero"
-    )
-    description_ru = (
-        'для платежей с типом иные номер счета получателя должно начинаться с '
-        "('03212', '03222', '03232', '03242', '03252', '03262', '03272') и ЮИН должен быть не нулевым"
-    )
-
-
 class UINValidationFNSValueError(UINValidationError):
     description = 'FNS base error'
     description_ru = 'базовая ФНС ошибка'
 
 
 class UINValidationFNSValueZeroError(UINValidationFNSValueError):
     description = (
@@ -203,14 +197,21 @@
 
 
 class UINValidationFNSNotValueZeroError(UINValidationFNSValueError):
     description = 'for FNS with payer status = "02" uin must be zero'
     description_ru = 'для платежей в ФНС со статусом плательщика "02" и пустым ИНН, УИН должен быть нулевым'
 
 
+class UINValidationBONotEmpty(UINValidationFNSValueError):
+    description = 'for budget other and payee number starting with 03212 uin must be filled'
+    description_ru = (
+        'для платежей в бюджет иные с номером счёта получателя, который начинается с "03212", УИН должен быть заполен'
+    )
+
+
 class UINValidationFNSLenError(UINValidationLenError):
     description = 'invalid uin: len uin for FNS payment must be 20 or 25 len'
     description_ru = 'длина УИН для платежей в ФНС должна быть 20 или 15 символов'
 
 
 class UINValidationOnlyZeroError(UINValidationError):
     description = 'cannot contains only 0 chars'
@@ -225,77 +226,85 @@
 
 
 class PurposeValidationTypeError(PurposeValidationError, PydanticTypeError):
     description = 'must be str'
     description_ru = 'должно быть строкой'
 
 
-class PurposeValidationMaxLenError(PydanticValueError):
+class PurposeValidationMaxLenError(PurposeValidationError):
     description = 'len can be from 1 to 210 chars'
     description_ru = 'длина должна быть от 1 до 210 символов'
 
 
 class PurposeValidationCharactersError(PurposeValidationError):
     description = f'can only consist of {CHARS_FOR_PURPOSE}'
     description_ru = f'может состоять только из символов {CHARS_FOR_PURPOSE}'
 
 
 class PurposeValidationIPNDSError(PurposeValidationError):
     description = 'for IP payment purpose must contains "НДС"'
     description_ru = 'для платежей ИП назначение должно содержать "НДС"'
 
 
-class PayerINNValidationCustomsLen10Error(INNValidationLenError):
+class PayerINNValidationError(INNValidationError):
+    target = 'payer inn'
+    target_ru = 'ИНН плательщика'
+
+
+class PayerINNValidationCustomsLen10Error(INNValidationLenError, PayerINNValidationError):
     description = 'for customs payment and payer status "06", inn must be 10'
     description_ru = 'для платежей в таможню и со статусом плательщика "06" ИНН должно быть "10"'
 
 
-class PayerINNValidationCustomsLen12Error(INNValidationLenError):
+class PayerINNValidationCustomsLen12Error(INNValidationLenError, PayerINNValidationError):
     description = 'for customs payment and payer status 16 or 17, inn must be 12'
     description_ru = 'для платежей таможню со статусом плательщика "16" или "17", значение ИНН должно быть "12"'
 
 
-class PayerINNValidationEmptyNotAllowedError(INNValidationError):
+class PayerINNValidationEmptyNotAllowedError(PayerINNValidationError):
     description = 'inn cannot be empty'
     description_ru = 'не может быть пустым'
 
 
-class PayerINNValidationStartWithZerosError(INNValidationError):
+class PayerINNValidationStartWithZerosError(PayerINNValidationError):
     description = 'cannot start with "00"'
     description_ru = 'не может начинаться с "00"'
 
 
-class PayerINNValidationFiveOnlyZerosError(INNValidationError):
+class PayerINNValidationFiveOnlyZerosError(PayerINNValidationError):
     description = 'inn with len 5 cannot be contains only zeros'
     description_ru = 'ИНН с длиной 5 символов не может содержать только нули'
 
 
-class PayeeINNValidationNonEmptyError(INNValidationError):
-    target_ru = 'payee inn'
-    target = 'ИНН получателя'
+class PayeeINNValidationError(INNValidationError):
+    target = 'payee inn'
+    target_ru = 'ИНН получателя'
+
+
+class PayeeINNValidationNonEmptyError(PayeeINNValidationError):
     description = 'cannot be empty'
     description_ru = 'не может быть пустым'
 
 
-class PayeeINNValidationFLenError(INNValidationLenError):
+class PayeeINNValidationFLenError(INNValidationLenError, PayeeINNValidationError):
     description = 'for fl payee inn must be 12'
     description_ru = 'для платежей ИП ИНН получателя должно быть длиной 12 символов'
 
 
-class PayeeINNValidationFLLenError(INNValidationLenError):
+class PayeeINNValidationFLLenError(INNValidationLenError, PayeeINNValidationError):
     description = 'for fl payee inn must be empty or 12 chars'
     description_ru = 'для платежей ИП ИНН получателя должно быть пустым или содержать 12 символов'
 
 
-class PayeeINNValidationIPLenError(INNValidationError):
+class PayeeINNValidationIPLenError(PayeeINNValidationError):
     description = 'for ip payee inn must be 12'
     description_ru = 'для платежей ИП ИНН получателя должно быть 12 символов'
 
 
-class PayeeINNValidationLELenError(INNValidationError):
+class PayeeINNValidationLELenError(PayeeINNValidationError):
     description = 'for fns, customs, bo and le inn must be 10'
     description_ru = 'для платежей в бюджет и платежей ЮЛ, ИНН должно быть 10 символов'
 
 
 class PayerAccountValidationError(VityaDescribedError, PydanticValueError):
     target = 'payer account'
     target_ru = 'счет плательщика'
@@ -392,31 +401,31 @@
     description = 'empty value is not allowed'
     description_ru = 'пустое значение не разрешено'
 
 
 class PayerKPPValidationError(KPPValidationError):
     target = 'payer kpp'
     target_ru = 'КПП плательщика'
-    description = 'ase error'
+    description = 'base error'
     description_ru = 'базовая ошибка'
 
 
 class PayerKPPValidationOnlyEmptyError(PayerKPPValidationError, KPPValidationOnlyEmptyError):
     description = 'for ip, fl or le value must be empty'
     description_ru = 'для платежей ИП, ФЛ, И ЮЛ значение должно быть пустым'
 
 
 class PayerKPPValidationINN10EmptyNotAllowed(PayerKPPValidationError, KPPValidationEmptyNotAllowed):
-    description = 'for budget payment with inn = 10 inn empty value is not allowed'
-    description_ru = 'для платежей в бюджет с ИНН = "10" значение КПП должно быть заполнено'
+    description = 'for budget payment with inn length 10 kpp empty value is not allowed'
+    description_ru = 'для платежей в бюджет с длиной ИНН равной 10 значение КПП должно быть заполнено'
 
 
 class PayerKPPValidationINN12OnlyEmptyError(PayerKPPValidationOnlyEmptyError):
-    description = 'for budget with inn = 12 only empty allowed'
-    description_ru = 'для платежей в бюджет с ИНН = "10" значение КПП должно быть пустым'
+    description = 'for budget with inn length 12 kpp only empty allowed'
+    description_ru = 'для платежей в бюджет с длиной ИНН равной 12 значение КПП должно быть пустым'
 
 
 class PayeeKPPValidationError(KPPValidationError):
     target = 'payee kpp'
     target_ru = 'КПП получателя'
     description = 'base error'
     description_ru = 'базовая ошибка'
```

### Comparing `vitya-0.14.0/vitya/payment_order/fields.py` & `vitya-0.15.0/vitya/payment_order/fields.py`

 * *Files identical despite different names*

### Comparing `vitya-0.14.0/vitya/payment_order/payments/checkers.py` & `vitya-0.15.0/vitya/payment_order/payments/checkers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from abc import ABC, abstractmethod
-from typing import Any, ClassVar, Dict, List, Tuple, Type, cast
+from typing import Any, ClassVar, Dict, List, Sequence, Tuple, Type
 
 from pydantic import BaseModel, root_validator
-from pydantic.errors import PydanticValueError
 
 from vitya.payment_order.enums import PaymentType
 from vitya.payment_order.fields import (
     CBC,
     UIN,
     AccountNumber,
     DocumentDate,
@@ -35,17 +34,20 @@
     check_tax_period,
     check_uin,
 )
 from vitya.pydantic_fields import BIC, INN, KPP, OKTMO
 
 
 class CheckerError(ValueError):
+    def __init__(self, errors: Sequence[Exception]):
+        self._errors = errors
+
     @property
-    def errors(self) -> List[Type[PydanticValueError]]:
-        return cast(List[Type[PydanticValueError]], self.args[0])
+    def errors(self) -> Sequence[Exception]:
+        return self._errors
 
 
 class BaseChecker(ABC):
     @abstractmethod
     def check(self) -> None:  # pragma: no cover
         pass
 
@@ -55,17 +57,17 @@
 
     def __init_subclass__(cls, **kwargs: Dict[str, Any]) -> None:  # pragma: no cover
         # built error
         errors = []
         for checker, fields in cls.__checkers__:
             wild_fields = set(fields) - cls.__fields__.keys()
             if wild_fields:
-                errors.append(ValueError(f'Checker {checker} require unknown model fields {wild_fields}'))
+                errors.append(f'Checker {checker} require unknown model fields {wild_fields}')
         if errors:
-            raise CheckerError(errors)
+            raise ValueError(errors)
 
     @root_validator(pre=False)
     def run_checkers(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         errors = []
         for checker, fields_names in cls.__checkers__:
             try:
                 args = [values[field_name] for field_name in fields_names]
@@ -128,36 +130,46 @@
             payment_type=self.payment_type,
             payer_status=self.payer_status,
             for_third_face=self.for_third_face
         )
 
 
 class UINChecker(BaseChecker):
-    def __init__(self, uin: UIN, payer_inn: INN, payer_status: PayerStatus, payment_type: PaymentType) -> None:
+    def __init__(
+        self,
+        uin: UIN,
+        payee_account: AccountNumber,
+        payer_inn: INN,
+        payer_status: PayerStatus,
+        payment_type: PaymentType,
+    ) -> None:
         self.uin = uin
+        self.payee_account = payee_account
         self.payer_inn = payer_inn
         self.payer_status = payer_status
         self.payment_type = payment_type
 
     def check(self) -> None:
         check_uin(
             value=self.uin,
+            payee_account=self.payee_account,
             payment_type=self.payment_type,
             payer_status=self.payer_status,
             payer_inn=self.payer_inn,
         )
 
 
 class PurposeChecker(BaseChecker):
-    def __init__(self, purpose: Purpose, payment_type: PaymentType) -> None:
+    def __init__(self, purpose: Purpose, payment_type: PaymentType, payer_account: AccountNumber) -> None:
         self.purpose = purpose
         self.payment_type = payment_type
+        self.payer_account = payer_account
 
     def check(self) -> None:
-        check_purpose(value=self.purpose, payment_type=self.payment_type)
+        check_purpose(value=self.purpose, payment_type=self.payment_type, payer_account=self.payer_account)
 
 
 class PayeeINNChecker(BaseChecker):
     def __init__(
         self,
         payee_inn: INN,
         payment_type: PaymentType
```

### Comparing `vitya-0.14.0/vitya/payment_order/payments/checks.py` & `vitya-0.15.0/vitya/payment_order/payments/checks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 from typing import Optional
 
-from vitya.payment_order.enums import PaymentType
+from vitya.payment_order.enums import AccountKind, PaymentType
 from vitya.payment_order.errors import (
     AccountValidationBICValueError,
     CBCValidationEmptyNotAllowed,
     DocumentDateValidationBOLenError,
     DocumentDateValidationCustomsLenError,
     DocumentDateValidationFNSOnlyEmptyError,
     DocumentNumberValidationBOEmptyNotAllowed,
@@ -46,35 +46,38 @@
     TaxPeriodValidationBOValueLenError,
     TaxPeriodValidationCustomsEmptyNotAllowed,
     TaxPeriodValidationCustomsValueLenError,
     TaxPeriodValidationFNS01OnlyEmpty,
     TaxPeriodValidationFNS02EmptyNotAllowed,
     TaxPeriodValidationFNSEmptyNotAllowed,
     TaxPeriodValidationFNSValueLenError,
+    UINValidationBONotEmpty,
     UINValidationFNSNotValueZeroError,
     UINValidationFNSValueZeroError,
     UINValidationValueZeroError,
 )
 from vitya.payment_order.fields import (
     CBC,
     UIN,
     AccountNumber,
     DocumentDate,
     DocumentNumber,
     OperationKind,
     PayerStatus,
     Purpose,
+    PurposeCode,
     Reason,
     TaxPeriod,
 )
 from vitya.payment_order.payments.constants import (
     CUSTOMS_REASONS,
     DOCUMENT_NUMBERS,
     FNS_PAYEE_ACCOUNT_NUMBER,
 )
+from vitya.payment_order.payments.tools import get_account_kind
 from vitya.pydantic_fields import BIC, INN, KPP, OKTMO
 
 
 def check_account_by_bic(
     account_number: AccountNumber,
     bic: BIC,
 ) -> None:
@@ -108,70 +111,77 @@
     if payment_type.is_budget:
         if value not in {'01', '02', '06'}:
             raise OperationKindValidationBudgetValueError
     return value
 
 
 def check_purpose_code(
-    value: Optional[int],
+    value: Optional[PurposeCode],
     payment_type: PaymentType,
-) -> Optional[int]:
+) -> Optional[PurposeCode]:
     if payment_type != PaymentType.FL:
         if value is not None:
             raise PurposeCodeValidationNullError
         return None
     if value is not None and value not in {1, 2, 3, 4, 5}:
         raise PurposeCodeValidationFlError
     return value
 
 
 def check_uin(
     value: Optional[UIN],
+    payee_account: AccountNumber,
     payment_type: PaymentType,
-    payer_status: PayerStatus,
+    payer_status: Optional[PayerStatus],
     payer_inn: Optional[str],
-) -> Optional[str]:
+) -> Optional[UIN]:
     if not payment_type.is_budget:
         return None
 
     if payer_status == '31' and value is None:
         raise UINValidationValueZeroError
 
     if payment_type == PaymentType.BUDGET_OTHER:
+        if payee_account.startswith('03212') and value is None:
+            raise UINValidationBONotEmpty
         return value
 
     if payment_type == PaymentType.FNS:
         if payer_status == '13' and payer_inn is None and value is None:
             raise UINValidationFNSValueZeroError
         if payer_status == '02':
             if value is not None:
                 raise UINValidationFNSNotValueZeroError
             return value
     return value
 
 
 def check_purpose(
     value: Optional[Purpose],
+    payer_account: AccountNumber,
     payment_type: PaymentType,
-) -> Optional[str]:
-    if value is None:
-        return None
-
-    if payment_type == PaymentType.IP:
-        if not re.search(r'(?i)\bНДС\b', value):
-            raise PurposeValidationIPNDSError
+) -> Optional[Purpose]:
+    if (
+        not payment_type.is_budget
+        and get_account_kind(payer_account) == AccountKind.IP
+        and (
+            value is None
+            or not re.search(r'(?i)\bНДС\b', value)
+        )
+    ):
+        raise PurposeValidationIPNDSError
     return value
 
 
 def check_payer_inn(
     value: Optional[INN],
     payment_type: PaymentType,
-    payer_status: PayerStatus,
-    for_third_face: bool = False,
-) -> Optional[str]:
+    payer_status: Optional[PayerStatus],
+    for_third_face: bool,
+) -> Optional[INN]:
     if not payment_type.is_budget:
         return value
 
     if value is None:
         if payment_type == PaymentType.BUDGET_OTHER:
             return None
         elif payment_type == PaymentType.FNS and payer_status == '13':
@@ -192,15 +202,15 @@
 
     return value
 
 
 def check_payee_inn(
     value: Optional[INN],
     payment_type: PaymentType,
-) -> Optional[str]:
+) -> Optional[INN]:
     if payment_type == PaymentType.IP:
         if value is None or len(value) != 12:
             raise PayeeINNValidationIPLenError
         return value
     elif payment_type == PaymentType.FL:
         if value is not None and len(value) != 12:
             raise PayeeINNValidationFLLenError
@@ -212,15 +222,15 @@
     return value
 
 
 def check_payer_status(
     value: Optional[PayerStatus],
     payment_type: PaymentType,
     for_third_face: bool,
-) -> Optional[str]:
+) -> Optional[PayerStatus]:
     if not payment_type.is_budget:
         return None
 
     if value is None:
         raise PayerStatusValidationNullNotAllowedError
 
     if payment_type == PaymentType.CUSTOMS and for_third_face and value == '06':
@@ -228,22 +238,22 @@
 
     return value
 
 
 def check_payer_kpp(
     value: Optional[KPP],
     payment_type: PaymentType,
-    payer_inn: str,
+    payer_inn: Optional[str],
 ) -> Optional[KPP]:
     if not payment_type.is_budget:
         return None
 
-    if len(payer_inn) == 10 and value is None:
+    if payer_inn is not None and len(payer_inn) == 10 and value is None:
         raise PayerKPPValidationINN10EmptyNotAllowed
-    elif len(payer_inn) == 12 and value is not None:
+    elif payer_inn is not None and len(payer_inn) == 12 and value is not None:
         raise PayerKPPValidationINN12OnlyEmptyError
     return value
 
 
 def check_payee_kpp(
     value: Optional[KPP],
     payment_type: PaymentType,
@@ -275,15 +285,15 @@
 
     return value
 
 
 def check_oktmo(
     value: Optional[OKTMO],
     payment_type: PaymentType,
-    payer_status: PayerStatus,
+    payer_status: Optional[PayerStatus],
 ) -> Optional[OKTMO]:
     if not payment_type.is_budget:
         return None
 
     if payment_type == PaymentType.FNS and payer_status in {'01', '13'} and value is None:
         return None
 
@@ -318,15 +328,15 @@
         raise ReasonValidationValueErrorCustoms
     return value
 
 
 def check_tax_period(
     value: Optional[TaxPeriod],
     payment_type: PaymentType,
-    payer_status: PayerStatus,
+    payer_status: Optional[PayerStatus],
 ) -> Optional[TaxPeriod]:
     if not payment_type.is_budget:
         return None
 
     if payment_type == PaymentType.BUDGET_OTHER:
         if value is None:
             return None
```

### Comparing `vitya-0.14.0/vitya/payment_order/payments/constants.py` & `vitya-0.15.0/vitya/payment_order/payments/constants.py`

 * *Files identical despite different names*

### Comparing `vitya-0.14.0/vitya/payment_order/validators.py` & `vitya-0.15.0/vitya/payment_order/validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import re
-from decimal import Decimal
+from decimal import Decimal, InvalidOperation
 from typing import Optional
 
 from vitya.payment_order.errors import (
     AccountNumberValidationDigitsOnlyError,
     AccountNumberValidationSizeError,
     AccountNumberValidationTypeError,
+    AmountNotANumber,
     AmountValidationLengthError,
     AmountValidationLessOrEqualZeroError,
     CBCValidationTypeError,
     CBCValidationValueCannotZerosOnly,
     CBCValidationValueDigitsOnlyError,
     CBCValidationValueLenError,
     CustomerValidationSizeError,
@@ -53,15 +54,18 @@
 
 
 def validate_amount(amount: str) -> Decimal:
     if isinstance(amount, str):
         if len(amount) > 18:
             raise AmountValidationLengthError
 
-    value = Decimal(amount)
+    try:
+        value = Decimal(amount)
+    except InvalidOperation:
+        raise AmountNotANumber
     if value <= Decimal(0.0):
         raise AmountValidationLessOrEqualZeroError
 
     return value
 
 
 def validate_customer(value: str) -> str:
```

### Comparing `vitya-0.14.0/vitya/pydantic_fields.py` & `vitya-0.15.0/vitya/pydantic_fields.py`

 * *Files identical despite different names*

### Comparing `vitya-0.14.0/vitya/validators.py` & `vitya-0.15.0/vitya/validators.py`

 * *Files identical despite different names*

### Comparing `vitya-0.14.0/vitya.egg-info/PKG-INFO` & `vitya-0.15.0/vitya.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vitya
-Version: 0.14.0
+Version: 0.15.0
 Summary: Validators for different russian banking values
 Home-page: https://github.com/hicebank/vitya
 Author: hicebank.ru
 Author-email: inyutin@hicebank.ru
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `vitya-0.14.0/vitya.egg-info/SOURCES.txt` & `vitya-0.15.0/vitya.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -17,8 +17,9 @@
 vitya/payment_order/enums.py
 vitya/payment_order/errors.py
 vitya/payment_order/fields.py
 vitya/payment_order/validators.py
 vitya/payment_order/payments/__init__.py
 vitya/payment_order/payments/checkers.py
 vitya/payment_order/payments/checks.py
-vitya/payment_order/payments/constants.py
+vitya/payment_order/payments/constants.py
+vitya/payment_order/payments/tools.py
```

