# Ubuntu Server – SIEM Host

An Ubuntu Server virtual machine was deployed to host Splunk Enterprise for centralized log collection and analysis.

## Configuration

- OS: Ubuntu Server
- Network: SIEM segment (192.168.5.0/24)
- Purpose: Aggregate and analyze logs from endpoints and security tools.

## Planned Components

- Splunk Enterprise for log ingestion and search
- Syslog forwarding from pfSense
- Endpoint telemetry from Windows systems
