# Comparing `tmp/momonga-0.0.2-py3-none-any.whl.zip` & `tmp/momonga-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 15389 bytes, number of entries: 11
+Zip file size: 15387 bytes, number of entries: 11
 -rw-rw-r--  2.0 unx      136 b- defN 24-Apr-20 08:49 momonga/__init__.py
--rw-rw-r--  2.0 unx    15099 b- defN 24-Apr-24 01:01 momonga/momonga.py
+-rw-rw-r--  2.0 unx    15159 b- defN 24-Apr-24 09:30 momonga/momonga.py
 -rw-rw-r--  2.0 unx      959 b- defN 24-Apr-23 04:16 momonga/momonga_exception.py
--rw-rw-r--  2.0 unx     2698 b- defN 24-Apr-20 01:17 momonga/momonga_response.py
--rw-rw-r--  2.0 unx    11964 b- defN 24-Apr-23 23:20 momonga/momonga_session_manager.py
--rw-rw-r--  2.0 unx     9392 b- defN 24-Apr-20 07:30 momonga/momonga_sk_wrapper.py
--rw-rw-r--  2.0 unx     1061 b- defN 24-Apr-24 01:25 momonga-0.0.2.dist-info/LICENSE
--rw-rw-r--  2.0 unx    10281 b- defN 24-Apr-24 01:25 momonga-0.0.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-24 01:25 momonga-0.0.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx        8 b- defN 24-Apr-24 01:25 momonga-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      883 b- defN 24-Apr-24 01:25 momonga-0.0.2.dist-info/RECORD
-11 files, 52573 bytes uncompressed, 13903 bytes compressed:  73.6%
+-rw-rw-r--  2.0 unx     2698 b- defN 24-Apr-24 09:24 momonga/momonga_response.py
+-rw-rw-r--  2.0 unx    11967 b- defN 24-Apr-24 09:20 momonga/momonga_session_manager.py
+-rw-rw-r--  2.0 unx     9392 b- defN 24-Apr-24 09:23 momonga/momonga_sk_wrapper.py
+-rw-rw-r--  2.0 unx     1061 b- defN 24-Apr-24 09:31 momonga-0.0.3.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    10268 b- defN 24-Apr-24 09:31 momonga-0.0.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-24 09:31 momonga-0.0.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        8 b- defN 24-Apr-24 09:31 momonga-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      883 b- defN 24-Apr-24 09:31 momonga-0.0.3.dist-info/RECORD
+11 files, 52623 bytes uncompressed, 13901 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: momonga/momonga_session_manager.py
 Comment: 
 
 Filename: momonga/momonga_sk_wrapper.py
 Comment: 
 
-Filename: momonga-0.0.2.dist-info/LICENSE
+Filename: momonga-0.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: momonga-0.0.2.dist-info/METADATA
+Filename: momonga-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: momonga-0.0.2.dist-info/WHEEL
+Filename: momonga-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: momonga-0.0.2.dist-info/top_level.txt
+Filename: momonga-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: momonga-0.0.2.dist-info/RECORD
+Filename: momonga-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## momonga/momonga.py

```diff
@@ -75,22 +75,22 @@
         else:
             esv = b'\x62' # get
         epc  = epc.to_bytes(1, 'big')
         pdc = len(edt).to_bytes(1, 'big')
 
         return ehd + tid + seoj + deoj + esv + opc + epc + pdc + edt
 
-    def __extruct_response_payload(self,
+    def __extract_response_payload(self,
                                    data: bytes,
                                    tid: int,
                                    epc: int,
                                   ):
         ehd = data[0:2]
         if  ehd != b'\x10\x81': # econet lite edata format 1
-            raise MomongaResponseNotExpected('The data format is not Econet Lite data format 1')
+            raise MomongaResponseNotExpected('The data format is not Econet Lite EDATA format 1')
 
         if int.from_bytes(data[2:4], 'big') != tid:
             raise MomongaResponseNotExpected('The transaction ID does not match.')
 
         seoj = data[4:7]
         if seoj != b'\x02\x88\x01': # low-voltage smart electric energy meter class
             raise MomongaResponseNotExpected('The source is not a smart meter.')
@@ -127,51 +127,51 @@
 
         for _ in range(12):
             self.session_manager.xmitter(tx_payload)
             while True:
                 try:
                     res = self.session_manager.recv_q.get(timeout=12)
                 except queue.Empty:
-                    logger.warning('Timed out to obtain a response for "%X" reqeust.' % (epc))
+                    logger.warning('Timed out to obtain a response for "%X" request.' % (epc))
                     break
                 if res.startswith('EVENT 21'):
                     param = res.split()[-1]
                     if param == '00':
-                        logger.info('Successfully transmitted a packet for "%X" reqeust.' % (epc))
+                        logger.info('Successfully transmitted a packet for "%X" request.' % (epc))
                         continue
                     elif param == '01':
-                        logger.warning('Retransmitting the packet for "%X" reqeust.' % (epc))
+                        logger.warning('Retransmitting the packet for "%X" request.' % (epc))
                         break # to rexmit
                     elif param == '02':
-                        logger.warning('Automatically retrying to transmit the packet for "%X" reqeust.' % (epc))
+                        logger.warning('Automatically retrying to transmit the packet for "%X" request.' % (epc))
                         continue
                 elif res.startswith('EVENT 02'):
-                    logger.info('Successfully retransmitted the packet for "%X" reqeust.' % (epc))
+                    logger.info('Successfully retransmitted the packet for "%X" request.' % (epc))
                     continue
                 elif res.startswith('ERXUDP'):
                     udp_pkt = SkEventRxUdp([res])
                     if not (udp_pkt.src_port == udp_pkt.dst_port == 0x0E1A):
                         continue
                     elif udp_pkt.side != 0:
                         continue
                     elif udp_pkt.src_addr != self.session_manager.smart_meter_addr:
                         continue
 
                     try:
-                        rx_payload = self.__extruct_response_payload(udp_pkt.data,
+                        rx_payload = self.__extract_response_payload(udp_pkt.data,
                                                                      self.transaction_id,
                                                                      epc)
                     except MomongaResponseNotExpected:
                         continue
 
-                    logger.info('Successfully received a packet for "%X" resnponse.' % (epc))
+                    logger.info('Successfully received a packet for "%X" response.' % (epc))
                     return rx_payload
 
-        logger.error('Gave up to obtain a response for "%X" reqeust. Close Momonga and open it again.' % (epc))
-        raise MomongaNeedToReopen('Gave up to obtain a response for "%X" reqeust. Close Momonga and open it again.' % (epc))
+        logger.error('Gave up to obtain a response for "%X" request. Close Momonga and open it again.' % (epc))
+        raise MomongaNeedToReopen('Gave up to obtain a response for "%X" request. Close Momonga and open it again.' % (epc))
 
     def __prepare_to_get_cumulative_energy(self) -> None:
         if self.energy_coefficient is None:
             try:
                 self.energy_coefficient = self.get_coefficient_for_cumulative_energy()
             except MomongaResponseNotPossible:
                 self.energy_coefficient = 1
@@ -304,18 +304,21 @@
                                       edt[2], edt[3], edt[4], edt[5], edt[6])
         cumulative_energy = int.from_bytes(edt[7:], 'big')
         cumulative_energy *= self.energy_coefficient
         cumulative_energy *= self.energy_unit 
         return {'timestamp': timestamp,
                 'cumulative_energy': cumulative_energy}
 
-    def get_historical_cumulative_energy_2(self,
-                                           timestamp: datetime.datetime = datetime.datetime.now(),
+    def get_historical_cumulative_energy_3(self,
+                                           timestamp: datetime.datetime = None,
                                            num_of_data_points: int = 12,
                                           ) -> list:
+        if timestamp is None:
+            timestamp = datetime.datetime.now()
+
         self.__prepare_to_get_cumulative_energy()
         self.set_time_for_which_to_retrieve_historical_data_2(timestamp, num_of_data_points)
 
         res = self.__request(0xEC)
         edt = res.get('edt')
         year = int.from_bytes(edt[0:2], 'big')
         num_of_data_points = edt[6]
```

## momonga/momonga_response.py

```diff
@@ -6,71 +6,71 @@
     def __init__(self, res):
         self.raw_response = res
         self.decode()
 
     def decode(self):
         pass
 
-    def extruct(self, key):
+    def extract(self, key):
         for elm in reversed(self.raw_response):
             if key in elm:
                 return elm
         raise MomongaKeyError(key)
 
 class SkVerResponse(MomongaSkResponseBase):
     def decode(self):
-        res_list = self.extruct('EVER').split()
+        res_list = self.extract('EVER').split()
         self.stack_ver = res_list[1]
 
 
 class SkAppVerResponse(MomongaSkResponseBase):
     def decode(self):
-        res_list = self.extruct('EAPPVER').split()
+        res_list = self.extract('EAPPVER').split()
         self.app_ver = res_list[1]
 
 
 class SkInfoResponse(MomongaSkResponseBase):
     def decode(self):
-        res_list = self.extruct('EINFO').split()
+        res_list = self.extract('EINFO').split()
         self.ip6_addr = res_list[1]
         self.mac_addr = bytes.fromhex(res_list[2])
         self.channel = int(res_list[3], 16)
         self.pan_id = bytes.fromhex(res_list[4])
         self.side = int(res_list[5], 16)
 
 
 class SkScanResponse(MomongaSkResponseBase):
     def decode(self):
-        self.channel = int(self.extruct('Channel:').split(':')[-1], 16)
-        self.channel_page = int(self.extruct('Channel Page:').split(':')[-1], 16)
-        self.pan_id = bytes.fromhex(self.extruct('Pan ID:').split(':')[-1])
-        self.mac_addr = bytes.fromhex(self.extruct('Addr:').split(':')[-1])
-        self.lqi = int(self.extruct('LQI:').split(':')[-1], 16)
+        self.channel = int(self.extract('Channel:').split(':')[-1], 16)
+        self.channel_page = int(self.extract('Channel Page:').split(':')[-1], 16)
+        self.pan_id = bytes.fromhex(self.extract('Pan ID:').split(':')[-1])
+        self.mac_addr = bytes.fromhex(self.extract('Addr:').split(':')[-1])
+        self.lqi = int(self.extract('LQI:').split(':')[-1], 16)
         self.rssi = 0.275 * self.lqi - 104.27
-        self.side = int(self.extruct('Side:').split(':')[-1], 16)
-        self.pair_id = bytes.fromhex(self.extruct('PairID:').split(':')[-1])
+        self.side = int(self.extract('Side:').split(':')[-1], 16)
+        self.pair_id = bytes.fromhex(self.extract('PairID:').split(':')[-1])
 
 
 class SkLl64Response(MomongaSkResponseBase):
     def decode(self):
-        self.ip6_addr = self.extruct('FE80:')
+        self.ip6_addr = self.extract('FE80:')
 
 
 class SkSendToResponse(MomongaSkResponseBase):
     def decode(self):
-        self.res_list = self.extruct('EVENT 21').split()
+        self.res_list = self.extract('EVENT 21').split()
         self.event_num = int(self.res_list[1], 16)
         self.src_addr = self.res_list[2]
         self.side = int(self.res_list[3], 16)
         self.param = int(self.res_list[4], 16)
 
 
 class SkEventRxUdp(MomongaSkResponseBase):
     def decode(self):
-        self.res_list = self.extruct('ERXUDP').split()
+        self.res_list = self.extract('ERXUDP').split()
         self.src_addr = self.res_list[1]
         self.des_addr = self.res_list[2]
         self.src_port = int(self.res_list[3], 16)
         self.dst_port = int(self.res_list[4], 16)
         self.src_mac = bytes.fromhex(self.res_list[5])
         self.lqi = int(self.res_list[6], 16)
         self.rssi = 0.275 * self.lqi - 104.27
```

## momonga/momonga_session_manager.py

```diff
@@ -72,15 +72,15 @@
 
             # to disable echoback.
             #self.sksreg('SFE', '0')
 
             # to show the rssi of the received packets.
             self.skw.sksreg('SA2', '1')
 
-            # scaning a PAN from here.
+            # scanning a PAN from here.
             # to set a route b id.
             self.skw.sksetrbid(self.rbid)
             # to set a pasword.
             self.skw.sksetpwd(self.pwd)
             logger.info('The Route-B ID and the password were registered.')
             try:
                 logger.info('Scanning PAN channels...')
@@ -245,27 +245,27 @@
             try:
                 self.skw.sksendto(self.smart_meter_addr, data)
                 xmitted = True
                 break
             except MomongaSkCommandExecutionFailure as e:
                 logger.warning('Failed to transmit a packet: %s' % str(e))
             except Exception as e:
-                logger.warning('An error occured to transmit a packet. %s: %s' % (type(e).__name__, str(e)))
+                logger.warning('An error occurred to transmit a packet. %s: %s' % (type(e).__name__, str(e)))
             finally:
                 self.xmit_lock.release()
             time.sleep(3)
         if xmitted is False:
             logger.error('Could not transmit a packet. Close Momonga and open it again.')
             raise MomongaNeedToReopen('Could not transmit a packet. Close Momonga and open it again.')
 
     def restrict_to_xmit(self) -> None:
         self.xmit_restriction_cnt += 1
         logger.debug('The counter for the restriction was incremented: %d' % (self.xmit_restriction_cnt))
 
-        assert self.xmit_restriction_cnt <= 2, 'The critical section counter for data transmition is inconsistent: The value is set too large for the counter.'
+        assert self.xmit_restriction_cnt <= 2, 'The critical section counter for data transmission is inconsistent: The value is set too large for the counter.'
 
         if self.xmit_restriction_cnt == 1:
             logger.debug('Trying to restrict data transmission.')
             self.xmit_lock.acquire()
             logger.debug('Data transmission is being restricted.')
 
     def unrestrict_to_xmit(self, force=False) -> None:
```

## momonga/momonga_sk_wrapper.py

```diff
@@ -64,15 +64,15 @@
         if self.ser is not None and not self.ser.closed:
             self.ser.close()
 
     def __clear_buf(self) -> None: # do not call this after open().
         self.ser.write(b'\r\n')
         self.ser.flush()
         timeout = self.ser.timeout
-        self.ser.timeout = 2 # will wait the specifyed seconds.
+        self.ser.timeout = 2 # will wait the specified seconds.
         while self.ser.read():
             # this loop clears garbage data if it exists.
             pass
         # to undo the timeout.
         self.ser.timeout = timeout
 
     def __exec_ropt(self) -> str: # do not call this after open().
@@ -212,17 +212,17 @@
     def skscan(self,
                retry: int = 3,
                ) -> SkScanResponse:
         duration = 6
         for _ in range(retry):
             logger.debug('Trying to scan a PAN... Duration: %d' % duration)
             res = self.exec_command(['SKSCAN', '2', 'FFFFFFFF', str(duration), '0'], 'EVENT 22')
-            # extimated execution time: 0.0096s*(2^(DURATION=6)+1)*28 = 17.5s
-            # extimated execution time: 0.0096s*(2^(DURATION=7)+1)*28 = 34.7s
-            # extimated execution time: 0.0096s*(2^(DURATION=8)+1)*28 = 69.1s
+            # estimated execution time: 0.0096s*(2^(DURATION=6)+1)*28 = 17.5s
+            # estimated execution time: 0.0096s*(2^(DURATION=7)+1)*28 = 34.7s
+            # estimated execution time: 0.0096s*(2^(DURATION=8)+1)*28 = 69.1s
             if 'EPANDESC' in res:
                 return SkScanResponse(res)
             duration += 1
         raise MomongaSkScanFailure('Could not find the specified PAN.')
 
     def skll64(self,
                mac_addr: bytes,
```

## Comparing `momonga-0.0.2.dist-info/LICENSE` & `momonga-0.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `momonga-0.0.2.dist-info/METADATA` & `momonga-0.0.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: momonga
-Version: 0.0.2
-Summary: Python Route B Library: A Comunicator for Low-voltage Smart Electric Energy Meters
+Version: 0.0.3
+Summary: Python Route B Library: A Communicator for Low-voltage Smart Electric Energy Meters
 Home-page: https://github.com/nbtk/momonga
 Author: nbtk
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyserial ~=3.5
 
 # Momonga
-Python Route B Library: A Comunicator for Low-voltage Smart Electric Energy Meters
+Python Route B Library: A Communicator for Low-voltage Smart Electric Energy Meters
 
-# Discription
+# Description
 MomongaはBルートサービスを利用してスマートメーターと通信するライブラリです。ターゲットデバイスはROHM社製Wi-SUNモジュールBP35C2を搭載したラトックシステムRS-WSUHA-Pです。
 
 # Preparation
 Momongaを使用するためには事前にWi-SUNモジュールにシリアル接続し`WOPT 01\r`コマンドを実行してUDPパケットのペイロードをASCIIフォーマットで出力するように設定してください。注意: WOPTコマンドは実行回数に制限がありますので初回のみ実行してください。設定は保存されます。
 
 # Installation
 ```shell
@@ -97,15 +97,15 @@
 
 ## momonga.MomongaSkJoinFailure
 PANAセッションを確立できなかったときに送出される。BルートIDとパスワードを確認し、再試行すること。
 
 ## momonga.MomongaNeedToReopen
 スマートメーターに対してコマンドを送信できなかったなどの理由で、スマートメーターに再接続が必要なときに送出される。
 
-## 例外を補足する例
+## 例外を捕捉する例
 ```python3
 import momonga
 import sys
 
 
 rbid = 'SET A ROUTE B ID'
 pwd  = 'SET A ROUTE B PASSWORD'
@@ -198,15 +198,16 @@
 - day: 積算履歴収集日(0:当日、1~:前日の日数)
 - reverse: Trueのとき逆方向の積算電力量を取得する
 ### Return Value
 - list: 収集日時と積算電力量(kWh)
 
 e.g.
 ```python3
-[{'timestamp': datetime.datetime, 'cumulative energy': float}]
+[{'timestamp': datetime.datetime,
+  'cumulative energy': float}]
 ```
 注意: 収集日時はスマートメーター側で設定されたものではなくMomonga自身が設定しているため、実行中に日を跨ぐと収集日時に齟齬が生じる可能性がある。
 
 ## momonga.set_day_for_which_to_retrieve_historical_data_1(day: int = 0)
 積算履歴収集日1を設定する。
 ### Arguments
 - day: 積算履歴収集日(0:当日、1~:前日の日数)
@@ -232,15 +233,16 @@
 ### Arguments
 - Void
 ### Return Value
 - dict: R相瞬時電流(A)とT相瞬時電流(A)
 
 e.g.
 ```python3
-{'r phase current': float, 't phase current': float}
+{'r phase current': float,
+ 't phase current': float}
 ```
 
 ## momonga.get_cumulative_energy_measured_at_fixed_time(reverse: bool = False)
 定時積算電力量計測値を取得する。
 ### Arguments
 - reverse: Trueのとき逆方向の積算電力量を取得する
 ### Return Value
@@ -248,15 +250,15 @@
 
 e.g.
 ```python3
 {'datetime': datetime.datetime,
  'cumulative energy': float}
 ```
 
-## momonga.get_historical_cumulative_energy_2(timestamp: datetime.datetime = datetime.datetime.now(), num_of_data_points: int = 12)
+## momonga.get_historical_cumulative_energy_2(timestamp: datetime.datetime = None, num_of_data_points: int = 12)
 積算履歴収集日時、収集コマ数ならびに積算電力量の計測結果履歴を、正・逆 30 分毎のデータで過去最大6時間分取得する。
 ### Arguments
 - timestamp: 収集日時
 - num_of_data_points: 収集コマ数 1~12
 ### Return Value
 - list: 収集日時と正方向および逆方向の積算電力量(kWh)
 
@@ -280,9 +282,10 @@
 ### Arguments
 - Void
 ### Return Value
 - dict: 収集日時と収集コマ数
 
 e.g.
 ```python3
-{'timestamp': datetime, 'number of data points': int}
+{'timestamp': datetime,
+ 'number of data points': int}
 ```
```

## Comparing `momonga-0.0.2.dist-info/RECORD` & `momonga-0.0.3.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 momonga/__init__.py,sha256=iWnaMiIWmYho2GfBZJiZ82rlo4znFfQlqNXkGwNXhLg,136
-momonga/momonga.py,sha256=VUcJlSWrgScf9JMs2rdnprc-5cc1TsCUjpszxRNplUU,15099
+momonga/momonga.py,sha256=oqerSKwFlTkgTfJYbwTsODJyz_KScZEVh32uoGbPZLs,15159
 momonga/momonga_exception.py,sha256=IPcOVNU7mpm-upYTLLo6gIxFHzjCXxs-YwzhIej8PMU,959
-momonga/momonga_response.py,sha256=ObNgkxz_HzhNQliG14775Xq-l8IEOm7jtRmn2haTzAM,2698
-momonga/momonga_session_manager.py,sha256=n27QZZHp71w-SW0kBOTyal3BFtvbqLNtdi88CNTncDU,11964
-momonga/momonga_sk_wrapper.py,sha256=U7FwKOkmaxMPEsgJ4sejL7e8yWcLxb-4G-TRL15pPXs,9392
-momonga-0.0.2.dist-info/LICENSE,sha256=pOXywwG9IIlOPHodSe52gNYGQZymYppp-BeVhAjPDME,1061
-momonga-0.0.2.dist-info/METADATA,sha256=ZcxMfRd_yQMbgFQ--Ojf9G2RRwfur8OJqWLSJ1yv9ho,10281
-momonga-0.0.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-momonga-0.0.2.dist-info/top_level.txt,sha256=wB9RSzcUXuE3oWO6vYrP1GBIbDG-FM6juEp8yztPzbM,8
-momonga-0.0.2.dist-info/RECORD,,
+momonga/momonga_response.py,sha256=_t_aaA6z5cpZVGWIkir7J_fgwYabPSNrpBAiS36Ro7c,2698
+momonga/momonga_session_manager.py,sha256=UV6BqWxuRx6D1TgKtFIpcoX7avOetVQ5J6eSpqD-t4I,11967
+momonga/momonga_sk_wrapper.py,sha256=xaffyj3D3Mt84LljroJ07j-GHJTpsXTMp695vztZbz4,9392
+momonga-0.0.3.dist-info/LICENSE,sha256=pOXywwG9IIlOPHodSe52gNYGQZymYppp-BeVhAjPDME,1061
+momonga-0.0.3.dist-info/METADATA,sha256=_TqXZksnZCvnt6WyE9hbYyjbhQjwYpJXVlzjNbRYU5M,10268
+momonga-0.0.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+momonga-0.0.3.dist-info/top_level.txt,sha256=wB9RSzcUXuE3oWO6vYrP1GBIbDG-FM6juEp8yztPzbM,8
+momonga-0.0.3.dist-info/RECORD,,
```

