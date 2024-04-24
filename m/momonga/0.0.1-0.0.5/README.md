# Comparing `tmp/momonga-0.0.1-py3-none-any.whl.zip` & `tmp/momonga-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 15120 bytes, number of entries: 11
+Zip file size: 15388 bytes, number of entries: 11
 -rw-rw-r--  2.0 unx      136 b- defN 24-Apr-20 08:49 momonga/__init__.py
--rw-rw-r--  2.0 unx    15010 b- defN 24-Apr-23 12:08 momonga/momonga.py
+-rw-rw-r--  2.0 unx    15159 b- defN 24-Apr-24 10:04 momonga/momonga.py
 -rw-rw-r--  2.0 unx      959 b- defN 24-Apr-23 04:16 momonga/momonga_exception.py
--rw-rw-r--  2.0 unx     2698 b- defN 24-Apr-20 01:17 momonga/momonga_response.py
--rw-rw-r--  2.0 unx    11969 b- defN 24-Apr-20 07:29 momonga/momonga_session_manager.py
--rw-rw-r--  2.0 unx     9392 b- defN 24-Apr-20 07:30 momonga/momonga_sk_wrapper.py
--rw-rw-r--  2.0 unx     1061 b- defN 24-Apr-23 12:53 momonga-0.0.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx     9344 b- defN 24-Apr-23 12:53 momonga-0.0.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-23 12:53 momonga-0.0.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx        8 b- defN 24-Apr-23 12:53 momonga-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      882 b- defN 24-Apr-23 12:53 momonga-0.0.1.dist-info/RECORD
-11 files, 51551 bytes uncompressed, 13634 bytes compressed:  73.6%
+-rw-rw-r--  2.0 unx     2698 b- defN 24-Apr-24 09:24 momonga/momonga_response.py
+-rw-rw-r--  2.0 unx    11967 b- defN 24-Apr-24 09:20 momonga/momonga_session_manager.py
+-rw-rw-r--  2.0 unx     9392 b- defN 24-Apr-24 09:23 momonga/momonga_sk_wrapper.py
+-rw-rw-r--  2.0 unx     1061 b- defN 24-Apr-24 10:26 momonga-0.0.5.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    10268 b- defN 24-Apr-24 10:26 momonga-0.0.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-24 10:26 momonga-0.0.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        8 b- defN 24-Apr-24 10:26 momonga-0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      883 b- defN 24-Apr-24 10:26 momonga-0.0.5.dist-info/RECORD
+11 files, 52623 bytes uncompressed, 13902 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: momonga/momonga_session_manager.py
 Comment: 
 
 Filename: momonga/momonga_sk_wrapper.py
 Comment: 
 
-Filename: momonga-0.0.1.dist-info/LICENSE
+Filename: momonga-0.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: momonga-0.0.1.dist-info/METADATA
+Filename: momonga-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: momonga-0.0.1.dist-info/WHEEL
+Filename: momonga-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: momonga-0.0.1.dist-info/top_level.txt
+Filename: momonga-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: momonga-0.0.1.dist-info/RECORD
+Filename: momonga-0.0.5.dist-info/RECORD
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
@@ -127,65 +127,65 @@
 
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
         if self.energy_unit is None:
             self.energy_unit = self.get_unit_for_cumulative_energy()
 
     def get_operation_status(self) -> int:
         res = self.__request(0x80)
         status = int.from_bytes(res.get('edt'), 'big')
-        if status == 0x30: # turned on
+        if status == 0x30:   # turned on
             status = True
         elif status == 0x31: # turned off
             status = False
         else:
             status = None
         return status
 
@@ -301,20 +301,24 @@
         res = self.__request(epc)
         edt = res.get('edt')
         timestamp = datetime.datetime(int.from_bytes(edt[0:2], 'big'),
                                       edt[2], edt[3], edt[4], edt[5], edt[6])
         cumulative_energy = int.from_bytes(edt[7:], 'big')
         cumulative_energy *= self.energy_coefficient
         cumulative_energy *= self.energy_unit 
-        return {timestamp: cumulative_energy}
+        return {'timestamp': timestamp,
+                'cumulative_energy': cumulative_energy}
 
     def get_historical_cumulative_energy_2(self,
-                                           timestamp: datetime.datetime = datetime.datetime.now(),
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
@@ -335,17 +339,17 @@
             if reverse_direction_energy == 0xFFFFFFFE:
                 reverse_direction_energy = None
             else:
                 reverse_direction_energy *= self.energy_coefficient
                 reverse_direction_energy *= self.energy_unit 
 
             historical_cumulative_energy.append(
-                {'timestamp': timestamp, 'cumulative energy': {
-                 'normal direction': normal_direction_energy,
-                 'reverse direction': reverse_direction_energy}})
+                {'timestamp': timestamp,
+                 'cumulative energy': {'normal direction': normal_direction_energy,
+                                       'reverse direction': reverse_direction_energy}})
             timestamp -= datetime.timedelta(minutes=30)
         return historical_cumulative_energy
  
     def set_time_for_which_to_retrieve_historical_data_2(self,
                                                          timestamp: datetime.datetime,
                                                          num_of_data_points: int = 12,
                                                         ) -> None:
@@ -369,8 +373,9 @@
         year = int.from_bytes(edt[0:2], 'big')
         if year == 0xFFFF:
             timestamp = None
         else:
             timestamp = datetime.datetime(year, edt[2], edt[3], edt[4], edt[5])
 
         num_of_data_points = edt[6]
-        return {'timestamp': timestamp, 'number of data points': num_of_data_points}
+        return {'timestamp': timestamp,
+                'number of data points': num_of_data_points}
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
 
-        assert self.xmit_restriction_cnt <= 2, 'The critical section counter for data transmition is inconsistent: The counter is set to a value that is a too big.'
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

## Comparing `momonga-0.0.1.dist-info/LICENSE` & `momonga-0.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `momonga-0.0.1.dist-info/METADATA` & `momonga-0.0.5.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,60 +1,73 @@
 Metadata-Version: 2.1
 Name: momonga
-Version: 0.0.1
-Summary: Python Route B Library: A Comunicator for Low-voltage Smart Electric Energy Meters
+Version: 0.0.5
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
-# Discription
+Python Route B Library: A Communicator for Low-voltage Smart Electric Energy Meters
+
+# Description
 MomongaはBルートサービスを利用してスマートメーターと通信するライブラリです。ターゲットデバイスはROHM社製Wi-SUNモジュールBP35C2を搭載したラトックシステムRS-WSUHA-Pです。
+
+# Preparation
+Momongaを使用するためには事前にWi-SUNモジュールにシリアル接続し`WOPT 01\r`コマンドを実行してUDPパケットのペイロードをASCIIフォーマットで出力するように設定してください。注意: WOPTコマンドは実行回数に制限がありますので初回のみ実行してください。設定は保存されます。
+
 # Installation
 ```shell
 $ pip install momonga
 ```
+
 # Simple Example
 下記のコードはPANAセッションを確立し、瞬時電力計測値を取得して表示します。PANのスキャンは最大で約２分、セッション確立は最大で約１分かかります。
 BルートID、パスワード、デバイスファイルへのパスは適宜変更してください。
 ```python3
 import momonga
 
 
 rbid = 'SET A ROUTE B ID'
 pwd  = 'SET A ROUTE B PASSWORD'
 dev  = '/dev/ttyUSB0' # in a case of RaspberryPi OS
 
 with momonga.Momonga(rbid, pwd, dev) as mo:
-    res = mo.get_instantaneous_power()
+    res = momonga.get_instantaneous_power()
     print('%0.1fW' % res)
 ```
+
 ### Arguments
 - rbid: BルートID
 - pwd: Bルートパスワード
 - dev: Wi-SUNモジュールのデバイスファイルへのパス
-- baudrate: シリアル通信のボーレート(デフォルトは11520)
+- baudrate: シリアル通信のボーレート(デフォルト: 11520)
+
 ### Return Value
 - mo: Momongaクラスのインスタンス
+
 # Logging
 Momongaには下記のロガーがあります。
+
 ## momonga.logger
-ECHONET Lite スマートメータークラスを抽象化したレイヤのログ
+ECHONET Liteスマートメータークラスを抽象化したレイヤのログ
+
 ## momonga.session_manager_logger
 PANAセッション管理レイヤのログ
+
 ## momonga.sk_wrapper_logger
 Wi-SUNモジュールとの通信ログ
+
 ## ログを有効にした例
 ```python3
 import momonga
 import logging
 
 
 log_fmt = logging.Formatter('%(asctime)s | %(levelname)s | %(name)s - %(message)s')
@@ -68,183 +81,211 @@
 momonga.sk_wrapper_logger.setLevel(logging.DEBUG)
 
 rbid = 'SET A ROUTE B ID'
 pwd  = 'SET A ROUTE B PASSWORD'
 dev  = '/dev/ttyUSB0' # in a case of RaspberryPi OS
 
 with momonga.Momonga(rbid, pwd, dev) as mo:
-    res = mo.get_instantaneous_power()
+    res = momonga.get_instantaneous_power()
     print('%0.1fW' % res)
 ```
-# Exceptions
+
+# Exception
 主な例外は下記です。
+
 ## momonga.MomongaSkScanFailure
 PANをスキャンしたが見つからなかったときに送出される。スマートメーターと通信できるロケーションか、またBルートIDが正しく設定されているかを確認し、再試行すること。
+
 ## momonga.MomongaSkJoinFailure
 PANAセッションを確立できなかったときに送出される。BルートIDとパスワードを確認し、再試行すること。
+
 ## momonga.MomongaNeedToReopen
 スマートメーターに対してコマンドを送信できなかったなどの理由で、スマートメーターに再接続が必要なときに送出される。
-## 例外を補足する例
+
+## 例外を捕捉する例
 ```python3
 import momonga
 import sys
 
 
 rbid = 'SET A ROUTE B ID'
 pwd  = 'SET A ROUTE B PASSWORD'
 dev  = '/dev/ttyUSB0' # in a case of RaspberryPi OS
 
 while True:
     try:
         with momonga.Momonga(rbid, pwd, dev) as mo:
-            res = mo.get_instantaneous_power()
+            res = momonga.get_instantaneous_power()
             print('%0.1fW' % res)
             break
     except (momonga.MomongaSkScanFailure,
             momonga.MomongaSkJoinFailure,
             momonga.MomongaNeedToReopen) as e:
         print('%s: %s' % (type(e).__name__, e), file=sys.stderr)
         continue
 ```
+
 # Transmission Restriction
 下記のイベントが発生したときMomongaはスマートメーターに対するコマンドの送信をブロッキングします。
-1. PANAセッションのライフタイムが近づきWi-SUNモジュールが再認証を試みているとき
-2. 送信データ量が規定値に達しWi-SUNモジュールが制限したとき
-3. シリアルデバイスとの通信がブロッキングされたとき
+1. PANAセッションのライフタイムが近づきWi-SUNモジュールが自動再認証を試みているとき
+2. 送信データ量が規定値に達しWi-SUNモジュールが送信制限しているとき
+3. 何らかの理由でシリアルデバイスとの通信がブロッキングされたとき
+
+したがって開発者はデータ設定または取得関数を呼び出したあと即座に応答が返ってこない可能性を考慮してください。
 
-したがって開発者はデータ取得関数を呼び出して、即座に応答が返ってこない可能性を考慮してください。
 # Consideration
-送信がブロッキングされるなど諸条件により関数呼び出しのあと応答が即座に返らないことがあるため、`mo.get_historical_cumulative_energy_1()`は呼び出したときに期待した履歴の日付と結果の日付に齟齬が生じる可能性があることに注意してください。特にこの関数は日を跨ぐタイミングで実行すべきではありません。
+- 送信がブロッキングされるなど諸条件により関数呼び出しのあと応答が即座に返らないことがあるため、`momonga.get_historical_cumulative_energy_1()`は呼び出したときに期待した履歴の日付と結果の日付に齟齬が生じる可能性があることに注意してください。特にこの関数は日を跨ぐタイミングで実行すべきではありません。
+
 # API
 ## momonga.Momonga(rbid: str, pwd: str, dev: str, baudrate: int = 115200, reset_dev: bool = True)
 Momongaクラスのインスタンス化。
 ### Arguments
 - rbid: BルートID
 - pwd: Bルートパスワード
 - dev: デバイスファイルへのパス
 - baudrate: シリアル通信のボーレート
-- reset_dev: mo.open()を実行するときSKRESETコマンドを実行するかどうか
-## mo.open()
+- reset_dev: momonga.open()を実行するときSKRESETコマンドを実行するかどうか
+
+## momonga.open()
 PANをスキャンし、PANAセッションの確立を行う。　
 ### Arguments
 - Void
 ### Return Value
 - None
-## mo.close()
+
+## momonga.close()
 PANAセッションを終了する。
 ### Arguments
 - Void
 ### Return Value
 - None
-## mo.get_operation_status()
+
+## momonga.get_operation_status()
 スマートメーターの状態を取得する。
 ### Arguments
 - Void
 ### Return Value
 - bool: スマートメーターの状態 (True: オン False: オフ None: 不明)
-## mo.get_coefficient_for_cumulative_energy()
+
+## momonga.get_coefficient_for_cumulative_energy()
 積算電力量計測値、履歴を実使用量に換算する係数を取得する。Momongaが出力する結果には適宜この値が乗じられている。
 ### Arguments
 - Void
 ### Return Value
-- Int: 係数
-## mo.get_number_of_effective_digits_for_cumulative_energy()
+- int: 係数
+
+## momonga.get_number_of_effective_digits_for_cumulative_energy()
 積算電力量計測値の有効桁数を取得する。
 - Void
 ### Return Value
-- Int: 有効桁数
-## mo.get_measured_cumulative_energy(reverse: bool = False)
+- int: 有効桁数
+## momonga.get_measured_cumulative_energy(reverse: bool = False)
 積算電力量計測値を取得する。
 ### Arguments
 - reverse: Trueのとき逆方向の積算電力量を取得する
 ### Return Value
 - float: 積算電力量(kWh)
-## mo.get_unit_for_cumulative_energy()
+
+## momonga.get_unit_for_cumulative_energy()
 積算電力量計測値、履歴の乗率を取得する。Momongaが出力する結果には適宜この値が乗じられている。
 ### Arguments
 - Void
 ### Return Value
 - int | float: 積算電力量の乗率
-## mo.get_historical_cumulative_energy_1(day: int = 0, reverse: bool = False)
+
+## momonga.get_historical_cumulative_energy_1(day: int = 0, reverse: bool = False)
 積算電力量計測値履歴1を取得する。
 ### Arguments
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
-Note: 収集日時はスマートメーター側で設定されたものではなくMomonga自身が設定しているため、実行中に日を跨ぐと収集日時に齟齬が生じる可能性がある。
-## mo.set_day_for_which_to_retrieve_historical_data_1(day: int = 0)
+注意: 収集日時はスマートメーター側で設定されたものではなくMomonga自身が設定しているため、実行中に日を跨ぐと収集日時に齟齬が生じる可能性がある。
+
+## momonga.set_day_for_which_to_retrieve_historical_data_1(day: int = 0)
 積算履歴収集日1を設定する。
 ### Arguments
-- day: 積算履歴収集日 0:当日、1~:前日の日数
+- day: 積算履歴収集日(0:当日、1~:前日の日数)
 ### Return Value
 - None
-## mo.get_day_for_which_to_retrieve_historical_data_1()
+
+## momonga.get_day_for_which_to_retrieve_historical_data_1()
 積算履歴収集日1を設定する。
 ### Arguments
 - Void
 ### Return Value
 - int: 積算履歴収集日1
-## mo.get_instantaneous_power()
+
+## momonga.get_instantaneous_power()
 瞬時電力計測値を取得する。
 ### Arguments
 - Void
 ### Return Value
 - float: 瞬時電力測定値(W)
-## mo.get_instantaneous_current()
+
+## momonga.get_instantaneous_current()
 瞬時電流計測値を取得する。
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
-## mo.get_cumulative_energy_measured_at_fixed_time(reverse: bool = False)
+
+## momonga.get_cumulative_energy_measured_at_fixed_time(reverse: bool = False)
 定時積算電力量計測値を取得する。
 ### Arguments
 - reverse: Trueのとき逆方向の積算電力量を取得する
 ### Return Value
 - dict: 収集日時と積算電力量(kWh)
 
 e.g.
 ```python3
-{datetime: float}
+{'datetime': datetime.datetime,
+ 'cumulative energy': float}
 ```
-## mo.get_historical_cumulative_energy_2(timestamp: datetime.datetime = datetime.datetime.now(), num_of_data_points: int = 12)
-### Arguments
-timestamp: 収集日時
-num_of_data_points: 収集コマ数 1~12
+
+## momonga.get_historical_cumulative_energy_2(timestamp: datetime.datetime = None, num_of_data_points: int = 12)
+積算履歴収集日時、収集コマ数ならびに積算電力量の計測結果履歴を、正・逆 30 分毎のデータで過去最大6時間分取得する。
 ### Arguments
-- Void
+- timestamp: 収集日時
+- num_of_data_points: 収集コマ数 1~12
 ### Return Value
 - list: 収集日時と正方向および逆方向の積算電力量(kWh)
+
 e.g.
 ```python3
 [{'timestamp': datetime.datetime,
-  'cumulative energy': {
-    'normal direction': float,
-    'reverse direction': float}}]
+  'cumulative energy': {'normal direction': float,
+                        'reverse direction': float}}]
 ```
-## mo.set_time_for_which_to_retrieve_historical_data_2(timestamp: datetime.datetime, num_of_data_points: int = 12)
+
+## momonga.set_time_for_which_to_retrieve_historical_data_2(timestamp: datetime.datetime, num_of_data_points: int = 12)
+積算履歴収集日時ならびに収集コマ数を設定する。
 ### Arguments
 - timestamp: 収集日時
 - num_of_data_points: 収集コマ数
 ### Return Value
 - None
-## mo.get_time_for_which_to_retrieve_historical_data_2()
+
+## momonga.get_time_for_which_to_retrieve_historical_data_2()
+積算履歴収集日時ならびに収集コマ数を取得する。
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

## Comparing `momonga-0.0.1.dist-info/RECORD` & `momonga-0.0.5.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 momonga/__init__.py,sha256=iWnaMiIWmYho2GfBZJiZ82rlo4znFfQlqNXkGwNXhLg,136
-momonga/momonga.py,sha256=f2nqCHhWOhFNq5Er0JVKRrNsjKsH3BRmLZZI7ZNyFtY,15010
+momonga/momonga.py,sha256=rufLe-sknKiyg4apyaifir_uEvQavcMDYjxUGSRxZzc,15159
 momonga/momonga_exception.py,sha256=IPcOVNU7mpm-upYTLLo6gIxFHzjCXxs-YwzhIej8PMU,959
-momonga/momonga_response.py,sha256=ObNgkxz_HzhNQliG14775Xq-l8IEOm7jtRmn2haTzAM,2698
-momonga/momonga_session_manager.py,sha256=kwx5gSuUAbN4WGJ1s28zp34cIxQSvrg-kNJhz8o-e2s,11969
-momonga/momonga_sk_wrapper.py,sha256=U7FwKOkmaxMPEsgJ4sejL7e8yWcLxb-4G-TRL15pPXs,9392
-momonga-0.0.1.dist-info/LICENSE,sha256=pOXywwG9IIlOPHodSe52gNYGQZymYppp-BeVhAjPDME,1061
-momonga-0.0.1.dist-info/METADATA,sha256=TMvPKTGkYRlJ1E6BFavqGFeJ1Slh5ewNdgMBX-wZTQM,9344
-momonga-0.0.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-momonga-0.0.1.dist-info/top_level.txt,sha256=wB9RSzcUXuE3oWO6vYrP1GBIbDG-FM6juEp8yztPzbM,8
-momonga-0.0.1.dist-info/RECORD,,
+momonga/momonga_response.py,sha256=_t_aaA6z5cpZVGWIkir7J_fgwYabPSNrpBAiS36Ro7c,2698
+momonga/momonga_session_manager.py,sha256=UV6BqWxuRx6D1TgKtFIpcoX7avOetVQ5J6eSpqD-t4I,11967
+momonga/momonga_sk_wrapper.py,sha256=xaffyj3D3Mt84LljroJ07j-GHJTpsXTMp695vztZbz4,9392
+momonga-0.0.5.dist-info/LICENSE,sha256=pOXywwG9IIlOPHodSe52gNYGQZymYppp-BeVhAjPDME,1061
+momonga-0.0.5.dist-info/METADATA,sha256=X_TKp-K1MUYpCxy00Gb9Cv5_qKoUMwxwd5m08D0e3ZU,10268
+momonga-0.0.5.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+momonga-0.0.5.dist-info/top_level.txt,sha256=wB9RSzcUXuE3oWO6vYrP1GBIbDG-FM6juEp8yztPzbM,8
+momonga-0.0.5.dist-info/RECORD,,
```

