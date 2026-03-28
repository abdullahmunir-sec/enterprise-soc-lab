# Security Onion Deployment

Security Onion was deployed as the primary network monitoring and intrusion detection platform within the enterprise SOC lab.

## Deployment Details

- Platform: Security Onion
- Role: Network Security Monitoring (NSM) and Intrusion Detection
- Interfaces:
  - Management Interface – Accessible via web UI
  - Monitoring Interface – Connected to mirrored/SPAN traffic

## Access

The Security Onion web interface is accessible over HTTPS from the management network and provides:

- Alerts and event dashboards
- Network traffic analysis
- Integration with IDS and log pipelines

## Integrated Security Tools

The deployment includes the following components:

- **Suricata** for network intrusion detection
- **Zeek** for network traffic analysis
- **Elastic Stack** for log storage and visualization
- **Fleet / Agents** for host monitoring capabilities
