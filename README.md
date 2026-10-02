# Multi-Tier LAN Topology & Packet Analysis in Cisco Packet Tracer

## 📌 Project Overview
Designed, configured, and tested a multi-tier local area network (LAN) connecting 9 end-user workstations and 2 local servers across 4 Cisco switches using Cisco Packet Tracer. The primary objective was to establish end-to-end Layer 3 connectivity, verify switch port convergence, and inspect ICMP packet encapsulation down to the OSI layer level.

## 🛠️ Network Specifications
• Core & Distribution Switches : 1 Central Switch (Core), 3 Sub-Switches (Access)
• Mail Server IP               : 192.168.1.1
• Web Server IP                : 192.168.1.2
• Workstations IP Range        : 192.168.1.3 to 192.168.1.11 (PC0 to PC8)
• Subnet Mask                  : 255.255.255.0 (Class C /24)
• Cabling Standard             : Straight-Through (Host-to-Switch) & Crossover (Switch-to-Switch)

## 📸 Network Topology Diagram
## 🔬 Technical Implementation & Key Concepts
1. Layer 2 Switching & Spanning Tree Protocol (STP)
   Monitored switch port convergence behavior as links transitioned from Listening/Learning to Forwarding state to prevent Layer 2 switching loops.
   <img width="1600" height="728" alt="network-topology png" src="https://github.com/user-attachments/assets/004024b2-9b4b-4cfa-b19d-6e1c9af708a3" />


3. Static IP Configuration
   Manually assigned static private IPv4 parameters across all end-user workstations and servers to maintain reliable local address allocation.

4. OSI Model Packet Inspection
   Utilized Simulation Mode to trace Protocol Data Units (PDUs) frame-by-frame, observing Layer 2 (Ethernet II MAC headers) and Layer 3 (IP/ICMP headers) encapsulation.
   
## 🧪 Testing & Verification Results
1. ICMP Ping Connectivity Test
Plaintext
COMMAND EXECUTED : ping 192.168.1.1
SOURCE DEVICE    : PC0 (192.168.1.3)
DESTINATION      : Mail Server (192.168.1.1)
RESULT           : 0% Packet Loss, Successful Round-Trip Echo Replies
<img width="825" height="745" alt="icmp-ping-test png" src="https://github.com/user-attachments/assets/ea0de6bd-868a-4a39-b207-af9ee1c6d222" />


3. PDU Simulation & Protocol Verification
PDU FLOW ANALYSIS : Captured and tracked ICMP frame propagation across switches in real-time simulation mode. Confirmed successful frame packaging from Layer 1 through Layer 7.
<img width="869" height="151" alt="pdu-simulation-analysis-and-verification png" src="https://github.com/user-attachments/assets/8115bc72-a779-4924-9447-2ff3d93cd84b" />



## 🚀 How to Run
1. Download and install Cisco Packet Tracer.
2. Clone or download this repository.
3. Open cisco-packet-tracer.pkt in Packet Tracer to inspect or test the network.


   
