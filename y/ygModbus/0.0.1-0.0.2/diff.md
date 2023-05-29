# Comparing `tmp/ygModbus-0.0.1-py3-none-any.whl.zip` & `tmp/ygModbus-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3105 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat       19 b- defN 23-May-25 23:03 ygModbus/__init__.py
--rw-rw-rw-  2.0 fat      272 b- defN 23-May-25 23:04 ygModbus/client.py
--rw-rw-rw-  2.0 fat     2185 b- defN 23-May-25 23:08 ygModbus/server.py
--rw-rw-rw-  2.0 fat      448 b- defN 23-May-25 23:53 ygModbus-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-25 23:53 ygModbus-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       50 b- defN 23-May-25 23:53 ygModbus-0.0.1.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        9 b- defN 23-May-25 23:53 ygModbus-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      620 b- defN 23-May-25 23:53 ygModbus-0.0.1.dist-info/RECORD
-8 files, 3695 bytes uncompressed, 2017 bytes compressed:  45.4%
+Zip file size: 3655 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat       19 b- defN 23-May-29 11:11 ygModbus/__init__.py
+-rw-rw-rw-  2.0 fat      278 b- defN 23-May-29 10:31 ygModbus/client.py
+-rw-rw-rw-  2.0 fat     4135 b- defN 23-May-29 11:11 ygModbus/server.py
+-rw-rw-rw-  2.0 fat      601 b- defN 23-May-29 11:22 ygModbus-0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-29 11:22 ygModbus-0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       50 b- defN 23-May-29 11:22 ygModbus-0.0.2.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        9 b- defN 23-May-29 11:22 ygModbus-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      620 b- defN 23-May-29 11:22 ygModbus-0.0.2.dist-info/RECORD
+8 files, 5804 bytes uncompressed, 2567 bytes compressed:  55.8%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: ygModbus/client.py
 Comment: 
 
 Filename: ygModbus/server.py
 Comment: 
 
-Filename: ygModbus-0.0.1.dist-info/METADATA
+Filename: ygModbus-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: ygModbus-0.0.1.dist-info/WHEEL
+Filename: ygModbus-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: ygModbus-0.0.1.dist-info/entry_points.txt
+Filename: ygModbus-0.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: ygModbus-0.0.1.dist-info/top_level.txt
+Filename: ygModbus-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: ygModbus-0.0.1.dist-info/RECORD
+Filename: ygModbus-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ygModbus/__init__.py

```diff
@@ -1 +1 @@
-__version__='0.0.1'
+__version__='0.0.2'
```

## ygModbus/client.py

```diff
@@ -1,9 +1,9 @@
-import pandas as pd
+# import pandas as pd
 import datetime as dt
-import sqlalchemy
-from sqlalchemy import create_engine
+# import sqlalchemy
+# from sqlalchemy import create_engine
 from pyModbusTCP.client import ModbusClient
 
 c = ModbusClient(host="127.0.0.1", port=502, auto_open=True)
 regs = c.read_holding_registers(reg_addr=40001,reg_nb=4)
 regs
```

## ygModbus/server.py

```diff
@@ -3,61 +3,111 @@
 """
 Modbus/TCP server with start/stop schedule
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Run this as root to listen on TCP privileged ports (<= 1024).
 
 Default Modbus/TCP port is 502, so we prefix call with sudo. With argument
-"--host 0.0.0.0", server listen on all IPv4 of the host. Instead of just
-open tcp/502 on local interface.
+"--host 0.0.0.0", the server listens on all IPv4 interfaces of the host, instead of just
+opening tcp/502 on the local interface.
 $ sudo ./server_schedule.py --host 0.0.0.0
 """
 
 import argparse
-from datetime import datetime
-from random import randint
+import json
+import random
+import signal
+import sys
 import time
+from datetime import datetime
 from pyModbusTCP.server import ModbusServer, DataBank
-# need https://github.com/dbader/schedule
 import schedule
 
 
 class MyDataBank(DataBank):
-    """A custom ModbusServerDataBank for override get_holding_registers method."""
+    """A custom ModbusServerDataBank for overriding the get_holding_registers method."""
 
-    def __init__(self):
-        # turn off allocation of memory for standard modbus object types
-        # only "holding registers" space will be replaced by dynamic build values.
+    def __init__(self, register_params):
+        # Turn off allocation of memory for standard Modbus object types.
+        # Only "holding registers" space will be replaced by dynamically built values.
         super().__init__(virtual_mode=True)
+        self.register_params = register_params
+        self.latest_data = {}
+
+    def update_holding_registers(self):
+        """Update the holding registers with random values based on the given parameters."""
+        for address, params in self.register_params.items():
+            self.latest_data[address] = random.randint(params['min_int'], params['max_int'])
+        self.set_holding_registers(0, list(self.latest_data.values()))
 
     def get_holding_registers(self, address, number=1, srv_info=None):
-        """Get virtual holding registers."""
+        """Get the latest values of holding registers."""
         try:
-            print('getting holding_registers')
-            return [randint(0,65535) for a in range(address, address+number)]
+            print(self.latest_data)
+            return [self.latest_data.get(str(a), 0) for a in range(address, address + number)]
         except KeyError:
             return
 
+def run_server():
+    # Parse command-line arguments
+    parser = argparse.ArgumentParser()
+    parser.add_argument('-H', '--host', type=str, default='127.0.0.1', help='Host (default: 127.0.0.1)')
+    parser.add_argument('-p', '--port', type=int, default=502, help='TCP port (default: 502)')
+    parser.add_argument('-j', '--json', type=str, default='register_params.json', help='JSON file with register parameters (default: register_params.json)')
+    parser.add_argument('-i', '--interval', type=float, default=1.0, help='Interval in seconds for updating holding registers (default: 1.0)')
+    args = parser.parse_args()
+
+    # Load register parameters from JSON file
+    try:
+        with open(args.json) as json_file:
+            register_params = json.load(json_file)
+    except FileNotFoundError:
+        print(f'Error: JSON file "{args.json}" not found.')
+        return
+    except json.JSONDecodeError:
+        print(f'Error: Invalid JSON format in "{args.json}".')
+        return
+
+    # Initialize Modbus server and start it
+    server = ModbusServer(host=args.host, port=args.port, no_block=True, data_bank=MyDataBank(register_params))
+    server.start()
+    print('Modbus TCP server is running on', args.host)
+
+    def terminate_server(signal, frame):
+        """Handler for terminating the server gracefully."""
+        print('\nTerminating server...')
+        server.stop()
+        sys.exit(0)
+
+    # Register signal handler for Ctrl+C
+    signal.signal(signal.SIGINT, terminate_server)
+
+    def update_holding_registers():
+        """Update the holding registers with random values based on the given parameters."""
+        server.data_bank.update_holding_registers()
+
+    # Schedule the update of holding registers at the specified interval
+    schedule.every(args.interval).seconds.do(update_holding_registers)
+
+    # Main loop
+    while True:
+        schedule.run_pending()
+        time.sleep(0.1)
+
+
+# if __name__ == "__main__":
+#     run_server()
+
+# run_server()
+
+if __name__ == "__main__":
+    parser = argparse.ArgumentParser(prog="ygModbus")
+    subparsers = parser.add_subparsers(dest="command")
+
+    runserver_parser = subparsers.add_parser("runserver", help="Run the server")
+
+    args = parser.parse_args()
+
+    if args.command == "runserver":
+        run_server()
+
 
-# parse args
-parser = argparse.ArgumentParser()
-parser.add_argument('-H', '--host', type=str, default='127.0.0.1', help='Host (default: 127.0.0.1)')
-parser.add_argument('-p', '--port', type=int, default=502, help='TCP port (default: 502)')
-args = parser.parse_args()
-# init modbus server and start it
-# server = ModbusServer(host=args.host, port=args.port, data_bank=MyDataBank())
-server = ModbusServer(host=args.host, port=args.port, no_block=True,data_bank=MyDataBank())
-server.start()
-print('Modbus TCP server is running on 127.0.0.1...')
-
-
-# init scheduler
-# schedule a daily downtime (from 18:00 to 06:00)
-# schedule.every().day.at('18:00').do(server.stop)
-# schedule.every().day.at('06:00').do(server.start)
-# update life word at @0
-# schedule.every(10).seconds.do(server.data_bank.set_holding_registers)
-
-# main loop
-while True:
-    schedule.run_pending()
-    time.sleep(1)
```

