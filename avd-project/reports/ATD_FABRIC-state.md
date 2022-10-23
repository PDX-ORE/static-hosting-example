
# Validate State Report

**Table of Contents:**

- [Validate State Report](validate-state-report)
  - [Test Results Summary](#test-results-summary)
  - [Failed Test Results Summary](#failed-test-results-summary)
  - [All Test Results](#all-test-results)

## Test Results Summary

### Summary Totals

| Total Tests | Total Tests Passed | Total Tests Failed |
| ----------- | ------------------ | ------------------ |
| 53 | 53 | 0 |

### Summary Totals Devices Under Tests

| DUT | Total Tests | Tests Passed | Tests Failed | Categories Failed |
| --- | ----------- | ------------ | ------------ | ----------------- |
| leaf1 |  20 | 20 | 0 | - |
| leaf2 |  20 | 20 | 0 | - |
| spine1 |  13 | 13 | 0 | - |

### Summary Totals Per Category

| Test Category | Total Tests | Tests Passed | Tests Failed |
| ------------- | ----------- | ------------ | ------------ |
| NTP |  3 | 3 | 0 |
| Interface State |  15 | 15 | 0 |
| LLDP Topology |  4 | 4 | 0 |
| IP Reachability |  4 | 4 | 0 |
| BGP |  11 | 11 | 0 |
| Routing Table |  10 | 10 | 0 |
| Loopback0 Reachability |  6 | 6 | 0 |

## Failed Test Results Summary

| Test ID | Node | Test Category | Test Description | Test | Test Result | Failure Reason |
| ------- | ---- | ------------- | ---------------- | ---- | ----------- | -------------- |

## All Test Results

| Test ID | Node | Test Category | Test Description | Test | Test Result | Failure Reason |
| ------- | ---- | ------------- | ---------------- | ---- | ----------- | -------------- |
| 1 | leaf1 | NTP | Synchronised with NTP server | NTP | PASS | - |
| 2 | leaf2 | NTP | Synchronised with NTP server | NTP | PASS | - |
| 3 | spine1 | NTP | Synchronised with NTP server | NTP | PASS | - |
| 4 | leaf1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet1 - P2P_LINK_TO_SPINE1_Ethernet1 | PASS | - |
| 5 | leaf2 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet1 - P2P_LINK_TO_SPINE1_Ethernet2 | PASS | - |
| 6 | spine1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet1 - P2P_LINK_TO_LEAF1_Ethernet1 | PASS | - |
| 7 | spine1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet2 - P2P_LINK_TO_LEAF2_Ethernet1 | PASS | - |
| 8 | leaf1 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan110 - Tenant_A_OP_Zone_1 | PASS | - |
| 9 | leaf2 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan110 - Tenant_A_OP_Zone_1 | PASS | - |
| 10 | leaf1 | Interface State | Vxlan Interface Status & Line Protocol == "up" | Vxlan1 | PASS | - |
| 11 | leaf2 | Interface State | Vxlan Interface Status & Line Protocol == "up" | Vxlan1 | PASS | - |
| 12 | leaf1 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback0 - EVPN_Overlay_Peering | PASS | - |
| 13 | leaf1 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback1 - VTEP_VXLAN_Tunnel_Source | PASS | - |
| 14 | leaf1 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback100 - Tenant_A_OP_Zone_VTEP_DIAGNOSTICS | PASS | - |
| 15 | leaf2 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback0 - EVPN_Overlay_Peering | PASS | - |
| 16 | leaf2 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback1 - VTEP_VXLAN_Tunnel_Source | PASS | - |
| 17 | leaf2 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback100 - Tenant_A_OP_Zone_VTEP_DIAGNOSTICS | PASS | - |
| 18 | spine1 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback0 - EVPN_Overlay_Peering | PASS | - |
| 19 | leaf1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet1 - remote: spine1_Ethernet1 | PASS | - |
| 20 | leaf2 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet1 - remote: spine1_Ethernet2 | PASS | - |
| 21 | spine1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet1 - remote: leaf1_Ethernet1 | PASS | - |
| 22 | spine1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet2 - remote: leaf2_Ethernet1 | PASS | - |
| 23 | leaf1 | IP Reachability | ip reachability test p2p links | Source: leaf1_Ethernet1 - Destination: spine1_Ethernet1 | PASS | - |
| 24 | leaf2 | IP Reachability | ip reachability test p2p links | Source: leaf2_Ethernet1 - Destination: spine1_Ethernet2 | PASS | - |
| 25 | spine1 | IP Reachability | ip reachability test p2p links | Source: spine1_Ethernet1 - Destination: leaf1_Ethernet1 | PASS | - |
| 26 | spine1 | IP Reachability | ip reachability test p2p links | Source: spine1_Ethernet2 - Destination: leaf2_Ethernet1 | PASS | - |
| 27 | leaf1 | BGP | ArBGP is configured and operating | ArBGP | PASS | - |
| 28 | leaf2 | BGP | ArBGP is configured and operating | ArBGP | PASS | - |
| 29 | spine1 | BGP | ArBGP is configured and operating | ArBGP | PASS | - |
| 30 | leaf1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.30.255.0 | PASS | - |
| 31 | leaf2 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.30.255.2 | PASS | - |
| 32 | spine1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.30.255.1 | PASS | - |
| 33 | spine1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.30.255.3 | PASS | - |
| 34 | leaf1 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 192.0.255.1 | PASS | - |
| 35 | leaf2 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 192.0.255.1 | PASS | - |
| 36 | spine1 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 192.0.255.3 | PASS | - |
| 37 | spine1 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 192.0.255.4 | PASS | - |
| 38 | leaf1 | Routing Table | Remote VTEP address | 192.0.254.3 | PASS | - |
| 39 | leaf1 | Routing Table | Remote VTEP address | 192.0.254.4 | PASS | - |
| 40 | leaf2 | Routing Table | Remote VTEP address | 192.0.254.3 | PASS | - |
| 41 | leaf2 | Routing Table | Remote VTEP address | 192.0.254.4 | PASS | - |
| 42 | leaf1 | Routing Table | Remote Lo0 address | 192.0.255.3 | PASS | - |
| 43 | leaf1 | Routing Table | Remote Lo0 address | 192.0.255.4 | PASS | - |
| 44 | leaf1 | Routing Table | Remote Lo0 address | 192.0.255.1 | PASS | - |
| 45 | leaf2 | Routing Table | Remote Lo0 address | 192.0.255.3 | PASS | - |
| 46 | leaf2 | Routing Table | Remote Lo0 address | 192.0.255.4 | PASS | - |
| 47 | leaf2 | Routing Table | Remote Lo0 address | 192.0.255.1 | PASS | - |
| 48 | leaf1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf1 - 192.0.255.3 Destination: 192.0.255.3 | PASS | - |
| 49 | leaf1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf1 - 192.0.255.3 Destination: 192.0.255.4 | PASS | - |
| 50 | leaf1 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf1 - 192.0.255.3 Destination: 192.0.255.1 | PASS | - |
| 51 | leaf2 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf2 - 192.0.255.4 Destination: 192.0.255.3 | PASS | - |
| 52 | leaf2 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf2 - 192.0.255.4 Destination: 192.0.255.4 | PASS | - |
| 53 | leaf2 | Loopback0 Reachability | Loopback0 Reachability | Source: leaf2 - 192.0.255.4 Destination: 192.0.255.1 | PASS | - |
