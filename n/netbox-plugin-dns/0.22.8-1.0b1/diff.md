# Comparing `tmp/netbox_plugin_dns-0.22.8.tar.gz` & `tmp/netbox_plugin_dns-1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_plugin_dns-0.22.8.tar", max compression
+gzip compressed data, was "netbox_plugin_dns-1.0b1.tar", max compression
```

## Comparing `netbox_plugin_dns-0.22.8.tar` & `netbox_plugin_dns-1.0b1.tar`

### file list

```diff
@@ -1,117 +1,103 @@
--rw-r--r--   0        0        0     1076 2024-04-01 17:13:14.517036 netbox_plugin_dns-0.22.8/LICENSE
--rw-r--r--   0        0        0     3696 2024-04-01 17:13:14.517036 netbox_plugin_dns-0.22.8/README.md
--rw-r--r--   0        0        0     1314 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/__init__.py
--rw-r--r--   0        0        0     3291 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/api/nested_serializers.py
--rw-r--r--   0        0        0     8203 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/api/serializers.py
--rw-r--r--   0        0        0      575 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/api/urls.py
--rw-r--r--   0        0        0     3527 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/api/views.py
--rw-r--r--   0        0        0      151 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/apps.py
--rw-r--r--   0        0        0       69 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/fields/__init__.py
--rw-r--r--   0        0        0     1494 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/fields/address.py
--rw-r--r--   0        0        0     3592 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/fields/network.py
--rw-r--r--   0        0        0     2521 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/fields/rfc2317.py
--rw-r--r--   0        0        0      136 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/filters/__init__.py
--rw-r--r--   0        0        0     1027 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/filters/contact.py
--rwxr-xr-x   0        0        0      522 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/filters/nameserver.py
--rwxr-xr-x   0        0        0     2256 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/filters/record.py
--rw-r--r--   0        0        0      911 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/filters/registrar.py
--rw-r--r--   0        0        0      497 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/filters/view.py
--rwxr-xr-x   0        0        0     3564 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/filters/zone.py
--rw-r--r--   0        0        0      136 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/forms/__init__.py
--rw-r--r--   0        0        0     4492 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/forms/contact.py
--rwxr-xr-x   0        0        0     2027 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/forms/nameserver.py
--rwxr-xr-x   0        0        0     6266 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/forms/record.py
--rw-r--r--   0        0        0     2832 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/forms/registrar.py
--rw-r--r--   0        0        0     1627 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/forms/view.py
--rwxr-xr-x   0        0        0    21740 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/forms/zone.py
--rw-r--r--   0        0        0      811 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/graphql/__init__.py
--rw-r--r--   0        0        0      497 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/graphql/contact.py
--rw-r--r--   0        0        0      527 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/graphql/nameserver.py
--rw-r--r--   0        0        0      487 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/graphql/record.py
--rw-r--r--   0        0        0      517 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/graphql/registrar.py
--rw-r--r--   0        0        0      221 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/graphql/schema.py
--rw-r--r--   0        0        0      467 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/graphql/view.py
--rw-r--r--   0        0        0      467 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/graphql/zone.py
--rw-r--r--   0        0        0     6050 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/management/commands/cleanup_database.py
--rw-r--r--   0        0        0     2077 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/management/commands/cleanup_rrset_ttl.py
--rw-r--r--   0        0        0     4580 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/management/commands/setup_coupling.py
--rw-r--r--   0        0        0      661 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/management/commands/update_soa.py
--rw-r--r--   0        0        0     4153 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0001_initial.py
--rw-r--r--   0        0        0    11466 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0001_squashed_netbox_dns_0_15.py
--rw-r--r--   0        0        0      437 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0002_zone_default_ttl.py
--rw-r--r--   0        0        0     3716 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0003_soa_managed_records.py
--rw-r--r--   0        0        0     2287 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0004_create_ptr_for_a_aaaa_records.py
--rw-r--r--   0        0        0     1156 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0005_update_ns_records.py
--rw-r--r--   0        0        0      861 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0006_zone_soa_serial_auto.py
--rw-r--r--   0        0        0      399 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0007_alter_zone_soa_serial_auto.py
--rw-r--r--   0        0        0      527 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0008_zone_status_names.py
--rw-r--r--   0        0        0     2176 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0009_netbox32.py
--rw-r--r--   0        0        0     1543 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0010_update_soa_records.py
--rw-r--r--   0        0        0     2201 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0011_add_view_model.py
--rw-r--r--   0        0        0      402 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0012_adjust_zone_and_record.py
--rw-r--r--   0        0        0      733 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0013_add_nameserver_zone_record_description.py
--rw-r--r--   0        0        0      428 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0014_add_view_description.py
--rw-r--r--   0        0        0      393 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0015_add_record_status.py
--rw-r--r--   0        0        0     1053 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0016_cleanup_ptr_records.py
--rw-r--r--   0        0        0      405 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0017_alter_record_ttl.py
--rw-r--r--   0        0        0     1553 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0018_zone_arpa_network.py
--rw-r--r--   0        0        0      433 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0019_update_ns_ttl.py
--rw-r--r--   0        0        0     1260 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0020_netbox_3_4.py
--rw-r--r--   0        0        0     3243 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0021_record_ip_address.py
--rw-r--r--   0        0        0      172 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0022_search.py
--rw-r--r--   0        0        0      378 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0023_alter_record_value.py
--rw-r--r--   0        0        0     1745 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0024_tenancy.py
--rw-r--r--   0        0        0      620 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0025_ipam_coupling_cf.py
--rw-r--r--   0        0        0     5796 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0026_domain_registration.py
--rw-r--r--   0        0        0      404 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0027_alter_registrar_iana_id.py
--rw-r--r--   0        0        0     1364 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0028_rfc2317_fields.py
--rw-r--r--   0        0        0      808 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/0029_record_fqdn.py
--rw-r--r--   0        0        0        0 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/migrations/__init__.py
--rw-r--r--   0        0        0      182 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/models/__init__.py
--rw-r--r--   0        0        0     2849 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/models/contact.py
--rw-r--r--   0        0        0     2941 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/models/nameserver.py
--rw-r--r--   0        0        0    23917 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/models/record.py
--rw-r--r--   0        0        0     1416 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/models/registrar.py
--rw-r--r--   0        0        0      920 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/models/view.py
--rw-r--r--   0        0        0    26637 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/models/zone.py
--rw-r--r--   0        0        0     4587 2024-04-01 17:13:14.553036 netbox_plugin_dns-0.22.8/netbox_dns/navigation.py
--rw-r--r--   0        0        0        0 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/signals/__init__.py
--rw-r--r--   0        0        0     5727 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/signals/ipam_coupling.py
--rw-r--r--   0        0        0      136 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/tables/__init__.py
--rw-r--r--   0        0        0      747 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/tables/contact.py
--rw-r--r--   0        0        0      819 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/tables/nameserver.py
--rw-r--r--   0        0        0     3162 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/tables/record.py
--rw-r--r--   0        0        0      621 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/tables/registrar.py
--rw-r--r--   0        0        0      501 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/tables/view.py
--rw-r--r--   0        0        0     1886 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/tables/zone.py
--rw-r--r--   0        0        0     3936 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/template_content.py
--rw-r--r--   0        0        0     2858 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/contact.html
--rw-r--r--   0        0        0     1623 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/nameserver.html
--rw-r--r--   0        0        0       89 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/record/managed.html
--rw-r--r--   0        0        0      742 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/record/related.html
--rw-r--r--   0        0        0     5835 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/record.html
--rw-r--r--   0        0        0     2130 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/registrar.html
--rw-r--r--   0        0        0      806 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/related_dns_objects.html
--rw-r--r--   0        0        0     1350 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/view.html
--rw-r--r--   0        0        0      460 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/zone/base.html
--rw-r--r--   0        0        0     2171 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/zone/child.html
--rw-r--r--   0        0        0      524 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/zone/managed_record.html
--rw-r--r--   0        0        0     2218 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/zone/record.html
--rw-r--r--   0        0        0     1283 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/zone/registration.html
--rw-r--r--   0        0        0      527 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/zone/rfc2317_child_zone.html
--rw-r--r--   0        0        0     7187 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/zone.html
--rw-r--r--   0        0        0     9172 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/urls.py
--rw-r--r--   0        0        0     1967 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/utilities/__init__.py
--rw-r--r--   0        0        0     3573 2024-04-01 17:13:14.557036 netbox_plugin_dns-0.22.8/netbox_dns/utilities/ipam_coupling.py
--rw-r--r--   0        0        0       47 2024-04-01 17:13:14.561036 netbox_plugin_dns-0.22.8/netbox_dns/validators/__init__.py
--rw-r--r--   0        0        0     2232 2024-04-01 17:13:14.561036 netbox_plugin_dns-0.22.8/netbox_dns/validators/dns_name.py
--rw-r--r--   0        0        0      503 2024-04-01 17:13:14.561036 netbox_plugin_dns-0.22.8/netbox_dns/validators/rfc2317.py
--rw-r--r--   0        0        0      136 2024-04-01 17:13:14.561036 netbox_plugin_dns-0.22.8/netbox_dns/views/__init__.py
--rw-r--r--   0        0        0     2235 2024-04-01 17:13:14.561036 netbox_plugin_dns-0.22.8/netbox_dns/views/contact.py
--rw-r--r--   0        0        0     2990 2024-04-01 17:13:14.561036 netbox_plugin_dns-0.22.8/netbox_dns/views/nameserver.py
--rw-r--r--   0        0        0     4904 2024-04-01 17:13:14.561036 netbox_plugin_dns-0.22.8/netbox_dns/views/record.py
--rw-r--r--   0        0        0     2072 2024-04-01 17:13:14.561036 netbox_plugin_dns-0.22.8/netbox_dns/views/registrar.py
--rw-r--r--   0        0        0     1895 2024-04-01 17:13:14.561036 netbox_plugin_dns-0.22.8/netbox_dns/views/view.py
--rw-r--r--   0        0        0     4587 2024-04-01 17:13:14.561036 netbox_plugin_dns-0.22.8/netbox_dns/views/zone.py
--rw-r--r--   0        0        0      741 2024-04-01 17:13:14.561036 netbox_plugin_dns-0.22.8/pyproject.toml
--rw-r--r--   0        0        0     4572 1970-01-01 00:00:00.000000 netbox_plugin_dns-0.22.8/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-04-03 13:17:52.207418 netbox_plugin_dns-1.0b1/LICENSE
+-rw-r--r--   0        0        0     3697 2024-04-03 13:17:52.207418 netbox_plugin_dns-1.0b1/README.md
+-rw-r--r--   0        0        0     1053 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/__init__.py
+-rw-r--r--   0        0        0     2145 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/api/nested_serializers.py
+-rw-r--r--   0        0        0      249 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/api/serializers.py
+-rw-r--r--   0        0        0        0 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/api/serializers_/__init__.py
+-rw-r--r--   0        0        0      929 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/api/serializers_/contact.py
+-rw-r--r--   0        0        0     1093 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/api/serializers_/nameserver.py
+-rw-r--r--   0        0        0     2284 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/api/serializers_/record.py
+-rw-r--r--   0        0        0      805 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/api/serializers_/registrar.py
+-rw-r--r--   0        0        0      798 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/api/serializers_/view.py
+-rw-r--r--   0        0        0     4759 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/api/serializers_/zone.py
+-rw-r--r--   0        0        0      575 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/api/urls.py
+-rw-r--r--   0        0        0     3566 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/api/views.py
+-rw-r--r--   0        0        0      151 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/apps.py
+-rw-r--r--   0        0        0       69 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/fields/__init__.py
+-rw-r--r--   0        0        0     1494 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/fields/address.py
+-rw-r--r--   0        0        0     3606 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/fields/network.py
+-rw-r--r--   0        0        0     2518 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/fields/rfc2317.py
+-rw-r--r--   0        0        0      136 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/filtersets/__init__.py
+-rw-r--r--   0        0        0     1057 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/filtersets/contact.py
+-rwxr-xr-x   0        0        0     1110 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/filtersets/nameserver.py
+-rwxr-xr-x   0        0        0     3687 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/filtersets/record.py
+-rw-r--r--   0        0        0      941 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/filtersets/registrar.py
+-rw-r--r--   0        0        0      505 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/filtersets/view.py
+-rwxr-xr-x   0        0        0     6564 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/filtersets/zone.py
+-rw-r--r--   0        0        0      136 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/forms/__init__.py
+-rw-r--r--   0        0        0     5220 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/forms/contact.py
+-rwxr-xr-x   0        0        0     2361 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/forms/nameserver.py
+-rwxr-xr-x   0        0        0     6272 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/forms/record.py
+-rw-r--r--   0        0        0     3638 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/forms/registrar.py
+-rw-r--r--   0        0        0     1932 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/forms/view.py
+-rwxr-xr-x   0        0        0    22627 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/forms/zone.py
+-rw-r--r--   0        0        0      358 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/graphql/__init__.py
+-rw-r--r--   0        0        0     1257 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/graphql/filters.py
+-rw-r--r--   0        0        0     1915 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/graphql/schema.py
+-rw-r--r--   0        0        0     4207 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/graphql/types.py
+-rw-r--r--   0        0        0     5960 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/management/commands/cleanup_database.py
+-rw-r--r--   0        0        0     2029 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/management/commands/cleanup_rrset_ttl.py
+-rw-r--r--   0        0        0     4556 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/management/commands/setup_coupling.py
+-rw-r--r--   0        0        0      660 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/management/commands/update_soa.py
+-rw-r--r--   0        0        0    10283 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/migrations/0001_squashed_netbox_dns_0_15.py
+-rw-r--r--   0        0        0    20243 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/migrations/0001_squashed_netbox_dns_0_22.py
+-rw-r--r--   0        0        0      583 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/migrations/0002_contact_description_registrar_description.py
+-rw-r--r--   0        0        0     1271 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/migrations/0020_netbox_3_4.py
+-rw-r--r--   0        0        0     3243 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/migrations/0021_record_ip_address.py
+-rw-r--r--   0        0        0      172 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/migrations/0022_search.py
+-rw-r--r--   0        0        0      378 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/migrations/0023_alter_record_value.py
+-rw-r--r--   0        0        0     1745 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/migrations/0024_tenancy.py
+-rw-r--r--   0        0        0      620 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/migrations/0025_ipam_coupling_cf.py
+-rw-r--r--   0        0        0     5796 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/migrations/0026_domain_registration.py
+-rw-r--r--   0        0        0      404 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/migrations/0027_alter_registrar_iana_id.py
+-rw-r--r--   0        0        0     1364 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/migrations/0028_rfc2317_fields.py
+-rw-r--r--   0        0        0      808 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/migrations/0029_record_fqdn.py
+-rw-r--r--   0        0        0        0 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/migrations/__init__.py
+-rw-r--r--   0        0        0      182 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/models/__init__.py
+-rw-r--r--   0        0        0     2958 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/models/contact.py
+-rw-r--r--   0        0        0     3021 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/models/nameserver.py
+-rw-r--r--   0        0        0    23740 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/models/record.py
+-rw-r--r--   0        0        0     1502 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/models/registrar.py
+-rw-r--r--   0        0        0      920 2024-04-03 13:17:52.239418 netbox_plugin_dns-1.0b1/netbox_dns/models/view.py
+-rw-r--r--   0        0        0    26519 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/models/zone.py
+-rw-r--r--   0        0        0     4062 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/navigation.py
+-rw-r--r--   0        0        0        0 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/signals/__init__.py
+-rw-r--r--   0        0        0     5595 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/signals/ipam_coupling.py
+-rw-r--r--   0        0        0      136 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/tables/__init__.py
+-rw-r--r--   0        0        0      774 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/tables/contact.py
+-rw-r--r--   0        0        0      767 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/tables/nameserver.py
+-rw-r--r--   0        0        0     3162 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/tables/record.py
+-rw-r--r--   0        0        0      648 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/tables/registrar.py
+-rw-r--r--   0        0        0      501 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/tables/view.py
+-rw-r--r--   0        0        0     1886 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/tables/zone.py
+-rw-r--r--   0        0        0     3805 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/template_content.py
+-rw-r--r--   0        0        0     2855 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/contact.html
+-rw-r--r--   0        0        0     1554 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/nameserver.html
+-rw-r--r--   0        0        0       89 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/record/managed.html
+-rw-r--r--   0        0        0      742 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/record/related.html
+-rw-r--r--   0        0        0     5481 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/record.html
+-rw-r--r--   0        0        0     2152 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/registrar.html
+-rw-r--r--   0        0        0      806 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/related_dns_objects.html
+-rw-r--r--   0        0        0     1321 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/view.html
+-rw-r--r--   0        0        0      495 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/zone/base.html
+-rw-r--r--   0        0        0     2147 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/zone/child.html
+-rw-r--r--   0        0        0      514 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/zone/managed_record.html
+-rw-r--r--   0        0        0     2194 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/zone/record.html
+-rw-r--r--   0        0        0     1151 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/zone/registration.html
+-rw-r--r--   0        0        0      517 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/zone/rfc2317_child_zone.html
+-rw-r--r--   0        0        0     6717 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/zone.html
+-rw-r--r--   0        0        0     9172 2024-04-03 13:17:52.243418 netbox_plugin_dns-1.0b1/netbox_dns/urls.py
+-rw-r--r--   0        0        0     1835 2024-04-03 13:17:52.247418 netbox_plugin_dns-1.0b1/netbox_dns/utilities/__init__.py
+-rw-r--r--   0        0        0     3441 2024-04-03 13:17:52.247418 netbox_plugin_dns-1.0b1/netbox_dns/utilities/ipam_coupling.py
+-rw-r--r--   0        0        0       47 2024-04-03 13:17:52.247418 netbox_plugin_dns-1.0b1/netbox_dns/validators/__init__.py
+-rw-r--r--   0        0        0     2097 2024-04-03 13:17:52.247418 netbox_plugin_dns-1.0b1/netbox_dns/validators/dns_name.py
+-rw-r--r--   0        0        0      501 2024-04-03 13:17:52.247418 netbox_plugin_dns-1.0b1/netbox_dns/validators/rfc2317.py
+-rw-r--r--   0        0        0      136 2024-04-03 13:17:52.247418 netbox_plugin_dns-1.0b1/netbox_dns/views/__init__.py
+-rw-r--r--   0        0        0     2253 2024-04-03 13:17:52.247418 netbox_plugin_dns-1.0b1/netbox_dns/views/contact.py
+-rw-r--r--   0        0        0     3011 2024-04-03 13:17:52.247418 netbox_plugin_dns-1.0b1/netbox_dns/views/nameserver.py
+-rw-r--r--   0        0        0     4928 2024-04-03 13:17:52.247418 netbox_plugin_dns-1.0b1/netbox_dns/views/record.py
+-rw-r--r--   0        0        0     2090 2024-04-03 13:17:52.247418 netbox_plugin_dns-1.0b1/netbox_dns/views/registrar.py
+-rw-r--r--   0        0        0     1913 2024-04-03 13:17:52.247418 netbox_plugin_dns-1.0b1/netbox_dns/views/view.py
+-rw-r--r--   0        0        0     4591 2024-04-03 13:17:52.247418 netbox_plugin_dns-1.0b1/netbox_dns/views/zone.py
+-rw-r--r--   0        0        0      732 2024-04-03 13:17:52.247418 netbox_plugin_dns-1.0b1/pyproject.toml
+-rw-r--r--   0        0        0     4460 1970-01-01 00:00:00.000000 netbox_plugin_dns-1.0b1/PKG-INFO
```

### Comparing `netbox_plugin_dns-0.22.8/LICENSE` & `netbox_plugin_dns-1.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.8/README.md` & `netbox_plugin_dns-1.0b1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 * Manage domain registrar and registrant information for domains related to zones
 * Manage RFC2317 reverse zones for IPv4 prefixes with a network mask length longer than 24 bits
 
 NetBox DNS is using the standardized NetBox plugin interface, so it also takes advantage of the NetBox tagging and change log features.
 
 ## Requirements
 
-* NetBox 3.5.0 or higher
-* Python 3.8 or higher
+* NetBox 4.0.0 or higher
+* Python 3.10 or higher
 
 ## Installation & Configuration
 
 ### Installation
 
 ```
 $ source /opt/netbox/venv/bin/activate
```

#### html2text {}

```diff
@@ -9,16 +9,16 @@
 ## Features * Manage name servers, zones and records * Automatically generate
 SOA and NS records for zones * Automatically create and update PTR records for
 IPv4 and IPv6 address records * Organize DNS zones in views for split horizon
 DNS and multi-site deployments * Manage domain registrar and registrant
 information for domains related to zones * Manage RFC2317 reverse zones for
 IPv4 prefixes with a network mask length longer than 24 bits NetBox DNS is
 using the standardized NetBox plugin interface, so it also takes advantage of
-the NetBox tagging and change log features. ## Requirements * NetBox 3.5.0 or
-higher * Python 3.8 or higher ## Installation & Configuration ### Installation
+the NetBox tagging and change log features. ## Requirements * NetBox 4.0.0 or
+higher * Python 3.10 or higher ## Installation & Configuration ### Installation
 ``` $ source /opt/netbox/venv/bin/activate (venv) $ pip install netbox-plugin-
 dns ``` ### NetBox Configuration Add the plugin to the NetBox config. `~/
 netbox/configuration.py` ```python PLUGINS = [ "netbox_dns", ] ``` To
 permanently keep the plugin installed when updating NetBox via `update.sh`: ```
 echo netbox-plugin-dns >> ~/netbox/local_requirements.txt ``` To add the
 required netbox_dns tables to your database run the following command from your
 NetBox directory: ``` ./manage.py migrate ``` Full documentation on using
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/api/nested_serializers.py` & `netbox_plugin_dns-1.0b1/netbox_dns/api/nested_serializers.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,15 @@
 from rest_framework import serializers
 
 from netbox.api.serializers import WritableNestedSerializer
 
-from netbox_dns.models import View, Zone, NameServer, Record, Registrar, Contact
+from netbox_dns.models import Zone, Record
+from netbox_dns.api.serializers_.view import ViewSerializer
 
 
-#
-# Views
-#
-class NestedViewSerializer(WritableNestedSerializer):
-    url = serializers.HyperlinkedIdentityField(
-        view_name="plugins-api:netbox_dns-api:view-detail"
-    )
-
-    class Meta:
-        model = View
-        fields = ["id", "url", "display", "name"]
-
-
-#
-# Zones
-#
 class NestedZoneSerializer(WritableNestedSerializer):
     def to_representation(self, instance):
         # +
         # Workaround for the problem that the serializer does not return the
         # annotation "active" when called with "many=False". See issue
         # https://github.com/peteeckel/netbox-plugin-dns/issues/132
         #
@@ -35,15 +20,16 @@
             representation["active"] = instance.is_active
 
         return representation
 
     url = serializers.HyperlinkedIdentityField(
         view_name="plugins-api:netbox_dns-api:zone-detail"
     )
-    view = NestedViewSerializer(
+    view = ViewSerializer(
+        nested=True,
         many=False,
         required=False,
         read_only=True,
         help_text="View the zone belongs to",
     )
     active = serializers.BooleanField(
         required=False,
@@ -61,30 +47,14 @@
             "view",
             "status",
             "active",
             "rfc2317_prefix",
         ]
 
 
-#
-# Nameservers
-#
-class NestedNameServerSerializer(WritableNestedSerializer):
-    url = serializers.HyperlinkedIdentityField(
-        view_name="plugins-api:netbox_dns-api:nameserver-detail"
-    )
-
-    class Meta:
-        model = NameServer
-        fields = ["id", "url", "display", "name"]
-
-
-#
-# Records
-#
 class NestedRecordSerializer(WritableNestedSerializer):
     url = serializers.HyperlinkedIdentityField(
         view_name="plugins-api:netbox_dns-api:record-detail"
     )
     zone = NestedZoneSerializer(
         many=False,
         required=False,
@@ -106,33 +76,7 @@
             "name",
             "value",
             "status",
             "ttl",
             "zone",
             "active",
         ]
-
-
-#
-# Registrars
-#
-class NestedRegistrarSerializer(WritableNestedSerializer):
-    url = serializers.HyperlinkedIdentityField(
-        view_name="plugins-api:netbox_dns-api:registrar-detail"
-    )
-
-    class Meta:
-        model = Registrar
-        fields = ["display", "id", "url", "name", "iana_id"]
-
-
-#
-# Contacts
-#
-class NestedContactSerializer(WritableNestedSerializer):
-    url = serializers.HyperlinkedIdentityField(
-        view_name="plugins-api:netbox_dns-api:contact-detail"
-    )
-
-    class Meta:
-        model = Contact
-        fields = ["display", "id", "url", "name", "contact_id"]
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/api/urls.py` & `netbox_plugin_dns-1.0b1/netbox_dns/api/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/api/views.py` & `netbox_plugin_dns-1.0b1/netbox_dns/api/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,34 +9,34 @@
     ViewSerializer,
     ZoneSerializer,
     NameServerSerializer,
     RecordSerializer,
     RegistrarSerializer,
     ContactSerializer,
 )
-from netbox_dns.filters import (
-    ViewFilter,
-    ZoneFilter,
-    NameServerFilter,
-    RecordFilter,
-    RegistrarFilter,
-    ContactFilter,
+from netbox_dns.filtersets import (
+    ViewFilterSet,
+    ZoneFilterSet,
+    NameServerFilterSet,
+    RecordFilterSet,
+    RegistrarFilterSet,
+    ContactFilterSet,
 )
 from netbox_dns.models import View, Zone, NameServer, Record, Registrar, Contact
 
 
 class NetBoxDNSRootView(APIRootView):
     def get_view_name(self):
         return "NetBoxDNS"
 
 
 class ViewViewSet(NetBoxModelViewSet):
     queryset = View.objects.all()
     serializer_class = ViewSerializer
-    filterset_class = ViewFilter
+    filterset_class = ViewFilterSet
 
     @action(detail=True, methods=["get"])
     def views(self, request, pk=None):
         views = View.objects.filter(zone=pk)
         serializer = ViewSerializer(views, many=True, context={"request": request})
         return Response(serializer.data)
 
@@ -47,15 +47,15 @@
         "nameservers",
         "tags",
         "soa_mname",
         "record_set",
         "tenant",
     )
     serializer_class = ZoneSerializer
-    filterset_class = ZoneFilter
+    filterset_class = ZoneFilterSet
 
     @action(detail=True, methods=["get"])
     def records(self, request, pk=None):
         records = Record.objects.filter(zone=pk)
         serializer = RecordSerializer(records, many=True, context={"request": request})
         return Response(serializer.data)
 
@@ -67,27 +67,27 @@
         )
         return Response(serializer.data)
 
 
 class NameServerViewSet(NetBoxModelViewSet):
     queryset = NameServer.objects.prefetch_related("zones", "tenant")
     serializer_class = NameServerSerializer
-    filterset_class = NameServerFilter
+    filterset_class = NameServerFilterSet
 
     @action(detail=True, methods=["get"])
     def zones(self, request, pk=None):
         zones = Zone.objects.filter(nameservers__id=pk)
         serializer = ZoneSerializer(zones, many=True, context={"request": request})
         return Response(serializer.data)
 
 
 class RecordViewSet(NetBoxModelViewSet):
     queryset = Record.objects.all().prefetch_related("zone", "zone__view", "tenant")
     serializer_class = RecordSerializer
-    filterset_class = RecordFilter
+    filterset_class = RecordFilterSet
 
     def destroy(self, request, *args, **kwargs):
         v_object = self.get_object()
         if v_object.managed:
             raise serializers.ValidationError(
                 f"{v_object} is managed, refusing deletion"
             )
@@ -101,14 +101,14 @@
 
         return super().update(request, *args, **kwargs)
 
 
 class RegistrarViewSet(NetBoxModelViewSet):
     queryset = Registrar.objects.all()
     serializer_class = RegistrarSerializer
-    filterset_class = RegistrarFilter
+    filterset_class = RegistrarFilterSet
 
 
 class ContactViewSet(NetBoxModelViewSet):
     queryset = Contact.objects.all()
     serializer_class = ContactSerializer
-    filterset_class = ContactFilter
+    filterset_class = ContactFilterSet
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/fields/address.py` & `netbox_plugin_dns-1.0b1/netbox_dns/fields/address.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/fields/network.py` & `netbox_plugin_dns-1.0b1/netbox_dns/fields/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from django import forms
 from django.db import models
-from django.db.models import Lookup, Transform
+from django.db.models import Lookup, Transform, IntegerField
 from django.core.exceptions import ValidationError
 
 from netaddr import AddrFormatError, IPNetwork
 
 
 class NetContains(Lookup):
     lookup_name = "net_contains"
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/fields/rfc2317.py` & `netbox_plugin_dns-1.0b1/netbox_dns/fields/rfc2317.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
     def to_python(self, value):
         if not value:
             return value
 
         try:
             ip_network = IPNetwork(value)
-        except (AddressFormatError, TypeError, ValueError) as exc:
+        except (AddrFormatError, TypeError, ValueError) as exc:
             raise ValidationError(exc)
 
         if ip_network.version != 4:
             raise ValidationError(INVALID_RFC2317)
 
         return ip_network
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/filters/contact.py` & `netbox_plugin_dns-1.0b1/netbox_dns/filtersets/contact.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from django.db.models import Q
 
 from netbox.filtersets import NetBoxModelFilterSet
 
 from netbox_dns.models import Contact
 
 
-class ContactFilter(NetBoxModelFilterSet):
+class ContactFilterSet(NetBoxModelFilterSet):
     class Meta:
         model = Contact
         fields = (
             "id",
             "name",
+            "description",
             "contact_id",
             "organization",
             "street",
             "city",
             "state_province",
             "postal_code",
             "country",
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/filters/registrar.py` & `netbox_plugin_dns-1.0b1/netbox_dns/filtersets/registrar.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from django.db.models import Q
 
 from netbox.filtersets import NetBoxModelFilterSet
 
 from netbox_dns.models import Registrar
 
 
-class RegistrarFilter(NetBoxModelFilterSet):
+class RegistrarFilterSet(NetBoxModelFilterSet):
     class Meta:
         model = Registrar
         fields = (
             "id",
             "name",
+            "description",
             "iana_id",
             "address",
             "referral_url",
             "whois_server",
             "abuse_email",
             "abuse_phone",
         )
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/filters/zone.py` & `netbox_plugin_dns-1.0b1/netbox_dns/filtersets/record.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,112 +1,124 @@
+import netaddr
+
 import django_filters
 from django.db.models import Q
 
 from netbox.filtersets import NetBoxModelFilterSet
 from tenancy.filtersets import TenancyFilterSet
+from utilities.filters import MultiValueCharFilter
+
+from ipam.models import IPAddress
 
-from netbox_dns.models import View, Zone, ZoneStatusChoices, Registrar, Contact
+from netbox_dns.models import View, Zone, Record, RecordTypeChoices, RecordStatusChoices
 
 
-class ZoneFilter(TenancyFilterSet, NetBoxModelFilterSet):
+class RecordFilterSet(TenancyFilterSet, NetBoxModelFilterSet):
+    fqdn = MultiValueCharFilter(
+        method="filter_fqdn",
+    )
+    type = django_filters.MultipleChoiceFilter(
+        choices=RecordTypeChoices,
+    )
     status = django_filters.MultipleChoiceFilter(
-        choices=ZoneStatusChoices,
+        choices=RecordStatusChoices,
+    )
+    zone_id = django_filters.ModelMultipleChoiceFilter(
+        queryset=Zone.objects.all(),
+        label="Parent Zone ID",
+    )
+    zone = django_filters.ModelMultipleChoiceFilter(
+        queryset=Zone.objects.all(),
+        field_name="zone__name",
+        to_field_name="name",
+        label="Parent Zone",
     )
     view_id = django_filters.ModelMultipleChoiceFilter(
         queryset=View.objects.all(),
-        label="View ID",
+        field_name="zone__view",
+        label="ID of the View the Parent Zone belongs to",
     )
     view = django_filters.ModelMultipleChoiceFilter(
         queryset=View.objects.all(),
-        field_name="view__name",
-        to_field_name="name",
-        label="View",
-    )
-    registrar_id = django_filters.ModelMultipleChoiceFilter(
-        queryset=Registrar.objects.all(),
-        label="Registrar ID",
-    )
-    registrar = django_filters.ModelMultipleChoiceFilter(
-        queryset=Registrar.objects.all(),
-        field_name="registrar__name",
+        field_name="zone__view__name",
         to_field_name="name",
-        label="Registrar",
+        label="View the Parent Zone belongs to",
     )
-    registrant_id = django_filters.ModelMultipleChoiceFilter(
-        queryset=Contact.objects.all(),
-        label="Registrant ID",
-    )
-    registrant = django_filters.ModelMultipleChoiceFilter(
-        queryset=Contact.objects.all(),
-        field_name="registrant__contact_id",
-        to_field_name="contact_id",
-        label="Registrant",
-    )
-    admin_c_id = django_filters.ModelMultipleChoiceFilter(
-        queryset=Contact.objects.all(),
-        label="Administrative Contact ID",
-    )
-    admin_c = django_filters.ModelMultipleChoiceFilter(
-        queryset=Contact.objects.all(),
-        field_name="admin_c__contact_id",
-        to_field_name="contact_id",
-        label="Administrative Contact",
-    )
-    tech_c_id = django_filters.ModelMultipleChoiceFilter(
-        queryset=Contact.objects.all(),
-        label="Technical Contact ID",
-    )
-    tech_c = django_filters.ModelMultipleChoiceFilter(
-        queryset=Contact.objects.all(),
-        field_name="tech_c__contact_id",
-        to_field_name="contact_id",
-        label="Technical Contact",
-    )
-    billing_c_id = django_filters.ModelMultipleChoiceFilter(
-        queryset=Contact.objects.all(),
-        label="Billing Contact ID",
-    )
-    billing_c = django_filters.ModelMultipleChoiceFilter(
-        queryset=Contact.objects.all(),
-        field_name="billing_c__contact_id",
-        to_field_name="contact_id",
-        label="Billing Contact",
+    address_record_id = django_filters.ModelMultipleChoiceFilter(
+        field_name="address_record",
+        queryset=Record.objects.all(),
+        to_field_name="id",
+        label="Address Record",
+    )
+    ptr_record_id = django_filters.ModelMultipleChoiceFilter(
+        field_name="ptr_record",
+        queryset=Record.objects.all(),
+        to_field_name="id",
+        label="Pointer Record",
+    )
+    rfc2317_cname_record_id = django_filters.ModelMultipleChoiceFilter(
+        field_name="rfc2317_cname_record",
+        queryset=Record.objects.all(),
+        to_field_name="id",
+        label="Pointer Record",
+    )
+    ipam_ip_address_id = django_filters.ModelMultipleChoiceFilter(
+        field_name="ipam_ip_address",
+        queryset=IPAddress.objects.all(),
+        to_field_name="id",
+        label="IPAM IP Address",
+    )
+    ip_address = MultiValueCharFilter(
+        method="filter_ip_address",
+        label="IP Address",
     )
 
-    active = django_filters.BooleanFilter(
-        label="Zone is active",
-    )
+    managed = django_filters.BooleanFilter()
 
     class Meta:
-        model = Zone
+        model = Record
         fields = (
             "id",
             "name",
-            "view",
-            "status",
-            "nameservers",
-            "registrar",
-            "registry_domain_id",
-            "registrant",
-            "admin_c",
-            "tech_c",
-            "billing_c",
-            "active",
-            "tenant",
+            "fqdn",
+            "description",
+            "ttl",
+            "value",
+            "disable_ptr",
+            "managed",
         )
 
+    def filter_fqdn(self, queryset, name, value):
+        if not value:
+            return queryset
+
+        fqdns = []
+        for fqdn in value:
+            if not fqdn.endswith("."):
+                fqdn = fqdn + "."
+            fqdns.append(fqdn)
+
+        return queryset.filter(fqdn__in=fqdns)
+
+    def filter_ip_address(self, queryset, name, value):
+        if not value:
+            return queryset
+        try:
+            ip_addresses = [
+                str(netaddr.IPAddress(item)) for item in value if item.strip()
+            ]
+            if not ip_addresses:
+                return queryset
+
+            return queryset.filter(ip_address__in=ip_addresses)
+        except (netaddr.AddrFormatError, ValueError):
+            return queryset.none()
+
     def search(self, queryset, name, value):
-        """Perform the filtered search."""
         if not value.strip():
             return queryset
         qs_filter = (
             Q(name__icontains=value)
-            | Q(status__icontains=value)
-            | Q(view__name__icontains=value)
-            | Q(registrar__name__icontains=value)
-            | Q(registry_domain_id__icontains=value)
-            | Q(registrant__name__icontains=value)
-            | Q(admin_c__name__icontains=value)
-            | Q(tech_c__name__icontains=value)
-            | Q(billing_c__name__icontains=value)
+            | Q(value__icontains=value)
+            | Q(zone__name__icontains=value)
         )
         return queryset.filter(qs_filter)
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/forms/contact.py` & `netbox_plugin_dns-1.0b1/netbox_dns/forms/contact.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,23 +3,46 @@
 from netbox.forms import (
     NetBoxModelBulkEditForm,
     NetBoxModelFilterSetForm,
     NetBoxModelImportForm,
     NetBoxModelForm,
 )
 from utilities.forms.fields import TagFilterField
+from utilities.forms.rendering import FieldSet
 
 from netbox_dns.models import Contact
 
 
 class ContactForm(NetBoxModelForm):
+    fieldsets = (
+        FieldSet(
+            "name",
+            "description",
+            "contact_id",
+            "organization",
+            "street",
+            "city",
+            "state_province",
+            "postal_code",
+            "country",
+            "phone",
+            "phone_ext",
+            "fax",
+            "fax_ext",
+            "email",
+            name="Contact",
+        ),
+        FieldSet("tags", name="Tags"),
+    )
+
     class Meta:
         model = Contact
         fields = (
             "name",
+            "description",
             "contact_id",
             "organization",
             "street",
             "city",
             "state_province",
             "postal_code",
             "country",
@@ -30,33 +53,36 @@
             "email",
             "tags",
         )
 
 
 class ContactFilterForm(NetBoxModelFilterSetForm):
     model = Contact
+
     fieldsets = (
-        (None, ("q", "name", "tags", "contact_id")),
-        (
-            "Address",
-            (
-                "organization",
-                "street",
-                "city",
-                "state_province",
-                "postal_code",
-                "country",
-            ),
+        FieldSet("q", "filter_id", "tag"),
+        FieldSet("name", "contact_id", "description", name="Attributes"),
+        FieldSet(
+            "organization",
+            "street",
+            "city",
+            "state_province",
+            "postal_code",
+            "country",
+            name="Address",
         ),
-        ("Communication", ("phone", "phone_ext", "fax", "fax_ext", "email")),
+        FieldSet("phone", "phone_ext", "fax", "fax_ext", "email", name="Communication"),
     )
 
     name = forms.CharField(
         required=False,
     )
+    description = forms.CharField(
+        required=False,
+    )
     contact_id = forms.CharField(
         required=False,
         label="Contact ID",
     )
     organization = forms.CharField(
         required=False,
     )
@@ -90,22 +116,23 @@
     fax_ext = forms.CharField(
         required=False,
         label="Fax Extension",
     )
     email = forms.CharField(
         required=False,
     )
-    tags = TagFilterField(Contact)
+    tag = TagFilterField(Contact)
 
 
 class ContactImportForm(NetBoxModelImportForm):
     class Meta:
         model = Contact
         fields = (
             "name",
+            "description",
             "contact_id",
             "organization",
             "street",
             "city",
             "state_province",
             "postal_code",
             "country",
@@ -121,14 +148,18 @@
 class ContactBulkEditForm(NetBoxModelBulkEditForm):
     model = Contact
 
     name = forms.CharField(
         required=False,
         label="Name",
     )
+    description = forms.CharField(
+        required=False,
+        label="Description",
+    )
     organization = forms.CharField(
         required=False,
         label="Organization",
     )
     street = forms.CharField(
         required=False,
         label="Street",
@@ -167,40 +198,37 @@
     )
     email = forms.CharField(
         required=False,
         label="Email Address",
     )
 
     fieldsets = (
-        (None, ("name",)),
-        (
-            "Address",
-            (
-                "organization",
-                "street",
-                "city",
-                "state_province",
-                "postal_code",
-                "country",
-            ),
+        FieldSet("name", "description", name="Attributes"),
+        FieldSet(
+            "organization",
+            "street",
+            "city",
+            "state_province",
+            "postal_code",
+            "country",
+            name="Address",
         ),
-        (
-            "Communication",
-            (
-                "phone",
-                "phone_ext",
-                "fax",
-                "fax_ext",
-                "email",
-            ),
+        FieldSet(
+            "phone",
+            "phone_ext",
+            "fax",
+            "fax_ext",
+            "email",
+            name="Communication",
         ),
     )
 
     nullable_fields = (
         "name",
+        "description",
         "organization",
         "street",
         "city",
         "state_province",
         "postal_code",
         "country",
         "phone",
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/forms/nameserver.py` & `netbox_plugin_dns-1.0b1/netbox_dns/forms/nameserver.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 )
 
 from utilities.forms.fields import (
     TagFilterField,
     CSVModelChoiceField,
     DynamicModelChoiceField,
 )
+from utilities.forms.rendering import FieldSet
 from tenancy.models import Tenant
 from tenancy.forms import TenancyForm, TenancyFilterForm
 
 from netbox_dns.models import NameServer
 from netbox_dns.utilities import name_to_unicode
 
 
@@ -24,36 +25,39 @@
         super().__init__(*args, **kwargs)
 
         initial_name = self.initial.get("name")
         if initial_name:
             self.initial["name"] = name_to_unicode(initial_name)
 
     fieldsets = (
-        ("Nameserver", ("name", "description", "tags")),
-        ("Tenancy", ("tenant_group", "tenant")),
+        FieldSet("name", "description", name="Nameserver"),
+        FieldSet("tenant_group", "tenant", name="Tenancy"),
+        FieldSet("tags", name="Tags"),
     )
 
     class Meta:
         model = NameServer
         fields = ("name", "description", "tags", "tenant")
 
 
 class NameServerFilterForm(TenancyFilterForm, NetBoxModelFilterSetForm):
     model = NameServer
 
     name = forms.CharField(
         required=False,
-        label="Name",
+    )
+    description = forms.CharField(
+        required=False,
     )
     tag = TagFilterField(NameServer)
 
     fieldsets = (
-        (None, ("q", "filter_id", "tag")),
-        ("Attributes", ("name",)),
-        ("Tenant", ("tenant_group_id", "tenant_id")),
+        FieldSet("q", "filter_id", "tag"),
+        FieldSet("name", "description", name="Attributes"),
+        FieldSet("tenant_group_id", "tenant_id", name="Tenancy"),
     )
 
 
 class NameServerImportForm(NetBoxModelImportForm):
     tenant = CSVModelChoiceField(
         queryset=Tenant.objects.all(),
         to_field_name="name",
@@ -74,9 +78,18 @@
 
 class NameServerBulkEditForm(NetBoxModelBulkEditForm):
     model = NameServer
 
     description = forms.CharField(max_length=200, required=False)
     tenant = DynamicModelChoiceField(queryset=Tenant.objects.all(), required=False)
 
-    class Meta:
-        nullable_fields = ("description", "tenant")
+    fieldsets = (
+        FieldSet(
+            "name",
+            "description",
+            "tenant",
+            "tags",
+            name="Attributes",
+        ),
+    )
+
+    nullable_fields = ("description", "tenant")
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/forms/record.py` & `netbox_plugin_dns-1.0b1/netbox_dns/forms/record.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     TagFilterField,
     CSVChoiceField,
     CSVModelChoiceField,
     DynamicModelChoiceField,
 )
 from utilities.forms.widgets import BulkEditNullBooleanSelect, APISelect
 from utilities.forms import add_blank_choice
+from utilities.forms.rendering import FieldSet
 from tenancy.models import Tenant
 from tenancy.forms import TenancyForm, TenancyFilterForm
 
 from netbox_dns.models import View, Zone, Record, RecordTypeChoices, RecordStatusChoices
 from netbox_dns.utilities import name_to_unicode
 
 
@@ -37,29 +38,27 @@
     )
     ttl = forms.IntegerField(
         required=False,
         label="TTL",
     )
 
     fieldsets = (
-        (
-            "Record",
-            (
-                "name",
-                "zone",
-                "type",
-                "value",
-                "status",
-                "ttl",
-                "disable_ptr",
-                "description",
-                "tags",
-            ),
+        FieldSet(
+            "name",
+            "zone",
+            "type",
+            "value",
+            "status",
+            "ttl",
+            "disable_ptr",
+            "description",
+            name="Record",
         ),
-        ("Tenancy", ("tenant_group", "tenant")),
+        FieldSet("tenant_group", "tenant", name="Tenancy"),
+        FieldSet("tags", name="Tags"),
     )
 
     class Meta:
         model = Record
 
         fields = (
             "name",
@@ -74,51 +73,53 @@
             "tenant",
         )
 
 
 class RecordFilterForm(TenancyFilterForm, NetBoxModelFilterSetForm):
     model = Record
     fieldsets = (
-        (None, ("q", "filter_id", "tag")),
-        (
-            "Attributes",
-            ("view_id", "zone_id", "name", "fqdn", "type", "value", "status"),
+        FieldSet("q", "filter_id", "tag"),
+        FieldSet(
+            "zone_id",
+            "name",
+            "fqdn",
+            "type",
+            "value",
+            "status",
+            "description",
+            name="Attributes",
         ),
-        ("Tenant", ("tenant_group_id", "tenant_id")),
+        FieldSet("tenant_group_id", "tenant_id", name="Tenancy"),
     )
 
     type = forms.MultipleChoiceField(
         choices=RecordTypeChoices,
         required=False,
     )
     name = forms.CharField(
         required=False,
-        label="Name",
     )
     fqdn = forms.CharField(
         required=False,
         label="FQDN",
     )
     value = forms.CharField(
         required=False,
-        label="Value",
     )
     status = forms.MultipleChoiceField(
         choices=RecordStatusChoices,
         required=False,
     )
     zone_id = DynamicModelMultipleChoiceField(
         queryset=Zone.objects.all(),
         required=False,
         label="Zone",
     )
-    view_id = DynamicModelMultipleChoiceField(
-        queryset=View.objects.all(),
+    description = forms.CharField(
         required=False,
-        label="View",
     )
     tag = TagFilterField(Record)
 
 
 class RecordImportForm(NetBoxModelImportForm):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -227,22 +228,20 @@
     disable_ptr = forms.NullBooleanField(
         required=False, widget=BulkEditNullBooleanSelect(), label="Disable PTR"
     )
     description = forms.CharField(max_length=200, required=False)
     tenant = DynamicModelChoiceField(queryset=Tenant.objects.all(), required=False)
 
     fieldsets = (
-        (
-            None,
-            (
-                "zone",
-                "type",
-                "value",
-                "status",
-                "ttl",
-                "disable_ptr",
-                "description",
-                "tenant",
-            ),
+        FieldSet(
+            "zone",
+            "type",
+            "value",
+            "status",
+            "ttl",
+            "disable_ptr",
+            "description",
+            name="Attributes",
         ),
+        FieldSet("tenant_group", "tenant", name="Tenancy"),
     )
     nullable_fields = ("description", "ttl", "tenant")
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/forms/registrar.py` & `netbox_plugin_dns-1.0b1/netbox_dns/forms/registrar.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,49 +3,73 @@
 from netbox.forms import (
     NetBoxModelBulkEditForm,
     NetBoxModelFilterSetForm,
     NetBoxModelImportForm,
     NetBoxModelForm,
 )
 from utilities.forms.fields import TagFilterField
+from utilities.forms.rendering import FieldSet
 
 from netbox_dns.models import Registrar
 
 
 class RegistrarForm(NetBoxModelForm):
     class Meta:
         model = Registrar
+        fieldsets = (
+            FieldSet(
+                "name",
+                "iana_id",
+                "description",
+                "address",
+                "referral_url",
+                "whois_server",
+                "abuse_email",
+                "abuse_phone",
+                name="Registrar",
+            ),
+            FieldSet("tags", name="Tags"),
+        )
         fields = (
             "name",
             "iana_id",
+            "description",
             "address",
             "referral_url",
             "whois_server",
             "abuse_email",
             "abuse_phone",
             "tags",
         )
 
 
 class RegistrarFilterForm(NetBoxModelFilterSetForm):
     model = Registrar
     fieldsets = (
-        (None, ("q", "name", "iana_id", "tags")),
-        (
-            "Contact",
-            ("address", "referral_url", "whois_server", "abuse_email", "abuse_phone"),
+        FieldSet("q", "filter_id", "tag"),
+        FieldSet("name", "iana_id", "description", name="Attributes"),
+        FieldSet(
+            "address",
+            "referral_url",
+            "whois_server",
+            "abuse_email",
+            "abuse_phone",
+            name="Contact",
         ),
     )
 
     name = forms.CharField(
         required=False,
     )
     address = forms.CharField(
         required=False,
     )
+    description = forms.CharField(
+        required=False,
+    )
     iana_id = forms.IntegerField(
         required=False,
         label="IANA ID",
     )
     referral_url = forms.CharField(
         required=False,
         label="Referral URL",
@@ -58,23 +82,24 @@
         required=False,
         label="Abuse Email",
     )
     abuse_phone = forms.CharField(
         required=False,
         label="Abuse Phone",
     )
-    tags = TagFilterField(Registrar)
+    tag = TagFilterField(Registrar)
 
 
 class RegistrarImportForm(NetBoxModelImportForm):
     class Meta:
         model = Registrar
         fields = (
             "name",
             "iana_id",
+            "description",
             "address",
             "referral_url",
             "whois_server",
             "abuse_email",
             "abuse_phone",
             "tags",
         )
@@ -83,16 +108,21 @@
 class RegistrarBulkEditForm(NetBoxModelBulkEditForm):
     model = Registrar
 
     iana_id = forms.IntegerField(
         required=False,
         label="IANA ID",
     )
+    description = forms.CharField(
+        required=False,
+        label="Description",
+    )
     address = forms.CharField(
         required=False,
+        label="Address",
     )
     referral_url = forms.CharField(
         required=False,
         label="Referral URL",
     )
     whois_server = forms.CharField(
         required=False,
@@ -104,28 +134,28 @@
     )
     abuse_phone = forms.CharField(
         required=False,
         label="Abuse Phone",
     )
 
     fieldsets = (
-        (
-            None,
-            (
-                "iana_id",
-                "address",
-                "referral_url",
-                "whois_server",
-                "abuse_email",
-                "abuse_phone",
-            ),
+        FieldSet(
+            "iana_id",
+            "description",
+            "address",
+            "referral_url",
+            "whois_server",
+            "abuse_email",
+            "abuse_phone",
+            name="Attributes",
         ),
     )
 
     nullable_fields = (
         "iana_id",
+        "description",
         "address",
         "referral_url",
         "whois_server",
         "abuse_email",
         "abuse_phone",
     )
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/forms/zone.py` & `netbox_plugin_dns-1.0b1/netbox_dns/forms/zone.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     TagFilterField,
     CSVChoiceField,
     CSVModelChoiceField,
     CSVModelMultipleChoiceField,
     DynamicModelChoiceField,
 )
 from utilities.forms.widgets import BulkEditNullBooleanSelect, APISelect
+from utilities.forms.rendering import FieldSet
 from utilities.forms import add_blank_choice
 from tenancy.models import Tenant
 from tenancy.forms import TenancyForm, TenancyFilterForm
 
 from netbox_dns.models import (
     View,
     Zone,
@@ -102,59 +103,51 @@
     rfc2317_parent_managed = forms.BooleanField(
         label="RFC2317 Parent Managed",
         help_text="IPv4 reverse zone for deletgating the RFC2317 PTR records is managed in NetBox DNS",
         required=False,
     )
 
     fieldsets = (
-        (
-            "Zone",
-            (
-                "view",
-                "name",
-                "status",
-                "nameservers",
-                "default_ttl",
-                "description",
-            ),
-        ),
-        (
-            "SOA",
-            (
-                "soa_ttl",
-                "soa_mname",
-                "soa_rname",
-                "soa_refresh",
-                "soa_retry",
-                "soa_expire",
-                "soa_minimum",
-                "soa_serial_auto",
-                "soa_serial",
-            ),
-        ),
-        (
-            "RFC2317",
-            (
-                "rfc2317_prefix",
-                "rfc2317_parent_managed",
-            ),
-        ),
-        (
-            "Domain Registration",
-            (
-                "registrar",
-                "registry_domain_id",
-                "registrant",
-                "admin_c",
-                "tech_c",
-                "billing_c",
-            ),
+        FieldSet(
+            "view",
+            "name",
+            "status",
+            "nameservers",
+            "default_ttl",
+            "description",
+            name="Zone",
+        ),
+        FieldSet(
+            "soa_ttl",
+            "soa_mname",
+            "soa_rname",
+            "soa_refresh",
+            "soa_retry",
+            "soa_expire",
+            "soa_minimum",
+            "soa_serial_auto",
+            "soa_serial",
+            name="SOA",
+        ),
+        FieldSet(
+            "rfc2317_prefix",
+            "rfc2317_parent_managed",
+            name="RFC 2317",
         ),
-        ("Tags", ("tags",)),
-        ("Tenancy", ("tenant_group", "tenant")),
+        FieldSet(
+            "registrar",
+            "registry_domain_id",
+            "registrant",
+            "admin_c",
+            "tech_c",
+            "billing_c",
+            name="Domain Registration",
+        ),
+        FieldSet("tags", name="Tags"),
+        FieldSet("tenant", name="Tenancy"),
     )
 
     def __init__(self, *args, **kwargs):
         """Override the __init__ method in order to provide the initial value for the default fields"""
         super().__init__(*args, **kwargs)
 
         initial_name = self.initial.get("name")
@@ -244,36 +237,78 @@
             "soa_mname": "Primary name server for the zone",
         }
 
 
 class ZoneFilterForm(TenancyFilterForm, NetBoxModelFilterSetForm):
     model = Zone
     fieldsets = (
-        (None, ("q", "filter_id", "tag")),
-        ("Attributes", ("view_id", "status", "name", "nameservers")),
-        ("Tenant", ("tenant_group_id", "tenant_id")),
+        FieldSet("q", "filter_id", "tag"),
+        FieldSet(
+            "view_id", "status", "name", "nameservers", "description", name="Attributes"
+        ),
+        FieldSet(
+            "registrar_id",
+            "registry_domain_id",
+            "registrant_id",
+            "admin_c_id",
+            "tech_c_id",
+            "billing_c_id",
+            name="Registration",
+        ),
+        FieldSet("tenant_group_id", "tenant_id", name="Tenancy"),
     )
 
     view_id = DynamicModelMultipleChoiceField(
         queryset=View.objects.all(),
         required=False,
         label="View",
     )
     status = forms.MultipleChoiceField(
         choices=ZoneStatusChoices,
         required=False,
     )
     name = forms.CharField(
         required=False,
-        label="Name",
     )
     nameservers = DynamicModelMultipleChoiceField(
         queryset=NameServer.objects.all(),
         required=False,
     )
+    description = forms.CharField(
+        required=False,
+    )
+    registrar_id = DynamicModelMultipleChoiceField(
+        queryset=Registrar.objects.all(),
+        required=False,
+        label="Registrar",
+    )
+    registry_domain_id = forms.CharField(
+        required=False,
+        label="Registry Domain ID",
+    )
+    registrant_id = DynamicModelMultipleChoiceField(
+        queryset=Contact.objects.all(),
+        required=False,
+        label="Registrant",
+    )
+    admin_c_id = DynamicModelMultipleChoiceField(
+        queryset=Contact.objects.all(),
+        required=False,
+        label="Admin-C",
+    )
+    tech_c_id = DynamicModelMultipleChoiceField(
+        queryset=Contact.objects.all(),
+        required=False,
+        label="Tech-C",
+    )
+    billing_c_id = DynamicModelMultipleChoiceField(
+        queryset=Contact.objects.all(),
+        required=False,
+        label="Billing-C",
+    )
     tag = TagFilterField(Zone)
 
 
 class ZoneImportForm(NetBoxModelImportForm):
     view = CSVModelChoiceField(
         queryset=View.objects.all(),
         required=False,
@@ -652,70 +687,60 @@
         help_text="Assigned tenant",
     )
     tenant = DynamicModelChoiceField(queryset=Tenant.objects.all(), required=False)
 
     model = Zone
 
     fieldsets = (
-        (
-            None,
-            (
-                "view",
-                "status",
-                "nameservers",
-                "default_ttl",
-                "description",
-                "tenant",
-            ),
-        ),
-        (
-            "SOA",
-            (
-                "soa_ttl",
-                "soa_mname",
-                "soa_rname",
-                "soa_serial_auto",
-                "soa_serial",
-                "soa_refresh",
-                "soa_retry",
-                "soa_expire",
-                "soa_minimum",
-            ),
-        ),
-        (
-            "RFC2317",
-            (
-                "rfc2317_prefix",
-                "rfc2317_parent_managed",
-            ),
-        ),
-        (
-            "Domain Registration",
-            (
-                "registrar",
-                "registry_domain_id",
-                "registrant",
-                "admin_c",
-                "tech_c",
-                "billing_c",
-            ),
+        FieldSet(
+            "view",
+            "status",
+            "nameservers",
+            "default_ttl",
+            "description",
+            name="Attributes",
+        ),
+        FieldSet(
+            "soa_ttl",
+            "soa_mname",
+            "soa_rname",
+            "soa_refresh",
+            "soa_retry",
+            "soa_expire",
+            "soa_minimum",
+            "soa_serial_auto",
+            "soa_serial",
+            name="SOA",
         ),
+        FieldSet(
+            "rfc2317_prefix",
+            "rfc2317_parent_managed",
+            name="RFC 2317",
+        ),
+        FieldSet(
+            "registrar",
+            "registry_domain_id",
+            "registrant",
+            "admin_c",
+            "tech_c",
+            "billing_c",
+            name="Domain Registration",
+        ),
+        FieldSet("tenant_group", "tenant", name="Tenancy"),
     )
+
     nullable_fields = (
         "view",
         "description",
         "rfc2317_prefix",
         "registrar",
         "registry_domain_id",
         "registrant",
         "admin_c",
         "tech_c",
         "billing_c",
     )
 
     def clean(self):
-        """
-        If soa_serial_auto is True, set soa_serial to None.
-        """
         cleaned_data = super().clean()
         if cleaned_data.get("soa_serial_auto"):
             cleaned_data["soa_serial"] = None
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/management/commands/cleanup_database.py` & `netbox_plugin_dns-1.0b1/netbox_dns/management/commands/cleanup_database.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,16 @@
-import dns
-from dns import rdtypes, rdata, rdatatype, rdataclass
-
 from netaddr import IPAddress, IPNetwork, AddrFormatError
 
 from django.core.management.base import BaseCommand
 
 from netbox_dns.models import (
     Zone,
     ZoneStatusChoices,
     Record,
     RecordTypeChoices,
-    RecordClassChoices,
 )
 
 
 def zone_rename_passive_status_to_parked(verbose=False):
     passive_zones = Zone.objects.filter(status="passive")
     if passive_zones:
         if verbose:
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/management/commands/cleanup_rrset_ttl.py` & `netbox_plugin_dns-1.0b1/netbox_dns/management/commands/cleanup_rrset_ttl.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,38 +25,36 @@
 
     def handle(self, *model_names, **options):
         self.cleanup_rrset_ttl(**options)
 
         self.stdout.write("RRSet cleanup completed.")
 
     def cleanup_rrset_ttl(self, **options):
-        verbose = options.get("verbosity") > 1
-
         ttl_records = (
             Record.objects.filter(ttl__isnull=False)
             .exclude(type=RecordTypeChoices.SOA)
             .exclude(type=RecordTypeChoices.PTR, maanged=True)
         )
         for record in ttl_records:
             records = Record.objects.filter(
                 name=record.name,
                 zone=record.zone,
                 type=record.type,
             ).exclude(type=RecordTypeChoices.PTR, maanged=True)
 
             if records.count() == 1:
                 if options.get("verbosity") > 2:
-                    self.stdout.write(f"Ignoring single record {record.id} ({record})")
+                    self.stdout.write(f"Ignoring single record {record.pk} ({record})")
                 continue
 
             if options.get("max"):
                 ttl = records.aggregate(Max("ttl")).get("ttl__max")
             else:
                 ttl = records.aggregate(Min("ttl")).get("ttl__min")
 
             for record in records.exclude(ttl=ttl):
                 if options.get("verbosity") > 1:
                     self.stdout.write(
-                        f"Updating TTL for record {record.id} ({record}) to {ttl}"
+                        f"Updating TTL for record {record.pk} ({record}) to {ttl}"
                     )
                 record.ttl = ttl
                 record.save(update_fields=["ttl"], update_rrset_ttl=False)
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/management/commands/setup_coupling.py` & `netbox_plugin_dns-1.0b1/netbox_dns/management/commands/setup_coupling.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,109 +1,109 @@
-from django.core.management.base import BaseCommand, CommandError
+from django.core.management.base import BaseCommand
 
-from django.contrib.contenttypes.models import ContentType
+from core.models import ObjectType
 from extras.models import CustomField
 from extras.choices import CustomFieldTypeChoices
 from ipam.models import IPAddress
-from netbox_dns.models import Record, Zone
+from netbox_dns.models import Zone
 
 
 class Command(BaseCommand):
     help = "Setup IPAddress custom fields needed for IPAM-DNS coupling"
 
     def add_arguments(self, parser):
         parser.add_argument(
             "--remove", action="store_true", help="Remove custom fields"
         )
         parser.add_argument("--verbose", action="store_true", help="Verbose output")
 
     def handle(self, *model_names, **options):
-        ipaddress_object_type = ContentType.objects.get_for_model(IPAddress)
+        ipaddress_object_type = ObjectType.objects.get_for_model(IPAddress)
 
         if options["remove"]:
             for cf in (
                 "ipaddress_dns_record_name",
                 "ipaddress_dns_record_ttl",
                 "ipaddress_dns_record_disable_ptr",
                 "ipaddress_dns_zone_id",
             ):
                 try:
                     CustomField.objects.get(
-                        name=cf, content_types=ipaddress_object_type
+                        name=cf, object_types=ipaddress_object_type
                     ).delete()
                     if options.get("verbose"):
                         self.stdout.write(f"Custom field '{cf}' removed")
-                except:
+                except CustomField.DoesNotExist:
                     pass
 
         else:
             if not CustomField.objects.filter(
                 name="ipaddress_dns_record_name",
                 type=CustomFieldTypeChoices.TYPE_TEXT,
-                content_types=ipaddress_object_type,
+                object_types=ipaddress_object_type,
             ).exists():
                 cf_name = CustomField.objects.create(
                     name="ipaddress_dns_record_name",
                     label="Name",
                     type=CustomFieldTypeChoices.TYPE_TEXT,
                     required=False,
                     group_name="DNS",
                 )
-                cf_name.content_types.set([ipaddress_object_type])
+                cf_name.object_types.set([ipaddress_object_type])
                 if options.get("verbose"):
                     self.stdout.write(
                         "Created custom field 'ipaddress_dns_record_name'"
                     )
 
             if not CustomField.objects.filter(
                 name="ipaddress_dns_record_ttl",
                 type=CustomFieldTypeChoices.TYPE_INTEGER,
-                content_types=ipaddress_object_type,
+                object_types=ipaddress_object_type,
             ).exists():
                 cf_ttl = CustomField.objects.create(
                     name="ipaddress_dns_record_ttl",
                     label="TTL",
                     type=CustomFieldTypeChoices.TYPE_INTEGER,
                     validation_minimum=0,
                     validation_maximum=2147483647,
                     required=False,
                     group_name="DNS",
                 )
-                cf_ttl.content_types.set([ipaddress_object_type])
+                cf_ttl.object_types.set([ipaddress_object_type])
                 if options.get("verbose"):
                     self.stdout.write("Created custom field 'ipaddress_dns_record_ttl'")
 
             if not CustomField.objects.filter(
                 name="ipaddress_dns_record_disable_ptr",
                 type=CustomFieldTypeChoices.TYPE_BOOLEAN,
-                content_types=ipaddress_object_type,
+                object_types=ipaddress_object_type,
             ).exists():
                 cf_disable_ptr = CustomField.objects.create(
                     name="ipaddress_dns_record_disable_ptr",
                     label="Disable PTR",
                     type=CustomFieldTypeChoices.TYPE_BOOLEAN,
                     required=False,
                     default=False,
                     group_name="DNS",
                 )
-                cf_disable_ptr.content_types.set([ipaddress_object_type])
+                cf_disable_ptr.object_types.set([ipaddress_object_type])
                 if options.get("verbose"):
                     self.stdout.write(
                         "Created custom field 'ipaddress_dns_record_disable_ptr'"
                     )
 
             if not CustomField.objects.filter(
                 name="ipaddress_dns_zone_id",
                 type=CustomFieldTypeChoices.TYPE_OBJECT,
-                content_types=ipaddress_object_type,
+                object_types=ipaddress_object_type,
             ).exists():
                 cf_zone = CustomField.objects.create(
                     name="ipaddress_dns_zone_id",
                     label="Zone",
                     type=CustomFieldTypeChoices.TYPE_OBJECT,
-                    object_type=ContentType.objects.get_for_model(Zone),
+                    related_object_type=ObjectType.objects.get_for_model(Zone),
                     required=False,
                     group_name="DNS",
                 )
-                cf_zone.content_types.set([ipaddress_object_type])
+                cf_zone.object_types.set([ipaddress_object_type])
                 if options.get("verbose"):
                     self.stdout.write("Created custom field 'ipaddress_dns_zone_id'")
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/management/commands/update_soa.py` & `netbox_plugin_dns-1.0b1/netbox_dns/management/commands/update_soa.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,8 +15,8 @@
         zones = Zone.objects.all()
 
         for zone in zones:
             if options["verbose"]:
                 self.stdout.write(f"Updating the SOA record for zone {zone.name}")
             zone.update_soa_record()
 
-        self.stdout.write(f"All SOA records have been updated")
+        self.stdout.write("All SOA records have been updated")
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/migrations/0001_squashed_netbox_dns_0_15.py` & `netbox_plugin_dns-1.0b1/netbox_dns/migrations/0001_squashed_netbox_dns_0_15.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,43 +5,16 @@
 import django.db.models.deletion
 from django.db import migrations, models
 
 import netbox_dns.fields.network
 
 
 class Migration(migrations.Migration):
-    replaces = [
-        ("netbox_dns", "0001_initial"),
-        ("netbox_dns", "0015_add_record_status"),
-        ("netbox_dns", "0013_add_nameserver_zone_record_description"),
-        ("netbox_dns", "0011_add_view_model"),
-        ("netbox_dns", "0002_zone_default_ttl"),
-        ("netbox_dns", "0003_soa_managed_records"),
-        ("netbox_dns", "0004_create_ptr_for_a_aaaa_records"),
-        ("netbox_dns", "0006_zone_soa_serial_auto"),
-        ("netbox_dns", "0007_alter_zone_soa_serial_auto"),
-        ("netbox_dns", "0005_update_ns_records"),
-        ("netbox_dns", "0008_zone_status_names"),
-        ("netbox_dns", "0009_netbox32"),
-        ("netbox_dns", "0010_update_soa_records"),
-        ("netbox_dns", "0012_adjust_zone_and_record"),
-        ("netbox_dns", "0014_add_view_description"),
-        ("netbox_dns", "0016_cleanup_ptr_records"),
-        ("netbox_dns", "0017_alter_record_ttl"),
-        ("netbox_dns", "0018_zone_arpa_network"),
-        ("netbox_dns", "0019_update_ns_ttl"),
-    ]
-
-    initial = True
-
     dependencies = [
-        ("extras", "0072_created_datetimefield"),
-        ("extras", "0062_clear_secrets_changelog"),
         ("extras", "0073_journalentry_tags_custom_fields"),
-        ("extras", "0059_exporttemplate_as_attachment"),
     ]
 
     operations = [
         migrations.CreateModel(
             name="NameServer",
             fields=[
                 ("created", models.DateTimeField(auto_now_add=True, null=True)),
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/migrations/0003_soa_managed_records.py` & `netbox_plugin_dns-1.0b1/netbox_dns/migrations/0021_record_ip_address.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,112 +1,110 @@
-# Generated by Django 3.2.9 on 2021-11-04 20:48
+import taggit.managers
 
 import django.core.validators
-from django.db import migrations, models
 import django.db.models.deletion
-import taggit.managers
+from django.db import migrations, models
+
+import netbox_dns.fields.address
+from netbox_dns.models import RecordTypeChoices
+from netbox_dns.utilities import arpa_to_prefix
+
+
+def fqdn(record):
+    if record.name == "@":
+        return f"{record.zone.name}."
+
+    return f"{record.name}.{record.zone.name}."
+
+
+def address_from_name(record):
+    prefix = arpa_to_prefix(fqdn(record))
+    if prefix is not None:
+        return prefix.ip
+
+    return None
+
+
+def update_ip_addresses(apps, schema_editor):
+    Record = apps.get_model("netbox_dns", "Record")
+
+    for record in Record.objects.filter(type=RecordTypeChoices.PTR):
+        record.ip_address = address_from_name(record)
+        record.save()
+
+    for record in Record.objects.filter(
+        type__in=(RecordTypeChoices.A, RecordTypeChoices.AAAA)
+    ):
+        record.ip_address = record.value
+        record.save()
 
 
 class Migration(migrations.Migration):
     dependencies = [
-        ("extras", "0062_clear_secrets_changelog"),
-        ("netbox_dns", "0002_zone_default_ttl"),
+        ("extras", "0084_staging"),
+        ("netbox_dns", "0020_netbox_3_4"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="record",
-            name="managed",
-            field=models.BooleanField(default=False),
+            name="ip_address",
+            field=netbox_dns.fields.address.AddressField(blank=True, null=True),
         ),
-        migrations.AddField(
+        migrations.AlterField(
+            model_name="record",
+            name="tags",
+            field=taggit.managers.TaggableManager(
+                through="extras.TaggedItem", to="extras.Tag"
+            ),
+        ),
+        migrations.AlterField(
             model_name="zone",
             name="soa_expire",
             field=models.PositiveIntegerField(
-                default=2592000,
-                validators=[django.core.validators.MinValueValidator(1)],
+                validators=[django.core.validators.MinValueValidator(1)]
             ),
-            preserve_default=False,
         ),
-        migrations.AddField(
+        migrations.AlterField(
             model_name="zone",
             name="soa_minimum",
             field=models.PositiveIntegerField(
-                default=3600, validators=[django.core.validators.MinValueValidator(1)]
+                validators=[django.core.validators.MinValueValidator(1)]
             ),
-            preserve_default=False,
         ),
-        migrations.AddField(
+        migrations.AlterField(
             model_name="zone",
             name="soa_mname",
             field=models.ForeignKey(
-                default=1,
                 on_delete=django.db.models.deletion.PROTECT,
                 related_name="zones_soa",
                 to="netbox_dns.nameserver",
             ),
-            preserve_default=False,
         ),
-        migrations.AddField(
+        migrations.AlterField(
             model_name="zone",
             name="soa_refresh",
             field=models.PositiveIntegerField(
-                default=172800, validators=[django.core.validators.MinValueValidator(1)]
+                validators=[django.core.validators.MinValueValidator(1)]
             ),
-            preserve_default=False,
         ),
-        migrations.AddField(
+        migrations.AlterField(
             model_name="zone",
             name="soa_retry",
             field=models.PositiveIntegerField(
-                default=7200, validators=[django.core.validators.MinValueValidator(1)]
+                validators=[django.core.validators.MinValueValidator(1)]
             ),
-            preserve_default=False,
         ),
-        migrations.AddField(
+        migrations.AlterField(
             model_name="zone",
             name="soa_rname",
-            field=models.CharField(default="hostmaster.example.com", max_length=255),
-            preserve_default=False,
-        ),
-        migrations.AddField(
-            model_name="zone",
-            name="soa_serial",
-            field=models.PositiveIntegerField(
-                default=1,
-                validators=[
-                    django.core.validators.MinValueValidator(1),
-                    django.core.validators.MaxValueValidator(2147483647),
-                ],
-            ),
-            preserve_default=False,
-        ),
-        migrations.AddField(
-            model_name="zone",
-            name="soa_ttl",
-            field=models.PositiveIntegerField(
-                default=86400, validators=[django.core.validators.MinValueValidator(1)]
-            ),
-            preserve_default=False,
-        ),
-        migrations.AlterField(
-            model_name="nameserver",
-            name="tags",
-            field=taggit.managers.TaggableManager(
-                blank=True, through="extras.TaggedItem", to="extras.Tag"
-            ),
-        ),
-        migrations.AlterField(
-            model_name="record",
-            name="tags",
-            field=taggit.managers.TaggableManager(
-                blank=True, through="extras.TaggedItem", to="extras.Tag"
-            ),
+            field=models.CharField(max_length=255),
         ),
         migrations.AlterField(
             model_name="zone",
-            name="default_ttl",
+            name="soa_ttl",
             field=models.PositiveIntegerField(
-                blank=True, validators=[django.core.validators.MinValueValidator(1)]
+                validators=[django.core.validators.MinValueValidator(1)]
             ),
         ),
+        migrations.RunPython(update_ip_addresses),
     ]
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/migrations/0006_zone_soa_serial_auto.py` & `netbox_plugin_dns-1.0b1/netbox_dns/migrations/0028_rfc2317_fields.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,44 @@
-# Generated by Django 3.2.9 on 2021-11-26 16:54
-
-import django.core.validators
 from django.db import migrations, models
+import django.db.models.deletion
+import netbox_dns.fields.rfc2317
 
 
 class Migration(migrations.Migration):
-    dependencies = [("netbox_dns", "0004_create_ptr_for_a_aaaa_records")]
+    dependencies = [
+        ("netbox_dns", "0027_alter_registrar_iana_id"),
+    ]
 
     operations = [
         migrations.AddField(
             model_name="zone",
-            name="soa_serial_auto",
+            name="rfc2317_prefix",
+            field=netbox_dns.fields.rfc2317.RFC2317NetworkField(blank=True, null=True),
+        ),
+        migrations.AddField(
+            model_name="zone",
+            name="rfc2317_parent_managed",
             field=models.BooleanField(default=False),
-            preserve_default=False,
         ),
-        migrations.AlterField(
+        migrations.AddField(
             model_name="zone",
-            name="soa_serial",
-            field=models.BigIntegerField(
+            name="rfc2317_parent_zone",
+            field=models.ForeignKey(
+                blank=True,
+                null=True,
+                on_delete=django.db.models.deletion.SET_NULL,
+                related_name="rfc2317_child_zones",
+                to="netbox_dns.zone",
+            ),
+        ),
+        migrations.AddField(
+            model_name="record",
+            name="rfc2317_cname_record",
+            field=models.ForeignKey(
                 blank=True,
                 null=True,
-                validators=[
-                    django.core.validators.MinValueValidator(1),
-                    django.core.validators.MaxValueValidator(4294967295),
-                ],
+                on_delete=django.db.models.deletion.SET_NULL,
+                related_name="rfc2317_ptr_records",
+                to="netbox_dns.record",
             ),
         ),
     ]
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/migrations/0020_netbox_3_4.py` & `netbox_plugin_dns-1.0b1/netbox_dns/migrations/0020_netbox_3_4.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from django.db import migrations, models
 import utilities.json
 
 
 class Migration(migrations.Migration):
     dependencies = [
-        ("netbox_dns", "0019_update_ns_ttl"),
+        ("netbox_dns", "0001_squashed_netbox_dns_0_15"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="nameserver",
             name="custom_field_data",
             field=models.JSONField(
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/migrations/0024_tenancy.py` & `netbox_plugin_dns-1.0b1/netbox_dns/migrations/0024_tenancy.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/migrations/0025_ipam_coupling_cf.py` & `netbox_plugin_dns-1.0b1/netbox_dns/migrations/0025_ipam_coupling_cf.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/migrations/0026_domain_registration.py` & `netbox_plugin_dns-1.0b1/netbox_dns/migrations/0026_domain_registration.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/migrations/0029_record_fqdn.py` & `netbox_plugin_dns-1.0b1/netbox_dns/migrations/0029_record_fqdn.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/models/contact.py` & `netbox_plugin_dns-1.0b1/netbox_dns/models/contact.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,18 @@
         max_length=50,
         unique=True,
     )
     name = models.CharField(
         blank=True,
         max_length=100,
     )
+    description = models.CharField(
+        blank=True,
+        max_length=200,
+    )
     organization = models.CharField(
         blank=True,
         max_length=200,
     )
     street = models.CharField(
         blank=True,
         max_length=50,
@@ -75,14 +79,15 @@
     tags = TaggableManager(
         through="extras.TaggedItem",
         related_name="netbox_dns_contact_set",
     )
 
     clone_fields = [
         "name",
+        "description",
         "organization",
         "street",
         "city",
         "state_province",
         "postal_code",
         "country",
         "phone",
@@ -90,15 +95,15 @@
         "fax",
         "fax_ext",
         "email",
         "tags",
     ]
 
     def get_absolute_url(self):
-        return reverse("plugins:netbox_dns:contact", kwargs={"pk": self.id})
+        return reverse("plugins:netbox_dns:contact", kwargs={"pk": self.pk})
 
     def __str__(self):
         if self.name is not None:
             return f"{self.contact_id} ({self.name})"
 
         return self.contact_id
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/models/nameserver.py` & `netbox_plugin_dns-1.0b1/netbox_dns/models/nameserver.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,14 +35,16 @@
         null=True,
     )
 
     clone_fields = ["name", "description"]
 
     class Meta:
         ordering = ("name",)
+        verbose_name = "Nameserver"
+        verbose_name_plural = "Nameservers"
 
     def __str__(self):
         try:
             return dns_name.from_text(self.name, origin=None).to_unicode()
         except dns_name.IDNAException:
             return self.name
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/models/record.py` & `netbox_plugin_dns-1.0b1/netbox_dns/models/record.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,28 +3,22 @@
 import dns
 from dns import rdata, rdatatype, rdataclass
 from dns import name as dns_name
 
 from django.core.exceptions import ValidationError
 from django.db import transaction, models
 from django.db.models import Q, ExpressionWrapper, BooleanField, Min
-from django.db.models.functions import Length
 from django.urls import reverse
 
 from netbox.models import NetBoxModel
 from netbox.search import SearchIndex, register_search
 from utilities.querysets import RestrictedQuerySet
 from utilities.choices import ChoiceSet
 
-try:
-    # NetBox 3.5.0 - 3.5.7, 3.5.9+
-    from extras.plugins import get_plugin_config
-except ImportError:
-    # NetBox 3.5.8
-    from extras.plugins.utils import get_plugin_config
+from netbox.plugins.utils import get_plugin_config
 
 from netbox_dns.fields import AddressField
 from netbox_dns.utilities import (
     arpa_to_prefix,
     name_to_unicode,
 )
 from netbox_dns.validators import (
@@ -39,15 +33,17 @@
 
 
 def min_ttl(*ttl_list):
     return min((ttl for ttl in ttl_list if ttl is not None), default=None)
 
 
 class RecordManager(models.Manager.from_queryset(RestrictedQuerySet)):
-    """Special Manager for records providing the activity status annotation"""
+    """
+    Custom manager for records providing the activity status annotation
+    """
 
     def get_queryset(self):
         return (
             super()
             .get_queryset()
             .annotate(
                 active=ExpressionWrapper(
@@ -214,28 +210,28 @@
         ordering = ("zone", "name", "type", "value", "status")
 
     def __str__(self):
         try:
             name = dns_name.from_text(self.fqdn).relativize(dns_name.root).to_unicode()
         except dns_name.IDNAException:
             name = self.name
-        except dns_name.LabelTooLong as exc:
+        except dns_name.LabelTooLong:
             name = f"{self.name[:59]}..."
 
         return f"{name} [{self.type}]"
 
     @property
     def display_name(self):
         return name_to_unicode(self.name)
 
     def get_status_color(self):
         return RecordStatusChoices.colors.get(self.status)
 
     def get_absolute_url(self):
-        return reverse("plugins:netbox_dns:record", kwargs={"pk": self.id})
+        return reverse("plugins:netbox_dns:record", kwargs={"pk": self.pk})
 
     @property
     def value_fqdn(self):
         if self.type != RecordTypeChoices.CNAME:
             return None
 
         zone = dns_name.from_text(self.zone.name)
@@ -665,15 +661,15 @@
                             "value": f"There is already an active record for name {ptr_cname_name} in zone {ptr_cname_zone}, RFC2317 CNAME is not allowed."
                         }
                     ) from None
 
         if self.type == RecordTypeChoices.SOA and self.name != "@":
             raise ValidationError(
                 {
-                    "name": f"SOA records are only allowed with name @ and are created automatically by NetBox DNS"
+                    "name": "SOA records are only allowed with name @ and are created automatically by NetBox DNS"
                 }
             ) from None
 
         if self.type == RecordTypeChoices.CNAME:
             if records.exclude(type=RecordTypeChoices.NSEC).exists():
                 raise ValidationError(
                     {
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/models/registrar.py` & `netbox_plugin_dns-1.0b1/netbox_dns/models/registrar.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,18 @@
     # +
     # Data fields according to https://www.icann.org/resources/pages/rdds-labeling-policy-2017-02-01-en
     # -
     name = models.CharField(
         unique=True,
         max_length=255,
     )
+    description = models.CharField(
+        blank=True,
+        max_length=200,
+    )
     iana_id = models.IntegerField(
         verbose_name="IANA ID",
         null=True,
         blank=True,
     )
     referral_url = models.URLField(
         verbose_name="Referral URL",
@@ -39,15 +43,15 @@
     abuse_phone = models.CharField(
         verbose_name="Abuse Phone",
         max_length=50,
         blank=True,
     )
 
     def get_absolute_url(self):
-        return reverse("plugins:netbox_dns:registrar", kwargs={"pk": self.id})
+        return reverse("plugins:netbox_dns:registrar", kwargs={"pk": self.pk})
 
     def __str__(self):
         return str(self.name)
 
     class Meta:
         ordering = ("name", "iana_id")
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/models/view.py` & `netbox_plugin_dns-1.0b1/netbox_dns/models/view.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         blank=True,
         null=True,
     )
 
     clone_fields = ["name", "description"]
 
     def get_absolute_url(self):
-        return reverse("plugins:netbox_dns:view", kwargs={"pk": self.id})
+        return reverse("plugins:netbox_dns:view", kwargs={"pk": self.pk})
 
     def __str__(self):
         return str(self.name)
 
     class Meta:
         ordering = ("name",)
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/models/zone.py` & `netbox_plugin_dns-1.0b1/netbox_dns/models/zone.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,20 +18,15 @@
 
 from netbox.models import NetBoxModel
 from netbox.search import SearchIndex, register_search
 from utilities.querysets import RestrictedQuerySet
 from utilities.choices import ChoiceSet
 from ipam.models import IPAddress
 
-try:
-    # NetBox 3.5.0 - 3.5.7, 3.5.9+
-    from extras.plugins import get_plugin_config
-except ImportError:
-    # NetBox 3.5.8
-    from extras.plugins.utils import get_plugin_config
+from netbox.plugins.utils import get_plugin_config
 
 from netbox_dns.fields import NetworkField, RFC2317NetworkField
 from netbox_dns.utilities import (
     arpa_to_prefix,
     name_to_unicode,
     normalize_name,
     NameFormatError,
@@ -44,15 +39,17 @@
 # +
 # This is a hack designed to break cyclic imports between Record and Zone
 # -
 import netbox_dns.models.record as record
 
 
 class ZoneManager(models.Manager.from_queryset(RestrictedQuerySet)):
-    """Special Manager for zones providing the activity status annotation"""
+    """
+    Custom manager for zones providing the activity status annotation
+    """
 
     def get_queryset(self):
         return (
             super()
             .get_queryset()
             .annotate(
                 active=ExpressionWrapper(
@@ -451,15 +448,15 @@
                 ns_warnings.append(
                     f"Nameserver {nameserver.name} does not have an active address record in zone {ns_zone}"
                 )
 
         return ns_warnings, ns_errors
 
     def get_auto_serial(self):
-        records = record.Record.objects.filter(zone=self).exclude(
+        records = record.Record.objects.filter(zone_id=self.pk).exclude(
             type=record.RecordTypeChoices.SOA
         )
         if records:
             soa_serial = (
                 records.aggregate(Max("last_updated"))
                 .get("last_updated__max")
                 .timestamp()
@@ -599,15 +596,15 @@
         if self.is_reverse_zone:
             self.arpa_network = self.network_from_name
 
         if self.is_rfc2317_zone:
             if self.arpa_network is not None:
                 raise ValidationError(
                     {
-                        "rfc2317_prefix": f"A regular reverse zone can not be used as an RFC2317 zone."
+                        "rfc2317_prefix": "A regular reverse zone can not be used as an RFC2317 zone."
                     }
                 )
 
             if self.rfc2317_parent_managed:
                 rfc2317_parent_zone = self.get_rfc2317_parent_zone()
 
                 if rfc2317_parent_zone is None:
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/signals/ipam_coupling.py` & `netbox_plugin_dns-1.0b1/netbox_dns/signals/ipam_coupling.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,20 +14,15 @@
     new_address_record,
     update_address_record,
     check_permission,
     dns_changed,
     DNSPermissionDenied,
 )
 
-try:
-    # NetBox 3.5.0 - 3.5.7, 3.5.9+
-    from extras.plugins import get_plugin_config
-except ImportError:
-    # NetBox 3.5.8
-    from extras.plugins.utils import get_plugin_config
+from netbox.plugins.utils import get_plugin_config
 
 
 @receiver(post_clean, sender=IPAddress)
 def ip_address_check_permissions_save(instance, **kwargs):
     if not instance.address:
         return
 
@@ -35,22 +30,22 @@
         return
 
     request = current_request.get()
     if request is None:
         return
 
     try:
-        if instance.id is None:
+        if instance.pk is None:
             record = new_address_record(instance)
             if record is not None:
                 record.full_clean()
                 check_permission(request, "netbox_dns.add_record", record)
 
         else:
-            if not dns_changed(IPAddress.objects.get(pk=instance.id), instance):
+            if not dns_changed(IPAddress.objects.get(pk=instance.pk), instance):
                 return
 
             record = get_address_record(instance)
             if record is not None:
                 name, ttl, disable_ptr, zone_id = ipaddress_cf_data(instance)
                 if zone_id is not None:
                     update_address_record(record, instance)
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/tables/contact.py` & `netbox_plugin_dns-1.0b1/netbox_dns/tables/contact.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     )
 
     class Meta(NetBoxTable.Meta):
         model = Contact
         fields = (
             "contact_id",
             "name",
+            "description",
             "organization",
             "street",
             "city",
             "state_province",
             "postal_code",
             "country",
             "phone",
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/tables/nameserver.py` & `netbox_plugin_dns-1.0b1/netbox_dns/tables/nameserver.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 from netbox.tables import NetBoxTable, TagColumn
 from tenancy.tables import TenancyColumnsMixin
 
 from netbox_dns.models import NameServer
 
 
 class NameServerTable(TenancyColumnsMixin, NetBoxTable):
-    """Table for displaying NameServer objects."""
-
     name = tables.Column(
         linkify=True,
     )
     tags = TagColumn(
         url_name="plugins:netbox_dns:nameserver_list",
     )
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/tables/record.py` & `netbox_plugin_dns-1.0b1/netbox_dns/tables/record.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/tables/registrar.py` & `netbox_plugin_dns-1.0b1/netbox_dns/tables/registrar.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,14 +13,15 @@
         url_name="plugins:netbox_dns:registrar_list",
     )
 
     class Meta(NetBoxTable.Meta):
         model = Registrar
         fields = (
             "name",
+            "description",
             "iana_id",
             "referral_url",
             "whois_server",
             "abuse_email",
             "abuse_phone",
             "tags",
         )
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/tables/zone.py` & `netbox_plugin_dns-1.0b1/netbox_dns/tables/zone.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/template_content.py` & `netbox_plugin_dns-1.0b1/netbox_dns/template_content.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 from packaging import version
+
 from django.conf import settings
 
-try:
-    # NetBox 3.5.0 - 3.5.7, 3.5.9+
-    from extras.plugins import get_plugin_config
-except ImportError:
-    # NetBox 3.5.8
-    from extras.plugins.utils import get_plugin_config
-from extras.plugins import PluginTemplateExtension
+from netbox.plugins.utils import get_plugin_config
+from netbox.plugins import PluginTemplateExtension
 
 from netbox_dns.models import Record, RecordTypeChoices, Zone, View, NameServer
 from netbox_dns.tables import RelatedRecordTable
 
 
 class RelatedDNSRecords(PluginTemplateExtension):
     model = "ipam.ipaddress"
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/contact.html` & `netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/contact.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,70 +1,74 @@
 {% extends 'generic/object.html' %}
 
 {% block content %}
     <div class="row">
         <div class="col col-md-6">
             <div class="card">
                 <h5 class="card-header">Contact</h5>
-                <div class="card-body">
-                    <table class="table table-hover attr-table">
-                        <tr>
-                            <th scope="row">Name</th>
-                            <td>{{ object.name }}</td>
-                        </tr>
-                        <tr>
-                            <th scope="row">Contact ID</th>
-                            <td>{{ object.contact_id }}</td>
-                        </tr>
-                        <tr>
-                            <th scope="row">Organization</th>
-                            <td>{{ object.organization }}</td>
-                        </tr>
-                        <tr>
-                            <th scope="row">Street</th>
-                            <td>{{ object.street }}</td>
-                        </tr>
-                        <tr>
-                            <th scope="row">City</th>
-                            <td>{{ object.city }}</td>
-                        </tr>
-                        <tr>
-                            <th scope="row">State/Province</th>
-                            <td>{{ object.state_province }}</td>
-                        </tr>
-                        <tr>
-                            <th scope="row">Postal Code</th>
-                            <td>{{ object.postal_code }}</td>
-                        </tr>
-                        <tr>
-                            <th scope="row">Country</th>
-                            <td>{{ object.country }}</td>
-                        </tr>
-                        <tr>
-                            <th scope="row">Phone</th>
-                            <td>{{ object.phone }}</td>
-                        </tr>
-                        <tr>
-                            <th scope="row">Phone Extension</th>
-                            <td>{{ object.phone_ext }}</td>
-                        </tr>
-                        <tr>
-                            <th scope="row">Fax</th>
-                            <td>{{ object.fax }}</td>
-                        </tr>
-                        <tr>
-                            <th scope="row">Fax Extension</th>
-                            <td>{{ object.fax_ext }}</td>
-                        </tr>
-                        <tr>
-                            <th scope="row">Email</th>
-                            <td>{{ object.email }}</td>
-                        </tr>
-                    </table>
-                </div>
+                <table class="table table-hover attr-table">
+                    <tr>
+                        <th scope="row">Name</th>
+                        <td>{{ object.name }}</td>
+                    </tr>
+                     {% if object.description %}
+                    <tr>
+                        <th scope="row">Description</th>
+                        <td style="word-break:break-all;">{{ object.description }}</td>
+                    </tr>
+                    {% endif %}
+                   <tr>
+                        <th scope="row">Contact ID</th>
+                        <td>{{ object.contact_id }}</td>
+                    </tr>
+                    <tr>
+                        <th scope="row">Organization</th>
+                        <td>{{ object.organization }}</td>
+                    </tr>
+                    <tr>
+                        <th scope="row">Street</th>
+                        <td>{{ object.street }}</td>
+                    </tr>
+                    <tr>
+                        <th scope="row">City</th>
+                        <td>{{ object.city }}</td>
+                    </tr>
+                    <tr>
+                        <th scope="row">State/Province</th>
+                        <td>{{ object.state_province }}</td>
+                    </tr>
+                    <tr>
+                        <th scope="row">Postal Code</th>
+                        <td>{{ object.postal_code }}</td>
+                    </tr>
+                    <tr>
+                        <th scope="row">Country</th>
+                        <td>{{ object.country }}</td>
+                    </tr>
+                    <tr>
+                        <th scope="row">Phone</th>
+                        <td>{{ object.phone }}</td>
+                    </tr>
+                    <tr>
+                        <th scope="row">Phone Extension</th>
+                        <td>{{ object.phone_ext }}</td>
+                    </tr>
+                    <tr>
+                        <th scope="row">Fax</th>
+                        <td>{{ object.fax }}</td>
+                    </tr>
+                    <tr>
+                        <th scope="row">Fax Extension</th>
+                        <td>{{ object.fax_ext }}</td>
+                    </tr>
+                    <tr>
+                        <th scope="row">Email</th>
+                        <td>{{ object.email }}</td>
+                    </tr>
+                </table>
             </div>
             {% include 'inc/panels/custom_fields.html' %}
         </div>
         <div class="col col-md-6">
             {% include 'inc/panels/tags.html' %}
         </div>
     </div>
```

#### html2text {}

```diff
@@ -1,10 +1,11 @@
 {% extends 'generic/object.html' %} {% block content %}
 **** CCoonnttaacctt ****
 NNaammee            {{ object.name }}
+DDeessccrriippttiioonn     {{ object.description }}
 CCoonnttaacctt IIDD      {{ object.contact_id }}
 OOrrggaanniizzaattiioonn    {{ object.organization }}
 SSttrreeeett          {{ object.street }}
 CCiittyy            {{ object.city }}
 SSttaattee//PPrroovviinnccee  {{ object.state_province }}
 PPoossttaall CCooddee     {{ object.postal_code }}
 CCoouunnttrryy         {{ object.country }}
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/nameserver.html` & `netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/view.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,35 @@
 {% extends 'generic/object.html' %}
 
 {% block content %}
     <div class="row">
         <div class="col col-md-6">
             <div class="card">
-                <h5 class="card-header">Name Server</h5>
-                <div class="card-body">
-                    <table class="table table-hover attr-table">
-                        <tr>
-                            <th scope="row">Name</th>
-                            <td>{{ object.name }}</td>
-                        </tr>
-                        {% if unicode_name %}
-                            <tr>
-                                <th scope="row">IDN</th>
-                                <td>{{ unicode_name }}</td>
-                            </tr>
-                        {% endif %}
-                        <tr>
-                            <th scope="row">Tenant</th>
-                            <td>
-                                {% if object.tenant.group %}
-                                    {{ object.tenant.group|linkify }} /
-                                {% endif %}
-                                {{ object.tenant|linkify|placeholder }}
-                            </td>
-                        </tr>
-                        <tr>
-                            <th scope="row">Description</th>
-                            <td>{{ object.description }}</td>
-                        </tr>
-                    </table>
-                </div>
+                <h5 class="card-header">View</h5>
+                <table class="table table-hover attr-table">
+                    <tr>
+                        <th scope="row">Name</th>
+                        <td>{{ object.name }}</td>
+                    </tr>
+                    {% if object.description %}
+                    <tr>
+                        <th scope="row">Description</th>
+                        <td style="word-break:break-all;">{{ object.description }}</td>
+                    </tr>
+                    {% endif %}
+                    <tr>
+                        <th scope="row">Tenant</th>
+                        <td>
+                            {% if object.tenant.group %}
+                                {{ object.tenant.group|linkify }} /
+                            {% endif %}
+                            {{ object.tenant|linkify|placeholder }}
+                        </td>
+                    </tr>
+                </table>
             </div>
             {% include 'inc/panels/custom_fields.html' %}
         </div>
         <div class="col col-md-6">
             {% include 'inc/panels/tags.html' %}
         </div>
     </div>
```

#### html2text {}

```diff
@@ -1,10 +1,9 @@
 {% extends 'generic/object.html' %} {% block content %}
-**** NNaammee SSeerrvveerr ****
+**** VViieeww ****
 NNaammee        {{ object.name }}
-IIDDNN         {{ unicode_name }}
+DDeessccrriippttiioonn {{ object.description }}
 TTeennaanntt      {% if object.tenant.group %} {{ object.tenant.group|linkify }} / {%
             endif %} {{ object.tenant|linkify|placeholder }}
-DDeessccrriippttiioonn {{ object.description }}
 {% include 'inc/panels/custom_fields.html' %}
 {% include 'inc/panels/tags.html' %}
 {% endblock %}
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/record/related.html` & `netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/record/related.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/record.html` & `netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/record.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 {% extends 'generic/object.html' %}
 {% load helpers %}
 {% load plugins %}
 {% load render_table from django_tables2 %}
 {% load perms %}
 
-{% block controls %}
+{% block control-buttons %}
 {% if object.managed %}
 {% else %}
 {{ block.super }}
 {% endif %}
-{% endblock controls %}
+{% endblock control-buttons %}
 
 {% block breadcrumbs %}
-{% if not object.managed %}
+{% if object.managed %}
+<li class="breadcrumb-item">
+    <a href="{% url 'plugins:netbox_dns:managed_record_list' %}">{{ 'Managed Records' }}</a>
+</li>
+{% else %}
 {{ block.super }}
 {% endif %}
 {% endblock %}
 
 {% block tabs %}
 {% if object.managed %}
 {% else %}
@@ -29,114 +33,108 @@
     {% if object.managed %}
     <div class="col col-md-12">
     {% else %}
     <div class="col col-md-8">
     {% endif %}
         <div class="card">
             <h5 class="card-header">Record</h5>
-            <div class="card-body">
-                <table class="table table-hover attr-table">
-                    <tr>
-                        <th scope="row">Name</th>
-                        <td style="word-break:break-all;">{{ object.name }}</td>
-                    </tr>
-                    {% if unicode_name %}
-                    <tr>
-                        <th scope="row">IDN</th>
-                        <td style="word-break:break-all;">{{ unicode_name }}</td>
-                    </tr>
-                    {% endif %}
-                    <tr>
-                        <th scope="row">Zone</th>
-                        {% if object.managed %}
-                        <td><a href="{% url 'plugins:netbox_dns:zone_managed_records' pk=object.zone.pk %}">{{ object.zone }}</a></td>
-                        {% else %}
-                        <td><a href="{% url 'plugins:netbox_dns:zone_records' pk=object.zone.pk %}">{{ object.zone }}</a></td>
-                        {% endif %}
-                    </tr>
-                    {% if not object.managed %}
-                    <tr>
-                        <th scope="row">Tenant</th>
-                        <td>
-                            {% if object.tenant.group %}
-                                {{ object.tenant.group|linkify }} /
-                            {% endif %}
-                            {{ object.tenant|linkify|placeholder }}
-                        </td>
-                    </tr>
-                    {% endif %}
-                    <tr>
-                        <th scope="row">Type</th>
-                        <td>{{ object.type }}</td>
-                    </tr>
-                    <tr>
-                        <th scope="row">Value</th>
-                        <td style="word-break:break-all;">{{ object.value }}</td>
-                    </tr>
-                    {% if unicode_value %}
-                    <tr>
-                        <th scope="row">Unicode Value</th>
-                        <td style="word-break:break-all;">{{ unicode_value }}</td>
-                    </tr>
-                    {% endif %}
-                    <tr>
-                        <th scope="row">TTL</th>
-                        <td>{{ object.ttl|placeholder }}</td>
-                    </tr>
-                    {% if object.type == 'A' or object.type == 'AAAA' %}
-                    <tr>
-                        <th scope="row">Disable PTR</th>
-                        <td>{% checkmark object.disable_ptr %}</td>
-                    </tr>
-                    {% endif %}
-                    {% if object.ptr_record %}
-                    <tr>
-                        <th scope="row">PTR Record</th>
-                        <td><a href="{% url 'plugins:netbox_dns:record' pk=object.ptr_record.pk %}">{{ object.ptr_record }}</td>
-                    </tr>
-                    {% endif %}
-                    {% if object.address_record %}
-                    <tr>
-                        <th scope="row">Address Record</th>
-                        <td><a href="{% url 'plugins:netbox_dns:record' pk=object.address_record.pk %}">{{ object.address_record }}</td>
-                    </tr>
-                        {% if object.address_record.ipam_ip_address %}
-                        <tr>
-                            <th scope="row">IPAM IP Address</th>
-                            <td><a href="{% url 'ipam:ipaddress' pk=object.address_record.ipam_ip_address.pk %}">{{ object.address_record.ipam_ip_address }}</td>
-                        </tr>
+            <table class="table table-hover attr-table">
+                <tr>
+                    <th scope="row">Name</th>
+                    <td style="word-break:break-all;">{{ object.name }}</td>
+                </tr>
+                {% if unicode_name %}
+                <tr>
+                    <th scope="row">IDN</th>
+                    <td style="word-break:break-all;">{{ unicode_name }}</td>
+                </tr>
+                {% endif %}
+                <tr>
+                    <th scope="row">Zone</th>
+                    {% if object.managed %}
+                    <td><a href="{% url 'plugins:netbox_dns:zone_managed_records' pk=object.zone.pk %}">{{ object.zone }}</a></td>
+                    {% else %}
+                    <td><a href="{% url 'plugins:netbox_dns:zone_records' pk=object.zone.pk %}">{{ object.zone }}</a></td>
+                    {% endif %}
+                </tr>
+                {% if not object.managed %}
+                <tr>
+                    <th scope="row">Tenant</th>
+                    <td>
+                        {% if object.tenant.group %}
+                            {{ object.tenant.group|linkify }} /
                         {% endif %}
-                    {% endif %}
-                    {% if object.ipam_ip_address %}
+                        {{ object.tenant|linkify|placeholder }}
+                    </td>
+                </tr>
+                {% endif %}
+                <tr>
+                    <th scope="row">Type</th>
+                    <td>{{ object.type }}</td>
+                </tr>
+                <tr>
+                    <th scope="row">Value</th>
+                    <td style="word-break:break-all;">{{ object.value }}</td>
+                </tr>
+                {% if unicode_value %}
+                <tr>
+                    <th scope="row">Unicode Value</th>
+                    <td style="word-break:break-all;">{{ unicode_value }}</td>
+                </tr>
+                {% endif %}
+                <tr>
+                    <th scope="row">TTL</th>
+                    <td>{{ object.ttl|placeholder }}</td>
+                </tr>
+                {% if object.type == 'A' or object.type == 'AAAA' %}
+                <tr>
+                    <th scope="row">Disable PTR</th>
+                    <td>{% checkmark object.disable_ptr %}</td>
+                </tr>
+                {% endif %}
+                {% if object.ptr_record %}
+                <tr>
+                    <th scope="row">PTR Record</th>
+                    <td><a href="{% url 'plugins:netbox_dns:record' pk=object.ptr_record.pk %}">{{ object.ptr_record }}</td>
+                </tr>
+                {% endif %}
+                {% if object.address_record %}
+                <tr>
+                    <th scope="row">Address Record</th>
+                    <td><a href="{% url 'plugins:netbox_dns:record' pk=object.address_record.pk %}">{{ object.address_record }}</td>
+                </tr>
+                    {% if object.address_record.ipam_ip_address %}
                     <tr>
                         <th scope="row">IPAM IP Address</th>
-                        <td><a href="{% url 'ipam:ipaddress' pk=object.ipam_ip_address.pk %}">{{ object.ipam_ip_address }}</td>
-                    </tr>
-                    {% endif %}
-                    <tr>
-                        <th scope="row">Status</th>
-                        <td>{% badge object.get_status_display bg_color=object.get_status_color %}</td>
-                    </tr>
-                    {% if object.description %}
-                    <tr>
-                        <th scope="row">Description</th>
-                        <td style="word-break:break-all;">{{ object.description }}</td>
+                        <td><a href="{% url 'ipam:ipaddress' pk=object.address_record.ipam_ip_address.pk %}">{{ object.address_record.ipam_ip_address }}</td>
                     </tr>
                     {% endif %}
-                </table>
-            </div>
+                {% endif %}
+                {% if object.ipam_ip_address %}
+                <tr>
+                    <th scope="row">IPAM IP Address</th>
+                    <td><a href="{% url 'ipam:ipaddress' pk=object.ipam_ip_address.pk %}">{{ object.ipam_ip_address }}</td>
+                </tr>
+                {% endif %}
+                <tr>
+                    <th scope="row">Status</th>
+                    <td>{% badge object.get_status_display bg_color=object.get_status_color %}</td>
+                </tr>
+                {% if object.description %}
+                <tr>
+                    <th scope="row">Description</th>
+                    <td style="word-break:break-all;">{{ object.description }}</td>
+                </tr>
+                {% endif %}
+            </table>
         </div>
         {% if cname_target_table and cname_target_table.rows|length > 0 %}
-        <div class="card">
-            {% include 'inc/panel_table.html' with table=cname_target_table heading='CNAME Targets' %}
-        </div>
+        {% include 'inc/panel_table.html' with table=cname_target_table heading='CNAME Targets' %}
         {% elif cname_table and cname_table.rows|length > 0 %}
-        <div class="card">
-            {% include 'inc/panel_table.html' with table=cname_table heading='CNAMEs' %}
-        </div>
+        {% include 'inc/panel_table.html' with table=cname_table heading='CNAMEs' %}
         {% endif %}
         {% if not object.managed %}
         {% include 'inc/panels/custom_fields.html' %}
         {% endif %}
     </div>
     {% if not object.managed %}
     <div class="col col-md-4">
```

#### html2text {}

```diff
@@ -1,13 +1,15 @@
 {% extends 'generic/object.html' %} {% load helpers %} {% load plugins %} {%
-load render_table from django_tables2 %} {% load perms %} {% block controls %}
-{% if object.managed %} {% else %} {{ block.super }} {% endif %} {% endblock
-controls %} {% block breadcrumbs %} {% if not object.managed %} {{ block.super
-}} {% endif %} {% endblock %} {% block tabs %} {% if object.managed %} {% else
-%} {{ block.super }} {% endif %} {% endblock %} {% block content %}
+load render_table from django_tables2 %} {% load perms %} {% block control-
+buttons %} {% if object.managed %} {% else %} {{ block.super }} {% endif %} {%
+endblock control-buttons %} {% block breadcrumbs %} {% if object.managed %}
+_{_{_ _'_M_a_n_a_g_e_d_ _R_e_c_o_r_d_s_'_ _}_}
+{% else %} {{ block.super }} {% endif %} {% endblock %} {% block tabs %} {% if
+object.managed %} {% else %} {{ block.super }} {% endif %} {% endblock %} {%
+block content %}
 {% if object.managed %}
 {% else %}
 {% endif %}
 **** RReeccoorrdd ****
 NNaammee            {{ object.name }}
 IIDDNN             {{ unicode_name }}
 ZZoonnee            _{_{_ _o_b_j_e_c_t_._z_o_n_e_ _}_}                           _{_{_ _o_b_j_e_c_t_._z_o_n_e_ _}_}
@@ -22,18 +24,16 @@
 PPTTRR RReeccoorrdd      _{_{_ _o_b_j_e_c_t_._p_t_r___r_e_c_o_r_d_ _}_}
 AAddddrreessss RReeccoorrdd  _{_{_ _o_b_j_e_c_t_._a_d_d_r_e_s_s___r_e_c_o_r_d_ _}_}
 IIPPAAMM IIPP AAddddrreessss _{_{_ _o_b_j_e_c_t_._a_d_d_r_e_s_s___r_e_c_o_r_d_._i_p_a_m___i_p___a_d_d_r_e_s_s_ _}_}
 IIPPAAMM IIPP AAddddrreessss _{_{_ _o_b_j_e_c_t_._i_p_a_m___i_p___a_d_d_r_e_s_s_ _}_}
 SSttaattuuss          {% badge object.get_status_display
                 bg_color=object.get_status_color %}
 DDeessccrriippttiioonn     {{ object.description }}
-{% if cname_target_table and cname_target_table.rows|length > 0 %}
-{% include 'inc/panel_table.html' with table=cname_target_table heading='CNAME
-Targets' %}
-{% elif cname_table and cname_table.rows|length > 0 %}
-{% include 'inc/panel_table.html' with table=cname_table heading='CNAMEs' %}
-{% endif %} {% if not object.managed %} {% include 'inc/panels/
-custom_fields.html' %} {% endif %}
+{% if cname_target_table and cname_target_table.rows|length > 0 %} {% include
+'inc/panel_table.html' with table=cname_target_table heading='CNAME Targets' %}
+{% elif cname_table and cname_table.rows|length > 0 %} {% include 'inc/
+panel_table.html' with table=cname_table heading='CNAMEs' %} {% endif %} {% if
+not object.managed %} {% include 'inc/panels/custom_fields.html' %} {% endif %}
 {% if not object.managed %}
 {% include 'inc/panels/tags.html' %}
 {% endif %}
 {% endblock %}
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/registrar.html` & `netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/registrar.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,53 +1,55 @@
 {% extends 'generic/object.html' %}
 
 {% block content %}
     <div class="row">
         <div class="col col-md-6">
             <div class="card">
                 <h5 class="card-header">Registrar</h5>
-                <div class="card-body">
-                    <table class="table table-hover attr-table">
-                        <tr>
-                            <th scope="row">Name</th>
-                            <td>{{ object.name }}</td>
-                        </tr>
-                        <tr>
-                            <th scope="row">IANA ID</th>
-                            <td>{{ object.iana_id }}</td>
-                        </tr>
-                    </table>
-                </div>
+                <table class="table table-hover attr-table">
+                    <tr>
+                        <th scope="row">Name</th>
+                        <td>{{ object.name }}</td>
+                    </tr>
+                    {% if object.description %}
+                    <tr>
+                        <th scope="row">Description</th>
+                        <td style="word-break:break-all;">{{ object.description }}</td>
+                    </tr>
+                    {% endif %}
+                    <tr>
+                        <th scope="row">IANA ID</th>
+                        <td>{{ object.iana_id }}</td>
+                    </tr>
+                </table>
             </div>
             <div class="card">
                 <h5 class="card-header">Contact Details</h5>
-                <div class="card-body">
-                    <table class="table table-hover attr-table">
-                        <tr>
-                            <th scope="row">Address</th>
-                            <td>{{ object.address }}</td>
-                        </tr>
-                        <tr>
-                            <th scope="row">Referral URL</th>
-                            <td><a href="{{ object.referral_url }}">{{ object.referral_url }}</a></td>
-                        </tr>
-                        <tr>
-                            <th scope="row">WHOIS Server</th>
-                            <td>{{ object.whois_server }}</td>
-                        </tr>
-                        <tr>
-                            <th scope="row">Abuse Email</th>
-                            <td>{{ object.abuse_email }}</td>
-                        </tr>
-                        <tr>
-                            <th scope="row">Abuse Phone</th>
-                            <td>{{ object.abuse_phone }}</td>
-                        </tr>
-                    </table>
-                </div>
+                <table class="table table-hover attr-table">
+                    <tr>
+                        <th scope="row">Address</th>
+                        <td>{{ object.address }}</td>
+                    </tr>
+                    <tr>
+                        <th scope="row">Referral URL</th>
+                        <td><a href="{{ object.referral_url }}">{{ object.referral_url }}</a></td>
+                    </tr>
+                    <tr>
+                        <th scope="row">WHOIS Server</th>
+                        <td>{{ object.whois_server }}</td>
+                    </tr>
+                    <tr>
+                        <th scope="row">Abuse Email</th>
+                        <td>{{ object.abuse_email }}</td>
+                    </tr>
+                    <tr>
+                        <th scope="row">Abuse Phone</th>
+                        <td>{{ object.abuse_phone }}</td>
+                    </tr>
+                </table>
             </div>
             {% include 'inc/panels/custom_fields.html' %}
         </div>
         <div class="col col-md-6">
             {% include 'inc/panels/tags.html' %}
         </div>
     </div>
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
 {% extends 'generic/object.html' %} {% block content %}
 **** RReeggiissttrraarr ****
-NNaammee    {{ object.name }}
-IIAANNAA IIDD {{ object.iana_id }}
+NNaammee        {{ object.name }}
+DDeessccrriippttiioonn {{ object.description }}
+IIAANNAA IIDD     {{ object.iana_id }}
 **** CCoonnttaacctt DDeettaaiillss ****
 AAddddrreessss      {{ object.address }}
 RReeffeerrrraall UURRLL _{_{_ _o_b_j_e_c_t_._r_e_f_e_r_r_a_l___u_r_l_ _}_}
 WWHHOOIISS SSeerrvveerr {{ object.whois_server }}
 AAbbuussee EEmmaaiill  {{ object.abuse_email }}
 AAbbuussee PPhhoonnee  {{ object.abuse_phone }}
 {% include 'inc/panels/custom_fields.html' %}
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/related_dns_objects.html` & `netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/related_dns_objects.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/view.html` & `netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/nameserver.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 {% extends 'generic/object.html' %}
 
 {% block content %}
     <div class="row">
         <div class="col col-md-6">
             <div class="card">
-                <h5 class="card-header">View</h5>
-                <div class="card-body">
-                    <table class="table table-hover attr-table">
-                        <tr>
-                            <th scope="row">Name</th>
-                            <td>{{ object.name }}</td>
-                        </tr>
-                        <tr>
-                            <th scope="row">Tenant</th>
-                            <td>
-                                {% if object.tenant.group %}
-                                    {{ object.tenant.group|linkify }} /
-                                {% endif %}
-                                {{ object.tenant|linkify|placeholder }}
-                            </td>
-                        </tr>
-                        <tr>
-                            <th scope="row">Description</th>
-                            <td>{{ object.description }}</td>
-                        </tr>
-                    </table>
-                </div>
+                <h5 class="card-header">Name Server</h5>
+                <table class="table table-hover attr-table">
+                    <tr>
+                        <th scope="row">Name</th>
+                        <td>{{ object.name }}</td>
+                    </tr>
+                    {% if unicode_name %}
+                    <tr>
+                        <th scope="row">IDN</th>
+                        <td>{{ unicode_name }}</td>
+                    </tr>
+                    {% endif %}
+                    {% if object.description %}
+                    <tr>
+                        <th scope="row">Description</th>
+                        <td style="word-break:break-all;">{{ object.description }}</td>
+                    </tr>
+                    {% endif %}
+                    <tr>
+                        <th scope="row">Tenant</th>
+                        <td>
+                            {% if object.tenant.group %}
+                                {{ object.tenant.group|linkify }} /
+                            {% endif %}
+                            {{ object.tenant|linkify|placeholder }}
+                        </td>
+                    </tr>
+                </table>
             </div>
             {% include 'inc/panels/custom_fields.html' %}
         </div>
         <div class="col col-md-6">
             {% include 'inc/panels/tags.html' %}
         </div>
     </div>
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
 {% extends 'generic/object.html' %} {% block content %}
-**** VViieeww ****
+**** NNaammee SSeerrvveerr ****
 NNaammee        {{ object.name }}
+IIDDNN         {{ unicode_name }}
+DDeessccrriippttiioonn {{ object.description }}
 TTeennaanntt      {% if object.tenant.group %} {{ object.tenant.group|linkify }} / {%
             endif %} {{ object.tenant|linkify|placeholder }}
-DDeessccrriippttiioonn {{ object.description }}
 {% include 'inc/panels/custom_fields.html' %}
 {% include 'inc/panels/tags.html' %}
 {% endblock %}
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/zone/child.html` & `netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/zone/child.html`

 * *Files 6% similar despite different names*

```diff
@@ -7,31 +7,31 @@
     {% include 'inc/table_controls_htmx.html' with table_modal="ZoneTable_config" %}
 
     <form method="post">
         {% csrf_token %}
         <input type="hidden" name="return_url" value="{% if return_url %}{{ return_url }}{% else %}{{ request.path }}{% if request.GET %}?{{ request.GET.urlencode }}{% endif %}{% endif %}" />
 
         <div class="card">
-            <div class="card-body htmx-container table-responsive" id="object_list">
+            <div class="htmx-container table-responsive" id="object_list">
                 {% include 'htmx/table.html' %}
             </div>
         </div>
 
         {% if perms.netbox_dns.change_zone or perms.netbox_dns.delete_zone %}
              {% with bulk_edit_url="plugins:netbox_dns:zone_bulk_edit" bulk_delete_url="plugins:netbox_dns:zone_bulk_delete" %}
                  <div class="noprint bulk-buttons">
                      <div class="bulk-button-group">
                          {% block bulk_buttons %}{% endblock %}
                          {% if bulk_edit_url and perms.netbox_dns.change_zone %}
-                             <button type="submit" name="_edit" formaction="{% url bulk_edit_url %}{% if request.GET %}?{{ request.GET.urlencode }}{% endif %}" class="btn btn-warning btn-sm">
+                             <button type="submit" name="_edit" formaction="{% url bulk_edit_url %}{% if request.GET %}?{{ request.GET.urlencode }}{% endif %}" class="btn btn-warning">
                                  <i class="mdi mdi-pencil" aria-hidden="true"></i> Edit Selected
                              </button>
                          {% endif %}
                          {% if bulk_delete_url and perms.netbox_dns.delete_zone %}
-                             <button type="submit" name="_delete" formaction="{% url bulk_delete_url %}{% if request.GET %}?{{ request.GET.urlencode }}{% endif %}" class="btn btn-danger btn-sm">
+                             <button type="submit" name="_delete" formaction="{% url bulk_delete_url %}{% if request.GET %}?{{ request.GET.urlencode }}{% endif %}" class="btn btn-danger">
                                  <i class="mdi mdi-trash-can-outline" aria-hidden="true"></i> Delete Selected
                              </button>
                          {% endif %}
                      </div>
                  </div>
              {% endwith %}
         {% endif %}
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/zone/managed_record.html` & `netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/zone/managed_record.html`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 {% load helpers %}
 {% load render_table from django_tables2 %}
 {% load perms %}
 
 {% block content %}
     {% include 'inc/table_controls_htmx.html' with table_modal="ManagedRecordTable_config" %}
     <div class="card">
-        <div class="card-body htmx-container table-responsive" id="object_list">
+        <div class="htmx-container table-responsive" id="object_list">
             {% include 'htmx/table.html' %}
         </div>
     </div>
 {% endblock %}
 
 {% block modals %}
     {{ block.super }}
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/zone/record.html` & `netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/zone/record.html`

 * *Files 9% similar despite different names*

```diff
@@ -7,31 +7,31 @@
     {% include 'inc/table_controls_htmx.html' with table_modal="RecordTable_config" %}
 
     <form method="post">
         {% csrf_token %}
         <input type="hidden" name="return_url" value="{% if return_url %}{{ return_url }}{% else %}{{ request.path }}{% if request.GET %}?{{ request.GET.urlencode }}{% endif %}{% endif %}" />
 
         <div class="card">
-            <div class="card-body htmx-container table-responsive" id="object_list">
+            <div class="htmx-container table-responsive" id="object_list">
                 {% include 'htmx/table.html' %}
             </div>
         </div>
 
         {% if perms.netbox_dns.change_record or perms.netbox_dns.delete_record %}
              {% with bulk_edit_url="plugins:netbox_dns:record_bulk_edit" bulk_delete_url="plugins:netbox_dns:record_bulk_delete" %}
                  <div class="noprint bulk-buttons">
                        <div class="bulk-button-group">
                            {% block bulk_buttons %}{% endblock %}
                            {% if bulk_edit_url and perms.netbox_dns.change_record %}
-                               <button type="submit" name="_edit" formaction="{% url bulk_edit_url %}{% if request.GET %}?{{ request.GET.urlencode }}{% endif %}" class="btn btn-warning btn-sm">
+                               <button type="submit" name="_edit" formaction="{% url bulk_edit_url %}{% if request.GET %}?{{ request.GET.urlencode }}{% endif %}" class="btn btn-warning">
                                    <i class="mdi mdi-pencil" aria-hidden="true"></i> Edit Selected
                                </button>
                            {% endif %}
                            {% if bulk_delete_url and perms.netbox_dns.delete_record %}
-                               <button type="submit" name="_delete" formaction="{% url bulk_delete_url %}{% if request.GET %}?{{ request.GET.urlencode }}{% endif %}" class="btn btn-danger btn-sm">
+                               <button type="submit" name="_delete" formaction="{% url bulk_delete_url %}{% if request.GET %}?{{ request.GET.urlencode }}{% endif %}" class="btn btn-danger">
                                    <i class="mdi mdi-trash-can-outline" aria-hidden="true"></i> Delete Selected
                                </button>
                            {% endif %}
                        </div>
                  </div>
              {% endwith %}
          {% endif %}
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/zone/registration.html` & `netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/zone/registration.html`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 {% extends 'netbox_dns/zone/base.html' %}
 {% load helpers %}
 
 {% block content %}
 <div class="card">
     <h5 class="card-header">Domain Registration</h5>
-    <div class="card-body">
-        <table class="table table-hover attr-table">
-            <tr>
-                <th scope="row">Registrar</th>
-                <td>{{ object.registrar|linkify|placeholder }}</td>
-            </tr>
-            <tr>
-                <th scope="row">Registry Domain ID</th>
-                <td>{{ object.registry_domain_id|placeholder }}</td>
-            </tr>
-            <tr>
-                <th scope="row">Registrant</th>
-                <td>{{ object.registrant|linkify|placeholder }}</td>
-            </tr>
-            <tr>
-                <th scope="row">Administrative Contact</th>
-                <td>{{ object.admin_c|linkify|placeholder }}</td>
-            </tr>
-            <tr>
-                <th scope="row">Technical Contact</th>
-                <td>{{ object.tech_c|linkify|placeholder }}</td>
-            </tr>
-            <tr>
-                <th scope="row">Billing Contact</th>
-                <td>{{ object.billing_c|linkify|placeholder }}</td>
-            </tr>
-        </table>
+    <table class="table table-hover attr-table">
+        <tr>
+            <th scope="row">Registrar</th>
+            <td>{{ object.registrar|linkify|placeholder }}</td>
+        </tr>
+        <tr>
+            <th scope="row">Registry Domain ID</th>
+            <td>{{ object.registry_domain_id|placeholder }}</td>
+        </tr>
+        <tr>
+            <th scope="row">Registrant</th>
+            <td>{{ object.registrant|linkify|placeholder }}</td>
+        </tr>
+        <tr>
+            <th scope="row">Administrative Contact</th>
+            <td>{{ object.admin_c|linkify|placeholder }}</td>
+        </tr>
+        <tr>
+            <th scope="row">Technical Contact</th>
+            <td>{{ object.tech_c|linkify|placeholder }}</td>
+        </tr>
+        <tr>
+            <th scope="row">Billing Contact</th>
+            <td>{{ object.billing_c|linkify|placeholder }}</td>
+        </tr>
+    </table>
     </div>
 </div>
 {% endblock %}
 
 {% block modals %}
     {{ block.super }}
 {% endblock modals %}
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/zone/rfc2317_child_zone.html` & `netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/zone/rfc2317_child_zone.html`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 {% load helpers %}
 {% load render_table from django_tables2 %}
 {% load perms %}
 
 {% block content %}
     {% include 'inc/table_controls_htmx.html' with table_modal="RFC2317ChildZoneTable_config" %}
     <div class="card">
-        <div class="card-body htmx-container table-responsive" id="object_list">
+        <div class="htmx-container table-responsive" id="object_list">
             {% include 'htmx/table.html' %}
         </div>
     </div>
 {% endblock %}
 
 {% block modals %}
     {{ block.super }}
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/templates/netbox_dns/zone.html` & `netbox_plugin_dns-1.0b1/netbox_dns/templates/netbox_dns/zone.html`

 * *Files 8% similar despite different names*

```diff
@@ -5,174 +5,175 @@
 {% block content %}
 <div class="row">
     <div class="col col-md-6">
         <div class="card">
             <h5 class="card-header">
                 Zone
             </h5>
-            <div class="card-body">
-                <table class="table table-hover attr-table">
-                    <tr>
-                        <th scope="row">Name</th>
-                        <td>{{ object.name }}</td>
-                    </tr>
-                    {% if unicode_name %}
-                        <tr>
-                            <th scope="row">IDN</th>
-                            <td>{{ unicode_name }}</td>
-                        </tr>
-                    {% endif %}
-                    {% if object.view %}
-                    <tr>
-                        <th scope="row">View</th>
-                        <td>
-                            <a href="{% url 'plugins:netbox_dns:view' pk=object.view.pk %}">
-                                {{ object.view }}
-                            </a>
-                        </td>
-                    </tr>
-                    {% endif %}
-                    <tr>
-                        <th scope="row">Tenant</th>
-                        <td>
-                            {% if object.tenant.group %}
-                                {{ object.tenant.group|linkify }} /
-                            {% endif %}
-                            {{ object.tenant|linkify|placeholder }}
-                        </td>
-                    </tr>
-                    <tr>
-                        <th scope="row">Status</th>
-                        <td>{% badge object.get_status_display bg_color=object.get_status_color %}</td>
-                    </tr>
-                    <tr>
-                        <th scope="row">Nameservers</th>
-                        <td>
-                            <table>
-                                {% for nameserver in object.nameservers.all %}
-                                <tr>
-                                    <td>
-                                        <a href="{% url 'plugins:netbox_dns:nameserver' pk=nameserver.pk %}">
-                                            {{ nameserver }}
-                                        </a>
-                                    </td>
-                                </tr>
-                                {% endfor %}
-                            </table>
-                        </td>
-                    {% if nameserver_warnings %}
-                    <tr>
-                        <th class="text-warning" scope="row">Warnings</th>
-                        <td>
-                            <table>
-                                {% for warning in nameserver_warnings %}
-                                <tr>
-                                    <td class="text-warning">{{ warning }}</td>
-                                </tr>
-                                {% endfor %}
-                            </table>
-                        </td>
-                    </tr>
-                    {% endif %}
-                    {% if nameserver_errors %}
-                    <tr>
-                        <th class="text-danger" scope="row">Errors</th>
-                        <td>
-                            <table>
-                                {% for error in nameserver_errors %}
-                                <tr>
-                                    <td class="text-danger">{{ error }}</td>
-                                </tr>
-                                {% endfor %}
-                            </table>
-                        </td>
-                    </tr>
-                    {% endif %}
-                    </tr>
-                    <tr>
-                        <th scope="row">Default TTL</th>
-                        <td>{{ object.default_ttl }}</td>
-                    </tr>
-                    <tr>
-                        <th scope="row">Description</th>
-                        <td>{{ object.description }}</td>
-                    </tr>
-                </table>
-            </div>
+            <table class="table table-hover attr-table">
+                <tr>
+                    <th scope="row">Name</th>
+                    <td>{{ object.name }}</td>
+                </tr>
+                {% if unicode_name %}
+                    <tr>
+                        <th scope="row">IDN</th>
+                        <td>{{ unicode_name }}</td>
+                    </tr>
+                {% endif %}
+                {% if object.view %}
+                <tr>
+                    <th scope="row">View</th>
+                    <td>
+                        <a href="{% url 'plugins:netbox_dns:view' pk=object.view.pk %}">
+                            {{ object.view }}
+                        </a>
+                    </td>
+                </tr>
+                {% endif %}
+                {% if object.description %}
+                <tr>
+                    <th scope="row">Description</th>
+                    <td style="word-break:break-all;">{{ object.description }}</td>
+                </tr>
+                {% endif %}
+                <tr>
+                    <th scope="row">Tenant</th>
+                    <td>
+                        {% if object.tenant.group %}
+                            {{ object.tenant.group|linkify }} /
+                        {% endif %}
+                        {{ object.tenant|linkify|placeholder }}
+                    </td>
+                </tr>
+                <tr>
+                    <th scope="row">Status</th>
+                    <td>{% badge object.get_status_display bg_color=object.get_status_color %}</td>
+                </tr>
+                <tr>
+                    <th scope="row">Nameservers</th>
+                    <td>
+                        <table>
+                            {% for nameserver in object.nameservers.all %}
+                            <tr>
+                                <td>
+                                    <a href="{% url 'plugins:netbox_dns:nameserver' pk=nameserver.pk %}">
+                                        {{ nameserver }}
+                                    </a>
+                                </td>
+                            </tr>
+                            {% endfor %}
+                        </table>
+                    </td>
+                {% if nameserver_warnings %}
+                <tr>
+                    <th class="text-warning" scope="row">Warnings</th>
+                    <td>
+                        <table>
+                            {% for warning in nameserver_warnings %}
+                            <tr>
+                                <td class="text-warning">{{ warning }}</td>
+                            </tr>
+                            {% endfor %}
+                        </table>
+                    </td>
+                </tr>
+                {% endif %}
+                {% if nameserver_errors %}
+                <tr>
+                    <th class="text-danger" scope="row">Errors</th>
+                    <td>
+                        <table>
+                            {% for error in nameserver_errors %}
+                            <tr>
+                                <td class="text-danger">{{ error }}</td>
+                            </tr>
+                            {% endfor %}
+                        </table>
+                    </td>
+                </tr>
+                {% endif %}
+                </tr>
+                <tr>
+                    <th scope="row">Default TTL</th>
+                    <td>{{ object.default_ttl }}</td>
+                </tr>
+                <tr>
+                    <th scope="row">Description</th>
+                    <td>{{ object.description }}</td>
+                </tr>
+            </table>
         </div>
 
         {% include 'inc/panels/tags.html' %}
         {% include 'inc/panels/custom_fields.html' %}
     </div>
     <div class="col col-md-6">
         <div class="card">
             <h5 class="card-header">Zone SOA</h5>
-            <div class="card-body">
-                <table class="table table-hover attr-table">
-                    <tr>
-                        <th scope="row">TTL</th>
-                        <td>{{ object.soa_ttl }}</td>
-                    </tr>
-                    <tr>
-                        <th scope="row">Primary Nameserver</th>
-                        <td><a href="{% url 'plugins:netbox_dns:nameserver' pk=object.soa_mname.pk %}">{{ object.soa_mname }}</a></td>
-                    </tr>
-                    <tr>
-                        <th scope="row">Responsible</th>
-                        <td>{{ object.soa_rname }}</td>
-                    </tr>
-                    {% if object.soa_serial_auto %}
-                    <tr>
-                        <th scope="row">Serial (auto-generated)</th>
-                        <td>{{ object.soa_serial }}</td>
-                    </tr>
-                    {% else %}
-                    <tr>
-                        <th scope="row">Serial</th>
-                        <td>{{ object.soa_serial }}</td>
-                    </tr>
-                    {% endif %}
-                    <tr>
-                        <th scope="row">Refresh</th>
-                        <td>{{ object.soa_refresh }}</td>
-                    </tr>
-                    <tr>
-                        <th scope="row">Retry</th>
-                        <td>{{ object.soa_retry }}</td>
-                    </tr>
-                    <tr>
-                        <th scope="row">Expire</th>
-                        <td>{{ object.soa_expire }}</td>
-                    </tr>
-                    <tr>
-                        <th scope="row">Minimum TTL</th>
-                        <td>{{ object.soa_minimum }}</td>
-                    </tr>
-                </table>
-            </div>
+            <table class="table table-hover attr-table">
+                <tr>
+                    <th scope="row">TTL</th>
+                    <td>{{ object.soa_ttl }}</td>
+                </tr>
+                <tr>
+                    <th scope="row">Primary Nameserver</th>
+                    <td><a href="{% url 'plugins:netbox_dns:nameserver' pk=object.soa_mname.pk %}">{{ object.soa_mname }}</a></td>
+                </tr>
+                <tr>
+                    <th scope="row">Responsible</th>
+                    <td>{{ object.soa_rname }}</td>
+                </tr>
+                {% if object.soa_serial_auto %}
+                <tr>
+                    <th scope="row">Serial (auto-generated)</th>
+                    <td>{{ object.soa_serial }}</td>
+                </tr>
+                {% else %}
+                <tr>
+                    <th scope="row">Serial</th>
+                    <td>{{ object.soa_serial }}</td>
+                </tr>
+                {% endif %}
+                <tr>
+                    <th scope="row">Refresh</th>
+                    <td>{{ object.soa_refresh }}</td>
+                </tr>
+                <tr>
+                    <th scope="row">Retry</th>
+                    <td>{{ object.soa_retry }}</td>
+                </tr>
+                <tr>
+                    <th scope="row">Expire</th>
+                    <td>{{ object.soa_expire }}</td>
+                </tr>
+                <tr>
+                    <th scope="row">Minimum TTL</th>
+                    <td>{{ object.soa_minimum }}</td>
+                </tr>
+            </table>
         </div>
         {% if object.rfc2317_prefix %}
         <div class="card">
             <h5 class="card-header">RFC2317</h5>
-            <div class="card-body">
-                <table class="table table-hover soa-table">
-                    <tr>
-                        <th scope="row">Prefix</th>
-                        <td>{{ object.rfc2317_prefix }}</td>
-                    </tr>
-                    <tr>
-                        <th scope="row">Parent Managed</th>
-                        <td>{% checkmark object.rfc2317_parent_managed %}</td>
-                    </tr>
-                    {% if object.rfc2317_parent_managed %}
-                    <tr>
-                        <th scope="row">Parent Zone</th>
-                        <td><a href="{% url 'plugins:netbox_dns:zone' pk=object.rfc2317_parent_zone.pk %}">{{ object.rfc2317_parent_zone }}</a></td>
-                    </tr>
-                    {% endif %}
-                </table>
+            <table class="table table-hover soa-table">
+                <tr>
+                    <th scope="row">Prefix</th>
+                    <td>{{ object.rfc2317_prefix }}</td>
+                </tr>
+                <tr>
+                    <th scope="row">Parent Managed</th>
+                    <td>{% checkmark object.rfc2317_parent_managed %}</td>
+                </tr>
+                {% if object.rfc2317_parent_managed %}
+                <tr>
+                    <th scope="row">Parent Zone</th>
+                    <td><a href="{% url 'plugins:netbox_dns:zone' pk=object.rfc2317_parent_zone.pk %}">{{ object.rfc2317_parent_zone }}</a></td>
+                </tr>
+                {% endif %}
+            </table>
             </div>
         </div>
         {% endif %}
     </div>
 </div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
 {% extends 'netbox_dns/zone/base.html' %} {% load helpers %} {% load
 render_table from django_tables2 %} {% block content %}
 **** ZZoonnee ****
 NNaammee        {{ object.name }}
 IIDDNN         {{ unicode_name }}
 VViieeww        _{_{_ _o_b_j_e_c_t_._v_i_e_w_ _}_}
+DDeessccrriippttiioonn {{ object.description }}
 TTeennaanntt      {% if object.tenant.group %} {{ object.tenant.group|linkify }} / {%
             endif %} {{ object.tenant|linkify|placeholder }}
 SSttaattuuss      {% badge object.get_status_display bg_color=object.get_status_color
             %}
 NNaammeesseerrvveerrss _{_{_ _n_a_m_e_s_e_r_v_e_r_ _}_}
 WWaarrnniinnggss    {{ warning }}
 EErrrroorrss      {{ error }}
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/urls.py` & `netbox_plugin_dns-1.0b1/netbox_dns/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/utilities/__init__.py` & `netbox_plugin_dns-1.0b1/netbox_dns/utilities/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 import re
 
 from dns import name as dns_name
 from dns.exception import DNSException
 from netaddr import IPNetwork, AddrFormatError
 
-try:
-    # NetBox 3.5.0 - 3.5.7, 3.5.9+
-    from extras.plugins import get_plugin_config
-except ImportError:
-    # NetBox 3.5.8
-    from extras.plugins.utils import get_plugin_config
+from netbox.plugins.utils import get_plugin_config
 
 
 class NameFormatError(Exception):
     pass
 
 
 def arpa_to_prefix(arpa_name):
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/utilities/ipam_coupling.py` & `netbox_plugin_dns-1.0b1/netbox_dns/utilities/ipam_coupling.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,13 @@
 from ipam.choices import IPAddressStatusChoices
 from utilities.permissions import resolve_permission
 
 from netbox_dns.models import Record, RecordTypeChoices, RecordStatusChoices
 
-try:
-    # NetBox 3.5.0 - 3.5.7, 3.5.9+
-    from extras.plugins import get_plugin_config
-except ImportError:
-    # NetBox 3.5.8
-    from extras.plugins.utils import get_plugin_config
+from netbox.plugins.utils import get_plugin_config
 
 
 class DNSPermissionDenied(Exception):
     pass
 
 
 def ipaddress_cf_data(ip_address):
@@ -65,15 +60,15 @@
         name=name,
         zone_id=zone_id,
         ttl=ttl,
         disable_ptr=disable_ptr,
         status=address_record_status(instance),
         type=address_record_type(instance),
         value=str(instance.address.ip),
-        ipam_ip_address_id=instance.id,
+        ipam_ip_address_id=instance.pk,
         managed=True,
     )
 
 
 def update_address_record(record, ip_address):
     name, ttl, disable_ptr, zone_id = ipaddress_cf_data(ip_address)
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/validators/dns_name.py` & `netbox_plugin_dns-1.0b1/netbox_dns/validators/dns_name.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 import re
 
 from django.core.exceptions import ValidationError
 
-try:
-    # NetBox 3.5.0 - 3.5.7, 3.5.9+
-    from extras.plugins import get_plugin_config
-except ImportError:
-    # NetBox 3.5.8
-    from extras.plugins.utils import get_plugin_config
+from netbox.plugins.utils import get_plugin_config
 
 LABEL = r"[a-z0-9][a-z0-9-]*(?<!-)"
 TOLERANT_LABEL = r"[a-z0-9][a-z0-9-_]*(?<![-_])"
 LEADING_UNDERSCORE_LABEL = r"[a-z0-9_][a-z0-9-]*(?<!-)"
 TOLERANT_LEADING_UNDERSCORE_LABEL = r"[a-z0-9_][a-z0-9-_]*(?<![-_])"
 
 
@@ -22,36 +17,36 @@
 def validate_fqdn(name):
     if get_plugin_config("netbox_dns", "tolerate_underscores_in_hostnames"):
         regex = rf"^(\*|{TOLERANT_LABEL})(\.{TOLERANT_LABEL})+\.?$"
     else:
         regex = rf"^(\*|{LABEL})(\.{LABEL})+\.?$"
 
     if not re.match(regex, name, flags=re.IGNORECASE) or has_invalid_double_dash(name):
-        raise ValidationError(f"Not a valid fully qualified DNS host name")
+        raise ValidationError("Not a valid fully qualified DNS host name")
 
 
 def validate_extended_hostname(name, tolerate_leading_underscores=False):
     if tolerate_leading_underscores:
         if get_plugin_config("netbox_dns", "tolerate_underscores_in_hostnames"):
             regex = rf"^([*@]|(\*\.)?{TOLERANT_LEADING_UNDERSCORE_LABEL}(\.{TOLERANT_LEADING_UNDERSCORE_LABEL})*\.?)$"
         else:
             regex = rf"^([*@]|(\*\.)?{LEADING_UNDERSCORE_LABEL}(\.{LEADING_UNDERSCORE_LABEL})*\.?)$"
     elif get_plugin_config("netbox_dns", "tolerate_underscores_in_hostnames"):
         regex = rf"^([*@]|(\*\.)?{TOLERANT_LABEL}(\.{TOLERANT_LABEL})*\.?)$"
     else:
         regex = rf"^([*@]|(\*\.)?{LABEL}(\.{LABEL})*\.?)$"
 
     if not re.match(regex, name, flags=re.IGNORECASE) or has_invalid_double_dash(name):
-        raise ValidationError(f"Not a valid DNS host name")
+        raise ValidationError("Not a valid DNS host name")
 
 
 def validate_domain_name(name):
     if name == "." and get_plugin_config("netbox_dns", "enable_root_zones"):
         return
 
     if get_plugin_config("netbox_dns", "tolerate_underscores_in_hostnames"):
         regex = rf"^{TOLERANT_LABEL}(\.{TOLERANT_LABEL})*\.?$"
     else:
         regex = rf"^{LABEL}(\.{LABEL})*\.?$"
 
     if not re.match(regex, name, flags=re.IGNORECASE) or has_invalid_double_dash(name):
-        raise ValidationError(f"Not a valid DNS domain name")
+        raise ValidationError("Not a valid DNS domain name")
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/views/contact.py` & `netbox_plugin_dns-1.0b1/netbox_dns/views/contact.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from django.db.models import Q
 
 from netbox.views import generic
 
 from utilities.views import ViewTab, register_model_view
 
 from netbox_dns.models import Contact, Zone
-from netbox_dns.filters import ContactFilter, ZoneFilter
+from netbox_dns.filtersets import ContactFilterSet, ZoneFilterSet
 from netbox_dns.forms import (
     ContactForm,
     ContactFilterForm,
     ContactImportForm,
     ContactBulkEditForm,
 )
 from netbox_dns.tables import ContactTable, ZoneTable
@@ -18,15 +18,15 @@
 class ContactView(generic.ObjectView):
     queryset = Contact.objects.all()
 
 
 class ContactListView(generic.ObjectListView):
     queryset = Contact.objects.all()
     table = ContactTable
-    filterset = ContactFilter
+    filterset = ContactFilterSet
     filterset_form = ContactFilterForm
 
 
 class ContactEditView(generic.ObjectEditView):
     queryset = Contact.objects.all()
     form = ContactForm
     default_return_url = "plugins:netbox_dns:contact_list"
@@ -42,15 +42,15 @@
     model_form = ContactImportForm
     table = ContactTable
     default_return_url = "plugins:netbox_dns:contact_list"
 
 
 class ContactBulkEditView(generic.BulkEditView):
     queryset = Contact.objects.all()
-    filterset = ContactFilter
+    filterset = ContactFilterSet
     table = ContactTable
     form = ContactBulkEditForm
 
 
 class ContactBulkDeleteView(generic.BulkDeleteView):
     queryset = Contact.objects.all()
     table = ContactTable
@@ -59,15 +59,15 @@
 @register_model_view(Contact, "zones")
 class ContactZoneListView(generic.ObjectChildrenView):
     queryset = Contact.objects.all().prefetch_related(
         "zone_set", "admin_c_zones", "tech_c_zones", "billing_c_zones"
     )
     child_model = Zone
     table = ZoneTable
-    filterset = ZoneFilter
+    filterset = ZoneFilterSet
     template_name = "netbox_dns/zone/child.html"
     hide_if_empty = True
 
     tab = ViewTab(
         label="Zones",
         permission="netbox_dns.view_zone",
         badge=lambda obj: len(obj.zones),
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/views/nameserver.py` & `netbox_plugin_dns-1.0b1/netbox_dns/views/nameserver.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from dns import name as dns_name
 
 from netbox.views import generic
 from utilities.views import ViewTab, register_model_view
 
-from netbox_dns.filters import NameServerFilter, ZoneFilter
+from netbox_dns.filtersets import NameServerFilterSet, ZoneFilterSet
 from netbox_dns.forms import (
     NameServerImportForm,
     NameServerFilterForm,
     NameServerForm,
     NameServerBulkEditForm,
 )
 from netbox_dns.models import Zone, NameServer
 from netbox_dns.tables import NameServerTable, ZoneTable
 
 
 class NameServerListView(generic.ObjectListView):
     queryset = NameServer.objects.all()
-    filterset = NameServerFilter
+    filterset = NameServerFilterSet
     filterset_form = NameServerFilterForm
     table = NameServerTable
 
 
 class NameServerView(generic.ObjectView):
     queryset = NameServer.objects.all().prefetch_related("zones")
 
@@ -50,30 +50,30 @@
     model_form = NameServerImportForm
     table = NameServerTable
     default_return_url = "plugins:netbox_dns:nameserver_list"
 
 
 class NameServerBulkEditView(generic.BulkEditView):
     queryset = NameServer.objects.all()
-    filterset = NameServerFilter
+    filterset = NameServerFilterSet
     table = NameServerTable
     form = NameServerBulkEditForm
 
 
 class NameServerBulkDeleteView(generic.BulkDeleteView):
     queryset = NameServer.objects.all()
     table = NameServerTable
 
 
 @register_model_view(NameServer, "zones")
 class NameServerZoneListView(generic.ObjectChildrenView):
     queryset = NameServer.objects.all().prefetch_related("zones")
     child_model = Zone
     table = ZoneTable
-    filterset = ZoneFilter
+    filterset = ZoneFilterSet
     template_name = "netbox_dns/zone/child.html"
     hide_if_empty = True
 
     tab = ViewTab(
         label="Zones",
         permission="netbox_dns.view_zone",
         badge=lambda obj: obj.zones.count(),
@@ -85,15 +85,15 @@
 
 
 @register_model_view(NameServer, "soa_zones")
 class NameServerSOAZoneListView(generic.ObjectChildrenView):
     queryset = NameServer.objects.all().prefetch_related("zones_soa")
     child_model = Zone
     table = ZoneTable
-    filterset = ZoneFilter
+    filterset = ZoneFilterSet
     template_name = "netbox_dns/zone/child.html"
     hide_if_empty = True
 
     tab = ViewTab(
         label="SOA Zones",
         permission="netbox_dns.view_zone",
         badge=lambda obj: obj.zones_soa.count(),
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/views/record.py` & `netbox_plugin_dns-1.0b1/netbox_dns/views/record.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dns import name as dns_name
 
 from django.db.models import Q
 from django.db.models.functions import Length
 
 from netbox.views import generic
 
-from netbox_dns.filters import RecordFilter
+from netbox_dns.filtersets import RecordFilterSet
 from netbox_dns.forms import (
     RecordImportForm,
     RecordFilterForm,
     RecordForm,
     RecordBulkEditForm,
 )
 from netbox_dns.models import Record, RecordTypeChoices, Zone
@@ -17,27 +17,27 @@
 from netbox_dns.utilities import value_to_unicode
 
 
 class RecordListView(generic.ObjectListView):
     queryset = Record.objects.filter(managed=False).prefetch_related(
         "zone", "ptr_record"
     )
-    filterset = RecordFilter
+    filterset = RecordFilterSet
     filterset_form = RecordFilterForm
     table = RecordTable
 
 
 class ManagedRecordListView(generic.ObjectListView):
     queryset = Record.objects.filter(managed=True).prefetch_related(
         "zone", "address_record"
     )
-    filterset = RecordFilter
+    filterset = RecordFilterSet
     filterset_form = RecordFilterForm
     table = ManagedRecordTable
-    actions = ("export",)
+    actions = {"export": {"view"}}
     template_name = "netbox_dns/record/managed.html"
 
 
 class RecordView(generic.ObjectView):
     queryset = Record.objects.all().prefetch_related("zone", "ptr_record")
 
     def get_value_records(self, instance):
@@ -145,15 +145,15 @@
     model_form = RecordImportForm
     table = RecordTable
     default_return_url = "plugins:netbox_dns:record_list"
 
 
 class RecordBulkEditView(generic.BulkEditView):
     queryset = Record.objects.filter(managed=False).prefetch_related("zone")
-    filterset = RecordFilter
+    filterset = RecordFilterSet
     table = RecordTable
     form = RecordBulkEditForm
 
 
 class RecordBulkDeleteView(generic.BulkDeleteView):
     queryset = Record.objects.filter(managed=False)
     table = RecordTable
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/views/registrar.py` & `netbox_plugin_dns-1.0b1/netbox_dns/views/registrar.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from netbox.views import generic
 
 from utilities.views import ViewTab, register_model_view
 
 from netbox_dns.models import Registrar, Zone
-from netbox_dns.filters import RegistrarFilter, ZoneFilter
+from netbox_dns.filtersets import RegistrarFilterSet, ZoneFilterSet
 from netbox_dns.forms import (
     RegistrarForm,
     RegistrarFilterForm,
     RegistrarImportForm,
     RegistrarBulkEditForm,
 )
 from netbox_dns.tables import RegistrarTable, ZoneTable
@@ -16,15 +16,15 @@
 class RegistrarView(generic.ObjectView):
     queryset = Registrar.objects.all()
 
 
 class RegistrarListView(generic.ObjectListView):
     queryset = Registrar.objects.all()
     table = RegistrarTable
-    filterset = RegistrarFilter
+    filterset = RegistrarFilterSet
     filterset_form = RegistrarFilterForm
 
 
 class RegistrarEditView(generic.ObjectEditView):
     queryset = Registrar.objects.all()
     form = RegistrarForm
     default_return_url = "plugins:netbox_dns:registrar_list"
@@ -40,30 +40,30 @@
     model_form = RegistrarImportForm
     table = RegistrarTable
     default_return_url = "plugins:netbox_dns:registrar_list"
 
 
 class RegistrarBulkEditView(generic.BulkEditView):
     queryset = Registrar.objects.all()
-    filterset = RegistrarFilter
+    filterset = RegistrarFilterSet
     table = RegistrarTable
     form = RegistrarBulkEditForm
 
 
 class RegistrarBulkDeleteView(generic.BulkDeleteView):
     queryset = Registrar.objects.all()
     table = RegistrarTable
 
 
 @register_model_view(Registrar, "zones")
 class RegistrarZoneListView(generic.ObjectChildrenView):
     queryset = Registrar.objects.all().prefetch_related("zone_set")
     child_model = Zone
     table = ZoneTable
-    filterset = ZoneFilter
+    filterset = ZoneFilterSet
     template_name = "netbox_dns/zone/child.html"
     hide_if_empty = True
 
     tab = ViewTab(
         label="Zones",
         permission="netbox_dns.view_zone",
         badge=lambda obj: obj.zone_set.count(),
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/views/view.py` & `netbox_plugin_dns-1.0b1/netbox_dns/views/view.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from utilities.views import ViewTab, register_model_view
 
 from netbox.views import generic
 
 from netbox_dns.models import View, Zone
-from netbox_dns.filters import ViewFilter, ZoneFilter
+from netbox_dns.filtersets import ViewFilterSet, ZoneFilterSet
 from netbox_dns.forms import ViewForm, ViewFilterForm, ViewImportForm, ViewBulkEditForm
 from netbox_dns.tables import ViewTable, ZoneTable
 
 
 class ViewView(generic.ObjectView):
     queryset = View.objects.all().prefetch_related("zone_set")
 
 
 class ViewListView(generic.ObjectListView):
     queryset = View.objects.all()
     table = ViewTable
-    filterset = ViewFilter
+    filterset = ViewFilterSet
     filterset_form = ViewFilterForm
 
 
 class ViewEditView(generic.ObjectEditView):
     queryset = View.objects.all()
     form = ViewForm
     default_return_url = "plugins:netbox_dns:view_list"
@@ -35,30 +35,30 @@
     model_form = ViewImportForm
     table = ViewTable
     default_return_url = "plugins:netbox_dns:view_list"
 
 
 class ViewBulkEditView(generic.BulkEditView):
     queryset = View.objects.all()
-    filterset = ViewFilter
+    filterset = ViewFilterSet
     table = ViewTable
     form = ViewBulkEditForm
 
 
 class ViewBulkDeleteView(generic.BulkDeleteView):
     queryset = View.objects.all()
     table = ViewTable
 
 
 @register_model_view(View, "zones")
 class ViewZoneListView(generic.ObjectChildrenView):
     queryset = View.objects.all().prefetch_related("zone_set")
     child_model = Zone
     table = ZoneTable
-    filterset = ZoneFilter
+    filterset = ZoneFilterSet
     template_name = "netbox_dns/zone/child.html"
     hide_if_empty = True
 
     tab = ViewTab(
         label="Zones",
         permission="netbox_dns.view_zone",
         badge=lambda obj: obj.zone_set.count(),
```

### Comparing `netbox_plugin_dns-0.22.8/netbox_dns/views/zone.py` & `netbox_plugin_dns-1.0b1/netbox_dns/views/zone.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from dns import name as dns_name
 
 from netbox.views import generic
 from utilities.views import ViewTab, register_model_view
 
-from netbox_dns.filters import ZoneFilter, RecordFilter
+from netbox_dns.filtersets import ZoneFilterSet, RecordFilterSet
 from netbox_dns.forms import (
     ZoneImportForm,
     ZoneForm,
     ZoneFilterForm,
     ZoneBulkEditForm,
 )
 from netbox_dns.models import Record, Zone
@@ -16,15 +16,15 @@
     RecordTable,
     ManagedRecordTable,
 )
 
 
 class ZoneListView(generic.ObjectListView):
     queryset = Zone.objects.all().prefetch_related("view", "tags")
-    filterset = ZoneFilter
+    filterset = ZoneFilterSet
     filterset_form = ZoneFilterForm
     table = ZoneTable
 
 
 class ZoneView(generic.ObjectView):
     queryset = Zone.objects.all().prefetch_related(
         "view",
@@ -71,15 +71,15 @@
     default_return_url = "plugins:netbox_dns:zone_list"
 
 
 class ZoneBulkEditView(generic.BulkEditView):
     queryset = Zone.objects.all().prefetch_related(
         "view", "tags", "nameservers", "soa_mname"
     )
-    filterset = ZoneFilter
+    filterset = ZoneFilterSet
     table = ZoneTable
     form = ZoneBulkEditForm
     default_return_url = "plugins:netbox_dns:zone_list"
 
 
 class ZoneBulkDeleteView(generic.BulkDeleteView):
     queryset = Zone.objects.all()
@@ -105,15 +105,15 @@
 
 
 @register_model_view(Zone, "records")
 class ZoneRecordListView(generic.ObjectChildrenView):
     queryset = Zone.objects.all()
     child_model = Record
     table = RecordTable
-    filterset = RecordFilter
+    filterset = RecordFilterSet
     template_name = "netbox_dns/zone/record.html"
     hide_if_empty = True
 
     tab = ViewTab(
         label="Records",
         permission="netbox_dns.view_record",
         badge=lambda obj: obj.record_count(managed=False),
@@ -127,17 +127,17 @@
 
 
 @register_model_view(Zone, "managed_records")
 class ZoneManagedRecordListView(generic.ObjectChildrenView):
     queryset = Zone.objects.all()
     child_model = Record
     table = ManagedRecordTable
-    filterset = RecordFilter
+    filterset = RecordFilterSet
     template_name = "netbox_dns/zone/managed_record.html"
-    actions = ("changelog",)
+    actions = {"changelog": {"view"}}
 
     tab = ViewTab(
         label="Managed Records",
         permission="netbox_dns.view_record",
         badge=lambda obj: obj.record_count(managed=True),
         hide_if_empty=True,
     )
@@ -149,17 +149,16 @@
 
 
 @register_model_view(Zone, "rfc2317_child_zones")
 class ZoneRFC2317ChildZoneListView(generic.ObjectChildrenView):
     queryset = Zone.objects.all()
     child_model = Zone
     table = ZoneTable
-    filterset = ZoneFilter
+    filterset = ZoneFilterSet
     template_name = "netbox_dns/zone/rfc2317_child_zone.html"
-    actions = ("changelog",)
 
     tab = ViewTab(
         label="RFC2317 Child Zones",
         permission="netbox_dns.view_zone",
         badge=lambda obj: obj.rfc2317_child_zone_count(),
         hide_if_empty=True,
     )
```

### Comparing `netbox_plugin_dns-0.22.8/pyproject.toml` & `netbox_plugin_dns-1.0b1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "netbox-plugin-dns"
-version = "0.22.8"
+version = "1.0-beta1"
 description = "NetBox DNS is a NetBox plugin for managing DNS data."
 authors = ["Peter Eckel <pete@netbox-dns.org>"]
 homepage = "https://github.com/peteeckel/netbox-plugin-dns"
 repository = "https://github.com/peteeckel/netbox-plugin-dns"
 license = "MIT"
 readme = "README.md"
 packages = [{include = "netbox_dns"}]
 exclude = ["netbox_dns/tests/*"]
 keywords = ["netbox", "netbox-plugin", "dns"]
 classifiers = [
-    "Development Status :: 5 - Production/Stable"
+    "Development Status :: 4 - Beta"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.10"
 dnspython = "^2.2.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">7.2.0"
 black = ">24"
 
 [build-system]
```

### Comparing `netbox_plugin_dns-0.22.8/PKG-INFO` & `netbox_plugin_dns-1.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: netbox-plugin-dns
-Version: 0.22.8
+Version: 1.0b1
 Summary: NetBox DNS is a NetBox plugin for managing DNS data.
 Home-page: https://github.com/peteeckel/netbox-plugin-dns
 License: MIT
 Keywords: netbox,netbox-plugin,dns
 Author: Peter Eckel
 Author-email: pete@netbox-dns.org
-Requires-Python: >=3.8,<4.0
-Classifier: Development Status :: 5 - Production/Stable
+Requires-Python: >=3.10,<4.0
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: dnspython (>=2.2.1,<3.0.0)
 Project-URL: Repository, https://github.com/peteeckel/netbox-plugin-dns
 Description-Content-Type: text/markdown
 
@@ -45,16 +43,16 @@
 * Manage domain registrar and registrant information for domains related to zones
 * Manage RFC2317 reverse zones for IPv4 prefixes with a network mask length longer than 24 bits
 
 NetBox DNS is using the standardized NetBox plugin interface, so it also takes advantage of the NetBox tagging and change log features.
 
 ## Requirements
 
-* NetBox 3.5.0 or higher
-* Python 3.8 or higher
+* NetBox 4.0.0 or higher
+* Python 3.10 or higher
 
 ## Installation & Configuration
 
 ### Installation
 
 ```
 $ source /opt/netbox/venv/bin/activate
```

#### html2text {}

```diff
@@ -1,36 +1,34 @@
-Metadata-Version: 2.1 Name: netbox-plugin-dns Version: 0.22.8 Summary: NetBox
+Metadata-Version: 2.1 Name: netbox-plugin-dns Version: 1.0b1 Summary: NetBox
 DNS is a NetBox plugin for managing DNS data. Home-page: https://github.com/
 peteeckel/netbox-plugin-dns License: MIT Keywords: netbox,netbox-plugin,dns
 Author: Peter Eckel Author-email: pete@netbox-dns.org Requires-Python:
->=3.8,<4.0 Classifier: Development Status :: 5 - Production/Stable Classifier:
-License :: OSI Approved :: MIT License Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3.12 Requires-Dist: dnspython
-(>=2.2.1,<3.0.0) Project-URL: Repository, https://github.com/peteeckel/netbox-
-plugin-dns Description-Content-Type: text/markdown # NetBox DNS The NetBox DNS
-plugin enables NetBox to manage operational DNS data such as name servers,
-zones, records and views, as well as registration data for domains. It can
-automate tasks like creating PTR records, generating zone serial numbers, NS
-and SOA records, as well as validate names and values values for resource
-records to ensure zone data is consistent, current and conforming to the
-relevant RFCs.
+>=3.10,<4.0 Classifier: Development Status :: 4 - Beta Classifier: License ::
+OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: dnspython (>=2.2.1,<3.0.0) Project-URL: Repository, https://
+github.com/peteeckel/netbox-plugin-dns Description-Content-Type: text/markdown
+# NetBox DNS The NetBox DNS plugin enables NetBox to manage operational DNS
+data such as name servers, zones, records and views, as well as registration
+data for domains. It can automate tasks like creating PTR records, generating
+zone serial numbers, NS and SOA records, as well as validate names and values
+values for resource records to ensure zone data is consistent, current and
+conforming to the relevant RFCs.
   _[_P_y_P_i_]_[_S_t_a_r_s_ _B_a_d_g_e_]_[_F_o_r_k_s_ _B_a_d_g_e_]_[_I_s_s_u_e_s_ _B_a_d_g_e_]_[_P_u_l_l_ _R_e_q_u_e_s_t_s_ _B_a_d_g_e_]_[_G_i_t_H_u_b
    _c_o_n_t_r_i_b_u_t_o_r_s_]_[_L_i_c_e_n_s_e_ _B_a_d_g_e_]_[_D_o_w_n_l_o_a_d_s_]_[_D_o_w_n_l_o_a_d_s_/_W_e_e_k_]_[_D_o_w_n_l_o_a_d_s_/_M_o_n_t_h_]
 ## Features * Manage name servers, zones and records * Automatically generate
 SOA and NS records for zones * Automatically create and update PTR records for
 IPv4 and IPv6 address records * Organize DNS zones in views for split horizon
 DNS and multi-site deployments * Manage domain registrar and registrant
 information for domains related to zones * Manage RFC2317 reverse zones for
 IPv4 prefixes with a network mask length longer than 24 bits NetBox DNS is
 using the standardized NetBox plugin interface, so it also takes advantage of
-the NetBox tagging and change log features. ## Requirements * NetBox 3.5.0 or
-higher * Python 3.8 or higher ## Installation & Configuration ### Installation
+the NetBox tagging and change log features. ## Requirements * NetBox 4.0.0 or
+higher * Python 3.10 or higher ## Installation & Configuration ### Installation
 ``` $ source /opt/netbox/venv/bin/activate (venv) $ pip install netbox-plugin-
 dns ``` ### NetBox Configuration Add the plugin to the NetBox config. `~/
 netbox/configuration.py` ```python PLUGINS = [ "netbox_dns", ] ``` To
 permanently keep the plugin installed when updating NetBox via `update.sh`: ```
 echo netbox-plugin-dns >> ~/netbox/local_requirements.txt ``` To add the
 required netbox_dns tables to your database run the following command from your
 NetBox directory: ``` ./manage.py migrate ``` Full documentation on using
```

