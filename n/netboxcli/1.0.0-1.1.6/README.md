# Comparing `tmp/netboxcli-1.0.0.tar.gz` & `tmp/netboxcli-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netboxcli-1.0.0.tar", last modified: Thu Sep 21 22:11:46 2023, max compression
+gzip compressed data, was "netboxcli-1.1.6.tar", max compression
```

## Comparing `netboxcli-1.0.0.tar` & `netboxcli-1.1.6.tar`

### file list

```diff
@@ -1,126 +1,106 @@
-drwxr-xr-x   0 kaio.guilherme   (501) staff       (20)        0 2023-09-21 22:11:46.050532 netboxcli-1.0.0/
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     1083 2023-08-29 22:17:00.000000 netboxcli-1.0.0/LICENSE.md
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     7979 2023-09-21 22:11:46.050315 netboxcli-1.0.0/PKG-INFO
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     7396 2023-09-21 22:11:28.000000 netboxcli-1.0.0/README.md
-drwxr-xr-x   0 kaio.guilherme   (501) staff       (20)        0 2023-09-21 22:11:46.027378 netboxcli-1.0.0/netboxCli/
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)      106 2023-08-29 19:26:46.000000 netboxcli-1.0.0/netboxCli/__init__.py
-drwxr-xr-x   0 kaio.guilherme   (501) staff       (20)        0 2023-09-21 22:11:46.029110 netboxcli-1.0.0/netboxCli/circuits/
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)      791 2023-09-21 21:41:31.000000 netboxcli-1.0.0/netboxCli/circuits/__init__.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     2001 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/circuits/circuit_types.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     2002 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/circuits/circuits.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     2005 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/circuits/provider_accounts.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     2005 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/circuits/provider_networks.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     1998 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/circuits/providers.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     1976 2023-09-21 22:07:06.000000 netboxcli-1.0.0/netboxCli/client.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     6440 2023-09-21 22:07:06.000000 netboxcli-1.0.0/netboxCli/compile.py
-drwxr-xr-x   0 kaio.guilherme   (501) staff       (20)        0 2023-09-21 22:11:46.030692 netboxcli-1.0.0/netboxCli/connections/
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)      794 2023-09-21 14:50:22.000000 netboxcli-1.0.0/netboxCli/connections/__init__.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     1995 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/connections/cables.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     2007 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/connections/console_connections.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     2009 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/connections/interface_connections.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     2005 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/connections/power_connections.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     2002 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/connections/wireless_links.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     1853 2023-09-21 15:28:11.000000 netboxcli-1.0.0/netboxCli/core.py
-drwxr-xr-x   0 kaio.guilherme   (501) staff       (20)        0 2023-09-21 22:11:46.032596 netboxcli-1.0.0/netboxCli/customization/
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     1268 2023-09-21 22:07:06.000000 netboxcli-1.0.0/netboxCli/customization/__init__.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     2007 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/customization/custom_field_choices.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     2001 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/customization/custom_fields.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     2000 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/customization/custom_links.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     2004 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/customization/export_templates.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     2005 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/customization/image_attachments.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     1996 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/customization/reports.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     2001 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/customization/saved_filters.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     1996 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/customization/scripts.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     1993 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/customization/tags.py
-drwxr-xr-x   0 kaio.guilherme   (501) staff       (20)        0 2023-09-21 22:11:46.036072 netboxcli-1.0.0/netboxCli/devices/
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     2550 2023-09-21 14:48:45.000000 netboxcli-1.0.0/netboxCli/devices/__init__.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     2001 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/devices/console_ports.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     2007 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/devices/console_server_ports.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     2000 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/devices/device_types.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     2001 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/devices/devices.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     2001 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/devices/devices_roles.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     1999 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/devices/front_ports.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     1999 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/devices/interfaces.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     2003 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/devices/inventory_items.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     2008 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/devices/inventory_items_roles.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     2002 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/devices/manufacturers.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     1996 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/devices/modules.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     2000 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/devices/modules_bays.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     2001 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/devices/modules_types.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     1998 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/devices/platforms.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     2001 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/devices/power_outlets.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     1999 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/devices/power_ports.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     1998 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/devices/rear_ports.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     2003 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/devices/virtual_chassis.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     2011 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/devices/virtual_chassis_contexts.py
-drwxr-xr-x   0 kaio.guilherme   (501) staff       (20)        0 2023-09-21 22:11:46.039118 netboxcli-1.0.0/netboxCli/ipam/
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     1699 2023-08-30 18:19:14.000000 netboxcli-1.0.0/netboxCli/ipam/__init__.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     1999 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/ipam/aggregates.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     1998 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/ipam/asn_ranges.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     1993 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/ipam/asns.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     1999 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/ipam/fhrp_groups.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     2000 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/ipam/ip_addresses.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     1997 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/ipam/ip_ranges.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     2000 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/ipam/prefix_roles.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     1997 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/ipam/prefixes.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     1993 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/ipam/rirs.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     2002 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/ipam/router_targets.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     1997 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/ipam/services.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     2006 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/ipam/services_templates.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     1999 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/ipam/vlan_groups.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     1994 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/ipam/vlans.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     1993 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/ipam/vrfs.py
-drwxr-xr-x   0 kaio.guilherme   (501) staff       (20)        0 2023-09-21 22:11:46.040031 netboxcli-1.0.0/netboxCli/operations/
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)      719 2023-09-21 22:07:06.000000 netboxcli-1.0.0/netboxCli/operations/__init__.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     1998 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/operations/change_log.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     2000 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/operations/data_sources.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     1993 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/operations/jobs.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     2003 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/operations/journal_entries.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     1997 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/operations/webhooks.py
-drwxr-xr-x   0 kaio.guilherme   (501) staff       (20)        0 2023-09-21 22:11:46.045892 netboxcli-1.0.0/netboxCli/organization/
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     1659 2023-08-30 19:00:09.000000 netboxcli-1.0.0/netboxCli/organization/__init__.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     2008 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/organization/contact_associations.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     2002 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/organization/contact_groups.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     2001 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/organization/contact_roles.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     1997 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/organization/contacts.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     1998 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/organization/locations.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     1994 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/organization/racks.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     1999 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/organization/racks_roles.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     1996 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/organization/regions.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     2001 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/organization/reservations.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     1999 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/organization/site_groups.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     1994 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/organization/sites.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     2001 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/organization/tenant_groups.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     1996 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/organization/tenants.py
-drwxr-xr-x   0 kaio.guilherme   (501) staff       (20)        0 2023-09-21 22:11:46.046500 netboxcli-1.0.0/netboxCli/overlay/
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)      322 2023-09-21 21:41:31.000000 netboxcli-1.0.0/netboxCli/overlay/__init__.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     1995 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/overlay/l2vpns.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     2001 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/overlay/terminations.py
-drwxr-xr-x   0 kaio.guilherme   (501) staff       (20)        0 2023-09-21 22:11:46.047238 netboxcli-1.0.0/netboxCli/power/
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)      332 2023-09-21 21:41:31.000000 netboxcli-1.0.0/netboxCli/power/__init__.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     1999 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/power/power_feeds.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     2000 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/power/power_panels.py
-drwxr-xr-x   0 kaio.guilherme   (501) staff       (20)        0 2023-09-21 22:11:46.047793 netboxcli-1.0.0/netboxCli/provisioning/
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)      393 2023-09-21 22:07:06.000000 netboxcli-1.0.0/netboxCli/provisioning/__init__.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     2003 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/provisioning/config_contexts.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     2004 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/provisioning/config_templates.py
-drwxr-xr-x   0 kaio.guilherme   (501) staff       (20)        0 2023-09-21 22:11:46.048841 netboxcli-1.0.0/netboxCli/virtualization/
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     1527 2023-08-30 18:28:18.000000 netboxcli-1.0.0/netboxCli/virtualization/__init__.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     2002 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/virtualization/cluster_groups.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     2001 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/virtualization/cluster_types.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     1997 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/virtualization/clusters.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     1999 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/virtualization/interfaces.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     2004 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/virtualization/virtual_machines.py
-drwxr-xr-x   0 kaio.guilherme   (501) staff       (20)        0 2023-09-21 22:11:46.049415 netboxcli-1.0.0/netboxCli/wireless/
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)      526 2023-09-21 15:09:18.000000 netboxcli-1.0.0/netboxCli/wireless/__init__.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     2006 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/wireless/wireless_lan_groups.py
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     2001 2023-09-21 22:03:39.000000 netboxcli-1.0.0/netboxCli/wireless/wireless_lans.py
-drwxr-xr-x   0 kaio.guilherme   (501) staff       (20)        0 2023-09-21 22:11:46.050040 netboxcli-1.0.0/netboxcli.egg-info/
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     7979 2023-09-21 22:11:46.000000 netboxcli-1.0.0/netboxcli.egg-info/PKG-INFO
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)     3669 2023-09-21 22:11:46.000000 netboxcli-1.0.0/netboxcli.egg-info/SOURCES.txt
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)        1 2023-09-21 22:11:46.000000 netboxcli-1.0.0/netboxcli.egg-info/dependency_links.txt
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)        9 2023-09-21 22:11:46.000000 netboxcli-1.0.0/netboxcli.egg-info/requires.txt
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)       10 2023-09-21 22:11:46.000000 netboxcli-1.0.0/netboxcli.egg-info/top_level.txt
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)      635 2023-09-21 22:11:28.000000 netboxcli-1.0.0/pyproject.toml
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)       38 2023-09-21 22:11:46.050573 netboxcli-1.0.0/setup.cfg
--rw-r--r--   0 kaio.guilherme   (501) staff       (20)      610 2023-09-21 22:11:28.000000 netboxcli-1.0.0/setup.py
+-rw-r--r--   0        0        0     1071 2024-04-24 15:18:16.992183 netboxcli-1.1.6/LICENSE
+-rw-r--r--   0        0        0     6700 2024-04-25 01:49:13.476771 netboxcli-1.1.6/README.md
+-rw-r--r--   0        0        0       76 2024-04-23 00:51:23.567947 netboxcli-1.1.6/netboxcli/__init__.py
+-rw-r--r--   0        0        0     1061 2024-04-23 00:51:23.568077 netboxcli-1.1.6/netboxcli/circuits/__init__.py
+-rw-r--r--   0        0        0     3670 2024-04-24 20:41:11.795528 netboxcli-1.1.6/netboxcli/circuits/circuit_types.py
+-rw-r--r--   0        0        0     3596 2024-04-24 20:41:11.795530 netboxcli-1.1.6/netboxcli/circuits/circuits.py
+-rw-r--r--   0        0        0     3734 2024-04-24 20:41:11.818295 netboxcli-1.1.6/netboxcli/circuits/provider_accounts.py
+-rw-r--r--   0        0        0     3734 2024-04-24 20:41:11.831893 netboxcli-1.1.6/netboxcli/circuits/provider_networks.py
+-rw-r--r--   0        0        0     3619 2024-04-24 20:41:11.832829 netboxcli-1.1.6/netboxcli/circuits/providers.py
+-rw-r--r--   0        0        0     3886 2024-04-24 21:46:42.423065 netboxcli-1.1.6/netboxcli/client.py
+-rw-r--r--   0        0        0      988 2024-04-23 00:51:23.568760 netboxcli-1.1.6/netboxcli/connections/__init__.py
+-rw-r--r--   0        0        0     3584 2024-04-24 20:41:11.843992 netboxcli-1.1.6/netboxcli/connections/cables.py
+-rw-r--r--   0        0        0     3711 2024-04-24 20:41:11.843191 netboxcli-1.1.6/netboxcli/connections/wireless_links.py
+-rw-r--r--   0        0        0     2960 2024-04-24 20:41:11.903352 netboxcli-1.1.6/netboxcli/core.py
+-rw-r--r--   0        0        0     1427 2024-04-23 00:51:23.569183 netboxcli-1.1.6/netboxcli/customization/__init__.py
+-rw-r--r--   0        0        0     3710 2024-04-24 20:41:11.858537 netboxcli-1.1.6/netboxcli/customization/custom_fields.py
+-rw-r--r--   0        0        0     3694 2024-04-24 20:41:11.848063 netboxcli-1.1.6/netboxcli/customization/custom_links.py
+-rw-r--r--   0        0        0     3758 2024-04-24 20:41:11.854208 netboxcli-1.1.6/netboxcli/customization/export_templates.py
+-rw-r--r--   0        0        0     3774 2024-04-24 20:41:11.846501 netboxcli-1.1.6/netboxcli/customization/image_attachments.py
+-rw-r--r--   0        0        0     3615 2024-04-24 20:41:11.855336 netboxcli-1.1.6/netboxcli/customization/reports.py
+-rw-r--r--   0        0        0     3710 2024-04-24 20:41:11.866146 netboxcli-1.1.6/netboxcli/customization/saved_filters.py
+-rw-r--r--   0        0        0     3615 2024-04-24 20:41:11.866879 netboxcli-1.1.6/netboxcli/customization/scripts.py
+-rw-r--r--   0        0        0     3567 2024-04-24 20:41:11.858744 netboxcli-1.1.6/netboxcli/customization/tags.py
+-rw-r--r--   0        0        0     2794 2024-04-23 00:51:23.569920 netboxcli-1.1.6/netboxcli/devices/__init__.py
+-rw-r--r--   0        0        0     3673 2024-04-24 20:41:11.879962 netboxcli-1.1.6/netboxcli/devices/console_ports.py
+-rw-r--r--   0        0        0     3784 2024-04-24 20:41:11.871072 netboxcli-1.1.6/netboxcli/devices/console_server_ports.py
+-rw-r--r--   0        0        0     3646 2024-04-24 20:41:11.892840 netboxcli-1.1.6/netboxcli/devices/device_types.py
+-rw-r--r--   0        0        0     3578 2024-04-24 20:41:11.903346 netboxcli-1.1.6/netboxcli/devices/devices.py
+-rw-r--r--   0        0        0     3662 2024-04-24 20:41:11.873894 netboxcli-1.1.6/netboxcli/devices/devices_roles.py
+-rw-r--r--   0        0        0     3641 2024-04-24 20:41:11.886377 netboxcli-1.1.6/netboxcli/devices/front_ports.py
+-rw-r--r--   0        0        0     3626 2024-04-24 20:41:11.883204 netboxcli-1.1.6/netboxcli/devices/interfaces.py
+-rw-r--r--   0        0        0     3694 2024-04-24 20:41:11.889290 netboxcli-1.1.6/netboxcli/devices/inventory_items.py
+-rw-r--r--   0        0        0     3789 2024-04-24 20:41:11.887249 netboxcli-1.1.6/netboxcli/devices/inventory_items_roles.py
+-rw-r--r--   0        0        0     3674 2024-04-24 20:41:11.910637 netboxcli-1.1.6/netboxcli/devices/manufacturers.py
+-rw-r--r--   0        0        0     3573 2024-04-24 20:41:11.902053 netboxcli-1.1.6/netboxcli/devices/modules.py
+-rw-r--r--   0        0        0     3646 2024-04-24 20:41:11.906964 netboxcli-1.1.6/netboxcli/devices/modules_bays.py
+-rw-r--r--   0        0        0     3662 2024-04-24 20:41:11.907469 netboxcli-1.1.6/netboxcli/devices/modules_types.py
+-rw-r--r--   0        0        0     3610 2024-04-24 20:41:11.910435 netboxcli-1.1.6/netboxcli/devices/platforms.py
+-rw-r--r--   0        0        0     3662 2024-04-24 20:41:11.918465 netboxcli-1.1.6/netboxcli/devices/power_outlets.py
+-rw-r--r--   0        0        0     3641 2024-04-24 20:41:11.930625 netboxcli-1.1.6/netboxcli/devices/power_ports.py
+-rw-r--r--   0        0        0     3625 2024-04-24 20:41:11.922720 netboxcli-1.1.6/netboxcli/devices/rear_ports.py
+-rw-r--r--   0        0        0     3705 2024-04-24 20:41:11.922470 netboxcli-1.1.6/netboxcli/devices/virtual_chassis.py
+-rw-r--r--   0        0        0     3837 2024-04-24 20:41:11.928099 netboxcli-1.1.6/netboxcli/devices/virtual_chassis_contexts.py
+-rw-r--r--   0        0        0     1762 2024-04-23 00:51:23.571529 netboxcli-1.1.6/netboxcli/ipam/__init__.py
+-rw-r--r--   0        0        0     3607 2024-04-24 20:41:11.935777 netboxcli-1.1.6/netboxcli/ipam/aggregates.py
+-rw-r--r--   0        0        0     3594 2024-04-24 20:41:11.931280 netboxcli-1.1.6/netboxcli/ipam/asn_ranges.py
+-rw-r--r--   0        0        0     3495 2024-04-24 20:41:11.961218 netboxcli-1.1.6/netboxcli/ipam/asns.py
+-rw-r--r--   0        0        0     3606 2024-04-24 20:41:11.945582 netboxcli-1.1.6/netboxcli/ipam/fhrp_groups.py
+-rw-r--r--   0        0        0     3622 2024-04-24 20:41:11.946885 netboxcli-1.1.6/netboxcli/ipam/ip_addresses.py
+-rw-r--r--   0        0        0     3574 2024-04-24 20:41:11.934862 netboxcli-1.1.6/netboxcli/ipam/ip_ranges.py
+-rw-r--r--   0        0        0     3627 2024-04-24 20:41:11.975295 netboxcli-1.1.6/netboxcli/ipam/prefix_roles.py
+-rw-r--r--   0        0        0     3575 2024-04-24 20:41:11.956754 netboxcli-1.1.6/netboxcli/ipam/prefixes.py
+-rw-r--r--   0        0        0     3495 2024-04-24 20:41:11.945434 netboxcli-1.1.6/netboxcli/ipam/rirs.py
+-rw-r--r--   0        0        0     3654 2024-04-24 20:41:11.964976 netboxcli-1.1.6/netboxcli/ipam/router_targets.py
+-rw-r--r--   0        0        0     3559 2024-04-24 20:41:11.952125 netboxcli-1.1.6/netboxcli/ipam/services.py
+-rw-r--r--   0        0        0     3718 2024-04-24 20:41:11.977858 netboxcli-1.1.6/netboxcli/ipam/services_templates.py
+-rw-r--r--   0        0        0     3606 2024-04-24 20:41:11.965386 netboxcli-1.1.6/netboxcli/ipam/vlan_groups.py
+-rw-r--r--   0        0        0     3511 2024-04-24 20:41:11.965466 netboxcli-1.1.6/netboxcli/ipam/vlans.py
+-rw-r--r--   0        0        0     3495 2024-04-24 20:41:11.974221 netboxcli-1.1.6/netboxcli/ipam/vrfs.py
+-rw-r--r--   0        0        0      651 2024-04-23 00:51:23.572772 netboxcli-1.1.6/netboxcli/operations/__init__.py
+-rw-r--r--   0        0        0     3670 2024-04-24 20:41:11.978961 netboxcli-1.1.6/netboxcli/operations/data_sources.py
+-rw-r--r--   0        0        0     3543 2024-04-24 20:41:11.988380 netboxcli-1.1.6/netboxcli/operations/jobs.py
+-rw-r--r--   0        0        0     3718 2024-04-24 20:41:11.984575 netboxcli-1.1.6/netboxcli/operations/journal_entries.py
+-rw-r--r--   0        0        0     3607 2024-04-24 20:41:11.985937 netboxcli-1.1.6/netboxcli/operations/webhooks.py
+-rw-r--r--   0        0        0     1768 2024-04-23 00:51:23.573238 netboxcli-1.1.6/netboxcli/organization/__init__.py
+-rw-r--r--   0        0        0     3798 2024-04-24 20:41:11.989838 netboxcli-1.1.6/netboxcli/organization/contact_assignments.py
+-rw-r--r--   0        0        0     3718 2024-04-24 20:41:11.987218 netboxcli-1.1.6/netboxcli/organization/contact_groups.py
+-rw-r--r--   0        0        0     3702 2024-04-24 20:41:11.998658 netboxcli-1.1.6/netboxcli/organization/contact_roles.py
+-rw-r--r--   0        0        0     3623 2024-04-24 20:41:12.025470 netboxcli-1.1.6/netboxcli/organization/contacts.py
+-rw-r--r--   0        0        0     3639 2024-04-24 20:41:11.995096 netboxcli-1.1.6/netboxcli/organization/locations.py
+-rw-r--r--   0        0        0     3575 2024-04-24 20:41:12.026947 netboxcli-1.1.6/netboxcli/organization/racks.py
+-rw-r--r--   0        0        0     3670 2024-04-24 20:41:12.000007 netboxcli-1.1.6/netboxcli/organization/racks_roles.py
+-rw-r--r--   0        0        0     3607 2024-04-24 20:41:12.044322 netboxcli-1.1.6/netboxcli/organization/regions.py
+-rw-r--r--   0        0        0     3687 2024-04-24 20:41:12.008898 netboxcli-1.1.6/netboxcli/organization/reservations.py
+-rw-r--r--   0        0        0     3670 2024-04-24 20:41:12.008157 netboxcli-1.1.6/netboxcli/organization/site_groups.py
+-rw-r--r--   0        0        0     3595 2024-04-24 20:41:12.014425 netboxcli-1.1.6/netboxcli/organization/sites.py
+-rw-r--r--   0        0        0     3702 2024-04-24 20:41:12.026117 netboxcli-1.1.6/netboxcli/organization/tenant_groups.py
+-rw-r--r--   0        0        0     3607 2024-04-24 20:41:12.021945 netboxcli-1.1.6/netboxcli/organization/tenants.py
+-rw-r--r--   0        0        0      357 2024-04-23 00:51:23.574391 netboxcli-1.1.6/netboxcli/power/__init__.py
+-rw-r--r--   0        0        0     3618 2024-04-24 20:41:12.027536 netboxcli-1.1.6/netboxcli/power/power_feeds.py
+-rw-r--r--   0        0        0     3634 2024-04-24 20:41:12.047531 netboxcli-1.1.6/netboxcli/power/power_panels.py
+-rw-r--r--   0        0        0      437 2024-04-23 00:51:23.574671 netboxcli-1.1.6/netboxcli/provisioning/__init__.py
+-rw-r--r--   0        0        0     3764 2024-04-24 20:41:12.033723 netboxcli-1.1.6/netboxcli/provisioning/config_contexts.py
+-rw-r--r--   0        0        0     3780 2024-04-24 20:41:12.036407 netboxcli-1.1.6/netboxcli/provisioning/config_templates.py
+-rw-r--r--   0        0        0     1615 2024-04-23 00:51:23.574947 netboxcli-1.1.6/netboxcli/virtualization/__init__.py
+-rw-r--r--   0        0        0     3733 2024-04-24 20:41:12.044595 netboxcli-1.1.6/netboxcli/virtualization/cluster_groups.py
+-rw-r--r--   0        0        0     3717 2024-04-24 20:41:12.059560 netboxcli-1.1.6/netboxcli/virtualization/cluster_types.py
+-rw-r--r--   0        0        0     3638 2024-04-24 20:41:12.064970 netboxcli-1.1.6/netboxcli/virtualization/clusters.py
+-rw-r--r--   0        0        0     3670 2024-04-24 20:41:12.045127 netboxcli-1.1.6/netboxcli/virtualization/interfaces.py
+-rw-r--r--   0        0        0     3765 2024-04-24 20:41:12.047911 netboxcli-1.1.6/netboxcli/virtualization/virtual_machines.py
+-rw-r--r--   0        0        0     1463 2024-04-23 00:51:23.575425 netboxcli-1.1.6/netboxcli/vpn/__init__.py
+-rw-r--r--   0        0        0     3629 2024-04-24 20:41:12.072597 netboxcli-1.1.6/netboxcli/vpn/ike_policies.py
+-rw-r--r--   0        0        0     3645 2024-04-24 20:41:12.059151 netboxcli-1.1.6/netboxcli/vpn/ike_proposals.py
+-rw-r--r--   0        0        0     3661 2024-04-24 20:41:12.064825 netboxcli-1.1.6/netboxcli/vpn/ipsec_policies.py
+-rw-r--r--   0        0        0     3661 2024-04-24 20:41:12.068780 netboxcli-1.1.6/netboxcli/vpn/ipsec_profiles.py
+-rw-r--r--   0        0        0     3677 2024-04-24 20:41:12.068976 netboxcli-1.1.6/netboxcli/vpn/ipsec_proposals.py
+-rw-r--r--   0        0        0     3534 2024-04-24 20:41:12.083757 netboxcli-1.1.6/netboxcli/vpn/l2vpns.py
+-rw-r--r--   0        0        0     3630 2024-04-24 20:41:12.085180 netboxcli-1.1.6/netboxcli/vpn/terminations.py
+-rw-r--r--   0        0        0     3645 2024-04-24 20:41:12.086768 netboxcli-1.1.6/netboxcli/vpn/tunnel_groups.py
+-rw-r--r--   0        0        0     3741 2024-04-24 20:41:12.084751 netboxcli-1.1.6/netboxcli/vpn/tunnel_terminations.py
+-rw-r--r--   0        0        0     3550 2024-04-24 20:41:12.090451 netboxcli-1.1.6/netboxcli/vpn/tunnels.py
+-rw-r--r--   0        0        0      574 2024-04-23 00:51:23.576292 netboxcli-1.1.6/netboxcli/wireless/__init__.py
+-rw-r--r--   0        0        0     3765 2024-04-24 20:41:12.091770 netboxcli-1.1.6/netboxcli/wireless/wireless_lan_groups.py
+-rw-r--r--   0        0        0     3670 2024-04-24 20:41:12.093963 netboxcli-1.1.6/netboxcli/wireless/wireless_lans.py
+-rw-r--r--   0        0        0     2068 2024-04-25 02:41:09.710878 netboxcli-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0     7693 1970-01-01 00:00:00.000000 netboxcli-1.1.6/PKG-INFO
```

### Comparing `netboxcli-1.0.0/LICENSE.md` & `netboxcli-1.1.6/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-
-The MIT License (MIT)
+MIT License
 
 Copyright (c) 2023 kaio Guilherme 
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
@@ -15,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `netboxcli-1.0.0/PKG-INFO` & `netboxcli-1.1.6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,65 +1,72 @@
 Metadata-Version: 2.1
 Name: netboxcli
-Version: 1.0.0
+Version: 1.1.6
 Summary: A Python package to interact with the NetBox API.
-Author-email: kaio Guilherme <kaioguilherme444@outlook.com>
-Project-URL: Homepage, https://github.com/Kaioguilherme1/netbox-client
-Project-URL: Bug Tracker, https://github.com/Kaioguilherme1/netbox-client/issues
-Classifier: Programming Language :: Python :: 3
+License: MIT
+Author: kaio Guilherme 
+Author-email: kaioguilherme444@gmail.com
+Requires-Python: >=3.12,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: System :: Networking
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Project-URL: Bug Tracker, https://github.com/Kaioguilherme1/netbox-client/issues
+Project-URL: Codigo, https://github.com/Kaioguilherme1/netbox-client
+Project-URL: Documentation, https://netboxcli.readthedocs.io/pt/latest/Client/
+Project-URL: Homepage, https://netboxcli.readthedocs.io/pt/latest/
 Description-Content-Type: text/markdown
-License-File: LICENSE.md
-Requires-Dist: requests
 
 # Netbox Client
 
 
-![Badge em Desenvolvimento](http://img.shields.io/static/v1?label=STATUS&message=EM%20DESENVOLVIMENTO&color=GREEN&style=for-the-badge)
+[![Documentation Status](https://readthedocs.org/projects/netboxcli/badge/?version=latest)](https://netboxcli.readthedocs.io/pt/latest/?badge=latest)
+[![pipeline](https://github.com/Kaioguilherme1/netbox-client/actions/workflows/pipeline.yml/badge.svg?branch=main)](https://github.com/Kaioguilherme1/netbox-client/actions/workflows/pipeline.yml)
+[![codecov](https://codecov.io/gh/Kaioguilherme1/netbox-client/graph/badge.svg?token=LMD2ILTE1N)](https://codecov.io/gh/Kaioguilherme1/netbox-client)
+[![PyPI version](https://badge.fury.io/py/netboxcli.svg)](https://badge.fury.io/py/netboxcli)
 ---
 
   O NetboxCli é um pacote Python projetado para simplificar e agilizar a interação com o NetBox, 
   uma popular plataforma de gerenciamento de infraestrutura de rede de código aberto. 
   Com este pacote, você pode facilmente interagir com as funcionalidades do NetBox, 
   como gerenciamento de endereços IP (IPAM) e virtualização.
 
 ## Índice
 * [Netbox Client](#netbox-client)
-* [Índice](#Índice)
 * [📄Dependências](#Dependências)
 * [🔧Instalação](#Instalação)
+* [🚀 Getting Started](https://netboxcli.readthedocs.io/pt/latest/Getting%20started/)
+* [📝Documentação](https://netboxcli.readthedocs.io/pt/latest/)
 * [⚙️Uso](#uso)
 * [📦Desenvolvimento](#Desenvolvimento)
 * [📌Versão](#Versão)
 * [👥Colaboradores](#Colaboradores)
 * [✒️Autores](#Autores)
 * [📑Licença](#Licença)
 
+### Documentação Disponível [aqui](https://netboxcli.readthedocs.io/pt/latest/)
+  
 ## 📄 Dependências 
   Lista as dependencias
   * requests
-  * python 3.11 ou superior
-  * [netbox](https://github.com/netbox-community/netbox)
-  
-## 🔧Instalação
+  * python 3.12 ou superior
+  * [netbox >=3.7.5](https://github.com/netbox-community/netbox)
 
-### 📁 Acesso ao projeto
+## 🔧 Instalação
 
-Apresentar formas de baixar seu projeto.
-
-[Baixar projeto](https://github.com/Kaioguilherme1/netbox-client/archive/refs/heads/main.zip)
-#### Baixar o pacote via terminal.
 ```
 pip install netboxcli
 ```
-## ⚙️ Uso
 
-O NetboxCli é uma ferramenta poderosa para interagir com o NetBox de maneira simples e eficiente. Ele oferece classes consistentes com métodos padronizados para lidar com diversas funcionalidades, incluindo IPAM e Virtualização. Você pode navegar entre as classes da mesma forma que nas abas do NetBox. Aqui estão os passos básicos para começar a usar o NetboxCli:
+## ⚙️ uso
 
 ### Importando o Módulo e Preparando a Conexão
 
 Antes de começar a interagir com o NetBox, você precisa importar o módulo `netboxcli` e criar um objeto NetBox para estabelecer a conexão com o servidor. Substitua `'sua_url_aqui'` pelo endereço IP e porta do seu servidor NetBox e `'seu_token_aqui'` pelo seu token de API.
 
 ```python
 import netboxcli as nb
@@ -115,23 +122,21 @@
 ### Exemplo de Virtualização: Excluir uma Máquina Virtual
 
 ```python
 # Exemplo de exclusão de uma máquina virtual pelo ID
 deleted_vm_id = nb_client.virtualization.virtual_machines.delete(id=1)
 
 ```
+para mais exemplos de uso acesse a [documentação](https://netboxcli.readthedocs.io/pt/latest/Getting%20started/)
 
 ### Personalizando e Extendendo
 
 Além das operações básicas, você pode personalizar e estender as funcionalidades do NetboxCli de acordo com suas necessidades específicas. As classes finais oferecem uma base sólida para construir interações mais avançadas com a API do NetBox.
 
 Lembre-se de substituir os exemplos de dados e IDs pelos valores reais correspondentes ao seu ambiente NetBox.
-## 📦 Desenvolvimento
-
-Nesta seção, você encontrará informações sobre o desenvolvimento contínuo do NetboxCli. Estamos trabalhando para expandir as funcionalidades e fornecer suporte abrangente para todas as abas disponíveis no NetBox 3.5 e versões posteriores. Atualizações e novas funcionalidades serão lançadas com o tempo, conforme o projeto evolui.
 
 ### Objetivo
 
 O objetivo do projeto NetboxCli é fornecer uma interface Python simples e eficiente para interagir com o NetBox. 
 oferecendo uma alternativa conveniente para os administradores de rede que desejam automatizar tarefas e gerenciar recursos de infraestrutura de maneira mais fácil.
 
 ## Checklist de Desenvolvimento
@@ -139,40 +144,34 @@
 Aqui está um checklist do que está atualmente disponível no NetboxCli e do que será adicionado no futuro:
 
 - [x]  **Organization:** Gerencie informações sobre organizações e empresas associadas aos seus recursos de rede.
 - [x]  **Devices:** Acesse e gerencie dispositivos de rede, incluindo servidores, roteadores e switches.
 - [x]  **Connections:** Interaja com conexões físicas e lógicas entre dispositivos de rede.
 - [x]  **Wireless:** Gerencie redes sem fio, pontos de acesso e configurações de Wi-Fi.
 - [x]  **IPAM:** Simplifique a gestão de blocos de endereços IP, facilitando a adição, recuperação e atualização.
-- [x]  **Overlay:** Suporte para redes de sobreposição, como VPNs e túneis.
+- [x]  **Vpn:** Suporte para redes de sobreposição, como VPNs e túneis.
 - [x]  **Virtualização:** Gerencie máquinas virtuais de maneira eficaz, desde a criação até a exclusão.
 - [x]  **Circuits:** Gerencie circuitos de rede, como conexões de fibra óptica e links externos.
 - [x]  **Power:** Acesse informações relacionadas ao fornecimento de energia e energia de seus dispositivos.
 - [x]  **Provisioning:** Suporte para provisionamento de rede, incluindo configurações de DHCP e DNS.
 - [x]  **Customization:** Gerencie modelos e configurações personalizadas para seus dispositivos de rede.
 - [x]  **Operations:** Acesse e gerencie informações sobre operações de rede, como manutenção e atualizações.
 - [x]  **Extras:** Integração com plugins e extensões adicionais para funcionalidades personalizadas.
 
 Este checklist será atualizado à medida que novas funcionalidades forem implementadas. 
 Agradecemos por seu interesse e paciência enquanto trabalhamos para tornar o NetboxCli mais abrangente e útil para suas necessidades de automação e gerenciamento de rede.
 
-## 📌 Versão 1.0.0
-
-### **Adições na Versão 1.0.0**
-
-- **Connections:** Adicionado suporte para conexões físicas e lógicas entre dispositivos de rede.
-- **Overlay:** Adicionado suporte para redes de sobreposição, como VPNs e túneis.
-- **Circuits:** Adicionado suporte para circuitos de rede, como conexões de fibra óptica e links externos.
-- **Power:** Adicionado suporte para informações relacionadas ao fornecimento de energia e energia de seus dispositivos.
-- **Provisioning:** Adicionado suporte para provisionamento de rede, incluindo configurações de DHCP e DNS.
-- **Customization:** Adicionado suporte para modelos e configurações personalizadas para seus dispositivos de rede.
-- **Operations:** Adicionado suporte para informações sobre operações de rede, como manutenção e atualizações.
+## 📌 Versão 1.1.5
 
+### **Adições na Versão 1.1.5**
 
+- **Correções de Bugs: ** Correção de bugs menores e melhorias de desempenho em todo o código.
+- **Melhorias de Desempenho: ** Otimização de consultas e operações para melhorar o desempenho geral do NetboxCli.
 
 ## ✒️ Autores
 
 * **developer** - *Initial Work* - [Kaio Guilherme](https://github.com/Kaioguilherme1)
 
 ## 📑 Licença
 
 Esse projeto esta sob a licença(MIT) - veja o arquivo [Licenca.md](https://github.com/Kaioguilherme1/netbox-client/blob/main/Licenca) para mais detalhes.
+
```

### Comparing `netboxcli-1.0.0/README.md` & `netboxcli-1.1.6/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,50 +1,49 @@
 # Netbox Client
 
 
-![Badge em Desenvolvimento](http://img.shields.io/static/v1?label=STATUS&message=EM%20DESENVOLVIMENTO&color=GREEN&style=for-the-badge)
+[![Documentation Status](https://readthedocs.org/projects/netboxcli/badge/?version=latest)](https://netboxcli.readthedocs.io/pt/latest/?badge=latest)
+[![pipeline](https://github.com/Kaioguilherme1/netbox-client/actions/workflows/pipeline.yml/badge.svg?branch=main)](https://github.com/Kaioguilherme1/netbox-client/actions/workflows/pipeline.yml)
+[![codecov](https://codecov.io/gh/Kaioguilherme1/netbox-client/graph/badge.svg?token=LMD2ILTE1N)](https://codecov.io/gh/Kaioguilherme1/netbox-client)
+[![PyPI version](https://badge.fury.io/py/netboxcli.svg)](https://badge.fury.io/py/netboxcli)
 ---
 
   O NetboxCli é um pacote Python projetado para simplificar e agilizar a interação com o NetBox, 
   uma popular plataforma de gerenciamento de infraestrutura de rede de código aberto. 
   Com este pacote, você pode facilmente interagir com as funcionalidades do NetBox, 
   como gerenciamento de endereços IP (IPAM) e virtualização.
 
 ## Índice
 * [Netbox Client](#netbox-client)
-* [Índice](#Índice)
 * [📄Dependências](#Dependências)
 * [🔧Instalação](#Instalação)
+* [🚀 Getting Started](https://netboxcli.readthedocs.io/pt/latest/Getting%20started/)
+* [📝Documentação](https://netboxcli.readthedocs.io/pt/latest/)
 * [⚙️Uso](#uso)
 * [📦Desenvolvimento](#Desenvolvimento)
 * [📌Versão](#Versão)
 * [👥Colaboradores](#Colaboradores)
 * [✒️Autores](#Autores)
 * [📑Licença](#Licença)
 
+### Documentação Disponível [aqui](https://netboxcli.readthedocs.io/pt/latest/)
+  
 ## 📄 Dependências 
   Lista as dependencias
   * requests
-  * python 3.11 ou superior
-  * [netbox](https://github.com/netbox-community/netbox)
-  
-## 🔧Instalação
-
-### 📁 Acesso ao projeto
+  * python 3.12 ou superior
+  * [netbox >=3.7.5](https://github.com/netbox-community/netbox)
 
-Apresentar formas de baixar seu projeto.
+## 🔧 Instalação
 
-[Baixar projeto](https://github.com/Kaioguilherme1/netbox-client/archive/refs/heads/main.zip)
-#### Baixar o pacote via terminal.
 ```
 pip install netboxcli
 ```
-## ⚙️ Uso
 
-O NetboxCli é uma ferramenta poderosa para interagir com o NetBox de maneira simples e eficiente. Ele oferece classes consistentes com métodos padronizados para lidar com diversas funcionalidades, incluindo IPAM e Virtualização. Você pode navegar entre as classes da mesma forma que nas abas do NetBox. Aqui estão os passos básicos para começar a usar o NetboxCli:
+## ⚙️ uso
 
 ### Importando o Módulo e Preparando a Conexão
 
 Antes de começar a interagir com o NetBox, você precisa importar o módulo `netboxcli` e criar um objeto NetBox para estabelecer a conexão com o servidor. Substitua `'sua_url_aqui'` pelo endereço IP e porta do seu servidor NetBox e `'seu_token_aqui'` pelo seu token de API.
 
 ```python
 import netboxcli as nb
@@ -100,23 +99,21 @@
 ### Exemplo de Virtualização: Excluir uma Máquina Virtual
 
 ```python
 # Exemplo de exclusão de uma máquina virtual pelo ID
 deleted_vm_id = nb_client.virtualization.virtual_machines.delete(id=1)
 
 ```
+para mais exemplos de uso acesse a [documentação](https://netboxcli.readthedocs.io/pt/latest/Getting%20started/)
 
 ### Personalizando e Extendendo
 
 Além das operações básicas, você pode personalizar e estender as funcionalidades do NetboxCli de acordo com suas necessidades específicas. As classes finais oferecem uma base sólida para construir interações mais avançadas com a API do NetBox.
 
 Lembre-se de substituir os exemplos de dados e IDs pelos valores reais correspondentes ao seu ambiente NetBox.
-## 📦 Desenvolvimento
-
-Nesta seção, você encontrará informações sobre o desenvolvimento contínuo do NetboxCli. Estamos trabalhando para expandir as funcionalidades e fornecer suporte abrangente para todas as abas disponíveis no NetBox 3.5 e versões posteriores. Atualizações e novas funcionalidades serão lançadas com o tempo, conforme o projeto evolui.
 
 ### Objetivo
 
 O objetivo do projeto NetboxCli é fornecer uma interface Python simples e eficiente para interagir com o NetBox. 
 oferecendo uma alternativa conveniente para os administradores de rede que desejam automatizar tarefas e gerenciar recursos de infraestrutura de maneira mais fácil.
 
 ## Checklist de Desenvolvimento
@@ -124,39 +121,32 @@
 Aqui está um checklist do que está atualmente disponível no NetboxCli e do que será adicionado no futuro:
 
 - [x]  **Organization:** Gerencie informações sobre organizações e empresas associadas aos seus recursos de rede.
 - [x]  **Devices:** Acesse e gerencie dispositivos de rede, incluindo servidores, roteadores e switches.
 - [x]  **Connections:** Interaja com conexões físicas e lógicas entre dispositivos de rede.
 - [x]  **Wireless:** Gerencie redes sem fio, pontos de acesso e configurações de Wi-Fi.
 - [x]  **IPAM:** Simplifique a gestão de blocos de endereços IP, facilitando a adição, recuperação e atualização.
-- [x]  **Overlay:** Suporte para redes de sobreposição, como VPNs e túneis.
+- [x]  **Vpn:** Suporte para redes de sobreposição, como VPNs e túneis.
 - [x]  **Virtualização:** Gerencie máquinas virtuais de maneira eficaz, desde a criação até a exclusão.
 - [x]  **Circuits:** Gerencie circuitos de rede, como conexões de fibra óptica e links externos.
 - [x]  **Power:** Acesse informações relacionadas ao fornecimento de energia e energia de seus dispositivos.
 - [x]  **Provisioning:** Suporte para provisionamento de rede, incluindo configurações de DHCP e DNS.
 - [x]  **Customization:** Gerencie modelos e configurações personalizadas para seus dispositivos de rede.
 - [x]  **Operations:** Acesse e gerencie informações sobre operações de rede, como manutenção e atualizações.
 - [x]  **Extras:** Integração com plugins e extensões adicionais para funcionalidades personalizadas.
 
 Este checklist será atualizado à medida que novas funcionalidades forem implementadas. 
 Agradecemos por seu interesse e paciência enquanto trabalhamos para tornar o NetboxCli mais abrangente e útil para suas necessidades de automação e gerenciamento de rede.
 
-## 📌 Versão 1.0.0
-
-### **Adições na Versão 1.0.0**
-
-- **Connections:** Adicionado suporte para conexões físicas e lógicas entre dispositivos de rede.
-- **Overlay:** Adicionado suporte para redes de sobreposição, como VPNs e túneis.
-- **Circuits:** Adicionado suporte para circuitos de rede, como conexões de fibra óptica e links externos.
-- **Power:** Adicionado suporte para informações relacionadas ao fornecimento de energia e energia de seus dispositivos.
-- **Provisioning:** Adicionado suporte para provisionamento de rede, incluindo configurações de DHCP e DNS.
-- **Customization:** Adicionado suporte para modelos e configurações personalizadas para seus dispositivos de rede.
-- **Operations:** Adicionado suporte para informações sobre operações de rede, como manutenção e atualizações.
+## 📌 Versão 1.1.5
 
+### **Adições na Versão 1.1.5**
 
+- **Correções de Bugs: ** Correção de bugs menores e melhorias de desempenho em todo o código.
+- **Melhorias de Desempenho: ** Otimização de consultas e operações para melhorar o desempenho geral do NetboxCli.
 
 ## ✒️ Autores
 
 * **developer** - *Initial Work* - [Kaio Guilherme](https://github.com/Kaioguilherme1)
 
 ## 📑 Licença
```

### Comparing `netboxcli-1.0.0/netboxCli/customization/__init__.py` & `netboxcli-1.1.6/netboxcli/customization/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,47 @@
-from netboxCli.core import Core
+from netboxcli.core import Core
 
 from .custom_fields import CustomFields
-from .custom_field_choices import CustomFieldChoices
 from .custom_links import CustomLinks
 from .export_templates import ExportTemplates
-from .saved_filters import SavedFilters
-from .tags import Tags
 from .image_attachments import ImageAttachments
 from .reports import Reports
+from .saved_filters import SavedFilters
 from .scripts import Scripts
+from .tags import Tags
 
 
 class Customization:
-    def __init__(self, netbox):
+    """
+    Customization module
+    """
+
+    def __init__(self, netbox: Core):
+        """
+        Initialize the Customization module.
+
+        Args:
+            netbox: (Core) The Netbox object generated by the Client class.
+        """
         # Customization
-        self.custom_fields = CustomFields(Core(netbox, '/api/extras/custom-fields/'))
-        self.custom_field_choices = CustomFieldChoices(Core(netbox, '/api/extras/custom-field-choices/'))
-        self.custom_links = CustomLinks(Core(netbox, '/api/extras/custom-links/'))
-        self.export_templates = ExportTemplates(Core(netbox, '/api/extras/export-templates/'))
-        self.saved_filters = SavedFilters(Core(netbox, '/api/extras/saved-filters/'))
+        self.custom_fields = CustomFields(
+            Core(netbox, '/api/extras/custom-fields/')
+        )
+        self.custom_links = CustomLinks(
+            Core(netbox, '/api/extras/custom-links/')
+        )
+        self.export_templates = ExportTemplates(
+            Core(netbox, '/api/extras/export-templates/')
+        )
+        self.saved_filters = SavedFilters(
+            Core(netbox, '/api/extras/saved-filters/')
+        )
         self.tags = Tags(Core(netbox, '/api/extras/tags/'))
-        self.image_attachments = ImageAttachments(Core(netbox, '/api/extras/image-attachments/'))
+        self.image_attachments = ImageAttachments(
+            Core(netbox, '/api/extras/image-attachments/')
+        )
         # Reports & Scripts
         self.reports = Reports(Core(netbox, '/api/extras/reports/'))
         self.scripts = Scripts(Core(netbox, '/api/extras/scripts/'))
 
 
 __all__ = ['Customization']
```

### Comparing `netboxcli-1.0.0/netboxCli/devices/__init__.py` & `netboxcli-1.1.6/netboxcli/devices/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,49 +1,72 @@
-from netboxCli.core import Core
+from netboxcli.core import Core
+
+from .console_ports import ConsolePorts
+from .console_server_ports import ConsoleServerPorts
+from .device_types import DeviceTypes
 from .devices import DevicesClass
-from .modules import Modules
 from .devices_roles import DevicesRoles
-from .platforms import Platforms
-from .virtual_chassis import VirtualChassis
-from .virtual_chassis_contexts import VirtualChassisContexts
-from .device_types import DeviceTypes
-from .modules_types import ModulesTypes
-from .manufacturers import Manufacturers
-from .interfaces import Interfaces
 from .front_ports import FrontPorts
-from .rear_ports import RearPorts
-from .console_ports import ConsolePorts
-from .console_server_ports import ConsoleServerPorts
-from .power_ports import PowerPorts
-from .power_outlets import PowerOutlets
-from .modules_bays import ModulesBays
+from .interfaces import Interfaces
 from .inventory_items import InventoryItems
 from .inventory_items_roles import InventoryItemsRoles
+from .manufacturers import Manufacturers
+from .modules import Modules
+from .modules_bays import ModulesBays
+from .modules_types import ModulesTypes
+from .platforms import Platforms
+from .power_outlets import PowerOutlets
+from .power_ports import PowerPorts
+from .rear_ports import RearPorts
+from .virtual_chassis import VirtualChassis
+from .virtual_chassis_contexts import VirtualChassisContexts
 
-class Devices:
 
+class Devices:
     def __init__(self, netbox):
-        #Devices
+        # Devices
         self.devices = DevicesClass(Core(netbox, '/api/dcim/devices/'))
         self.modules = Modules(Core(netbox, '/api/dcim/modules/'))
-        self.devices_roles = DevicesRoles(Core(netbox, '/api/dcim/device-roles/'))
+        self.devices_roles = DevicesRoles(
+            Core(netbox, '/api/dcim/device-roles/')
+        )
         self.platforms = Platforms(Core(netbox, '/api/dcim/platforms/'))
-        self.virtual_chassis = VirtualChassis(Core(netbox, '/api/dcim/virtual-chassis/'))
-        self.virtual_chassis_contexts = VirtualChassisContexts(Core(netbox, '/api/dcim/virtual-chassis-contexts/'))
-        #Devices types
-        self.device_types = DeviceTypes(Core(netbox, '/api/dcim/device-types/'))
-        self.modules_types = ModulesTypes(Core(netbox, '/api/dcim/module-types/'))
-        self.manufacturers = Manufacturers(Core(netbox, '/api/dcim/manufacturers/'))
-        #Devices Components
+        self.virtual_chassis = VirtualChassis(
+            Core(netbox, '/api/dcim/virtual-chassis/')
+        )
+        self.virtual_chassis_contexts = VirtualChassisContexts(
+            Core(netbox, '/api/dcim/virtual-device-contexts/')
+        )
+        # Devices types
+        self.device_types = DeviceTypes(
+            Core(netbox, '/api/dcim/device-types/')
+        )
+        self.modules_types = ModulesTypes(
+            Core(netbox, '/api/dcim/module-types/')
+        )
+        self.manufacturers = Manufacturers(
+            Core(netbox, '/api/dcim/manufacturers/')
+        )
+        # Devices Components
         self.interfaces = Interfaces(Core(netbox, '/api/dcim/interfaces/'))
         self.front_ports = FrontPorts(Core(netbox, '/api/dcim/front-ports/'))
         self.rear_ports = RearPorts(Core(netbox, '/api/dcim/rear-ports/'))
-        self.console_ports = ConsolePorts(Core(netbox, '/api/dcim/console-ports/'))
-        self.console_server_ports = ConsoleServerPorts(Core(netbox, '/api/dcim/console-server-ports/'))
+        self.console_ports = ConsolePorts(
+            Core(netbox, '/api/dcim/console-ports/')
+        )
+        self.console_server_ports = ConsoleServerPorts(
+            Core(netbox, '/api/dcim/console-server-ports/')
+        )
         self.power_ports = PowerPorts(Core(netbox, '/api/dcim/power-ports/'))
-        self.power_outlets = PowerOutlets(Core(netbox, '/api/dcim/power-outlets/'))
+        self.power_outlets = PowerOutlets(
+            Core(netbox, '/api/dcim/power-outlets/')
+        )
         self.modules_bays = ModulesBays(Core(netbox, '/api/dcim/device-bays/'))
-        self.inventory_items = InventoryItems(Core(netbox, '/api/dcim/inventory-items/'))
-        self.inventory_items_roles = InventoryItemsRoles(Core(netbox, '/api/dcim/inventory-items-roles/'))
+        self.inventory_items = InventoryItems(
+            Core(netbox, '/api/dcim/inventory-items/')
+        )
+        self.inventory_items_roles = InventoryItemsRoles(
+            Core(netbox, '/api/dcim/inventory-item-roles/')
+        )
 
-__all__ = ['Devices']
 
+__all__ = ['Devices']
```

### Comparing `netboxcli-1.0.0/netboxCli/ipam/__init__.py` & `netboxcli-1.1.6/netboxcli/ipam/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,51 @@
-from netboxCli.core import Core
+from netboxcli.core import Core
 
+from .aggregates import Aggregates
+from .asn_ranges import AsnRanges
+from .asns import Asns
+from .fhrp_groups import FhrpGroups
 from .ip_addresses import IpAddresses
 from .ip_ranges import IpRanges
-from .prefixes import Prefixes
 from .prefix_roles import PrefixRoles
-from .asn_ranges import AsnRanges
-from .asns import Asns
-from .aggregates import Aggregates
+from .prefixes import Prefixes
 from .rirs import Rirs
-from .vrfs import Vrfs
 from .router_targets import RouterTargets
-from .vlans import Vlans
-from .vlan_groups import VlanGroups
-from .fhrp_groups import FhrpGroups
-from .services_templates import ServicesTemplates
 from .services import Services
+from .services_templates import ServicesTemplates
+from .vlan_groups import VlanGroups
+from .vlans import Vlans
+from .vrfs import Vrfs
+
 
 class Ipam:
     def __init__(self, netbox):
-        self.ip_addresses = IpAddresses(Core(netbox, '/api/ipam/ip-addresses/'))
+        self.ip_addresses = IpAddresses(
+            Core(netbox, '/api/ipam/ip-addresses/')
+        )
         self.ip_ranges = IpRanges(Core(netbox, '/api/ipam/ip-ranges/'))
 
         self.prefixes = Prefixes(Core(netbox, '/api/ipam/prefixes/'))
         self.prefix_roles = PrefixRoles(Core(netbox, '/api/ipam/roles/'))
 
         self.asn_ranges = AsnRanges(Core(netbox, '/api/ipam/asn-ranges/'))
         self.asns = Asns(Core(netbox, '/api/ipam/asns/'))
 
         self.aggregates = Aggregates(Core(netbox, '/api/ipam/aggregates/'))
         self.rirs = Rirs(Core(netbox, '/api/ipam/rirs/'))
 
         self.vrfs = Vrfs(Core(netbox, '/api/ipam/vrfs/'))
-        self.router_targets = RouterTargets(Core(netbox, '/api/ipam/router-targets/'))
+        self.router_targets = RouterTargets(
+            Core(netbox, '/api/ipam/route-targets/')
+        )
 
         self.vlans = Vlans(Core(netbox, '/api/ipam/vlans/'))
         self.vlan_groups = VlanGroups(Core(netbox, '/api/ipam/vlan-groups/'))
 
         self.fhrp_groups = FhrpGroups(Core(netbox, '/api/ipam/fhrp-groups/'))
-        self.services_templates = ServicesTemplates(Core(netbox, '/api/ipam/services-templates/'))
+        self.services_templates = ServicesTemplates(
+            Core(netbox, '/api/ipam/service-templates/')
+        )
         self.services = Services(Core(netbox, '/api/ipam/services/'))
 
 
 __all__ = ['Ipam']
-
-
```

### Comparing `netboxcli-1.0.0/netboxCli/virtualization/__init__.py` & `netboxcli-1.1.6/netboxcli/virtualization/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from netboxCli.core import Core
+from netboxcli.core import Core
 
-from .virtual_machines import VirtualMachines
-from .interfaces import Interfaces
-from .clusters import Clusters
-from .cluster_types import ClusterTypes
 from .cluster_groups import ClusterGroups
-
+from .cluster_types import ClusterTypes
+from .clusters import Clusters
+from .interfaces import Interfaces
+from .virtual_machines import VirtualMachines
 
 
 class Virtualization:
     """
     Class for managing virtualization-related resources.
 
     Args:
@@ -18,22 +17,31 @@
     Attributes:
         vms (Vms): Instance of the Vms class for managing virtual machines.
         interfaces (Interfaces): Instance of the Interfaces class for managing interfaces.
         clusters (Clusters): Instance of the Clusters class for managing clusters.
         cluster_types (ClusterTypes): Instance of the ClusterTypes class for managing cluster types.
         cluster_groups (ClusterGroups): Instance of the ClusterGroups class for managing cluster groups.
     """
+
     def __init__(self, netbox):
         """
         Initialize Virtualization class with Netbox API instance.
 
         Args:
             netbox (obj): Netbox API instance.
         """
-        self.virtual_machines = VirtualMachines(Core(netbox, '/api/virtualization/virtual-machines/'))
-        self.interfaces = Interfaces(Core(netbox, '/api/virtualization/interfaces/'))
+        self.virtual_machines = VirtualMachines(
+            Core(netbox, '/api/virtualization/virtual-machines/')
+        )
+        self.interfaces = Interfaces(
+            Core(netbox, '/api/virtualization/interfaces/')
+        )
         self.clusters = Clusters(Core(netbox, '/api/virtualization/clusters/'))
-        self.cluster_types = ClusterTypes(Core(netbox, '/api/virtualization/cluster-types/'))
-        self.cluster_groups = ClusterGroups(Core(netbox, '/api/virtualization/cluster-groups/'))
+        self.cluster_types = ClusterTypes(
+            Core(netbox, '/api/virtualization/cluster-types/')
+        )
+        self.cluster_groups = ClusterGroups(
+            Core(netbox, '/api/virtualization/cluster-groups/')
+        )
 
 
 __all__ = ['Virtualization']
```

