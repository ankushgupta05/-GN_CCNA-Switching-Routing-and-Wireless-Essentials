Here are the correct answers with explanations for **2.2.4 Check Your Understanding – Switching Domains**:

---

### **Question 1:**

**Which port speed will be autonegotiated between a host with a 1 Gbps NIC connecting to a Cisco Catalyst 2960 switch with a 100 Mbps port?**

* ⭕ 10 Mbps
* ✅ **100 Mbps**
* ⭕ 1 Gbps
* ⭕ 10 Gbps

**Explanation:** Autonegotiation selects the highest common speed between both devices. The host supports 1 Gbps, but the switch port supports only 100 Mbps, so they settle at **100 Mbps**.

---

### **Question 2:**

**Which device separates broadcast domains?**

* ⭕ Access point
* ⭕ Hub
* ✅ **Router**
* ⭕ Switch

**Explanation:** A **router** separates broadcast domains by default. Switches separate collision domains but not broadcast domains unless VLANs are configured.

---

### **Question 3:**

**Which two special characteristics do LAN switches use to alleviate network congestion? (Choose two.)**

* ✅ **Fast port speeds**
* ✅ **Fast internal switching**
* ⭕ Low port densities
* ⭕ Small frame buffers

**Explanation:**

* **Fast port speeds** allow high-throughput data transfers.
* **Fast internal switching** (e.g., store-and-forward or cut-through) ensures quick frame forwarding.
* **Low port density** and **small frame buffers** would **not** help alleviate congestion—in fact, they can worsen it.

---

Let me know if you'd like these compiled into a notes file or visual summary!










Here are the **correct answers with explanations** for the **2.3.2 Module Quiz – Switching Concepts**:

---

### **Question 1:**

**Which statement is true about broadcast and collision domains?**

* ⭕ Adding a router to a network will increase the size of the collision domain.
* ⭕ The size of the collision domain can be reduced by adding hubs to a network.
* ⭕ The more interfaces a router has the larger the resulting broadcast domain.
* ✅ **Adding a switch to a network will increase the size of the broadcast domain.**

**Explanation:** Switches forward broadcasts out all ports within the same VLAN. So adding switches can expand the broadcast domain unless VLANs or routers are used to segment it.

---

### **Question 2:**

**What is one function of a Layer 2 switch?**

* ⭕ Forwards data based on logical addressing
* ⭕ Duplicates the electrical signal of each frame to every port
* ⭕ Learns the port assigned to a host by examining the destination MAC address
* ✅ **Determines which interface is used to forward a frame based on the destination MAC address**

**Explanation:** Layer 2 switches use **MAC addresses** to determine the correct port for forwarding frames.

---

### **Question 3:**

**What is the significant difference between a hub and a Layer 2 LAN switch?**

* ⭕ A hub divides collision domains, and a switch divides broadcast domains.
* ✅ **A switch creates many smaller collision domains, and a hub increases the size of a single collision domain.**
* ⭕ Each port of a hub is a collision domain, and each port of a switch is a broadcast domain.
* ⭕ A hub forwards frames, and a switch forwards only packets.

**Explanation:** Each port on a switch is its **own collision domain**, reducing collisions. Hubs share one big collision domain, which increases traffic conflicts.

---

### **Question 4:**

**What will a Cisco LAN switch do if it receives an incoming frame and the destination MAC address is not listed in the MAC address table?**

* ⭕ Drop the frame.
* ⭕ Send the frame to the default gateway address.
* ⭕ Use ARP to resolve the port that is related to the frame.
* ✅ **Forward the frame out all ports except the port where the frame is received.**

**Explanation:** This is called **flooding**. The switch floods unknown destination MAC frames to learn where that device is located.

---

### **Question 5:**

**Which switch characteristic helps alleviate network congestion when a 10 Gbps port is forwarding data to a 1 Gbps port?**

* ⭕ Fast internal switching
* ⭕ High port density
* ⭕ Fast port speed
* ✅ **Frame buffering**

**Explanation:** Frame buffering temporarily stores frames in memory during congestion to prevent data loss.

---

### **Question 6:**

**Which switching method makes use of the FCS value?**

* ⭕ Broadcast
* ⭕ Cut-through
* ⭕ Large frame buffer
* ✅ **Store-and-forward**

**Explanation:** **Store-and-forward** receives the entire frame and checks the **FCS (Frame Check Sequence)** for errors before forwarding.

---

### **Question 7:**

**What does the term "port density" represent for an Ethernet switch?**

* ⭕ The memory space that is allocated to each switch port
* ✅ **The number of available ports**
* ⭕ The numbers of hosts that are connected to each switch port
* ⭕ The speed of each port

**Explanation:** Port density refers to how many physical ports are available on the switch.

---

### **Question 8:**

**Which information does a switch use to keep the MAC address table information current?**

* ⭕ The destination MAC address and the incoming port
* ⭕ The destination MAC address and the outgoing port
* ⭕ The source and destination MAC addresses and the incoming port
* ⭕ The source and destination MAC addresses and the outgoing port
* ✅ **The source MAC address and the incoming port**
* ⭕ The source MAC address and the outgoing port

**Explanation:** The switch updates its MAC address table by learning the **source MAC address** from each frame received on a specific port.

---

### **Question 9:**

**Which two statements are true about half-duplex and full-duplex communications?** (Choose two)

* ✅ **Full duplex offers 100 percent potential use of the bandwidth.**
* ⭕ Half duplex has only one channel.
* ⭕ All modern NICs support both half-duplex and full-duplex communication.
* ✅ **Full duplex allows both ends to transmit and receive simultaneously.**
* ⭕ Full duplex increases the effective bandwidth.

**Explanation:**

* **Full duplex** allows simultaneous transmission and reception.
* Full duplex achieves **100% bandwidth utilization**, avoiding collisions.

---

### **Question 10:**

**Which type of address does a switch use to build the MAC address table?**

* ⭕ Destination IP address
* ⭕ Source IP address
* ⭕ Destination MAC address
* ✅ **Source MAC address**

**Explanation:** Switches use the **source MAC address** of incoming frames to learn which device is on which port.

---

### **Question 11:**

**Which option correctly describes a switching method?**

* ⭕ Cut-through: makes a forwarding decision after receiving the entire frame
* ⭕ Store-and-forward: forwards the frame immediately after examining its destination MAC address
* ⭕ Cut-through: provides the flexibility to support any mix of Ethernet speeds
* ✅ **Store-and-forward: ensures that the frame is free of physical and data-link errors**

**Explanation:** Store-and-forward waits for the full frame and verifies it using the **FCS** to ensure there are no errors.

---

### **Question 12:**

**Which network device can serve as a boundary to divide a Layer 2 broadcast domain?**

* ✅ **Router**
* ⭕ Ethernet bridge
* ⭕ Ethernet hub
* ⭕ Access point

**Explanation:** Only **routers** (or Layer 3 devices) separate **broadcast domains** by default.

---

### **Question 13:**

**What is the purpose of frame buffers on a switch?**

* ⭕ They provide a basic security scan on received frames.
* ⭕ They provide temporary storage of the frame checksum.
* ⭕ They execute checksum values before transmission.
* ✅ **They hold traffic, thus alleviating network congestion.**

**Explanation:** Frame buffers temporarily store data to manage traffic congestion during high-load periods.

---

### **Question 14:**

**Which network device can be used to eliminate collisions on an Ethernet network?**

* ⭕ Firewall
* ⭕ Hub
* ⭕ Router
* ✅ **Switch**

**Explanation:** A **switch** eliminates collisions by providing a separate collision domain for each connected device.

---

Let me know if you'd like this in a table format or exported as a study sheet!
