# Comparing `tmp/ANX-0.7.9.tar.gz` & `tmp/ANX-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ANX-0.7.9.tar", last modified: Thu May 16 09:05:58 2024, max compression
+gzip compressed data, was "ANX-0.8.0.tar", last modified: Thu May 23 07:49:20 2024, max compression
```

## Comparing `ANX-0.7.9.tar` & `ANX-0.8.0.tar`

### file list

```diff
@@ -1,166 +1,166 @@
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-16 09:05:58.190824 ANX-0.7.9/
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-16 09:05:58.150524 ANX-0.7.9/ANX.egg-info/
--rw-r--r--   0 1a         (501) staff       (20)      125 2024-05-16 09:05:58.000000 ANX-0.7.9/ANX.egg-info/PKG-INFO
--rw-r--r--   0 1a         (501) staff       (20)     4882 2024-05-16 09:05:58.000000 ANX-0.7.9/ANX.egg-info/SOURCES.txt
--rw-r--r--   0 1a         (501) staff       (20)        1 2024-05-16 09:05:58.000000 ANX-0.7.9/ANX.egg-info/dependency_links.txt
--rw-r--r--   0 1a         (501) staff       (20)      108 2024-05-16 09:05:58.000000 ANX-0.7.9/ANX.egg-info/requires.txt
--rw-r--r--   0 1a         (501) staff       (20)       10 2024-05-16 09:05:58.000000 ANX-0.7.9/ANX.egg-info/top_level.txt
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-16 09:05:58.152641 ANX-0.7.9/AndroidQQ/
--rw-r--r--   0 1a         (501) staff       (20)    34955 2024-05-16 09:04:26.000000 ANX-0.7.9/AndroidQQ/Android.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-16 09:05:58.153091 ANX-0.7.9/AndroidQQ/Echo/
--rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/Echo/Tcp.py
--rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/Echo/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     4522 2024-05-15 01:55:22.000000 ANX-0.7.9/AndroidQQ/Tcp.py
--rw-r--r--   0 1a         (501) staff       (20)       71 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-16 09:05:58.157266 ANX-0.7.9/AndroidQQ/http/
--rw-r--r--   0 1a         (501) staff       (20)     2195 2024-04-08 06:23:23.000000 ANX-0.7.9/AndroidQQ/http/ClientKey.py
--rw-r--r--   0 1a         (501) staff       (20)      138 2024-04-08 05:21:16.000000 ANX-0.7.9/AndroidQQ/http/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     2009 2024-04-08 05:37:11.000000 ANX-0.7.9/AndroidQQ/http/accounts.py
--rw-r--r--   0 1a         (501) staff       (20)      820 2024-04-08 05:31:10.000000 ANX-0.7.9/AndroidQQ/http/cip.py
--rw-r--r--   0 1a         (501) staff       (20)     4061 2024-04-08 05:46:08.000000 ANX-0.7.9/AndroidQQ/http/friends.py
--rw-r--r--   0 1a         (501) staff       (20)     4734 2024-04-11 04:47:50.000000 ANX-0.7.9/AndroidQQ/http/game_credit.py
--rw-r--r--   0 1a         (501) staff       (20)      422 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/http/headers.py
--rw-r--r--   0 1a         (501) staff       (20)     7243 2024-04-25 09:25:24.000000 ANX-0.7.9/AndroidQQ/http/level.py
--rw-r--r--   0 1a         (501) staff       (20)    11548 2024-04-25 09:27:50.000000 ANX-0.7.9/AndroidQQ/http/music.py
--rw-r--r--   0 1a         (501) staff       (20)     1499 2024-04-08 05:42:12.000000 ANX-0.7.9/AndroidQQ/http/qqsignin.py
--rw-r--r--   0 1a         (501) staff       (20)     1325 2024-04-08 05:50:32.000000 ANX-0.7.9/AndroidQQ/http/weishi.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-16 09:05:58.157544 ANX-0.7.9/AndroidQQ/im/
--rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/im/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-16 09:05:58.157683 ANX-0.7.9/AndroidQQ/im/oidb/
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-16 09:05:58.158045 ANX-0.7.9/AndroidQQ/im/oidb/OidbSvc_0xc96/
--rw-r--r--   0 1a         (501) staff       (20)     2797 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/im/oidb/OidbSvc_0xc96/OidbSvc_0xc96_pb2.py
--rw-r--r--   0 1a         (501) staff       (20)       34 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/im/oidb/OidbSvc_0xc96/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/im/oidb/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-16 09:05:58.158578 ANX-0.7.9/AndroidQQ/im/oidb/cmd0x88d/
--rw-r--r--   0 1a         (501) staff       (20)       30 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/im/oidb/cmd0x88d/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     2139 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/im/oidb/cmd0x88d/oidb_0x88d_pb2.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-16 09:05:58.159591 ANX-0.7.9/AndroidQQ/im/oidb/cmd0x922/
--rw-r--r--   0 1a         (501) staff       (20)     1343 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/im/oidb/cmd0x922/PushInfo_pb2.py
--rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/im/oidb/cmd0x922/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1542 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/im/oidb/cmd0x922/cmd0x922_pb2.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-16 09:05:58.160166 ANX-0.7.9/AndroidQQ/im/oidb/cmd0xeb8/
--rw-r--r--   0 1a         (501) staff       (20)       28 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/im/oidb/cmd0xeb8/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1872 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/im/oidb/cmd0xeb8/cmd0xeb8_pb2.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-16 09:05:58.160716 ANX-0.7.9/AndroidQQ/im/oidb/oidb_0xc05/
--rw-r--r--   0 1a         (501) staff       (20)       30 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/im/oidb/oidb_0xc05/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     2603 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/im/oidb/oidb_0xc05/oidb_0xc05_pb2.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-16 09:05:58.161401 ANX-0.7.9/AndroidQQ/im/oidb/oidb_sso/
--rw-r--r--   0 1a         (501) staff       (20)       27 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/im/oidb/oidb_sso/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1468 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/im/oidb/oidb_sso/oidb_sso_pb2.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-16 09:05:58.162034 ANX-0.7.9/AndroidQQ/im/oidb/qqconnect/
--rw-r--r--   0 1a         (501) staff       (20)       29 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/im/oidb/qqconnect/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     2618 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/im/oidb/qqconnect/qqconnect_pb2.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-16 09:05:58.163070 ANX-0.7.9/AndroidQQ/im/oidb/scanlogin/
--rw-r--r--   0 1a         (501) staff       (20)       29 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/im/oidb/scanlogin/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1385 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/im/oidb/scanlogin/scanlogin_pb2.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-16 09:05:58.163398 ANX-0.7.9/AndroidQQ/log/
--rw-r--r--   0 1a         (501) staff       (20)       33 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/log/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-16 09:05:58.167336 ANX-0.7.9/AndroidQQ/pack/
--rw-r--r--   0 1a         (501) staff       (20)      395 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/pack/Heartbeat_Alive.py
--rw-r--r--   0 1a         (501) staff       (20)      872 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/pack/MQUpdateSvc_com_qq_ti_web_scanlogin.py
--rw-r--r--   0 1a         (501) staff       (20)      733 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/pack/MQUpdateSvc_com_qq_vip_zb_web_OidbSvc_0xdfa_0.py
--rw-r--r--   0 1a         (501) staff       (20)     1368 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/pack/OidbSvc_0x88d_1.py
--rw-r--r--   0 1a         (501) staff       (20)      986 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/pack/OidbSvc_0xc05.py
--rw-r--r--   0 1a         (501) staff       (20)     1141 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/pack/OidbSvc_0xc96.py
--rw-r--r--   0 1a         (501) staff       (20)      872 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/pack/OidbSvc_0xeb8.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-16 09:05:58.169341 ANX-0.7.9/AndroidQQ/pack/SQQzoneSvc/
--rw-r--r--   0 1a         (501) staff       (20)       94 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/pack/SQQzoneSvc/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1124 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/pack/SQQzoneSvc/delUgc.py
--rw-r--r--   0 1a         (501) staff       (20)     2637 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/pack/SQQzoneSvc/like.py
--rw-r--r--   0 1a         (501) staff       (20)     2631 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/pack/SQQzoneSvc/publishmood.py
--rw-r--r--   0 1a         (501) staff       (20)     2152 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/pack/SQQzoneSvc/shuoshuo.py
--rw-r--r--   0 1a         (501) staff       (20)     1116 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/pack/StatSvc_register.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-16 09:05:58.169766 ANX-0.7.9/AndroidQQ/pack/SummaryCard/
--rw-r--r--   0 1a         (501) staff       (20)     1349 2024-03-07 10:14:41.000000 ANX-0.7.9/AndroidQQ/pack/SummaryCard/ReqSummaryCard.py
--rw-r--r--   0 1a         (501) staff       (20)       29 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/pack/SummaryCard/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)      402 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/pack/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1383 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/pack/friendlist.py
--rw-r--r--   0 1a         (501) staff       (20)      543 2024-03-06 13:46:02.000000 ANX-0.7.9/AndroidQQ/pack/test.py
--rw-r--r--   0 1a         (501) staff       (20)    46467 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/pack/trpc_metaverse_mob_proxy_svr_MobProxy_SsoHandle.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-16 09:05:58.170348 ANX-0.7.9/AndroidQQ/proto/
--rw-r--r--   0 1a         (501) staff       (20)     4301 2024-02-12 04:07:38.000000 ANX-0.7.9/AndroidQQ/proto/IM_r_pb2.py
--rw-r--r--   0 1a         (501) staff       (20)       67 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/proto/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1308 2023-10-29 17:25:21.000000 ANX-0.7.9/AndroidQQ/proto/wtlogin_pb2.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-16 09:05:58.172561 ANX-0.7.9/AndroidQQ/struct/
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-16 09:05:58.173711 ANX-0.7.9/AndroidQQ/struct/Avatarlnfo/
--rw-r--r--   0 1a         (501) staff       (20)      444 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/Avatarlnfo/DestQQHeadInfo.py
--rw-r--r--   0 1a         (501) staff       (20)     1061 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/Avatarlnfo/QQHeadInfo.py
--rw-r--r--   0 1a         (501) staff       (20)      853 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/Avatarlnfo/QQHeadUrlReq.py
--rw-r--r--   0 1a         (501) staff       (20)      673 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/Avatarlnfo/QQHeadUrlResp.py
--rw-r--r--   0 1a         (501) staff       (20)     1028 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/Avatarlnfo/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)      894 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/MessageSvc.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-16 09:05:58.174288 ANX-0.7.9/AndroidQQ/struct/NS_MOBILE_COMM/
--rw-r--r--   0 1a         (501) staff       (20)      373 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/NS_MOBILE_COMM/UgcRightInfo.py
--rw-r--r--   0 1a         (501) staff       (20)       28 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/NS_MOBILE_COMM/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-16 09:05:58.179786 ANX-0.7.9/AndroidQQ/struct/NS_MOBILE_FEEDS/
--rw-r--r--   0 1a         (501) staff       (20)       70 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/NS_MOBILE_FEEDS/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     3064 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_comm.py
--rw-r--r--   0 1a         (501) staff       (20)     1565 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_operation.py
--rw-r--r--   0 1a         (501) staff       (20)      565 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_userinfo.py
--rw-r--r--   0 1a         (501) staff       (20)      895 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/NS_MOBILE_FEEDS/mobile_applist_req.py
--rw-r--r--   0 1a         (501) staff       (20)     1789 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/NS_MOBILE_FEEDS/mobile_applist_rsp.py
--rw-r--r--   0 1a         (501) staff       (20)      451 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/NS_MOBILE_FEEDS/s_arkshare.py
--rw-r--r--   0 1a         (501) staff       (20)      673 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/NS_MOBILE_FEEDS/s_outshare.py
--rw-r--r--   0 1a         (501) staff       (20)      728 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/NS_MOBILE_FEEDS/s_picurl.py
--rw-r--r--   0 1a         (501) staff       (20)      249 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/NS_MOBILE_FEEDS/s_user.py
--rw-r--r--   0 1a         (501) staff       (20)     1163 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/NS_MOBILE_FEEDS/single_feed.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-16 09:05:58.182512 ANX-0.7.9/AndroidQQ/struct/NS_MOBILE_OPERATION/
--rw-r--r--   0 1a         (501) staff       (20)      479 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/NS_MOBILE_OPERATION/Source.py
--rw-r--r--   0 1a         (501) staff       (20)      187 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/NS_MOBILE_OPERATION/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)      656 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/NS_MOBILE_OPERATION/cmshow_active_result.py
--rw-r--r--   0 1a         (501) staff       (20)     1161 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_delugc_req.py
--rw-r--r--   0 1a         (501) staff       (20)     1300 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_like_req.py
--rw-r--r--   0 1a         (501) staff       (20)      560 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_like_rsp.py
--rw-r--r--   0 1a         (501) staff       (20)     3031 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_publishmood_req.py
--rw-r--r--   0 1a         (501) staff       (20)      503 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_publishmood_rsp.py
--rw-r--r--   0 1a         (501) staff       (20)      594 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/OidbSvc.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-16 09:05:58.184945 ANX-0.7.9/AndroidQQ/struct/QMF_PROTOCAL/
--rw-r--r--   0 1a         (501) staff       (20)      504 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/QMF_PROTOCAL/QmfBusiControl.py
--rw-r--r--   0 1a         (501) staff       (20)      630 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/QMF_PROTOCAL/QmfClientIpInfo.py
--rw-r--r--   0 1a         (501) staff       (20)      714 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/QMF_PROTOCAL/QmfDownstream.py
--rw-r--r--   0 1a         (501) staff       (20)      526 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/QMF_PROTOCAL/QmfTokenInfo.py
--rw-r--r--   0 1a         (501) staff       (20)     1180 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/QMF_PROTOCAL/QmfUpstream.py
--rw-r--r--   0 1a         (501) staff       (20)      489 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/QMF_PROTOCAL/RetryInfo.py
--rw-r--r--   0 1a         (501) staff       (20)       87 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/QMF_PROTOCAL/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-16 09:05:58.185354 ANX-0.7.9/AndroidQQ/struct/QQService/
--rw-r--r--   0 1a         (501) staff       (20)     1112 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/QQService/SvcReqGetDevLoginInfo.py
--rw-r--r--   0 1a         (501) staff       (20)      878 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/QQService/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1043 2024-05-10 20:44:20.000000 ANX-0.7.9/AndroidQQ/struct/StatSvc.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-16 09:05:58.186763 ANX-0.7.9/AndroidQQ/struct/SummaryCard/
--rw-r--r--   0 1a         (501) staff       (20)     2861 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/SummaryCard/ReqSummaryCard.py
--rw-r--r--   0 1a         (501) staff       (20)      493 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/SummaryCard/UserLocaleInfo.py
--rw-r--r--   0 1a         (501) staff       (20)       61 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/SummaryCard/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)    15568 2024-03-05 18:40:23.000000 ANX-0.7.9/AndroidQQ/struct/Tlv.py
--rw-r--r--   0 1a         (501) staff       (20)     4784 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/Tlv_res.py
--rw-r--r--   0 1a         (501) staff       (20)      131 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-16 09:05:58.187479 ANX-0.7.9/AndroidQQ/struct/cooperation/
--rw-r--r--   0 1a         (501) staff       (20)       23 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/cooperation/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-16 09:05:58.187987 ANX-0.7.9/AndroidQQ/struct/cooperation/qzone/
--rw-r--r--   0 1a         (501) staff       (20)     4558 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/cooperation/qzone/WNSStream.py
--rw-r--r--   0 1a         (501) staff       (20)       26 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/cooperation/qzone/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-16 09:05:58.188322 ANX-0.7.9/AndroidQQ/struct/feedcomponent/
--rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/feedcomponent/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1482 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/feedcomponent/model.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-16 09:05:58.188630 ANX-0.7.9/AndroidQQ/struct/friendlist/
--rw-r--r--   0 1a         (501) staff       (20)     2842 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/friendlist/AddFriendReq.py
--rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/friendlist/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     7428 2024-03-07 10:14:48.000000 ANX-0.7.9/AndroidQQ/struct/head.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-16 09:05:58.188995 ANX-0.7.9/AndroidQQ/struct/push/
--rw-r--r--   0 1a         (501) staff       (20)     3536 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/push/SvcReqRegister.py
--rw-r--r--   0 1a         (501) staff       (20)     2084 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/push/SvcRespRegister.py
--rw-r--r--   0 1a         (501) staff       (20)       31 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/struct/push/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)    27313 2024-03-05 18:40:23.000000 ANX-0.7.9/AndroidQQ/struct/wtlogin.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-16 09:05:58.189731 ANX-0.7.9/AndroidQQ/utils/
--rw-r--r--   0 1a         (501) staff       (20)       20 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/utils/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)      523 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/utils/build_device.py
--rw-r--r--   0 1a         (501) staff       (20)     1140 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/utils/ecdh.py
--rw-r--r--   0 1a         (501) staff       (20)     1379 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/utils/sso_server.py
--rw-r--r--   0 1a         (501) staff       (20)      735 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/utils/tool.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-16 09:05:58.189885 ANX-0.7.9/AndroidQQ/wlogin_sdk/
--rw-r--r--   0 1a         (501) staff       (20)       25 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/wlogin_sdk/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-16 09:05:58.190056 ANX-0.7.9/AndroidQQ/wlogin_sdk/request/
--rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.9/AndroidQQ/wlogin_sdk/request/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)      125 2024-05-16 09:05:58.190429 ANX-0.7.9/PKG-INFO
--rw-r--r--   0 1a         (501) staff       (20)       34 2023-08-04 12:41:32.000000 ANX-0.7.9/README.md
--rw-r--r--   0 1a         (501) staff       (20)       38 2024-05-16 09:05:58.190926 ANX-0.7.9/setup.cfg
--rw-r--r--   0 1a         (501) staff       (20)      601 2024-05-16 09:05:50.000000 ANX-0.7.9/setup.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.837765 ANX-0.8.0/
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.803773 ANX-0.8.0/ANX.egg-info/
+-rw-r--r--   0 1a         (501) staff       (20)      125 2024-05-23 07:49:20.000000 ANX-0.8.0/ANX.egg-info/PKG-INFO
+-rw-r--r--   0 1a         (501) staff       (20)     4882 2024-05-23 07:49:20.000000 ANX-0.8.0/ANX.egg-info/SOURCES.txt
+-rw-r--r--   0 1a         (501) staff       (20)        1 2024-05-23 07:49:20.000000 ANX-0.8.0/ANX.egg-info/dependency_links.txt
+-rw-r--r--   0 1a         (501) staff       (20)      108 2024-05-23 07:49:20.000000 ANX-0.8.0/ANX.egg-info/requires.txt
+-rw-r--r--   0 1a         (501) staff       (20)       10 2024-05-23 07:49:20.000000 ANX-0.8.0/ANX.egg-info/top_level.txt
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.804326 ANX-0.8.0/AndroidQQ/
+-rw-r--r--   0 1a         (501) staff       (20)    34971 2024-05-23 07:48:15.000000 ANX-0.8.0/AndroidQQ/Android.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.804689 ANX-0.8.0/AndroidQQ/Echo/
+-rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/Echo/Tcp.py
+-rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/Echo/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     4522 2024-05-15 01:55:22.000000 ANX-0.8.0/AndroidQQ/Tcp.py
+-rw-r--r--   0 1a         (501) staff       (20)       71 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.807541 ANX-0.8.0/AndroidQQ/http/
+-rw-r--r--   0 1a         (501) staff       (20)     2195 2024-04-08 06:23:23.000000 ANX-0.8.0/AndroidQQ/http/ClientKey.py
+-rw-r--r--   0 1a         (501) staff       (20)      138 2024-04-08 05:21:16.000000 ANX-0.8.0/AndroidQQ/http/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     2009 2024-04-08 05:37:11.000000 ANX-0.8.0/AndroidQQ/http/accounts.py
+-rw-r--r--   0 1a         (501) staff       (20)      820 2024-04-08 05:31:10.000000 ANX-0.8.0/AndroidQQ/http/cip.py
+-rw-r--r--   0 1a         (501) staff       (20)     4061 2024-04-08 05:46:08.000000 ANX-0.8.0/AndroidQQ/http/friends.py
+-rw-r--r--   0 1a         (501) staff       (20)     4734 2024-05-19 23:14:02.000000 ANX-0.8.0/AndroidQQ/http/game_credit.py
+-rw-r--r--   0 1a         (501) staff       (20)      422 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/http/headers.py
+-rw-r--r--   0 1a         (501) staff       (20)     7243 2024-04-25 09:25:24.000000 ANX-0.8.0/AndroidQQ/http/level.py
+-rw-r--r--   0 1a         (501) staff       (20)    11548 2024-04-25 09:27:50.000000 ANX-0.8.0/AndroidQQ/http/music.py
+-rw-r--r--   0 1a         (501) staff       (20)     1499 2024-04-08 05:42:12.000000 ANX-0.8.0/AndroidQQ/http/qqsignin.py
+-rw-r--r--   0 1a         (501) staff       (20)     1325 2024-04-08 05:50:32.000000 ANX-0.8.0/AndroidQQ/http/weishi.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.807762 ANX-0.8.0/AndroidQQ/im/
+-rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/im/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.807852 ANX-0.8.0/AndroidQQ/im/oidb/
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.808189 ANX-0.8.0/AndroidQQ/im/oidb/OidbSvc_0xc96/
+-rw-r--r--   0 1a         (501) staff       (20)     2797 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/im/oidb/OidbSvc_0xc96/OidbSvc_0xc96_pb2.py
+-rw-r--r--   0 1a         (501) staff       (20)       34 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/im/oidb/OidbSvc_0xc96/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/im/oidb/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.808710 ANX-0.8.0/AndroidQQ/im/oidb/cmd0x88d/
+-rw-r--r--   0 1a         (501) staff       (20)       30 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/im/oidb/cmd0x88d/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     2139 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/im/oidb/cmd0x88d/oidb_0x88d_pb2.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.810253 ANX-0.8.0/AndroidQQ/im/oidb/cmd0x922/
+-rw-r--r--   0 1a         (501) staff       (20)     1343 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/im/oidb/cmd0x922/PushInfo_pb2.py
+-rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/im/oidb/cmd0x922/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1542 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/im/oidb/cmd0x922/cmd0x922_pb2.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.810772 ANX-0.8.0/AndroidQQ/im/oidb/cmd0xeb8/
+-rw-r--r--   0 1a         (501) staff       (20)       28 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/im/oidb/cmd0xeb8/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1872 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/im/oidb/cmd0xeb8/cmd0xeb8_pb2.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.811313 ANX-0.8.0/AndroidQQ/im/oidb/oidb_0xc05/
+-rw-r--r--   0 1a         (501) staff       (20)       30 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/im/oidb/oidb_0xc05/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     2603 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/im/oidb/oidb_0xc05/oidb_0xc05_pb2.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.811830 ANX-0.8.0/AndroidQQ/im/oidb/oidb_sso/
+-rw-r--r--   0 1a         (501) staff       (20)       27 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/im/oidb/oidb_sso/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1468 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/im/oidb/oidb_sso/oidb_sso_pb2.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.812397 ANX-0.8.0/AndroidQQ/im/oidb/qqconnect/
+-rw-r--r--   0 1a         (501) staff       (20)       29 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/im/oidb/qqconnect/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     2618 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/im/oidb/qqconnect/qqconnect_pb2.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.813382 ANX-0.8.0/AndroidQQ/im/oidb/scanlogin/
+-rw-r--r--   0 1a         (501) staff       (20)       29 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/im/oidb/scanlogin/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1385 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/im/oidb/scanlogin/scanlogin_pb2.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.813683 ANX-0.8.0/AndroidQQ/log/
+-rw-r--r--   0 1a         (501) staff       (20)       33 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/log/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.817493 ANX-0.8.0/AndroidQQ/pack/
+-rw-r--r--   0 1a         (501) staff       (20)      395 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/pack/Heartbeat_Alive.py
+-rw-r--r--   0 1a         (501) staff       (20)      872 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/pack/MQUpdateSvc_com_qq_ti_web_scanlogin.py
+-rw-r--r--   0 1a         (501) staff       (20)      733 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/pack/MQUpdateSvc_com_qq_vip_zb_web_OidbSvc_0xdfa_0.py
+-rw-r--r--   0 1a         (501) staff       (20)     1368 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/pack/OidbSvc_0x88d_1.py
+-rw-r--r--   0 1a         (501) staff       (20)      986 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/pack/OidbSvc_0xc05.py
+-rw-r--r--   0 1a         (501) staff       (20)     1141 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/pack/OidbSvc_0xc96.py
+-rw-r--r--   0 1a         (501) staff       (20)      872 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/pack/OidbSvc_0xeb8.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.819100 ANX-0.8.0/AndroidQQ/pack/SQQzoneSvc/
+-rw-r--r--   0 1a         (501) staff       (20)       94 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/pack/SQQzoneSvc/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1124 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/pack/SQQzoneSvc/delUgc.py
+-rw-r--r--   0 1a         (501) staff       (20)     2637 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/pack/SQQzoneSvc/like.py
+-rw-r--r--   0 1a         (501) staff       (20)     2631 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/pack/SQQzoneSvc/publishmood.py
+-rw-r--r--   0 1a         (501) staff       (20)     2152 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/pack/SQQzoneSvc/shuoshuo.py
+-rw-r--r--   0 1a         (501) staff       (20)     1116 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/pack/StatSvc_register.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.819512 ANX-0.8.0/AndroidQQ/pack/SummaryCard/
+-rw-r--r--   0 1a         (501) staff       (20)     1349 2024-03-07 10:14:41.000000 ANX-0.8.0/AndroidQQ/pack/SummaryCard/ReqSummaryCard.py
+-rw-r--r--   0 1a         (501) staff       (20)       29 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/pack/SummaryCard/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)      402 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/pack/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1383 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/pack/friendlist.py
+-rw-r--r--   0 1a         (501) staff       (20)      543 2024-03-06 13:46:02.000000 ANX-0.8.0/AndroidQQ/pack/test.py
+-rw-r--r--   0 1a         (501) staff       (20)    46467 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/pack/trpc_metaverse_mob_proxy_svr_MobProxy_SsoHandle.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.820230 ANX-0.8.0/AndroidQQ/proto/
+-rw-r--r--   0 1a         (501) staff       (20)     4301 2024-02-12 04:07:38.000000 ANX-0.8.0/AndroidQQ/proto/IM_r_pb2.py
+-rw-r--r--   0 1a         (501) staff       (20)       67 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/proto/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1308 2023-10-29 17:25:21.000000 ANX-0.8.0/AndroidQQ/proto/wtlogin_pb2.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.822502 ANX-0.8.0/AndroidQQ/struct/
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.823667 ANX-0.8.0/AndroidQQ/struct/Avatarlnfo/
+-rw-r--r--   0 1a         (501) staff       (20)      444 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/Avatarlnfo/DestQQHeadInfo.py
+-rw-r--r--   0 1a         (501) staff       (20)     1061 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/Avatarlnfo/QQHeadInfo.py
+-rw-r--r--   0 1a         (501) staff       (20)      853 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/Avatarlnfo/QQHeadUrlReq.py
+-rw-r--r--   0 1a         (501) staff       (20)      673 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/Avatarlnfo/QQHeadUrlResp.py
+-rw-r--r--   0 1a         (501) staff       (20)     1028 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/Avatarlnfo/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)      894 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/MessageSvc.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.824183 ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_COMM/
+-rw-r--r--   0 1a         (501) staff       (20)      373 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_COMM/UgcRightInfo.py
+-rw-r--r--   0 1a         (501) staff       (20)       28 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_COMM/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.827431 ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_FEEDS/
+-rw-r--r--   0 1a         (501) staff       (20)       70 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_FEEDS/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     3064 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_comm.py
+-rw-r--r--   0 1a         (501) staff       (20)     1565 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_operation.py
+-rw-r--r--   0 1a         (501) staff       (20)      565 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_userinfo.py
+-rw-r--r--   0 1a         (501) staff       (20)      895 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_FEEDS/mobile_applist_req.py
+-rw-r--r--   0 1a         (501) staff       (20)     1789 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_FEEDS/mobile_applist_rsp.py
+-rw-r--r--   0 1a         (501) staff       (20)      451 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_FEEDS/s_arkshare.py
+-rw-r--r--   0 1a         (501) staff       (20)      673 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_FEEDS/s_outshare.py
+-rw-r--r--   0 1a         (501) staff       (20)      728 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_FEEDS/s_picurl.py
+-rw-r--r--   0 1a         (501) staff       (20)      249 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_FEEDS/s_user.py
+-rw-r--r--   0 1a         (501) staff       (20)     1163 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_FEEDS/single_feed.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.829812 ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_OPERATION/
+-rw-r--r--   0 1a         (501) staff       (20)      479 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_OPERATION/Source.py
+-rw-r--r--   0 1a         (501) staff       (20)      187 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_OPERATION/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)      656 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_OPERATION/cmshow_active_result.py
+-rw-r--r--   0 1a         (501) staff       (20)     1161 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_delugc_req.py
+-rw-r--r--   0 1a         (501) staff       (20)     1300 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_like_req.py
+-rw-r--r--   0 1a         (501) staff       (20)      560 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_like_rsp.py
+-rw-r--r--   0 1a         (501) staff       (20)     3031 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_publishmood_req.py
+-rw-r--r--   0 1a         (501) staff       (20)      503 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_publishmood_rsp.py
+-rw-r--r--   0 1a         (501) staff       (20)      594 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/OidbSvc.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.832938 ANX-0.8.0/AndroidQQ/struct/QMF_PROTOCAL/
+-rw-r--r--   0 1a         (501) staff       (20)      504 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/QMF_PROTOCAL/QmfBusiControl.py
+-rw-r--r--   0 1a         (501) staff       (20)      630 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/QMF_PROTOCAL/QmfClientIpInfo.py
+-rw-r--r--   0 1a         (501) staff       (20)      714 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/QMF_PROTOCAL/QmfDownstream.py
+-rw-r--r--   0 1a         (501) staff       (20)      526 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/QMF_PROTOCAL/QmfTokenInfo.py
+-rw-r--r--   0 1a         (501) staff       (20)     1180 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/QMF_PROTOCAL/QmfUpstream.py
+-rw-r--r--   0 1a         (501) staff       (20)      489 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/QMF_PROTOCAL/RetryInfo.py
+-rw-r--r--   0 1a         (501) staff       (20)       87 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/QMF_PROTOCAL/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.833278 ANX-0.8.0/AndroidQQ/struct/QQService/
+-rw-r--r--   0 1a         (501) staff       (20)     1112 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/QQService/SvcReqGetDevLoginInfo.py
+-rw-r--r--   0 1a         (501) staff       (20)      878 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/QQService/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1043 2024-05-10 20:44:20.000000 ANX-0.8.0/AndroidQQ/struct/StatSvc.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.834214 ANX-0.8.0/AndroidQQ/struct/SummaryCard/
+-rw-r--r--   0 1a         (501) staff       (20)     2861 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/SummaryCard/ReqSummaryCard.py
+-rw-r--r--   0 1a         (501) staff       (20)      493 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/SummaryCard/UserLocaleInfo.py
+-rw-r--r--   0 1a         (501) staff       (20)       61 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/SummaryCard/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)    15568 2024-03-05 18:40:23.000000 ANX-0.8.0/AndroidQQ/struct/Tlv.py
+-rw-r--r--   0 1a         (501) staff       (20)     4784 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/Tlv_res.py
+-rw-r--r--   0 1a         (501) staff       (20)      131 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.834701 ANX-0.8.0/AndroidQQ/struct/cooperation/
+-rw-r--r--   0 1a         (501) staff       (20)       23 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/cooperation/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.835225 ANX-0.8.0/AndroidQQ/struct/cooperation/qzone/
+-rw-r--r--   0 1a         (501) staff       (20)     4558 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/cooperation/qzone/WNSStream.py
+-rw-r--r--   0 1a         (501) staff       (20)       26 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/cooperation/qzone/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.835514 ANX-0.8.0/AndroidQQ/struct/feedcomponent/
+-rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/feedcomponent/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1482 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/feedcomponent/model.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.835889 ANX-0.8.0/AndroidQQ/struct/friendlist/
+-rw-r--r--   0 1a         (501) staff       (20)     2842 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/friendlist/AddFriendReq.py
+-rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/friendlist/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     7428 2024-03-07 10:14:48.000000 ANX-0.8.0/AndroidQQ/struct/head.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.836317 ANX-0.8.0/AndroidQQ/struct/push/
+-rw-r--r--   0 1a         (501) staff       (20)     3536 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/push/SvcReqRegister.py
+-rw-r--r--   0 1a         (501) staff       (20)     2084 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/push/SvcRespRegister.py
+-rw-r--r--   0 1a         (501) staff       (20)       31 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/struct/push/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)    27313 2024-03-05 18:40:23.000000 ANX-0.8.0/AndroidQQ/struct/wtlogin.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.837132 ANX-0.8.0/AndroidQQ/utils/
+-rw-r--r--   0 1a         (501) staff       (20)       20 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/utils/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)      523 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/utils/build_device.py
+-rw-r--r--   0 1a         (501) staff       (20)     1140 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/utils/ecdh.py
+-rw-r--r--   0 1a         (501) staff       (20)     1379 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/utils/sso_server.py
+-rw-r--r--   0 1a         (501) staff       (20)      735 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/utils/tool.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.837295 ANX-0.8.0/AndroidQQ/wlogin_sdk/
+-rw-r--r--   0 1a         (501) staff       (20)       25 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/wlogin_sdk/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-05-23 07:49:20.837443 ANX-0.8.0/AndroidQQ/wlogin_sdk/request/
+-rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.8.0/AndroidQQ/wlogin_sdk/request/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)      125 2024-05-23 07:49:20.837611 ANX-0.8.0/PKG-INFO
+-rw-r--r--   0 1a         (501) staff       (20)       34 2023-08-04 12:41:32.000000 ANX-0.8.0/README.md
+-rw-r--r--   0 1a         (501) staff       (20)       38 2024-05-23 07:49:20.837818 ANX-0.8.0/setup.cfg
+-rw-r--r--   0 1a         (501) staff       (20)      601 2024-05-23 07:49:04.000000 ANX-0.8.0/setup.py
```

### Comparing `ANX-0.7.9/ANX.egg-info/SOURCES.txt` & `ANX-0.8.0/ANX.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/Android.py` & `ANX-0.8.0/AndroidQQ/Android.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,16 +244,16 @@
             self.info.UN_Tlv_list.userSt_Key = bytes.fromhex(json_data.get('T10E', ''))
             self.info.UN_Tlv_list.userStSig = bytes.fromhex(json_data.get('T114', ''))
             self.info.UN_Tlv_list.wtSessionTicket = bytes.fromhex(json_data['T133'])
             self.info.UN_Tlv_list.wtSessionTicketKey = bytes.fromhex(json_data['T134'])
 
         if json_data.get('cookies', None) is None:
             return
-        self.info.cookies.skey = json_data['cookies']['skey']
-        self.info.cookies.p_skey = json_data['cookies']['p_skey']
+        self.info.cookies.skey = json_data['cookies'].get('skey', '')
+        self.info.cookies.p_skey = json_data['cookies'].get('p_skey', {})
         self.info.cookies.client_key = json_data.get('cookies', {}).get('client_key', '')
 
         # self.info.cookies.client_key = json_data['cookies']['client_key']
 
     def get_tokenA(self):
         # print('get_tokenA', self.info)
         tokenA = {
```

### Comparing `ANX-0.7.9/AndroidQQ/Tcp.py` & `ANX-0.8.0/AndroidQQ/Tcp.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/http/ClientKey.py` & `ANX-0.8.0/AndroidQQ/http/ClientKey.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/http/accounts.py` & `ANX-0.8.0/AndroidQQ/http/accounts.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/http/cip.py` & `ANX-0.8.0/AndroidQQ/http/cip.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/http/friends.py` & `ANX-0.8.0/AndroidQQ/http/friends.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/http/game_credit.py` & `ANX-0.8.0/AndroidQQ/http/game_credit.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/http/level.py` & `ANX-0.8.0/AndroidQQ/http/level.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/http/music.py` & `ANX-0.8.0/AndroidQQ/http/music.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/http/qqsignin.py` & `ANX-0.8.0/AndroidQQ/http/qqsignin.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/http/weishi.py` & `ANX-0.8.0/AndroidQQ/http/weishi.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/im/oidb/OidbSvc_0xc96/OidbSvc_0xc96_pb2.py` & `ANX-0.8.0/AndroidQQ/im/oidb/OidbSvc_0xc96/OidbSvc_0xc96_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/im/oidb/cmd0x88d/oidb_0x88d_pb2.py` & `ANX-0.8.0/AndroidQQ/im/oidb/cmd0x88d/oidb_0x88d_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/im/oidb/cmd0x922/PushInfo_pb2.py` & `ANX-0.8.0/AndroidQQ/im/oidb/cmd0x922/PushInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/im/oidb/cmd0x922/cmd0x922_pb2.py` & `ANX-0.8.0/AndroidQQ/im/oidb/cmd0x922/cmd0x922_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/im/oidb/cmd0xeb8/cmd0xeb8_pb2.py` & `ANX-0.8.0/AndroidQQ/im/oidb/cmd0xeb8/cmd0xeb8_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/im/oidb/oidb_0xc05/oidb_0xc05_pb2.py` & `ANX-0.8.0/AndroidQQ/im/oidb/oidb_0xc05/oidb_0xc05_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/im/oidb/oidb_sso/oidb_sso_pb2.py` & `ANX-0.8.0/AndroidQQ/im/oidb/oidb_sso/oidb_sso_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/im/oidb/qqconnect/qqconnect_pb2.py` & `ANX-0.8.0/AndroidQQ/im/oidb/qqconnect/qqconnect_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/im/oidb/scanlogin/scanlogin_pb2.py` & `ANX-0.8.0/AndroidQQ/im/oidb/scanlogin/scanlogin_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/pack/MQUpdateSvc_com_qq_ti_web_scanlogin.py` & `ANX-0.8.0/AndroidQQ/pack/MQUpdateSvc_com_qq_ti_web_scanlogin.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/pack/MQUpdateSvc_com_qq_vip_zb_web_OidbSvc_0xdfa_0.py` & `ANX-0.8.0/AndroidQQ/pack/MQUpdateSvc_com_qq_vip_zb_web_OidbSvc_0xdfa_0.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/pack/OidbSvc_0x88d_1.py` & `ANX-0.8.0/AndroidQQ/pack/OidbSvc_0x88d_1.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/pack/OidbSvc_0xc05.py` & `ANX-0.8.0/AndroidQQ/pack/OidbSvc_0xc05.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/pack/OidbSvc_0xc96.py` & `ANX-0.8.0/AndroidQQ/pack/OidbSvc_0xc96.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/pack/OidbSvc_0xeb8.py` & `ANX-0.8.0/AndroidQQ/pack/OidbSvc_0xeb8.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/pack/SQQzoneSvc/delUgc.py` & `ANX-0.8.0/AndroidQQ/pack/SQQzoneSvc/delUgc.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/pack/SQQzoneSvc/like.py` & `ANX-0.8.0/AndroidQQ/pack/SQQzoneSvc/like.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/pack/SQQzoneSvc/publishmood.py` & `ANX-0.8.0/AndroidQQ/pack/SQQzoneSvc/publishmood.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/pack/SQQzoneSvc/shuoshuo.py` & `ANX-0.8.0/AndroidQQ/pack/SQQzoneSvc/shuoshuo.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/pack/StatSvc_register.py` & `ANX-0.8.0/AndroidQQ/pack/StatSvc_register.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/pack/SummaryCard/ReqSummaryCard.py` & `ANX-0.8.0/AndroidQQ/pack/SummaryCard/ReqSummaryCard.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/pack/friendlist.py` & `ANX-0.8.0/AndroidQQ/pack/friendlist.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/pack/test.py` & `ANX-0.8.0/AndroidQQ/pack/test.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/pack/trpc_metaverse_mob_proxy_svr_MobProxy_SsoHandle.py` & `ANX-0.8.0/AndroidQQ/pack/trpc_metaverse_mob_proxy_svr_MobProxy_SsoHandle.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/proto/IM_r_pb2.py` & `ANX-0.8.0/AndroidQQ/proto/IM_r_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/proto/wtlogin_pb2.py` & `ANX-0.8.0/AndroidQQ/proto/wtlogin_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/struct/Avatarlnfo/QQHeadInfo.py` & `ANX-0.8.0/AndroidQQ/struct/Avatarlnfo/QQHeadInfo.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/struct/Avatarlnfo/QQHeadUrlReq.py` & `ANX-0.8.0/AndroidQQ/struct/Avatarlnfo/QQHeadUrlReq.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/struct/Avatarlnfo/QQHeadUrlResp.py` & `ANX-0.8.0/AndroidQQ/struct/Avatarlnfo/QQHeadUrlResp.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/struct/Avatarlnfo/__init__.py` & `ANX-0.8.0/AndroidQQ/struct/Avatarlnfo/__init__.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/struct/MessageSvc.py` & `ANX-0.8.0/AndroidQQ/struct/MessageSvc.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_comm.py` & `ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_comm.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_operation.py` & `ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_operation.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_userinfo.py` & `ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_userinfo.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/struct/NS_MOBILE_FEEDS/mobile_applist_req.py` & `ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_FEEDS/mobile_applist_req.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/struct/NS_MOBILE_FEEDS/mobile_applist_rsp.py` & `ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_FEEDS/mobile_applist_rsp.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/struct/NS_MOBILE_FEEDS/s_outshare.py` & `ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_FEEDS/s_outshare.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/struct/NS_MOBILE_FEEDS/s_picurl.py` & `ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_FEEDS/s_picurl.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/struct/NS_MOBILE_FEEDS/single_feed.py` & `ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_FEEDS/single_feed.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/struct/NS_MOBILE_OPERATION/cmshow_active_result.py` & `ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_OPERATION/cmshow_active_result.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_delugc_req.py` & `ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_delugc_req.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_like_req.py` & `ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_like_req.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_like_rsp.py` & `ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_like_rsp.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_publishmood_req.py` & `ANX-0.8.0/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_publishmood_req.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/struct/OidbSvc.py` & `ANX-0.8.0/AndroidQQ/struct/OidbSvc.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/struct/QMF_PROTOCAL/QmfClientIpInfo.py` & `ANX-0.8.0/AndroidQQ/struct/QMF_PROTOCAL/QmfClientIpInfo.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/struct/QMF_PROTOCAL/QmfDownstream.py` & `ANX-0.8.0/AndroidQQ/struct/QMF_PROTOCAL/QmfDownstream.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/struct/QMF_PROTOCAL/QmfTokenInfo.py` & `ANX-0.8.0/AndroidQQ/struct/QMF_PROTOCAL/QmfTokenInfo.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/struct/QMF_PROTOCAL/QmfUpstream.py` & `ANX-0.8.0/AndroidQQ/struct/QMF_PROTOCAL/QmfUpstream.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/struct/QQService/SvcReqGetDevLoginInfo.py` & `ANX-0.8.0/AndroidQQ/struct/QQService/SvcReqGetDevLoginInfo.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/struct/QQService/__init__.py` & `ANX-0.8.0/AndroidQQ/struct/QQService/__init__.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/struct/StatSvc.py` & `ANX-0.8.0/AndroidQQ/struct/StatSvc.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/struct/SummaryCard/ReqSummaryCard.py` & `ANX-0.8.0/AndroidQQ/struct/SummaryCard/ReqSummaryCard.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/struct/Tlv.py` & `ANX-0.8.0/AndroidQQ/struct/Tlv.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/struct/Tlv_res.py` & `ANX-0.8.0/AndroidQQ/struct/Tlv_res.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/struct/cooperation/qzone/WNSStream.py` & `ANX-0.8.0/AndroidQQ/struct/cooperation/qzone/WNSStream.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/struct/feedcomponent/model.py` & `ANX-0.8.0/AndroidQQ/struct/feedcomponent/model.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/struct/friendlist/AddFriendReq.py` & `ANX-0.8.0/AndroidQQ/struct/friendlist/AddFriendReq.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/struct/head.py` & `ANX-0.8.0/AndroidQQ/struct/head.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/struct/push/SvcReqRegister.py` & `ANX-0.8.0/AndroidQQ/struct/push/SvcReqRegister.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/struct/push/SvcRespRegister.py` & `ANX-0.8.0/AndroidQQ/struct/push/SvcRespRegister.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/struct/wtlogin.py` & `ANX-0.8.0/AndroidQQ/struct/wtlogin.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/utils/build_device.py` & `ANX-0.8.0/AndroidQQ/utils/build_device.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/utils/ecdh.py` & `ANX-0.8.0/AndroidQQ/utils/ecdh.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/utils/sso_server.py` & `ANX-0.8.0/AndroidQQ/utils/sso_server.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/AndroidQQ/utils/tool.py` & `ANX-0.8.0/AndroidQQ/utils/tool.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.9/setup.py` & `ANX-0.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 setuptools.setup(
     name='ANX',
-    version='0.7.9',
+    version='0.8.0',
     url='https://github.com/grayrail000/AndroidQQ',
     packages=setuptools.find_packages(exclude=["tests", "tests.*"]),
     license='',
     author='1x',
     author_email='',
     description='',
     install_requires=[
```

