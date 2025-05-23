
Here's a table with **all questions**, **all options**, and ✅ for **correct answers**:

---

### ✅ **Networking Quiz Answers with Explanations**

| Q# | Question                                                                                                                            | Options                                                                                                                                                                                                                                                                                                                         | Answer                                                                                                                                                |
| -- | ----------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1  | In what situation would a Layer 2 switch have an IP address configured?                                                             | • when the Layer 2 switch needs to be remotely managed ✅<br>• when the Layer 2 switch needs to forward user traffic to another device<br>• when the Layer 2 switch is the default gateway of user traffic<br>• when the Layer 2 switch is using a routed port                                                                   | ✅ when the Layer 2 switch needs to be remotely managed                                                                                                |
| 2  | A technician is configuring a new Cisco 2960 switch. What is the effect of issuing the `BranchSw(config)#interface VLAN88` command? | • It permits an IPv6 address to be configured on a switch physical interface<br>• It applies an IPv6 address to the virtual interface<br>• It enters configuration mode for a switch virtual interface ✅<br>• It updates the MAC address table for the associated port<br>• It applies an IPv4 address to the virtual interface | ✅ It enters configuration mode for a switch virtual interface                                                                                         |
| 3  | Which problem is evident if `show ip interface` shows interface is down and line protocol is down?                                  | • An encapsulation mismatch has occurred<br>• There is an IP address conflict<br>• The `no shutdown` command has not been issued<br>• A cable has not been attached to the port ✅                                                                                                                                               | ✅ A cable has not been attached to the port                                                                                                           |
| 4  | What is a result of connecting two or more switches together?                                                                       | • The size of the collision domain is increased<br>• The number of broadcast domains is increased<br>• The size of the broadcast domain is increased ✅<br>• The number of collision domains is reduced                                                                                                                          | ✅ The size of the broadcast domain is increased                                                                                                       |
| 5  | How is a frame from PCA forwarded to PCC if SW1’s MAC table is empty?                                                               | • SW1 floods the frame on all ports except incoming ✅<br>• SW1 floods but excludes SW2’s link and incoming port<br>• SW1 drops the frame<br>• SW1 forwards to SW2 and SW2 floods it                                                                                                                                             | ✅ SW1 floods the frame on all ports on SW1, excluding the port through which the frame entered                                                        |
| 6  | What are two switch characteristics that could help alleviate network congestion?                                                   | • large frame buffers ✅<br>• low port density<br>• frame check sequence (FCS) check<br>• fast internal switching ✅<br>• store-and-forward switching                                                                                                                                                                             | ✅ large frame buffers, fast internal switching                                                                                                        |
| 7  | How can a network admin reduce number of devices receiving broadcast traffic?                                                       | • Replace switches with more port switches<br>• Segment LAN into smaller LANs and route ✅<br>• Add more switches<br>• Replace switches with hubs                                                                                                                                                                                | ✅ Segment the LAN into smaller LANs and route between them                                                                                            |
| 8  | PC-A in VLAN 60 can’t talk to PC-B (also VLAN 60), trunk info given. What’s the issue?                                              | • Native VLAN should be 60<br>• Native VLAN is pruned<br>• VLAN 60 is not allowed on trunk ✅<br>• Trunk has `nonegotiate`                                                                                                                                                                                                       | ✅ The VLAN that is used by PC-A is not in the list of allowed VLANs on the trunk                                                                      |
| 9  | Match DTP modes to functions                                                                                                        | **Dynamic desirable** – Actively attempts to convert to trunk ✅<br>**Nonegotiate** – Requires manual configuration ✅<br>**Trunk** – Permanent trunking mode ✅<br>**Dynamic auto** – Passively waits for neighbor ✅                                                                                                              | ✅ A: Dynamic desirable – Actively attempts<br>✅ B: Nonegotiate – Manual config<br>✅ C: Trunk – Permanent trunk<br>✅ D: Dynamic auto – Waits passively |
| 10 | Which type of traffic is designed for a native VLAN?                                                                                | • tagged<br>• management<br>• user-generated<br>• untagged ✅                                                                                                                                                                                                                                                                    | ✅ untagged                                                                                                                                            |

---

Let me know if you'd like this exported as a Markdown file or formatted in any other way!



Here are **Questions 11 to 20** presented in a clear **table format** with all options, correct answers, and explanations:

---

### ✅ **Questions 11–20 with Options, Correct Answers, and Explanations**

| **Q#** | **Question Summary**                                                | **Options**                                                                                                                                                                                                | **Correct Answer**               | **Explanation**                                                                                                            |
| ------ | ------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------- | -------------------------------------------------------------------------------------------------------------------------- |
| **11** | Native VLAN mismatch between DLS1 and DLS2 (99 vs. 66)              | A. `switchport nonegotiate`<br>B. `switchport trunk native vlan 66`<br>C. `switchport trunk allowed vlan add 99`<br>D. `switchport mode dynamic auto`                                                      | **B**                            | The native VLAN must match on both sides. DLS2 uses 66, so DLS1 should be set to `native vlan 66`.                         |
| **12** | Type of VLAN for management traffic (SSH, SNMP, etc.)               | A. `trunk VLAN`<br>B. `voice VLAN`<br>C. `security VLAN`<br>D. `management VLAN`                                                                                                                           | **D**                            | Management VLAN is specifically designated for administrative access like SSH, Telnet, SNMP.                               |
| **13** | Preparing switch port for router-on-a-stick setup                   | A. `spanning-tree vlan 1`<br>B. `switchport mode trunk`<br>C. `spanning-tree portfast`<br>D. `switchport access vlan 1`                                                                                    | **B**                            | Router-on-a-stick requires the port to the router to be in **trunk mode** to carry multiple VLANs.                         |
| **14** | Inter-VLAN routing fails – switch config shows trunk port as access | A. `Fa0/1 should be trunk, not access`<br>B. `Access ports should negotiate`<br>C. `Fa0/1 should negotiate`<br>D. `Access interfaces need IPs`                                                             | **A**                            | The port Fa0/1 must be a trunk port to carry multiple VLANs; it's incorrectly set as an access port.                       |
| **15** | Hosts H1 (VLAN 10) and H2 (VLAN 20) can't communicate               | A. `VLAN configuration`<br>B. `port mode on Fa0/1 and Fa0/2`<br>C. `router port configuration`<br>D. `trunking`                                                                                            | **A**                            | The VLANs (10, 20) are not shown as created. VLANs must exist for routing to work.                                         |
| **16** | Advantage of PVST+ (Per VLAN Spanning Tree Plus)                    | A. `Optimizes performance via load sharing`<br>B. `Auto-selects root bridge`<br>C. `Reduces bandwidth compared to CST`<br>D. `Uses fewer CPU cycles`                                                       | **A**                            | PVST+ allows different VLANs to use different STP instances, which can load balance traffic.                               |
| **17** | Components of Bridge ID (Choose 3)                                  | A. `IP address`<br>B. `extended system ID`<br>C. `bridge priority`<br>D. `MAC address`<br>E. `port ID`<br>F. `cost`                                                                                        | **B, C, D**                      | Bridge ID = bridge priority + extended system ID + MAC address.                                                            |
| **18** | Match Spanning-Tree Features to Protocols                           | - Proprietary per VLAN IEEE 802.1w → **A. PVST+**<br>- IEEE standard reducing STP instances → **B. MST**<br>- Cisco implementation of 802.1D → **C. PVST+**<br>- Fast convergence for 802.1D → **D. RSTP** | A → D<br>B → A<br>C → D<br>D → C | Matches:<br>- PVST+ = proprietary per-VLAN STP<br>- MST = fewer STP instances<br>- RSTP = fast convergence of 802.1D       |
| **19** | Start LACP EtherChannel on 2 interfaces                             | A. `interface port-channel 2`<br>B. `channel-group 1 mode desirable`<br>C. `interface range Gi0/4 - 5`<br>D. `channel-group 2 mode auto`                                                                   | **C**                            | First step is selecting the interface range for the EtherChannel with `interface range`. Then you apply LACP settings.     |
| **20** | Identify command from EtherChannel troubleshooting output           | A. `show interfaces Port-channel11`<br>B. `show etherchannel summary`<br>C. `show etherchannel Port-channel`<br>D. `show interfaces fastethernet 0/11 etherchannel`                                        | **D**                            | The output shows LACP details for a specific interface (Fa0/11). Correct command is `show interfaces fa0/11 etherchannel`. |

---

Let me know if you want this in **Markdown**, **PDF**, or embedded in a README file.



Here are **Questions 21 to 30** with **full question text**, **all options**, and the **correct answer marked**, without sorting or removing anything:

---

### **Question 21**

The exhibit displays the following command and some partial output:
`S1# show etherchannel summary`

```
<output omitted>  
Number of channel-groups in use: 1  
Number of aggregators: 1  
Group   Port-channel   Protocol    Ports  
1       Po1(SU)          -        Fa0/10(P)  Fa0/11(p)
```

Refer to the exhibit. Based on the command output shown, what is the status of the EtherChannel?

* The EtherChannel is partially functional as indicated by the P flags for the FastEthernet ports.
* ✅ The EtherChannel is in use and functional as indicated by the SU and P flags in the command output.
* The EtherChannel is down as evidenced by the protocol field being empty.
* The EtherChannel is dynamic and is using ports Fa0/10 and Fa0/11 as passive ports.

---

### **Question 22**

Match the purpose with its DHCP message type.

**Categories:**
DHCPOFFER
DHCPDISCOVER
DHCPNAK
DHCPREQUEST
DHCPACK

**Options:**

* A message that is used to locate any available DHCP server on a network
* A message that is used to acknowledge that the lease is successful
* A message is used by a server to finalize a successful lease with a client
* A message that is used to identify the explicit server and lease offer to accept
* A message that is used to suggest a lease to a client

✅ Matching:

* DHCPDISCOVER → A message that is used to locate any available DHCP server on a network
* DHCPOFFER → A message that is used to suggest a lease to a client
* DHCPREQUEST → A message that is used to identify the explicit server and lease offer to accept
* DHCPACK → A message that is used to acknowledge that the lease is successful
* DHCPNAK → A message is used by a server to finalize a successful lease with a client

---

### **Question 23**

An administrator has configured a DHCPv4 relay router and issued these commands:

```
Router(config)# interface g0/0  
Router(config-if)# ip address 10.0.1.1 255.255.255.0  
Router(config-if)# no shutdown  
Router(config-if)# exit  
Router(config)# ip dhcp pool RELAY  
Router(dhcp-config)# end
```

The clients are not receiving IP parameters from the DHCPv4 server. What is a possible cause?

* The router is configured as a DHCPv4 client.
* The IP address is incorrect for the subnet mask that is used.
* ✅ The ip helper-address command is missing.
* The pool cannot be named 'RELAY'.

---

### **Question 24**

A small coffee shop is offering free Wi-Fi to customers. The network includes a wireless router and a DSL modem that is connected to the local phone company. What method is typically used to configure the connection to the phone company?

* ✅ Set the DSL modem as a DHCP client to the phone company and a DHCP server for the internal connection.
* Set the WAN connection in the wireless router as a DHCP client.
* Set the connection between the wireless router and the DSL modem as a private IP network.
* Set the DSL modem as a DHCP client to get a public IP address from the wireless router.

---

### **Question 25**

A network administrator is implementing DHCPv6 for the company. The administrator configures a router to send RA messages with M flag as 1 by using the interface command `ipv6 nd managed-config-flag`. What effect will this configuration have on the operation of the clients?

* ✅ Clients must use all configuration information that is provided by a DHCPv6 server.
* Clients must use the information that is contained in RA messages.
* Clients must use the prefix and prefix length that are provided by RA messages and obtain additional information from a DHCPv6 server.
* Clients must use the prefix and prefix length that are provided by a DHCPv6 server and generate a random interface ID.

---

### **Question 26**

```
R1# show running-config  
<output omitted>  
ipv6 unicast-routing  
!  
ipv6 dhcp pool LAN1  
 prefix-delegation 2001:DB8:5::/48 00030001000E84244E70  
 dns-server 2001:DB8:5::8  
 domain-name cisco.com  
!  
interface FastEthernet0/0  
 no ip address  
 ipv6 address 2001:DB8:5::100/48  
 ipv6 dhcp server LAN1
```

Refer to the exhibit. The users on the LAN network of R1 cannot receive an IPv6 address from the configured stateful DHCPv6 server. What is missing from the stateful DHCPv6 configuration on router R1?

* ✅ The FA0/0 interface is missing the command that informs the clients to use stateful DHCPv6.
* The DHCPv6 pool has not been bound to the LAN interface.
* IPv6 has not been enabled globally on router R1.
* The DHCPv6 pool does not match the IPv6 address configured on interface FA0/0.

---

### **Question 27**

A network engineer is configuring a LAN with a redundant first hop to make better use of the available network resources. Which protocol should the engineer implement?

* GLBP
* FHRP
* VRRP
* ✅ HSRP

---

### **Question 28**

Match the FHRP protocols to the appropriate description.

**Categories:**
VRRP
GLBP
HSRP

**Options:**

* A Cisco proprietary FHRP that provides redundancy through use of an active device and standby device
* An open standard FHRP that provides redundancy through use of a virtual router’s master and one or more backups
* A Cisco proprietary FHRP that provides load sharing in addition to redundancy

✅ Matching:

* HSRP → A Cisco proprietary FHRP that provides redundancy through use of an active device and standby device
* VRRP → An open standard FHRP that provides redundancy through use of a virtual router’s master and one or more backups
* GLBP → A Cisco proprietary FHRP that provides load sharing in addition to redundancy

---

### **Question 29**

Which term describes the role of a Cisco switch in the 802.1X port-based access control?

* supplicant
* ✅ authenticator
* agent
* authentication server

---

### **Question 30**

Which statement describes the behavior of a switch when the MAC address table is full?

* It treats frames as unknown unicast and floods all incoming frames to all ports within the collision domain.
* It treats frames as unknown unicast and floods all incoming frames to all ports on the switch.
* ✅ It treats frames as unknown unicast and floods all incoming frames to all ports within the local VLAN.
* It treats frames as unknown unicast and floods all incoming frames to all ports across multiple switches.

---

Let me know if you want the next set of questions!




Here are **Questions 31 to 39** with all options and the correct answer clearly marked:

---

### **Question 31**

**Which Cisco solution helps prevent ARP spoofing and ARP poisoning attacks?**

* DHCP Snooping
* Port Security
* ✅ Dynamic ARP Inspection
* IP Source Guard

---

### **Question 32**

**After sticky learning of MAC addresses is enabled, what action is needed to prevent dynamically learned MAC addresses from being lost in the event that an associated interface goes down?**

* Reboot the switch.
* ✅ Copy the running configuration to the startup configuration.
* Configure port security for violation protect mode.
* Shut down the interface then enable it again with the no shutdown command.

---

### **Question 33**

**What is the best way to prevent a VLAN hopping attack?**

* Use VLAN 1 as the native VLAN on trunk ports.
* Disable STP on all nontrunk ports.
* ✅ Disable trunk negotiation for trunk ports and statically set nontrunk ports as access ports.
* Use ISL encapsulation on all trunk links.

---

### **Question 34**

**Refer to the exhibit. A network administrator is configuring DAI on switch SW1. What is the result of entering the exhibited commands?**

```
SW1(config)# ip arp inspection validate ip  
SW1(config)# ip arp inspection validate src-mac  
SW1(config)# ip arp inspection validate dst-mac  
```

* DAI will validate only the IP addresses.
* ✅ DAI will validate both source and destination MAC addresses as well as the IP addresses in the order specified. If all parameters are valid then the ARP packet is allowed to pass.
* DAI will validate both source and destination MAC addresses as well as the IP addresses in the order specified. When one set of parameters are valid, the ARP packet is allowed to pass.
* DAI will validate only the destination MAC addresses.

---

### **Question 35**

**On which port should Dynamic ARP Inspection (DAI) be configured on a switch?**

* access ports only
* ✅ any untrusted port
* on any port where DHCP snooping is disabled
* an uplink port to another switch

---

### **Question 36**

**Refer to the exhibit. The administrator wants to enable port security on an interface on switch S1, but the command was rejected. Which conclusion can be drawn?**

```
S1(config)# interface fa0/1  
S1(config-if)# switchport port-security  
Command rejected: FastEthernet0/1 is a dynamic port.
```

* ✅ The interface must be initially configured with the switchport mode access command.
* The interface needs to be previously configured with the no shutdown command.
* The interface needs to be configured initially with an IP address.
* The interface must be initially configured with the switchport mode trunk command.

---

### **Question 37**

**Which combination of WLAN authentication and encryption is recommended as a best practice for home users?**

* ✅ WPA2 and AES
* EAP and AES
* WEP and TKIP
* WPA and PSK
* WEP and RC4

---

### **Question 38**

**An employee connects wirelessly to the company network using a cell phone. The employee then configures the cell phone to act as a wireless access point that will allow new employees to connect to the company network. Which type of security threat best describes this situation?**

* denial of service
* cracking
* ✅ rogue access point
* spoofing

---

### **Question 39**

**What are the two methods that a wireless NIC can use to discover an AP? (Choose two.)**

* ⬜ sending an ARP request broadcast
* ⬜ initiating a three-way handshake
* ✅ receiving a broadcast beacon frame
* ⬜ sending a multicast frame
* ✅ transmitting a probe request

---

Let me know when you're ready for the next batch!










Here's the full table including **Questions 40–49**, with **all options**, the **correct answer marked**, and a **clear explanation**:

---

### ✅ Questions 40–49 with Options, Answers & Explanations:

| Q#     | Question                                                                                                                                                                                                                           | Option                                                                                                                                 | Answer | Explanation                                                                         |
| ------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------- | ------ | ----------------------------------------------------------------------------------- |
| **40** | What is the reason for disabling SSID broadcasting and changing the default SSID on a wireless access point?                                                                                                                       | The access point stops broadcasting its own MAC address, thus preventing unauthorized wireless clients from connecting to the network. | ❌      | MAC address is still visible; SSID broadcasting doesn’t hide it.                    |
|        |                                                                                                                                                                                                                                    | Disabling SSID broadcasting frees up radio frequency bandwidth and increases the data throughput of the access point.                  | ❌      | It does not affect throughput or bandwidth.                                         |
|        |                                                                                                                                                                                                                                    | Anyone with the default SSID can gain access to the access point and change the configuration.                                         | ❌      | Changing the SSID helps avoid easy guessing but configuration requires credentials. |
|        |                                                                                                                                                                                                                                    | **Wireless clients must then have the SSID manually configured to connect to the wireless network.**                                   | ✅      | Hiding SSID means devices must be manually configured with the network name.        |
| **41** | What is a potential issue when using the WLC to upgrade and deploy the latest firmware image to all APs?                                                                                                                           | Usernames and passwords must be manually entered into the AP so that WLAN authentication continues during the upgrade.                 | ❌      | Credentials are centrally managed; this is not required.                            |
|        |                                                                                                                                                                                                                                    | Only one of the two bands would work at a time.                                                                                        | ❌      | This is not typically caused by firmware upgrades.                                  |
|        |                                                                                                                                                                                                                                    | **Users will not be able to use the WLAN.**                                                                                            | ✅      | Firmware upgrade may take APs offline temporarily, disrupting connectivity.         |
|        |                                                                                                                                                                                                                                    | Old 802.11 standards may not be supported anymore.                                                                                     | ❌      | Possible, but not a primary concern during regular upgrades.                        |
| **42** | A network administrator of a college is configuring WLAN security with WPA2 Enterprise authentication. Which server is required when deploying this type of authentication?                                                        | **RADIUS**                                                                                                                             | ✅      | WPA2 Enterprise requires a RADIUS server for centralized authentication.            |
|        |                                                                                                                                                                                                                                    | SNMP                                                                                                                                   | ❌      | Used for monitoring, not authentication.                                            |
|        |                                                                                                                                                                                                                                    | AAA                                                                                                                                    | ❌      | AAA is the framework; RADIUS is the server implementing it.                         |
|        |                                                                                                                                                                                                                                    | DHCP                                                                                                                                   | ❌      | DHCP provides IP addresses, not authentication.                                     |
| **43** | A network administrator is configuring a WLC to provide WLAN access to users in an office building. When testing the newly created WLAN, the administrator does not see the SSID from a wireless device. What is a possible cause? | **The new WLAN needs to be enabled.**                                                                                                  | ✅      | If the WLAN is not enabled on the WLC, the SSID won’t be broadcast.                 |
|        |                                                                                                                                                                                                                                    | The WLAN security setting is incorrect.                                                                                                | ❌      | This would prevent access but not SSID visibility.                                  |
|        |                                                                                                                                                                                                                                    | The RADIUS server is not operational.                                                                                                  | ❌      | Again, this affects authentication, not visibility of SSID.                         |
|        |                                                                                                                                                                                                                                    | The APs have not been configured for the new WLAN.                                                                                     | ❌      | Could be a cause, but more likely it’s just disabled.                               |
| **44** | Refer to the exhibit. Which interface will be the exit interface to forward a data packet that has the destination IP address 172.18.109.152?                                                                                      | None, the packet will be dropped                                                                                                       | ❌      | There is a valid route for the subnet.                                              |
|        |                                                                                                                                                                                                                                    | GigabitEthernet0/1                                                                                                                     | ❌      | 172.18.109.224/27 is on this interface, which does not include .152.                |
|        |                                                                                                                                                                                                                                    | **Serial0/0/0**                                                                                                                        | ✅      | Route to 172.18.109.128/26 via 172.18.32.1 (Serial0/0/0) includes 172.18.109.152.   |
|        |                                                                                                                                                                                                                                    | GigabitEthernet0/0                                                                                                                     | ❌      | This interface handles 192/27 subnet, which doesn’t cover 152.                      |
| **45** | What are two characteristics of Cisco Express Forwarding (CEF)?                                                                                                                                                                    | With this switching method, flow information for a packet is stored in the fast-switching cache...                                     | ❌      | That’s fast switching, not CEF.                                                     |
|        |                                                                                                                                                                                                                                    | When a packet arrives... it is forwarded to the control plane where the CPU matches...                                                 | ❌      | That’s process switching, not CEF.                                                  |
|        |                                                                                                                                                                                                                                    | **Packets are forwarded based on information in the FIB and an adjacency table.**                                                      | ✅      | This is the core mechanism of CEF.                                                  |
|        |                                                                                                                                                                                                                                    | **This is the fastest forwarding mechanism on Cisco routers and multilayer switches.**                                                 | ✅      | CEF provides high-speed, low-latency forwarding.                                    |
|        |                                                                                                                                                                                                                                    | When a packet arrives... searches for a match in the fast-switching cache.                                                             | ❌      | Again, this is fast switching, not CEF.                                             |
| **46** | Match the dynamic routing protocol component to the characteristic:                                                                                                                                                                | Algorithm → A finite list of steps used to determine the best path                                                                     | ✅      | Algorithms like Dijkstra or Bellman-Ford find best paths.                           |
|        |                                                                                                                                                                                                                                    | Data structures → Tables or databases stored in RAM                                                                                    | ✅      | Routing tables, topology tables, etc., are stored in RAM.                           |
|        |                                                                                                                                                                                                                                    | Routing protocol messages → Exchanges routing information and maintains accuracy                                                       | ✅      | Messages like Hello, Update, etc., maintain routing info.                           |
| **47** | What address and prefix length is used when configuring an IPv6 default static route?                                                                                                                                              | FF02::1/8                                                                                                                              | ❌      | This is a multicast address.                                                        |
|        |                                                                                                                                                                                                                                    | 0.0.0.0/0                                                                                                                              | ❌      | This is for IPv4, not IPv6.                                                         |
|        |                                                                                                                                                                                                                                    | **::/0**                                                                                                                               | ✅      | IPv6 default route is denoted as `::/0`.                                            |
|        |                                                                                                                                                                                                                                    | ::1/128                                                                                                                                | ❌      | This is the loopback address.                                                       |
| **48** | Match the description with the routing table entries:                                                                                                                                                                              | Metric → 21024000                                                                                                                      | ✅      | Indicates cost of the route.                                                        |
|        |                                                                                                                                                                                                                                    | Administrative distance → 1                                                                                                            | ✅      | Lower value = more trusted route.                                                   |
|        |                                                                                                                                                                                                                                    | Next hop → 172.16.2.2                                                                                                                  | ✅      | Next router to reach destination.                                                   |
|        |                                                                                                                                                                                                                                    | Route timestamp → 00:22:15                                                                                                             | ✅      | Time since the route was learned.                                                   |
|        |                                                                                                                                                                                                                                    | Route source protocol → D                                                                                                              | ✅      | “D” denotes EIGRP.                                                                  |
|        |                                                                                                                                                                                                                                    | Destination network → 10.3.0.0                                                                                                         | ✅      | Network for which this route applies.                                               |
| **49** | Which command would create a valid IPv6 default route?                                                                                                                                                                             | **ipv6 route ::/0 fe80::1**                                                                                                            | ✅      | This creates a default route using a link-local next hop.                           |
|        |                                                                                                                                                                                                                                    | **ipv6 route ::/0 2001\:db8\:acad:2::a**                                                                                               | ✅      | Also valid with a global unicast address.                                           |
|        |                                                                                                                                                                                                                                    | ipv6 route 2001\:db8\:acad:1::/64 ::1                                                                                                  | ❌      | This is not a default route.                                                        |
|        |                                                                                                                                                                                                                                    | ipv6 route ::/128 2001\:db8\:acad:1::1                                                                                                 | ❌      | `::/128` matches only the loopback.                                                 |

---

Let me know if you’d like this as a markdown table for your report or README!







Here are the questions with their correct answers and explanations:

---

### Question 50

**Consider the following command:**

```
ip route 192.168.10.0 255.255.255.0 10.10.10.2 5
```

**What does the 5 at the end of the command signify?**

* administrative distance  ✔️
* metric
* exit interface
* maximum number of hops to the 192.168.10.0/24 network

**Answer:** administrative distance

**Explanation:**
The last number in the `ip route` command represents the **administrative distance (AD)** of the static route. AD is used by the router to select the best path when there are multiple routes to the same destination learned from different routing protocols or static routes. Lower AD is preferred.

---

### Question 51

```
Gateway of last resort is not set
10.0.0.0/30 is subnetted, 2 subnets
C 10.0.0.0 is directly connected, Serial0/0/0
C 10.0.0.4 is directly connected, Serial0/0/1
192.168.10.0/26 is subnetted, 3 subnets
S 192.168.10.0 is directly connected, Serial0/0/0
C 192.168.10.64 is directly connected, FastEthernet0/0
S 192.168.10.128 [1/0] via 10.0.0.6
```

**What will router R2 do with a packet destined for 192.168.10.129?**

* send the packet out interface FastEthernet0/0
* drop the packet
* send the packet out interface Serial0/0/0
* send the packet out interface Serial0/0/1  ✔️

**Answer:** send the packet out interface Serial0/0/1

**Explanation:**
The route to `192.168.10.128` with mask `/26` includes IP addresses from 192.168.10.128 to 192.168.10.191. The packet destined to 192.168.10.129 falls into this range, so the router uses the static route via next hop `10.0.0.6` which is reachable through interface `Serial0/0/1`.

---

### Question 52

**OSPF link is up on WAN 192.168.0.32/30 but backup static route using:**

```
ip route 0.0.0.0 0.0.0.0 S0/0/1 100
```

**Traffic uses backup even when primary is up. What change should be made?**

* Change the destination network to 192.168.0.34.
* Add the next hop neighbor address of 192.168.0.36.  ✔️
* Change the administrative distance to 1.
* Change the administrative distance to 120.

**Answer:** Add the next hop neighbor address of 192.168.0.36.

**Explanation:**
When specifying a static route with an exit interface only (no next-hop IP), some IOS versions might consider it as preferred or unreliable depending on interface state. Adding the next-hop IP address (next hop neighbor) with administrative distance 100 ensures the route is only used if the next hop is reachable and has higher AD than OSPF (which is 110 by default). This prevents the backup route from being used unnecessarily.

---

### Question 53

**When a packet arrives on interface Serial0/0/0 on R1 destined for PC1 (192.168.10.2), which two events occur?**

* Router R1 will forward the packet out S0/0/0.
* Router R1 will forward the packet out Gig0/0.
* Router R1 will de-encapsulate the packet and encapsulate it in an Ethernet frame.  ✔️
* Router R1 will forward the packet out Gig0/1.  ✔️
* Router R1 will de-encapsulate the packet and encapsulate it in a PPP frame.

**Answers:**

* Router R1 will de-encapsulate the packet and encapsulate it in an Ethernet frame.
* Router R1 will forward the packet out Gig0/1.

**Explanation:**
The packet arrives on a serial interface (PPP encapsulated), destined for PC1 on the LAN connected to GigabitEthernet0/1. The router will remove the PPP encapsulation and forward it out the Gig0/1 interface, encapsulated in Ethernet frames.

---

### Question 54

**Given the IPv6 routing table snippet including:**

```
S 2001:DB8:CAFE:4::1/128 [1/0] via Serial0/0/0, directly connected
```

**How was this host route installed?**

* The route was dynamically learned from another router.
* The route was automatically installed when an IP address was configured on an active interface.
* The route was manually entered by an administrator.  ✔️
* The route was dynamically created by router R1.

**Answer:** The route was manually entered by an administrator.

**Explanation:**
The route is marked with "S" which means it is a static route. Static routes are manually configured by an administrator.

---

### Question 55

**A junior technician configured a route but traceroute shows wrong path/unreachable. What should be done?**

* Create a floating static route to that network.
* Check the configuration of the exit interface on the new static route.  ✔️
* Check the configuration on the floating static route and adjust the AD.
* Verify that the static route to the server is present in the routing table.

**Answer:** Check the configuration of the exit interface on the new static route.

**Explanation:**
Incorrect exit interface configuration is a common cause of routing issues. It's important to verify that the exit interface configured on the static route is correct and operational.

---

If you want, I can also provide more detailed explanations or examples for any question!







