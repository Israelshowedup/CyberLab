# CyberLab

A personal cybersecurity lab showcasing hands-on projects in networking, scanning, and SIEM-based security monitoring.
### 🔹 Network Intrusion Detection Lab (Suricata)
- Analyzed network traffic using Suricata IDS and custom detection rules  
- Generated and investigated alert logs (fast.log, eve.json)  
- Parsed JSON data using jq to extract key network information  
- [View Project](./suricata-intrusion-detection-lab)

### Wireshark Network Traffic Analysis

- Analyzed network traffic using Wireshark to inspect packets and identify communication patterns  
- Applied filters such as `ip.addr`, `tcp.port`, and `tcp contains "curl"` to isolate relevant traffic  
- Examined TCP, DNS, and HTTP protocols, including ports, sequence numbers, and payload data  
- Identified internal vs external communication and analyzed request/response behavior  

Folder:[View Projec](./wireshark-network-traffic-analysis)

## Projects

### 🔹 Splunk Endpoint Authentication Monitoring (SIEM)
- Ingested Windows Security Event Logs into Splunk
- Built SPL queries to detect failed login attempts (EventCode 4625)
- Created dashboards to monitor endpoint authentication activity

Folder: `Splunk-Endpoint-Authentication-Monitoring`

### 🔹 Local Port Scanner (Python | Nmap)
- Developed a Python-based port scanner to identify open TCP ports and running services
- Automated host and service detection for approved lab environments

Folder: `local-port-scanner`

