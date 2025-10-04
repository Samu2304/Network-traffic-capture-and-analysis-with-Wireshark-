# Network-traffic-capture-and-analysis-with-Wireshark
## AIM:
To capture and analyze network traffic using Wireshark in order to observe protocols, packets, and potential anomalies.
## Requirements:
- **Hardware:**
    - Computer with internet access
    - Network adapter (Ethernet/Wi-Fi)
- **Software:**
    - Wireshark (latest stable version)
    - Sample PCAP files (optional for offline analysis)
## Architecture:
```mermaid
flowchart TD
    A[Network Interface Card] --> B[Wireshark Packet Capture Engine]
    B --> C[Packet Decoder & Protocol Analyzer]
    C --> D[Packet Display & Filtering Interface]
    D --> E[Investigator Analyzes Network Data]
    E --> F[Findings: IPs, Ports, Protocols, Anomalies]
```
## DESIGN STEPS:
### Step 1:
Install Wireshark on the system.

### Step 2:
Launch Wireshark and select the network interface (Ethernet/Wi-Fi).

### Step 3:
Start the capture, apply filters (like http, tcp, ip.addr == x.x.x.x) to analyze specific traffic, and stop the capture after observing relevant data.
### Step 4:
**Analyze traffic to identify:**
  - Source & Destination IP addresses
  - Protocols (HTTP, DNS, TCP, UDP, etc.)
  - Suspicious activities (e.g., unusual ports, repeated requests).
## PROGRAM:
Wireshark Packet Capture and Filter Usage

1. Open Wireshark and Select a Network Interface
• Launch Wireshark. • Select an active interface (like Wi-Fi or Ethernet) to start capturing packets.

![WhatsApp Image 2025-10-04 at 11 21 56_947e9563](https://github.com/user-attachments/assets/70fbc780-a387-44ac-9611-4a98fffef0de)


2. Start Capturing Packets
• Click the blue shark fin icon or double-click the interface. • Wireshark will start capturing all real-time traffic.

![WhatsApp Image 2025-10-04 at 11 20 20_000bb5b0](https://github.com/user-attachments/assets/3bd00f7a-54e9-47db-ba0c-57c6f8a9b310)


3. Apply Filters to Focus on Specific Traffic
• Use filters like http, ip.addr == 192.168.1.1, or tcp.port == 80 in the top filter bar to narrow down results.

![WhatsApp Image 2025-10-04 at 11 24 43_428cca99](https://github.com/user-attachments/assets/05ed4224-8006-4d25-ab35-a92abb973fc2)


4. Analyze Packet Details
• Click on a packet to view its detailed breakdown including frame, Ethernet, IP, TCP/UDP layers, and data payload.

![WhatsApp Image 2025-10-04 at 11 26 25_0c745e10](https://github.com/user-attachments/assets/3e7536a3-7076-4c60-979e-bdca697ab613)


5. Export or Save the Capture
• Go to File > Save As to store the capture in .pcap format for future analysis.

![WhatsApp Image 2025-10-04 at 11 27 59_80710394](https://github.com/user-attachments/assets/7369f32d-eb21-43ff-af80-c53c2ff3f5df)


## OUTPUT:
Captured Packets with Protocol Analysis and Detailed Packet Info

## RESULT:
Network traffic was successfully captured and analyzed using Wireshark.
