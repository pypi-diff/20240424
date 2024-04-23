# Comparing `tmp/sippy-2.0.2.tar.gz` & `tmp/sippy-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sippy-2.0.2.tar", last modified: Tue Oct 18 20:29:17 2022, max compression
+gzip compressed data, was "sippy-2.1.0.tar", last modified: Tue Apr 23 22:19:21 2024, max compression
```

## Comparing `sippy-2.0.2.tar` & `sippy-2.1.0.tar`

### file list

```diff
@@ -1,129 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 20:29:16.999493 sippy-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1430 2022-10-18 20:29:05.000000 sippy-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-10-18 20:29:05.000000 sippy-2.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3396 2022-10-18 20:29:16.999493 sippy-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2939 2022-10-18 20:29:05.000000 sippy-2.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-10-18 20:29:05.000000 sippy-2.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-18 20:29:16.999493 sippy-2.0.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1171 2022-10-18 20:29:05.000000 sippy-2.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 20:29:16.991492 sippy-2.0.2/sippy/
--rw-r--r--   0 runner    (1001) docker     (121)     7858 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/B2BRoute.py
--rw-r--r--   0 runner    (1001) docker     (121)     3907 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/CCEvents.py
--rw-r--r--   0 runner    (1001) docker     (121)     9544 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/CLIManager.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 20:29:16.995492 sippy-2.0.2/sippy/Core/
--rw-r--r--   0 runner    (1001) docker     (121)    10348 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/Core/EventDispatcher.py
--rw-r--r--   0 runner    (1001) docker     (121)     3472 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/Core/Exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/Core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1585 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/ESipHeaderCSV.py
--rw-r--r--   0 runner    (1001) docker     (121)     1525 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/ESipHeaderIgnore.py
--rw-r--r--   0 runner    (1001) docker     (121)      609 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/ESipParseException.py
--rw-r--r--   0 runner    (1001) docker     (121)     6010 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/External_command.py
--rw-r--r--   0 runner    (1001) docker     (121)     1589 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/FakeAccounting.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 20:29:16.995492 sippy-2.0.2/sippy/Math/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/Math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2154 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/Math/recfilter.py
--rw-r--r--   0 runner    (1001) docker     (121)     2750 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/MsgBody.py
--rw-r--r--   0 runner    (1001) docker     (121)    12130 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/MyConfigParser.py
--rw-r--r--   0 runner    (1001) docker     (121)     8722 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/RadiusAccounting.py
--rw-r--r--   0 runner    (1001) docker     (121)     3622 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/RadiusAuthorisation.py
--rw-r--r--   0 runner    (1001) docker     (121)     4111 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/Radius_client.py
--rw-r--r--   0 runner    (1001) docker     (121)    10686 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/Rtp_proxy_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     2327 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/Rtp_proxy_client_local.py
--rw-r--r--   0 runner    (1001) docker     (121)     2087 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/Rtp_proxy_client_net.py
--rw-r--r--   0 runner    (1001) docker     (121)     8343 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/Rtp_proxy_client_stream.py
--rw-r--r--   0 runner    (1001) docker     (121)     9061 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/Rtp_proxy_client_udp.py
--rw-r--r--   0 runner    (1001) docker     (121)     8682 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/Rtp_proxy_cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)    19739 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/Rtp_proxy_session.py
--rw-r--r--   0 runner    (1001) docker     (121)    10406 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SdpBody.py
--rw-r--r--   0 runner    (1001) docker     (121)     2057 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SdpConnecton.py
--rw-r--r--   0 runner    (1001) docker     (121)     1585 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SdpGeneric.py
--rw-r--r--   0 runner    (1001) docker     (121)     2959 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SdpMedia.py
--rw-r--r--   0 runner    (1001) docker     (121)     4844 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SdpMediaDescription.py
--rw-r--r--   0 runner    (1001) docker     (121)     3345 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SdpOrigin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 20:29:16.995492 sippy-2.0.2/sippy/Security/
--rw-r--r--   0 runner    (1001) docker     (121)     5055 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/Security/SipNonce.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/Security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3672 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/Signal.py
--rw-r--r--   0 runner    (1001) docker     (121)     6331 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SipAddress.py
--rw-r--r--   0 runner    (1001) docker     (121)     3335 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SipAddressHF.py
--rw-r--r--   0 runner    (1001) docker     (121)     2246 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SipAllow.py
--rw-r--r--   0 runner    (1001) docker     (121)     1530 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SipAlso.py
--rw-r--r--   0 runner    (1001) docker     (121)     8108 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SipAuthorization.py
--rw-r--r--   0 runner    (1001) docker     (121)     1625 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SipCCDiversion.py
--rw-r--r--   0 runner    (1001) docker     (121)     2600 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SipCSeq.py
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SipCallId.py
--rw-r--r--   0 runner    (1001) docker     (121)     2820 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SipCiscoGUID.py
--rw-r--r--   0 runner    (1001) docker     (121)     2255 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SipConf.py
--rw-r--r--   0 runner    (1001) docker     (121)     2372 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SipContact.py
--rw-r--r--   0 runner    (1001) docker     (121)     1678 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SipContentLength.py
--rw-r--r--   0 runner    (1001) docker     (121)     1772 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SipContentType.py
--rw-r--r--   0 runner    (1001) docker     (121)     1617 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SipDiversion.py
--rw-r--r--   0 runner    (1001) docker     (121)     1638 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SipExpires.py
--rw-r--r--   0 runner    (1001) docker     (121)     2788 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SipFrom.py
--rw-r--r--   0 runner    (1001) docker     (121)     2007 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SipGenericHF.py
--rw-r--r--   0 runner    (1001) docker     (121)     4939 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SipHeader.py
--rw-r--r--   0 runner    (1001) docker     (121)     7704 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SipLogger.py
--rw-r--r--   0 runner    (1001) docker     (121)     1726 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SipMaxForwards.py
--rw-r--r--   0 runner    (1001) docker     (121)    11154 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SipMsg.py
--rw-r--r--   0 runner    (1001) docker     (121)     2189 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SipNumericHF.py
--rw-r--r--   0 runner    (1001) docker     (121)     1696 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SipPAssertedIdentity.py
--rw-r--r--   0 runner    (1001) docker     (121)     1758 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SipProxyAuthenticate.py
--rw-r--r--   0 runner    (1001) docker     (121)     1658 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SipProxyAuthorization.py
--rw-r--r--   0 runner    (1001) docker     (121)     2549 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SipRAck.py
--rw-r--r--   0 runner    (1001) docker     (121)     1768 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SipRSeq.py
--rw-r--r--   0 runner    (1001) docker     (121)     2871 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SipReason.py
--rw-r--r--   0 runner    (1001) docker     (121)     1782 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SipRecordRoute.py
--rw-r--r--   0 runner    (1001) docker     (121)     1541 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SipReferTo.py
--rw-r--r--   0 runner    (1001) docker     (121)     1543 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SipReferredBy.py
--rw-r--r--   0 runner    (1001) docker     (121)     5217 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SipRegistrationAgent.py
--rw-r--r--   0 runner    (1001) docker     (121)     3184 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SipReplaces.py
--rw-r--r--   0 runner    (1001) docker     (121)     7625 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SipRequest.py
--rw-r--r--   0 runner    (1001) docker     (121)     3496 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SipResponse.py
--rw-r--r--   0 runner    (1001) docker     (121)     1769 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SipRoute.py
--rw-r--r--   0 runner    (1001) docker     (121)     1991 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SipServer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2283 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SipSupported.py
--rw-r--r--   0 runner    (1001) docker     (121)     1653 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SipTo.py
--rw-r--r--   0 runner    (1001) docker     (121)    31145 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SipTransactionManager.py
--rw-r--r--   0 runner    (1001) docker     (121)    12172 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SipURL.py
--rw-r--r--   0 runner    (1001) docker     (121)     1610 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SipUserAgent.py
--rw-r--r--   0 runner    (1001) docker     (121)     5883 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SipVia.py
--rw-r--r--   0 runner    (1001) docker     (121)     6227 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SipWWWAuthenticate.py
--rw-r--r--   0 runner    (1001) docker     (121)     2487 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/SipWarning.py
--rw-r--r--   0 runner    (1001) docker     (121)     2229 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/StatefulProxy.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 20:29:16.995492 sippy-2.0.2/sippy/Time/
--rw-r--r--   0 runner    (1001) docker     (121)     7750 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/Time/MonoTime.py
--rw-r--r--   0 runner    (1001) docker     (121)     4136 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/Time/Timeout.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/Time/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4703 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/Time/clock_dtime.py
--rw-r--r--   0 runner    (1001) docker     (121)    15672 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/UA.py
--rw-r--r--   0 runner    (1001) docker     (121)    15147 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/UaStateConnected.py
--rw-r--r--   0 runner    (1001) docker     (121)     2232 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/UaStateDead.py
--rw-r--r--   0 runner    (1001) docker     (121)     2411 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/UaStateDisconnected.py
--rw-r--r--   0 runner    (1001) docker     (121)     1993 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/UaStateFailed.py
--rw-r--r--   0 runner    (1001) docker     (121)     1909 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/UaStateGeneric.py
--rw-r--r--   0 runner    (1001) docker     (121)     5136 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/UacStateCancelling.py
--rw-r--r--   0 runner    (1001) docker     (121)     5887 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/UacStateIdle.py
--rw-r--r--   0 runner    (1001) docker     (121)     8647 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/UacStateRinging.py
--rw-r--r--   0 runner    (1001) docker     (121)    10493 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/UacStateTrying.py
--rw-r--r--   0 runner    (1001) docker     (121)     6787 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/UacStateUpdating.py
--rw-r--r--   0 runner    (1001) docker     (121)     5777 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/UasStateIdle.py
--rw-r--r--   0 runner    (1001) docker     (121)     7710 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/UasStateRinging.py
--rw-r--r--   0 runner    (1001) docker     (121)     7755 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/UasStateTrying.py
--rw-r--r--   0 runner    (1001) docker     (121)     7114 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/UasStateUpdating.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    13771 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/Udp_server.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     9603 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/XMPP_server.py
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    35563 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/b2bua_radius.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5528 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/b2bua_simple.py
--rw-r--r--   0 runner    (1001) docker     (121)     9247 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/dictionary
--rw-r--r--   0 runner    (1001) docker     (121)     2545 2022-10-18 20:29:05.000000 sippy-2.0.2/sippy/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 20:29:16.995492 sippy-2.0.2/sippy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3396 2022-10-18 20:29:16.000000 sippy-2.0.2/sippy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2665 2022-10-18 20:29:16.000000 sippy-2.0.2/sippy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-18 20:29:16.000000 sippy-2.0.2/sippy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-10-18 20:29:16.000000 sippy-2.0.2/sippy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-10-18 20:29:16.000000 sippy-2.0.2/sippy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-10-18 20:29:16.000000 sippy-2.0.2/sippy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 20:29:16.995492 sippy-2.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-18 20:29:05.000000 sippy-2.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2816 2022-10-18 20:29:05.000000 sippy-2.0.2/tests/test_SdbBody.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:19:21.865348 sippy-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-23 22:19:14.000000 sippy-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-23 22:19:14.000000 sippy-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-23 22:19:21.865348 sippy-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-04-23 22:19:14.000000 sippy-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-23 22:19:14.000000 sippy-2.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 22:19:21.865348 sippy-2.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1170 2024-04-23 22:19:14.000000 sippy-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:19:21.861348 sippy-2.1.0/sippy/
+-rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/B2BRoute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/CCEvents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9642 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/CLIManager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:19:21.865348 sippy-2.1.0/sippy/Core/
+-rw-r--r--   0 runner    (1001) docker     (127)    10378 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/Core/EventDispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/Core/Exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/Core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/ESipHeaderCSV.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/ESipHeaderIgnore.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:19:21.865348 sippy-2.1.0/sippy/Exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/Exceptions/RtpProxyError.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/Exceptions/SipParseError.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/Exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6010 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/External_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/FakeAccounting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:19:21.865348 sippy-2.1.0/sippy/Math/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/Math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/Math/recfilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/MsgBody.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/MultipartMixBody.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12130 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/MyConfigParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8722 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/RadiusAccounting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/RadiusAuthorisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/Radius_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10676 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/Rtp_proxy_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/Rtp_proxy_client_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/Rtp_proxy_client_net.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8353 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/Rtp_proxy_client_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9061 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/Rtp_proxy_client_udp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8727 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/Rtp_proxy_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23877 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/Rtp_proxy_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10420 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SdpBody.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SdpConnecton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SdpGeneric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SdpMedia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SdpMediaDescription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SdpOrigin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:19:21.865348 sippy-2.1.0/sippy/Security/
+-rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/Security/SipNonce.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/Security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/Signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipAddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipAddressHF.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipAllow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipAlso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8108 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipAuthorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipCCDiversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipCSeq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipCallId.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipCiscoGUID.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipConf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipContact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipContentLength.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipContentType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipDiversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipExpires.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipFrom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipGenericHF.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7704 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipLogger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipMaxForwards.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11132 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipMsg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipNumericHF.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipPAssertedIdentity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipProxyAuthenticate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipProxyAuthorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipRAck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipRSeq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipReason.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipRecordRoute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipReferTo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipReferredBy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipRegistrationAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipReplaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7621 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipRoute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipServer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipSupported.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipTo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31731 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipTransactionManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12172 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipURL.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipUserAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipVia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6257 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipWWWAuthenticate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/SipWarning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/StatefulProxy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:19:21.865348 sippy-2.1.0/sippy/Time/
+-rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/Time/MonoTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/Time/Timeout.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/Time/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/Time/clock_dtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15766 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/UA.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15198 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/UaStateConnected.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/UaStateDead.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/UaStateDisconnected.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/UaStateFailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/UaStateGeneric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/UacStateCancelling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/UacStateIdle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8670 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/UacStateRinging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10516 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/UacStateTrying.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/UacStateUpdating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5804 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/UasStateIdle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7729 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/UasStateRinging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7774 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/UasStateTrying.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7133 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/UasStateUpdating.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14425 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/Udp_server.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9603 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/XMPP_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    35567 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/b2bua_radius.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5527 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/b2bua_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9247 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/dictionary
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-23 22:19:14.000000 sippy-2.1.0/sippy/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:19:21.865348 sippy-2.1.0/sippy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-23 22:19:21.000000 sippy-2.1.0/sippy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-23 22:19:21.000000 sippy-2.1.0/sippy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 22:19:21.000000 sippy-2.1.0/sippy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-23 22:19:21.000000 sippy-2.1.0/sippy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-23 22:19:21.000000 sippy-2.1.0/sippy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-23 22:19:21.000000 sippy-2.1.0/sippy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:19:21.865348 sippy-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 22:19:14.000000 sippy-2.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-04-23 22:19:14.000000 sippy-2.1.0/tests/test_SdbBody.py
```

### Comparing `sippy-2.0.2/LICENSE` & `sippy-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/PKG-INFO` & `sippy-2.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: sippy
-Version: 2.0.2
+Version: 2.1.0
 Summary: RFC3261 SIP Stack and Back-to-Back User Agent (B2BUA)
 Home-page: http://www.b2bua.org/
 Author: Sippy Software, Inc.
 Author-email: sobomax@sippysoft.com
 License: BSD
 Keywords: sip,b2bua,voip,rfc3261,sippy
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: ElPeriodic>=1.1
+Requires-Dist: pycryptodome
 
 [![Build Status@GitHub](https://github.com/sippy/b2bua/workflows/Check%20Python%20Wheels/badge.svg?branch=master)](https://github.com/sippy/b2bua/actions?query=branch%3Amaster++)
 
 # Sippy B2BUA
 
 Sippy B2BUA is a [RFC3261](https://www.ietf.org/rfc/rfc3261.txt)-compliant
 Session Initiation Protocol (SIP) stack and
@@ -47,19 +49,19 @@
 - Simple and clean, yet flexible, internal design making implementing new
   features and services easy
 - Sippy B2BUA could be easily combined with other Open Source software, such as
   SIP Express Router / OpenSIPS to build complete softswitch solution
 
 ## Installation
 
-### Install libelperiodic (if not installed)
+### Install latest stable version
 
-`pip install ElPeriodic`
+`pip install sippy`
 
-### Install B2BUA
+### Install latest development version
 
 `pip install git+https://github.com/sippy/b2bua`
 
 ## Running
 
 To get started, you can use the b2bua_simple implementation. The following
 example will cause the b2bua run in the foreground so you can see the SIP
```

### Comparing `sippy-2.0.2/README.md` & `sippy-2.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 - Simple and clean, yet flexible, internal design making implementing new
   features and services easy
 - Sippy B2BUA could be easily combined with other Open Source software, such as
   SIP Express Router / OpenSIPS to build complete softswitch solution
 
 ## Installation
 
-### Install libelperiodic (if not installed)
+### Install latest stable version
 
-`pip install ElPeriodic`
+`pip install sippy`
 
-### Install B2BUA
+### Install latest development version
 
 `pip install git+https://github.com/sippy/b2bua`
 
 ## Running
 
 To get started, you can use the b2bua_simple implementation. The following
 example will cause the b2bua run in the foreground so you can see the SIP
```

### Comparing `sippy-2.0.2/setup.py` & `sippy-2.1.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-#!/usr/bin/env python2
+#!/usr/bin/env python
 from setuptools import setup, find_packages
 
 requirements = [x.strip() for x in open("requirements.txt", "r").readlines()]
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name = "sippy",
-    version = "2.0.2",
+    version = "2.1.0",
     packages = find_packages(),
 
     install_requires = requirements,
     package_data = {
         '': ['dictionary', '*.md']
         },
     test_suite = 'tests',
```

### Comparing `sippy-2.0.2/sippy/B2BRoute.py` & `sippy-2.1.0/sippy/B2BRoute.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/CCEvents.py` & `sippy-2.1.0/sippy/CCEvents.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/CLIManager.py` & `sippy-2.1.0/sippy/CLIManager.py`

 * *Files 0% similar despite different names*

```diff
@@ -249,26 +249,30 @@
         try:
             self.command_cb(self, cmd)
         except:
             dump_exception('CLIManager: unhandled exception when processing incoming data')
             self.close()
 
     def send(self, data):
+        if self.wthr is None:
+            return
         if not isinstance(data, _uobj):
             data = data.encode('ascii')
         self.wthr.send(data)
 
     def write(self, data):
         return self.send(data)
 
     def close(self):
+        if self.wthr is None:
+            return
         self.wthr.shutdown(soft = True)
 
     def shutdown(self):
-        if self.wthr == None:
+        if self.wthr is None:
             return
         self.wthr.shutdown()
         try:
             self.clientsock.shutdown(socket.SHUT_RDWR)
         except Exception as e:
             if not isinstance(e, socket.error) or e.errno != ENOTCONN:
                 dump_exception('self.clientsock.shutdown(socket.SHUT_RDWR)')
```

### Comparing `sippy-2.0.2/sippy/Core/EventDispatcher.py` & `sippy-2.1.0/sippy/Core/EventDispatcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,23 +22,21 @@
 # LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
 # ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from __future__ import print_function
 
+from functools import partial
 from datetime import datetime
 from heapq import heappush, heappop, heapify
 from threading import Lock
 from random import random
 import sys, traceback, signal
-if sys.version_info[0] < 3:
-    from thread import get_ident
-else:
-    from _thread import get_ident
+from _thread import get_ident
 from sippy.Time.MonoTime import MonoTime
 from sippy.Core.Exceptions import dump_exception, StdException
 
 from elperiodic.ElPeriodic import ElPeriodic
 
 class EventListener(object):
     etime = None
@@ -63,15 +61,16 @@
         self.cb_func = None
         self.cb_params = None
         self.cb_kw_args = None
         self.ed = None
         self.randomize_runs = None
 
     def get_randomizer(self, p):
-        return lambda x: x * (1.0 + p * (1.0 - 2.0 * random()))
+        def randomizer(p, x): return x * (1.0 + p * (1.0 - 2.0 * random()))
+        return partial(randomizer, p)
 
     def spread_runs(self, p):
         self.randomize_runs = self.get_randomizer(p)
 
     def go(self):
         if self.ed.my_ident != get_ident():
             print(datetime.now(), 'EventDispatcher2: Timer.go() from wrong thread, expect Bad Stuff[tm] to happen')
@@ -115,14 +114,15 @@
     def __sinit__(self, *args, **kwds):
         pass
 
 class EventDispatcher2(Singleton):
     tlisteners = None
     slisteners = None
     endloop = False
+    el_rval = None
     signals_pending = None
     twasted = 0
     tcbs_lock = None
     last_ts = None
     my_ident = None
     state_lock = Lock()
     ed_inum = 0
@@ -261,33 +261,33 @@
         self.endloop = False
         self.last_ts = MonoTime()
         if timeout != None:
             etime = self.last_ts.getOffsetCopy(timeout)
         while True:
             if len(self.signals_pending) > 0:
                 self.dispatchSignals()
-                if self.endloop:
-                    return
             if self.endloop:
-                return
+                break
             self.dispatchTimers()
             if self.endloop:
-                return
+                break
             if self.twasted * 2 > len(self.tlisteners):
                 # Clean-up removed timers when their share becomes more than 50%
                 self.tlisteners = [x for x in self.tlisteners if x.cb_func != None]
                 heapify(self.tlisteners)
                 self.twasted = 0
             if (timeout != None and self.last_ts > etime) or self.endloop:
                 self.endloop = False
                 break
             self.elp.procrastinate()
             self.last_ts = MonoTime()
+        return self.el_rval
 
-    def breakLoop(self):
+    def breakLoop(self, rval=0):
         self.endloop = True
+        self.el_rval = rval
         #print('breakLoop')
         #import traceback
         #import sys
         #traceback.print_stack(file = sys.stdout)
 
 ED2 = EventDispatcher2()
```

### Comparing `sippy-2.0.2/sippy/Core/Exceptions.py` & `sippy-2.1.0/sippy/Core/Exceptions.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/ESipHeaderCSV.py` & `sippy-2.1.0/sippy/ESipHeaderCSV.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/ESipHeaderIgnore.py` & `sippy-2.1.0/sippy/ESipHeaderIgnore.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/External_command.py` & `sippy-2.1.0/sippy/External_command.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/FakeAccounting.py` & `sippy-2.1.0/sippy/FakeAccounting.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/Math/recfilter.py` & `sippy-2.1.0/sippy/Math/recfilter.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/MsgBody.py` & `sippy-2.1.0/sippy/MsgBody.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,55 +22,64 @@
 # (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 # LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
 # ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from sippy.SdpBody import SdpBody
-
-b_types = {'application/sdp':SdpBody}
+from sippy.SipContentType import SipContentType
 
 try:
     # Python < 3
     str_types = (str, unicode)
 except NameError:
     str_types = (str,)
 
+DEFAULT_CTYPE = SipContentType('application/sdp')
+DEFAULT_CTYPE.parse()
+
 class MsgBody(object):
     content = None
     mtype = None
     needs_update = True
     parsed = False
 
-    def __init__(self, content = None, mtype = 'application/sdp', cself = None):
+    def __init__(self, content = None, mtype = DEFAULT_CTYPE, cself = None):
         if content != None:
             self.mtype = mtype
             self.content = content
-        else:
+            return
+        if cself is not None:
             if type(cself.content) in str_types:
                 self.content = cself.content
             else:
                 self.content = cself.content.getCopy()
-            self.mtype = cself.mtype
+            self.mtype = cself.mtype.getCopy()
             self.parsed = True
 
     def parse(self):
+        b_types = {'application/sdp':SdpBody,
+                   'multipart/mixed':MultipartMixBody}
         if not self.parsed:
-            if self.mtype in b_types:
-                self.content = b_types[self.mtype](self.content)
+            mtype = self.getType()
+            if mtype in b_types:
+                self.content = b_types[mtype](self.content, ctype=self.mtype)
             self.parsed = True
 
     def __str__(self):
         return str(self.content)
 
     def localStr(self, local_addr = None, local_port = None):
         if type(self.content) in str_types:
             return self.content
         return self.content.localStr(local_addr, local_port)
 
     def getType(self):
-        return self.mtype
+        return self.mtype.name.lower()
 
     def getCopy(self):
         if not self.parsed:
             return MsgBody(self.content)
         return MsgBody(cself = self)
+
+if not 'MultipartMixBody' in globals():
+    from sippy.MultipartMixBody import MultipartMixBody
```

### Comparing `sippy-2.0.2/sippy/MyConfigParser.py` & `sippy-2.1.0/sippy/MyConfigParser.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/RadiusAccounting.py` & `sippy-2.1.0/sippy/RadiusAccounting.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/RadiusAuthorisation.py` & `sippy-2.1.0/sippy/RadiusAuthorisation.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/Radius_client.py` & `sippy-2.1.0/sippy/Radius_client.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/Rtp_proxy_client.py` & `sippy-2.1.0/sippy/Rtp_proxy_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,15 +223,15 @@
         to.go()
 
     def go_online(self):
         if self.shut_down:
             return
         if not self.online:
             if not self.caps_done:
-                rtpp_cc = Rtpp_caps_checker(self)
+                Rtpp_caps_checker(self)
                 return
             self.online = True
             self.heartbeat()
 
     def go_offline(self):
         if self.shut_down:
             return
```

### Comparing `sippy-2.0.2/sippy/Rtp_proxy_client_local.py` & `sippy-2.1.0/sippy/Rtp_proxy_client_local.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/Rtp_proxy_client_net.py` & `sippy-2.1.0/sippy/Rtp_proxy_client_net.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/Rtp_proxy_client_stream.py` & `sippy-2.1.0/sippy/Rtp_proxy_client_stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,44 +58,45 @@
         else:
             address = self.userv.address
         self.s.connect(address)
 
     def send_raw(self, command, _recurse = 0, stime = None):
         if _recurse > _MAX_RECURSE:
             raise Exception('Cannot reconnect: %s' % (str(self.userv.address),))
+        _recurse += 1
         if self.s == None:
             self.connect()
         #print('%s.send_raw(%s)' % (id(self), command))
         if stime == None:
             stime = MonoTime()
         while True:
             try:
                 self.s.send(command.encode())
                 break
             except socket.error as why:
                 if why.errno == EINTR:
                     continue
                 elif why.errno in (EPIPE, ENOTCONN, ECONNRESET):
                     self.s = None
-                    return self.send_raw(command, _recurse + 1, stime)
+                    return self.send_raw(command, _recurse, stime)
                 raise why
         while True:
             try:
                 rval = self.s.recv(1024)
                 if len(rval) == 0:
                     self.s = None
-                    return self.send_raw(command, _MAX_RECURSE, stime)
+                    return self.send_raw(command, _recurse, stime)
                 rval = rval.decode().strip()
                 break
             except socket.error as why:
                 if why.errno == EINTR:
                     continue
                 elif why.errno in (EPIPE, ENOTCONN, ECONNRESET):
                     self.s = None
-                    return self.send_raw(command, _recurse + 1, stime)
+                    return self.send_raw(command, _recurse, stime)
                 raise why
         rtpc_delay = stime.offsetFromNow()
         return (rval, rtpc_delay)
 
     def run(self):
         #print(self.run, 'enter')
         while True:
```

### Comparing `sippy-2.0.2/sippy/Rtp_proxy_client_udp.py` & `sippy-2.1.0/sippy/Rtp_proxy_client_udp.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/Rtp_proxy_cmd.py` & `sippy-2.1.0/sippy/Rtp_proxy_cmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,30 +59,30 @@
         self.otherparams = ''
         while len(s) > 0:
             if s[0] == 'R':
                 val, s = extract_to_next_token(s[1:], ('1', '2', '3', '4', '5', '6', '7', '8', '9', '0', '.'))
                 val = val.strip()
                 if len(val) > 0:
                     self.destination_ip = val
-            if s[0] == 'L':
+            elif s[0] == 'L':
                 val, s = extract_to_next_token(s[1:], ('1', '2', '3', '4', '5', '6', '7', '8', '9', '0', '.'))
                 val = val.strip()
                 if len(val) > 0:
                     self.local_ip = val
             elif s[0] == 'c':
                 val, s = extract_to_next_token(s[1:], ('1', '2', '3', '4', '5', '6', '7', '8', '9', '0', ','))
                 val = val.strip()
                 if len(val) > 0:
                     self.codecs = [int(x) for x in val.split(',')]
             else:
                 val, s = extract_to_next_token(s, ('c', 'R'), True)
                 if len(val) > 0:
                     self.otherparams += val
 
-    def getstr(self, call_id, swaptags = False):
+    def getstr(self, call_id, swaptags = False, skipnotify = False):
         s = ''
         if self.destination_ip != None:
             s += 'R%s' % (self.destination_ip,)
         if self.local_ip != None:
             s += 'L%s' % (self.local_ip,)
         if self.codecs != None:
             s += 'c'
@@ -98,22 +98,23 @@
             s = '%s %s' % (s, self.remote_port)
         if not swaptags:
             from_tag, to_tag = (self.from_tag, self.to_tag)
         else:
             if self.to_tag == None:
                 raise Exception('UpdateLookupOpts::getstr(swaptags = True): to_tag is not set')
             to_tag, from_tag = (self.from_tag, self.to_tag)
-        if self.from_tag != None:
-            s = '%s %s' % (s, self.from_tag)
-        if self.to_tag != None:
-            s = '%s %s' % (s, self.to_tag)
-        if self.notify_socket != None:
-            s = '%s %s' % (s, self.notify_socket)
-        if self.notify_tag != None:
-            s = '%s %s' % (s, self.notify_tag)
+        if from_tag != None:
+            s = '%s %s' % (s, from_tag)
+        if to_tag != None:
+            s = '%s %s' % (s, to_tag)
+        if not skipnotify:
+            if self.notify_socket != None:
+                s = '%s %s' % (s, self.notify_socket)
+            if self.notify_tag != None:
+                s = '%s %s' % (s, self.notify_tag)
         if self.subargs != None:
             s = '%s && %s' % (s, self.subargs)
         return s
 
 class Rtp_proxy_cmd(object):
     type = None
     ul_opts = None
```

### Comparing `sippy-2.0.2/sippy/Rtp_proxy_session.py` & `sippy-2.1.0/sippy/Rtp_proxy_session.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,14 +33,16 @@
     from _thread import get_ident
 except ImportError:
     from thread import get_ident
 import sys
 
 from sippy.Core.Exceptions import dump_exception
 from sippy.Core.EventDispatcher import ED2
+from sippy.Exceptions.RtpProxyError import RtpProxyError
+from sippy.Exceptions.SipParseError import SdpParseError
 
 try:
     strtypes = (str, unicode)
 except NameError:
     strtypes = (str,)
 
 class Rtp_proxy_cmd_sequencer(object):
@@ -77,128 +79,169 @@
     def delete(self):
         if self.inflight is not None:
             self.deleted = True
             return
         # break the reference loop
         self.rtp_proxy_client = None
 
-class _rtpps_callback_params(object):
-    proxy_address = None
-    callback_parameters = None
-    atype = None
-    remote_ip = None
-
-    def __init__(self, proxy_address, callback_parameters, atype):
-        self.proxy_address = proxy_address
-        self.callback_parameters = callback_parameters
-        self.atype = atype
+class update_params():
+    rtpps = None
+    remote_ip = '0.0.0.0'
+    remote_port = 0
+    result_callback = None
+    options = ''
+    index = 0
+    atype = 'IP4'
+    callback_parameters = ()
+    subcommands = None
+
+    def __init__(self):
+        self.subcommands = []
+
+class update_result():
+    rtpproxy_address = None
+    rtpproxy_port = None
+    family = None
+    sendonly = None
+    dtls_mode = None
+    dtls_fingerprint = None
+
+DTLS_TRANSPORTS = ('UDP/TLS/RTP/SAVP', 'UDP/TLS/RTP/SAVPF')
+DTLS_ATTRS = ('setup', 'fingerprint', 'rtcp', 'ssrc')
+DTLS_ATTRS_RM = tuple([a for a in DTLS_ATTRS if a != 'ssrc'])
 
 class _rtpps_side(object):
     session_exists = False
     codecs = None
     raddress = None
     laddress = None
     origin = None
     oh_remote = None
     repacketize = None
+    gateway_dtls = 'pass'
     soft_repacketize = False
+    after_sdp_change = None
+    needs_new_port = False
+    transports = None
+    rinfo_hst = None
 
-    def __init__(self):
+    def __init__(self, name):
         self.origin = SdpOrigin()
+        self.name = name
+        self.transports = {}
+        self.rinfo_hst = []
+
+    def __str__(self):
+        return f'_rtpps_side("name={self.name},transports={self.transports}")'
 
-    def update(self, rtpps, remote_ip, remote_port, result_callback, options = '', index = 0, \
-      atype = 'IP4', *callback_parameters):
+    def update(self, up):
         command = 'U'
-        rtpps.max_index = max(rtpps.max_index, index)
-        rtpc = rtpps.rtp_proxy_client
-        rtpq = rtpps.rtpp_seq
+        up.rtpps.max_index = max(up.rtpps.max_index, up.index)
+        rtpc = up.rtpps.rtp_proxy_client
+        rtpq = up.rtpps.rtpp_seq
+        options = up.options
         if rtpc.sbind_supported:
             if self.raddress != None:
-                #if rtpc.is_local and atype == 'IP4':
-                #    options += 'L%s' % rtpps.global_config['_sip_tm'].l4r.getServer( \
+                #if rtpc.is_local and up.atype == 'IP4':
+                #    options += 'L%s' % up.rtpps.global_config['_sip_tm'].l4r.getServer( \
                 #      self.raddress).uopts.laddress[0]
                 #elif not rtpc.is_local:
                 options += 'R%s' % self.raddress[0]
             elif self.laddress != None and rtpc.is_local:
                 options += 'L%s' % self.laddress
+        otherside = self.getother(up.rtpps)
+        if otherside.needs_new_port:
+            options += 'N'
+            otherside.needs_new_port = False
         command += options
-        from_tag, to_tag = self.gettags(rtpps)
-        otherside = self.getother(rtpps)
+        from_tag, to_tag = self.gettags(up.rtpps)
         if otherside.session_exists:
-            command += ' %s %s %d %s %s' % ('%s-%d' % (rtpps.call_id, index), remote_ip, remote_port, from_tag, to_tag)
+            command += ' %s %s %d %s %s' % ('%s-%d' % (up.rtpps.call_id, up.index), up.remote_ip, up.remote_port, from_tag, to_tag)
         else:
-            command += ' %s %s %d %s' % ('%s-%d' % (rtpps.call_id, index), remote_ip, remote_port, from_tag)
-        if rtpps.notify_socket != None and index == 0 and \
+            command += ' %s %s %d %s' % ('%s-%d' % (up.rtpps.call_id, up.index), up.remote_ip, up.remote_port, from_tag)
+        if up.rtpps.notify_socket != None and up.index == 0 and \
           rtpc.tnot_supported:
-            command += ' %s %s' % (rtpps.notify_socket, rtpps.notify_tag)
-        cpo = _rtpps_callback_params(rtpc.proxy_address, callback_parameters, atype)
-        cpo.remote_ip = remote_ip
-        rtpq.send_command(command, self.update_result, (rtpps, result_callback, cpo))
+            command += ' %s %s' % (up.rtpps.notify_socket, up.rtpps.notify_tag)
+        if len(up.subcommands) > 0:
+            command = ' && '.join([command,] + up.subcommands)
+        rtpq.send_command(command, self.update_result, up)
 
     def gettags(self, rtpps):
         if self not in (rtpps.caller, rtpps.callee):
-            raise Exception("Corrupt Rtp_proxy_session")
+            raise AssertionError("Corrupt Rtp_proxy_session")
         if self == rtpps.caller:
             return (rtpps.from_tag, rtpps.to_tag)
         else:
             return (rtpps.to_tag, rtpps.from_tag)
 
     def getother(self, rtpps):
         if self not in (rtpps.caller, rtpps.callee):
-            raise Exception("Corrupt Rtp_proxy_session")
+            raise AssertionError("Corrupt Rtp_proxy_session")
         if self == rtpps.caller:
             return rtpps.callee
         else:
             return rtpps.caller
 
-    def update_result(self, result, args):
-        #print '%s.update_result(%s)' % (id(self), result)
-        rtpps, result_callback, cpo = args
+    def update_result(self, result, up):
+        #print('%s.update_result(%s)' % (id(self), result))
         self.session_exists = True
         if result == None:
-            result_callback(None, rtpps, *cpo.callback_parameters)
+            up.result_callback(None, up.rtpps, *up.callback_parameters)
             return
-        t1 = result.split()
+        t0 = result.split('&&', 1)
+        t1 = t0[0].split()
         if t1[0][0] == 'E':
-            result_callback(None, rtpps, *cpo.callback_parameters)
+            up.result_callback(None, up.rtpps, *up.callback_parameters)
             return
-        rtpproxy_port = int(t1[0])
-        if rtpproxy_port == 0:
-            result_callback(None, rtpps, *cpo.callback_parameters)
+        ur = update_result()
+        if len(t0) > 1:
+            subc_res = t0[1].lstrip()
+            if subc_res == '-1':
+                up.result_callback(None, up.rtpps, *up.callback_parameters)
+                return
+            ur.dtls_mode, ur.dtls_fingerprint = subc_res.split(' ', 1)
+        ur.rtpproxy_port = int(t1[0])
+        if ur.rtpproxy_port == 0:
+            up.result_callback(None, up.rtpps, *up.callback_parameters)
             return
-        family = 'IP4'
+        ur.family = 'IP4'
         if len(t1) > 1:
-            rtpproxy_address = t1[1]
+            ur.rtpproxy_address = t1[1]
             if len(t1) > 2 and t1[2] == '6':
-                family = 'IP6'
+                ur.family = 'IP6'
         else:
-            rtpproxy_address = cpo.proxy_address
+            ur.rtpproxy_address = up.rtpps.rtp_proxy_client.proxy_address
         # Old-style request to put session on hold, convert it into
         # a new-style request.
-        if cpo.atype == 'IP4' and cpo.remote_ip == '0.0.0.0':
-            sendonly = True
-        elif cpo.atype == 'IP6' and cpo.remote_ip == '::':
-            sendonly = True
-        else:
-            sendonly = False
-        cb_args = (rtpproxy_address, rtpproxy_port, family, sendonly)
-        result_callback(cb_args, rtpps, *cpo.callback_parameters)
+        if up.atype == 'IP4' and up.remote_ip == '0.0.0.0':
+            ur.sendonly = True
+        elif up.atype == 'IP6' and up.remote_ip == '::':
+            ur.sendonly = True
+        else:
+            ur.sendonly = False
+        self.rinfo_hst.append(ur)
+        up.result_callback(ur, up.rtpps, *up.callback_parameters)
 
     def __play(self, result, rtpps, prompt_name, times, result_callback, index):
         from_tag, to_tag = self.gettags(rtpps)
         command = 'P%d %s %s %s %s %s' % (times, '%s-%d' % (rtpps.call_id, index), prompt_name, self.codecs, from_tag, to_tag)
         rtpps.rtpp_seq.send_command(command, rtpps.command_result, result_callback)
 
     def _play(self, rtpps, prompt_name, times = 1, result_callback = None, index = 0):
         if not self.session_exists:
             ED2.callFromThread(rtpps.command_result, None, result_callback)
             return
         otherside = self.getother(rtpps)
         if not otherside.session_exists:
-            otherside.update(rtpps, '0.0.0.0', 0, self.__play, '', index, 'IP4', prompt_name, times, result_callback, index)
+            up = update_params()
+            up.rtpps = rtpps
+            up.index = index
+            up.result_callback = self.__play
+            up.callback_parameters = (prompt_name, times, result_callback, index)
+            otherside.update(up)
             return
         self.__play(None, rtpps, prompt_name, times, result_callback, index)
 
     def _stop_play(self, rtpps, result_callback = None, index = 0):
         if not self.session_exists:
             ED2.callFromThread(rtpps.command_result, None, result_callback)
             return
@@ -207,72 +250,120 @@
         rtpps.rtpp_seq.send_command(command, rtpps.command_result, result_callback)
 
     def _on_sdp_change(self, rtpps, sdp_body, result_callback, en_excpt):
         sects = []
         try:
             sdp_body.parse()
         except Exception as exception:
-            dump_exception('can\'t parse SDP body', extra = sdp_body.content)
-            if en_excpt:
+            is_spe = isinstance(exception, SdpParseError)
+            if not is_spe:
+                dump_exception('can\'t parse SDP body', extra = sdp_body.content)
+            if is_spe or en_excpt:
                 raise exception
             else:
                 return
         if isinstance(sdp_body.content, strtypes):
             sdp_body.needs_update = False
             result_callback(sdp_body)
             return
-        for i in range(0, len(sdp_body.content.sections)):
-            sect = sdp_body.content.sections[i]
-            if sect.m_header.transport.lower() not in ('udp', 'udptl', 'rtp/avp', \
-              'rtp/savp', 'udp/bfcp'):
+        for i, sect in enumerate(sdp_body.content.sections):
+            if sect.m_header.transport.lower() not in rtpps.SUPPORTED_TRTYPES:
                 continue
             sects.append(sect)
         if len(sects) == 0:
             sdp_body.needs_update = False
             result_callback(sdp_body)
             return
         formats = sects[0].m_header.formats
         self.codecs = ','.join([ str(x) for x in formats ])
         if self.repacketize is not None and not self.soft_repacketize:
             options = 'z%d' % self.repacketize
         else:
             options = ''
-        for sect in sects:
+        otherside = self.getother(rtpps)
+        for si, sect in enumerate(sects):
+            self.transports[si] = sect.m_header.transport
             if sect.c_header.atype == 'IP6':
                 sect_options = '6' + options
             else:
                 sect_options = options
-            self.update(rtpps, sect.c_header.addr, sect.m_header.port, self._sdp_change_finish, sect_options, \
-              sects.index(sect), sect.c_header.atype, sdp_body, sect, sects, result_callback)
+            up = update_params()
+            up.rtpps = rtpps
+            up.remote_ip = sect.c_header.addr
+            up.remote_port = sect.m_header.port
+            up.atype = sect.c_header.atype
+            up.options = sect_options
+            up.index = si
+            up.result_callback = self._sdp_change_finish
+            if otherside.gateway_dtls == 'dtls':
+                up.subcommands.append('M4:1 S')
+                otherside.transports[si] = 'UDP/TLS/RTP/SAVP'
+            if self.gateway_dtls == 'dtls' and sect.m_header.transport in DTLS_TRANSPORTS:
+                adict = dict([(x.name, x.value) for x in sect.a_headers
+                              if x.name in DTLS_ATTRS])
+                if 'setup' not in adict:
+                    raise SdpParseError('Missing DTLS connection mode parameter')
+                if 'fingerprint' not in adict:
+                    raise SdpParseError('Missing DTLS fingerprint parameter')
+                asetup = adict['setup']
+                if asetup in ('active', 'actpass'):
+                    subcommand = 'M4:1 A'
+                elif asetup in ('passive',):
+                    subcommand = 'M4:1 P'
+                else:
+                    raise SdpParseError(F'Unknown connection mode: "{asetup}"')
+                subcommand += F' {adict["fingerprint"]}'
+                if 'ssrc' in adict:
+                    ssrc = adict['ssrc'].split(None, 1)[0]
+                    subcommand += F' {ssrc}'
+                up.subcommands.append(subcommand)
+                if otherside.gateway_dtls == 'rtp':
+                    otherside.transports[si] = 'RTP/AVP'
+            up.callback_parameters = (sdp_body, sect, sects, result_callback)
+            self.update(up)
         return
 
-    def _sdp_change_finish(self, cb_args, rtpps, sdp_body, sect, sects, result_callback):
+    def _sdp_change_finish(self, ur, rtpps, sdp_body, sect, sects, result_callback):
         sect.needs_update = False
-        if cb_args != None:
-            rtpproxy_address, rtpproxy_port, family, sendonly = cb_args
-            sect.c_header.atype = family
-            sect.c_header.addr = rtpproxy_address
+        if ur != None:
+            otherside = self.getother(rtpps)
+            if self.after_sdp_change != None:
+                self.after_sdp_change(ur.rtpproxy_address) # pylint: disable=not-callable
+            si = sects.index(sect)
+            if si in otherside.transports and self.gateway_dtls != 'pass' \
+              and otherside.transports[si] != sect.m_header.transport:
+                sect.m_header.transport = otherside.transports[si]
+                for dtls_hdr in [x for x in sect.a_headers
+                                 if x.name in DTLS_ATTRS_RM]:
+                    sect.a_headers.remove(dtls_hdr)
+            if ur.dtls_fingerprint:
+                for dtls_hdr in [x for x in sect.a_headers if x.name in DTLS_ATTRS_RM]:
+                    sect.a_headers.remove(dtls_hdr)
+                sect.addHeader('a', F'setup:{ur.dtls_mode}')
+                sect.addHeader('a', F'fingerprint:{ur.dtls_fingerprint}')
+            sect.c_header.atype = ur.family
+            sect.c_header.addr = ur.rtpproxy_address
             if sect.m_header.port != 0:
-                sect.m_header.port = rtpproxy_port
-            if sendonly:
+                sect.m_header.port = ur.rtpproxy_port
+            if ur.sendonly:
                 for sendrecv in [x for x in sect.a_headers if x.name == 'sendrecv']:
                     sect.a_headers.remove(sendrecv)
                 if len([x for x in sect.a_headers if x.name == 'sendonly']) == 0:
                     sect.addHeader('a', 'sendonly')
             if self.soft_repacketize or self.repacketize is not None:
                 fidx = -1
                 for a_header in sect.a_headers[:]:
                     if a_header.name == 'ptime':
                         fidx = sect.a_headers.index(a_header)
                         sect.a_headers.remove(a_header)
                     elif fidx == -1 and a_header.name == 'fmtp':
                         fidx = sect.a_headers.index(a_header) + 1
                 sect.insertHeader(fidx, 'a', 'ptime:%d' % self.repacketize)
             for rtcp_header in [x for x in sect.a_headers if x.name == 'rtcp']:
-                rtcp_header.value = '%d IN %s %s' % (rtpproxy_port + 1, family, rtpproxy_address)
+                rtcp_header.value = '%d IN %s %s' % (ur.rtpproxy_port + 1, ur.family, ur.rtpproxy_address)
 
         if len([x for x in sects if x.needs_update]) == 0:
             if self.oh_remote != None:
                 if self.oh_remote.session_id != sdp_body.content.o_header.session_id:
                     self.origin = SdpOrigin()
                 elif self.oh_remote.version != sdp_body.content.o_header.version:
                     self.origin.version += 1
@@ -281,24 +372,31 @@
             if rtpps.insert_nortpp:
                 sdp_body.content += 'a=nortpproxy:yes\r\n'
             sdp_body.needs_update = False
             result_callback(sdp_body)
 
     def _copy(self, rtpps, remote_ip, remote_port, result_callback = None, index = 0):
         if not self.session_exists:
-            self.update(self, '0.0.0.0', 0, self.__copy, '', index, 'IP4', remote_ip, remote_port, result_callback, index)
+            up = update_params()
+            up.rtpps = self
+            up.index = index
+            up.result_callback = self.__copy
+            up.callback_parameters = (remote_ip, remote_port, result_callback, index)
+            self.update(up)
             return
         self.__copy(None, rtpps, remote_ip, remote_port, result_callback, index)
 
     def __copy(self, result, rtpps, remote_ip, remote_port, result_callback = None, index = 0):
         from_tag, to_tag = self.gettags(rtpps)
         command = 'C %s udp:%s:%d %s %s' % ('%s-%d' % (rtpps.call_id, index), remote_ip, remote_port, from_tag, to_tag)
         rtpps.rtpp_seq.send_command(command, rtpps.command_result, result_callback)
 
 class Rtp_proxy_session(object):
+    AV_TRTYPES = ('rtp/avp', 'rtp/savp', 'rtp/savpf', 'udp/tls/rtp/savp', 'udp/tls/rtp/savpf')
+    SUPPORTED_TRTYPES = AV_TRTYPES + ('udp', 'udptl', 'udp/bfcp')
     rtp_proxy_client = None
     rtpp_seq = None
     call_id = None
     from_tag = None
     to_tag = None
     caller = None
     callee = None
@@ -313,20 +411,20 @@
       notify_socket = None, notify_tag = None):
         self.global_config = global_config
         self.my_ident = get_ident()
         if '_rtp_proxy_clients' in global_config:
             rtp_proxy_clients = [x for x in global_config['_rtp_proxy_clients'] if x.online]
             n = len(rtp_proxy_clients)
             if n == 0:
-                raise Exception('No online RTP proxy client has been found')
+                raise RtpProxyError('No online RTP proxy client has been found')
             self.rtp_proxy_client = rtp_proxy_clients[int(random() * n)]
         else:
             self.rtp_proxy_client = global_config['rtp_proxy_client']
             if not self.rtp_proxy_client.online:
-                raise Exception('No online RTP proxy client has been found')
+                raise RtpProxyError('No online RTP proxy client has been found')
         self.rtpp_seq = Rtp_proxy_cmd_sequencer(self.rtp_proxy_client)
         if call_id != None:
             self.call_id = call_id
         else:
             salt = str(random()) + str(time())
             self.call_id = md5(salt.encode()).hexdigest()
         if from_tag != None:
@@ -337,16 +435,16 @@
         if to_tag != None:
             self.to_tag = to_tag
         else:
             salt = str(random()) + str(time())
             self.to_tag = md5(salt.encode()).hexdigest()
         self.notify_socket = notify_socket
         self.notify_tag = notify_tag
-        self.caller = _rtpps_side()
-        self.callee = _rtpps_side()
+        self.caller = _rtpps_side('caller')
+        self.callee = _rtpps_side('callee')
 
     def version(self, result_callback):
         self.rtp_proxy_client.send_command('V', self.version_result, result_callback)
 
     def version_result(self, result, result_callback):
         result_callback(result)
 
@@ -366,15 +464,20 @@
         return self.caller._copy(self, remote_ip, remote_port, result_callback, index)
 
     def copy_callee(self, remote_ip, remote_port, result_callback = None, index = 0):
         return self.callee._copy(self, remote_ip, remote_port, result_callback, index)
 
     def start_recording(self, rname = None, result_callback = None, index = 0):
         if not self.caller.session_exists:
-            self.caller.update(self, '0.0.0.0', 0, self._start_recording, '', index, 'IP4', rname, result_callback, index)
+            up = update_params()
+            up.rtpps = self
+            up.index = index
+            up.result_callback = self._start_recording
+            up.callback_parameters = (rname, result_callback, index)
+            self.caller.update(up)
             return
         self._start_recording(None, self, rname, result_callback, index)
 
     def _start_recording(self, result, rtpps, rname, result_callback, index):
         if rname == None:
             command = 'R %s %s %s' % ('%s-%d' % (self.call_id, index), self.from_tag, self.to_tag)
             return self.rtpp_seq.send_command(command, self.command_result, result_callback)
@@ -384,15 +487,15 @@
 
     def _start_recording1(self, result, args):
         rname, result_callback, index = args
         command = 'C %s %s.o %s %s' % ('%s-%d' % (self.call_id, index), rname, self.to_tag, self.from_tag)
         return self.rtpp_seq.send_command(command, self.command_result, result_callback)
 
     def command_result(self, result, result_callback):
-        #print '%s.command_result(%s)' % (id(self), result)
+        #print('%s.command_result(%s)' % (id(self), result))
         if result_callback != None:
             result_callback(result)
 
     def delete(self):
         if self.rtp_proxy_client == None:
             return
         while self.max_index >= 0:
@@ -419,15 +522,15 @@
             result_callback(None, *callback_parameters)
             return
         ttl, caller_rcount, callee_rcount, fwd_rcount, drop_rcount = [int(x) for x in t1]
         result_callback((ttl, caller_rcount, callee_rcount, fwd_rcount, drop_rcount), *callback_parameters)
 
     def __del__(self):
         if self.my_ident != get_ident():
-            #print 'Rtp_proxy_session.__del__() from wrong thread, re-routing'
+            #print('Rtp_proxy_session.__del__() from wrong thread, re-routing')
             ED2.callFromThread(self.delete)
         else:
             self.delete()
 
 if __name__ == '__main__':
     from sippy.Time.Timeout import Timeout
     from sippy.Rtp_proxy_client import Rtp_proxy_client
```

### Comparing `sippy-2.0.2/sippy/SdpBody.py` & `sippy-2.1.0/sippy/SdpBody.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     first_half = ('v', 'o', 's', 'i', 'u', 'e', 'p')
     second_half = ('b', 't', 'r', 'z', 'k')
     all_headers = ('v', 'o', 's', 'i', 'u', 'e', 'p', 'c', 'b', 't', 'r', 'z', 'k')
     top_hdrs_req = ('v', 'o', 's', 't')
     sect_hdrs_req = ('c', 'm')
     sections = None
 
-    def __init__(self, body = None, cself = None):
+    def __init__(self, body = None, cself = None, ctype = None):
         if cself != None:
             for header_name in [x + '_header' for x in self.all_headers]:
                 try:
                     setattr(self, header_name, getattr(cself, header_name).getCopy())
                 except AttributeError:
                     pass
             self.a_headers = [x.getCopy() for x in cself.a_headers]
```

### Comparing `sippy-2.0.2/sippy/SdpConnecton.py` & `sippy-2.1.0/sippy/SdpConnecton.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/SdpGeneric.py` & `sippy-2.1.0/sippy/SdpGeneric.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/SdpMedia.py` & `sippy-2.1.0/sippy/SdpMedia.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/SdpMediaDescription.py` & `sippy-2.1.0/sippy/SdpMediaDescription.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/SdpOrigin.py` & `sippy-2.1.0/sippy/SdpOrigin.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/Security/SipNonce.py` & `sippy-2.1.0/sippy/Security/SipNonce.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,34 +21,24 @@
 # LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
 # ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 #import sys; sys.path.append('..')
 
+from functools import partial
 from base64 import b64encode, b64decode
 
 from Crypto import Random
 from Crypto.Cipher import AES
 
 from sippy.Time.clock_dtime import clock_getntime, CLOCK_MONOTONIC
 
-# Python 2.7 compat shims
-to_bytes_be = lambda x, sz: x.to_bytes(sz, 'big')
-try:
-    to_bytes_be(int(1), 1)
-except AttributeError:
-    to_bytes_be = lambda x, sz: '{:0{}x}'.format(x, sz * 2).decode('hex')
-
-from_bytes_be = lambda x: int.from_bytes(x, 'big')
-try:
-    from_bytes_be(to_bytes_be(1, 1))
-except AttributeError:
-    from_bytes_be = lambda x: int(x.encode('hex'), 16)
-
+to_bytes_be = partial(int.to_bytes, byteorder='big')
+from_bytes_be = partial(int.from_bytes, byteorder='big')
 
 def bxor(ba1, ba2):
     olen = len(ba1)
     ba1 = from_bytes_be(ba1)
     ba2 = from_bytes_be(ba2)
     return to_bytes_be(ba1 ^ ba2, olen)
```

### Comparing `sippy-2.0.2/sippy/Signal.py` & `sippy-2.1.0/sippy/Signal.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/SipAddress.py` & `sippy-2.1.0/sippy/SipAddress.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/SipAddressHF.py` & `sippy-2.1.0/sippy/SipAddressHF.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/SipAllow.py` & `sippy-2.1.0/sippy/SipAllow.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/SipAlso.py` & `sippy-2.1.0/sippy/SipAlso.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/SipAuthorization.py` & `sippy-2.1.0/sippy/SipAuthorization.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/SipCCDiversion.py` & `sippy-2.1.0/sippy/SipCCDiversion.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/SipCSeq.py` & `sippy-2.1.0/sippy/SipCSeq.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/SipCallId.py` & `sippy-2.1.0/sippy/SipCallId.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/SipCiscoGUID.py` & `sippy-2.1.0/sippy/SipCiscoGUID.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/SipConf.py` & `sippy-2.1.0/sippy/SipConf.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/SipContact.py` & `sippy-2.1.0/sippy/SipContact.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/SipContentLength.py` & `sippy-2.1.0/sippy/SipContentLength.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/SipContentType.py` & `sippy-2.1.0/sippy/SipProxyAuthorization.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,20 +20,14 @@
 # ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
 # (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 # LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
 # ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-from sippy.SipGenericHF import SipGenericHF
+from sippy.SipAuthorization import SipAuthorization
 
-class SipContentType(SipGenericHF):
-    hf_names = ('content-type', 'c')
-
-    def __init__(self, body):
-        SipGenericHF.__init__(self, body)
-        self.parsed = True
+class SipProxyAuthorization(SipAuthorization):
+    hf_names = ('proxy-authorization',)
 
     def getCanName(self, name, compact = False):
-        if compact:
-            return 'c'
-        return 'Content-Type'
+        return 'Proxy-Authorization'
```

### Comparing `sippy-2.0.2/sippy/SipDiversion.py` & `sippy-2.1.0/sippy/SipDiversion.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/SipExpires.py` & `sippy-2.1.0/sippy/SipExpires.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/SipFrom.py` & `sippy-2.1.0/sippy/SipFrom.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/SipGenericHF.py` & `sippy-2.1.0/sippy/SipGenericHF.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/SipHeader.py` & `sippy-2.1.0/sippy/SipHeader.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/SipLogger.py` & `sippy-2.1.0/sippy/SipLogger.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/SipMaxForwards.py` & `sippy-2.1.0/sippy/SipMaxForwards.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/SipMsg.py` & `sippy-2.1.0/sippy/SipMsg.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 from sippy.SipHeader import SipHeader
 from sippy.SipContentLength import SipContentLength
 from sippy.SipContentType import SipContentType
 from sippy.MsgBody import MsgBody
 from sippy.ESipHeaderCSV import ESipHeaderCSV
 from sippy.ESipHeaderIgnore import ESipHeaderIgnore
-from sippy.ESipParseException import ESipParseException
+from sippy.Exceptions.SipParseError import SipParseError
 
 class SipMsg(object):
     headers = None
     body = None
     startline = None
     target = None
     source = None
@@ -109,15 +109,15 @@
                 mblen = len(self.__mbody)
             if blen == 0:
                 self.__mbody = None
                 mblen = 0
             elif self.__mbody == None:
                 # XXX: Should generate 400 Bad Request if such condition
                 # happens with request
-                raise ESipParseException('Missed SIP body, %d bytes expected' % blen)
+                raise SipParseError('Missed SIP body, %d bytes expected' % blen)
             elif blen > mblen:
                 if blen - mblen < 7 and mblen > 7 and self.__mbody[-4:] == '\r\n\r\n':
                     # XXX: we should not really be doing this, but it appears to be
                     # a common off-by-one/two/.../six problem with SDPs generates by
                     # the consumer-grade devices.
                     print('Truncated SIP body, %d bytes expected, %d received, fixing...' % (blen, mblen))
                     blen = mblen
@@ -134,21 +134,21 @@
                     print('Truncated SIP body, %d bytes expected, %d received, fixing...' % (blen, mblen))
                     self.__mbody += '\r\n'
                     blen += 1
                     mblen += 2
                 else:
                     # XXX: Should generate 400 Bad Request if such condition
                     # happens with request
-                    raise ESipParseException('Truncated SIP body, %d bytes expected, %d received' % (blen, mblen))
+                    raise SipParseError('Truncated SIP body, %d bytes expected, %d received' % (blen, mblen))
             elif blen < mblen:
                 self.__mbody = self.__mbody[:blen]
                 mblen = blen
         if self.__mbody != None:
             if self.__content_type != None:
-                self.body = MsgBody(self.__mbody, str(self.__content_type.getBody()).lower())
+                self.body = MsgBody(self.__mbody, self.__content_type.getBody())
             else:
                 self.body = MsgBody(self.__mbody)
 
     def __str__(self):
         s = self.getSL() + '\r\n'
         for header in self.headers:
             s += str(header) + '\r\n'
```

### Comparing `sippy-2.0.2/sippy/SipNumericHF.py` & `sippy-2.1.0/sippy/SipNumericHF.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/SipPAssertedIdentity.py` & `sippy-2.1.0/sippy/SipPAssertedIdentity.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/SipProxyAuthenticate.py` & `sippy-2.1.0/sippy/SipProxyAuthenticate.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/SipProxyAuthorization.py` & `sippy-2.1.0/sippy/SipReferTo.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,14 +20,11 @@
 # ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
 # (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 # LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
 # ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-from sippy.SipAuthorization import SipAuthorization
+from sippy.SipAddressHF import SipAddressHF
 
-class SipProxyAuthorization(SipAuthorization):
-    hf_names = ('proxy-authorization',)
-
-    def getCanName(self, name, compact = False):
-        return 'Proxy-Authorization'
+class SipReferTo(SipAddressHF):
+    hf_names = ('refer-to', 'r')
```

### Comparing `sippy-2.0.2/sippy/SipRAck.py` & `sippy-2.1.0/sippy/SipRAck.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/SipRSeq.py` & `sippy-2.1.0/sippy/SipRSeq.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/SipReason.py` & `sippy-2.1.0/sippy/SipReason.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/SipRecordRoute.py` & `sippy-2.1.0/sippy/SipRecordRoute.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/SipReferTo.py` & `sippy-2.1.0/sippy/SipReferredBy.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,9 +22,9 @@
 # LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
 # ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from sippy.SipAddressHF import SipAddressHF
 
-class SipReferTo(SipAddressHF):
-    hf_names = ('refer-to', 'r')
+class SipReferredBy(SipAddressHF):
+    hf_names = ('referred-by',)
```

### Comparing `sippy-2.0.2/sippy/SipReferredBy.py` & `sippy-2.1.0/sippy/SipTo.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,11 +20,17 @@
 # ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
 # (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 # LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
 # ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-from sippy.SipAddressHF import SipAddressHF
+from sippy.SipFrom import SipFrom
 
-class SipReferredBy(SipAddressHF):
-    hf_names = ('referred-by',)
+class SipTo(SipFrom):
+    hf_names = ('to', 't')
+    relaxedparser = True
+
+    def getCanName(self, name, compact = False):
+        if compact:
+            return 't'
+        return 'To'
```

### Comparing `sippy-2.0.2/sippy/SipRegistrationAgent.py` & `sippy-2.1.0/sippy/SipRegistrationAgent.py`

 * *Files 8% similar despite different names*

```diff
@@ -88,31 +88,30 @@
             else:
                 tout = 180
             timer = Timeout(self.doregister, tout)
             if self.rok_cb != None:
                 self.rok_cb(timer.etime.realt, contact, self.cb_arg)
             self.atries = 0
             return
-        if resp.scode == 401 and resp.countHFs('www-authenticate') != 0 and \
-          self.user != None and self.passw != None and self.atries < 3:
-            challenge = resp.getHFBody('www-authenticate')
-            auth = challenge.genAuthHF(self.user, self.passw, 'REGISTER', str(self.rmsg.ruri))
-            for authorization in self.rmsg.getHFs('authorization'):
-                self.rmsg.removeHeader(authorization)
-            self.rmsg.appendHeader(SipHeader(name = 'authorization', body = auth))
-            self.atries += 1
-            self.doregister()
-            return
-        if resp.scode == 407 and resp.countHFs('proxy-authenticate') != 0 and \
-          self.user != None and self.passw != None and self.atries < 3:
-            challenge = resp.getHFBody('proxy-authenticate')
-            auth = challenge.genAuthHF(self.user, self.passw, 'REGISTER', str(self.rmsg.ruri))
-            for authorization in self.rmsg.getHFs('proxy-authorization'):
-                self.rmsg.removeHeader(authorization)
-            self.rmsg.appendHeader(SipHeader(name = 'proxy-authorization', body = auth))
-            self.atries += 1
-            self.doregister()
-            return
+        if self.user != None and self.passw != None and self.atries < 3:
+            for sc, chn, rhn in ((401, 'www-authenticate', 'authorization'),
+                                 (407, 'proxy-authenticate', 'authorization')):
+                if resp.scode != sc:
+                    continue
+                if resp.countHFs(chn) == 0:
+                    break
+                challenge = resp.getHFBody(chn)
+                supported, qop = challenge.supportedAlgorithm()
+                if not supported:
+                    break
+                auth = challenge.genAuthHF(self.user, self.passw, 'REGISTER',
+                                           str(self.rmsg.ruri), qop=qop)
+                for authorization in self.rmsg.getHFs(rhn):
+                    self.rmsg.removeHeader(authorization)
+                self.rmsg.appendHeader(SipHeader(name = rhn, body = auth))
+                self.atries += 1
+                self.doregister()
+                return
         if self.rfail_cb != None:
             self.rfail_cb(resp.getSL(), self.cb_arg)
         Timeout(self.doregister, 60)
         self.atries = 0
```

### Comparing `sippy-2.0.2/sippy/SipReplaces.py` & `sippy-2.1.0/sippy/SipReplaces.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/SipRequest.py` & `sippy-2.1.0/sippy/SipRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,30 +28,30 @@
 from sippy.SipHeader import SipHeader
 from sippy.SipCSeq import SipCSeq
 from sippy.SipTo import SipTo
 from sippy.SipResponse import SipResponse
 from sippy.SipURL import SipURL
 from sippy.SipAddress import SipAddress
 from sippy.SipExpires import SipExpires
-from sippy.ESipParseException import ESipParseException
+from sippy.Exceptions.SipParseError import SipParseError
 
 class SipRequest(SipMsg):
     method = None
     ruri = None
     sipver = None
     user_agent = None
 
     def __init__(self, buf = None, method = None, ruri = None, sipver = 'SIP/2.0', to = None, fr0m = None, via = None, cseq = None, \
                  callid = None, maxforwards = None, body = None, contact = None, routes = (), target = None,
                  user_agent = None, expires = None):
         SipMsg.__init__(self, buf)
         if buf != None:
             try:
                 SipMsg.init_body(self)
-            except ESipParseException as e:
+            except SipParseError as e:
                 try:
                     e.sip_response = self.genResponse(400, 'Bad Request - %s' % str(e))
                 except Exception as e1:
                     print('BUG: Double exception, should not be happening:\n', str(e1))
                 raise e
             return
         self.method = method
```

### Comparing `sippy-2.0.2/sippy/SipResponse.py` & `sippy-2.1.0/sippy/SipResponse.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/SipRoute.py` & `sippy-2.1.0/sippy/SipRoute.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/SipServer.py` & `sippy-2.1.0/sippy/SipServer.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/SipSupported.py` & `sippy-2.1.0/sippy/SipSupported.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/SipTo.py` & `sippy-2.1.0/sippy/SipUserAgent.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,17 +20,14 @@
 # ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
 # (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 # LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
 # ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-from sippy.SipFrom import SipFrom
+from sippy.SipServer import SipServer
 
-class SipTo(SipFrom):
-    hf_names = ('to', 't')
-    relaxedparser = True
+class SipUserAgent(SipServer):
+    hf_names = ('user-agent',)
 
     def getCanName(self, name, compact = False):
-        if compact:
-            return 't'
-        return 'To'
+        return 'User-Agent'
```

### Comparing `sippy-2.0.2/sippy/SipTransactionManager.py` & `sippy-2.1.0/sippy/SipTransactionManager.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,17 @@
 from sippy.Time.Timeout import Timeout
 from sippy.SipHeader import SipHeader
 from sippy.SipResponse import SipResponse
 from sippy.SipRequest import SipRequest
 from sippy.SipAddress import SipAddress
 from sippy.SipRoute import SipRoute
 from sippy.SipHeader import SipHeader
-from sippy.ESipParseException import ESipParseException
+from sippy.Exceptions.SipParseError import SipParseError, SdpParseError
+from sippy.Exceptions.RtpProxyError import RtpProxyError
+from sippy.Udp_server import Udp_server, Udp_server_opts
 from datetime import datetime
 from hashlib import md5
 from traceback import print_exc
 from functools import reduce
 import sys, socket
 
 class NETS_1918(object):
@@ -50,14 +52,17 @@
         for naddr, mask in NETS_1918.nets:
             if addr & mask == naddr:
                 return True
     except:
         pass
     return False
 
+def check7118(host):
+    return host.endswith('.invalid')
+
 class SipTransactionConsumer(object):
     compact = False
     cobj = None
 
     def __init__(self, cobj, compact):
         self.compact = compact
         self.cobj = cobj
@@ -121,26 +126,18 @@
     cache_r2l_old = None
     cache_l2s = None
     skt = None
     handleIncoming = None
     fixed = False
     ploss_out_rate = 0.0
     pdelay_out_max = 0.0
-    nworkers_udp = None
 
-    def __init__(self, global_config, handleIncoming, nworkers_udp = None):
-        if not '_xmpp_mode' in global_config or not global_config['_xmpp_mode']:
-            from sippy.Udp_server import Udp_server, Udp_server_opts
-            self.Udp_server_opts = Udp_server_opts
-            self.udp_server_class = Udp_server
-        else:
-            from sippy.XMPP_server import XMPP_server, XMPP_server_opts
-            self.Udp_server_opts = XMPP_server_opts
-            self.udp_server_class = XMPP_server
-        self.nworkers_udp = nworkers_udp
+    def __init__(self, global_config, handleIncoming, usc, usoc):
+        self.Udp_server_opts = usoc
+        self.udp_server_class = usc
         self.global_config = global_config
         self.cache_r2l = {}
         self.cache_r2l_old = {}
         self.cache_l2s = {}
         self.handleIncoming = handleIncoming
         try:
             # Python can be compiled with IPv6 support, but if kernel
@@ -154,23 +151,30 @@
             if socket.has_ipv6:
                 laddresses = (('0.0.0.0', global_config['_sip_port']), ('[::]', global_config['_sip_port']))
             else:
                 laddresses = (('0.0.0.0', global_config['_sip_port']),)
         else:
             laddresses = ((global_config['_sip_address'], global_config['_sip_port']),)
             self.fixed = True
-        for laddress in laddresses:
-            self.initServer(laddress)
+        # Since we are (an)using SO_REUSEXXX do a quick dry run to make
+        # sure no existing app is running on the same port.
+        for dryr in (True, False):
+            for laddress in laddresses:
+                self.initServer(laddress, dryr)
 
-    def initServer(self, laddress):
+    def initServer(self, laddress, dryr=False):
         sopts = self.Udp_server_opts(laddress, self.handleIncoming)
         sopts.ploss_out_rate = self.ploss_out_rate
         sopts.pdelay_out_max = self.pdelay_out_max
-        sopts.nworkers = self.nworkers_udp
+        if dryr:
+            sopts.flags = 0
         server = self.udp_server_class(self.global_config, sopts)
+        if dryr:
+            server.shutdown()
+            return None
         self.cache_l2s[laddress] = server
         return server
 
     def getServer(self, address, is_local = False):
         if self.fixed:
             return tuple(self.cache_l2s.items())[0][1]
         if not is_local:
@@ -236,19 +240,19 @@
     l1rcache = None
     l2rcache = None
     nat_traversal = False
     req_consumers = None
     provisional_retr = 0
     ploss_out_rate = 0.0
     pdelay_out_max = 0.0
-    nworkers_udp = None
+    model_udp_server = (Udp_server, Udp_server_opts)
 
     def __init__(self, global_config, req_cb = None):
         self.global_config = global_config
-        self.l4r = local4remote(global_config, self.handleIncoming, self.nworkers_udp)
+        self.l4r = local4remote(global_config, self.handleIncoming, *self.model_udp_server)
         self.l4r.ploss_out_rate = self.ploss_out_rate
         self.l4r.pdelay_out_max = self.pdelay_out_max
         self.tclient = {}
         self.tserver = {}
         self.req_cb = req_cb
         self.l1rcache = {}
         self.l2rcache = {}
@@ -300,24 +304,26 @@
             resp.setSource(address)
             self.incomingResponse(resp, t, checksum)
         else:
             try:
                 req = SipRequest(data)
                 tids = req.getTIds()
             except Exception as exception:
-                if isinstance(exception, ESipParseException) and exception.sip_response != None:
-                    self.transmitMsg(server, exception.sip_response, address, checksum)
+                if isinstance(exception, SipParseError):
+                    resp = exception.getResponse()
+                    if resp is not None:
+                        self.transmitMsg(server, resp, address, checksum)
                 dump_exception('can\'t parse SIP request from %s:%d' % (address[0], address[1]), extra = data)
                 self.l1rcache[checksum] = SipTMRetransmitO()
                 return
             req.rtime = rtime
             via0 = req.getHFBody('via')
             ahost, aport = via0.getAddr()
             rhost, rport = address
-            if self.nat_traversal and rport != aport and check1918(ahost):
+            if self.nat_traversal and rport != aport and (check1918(ahost) or check7118(ahost)):
                 req.nated = True
             if ahost != rhost:
                 via0.params['received'] = rhost
             if 'rport' in via0.params or req.nated:
                 via0.params['rport'] = str(rport)
             if self.nat_traversal and req.countHFs('contact') > 0 and req.countHFs('via') == 1:
                 try:
@@ -328,15 +334,28 @@
                     return
                 if not cbody.asterisk:
                     curl = cbody.getUrl()
                     if check1918(curl.host) or curl.port == 0 or curl.host == '255.255.255.255':
                         curl.host, curl.port = address
                         req.nated = True
             req.setSource(address)
-            self.incomingRequest(req, checksum, tids, server)
+            try:
+                self.incomingRequest(req, checksum, tids, server)
+            except RtpProxyError as ex:
+                resp = ex.getResponse(req)
+                self.sendResponse(resp)
+                raise
+            except SdpParseError as ex:
+                resp = ex.getResponse(req)
+                self.sendResponse(resp)
+            except SipParseError as ex:
+                resp = ex.getResponse(req)
+                if resp is None:
+                    raise ex
+                self.sendResponse(resp)
 
     # 1. Client transaction methods
     def newTransaction(self, msg, resp_cb = None, laddress = None, userv = None, \
       cb_ifver = 1, compact = False, t = None):
         if t == None:
             t = SipTransaction()
         t.rtime = MonoTime()
```

### Comparing `sippy-2.0.2/sippy/SipURL.py` & `sippy-2.1.0/sippy/SipURL.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/SipUserAgent.py` & `sippy-2.1.0/sippy/UaStateFailed.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,14 +20,25 @@
 # ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
 # (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 # LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
 # ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-from sippy.SipServer import SipServer
+from sippy.Time.Timeout import Timeout
+from sippy.UaStateGeneric import UaStateGeneric
 
-class SipUserAgent(SipServer):
-    hf_names = ('user-agent',)
+class UaStateFailed(UaStateGeneric):
+    sname = 'Failed'
 
-    def getCanName(self, name, compact = False):
-        return 'User-Agent'
+    def __init__(self, ua):
+        UaStateGeneric.__init__(self, ua)
+        ua.on_local_sdp_change = None
+        ua.on_remote_sdp_change = None
+        Timeout(self.goDead, ua.godead_timeout)
+
+    def goDead(self):
+        #print 'Time in Failed state expired, going to the Dead state'
+        self.ua.changeState((UaStateDead,))
+
+if not 'UaStateDead' in globals():
+    from sippy.UaStateDead import UaStateDead
```

### Comparing `sippy-2.0.2/sippy/SipVia.py` & `sippy-2.1.0/sippy/SipVia.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/SipWWWAuthenticate.py` & `sippy-2.1.0/sippy/SipWWWAuthenticate.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
         auth = self.aclass(realm = self.realm, nonce = self.nonce, uri = uri, username = username)
         auth.algorithm = self.algorithm
         if self.qop is not None and qop is not None:
             auth.qop = qop
             auth.nc = '00000001'
             auth.cnonce = self.readhex(4)
         if self.opaque != None:
-            auth.opaque = self.opaque
+            auth.otherparams.append(('opaque', f'"{self.opaque}"'))
         auth.genAuthResponse(password, method, body)
         return auth
 
     def supportedAlgorithm(self):
         if self.qop is not None:
             qops = [x for x in self.qop if x in ('auth', 'auth-int')]
             if len(qops) == 0:
```

### Comparing `sippy-2.0.2/sippy/SipWarning.py` & `sippy-2.1.0/sippy/SipWarning.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/StatefulProxy.py` & `sippy-2.1.0/sippy/StatefulProxy.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/Time/MonoTime.py` & `sippy-2.1.0/sippy/Time/MonoTime.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/Time/Timeout.py` & `sippy-2.1.0/sippy/Time/Timeout.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/Time/clock_dtime.py` & `sippy-2.1.0/sippy/Time/clock_dtime.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/UA.py` & `sippy-2.1.0/sippy/UA.py`

 * *Files 1% similar despite different names*

```diff
@@ -387,14 +387,17 @@
         return tuple(rval)
 
     def delayed_remote_sdp_update(self, event, remote_sdp_body):
         self.rSDP = remote_sdp_body.getCopy()
         self.equeue.append(event)
         self.emitPendingEvents()
 
+    def delayed_local_sdp_update(self, event, local_sdp_body):
+        self.recvEvent(event)
+
     def getAcct(self):
         if self.disconnect_ts != None:
             disconnect_ts = self.disconnect_ts
             disconnected = True
         else:
             disconnect_ts = MonoTime()
             disconnected = False
```

### Comparing `sippy-2.0.2/sippy/UaStateConnected.py` & `sippy-2.1.0/sippy/UaStateConnected.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 # ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
 # (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 # LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
 # ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+from functools import partial
+
 from sippy.Time.Timeout import Timeout
 from sippy.UaStateGeneric import UaStateGeneric
 from sippy.SipAlso import SipAlso
 from sippy.SipAddress import SipAddress
 from sippy.SipHeader import SipHeader
 from sippy.SipReferTo import SipReferTo
 from sippy.SipReferredBy import SipReferredBy
@@ -81,15 +83,15 @@
                 pass
             try:
                 event.max_forwards = req.getHFBody('max-forwards').getNum()
             except:
                 pass
             if body != None:
                 if self.ua.on_remote_sdp_change != None:
-                    self.ua.on_remote_sdp_change(body, lambda x: self.ua.delayed_remote_sdp_update(event, x))
+                    self.ua.on_remote_sdp_change(body, partial(self.ua.delayed_remote_sdp_update, event))
                     return (UasStateUpdating,)
                 else:
                     self.ua.rSDP = body.getCopy()
             else:
                 self.ua.rSDP = None
             self.ua.equeue.append(event)
             return (UasStateUpdating,)
@@ -133,15 +135,15 @@
             self.ua.expire_timer = None
         self.ua.startCreditTimer(req.rtime)
         self.ua.connect_ts = req.rtime
         for callback in self.ua.conn_cbs:
             callback(self.ua, req.rtime, self.ua.origin)
         if body != None:
             if self.ua.on_remote_sdp_change != None:
-                self.ua.on_remote_sdp_change(body, lambda x: self.ua.delayed_remote_sdp_update(event, x))
+                self.ua.on_remote_sdp_change(body, partial(self.ua.delayed_remote_sdp_update, event))
                 return None
             else:
                 self.ua.rSDP = body.getCopy()
         else:
             self.ua.rSDP = None
         self.ua.equeue.append(event)
         return None
@@ -184,15 +186,15 @@
                         rtime = event.rtime, origin = event.origin))
                 else:
                     self.ua.equeue.append(CCEventConnect((200, 'OK', None), rtime = event.rtime, \
                       origin = event.origin))
                 return None
             if body != None and self.ua.on_local_sdp_change != None and body.needs_update:
                 try:
-                    self.ua.on_local_sdp_change(body, lambda x: self.ua.recvEvent(event), en_excpt = True)
+                    self.ua.on_local_sdp_change(body, partial(self.ua.delayed_local_sdp_update, event), en_excpt = True)
                 except Exception as e:
                     event = CCEventFail((400, 'Malformed SDP Body'), rtime = event.rtime)
                     event.setWarning(str(e))
                     self.ua.equeue.append(event)
                 return None
             if event.max_forwards != None:
                 if event.max_forwards <= 0:
@@ -218,15 +220,15 @@
             return None
         if self.ua.pending_tr != None and isinstance(event, CCEventConnect):
             if self.ua.expire_timer != None:
                 self.ua.expire_timer.cancel()
                 self.ua.expire_timer = None
             code, reason, body = event.getData()
             if body != None and self.ua.on_local_sdp_change != None and body.needs_update:
-                self.ua.on_local_sdp_change(body, lambda x: self.ua.recvEvent(event))
+                self.ua.on_local_sdp_change(body, partial(self.ua.delayed_local_sdp_update, event))
                 return None
             self.ua.startCreditTimer(event.rtime)
             self.ua.connect_ts = event.rtime
             self.ua.lSDP = body
             self.ua.pending_tr.ack.setBody(body)
             self.ua.global_config['_sip_tm'].sendACK(self.ua.pending_tr)
             self.ua.pending_tr = None
```

### Comparing `sippy-2.0.2/sippy/UaStateDead.py` & `sippy-2.1.0/sippy/UaStateDead.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/UaStateDisconnected.py` & `sippy-2.1.0/sippy/UaStateDisconnected.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/UaStateFailed.py` & `sippy-2.1.0/sippy/Exceptions/RtpProxyError.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# Copyright (c) 2003-2005 Maxim Sobolev. All rights reserved.
-# Copyright (c) 2006-2014 Sippy Software, Inc. All rights reserved.
+# Copyright (c) 2023 Sippy Software, Inc. All rights reserved.
 #
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without modification,
 # are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
@@ -20,25 +19,20 @@
 # ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
 # (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 # LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
 # ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-from sippy.Time.Timeout import Timeout
-from sippy.UaStateGeneric import UaStateGeneric
+from sippy.Exceptions.SipParseError import SdpParseError
 
-class UaStateFailed(UaStateGeneric):
-    sname = 'Failed'
+class RtpProxyError(Exception):
+    sip_response = None
+    arg = None
+    code = 502
+    msg = 'Bad Gateway'
+    def __init__(self, arg):
+        super().__init__()
+        self.arg = arg
 
-    def __init__(self, ua):
-        UaStateGeneric.__init__(self, ua)
-        ua.on_local_sdp_change = None
-        ua.on_remote_sdp_change = None
-        Timeout(self.goDead, ua.godead_timeout)
-
-    def goDead(self):
-        #print 'Time in Failed state expired, going to the Dead state'
-        self.ua.changeState((UaStateDead,))
-
-if not 'UaStateDead' in globals():
-    from sippy.UaStateDead import UaStateDead
+    def getResponse(self, req):
+        return SdpParseError.getResponse(self, req)
```

### Comparing `sippy-2.0.2/sippy/UaStateGeneric.py` & `sippy-2.1.0/sippy/UaStateGeneric.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/UacStateCancelling.py` & `sippy-2.1.0/sippy/UacStateCancelling.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/UacStateIdle.py` & `sippy-2.1.0/sippy/UacStateIdle.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 # ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
 # (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 # LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
 # ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+from functools import partial
+
 from sippy.Time.Timeout import TimeoutAbsMono
 from sippy.UaStateGeneric import UaStateGeneric
 from sippy.CCEvents import CCEventTry, CCEventFail, CCEventRedirect, CCEventDisconnect
 from sippy.SipContact import SipContact
 from sippy.SipAddress import SipAddress
 from sippy.SipURL import SipURL
 from sippy.SipTo import SipTo
@@ -42,15 +44,15 @@
         if isinstance(event, CCEventTry):
             if self.ua.setup_ts == None:
                 self.ua.setup_ts = event.rtime
             self.ua.origin = 'callee'
             cId, callingID, calledID, body, auth, callingName = event.getData()
             if body != None:
                 if self.ua.on_local_sdp_change != None and body.needs_update:
-                    self.ua.on_local_sdp_change(body, lambda x: self.ua.recvEvent(event))
+                    self.ua.on_local_sdp_change(body, partial(self.ua.delayed_local_sdp_update, event))
                     return None
             else:
                 self.ua.late_media = True
             if cId == None:
                 self.ua.cId = SipCallId()
             else:
                 self.ua.cId = cId.getCopy()
```

### Comparing `sippy-2.0.2/sippy/UacStateRinging.py` & `sippy-2.1.0/sippy/UacStateRinging.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 # ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
 # (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 # LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
 # ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+from functools import partial
+
 from sippy.SipAddress import SipAddress
 from sippy.SipRoute import SipRoute
 from sippy.UaStateGeneric import UaStateGeneric
 from sippy.CCEvents import CCEventRing, CCEventConnect, CCEventFail, CCEventRedirect, \
   CCEventDisconnect, CCEventPreConnect
 
 class UacStateRinging(UaStateGeneric):
@@ -43,15 +45,15 @@
                 self.ua.p1xx_ts = resp.rtime
             self.ua.last_scode = code
             event = CCEventRing(scode, rtime = resp.rtime, origin = self.ua.origin)
             for ring_cb in self.ua.ring_cbs:
                 ring_cb(self.ua, resp.rtime, self.ua.origin, code)
             if body != None:
                 if self.ua.on_remote_sdp_change != None:
-                    self.ua.on_remote_sdp_change(body, lambda x: self.ua.delayed_remote_sdp_update(event, x))
+                    self.ua.on_remote_sdp_change(body, partial(self.ua.delayed_remote_sdp_update, event))
                     return None
                 else:
                     self.ua.rSDP = body.getCopy()
             else:
                 self.ua.rSDP = None
             self.ua.equeue.append(event)
             return None
@@ -117,15 +119,15 @@
             else:
                 event = CCEventPreConnect(scode, rtime = resp.rtime, origin = self.ua.origin)
                 tr.uack = True
                 self.ua.pending_tr = tr
                 rval = (UaStateConnected,)
             if body != None:
                 if self.ua.on_remote_sdp_change != None:
-                    self.ua.on_remote_sdp_change(body, lambda x: self.ua.delayed_remote_sdp_update(event, x))
+                    self.ua.on_remote_sdp_change(body, partial(self.ua.delayed_remote_sdp_update, event))
                     return rval
                 else:
                     self.ua.rSDP = body.getCopy()
             else:
                 self.ua.rSDP = None
             self.ua.equeue.append(event)
             return rval
```

### Comparing `sippy-2.0.2/sippy/UacStateTrying.py` & `sippy-2.1.0/sippy/UacStateTrying.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 # ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
 # (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 # LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
 # ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+from functools import partial
+
 from sippy.SipAddress import SipAddress
 from sippy.SipRoute import SipRoute
 from sippy.UaStateGeneric import UaStateGeneric
 from sippy.Time.Timeout import TimeoutAbsMono
 from sippy.CCEvents import CCEventRing, CCEventConnect, CCEventFail, CCEventRedirect, \
   CCEventDisconnect, CCEventPreConnect
 
@@ -58,15 +60,15 @@
             self.ua.no_progress_timer = None
             if code < 200 and self.ua.expire_time != None:
                 self.ua.expire_timer = TimeoutAbsMono(self.ua.expires, self.ua.expire_mtime)
         if code < 200:
             event = CCEventRing(scode, rtime = resp.rtime, origin = self.ua.origin)
             if body != None:
                 if self.ua.on_remote_sdp_change != None:
-                    self.ua.on_remote_sdp_change(body, lambda x: self.ua.delayed_remote_sdp_update(event, x))
+                    self.ua.on_remote_sdp_change(body, partial(self.ua.delayed_remote_sdp_update, event))
                     self.ua.p1xx_ts = resp.rtime
                     return (UacStateRinging, self.ua.ring_cbs, resp.rtime, self.ua.origin, code)
                 else:
                     self.ua.rSDP = body.getCopy()
             else:
                 self.ua.rSDP = None
             self.ua.equeue.append(event)
@@ -135,15 +137,15 @@
             else:
                 event = CCEventPreConnect(scode, rtime = resp.rtime, origin = self.ua.origin)
                 tr.uack = True
                 self.ua.pending_tr = tr
                 rval = (UaStateConnected,)
             if body != None:
                 if self.ua.on_remote_sdp_change != None:
-                    self.ua.on_remote_sdp_change(body, lambda x: self.ua.delayed_remote_sdp_update(event, x))
+                    self.ua.on_remote_sdp_change(body, partial(self.ua.delayed_remote_sdp_update, event))
                     return rval
                 else:
                     self.ua.rSDP = body.getCopy()
             else:
                 self.ua.rSDP = None
             self.ua.equeue.append(event)
             return rval
```

### Comparing `sippy-2.0.2/sippy/UacStateUpdating.py` & `sippy-2.1.0/sippy/UacStateUpdating.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 # ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
 # (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 # LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
 # ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+from functools import partial
+
 from sippy.UaStateGeneric import UaStateGeneric
 from sippy.CCEvents import CCEventDisconnect, CCEventRing, CCEventConnect, CCEventFail, CCEventRedirect
 
 class UacStateUpdating(UaStateGeneric):
     sname = 'Updating(UAC)'
     triedauth = False
     connected = True
@@ -59,15 +61,15 @@
         if code < 200:
             self.ua.equeue.append(CCEventRing(scode, rtime = resp.rtime, origin = self.ua.origin))
             return None
         if code >= 200 and code < 300:
             event = CCEventConnect(scode, rtime = resp.rtime, origin = self.ua.origin)
             if body != None:
                 if self.ua.on_remote_sdp_change != None:
-                    cb_func = lambda x: self.ua.delayed_remote_sdp_update(event, x)
+                    cb_func = partial(self.ua.delayed_remote_sdp_update, event)
                     try:
                         self.ua.on_remote_sdp_change(body, cb_func, en_excpt = True)
                     except Exception as e:
                         event = CCEventFail((502, 'Bad Gateway'), rtime = event.rtime)
                         event.setWarning('Malformed SDP Body received from ' \
                           'downstream: "%s"' % str(e))
                         return self.updateFailed(event)
```

### Comparing `sippy-2.0.2/sippy/UasStateIdle.py` & `sippy-2.1.0/sippy/UasStateIdle.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 # ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
 # (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 # LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
 # ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+from functools import partial
+
 from sippy.Time.Timeout import TimeoutAbsMono
 from sippy.SipAddress import SipAddress
 from sippy.SipRoute import SipRoute
 from sippy.UaStateGeneric import UaStateGeneric
 from sippy.CCEvents import CCEventTry
 from sippy.SipContact import SipContact
 from sippy.SipFrom import SipFrom
@@ -94,15 +96,15 @@
                 self.ua.no_progress_time = None
         if self.ua.no_progress_time != None:
             self.ua.no_progress_timer = TimeoutAbsMono(self.ua.no_progress_expires, self.ua.no_progress_mtime)
         elif self.ua.expire_time != None:
             self.ua.expire_timer = TimeoutAbsMono(self.ua.expires, self.ua.expire_mtime)
         if body != None:
             if self.ua.on_remote_sdp_change != None:
-                self.ua.on_remote_sdp_change(body, lambda x: self.ua.delayed_remote_sdp_update(event, x))
+                self.ua.on_remote_sdp_change(body, partial(self.ua.delayed_remote_sdp_update, event))
                 self.ua.setup_ts = req.rtime
                 return (UasStateTrying,)
             else:
                 self.ua.rSDP = body.getCopy()
         else:
             self.ua.rSDP = None
         self.ua.equeue.append(event)
```

### Comparing `sippy-2.0.2/sippy/UasStateRinging.py` & `sippy-2.1.0/sippy/UasStateRinging.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,19 +20,20 @@
 # ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
 # (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 # LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
 # ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+from functools import partial
+
 from sippy.UaStateGeneric import UaStateGeneric
 from sippy.CCEvents import CCEventRing, CCEventConnect, CCEventFail, CCEventRedirect, \
   CCEventDisconnect, CCEventPreConnect
 from sippy.SipContact import SipContact
-from sippy.SipAddress import SipAddress
 
 class UasStateRinging(UaStateGeneric):
     sname = 'Ringing(UAS)'
     rseq = None
 
     def recvEvent(self, event):
         if isinstance(event, CCEventRing):
@@ -40,27 +41,27 @@
             if scode == None:
                 code, reason, body = (180, 'Ringing', None)
             else:
                 code, reason, body = scode
                 if code == 100:
                     return None
                 if body != None and self.ua.on_local_sdp_change != None and body.needs_update:
-                    self.ua.on_local_sdp_change(body, lambda x: self.ua.recvEvent(event))
+                    self.ua.on_local_sdp_change(body, partial(self.ua.delayed_local_sdp_update, event))
                     return None
             self.ua.lSDP = body
             if self.ua.p1xx_ts == None:
                 self.ua.p1xx_ts = event.rtime
             self.ua.sendUasResponse(code, reason, body)
             for ring_cb in self.ua.ring_cbs:
                 ring_cb(self.ua, event.rtime, event.origin, code)
             return None
         elif isinstance(event, CCEventConnect) or isinstance(event, CCEventPreConnect):
             code, reason, body = event.getData()
             if body != None and self.ua.on_local_sdp_change != None and body.needs_update:
-                self.ua.on_local_sdp_change(body, lambda x: self.ua.recvEvent(event))
+                self.ua.on_local_sdp_change(body, partial(self.ua.delayed_local_sdp_update, event))
                 return None
             if event.extra_headers != None:
                 extra_headers = tuple(event.extra_headers)
             else:
                 extra_headers = None
             self.ua.lSDP = body
             if isinstance(event, CCEventConnect):
```

### Comparing `sippy-2.0.2/sippy/UasStateTrying.py` & `sippy-2.1.0/sippy/UasStateTrying.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,19 +20,20 @@
 # ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
 # (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 # LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
 # ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+from functools import partial
+
 from sippy.UaStateGeneric import UaStateGeneric
 from sippy.CCEvents import CCEventRing, CCEventConnect, CCEventFail, CCEventRedirect, \
   CCEventDisconnect, CCEventPreConnect
 from sippy.SipContact import SipContact
-from sippy.SipAddress import SipAddress
 from sippy.Time.Timeout import TimeoutAbsMono
 
 class UasStateTrying(UaStateGeneric):
     sname = 'Trying(UAS)'
 
     def recvEvent(self, event):
         if isinstance(event, CCEventRing):
@@ -40,30 +41,30 @@
             if scode == None:
                 code, reason, body = (180, 'Ringing', None)
             else:
                 code, reason, body = scode
                 if code == 100:
                     return None
                 if body != None and self.ua.on_local_sdp_change != None and body.needs_update:
-                    self.ua.on_local_sdp_change(body, lambda x: self.ua.recvEvent(event))
+                    self.ua.on_local_sdp_change(body, partial(self.ua.delayed_local_sdp_update, event))
                     return None
             self.ua.lSDP = body
             self.ua.sendUasResponse(code, reason, body)
             if self.ua.no_progress_timer != None:
                 self.ua.no_progress_timer.cancel()
                 self.ua.no_progress_timer = None
                 if self.ua.expire_time != None:
                     self.ua.expire_timer = TimeoutAbsMono(self.ua.expires, self.ua.expire_mtime)
             if self.ua.p1xx_ts == None:
                 self.ua.p1xx_ts = event.rtime
             return (UasStateRinging, self.ua.ring_cbs, event.rtime, event.origin, code)
         elif isinstance(event, CCEventConnect) or isinstance(event, CCEventPreConnect):
             code, reason, body = event.getData()
             if body != None and self.ua.on_local_sdp_change != None and body.needs_update:
-                self.ua.on_local_sdp_change(body, lambda x: self.ua.recvEvent(event))
+                self.ua.on_local_sdp_change(body, partial(self.ua.delayed_local_sdp_update, event))
                 return None
             if event.extra_headers != None:
                 extra_headers = tuple(event.extra_headers)
             else:
                 extra_headers = None
             self.ua.lSDP = body
             if self.ua.no_progress_timer != None:
```

### Comparing `sippy-2.0.2/sippy/UasStateUpdating.py` & `sippy-2.1.0/sippy/UasStateUpdating.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,17 @@
 # ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
 # (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 # LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
 # ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+from functools import partial
+
 from sippy.SipContact import SipContact
-from sippy.SipAddress import SipAddress
 from sippy.UaStateGeneric import UaStateGeneric
 from sippy.CCEvents import CCEventDisconnect, CCEventRing, CCEventConnect, CCEventFail, CCEventRedirect
 
 class UasStateUpdating(UaStateGeneric):
     sname = 'Updating(UAS)'
     connected = True
 
@@ -71,23 +72,23 @@
     def recvEvent(self, event):
         if isinstance(event, CCEventRing):
             scode = event.getData()
             if scode == None:
                 scode = (180, 'Ringing', None)
             body = scode[2]
             if body != None and self.ua.on_local_sdp_change != None and body.needs_update:
-                self.ua.on_local_sdp_change(body, lambda x: self.ua.recvEvent(event))
+                self.ua.on_local_sdp_change(body, partial(self.ua.delayed_local_sdp_update, event))
                 return None
             self.ua.lSDP = body
             self.ua.sendUasResponse(scode[0], scode[1], body)
             return None
         elif isinstance(event, CCEventConnect):
             code, reason, body = event.getData()
             if body != None and self.ua.on_local_sdp_change != None and body.needs_update:
-                self.ua.on_local_sdp_change(body, lambda x: self.ua.recvEvent(event))
+                self.ua.on_local_sdp_change(body, partial(self.ua.delayed_local_sdp_update, event))
                 return None
             self.ua.lSDP = body
             self.ua.sendUasResponse(code, reason, body, (self.ua.lContact,))
             return (UaStateConnected,)
         elif isinstance(event, CCEventRedirect):
             scode = event.getData()
             contacts = None
```

### Comparing `sippy-2.0.2/sippy/Udp_server.py` & `sippy-2.1.0/sippy/Udp_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 from random import random
 import socket
 
 from sippy.Core.EventDispatcher import ED2
 from sippy.Core.Exceptions import dump_exception
 from sippy.Time.Timeout import Timeout
 from sippy.Time.MonoTime import MonoTime
+from sippy.SipConf import MyPort
 
 class AsyncSender(Thread):
     userv = None
 
     def __init__(self, userv):
         Thread.__init__(self)
         self.userv = userv
@@ -121,50 +122,65 @@
                     continue
                 else:
                     dump_exception('Udp_server: unhandled exception when receiving incoming data')
                     sleep(1)
                     continue
             if self.userv.uopts.family == socket.AF_INET6:
                 address = ('[%s]' % address[0], address[1])
-            ED2.callFromThread(self.userv.handle_read, data, address, rtime)
+            if not self.userv.uopts.direct_dispatch:
+                ED2.callFromThread(self.userv.handle_read, data, address, rtime)
+            else:
+                self.userv.handle_read(data, address, rtime)
         self.userv = None
 
 _DEFAULT_FLAGS = socket.SO_REUSEADDR
 if hasattr(socket, 'SO_REUSEPORT'):
     _DEFAULT_FLAGS |= socket.SO_REUSEPORT
 _DEFAULT_NWORKERS = 30
 
 class Udp_server_opts(object):
     laddress = None
     data_callback = None
+    direct_dispatch = False
     family = None
     flags = _DEFAULT_FLAGS
-    nworkers = None
+    nworkers = _DEFAULT_NWORKERS
     ploss_out_rate = 0.0
     pdelay_out_max = 0.0
     ploss_in_rate = 0.0
     pdelay_in_max = 0.0
 
     def __init__(self, laddress, data_callback, family = None, o = None):
-        if o == None:
-            if family == None:
-                if laddress != None and laddress[0].startswith('['):
-                    family = socket.AF_INET6
-                    laddress = (laddress[0][1:-1], laddress[1])
-                else:
-                    family = socket.AF_INET
-            self.family = family
-            self.laddress = laddress
-            self.data_callback = data_callback
-        else:
+        if o != None:
             self.laddress, self.data_callback, self.family, self.nworkers, self.flags, \
               self.ploss_out_rate, self.pdelay_out_max, self.ploss_in_rate, \
               self.pdelay_in_max = o.laddress, o.data_callback, o.family, \
               o.nworkers, o.flags, o.ploss_out_rate, o.pdelay_out_max, o.ploss_in_rate, \
               o.pdelay_in_max
+            return
+        if family == None:
+            if laddress != None and laddress[0].startswith('['):
+                family = socket.AF_INET6
+                laddress = (laddress[0][1:-1], laddress[1])
+            else:
+                family = socket.AF_INET
+        self.family = family
+        self.laddress = laddress
+        self.data_callback = data_callback
+
+    def getSockOpts(self):
+        sockopts = []
+        if self.family == socket.AF_INET6 and self.isWildCard():
+            sockopts.append((socket.IPPROTO_IPV6, socket.IPV6_V6ONLY, 1))
+        if (self.flags & socket.SO_REUSEADDR) != 0:
+            sockopts.append((socket.SOL_SOCKET, socket.SO_REUSEADDR, 1))
+        if self.nworkers > 1 and hasattr(socket, 'SO_REUSEPORT') and \
+          (self.flags & socket.SO_REUSEPORT) != 0:
+            sockopts.append((socket.SOL_SOCKET, socket.SO_REUSEPORT, 1))
+        return sockopts
 
     def getCopy(self):
         return self.__class__(None, None, o = self)
 
     def getSIPaddr(self):
         if self.family == socket.AF_INET:
             return self.laddress
@@ -191,33 +207,31 @@
         self.skt = socket.socket(self.uopts.family, socket.SOCK_DGRAM)
         if self.uopts.laddress != None:
             ai = socket.getaddrinfo(self.uopts.laddress[0], None, self.uopts.family)
             if self.uopts.family == socket.AF_INET:
                 address = (ai[0][4][0], self.uopts.laddress[1])
             else:
                 address = (ai[0][4][0], self.uopts.laddress[1], ai[0][4][2], ai[0][4][3])
-            if (self.uopts.flags & socket.SO_REUSEADDR) != 0:
-                self.skt.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
-            if hasattr(socket, 'SO_REUSEPORT') and \
-              (self.uopts.flags & socket.SO_REUSEPORT) != 0:
-                self.skt.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEPORT, 1)
+            for so_val in self.uopts.getSockOpts():
+                self.skt.setsockopt(*so_val)
+            if isinstance(address[1], MyPort):
+                # XXX with some python 3.10 version I am getting
+                # TypeError: 'MyPort' object cannot be interpreted as an integer
+                # might be something inside socket.bind?
+                address = (address[0], int(address[1]))
             self.skt.bind(address)
             if self.uopts.laddress[1] == 0:
                 self.uopts.laddress = self.skt.getsockname()
         self.sendqueue = []
         self.stats = [0, 0, 0]
         self.wi_available = Condition()
         self.wi = []
         self.asenders = []
         self.areceivers = []
-        if self.uopts.nworkers == None:
-            nworkers = _DEFAULT_NWORKERS
-        else:
-            nworkers = self.uopts.nworkers
-        for i in range(0, nworkers):
+        for i in range(0, self.uopts.nworkers):
             self.asenders.append(AsyncSender(self))
             self.areceivers.append(AsyncReceiver(self))
 
     def send_to(self, data, address, delayed = False):
         if not isinstance(address, tuple):
             raise Exception('Invalid address, not a tuple: %s' % str(address))
         if not isinstance(data, bytes):
```

### Comparing `sippy-2.0.2/sippy/XMPP_server.py` & `sippy-2.1.0/sippy/XMPP_server.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/b2bua_radius.py` & `sippy-2.1.0/sippy/b2bua_radius.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python2
+#!/usr/bin/env python
 #
 # Copyright (c) 2003-2005 Maxim Sobolev. All rights reserved.
 # Copyright (c) 2006-2014 Sippy Software, Inc. All rights reserved.
 #
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without modification,
@@ -156,15 +156,15 @@
                     except:
                         self.uaA.recvEvent(CCEventFail((400, 'Malformed SDP Body'), rtime = event.rtime))
                         self.state = CCStateDead
                         return
                     allowed_pts = self.global_config['_allowed_pts']
                     for sect in body.content.sections:
                         mbody = sect.m_header
-                        if mbody.transport.lower() not in ('rtp/avp', 'rtp/savp'):
+                        if mbody.transport.lower() not in Rtp_proxy_session.AV_TRTYPES:
                             continue
                         old_len = len(mbody.formats)
                         mbody.formats = [x for x in mbody.formats if x in allowed_pts]
                         if len(mbody.formats) == 0:
                             self.uaA.recvEvent(CCEventFail((488, 'Not Acceptable Here')))
                             self.state = CCStateDead
                             return
```

### Comparing `sippy-2.0.2/sippy/b2bua_simple.py` & `sippy-2.1.0/sippy/b2bua_simple.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python2
+#!/usr/bin/env python
 #
 # Copyright (c) 2003-2005 Maxim Sobolev. All rights reserved.
 # Copyright (c) 2006-2014 Sippy Software, Inc. All rights reserved.
 #
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without modification,
```

### Comparing `sippy-2.0.2/sippy/dictionary` & `sippy-2.1.0/sippy/dictionary`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy/misc.py` & `sippy-2.1.0/sippy/misc.py`

 * *Files identical despite different names*

### Comparing `sippy-2.0.2/sippy.egg-info/PKG-INFO` & `sippy-2.1.0/sippy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: sippy
-Version: 2.0.2
+Version: 2.1.0
 Summary: RFC3261 SIP Stack and Back-to-Back User Agent (B2BUA)
 Home-page: http://www.b2bua.org/
 Author: Sippy Software, Inc.
 Author-email: sobomax@sippysoft.com
 License: BSD
 Keywords: sip,b2bua,voip,rfc3261,sippy
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: ElPeriodic>=1.1
+Requires-Dist: pycryptodome
 
 [![Build Status@GitHub](https://github.com/sippy/b2bua/workflows/Check%20Python%20Wheels/badge.svg?branch=master)](https://github.com/sippy/b2bua/actions?query=branch%3Amaster++)
 
 # Sippy B2BUA
 
 Sippy B2BUA is a [RFC3261](https://www.ietf.org/rfc/rfc3261.txt)-compliant
 Session Initiation Protocol (SIP) stack and
@@ -47,19 +49,19 @@
 - Simple and clean, yet flexible, internal design making implementing new
   features and services easy
 - Sippy B2BUA could be easily combined with other Open Source software, such as
   SIP Express Router / OpenSIPS to build complete softswitch solution
 
 ## Installation
 
-### Install libelperiodic (if not installed)
+### Install latest stable version
 
-`pip install ElPeriodic`
+`pip install sippy`
 
-### Install B2BUA
+### Install latest development version
 
 `pip install git+https://github.com/sippy/b2bua`
 
 ## Running
 
 To get started, you can use the b2bua_simple implementation. The following
 example will cause the b2bua run in the foreground so you can see the SIP
```

### Comparing `sippy-2.0.2/sippy.egg-info/SOURCES.txt` & `sippy-2.1.0/sippy.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 requirements.txt
 setup.py
 sippy/B2BRoute.py
 sippy/CCEvents.py
 sippy/CLIManager.py
 sippy/ESipHeaderCSV.py
 sippy/ESipHeaderIgnore.py
-sippy/ESipParseException.py
 sippy/External_command.py
 sippy/FakeAccounting.py
 sippy/MsgBody.py
+sippy/MultipartMixBody.py
 sippy/MyConfigParser.py
 sippy/RadiusAccounting.py
 sippy/RadiusAuthorisation.py
 sippy/Radius_client.py
 sippy/Rtp_proxy_client.py
 sippy/Rtp_proxy_client_local.py
 sippy/Rtp_proxy_client_net.py
@@ -103,14 +103,17 @@
 sippy.egg-info/dependency_links.txt
 sippy.egg-info/entry_points.txt
 sippy.egg-info/requires.txt
 sippy.egg-info/top_level.txt
 sippy/Core/EventDispatcher.py
 sippy/Core/Exceptions.py
 sippy/Core/__init__.py
+sippy/Exceptions/RtpProxyError.py
+sippy/Exceptions/SipParseError.py
+sippy/Exceptions/__init__.py
 sippy/Math/__init__.py
 sippy/Math/recfilter.py
 sippy/Security/SipNonce.py
 sippy/Security/__init__.py
 sippy/Time/MonoTime.py
 sippy/Time/Timeout.py
 sippy/Time/__init__.py
```

### Comparing `sippy-2.0.2/tests/test_SdbBody.py` & `sippy-2.1.0/tests/test_SdbBody.py`

 * *Files identical despite different names*

