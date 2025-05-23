Here are the correct answers with all options shown and correct ones marked:

---

### **Question 1**

**What represents a best practice concerning discovery protocols such as CDP and LLDP on network devices?**

* ⬜ Use the open standard LLDP rather than CDP.
* ⬜ Enable CDP on edge devices, and enable LLDP on interior devices.
* ✅ **Disable both protocols on all interfaces where they are not required.**
* ⬜ Use the default router settings for CDP and LLDP.

---

### **Question 2**

**What are three techniques for mitigating VLAN attacks? (Choose three.)**

* ✅ **Enable trunking manually.**
* ✅ **Disable DTP.**
* ⬜ Enable Source Guard.
* ✅ **Use private VLANs.**
* ✅ **Set the native VLAN to an unused VLAN.**
* ⬜ Enable BPDU guard.

---

### **Question 3**

**Which wireless network topology would be used by network engineers to provide a wireless network for an entire college building?**

* ⬜ Ad hoc
* ⬜ Mixed mode
* ⬜ Hotspot
* ✅ **Infrastructure**

---

### **Question 4**

**Which two commands can be used to enable BPDU guard on a switch? (Choose two.)**

* ⬜ S1(config-if)# enable spanning-tree bpduguard
* ✅ **S1(config-if)# spanning-tree bpduguard enable**
* ✅ **S1(config)# spanning-tree portfast bpduguard default**
* ⬜ S1(config)# spanning-tree bpduguard default
* ⬜ S1(config-if)# spanning-tree portfast bpduguard

---

### **Question 5**

**A network administrator enters the following commands on the switch SW1.**

```
SW1(config)# interface range fa0/5 – 10  
SW1(config-if)# ip dhcp snooping limit rate 6
```

**What is the effect after these commands are entered?**

* ✅ **If any of the FastEthernet ports 5 through 10 receive more than 6 DHCP messages per second, the port will be shut down.**
* ⬜ FastEthernet ports 5 through 10 can receive up to 6 DHCP discovery messages per second.
* ⬜ FastEthernet ports 5 through 10 can receive up to 6 DHCP messages per second of any type.
* ⬜ If any of the FastEthernet ports 5 through 10 receive more than 6 DHCP messages per second, the port will continue to operate and an error message will be sent to the network administrator.

---

### **Question 6**

**Which type of wireless network is suitable for national and global communications?**

* ⬜ Wireless local-area network
* ⬜ Wireless metropolitan-area network
* ⬜ Wireless personal-area network
* ✅ **Wireless wide-area network**

---

### **Question 7**

**An IT security specialist enables port security on a switch port of a Cisco switch. What is the default violation mode in use until the switch port is configured to use a different violation mode?**

* ⬜ Disabled
* ✅ **Shutdown**
* ⬜ Restrict
* ⬜ Protect

---

### **Question 8**

**Which step is required before creating a new WLAN on a Cisco 3500 series WLC?**

* ✅ **Create a new VLAN interface.**
* ⬜ Create a new SSID.
* ⬜ Build or have a RADIUS server available.
* ⬜ Build or have an SNMP server available.

---

### **Question 9**

**Which access control component, implementation, or protocol is based on device roles of supplicant, authenticator, and authentication server?**

* ⬜ Accounting
* ✅ **802.1X**
* ⬜ Authentication
* ⬜ Authorization

---

### **Question 10**

**Which event will take place if there is a port security violation on switch S1 interface Fa0/1?**

* ⬜ A notification is sent.
* ⬜ Packets with unknown source addresses will be dropped.
* ⬜ A syslog message is logged.
* ✅ **The interface will go into error-disabled state.**

---

Let me know if you’d like these exported in a specific format or explained further.



Here are the **correct answers** for Questions **11 to 20** with ✅ (correct) and ❌ (incorrect) indicators for all options:

---

### **Question 11**

**What is the purpose of the shared secret password in a RADIUS configuration?**

* ❌ It is used by the RADIUS server to authenticate WLAN users.
* ❌ It is used to authenticate and encrypt user data on the WLAN.
* ✅ **It is used to encrypt the messages between the WLC and the RADIUS server.**
* ❌ It allows users to authenticate and access the WLAN.

---

### **Question 12**

**What action will occur when PC1 is connected with a different MAC than configured?**

* ❌ Frames from PC1 will cause the interface to shut down immediately, and a log entry will be made.
* ✅ **Frames from PC1 will be dropped, and there will be no log of the violation.**
* ❌ Frames from PC1 will be forwarded to its destination, but a log entry will not be created.
* ❌ Frames from PC1 will be forwarded to its destination, and a log entry will be created.
* ❌ Frames from PC1 will be dropped, and a log message will be created.
* ❌ Frames from PC1 will be forwarded since the switchport port-security violation command is missing.

> Note: Since no `violation` mode is set, default is **shutdown**, so the most accurate should be **first**, but your marked choice assumes **restrict/protect** mode.

---

### **Question 13**

**Best way to improve 802.11n network performance when it's slow?**

* ✅ **Split the traffic between the 2.4 GHz and 5 GHz frequency bands.**
* ❌ Replace the wireless NICs on the computers that are experiencing slow connections.
* ❌ Disable DHCP on the access point and assign static addresses to the wireless clients.
* ❌ Upgrade the firmware on the wireless access point.

---

### **Question 14**

**Which VLAN-hopping attack is mitigated by setting an unused VLAN as the native VLAN?**

* ❌ DTP spoofing
* ✅ **VLAN double-tagging**
* ❌ DHCP spoofing
* ❌ DHCP starvation

---

### **Question 15**

**What service is used to allow internal clients to access the Internet?**

* ✅ **NAT**
* ❌ DHCP
* ❌ DNS
* ❌ RADIUS

---

### **Question 16**

**Most appropriate port-security configuration for Fa0/2 with an IP phone and a PC?**

* ❌ `switchport port-security mac-address sticky` + `maximum 2`
* ✅ **`switchport port-security` + `maximum 2` + `mac-address sticky`**
* ❌ `switchport port-security` + `mac-address sticky`
* ❌ `switchport port-security` + `maximum 2` + `mac-address sticky` + `violation restrict`

> Best matches the admin’s goals (detect both MACs automatically, shutdown on unknown devices).

---

### **Question 17**

**Which option on a Cisco 3504 WLC dashboard provides access to full menu of features?**

* ❌ Access Points
* ❌ Network Summary
* ❌ Rogues
* ✅ **Advanced**

---

### **Question 18**

**Which switch feature makes it vulnerable to VLAN hopping attacks?**

* ✅ **The automatic trunking port feature enabled for all ports by default**
* ❌ The mixed duplex mode enabled for all ports by default
* ❌ The limited size of content-addressable memory space
* ❌ Mixed port bandwidth support enabled for all ports by default

---

### **Question 19**

**Which two Cisco solutions help prevent DHCP starvation attacks?** (Choose two)

* ❌ Dynamic ARP Inspection
* ✅ **Port Security**
* ❌ Web Security Appliance
* ✅ **DHCP Snooping**
* ❌ IP Source Guard

---

### **Question 20**

**Which server verifies usernames and passwords for WLAN authentication?**

* ✅ **RADIUS**
* ❌ AAA *(AAA is a framework; RADIUS is the actual server implementation)*
* ❌ SNMP
* ❌ NAT

---

Let me know if you want this in a **markdown table format** or exported to a file!







Sure! Here's the full Q\&A for **Questions 21 to 30** with **all options** and **correct answer marked** (with green check) and **explanations**:

---

### Question 21

**Which component of AAA allows an administrator to track individuals who access network resources and any changes that are made to those resources?**

* ⬜ Authentication
* ⬜ Authorization
* ✅ **Accounting**
* ⬜ Accessibility

**Explanation:** Accounting records user activities and tracks what resources were accessed or changed.

---

### Question 22

**A technician is about to install and configure a wireless network at a small branch office. What is the first security measure the technician should apply immediately upon powering up the wireless router?**

* ⬜ Configure encryption on the wireless router and the connected wireless devices.
* ⬜ Enable MAC address filtering on the wireless router.
* ⬜ Disable the wireless network SSID broadcast.
* ✅ **Change the default user-name and password of the wireless router.**

**Explanation:** Changing default credentials protects the router from unauthorized admin access.

---

### Question 23

**A technician is troubleshooting a slow WLAN that consists of 802.11b and 802.11g devices. A new 802.11n/ac dual-band router has been deployed on the network to replace the old 802.11g router. What can the technician do to address the slow wireless speed?**

* ⬜ Update the firmware on the new router.
* ✅ **Split the wireless traffic between the 802.11n 2.4 GHz band and the 5 GHz band.**
* ⬜ Configure devices to use a different channel.
* ⬜ Change the SSID.

**Explanation:** Using dual bands reduces congestion and interference on the 2.4 GHz band.

---

### Question 24

**What are the two methods that are used by a wireless NIC to discover an AP? (Choose two.)**

* ✅ Receiving a broadcast beacon frame
* ⬜ Sending an ARP request
* ✅ Transmitting a probe request
* ⬜ Delivering a broadcast frame
* ⬜ Initiating a three-way handshake

**Explanation:** Wireless NICs either passively receive beacon frames or actively send probe requests to discover APs.

---

### Question 25

**Refer to the exhibit. What can be determined about port security from the information that is shown?**

* ⬜ The port has been shut down.
* ⬜ The port has two attached devices.
* ✅ **The port violation mode is the default for any port that has port security enabled.**
* ⬜ The port has the maximum number of MAC addresses that is supported by a Layer 2 switch port which is configured for port security.

**Explanation:** The violation mode is **Shutdown**, which is the default violation mode.

---

### Question 26

**The company handbook states that employees cannot have microwave ovens in their offices. Instead, all employees must use the microwave ovens located in the employee cafeteria. What wireless security risk is the company trying to avoid?**

* ⬜ Improperly configured devices
* ✅ **Accidental interference**
* ⬜ Rogue access points
* ⬜ Interception of data

**Explanation:** Microwave ovens can cause interference in the 2.4 GHz wireless frequency.

---

### Question 27

**While attending a conference, participants are using laptops for network connectivity. When a guest speaker attempts to connect to the network, the laptop fails to display any available wireless networks. The access point must be operating in which mode?**

* ⬜ Mixed
* ✅ **Passive**
* ⬜ Open
* ⬜ Active

**Explanation:** In passive mode, APs do not broadcast SSIDs, so networks won't show in scans.

---

### Question 28

**Match each functional component of AAA with its description.**

| Category           | Description                                                               |
| ------------------ | ------------------------------------------------------------------------- |
| Accounting (A)     | Records what users do and what they access                                |
| Authentication (B) | Proves that users are who they say they are                               |
| Authorization (C)  | Determines what resources users can access or operations they can perform |

---

### Question 29

**Which feature or configuration on a switch makes it vulnerable to VLAN double-tagging attacks?**

* ⬜ The automatic trunking port feature enabled for all ports by default
* ✅ **The native VLAN of the trunking port being the same as a user VLAN**
* ⬜ The limited size of content-addressable memory space
* ⬜ Mixed duplex mode enabled for all ports by default

**Explanation:** VLAN double-tagging exploits the native VLAN to sneak into other VLANs.

---

### Question 30

**A technician is configuring the channel on a wireless router to either 1, 6, or 11. What is the purpose of adjusting the channel?**

* ⬜ To disable broadcasting of the SSID
* ⬜ To provide stronger security modes
* ✅ **To avoid interference from nearby wireless devices**
* ⬜ To enable different 802.11 standards

**Explanation:** Channels 1, 6, and 11 are non-overlapping to reduce wireless interference.

---

If you want, I can format this in **colored styles** (like green for correct, red for incorrect) or generate a neat table! Just let me know.




Here are the answers with all options for **Questions 31 to 33**, including the correct ones and explanations:

---

### Question 31

**Which protocol can be used to monitor the network?**

* ✅ **SNMP**
* ⬜ DHCP
* ⬜ RADIUS
* ⬜ AAA

**Explanation:**
**SNMP** (Simple Network Management Protocol) is designed specifically for network monitoring and management.

---

### Question 32

**What is the function provided by CAPWAP protocol in a corporate wireless network?**

* ⬜ CAPWAP provides the encryption of wireless user traffic between an access point and a wireless client.
* ⬜ CAPWAP provides connectivity between an access point using IPv6 addressing and a wireless client using IPv4 addressing.
* ⬜ CAPWAP creates a tunnel on Transmission Control Protocol (TCP) ports in order to allow a WLC to configure an autonomous access point.
* ✅ **CAPWAP provides the encapsulation and forwarding of wireless user traffic between an access point and a wireless LAN controller.**

**Explanation:**
CAPWAP (Control And Provisioning of Wireless Access Points) is a protocol that encapsulates and forwards wireless traffic between APs and Wireless LAN Controllers.

---

### Question 33

**Which statement describes the behavior of a switch when the MAC address table is full?**

* ⬜ It treats frames as unknown unicast and floods all incoming frames to all ports on the switch.
* ✅ **It treats frames as unknown unicast and floods all incoming frames to all ports within the local VLAN.**
* ⬜ It treats frames as unknown unicast and floods all incoming frames to all ports across multiple switches.
* ⬜ It treats frames as unknown unicast and floods all incoming frames to all ports within the collision domain.

**Explanation:**
When the MAC table is full, the switch floods unknown unicast frames to all ports in the VLAN to ensure delivery.

---

If you'd like, I can continue with more questions or provide explanations in detail!
