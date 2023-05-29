# Comparing `tmp/ldeep-1.0.8.tar.gz` & `tmp/ldeep-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ldeep-1.0.8.tar", last modified: Tue Jun 18 21:40:43 2019, max compression
+gzip compressed data, was "dist/ldeep-1.0.9.tar", last modified: Thu Dec 17 20:10:15 2020, max compression
```

## Comparing `ldeep-1.0.8.tar` & `ldeep-1.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 marauder  (1000) marauder  (1000)        0 2019-06-18 21:40:43.000000 ldeep-1.0.8/
--rw-r--r--   0 marauder  (1000) marauder  (1000)       41 2019-06-18 21:39:35.000000 ldeep-1.0.8/MANIFEST.in
--rw-r--r--   0 marauder  (1000) marauder  (1000)     8277 2019-06-18 21:40:43.000000 ldeep-1.0.8/PKG-INFO
--rw-r--r--   0 marauder  (1000) marauder  (1000)     6118 2019-06-18 21:39:35.000000 ldeep-1.0.8/README.rst
--rw-r--r--   0 marauder  (1000) marauder  (1000)        6 2019-06-18 21:40:27.000000 ldeep-1.0.8/VERSION
-drwxr-xr-x   0 marauder  (1000) marauder  (1000)        0 2019-06-18 21:40:43.000000 ldeep-1.0.8/ldeep/
--rw-r--r--   0 marauder  (1000) marauder  (1000)        0 2019-06-18 21:39:35.000000 ldeep-1.0.8/ldeep/__init__.py
--rwxr-xr-x   0 marauder  (1000) marauder  (1000)    17622 2019-06-18 21:39:35.000000 ldeep-1.0.8/ldeep/__main__.py
-drwxr-xr-x   0 marauder  (1000) marauder  (1000)        0 2019-06-18 21:40:43.000000 ldeep-1.0.8/ldeep/ldap/
--rw-r--r--   0 marauder  (1000) marauder  (1000)        0 2019-06-18 21:39:35.000000 ldeep-1.0.8/ldeep/ldap/__init__.py
--rw-r--r--   0 marauder  (1000) marauder  (1000)    10473 2019-06-18 21:39:35.000000 ldeep-1.0.8/ldeep/ldap/activedirectory.py
--rw-r--r--   0 marauder  (1000) marauder  (1000)     5728 2019-06-18 21:39:35.000000 ldeep-1.0.8/ldeep/ldap/constants.py
-drwxr-xr-x   0 marauder  (1000) marauder  (1000)        0 2019-06-18 21:40:43.000000 ldeep-1.0.8/ldeep/utils/
--rw-r--r--   0 marauder  (1000) marauder  (1000)     1754 2019-06-18 21:39:35.000000 ldeep-1.0.8/ldeep/utils/__init__.py
--rw-r--r--   0 marauder  (1000) marauder  (1000)     5323 2019-06-18 21:39:35.000000 ldeep-1.0.8/ldeep/utils/sddl.py
-drwxr-xr-x   0 marauder  (1000) marauder  (1000)        0 2019-06-18 21:40:43.000000 ldeep-1.0.8/ldeep.egg-info/
--rw-r--r--   0 marauder  (1000) marauder  (1000)     8277 2019-06-18 21:40:43.000000 ldeep-1.0.8/ldeep.egg-info/PKG-INFO
--rw-r--r--   0 marauder  (1000) marauder  (1000)      413 2019-06-18 21:40:43.000000 ldeep-1.0.8/ldeep.egg-info/SOURCES.txt
--rw-r--r--   0 marauder  (1000) marauder  (1000)        1 2019-06-18 21:40:43.000000 ldeep-1.0.8/ldeep.egg-info/dependency_links.txt
--rw-r--r--   0 marauder  (1000) marauder  (1000)       47 2019-06-18 21:40:43.000000 ldeep-1.0.8/ldeep.egg-info/entry_points.txt
--rw-r--r--   0 marauder  (1000) marauder  (1000)       74 2019-06-18 21:40:43.000000 ldeep-1.0.8/ldeep.egg-info/requires.txt
--rw-r--r--   0 marauder  (1000) marauder  (1000)        6 2019-06-18 21:40:43.000000 ldeep-1.0.8/ldeep.egg-info/top_level.txt
--rw-r--r--   0 marauder  (1000) marauder  (1000)        1 2019-06-18 21:40:43.000000 ldeep-1.0.8/ldeep.egg-info/zip-safe
--rw-r--r--   0 marauder  (1000) marauder  (1000)       74 2019-06-18 21:39:35.000000 ldeep-1.0.8/requirements.txt
--rw-r--r--   0 marauder  (1000) marauder  (1000)       38 2019-06-18 21:40:43.000000 ldeep-1.0.8/setup.cfg
--rw-r--r--   0 marauder  (1000) marauder  (1000)     1465 2019-06-18 21:39:35.000000 ldeep-1.0.8/setup.py
+drwxr-xr-x   0 marauder  (1000) marauder  (1000)        0 2020-12-17 20:10:15.155161 ldeep-1.0.9/
+-rw-r--r--   0 marauder  (1000) marauder  (1000)       41 2019-06-18 21:39:35.000000 ldeep-1.0.9/MANIFEST.in
+-rw-r--r--   0 marauder  (1000) marauder  (1000)     8277 2020-12-17 20:10:15.155161 ldeep-1.0.9/PKG-INFO
+-rw-r--r--   0 marauder  (1000) marauder  (1000)     6118 2019-06-18 21:39:35.000000 ldeep-1.0.9/README.rst
+-rw-r--r--   0 marauder  (1000) marauder  (1000)        6 2020-12-17 20:09:59.000000 ldeep-1.0.9/VERSION
+drwxr-xr-x   0 marauder  (1000) marauder  (1000)        0 2020-12-17 20:10:15.153161 ldeep-1.0.9/ldeep/
+-rw-r--r--   0 marauder  (1000) marauder  (1000)        0 2019-06-18 21:39:35.000000 ldeep-1.0.9/ldeep/__init__.py
+-rwxr-xr-x   0 marauder  (1000) marauder  (1000)    18410 2020-12-17 20:09:50.000000 ldeep-1.0.9/ldeep/__main__.py
+drwxr-xr-x   0 marauder  (1000) marauder  (1000)        0 2020-12-17 20:10:15.154161 ldeep-1.0.9/ldeep/ldap/
+-rw-r--r--   0 marauder  (1000) marauder  (1000)        0 2019-06-18 21:39:35.000000 ldeep-1.0.9/ldeep/ldap/__init__.py
+-rw-r--r--   0 marauder  (1000) marauder  (1000)    10473 2019-06-18 21:39:35.000000 ldeep-1.0.9/ldeep/ldap/activedirectory.py
+-rw-r--r--   0 marauder  (1000) marauder  (1000)     5729 2020-12-17 20:09:50.000000 ldeep-1.0.9/ldeep/ldap/constants.py
+drwxr-xr-x   0 marauder  (1000) marauder  (1000)        0 2020-12-17 20:10:15.155161 ldeep-1.0.9/ldeep/utils/
+-rw-r--r--   0 marauder  (1000) marauder  (1000)     1754 2019-06-18 21:39:35.000000 ldeep-1.0.9/ldeep/utils/__init__.py
+-rw-r--r--   0 marauder  (1000) marauder  (1000)     5848 2020-12-17 20:09:50.000000 ldeep-1.0.9/ldeep/utils/sddl.py
+drwxr-xr-x   0 marauder  (1000) marauder  (1000)        0 2020-12-17 20:10:15.153161 ldeep-1.0.9/ldeep.egg-info/
+-rw-r--r--   0 marauder  (1000) marauder  (1000)     8277 2020-12-17 20:10:15.000000 ldeep-1.0.9/ldeep.egg-info/PKG-INFO
+-rw-r--r--   0 marauder  (1000) marauder  (1000)      413 2020-12-17 20:10:15.000000 ldeep-1.0.9/ldeep.egg-info/SOURCES.txt
+-rw-r--r--   0 marauder  (1000) marauder  (1000)        1 2020-12-17 20:10:15.000000 ldeep-1.0.9/ldeep.egg-info/dependency_links.txt
+-rw-r--r--   0 marauder  (1000) marauder  (1000)       47 2020-12-17 20:10:15.000000 ldeep-1.0.9/ldeep.egg-info/entry_points.txt
+-rw-r--r--   0 marauder  (1000) marauder  (1000)       74 2020-12-17 20:10:15.000000 ldeep-1.0.9/ldeep.egg-info/requires.txt
+-rw-r--r--   0 marauder  (1000) marauder  (1000)        6 2020-12-17 20:10:15.000000 ldeep-1.0.9/ldeep.egg-info/top_level.txt
+-rw-r--r--   0 marauder  (1000) marauder  (1000)        1 2019-06-18 21:40:43.000000 ldeep-1.0.9/ldeep.egg-info/zip-safe
+-rw-r--r--   0 marauder  (1000) marauder  (1000)       74 2019-06-18 21:39:35.000000 ldeep-1.0.9/requirements.txt
+-rw-r--r--   0 marauder  (1000) marauder  (1000)       38 2020-12-17 20:10:15.155161 ldeep-1.0.9/setup.cfg
+-rw-r--r--   0 marauder  (1000) marauder  (1000)     1465 2019-06-18 21:39:35.000000 ldeep-1.0.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ldeep-1.0.8/PKG-INFO` & `ldeep-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ldeep
-Version: 1.0.8
+Version: 1.0.9
 Summary: In-depth ldap enumeration utility
 Home-page: https://github.com/franc-pentest/ldeep
 Author: b0z, flgy
 Author-email: bastien@faure.io, florian.guilbert@synacktiv.com
 License: MIT
 Description: =====
         LDEEP
```

### Comparing `ldeep-1.0.8/README.rst` & `ldeep-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `ldeep-1.0.8/ldeep/__main__.py` & `ldeep-1.0.9/ldeep/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -233,19 +233,21 @@
 			"msDS-MaximumPasswordAge",
 		]
 		psos = self.ldap.query(PSO_INFO_FILTER)
 		for policy in psos:
 			for field in FIELDS_TO_PRINT:
 				if isinstance(policy[field], list):
 					val = policy[field][0]
+				else:
+					val = policy[field]
 
 				if field in FILETIME_TIMESTAMP_FIELDS.keys():
 					val = int((fabs(float(val)) / 10**7) / FILETIME_TIMESTAMP_FIELDS[field][0])
 					val = "{val} {typ}".format(val=val, typ=FILETIME_TIMESTAMP_FIELDS[field][1])
-			print("{field}: {val}".format(field=field, val=val))
+				print("{field}: {val}".format(field=field, val=val))
 
 	def list_trusts(self, kwargs):
 		"""
 		List the domain's trust relationships.
 		"""
 		results = self.ldap.query(TRUSTS_INFO_FILTER)
 		FIELDS_TO_PRINT = ["dn", "cn", "securityIdentifier", "name", "trustDirection", "trustPartner", "trustType", "trustAttributes", "flatName"]
@@ -342,22 +344,44 @@
 	def get_memberships(self, kwargs):
 		"""
 		List the group for which `users` belongs to.
 
 		Arguments:
 			#user:string
 				User to list memberships
+			@recursive:bool
+				List recursively the groups
 		"""
 		user = kwargs["user"]
+		recursive = kwargs.get("recursive", False)
+
+		already_printed = set()
+
+		def lookup_groups(dn, leading_sp, already_treated):
+			groups = []
+			results = self.ldap.query("(distinguishedName={})".format(dn), ["memberOf"])
+			for result in results:
+				if "memberOf" in result:
+					for group_dn in result["memberOf"]:
+						if group_dn not in already_treated:
+							print("{g:>{width}}".format(g=group_dn, width=leading_sp + len(group_dn)))
+							already_treated.add(group_dn)
+							lookup_groups(group_dn, leading_sp + 4, already_treated)
+
+			return already_treated
 
 		results = self.ldap.query(USER_IN_GROUPS_FILTER.format(username=user), ["memberOf"])
 		for result in results:
 			if "memberOf" in result:
 				for group_dn in result["memberOf"]:
 					print(group_dn)
+					if recursive:
+						already_printed.add(group_dn)
+						s = lookup_groups(group_dn, 4, already_printed)
+						already_printed.union(s)
 			else:
 				error("No groups for user {}".format(user))
 
 	def get_from_sid(self, kwargs):
 		"""
 		Return the object associated with the given `sid`.
 
@@ -440,15 +464,15 @@
 				Comma separated list of attributes to display, ALL for every possible attribute
 		"""
 		attr = kwargs["attributes"]
 		filter_ = kwargs["filter"]
 
 		try:
 			if attr and attr != "ALL":
-				results = self.ldap.query(filter_, [attr])
+				results = self.ldap.query(filter_, attr.split(","))
 			else:
 				results = self.ldap.query(filter_)
 			self.display(results, True)
 		except Exception as e:
 			error(e)
 
 	def misc_all(self, kwargs):
@@ -550,15 +574,15 @@
 	Ldeep.add_subparsers(parser, ["list_", "get_", "misc_", "action_"], title="commands", description="available commands")
 	args = parser.parse_args()
 
 	# Authentication
 	method = "NTLM"
 	if args.kerberos:
 		method = "Kerberos"
-	elif args.username and args.password:
+	elif args.username:
 		method = "NTLM"
 	elif args.anonymous:
 		method = "anonymous"
 	else:
 		error("Lack of authentication options: either Kerberos or Username with Password (can be a NTLM hash).")
 
 	# Output
```

### Comparing `ldeep-1.0.8/ldeep/ldap/activedirectory.py` & `ldeep-1.0.9/ldeep/ldap/activedirectory.py`

 * *Files identical despite different names*

### Comparing `ldeep-1.0.8/ldeep/ldap/constants.py` & `ldeep-1.0.9/ldeep/ldap/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 }
 
 PWD_PROPERTIES = {
 	"DOMAIN_PASSWORD_COMPLEX": 0x1,
 	"DOMAIN_PASSWORD_NO_ANON_CHANGE": 0x2,
 	"DOMAIN_PASSWORD_NO_CLEAR_CHANGE": 0x4,
 	"DOMAIN_LOCKOUT_ADMINS": 0x8,
-	"DOMAIN_PASSWORD_STORE_CLEARTEXT": 0xf,
+	"DOMAIN_PASSWORD_STORE_CLEARTEXT": 0x10,
 	"DOMAIN_REFUSE_PASSWORD_CHANGE": 0x20
 }
 
 USER_LOCKED_FILTER = "(&(objectCategory=Person)(objectClass=user)(lockoutTime:1.2.840.113556.1.4.804:=4294967295))"
 GROUPS_FILTER = "(objectClass=group)"
 ZONES_FILTER = "(&(objectClass=dnsZone)(!(dc=RootDNSServers)))"
 ZONE_FILTER = "(objectClass=dnsNode)"
```

### Comparing `ldeep-1.0.8/ldeep/utils/__init__.py` & `ldeep-1.0.9/ldeep/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ldeep-1.0.8/ldeep/utils/sddl.py` & `ldeep-1.0.9/ldeep/utils/sddl.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 #!/usr/bin/env python3
 
+"""
+A module used to handle binary ntSecurityDescriptor from Active Directory LDAP.
+"""
+
 from struct import unpack
 
 from ldap3.protocol.formatters.formatters import format_sid, format_uuid
 
 SDDLTypeFlags = {
 	'Self Relative'					: 0b1000000000000000,
 	'RM Control Valid'				: 0b0100000000000000,
@@ -48,33 +52,53 @@
 	if out['Type']['DACL Present']:
 		out['DACL'] = parse_acl(input_buffer[out['Offset to DACL']:])
 
 	return out
 
 
 def resolve_flags(bfr, flags):
+	"""
+	Helper to resolve flag values and names.
+
+	Arguments:
+		#bfr:integer
+			The buffer containing flags.
+		#flags:dict
+			The dictionary of flag names and values.
+	"""
 	return {k: v & bfr != 0 for k, v in flags.items()}
 
 
 def parse_sddl_type(typeflags):
+	"""
+	Parses SDDL Type flags.
+	"""
 	return resolve_flags(typeflags, SDDLTypeFlags)
 
 
 def parse_acl(input_buffer):
+	"""
+	Parses ACL from SDDL.
+
+	Returns a list of ACEs.
+	"""
 	out = dict()
 	fields = ('Revision', 'Size', 'Num ACEs')
 
 	for k, v in zip(fields, unpack('<HHI', input_buffer[:8])):
 		out[k] = v
 
 	out['ACEs'] = parse_aces(input_buffer[8:8 + out['Size']], out['Num ACEs'])
 	return out
 
 
 def parse_aces(input_buffer, count):
+	"""
+	Parses the list of ACEs.
+	"""
 	out = []
 	while len(out) < count:
 		ace = dict()
 		fields = ('Raw Type', 'Raw Flags', 'Size', 'Raw Access Required')
 		for k, v in zip(fields, unpack('<BBHI', input_buffer[:8])):
 			ace[k] = v
 
@@ -129,24 +153,30 @@
 	'Ads List'				: 0b00000000000000000000000000000100,
 	'Ads Delete Child'		: 0b00000000000000000000000000000010,
 	'Ads Create Child'		: 0b00000000000000000000000000000001
 }
 
 
 def parse_ace_access(input_buffer):
+	"""
+	Parses access flags in an ACE.
+	"""
 	return resolve_flags(input_buffer, ACEAccessFlags)
 
 
 ACEObjectFlags = {
 	'Object Type Present'				: 0b00000000000000000000000000000010,
 	'Inherited Object Type Present'		: 0b00000000000000000000000000000001
 }
 
 
 def parse_ace_object_flags(input_buffer):
+	"""
+	Parses flags in an ACE containing an object.
+	"""
 	return resolve_flags(input_buffer, ACEObjectFlags)
 
 
 ACEType = {
 	0x00: 'Access Allowed',
 	0x01: 'Access Denied',
 	0x02: 'System Audit',
@@ -167,8 +197,11 @@
 	0x11: 'System Mandatory Label',
 	0x12: 'System Resource Attribute',
 	0x13: 'System Scoped Policy ID'
 }
 
 
 def parse_sddl_dacl_ace_type(ace_type):
+	"""
+	Parses the type of an ACE.
+	"""
 	return ACEType[ace_type]
```

### Comparing `ldeep-1.0.8/ldeep.egg-info/PKG-INFO` & `ldeep-1.0.9/ldeep.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ldeep
-Version: 1.0.8
+Version: 1.0.9
 Summary: In-depth ldap enumeration utility
 Home-page: https://github.com/franc-pentest/ldeep
 Author: b0z, flgy
 Author-email: bastien@faure.io, florian.guilbert@synacktiv.com
 License: MIT
 Description: =====
         LDEEP
```

### Comparing `ldeep-1.0.8/setup.py` & `ldeep-1.0.9/setup.py`

 * *Files identical despite different names*

