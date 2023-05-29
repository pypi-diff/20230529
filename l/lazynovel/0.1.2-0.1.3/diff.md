# Comparing `tmp/lazynovel-0.1.2.tar.gz` & `tmp/lazynovel-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazynovel-0.1.2.tar", last modified: Thu May 25 10:17:43 2023, max compression
+gzip compressed data, was "lazynovel-0.1.3.tar", last modified: Mon May 29 10:33:16 2023, max compression
```

## Comparing `lazynovel-0.1.2.tar` & `lazynovel-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-05-25 10:17:43.184049 lazynovel-0.1.2/
--rw-r--r--   0 zeroseeker   (501) staff       (20)    35181 2023-02-28 06:27:15.000000 lazynovel-0.1.2/LICENSE
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1305 2023-05-25 10:17:43.183885 lazynovel-0.1.2/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)      954 2023-02-28 06:27:15.000000 lazynovel-0.1.2/README.md
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-05-25 10:17:43.182518 lazynovel-0.1.2/lazynovel/
--rw-r--r--   0 zeroseeker   (501) staff       (20)      415 2023-05-25 10:17:10.000000 lazynovel-0.1.2/lazynovel/__init__.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     6989 2023-05-25 08:04:09.000000 lazynovel-0.1.2/lazynovel/crawler_changdu.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    10729 2023-02-28 06:27:15.000000 lazynovel-0.1.2/lazynovel/crawler_mbookcn.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1932 2023-02-28 06:27:15.000000 lazynovel-0.1.2/lazynovel/crawler_reading163.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    10568 2023-02-28 06:27:15.000000 lazynovel-0.1.2/lazynovel/open_changdu.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     9853 2023-02-28 06:27:15.000000 lazynovel-0.1.2/lazynovel/open_dianzhong.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     9680 2023-02-28 06:27:15.000000 lazynovel-0.1.2/lazynovel/open_mbookcn.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    14527 2023-02-28 06:27:15.000000 lazynovel-0.1.2/lazynovel/open_reading163.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      830 2023-02-28 06:27:15.000000 lazynovel-0.1.2/lazynovel/open_yangguang.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     2694 2023-02-28 06:27:15.000000 lazynovel-0.1.2/lazynovel/open_yiqbook.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    57844 2023-02-28 06:27:15.000000 lazynovel-0.1.2/lazynovel/open_yuewen.py
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-05-25 10:17:43.183554 lazynovel-0.1.2/lazynovel.egg-info/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1305 2023-05-25 10:17:43.000000 lazynovel-0.1.2/lazynovel.egg-info/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)      490 2023-05-25 10:17:43.000000 lazynovel-0.1.2/lazynovel.egg-info/SOURCES.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2023-05-25 10:17:43.000000 lazynovel-0.1.2/lazynovel.egg-info/dependency_links.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       15 2023-05-25 10:17:43.000000 lazynovel-0.1.2/lazynovel.egg-info/requires.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       10 2023-05-25 10:17:43.000000 lazynovel-0.1.2/lazynovel.egg-info/top_level.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2023-05-25 10:17:43.184151 lazynovel-0.1.2/setup.cfg
--rw-r--r--   0 zeroseeker   (501) staff       (20)      869 2023-05-25 10:17:25.000000 lazynovel-0.1.2/setup.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-05-29 10:33:16.983145 lazynovel-0.1.3/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    35181 2023-02-28 06:27:15.000000 lazynovel-0.1.3/LICENSE
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1305 2023-05-29 10:33:16.983034 lazynovel-0.1.3/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      954 2023-02-28 06:27:15.000000 lazynovel-0.1.3/README.md
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-05-29 10:33:16.982157 lazynovel-0.1.3/lazynovel/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      415 2023-05-25 10:17:10.000000 lazynovel-0.1.3/lazynovel/__init__.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     6989 2023-05-25 08:04:09.000000 lazynovel-0.1.3/lazynovel/crawler_changdu.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    10729 2023-02-28 06:27:15.000000 lazynovel-0.1.3/lazynovel/crawler_mbookcn.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1932 2023-02-28 06:27:15.000000 lazynovel-0.1.3/lazynovel/crawler_reading163.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    10568 2023-02-28 06:27:15.000000 lazynovel-0.1.3/lazynovel/open_changdu.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     9853 2023-02-28 06:27:15.000000 lazynovel-0.1.3/lazynovel/open_dianzhong.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     9680 2023-02-28 06:27:15.000000 lazynovel-0.1.3/lazynovel/open_mbookcn.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    21587 2023-05-29 10:32:37.000000 lazynovel-0.1.3/lazynovel/open_reading163.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      830 2023-02-28 06:27:15.000000 lazynovel-0.1.3/lazynovel/open_yangguang.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     2694 2023-02-28 06:27:15.000000 lazynovel-0.1.3/lazynovel/open_yiqbook.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    57844 2023-02-28 06:27:15.000000 lazynovel-0.1.3/lazynovel/open_yuewen.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-05-29 10:33:16.982858 lazynovel-0.1.3/lazynovel.egg-info/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1305 2023-05-29 10:33:16.000000 lazynovel-0.1.3/lazynovel.egg-info/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      490 2023-05-29 10:33:16.000000 lazynovel-0.1.3/lazynovel.egg-info/SOURCES.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2023-05-29 10:33:16.000000 lazynovel-0.1.3/lazynovel.egg-info/dependency_links.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       15 2023-05-29 10:33:16.000000 lazynovel-0.1.3/lazynovel.egg-info/requires.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       10 2023-05-29 10:33:16.000000 lazynovel-0.1.3/lazynovel.egg-info/top_level.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2023-05-29 10:33:16.983196 lazynovel-0.1.3/setup.cfg
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      869 2023-05-29 10:32:37.000000 lazynovel-0.1.3/setup.py
```

### Comparing `lazynovel-0.1.2/LICENSE` & `lazynovel-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.2/PKG-INFO` & `lazynovel-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazynovel
-Version: 0.1.2
+Version: 0.1.3
 Summary: 小说平台接口封包
 Home-page: https://gitee.com/ZeroSeeker/lazynovel
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `lazynovel-0.1.2/README.md` & `lazynovel-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.2/lazynovel/crawler_changdu.py` & `lazynovel-0.1.3/lazynovel/crawler_changdu.py`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.2/lazynovel/crawler_mbookcn.py` & `lazynovel-0.1.3/lazynovel/crawler_mbookcn.py`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.2/lazynovel/crawler_reading163.py` & `lazynovel-0.1.3/lazynovel/crawler_reading163.py`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.2/lazynovel/open_changdu.py` & `lazynovel-0.1.3/lazynovel/open_changdu.py`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.2/lazynovel/open_dianzhong.py` & `lazynovel-0.1.3/lazynovel/open_dianzhong.py`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.2/lazynovel/open_mbookcn.py` & `lazynovel-0.1.3/lazynovel/open_mbookcn.py`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.2/lazynovel/open_reading163.py` & `lazynovel-0.1.3/lazynovel/open_reading163.py`

 * *Files 24% similar despite different names*

```diff
@@ -419,7 +419,181 @@
     url = 'https://quickbi.yunydbook163.com/dist-api/recharge/list'
     response = requests.request(
         method='GET',
         url=url,
         params=data
     )
     return response.json()
+
+
+def get_user_data(
+        consumer_key: str,
+        secret_key: str,
+        site_id: int,
+        start_time: int = None,
+        end_time: int = None,
+        page: int = 1,
+        page_size: int = 20,
+        user_id: str = None,
+        user_openid: str = None
+):
+    """
+    2.3. 分销站点用户信息列表
+    适用于微信公众号
+
+    输入参数
+        名称	类型	必须	描述
+        consumerkey	long	是	分销商唯一标识
+        timestamp	long	是	当前时间戳，取13位毫秒时间戳
+        sign	string	是	API输入参数签名结果，使用md5加密,见MD5签名规则
+        siteid	long	是	站点id
+        starttime	long	否	开始时间，格式yyyyMMddHHmm 包含
+        endtime	long	否	结束时间，格式yyyyMMddHHmm 不包含
+        pageSize	int	否	默认一页显示20条记录,可以根据自身需求设置，限制10000条
+        page	int	否	默认第一页
+        userid	long	否	用户id
+        useropenid	string	否	用户公众号openid
+
+    注：
+        1. userid和useropenid选择其一即可，若都不选则按照siteid维度获取用户
+        2. siteid维度获取用户时，starttime和endtime不传默认获取当天的用户信息列表
+        3. 请求参数包含userid或useropenid，则starttime和endtime参数条件将无效
+
+    返回结果
+        名称	类型	必须	描述
+        code	int	是	返回值
+        message	string	是	信息描述
+        totalPage	int	是	总页数
+        userId	long	是	用户id
+        nickName	string	是	用户昵称
+        gender	string	是	性别 ：0-未知，1-男，2-女
+        userRegisterTime	long	是	用户注册时间
+        userFollowed	int	是	是否关注：0-未关注，1-关注
+        firstFocusTime	 long	是	关注时间
+        appId	String	是	公众号appid
+        wxMpName	String	是	公众号名称
+        wxOpenId	String	是	微信用户openId
+        vip	int	是	是否包年：0-非包年，1-包年
+        vipEndTime	String	否	包年结束时间：xx年xx月xx日
+        balance	int	是	阅点余额
+        hongbao	int	是	有效的红包余额
+        totalRechargeMoney	long	是	总充值金额
+        totalRechargeTimes	int	是	总充值次数
+        linkId	long	否	链接ID
+        linkName	String	否	推广链接名称
+
+    data详情：
+        名称	类型	必须	描述
+        totalPage	int	是	当前查询条件对应结果集列表总页数
+        rechargeSid	string	是	充值流水号，唯一
+        money	int	是	充值金额，单位分
+        payStatus	int	是	充值状态 0：未付款；1：已付款
+        payTime	long	否	支付时间，13位毫秒时间戳，payStatus=1时有值
+        ewTradeId	string	否	支付订单的订单号，payStatus=1时有值
+        createTime	long	是	下单时间，13位毫秒时间戳
+        updateTime	long	是	订单状态更新时间，13位毫秒时间戳
+        userId	long	是	用户id
+        userRegisterTime	long	是	用户注册时间，13位毫秒时间戳
+        userLinkId	long	否	用户注册时的推广链接id
+        bookId	string	否	订单关联书籍id
+        bookTitle	string	否	订单关联书籍名称
+        subProviderEmail	string	否	用户关联的子账号邮箱，可能为null，表示不关联任何子账号
+        subProviderName	string	否	用户关联的子账号姓名/昵称，可能为null，表示不关联任何子账号
+        aid	string	否	广告计划id，字符串格式，可能为null
+        cid	string	否	广告创意id，字符串格式，可能为null
+
+    返回示例:
+        {
+            "code": 200,
+            "data": {
+                "userData": [
+                    {
+                        "userId": 111341,
+                        "nickName": "李白",
+                        "gender": 1,
+                        "userRegisterTime": 1586863158396,
+                        "userFollowed": 1,
+                        "firstFocusTime": 1586863162805,
+                        "appId": "wx9b1ec4dd515bb949",
+                        "wxMpName": "测试一号站",
+                        "wxOpenId": "o2JVZv_V8yHARgoisIzbBSxr830s",
+                        "vip": 1,
+                        "vipEndTime": "2022年01月12日",
+                        "balance": 28332,
+                        "hongbao": 0,
+                        "totalRechargeMoney": 66800,
+                        "totalRechargeTimes": 12,
+                        "linkId": null,
+                        "linkName": null
+                    },
+                    {
+                        "userId": 112301,
+                        "nickName": "马可波罗",
+                        "gender": 1,
+                        "userRegisterTime": 1586922884095,
+                        "userFollowed": 1,
+                        "firstFocusTime": 1586922884125,
+                        "appId": "wx9b1ec4dd515bb949",
+                        "wxMpName": "测试一号站",
+                        "wxOpenId": "o2JVZv42ED7K2IJOdMyFs-zjnfo4",
+                        "vip": 0,
+                        "vipEndTime": null,
+                        "balance": 0,
+                        "hongbao": 0,
+                        "totalRechargeMoney": 0,
+                        "totalRechargeTimes": 0,
+                        "linkId": null,
+                        "linkName": null
+                    },
+                    {
+                        "userId": 112303,
+                        "nickName": "赵云",
+                        "gender": 1,
+                        "userRegisterTime": 1586934346881,
+                        "userFollowed": 1,
+                        "firstFocusTime": 1586934348909,
+                        "appId": "wx9b1ec4dd515bb949",
+                        "wxMpName": "测试一号站",
+                        "wxOpenId": "o2JVZv17OU-gyulUfFUR5ZWie9j8",
+                        "vip": 1,
+                        "vipEndTime": "2022年12月29日",
+                        "balance": 11200,
+                        "hongbao": 0,
+                        "totalRechargeMoney": 88589,
+                        "totalRechargeTimes": 8,
+                        "linkId": null,
+                        "linkName": null
+                    },
+                ],
+                "totalPage": 1
+            },
+            "message": "success"
+        }
+    """
+    local_data = {
+        'siteid': site_id
+    }
+    if start_time:
+        local_data['starttime'] = start_time
+    if end_time:
+        local_data['endtime'] = end_time
+    if page_size:
+        local_data['pageSize'] = page_size
+    if page:
+        local_data['page'] = page
+    if user_id:
+        local_data['userid'] = user_id
+    if user_openid:
+        local_data['useropenid'] = user_openid
+
+    data = make_sign(
+        consumer_key=consumer_key,
+        secret_key=secret_key,
+        data=local_data
+    )
+    url = 'https://bi.reading.163.com/dist-api/getUserData'
+    response = requests.request(
+        method='GET',
+        url=url,
+        params=data
+    )
+    return response.json()
```

### Comparing `lazynovel-0.1.2/lazynovel/open_yangguang.py` & `lazynovel-0.1.3/lazynovel/open_yangguang.py`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.2/lazynovel/open_yiqbook.py` & `lazynovel-0.1.3/lazynovel/open_yiqbook.py`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.2/lazynovel/open_yuewen.py` & `lazynovel-0.1.3/lazynovel/open_yuewen.py`

 * *Files identical despite different names*

### Comparing `lazynovel-0.1.2/lazynovel.egg-info/PKG-INFO` & `lazynovel-0.1.3/lazynovel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazynovel
-Version: 0.1.2
+Version: 0.1.3
 Summary: 小说平台接口封包
 Home-page: https://gitee.com/ZeroSeeker/lazynovel
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `lazynovel-0.1.2/setup.py` & `lazynovel-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lazynovel",
-    version="0.1.2",
+    version="0.1.3",
     description="小说平台接口封包",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ZeroSeeker",
     author_email="zeroseeker@foxmail.com",
     url="https://gitee.com/ZeroSeeker/lazynovel",
     packages=setuptools.find_packages(),
```

