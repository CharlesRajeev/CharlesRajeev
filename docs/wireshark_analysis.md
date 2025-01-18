# Wireshark Analysis Report

## Overview
This report details the network traffic analysis performed using Wireshark. The goal was to capture and analyze network traffic while browsing to identify protocols like HTTP, DNS, TCP/UDP.

## Key Activities

### 1. Capture Network Traffic
- **Capture Setup**:
  - Open Wireshark and select the appropriate network interface.
  - Start capturing packets.
  - Perform network activities (e.g., browsing the web).
  - Stop the capture.

### 2. Analyze Captured Traffic
- **Filter by Protocol**:
  - Apply filters to focus on specific protocols:
    - HTTP: `http`
    - DNS: `dns`
    - TCP: `tcp`
    - UDP: `udp`
- **Identify Traffic Patterns**:
  - Examine the packets to understand the flow of data.
  - Look for any unusual or suspicious traffic.

## Screenshots and Analysis
### HTTP Traffic
![HTTP Traffic](../assets/screenshots/wireshark_http.png)
- **Observations**:
  - Identified HTTP requests and responses.
  - Analyzed the HTTP methods (GET, POST) and response codes.

### DNS Traffic
![DNS Traffic](../assets/screenshots/wireshark_dns.png)
- **Observations**:
  - Identified DNS queries and responses.
  - Analyzed the DNS query types (A, AAAA, MX) and response times.

### TCP Traffic
![TCP Traffic](../assets/screenshots/wireshark_tcp.png)
- **Observations**:
  - Analyzed TCP handshakes (SYN, SYN-ACK, ACK).
  - Looked for retransmissions and window sizes.

### UDP Traffic
![UDP Traffic](../assets/screenshots/wireshark_udp.png)
- **Observations**:
  - Identified UDP packets and their sources/destinations.
  - Analyzed the payload and packet loss.

