# Comparing `tmp/rosrestpy-0.8.0.tar.gz` & `tmp/rosrestpy-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rosrestpy-0.8.0.tar", max compression
+gzip compressed data, was "rosrestpy-0.9.0.tar", max compression
```

## Comparing `rosrestpy-0.8.0.tar` & `rosrestpy-0.9.0.tar`

### file list

```diff
@@ -1,98 +1,111 @@
--rw-r--r--   0        0        0    35149 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/LICENSE
--rw-r--r--   0        0        0     2543 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/README.md
--rw-r--r--   0        0        0     1222 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      553 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/__init__.py
--rw-r--r--   0        0        0     2659 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/_base.py
--rw-r--r--   0        0        0     4631 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/_literals.py
--rw-r--r--   0        0        0     1246 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/_utils.py
--rw-r--r--   0        0        0      301 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/error.py
--rw-r--r--   0        0        0     1851 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/inteface/__init__.py
--rw-r--r--   0        0        0     1002 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/inteface/bridge/__init__.py
--rw-r--r--   0        0        0      686 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/inteface/bridge/bridge.py
--rw-r--r--   0        0        0      262 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/inteface/bridge/msti.py
--rw-r--r--   0        0        0      763 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/inteface/bridge/port.py
--rw-r--r--   0        0        0      322 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/inteface/bridge/vlan.py
--rw-r--r--   0        0        0     1008 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/inteface/eoip.py
--rw-r--r--   0        0        0     1980 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/inteface/ethernet.py
--rw-r--r--   0        0        0      754 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/inteface/interface.py
--rw-r--r--   0        0        0      572 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/inteface/list/__init__.py
--rw-r--r--   0        0        0      244 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/inteface/list/list.py
--rw-r--r--   0        0        0      246 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/inteface/list/member.py
--rw-r--r--   0        0        0     2758 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/ip/__init__.py
--rw-r--r--   0        0        0      392 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/ip/address.py
--rw-r--r--   0        0        0      544 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/ip/arp.py
--rw-r--r--   0        0        0      278 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/ip/cloud.py
--rw-r--r--   0        0        0     1285 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/ip/dhcp_client.py
--rw-r--r--   0        0        0      470 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/ip/dhcp_relay.py
--rw-r--r--   0        0        0      771 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/ip/dhcp_server/__init__.py
--rw-r--r--   0        0        0      153 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/ip/dhcp_server/_literals.py
--rw-r--r--   0        0        0     1100 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/ip/dhcp_server/dhcp_server.py
--rw-r--r--   0        0        0     1050 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/ip/dhcp_server/lease.py
--rw-r--r--   0        0        0      423 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/ip/dhcp_server/network.py
--rw-r--r--   0        0        0     1032 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/ip/dns/__init__.py
--rw-r--r--   0        0        0      126 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/ip/dns/_literals.py
--rw-r--r--   0        0        0      195 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/ip/dns/cache.py
--rw-r--r--   0        0        0      626 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/ip/dns/static.py
--rw-r--r--   0        0        0     1472 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/ip/firewall/__init__.py
--rw-r--r--   0        0        0      282 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/ip/firewall/_literals.py
--rw-r--r--   0        0        0      748 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/ip/firewall/connection.py
--rw-r--r--   0        0        0     2703 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/ip/firewall/filter.py
--rw-r--r--   0        0        0     2978 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/ip/firewall/mangle.py
--rw-r--r--   0        0        0     2413 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/ip/firewall/nat.py
--rw-r--r--   0        0        0     3180 2023-07-02 14:47:03.850878 rosrestpy-0.8.0/ros/ip/hotspot/__init__.py
--rw-r--r--   0        0        0      454 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/ip/hotspot/active.py
--rw-r--r--   0        0        0      214 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/ip/hotspot/cookie.py
--rw-r--r--   0        0        0      625 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/ip/hotspot/host.py
--rw-r--r--   0        0        0      529 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/ip/hotspot/hotspot.py
--rw-r--r--   0        0        0      637 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/ip/hotspot/ip_binding.py
--rw-r--r--   0        0        0     1325 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/ip/hotspot/profile.py
--rw-r--r--   0        0        0      182 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/ip/hotspot/service_port.py
--rw-r--r--   0        0        0     1236 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/ip/hotspot/user/__init__.py
--rw-r--r--   0        0        0     1108 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/ip/hotspot/user/profile.py
--rw-r--r--   0        0        0      998 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/ip/hotspot/walled_garden/__init__.py
--rw-r--r--   0        0        0      557 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/ip/hotspot/walled_garden/ip.py
--rw-r--r--   0        0        0     1042 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/ip/route.py
--rw-r--r--   0        0        0      565 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/ip/setting.py
--rw-r--r--   0        0        0      181 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/log.py
--rw-r--r--   0        0        0      744 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/ppp/__init__.py
--rw-r--r--   0        0        0      220 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/ppp/_literals.py
--rw-r--r--   0        0        0      160 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/ppp/aaa.py
--rw-r--r--   0        0        0     1147 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/ppp/profile.py
--rw-r--r--   0        0        0      640 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/ppp/secret.py
--rw-r--r--   0        0        0      826 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/queue/__init__.py
--rw-r--r--   0        0        0      153 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/queue/interface.py
--rw-r--r--   0        0        0     2076 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/queue/simple.py
--rw-r--r--   0        0        0      726 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/queue/tree.py
--rw-r--r--   0        0        0     7146 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/ros.py
--rw-r--r--   0        0        0      604 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/routing/__init__.py
--rw-r--r--   0        0        0      467 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/routing/rule.py
--rw-r--r--   0        0        0      334 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/routing/table.py
--rw-r--r--   0        0        0     2407 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/system/__init__.py
--rw-r--r--   0        0        0      123 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/system/health.py
--rw-r--r--   0        0        0      214 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/system/history.py
--rw-r--r--   0        0        0      126 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/system/identity.py
--rw-r--r--   0        0        0      122 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/system/license.py
--rw-r--r--   0        0        0      248 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/system/logging.py
--rw-r--r--   0        0        0      146 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/system/note.py
--rw-r--r--   0        0        0      580 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/system/package/__init__.py
--rw-r--r--   0        0        0      101 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/system/package/_literals.py
--rw-r--r--   0        0        0      297 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/system/package/package.py
--rw-r--r--   0        0        0      774 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/system/package/update.py
--rw-r--r--   0        0        0      460 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/system/resource.py
--rw-r--r--   0        0        0      232 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/system/routerboard.py
--rw-r--r--   0        0        0     6722 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/tool/__init__.py
--rw-r--r--   0        0        0      223 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/tool/bandwith_server.py
--rw-r--r--   0        0        0      546 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/tool/bandwith_test.py
--rw-r--r--   0        0        0      158 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/tool/ip_scan.py
--rw-r--r--   0        0        0     1042 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/tool/netwatch.py
--rw-r--r--   0        0        0      236 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/tool/ping.py
--rw-r--r--   0        0        0      416 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/tool/torch.py
--rw-r--r--   0        0        0      290 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/tool/traceroute.py
--rw-r--r--   0        0        0     1746 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/user/__init__.py
--rw-r--r--   0        0        0      168 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/user/aaa.py
--rw-r--r--   0        0        0      167 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/user/active.py
--rw-r--r--   0        0        0      188 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/user/group.py
--rw-r--r--   0        0        0      129 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/user/settings.py
--rw-r--r--   0        0        0      205 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/user/ssh_keys.py
--rw-r--r--   0        0        0      249 2023-07-02 14:47:03.854878 rosrestpy-0.8.0/ros/user/user.py
--rw-r--r--   0        0        0     3723 1970-01-01 00:00:00.000000 rosrestpy-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/LICENSE
+-rw-r--r--   0        0        0     2543 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/README.md
+-rw-r--r--   0        0        0     1222 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      553 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/__init__.py
+-rw-r--r--   0        0        0     2735 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/_base.py
+-rw-r--r--   0        0        0     4631 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/_literals.py
+-rw-r--r--   0        0        0     1246 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/_utils.py
+-rw-r--r--   0        0        0      301 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/error.py
+-rw-r--r--   0        0        0     2885 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/inteface/__init__.py
+-rw-r--r--   0        0        0     1002 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/inteface/bridge/__init__.py
+-rw-r--r--   0        0        0      686 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/inteface/bridge/bridge.py
+-rw-r--r--   0        0        0      262 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/inteface/bridge/msti.py
+-rw-r--r--   0        0        0      763 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/inteface/bridge/port.py
+-rw-r--r--   0        0        0      322 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/inteface/bridge/vlan.py
+-rw-r--r--   0        0        0     1008 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/inteface/eoip.py
+-rw-r--r--   0        0        0     1980 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/inteface/ethernet.py
+-rw-r--r--   0        0        0      754 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/inteface/interface.py
+-rw-r--r--   0        0        0      572 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/inteface/list/__init__.py
+-rw-r--r--   0        0        0      244 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/inteface/list/list.py
+-rw-r--r--   0        0        0      246 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/inteface/list/member.py
+-rw-r--r--   0        0        0      233 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/inteface/veth.py
+-rw-r--r--   0        0        0      732 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/inteface/vlan.py
+-rw-r--r--   0        0        0      945 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/inteface/vrrp.py
+-rw-r--r--   0        0        0      166 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/inteface/wireguard/__init__.py
+-rw-r--r--   0        0        0      280 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/inteface/wireguard/wireguard.py
+-rw-r--r--   0        0        0     4390 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/ip/__init__.py
+-rw-r--r--   0        0        0      392 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/ip/address.py
+-rw-r--r--   0        0        0      544 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/ip/arp.py
+-rw-r--r--   0        0        0      278 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/ip/cloud.py
+-rw-r--r--   0        0        0     1285 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/ip/dhcp_client.py
+-rw-r--r--   0        0        0      470 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/ip/dhcp_relay.py
+-rw-r--r--   0        0        0      771 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/ip/dhcp_server/__init__.py
+-rw-r--r--   0        0        0      153 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/ip/dhcp_server/_literals.py
+-rw-r--r--   0        0        0     1100 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/ip/dhcp_server/dhcp_server.py
+-rw-r--r--   0        0        0     1050 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/ip/dhcp_server/lease.py
+-rw-r--r--   0        0        0      423 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/ip/dhcp_server/network.py
+-rw-r--r--   0        0        0     1032 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/ip/dns/__init__.py
+-rw-r--r--   0        0        0      126 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/ip/dns/_literals.py
+-rw-r--r--   0        0        0      195 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/ip/dns/cache.py
+-rw-r--r--   0        0        0      626 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/ip/dns/static.py
+-rw-r--r--   0        0        0     1472 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/ip/firewall/__init__.py
+-rw-r--r--   0        0        0      282 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/ip/firewall/_literals.py
+-rw-r--r--   0        0        0      748 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/ip/firewall/connection.py
+-rw-r--r--   0        0        0     2703 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/ip/firewall/filter.py
+-rw-r--r--   0        0        0     2978 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/ip/firewall/mangle.py
+-rw-r--r--   0        0        0     2413 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/ip/firewall/nat.py
+-rw-r--r--   0        0        0     3180 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/ip/hotspot/__init__.py
+-rw-r--r--   0        0        0      454 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/ip/hotspot/active.py
+-rw-r--r--   0        0        0      214 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/ip/hotspot/cookie.py
+-rw-r--r--   0        0        0      625 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/ip/hotspot/host.py
+-rw-r--r--   0        0        0      529 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/ip/hotspot/hotspot.py
+-rw-r--r--   0        0        0      637 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/ip/hotspot/ip_binding.py
+-rw-r--r--   0        0        0     1325 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/ip/hotspot/profile.py
+-rw-r--r--   0        0        0      182 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/ip/hotspot/service_port.py
+-rw-r--r--   0        0        0     1236 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/ip/hotspot/user/__init__.py
+-rw-r--r--   0        0        0     1108 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/ip/hotspot/user/profile.py
+-rw-r--r--   0        0        0      998 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/ip/hotspot/walled_garden/__init__.py
+-rw-r--r--   0        0        0      557 2023-07-15 20:12:21.679077 rosrestpy-0.9.0/ros/ip/hotspot/walled_garden/ip.py
+-rw-r--r--   0        0        0      427 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/ip/kid_control/__init__.py
+-rw-r--r--   0        0        0      511 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/ip/kid_control/device.py
+-rw-r--r--   0        0        0      559 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/ip/kid_control/kid.py
+-rw-r--r--   0        0        0      457 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/ip/neighbor.py
+-rw-r--r--   0        0        0      235 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/ip/pool.py
+-rw-r--r--   0        0        0     1042 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/ip/route.py
+-rw-r--r--   0        0        0      415 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/ip/service.py
+-rw-r--r--   0        0        0      565 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/ip/setting.py
+-rw-r--r--   0        0        0      291 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/ip/vrf.py
+-rw-r--r--   0        0        0      181 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/log.py
+-rw-r--r--   0        0        0      744 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/ppp/__init__.py
+-rw-r--r--   0        0        0      220 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/ppp/_literals.py
+-rw-r--r--   0        0        0      160 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/ppp/aaa.py
+-rw-r--r--   0        0        0     1147 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/ppp/profile.py
+-rw-r--r--   0        0        0      640 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/ppp/secret.py
+-rw-r--r--   0        0        0      826 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/queue/__init__.py
+-rw-r--r--   0        0        0      153 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/queue/interface.py
+-rw-r--r--   0        0        0     2076 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/queue/simple.py
+-rw-r--r--   0        0        0      726 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/queue/tree.py
+-rw-r--r--   0        0        0     7146 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/ros.py
+-rw-r--r--   0        0        0      818 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/routing/__init__.py
+-rw-r--r--   0        0        0      268 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/routing/id.py
+-rw-r--r--   0        0        0      467 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/routing/rule.py
+-rw-r--r--   0        0        0      334 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/routing/table.py
+-rw-r--r--   0        0        0     2407 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/system/__init__.py
+-rw-r--r--   0        0        0      123 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/system/health.py
+-rw-r--r--   0        0        0      214 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/system/history.py
+-rw-r--r--   0        0        0      126 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/system/identity.py
+-rw-r--r--   0        0        0      122 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/system/license.py
+-rw-r--r--   0        0        0      248 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/system/logging.py
+-rw-r--r--   0        0        0      146 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/system/note.py
+-rw-r--r--   0        0        0      580 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/system/package/__init__.py
+-rw-r--r--   0        0        0      101 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/system/package/_literals.py
+-rw-r--r--   0        0        0      297 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/system/package/package.py
+-rw-r--r--   0        0        0      774 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/system/package/update.py
+-rw-r--r--   0        0        0      460 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/system/resource.py
+-rw-r--r--   0        0        0      232 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/system/routerboard.py
+-rw-r--r--   0        0        0     6722 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/tool/__init__.py
+-rw-r--r--   0        0        0      223 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/tool/bandwith_server.py
+-rw-r--r--   0        0        0      546 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/tool/bandwith_test.py
+-rw-r--r--   0        0        0      158 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/tool/ip_scan.py
+-rw-r--r--   0        0        0     1042 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/tool/netwatch.py
+-rw-r--r--   0        0        0      236 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/tool/ping.py
+-rw-r--r--   0        0        0      416 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/tool/torch.py
+-rw-r--r--   0        0        0      290 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/tool/traceroute.py
+-rw-r--r--   0        0        0     1746 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/user/__init__.py
+-rw-r--r--   0        0        0      168 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/user/aaa.py
+-rw-r--r--   0        0        0      167 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/user/active.py
+-rw-r--r--   0        0        0      188 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/user/group.py
+-rw-r--r--   0        0        0      129 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/user/settings.py
+-rw-r--r--   0        0        0      205 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/user/ssh_keys.py
+-rw-r--r--   0        0        0      249 2023-07-15 20:12:21.683077 rosrestpy-0.9.0/ros/user/user.py
+-rw-r--r--   0        0        0     3723 1970-01-01 00:00:00.000000 rosrestpy-0.9.0/PKG-INFO
```

### Comparing `rosrestpy-0.8.0/LICENSE` & `rosrestpy-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.8.0/README.md` & `rosrestpy-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.8.0/pyproject.toml` & `rosrestpy-0.9.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rosrestpy"
-version = "0.8.0"
+version = "0.9.0"
 description = "RouterOS v7 REST API python module"
 authors = ["hexatester <hexatester@protonmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/hexatester/rosrestpy"
 packages = [
     { include = "ros" },
```

### Comparing `rosrestpy-0.8.0/ros/__init__.py` & `rosrestpy-0.9.0/ros/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.8.0"
+__version__ = "0.9.0"
 from .inteface import InterfaceModule
 from .ip import IPModule
 from .ppp import PPPModule
 from .queue import QueueModule
 from .routing import RoutingModule
 from .system import SystemModule
 from .tool import ToolModule
```

### Comparing `rosrestpy-0.8.0/ros/_base.py` & `rosrestpy-0.9.0/ros/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 
 @define
 class BaseProps(Generic[PR]):
     ros: "Ros"
     filename: str
     cl: Type[PR]
     _create: bool = True
+    _disable: bool = True
     _delete: bool = True
     _write: bool = True
 
     def __call__(self, **kwds: Any) -> List[PR]:
         return self.print(**kwds)
 
     @staticmethod
@@ -75,14 +76,15 @@
     def _disabled(self, o: PR, s: bool) -> PR:
         assert self._write, "Not writeable"
         return self.ros.patch_as(
             self.filename + f"/{self._getid(o)}", self.cl, {"disabled": s}
         )
 
     def disable(self, o: PR) -> PR:
+        assert self._disable, "Not allow disable"
         return self._disabled(o, True)
 
     def enable(self, o: PR) -> PR:
         return self._disabled(o, False)
 
     def print(self, **kwds: Any) -> List[PR]:
         return self.ros.get_as(self.filename, List[self.cl], kwds)
```

### Comparing `rosrestpy-0.8.0/ros/_literals.py` & `rosrestpy-0.9.0/ros/_literals.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.8.0/ros/_utils.py` & `rosrestpy-0.9.0/ros/_utils.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.8.0/ros/inteface/bridge/__init__.py` & `rosrestpy-0.9.0/ros/inteface/bridge/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.8.0/ros/inteface/bridge/bridge.py` & `rosrestpy-0.9.0/ros/inteface/bridge/bridge.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.8.0/ros/inteface/bridge/port.py` & `rosrestpy-0.9.0/ros/inteface/bridge/port.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.8.0/ros/inteface/eoip.py` & `rosrestpy-0.9.0/ros/inteface/eoip.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.8.0/ros/inteface/ethernet.py` & `rosrestpy-0.9.0/ros/inteface/ethernet.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.8.0/ros/inteface/interface.py` & `rosrestpy-0.9.0/ros/inteface/interface.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.8.0/ros/inteface/list/__init__.py` & `rosrestpy-0.9.0/ros/inteface/list/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.8.0/ros/ip/__init__.py` & `rosrestpy-0.9.0/ros/ip/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,28 +5,38 @@
 from .cloud import Cloud
 from .dhcp_client import DHCPClient
 from .dhcp_relay import DHCPRelay
 from .dhcp_server import DHCPServerModule, DHCPServer
 from .dns import DNS
 from .firewall import IPFirewallModule
 from .hotspot import HotspotModule, HotspotServer
+from .kid_control import KidControlModule, KidControl
+from .neighbor import IPNeighbor
+from .pool import IPPool
 from .route import Route
+from .service import Service
 from .setting import Setting
+from .vrf import Vrf
 
 
 class IPModule(BaseModule):
     _dhcp_server: DHCPServerModule = None
     _firewall: IPFirewallModule = None
     _hotspot: HotspotModule = None
 
     _address: BaseProps[Address] = None
     _arp: BaseProps[ARP] = None
     _dhcp_client: BaseProps[DHCPClient] = None
     _dhcp_relay: BaseProps[DHCPRelay] = None
+    _kid_control: KidControlModule = None
+    _pool: BaseProps[IPPool] = None
+    _neighbor: BaseProps[IPNeighbor] = None
     _route: BaseProps[Route] = None
+    _service: BaseProps[Service] = None
+    _vrf: BaseProps[Vrf] = None
 
     @property
     def address(self):
         if not self._address:
             self._address = BaseProps(self.ros, "/ip/address", Address)
         return self._address
 
@@ -75,29 +85,70 @@
     @property
     def hotspot(self) -> HotspotModule:
         if not self._hotspot:
             self._hotspot = HotspotModule(self.ros, "/ip/hotspot", HotspotServer)
         return self._hotspot
 
     @property
+    def kid_control(self) -> KidControlModule:
+        if not self._kid_control:
+            self._kid_control = KidControlModule(
+                self.ros, "/ip/kid-control", KidControl
+            )
+        return self._kid_control
+
+    @property
+    def neighbor(self) -> BaseProps[IPNeighbor]:
+        if not self._neighbor:
+            self._neighbor = BaseProps(self.ros, "/ip/neighbor", IPNeighbor)
+            self._neighbor._delete = False
+            self._neighbor._write = False
+            self._neighbor._disable = False
+        return self._neighbor
+
+    @property
+    def pool(self) -> BaseProps[IPPool]:
+        if not self._pool:
+            self._pool = BaseProps(self.ros, "/ip/pool", IPPool)
+            self._pool._disable = False
+        return self._pool
+
+    @property
     def route(self) -> BaseProps[Route]:
         if not self._route:
             self._route = BaseProps(self.ros, "/ip/route", Route)
         return self._route
 
     @property
+    def service(self) -> BaseProps[Service]:
+        if not self._service:
+            self._service = BaseProps(self.ros, "/ip/service", Service)
+            self._service._create = False
+            self._service._delete = False
+        return self._service
+
+    @property
     def setting(self) -> Setting:
         return self.ros.get_as("/ip/setting", Setting)
 
+    @property
+    def vrf(self) -> BaseProps[Vrf]:
+        if not self._vrf:
+            self._vrf = BaseProps(self.ros, "/ip/vrf", Vrf)
+        return self._vrf
+
 
 __all__ = [
     "Address",
     "ARP",
     "IPModule",
     "Cloud",
     "DHCPClient",
     "DHCPRelay",
     "DHCPServer",
     "DNS",
+    "KidControl",
     "Route",
+    "Service",
     "Setting",
+    "Vrf",
 ]
```

### Comparing `rosrestpy-0.8.0/ros/ip/arp.py` & `rosrestpy-0.9.0/ros/ip/arp.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.8.0/ros/ip/dhcp_client.py` & `rosrestpy-0.9.0/ros/ip/dhcp_client.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.8.0/ros/ip/dhcp_server/__init__.py` & `rosrestpy-0.9.0/ros/ip/dhcp_server/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.8.0/ros/ip/dhcp_server/dhcp_server.py` & `rosrestpy-0.9.0/ros/ip/dhcp_server/dhcp_server.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.8.0/ros/ip/dhcp_server/lease.py` & `rosrestpy-0.9.0/ros/ip/dhcp_server/lease.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.8.0/ros/ip/dns/__init__.py` & `rosrestpy-0.9.0/ros/ip/dns/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.8.0/ros/ip/dns/static.py` & `rosrestpy-0.9.0/ros/ip/dns/static.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.8.0/ros/ip/firewall/__init__.py` & `rosrestpy-0.9.0/ros/ip/firewall/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.8.0/ros/ip/firewall/connection.py` & `rosrestpy-0.9.0/ros/ip/firewall/connection.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.8.0/ros/ip/firewall/filter.py` & `rosrestpy-0.9.0/ros/ip/firewall/filter.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.8.0/ros/ip/firewall/mangle.py` & `rosrestpy-0.9.0/ros/ip/firewall/mangle.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.8.0/ros/ip/firewall/nat.py` & `rosrestpy-0.9.0/ros/ip/firewall/nat.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.8.0/ros/ip/hotspot/__init__.py` & `rosrestpy-0.9.0/ros/ip/hotspot/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.8.0/ros/ip/hotspot/host.py` & `rosrestpy-0.9.0/ros/ip/hotspot/host.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.8.0/ros/ip/hotspot/hotspot.py` & `rosrestpy-0.9.0/ros/ip/hotspot/hotspot.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.8.0/ros/ip/hotspot/ip_binding.py` & `rosrestpy-0.9.0/ros/ip/hotspot/ip_binding.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.8.0/ros/ip/hotspot/profile.py` & `rosrestpy-0.9.0/ros/ip/hotspot/profile.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.8.0/ros/ip/hotspot/user/__init__.py` & `rosrestpy-0.9.0/ros/ip/hotspot/user/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.8.0/ros/ip/hotspot/user/profile.py` & `rosrestpy-0.9.0/ros/ip/hotspot/user/profile.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.8.0/ros/ip/hotspot/walled_garden/__init__.py` & `rosrestpy-0.9.0/ros/ip/hotspot/walled_garden/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.8.0/ros/ip/hotspot/walled_garden/ip.py` & `rosrestpy-0.9.0/ros/ip/hotspot/walled_garden/ip.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.8.0/ros/ip/route.py` & `rosrestpy-0.9.0/ros/ip/route.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.8.0/ros/ip/setting.py` & `rosrestpy-0.9.0/ros/ip/setting.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.8.0/ros/ppp/__init__.py` & `rosrestpy-0.9.0/ros/ppp/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.8.0/ros/ppp/profile.py` & `rosrestpy-0.9.0/ros/ppp/profile.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.8.0/ros/ppp/secret.py` & `rosrestpy-0.9.0/ros/ppp/secret.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.8.0/ros/queue/__init__.py` & `rosrestpy-0.9.0/ros/queue/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.8.0/ros/queue/simple.py` & `rosrestpy-0.9.0/ros/queue/simple.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.8.0/ros/queue/tree.py` & `rosrestpy-0.9.0/ros/queue/tree.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.8.0/ros/ros.py` & `rosrestpy-0.9.0/ros/ros.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.8.0/ros/routing/__init__.py` & `rosrestpy-0.9.0/ros/routing/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 from ros._base import BaseModule, BaseProps
 
+from .id import RoutingId
 from .rule import RoutingRule
 from .table import RoutingTable
 
 
 class RoutingModule(BaseModule):
+    _id: BaseProps[RoutingId] = None
     _rule: BaseProps[RoutingRule] = None
     _table: BaseProps[RoutingTable] = None
 
     @property
+    def id(self):
+        if not self._id:
+            self._id = BaseProps(self.ros, "/routing/id", RoutingId)
+        return self._id
+
+    @property
     def rule(self):
         if not self._rule:
             self._rule = BaseProps(self.ros, "/routing/rule", RoutingRule)
         return self._rule
 
     @property
     def table(self):
```

### Comparing `rosrestpy-0.8.0/ros/system/__init__.py` & `rosrestpy-0.9.0/ros/system/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.8.0/ros/system/package/__init__.py` & `rosrestpy-0.9.0/ros/system/package/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.8.0/ros/system/package/update.py` & `rosrestpy-0.9.0/ros/system/package/update.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.8.0/ros/tool/__init__.py` & `rosrestpy-0.9.0/ros/tool/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.8.0/ros/tool/bandwith_test.py` & `rosrestpy-0.9.0/ros/tool/bandwith_test.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.8.0/ros/tool/netwatch.py` & `rosrestpy-0.9.0/ros/tool/netwatch.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.8.0/ros/user/__init__.py` & `rosrestpy-0.9.0/ros/user/__init__.py`

 * *Files identical despite different names*

### Comparing `rosrestpy-0.8.0/PKG-INFO` & `rosrestpy-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosrestpy
-Version: 0.8.0
+Version: 0.9.0
 Summary: RouterOS v7 REST API python module
 Home-page: https://github.com/hexatester/rosrestpy
 License: GPL-3.0-only
 Author: hexatester
 Author-email: hexatester@protonmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

