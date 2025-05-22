Here are the **correct answers** for the **4.4.7 Check Your Understanding - Troubleshoot Inter-VLAN Routing** quiz:

---

### **Question 1**

**You are troubleshooting an inter-VLAN issue on a switch and need to verify that the subinterfaces are in the routing table.**
✅ **Correct Answer:** `show ip route`

* ✅ `show ip route` → Displays the routing table, including subinterfaces (e.g., `GigabitEthernet0/0.10`, `0/0.20`, etc.) used in inter-VLAN routing.
* ⬜ `show interfaces`
* ⬜ `show interfaces interface-id switchport`
* ⬜ `show ip interface brief`
* ⬜ `show vlan`

---

### **Question 2**

**You are troubleshooting an inter-VLAN issue on a switch and need to check the list of VLANs and their assigned ports.**
✅ **Correct Answer:** `show vlan`

* ✅ `show vlan` → Shows the VLANs configured on the switch and which ports are assigned to each VLAN.
* ⬜ `show interfaces`
* ⬜ `show interfaces interface-id switchport`
* ⬜ `show ip interface brief`
* ⬜ `show ip route`

---

### **Question 3**

**You are troubleshooting an inter-VLAN issue on a switch and need to verify the status of an access port and its access mode VLAN.**
✅ **Correct Answer:** `show interfaces interface-id switchport`

* ✅ `show interfaces interface-id switchport` → Displays switchport mode, VLAN assignment, and operational status for a specific interface.
* ⬜ `show interfaces`
* ⬜ `show ip interface brief`
* ⬜ `show ip route`
* ⬜ `show vlan`

---

### **Question 4**

**You are troubleshooting an inter-VLAN issue on a switch and need to verify the status and IP address of all interfaces in a condensed format.**
✅ **Correct Answer:** `show ip interface brief`

* ✅ `show ip interface brief` → Provides a summarized view of all interfaces, including status and IP address.
* ⬜ `show interfaces`
* ⬜ `show interfaces interface-id switchport`
* ⬜ `show ip route`
* ⬜ `show vlan`

---

Let me know if you'd like a compiled table with all these answers!






Here are the **answers with all options listed** for the **4.5.4 Module Quiz - Inter-VLAN Routing**:

---

### **Question 1**

**A PC is to access a web server on another network. Which inter-VLAN method will provide the highest bandwidth at Layer 3 and also provide a default gateway for the PC?**

* ⭕ Router on a stick
* ✅ **Multilayer switch with routing enabled**
* ⭕ Trunked interface between the router and the switch
* ⭕ Multiple physical interfaces on the router, all connected to a Layer 2 switch

---

### **Question 2**

**Which scalable method must be implemented in order to provide inter-VLAN routing on a switched network with more than 1000 VLANs?**

* ⭕ Configuring static routes on a Layer 2 switch device
* ✅ **Routing traffic internally to a Layer 3 switch device**
* ⭕ Connecting each physical router interface to a different physical switch port, with each switch port assigned to a different VLAN
* ⭕ Connecting a router interface to a switch port that is configured in trunk mode to route packets between VLANs, with each VLAN assigned to a router subinterface

---

### **Question 3**

**When configuring a router as part of a router-on-a-stick inter-VLAN routing topology, where should the IP address be assigned?**

* ⭕ To the interface
* ✅ **To the subinterface**
* ⭕ To the SVI
* ⭕ To the VLAN

---

### **Question 4**

**A small college uses VLAN 10 for the classroom network and VLAN 20 for the office network. What is needed to enable communication between these two VLANs while using legacy inter-VLAN routing?**

* ✅ **A router with at least two LAN interfaces should be used.**
* ⭕ Two groups of switches are needed, each with ports that are configured for one VLAN.
* ⭕ A router with one VLAN interface is needed to connect to the SVI on a switch.
* ⭕ A switch with a port that is configured as trunk is needed to connect to a router.

---

### **Question 5**

**What is a disadvantage of using multilayer switches for inter-VLAN routing?**

* ⭕ Multilayer switches have higher latency for Layer 3 routing.
* ✅ **Multilayer switches are more expensive than router-on-a-stick implementations.**
* ⭕ Spanning tree must be disabled in order to implement routing on a multilayer switch.
* ⭕ Multilayer switches are limited to using trunk links for Layer 3 routing.

---

### **Question 6**

**Which type of inter-VLAN communication design requires the configuration of multiple subinterfaces?**

* ✅ **Router on a stick**
* ⭕ Routing via a multilayer switch
* ⭕ Routing for the management VLAN
* ⭕ Legacy inter-VLAN routing

---

### **Question 7**

**What is a disadvantage of using router-on-a-stick inter-VLAN routing?**

* ⭕ Does not support VLAN-tagged packets
* ⭕ Requires the use of more physical interfaces than legacy inter-VLAN routing
* ✅ **Does not scale well beyond 50 VLANs**
* ⭕ Requires the use of multiple router interfaces configured to operate as access links

---

### **Question 8**

**What is the meaning of the number 10 in the `encapsulation dot1Q 10 native` router subinterface command?**

* ⭕ The interface number
* ⭕ The subinterface number
* ⭕ The subnet number
* ✅ **The VLAN ID**

---

### **Question 9**

**While configuring inter-VLAN routing on a multilayer switch, a network administrator issues the `no switchport` command on an interface that is connected to another switch. What is the purpose of this command?**

* ✅ **To create a routed port for a single network**
* ⭕ To provide a static trunk link
* ⭕ To create a switched virtual interface
* ⭕ To provide an access link that tags VLAN traffic

---

### **Question 10**

**A network administrator enters the following command sequence on a Cisco 3560 switch. What is the purpose of these commands?**

```
Switch(config)# interface gigabitethernet 0/1  
Switch(config-if)# no switchport  
```

* ⭕ To shut down the Gi0/1 port
* ✅ **To make the Gi0/1 port a routed port**
* ⭕ To enable the Gi0/1 port as a switch virtual interface
* ⭕ To enable the Gi0/1 port as a bridge virtual interface

---

### **Question 11**

**What operational mode should be used on a switch port to connect it to a router for router-on-a-stick inter-VLAN routing?**

* ✅ **Trunk**
* ⭕ Access
* ⭕ Dynamic auto
* ⭕ Dynamic desirable

---

### **Question 12**

**Which sentence correctly describes the SVI inter-VLAN routing method?**

* ⭕ Subinterfaces have to be created.
* ⭕ The encapsulation type must be configured on the SVI.
* ✅ **An SVI is needed for each VLAN.**
* ⭕ A physical interface is needed for every VLAN that is created.

---

### **Question 13**

**How is traffic routed between multiple VLANs on a multilayer switch?**

* ⭕ Traffic is routed via physical interfaces.
* ✅ **Traffic is routed via internal VLAN interfaces.**
* ⭕ Traffic is broadcast out all physical interfaces.
* ⭕ Traffic is routed via subinterfaces.

---

### **Question 14**

**What is required to perform router-on-a-stick inter-VLAN routing?**

* ⭕ A Layer 2 switch that is configured with multiple trunk ports
* ⭕ A router with multiple physical interfaces
* ⭕ A multilayer switch
* ✅ **A router that is configured with multiple subinterfaces**

---

### **Question 15**

**Which two commands can the administrator use in the router to identify VLAN configuration problems? (Choose two.)**

* ⭕ show controllers
* ✅ **show ip interface**
* ⭕ show ip protocols
* ✅ **show running-config**
* ⭕ show vlan

---

Let me know if you want all these in a table format (e.g., for a README or document)!
