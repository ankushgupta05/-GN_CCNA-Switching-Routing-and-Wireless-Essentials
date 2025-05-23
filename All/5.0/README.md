Here’s the **Check Your Understanding - Purpose of STP** section in a clear table format, with **all options**, correct answers marked, and explanations included:

---

### 📘 **5.1.10 Check Your Understanding – Purpose of STP**

| **Q#** | **Question**                                                                                                                 | **Options**                                                                                                                                                                                                                                  | **Correct Answer** | **Explanation**                                                                                                                              |
| ------ | ---------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------ | -------------------------------------------------------------------------------------------------------------------------------------------- |
| 1      | Which statement describes STP?                                                                                               | a) STP is a Layer 2 routing protocol. <br> b) STP is a Layer 3 routing protocol for Ethernet LANs. <br> c) STP is a Layer 2 loop prevention protocol for Ethernet LANs. ✅ <br> d) STP is a Layer 3 loop prevention protocol for IP networks. | **c**              | STP (Spanning Tree Protocol) works at Layer 2 to prevent loops in Ethernet LANs by blocking redundant paths.                                 |
| 2      | Without STP on the Ethernet LAN, which three types of frames could cause a catastrophic loop in the network? (Choose three.) | a) Unicast ❌ <br> b) Unknown unicast ✅ <br> c) Multicast ✅ <br> d) Broadcast ✅                                                                                                                                                               | **b, c, d**        | Without STP, frames like broadcast, multicast, and unknown unicast keep looping in the network, causing congestion and instability.          |
| 3      | What device is elected by the Spanning Tree Algorithm? All other switches determine a single least-cost path to this device. | a) Root bridge ✅ <br> b) Dedicated bridge ❌ <br> c) Default gateway ❌ <br> d) Core switch ❌                                                                                                                                                  | **a**              | The **root bridge** is the logical center of the STP topology. All switches compute the shortest path to it to maintain a loop-free network. |

---

Let me know if you'd like this converted into a Markdown file (`README.md`) or exported in another format!



Here’s the **Check Your Understanding – STP Operations (5.2.12)** section with **all options**, **correct answers marked**, and **explanations** in a clear table format:

---

### 📘 **5.2.12 Check Your Understanding – STP Operations**

| **Q#** | **Question**                                                                                              | **Options**                                                                                                                      | **Correct Answer** | **Explanation**                                                                                                                      |
| ------ | --------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- | ------------------ | ------------------------------------------------------------------------------------------------------------------------------------ |
| 1      | By default (without any configuration on a switch), what will determine which switch is the root bridge?  | a) The bridge priority ❌ <br> b) The extended system ID ❌ <br> c) The MAC address of the switch ❌ <br> d) The bridge ID ✅        | **d**              | The root bridge is elected based on the **lowest bridge ID**, which is a combination of the **bridge priority** and **MAC address**. |
| 2      | The root bridge will be the switch with the:                                                              | a) Lowest bridge ID ✅ <br> b) Highest bridge ID ❌ <br> c) Lowest port priority ❌ <br> d) Highest port priority ❌                 | **a**              | STP selects the root bridge by choosing the switch with the **lowest bridge ID** (priority + MAC).                                   |
| 3      | The port closest to the root bridge in terms of least overall cost (best path) to the root bridge is the: | a) Designated port ❌ <br> b) Blocked port or non-designated port ❌ <br> c) Root port ✅ <br> d) Routed Port ❌                     | **c**              | The **Root Port** is the port on a non-root switch that has the least-cost path to the root bridge.                                  |
| 4      | The port on the segment (with two switches) that has the lowest path cost to the root bridge is the:      | a) Designated port ✅ <br> b) Blocked port or non-designated port ❌ <br> c) Root port ❌ <br> d) Routed Port ❌                     | **a**              | A **Designated Port** is selected on each network segment. It's the port with the lowest cost to the root bridge for that segment.   |
| 5      | Which of the following ports will forward Ethernet frames? (Choose two.)                                  | a) Designated port ✅ <br> b) Blocked port or non-designated port ❌ <br> c) Root port ✅                                           | **a, c**           | Only **Designated Ports** and **Root Ports** forward frames. Blocked ports do not.                                                   |
| 6      | The sum of individual port costs along the path from the switch to the root bridge is known as the:       | a) Least cost path ❌ <br> b) Shortest path cost ❌ <br> c) Best path cost ❌ <br> d) Root path cost ✅                              | **d**              | **Root Path Cost** is the total cost from a switch to the root bridge, used in calculating the shortest path.                        |
| 7      | How often does a switch send a BPDU?                                                                      | a) Every 2 seconds ✅ <br> b) Every 15 seconds ❌ <br> c) Every 20 seconds ❌ <br> d) Only when there is a change in the topology ❌ | **a**              | **BPDUs (Bridge Protocol Data Units)** are sent every **2 seconds** by default to maintain STP topology information.                 |

---

Let me know if you'd like this exported to a file like `README.md`, PDF, or Excel!






Here's the **5.3.6 Check Your Understanding – Evolution of STP** section with **all options**, **correct answers**, and **clear explanations** in table format:

---

### 📘 **5.3.6 Check Your Understanding – Evolution of STP**

| **Q#** | **Question**                                                                                                                               | **Options**                                                                                  | **Correct Answer(s)** | **Explanation**                                                                                                                                  |
| ------ | ------------------------------------------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------- | --------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------ |
| 1      | Which three STP port states are merged into the RSTP discarding port state? (Choose three.)                                                | a) Disabled ✅ <br> b) Blocking ✅ <br> c) Listening ✅ <br> d) Learning ❌ <br> e) Forwarding ❌ | **a, b, c**           | In **RSTP**, the port states **Disabled**, **Blocking**, and **Listening** are all replaced by a single state called **Discarding**.             |
| 2      | Which protocol was designed to bring faster convergence to STP?                                                                            | a) PortFast ❌ <br> b) RSTP ✅ <br> c) PVST ❌ <br> d) MSTP ❌                                   | **b**                 | **Rapid Spanning Tree Protocol (RSTP)** improves convergence time over traditional STP.                                                          |
| 3      | Which technology solves the problem of a device being unable to get an IPv4 address from a DHCP server due to STP forwarding delay timers? | a) PortFast ✅ <br> b) BPDU guard ❌ <br> c) PVST ❌ <br> d) MSTP ❌                             | **a**                 | **PortFast** allows a port to bypass STP listening/learning states and go straight to forwarding, enabling fast device connectivity (like DHCP). |

---

Let me know if you’d like the answers compiled into a markdown or PDF file for easier review.











Here is the **5.4.2 Module Quiz – STP** with all options, correct answers, and explanations in a clear table format:

---

### 📘 **5.4.2 Module Quiz – Spanning Tree Protocol (STP)**

| **Q#** | **Question**                                                                               | **Options**                                                                                                                                                                                      | **Correct Answer(s)** | **Explanation**                                                                                               |
| ------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | --------------------- | ------------------------------------------------------------------------------------------------------------- |
| 1      | Which port state will switch ports immediately transition to when configured for PortFast? | a) Listening ❌<br>b) Learning ❌<br>c) Forwarding ✅<br>d) Blocking ❌                                                                                                                              | **c**                 | PortFast causes a port to skip listening/learning states and go directly to **Forwarding**.                   |
| 2      | After the election of the root bridge, how do switches find the best paths?                | a) Fewest hops ❌<br>b) Lowest BID neighbors ❌<br>c) Port states ❌<br>d) Sum of port costs ✅                                                                                                      | **d**                 | STP uses **cumulative port costs** to determine the best path to the root bridge.                             |
| 3      | Default STP mode on Cisco Catalyst switches?                                               | a) RSTP ❌<br>b) PVST+ ✅<br>c) MST ❌<br>d) MSTP ❌<br>e) Rapid PVST+ ❌                                                                                                                             | **b**                 | Cisco Catalyst switches use **PVST+** by default (Per VLAN Spanning Tree Plus).                               |
| 4      | What value determines the root bridge (default config)?                                    | a) VLAN ID ❌<br>b) MAC address ✅<br>c) Extended system ID ❌<br>d) Bridge priority ❌                                                                                                              | **b**                 | With default settings, all switches have the same priority, so the **lowest MAC address** becomes root.       |
| 5      | First step of spanning-tree election after reboot?                                         | a) Lower root ID doesn’t send BPDUs ❌<br>b) All advertise as root ✅<br>c) Determine best path ❌<br>d) Block loop ports ❌                                                                         | **b**                 | Initially, **all switches believe they are the root** and send BPDUs announcing this.                         |
| 6      | Concepts for ports with only end devices (Choose two)                                      | a) Bridge ID ❌<br>b) Edge port ✅<br>c) Extended system ID ❌<br>d) PortFast ✅<br>e) PVST+ ❌                                                                                                       | **b, d**              | **Edge ports** are intended for end devices. **PortFast** is often enabled on them.                           |
| 7      | Port states used by Rapid PVST+ (Choose three)                                             | a) Discarding ✅<br>b) Blocking ❌<br>c) Trunking ❌<br>d) Listening ❌<br>e) Learning ✅<br>f) Forwarding ✅                                                                                          | **a, e, f**           | Rapid PVST+ uses only **Discarding**, **Learning**, and **Forwarding** states.                                |
| 8      | In PVST, which state can forward BPDUs but not data frames?                                | a) Blocking ✅<br>b) Listening ❌<br>c) Forwarding ❌<br>d) Disabled ❌                                                                                                                              | **a**                 | **Blocking** ports do not forward data but can process and forward **BPDUs**.                                 |
| 9      | Which port becomes the root port?                                                          | a) Designated ❌<br>b) Root port ✅<br>c) Alternate ❌<br>d) Disabled ❌                                                                                                                             | **b**                 | The **Root Port** is the port with the **lowest path cost** to the root bridge.                               |
| 10     | PortFast switch port behavior (Choose two)                                                 | a) From listening to forwarding ❌<br>b) From blocking to forwarding ✅<br>c) Should never receive BPDUs ✅<br>d) Processes BPDUs before forwarding ❌<br>e) Sends DHCP requests before forwarding ❌ | **b, c**              | **PortFast** transitions ports immediately to forwarding and is for **end devices**, not for receiving BPDUs. |
| 11     | One way to fix spanning tree failure?                                                      | a) Replace STP with RSTP ❌<br>b) Insert redundant links ❌<br>c) Replace cables ❌<br>d) Manually remove redundant links ✅                                                                         | **d**                 | A common fix is to **eliminate redundant links** manually in the absence of functioning STP.                  |
| 12     | What info is in the 12-bit extended system ID in a BPDU?                                   | a) MAC address ❌<br>b) VLAN ID ✅<br>c) IP address ❌<br>d) Port ID ❌                                                                                                                              | **b**                 | The **extended system ID** includes the **VLAN ID**, allowing unique BIDs per VLAN.                           |
| 13     | Command to verify if switch is root bridge?                                                | a) show spanning-tree ✅<br>b) show running-config ❌<br>c) show startup-config ❌<br>d) show vlan ❌                                                                                                | **a**                 | `**show spanning-tree**` displays the **bridge role**, including if it’s root.                                |
| 14     | What is redundancy?                                                                        | a) MAC address DB ❌<br>b) Interface security ❌<br>c) Multiple virtual devices ❌<br>d) Multiple switch paths ✅                                                                                    | **d**                 | **Redundancy** means **multiple paths between switches** to prevent a single point of failure.                |

---

Would you like this in Markdown, PDF, or added to a study guide?


