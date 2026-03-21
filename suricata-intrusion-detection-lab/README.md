# Network Intrusion Detection Lab (Suricata)

## Overview
This project demonstrates my skills in the use of Suricata IDS to analyze network traffic, create custom detection rules, and investigate alerts from PCAP data.

## Tools Used
- Suricata
- Wireshark
- jq
- Kali Linux

## Custom Rule
```bash
alert http $HOME_NET any -> $EXTERNAL_NET any (msg:"GET on wire"; flow:established,to_server; content:"GET"; http_method; sid:12345; rev:3;)

## Findings
- The custom Suricata rule successfully detected HTTP GET requests from internal to external network traffic  
- Alerts were generated with the signature "GET on wire," confirming proper rule configuration and execution  
- Log analysis revealed key network details such as source IP, destination IP, protocol (TCP), and HTTP request behavior  
- JSON output (eve.json) provided structured data for deeper analysis, including HTTP metadata and flow information  
- The use of jq enabled efficient extraction of relevant fields, improving readability and analysis of log data  
