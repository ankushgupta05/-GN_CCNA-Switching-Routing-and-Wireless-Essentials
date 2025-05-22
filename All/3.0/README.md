Here are the **correct answers** to the "3.1.5 Check Your Understanding - Overview of VLANs" questions, with **all options shown**:

---

### **Question 1**

**True or False? VLANs improve network performance by segmenting broadcast domains.**
✅ **Correct Answer:** `True`

* ✅ True
* ⬜ False

**Explanation:** VLANs reduce broadcast traffic by segmenting networks into separate broadcast domains, which enhances performance.

---

### **Question 2**

**True or False? VLANs can improve security by isolating sensitive data from the rest of the network.**
✅ **Correct Answer:** `True`

* ✅ True
* ⬜ False

**Explanation:** VLANs isolate traffic, allowing sensitive data to be separated from general network traffic, improving security.

---

### **Question 3**

**Which type of VLAN is assigned to 802.1Q trunk ports to carry untagged traffic?**
✅ **Correct Answer:** `Native`

* ⬜ Default
* ✅ Native
* ⬜ Data
* ⬜ Management

**Explanation:** The **Native VLAN** is used for untagged traffic on an 802.1Q trunk port.

---

### **Question 4**

**True or False? It is a best practice to configure the native VLAN as VLAN 1.**
✅ **Correct Answer:** `False`

* ⬜ True
* ✅ False

**Explanation:** It is **not** best practice to leave the native VLAN as VLAN 1 because it is the default VLAN and could be a security risk.

---

### **Question 5**

**Which is true of VLAN 1? (Choose all that apply.)**
✅ **Correct Answers:**

* ✅ All switch ports are assigned to VLAN 1 by default.
* ✅ The native VLAN is VLAN 1 by default.
* ⬜ The management VLAN is VLAN 1 by default. *(Not always true; management VLAN is configurable.)*
* ✅ VLAN 1 cannot be renamed or deleted.

**Explanation:**

* By default, all switch ports are in VLAN 1.
* VLAN 1 is the default native VLAN.
* VLAN 1 cannot be renamed or deleted.
* The **management VLAN** can be configured and is **not necessarily** VLAN 1.

---

Let me know if you'd like this formatted as a study sheet or table!






Here are the **correct answers** to the “3.2.9 Check Your Understanding – VLANs in a Multi-Switch Environment” activity, based on the described topologies and VLAN configurations:

---

### **Question 1**

**Scenario:**

* PC1 (VLAN 10) sends an ARP broadcast.
* PCs in **VLAN 10**: PC1, PC4 (same VLAN, different switch).
* VLANs segment broadcast domains, so only devices in **VLAN 10** will receive the broadcast.

✅ **Correct Answer:** `PC4`

* ⬜ PC2
* ⬜ PC3
* ✅ PC4
* ⬜ PC5
* ⬜ PC6

---

### **Question 2**

**Scenario:**

* PC2 (VLAN 20) sends an ARP broadcast.
* PCs in **VLAN 20**: PC2, PC5 (same VLAN, different switch).
* Only devices in VLAN 20 will receive the ARP broadcast.

✅ **Correct Answers:**

* ⬜ PC1
* ⬜ PC3
* ⬜ PC4
* ✅ PC5
* ⬜ PC6

---

### **Question 3**

**Scenario:**

* PC3 (VLAN 30) sends an ARP broadcast.
* PCs in **VLAN 30**: PC3, PC6
* Only PC6 is in the same VLAN and will receive the broadcast.

✅ **Correct Answer:** `PC6`

* ⬜ PC1
* ⬜ PC2
* ⬜ PC4
* ⬜ PC5
* ✅ PC6

---

Let me know if you’d like diagrams or tables for easier review!









Here are the **correct answers** to the “3.2.9 Check Your Understanding – VLANs in a Multi-Switch Environment” activity, based on the described topologies and VLAN configurations:

---

### **Question 1**

**Scenario:**

* PC1 (VLAN 10) sends an ARP broadcast.
* PCs in **VLAN 10**: PC1, PC4 (same VLAN, different switch).
* VLANs segment broadcast domains, so only devices in **VLAN 10** will receive the broadcast.

✅ **Correct Answer:** `PC4`

* ⬜ PC2
* ⬜ PC3
* ✅ PC4
* ⬜ PC5
* ⬜ PC6

---

### **Question 2**

**Scenario:**

* PC2 (VLAN 20) sends an ARP broadcast.
* PCs in **VLAN 20**: PC2, PC5 (same VLAN, different switch).
* Only devices in VLAN 20 will receive the ARP broadcast.

✅ **Correct Answers:**

* ⬜ PC1
* ⬜ PC3
* ⬜ PC4
* ✅ PC5
* ⬜ PC6

---

### **Question 3**

**Scenario:**

* PC3 (VLAN 30) sends an ARP broadcast.
* PCs in **VLAN 30**: PC3, PC6
* Only PC6 is in the same VLAN and will receive the broadcast.

✅ **Correct Answer:** `PC6`

* ⬜ PC1
* ⬜ PC2
* ⬜ PC4
* ⬜ PC5
* ✅ PC6

---

Let me know if you’d like diagrams or tables for easier review!



Here are the **correct answers** to the “3.5.6 Check Your Understanding – Dynamic Trunking Protocol” activity:

---

### **Question 1**

**True or false? DTP is an open standard IEEE protocol that specifies auto negotiation of switch trunk links.**
✅ **Correct Answer:** `False`

* ⬜ True
* ✅ False

**Explanation:** DTP (Dynamic Trunking Protocol) is **Cisco proprietary**, not an IEEE open standard.

---

### **Question 2**

**What is the default switchport mode for Cisco Catalyst switches?**
✅ **Correct Answer:** `Dynamic auto`

* ⬜ Access
* ⬜ Trunk
* ✅ Dynamic auto
* ⬜ Dynamic desirable

**Explanation:** Cisco Catalyst switches default to **dynamic auto**, meaning they wait for the other end to initiate trunk negotiation.

---

### **Question 3**

**True or false? Two switchports on a link both configured as dynamic auto will successfully negotiate a trunk.**
✅ **Correct Answer:** `False`

* ⬜ True
* ✅ False

**Explanation:** Two `dynamic auto` ports will **not** form a trunk because neither initiates trunking; both are passive.

---

### **Question 4**

**Which two DTP modes will form a trunk with an interface that is configured as dynamic auto? (Choose two.)**
✅ **Correct Answers:**

* ⬜ Access
* ✅ Trunk
* ⬜ Dynamic auto
* ✅ Dynamic desirable

**Explanation:**

* `Dynamic auto` forms a trunk with:

  * a port set to `trunk` (unconditionally trunks)
  * a port set to `dynamic desirable` (actively negotiates trunking)

---

Let me know if you'd like a summary chart or flashcard version for studying!



Here are the **correct answers** for the **3.6.4 Module Quiz – VLANs** with explanations:

---

### **Question 1**

**What happens to a port that is associated with VLAN 10 when the administrator deletes VLAN 10 from the switch?**
✅ **Correct Answer:** `The port becomes inactive.`

* ✅ The port becomes inactive.
* ⬜ The port goes back to the default VLAN.
* ⬜ The port automatically associates itself with the native VLAN.
* ⬜ The port creates the VLAN again.

**Explanation:** When a VLAN is deleted, any port assigned to it becomes inactive until it's assigned to a valid VLAN.

---

### **Question 2**

**In which memory location are the VLAN configurations of normal range VLANs stored on a Catalyst switch?**
✅ **Correct Answer:** `Flash`

* ✅ Flash
* ⬜ NVRAM
* ⬜ RAM
* ⬜ ROM

**Explanation:** VLAN configurations are stored in the `vlan.dat` file, which resides in **Flash** memory.

---

### **Question 3**

**Why aren’t the switches negotiating a trunk?**
✅ **Correct Answer:** `Switches from other vendors do not support DTP.`

* ⬜ Both switches are in trunk mode.
* ⬜ Both switches are in nonegotiate mode.
* ✅ Switches from other vendors do not support DTP.
* ⬜ DTP frames are flooding the entire network.

**Explanation:** **DTP is Cisco proprietary**, so it doesn't work with non-Cisco switches unless manually configured.

---

### **Question 4**

**What is the purpose of the vlan.dat file on a switch?**
✅ **Correct Answer:** `It holds the VLAN database.`

* ⬜ It holds the running configuration.
* ⬜ It holds the saved configuration.
* ✅ It holds the VLAN database.
* ⬜ It holds the operating system.

**Explanation:** The `vlan.dat` file stores VLAN information like IDs and names.

---

### **Question 5**

**What is the purpose of setting the native VLAN separate from data VLANs?**
✅ **Correct Answer:** `A separate VLAN should be used to carry uncommon untagged frames to avoid bandwidth contention on data VLANs.`

* ⬜ The native VLAN is for carrying VLAN management traffic only.
* ⬜ The security of management frames that are carried in the native VLAN can be enhanced.
* ✅ A separate VLAN should be used to carry uncommon untagged frames to avoid bandwidth contention on data VLANs.
* ⬜ The native VLAN is for routers and switches to exchange their management information.

**Explanation:** Separating native VLAN from data VLANs improves security and isolates untagged traffic.

---

### **Question 6**

**When a Cisco switch receives untagged frames on a 802.1Q trunk port, which VLAN ID is the traffic switched to by default?**
✅ **Correct Answer:** `Native VLAN ID`

* ⬜ Unused VLAN ID
* ✅ Native VLAN ID
* ⬜ Data VLAN ID
* ⬜ Management VLAN ID

**Explanation:** Untagged traffic on a trunk port is associated with the **native VLAN** by default.

---

### **Question 7**

**Which two types of point-to-point connections utilize VLAN trunking?**
✅ **Correct Answers:**

* ✅ Between two switches that utilize multiple VLANs

* ✅ Between a switch and a server that has an 802.1Q NIC

* ✅ Between two switches that utilize multiple VLANs

* ⬜ Between a switch and a client PC

* ✅ Between a switch and a server that has an 802.1Q NIC

* ⬜ Between a switch and a network printer

* ⬜ Between two switches that share a common VLAN

**Explanation:** Trunking is used when devices (like switches or VLAN-aware servers) need to carry multiple VLANs.

---

### **Question 8**

**What are three primary benefits of using VLANs?**
✅ **Correct Answers:**

* ✅ Security

* ✅ Cost reduction

* ✅ Improved IT Staff efficiency

* ✅ Security

* ⬜ A reduction in the number of trunk links

* ✅ Cost reduction

* ⬜ End user satisfaction

* ✅ Improved IT Staff efficiency

**Explanation:** VLANs segment the network, improve security, reduce unnecessary traffic, and make network management easier and more cost-effective.

---

Let me know if you want a downloadable version or printable summary!










Here are the **correct answers** for **Questions 9 to 15** of the VLAN module quiz, along with explanations:

---

### **Question 9**

**On a Cisco switch, where is extended range VLAN information stored?**
✅ **Correct Answer:** `Running configuration file`

* ✅ Running configuration file
* ⬜ Startup configuration file
* ⬜ NVRAM
* ⬜ Flash

**Explanation:** Extended range VLANs (1006–4094) are stored in the **running configuration**, not in the `vlan.dat` file.

---

### **Question 10**

**In which location are the normal range VLANs stored on a Cisco switch by default?**
✅ **Correct Answer:** `Flash memory`

* ✅ Flash memory
* ⬜ Startup-config
* ⬜ Running-config
* ⬜ RAM

**Explanation:** Normal range VLANs (1–1005) are stored in the **vlan.dat** file located in **Flash memory**.

---

### **Question 11**

**Which distinct type of VLAN is used by an administrator to access and configure a switch?**
✅ **Correct Answer:** `Management VLAN`

* ⬜ Default VLAN
* ⬜ Native VLAN
* ⬜ Data VLAN
* ✅ Management VLAN

**Explanation:** The **management VLAN** is used to remotely access and configure the switch, typically via SSH or Telnet.

---

### **Question 12**

**For what reason would a network administrator use the `show interfaces trunk` command on a switch?**
✅ **Correct Answer:** `To view the native VLAN`

* ✅ To view the native VLAN
* ⬜ To examine DTP negotiation as it occurs
* ⬜ To verify port association with a particular VLAN
* ⬜ To display an IP address for any existing VLAN

**Explanation:** `show interfaces trunk` displays trunk interfaces, allowed VLANs, and the **native VLAN** for each trunk.

---

### **Question 13**

**Where is the vlan.dat file stored on a switch?**
✅ **Correct Answer:** `In flash memory`

* ⬜ In RAM
* ⬜ In NVRAM
* ✅ In flash memory
* ⬜ On the externally attached storage media or internal hard drive

**Explanation:** The **vlan.dat** file that stores normal range VLAN info is located in **Flash memory**.

---

### **Question 14**

**What design feature must be considered for Cisco IP phones to ensure voice quality?**
✅ **Correct Answer:** `A separate VLAN is needed for voice traffic.`

* ⬜ Voice traffic needs to be tagged with the native VLAN.
* ✅ A separate VLAN is needed for voice traffic.
* ⬜ Additional switch ports dedicated to Cisco IP phones are required.
* ⬜ Voice and data traffic require separate trunk links.

**Explanation:** Voice traffic should be placed in a **separate VLAN** from data to ensure QoS and prioritize voice traffic.

---

### **Question 15**

**Effect of issuing `switchport trunk allowed vlan 30` on Fa0/5 when it currently allows VLANs 10 and 20?**
✅ **Correct Answer:** `It allows only VLAN 30 on Fa0/5.`

* ⬜ It allows VLANs 1 to 30 on Fa0/5.
* ⬜ It allows VLANs 10, 20, and 30 on Fa0/5.
* ✅ It allows only VLAN 30 on Fa0/5.
* ⬜ It allows a native VLAN of 30 to be implemented on Fa0/5.

**Explanation:** The command **replaces** the current VLAN list with **only VLAN 30** on the trunk port.

---

Let me know if you'd like a compiled answer key for all questions!
