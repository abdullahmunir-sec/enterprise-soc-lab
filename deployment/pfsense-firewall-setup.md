# pfSense Firewall Deployment

A pfSense firewall was deployed to control routing between segmented networks and simulate an enterprise perimeter firewall.

## Network Interfaces

- WAN – Connected to external / simulated internet network
- LAN – Internal network (192.168.1.0/24)
- OPT1 – Attacker network (192.168.3.0/24)
- OPT2 – SIEM network (192.168.5.0/24)
- OPT3 – Management network (192.168.114.0/24)

## Role in the SOC Architecture

The firewall is responsible for:
- Routing traffic between network segments
- Enforcing network isolation
- Providing a point for traffic mirroring toward Security Onion

## Interface Mapping

The pfSense firewall was configured with multiple virtual network interfaces to support network segmentation:

- **em0** – WAN / External network
- **em1** – Internal LAN (192.168.1.254/24)
- **em2** – SPAN / Monitoring interface for Security Onion
- **em3** – Attacker network (192.168.3.254/24)
- **em4** – Security Onion / Management network (192.168.4.254/24)
- **em5** – SIEM network (192.168.5.254/24)

Each interface was assigned a dedicated subnet to simulate a real enterprise firewall deployment with isolated security zones.
