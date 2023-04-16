# Comparing `tmp/ediri_vultr-2.13.0.tar.gz` & `tmp/ediri_vultr-2.14.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ediri_vultr-2.13.0.tar", last modified: Tue Apr  4 20:54:47 2023, max compression
+gzip compressed data, was "ediri_vultr-2.14.0.tar", last modified: Sun Apr 16 11:30:48 2023, max compression
```

## Comparing `ediri_vultr-2.13.0.tar` & `ediri_vultr-2.14.0.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:54:47.105820 ediri_vultr-2.13.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-04-04 20:54:47.105820 ediri_vultr-2.13.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:54:47.101820 ediri_vultr-2.13.0/ediri_vultr/
--rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48976 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    56372 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/bare_metal_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    22078 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/block_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:54:47.105820 ediri_vultr-2.13.0/ediri_vultr/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    11631 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/dns_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)    15367 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/dns_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    12540 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/firewall_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    21767 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/firewall_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/get_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/get_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/get_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     7964 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/get_bare_metal_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    12578 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/get_bare_metal_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     7965 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/get_block_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/get_dns_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/get_firewall_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    18081 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/get_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/get_instance_ipv4.py
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/get_iso_private.py
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/get_iso_public.py
--rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/get_kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12356 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/get_load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/get_object_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/get_object_storage_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/get_os.py
--rw-r--r--   0 runner    (1001) docker     (123)     7665 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/get_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/get_private_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/get_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/get_reserved_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/get_reverse_ipv4.py
--rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/get_reverse_ipv6.py
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/get_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/get_ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/get_startup_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/get_vpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    81215 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    12872 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/instance_ipv4.py
--rw-r--r--   0 runner    (1001) docker     (123)     9029 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/iso_private.py
--rw-r--r--   0 runner    (1001) docker     (123)    22605 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)    25686 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/kubernetes_node_pools.py
--rw-r--r--   0 runner    (1001) docker     (123)    41761 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (123)    16291 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/object_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    47909 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15077 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/private_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15244 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/reserved_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)    12813 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/reverse_ipv4.py
--rw-r--r--   0 runner    (1001) docker     (123)     9869 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/reverse_ipv6.py
--rw-r--r--   0 runner    (1001) docker     (123)    14099 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/snapshot_from_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    12267 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/startup_script.py
--rw-r--r--   0 runner    (1001) docker     (123)    15601 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    14407 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/ediri_vultr/vpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:54:47.105820 ediri_vultr-2.13.0/ediri_vultr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-04-04 20:54:47.000000 ediri_vultr-2.13.0/ediri_vultr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-04-04 20:54:47.000000 ediri_vultr-2.13.0/ediri_vultr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 20:54:47.000000 ediri_vultr-2.13.0/ediri_vultr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 20:54:47.000000 ediri_vultr-2.13.0/ediri_vultr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-04 20:54:47.000000 ediri_vultr-2.13.0/ediri_vultr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-04 20:54:47.000000 ediri_vultr-2.13.0/ediri_vultr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 20:54:47.105820 ediri_vultr-2.13.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-04 20:54:46.000000 ediri_vultr-2.13.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:30:48.665268 ediri_vultr-2.14.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-04-16 11:30:48.665268 ediri_vultr-2.14.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:30:48.661267 ediri_vultr-2.14.0/ediri_vultr/
+-rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48976 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56372 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/bare_metal_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22078 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/block_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:30:48.665268 ediri_vultr-2.14.0/ediri_vultr/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11631 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/dns_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15367 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/dns_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12540 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/firewall_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21767 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/firewall_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7964 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_bare_metal_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12578 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_bare_metal_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7965 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_block_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_dns_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_firewall_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18081 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_instance_ipv4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_iso_private.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_iso_public.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12356 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_object_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_object_storage_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_os.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7665 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_private_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_reserved_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_reverse_ipv4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_reverse_ipv6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_startup_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/get_vpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81215 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12872 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/instance_ipv4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9029 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/iso_private.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22755 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25686 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/kubernetes_node_pools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41761 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16291 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/object_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47909 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15077 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/private_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    15244 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/reserved_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12813 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/reverse_ipv4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9869 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/reverse_ipv6.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14099 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/snapshot_from_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12267 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/startup_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15601 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14407 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr/vpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:30:48.661267 ediri_vultr-2.14.0/ediri_vultr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/ediri_vultr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 11:30:48.665268 ediri_vultr-2.14.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-16 11:30:48.000000 ediri_vultr-2.14.0/setup.py
```

### Comparing `ediri_vultr-2.13.0/PKG-INFO` & `ediri_vultr-2.14.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ediri_vultr
-Version: 2.13.0
+Version: 2.14.0
 Summary: A Pulumi package for creating and managing Vultr cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/dirien/pulumi-vultr
 Keywords: pulumi vultr category/utility
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `ediri_vultr-2.13.0/README.md` & `ediri_vultr-2.14.0/README.md`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/__init__.py` & `ediri_vultr-2.14.0/ediri_vultr/__init__.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/_inputs.py` & `ediri_vultr-2.14.0/ediri_vultr/_inputs.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/_utilities.py` & `ediri_vultr-2.14.0/ediri_vultr/_utilities.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/bare_metal_server.py` & `ediri_vultr-2.14.0/ediri_vultr/bare_metal_server.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/block_storage.py` & `ediri_vultr-2.14.0/ediri_vultr/block_storage.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/config/vars.py` & `ediri_vultr-2.14.0/ediri_vultr/config/vars.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/dns_domain.py` & `ediri_vultr-2.14.0/ediri_vultr/dns_domain.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/dns_record.py` & `ediri_vultr-2.14.0/ediri_vultr/dns_record.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/firewall_group.py` & `ediri_vultr-2.14.0/ediri_vultr/firewall_group.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/firewall_rule.py` & `ediri_vultr-2.14.0/ediri_vultr/firewall_rule.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/get_account.py` & `ediri_vultr-2.14.0/ediri_vultr/get_account.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/get_application.py` & `ediri_vultr-2.14.0/ediri_vultr/get_application.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/get_backup.py` & `ediri_vultr-2.14.0/ediri_vultr/get_backup.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/get_bare_metal_plan.py` & `ediri_vultr-2.14.0/ediri_vultr/get_bare_metal_plan.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/get_bare_metal_server.py` & `ediri_vultr-2.14.0/ediri_vultr/get_bare_metal_server.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/get_block_storage.py` & `ediri_vultr-2.14.0/ediri_vultr/get_block_storage.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/get_dns_domain.py` & `ediri_vultr-2.14.0/ediri_vultr/get_dns_domain.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/get_firewall_group.py` & `ediri_vultr-2.14.0/ediri_vultr/get_firewall_group.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/get_instance.py` & `ediri_vultr-2.14.0/ediri_vultr/get_instance.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/get_instance_ipv4.py` & `ediri_vultr-2.14.0/ediri_vultr/get_instance_ipv4.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/get_iso_private.py` & `ediri_vultr-2.14.0/ediri_vultr/get_iso_private.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/get_iso_public.py` & `ediri_vultr-2.14.0/ediri_vultr/get_iso_public.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/get_kubernetes.py` & `ediri_vultr-2.14.0/ediri_vultr/get_kubernetes.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/get_load_balancer.py` & `ediri_vultr-2.14.0/ediri_vultr/get_load_balancer.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/get_object_storage.py` & `ediri_vultr-2.14.0/ediri_vultr/get_object_storage.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/get_object_storage_cluster.py` & `ediri_vultr-2.14.0/ediri_vultr/get_object_storage_cluster.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/get_os.py` & `ediri_vultr-2.14.0/ediri_vultr/get_os.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/get_plan.py` & `ediri_vultr-2.14.0/ediri_vultr/get_plan.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/get_private_network.py` & `ediri_vultr-2.14.0/ediri_vultr/get_private_network.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/get_region.py` & `ediri_vultr-2.14.0/ediri_vultr/get_region.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/get_reserved_ip.py` & `ediri_vultr-2.14.0/ediri_vultr/get_reserved_ip.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/get_reverse_ipv4.py` & `ediri_vultr-2.14.0/ediri_vultr/get_reverse_ipv4.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/get_reverse_ipv6.py` & `ediri_vultr-2.14.0/ediri_vultr/get_reverse_ipv6.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/get_snapshot.py` & `ediri_vultr-2.14.0/ediri_vultr/get_snapshot.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/get_ssh_key.py` & `ediri_vultr-2.14.0/ediri_vultr/get_ssh_key.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/get_startup_script.py` & `ediri_vultr-2.14.0/ediri_vultr/get_startup_script.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/get_user.py` & `ediri_vultr-2.14.0/ediri_vultr/get_user.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/get_vpc.py` & `ediri_vultr-2.14.0/ediri_vultr/get_vpc.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/instance.py` & `ediri_vultr-2.14.0/ediri_vultr/instance.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/instance_ipv4.py` & `ediri_vultr-2.14.0/ediri_vultr/instance_ipv4.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/iso_private.py` & `ediri_vultr-2.14.0/ediri_vultr/iso_private.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/kubernetes.py` & `ediri_vultr-2.14.0/ediri_vultr/kubernetes.py`

 * *Files 1% similar despite different names*

```diff
@@ -424,14 +424,16 @@
             __props__.__dict__["cluster_subnet"] = None
             __props__.__dict__["date_created"] = None
             __props__.__dict__["endpoint"] = None
             __props__.__dict__["ip"] = None
             __props__.__dict__["kube_config"] = None
             __props__.__dict__["service_subnet"] = None
             __props__.__dict__["status"] = None
+        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["kubeConfig"])
+        opts = pulumi.ResourceOptions.merge(opts, secret_opts)
         super(Kubernetes, __self__).__init__(
             'vultr:index/kubernetes:Kubernetes',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
```

### Comparing `ediri_vultr-2.13.0/ediri_vultr/kubernetes_node_pools.py` & `ediri_vultr-2.14.0/ediri_vultr/kubernetes_node_pools.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/load_balancer.py` & `ediri_vultr-2.14.0/ediri_vultr/load_balancer.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/object_storage.py` & `ediri_vultr-2.14.0/ediri_vultr/object_storage.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/outputs.py` & `ediri_vultr-2.14.0/ediri_vultr/outputs.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/private_network.py` & `ediri_vultr-2.14.0/ediri_vultr/private_network.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/provider.py` & `ediri_vultr-2.14.0/ediri_vultr/provider.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/reserved_ip.py` & `ediri_vultr-2.14.0/ediri_vultr/reserved_ip.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/reverse_ipv4.py` & `ediri_vultr-2.14.0/ediri_vultr/reverse_ipv4.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/reverse_ipv6.py` & `ediri_vultr-2.14.0/ediri_vultr/reverse_ipv6.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/snapshot.py` & `ediri_vultr-2.14.0/ediri_vultr/snapshot.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/snapshot_from_url.py` & `ediri_vultr-2.14.0/ediri_vultr/snapshot_from_url.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/ssh_key.py` & `ediri_vultr-2.14.0/ediri_vultr/ssh_key.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/startup_script.py` & `ediri_vultr-2.14.0/ediri_vultr/startup_script.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/user.py` & `ediri_vultr-2.14.0/ediri_vultr/user.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr/vpc.py` & `ediri_vultr-2.14.0/ediri_vultr/vpc.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/ediri_vultr.egg-info/PKG-INFO` & `ediri_vultr-2.14.0/ediri_vultr.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ediri-vultr
-Version: 2.13.0
+Version: 2.14.0
 Summary: A Pulumi package for creating and managing Vultr cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/dirien/pulumi-vultr
 Keywords: pulumi vultr category/utility
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `ediri_vultr-2.13.0/ediri_vultr.egg-info/SOURCES.txt` & `ediri_vultr-2.14.0/ediri_vultr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.13.0/setup.py` & `ediri_vultr-2.14.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "2.13.0"
-PLUGIN_VERSION = "2.13.0"
+VERSION = "2.14.0"
+PLUGIN_VERSION = "2.14.0"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'vultr', PLUGIN_VERSION, '--server', 'github://api.github.com/dirien/pulumi-vultr'])
         except OSError as error:
```

