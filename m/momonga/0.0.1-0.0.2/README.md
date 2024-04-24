# Comparing `tmp/momonga-0.0.1-py3-none-any.whl.zip` & `tmp/momonga-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 15120 bytes, number of entries: 11
+Zip file size: 15389 bytes, number of entries: 11
 -rw-rw-r--  2.0 unx      136 b- defN 24-Apr-20 08:49 momonga/__init__.py
--rw-rw-r--  2.0 unx    15010 b- defN 24-Apr-23 12:08 momonga/momonga.py
+-rw-rw-r--  2.0 unx    15099 b- defN 24-Apr-24 01:01 momonga/momonga.py
 -rw-rw-r--  2.0 unx      959 b- defN 24-Apr-23 04:16 momonga/momonga_exception.py
 -rw-rw-r--  2.0 unx     2698 b- defN 24-Apr-20 01:17 momonga/momonga_response.py
--rw-rw-r--  2.0 unx    11969 b- defN 24-Apr-20 07:29 momonga/momonga_session_manager.py
+-rw-rw-r--  2.0 unx    11964 b- defN 24-Apr-23 23:20 momonga/momonga_session_manager.py
 -rw-rw-r--  2.0 unx     9392 b- defN 24-Apr-20 07:30 momonga/momonga_sk_wrapper.py
--rw-rw-r--  2.0 unx     1061 b- defN 24-Apr-23 12:53 momonga-0.0.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx     9344 b- defN 24-Apr-23 12:53 momonga-0.0.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-23 12:53 momonga-0.0.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx        8 b- defN 24-Apr-23 12:53 momonga-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      882 b- defN 24-Apr-23 12:53 momonga-0.0.1.dist-info/RECORD
-11 files, 51551 bytes uncompressed, 13634 bytes compressed:  73.6%
+-rw-rw-r--  2.0 unx     1061 b- defN 24-Apr-24 01:25 momonga-0.0.2.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    10281 b- defN 24-Apr-24 01:25 momonga-0.0.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-24 01:25 momonga-0.0.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        8 b- defN 24-Apr-24 01:25 momonga-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      883 b- defN 24-Apr-24 01:25 momonga-0.0.2.dist-info/RECORD
+11 files, 52573 bytes uncompressed, 13903 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: momonga/momonga_session_manager.py
 Comment: 
 
 Filename: momonga/momonga_sk_wrapper.py
 Comment: 
 
-Filename: momonga-0.0.1.dist-info/LICENSE
+Filename: momonga-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: momonga-0.0.1.dist-info/METADATA
+Filename: momonga-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: momonga-0.0.1.dist-info/WHEEL
+Filename: momonga-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: momonga-0.0.1.dist-info/top_level.txt
+Filename: momonga-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: momonga-0.0.1.dist-info/RECORD
+Filename: momonga-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## momonga/momonga.py

```diff
@@ -177,15 +177,15 @@
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
 
@@ -301,15 +301,16 @@
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
                                            timestamp: datetime.datetime = datetime.datetime.now(),
                                            num_of_data_points: int = 12,
                                           ) -> list:
         self.__prepare_to_get_cumulative_energy()
         self.set_time_for_which_to_retrieve_historical_data_2(timestamp, num_of_data_points)
@@ -335,17 +336,17 @@
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
@@ -369,8 +370,9 @@
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

## momonga/momonga_session_manager.py

```diff
@@ -257,15 +257,15 @@
             logger.error('Could not transmit a packet. Close Momonga and open it again.')
             raise MomongaNeedToReopen('Could not transmit a packet. Close Momonga and open it again.')
 
     def restrict_to_xmit(self) -> None:
         self.xmit_restriction_cnt += 1
         logger.debug('The counter for the restriction was incremented: %d' % (self.xmit_restriction_cnt))
 
-        assert self.xmit_restriction_cnt <= 2, 'The critical section counter for data transmition is inconsistent: The counter is set to a value that is a too big.'
+        assert self.xmit_restriction_cnt <= 2, 'The critical section counter for data transmition is inconsistent: The value is set too large for the counter.'
 
         if self.xmit_restriction_cnt == 1:
             logger.debug('Trying to restrict data transmission.')
             self.xmit_lock.acquire()
             logger.debug('Data transmission is being restricted.')
 
     def unrestrict_to_xmit(self, force=False) -> None:
```

## Comparing `momonga-0.0.1.dist-info/LICENSE` & `momonga-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `momonga-0.0.1.dist-info/METADATA` & `momonga-0.0.2.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,60 +1,73 @@
 Metadata-Version: 2.1
 Name: momonga
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python Route B Library: A Comunicator for Low-voltage Smart Electric Energy Meters
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
 Python Route B Library: A Comunicator for Low-voltage Smart Electric Energy Meters
+
 # Discription
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
@@ -68,181 +81,206 @@
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
+
 ## 例外を補足する例
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
 [{'timestamp': datetime.datetime, 'cumulative energy': float}]
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
 {'r phase current': float, 't phase current': float}
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
+## momonga.get_historical_cumulative_energy_2(timestamp: datetime.datetime = datetime.datetime.now(), num_of_data_points: int = 12)
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
```

## Comparing `momonga-0.0.1.dist-info/RECORD` & `momonga-0.0.2.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 momonga/__init__.py,sha256=iWnaMiIWmYho2GfBZJiZ82rlo4znFfQlqNXkGwNXhLg,136
-momonga/momonga.py,sha256=f2nqCHhWOhFNq5Er0JVKRrNsjKsH3BRmLZZI7ZNyFtY,15010
+momonga/momonga.py,sha256=VUcJlSWrgScf9JMs2rdnprc-5cc1TsCUjpszxRNplUU,15099
 momonga/momonga_exception.py,sha256=IPcOVNU7mpm-upYTLLo6gIxFHzjCXxs-YwzhIej8PMU,959
 momonga/momonga_response.py,sha256=ObNgkxz_HzhNQliG14775Xq-l8IEOm7jtRmn2haTzAM,2698
-momonga/momonga_session_manager.py,sha256=kwx5gSuUAbN4WGJ1s28zp34cIxQSvrg-kNJhz8o-e2s,11969
+momonga/momonga_session_manager.py,sha256=n27QZZHp71w-SW0kBOTyal3BFtvbqLNtdi88CNTncDU,11964
 momonga/momonga_sk_wrapper.py,sha256=U7FwKOkmaxMPEsgJ4sejL7e8yWcLxb-4G-TRL15pPXs,9392
-momonga-0.0.1.dist-info/LICENSE,sha256=pOXywwG9IIlOPHodSe52gNYGQZymYppp-BeVhAjPDME,1061
-momonga-0.0.1.dist-info/METADATA,sha256=TMvPKTGkYRlJ1E6BFavqGFeJ1Slh5ewNdgMBX-wZTQM,9344
-momonga-0.0.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-momonga-0.0.1.dist-info/top_level.txt,sha256=wB9RSzcUXuE3oWO6vYrP1GBIbDG-FM6juEp8yztPzbM,8
-momonga-0.0.1.dist-info/RECORD,,
+momonga-0.0.2.dist-info/LICENSE,sha256=pOXywwG9IIlOPHodSe52gNYGQZymYppp-BeVhAjPDME,1061
+momonga-0.0.2.dist-info/METADATA,sha256=ZcxMfRd_yQMbgFQ--Ojf9G2RRwfur8OJqWLSJ1yv9ho,10281
+momonga-0.0.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+momonga-0.0.2.dist-info/top_level.txt,sha256=wB9RSzcUXuE3oWO6vYrP1GBIbDG-FM6juEp8yztPzbM,8
+momonga-0.0.2.dist-info/RECORD,,
```

