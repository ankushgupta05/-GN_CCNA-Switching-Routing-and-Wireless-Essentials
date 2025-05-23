Here are the answers with **all options listed** and the **correct ones clearly indicated** along with brief explanations:

---

### **Question 1**

**How does the host verify that the address is unique and therefore usable?**

* ❌ The host checks the local neighbor cache for the learned address and if the address is not cached, it is considered unique.
* ✅ **The host sends an ICMPv6 neighbor solicitation message to the DHCP or SLAAC-learned address and if no neighbor advertisement is returned, the address is considered unique.**
* ❌ The host sends an ICMPv6 echo request message to the DHCPv6 or SLAAC-learned address and if no reply is returned, the address is considered unique.
* ❌ The host sends an ARP broadcast to the local link and if no hosts send a reply, the address is considered unique.
  **Explanation:** IPv6 uses **Neighbor Solicitation (NS)** and **Neighbor Advertisement (NA)** messages for Duplicate Address Detection (DAD), not ARP or ICMP echo.

---

### **Question 2**

**What is the keyword that is displayed on [www.netacad.com](http://www.netacad.com)?**

* ✅ **Cisco**
* ❌ DHCP
* ❌ IPv6
* ❌ switch
* ❌ networking
* ❌ Router
  **Explanation:** The Packet Tracer activity for this typically displays the word **Cisco** on the website.

---

### **Question 3**

**Match the DHCP message types to the order of the DHCPv4 process:**

* **Step 1** → ✅ **DHCPDISCOVER**
* **Step 2** → ✅ **DHCPOFFER**
* **Step 3** → ✅ **DHCPREQUEST**
* **Step 4** → ✅ **DHCPACK**
  **Explanation:** The four-step DHCP process is commonly remembered as **DORA** (Discover, Offer, Request, Acknowledge).

---

### **Question 4**

**Which statement describes HSRP?**

* ❌ It uses ICMP to allow IPv4 hosts to locate routers that provide IPv4 connectivity to remote IP networks.
* ❌ It is an open standard protocol.
* ✅ **It is used within a group of routers for selecting an active device and a standby device to provide gateway services to a LAN.**
* ❌ If the virtual router master fails, one router is elected as the virtual router master with the other routers acting as backups.
  **Explanation:** HSRP (Hot Standby Router Protocol) is a **Cisco proprietary** FHRP that provides **gateway redundancy** by assigning an active and standby router.

---

### **Question 5**

**Which command will allow a network administrator to check the IP address assigned to a MAC address?**

* ❌ `Router# show ip dhcp server statistics`
* ❌ `Router# show running-config | section_dhcp`
* ✅ **`Router# show ip dhcp binding`**
* ❌ `Router# show ip dhcp pool`
  **Explanation:** `show ip dhcp binding` shows a list of DHCP-assigned IP addresses and their corresponding MAC addresses.

---

### **Question 6**

**Which two UDP ports are used to forward DHCP traffic?** (Choose two)

* ❌ 53
* ✅ **67**
* ❌ 80
* ❌ 23
* ✅ **68**
  **Explanation:** DHCP uses **UDP port 67 (server)** and **UDP port 68 (client)** for communication.

---

### **Question 7**

**Which DHCPv4 message will a client send to accept an IPv4 address that is offered by a DHCP server?**

* ✅ **broadcast DHCPREQUEST**
* ❌ broadcast DHCPACK
* ❌ unicast DHCPACK
* ❌ unicast DHCPREQUEST
  **Explanation:** The client broadcasts a **DHCPREQUEST** message to accept the IP offer and inform other servers that their offers are declined.

---

### **Question 8**

**Match the purpose with its DHCP message type:**

* **A message that is used to identify the explicit server and lease offer to accept** → ✅ **DHCPREQUEST**
* **A message that is used to locate any available DHCP server on a network** → ✅ **DHCPDISCOVER**
* **A message that is used to suggest a lease to a client** → ✅ **DHCPOFFER**
* **A message that is used to acknowledge that the lease is successful** → ✅ **DHCPACK**
  **Explanation:** Standard DORA workflow again, matching message types to their purpose.

---

### **Question 9**

**Which statement is true about DHCP operation?**

* ❌ A client must wait for lease expiration before it sends another DHCPREQUEST message.
* ❌ If the client receives several DHCPOFFER messages from different servers, it sends a unicast DHCPREQUEST message to the server from which it chooses to obtain the IP information.
* ✅ **When a device that is configured to use DHCP boots, the client broadcasts a DHCPDISCOVER message to identify any available DHCP servers on the network.**
* ❌ The DHCPDISCOVER message contains the IP address and subnet mask to be assigned, the IP address of the DNS server, and the IP address of the default gateway.
  **Explanation:** DHCPDISCOVER is the initial broadcast message to find servers.

---

### **Question 10**

**What is a result when the DHCP servers are not operational in a network?**

* ❌ Workstations are assigned with the IP address 0.0.0.0.
* ❌ Workstations are assigned with IP addresses in the 10.0.0.0/8 network.
* ✅ **Workstations are assigned with IP addresses in the 169.254.0.0/16 network.**
* ❌ Workstations are assigned with the IP address 127.0.0.1.
  **Explanation:** Windows and some OSs use **APIPA** (Automatic Private IP Addressing) in the range **169.254.0.0/16** when DHCP fails.

---

Would you like a downloadable PDF or markdown table for easier review?




Here are the correct matches for **Question 22** on **DHCPv6 server types**:

| **Description**                                                      | **DHCPv6 Server Type** |
| -------------------------------------------------------------------- | ---------------------- |
| enabled in RA messages with the `ipv6 nd other-config-flag` command  | Stateless DHCPv6       |
| clients send only DHCPv6 INFORMATION-REQUEST messages to the server  | Stateless DHCPv6       |
| enabled on the client with the `ipv6 address autoconfig` command     | Stateless DHCPv6       |
| the M flag is set to 1 in RA messages                                | Stateful DHCPv6        |
| uses the `address` command to create a pool of addresses for clients | Stateful DHCPv6        |
| enabled on the client with the `ipv6 address dhcp` command           | Stateful DHCPv6        |

Let me know if you’d like the entire set of answers compiled in a table format or document.





Certainly! Here's the full response for **Questions 23 to 30** including **all options and the correct one marked**:

---

### **Question 23**

**Which conclusion can be drawn based on the commands?**
*Refer to the exhibit.*

* ⭕ The router is configured for stateful DHCPv6 operation, but the DHCP pool configuration is incomplete.
* ⭕ The DHCPv6 server name is ACAD\_CLASS.
* ✅ **The router is configured for stateless DHCPv6 operation.**
* ⭕ Clients would configure the interface IDs above 0010.

---

### **Question 24**

**What kind of IPv6 addressing is being configured?**
*Refer to the exhibit.*

* ✅ **stateless DHCPv6**
* ⭕ stateful DHCPv6
* ⭕ static link-local
* ⭕ SLAAC

---

### **Question 25**

**Effect of M flag = 0 and O flag = 1 in RA messages when a PC tries to configure its IPv6 address**

* ⭕ It should use the information that is contained in the RA message exclusively.
* ✅ **It should use the information that is contained in the RA message and contact a DHCPv6 server for additional information.**
* ⭕ It should contact a DHCPv6 server for the prefix, the prefix-length information, and an interface ID that is both random and unique.
* ⭕ It should contact a DHCPv6 server for all the information that it needs.

---

### **Question 26**

**Match the step number to the HSRP failover process**

| **Step** | **Correct Match**                                                                        |
| -------- | ---------------------------------------------------------------------------------------- |
| Step 1   | ✅ The forwarding router fails.                                                           |
| Step 2   | ✅ The standby router stops seeing hello messages from the forwarding router.             |
| Step 3   | ✅ The standby router assumes the role of the forwarding router.                          |
| Step 4   | ✅ The new forwarding router assumes both the IP and MAC addresses of the virtual router. |

---

### **Question 27**

**Which destination MAC address is used when frames are sent from the workstation to the default gateway?**

* ⭕ MAC address of the forwarding router
* ✅ **MAC address of the virtual router**
* ⭕ MAC address of the standby router
* ⭕ MAC addresses of both the forwarding and standby routers

---

### **Question 28**

**What protocol allows load balancing across two gateways to the Internet?**

* ✅ **GLBP**
* ⭕ STP
* ⭕ PVST
* ⭕ PVST+

---

### **Question 29**

**Which IPv4 gateway address should be configured on the host?**

* ⭕ 192.168.2.2
* ✅ **192.168.2.100**
* ⭕ 192.168.2.1
* ⭕ 192.168.2.0

**Explanation:**
The host uses the **virtual IP address** `192.168.2.100` as the default gateway.

---

### **Question 30**

**Match the FHRP protocols to their descriptions**

| **Protocol** | **Description**                                                                                                   |
| ------------ | ----------------------------------------------------------------------------------------------------------------- |
| **VRRP**     | ✅ An open standard FHRP that provides redundancy through use of a virtual router’s master and one or more backups |
| **GLBP**     | ✅ A Cisco proprietary FHRP that provides load sharing in addition to redundancy                                   |
| **HSRP**     | ✅ A Cisco proprietary FHRP that provides redundancy through use of an active device and standby device            |

---

Let me know if you want these in a table format or need an explanation for any question!





Here are the **answers for Questions 31 to 33**, including **all options** with the **correct one marked**:

---

### **Question 31**

**Which statement describes a feature that is associated with HSRP?**

* ✅ **HSRP uses active and standby routers.**
* ⭕ It uses ICMP messages in order to assign the default gateway to hosts.
* ⭕ HSRP is nonproprietary.
* ⭕ It allows load balancing between a group of redundant routers.

**Explanation:** HSRP (Hot Standby Router Protocol) is a **Cisco proprietary** protocol that provides **gateway redundancy** using an **active and standby router** model. It does **not** use ICMP for gateway assignment and does **not support load balancing** (unlike GLBP).

---

### **Question 32**

**Which FHRP implementation is a nonproprietary IPv4-only election protocol which has one master router per group?**

* ⭕ VRRPv3
* ✅ **VRRPv2**
* ⭕ GLBP
* ⭕ HSRP for IPv6

**Explanation:**
**VRRPv2** is an open-standard (nonproprietary) protocol for IPv4 that uses a **single master router per group**.

* **VRRPv3** supports **IPv6**,
* **GLBP** supports load balancing,
* **HSRP for IPv6** is Cisco proprietary.

---

### **Question 33**

**The address pool of a DHCP server is configured with 10.3.2.0/24. The network administrator reserves 3 IP addresses for printers. How many IP addresses are left in the pool to be assigned to other hosts?**

* ⭕ 249
* ⭕ 252
* ✅ **251**
* ⭕ 255
* ⭕ 241

**Explanation:**

* A `/24` network = **256 IPs** (from 10.3.2.0 to 10.3.2.255)
* Subtract:

  * 1 for **network address** (10.3.2.0)
  * 1 for **broadcast address** (10.3.2.255)
  * 3 for **printer reservations**
    → 256 − 1 − 1 − 3 = **251 usable IPs**

---

Let me know if you want a table or explanation for any of these!
