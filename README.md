**NetAssist — Network Troubleshooting Lab**



**Overview**



NetAssist is a hands-on networking project focused on building a virtual network, diagnosing connectivity failures, and documenting troubleshooting procedures.



**Tools Used**



* Cisco Packet Tracer
* Wireshark 4.6.9
* Npcap
* Ubuntu 24.04 on WSL 2



**Project Structure**



* network-topology/ — Baseline and scenario Packet Tracer files
* test-scenarios/ — Test scenario resources
* packet-captures/ — Saved network packet captures
* screenshots/ — Evidence of tests and recovery
* documentation/ — Troubleshooting log and findings
* scripts/ — Supporting scripts



**Network Troubleshooting Scenarios**



* Incorrect destination IP address
* Disconnected network cable
* Devices configured on different IP subnets
* Administratively disabled switch port



Each scenario was tested by introducing a fault, checking connectivity, correcting the fault, and verifying recovery.



**Wireshark Analysis**



Captured live traffic on the Windows Wi-Fi interface and used the icmp display filter to identify ICMP Echo requests and replies during a ping test to 1.1.1.1.



Capture file: packet-captures/netassist-icmp-capture.pcapng



**Linux Network Checks**



**Using Ubuntu 24.04 under WSL 2, performed:**



* Interface and IP address inspection with ip addr
* External connectivity testing with ping
* DNS resolution testing with getent hosts
* Routing table inspection with ip route



**Results**



* Verified connectivity recovery across four simulated network fault scenarios.
* Captured and identified ICMP traffic with Wireshark.
* Verified Linux interface configuration, external connectivity, DNS resolution, and routing.



**Documentation**



Detailed test observations and results are recorded in documentation/troubleshooting-log.txt.

