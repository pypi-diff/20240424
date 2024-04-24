# Comparing `tmp/gattlib-py-0.7.1.tar.gz` & `tmp/gattlib-py-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gattlib-py-0.7.1.tar", last modified: Thu Apr 11 20:39:07 2024, max compression
+gzip compressed data, was "gattlib-py-0.7.2.tar", last modified: Wed Apr 24 12:56:08 2024, max compression
```

## Comparing `gattlib-py-0.7.1.tar` & `gattlib-py-0.7.2.tar`

### file list

```diff
@@ -1,209 +1,210 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.211399 gattlib-py-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/CrossCompilation.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-11 20:39:07.211399 gattlib-py-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.187399 gattlib-py-0.7.1/bluez/
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.183399 gattlib-py-0.7.1/bluez/bluez4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.191399 gattlib-py-0.7.1/bluez/bluez4/attrib/
--rw-r--r--   0 runner    (1001) docker     (127)    18727 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez4/attrib/att.c
--rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez4/attrib/att.h
--rw-r--r--   0 runner    (1001) docker     (127)    14820 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez4/attrib/gatt.c
--rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez4/attrib/gatt.h
--rw-r--r--   0 runner    (1001) docker     (127)    14131 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez4/attrib/gattrib.c
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez4/attrib/gattrib.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.191399 gattlib-py-0.7.1/bluez/bluez4/btio/
--rw-r--r--   0 runner    (1001) docker     (127)    29676 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez4/btio/btio.c
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez4/btio/btio.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.191399 gattlib-py-0.7.1/bluez/bluez4/lib/
--rw-r--r--   0 runner    (1001) docker     (127)    10884 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez4/lib/bluetooth.c
--rw-r--r--   0 runner    (1001) docker     (127)     7574 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez4/lib/bluetooth.h
--rw-r--r--   0 runner    (1001) docker     (127)    61436 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez4/lib/hci.c
--rw-r--r--   0 runner    (1001) docker     (127)    61945 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez4/lib/hci.h
--rw-r--r--   0 runner    (1001) docker     (127)     9916 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez4/lib/hci_lib.h
--rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez4/lib/l2cap.h
--rw-r--r--   0 runner    (1001) docker     (127)   113715 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez4/lib/sdp.c
--rw-r--r--   0 runner    (1001) docker     (127)    17273 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez4/lib/sdp.h
--rw-r--r--   0 runner    (1001) docker     (127)    21697 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez4/lib/sdp_lib.h
--rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez4/lib/uuid.c
--rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez4/lib/uuid.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.191399 gattlib-py-0.7.1/bluez/bluez4/src/
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez4/src/log.c
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez4/src/log.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.187399 gattlib-py-0.7.1/bluez/bluez5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.191399 gattlib-py-0.7.1/bluez/bluez5/attrib/
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/attrib/att-database.h
--rw-r--r--   0 runner    (1001) docker     (127)    24811 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/attrib/att.c
--rw-r--r--   0 runner    (1001) docker     (127)     8198 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/attrib/att.h
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/attrib/gatt-service.h
--rw-r--r--   0 runner    (1001) docker     (127)    27805 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/attrib/gatt.c
--rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/attrib/gatt.h
--rw-r--r--   0 runner    (1001) docker     (127)    10254 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/attrib/gattrib.c
--rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/attrib/gattrib.h
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/attrib/gatttool.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.191399 gattlib-py-0.7.1/bluez/bluez5/btio/
--rw-r--r--   0 runner    (1001) docker     (127)    37670 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/btio/btio.c
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/btio/btio.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.195399 gattlib-py-0.7.1/bluez/bluez5/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/lib/a2mp.h
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/lib/amp.h
--rw-r--r--   0 runner    (1001) docker     (127)    49250 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/lib/bluetooth.c
--rw-r--r--   0 runner    (1001) docker     (127)     9415 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/lib/bluetooth.h
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/lib/bluez.pc
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/lib/bluez.pc.in
--rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/lib/bnep.h
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/lib/cmtp.h
--rw-r--r--   0 runner    (1001) docker     (127)    65395 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/lib/hci.c
--rw-r--r--   0 runner    (1001) docker     (127)    63804 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/lib/hci.h
--rw-r--r--   0 runner    (1001) docker     (127)    10494 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/lib/hci_lib.h
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/lib/hidp.h
--rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/lib/l2cap.h
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/lib/libbluetooth-internal.la
--rw-r--r--   0 runner    (1001) docker     (127)    21400 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/lib/mgmt.h
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/lib/rfcomm.h
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/lib/sco.h
--rw-r--r--   0 runner    (1001) docker     (127)   115468 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/lib/sdp.c
--rw-r--r--   0 runner    (1001) docker     (127)    18250 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/lib/sdp.h
--rw-r--r--   0 runner    (1001) docker     (127)    21725 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/lib/sdp_lib.h
--rw-r--r--   0 runner    (1001) docker     (127)     6893 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/lib/uuid.c
--rw-r--r--   0 runner    (1001) docker     (127)     6757 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/lib/uuid.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.195399 gattlib-py-0.7.1/bluez/bluez5/monitor/
--rw-r--r--   0 runner    (1001) docker     (127)    78785 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/monitor/bt.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.187399 gattlib-py-0.7.1/bluez/bluez5/profiles/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.195399 gattlib-py-0.7.1/bluez/bluez5/profiles/input/
--rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/profiles/input/uhid_copy.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.195399 gattlib-py-0.7.1/bluez/bluez5/src/
--rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/eir.h
--rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/log.c
--rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/log.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.203399 gattlib-py-0.7.1/bluez/bluez5/src/shared/
--rw-r--r--   0 runner    (1001) docker     (127)    13253 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/ad.c
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/ad.h
--rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/att-types.h
--rw-r--r--   0 runner    (1001) docker     (127)    33357 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/att.c
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/att.h
--rw-r--r--   0 runner    (1001) docker     (127)    10430 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/btsnoop.c
--rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/btsnoop.h
--rw-r--r--   0 runner    (1001) docker     (127)    15523 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/crypto.c
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/crypto.h
--rw-r--r--   0 runner    (1001) docker     (127)    21679 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/ecc.c
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/ecc.h
--rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/gap.c
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/gap.h
--rw-r--r--   0 runner    (1001) docker     (127)    73336 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/gatt-client.c
--rw-r--r--   0 runner    (1001) docker     (127)     5472 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/gatt-client.h
--rw-r--r--   0 runner    (1001) docker     (127)    39496 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/gatt-db.c
--rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/gatt-db.h
--rw-r--r--   0 runner    (1001) docker     (127)    33891 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/gatt-helpers.c
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/gatt-helpers.h
--rw-r--r--   0 runner    (1001) docker     (127)    37513 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/gatt-server.c
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/gatt-server.h
--rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/hci-crypto.c
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/hci-crypto.h
--rw-r--r--   0 runner    (1001) docker     (127)    10786 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/hci.c
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/hci.h
--rw-r--r--   0 runner    (1001) docker     (127)    29458 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/hfp.c
--rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/hfp.h
--rw-r--r--   0 runner    (1001) docker     (127)     5790 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/io-glib.c
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/io.h
--rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/mainloop.c
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/mainloop.h
--rw-r--r--   0 runner    (1001) docker     (127)    16958 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/mgmt.c
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/mgmt.h
--rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/pcap.c
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/pcap.h
--rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/queue.c
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/queue.h
--rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/ringbuf.c
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/ringbuf.h
--rw-r--r--   0 runner    (1001) docker     (127)    16939 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/tester.c
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/tester.h
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/timeout-glib.c
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/timeout-mainloop.c
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/timeout.h
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/tty.h
--rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/uhid.c
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/uhid.h
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/util.c
--rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/bluez5/src/shared/util.h
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/gattlib.pc.in
--rw-r--r--   0 runner    (1001) docker     (127)     6951 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/gattlib_adapter.c
--rw-r--r--   0 runner    (1001) docker     (127)    16490 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/gattlib_connect.c
--rw-r--r--   0 runner    (1001) docker     (127)    10517 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/gattlib_discover.c
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/gattlib_internal.h
--rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/bluez/gattlib_read_write.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.203399 gattlib-py-0.7.1/common/
--rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/common/gattlib_callback_connected_device.c
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/common/gattlib_callback_disconnected_device.c
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/common/gattlib_callback_discovered_device.c
--rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/common/gattlib_callback_notification_device.c
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/common/gattlib_callback_python.c
--rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/common/gattlib_common.c
--rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/common/gattlib_common_adapter.c
--rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/common/gattlib_device_state_management.c
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/common/gattlib_eddystone.c
--rw-r--r--   0 runner    (1001) docker     (127)     6334 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/common/gattlib_internal.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.187399 gattlib-py-0.7.1/common/logging_backend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.203399 gattlib-py-0.7.1/common/logging_backend/printf/
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/common/logging_backend/printf/gattlib_logging.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.203399 gattlib-py-0.7.1/common/logging_backend/python/
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/common/logging_backend/python/gattlib_logging.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.203399 gattlib-py-0.7.1/common/logging_backend/syslog/
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/common/logging_backend/syslog/gattlib_logging.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.203399 gattlib-py-0.7.1/common/mainloop/
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/common/mainloop/gattlib_glib_mainloop.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.207399 gattlib-py-0.7.1/dbus/
--rw-r--r--   0 runner    (1001) docker     (127)     7092 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.187399 gattlib-py-0.7.1/dbus/bluez5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.207399 gattlib-py-0.7.1/dbus/bluez5/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     6899 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/bluez5/lib/uuid.c
--rw-r--r--   0 runner    (1001) docker     (127)     6757 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/bluez5/lib/uuid.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.207399 gattlib-py-0.7.1/dbus/dbus-bluez-pre-v5.40/
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/dbus-bluez-pre-v5.40/org.bluez.Adapter1.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/dbus-bluez-pre-v5.40/org.bluez.Device1.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/dbus-bluez-pre-v5.40/org.bluez.GattCharacteristic1.xml
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/dbus-bluez-pre-v5.40/org.bluez.GattDescriptor1.xml
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/dbus-bluez-pre-v5.40/org.bluez.GattService1.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.207399 gattlib-py-0.7.1/dbus/dbus-bluez-v5.40/
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/dbus-bluez-v5.40/org.bluez.Adapter1.xml
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/dbus-bluez-v5.40/org.bluez.Battery1.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/dbus-bluez-v5.40/org.bluez.Device1.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/dbus-bluez-v5.40/org.bluez.GattCharacteristic1.xml
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/dbus-bluez-v5.40/org.bluez.GattDescriptor1.xml
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/dbus-bluez-v5.40/org.bluez.GattService1.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.207399 gattlib-py-0.7.1/dbus/dbus-bluez-v5.48/
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/dbus-bluez-v5.48/org.bluez.Adapter1.xml
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/dbus-bluez-v5.48/org.bluez.Battery1.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/dbus-bluez-v5.48/org.bluez.Device1.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/dbus-bluez-v5.48/org.bluez.GattCharacteristic1.xml
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/dbus-bluez-v5.48/org.bluez.GattDescriptor1.xml
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/dbus-bluez-v5.48/org.bluez.GattService1.xml
--rw-r--r--   0 runner    (1001) docker     (127)    38771 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/gattlib.c
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/gattlib.pc.in
--rw-r--r--   0 runner    (1001) docker     (127)    25348 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/gattlib_adapter.c
--rw-r--r--   0 runner    (1001) docker     (127)     5799 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/gattlib_advertisement.c
--rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/gattlib_backend.h
--rw-r--r--   0 runner    (1001) docker     (127)    16209 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/gattlib_char.c
--rw-r--r--   0 runner    (1001) docker     (127)     9844 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/gattlib_notification.c
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/dbus/gattlib_stream.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.211399 gattlib-py-0.7.1/gattlib/
--rw-r--r--   0 runner    (1001) docker     (127)    11285 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/gattlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-11 20:39:07.000000 gattlib-py-0.7.1/gattlib/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    10827 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/gattlib/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    11159 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/gattlib/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/gattlib/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/gattlib/gatt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/gattlib/mainloop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/gattlib/uuid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.211399 gattlib-py-0.7.1/gattlib_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-11 20:39:07.000000 gattlib-py-0.7.1/gattlib_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-11 20:39:07.000000 gattlib-py-0.7.1/gattlib_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 20:39:07.000000 gattlib-py-0.7.1/gattlib_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-11 20:39:07.000000 gattlib-py-0.7.1/gattlib_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 20:39:07.000000 gattlib-py-0.7.1/gattlib_py.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:39:07.211399 gattlib-py-0.7.1/include/
--rw-r--r--   0 runner    (1001) docker     (127)    30854 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/include/gattlib.h
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 20:39:07.211399 gattlib-py-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     7503 2024-04-11 20:21:23.000000 gattlib-py-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:56:08.134700 gattlib-py-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     5953 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/CrossCompilation.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-24 12:56:08.134700 gattlib-py-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:56:08.110700 gattlib-py-0.7.2/bluez/
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:56:08.106700 gattlib-py-0.7.2/bluez/bluez4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:56:08.110700 gattlib-py-0.7.2/bluez/bluez4/attrib/
+-rw-r--r--   0 runner    (1001) docker     (127)    18727 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez4/attrib/att.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez4/attrib/att.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14820 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez4/attrib/gatt.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez4/attrib/gatt.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14131 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez4/attrib/gattrib.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez4/attrib/gattrib.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:56:08.110700 gattlib-py-0.7.2/bluez/bluez4/btio/
+-rw-r--r--   0 runner    (1001) docker     (127)    29676 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez4/btio/btio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez4/btio/btio.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:56:08.114700 gattlib-py-0.7.2/bluez/bluez4/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)    10884 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez4/lib/bluetooth.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7574 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez4/lib/bluetooth.h
+-rw-r--r--   0 runner    (1001) docker     (127)    61436 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez4/lib/hci.c
+-rw-r--r--   0 runner    (1001) docker     (127)    61945 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez4/lib/hci.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9916 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez4/lib/hci_lib.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez4/lib/l2cap.h
+-rw-r--r--   0 runner    (1001) docker     (127)   113715 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez4/lib/sdp.c
+-rw-r--r--   0 runner    (1001) docker     (127)    17273 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez4/lib/sdp.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21697 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez4/lib/sdp_lib.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez4/lib/uuid.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez4/lib/uuid.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:56:08.114700 gattlib-py-0.7.2/bluez/bluez4/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez4/src/log.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez4/src/log.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:56:08.106700 gattlib-py-0.7.2/bluez/bluez5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:56:08.114700 gattlib-py-0.7.2/bluez/bluez5/attrib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/attrib/att-database.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24811 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/attrib/att.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8198 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/attrib/att.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/attrib/gatt-service.h
+-rw-r--r--   0 runner    (1001) docker     (127)    27805 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/attrib/gatt.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/attrib/gatt.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10254 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/attrib/gattrib.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/attrib/gattrib.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/attrib/gatttool.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:56:08.114700 gattlib-py-0.7.2/bluez/bluez5/btio/
+-rw-r--r--   0 runner    (1001) docker     (127)    37670 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/btio/btio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/btio/btio.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:56:08.118700 gattlib-py-0.7.2/bluez/bluez5/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/lib/a2mp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/lib/amp.h
+-rw-r--r--   0 runner    (1001) docker     (127)    49250 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/lib/bluetooth.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9415 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/lib/bluetooth.h
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/lib/bluez.pc
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/lib/bluez.pc.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/lib/bnep.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/lib/cmtp.h
+-rw-r--r--   0 runner    (1001) docker     (127)    65395 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/lib/hci.c
+-rw-r--r--   0 runner    (1001) docker     (127)    63804 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/lib/hci.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10494 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/lib/hci_lib.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/lib/hidp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/lib/l2cap.h
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/lib/libbluetooth-internal.la
+-rw-r--r--   0 runner    (1001) docker     (127)    21400 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/lib/mgmt.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/lib/rfcomm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/lib/sco.h
+-rw-r--r--   0 runner    (1001) docker     (127)   115468 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/lib/sdp.c
+-rw-r--r--   0 runner    (1001) docker     (127)    18250 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/lib/sdp.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21725 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/lib/sdp_lib.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6893 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/lib/uuid.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6757 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/lib/uuid.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:56:08.118700 gattlib-py-0.7.2/bluez/bluez5/monitor/
+-rw-r--r--   0 runner    (1001) docker     (127)    78785 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/monitor/bt.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:56:08.106700 gattlib-py-0.7.2/bluez/bluez5/profiles/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:56:08.118700 gattlib-py-0.7.2/bluez/bluez5/profiles/input/
+-rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/profiles/input/uhid_copy.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:56:08.118700 gattlib-py-0.7.2/bluez/bluez5/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/eir.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/log.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/log.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:56:08.126700 gattlib-py-0.7.2/bluez/bluez5/src/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)    13253 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/shared/ad.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/shared/ad.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/shared/att-types.h
+-rw-r--r--   0 runner    (1001) docker     (127)    33357 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/shared/att.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/shared/att.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10430 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/shared/btsnoop.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/shared/btsnoop.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15523 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/shared/crypto.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/shared/crypto.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21679 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/shared/ecc.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/shared/ecc.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/shared/gap.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/shared/gap.h
+-rw-r--r--   0 runner    (1001) docker     (127)    73336 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/shared/gatt-client.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5472 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/shared/gatt-client.h
+-rw-r--r--   0 runner    (1001) docker     (127)    39496 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/shared/gatt-db.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/shared/gatt-db.h
+-rw-r--r--   0 runner    (1001) docker     (127)    33891 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/shared/gatt-helpers.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/shared/gatt-helpers.h
+-rw-r--r--   0 runner    (1001) docker     (127)    37513 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/shared/gatt-server.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/shared/gatt-server.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/shared/hci-crypto.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/shared/hci-crypto.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10786 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/shared/hci.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/shared/hci.h
+-rw-r--r--   0 runner    (1001) docker     (127)    29458 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/shared/hfp.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/shared/hfp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5790 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/shared/io-glib.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/shared/io.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/shared/mainloop.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/shared/mainloop.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16958 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/shared/mgmt.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/shared/mgmt.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/shared/pcap.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/shared/pcap.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/shared/queue.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/shared/queue.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/shared/ringbuf.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/shared/ringbuf.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16939 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/shared/tester.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/shared/tester.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/shared/timeout-glib.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/shared/timeout-mainloop.c
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/shared/timeout.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/shared/tty.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/shared/uhid.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/shared/uhid.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/shared/util.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/bluez5/src/shared/util.h
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/gattlib.pc.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6951 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/gattlib_adapter.c
+-rw-r--r--   0 runner    (1001) docker     (127)    16490 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/gattlib_connect.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10517 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/gattlib_discover.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/gattlib_internal.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/bluez/gattlib_read_write.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:56:08.126700 gattlib-py-0.7.2/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/common/gattlib_callback_connected_device.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/common/gattlib_callback_disconnected_device.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/common/gattlib_callback_discovered_device.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/common/gattlib_callback_notification_device.c
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/common/gattlib_callback_python.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9195 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/common/gattlib_common.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/common/gattlib_common_adapter.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/common/gattlib_device_state_management.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/common/gattlib_eddystone.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6334 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/common/gattlib_internal.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:56:08.106700 gattlib-py-0.7.2/common/logging_backend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:56:08.126700 gattlib-py-0.7.2/common/logging_backend/printf/
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/common/logging_backend/printf/gattlib_logging.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:56:08.126700 gattlib-py-0.7.2/common/logging_backend/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/common/logging_backend/python/gattlib_logging.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:56:08.126700 gattlib-py-0.7.2/common/logging_backend/syslog/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/common/logging_backend/syslog/gattlib_logging.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:56:08.126700 gattlib-py-0.7.2/common/mainloop/
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/common/mainloop/gattlib_glib_mainloop.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:56:08.130700 gattlib-py-0.7.2/dbus/
+-rw-r--r--   0 runner    (1001) docker     (127)     7092 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/dbus/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:56:08.106700 gattlib-py-0.7.2/dbus/bluez5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:56:08.130700 gattlib-py-0.7.2/dbus/bluez5/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     6899 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/dbus/bluez5/lib/uuid.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6757 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/dbus/bluez5/lib/uuid.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:56:08.130700 gattlib-py-0.7.2/dbus/dbus-bluez-pre-v5.40/
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/dbus/dbus-bluez-pre-v5.40/org.bluez.Adapter1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/dbus/dbus-bluez-pre-v5.40/org.bluez.Device1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/dbus/dbus-bluez-pre-v5.40/org.bluez.GattCharacteristic1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/dbus/dbus-bluez-pre-v5.40/org.bluez.GattDescriptor1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/dbus/dbus-bluez-pre-v5.40/org.bluez.GattService1.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:56:08.130700 gattlib-py-0.7.2/dbus/dbus-bluez-v5.40/
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/dbus/dbus-bluez-v5.40/org.bluez.Adapter1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/dbus/dbus-bluez-v5.40/org.bluez.Battery1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/dbus/dbus-bluez-v5.40/org.bluez.Device1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/dbus/dbus-bluez-v5.40/org.bluez.GattCharacteristic1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/dbus/dbus-bluez-v5.40/org.bluez.GattDescriptor1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/dbus/dbus-bluez-v5.40/org.bluez.GattService1.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:56:08.130700 gattlib-py-0.7.2/dbus/dbus-bluez-v5.48/
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/dbus/dbus-bluez-v5.48/org.bluez.Adapter1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/dbus/dbus-bluez-v5.48/org.bluez.Battery1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/dbus/dbus-bluez-v5.48/org.bluez.Device1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/dbus/dbus-bluez-v5.48/org.bluez.GattCharacteristic1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/dbus/dbus-bluez-v5.48/org.bluez.GattDescriptor1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/dbus/dbus-bluez-v5.48/org.bluez.GattService1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    38771 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/dbus/gattlib.c
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/dbus/gattlib.pc.in
+-rw-r--r--   0 runner    (1001) docker     (127)    25348 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/dbus/gattlib_adapter.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5799 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/dbus/gattlib_advertisement.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/dbus/gattlib_backend.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16209 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/dbus/gattlib_char.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9844 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/dbus/gattlib_notification.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/dbus/gattlib_stream.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:56:08.134700 gattlib-py-0.7.2/gattlib/
+-rw-r--r--   0 runner    (1001) docker     (127)    12281 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/gattlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 12:56:07.000000 gattlib-py-0.7.2/gattlib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9606 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/gattlib/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11161 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/gattlib/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/gattlib/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/gattlib/gatt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/gattlib/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/gattlib/mainloop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/gattlib/uuid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:56:08.134700 gattlib-py-0.7.2/gattlib_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-24 12:56:08.000000 gattlib-py-0.7.2/gattlib_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-04-24 12:56:08.000000 gattlib-py-0.7.2/gattlib_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 12:56:08.000000 gattlib-py-0.7.2/gattlib_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-24 12:56:08.000000 gattlib-py-0.7.2/gattlib_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-24 12:56:08.000000 gattlib-py-0.7.2/gattlib_py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:56:08.134700 gattlib-py-0.7.2/include/
+-rw-r--r--   0 runner    (1001) docker     (127)    30835 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/include/gattlib.h
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 12:56:08.134700 gattlib-py-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     7503 2024-04-24 12:38:21.000000 gattlib-py-0.7.2/setup.py
```

### Comparing `gattlib-py-0.7.1/CMakeLists.txt` & `gattlib-py-0.7.2/CMakeLists.txt`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
   # Examples
   add_subdirectory(examples/advertisement_data)
   add_subdirectory(examples/ble_scan)
   add_subdirectory(examples/discover)
   add_subdirectory(examples/find_eddystone)
   add_subdirectory(examples/read_write)
   #add_subdirectory(examples/read_write_memory)
-  #add_subdirectory(examples/notification)
+  add_subdirectory(examples/notification)
   #add_subdirectory(examples/nordic_uart)
   add_subdirectory(tests/test_continuous_connection)
 
   # Some examples require Bluez code and other DBus support
   if (NOT GATTLIB_DBUS)
     add_subdirectory(examples/gatttool)
   endif()
```

### Comparing `gattlib-py-0.7.1/CrossCompilation.cmake` & `gattlib-py-0.7.2/CrossCompilation.cmake`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/PKG-INFO` & `gattlib-py-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gattlib-py
-Version: 0.7.1
+Version: 0.7.2
 Summary: Python wrapper for gattlib library
 Home-page: https://github.com/labapart/gattlib/gattlib-py
 Author: Olivier Martin
 Author-email: olivier@labapart.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `gattlib-py-0.7.1/bluez/CMakeLists.txt` & `gattlib-py-0.7.2/bluez/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez4/attrib/att.c` & `gattlib-py-0.7.2/bluez/bluez4/attrib/att.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez4/attrib/att.h` & `gattlib-py-0.7.2/bluez/bluez4/attrib/att.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez4/attrib/gatt.c` & `gattlib-py-0.7.2/bluez/bluez4/attrib/gatt.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez4/attrib/gatt.h` & `gattlib-py-0.7.2/bluez/bluez4/attrib/gatt.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez4/attrib/gattrib.c` & `gattlib-py-0.7.2/bluez/bluez4/attrib/gattrib.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez4/attrib/gattrib.h` & `gattlib-py-0.7.2/bluez/bluez4/attrib/gattrib.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez4/btio/btio.c` & `gattlib-py-0.7.2/bluez/bluez4/btio/btio.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez4/btio/btio.h` & `gattlib-py-0.7.2/bluez/bluez4/btio/btio.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez4/lib/bluetooth.c` & `gattlib-py-0.7.2/bluez/bluez4/lib/bluetooth.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez4/lib/bluetooth.h` & `gattlib-py-0.7.2/bluez/bluez4/lib/bluetooth.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez4/lib/hci.c` & `gattlib-py-0.7.2/bluez/bluez4/lib/hci.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez4/lib/hci.h` & `gattlib-py-0.7.2/bluez/bluez4/lib/hci.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez4/lib/hci_lib.h` & `gattlib-py-0.7.2/bluez/bluez4/lib/hci_lib.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez4/lib/l2cap.h` & `gattlib-py-0.7.2/bluez/bluez4/lib/l2cap.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez4/lib/sdp.c` & `gattlib-py-0.7.2/bluez/bluez4/lib/sdp.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez4/lib/sdp.h` & `gattlib-py-0.7.2/bluez/bluez4/lib/sdp.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez4/lib/sdp_lib.h` & `gattlib-py-0.7.2/bluez/bluez4/lib/sdp_lib.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez4/lib/uuid.c` & `gattlib-py-0.7.2/bluez/bluez4/lib/uuid.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez4/lib/uuid.h` & `gattlib-py-0.7.2/bluez/bluez4/lib/uuid.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez4/src/log.c` & `gattlib-py-0.7.2/bluez/bluez4/src/log.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez4/src/log.h` & `gattlib-py-0.7.2/bluez/bluez4/src/log.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/attrib/att-database.h` & `gattlib-py-0.7.2/bluez/bluez5/attrib/att-database.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/attrib/att.c` & `gattlib-py-0.7.2/bluez/bluez5/attrib/att.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/attrib/att.h` & `gattlib-py-0.7.2/bluez/bluez5/attrib/att.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/attrib/gatt-service.h` & `gattlib-py-0.7.2/bluez/bluez5/attrib/gatt-service.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/attrib/gatt.c` & `gattlib-py-0.7.2/bluez/bluez5/attrib/gatt.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/attrib/gatt.h` & `gattlib-py-0.7.2/bluez/bluez5/attrib/gatt.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/attrib/gattrib.c` & `gattlib-py-0.7.2/bluez/bluez5/attrib/gattrib.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/attrib/gattrib.h` & `gattlib-py-0.7.2/bluez/bluez5/attrib/gattrib.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/attrib/gatttool.h` & `gattlib-py-0.7.2/bluez/bluez5/attrib/gatttool.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/btio/btio.c` & `gattlib-py-0.7.2/bluez/bluez5/btio/btio.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/btio/btio.h` & `gattlib-py-0.7.2/bluez/bluez5/btio/btio.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/lib/a2mp.h` & `gattlib-py-0.7.2/bluez/bluez5/lib/a2mp.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/lib/amp.h` & `gattlib-py-0.7.2/bluez/bluez5/lib/amp.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/lib/bluetooth.c` & `gattlib-py-0.7.2/bluez/bluez5/lib/bluetooth.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/lib/bluetooth.h` & `gattlib-py-0.7.2/bluez/bluez5/lib/bluetooth.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/lib/bnep.h` & `gattlib-py-0.7.2/bluez/bluez5/lib/bnep.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/lib/cmtp.h` & `gattlib-py-0.7.2/bluez/bluez5/lib/cmtp.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/lib/hci.c` & `gattlib-py-0.7.2/bluez/bluez5/lib/hci.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/lib/hci.h` & `gattlib-py-0.7.2/bluez/bluez5/lib/hci.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/lib/hci_lib.h` & `gattlib-py-0.7.2/bluez/bluez5/lib/hci_lib.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/lib/hidp.h` & `gattlib-py-0.7.2/bluez/bluez5/lib/hidp.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/lib/l2cap.h` & `gattlib-py-0.7.2/bluez/bluez5/lib/l2cap.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/lib/libbluetooth-internal.la` & `gattlib-py-0.7.2/bluez/bluez5/lib/libbluetooth-internal.la`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/lib/mgmt.h` & `gattlib-py-0.7.2/bluez/bluez5/lib/mgmt.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/lib/rfcomm.h` & `gattlib-py-0.7.2/bluez/bluez5/lib/rfcomm.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/lib/sco.h` & `gattlib-py-0.7.2/bluez/bluez5/lib/sco.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/lib/sdp.c` & `gattlib-py-0.7.2/bluez/bluez5/lib/sdp.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/lib/sdp.h` & `gattlib-py-0.7.2/bluez/bluez5/lib/sdp.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/lib/sdp_lib.h` & `gattlib-py-0.7.2/bluez/bluez5/lib/sdp_lib.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/lib/uuid.c` & `gattlib-py-0.7.2/bluez/bluez5/lib/uuid.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/lib/uuid.h` & `gattlib-py-0.7.2/bluez/bluez5/lib/uuid.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/monitor/bt.h` & `gattlib-py-0.7.2/bluez/bluez5/monitor/bt.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/profiles/input/uhid_copy.h` & `gattlib-py-0.7.2/bluez/bluez5/profiles/input/uhid_copy.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/eir.h` & `gattlib-py-0.7.2/bluez/bluez5/src/eir.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/log.c` & `gattlib-py-0.7.2/bluez/bluez5/src/log.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/log.h` & `gattlib-py-0.7.2/bluez/bluez5/src/log.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/shared/ad.c` & `gattlib-py-0.7.2/bluez/bluez5/src/shared/ad.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/shared/ad.h` & `gattlib-py-0.7.2/bluez/bluez5/src/shared/ad.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/shared/att-types.h` & `gattlib-py-0.7.2/bluez/bluez5/src/shared/att-types.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/shared/att.c` & `gattlib-py-0.7.2/bluez/bluez5/src/shared/att.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/shared/att.h` & `gattlib-py-0.7.2/bluez/bluez5/src/shared/att.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/shared/btsnoop.c` & `gattlib-py-0.7.2/bluez/bluez5/src/shared/btsnoop.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/shared/btsnoop.h` & `gattlib-py-0.7.2/bluez/bluez5/src/shared/btsnoop.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/shared/crypto.c` & `gattlib-py-0.7.2/bluez/bluez5/src/shared/crypto.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/shared/crypto.h` & `gattlib-py-0.7.2/bluez/bluez5/src/shared/crypto.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/shared/ecc.c` & `gattlib-py-0.7.2/bluez/bluez5/src/shared/ecc.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/shared/ecc.h` & `gattlib-py-0.7.2/bluez/bluez5/src/shared/ecc.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/shared/gap.c` & `gattlib-py-0.7.2/bluez/bluez5/src/shared/gap.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/shared/gap.h` & `gattlib-py-0.7.2/bluez/bluez5/src/shared/gap.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/shared/gatt-client.c` & `gattlib-py-0.7.2/bluez/bluez5/src/shared/gatt-client.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/shared/gatt-client.h` & `gattlib-py-0.7.2/bluez/bluez5/src/shared/gatt-client.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/shared/gatt-db.c` & `gattlib-py-0.7.2/bluez/bluez5/src/shared/gatt-db.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/shared/gatt-db.h` & `gattlib-py-0.7.2/bluez/bluez5/src/shared/gatt-db.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/shared/gatt-helpers.c` & `gattlib-py-0.7.2/bluez/bluez5/src/shared/gatt-helpers.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/shared/gatt-helpers.h` & `gattlib-py-0.7.2/bluez/bluez5/src/shared/gatt-helpers.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/shared/gatt-server.c` & `gattlib-py-0.7.2/bluez/bluez5/src/shared/gatt-server.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/shared/gatt-server.h` & `gattlib-py-0.7.2/bluez/bluez5/src/shared/gatt-server.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/shared/hci-crypto.c` & `gattlib-py-0.7.2/bluez/bluez5/src/shared/hci-crypto.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/shared/hci-crypto.h` & `gattlib-py-0.7.2/bluez/bluez5/src/shared/hci-crypto.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/shared/hci.c` & `gattlib-py-0.7.2/bluez/bluez5/src/shared/hci.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/shared/hci.h` & `gattlib-py-0.7.2/bluez/bluez5/src/shared/hci.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/shared/hfp.c` & `gattlib-py-0.7.2/bluez/bluez5/src/shared/hfp.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/shared/hfp.h` & `gattlib-py-0.7.2/bluez/bluez5/src/shared/hfp.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/shared/io-glib.c` & `gattlib-py-0.7.2/bluez/bluez5/src/shared/io-glib.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/shared/io.h` & `gattlib-py-0.7.2/bluez/bluez5/src/shared/io.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/shared/mainloop.c` & `gattlib-py-0.7.2/bluez/bluez5/src/shared/mainloop.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/shared/mainloop.h` & `gattlib-py-0.7.2/bluez/bluez5/src/shared/mainloop.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/shared/mgmt.c` & `gattlib-py-0.7.2/bluez/bluez5/src/shared/mgmt.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/shared/mgmt.h` & `gattlib-py-0.7.2/bluez/bluez5/src/shared/mgmt.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/shared/pcap.c` & `gattlib-py-0.7.2/bluez/bluez5/src/shared/pcap.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/shared/pcap.h` & `gattlib-py-0.7.2/bluez/bluez5/src/shared/pcap.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/shared/queue.c` & `gattlib-py-0.7.2/bluez/bluez5/src/shared/queue.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/shared/queue.h` & `gattlib-py-0.7.2/bluez/bluez5/src/shared/queue.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/shared/ringbuf.c` & `gattlib-py-0.7.2/bluez/bluez5/src/shared/ringbuf.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/shared/ringbuf.h` & `gattlib-py-0.7.2/bluez/bluez5/src/shared/ringbuf.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/shared/tester.c` & `gattlib-py-0.7.2/bluez/bluez5/src/shared/tester.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/shared/tester.h` & `gattlib-py-0.7.2/bluez/bluez5/src/shared/tester.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/shared/timeout-glib.c` & `gattlib-py-0.7.2/bluez/bluez5/src/shared/timeout-glib.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/shared/timeout-mainloop.c` & `gattlib-py-0.7.2/bluez/bluez5/src/shared/timeout-mainloop.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/shared/timeout.h` & `gattlib-py-0.7.2/bluez/bluez5/src/shared/timeout.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/shared/tty.h` & `gattlib-py-0.7.2/bluez/bluez5/src/shared/tty.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/shared/uhid.c` & `gattlib-py-0.7.2/bluez/bluez5/src/shared/uhid.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/shared/uhid.h` & `gattlib-py-0.7.2/bluez/bluez5/src/shared/uhid.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/shared/util.c` & `gattlib-py-0.7.2/bluez/bluez5/src/shared/util.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/bluez5/src/shared/util.h` & `gattlib-py-0.7.2/bluez/bluez5/src/shared/util.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/gattlib_adapter.c` & `gattlib-py-0.7.2/bluez/gattlib_adapter.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/gattlib_connect.c` & `gattlib-py-0.7.2/bluez/gattlib_connect.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/gattlib_discover.c` & `gattlib-py-0.7.2/bluez/gattlib_discover.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/gattlib_internal.h` & `gattlib-py-0.7.2/bluez/gattlib_internal.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/bluez/gattlib_read_write.c` & `gattlib-py-0.7.2/bluez/gattlib_read_write.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/common/gattlib_callback_connected_device.c` & `gattlib-py-0.7.2/common/gattlib_callback_connected_device.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/common/gattlib_callback_disconnected_device.c` & `gattlib-py-0.7.2/common/gattlib_callback_disconnected_device.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/common/gattlib_callback_discovered_device.c` & `gattlib-py-0.7.2/common/gattlib_callback_discovered_device.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/common/gattlib_callback_notification_device.c` & `gattlib-py-0.7.2/common/gattlib_callback_notification_device.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/common/gattlib_callback_python.c` & `gattlib-py-0.7.2/common/gattlib_callback_python.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/common/gattlib_common_adapter.c` & `gattlib-py-0.7.2/common/gattlib_common_adapter.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/common/gattlib_device_state_management.c` & `gattlib-py-0.7.2/common/gattlib_device_state_management.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/common/gattlib_eddystone.c` & `gattlib-py-0.7.2/common/gattlib_eddystone.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/common/gattlib_internal.h` & `gattlib-py-0.7.2/common/gattlib_internal.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/common/logging_backend/python/gattlib_logging.c` & `gattlib-py-0.7.2/common/logging_backend/python/gattlib_logging.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/common/mainloop/gattlib_glib_mainloop.c` & `gattlib-py-0.7.2/common/mainloop/gattlib_glib_mainloop.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/dbus/CMakeLists.txt` & `gattlib-py-0.7.2/dbus/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/dbus/bluez5/lib/uuid.c` & `gattlib-py-0.7.2/dbus/bluez5/lib/uuid.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/dbus/bluez5/lib/uuid.h` & `gattlib-py-0.7.2/dbus/bluez5/lib/uuid.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/dbus/dbus-bluez-pre-v5.40/org.bluez.Adapter1.xml` & `gattlib-py-0.7.2/dbus/dbus-bluez-pre-v5.40/org.bluez.Adapter1.xml`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/dbus/dbus-bluez-pre-v5.40/org.bluez.Device1.xml` & `gattlib-py-0.7.2/dbus/dbus-bluez-pre-v5.40/org.bluez.Device1.xml`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/dbus/dbus-bluez-pre-v5.40/org.bluez.GattCharacteristic1.xml` & `gattlib-py-0.7.2/dbus/dbus-bluez-pre-v5.40/org.bluez.GattCharacteristic1.xml`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/dbus/dbus-bluez-pre-v5.40/org.bluez.GattDescriptor1.xml` & `gattlib-py-0.7.2/dbus/dbus-bluez-pre-v5.40/org.bluez.GattDescriptor1.xml`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/dbus/dbus-bluez-pre-v5.40/org.bluez.GattService1.xml` & `gattlib-py-0.7.2/dbus/dbus-bluez-pre-v5.40/org.bluez.GattService1.xml`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/dbus/dbus-bluez-v5.40/org.bluez.Adapter1.xml` & `gattlib-py-0.7.2/dbus/dbus-bluez-v5.40/org.bluez.Adapter1.xml`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/dbus/dbus-bluez-v5.40/org.bluez.Device1.xml` & `gattlib-py-0.7.2/dbus/dbus-bluez-v5.40/org.bluez.Device1.xml`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/dbus/dbus-bluez-v5.40/org.bluez.GattCharacteristic1.xml` & `gattlib-py-0.7.2/dbus/dbus-bluez-v5.40/org.bluez.GattCharacteristic1.xml`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/dbus/dbus-bluez-v5.40/org.bluez.GattDescriptor1.xml` & `gattlib-py-0.7.2/dbus/dbus-bluez-v5.40/org.bluez.GattDescriptor1.xml`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/dbus/dbus-bluez-v5.40/org.bluez.GattService1.xml` & `gattlib-py-0.7.2/dbus/dbus-bluez-v5.40/org.bluez.GattService1.xml`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/dbus/dbus-bluez-v5.48/org.bluez.Adapter1.xml` & `gattlib-py-0.7.2/dbus/dbus-bluez-v5.48/org.bluez.Adapter1.xml`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/dbus/dbus-bluez-v5.48/org.bluez.Device1.xml` & `gattlib-py-0.7.2/dbus/dbus-bluez-v5.48/org.bluez.Device1.xml`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/dbus/dbus-bluez-v5.48/org.bluez.GattCharacteristic1.xml` & `gattlib-py-0.7.2/dbus/dbus-bluez-v5.48/org.bluez.GattCharacteristic1.xml`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/dbus/dbus-bluez-v5.48/org.bluez.GattDescriptor1.xml` & `gattlib-py-0.7.2/dbus/dbus-bluez-v5.48/org.bluez.GattDescriptor1.xml`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/dbus/dbus-bluez-v5.48/org.bluez.GattService1.xml` & `gattlib-py-0.7.2/dbus/dbus-bluez-v5.48/org.bluez.GattService1.xml`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/dbus/gattlib.c` & `gattlib-py-0.7.2/dbus/gattlib.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/dbus/gattlib_adapter.c` & `gattlib-py-0.7.2/dbus/gattlib_adapter.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/dbus/gattlib_advertisement.c` & `gattlib-py-0.7.2/dbus/gattlib_advertisement.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/dbus/gattlib_backend.h` & `gattlib-py-0.7.2/dbus/gattlib_backend.h`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/dbus/gattlib_char.c` & `gattlib-py-0.7.2/dbus/gattlib_char.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/dbus/gattlib_notification.c` & `gattlib-py-0.7.2/dbus/gattlib_notification.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/dbus/gattlib_stream.c` & `gattlib-py-0.7.2/dbus/gattlib_stream.c`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.7.1/gattlib/__init__.py` & `gattlib-py-0.7.2/gattlib/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 #
 # SPDX-License-Identifier: BSD-3-Clause
 #
 # Copyright (c) 2016-2024, Olivier Martin <olivier@labapart.org>
 #
 
+"""Gattlib C types and functions"""
+
 from ctypes import *
 import logging
 import pathlib
 
 try:
     # '_version.py' is generated by 'setup.py'
-    from ._version import __version__
-except:
+    from ._version import __version__  #pylint: disable=import-error
+except:  #pylint: disable=bare-except
     pass
 
 logger = logging.getLogger(__name__)
 
 try:
     gattlib = cdll.LoadLibrary(str(pathlib.Path(__file__).with_name('libgattlib.so')))
 except OSError:
     # While in development, we might not have 'libgattlib.so' into the python directory
     # We can define 'libgattlib.so' location using LD_LIBRARY_PATH
     gattlib = CDLL('libgattlib.so')
 
 def native_logging(level: int, string: str):
+    """Convert Gattlib logging to Python logging."""
     if level == 3:
         logger.debug(string)
     elif level == 2:
         logger.info(string)
     elif level == 1:
         logger.warning(string)
     elif level == 0:
@@ -46,73 +49,80 @@
     # Excepted when using a Gattlib logging backend without 'gattlib_log_init'
     pass
 
 # typedef struct {
 #    uint8_t data[16];
 # } uint128_t;
 class GattlibUuid128(Structure):
+    """Python class representing the C structure 'uint128_t'."""
     _fields_ = [("data", c_byte * 16)]
 
 
 # typedef struct {
 #    uint8_t type;
 #    union {
 #        uint16_t  uuid16;
 #        uint32_t  uuid32;
 #        uint128_t uuid128;
 #    } value;
 # } uuid_t;
 class GattlibUuidValue(Union):
+    """Python class representing the C structure of the value of 'uuid_t'."""
     _fields_ = [("uuid16", c_ushort), ("uuid32", c_uint), ("uuid128", GattlibUuid128)]
 
 
 class GattlibUuid(Structure):
+    """Python class representing the C structure 'uuid_t'."""
     _fields_ = [("type", c_byte), ("value", GattlibUuidValue)]
 
 
 # typedef struct {
 #    uint16_t  attr_handle_start;
 #    uint16_t  attr_handle_end;
 #    uuid_t    uuid;
 # } gattlib_primary_service_t;
 class GattlibPrimaryService(Structure):
+    """Python class representing the C structure 'gattlib_primary_service_t'."""
     _fields_ = [("attr_handle_start", c_ushort),
                 ("attr_handle_end", c_ushort),
                 ("uuid", GattlibUuid)]
 
 
 # typedef struct {
 #    uint16_t  handle;
 #    uint8_t   properties;
 #    uint16_t  value_handle;
 #    uuid_t    uuid;
 # } gattlib_characteristic_t;
 class GattlibCharacteristic(Structure):
+    """Python class representing the C structure 'gattlib_characteristic_t'."""
     _fields_ = [("handle", c_ushort),
                 ("properties", c_byte),
                 ("value_handle", c_ushort),
                 ("uuid", GattlibUuid)]
 
 
 # typedef struct {
 #     uuid_t   uuid;
 #     uint8_t* data;
 #     size_t   data_length;
 # } gattlib_advertisement_data_t;
 class GattlibAdvertisementData(Structure):
+    """Python class representing the C structure 'gattlib_advertisement_data_t'."""
     _fields_ = [("uuid", GattlibUuid),
                 ("data", c_void_p),
                 ("data_length", c_size_t)]
 
 # typedef struct {
 # 	uint16_t manufacturer_id;
 # 	uint8_t* data;
 # 	size_t data_size;
 # } gattlib_manufacturer_data_t;
 class GattlibManufacturerData(Structure):
+    """Python class representing the C structure 'gattlib_manufacturer_data_t'."""
     _fields_ = [("manufacturer_id", c_ushort),
                 ("data", c_void_p),
                 ("data_size", c_size_t)]
 
 
 # int gattlib_adapter_open(const char* adapter_name, gattlib_adapter_t** adapter);
 gattlib_adapter_open = gattlib.gattlib_adapter_open
@@ -124,15 +134,16 @@
 gattlib_adapter_get_name.restype = c_char_p
 
 # void gattlib_discovered_device_python_callback(gattlib_adapter_t* adapter, const char* addr, const char* name, void *user_data)
 gattlib_discovered_device_python_callback = gattlib.gattlib_discovered_device_python_callback
 gattlib_discovered_device_python_callback.argtypes = [c_void_p, c_char_p, c_char_p, py_object]
 gattlib_discovered_device_python_callback.restype = c_void_p
 
-# void gattlib_connected_device_python_callback(gattlib_adapter_t* adapter, const char *dst, gattlib_connection_t* connection, int error, void* user_data);
+# void gattlib_connected_device_python_callback(gattlib_adapter_t* adapter, const char *dst, gattlib_connection_t* connection,
+#                                               int error, void* user_data);
 gattlib_connected_device_python_callback = gattlib.gattlib_connected_device_python_callback
 gattlib_connected_device_python_callback.argtypes = [c_void_p, c_char_p, c_void_p, c_int, py_object]
 gattlib_connected_device_python_callback.restype = c_void_p
 
 # void gattlib_disconnected_device_python_callback(void *user_data)
 gattlib_disconnected_device_python_callback = gattlib.gattlib_disconnected_device_python_callback
 gattlib_disconnected_device_python_callback.argtypes = [py_object]
@@ -144,18 +155,20 @@
 gattlib_notification_device_python_callback.restype = c_void_p
 
 # void* gattlib_python_callback_args(PyObject* python_callback, PyObject* python_args) {
 gattlib_python_callback_args = gattlib.gattlib_python_callback_args
 gattlib_python_callback_args.argtypes = [py_object, py_object]
 gattlib_python_callback_args.restype = c_void_p
 
-# int gattlib_adapter_scan_enable_with_filter_non_blocking(gattlib_adapter_t* adapter, uuid_t **uuid_list, int16_t rssi_threshold, uint32_t enabled_filters,
+# int gattlib_adapter_scan_enable_with_filter_non_blocking(gattlib_adapter_t* adapter, uuid_t **uuid_list,
+#        int16_t rssi_threshold, uint32_t enabled_filters,
 #        gattlib_discovered_device_t discovered_device_cb, size_t timeout, void *user_data)
 gattlib_adapter_scan_enable_with_filter_non_blocking = gattlib.gattlib_adapter_scan_enable_with_filter_non_blocking
-gattlib_adapter_scan_enable_with_filter_non_blocking.argtypes = [c_void_p, POINTER(POINTER(GattlibUuid)), c_int16, c_uint32, c_void_p, c_size_t, c_void_p]
+gattlib_adapter_scan_enable_with_filter_non_blocking.argtypes = [c_void_p, POINTER(POINTER(GattlibUuid)),
+                                                                 c_int16, c_uint32, c_void_p, c_size_t, c_void_p]
 
 # int gattlib_adapter_scan_eddystone(gattlib_adapter_t* adapter, int16_t rssi_threshold, uint32_t eddsytone_types,
 #        gattlib_discovered_device_with_data_t discovered_device_cb, size_t timeout, void *user_data)
 gattlib_adapter_scan_eddystone = gattlib.gattlib_adapter_scan_eddystone
 gattlib_adapter_scan_eddystone.argtypes = [c_void_p, c_int16, c_uint32, py_object, c_size_t, py_object]
 
 # int gattlib_connect(gattlib_adapter_t* adapter, const char *dst, unsigned long options, gatt_connect_cb_t connect_cb, void* user_data)
@@ -218,21 +231,25 @@
 gattlib_get_rssi_from_mac = gattlib.gattlib_get_rssi_from_mac
 gattlib_get_rssi_from_mac.argtypes = [c_void_p, c_char_p, POINTER(c_int16)]
 
 # int gattlib_get_advertisement_data(gattlib_connection_t *connection,
 # 		 gattlib_advertisement_data_t **advertisement_data, size_t *advertisement_data_count,
 # 		 gattlib_manufacturer_data_t** manufacturer_data, size_t* manufacturer_data_count)
 gattlib_get_advertisement_data = gattlib.gattlib_get_advertisement_data
-gattlib_get_advertisement_data.argtypes = [c_void_p, POINTER(POINTER(GattlibAdvertisementData)), POINTER(c_size_t), POINTER(POINTER(GattlibManufacturerData)), POINTER(c_size_t)]
+gattlib_get_advertisement_data.argtypes = [c_void_p,
+                                           POINTER(POINTER(GattlibAdvertisementData)), POINTER(c_size_t),
+                                           POINTER(POINTER(GattlibManufacturerData)), POINTER(c_size_t)]
 
 # int gattlib_get_advertisement_data_from_mac(gattlib_adapter_t* adapter, const char *mac_address,
 #        gattlib_advertisement_data_t **advertisement_data, size_t *advertisement_data_length,
 #        gattlib_manufacturer_data_t** manufacturer_data, size_t* manufacturer_data_count)
 gattlib_get_advertisement_data_from_mac = gattlib.gattlib_get_advertisement_data_from_mac
-gattlib_get_advertisement_data_from_mac.argtypes = [c_void_p, c_char_p, POINTER(POINTER(GattlibAdvertisementData)), POINTER(c_size_t), POINTER(POINTER(GattlibManufacturerData)), POINTER(c_size_t)]
+gattlib_get_advertisement_data_from_mac.argtypes = [c_void_p, c_char_p,
+                                                    POINTER(POINTER(GattlibAdvertisementData)), POINTER(c_size_t),
+                                                    POINTER(POINTER(GattlibManufacturerData)), POINTER(c_size_t)]
 
 # int gattlib_mainloop_python(PyObject *handler, PyObject *user_data)
 gattlib_mainloop = gattlib.gattlib_mainloop_python
 gattlib_mainloop.argtypes = [py_object, py_object]
 
 # void gattlib_free_mem(void *ptr])
 gattlib_free_mem = gattlib.gattlib_free_mem
```

### Comparing `gattlib-py-0.7.1/gattlib/adapter.py` & `gattlib-py-0.7.2/gattlib/adapter.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 #
 # SPDX-License-Identifier: BSD-3-Clause
 #
 # Copyright (c) 2016-2024, Olivier Martin <olivier@labapart.org>
 #
 
+"""Gattlib Adapter API"""
+
 import threading
 from uuid import UUID
 
-from gattlib import *
+from gattlib import *  #pylint: disable=wildcard-import,unused-wildcard-import
 from .device import Device
 from .exception import handle_return
-from .uuid import gattlib_uuid_to_int
+from .helpers import convert_gattlib_advertisement_c_data_to_dict
 
 GATTLIB_DISCOVER_FILTER_USE_UUID = (1 << 0)
 GATTLIB_DISCOVER_FILTER_USE_RSSI = (1 << 1)
 GATTLIB_DISCOVER_FILTER_NOTIFY_CHANGE = (1 << 2)
 
 GATTLIB_EDDYSTONE_TYPE_UID = (1 << 0)
 GATTLIB_EDDYSTONE_TYPE_URL = (1 << 1)
@@ -34,72 +36,71 @@
     0x01: "https://www.",
     0x02: "http://",
     0x03: "https://",
 }
 
 
 class Adapter:
-
+    """Bluetooth adapter."""
     def __init__(self, name=c_char_p(None)):
         self._name = name
         self._adapter = c_void_p(None)
         self._is_opened = False  # Note: 'self._adapter != c_void_p(None)' does not seem to return the expected result
         self._lock = threading.Lock()
+        self._on_discovered_device_callback = None
+        self._on_discovered_device_user_callback = None
 
     def __str__(self) -> str:
         if self._name:
             return self._name
         else:
             return f"adapter@{self._adapter}"
 
     @property
     def name(self):
+        """Return adapter name."""
         return self._name
 
-    @staticmethod
-    def list():
-        # TODO: Add support
-        return []
+    #@staticmethod
+    #def list():
+    #    # TODO: Add support
+    #    return []
 
     def open(self):
-        self._lock.acquire()
-        if self._is_opened:
-            self._lock.release()
-            return
+        """Open adapter."""
+        with self._lock:
+            if self._is_opened:
+                return
 
-        try:
             self._adapter = c_void_p(None)
             ret = gattlib_adapter_open(self._name, byref(self._adapter))
             if ret == 0:
                 self._is_opened = True
                 if self._name is None:
                     self._name = gattlib_adapter_get_name(self._adapter)
             else:
                 handle_return(ret)
-        finally:
-            self._lock.release()
 
     def close(self):
-        self._lock.acquire()
-        try:
+        """Close adapter."""
+        with self._lock:
             if self._adapter:
                 ret = gattlib.gattlib_adapter_close(self._adapter)
                 handle_return(ret)
             self._is_opened = False
             self._adapter = None
-        finally:
-            self._lock.release()
 
     # Use a closure to return a method that can be called by the C-library (see: https://stackoverflow.com/a/7261524/6267288)
     def get_on_discovered_device_callback(self):
+        """Return a callback for newly discovered device."""
         def on_discovered_device(adapter, addr, name, user_data):
             try:
                 device = Device(self, addr, name)
-                self.on_discovered_device_user_callback(device, user_data)
-            except Exception as e:
+                self._on_discovered_device_user_callback(device, user_data)
+            except Exception as e:  #pylint: disable=broad-exception-caught
                 logger.exception(e)
         return on_discovered_device
 
     def scan_enable(self, on_discovered_device_callback, timeout, notify_change=False, uuids=None, rssi_threshold=None, user_data=None):
         """
         Scan for BLE devices
 
@@ -111,19 +112,19 @@
         @param rssi_threshold: is the imposed RSSI threshold for the returned devices.
         @param enabled_filters: defines the parameters to use for filtering. There are selected by using the macros
                GATTLIB_DISCOVER_FILTER_USE_UUID and GATTLIB_DISCOVER_FILTER_USE_RSSI.
         @param discovered_device_cb: is the function callback called for each new Bluetooth device discovered
         @param timeout: defines the duration of the Bluetooth scanning. When timeout=None or 0, we scan indefinitely.
         @param user_data: is the data passed to the callback `discovered_device_cb()`
         """
-        assert on_discovered_device_callback != None
-        self.on_discovered_device_user_callback = on_discovered_device_callback
-        # Save callback to prevent it to be cleaned by garbage collector see
-        # comment: https://stackoverflow.com/questions/7259794/how-can-i-get-methods-to-work-as-callbacks-with-python-ctypes#comment38658391_7261524
-        self.on_discovered_device_callback = self.get_on_discovered_device_callback()
+        assert on_discovered_device_callback is not None
+        self._on_discovered_device_user_callback = on_discovered_device_callback
+        # Save callback to prevent it to be cleaned by garbage collector see comment:
+        # https://stackoverflow.com/questions/7259794/how-can-i-get-methods-to-work-as-callbacks-with-python-ctypes#comment38658391_7261524
+        self._on_discovered_device_callback = self.get_on_discovered_device_callback()
 
         # Ensure BLE adapter it opened
         if not self._is_opened:
             self.open()
 
         enabled_filters = 0
         uuid_list = None
@@ -160,49 +161,31 @@
         if timeout is None:
             timeout = 0
 
         ret = gattlib_adapter_scan_enable_with_filter_non_blocking(self._adapter,
                                                       uuid_list, rssi, enabled_filters,
                                                       gattlib_discovered_device_python_callback,
                                                       timeout,
-                                                      gattlib_python_callback_args(self.on_discovered_device_callback, user_data))
+                                                      gattlib_python_callback_args(self._on_discovered_device_callback, user_data))
         handle_return(ret)
 
     @staticmethod
     def on_discovered_ble_device_with_details(adapter, mac_addr, name, advertisement_data_buffer, advertisement_data_count,
-                                              manufacturer_id, manufacturer_data_buffer, manufacturer_data_size,
+                                              manufacturer_data_buffer, manufacturer_data_count,
                                               user_data):
-        advertisement_data = {}
-        manufacturer_data = None
-
-        for i in range(0, advertisement_data_count):
-            service_data = advertisement_data_buffer[i]
-            uuid = gattlib_uuid_to_int(service_data.uuid)
-
-            pointer_type = POINTER(c_byte * service_data.data_length)
-            c_bytearray = cast(service_data.data, pointer_type)
-
-            data = bytearray(service_data.data_length)
-            for i in range(service_data.data_length):
-                data[i] = c_bytearray.contents[i] & 0xFF
-
-            advertisement_data[uuid] = data
-
-        if manufacturer_data_size > 0:
-            pointer_type = POINTER(c_byte * manufacturer_data_size)
-            c_bytearray = cast(manufacturer_data_buffer, pointer_type)
-
-            manufacturer_data = bytearray(manufacturer_data_size)
-            for i in range(manufacturer_data_size):
-                manufacturer_data[i] = c_bytearray.contents[i] & 0xFF
+        """Callback invoked when a new device has been discovered."""
+        advertisement_data, manufacturer_data = convert_gattlib_advertisement_c_data_to_dict(
+                advertisement_data_buffer, advertisement_data_count,
+                manufacturer_data_buffer, manufacturer_data_count)
 
         device = Device(user_data["adapter"], mac_addr, name)
-        user_data["callback"](device, advertisement_data, manufacturer_id, manufacturer_data, user_data["user_data"])
+        user_data["callback"](device, advertisement_data, manufacturer_data, user_data["user_data"])
 
     def scan_eddystone_enable(self, on_discovered_device_callback, eddystone_filters, timeout, rssi_threshold=None, user_data=None):
+        """Enable BLE scan for Eddystone devices."""
         # Ensure BLE adapter it opened
         if not self._is_opened:
             self.open()
 
         rssi = 0
 
         if rssi_threshold is not None:
@@ -217,66 +200,41 @@
 
         ret = gattlib_adapter_scan_eddystone(self._adapter, rssi, eddystone_filters,
                                              Adapter.on_discovered_ble_device_with_details,
                                              timeout, args)
         handle_return(ret)
 
     def scan_disable(self):
+        """Disable BLE scan."""
         ret = gattlib.gattlib_adapter_scan_disable(self._adapter)
         handle_return(ret)
 
     def get_rssi_from_mac(self, mac_address):
+        """
+        Return RSSI of a device defined by its MAC address.
+
+        Note: The RSSI is 0 when the device is connected.
+        """
         if isinstance(mac_address, str):
             mac_address = mac_address.encode("utf-8")
 
         rssi = c_int16(0)
         gattlib_get_rssi_from_mac(self._adapter, mac_address, byref(rssi))
         return rssi.value
 
     def gattlib_get_advertisement_data_from_mac(self, mac_address):
+        """Return advertisement and manufacturer data of the device."""
         if isinstance(mac_address, str):
             mac_address = mac_address.encode("utf-8")
 
         _advertisement_data = POINTER(GattlibAdvertisementData)()
         _advertisement_data_count = c_size_t(0)
         _manufacturer_data = POINTER(GattlibManufacturerData)()
-        _manufacturer_data_len = c_size_t(0)
+        _manufacturer_data_count = c_size_t(0)
 
         ret = gattlib_get_advertisement_data_from_mac(self._adapter, mac_address,
                                                       byref(_advertisement_data), byref(_advertisement_data_count),
-                                                      byref(_manufacturer_data), byref(_manufacturer_data_len))
+                                                      byref(_manufacturer_data), byref(_manufacturer_data_count))
         handle_return(ret)
 
-        advertisement_data = {}
-        manufacturer_data = {}
-
-        for i in range(0, _advertisement_data_count.value):
-            service_data = _advertisement_data[i]
-            uuid = gattlib_uuid_to_int(service_data.uuid)
-
-            pointer_type = POINTER(c_byte * service_data.data_length)
-            c_bytearray = cast(service_data.data, pointer_type)
-
-            data = bytearray(service_data.data_length)
-            for i in range(service_data.data_length):
-                data[i] = c_bytearray.contents[i] & 0xFF
-
-            advertisement_data[uuid] = data
-
-        for i in range(0, _manufacturer_data_len.value):
-            _manufacturer_data = _manufacturer_data[i]
-
-            pointer_type = POINTER(c_byte * _manufacturer_data.data_size.value)
-            c_bytearray = cast(_manufacturer_data.data, pointer_type)
-
-            data = bytearray(_manufacturer_data.data_size.value)
-            for j in range(_manufacturer_data.data_size.value):
-                data[j] = c_bytearray.contents[j] & 0xFF
-
-            manufacturer_data[_manufacturer_data.manufacturer_id] = data
-
-            gattlib_free_mem(_manufacturer_data.data)
-
-        gattlib_free_mem(_advertisement_data)
-        gattlib_free_mem(_manufacturer_data)
-
-        return advertisement_data, manufacturer_data
+        return convert_gattlib_advertisement_c_data_to_dict(
+            _advertisement_data, _advertisement_data_count, _manufacturer_data, _manufacturer_data_count)
```

### Comparing `gattlib-py-0.7.1/gattlib/device.py` & `gattlib-py-0.7.2/gattlib/device.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 #
 # SPDX-License-Identifier: BSD-3-Clause
 #
 # Copyright (c) 2016-2024, Olivier Martin <olivier@labapart.org>
 #
 
+"""Gattlib Device API"""
+
 from __future__ import annotations
-import logging
 import uuid
 import threading
 from typing import TYPE_CHECKING
 
-from gattlib import *
-from .exception import handle_return, DeviceError, InvalidParameter
+from gattlib import *   #pylint: disable=wildcard-import,unused-wildcard-import
+from .exception import handle_return, InvalidParameter
 from .gatt import GattService, GattCharacteristic
-from .uuid import gattlib_uuid_to_int
+from .helpers import convert_gattlib_advertisement_c_data_to_dict
 
 if TYPE_CHECKING:
     from .adapter import Adapter
 
 CONNECTION_OPTIONS_LEGACY_BDADDR_LE_PUBLIC = (1 << 0)
 CONNECTION_OPTIONS_LEGACY_BDADDR_LE_RANDOM = (1 << 1)
 CONNECTION_OPTIONS_LEGACY_BT_SEC_LOW = (1 << 2)
@@ -27,30 +28,34 @@
 CONNECTION_OPTIONS_LEGACY_DEFAULT = \
         CONNECTION_OPTIONS_LEGACY_BDADDR_LE_PUBLIC | \
         CONNECTION_OPTIONS_LEGACY_BDADDR_LE_RANDOM | \
         CONNECTION_OPTIONS_LEGACY_BT_SEC_LOW
 
 
 class Device:
-
+    """GATT device"""
     def __init__(self, adapter: Adapter, addr: str, name: str = None):
         self._adapter = adapter
-        if type(addr) == str:
+        if isinstance(addr, str):
             self._addr = addr.encode("utf-8")
         else:
             self._addr = addr
         self._name = name
         self._connection = None
         # We use a lock because on disconnection, we will set self._connection to None
         self._connection_lock = threading.Lock()
         # We use a lock on disconnection to ensure the memory is safely freed
         self._disconnection_lock = threading.Lock()
 
+        self._services: dict[int, GattService] = {}
+        self._characteristics: dict[int, GattCharacteristic] = {}
+
         self.on_connection_callback = None
         self.on_connection_error_callback = None
+        self.disconnection_callback = None
 
         # Keep track if notification handler has been initialized
         self._is_notification_init = False
 
         # Dictionnary for GATT characteristic callback
         self._gatt_characteristic_callbacks = {}
 
@@ -61,207 +66,180 @@
     @property
     def mac_address(self) -> str:
         """Return Device MAC Address"""
         return self._addr.decode("utf-8")
 
     @property
     def connection(self):
+        """Return Gattlib connection C handle."""
         if self._connection:
             return self._connection
         else:
             return c_void_p(None)
 
     @property
     def is_connected(self) -> bool:
+        """Return True if the device is connected."""
         return (self._connection is not None)
 
     def connect(self, options=CONNECTION_OPTIONS_LEGACY_DEFAULT):
+        """Connect the device."""
         def _on_connection(adapter: c_void_p, mac_address: c_char_p, connection: c_void_p, error: c_int, user_data: py_object):
             if error:
                 self._connection = None
                 self.on_connection_error(error, user_data)
             else:
                 self._connection = connection
                 self.on_connection(user_data)
 
         if self._adapter is None:
             adapter = None
         else:
-            adapter = self._adapter._adapter
+            adapter = self._adapter._adapter  #pylint: disable=protected-access
 
         ret = gattlib_connect(adapter, self._addr, options,
                               gattlib_connected_device_python_callback,
                               gattlib_python_callback_args(_on_connection, self))
         handle_return(ret)
 
     def on_connection(self, user_data: py_object):
-        if self.on_connection_callback:
-            self.on_connection_callback(self, user_data)
+        """Method called on device connection."""
+        if callable(self.on_connection_callback):
+            self.on_connection_callback(self, user_data)  #pylint: disable=not-callable
 
     def on_connection_error(self, error: c_int, user_data: py_object):
+        """Method called on device connection error."""
         logger.error("Failed to connect due to error '0x%x'", error)
-        if self.on_connection_error_callback:
-            self.on_connection_error_callback(self, error, user_data)
+        if callable(self.on_connection_error_callback):
+            self.on_connection_error_callback(self, error, user_data)  #pylint: disable=not-callable
 
     @property
     def rssi(self):
+        """Return connection RSSI."""
         _rssi = c_int16(0)
         if self._connection:
             ret = gattlib_get_rssi(self._connection, byref(_rssi))
             handle_return(ret)
             return _rssi.value
         else:
             return self._adapter.get_rssi_from_mac(self._addr)
 
     def register_on_disconnect(self, callback, user_data=None):
+        """Register disconnection callback."""
         self.disconnection_callback = callback
 
         def on_disconnection(user_data):
-            self._disconnection_lock.acquire()
-
-            if self.disconnection_callback:
-                self.disconnection_callback()
-
-            # On disconnection, we do not need the list of GATT services and GATT characteristics
-            if self._services_ptr:
-                gattlib_free_mem(self._services_ptr)
-                self._services_ptr = None
-            if self._characteristics_ptr:
-                gattlib_free_mem(self._characteristics_ptr)
-                self._characteristics_ptr = None
-
-            # Reset the connection handler
-            self._connection = None
+            with self._disconnection_lock:
+                if self.disconnection_callback:
+                    self.disconnection_callback()
+
+                # On disconnection, we do not need the list of GATT services and GATT characteristics
+                if self._services_ptr:
+                    gattlib_free_mem(self._services_ptr)
+                    self._services_ptr = None
+                if self._characteristics_ptr:
+                    gattlib_free_mem(self._characteristics_ptr)
+                    self._characteristics_ptr = None
 
-            self._disconnection_lock.release()
+                # Reset the connection handler
+                self._connection = None
 
         gattlib_register_on_disconnect(self.connection,
                                        gattlib_disconnected_device_python_callback,
                                        gattlib_python_callback_args(on_disconnection, user_data))
 
     def disconnect(self, wait_disconnection: bool = False):
-        self._connection_lock.acquire()
-        try:
+        """Disconnect connected device."""
+        with self._connection_lock:
             if self._connection:
                 ret = gattlib_disconnect(self.connection, wait_disconnection)
                 handle_return(ret)
             self._connection = None
-        finally:
-            self._connection_lock.release()
 
     def discover(self):
-        #
-        # Discover GATT Services
-        #
+        """Discover GATT Services."""
         self._services_ptr = POINTER(GattlibPrimaryService)()
-        _services_count = c_int(0)
-        ret = gattlib_discover_primary(self.connection, byref(self._services_ptr), byref(_services_count))
+        services_count = c_int(0)
+        ret = gattlib_discover_primary(self.connection, byref(self._services_ptr), byref(services_count))
         handle_return(ret)
 
         self._services = {}
-        for i in range(0, _services_count.value):
+        for i in range(0, services_count.value):
             service = GattService(self, self._services_ptr[i])
             self._services[service.short_uuid] = service
 
-            logger.debug("Service UUID:0x%x" % service.short_uuid)
+            logger.debug("Service UUID:0x%x", service.short_uuid)
 
         #
         # Discover GATT Characteristics
         #
         self._characteristics_ptr = POINTER(GattlibCharacteristic)()
         _characteristics_count = c_int(0)
         ret = gattlib_discover_char(self.connection, byref(self._characteristics_ptr), byref(_characteristics_count))
         handle_return(ret)
 
         self._characteristics = {}
         for i in range(0, _characteristics_count.value):
             characteristic = GattCharacteristic(self, self._characteristics_ptr[i])
             self._characteristics[characteristic.short_uuid] = characteristic
 
-            logger.debug("Characteristic UUID:0x%x" % characteristic.short_uuid)
+            logger.debug("Characteristic UUID:0x%x", characteristic.short_uuid)
 
     def get_advertisement_data(self):
-        _advertisement_data = POINTER(GattlibAdvertisementData)()
-        _advertisement_data_count = c_size_t(0)
-        _manufacturer_data = POINTER(GattlibManufacturerData)()
-        _manufacturer_data_len = c_size_t(0)
+        """Return advertisement and manufacturer data of the device."""
+        advertisement_data = POINTER(GattlibAdvertisementData)()
+        advertisement_data_count = c_size_t(0)
+        manufacturer_data = POINTER(GattlibManufacturerData)()
+        manufacturer_data_count = c_size_t(0)
 
         if self._connection is None:
-            ret = gattlib_get_advertisement_data_from_mac(self._adapter._adapter, self._addr,
-                                                          byref(_advertisement_data), byref(_advertisement_data_count),
-                                                          byref(_manufacturer_data), byref(_manufacturer_data_len))
+            ret = gattlib_get_advertisement_data_from_mac(self._adapter._adapter, self._addr,  #pylint: disable=protected-access
+                                                          byref(advertisement_data), byref(advertisement_data_count),
+                                                          byref(manufacturer_data), byref(manufacturer_data_count))
         else:
             ret = gattlib_get_advertisement_data(self._connection,
-                                                 byref(_advertisement_data), byref(_advertisement_data_count),
-                                                 byref(_manufacturer_data), byref(_manufacturer_data_len))
+                                                 byref(advertisement_data), byref(advertisement_data_count),
+                                                 byref(manufacturer_data), byref(manufacturer_data_count))
 
         handle_return(ret)
 
-        advertisement_data = {}
-        manufacturer_data = {}
-
-        for i in range(0, _advertisement_data_count.value):
-            service_data = _advertisement_data[i]
-            uuid = gattlib_uuid_to_int(service_data.uuid)
-
-            pointer_type = POINTER(c_byte * service_data.data_length)
-            c_bytearray = cast(service_data.data, pointer_type)
-
-            data = bytearray(service_data.data_length)
-            for i in range(service_data.data_length):
-                data[i] = c_bytearray.contents[i] & 0xFF
-
-            advertisement_data[uuid] = data
-
-        for i in range(0, _manufacturer_data_len.value):
-            _manufacturer_data = _manufacturer_data[i]
-
-            pointer_type = POINTER(c_byte * _manufacturer_data.data_size.value)
-            c_bytearray = cast(_manufacturer_data.data, pointer_type)
-
-            data = bytearray(_manufacturer_data.data_size.value)
-            for j in range(_manufacturer_data.data_size.value):
-                data[j] = c_bytearray.contents[j] & 0xFF
-
-            manufacturer_data[_manufacturer_data.manufacturer_id] = data
-
-            gattlib_free_mem(_manufacturer_data.data)
-
-        gattlib_free_mem(_advertisement_data)
-        gattlib_free_mem(_manufacturer_data)
-
-        return advertisement_data, manufacturer_data
+        return convert_gattlib_advertisement_c_data_to_dict(  #pylint: disable=protected-access
+            advertisement_data, advertisement_data_count,
+            manufacturer_data, manufacturer_data_count)
 
     @property
-    def services(self):
+    def services(self) -> dict[int, GattService]:
+        """Return a GATT Service dictionary - the GATT UUID being the key."""
         if not hasattr(self, '_services'):
             logger.warning("Start GATT discovery implicitly")
             self.discover()
 
         return self._services
 
     @property
-    def characteristics(self):
+    def characteristics(self) -> dict[int, GattCharacteristic]:
+        """Return a GATT Characteristic dictionary - the GATT UUID being the key."""
         if not hasattr(self, '_characteristics'):
             logger.warning("Start GATT discovery implicitly")
             self.discover()
 
         return self._characteristics
 
     @staticmethod
-    def notification_callback(uuid_str, data, data_len, user_data):
+    def _notification_callback(uuid_str, data, data_len, user_data):
+        """Helper method to call back characteristic callback."""
         this = user_data
 
         notification_uuid = uuid.UUID(uuid_str)
 
         short_uuid = notification_uuid.int
-        if short_uuid not in this._gatt_characteristic_callbacks:
+        if short_uuid not in this._gatt_characteristic_callbacks:  #pylint: disable=protected-access
             raise RuntimeError("UUID '%s' is expected to be part of the notification list")
-        else:
-            characteristic_callback = this._gatt_characteristic_callbacks[short_uuid]
+
+        characteristic_callback = this._gatt_characteristic_callbacks[short_uuid]  #pylint: disable=protected-access
 
         # value = bytearray(data_len)
         # for i in range(data_len):
         #    value[i] = data[i]
 
         pointer_type = POINTER(c_ubyte * data_len)
         c_bytearray = cast(data, pointer_type)
@@ -277,15 +255,15 @@
         if self._is_notification_init:
             return
 
         self._is_notification_init = True
 
         gattlib_register_notification(self._connection,
                                       gattlib_notification_device_python_callback,
-                                      gattlib_python_callback_args(Device.notification_callback, self))
+                                      gattlib_python_callback_args(Device._notification_callback, self))
 
     def _notification_add_gatt_characteristic_callback(self, gatt_characteristic, callback, user_data):
         if not callable(callback):
             raise InvalidParameter("Notification callback is not callable.")
 
         if not self._is_notification_init:
             self._notification_init()
```

### Comparing `gattlib-py-0.7.1/gattlib/exception.py` & `gattlib-py-0.7.2/gattlib/exception.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 #
 # SPDX-License-Identifier: BSD-3-Clause
 #
 # Copyright (c) 2016-2024, Olivier Martin <olivier@labapart.org>
 #
 
+"""Gattlib Exceptions"""
+
 GATTLIB_SUCCESS = 0
 GATTLIB_INVALID_PARAMETER = 1
 GATTLIB_NOT_FOUND = 2
 GATTLIB_TIMEOUT = 3
 GATTLIB_OUT_OF_MEMORY = 4
 GATTLIB_NOT_SUPPORTED = 5
 GATTLIB_DEVICE_ERROR = 6
@@ -21,96 +23,99 @@
 GATTLIB_ERROR_MODULE_MASK      = 0xF0000000
 GATTLIB_ERROR_DBUS             = 0x10000000
 GATTLIB_ERROR_BLUEZ            = 0x20000000
 GATTLIB_ERROR_INTERNAL         = 0x80000000
 
 
 class GattlibException(Exception):
-    pass
+    """Generic Gattlib exception."""
 
 class NoAdapter(GattlibException):
-    pass
+    """Gattlib exception raised when no adapter is present."""
 
 class Busy(GattlibException):
-    pass
+    """Gattlib busy exception."""
 
 class Unexpected(GattlibException):
-    pass
+    """Gattlib unexpected exception."""
 
 class AdapterNotOpened(GattlibException):
-    pass
+    """Gattlib exception raised when adapter is not opened yet."""
 
 class InvalidParameter(GattlibException):
-    pass
+    """Gattlib invalid parameter exception."""
 
 class NotFound(GattlibException):
-    pass
+    """Gattlib not found exception."""
 
 class OutOfMemory(GattlibException):
-    pass
+    """Gattlib out of memory exception."""
 
 class NotSupported(GattlibException):
-    pass
+    """Gattlib not supported exception."""
 
 class NotConnected(GattlibException):
-    pass
+    """Gattlib exception raised when device is not connected."""
 
 class AdapterClose(GattlibException):
-    pass
+    """Gattlib exception raised when the adapter is closed."""
 
 class Disconnected(GattlibException):
-    pass
+    """Gattlib exception raised when the device is disconnected."""
 
 class DeviceError(GattlibException):
+    """Gattlib device exception."""
     def __init__(self, adapter: str = None, mac_address: str = None) -> None:
         self.adapter = adapter
         self.mac_address = mac_address
 
     def __str__(self) -> str:
         return f"Error with device {self.mac_address} on adapter {self.adapter}"
 
 class DBusError(GattlibException):
+    """Gattlib DBUS exception."""
     def __init__(self, domain: int, code: int) -> None:
         self.domain = domain
         self.code = code
 
     def __str__(self) -> str:
         if self.domain == 238 and self.code == 60964:
-            return f"DBus Error: le-connection-abort-by-local"
+            return "DBus Error: le-connection-abort-by-local"
         elif self.domain == 238 and self.code == 60952:
-            return f"DBus Error: Timeout was reached"
+            return "DBus Error: Timeout was reached"
         elif self.domain == 238 and self.code == 60964:
-            return f"DBus Error: Timeout was reached"
+            return "DBus Error: Timeout was reached"
         else:
             return f"DBus Error domain={self.domain},code={self.code}"
 
 def handle_return(ret):
+    """Function to convert gattlib error to Python exception."""
     if ret == GATTLIB_INVALID_PARAMETER:
         raise InvalidParameter()
-    elif ret == GATTLIB_NOT_FOUND:
+    if ret == GATTLIB_NOT_FOUND:
         raise NotFound()
-    elif ret == GATTLIB_OUT_OF_MEMORY:
+    if ret == GATTLIB_OUT_OF_MEMORY:
         raise OutOfMemory()
-    elif ret == GATTLIB_TIMEOUT:
+    if ret == GATTLIB_TIMEOUT:
         raise TimeoutError()
-    elif ret == GATTLIB_NOT_SUPPORTED:
+    if ret == GATTLIB_NOT_SUPPORTED:
         raise NotSupported()
-    elif ret == GATTLIB_DEVICE_ERROR:
+    if ret == GATTLIB_DEVICE_ERROR:
         raise DeviceError()
-    elif ret == GATTLIB_DEVICE_NOT_CONNECTED:
+    if ret == GATTLIB_DEVICE_NOT_CONNECTED:
         raise NotConnected()
-    elif ret == GATTLIB_NO_ADAPTER:
+    if ret == GATTLIB_NO_ADAPTER:
         raise NoAdapter()
-    elif ret == GATTLIB_BUSY:
+    if ret == GATTLIB_BUSY:
         raise Busy()
-    elif ret == GATTLIB_UNEXPECTED:
+    if ret == GATTLIB_UNEXPECTED:
         raise Unexpected()
-    elif ret == GATTLIB_ADAPTER_CLOSE:
+    if ret == GATTLIB_ADAPTER_CLOSE:
         raise AdapterClose()
-    elif ret == GATTLIB_DEVICE_DISCONNECTED:
+    if ret == GATTLIB_DEVICE_DISCONNECTED:
         raise Disconnected()
-    elif (ret & GATTLIB_ERROR_MODULE_MASK) == GATTLIB_ERROR_DBUS:
+    if (ret & GATTLIB_ERROR_MODULE_MASK) == GATTLIB_ERROR_DBUS:
         raise DBusError((ret >> 8) & 0xFFF, ret & 0xFFFF)
-    elif ret == -22: # From '-EINVAL'
+    if ret == -22: # From '-EINVAL'
         raise ValueError("Gattlib value error")
-    elif ret != 0:
-        raise RuntimeError("Gattlib exception %d" % ret)
+    if ret != 0:
+        raise RuntimeError(f"Gattlib exception {ret}")
```

### Comparing `gattlib-py-0.7.1/gattlib/mainloop.py` & `gattlib-py-0.7.2/gattlib/mainloop.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 #
 # SPDX-License-Identifier: BSD-3-Clause
 #
 # Copyright (c) 2016-2024, Olivier Martin <olivier@labapart.org>
 #
 
+"""Module for exposing main loop for Gattlib execution."""
+
 import threading
 import time
 import traceback
 
 #import dbus.mainloop.glib
 from gi.repository import GObject
 
@@ -15,36 +17,41 @@
 
 gobject_mainloop: GObject.MainLoop = None
 task_returned_code: int = -1
 task_exception: Exception = None
 
 def _user_thread_main(task):
     """Main entry point for the thread that will run user's code."""
-    global gobject_mainloop, task_returned_code, task_exception
+    global task_returned_code, task_exception
 
     try:
         # Wait for GLib main loop to start running before starting user code.
         while True:
             if gobject_mainloop is not None and gobject_mainloop.is_running():
                 # Main loop is running, we should be ready to make bluez DBus calls.
                 break
             # Main loop isn't running yet, give time back to other threads.
             time.sleep(0)
 
         # Run user's code.
         task_returned_code = task()
-    except Exception as ex:
+    except Exception as ex:  #pylint: disable=broad-except
         logger.error("Exception in %s: %s: %s", task, type(ex), str(ex))
         traceback.print_exception(type(ex), ex, ex.__traceback__)
         task_exception = ex
     finally:
         gobject_mainloop.quit()
 
 def run_mainloop_with(task):
-    global gobject_mainloop, task_returned_code, task_exception
+    """
+    Run main loop with the given task.
+
+    The main loop ends when the task has completed.
+    """
+    global gobject_mainloop
 
     if gobject_mainloop:
         raise RuntimeError("A mainloop is already running")
 
     # Ensure GLib's threading is initialized to support python threads, and
     # make a default mainloop that all DBus objects will inherit.  These
     # commands MUST execute before any other DBus commands!
```

### Comparing `gattlib-py-0.7.1/gattlib/uuid.py` & `gattlib-py-0.7.2/gattlib/uuid.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,55 @@
 #
 # SPDX-License-Identifier: BSD-3-Clause
 #
 # Copyright (c) 2016-2024, Olivier Martin <olivier@labapart.org>
 #
 
+"""Module to manipulate Gattlib UUID in Python environment."""
+
 import re
 from uuid import UUID
 
-from gattlib import *
+from gattlib import *  #pylint: disable=wildcard-import,unused-wildcard-import
 
 SDP_UUID16 = 0x19
 SDP_UUID32 = 0x1A
 SDP_UUID128 = 0x1C
 
-GATT_STANDARD_UUID_FORMAT = re.compile("(\S+)-0000-1000-8000-00805f9b34fb", flags=re.IGNORECASE)
+GATT_STANDARD_UUID_FORMAT = re.compile(r"(\S+)-0000-1000-8000-00805f9b34fb", flags=re.IGNORECASE)
 
 
-def gattlib_uuid_to_uuid(gattlib_uuid):
+def gattlib_uuid_to_uuid(gattlib_uuid) -> UUID:
+    """Convert Gattlib UUID to Python UUID"""
     if gattlib_uuid.type == SDP_UUID16:
         return UUID(fields=(gattlib_uuid.value.uuid16, 0x0000, 0x1000, 0x80, 0x00, 0x00805f9b34fb))
     elif gattlib_uuid.type == SDP_UUID32:
         return UUID(fields=(gattlib_uuid.value.uuid32, 0x0000, 0x1000, 0x80, 0x00, 0x00805f9b34fb))
     elif gattlib_uuid.type == SDP_UUID128:
         data = bytes(gattlib_uuid.value.uuid128.data)
         return UUID(bytes=data)
     else:
-        return ValueError("Gattlib UUID not recognized (type:0x%x)" % gattlib_uuid.type)
+        return ValueError(f"Gattlib UUID not recognized (type:0x{gattlib_uuid.type:02x})")
 
 
-def gattlib_uuid_to_int(gattlib_uuid):
+def gattlib_uuid_to_int(gattlib_uuid) -> int:
+    """Convert Gattlib UUID to integer."""
     if gattlib_uuid.type == SDP_UUID16:
         return gattlib_uuid.value.uuid16
     elif gattlib_uuid.type == SDP_UUID32:
         return gattlib_uuid.value.uuid32
     elif gattlib_uuid.type == SDP_UUID128:
         data = bytes(gattlib_uuid.value.uuid128.data)
         return int.from_bytes(data, byteorder='big')
     else:
-        return ValueError("Gattlib UUID not recognized (type:0x%x)" % gattlib_uuid.type)
+        return ValueError(f"Gattlib UUID not recognized (type:0x{gattlib_uuid.type:02x})")
 
 
 def gattlib_uuid_str_to_int(uuid_str: str) -> int:
+    """Convert uuid string to integer"""
     # Check if the string could already encode a UUID16 or UUID32
     if len(uuid_str) <= 8:
         return int(uuid_str, 16)
 
     # Check if it is a standard UUID or not
     match = GATT_STANDARD_UUID_FORMAT.search(uuid_str)
     if match:
```

### Comparing `gattlib-py-0.7.1/gattlib_py.egg-info/PKG-INFO` & `gattlib-py-0.7.2/gattlib_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gattlib-py
-Version: 0.7.1
+Version: 0.7.2
 Summary: Python wrapper for gattlib library
 Home-page: https://github.com/labapart/gattlib/gattlib-py
 Author: Olivier Martin
 Author-email: olivier@labapart.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `gattlib-py-0.7.1/gattlib_py.egg-info/SOURCES.txt` & `gattlib-py-0.7.2/gattlib_py.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -162,14 +162,15 @@
 dbus/dbus-bluez-v5.48/org.bluez.GattService1.xml
 gattlib/__init__.py
 gattlib/_version.py
 gattlib/adapter.py
 gattlib/device.py
 gattlib/exception.py
 gattlib/gatt.py
+gattlib/helpers.py
 gattlib/mainloop.py
 gattlib/uuid.py
 gattlib_py.egg-info/PKG-INFO
 gattlib_py.egg-info/SOURCES.txt
 gattlib_py.egg-info/dependency_links.txt
 gattlib_py.egg-info/requires.txt
 gattlib_py.egg-info/top_level.txt
```

### Comparing `gattlib-py-0.7.1/include/gattlib.h` & `gattlib-py-0.7.2/include/gattlib.h`

 * *Files 0% similar despite different names*

```diff
@@ -675,16 +675,16 @@
  */
 int gattlib_get_rssi(gattlib_connection_t *connection, int16_t *rssi);
 #endif
 
 /**
  * @brief Function to retrieve RSSI from a MAC Address
  *
- * @note: This function is mainly used before a connection is established. Once the connection
- * established, the function `gattlib_get_rssi()` should be preferred.
+ * @note: This function must be used before a connection is established. Once the connection
+ * established, the function will return a null RSSI.
  *
  * @param adapter is the adapter the new device has been seen
  * @param mac_address is the MAC address of the device to get the RSSI
  * @param rssi is the Received Signal Strength Indicator of the remote device
  *
  * @return GATTLIB_SUCCESS on success or GATTLIB_* error code
  */
```

### Comparing `gattlib-py-0.7.1/setup.py` & `gattlib-py-0.7.2/setup.py`

 * *Files identical despite different names*

