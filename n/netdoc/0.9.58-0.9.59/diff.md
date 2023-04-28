# Comparing `tmp/netdoc-0.9.58.tar.gz` & `tmp/netdoc-0.9.59.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netdoc-0.9.58.tar", last modified: Thu Apr 27 13:34:29 2023, max compression
+gzip compressed data, was "netdoc-0.9.59.tar", last modified: Fri Apr 28 10:13:58 2023, max compression
```

## Comparing `netdoc-0.9.58.tar` & `netdoc-0.9.59.tar`

### file list

```diff
@@ -1,188 +1,189 @@
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-27 13:34:29.217437 netdoc-0.9.58/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    35149 2023-04-05 08:40:22.000000 netdoc-0.9.58/LICENSE
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      241 2023-04-05 08:40:22.000000 netdoc-0.9.58/MANIFEST.in
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      469 2023-04-27 13:34:29.217437 netdoc-0.9.58/PKG-INFO
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     9982 2023-04-24 17:00:01.000000 netdoc-0.9.58/README.md
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-27 13:34:28.741428 netdoc-0.9.58/netdoc/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2218 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/__init__.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-27 13:34:28.937431 netdoc-0.9.58/netdoc/api/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/api/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2812 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/api/serializers.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      597 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/api/urls.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1207 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/api/views.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-27 13:34:28.941431 netdoc-0.9.58/netdoc/discoverers/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/discoverers/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     6978 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/discoverers/netmiko_cisco_ios.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     5160 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/discoverers/netmiko_cisco_nxos.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     6514 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/discoverers/netmiko_cisco_xr.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     6406 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/discoverers/netmiko_hp_comware.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     4511 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/discoverers/netmiko_linux.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3613 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/filtersets.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     6587 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/forms.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-27 13:34:28.973432 netdoc-0.9.58/netdoc/ingestors/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1205 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_ios_hostname.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3710 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_ios_show_cdp_neighbors_detail.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2014 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_ios_show_etherchannel_summary.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2457 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_ios_show_interfaces.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1705 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_ios_show_interfaces_switchport.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      822 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_ios_show_inventory.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1544 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_ios_show_ip_arp.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1951 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_ios_show_ip_interface.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2678 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_ios_show_ip_route.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3959 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_ios_show_lldp_neighbors_detail.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1660 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_ios_show_mac_address_table.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      886 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_ios_show_vlan.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1010 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_ios_show_vrf.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1238 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_nxos_hostname.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3677 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_nxos_show_cdp_neighbors_detail.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2349 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_nxos_show_interface.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1986 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_nxos_show_interface_switchport.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      824 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_nxos_show_inventory.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1539 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_nxos_show_ip_arp.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2000 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_nxos_show_ip_interface.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2851 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_nxos_show_ip_route_vrf_all.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3936 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_nxos_show_lldp_neighbors_detail.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1509 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_nxos_show_mac_address_table.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2020 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_nxos_show_port_channel_summary.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      888 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_nxos_show_vlan.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      909 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_nxos_show_vrf.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1204 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_xr_hostname.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1529 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_xr_show_arp.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3673 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_xr_show_cdp_neighbors_detail.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2347 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_xr_show_interfaces.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1802 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_xr_show_ipv4_interface.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2921 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_xr_show_lldp_neighbors.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2785 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_xr_show_route.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      980 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_xr_show_vrf_all_detail.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1562 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_hp_comware_display_arp.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      894 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_hp_comware_display_device_manuinfo.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2980 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_hp_comware_display_interface.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1385 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_hp_comware_display_ip_interface.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2702 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_hp_comware_display_ip_routing_table.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1038 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_hp_comware_display_ip_vpn_instance.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1687 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_hp_comware_display_ip_vpn_instance_instance_name.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2035 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_hp_comware_display_link_aggregation_verbose.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2962 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_hp_comware_display_lldp_neighbor_information_list.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3964 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_hp_comware_display_lldp_neighbor_information_verbose.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1514 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_hp_comware_display_mac_address.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      895 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_hp_comware_display_vlan_all.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      899 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_hp_comware_display_vlan_brief.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1202 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_hp_comware_hostname.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1539 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_linux_arp__an.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1008 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_linux_hostname.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1412 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_linux_ip_address_show.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1933 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_linux_ip_link_show.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2526 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_linux_ip_route_show.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      711 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/ingestors/netmiko_linux_ip_vrf_show.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-27 13:34:28.993433 netdoc-0.9.58/netdoc/migrations/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    13632 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/migrations/0001_initial.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1800 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/migrations/0002_alter_arptableentry_custom_field_data_and_more.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3399 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/migrations/0003_alter_arptableentry_options_alter_credential_options_and_more.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3022 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/migrations/0004_alter_macaddresstableentry_options_and_more.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      577 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/migrations/0005_diagram_include_global_vrf_alter_diagram_details.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      453 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/migrations/0006_alter_routetableentry_metric.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      419 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/migrations/0007_discoverylog_supported.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/migrations/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    15079 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/models.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2436 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/navigation.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2988 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/nornir_inventory.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-27 13:34:28.993433 netdoc-0.9.58/netdoc/reports/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     5880 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/reports/NetDoc.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-27 13:34:29.001433 netdoc-0.9.58/netdoc/schemas/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/schemas/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1937 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/schemas/arptableentry.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     4532 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/schemas/cable.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1739 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/schemas/credential.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     4374 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/schemas/device.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1508 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/schemas/devicerole.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1714 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/schemas/devicetype.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3905 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/schemas/discoverable.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3176 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/schemas/discoverylog.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     8843 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/schemas/interface.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1362 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/schemas/ipaddress.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1978 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/schemas/macaddresstableentry.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1453 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/schemas/manufacturer.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2015 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/schemas/prefix.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3018 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/schemas/routetableentry.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      884 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/schemas/site.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1623 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/schemas/vlan.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2476 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/schemas/vrf.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-27 13:34:29.001433 netdoc-0.9.58/netdoc/scripts/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    13085 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/scripts/NetDoc.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-27 13:34:28.717427 netdoc-0.9.58/netdoc/static/
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-27 13:34:28.717427 netdoc-0.9.58/netdoc/static/netdoc/
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-27 13:34:29.013433 netdoc-0.9.58/netdoc/static/netdoc/css/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    35149 2023-04-05 08:40:22.000000 netdoc-0.9.58/netdoc/static/netdoc/css/LICENSE
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      494 2023-04-05 08:40:22.000000 netdoc-0.9.58/netdoc/static/netdoc/css/README.md
--rw-rw-r--   0 andrea    (1000) andrea    (1000)   220164 2023-04-05 08:40:22.000000 netdoc-0.9.58/netdoc/static/netdoc/css/vis-network.min.css
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-27 13:34:29.181436 netdoc-0.9.58/netdoc/static/netdoc/img/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    35149 2023-04-05 08:40:22.000000 netdoc-0.9.58/netdoc/static/netdoc/img/LICENSE
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      305 2023-04-05 08:40:22.000000 netdoc-0.9.58/netdoc/static/netdoc/img/README.md
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     7415 2023-04-05 08:40:22.000000 netdoc-0.9.58/netdoc/static/netdoc/img/access-switch.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     5648 2023-04-05 08:40:22.000000 netdoc-0.9.58/netdoc/static/netdoc/img/backup.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    28633 2023-04-05 08:40:22.000000 netdoc-0.9.58/netdoc/static/netdoc/img/circuit.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     8387 2023-04-05 08:40:22.000000 netdoc-0.9.58/netdoc/static/netdoc/img/core-switch.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     9522 2023-04-05 08:40:22.000000 netdoc-0.9.58/netdoc/static/netdoc/img/distribution-switch.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    15596 2023-04-05 08:40:22.000000 netdoc-0.9.58/netdoc/static/netdoc/img/firewall.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1614 2023-04-05 08:40:22.000000 netdoc-0.9.58/netdoc/static/netdoc/img/internal-switch.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     5537 2023-04-05 08:40:22.000000 netdoc-0.9.58/netdoc/static/netdoc/img/isp-cpe-material.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     5079 2023-04-05 08:40:22.000000 netdoc-0.9.58/netdoc/static/netdoc/img/non-racked-devices.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    15857 2023-04-05 08:40:22.000000 netdoc-0.9.58/netdoc/static/netdoc/img/power-feed.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    18685 2023-04-05 08:40:22.000000 netdoc-0.9.58/netdoc/static/netdoc/img/power-panel.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     4710 2023-04-05 08:40:22.000000 netdoc-0.9.58/netdoc/static/netdoc/img/power-units.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    34335 2023-04-05 08:40:22.000000 netdoc-0.9.58/netdoc/static/netdoc/img/provider-networks.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    13504 2023-04-05 08:40:22.000000 netdoc-0.9.58/netdoc/static/netdoc/img/router.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     4484 2023-04-05 08:40:22.000000 netdoc-0.9.58/netdoc/static/netdoc/img/server.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     5648 2023-04-05 08:40:22.000000 netdoc-0.9.58/netdoc/static/netdoc/img/storage.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     8308 2023-04-05 08:40:22.000000 netdoc-0.9.58/netdoc/static/netdoc/img/unknown.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     7415 2023-04-05 08:40:22.000000 netdoc-0.9.58/netdoc/static/netdoc/img/wan-network.png
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     6975 2023-04-05 08:40:22.000000 netdoc-0.9.58/netdoc/static/netdoc/img/wireless-ap.png
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-27 13:34:29.197437 netdoc-0.9.58/netdoc/static/netdoc/js/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    35149 2023-04-05 08:40:22.000000 netdoc-0.9.58/netdoc/static/netdoc/js/LICENSE
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      494 2023-04-05 08:40:22.000000 netdoc-0.9.58/netdoc/static/netdoc/js/README.md
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     4198 2023-04-05 14:32:29.000000 netdoc-0.9.58/netdoc/static/netdoc/js/diagram.js
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1739 2023-04-05 08:40:22.000000 netdoc-0.9.58/netdoc/static/netdoc/js/netdoc.js
--rw-rw-r--   0 andrea    (1000) andrea    (1000)   702066 2023-04-05 08:40:22.000000 netdoc-0.9.58/netdoc/static/netdoc/js/vis-network.min.js
--rw-rw-r--   0 andrea    (1000) andrea    (1000)  1930592 2023-04-05 08:40:22.000000 netdoc-0.9.58/netdoc/static/netdoc/js/vis-network.min.js.map
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     8272 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/tables.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3912 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/tasks.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-27 13:34:28.721427 netdoc-0.9.58/netdoc/templates/
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-27 13:34:29.209437 netdoc-0.9.58/netdoc/templates/netdoc/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3038 2023-04-10 16:21:20.000000 netdoc-0.9.58/netdoc/templates/netdoc/arptableentry.html
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-27 13:34:29.217437 netdoc-0.9.58/netdoc/templates/netdoc/buttons/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      451 2023-04-10 16:17:25.000000 netdoc-0.9.58/netdoc/templates/netdoc/buttons/discover.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      337 2023-04-10 16:17:25.000000 netdoc-0.9.58/netdoc/templates/netdoc/buttons/export.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1669 2023-04-10 16:21:17.000000 netdoc-0.9.58/netdoc/templates/netdoc/credential.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1439 2023-04-10 16:29:06.000000 netdoc-0.9.58/netdoc/templates/netdoc/diagram.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     2654 2023-04-10 16:23:32.000000 netdoc-0.9.58/netdoc/templates/netdoc/discoverable.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1217 2023-04-10 16:26:08.000000 netdoc-0.9.58/netdoc/templates/netdoc/discoverable_bulk_discover.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      638 2023-04-10 16:26:30.000000 netdoc-0.9.58/netdoc/templates/netdoc/discoverable_discover.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1006 2023-04-10 16:23:40.000000 netdoc-0.9.58/netdoc/templates/netdoc/discoverable_list.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     5123 2023-04-10 16:23:17.000000 netdoc-0.9.58/netdoc/templates/netdoc/discoverylog.html
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-27 13:34:29.217437 netdoc-0.9.58/netdoc/templates/netdoc/htmx/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1005 2023-04-10 16:17:25.000000 netdoc-0.9.58/netdoc/templates/netdoc/htmx/discover_form.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1025 2023-04-10 16:17:25.000000 netdoc-0.9.58/netdoc/templates/netdoc/htmx/logexport_form.html
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     3046 2023-04-10 16:20:47.000000 netdoc-0.9.58/netdoc/templates/netdoc/macaddresstableentry.html
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-27 13:34:29.217437 netdoc-0.9.58/netdoc/templatetags/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/templatetags/__init__.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-27 13:34:29.217437 netdoc-0.9.58/netdoc/templatetags/__pycache__/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      148 2023-04-26 16:55:07.000000 netdoc-0.9.58/netdoc/templatetags/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1048 2023-04-26 16:55:07.000000 netdoc-0.9.58/netdoc/templatetags/__pycache__/netdoc_buttons.cpython-310.pyc
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      890 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/templatetags/netdoc_buttons.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-27 13:34:29.217437 netdoc-0.9.58/netdoc/tests/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/tests/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    17018 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/tests/test.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    11597 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/topologies.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     5128 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/urls.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    28164 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/utils.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    18389 2023-04-27 13:34:24.000000 netdoc-0.9.58/netdoc/views.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-27 13:34:28.937431 netdoc-0.9.58/netdoc.egg-info/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      469 2023-04-27 13:34:28.000000 netdoc-0.9.58/netdoc.egg-info/PKG-INFO
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     6905 2023-04-27 13:34:28.000000 netdoc-0.9.58/netdoc.egg-info/SOURCES.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        1 2023-04-27 13:34:28.000000 netdoc-0.9.58/netdoc.egg-info/dependency_links.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        1 2023-04-05 14:49:45.000000 netdoc-0.9.58/netdoc.egg-info/not-zip-safe
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      132 2023-04-27 13:34:28.000000 netdoc-0.9.58/netdoc.egg-info/requires.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        7 2023-04-27 13:34:28.000000 netdoc-0.9.58/netdoc.egg-info/top_level.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      103 2023-04-27 13:34:29.221437 netdoc-0.9.58/setup.cfg
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1272 2023-04-27 13:34:24.000000 netdoc-0.9.58/setup.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-28 10:13:58.080562 netdoc-0.9.59/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    35149 2023-04-05 08:40:22.000000 netdoc-0.9.59/LICENSE
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      241 2023-04-05 08:40:22.000000 netdoc-0.9.59/MANIFEST.in
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      469 2023-04-28 10:13:58.080562 netdoc-0.9.59/PKG-INFO
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     9982 2023-04-24 17:00:01.000000 netdoc-0.9.59/README.md
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-28 10:13:57.836557 netdoc-0.9.59/netdoc/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2218 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/__init__.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-28 10:13:57.844557 netdoc-0.9.59/netdoc/api/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/api/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2812 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/api/serializers.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      597 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/api/urls.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1207 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/api/views.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-28 10:13:57.852558 netdoc-0.9.59/netdoc/discoverers/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/discoverers/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     6978 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/discoverers/netmiko_cisco_ios.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     5160 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/discoverers/netmiko_cisco_nxos.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     6520 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/discoverers/netmiko_cisco_xr.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     6406 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/discoverers/netmiko_hp_comware.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     4511 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/discoverers/netmiko_linux.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3613 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/filtersets.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     6587 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/forms.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-28 10:13:57.912559 netdoc-0.9.59/netdoc/ingestors/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1205 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_ios_hostname.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3710 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_ios_show_cdp_neighbors_detail.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2014 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_ios_show_etherchannel_summary.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2457 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_ios_show_interfaces.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1705 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_ios_show_interfaces_switchport.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      912 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_ios_show_inventory.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1544 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_ios_show_ip_arp.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1951 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_ios_show_ip_interface.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2678 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_ios_show_ip_route.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3959 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_ios_show_lldp_neighbors_detail.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1660 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_ios_show_mac_address_table.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      886 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_ios_show_vlan.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1010 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_ios_show_vrf.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1238 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_nxos_hostname.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3677 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_nxos_show_cdp_neighbors_detail.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2349 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_nxos_show_interface.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1986 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_nxos_show_interface_switchport.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      914 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_nxos_show_inventory.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1539 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_nxos_show_ip_arp.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2000 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_nxos_show_ip_interface.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2851 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_nxos_show_ip_route_vrf_all.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3936 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_nxos_show_lldp_neighbors_detail.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1509 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_nxos_show_mac_address_table.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2020 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_nxos_show_port_channel_summary.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      888 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_nxos_show_vlan.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      909 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_nxos_show_vrf.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      915 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_xr_admin_show_inventory.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1204 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_xr_hostname.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1529 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_xr_show_arp.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3673 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_xr_show_cdp_neighbors_detail.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2347 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_xr_show_interfaces.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1802 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_xr_show_ipv4_interface.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2921 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_xr_show_lldp_neighbors.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2785 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_xr_show_route.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      980 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_xr_show_vrf_all_detail.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1562 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_hp_comware_display_arp.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      894 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_hp_comware_display_device_manuinfo.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2980 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_hp_comware_display_interface.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1385 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_hp_comware_display_ip_interface.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2702 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_hp_comware_display_ip_routing_table.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1038 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_hp_comware_display_ip_vpn_instance.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1687 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_hp_comware_display_ip_vpn_instance_instance_name.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2035 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_hp_comware_display_link_aggregation_verbose.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2962 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_hp_comware_display_lldp_neighbor_information_list.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3964 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_hp_comware_display_lldp_neighbor_information_verbose.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1514 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_hp_comware_display_mac_address.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      895 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_hp_comware_display_vlan_all.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      899 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_hp_comware_display_vlan_brief.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1202 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_hp_comware_hostname.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1539 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_linux_arp__an.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1008 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_linux_hostname.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1412 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_linux_ip_address_show.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1933 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_linux_ip_link_show.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2526 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_linux_ip_route_show.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      711 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/ingestors/netmiko_linux_ip_vrf_show.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-28 10:13:57.924559 netdoc-0.9.59/netdoc/migrations/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    13632 2023-04-28 10:13:54.000000 netdoc-0.9.59/netdoc/migrations/0001_initial.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1800 2023-04-28 10:13:54.000000 netdoc-0.9.59/netdoc/migrations/0002_alter_arptableentry_custom_field_data_and_more.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3399 2023-04-28 10:13:54.000000 netdoc-0.9.59/netdoc/migrations/0003_alter_arptableentry_options_alter_credential_options_and_more.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3022 2023-04-28 10:13:54.000000 netdoc-0.9.59/netdoc/migrations/0004_alter_macaddresstableentry_options_and_more.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      577 2023-04-28 10:13:54.000000 netdoc-0.9.59/netdoc/migrations/0005_diagram_include_global_vrf_alter_diagram_details.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      453 2023-04-28 10:13:54.000000 netdoc-0.9.59/netdoc/migrations/0006_alter_routetableentry_metric.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      419 2023-04-28 10:13:54.000000 netdoc-0.9.59/netdoc/migrations/0007_discoverylog_supported.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-28 10:13:54.000000 netdoc-0.9.59/netdoc/migrations/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    15079 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/models.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2436 2023-04-28 10:13:54.000000 netdoc-0.9.59/netdoc/navigation.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2988 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/nornir_inventory.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-28 10:13:57.924559 netdoc-0.9.59/netdoc/reports/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     5880 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/reports/NetDoc.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-28 10:13:57.928559 netdoc-0.9.59/netdoc/schemas/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/schemas/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1937 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/schemas/arptableentry.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     4532 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/schemas/cable.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1739 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/schemas/credential.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     6493 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/schemas/device.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1508 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/schemas/devicerole.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1714 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/schemas/devicetype.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3905 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/schemas/discoverable.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3176 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/schemas/discoverylog.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    10126 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/schemas/interface.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1362 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/schemas/ipaddress.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1978 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/schemas/macaddresstableentry.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1453 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/schemas/manufacturer.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2015 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/schemas/prefix.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3018 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/schemas/routetableentry.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      884 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/schemas/site.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1623 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/schemas/vlan.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2476 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/schemas/vrf.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-28 10:13:57.928559 netdoc-0.9.59/netdoc/scripts/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    13085 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/scripts/NetDoc.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-28 10:13:57.820557 netdoc-0.9.59/netdoc/static/
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-28 10:13:57.820557 netdoc-0.9.59/netdoc/static/netdoc/
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-28 10:13:57.940559 netdoc-0.9.59/netdoc/static/netdoc/css/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    35149 2023-04-05 08:40:22.000000 netdoc-0.9.59/netdoc/static/netdoc/css/LICENSE
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      494 2023-04-05 08:40:22.000000 netdoc-0.9.59/netdoc/static/netdoc/css/README.md
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)   220164 2023-04-05 08:40:22.000000 netdoc-0.9.59/netdoc/static/netdoc/css/vis-network.min.css
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-28 10:13:58.044561 netdoc-0.9.59/netdoc/static/netdoc/img/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    35149 2023-04-05 08:40:22.000000 netdoc-0.9.59/netdoc/static/netdoc/img/LICENSE
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      305 2023-04-05 08:40:22.000000 netdoc-0.9.59/netdoc/static/netdoc/img/README.md
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     7415 2023-04-05 08:40:22.000000 netdoc-0.9.59/netdoc/static/netdoc/img/access-switch.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     5648 2023-04-05 08:40:22.000000 netdoc-0.9.59/netdoc/static/netdoc/img/backup.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    28633 2023-04-05 08:40:22.000000 netdoc-0.9.59/netdoc/static/netdoc/img/circuit.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     8387 2023-04-05 08:40:22.000000 netdoc-0.9.59/netdoc/static/netdoc/img/core-switch.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     9522 2023-04-05 08:40:22.000000 netdoc-0.9.59/netdoc/static/netdoc/img/distribution-switch.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    15596 2023-04-05 08:40:22.000000 netdoc-0.9.59/netdoc/static/netdoc/img/firewall.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1614 2023-04-05 08:40:22.000000 netdoc-0.9.59/netdoc/static/netdoc/img/internal-switch.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     5537 2023-04-05 08:40:22.000000 netdoc-0.9.59/netdoc/static/netdoc/img/isp-cpe-material.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     5079 2023-04-05 08:40:22.000000 netdoc-0.9.59/netdoc/static/netdoc/img/non-racked-devices.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    15857 2023-04-05 08:40:22.000000 netdoc-0.9.59/netdoc/static/netdoc/img/power-feed.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    18685 2023-04-05 08:40:22.000000 netdoc-0.9.59/netdoc/static/netdoc/img/power-panel.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     4710 2023-04-05 08:40:22.000000 netdoc-0.9.59/netdoc/static/netdoc/img/power-units.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    34335 2023-04-05 08:40:22.000000 netdoc-0.9.59/netdoc/static/netdoc/img/provider-networks.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    13504 2023-04-05 08:40:22.000000 netdoc-0.9.59/netdoc/static/netdoc/img/router.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     4484 2023-04-05 08:40:22.000000 netdoc-0.9.59/netdoc/static/netdoc/img/server.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     5648 2023-04-05 08:40:22.000000 netdoc-0.9.59/netdoc/static/netdoc/img/storage.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     8308 2023-04-05 08:40:22.000000 netdoc-0.9.59/netdoc/static/netdoc/img/unknown.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     7415 2023-04-05 08:40:22.000000 netdoc-0.9.59/netdoc/static/netdoc/img/wan-network.png
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     6975 2023-04-05 08:40:22.000000 netdoc-0.9.59/netdoc/static/netdoc/img/wireless-ap.png
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-28 10:13:58.064561 netdoc-0.9.59/netdoc/static/netdoc/js/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    35149 2023-04-05 08:40:22.000000 netdoc-0.9.59/netdoc/static/netdoc/js/LICENSE
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      494 2023-04-05 08:40:22.000000 netdoc-0.9.59/netdoc/static/netdoc/js/README.md
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     4198 2023-04-05 14:32:29.000000 netdoc-0.9.59/netdoc/static/netdoc/js/diagram.js
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1739 2023-04-05 08:40:22.000000 netdoc-0.9.59/netdoc/static/netdoc/js/netdoc.js
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)   702066 2023-04-05 08:40:22.000000 netdoc-0.9.59/netdoc/static/netdoc/js/vis-network.min.js
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)  1930592 2023-04-05 08:40:22.000000 netdoc-0.9.59/netdoc/static/netdoc/js/vis-network.min.js.map
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     8272 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/tables.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3912 2023-04-28 10:13:54.000000 netdoc-0.9.59/netdoc/tasks.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-28 10:13:57.820557 netdoc-0.9.59/netdoc/templates/
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-28 10:13:58.076562 netdoc-0.9.59/netdoc/templates/netdoc/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3038 2023-04-10 16:21:20.000000 netdoc-0.9.59/netdoc/templates/netdoc/arptableentry.html
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-28 10:13:58.080562 netdoc-0.9.59/netdoc/templates/netdoc/buttons/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      451 2023-04-10 16:17:25.000000 netdoc-0.9.59/netdoc/templates/netdoc/buttons/discover.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      337 2023-04-10 16:17:25.000000 netdoc-0.9.59/netdoc/templates/netdoc/buttons/export.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1669 2023-04-10 16:21:17.000000 netdoc-0.9.59/netdoc/templates/netdoc/credential.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1439 2023-04-10 16:29:06.000000 netdoc-0.9.59/netdoc/templates/netdoc/diagram.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     2654 2023-04-10 16:23:32.000000 netdoc-0.9.59/netdoc/templates/netdoc/discoverable.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1217 2023-04-10 16:26:08.000000 netdoc-0.9.59/netdoc/templates/netdoc/discoverable_bulk_discover.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      638 2023-04-10 16:26:30.000000 netdoc-0.9.59/netdoc/templates/netdoc/discoverable_discover.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1006 2023-04-10 16:23:40.000000 netdoc-0.9.59/netdoc/templates/netdoc/discoverable_list.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     5123 2023-04-10 16:23:17.000000 netdoc-0.9.59/netdoc/templates/netdoc/discoverylog.html
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-28 10:13:58.080562 netdoc-0.9.59/netdoc/templates/netdoc/htmx/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1005 2023-04-10 16:17:25.000000 netdoc-0.9.59/netdoc/templates/netdoc/htmx/discover_form.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1025 2023-04-10 16:17:25.000000 netdoc-0.9.59/netdoc/templates/netdoc/htmx/logexport_form.html
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     3046 2023-04-10 16:20:47.000000 netdoc-0.9.59/netdoc/templates/netdoc/macaddresstableentry.html
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-28 10:13:58.080562 netdoc-0.9.59/netdoc/templatetags/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/templatetags/__init__.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-28 10:13:58.080562 netdoc-0.9.59/netdoc/templatetags/__pycache__/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      148 2023-04-27 13:34:30.000000 netdoc-0.9.59/netdoc/templatetags/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1048 2023-04-27 13:34:30.000000 netdoc-0.9.59/netdoc/templatetags/__pycache__/netdoc_buttons.cpython-310.pyc
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      890 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/templatetags/netdoc_buttons.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-28 10:13:58.080562 netdoc-0.9.59/netdoc/tests/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        0 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/tests/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    17018 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/tests/test.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    11615 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/topologies.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     5128 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/urls.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    28388 2023-04-28 10:13:55.000000 netdoc-0.9.59/netdoc/utils.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    18479 2023-04-28 10:13:54.000000 netdoc-0.9.59/netdoc/views.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-28 10:13:57.844557 netdoc-0.9.59/netdoc.egg-info/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      469 2023-04-28 10:13:57.000000 netdoc-0.9.59/netdoc.egg-info/PKG-INFO
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     6963 2023-04-28 10:13:57.000000 netdoc-0.9.59/netdoc.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        1 2023-04-28 10:13:57.000000 netdoc-0.9.59/netdoc.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        1 2023-04-05 14:49:45.000000 netdoc-0.9.59/netdoc.egg-info/not-zip-safe
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      132 2023-04-28 10:13:57.000000 netdoc-0.9.59/netdoc.egg-info/requires.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)        7 2023-04-28 10:13:57.000000 netdoc-0.9.59/netdoc.egg-info/top_level.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      103 2023-04-28 10:13:58.084562 netdoc-0.9.59/setup.cfg
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1272 2023-04-28 10:13:55.000000 netdoc-0.9.59/setup.py
```

### Comparing `netdoc-0.9.58/LICENSE` & `netdoc-0.9.59/LICENSE`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/README.md` & `netdoc-0.9.59/README.md`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/__init__.py` & `netdoc-0.9.59/netdoc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Main class."""
 __author__ = "Andrea Dainese"
 __contact__ = "andrea@adainese.it"
 __copyright__ = "Copyright 2022, Andrea Dainese"
 __license__ = "GPLv3"
-__version__ = "0.9.58"
+__version__ = "0.9.59"
 
 import os
 import pkgutil
 import shutil
 
 from django.conf import settings
```

### Comparing `netdoc-0.9.58/netdoc/api/serializers.py` & `netdoc-0.9.59/netdoc/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/api/urls.py` & `netdoc-0.9.59/netdoc/api/urls.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/api/views.py` & `netdoc-0.9.59/netdoc/api/views.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/discoverers/netmiko_cisco_ios.py` & `netdoc-0.9.59/netdoc/discoverers/netmiko_cisco_ios.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/discoverers/netmiko_cisco_nxos.py` & `netdoc-0.9.59/netdoc/discoverers/netmiko_cisco_nxos.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/discoverers/netmiko_cisco_xr.py` & `netdoc-0.9.59/netdoc/discoverers/netmiko_cisco_xr.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             [
                 "show running-config",
                 "show interfaces",
                 "show cdp neighbors detail",
                 "show lldp neighbors",
                 "show vrf all detail",
                 "show ipv4 interface",
-                "show inventory",
+                "admin show inventory",
             ],
             order=10,
         )
         utils.append_nornir_netmiko_task(
             task,
             [
                 "show inventory",
```

### Comparing `netdoc-0.9.58/netdoc/discoverers/netmiko_hp_comware.py` & `netdoc-0.9.59/netdoc/discoverers/netmiko_hp_comware.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/discoverers/netmiko_linux.py` & `netdoc-0.9.59/netdoc/discoverers/netmiko_linux.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/filtersets.py` & `netdoc-0.9.59/netdoc/filtersets.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/forms.py` & `netdoc-0.9.59/netdoc/forms.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_ios_hostname.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_ios_hostname.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_ios_show_cdp_neighbors_detail.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_ios_show_cdp_neighbors_detail.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_ios_show_etherchannel_summary.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_ios_show_etherchannel_summary.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_ios_show_interfaces.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_ios_show_interfaces.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_ios_show_interfaces_switchport.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_ios_show_interfaces_switchport.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_ios_show_inventory.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_ios_show_inventory.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 """Ingestor for netmiko_cisco_ios_show_inventory."""
 __author__ = "Andrea Dainese"
 __contact__ = "andrea@adainese.it"
 __copyright__ = "Copyright 2022, Andrea Dainese"
 __license__ = "GPLv3"
 
+from netdoc.schemas import device
+
 
 def ingest(log):
     """Processing parsed output."""
     device_o = log.discoverable.device
 
     for item in log.parsed_output:
         # See https://github.com/networktocode/ntc-templates/tree/master/tests/cisco_ios/show_inventory # pylint: disable=line-too-long
         part_description = item.get("name")
         part_serial_number = item.get("sn")
-        # part_id = item.get("pid")
+        part_number = item.get("pid")
 
         if "chassis" in part_description.lower():
-            # Chassis Serial Number
-            device_o.serial = part_serial_number
-            device_o.save()
+            # Chassis model and Serial Number
+            device.update(
+                device_o, serial=part_serial_number, model_keyword=part_number
+            )
             break
 
     # Update the log
     log.ingested = True
     log.save()
```

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_ios_show_ip_arp.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_ios_show_ip_arp.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_ios_show_ip_interface.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_ios_show_ip_interface.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_ios_show_ip_route.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_ios_show_ip_route.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_ios_show_lldp_neighbors_detail.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_ios_show_lldp_neighbors_detail.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_ios_show_mac_address_table.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_ios_show_mac_address_table.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_ios_show_vlan.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_ios_show_vlan.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_ios_show_vrf.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_ios_show_vrf.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_nxos_hostname.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_nxos_hostname.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_nxos_show_cdp_neighbors_detail.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_nxos_show_cdp_neighbors_detail.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_nxos_show_interface.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_nxos_show_interface.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_nxos_show_interface_switchport.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_nxos_show_interface_switchport.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_nxos_show_inventory.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_nxos_show_inventory.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 """Ingestor for netmiko_cisco_nxos_show_inventory."""
 __author__ = "Andrea Dainese"
 __contact__ = "andrea@adainese.it"
 __copyright__ = "Copyright 2022, Andrea Dainese"
 __license__ = "GPLv3"
 
+from netdoc.schemas import device
+
 
 def ingest(log):
     """Processing parsed output."""
     device_o = log.discoverable.device
 
     for item in log.parsed_output:
         # See https://github.com/networktocode/ntc-templates/tree/master/tests/cisco_nxos/show_inventory # pylint: disable=line-too-long
         part_description = item.get("name")
         part_serial_number = item.get("sn")
-        # part_id = item.get("pid")
+        part_number = item.get("pid")
 
         if "chassis" in part_description.lower():
-            # Chassis Serial Number
-            device_o.serial = part_serial_number
-            device_o.save()
+            # Chassis model and Serial Number
+            device.update(
+                device_o, serial=part_serial_number, model_keyword=part_number
+            )
             break
 
     # Update the log
     log.ingested = True
     log.save()
```

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_nxos_show_ip_arp.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_nxos_show_ip_arp.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_nxos_show_ip_interface.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_nxos_show_ip_interface.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_nxos_show_ip_route_vrf_all.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_nxos_show_ip_route_vrf_all.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_nxos_show_lldp_neighbors_detail.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_nxos_show_lldp_neighbors_detail.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_nxos_show_mac_address_table.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_nxos_show_mac_address_table.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_nxos_show_port_channel_summary.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_nxos_show_port_channel_summary.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_nxos_show_vlan.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_nxos_show_vlan.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_nxos_show_vrf.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_nxos_show_vrf.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_xr_hostname.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_xr_hostname.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_xr_show_arp.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_xr_show_arp.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_xr_show_cdp_neighbors_detail.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_xr_show_cdp_neighbors_detail.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_xr_show_interfaces.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_xr_show_interfaces.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_xr_show_ipv4_interface.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_xr_show_ipv4_interface.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_xr_show_lldp_neighbors.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_xr_show_lldp_neighbors.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_xr_show_route.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_xr_show_route.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_cisco_xr_show_vrf_all_detail.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_cisco_xr_show_vrf_all_detail.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_hp_comware_display_arp.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_hp_comware_display_arp.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_hp_comware_display_device_manuinfo.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_hp_comware_display_device_manuinfo.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_hp_comware_display_interface.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_hp_comware_display_interface.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_hp_comware_display_ip_interface.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_hp_comware_display_ip_interface.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_hp_comware_display_ip_routing_table.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_hp_comware_display_ip_routing_table.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_hp_comware_display_ip_vpn_instance.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_hp_comware_display_ip_vpn_instance.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_hp_comware_display_ip_vpn_instance_instance_name.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_hp_comware_display_ip_vpn_instance_instance_name.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_hp_comware_display_link_aggregation_verbose.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_hp_comware_display_link_aggregation_verbose.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_hp_comware_display_lldp_neighbor_information_list.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_hp_comware_display_lldp_neighbor_information_list.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_hp_comware_display_lldp_neighbor_information_verbose.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_hp_comware_display_lldp_neighbor_information_verbose.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_hp_comware_display_mac_address.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_hp_comware_display_mac_address.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_hp_comware_display_vlan_all.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_hp_comware_display_vlan_all.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_hp_comware_display_vlan_brief.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_hp_comware_display_vlan_brief.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_hp_comware_hostname.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_hp_comware_hostname.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_linux_arp__an.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_linux_arp__an.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_linux_hostname.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_linux_hostname.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_linux_ip_address_show.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_linux_ip_address_show.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_linux_ip_link_show.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_linux_ip_link_show.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_linux_ip_route_show.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_linux_ip_route_show.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/ingestors/netmiko_linux_ip_vrf_show.py` & `netdoc-0.9.59/netdoc/ingestors/netmiko_linux_ip_vrf_show.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/migrations/0001_initial.py` & `netdoc-0.9.59/netdoc/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/migrations/0002_alter_arptableentry_custom_field_data_and_more.py` & `netdoc-0.9.59/netdoc/migrations/0002_alter_arptableentry_custom_field_data_and_more.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/migrations/0003_alter_arptableentry_options_alter_credential_options_and_more.py` & `netdoc-0.9.59/netdoc/migrations/0003_alter_arptableentry_options_alter_credential_options_and_more.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/migrations/0004_alter_macaddresstableentry_options_and_more.py` & `netdoc-0.9.59/netdoc/migrations/0004_alter_macaddresstableentry_options_and_more.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/migrations/0005_diagram_include_global_vrf_alter_diagram_details.py` & `netdoc-0.9.59/netdoc/migrations/0005_diagram_include_global_vrf_alter_diagram_details.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/models.py` & `netdoc-0.9.59/netdoc/models.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/navigation.py` & `netdoc-0.9.59/netdoc/navigation.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/nornir_inventory.py` & `netdoc-0.9.59/netdoc/nornir_inventory.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/reports/NetDoc.py` & `netdoc-0.9.59/netdoc/reports/NetDoc.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/schemas/arptableentry.py` & `netdoc-0.9.59/netdoc/schemas/arptableentry.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/schemas/cable.py` & `netdoc-0.9.59/netdoc/schemas/cable.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/schemas/credential.py` & `netdoc-0.9.59/netdoc/schemas/credential.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/schemas/device.py` & `netdoc-0.9.59/netdoc/schemas/discoverable.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,149 +1,129 @@
-"""Schema validation for Device."""
+"""Schema validation for Discoverable."""
 __author__ = "Andrea Dainese"
 __contact__ = "andrea@adainese.it"
 __copyright__ = "Copyright 2022, Andrea Dainese"
 __license__ = "GPLv3"
 
 from jsonschema import validate, FormatChecker
 
-from dcim.models import (
-    DeviceRole as DeviceRole_model,
-    DeviceType as DeviceType_model,
-    Manufacturer as Manufacturer_model,
-    Site,
-    Device,
-)
+from django.utils import timezone
 
+from dcim.models import Device, Site
+
+from netdoc.models import Discoverable, Credential, DiscoveryModeChoices
 from netdoc import utils
-from netdoc.schemas import manufacturer as manufacturer_api, devicerole, devicetype
 
 
 def get_schema():
-    """Return the JSON schema to validate Device data."""
+    """Return the JSON schema to validate Discoverable data."""
     return {
         "type": "object",
         "properties": {
-            "name": {
+            "address": {
                 "type": "string",
-                "transform": ["toUpperCase"],
+                "format": "ipv4",
             },
-            "device_role_id": {
+            "device_id": {
                 "type": "integer",
-                "enum": list(
-                    DeviceRole_model.objects.all().values_list("id", flat=True)
-                ),
+                "enum": list(Device.objects.all().values_list("id", flat=True)),
             },
-            "manufacturer_id": {
+            "credential_id": {
                 "type": "integer",
-                "enum": list(
-                    Manufacturer_model.objects.all().values_list("id", flat=True)
-                ),
+                "enum": list(Credential.objects.all().values_list("id", flat=True)),
             },
-            "device_type_id": {
-                "type": "integer",
-                "enum": list(
-                    DeviceType_model.objects.all().values_list("id", flat=True)
-                ),
+            "discoverable": {
+                "type": "boolean",
+            },
+            "last_discovered_at": {
+                "type": "string",
+                "format": "date-time",
             },
-            "serial_number": {
+            "mode": {
                 "type": "string",
-                "transform": ["toUpperCase"],
+                "enum": [key for key, value in DiscoveryModeChoices()],
             },
             "site_id": {
                 "type": "integer",
                 "enum": list(Site.objects.all().values_list("id", flat=True)),
             },
         },
     }
 
 
 def get_schema_create():
-    """Return the JSON schema to validate new Device objects."""
+    """Return the JSON schema to validate new Discoverable objects."""
     schema = get_schema()
     schema["required"] = [
-        "name",
-        "device_role_id",
-        "device_type_id",
+        "address",
+        "credential_id",
+        "mode",
         "site_id",
     ]
     return schema
 
 
-def create(manufacturer="Unknown", **kwargs):
-    """Create a Device.
-
-    Before need to get or create Manufacturer, DeviceModel, and DeviceType.
-    """
-    unknown_model = (
-        "Unknown device"
-        if manufacturer == "Unknown"
-        else f"Unknown {manufacturer} device"
-    )
-    manufacturer_o = manufacturer_api.get(name=manufacturer)
-    if not manufacturer_o:
-        manufacturer_o = manufacturer_api.create(name=manufacturer)
-
-    devicerole_o = devicerole.get(name="Unknown")
-    if not devicerole_o:
-        devicerole_o = devicerole.create(name="Unknown")
-
-    devicetype_o = devicetype.get(
-        model=unknown_model, manufacturer_id=manufacturer_o.id
-    )
-    if not devicetype_o:
-        devicetype_o = devicetype.create(
-            model=unknown_model, manufacturer_id=manufacturer_o.id
-        )
-
-    kwargs.update(
-        {
-            "device_role_id": devicerole_o.id,
-            "device_type_id": devicetype_o.id,
-        }
-    )
-
+def create(**kwargs):
+    """Create a Discoverable."""
     kwargs = utils.delete_empty_keys(kwargs)
     validate(kwargs, get_schema_create(), format_checker=FormatChecker())
-    obj = utils.object_create(Device, **kwargs)
+    obj = utils.object_create(Discoverable, **kwargs)
     return obj
 
 
-def get(name):
-    """Return a Device."""
-    obj = utils.object_get_or_none(Device, name=name)
+def get(address, discovered=False):
+    """Return a Discoverable given IP address.
+
+    Update last_discovered_at if required.
+    """
+    obj = utils.object_get_or_none(Discoverable, address=address)
+    if obj and discovered:
+        obj = utils.object_update(obj, last_discovered_at=timezone.now())
     return obj
 
 
 def get_list(**kwargs):
-    """Get a list of Device objects."""
+    """Get a list of Discoverable objects."""
     validate(kwargs, get_schema(), format_checker=FormatChecker())
-    result = utils.object_list(Device, **kwargs)
+    result = utils.object_list(Discoverable, **kwargs)
     return result
 
 
+def get_or_create(address, **kwargs):
+    """Get or create a Discoverable."""
+    created = False
+    data = {
+        **kwargs,
+        "address": address,
+    }
+    data = utils.delete_empty_keys(data)
+    validate(data, get_schema_create(), format_checker=FormatChecker())
+
+    obj = utils.object_get_or_none(Discoverable, address=address)
+    if not obj:
+        obj = utils.object_create(Discoverable, address=address, **kwargs)
+        created = True
+
+    return obj, created
+
+
 def update(obj, **kwargs):
-    """Update a Device."""
-    update_if_not_set = ["serial_number"]
+    """Update a Discoverable."""
+    update_if_not_set = ["device_id"]
+    update_always = ["last_discovered_at"]
 
-    kwargs = utils.delete_empty_keys(kwargs)
     validate(kwargs, get_schema(), format_checker=FormatChecker())
     kwargs_if_not_set = utils.filter_keys(kwargs, update_if_not_set)
+    kwargs_always = utils.filter_keys(kwargs, update_always)
+    obj = utils.object_update(obj, **kwargs_always, force=True)
+
+    # Before updating device_id we need to check for integrity
+    if kwargs_if_not_set.get("device_id"):
+        # Check if the device is already associated
+        obj_qs = Discoverable.objects.filter(
+            device_id=kwargs_if_not_set.get("device_id")
+        )
+        if obj_qs:
+            # A Discoverable with the same address or the same Device ID already exist
+            return obj_qs[0]
     obj = utils.object_update(obj, **kwargs_if_not_set, force=False)
     return obj
-
-
-def update_management(obj, discoverable_ip_address):
-    """Update primary IP address if match the Discoverable IP address.
-
-    Return True if management IP is set.
-    """
-    # Set management IP address
-    for interface in obj.interfaces.filter(ip_addresses__isnull=False):
-        # For each interface
-        for ip_address_o in interface.ip_addresses.all():
-            # For each configured IP address
-            if discoverable_ip_address == str(ip_address_o.address.ip):
-                obj.primary_ip4 = ip_address_o
-                obj.save()
-                return True
-    return False
```

### Comparing `netdoc-0.9.58/netdoc/schemas/devicerole.py` & `netdoc-0.9.59/netdoc/schemas/devicerole.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/schemas/devicetype.py` & `netdoc-0.9.59/netdoc/schemas/devicetype.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/schemas/discoverylog.py` & `netdoc-0.9.59/netdoc/schemas/discoverylog.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/schemas/interface.py` & `netdoc-0.9.59/netdoc/schemas/interface.py`

 * *Files 17% similar despite different names*

```diff
@@ -194,32 +194,68 @@
         tagged_vlans = []
 
     if mode == "tagged" and tagged_vlans and len(tagged_vlans) >= 4093:
         # Trunk with all VLANs (override mode)
         # In some switch the trunk is excluding native VLAN, so total is 4093.
         obj.mode = "tagged-all"
         obj.save()
-    elif mode == "tagged" and tagged_vlans:
+    elif mode == "tagged":
         # Trunk with some VLANs
-        # Get current VLAN IDs and compare them with tagged_vlans
+        # Query once to speed up the process
+        current_tagged_vlan_list = list(
+            obj.tagged_vlans.all().order_by("vid").values_list("vid", flat=True)
+        )
+        existent_vlan_qs = VLAN_model.objects.all()
+        existent_vlan_list = list(
+            existent_vlan_qs.values_list("vid", flat=True).order_by("vid").distinct()
+        )
+        vlans_to_be_created = []
+        vlans_to_be_added = []
+        vlans_to_be_removed = []
+
+        # Find VLANs to be added
         for vid in tagged_vlans:
-            # Add missing VLANs
-            if not obj.tagged_vlans.filter(vid=vid):
-                vlan_qs = vlan.get_list(vid=vid)
-                if vlan_qs:
-                    vlan_o = vlan_qs.pop()
-                else:
-                    # VLAN does not exist, creating one with default name
-                    vlan_o = vlan.create(vid=vid, name=f"VLAN{vid:04d}")
+            if vid not in current_tagged_vlan_list:
+                vlans_to_be_added.append(vid)
+
+        # Find VLANs to be removed
+        for vid in current_tagged_vlan_list:
+            if vid not in tagged_vlans:
+                vlans_to_be_removed.append(vlan)
+
+        # Find missing VLANs
+        for tagged_vlan in tagged_vlans:
+            if tagged_vlan not in existent_vlan_list:
+                # VLAN needs to be created and added to interface (tagged)
+                vlans_to_be_created.append(
+                    VLAN_model(
+                        vid=tagged_vlan, name=f"VLAN{tagged_vlan:04d}", status="active"
+                    )
+                )
+
+        # Bulk create missing VLANs
+        VLAN_model.objects.bulk_create(vlans_to_be_created)
+
+        if vlans_to_be_added or vlans_to_be_removed:
+            # Map VLAN ID with primary key to speed up the process
+            vlan_vid_id_map = {
+                vlan_item["vid"]: vlan_item["pk"]
+                for vlan_item in list(VLAN_model.objects.all().values("vid", "pk"))
+            }
+
+            for vid in vlans_to_be_added:
+                # Add missing VLAN
+                vlan_o = existent_vlan_qs.get(id=vlan_vid_id_map[vid])
                 obj.tagged_vlans.add(vlan_o)
 
-        for vlan_o in obj.tagged_vlans.all():
-            # Remove unconfigured VLANs
-            if vlan_o.vid not in tagged_vlans:
+            for vlan_o in vlans_to_be_removed:
+                # Remove unconfigured VLANs
+                vlan_o = existent_vlan_qs.get(id=vlan_vid_id_map[vid])
                 obj.tagged_vlans.remove(vlan_o)
+
         obj.mode = mode
         obj.save()
 
     if untagged_vlan and mode in ["tagged", "access"]:
         # Get current VLAN IDs and compare them with untagged_vlan
         if not obj.untagged_vlan or obj.untagged_vlan != untagged_vlan:
             # A VLAN with a different VLAN ID is set
```

### Comparing `netdoc-0.9.58/netdoc/schemas/ipaddress.py` & `netdoc-0.9.59/netdoc/schemas/ipaddress.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/schemas/macaddresstableentry.py` & `netdoc-0.9.59/netdoc/schemas/macaddresstableentry.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/schemas/manufacturer.py` & `netdoc-0.9.59/netdoc/schemas/manufacturer.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/schemas/prefix.py` & `netdoc-0.9.59/netdoc/schemas/prefix.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/schemas/routetableentry.py` & `netdoc-0.9.59/netdoc/schemas/routetableentry.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/schemas/site.py` & `netdoc-0.9.59/netdoc/schemas/site.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/schemas/vlan.py` & `netdoc-0.9.59/netdoc/schemas/vlan.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/schemas/vrf.py` & `netdoc-0.9.59/netdoc/schemas/vrf.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/scripts/NetDoc.py` & `netdoc-0.9.59/netdoc/scripts/NetDoc.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/static/netdoc/css/LICENSE` & `netdoc-0.9.59/netdoc/static/netdoc/css/LICENSE`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/static/netdoc/css/vis-network.min.css` & `netdoc-0.9.59/netdoc/static/netdoc/css/vis-network.min.css`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/static/netdoc/img/LICENSE` & `netdoc-0.9.59/netdoc/static/netdoc/img/LICENSE`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/static/netdoc/img/access-switch.png` & `netdoc-0.9.59/netdoc/static/netdoc/img/access-switch.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/static/netdoc/img/backup.png` & `netdoc-0.9.59/netdoc/static/netdoc/img/backup.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/static/netdoc/img/circuit.png` & `netdoc-0.9.59/netdoc/static/netdoc/img/circuit.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/static/netdoc/img/core-switch.png` & `netdoc-0.9.59/netdoc/static/netdoc/img/core-switch.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/static/netdoc/img/distribution-switch.png` & `netdoc-0.9.59/netdoc/static/netdoc/img/distribution-switch.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/static/netdoc/img/firewall.png` & `netdoc-0.9.59/netdoc/static/netdoc/img/firewall.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/static/netdoc/img/internal-switch.png` & `netdoc-0.9.59/netdoc/static/netdoc/img/internal-switch.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/static/netdoc/img/isp-cpe-material.png` & `netdoc-0.9.59/netdoc/static/netdoc/img/isp-cpe-material.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/static/netdoc/img/non-racked-devices.png` & `netdoc-0.9.59/netdoc/static/netdoc/img/non-racked-devices.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/static/netdoc/img/power-feed.png` & `netdoc-0.9.59/netdoc/static/netdoc/img/power-feed.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/static/netdoc/img/power-panel.png` & `netdoc-0.9.59/netdoc/static/netdoc/img/power-panel.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/static/netdoc/img/power-units.png` & `netdoc-0.9.59/netdoc/static/netdoc/img/power-units.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/static/netdoc/img/provider-networks.png` & `netdoc-0.9.59/netdoc/static/netdoc/img/provider-networks.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/static/netdoc/img/router.png` & `netdoc-0.9.59/netdoc/static/netdoc/img/router.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/static/netdoc/img/server.png` & `netdoc-0.9.59/netdoc/static/netdoc/img/server.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/static/netdoc/img/storage.png` & `netdoc-0.9.59/netdoc/static/netdoc/img/storage.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/static/netdoc/img/unknown.png` & `netdoc-0.9.59/netdoc/static/netdoc/img/unknown.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/static/netdoc/img/wan-network.png` & `netdoc-0.9.59/netdoc/static/netdoc/img/wan-network.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/static/netdoc/img/wireless-ap.png` & `netdoc-0.9.59/netdoc/static/netdoc/img/wireless-ap.png`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/static/netdoc/js/LICENSE` & `netdoc-0.9.59/netdoc/static/netdoc/js/LICENSE`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/static/netdoc/js/diagram.js` & `netdoc-0.9.59/netdoc/static/netdoc/js/diagram.js`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/static/netdoc/js/netdoc.js` & `netdoc-0.9.59/netdoc/static/netdoc/js/netdoc.js`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/static/netdoc/js/vis-network.min.js` & `netdoc-0.9.59/netdoc/static/netdoc/js/vis-network.min.js`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/static/netdoc/js/vis-network.min.js.map` & `netdoc-0.9.59/netdoc/static/netdoc/js/vis-network.min.js.map`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/tables.py` & `netdoc-0.9.59/netdoc/tables.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/tasks.py` & `netdoc-0.9.59/netdoc/tasks.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/templates/netdoc/arptableentry.html` & `netdoc-0.9.59/netdoc/templates/netdoc/arptableentry.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/templates/netdoc/credential.html` & `netdoc-0.9.59/netdoc/templates/netdoc/credential.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/templates/netdoc/diagram.html` & `netdoc-0.9.59/netdoc/templates/netdoc/diagram.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/templates/netdoc/discoverable.html` & `netdoc-0.9.59/netdoc/templates/netdoc/discoverable.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/templates/netdoc/discoverable_bulk_discover.html` & `netdoc-0.9.59/netdoc/templates/netdoc/discoverable_bulk_discover.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/templates/netdoc/discoverable_discover.html` & `netdoc-0.9.59/netdoc/templates/netdoc/discoverable_discover.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/templates/netdoc/discoverable_list.html` & `netdoc-0.9.59/netdoc/templates/netdoc/discoverable_list.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/templates/netdoc/discoverylog.html` & `netdoc-0.9.59/netdoc/templates/netdoc/discoverylog.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/templates/netdoc/htmx/discover_form.html` & `netdoc-0.9.59/netdoc/templates/netdoc/htmx/discover_form.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/templates/netdoc/htmx/logexport_form.html` & `netdoc-0.9.59/netdoc/templates/netdoc/htmx/logexport_form.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/templates/netdoc/macaddresstableentry.html` & `netdoc-0.9.59/netdoc/templates/netdoc/macaddresstableentry.html`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/templatetags/__pycache__/netdoc_buttons.cpython-310.pyc` & `netdoc-0.9.59/netdoc/templatetags/__pycache__/netdoc_buttons.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Apr 26 16:55:00 2023 UTC, .py size: 890 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6457 4964 7a03 0000  o.......dWIdz...
+00000000: 6f0d 0d0a 0000 0000 e079 4a64 7a03 0000  o........yJdz...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
 00000030: 5a00 6401 5a01 6402 5a02 6403 5a03 6404  Z.d.Z.d.Z.d.Z.d.
 00000040: 5a04 6405 6406 6c05 6d06 5a06 0100 6405  Z.d.d.l.m.Z...d.
 00000050: 6407 6c07 6d08 5a08 0100 6405 6408 6c09  d.l.m.Z...d.d.l.
 00000060: 6d0a 5a0a 0100 6506 a00b a100 5a0c 650c  m.Z...e.....Z.e.
 00000070: a00d 6409 a101 640a 640b 8400 8301 5a0e  ..d...d.d.....Z.
```

### Comparing `netdoc-0.9.58/netdoc/templatetags/netdoc_buttons.py` & `netdoc-0.9.59/netdoc/templatetags/netdoc_buttons.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/tests/test.py` & `netdoc-0.9.59/netdoc/tests/test.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/topologies.py` & `netdoc-0.9.59/netdoc/topologies.py`

 * *Files 0% similar despite different names*

```diff
@@ -265,15 +265,16 @@
                     networks[network_id]["y"] = details["positions"][
                         str(network_id)
                     ].get("y")
 
             # Create link (Interface to Network)
             link_id = f"{device_id}-{network_id}"
             if link_id not in links and device_id in nodes and network_id in networks:
-                # Add link only if not already added and if device_id and network_id are in the query
+                # Add link only if not already added and if
+                # device_id and network_id are in the query
                 links[link_id] = {
                     "id": link_id,
                     "from": device_id,
                     "from_label": str(address_o.address),
                     "to": network_id,
                     "title": Template(NETWORK_TEMPLATE).render(
                         interface=interface_o, address=address_o
```

### Comparing `netdoc-0.9.58/netdoc/urls.py` & `netdoc-0.9.59/netdoc/urls.py`

 * *Files identical despite different names*

### Comparing `netdoc-0.9.58/netdoc/utils.py` & `netdoc-0.9.59/netdoc/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -767,14 +767,19 @@
 def parent_interface(label):
     """If subinterface return parent interface else return None."""
     label = normalize_interface_label(label)
     if re.match(r"^[^.]+\.[0-9]+$", label):
         # Contains only one "." and ends with numbers
         parent_label = re.sub(r".[0-9]+$", "", label)
         return parent_label
+    if re.match(r"^[^+]+\+\S+$", label):
+        # Contains only one "+" and ends with alphanumeric
+        # Cisco "service instance" Ethernet
+        parent_label = re.sub(r"\+\S+$", "", label)
+        return parent_label
     return None
 
 
 def parse_netmiko_output(output, command, platform, template=None):
     """Parse Netmiko output using NTC templates."""
     if not template:
         # If template is empty, use command as template
```

### Comparing `netdoc-0.9.58/netdoc/views.py` & `netdoc-0.9.59/netdoc/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,17 @@
     """Summary view listing all ARP."""
 
     queryset = models.ArpTableEntry.objects.all().order_by(
         "interface__device__name", "interface__name", "ip_address"
     )
     table = tables.ArpTableEntryTable
     filterset = filtersets.ArpTableEntryFilterSet
-    actions = []  # Read only table
+    actions = [
+        "export",
+    ]
 
 
 class ArpTableView(generic.ObjectView):
     """Detailed ARP table entry view."""
 
     queryset = models.ArpTableEntry.objects.all()
 
@@ -71,14 +73,19 @@
     """Summary view listing all Credential objects."""
 
     queryset = models.Credential.objects.annotate(
         discoverables_count=Count("discoverables")
     ).order_by("name")
     table = tables.CredentialTable
     filterset = filtersets.CredentialFilterSet
+    actions = [
+        "add",
+        "import",
+        "bulk_delete",
+    ]
 
 
 class CredentialView(generic.ObjectView):
     """Detailed Credential view."""
 
     queryset = models.Credential.objects.all()
 
@@ -549,15 +556,17 @@
     """Summary view listing all MAC address."""
 
     queryset = models.MacAddressTableEntry.objects.all().order_by(
         "interface__device__name", "interface__name", "mac_address"
     )
     table = tables.MacAddressTableEntryTable
     filterset = filtersets.MacAddressTableEntryFilterSet
-    actions = []  # Read only table
+    actions = [
+        "export",
+    ]
 
 
 class MacAddressTableView(generic.ObjectView):
     """Detailed MAC address entry view."""
 
     queryset = models.MacAddressTableEntry.objects.all()
     actions = []  # Read only table
@@ -591,8 +600,10 @@
     """Summary view listing all routes."""
 
     queryset = models.RouteTableEntry.objects.all().order_by(
         "device__name", "destination", "protocol", "nexthop_if__name"
     )
     table = tables.RouteTableEntryTable
     filterset = filtersets.RouteTableEntryFilterSet
-    actions = []  # Read only table
+    actions = [
+        "export",
+    ]
```

### Comparing `netdoc-0.9.58/netdoc.egg-info/SOURCES.txt` & `netdoc-0.9.59/netdoc.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 netdoc/ingestors/netmiko_cisco_nxos_show_ip_interface.py
 netdoc/ingestors/netmiko_cisco_nxos_show_ip_route_vrf_all.py
 netdoc/ingestors/netmiko_cisco_nxos_show_lldp_neighbors_detail.py
 netdoc/ingestors/netmiko_cisco_nxos_show_mac_address_table.py
 netdoc/ingestors/netmiko_cisco_nxos_show_port_channel_summary.py
 netdoc/ingestors/netmiko_cisco_nxos_show_vlan.py
 netdoc/ingestors/netmiko_cisco_nxos_show_vrf.py
+netdoc/ingestors/netmiko_cisco_xr_admin_show_inventory.py
 netdoc/ingestors/netmiko_cisco_xr_hostname.py
 netdoc/ingestors/netmiko_cisco_xr_show_arp.py
 netdoc/ingestors/netmiko_cisco_xr_show_cdp_neighbors_detail.py
 netdoc/ingestors/netmiko_cisco_xr_show_interfaces.py
 netdoc/ingestors/netmiko_cisco_xr_show_ipv4_interface.py
 netdoc/ingestors/netmiko_cisco_xr_show_lldp_neighbors.py
 netdoc/ingestors/netmiko_cisco_xr_show_route.py
```

### Comparing `netdoc-0.9.58/setup.py` & `netdoc-0.9.59/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     twine upload dist/*
 """
 
 __author__ = "Andrea Dainese"
 __contact__ = "andrea@adainese.it"
 __copyright__ = "Copyright 2022, Andrea Dainese"
 __license__ = "GPLv3"
-__version__ = "0.9.58"
+__version__ = "0.9.59"
 
 from setuptools import find_packages, setup
 
 setup(
     name="netdoc",
     version=__version__,
     description="Network Documentation plugin for NetBox",
```

