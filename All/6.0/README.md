Here's the **EtherChannel Quiz** with **all options**, including the correct answers clearly marked and explanations for each:

---

### ✅ **Question 1: Which are benefits of EtherChannel technology? (Choose all that apply.)**

| Option              | Correct? | Explanation                                                             |
| ------------------- | -------- | ----------------------------------------------------------------------- |
| Fault-tolerance     | ✅        | EtherChannel provides redundancy; if one link fails, traffic continues. |
| Load sharing        | ✅        | EtherChannel distributes traffic across links for better performance.   |
| Increased bandwidth | ✅        | Multiple links combine to increase the effective bandwidth.             |
| Link redundancy     | ✅        | Multiple links provide backup if one fails, reducing downtime.          |

---

### ✅ **Question 2: True or False? FastEthernet and GigabitEthernet links can be combined into a single EtherChannel.**

| Option | Correct? | Explanation                                                                    |
| ------ | -------- | ------------------------------------------------------------------------------ |
| True   | ❌        | All links must be of the **same type and speed** to form a valid EtherChannel. |
| False  | ✅        | Mixing FastEthernet and GigabitEthernet is not allowed.                        |

---

### ✅ **Question 3: True or False? PAgP and LACP are both Cisco-proprietary link aggregation protocols.**

| Option | Correct? | Explanation                                                                      |
| ------ | -------- | -------------------------------------------------------------------------------- |
| True   | ❌        | **Only PAgP** is Cisco proprietary; **LACP is an open standard** (IEEE 802.3ad). |
| False  | ✅        | Correct — LACP is **not** Cisco-proprietary.                                     |

---

### ✅ **Question 4: Which three are PAgP interface modes? (Choose three.)**

| Option    | Correct? | Explanation                                              |
| --------- | -------- | -------------------------------------------------------- |
| On        | ✅        | Forces EtherChannel without negotiation.                 |
| Auto      | ✅        | Passive mode; waits for negotiation from the other side. |
| Active    | ❌        | **LACP** mode, not used in PAgP.                         |
| Passive   | ❌        | **LACP** mode, not used in PAgP.                         |
| Desirable | ✅        | Actively negotiates PAgP EtherChannel.                   |

---

### ✅ **Question 5: Which PAgP interface mode will initiate negotiation with other interfaces?**

| Option    | Correct? | Explanation                                                          |
| --------- | -------- | -------------------------------------------------------------------- |
| On        | ❌        | "On" does not use negotiation; it forces channeling.                 |
| Desirable | ✅        | Actively initiates PAgP negotiation.                                 |
| Auto      | ❌        | Waits for the other side to initiate; does not initiate negotiation. |

---

### ✅ **Question 6: Which combinations of PAgP modes will form an EtherChannel? (Choose all that apply.)**

| Combination      | Correct? | Explanation                                                          |
| ---------------- | -------- | -------------------------------------------------------------------- |
| Auto > Desirable | ✅        | Valid — Desirable initiates, Auto responds.                          |
| Desirable > On   | ❌        | Invalid — "On" doesn’t participate in negotiation.                   |
| Auto > On        | ❌        | Invalid — "Auto" won’t initiate, and "On" doesn’t negotiate.         |
| On > On          | ✅        | Valid — "On" forces the EtherChannel on both sides.                  |
| On > Active      | ❌        | Invalid — Active is an **LACP** mode, not compatible with PAgP.      |
| Active > Passive | ❌        | Invalid — This is an **LACP** negotiation combo, not used with PAgP. |

---

Let me know if you'd like this exported to a markdown (`README.md`) or PDF format!







Here are the **correct answers** for the **6.4.4 Module Quiz – EtherChannel**, with **all options** and **explanations**:

---

### ✅ **Question 1**

**An EtherChannel link using LACP was formed between two switches, S1 and S2. While verifying the configuration, which mode combination could be utilized on both switches?**

| Option                    | Correct? | Explanation                                                               |
| ------------------------- | -------- | ------------------------------------------------------------------------- |
| S1-on and S2-passive      | ❌        | “On” forces channeling, "passive" waits for LACP packets; not compatible. |
| S1-passive and S2-passive | ❌        | Both sides are waiting; channel will not form.                            |
| S1-on and S2-active       | ❌        | “On” does not use negotiation protocols; incompatible with “active”.      |
| S1-passive and S2-active  | ✅        | Valid LACP combination; active initiates, passive responds.               |

---

### ✅ **Question 2**

**When a range of ports is being configured for EtherChannel, which mode will configure PAgP so that it initiates the EtherChannel negotiation?**

| Option    | Correct? | Explanation                                 |
| --------- | -------- | ------------------------------------------- |
| Active    | ❌        | Used with LACP, not PAgP.                   |
| Auto      | ❌        | Waits for negotiation; doesn’t initiate it. |
| Desirable | ✅        | Initiates PAgP negotiation.                 |
| Passive   | ❌        | Used with LACP, not PAgP.                   |

---

### ✅ **Question 3**

**Which three interface parameters must match for an EtherChannel to form?** (Choose three)

| Option              | Correct? | Explanation                                                                |
| ------------------- | -------- | -------------------------------------------------------------------------- |
| Allowed VLANs       | ✅        | Must match for trunk ports.                                                |
| EtherChannel mode   | ✅        | Modes must be compatible (e.g., LACP active/passive).                      |
| Native VLAN         | ✅        | Important for trunk links; must be the same.                               |
| PortFast mode       | ❌        | Not related to EtherChannel formation.                                     |
| Spanning-tree state | ❌        | Automatically managed by STP; doesn’t need to match.                       |
| Trunking mode       | ✅        | (if more than 3 correct allowed) All ports must be either access or trunk. |

---

### ✅ **Question 4**

**What are three advantages of using EtherChannel technology?** (Choose three)

| Option                                                                                         | Correct? | Explanation                                                                  |
| ---------------------------------------------------------------------------------------------- | -------- | ---------------------------------------------------------------------------- |
| EtherChannel uses multiple logical links to provide redundancy.                                | ❌        | EtherChannel uses **physical** links, not multiple logical ones.             |
| Configuration tasks can be done on the EtherChannel interface.                                 | ✅        | Yes, simplifying configuration and management.                               |
| There is no need to upgrade links to faster connections to increase bandwidth.                 | ✅        | Combining links increases bandwidth without upgrading to higher-speed links. |
| Load balancing is not needed with EtherChannel.                                                | ❌        | Load balancing is used across the links in EtherChannel.                     |
| The Spanning Tree Protocol shuts down the unused interfaces in the bundle to avoid loops.      | ❌        | STP sees EtherChannel as one link; does not block individual links.          |
| A spanning tree recalculation is not required when a single link within the channel goes down. | ✅        | Yes, this avoids STP reconvergence and improves stability.                   |

---

### ✅ **Question 5**

**A network administrator is configuring an EtherChannel link between two physical ports on a switch. Which statement describes the result when one of the physical ports fails?**

| Option                                                               | Correct? | Explanation                                                   |
| -------------------------------------------------------------------- | -------- | ------------------------------------------------------------- |
| The EtherChannel link fails.                                         | ❌        | Only one link fails; the channel remains up with fewer links. |
| An STP recalculation is needed.                                      | ❌        | STP sees EtherChannel as one link; no recalculation needed.   |
| The EtherChannel stops transmitting data until it is restarted.      | ❌        | No; it continues with reduced bandwidth.                      |
| The EtherChannel continues transmitting data with reduced bandwidth. | ✅        | Correct — traffic continues using remaining links.            |

---

### ✅ **Question 6**

**When EtherChannel is implemented, multiple physical interfaces are bundled into which type of logical connection?**

| Option          | Correct? | Explanation                                            |
| --------------- | -------- | ------------------------------------------------------ |
| Interface range | ❌        | Used only for configuration, not a logical interface.  |
| Loopback        | ❌        | Not related to EtherChannel.                           |
| VLAN interface  | ❌        | Used for Layer 3 SVI, not EtherChannel.                |
| Port channel    | ✅        | This is the logical interface representing the bundle. |

---

### ✅ **Question 7**

**When a range of ports is being configured for EtherChannel by the use of PAgP, which mode will form the bundled channel only if the port receives PAgP packets from another device?**

| Option    | Correct? | Explanation                                     |
| --------- | -------- | ----------------------------------------------- |
| Active    | ❌        | LACP mode                                       |
| Auto      | ✅        | Waits for PAgP packets from the other side      |
| Desirable | ❌        | Actively sends PAgP packets to form the channel |
| Passive   | ❌        | LACP mode                                       |

---

### ✅ **Question 8**

**Which two load balancing methods can be implemented with EtherChannel technology?** (Choose two)

| Option                            | Correct? | Explanation                             |
| --------------------------------- | -------- | --------------------------------------- |
| Destination MAC to destination IP | ❌        | Not a valid combination                 |
| Destination IP to destination MAC | ❌        | Not standard                            |
| Source MAC to destination MAC     | ✅        | Valid method for Layer 2 load balancing |
| Source IP to destination IP       | ✅        | Valid method for Layer 3 load balancing |
| Destination MAC to source MAC     | ❌        | Not standard                            |
| Destination IP to source IP       | ❌        | Not commonly used                       |

---

### ✅ **Question 9**

**Which function is provided by EtherChannel?**

| Option                                                                              | Correct? | Explanation                                                           |
| ----------------------------------------------------------------------------------- | -------- | --------------------------------------------------------------------- |
| Spreading traffic across multiple physical WAN links                                | ❌        | EtherChannel is used in LAN environments, not WAN                     |
| Dividing the bandwidth of a single link into separate time slots                    | ❌        | That describes **Time Division Multiplexing (TDM)**, not EtherChannel |
| Enabling traffic from multiple VLANs to travel over a single Layer 2 link           | ❌        | That describes **trunking**, not EtherChannel                         |
| Creating one logical link by using multiple physical links between two LAN switches | ✅        | This is exactly what EtherChannel does — it bundles links             |

---

Let me know if you'd like this exported as a table in `README.md` format!










Here are the **answers with all options shown** for **Questions 10 to 15** with correct answers marked and explanations:

---

### **Question 10**

Which statement is true about EtherChannel technology?

* ⬜ All configuration tasks must be done on the individual ports in the EtherChannel link.
* ✅ **EtherChannel uses existing switch ports.**
* ⬜ Links must be upgraded to support EtherChannel.
* ⬜ STP does not run on redundant EtherChannel links.
  **Explanation:** EtherChannel bundles existing physical ports into one logical link; STP does run on EtherChannel logical links.

---

### **Question 11**

Which two mode combinations would result in the successful negotiation of an EtherChannel? (Choose two.)

* ✅ **Active; passive**
* ⬜ Passive; auto
* ✅ **Desirable; active**
* ⬜ Auto; auto
* ✅ **Desirable; desirable**
* ⬜ Active; on
  **Explanation:**
* For LACP: active/passive works
* For PAgP: desirable/desirable or desirable/active work
* “On” mode does not negotiate, so active/on doesn't form negotiation

---

### **Question 12**

Which two protocols are link aggregation protocols? (Choose two.)

* ✅ **802.3ad** (standard for LACP)
* ✅ **PAgP**
* ⬜ STP
* ⬜ EtherChannel (not a protocol, but a technology)
* ⬜ RSTP
  **Explanation:**
  802.3ad (LACP) and PAgP are protocols for link aggregation.

---

### **Question 13**

When a range of ports is being configured for EtherChannel, which mode will configure LACP so that it initiates the EtherChannel negotiation?

* ✅ **Active**
* ⬜ Auto
* ⬜ Desirable
* ⬜ Passive
  **Explanation:** LACP’s **active** mode actively initiates negotiation.

---

### **Question 14**

What will happen if a network administrator puts a port that is part of an EtherChannel bundle into a different VLAN than the other ports in that bundle?

* ⬜ The EtherChannel bundle will stay up only if PAgP is used.
* ⬜ The EtherChannel bundle will stay up only if LACP is used.
* ⬜ The EtherChannel bundle will stay up if either PAgP or LACP is used.
* ⬜ The EtherChannel bundle will stay up if the ports were configured with no negotiation between the switches to form the EtherChannel.
* ✅ **The EtherChannel will fail.**
  **Explanation:** All ports in an EtherChannel must belong to the same VLAN; otherwise, the bundle fails.

---

### **Question 15**

When a range of ports is being configured for EtherChannel, which mode will configure LACP on a port only if the port receives LACP packets from another device?

* ⬜ Active
* ✅ **Passive**
* ⬜ Desirable
* ⬜ Auto
  **Explanation:** LACP **passive** mode waits for LACP packets before forming the channel.

---

If you want, I can prepare a full quiz with answers & explanations for all 15 questions in one place!
