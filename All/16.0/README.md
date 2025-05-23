Here are the **correct answers with explanations** for **Questions 1 to 3**. These answers assume standard routing and Ethernet behavior in a typical network scenario:

---

| **Q#** | **Correct Answer** | **Option Text**      | **Explanation**                                                                                                                                      |
| ------ | ------------------ | -------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1      | ✅ True             | True                 | When a router like **R1** receives a packet and forwards it to another router (e.g., R2), it must encapsulate the packet in a **new Layer 2 frame**. |
| 2      | ✅ False            | False                | Routers **do not use broadcast MAC addresses** (all 1s) to forward frames to other routers. They use the MAC of the **next-hop device**.             |
| 3      | ✅ C                | Sends an ARP request | If **R3** doesn't have an ARP entry for the destination IP, it will **send an ARP request** to resolve the MAC address of the next-hop device.       |

---

If you can upload or describe the **exhibits (network diagrams)** mentioned in the questions, I can give even more precise answers based on the scenario.






Here are the **correct answers** along with **all options and detailed explanations** for the **16.3.4 Module Quiz - Troubleshoot Static and Default Routes**:

---

### ✅ **Question 1:**

**Which sequence correctly identifies the order of the steps that a router will perform when it receives a packet on an Ethernet interface?**

| Option | Steps                                                                                                                                                                                                                     | Correct? | Explanation                                                     |
| ------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------- | --------------------------------------------------------------- |
| A      | 1. The router examines the destination IP address. <br> 2. The router examines the destination MAC address. <br> 3. The router identifies the Ethernet Type field. <br> 4. The router de-encapsulates the Ethernet frame. | ❌        | IP is examined after de-encapsulation.                          |
| B      | 1. The router examines the destination MAC address. <br> 2. The router identifies the Ethernet Type field. <br> 3. The router de-encapsulates the Ethernet frame. <br> 4. The router examines the destination IP address. | ✅        | ✔ Correct order: MAC → Type → De-encap → IP                     |
| C      | 1. The router examines the destination IP address. <br> 2. The router examines the destination MAC address. <br> 3. The router de-encapsulates the Ethernet frame. <br> 4. The router identifies the Ethernet Type field. | ❌        | IP is checked last, after de-encapsulation.                     |
| D      | 1. The router de-encapsulates the Ethernet frame. <br> 2. The router examines the destination MAC address. <br> 3. The router identifies the Ethernet Type field. <br> 4. The router examines the destination IP address. | ❌        | De-encapsulation must happen after MAC check.                   |
| E      | 1. The router examines the destination MAC address. <br> 2. The router identifies the Ethernet Type field. <br> 3. The router examines the destination IP address. <br> 4. The router de-encapsulates the Ethernet frame. | ❌        | IP is inside the frame, not accessible before de-encapsulation. |

**✅ Correct answer: B**

---

### ✅ **Question 2:**

**Which three IOS troubleshooting commands can help to isolate problems with a static route?** *(Choose 3)*

| Option | Command                   | Correct? | Explanation                                                       |
| ------ | ------------------------- | -------- | ----------------------------------------------------------------- |
| A      | `show version`            | ❌        | Displays hardware/software version, not useful for static routes. |
| B      | `ping`                    | ✅        | ✔ Tests reachability of next-hop or destination.                  |
| C      | `tracert`                 | ❌        | ❌ Not a Cisco IOS command; use `traceroute` in IOS.               |
| D      | `show ip route`           | ✅        | ✔ Checks if static route is in the routing table.                 |
| E      | `show ip interface brief` | ✅        | ✔ Verifies interface status (up/down).                            |
| F      | `show arp`                | ❌        | Shows MAC/IP mappings, but not typically for static route issues. |

**✅ Correct answers: B, D, E**

---

### ✅ **Question 3:**

**A static route is not shown in the routing table. Which command verifies that the exit interface is up?**

| Option | Command                   | Correct? | Explanation                                            |
| ------ | ------------------------- | -------- | ------------------------------------------------------ |
| A      | `show ip interface brief` | ✅        | ✔ Verifies status of all interfaces (up/down).         |
| B      | `show ip protocols`       | ❌        | Used for dynamic protocols, not static routes.         |
| C      | `show ip route`           | ❌        | Shows routing table, but not interface state directly. |
| D      | `tracert`                 | ❌        | Not valid in IOS; should be `traceroute`.              |

**✅ Correct answer: A**

---

### ✅ **Question 4:**

**A static route is configured, but the destination network no longer exists. What should be done?**

| Option | Action                         | Correct? | Explanation                                          |
| ------ | ------------------------------ | -------- | ---------------------------------------------------- |
| A      | Change the routing metric      | ❌        | Static routes don't use metrics like dynamic routes. |
| B      | Do nothing                     | ❌        | Static routes stay until manually removed.           |
| C      | Change administrative distance | ❌        | Doesn't remove route, just alters priority.          |
| D      | Remove using `no ip route`     | ✅        | ✔ Correct method to remove static route.             |

**✅ Correct answer: D**

---

### ✅ **Question 5:**

**What does a router do when receiving a packet for another network?**

| Option | Action                                            | Correct? | Explanation                                   |
| ------ | ------------------------------------------------- | -------- | --------------------------------------------- |
| A      | Forwards directly                                 | ❌        | Must route, not direct unless in same subnet. |
| B      | De-encapsulates, selects path, encapsulates again | ✅        | ✔ Correct routing behavior.                   |
| C      | De-encapsulates and forwards                      | ❌        | Must re-encapsulate as well.                  |
| D      | Selects path and forwards                         | ❌        | Needs to examine and encapsulate.             |

**✅ Correct answer: B**

---

### ✅ **Question 6:**

**Purpose of `show cdp neighbors` command?**

| Option | Purpose                    | Correct? | Explanation                                     |
| ------ | -------------------------- | -------- | ----------------------------------------------- |
| A      | Info about Cisco neighbors | ✅        | ✔ CDP reveals directly connected Cisco devices. |
| B      | Advertised networks        | ❌        | That’s for dynamic protocols like OSPF.         |
| C      | Verify attached addresses  | ❌        | Not CDP’s purpose.                              |
| D      | Check PC connectivity      | ❌        | Not relevant to CDP.                            |

**✅ Correct answer: A**

---

### ✅ **Question 7:**

**Static route not showing in table. Which 2 commands help verify exit interface and next-hop reachability?** *(Choose 2)*

| Option | Command                   | Correct? | Explanation                                                   |
| ------ | ------------------------- | -------- | ------------------------------------------------------------- |
| A      | `ping`                    | ✅        | ✔ Check reachability of next-hop address.                     |
| B      | `show ip protocols`       | ❌        | Only for dynamic protocols.                                   |
| C      | `show ip interface brief` | ✅        | ✔ Verifies if the interface is up.                            |
| D      | `show ip route`           | ❌        | Shows route table, but may not help if route isn’t installed. |
| E      | `tracert`                 | ❌        | Not valid IOS command (use `traceroute`).                     |

**✅ Correct answers: A, C**

---

### ✅ **Question 8:**

**Why is this route not in the routing table?**

```bash
ip route 192.168.10.64 255.255.255.192 serial0/0/1
```

| Option | Action                                    | Correct? | Explanation                                       |
| ------ | ----------------------------------------- | -------- | ------------------------------------------------- |
| A      | Re-enter with correct mask                | ❌        | Mask is valid.                                    |
| B      | Verify if interface is active             | ✅        | ✔ Most likely reason: interface is down.          |
| C      | Verify if 192.168.10.64 network is active | ❌        | Static routes don’t depend on that.               |
| D      | Re-enter using network number             | ❌        | 192.168.10.64 **is** the correct network address. |

**✅ Correct answer: B**

---

Let me know if you want these answers in **markdown table format** for your notes or submission.


Here are the correct answers with explanations for **Questions 9 and 10**:

---

### ✅ **Question 9**

**What will a router do if it does not have a default route configured and a packet needs to be forwarded to a destination network that is not listed in the routing table?**

| Option                          | Correct? | Explanation                                                                       |
| ------------------------------- | -------- | --------------------------------------------------------------------------------- |
| A. Forward it to another router | ❌        | It has no idea **where** to send it without a route or default.                   |
| B. **Drop it**                  | ✅        | ✔ If no route matches and no default is present, the router **drops the packet**. |
| C. Send it back to the source   | ❌        | Routers do not send packets back if the route is missing.                         |

**✅ Correct Answer: B – Drop it**

---

### ✅ **Question 10**

**What does the letter `C` mean next to an entry in the output of the `show ip route` command?**

| Option                                                                   | Correct? | Explanation                            |
| ------------------------------------------------------------------------ | -------- | -------------------------------------- |
| A. It identifies a network that is a static route.                       | ❌        | Static routes are marked with `S`.     |
| B. It identifies a network that is learned through OSPF.                 | ❌        | OSPF routes are marked with `O`.       |
| C. It identifies a network that is learned through EIGRP.                | ❌        | EIGRP routes are marked with `D`.      |
| D. **It identifies a network that is directly connected to the router.** | ✅        | ✔ The `C` means **Connected** network. |

**✅ Correct Answer: D – It identifies a network that is directly connected to the router.**

---

Let me know if you'd like all 10 questions compiled in a markdown or PDF format.
