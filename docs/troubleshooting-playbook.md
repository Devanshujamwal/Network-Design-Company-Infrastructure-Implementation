# Network Troubleshooting Playbook

A repeatable workflow for diagnosing connectivity issues in a routed lab environment.

## 1. Define the scope

Determine whether the problem affects:

- one host;
- one VLAN/subnet;
- one site;
- or communication between multiple sites.

## 2. Validate host configuration

Check:

- IPv4/IPv6 address
- subnet mask/prefix
- default gateway
- DNS configuration

## 3. Check local connectivity

Verify the host can reach its default gateway before troubleshooting remote routing or services.

## 4. Check switching and VLANs

Confirm:

- access-port assignment
- VLAN existence
- trunk expectations
- interface state

## 5. Check routing

Review:

- directly connected networks
- learned routes
- OSPF adjacency/route information where applicable
- next-hop reachability

## 6. Check services

If basic routing works, move to DHCP, DNS, NAT, or application-specific checks.

## 7. Retest after one change

Make one controlled change at a time and repeat the same connectivity test. This makes the effect of each change clear.

## Documentation review

The Site 3 report contains an interface/gateway inconsistency. The portfolio treats it as a documentation discrepancy requiring comparison with the running configuration, rather than assuming a live network fault.
