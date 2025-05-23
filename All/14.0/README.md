Here are the answers with all options for **14.1.7 Check Your Understanding - Path Determination** Questions 1 to 4:

---

### Question 1

**What table does a router use to determine how to forward an IP packet?**

* ⬜ ARP table
* ⬜ MAC address table
* ⬜ Neighbor cache
* ✅ **Routing table**

**Explanation:**
Routers use the **routing table** to decide where to forward IP packets based on destination IP addresses.

---

### Question 2

**What action will a router take on a packet with a destination IP address that is on a remote network?**

* ⬜ It will forward the packet directly to the device with the destination IP address of the packet.
* ✅ **It will forward the packet to a next-hop router.**
* ⬜ It will forward the packet to an Ethernet switch.
* ⬜ It will drop the packet.

**Explanation:**
For remote networks, routers forward packets to the next-hop router toward the destination.

---

### Question 3

**Which of the following routes may be found in a routing table? (Choose all that apply.)**

* ✅ **Directly connected networks**
* ✅ **Static routes**
* ✅ **Dynamic routing protocol routes**
* ✅ **Default route**

**Explanation:**
Routing tables can contain all these types of routes: directly connected, static, dynamic, and default.

---

### Question 4

**What is used to determine the minimum number of far-left bits that must match between the prefix in the route entry and the destination IP address?**

* ✅ **Prefix length in the routing table entry**
* ⬜ Prefix length of the destination IP address
* ⬜ The classful address of the network address

**Explanation:**
The **prefix length** (also called subnet mask length) defines how many leftmost bits must match in routing decisions.

---

Want me to continue with more questions?



Here are the answers for **14.2.4 Check Your Understanding - Packet Forwarding** questions 1 to 3 with all options:

---

### Question 1

**If a router needs to send an ARP Request for the destination IPv4 address of the packet, this means the packet will be forwarded:**

* ⬜ To a next-hop router
* ✅ **To the device with the destination IPv4 address of the packet**

**Explanation:**
If the router sends an ARP request for the destination IPv4 address, it means the destination is on a directly connected network, so the packet will be forwarded directly to the device.

---

### Question 2

**If a router needs to send an ARP Request for the IPv4 address in one of its route entries, this means the packet will be forwarded:**

* ✅ **To a next-hop router**
* ⬜ To the device with the destination IPv4 address of the packet

**Explanation:**
If the ARP request is for the next-hop IP address (from the route entry), the packet will be forwarded to the next-hop router, not directly to the destination.

---
Thanks for catching that! Let me correct it:

---

### Question 3

**Which packet forwarding method is used by default on Cisco routers?**

* ⬜ Process switching
* ⬜ Fast switching
* ✅ **Cisco Express Forwarding**
* ⬜ Ethernet switching

**Correct Explanation:**
Modern Cisco routers use **Cisco Express Forwarding (CEF)** as the default packet forwarding method because it is the most efficient, using a forwarding information base (FIB) and adjacency tables to speed up packet forwarding and reduce CPU load.

---

So the corrected answer for Question 3 is **Cisco Express Forwarding** (CEF).

---

If you want, I can help with more questions or explain why the other methods are less commonly the default!
