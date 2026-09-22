# Network Architecture Notes

This document expands the conceptual design behind the multi-site Packet Tracer project.

## Logical topology

```text
                 Inter-site routing
                        |
        +---------------+---------------+
        |               |               |
        v               v               v
   Calgary (HQ)      Red Deer        Edmonton
        |               |               |
    Switching         Switching        Switching
        |               |               |
    Endpoints         Endpoints        Endpoints
```

## Design principles

### Addressing
The project uses structured IPv4 addressing and IPv6 documentation so each site can be identified and routed consistently.

### Subnetting
VLSM is used to divide larger address space into networks sized for different LAN requirements.

### Switching
Local switching and VLAN concepts provide segmentation inside each site.

### Routing
OSPF is part of the broader routed design and provides a scalable way to exchange routes between network segments/sites in the lab.

### Network services
The project also covers common infrastructure services and concepts including DHCP, NAT, and DNS.

## Site 3 contribution

My documented contribution focused on Site 3 IPv4/IPv6 addressing and network documentation, including subnet and gateway planning.

## Evidence boundary

The original Packet Tracer file and project PDFs are preserved in the repository. This documentation does not invent CLI output or configurations that are not preserved in those source files.
