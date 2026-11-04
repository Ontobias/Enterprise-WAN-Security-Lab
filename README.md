# Enterprise-WAN-Security-Lab
Designed and deployed a full-scale enterprise network in Cisco Packet Tracer featuring Layer 3 switching, IPsec Site-to-Site VPNs, Zone-Based Firewalls (ZBF), and centralized network management (Syslog/TFTP/SSH).
# Enterprise Multi-Branch WAN & Security Lab

## 📖 Project Overview
This repository contains the complete configuration and documentation for a simulated enterprise network connecting a Headquarters (HQ) to two remote Branch offices. 

The objective was to design a scalable, highly available, and secure network architecture using Cisco IOS in Packet Tracer. The topology utilizes a standard Core/Distribution/Access model where VLAN routing is handled by Layer 3 Multilayer Switches (3560s), while edge routers manage WAN connectivity, NAT, and encrypted Site-to-Site VPN tunnels.

## 🖼️ Network Topology
<img width="1728" height="1117" alt="Screenshot 2026-11-04 at 2 12 56 AM" src="https://github.com/user-attachments/assets/9db565b5-bb73-41c5-90cc-c22a937ff0ed" />
<img width="1728" height="1117" alt="Screenshot 2026-11-04 at 2 21 55 AM" src="https://github.com/user-attachments/assets/c680843e-984f-4d1e-a04c-66afb00c1fb5" />
<img width="1728" height="1117" alt="Screenshot 2026-11-04 at 2 18 29 AM" src="https://github.com/user-attachments/assets/685ec619-3cc6-45d4-a5a8-68f7c29e558c" />
<img width="1728" height="1117" alt="Screenshot 2026-11-04 at 2 17 32 AM" src="https://github.com/user-attachments/assets/65680e03-9279-46d1-8f6b-56318e48c2e4" />
<img width="1728" height="1117" alt="Screenshot 2026-11-04 at 2 15 56 AM" src="https://github.com/user-attachments/assets/db73b396-33c4-48f0-b1bd-173795263fe1" />
<img width="1728" height="1117" alt="Screenshot 2026-11-04 at 2 14 19 AM" src="https://github.com/user-attachments/assets/5a1def8b-3683-4a09-8c64-cbfc690b6e7f" />
<img width="1728" height="1117" alt="Screenshot 2026-11-04 at 2 12 48 AM" src="https://github.com/user-attachments/assets/16b9fbca-001d-402a-be7e-6c132b2369ff" />
<img width="1728" height="1117" alt="Screenshot 2026-11-04 at 2 10 23 AM" src="https://github.com/user-attachments/assets/92b2badb-6ee1-41d9-b154-c7a08c19e1cd" />
<img width="1728" height="1117" alt="Screenshot 2026-11-04 at 2 10 13 AM" src="https://github.com/user-attachments/assets/93c40343-c37d-4b16-b849-58bcfafec503" />
<img width="1728" height="1117" alt="Screenshot 2026-11-04 at 2 10 11 AM" src="https://github.com/user-attachments/assets/80e16f72-8654-4332-b6da-55130b221b24" />
<img width="1728" height="1117" alt="Screenshot 2026-11-04 at 2 10 20 AM" src="https://github.com/user-attachments/assets/ee8ef6b2-5a2e-431b-a93c-dbb032471b8f" />
<img width="1728" height="1117" alt="Screenshot 2026-11-04 at 2 10 07 AM" src="https://github.com/user-attachments/assets/4046b420-bb98-4a3d-868e-1aaef186c247" />
<img width="1728" height="1117" alt="Screenshot 2026-11-04 at 2 09 57 AM" src="https://github.com/user-attachments/assets/c8411fbb-1d72-42f0-9712-b122358cff5b" />
<img width="1728" height="1117" alt="Screenshot 2026-11-04 at 2 09 51 AM" src="https://github.com/user-attachments/assets/e6c63154-afee-4b18-aa4d-af510c33513e" />
<img width="1728" height="1117" alt="Screenshot 2026-11-04 at 2 09 46 AM" src="https://github.com/user-attachments/assets/de586395-282a-4f30-96e9-989d914f6fc6" />
<img width="1728" height="1117" alt="Screenshot 2026-11-04 at 2 09 42 AM" src="https://github.com/user-attachments/assets/e7f20a9c-6c8f-43a2-8e82-67bb8b3ba2f1" />
<img width="1728" height="1117" alt="Screenshot 2026-11-04 at 2 09 38 AM" src="https://github.com/user-attachments/assets/ef5f8b8d-9840-438c-b190-1648a2aa702f" />
<img width="1728" height="1117" alt="Screenshot 2026-11-04 at 2 09 31 AM" src="https://github.com/user-attachments/assets/3e29423c-42e4-444a-ad72-cbe51d57a990" />
<img width="1728" height="1117" alt="Screenshot 2026-11-04 at 2 09 19 AM" src="https://github.com/user-attachments/assets/9b03f423-2e39-4ccf-b2c5-4cb7090d7409" />
<img width="1728" height="1117" alt="Screenshot 2026-11-04 at 2 07 49 AM" src="https://github.com/user-attachments/assets/c66684ed-a413-46ab-8d51-73d2c500f118" />
<img width="1728" height="1117" alt="Screenshot 2026-11-04 at 2 07 40 AM" src="https://github.com/user-attachments/assets/e62e1df3-a217-469d-a0b2-776c11fdeaec" />
<img width="1728" height="1117" alt="Screenshot 2026-11-04 at 2 07 31 AM" src="https://github.com/user-attachments/assets/1e37e634-d8aa-49df-9372-862942d9a144" />

## 🛠️ Technologies & Features Implemented
*   *Routing & Switching:* Layer 3 Switching (SVIs), Router-on-a-Stick, Rapid Spanning Tree Protocol (RSTP), 802.1Q Trunking.
*   *WAN & Edge:* Point-to-Point ⁠ /30 ⁠ links, Static Routing, NAT (PAT) for internet access.
*   *Security:* 
    *   Site-to-Site IPsec VPN (IKEv1, AES, SHA) for encrypted cross-site traffic.
    *   Zone-Based Policy Firewall (ZBF) at the HQ edge.
    *   Department-level ACLs (Restricting HR and Accounting data).
    *   Port Security (Sticky MAC) on all access switches.
*   *Management:* SSH for secure remote access, Syslog for centralized logging, TFTP for configuration backups

## 📊 IP Addressing Scheme
| Site | VLAN 10 (MGMT) | VLAN 20 (Sales) | VLAN 30 (HR) | VLAN 40 (IT) | VLAN 50 (Account) |
| :--- | :--- | :--- | :--- | :--- | :--- |
| *HQ* | 192.168.10.0/24 | 192.168.20.0/24 | 192.168.30.0/24 | 192.168.40.0/24 | 192.168.50.0/24 |
| *Branch 1* | 172.16.10.0/24 | 172.16.20.0/24 | 172.16.30.0/24 | 172.16.40.0/24 | 172.16.50.0/24 |
| *Branch 2* | 172.17.10.0/24 | 172.17.20.0/24 | 172.17.30.0/24 | 172.17.40.0/24 | 172.17.50.0/24 |

## 🚧 Troubleshooting Log (Real-World Challenges)
During the deployment, I encountered and resolved several complex networking issues:

1.⁠ ⁠*Routing Loop Blackhole:* PCs could not ping remote WAN IPs. Resolution: Audited the routing table and removed a static route that pointed the HQ router to its own IP address.
2.⁠ ⁠*VPN Phase 1 & 2 Failures:* The IPsec tunnel would not establish. Resolution: Discovered mismatched Pre-Shared Keys (PSK) between peers and forced the IPsec transform-set into memory after a Packet Tracer syntax rejection.
3.⁠ ⁠*DHCP APIPA Failures:* Sales PCs received 169.254.x.x addresses. Resolution: Corrected misconfigured access switch ports that were left in the default VLAN 1 instead of the Sales VLAN.
4.⁠ ⁠*Firewall Verification:* After configuring ZBF, the ISP could still ping the HQ router's WAN IP. Resolution: Proved the firewall was working by pinging an internal L3 switch (which failed with 0% success), confirming stateful traffic inspection was blocking outside-to-inside access.

## 🚀 How to Use This Repository
1.⁠ ⁠Download the ⁠ .pkt ⁠ file (if you upload the actual Packet Tracer file).
2.⁠ ⁠Open the ⁠ /Configurations ⁠ folder to view the raw CLI configurations for any specific device.
3.⁠ ⁠Check the ⁠ /Images ⁠ folder for verification screenshots (VPN status, firewall tests, Syslog).

How to view the configurations: Download the .pkt file and open it in Cisco Packet Tracer. Use the CLI to view the running-config on each device.****


******************
•⁠  ⁠Author: OSCAR TOBIAS                             
•⁠  ⁠Project: Enterprise WAN & Security Lab           
•⁠  ⁠Date: 4/11/2026                            
******************
#
