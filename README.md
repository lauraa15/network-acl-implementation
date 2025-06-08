Network Security: Standard ACL Implementation
Task 2 - Week 1 Cyber Bootcamp
Objective:
Demonstrate basic network segmentation using Standard ACLs to block a specific subnet (192.168.10.0/24) from accessing servers while allowing another subnet (192.168.20.0/28).

Key Steps:
1. Created Standard ACL on Cisco router:
  - access-list 1 deny 192.168.10.0 0.0.0.255
  - access-list 1 permit any

2. Applied ACL inbound on the server-facing interface (FastEthernet6/0).

Verification:
- Confirmed blocked traffic from PC subnet (show ip access-lists showed matches).
- Laptop subnet retained server access.

Tools: Cisco Packet Tracer

Conclusion: Successfully implemented basic traffic control between subnets using Standard ACLs.
