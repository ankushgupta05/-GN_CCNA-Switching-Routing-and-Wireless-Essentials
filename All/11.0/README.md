Here are the answers to your **11.6.4 Module Quiz - Switch Security Configuration** with explanations:

---

### Question 1

**What is a recommended best practice when dealing with the native VLAN?**

* ⬜ Turn off DTP.
* ⬜ Use port security.
* ✅ **Assign it to an unused VLAN.**
* ⬜ Assign the same VLAN number as the management VLAN.

**Explanation:**
Assigning the native VLAN to an unused VLAN reduces the risk of VLAN hopping attacks.

---

### Question 2

**On what switch ports should PortFast be enabled to enhance STP stability?**

* ✅ **All end-user ports**
* ⬜ Only ports that attach to a neighboring switch
* ⬜ All trunk ports that are not root ports
* ⬜ Only ports that are elected as designated ports

**Explanation:**
PortFast should be enabled on ports connected to end devices to avoid STP delays.

---

### Question 3

**Which command would be best to use on an unused switch port if a company adheres to the best practices as recommended by Cisco?**

* ✅ **shutdown**
* ⬜ ip dhcp snooping
* ⬜ switchport port-security mac-address sticky
* ⬜ switchport port-security violation shutdown
* ⬜ switchport port-security mac-address sticky mac-address

**Explanation:**
Best practice is to administratively shut down unused ports.

---

### Question 4

**Which two features on a Cisco Catalyst switch can be used to mitigate DHCP starvation and DHCP spoofing attacks? (Choose two.)**

* ✅ **Port security**
* ⬜ Extended ACL
* ✅ **DHCP snooping**
* ⬜ DHCP server failover
* ⬜ Strong password on DHCP servers

**Explanation:**
Port security limits MAC addresses, DHCP snooping validates DHCP messages, both mitigate DHCP attacks.

---

### Question 5

**What is the best way to prevent a VLAN hopping attack?**

* ⬜ Disable STP on all nontrunk ports.
* ⬜ Use ISL encapsulation on all trunk links.
* ⬜ Use VLAN 1 as the native VLAN on trunk ports.
* ✅ **Disable trunk negotiation for trunk ports and statically set nontrunk ports as access ports.**

**Explanation:**
Disabling DTP and manually configuring trunk ports prevent VLAN hopping.

---

### Question 6

**Which procedure is recommended to mitigate the chances of ARP spoofing?**

* ⬜ Enable port security globally.
* ✅ **Enable DHCP snooping on selected VLANs.**
* ⬜ Enable DAI on the management VLAN.
* ⬜ Enable IP Source Guard on trusted ports.

**Explanation:**
DHCP snooping works with DAI to help prevent ARP spoofing by validating DHCP info.

---

### Question 7

**What are two types of switch ports that are used on Cisco switches as part of the defense against DHCP spoofing attacks? (Choose two.)**

* ⬜ Unknown port
* ✅ **Untrusted port**
* ⬜ Unauthorized port
* ✅ **Trusted DHCP port**
* ⬜ Authorized DHCP port
* ⬜ Established DHCP port

**Explanation:**
Trusted ports allow DHCP servers, untrusted ports do not, protecting against rogue DHCP servers.

---

### Question 8

**Which two commands can be used to enable PortFast on a switch? (Choose two.)**

* ✅ **S1(config-if)# spanning-tree portfast**
* ⬜ S1(config-line)# spanning-tree portfast
* ✅ **S1(config)# spanning-tree portfast default**
* ⬜ S1(config-if)# enable spanning-tree portfast
* ⬜ S1(config)# enable spanning-tree portfast default

**Explanation:**
`spanning-tree portfast` on interface config enables it on one port; `spanning-tree portfast default` enables it globally.

---

### Question 9

**An administrator who is troubleshooting connectivity issues on a switch notices that a switch port configured for port security is in the err-disabled state. After verifying the cause of the violation, how should the administrator re-enable the port without disrupting network operation?**

* ⬜ Reboot the switch.
* ✅ **Issue the shutdown command followed by the no shutdown command on the interface.**
* ⬜ Issue the no switchport port-security command, then re-enable port security.
* ⬜ Issue the no switchport port-security violation shutdown command on the interface.

**Explanation:**
Shutting down and bringing the interface back up resets the err-disabled state.

---

### Question 10

**A network administrator is configuring DHCP snooping on a switch. Which configuration command should be used first?**

* ⬜ ip dhcp snooping
* ✅ **ip dhcp snooping vlan**
* ⬜ ip dhcp snooping trust
* ⬜ ip dhcp snooping limit rate

**Explanation:**
First, specify which VLANs DHCP snooping applies to.

---

### Question 11

**A network administrator is configuring DAI on a switch with the command ip arp inspection validate dst-mac. What is the purpose of this configuration command?**

* ⬜ To check the destination MAC address in the Ethernet header against the MAC address table
* ⬜ To check the destination MAC address in the Ethernet header against the user-configured ARP ACLs
* ✅ **To check the destination MAC address in the Ethernet header against the target MAC address in the ARP body**
* ⬜ To check the destination MAC address in the Ethernet header against the source MAC address in the ARP body

**Explanation:**
Validates that the destination MAC in Ethernet header matches the target MAC in ARP.

---

### Question 12

**Which security feature should be enabled in order to prevent an attacker from overflowing the MAC address table of a switch?**

* ⬜ BPDU filter
* ✅ **Port security**
* ⬜ Storm control
* ⬜ Root guard

**Explanation:**
Port security limits number of MAC addresses per port preventing MAC flooding.

---

### Question 13

**What Layer 2 attack is mitigated by disabling Dynamic Trunking Protocol?**

* ✅ **VLAN hopping**
* ⬜ DHCP spoofing
* ⬜ ARP poisoning
* ⬜ ARP spoofing

**Explanation:**
Disabling DTP prevents unauthorized trunk formation, blocking VLAN hopping.

---

### Question 14

**A network administrator is configuring DAI on a switch. Which command should be used on the uplink interface that connects to a router?**

* ⬜ ip arp inspection vlan
* ✅ **ip arp inspection trust**
* ⬜ ip dhcp snooping
* ⬜ spanning-tree portfast

**Explanation:**
The uplink interface to a trusted device (router) must be trusted by DAI.

---

### Question 15

**Where are dynamically learned MAC addresses stored when sticky learning is enabled with the switchport port-security mac-address sticky command?**

* ⬜ ROM
* ⬜ RAM
* ✅ **NVRAM**
* ⬜ Flash

**Explanation:**
Sticky MAC addresses are saved in **NVRAM** to persist across reboots.

---

Let me know if you want me to put these answers in a table or provide more detailed explanations!
