Here are the questions from **9.1.5 Check Your Understanding - First Hop Redundancy Protocols** with all options and the correct answers marked:

---

### Question 1

What type of device routes traffic destined to network segments beyond the source network segment for which the sending node may not have explicit routing information?

* ⬜ Virtual router
* ⬜ Standby router
* ✔️ Default gateway
* ⬜ Layer 3 switch

---

### Question 2

What device presents the illusion of a single router to hosts on a LAN segment but actually represents a set of routers working together?

* ✔️ Virtual router
* ⬜ Forwarding router
* ⬜ Default gateway
* ⬜ Layer 3 switch

---

### Question 3

What device is part of a virtual router group assigned the role of alternate default gateway?

* ⬜ Virtual router
* ✔️ Standby router
* ⬜ Default gateway
* ⬜ Layer 3 switch

---

### Question 4

What device that is part of a virtual router group assigned to the role of default gateway?

* ⬜ Virtual router
* ✔️ Forwarding router
* ⬜ Default gateway
* ⬜ Layer 3 switch

---

### Question 5

Which FHRPs are Cisco-proprietary? (Choose two.)

* ⬜ IRDP
* ✔️ HSRP
* ✔️ HSRP for IPv6
* ⬜ VRRPv2

---

If you want me to continue with more questions or explanations, just say!


Thanks for pointing that out! Let's correct the answers for questions 2 and 4.

Here’s the corrected version:

---

### Question 1

What is the default HSRP priority?

* ⬜ 50
* ✔️ 100
* ⬜ 150
* ⬜ 255

---

### Question 2

True or False? If a router with a higher HSRP priority joins the network, it will take over the active router role from an existing active router which has a lower priority.

* ⬜ True
* ✔️ False

**Explanation:** A router with a higher priority will take over the active role only during initial election or if the active router fails. It will not preempt the current active router unless preemption is enabled.

---

### Question 3

During which HSRP state does an interface begin sending periodic hello messages?

* ⬜ Initial
* ⬜ Listen
* ✔️ Speak
* ⬜ Active

---

### Question 4

Which is a characteristic of the HSRP learn state?

* ✔️ The router has not determined the virtual IP address
* ⬜ The router knows the virtual IP address
* ⬜ The router sends periodic hello messages
* ⬜ The router actively participates in the active/standby election process

---

Let me know if you want more detailed explanations!



Sure! Here’s the full quiz with **all options** and the **correct answers** marked clearly:

---

### Question 1

**What is the purpose of HSRP?**

* ⬜ It prevents a rogue switch from becoming the STP root.
* ⬜ It enables an access port to immediately transition to the forwarding state.
* ⬜ It prevents malicious hosts from connecting to trunk ports.
* **✅ It provides a continuous network connection when a router fails.**

---

### Question 2

**Which nonproprietary protocol provides router redundancy for a group of routers which support IPv4 LANs?**

* ⬜ HSRP
* **✅ VRRPv2**
* ⬜ GLBP
* ⬜ SLB

---

### Question 3

**A network administrator is analyzing first-hop router redundancy protocols. What is a characteristic of VRRPv3?**

* ⬜ VRRPv3 is Cisco proprietary.
* **✅ It supports IPv6 and IPv4 addressing.**
* ⬜ It works together with HSRP.
* ⬜ It allows load balancing between routers.

---

### Question 4

**What is a potential disadvantage when implementing HSRP as compared to GLBP?**

* ⬜ HSRP does not function in a multivendor environment.
* **✅ HSRP does not provide load balancing with multiple active routers.**
* ⬜ HSRP does not have the capability to support IPv6 addresses.
* ⬜ HSRP provides default gateway failover only when the active router fails.

---

### Question 5

**A network engineer is configuring a LAN with a redundant first hop to make better use of the available network resources. Which protocol should the engineer implement?**

* ⬜ FHRP
* **✅ GLBP**
* ⬜ HSRP
* ⬜ VRRP

---

### Question 6

**When first hop redundancy protocols are used, which two items will be shared by a set of routers that are presenting the illusion of being a single router? (Choose two.)**

* ⬜ Hostname
* **✅ IP address**
* ⬜ BID
* ⬜ Static route
* **✅ MAC address**

---

### Question 7

**In FHRP terminology, what represents a set of routers that present the illusion of a single router to hosts?**

* ⬜ Standby router
* **✅ Virtual router**
* ⬜ Forwarding router
* ⬜ Default gateway

---

### Question 8

**A user needs to add redundancy to the routers in a company. What are the three options the user can use? (Choose three.)**

* **✅ HSRP**
* **✅ VRRP**
* ⬜ STP
* ⬜ IPFIX
* ⬜ RAID
* **✅ GLBP**

---

### Question 9

**Which two protocols provide gateway redundancy at Layer 3? (Choose two.)**

* **✅ VRRP**
* ⬜ STP
* ⬜ PVST
* ⬜ RSTP
* **✅ HSRP**

---

### Question 10

**A network administrator is overseeing the implementation of first hop redundancy protocols. Which two protocols are Cisco proprietary? (Choose two.)**

* **✅ HSRP**
* ⬜ VRRP
* **✅ GLBP**
* ⬜ IRDP
* ⬜ VRRPv2

---

### Question 11

**Which statement describes a characteristic of GLBP?**

* ⬜ It does not provide support for IPv6.
* **✅ It provides load balancing for a maximum of four gateways.**
* ⬜ It provides multiple virtual IP addresses and multiple virtual MAC addresses.
* ⬜ It provides automatic rerouting if any router in the group fails.

---

### Question 12

**A network administrator is analyzing the features that are supported by different first-hop router redundancy protocols. Which statement is a feature that is associated with GLBP?**

* **✅ GLBP allows load balancing between routers.**
* ⬜ It is nonproprietary.
* ⬜ It uses a virtual router master.
* ⬜ It works together with VRRP.

---

If you want, I can also add explanations for the answers!



