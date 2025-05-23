Here are the **correct answers** for the 10.1.6 "Check Your Understanding – Endpoint Security" questions:

---

### **Question 1**

**Which attack encrypts the data on hosts in an attempt to extract a monetary payment from the victim?**

* ⭕ DDoS
* ⭕ Data breach
* ⭕ Malware
* ✅ **Ransomware**

**Explanation:**
**Ransomware** encrypts a victim's data and demands payment (usually cryptocurrency) to decrypt it. It's a specific type of malware aimed at extortion.

---

### **Question 2**

**Which devices are specifically designed for network security?** (Choose **three**)

* ✅ **VPN-enabled router**
* ✅ **NGFW** (Next-Generation Firewall)
* ⭕ Switch
* ⭕ WLC (Wireless LAN Controller)
* ✅ **NAC** (Network Access Control)

**Explanation:**

* **VPN-enabled routers** secure remote connections.
* **NGFWs** provide deep packet inspection, application awareness, and threat intelligence.
* **NAC** ensures devices comply with security policies before allowing access.
* **Switches and WLCs** are network infrastructure devices, not specifically security-focused.

---

### **Question 3**

**Which device monitors SMTP traffic to block threats and encrypt outgoing messages to prevent data loss?**

* ⭕ NGFW
* ✅ **ESA** (Email Security Appliance)
* ⭕ NAC
* ⭕ WSA

**Explanation:**
**ESA** focuses on email traffic (SMTP) to block spam, phishing, malware, and encrypt outgoing emails.

---

### **Question 4**

**Which device monitors HTTP traffic to block access to risky sites and encrypt outgoing messages?**

* ⭕ NGFW
* ⭕ ESA
* ⭕ NAC
* ✅ **WSA** (Web Security Appliance)

**Explanation:**
**WSA** is designed for monitoring and securing web traffic (HTTP/HTTPS), blocking malicious sites, and enforcing web usage policies.

---

Let me know if you'd like a summary table or printable format!





Here are all the questions with **all options**, the **correct answer marked**, and **explanations**:

---

### ✅ **Question 1**

**Which AAA component is responsible for collecting and reporting usage data for auditing and billing purposes?**

* ⭕ Authentication
* ⭕ Authorization
* ✅ **Accounting**

**Explanation:**
**Accounting** keeps track of user activities such as login times, duration, accessed services, and bandwidth usage. This is vital for auditing and billing.

---

### ✅ **Question 2**

**Which AAA component is responsible for controlling who is permitted to access the network?**

* ✅ **Authentication**
* ⭕ Authorization
* ⭕ Accounting

**Explanation:**
**Authentication** checks the credentials of users or devices before allowing access. It answers the question: *Who are you?*

---

### ✅ **Question 3**

**Which AAA component is responsible for determining what the user can access?**

* ⭕ Authentication
* ✅ **Authorization**
* ⭕ Accounting

**Explanation:**
**Authorization** determines the permissions granted to the user after they have been authenticated. It answers: *What are you allowed to do?*

---

### ✅ **Question 4**

**In an 802.1X implementation, which device is responsible for relaying responses?**

* ⭕ Supplicant
* ✅ **Authenticator**
* ⭕ Router
* ⭕ Authentication server
* ⭕ Client

**Explanation:**
In the 802.1X framework:

* **Supplicant**: the device trying to gain access (e.g., a laptop).
* **Authenticator**: typically a switch or access point that **relays messages** between the supplicant and the server.
* **Authentication Server**: validates the credentials (commonly a RADIUS server).

---

Let me know if you want this formatted in a table or exported as a document.







Here are the answers to **10.3.4 Check Your Understanding - Layer 2 Security Threats** with **all options**, **correct answers marked**, and **clear explanations**:

---

### ✅ **Question 1**

**Which of the following mitigation techniques are used to protect Layer 3 through Layer 7 of the OSI Model? (Choose three.)**

* ⭕ DHCP snooping
* ✅ **VPN**
* ✅ **Firewalls**
* ⭕ IPSG (IP Source Guard)
* ✅ **IPS devices (Intrusion Prevention Systems)**

**Explanation:**

* **VPNs** protect data at Layer 3 (network layer) by encrypting traffic.
* **Firewalls** operate from Layer 3 to Layer 7, filtering and controlling traffic.
* **IPS devices** protect applications by inspecting Layer 3–7 traffic for threats.
* **DHCP snooping** and **IPSG** are Layer 2 protection mechanisms.

---

### ✅ **Question 2**

**Which of the following mitigation techniques prevents many types of attacks including MAC address table overflow and DHCP starvation attacks?**

* ⭕ IPSG
* ⭕ DHCP snooping
* ⭕ DAI
* ✅ **Port security**

**Explanation:**
**Port Security** limits the number of valid MAC addresses on a port, helping prevent **MAC flooding** and **DHCP starvation attacks** by controlling how many devices can connect.

---

### ✅ **Question 3**

**Which of the following mitigation techniques prevents MAC and IP address spoofing?**

* ✅ **IPSG (IP Source Guard)**
* ⭕ DHCP snooping
* ⭕ DAI
* ⭕ Port security

**Explanation:**
**IP Source Guard** ensures that only packets with valid IP-MAC bindings (learned via DHCP snooping) are allowed, thus preventing **spoofing attacks**.

---

### ✅ **Question 4**

**Which of the following mitigation techniques prevents ARP spoofing and ARP poisoning attacks?**

* ⭕ IPSG
* ⭕ DHCP snooping
* ✅ **DAI (Dynamic ARP Inspection)**
* ⭕ Port security

**Explanation:**
**DAI** uses trusted DHCP snooping bindings to verify ARP packets, thereby blocking **ARP spoofing/poisoning attacks**.

---

### ✅ **Question 5**

**Which of the following mitigation techniques prevents DHCP starvation and DHCP spoofing attacks?**

* ⭕ IPSG
* ✅ **DHCP snooping**
* ⭕ DAI
* ⭕ Port security

**Explanation:**
**DHCP snooping** filters DHCP messages to protect against **DHCP spoofing** (malicious DHCP servers) and **starvation attacks** (exhausting DHCP pool using fake requests).

---

Let me know if you'd like this in table format or added to a markdown file.








Here are the correct answers for **10.4.4 Check Your Understanding - MAC Address Table Attacks** with **all options shown**, **correct answers marked**, and **explanations**:

---

### ✅ **Question 1**

**What is the behavior of a switch as a result of a successful MAC address table attack?**

* ⭕ The switch will shut down.
* ⭕ The switch interfaces will transition to the error-disabled state.
* ✅ **The switch will forward all received frames to all other ports within the VLAN.**
* ⭕ The switch will drop all received frames.

**Explanation:**
When a **MAC address table overflow** attack (also known as **MAC flooding**) succeeds, the switch's MAC table fills up. As a result, the switch is unable to make forwarding decisions based on MAC addresses and instead **floods all frames out all ports**, like a hub.

---

### ✅ **Question 2**

**What would be the primary reason a threat actor would launch a MAC address overflow attack?**

* ✅ **So that the threat actor can see frames that are destined for other devices.**
* ⭕ So that the threat actor can execute arbitrary code on the switch.
* ⭕ So that the switch stops forwarding traffic.
* ⭕ So that legitimate hosts cannot obtain a MAC address.

**Explanation:**
By flooding the MAC table, a threat actor can force the switch to flood all traffic, allowing the attacker to **eavesdrop** on traffic intended for other devices. This is a classic **man-in-the-middle (MitM)** tactic.

---

### ✅ **Question 3**

**What mitigation technique must be implemented to prevent MAC address overflow attacks?**

* ⭕ IPSG
* ⭕ DAI
* ✅ **Port security**
* ⭕ DHCP snooping

**Explanation:**
**Port Security** limits the number of MAC addresses learned on a port, preventing attackers from flooding the switch with fake MAC addresses and thus **protecting against MAC table overflow attacks**.

---

Let me know if you'd like these compiled into a markdown table or study sheet.









Here are the correct answers for **10.5.11 Check Your Understanding - LAN Attacks**, with all options shown, correct answers marked, and explanations included:

---

### ✅ **Question 1**

**A threat actor changes the MAC address of the threat actor's device to the MAC address of the default gateway. What type of attack is this?**

* ✅ **Address spoofing**
* ⭕ ARP spoofing
* ⭕ CDP reconnaissance
* ⭕ DHCP starvation
* ⭕ STP attack
* ⭕ VLAN hopping

**Explanation:**
This is **address spoofing**, where a device is configured with the MAC address of the gateway to intercept traffic. If the actor sends fake ARP responses too, it becomes **ARP spoofing**, but changing just the MAC address falls under **address spoofing**.

---

### ✅ **Question 2**

**A threat actor sends a BPDU message with priority 0. What type of attack is this?**

* ⭕ Address spoofing
* ⭕ ARP spoofing
* ⭕ CDP reconnaissance
* ⭕ DHCP starvation
* ✅ **STP attack**
* ⭕ VLAN hopping

**Explanation:**
Sending a **Bridge Protocol Data Unit (BPDU)** with priority 0 attempts to become the root bridge in the Spanning Tree Protocol (STP), causing network instability—this is a classic **STP attack**.

---

### ✅ **Question 3**

**A threat actor leases all the available IP addresses on a subnet. What type of attack is this?**

* ⭕ Address spoofing
* ⭕ ARP spoofing
* ⭕ CDP reconnaissance
* ✅ **DHCP starvation**
* ⭕ STP attack
* ⭕ VLAN hopping

**Explanation:**
This is a **DHCP starvation attack**, where an attacker uses many spoofed MAC addresses to exhaust the DHCP server’s IP pool, preventing legitimate devices from obtaining IP addresses.

---

### ✅ **Question 4**

**A threat actor sends a message that causes all other devices to believe the MAC address of the threat actor's device is the default gateway. What type of attack is this?**

* ⭕ Address spoofing
* ✅ **ARP spoofing**
* ⭕ CDP reconnaissance
* ⭕ DHCP starvation
* ⭕ STP attack
* ⭕ VLAN hopping

**Explanation:**
This is **ARP spoofing**, where the attacker sends fake ARP replies to associate their MAC address with the IP address of the default gateway, intercepting traffic.

---

### ✅ **Question 5**

**A threat actor configures a host with the 802.1Q protocol and forms a trunk with the connected switch. What type of attack is this?**

* ⭕ Address spoofing
* ⭕ ARP spoofing
* ⭕ CDP reconnaissance
* ⭕ DHCP starvation
* ⭕ STP attack
* ✅ **VLAN hopping**

**Explanation:**
This is **VLAN hopping**, where the attacker uses 802.1Q trunking to access multiple VLANs by creating a trunk link from a host.

---

### ✅ **Question 6**

**A threat actor discovers the IOS version and IP addresses of the local switch. What type of attack is this?**

* ⭕ Address spoofing
* ⭕ ARP spoofing
* ✅ **CDP reconnaissance**
* ⭕ DHCP starvation
* ⭕ STP attack
* ⭕ VLAN hopping

**Explanation:**
This is **CDP (Cisco Discovery Protocol) reconnaissance**. The attacker uses CDP messages to gather detailed information about connected Cisco devices, such as the IOS version and IP addresses.

---

Let me know if you'd like this in a table format or as part of a compiled PDF/README for study.



Here are the answers with all options listed for **10.6.2 Module Quiz - LAN Security Concepts**, plus the correct answers marked and explanations:

---

### Question 1

**What two protocols are supported on Cisco devices for AAA communications? (Choose two.)**

* ⬜ VTP
* ⬜ LLDP
* ⬜ HSRP
* ✅ **RADIUS**
* ✅ **TACACS+**

**Explanation:**
Cisco devices support **RADIUS** and **TACACS+** protocols for AAA (Authentication, Authorization, and Accounting) communications.

---

### Question 2

**Which service is enabled on a Cisco router by default that can reveal significant information about the router and potentially make it more vulnerable to attack?**

* ⬜ HTTP
* ✅ **CDP**
* ⬜ FTP
* ⬜ LLDP

**Explanation:**
**Cisco Discovery Protocol (CDP)** is enabled by default and can reveal device information, which can be exploited if not managed.

---

### Question 3

**When security is a concern, which OSI Layer is considered to be the weakest link in a network system?**

* ⬜ Layer 4
* ✅ **Layer 2**
* ⬜ Layer 3
* ⬜ Layer 7

**Explanation:**
**Layer 2** is considered the weakest due to vulnerabilities like MAC spoofing, VLAN hopping, and other Layer 2 attacks.

---

### Question 4

**Which Layer 2 attack will result in a switch flooding incoming frames to all ports?**

* ⬜ ARP poisoning
* ⬜ IP address spoofing
* ✅ **MAC address overflow**
* ⬜ Spanning Tree Protocol manipulation

**Explanation:**
A **MAC address overflow** attack fills the switch’s MAC table causing it to flood frames to all ports, exposing traffic.

---

### Question 5

**Why is authentication with AAA preferred over a local database method?**

* ⬜ It uses less network bandwidth.
* ⬜ It requires a login and password combination on the console, vty lines, and aux ports.
* ⬜ It provides a fallback authentication method if the administrator forgets the username or password.
* ✅ **It specifies a different password for each line or port.**

**Explanation:**
AAA can enforce different credentials and granular access control per line or port, improving security and manageability compared to a local database.

---

### Question 6

**In a server-based AAA implementation, which protocol will allow the router to successfully communicate with the AAA server?**

* ⬜ SSH
* ✅ **RADIUS**
* ⬜ TACACS
* ⬜ 802.1x

**Explanation:**
**RADIUS** (and also TACACS+) are protocols used by routers to communicate with AAA servers. Here, RADIUS is the best choice for the router-AAA server communication.

---

### Question 7

**Which Cisco solution helps prevent MAC and IP address spoofing attacks?**

* ⬜ Port Security
* ⬜ DHCP Snooping
* ✅ **IP Source Guard**
* ⬜ Dynamic ARP Inspection

**Explanation:**
**IP Source Guard** prevents IP address spoofing by filtering IP-to-MAC bindings; **Port Security** limits MAC addresses; **Dynamic ARP Inspection** helps prevent ARP spoofing, but IP Source Guard best prevents MAC and IP spoofing.

---

### Question 8

**What is the purpose of AAA accounting?**

* ✅ **To collect and report application usage**
* ⬜ To determine which resources the user can access
* ⬜ To prove users are who they say they are
* ⬜ To determine which operations the user can perform

**Explanation:**
**Accounting** tracks and logs user activities for auditing and billing.

---

Let me know if you'd like me to format this as a table or provide more explanations!











Here are the answers to your latest questions with explanations:

---

### Question 9

**Which Layer 2 attack will result in legitimate users not getting valid IP addresses?**

* ⬜ ARP spoofing
* ✅ **DHCP starvation**
* ⬜ IP address spoofing
* ⬜ MAC address flooding

**Explanation:**
**DHCP starvation** floods the DHCP server with bogus requests, exhausting the IP address pool and preventing legitimate users from obtaining IP addresses.

---

### Question 10

**Which three Cisco products focus on endpoint security solutions? (Choose three.)**

* ✅ **IPS Sensor Appliance**
* ✅ **Web Security Appliance**
* ✅ **Email Security Appliance**
* ⬜ SSL/IPsec VPN Appliance
* ⬜ Adaptive Security Appliance
* ⬜ NAC Appliance

**Explanation:**
Cisco’s endpoint security products include **IPS Sensor Appliance**, **Web Security Appliance**, and **Email Security Appliance**, which provide protection directly relevant to endpoints.

---

### Question 11

**True or False?**
In the 802.1X standard, the client attempting to access the network is referred to as the supplicant.

* ✅ True
* ⬜ False

**Explanation:**
The **supplicant** is the client device that requests access in 802.1X authentication.

---

### Question 12

**What is involved in an IP address spoofing attack?**

* ✅ **A legitimate network IP address is hijacked by a rogue node.**
* ⬜ A rogue node replies to an ARP request with its own MAC address indicated for the target IP address.
* ⬜ A rogue DHCP server provides false IP configuration parameters to legitimate DHCP clients.
* ⬜ Bogus DHCPDISCOVER messages are sent to consume all the available IP addresses on a DHCP server.

**Explanation:**
IP address spoofing involves impersonating a legitimate IP address to intercept or misdirect traffic.

---

### Question 13

**What three services are provided by the AAA framework? (Choose three.)**

* ✅ **Accounting**
* ⬜ Automation
* ✅ **Authorization**
* ✅ **Authentication**
* ⬜ Autobalancing
* ⬜ Autoconfiguration

**Explanation:**
AAA stands for **Authentication, Authorization, and Accounting**.

---

### Question 14

**Because of implemented security controls, a user can only access a server with FTP. Which AAA component accomplishes this?**

* ⬜ Accessibility
* ⬜ Accounting
* ⬜ Auditing
* ⬜ Authentication
* ✅ **Authorization**

**Explanation:**
**Authorization** controls what a user is allowed to access or do after successful authentication.

---

### Question 15

**What mitigation plan is best for thwarting a DoS attack that is creating a MAC address table overflow?**

* ⬜ Disable DTP.
* ⬜ Disable STP.
* ✅ **Enable port security.**
* ⬜ Place unused ports in an unused VLAN.

**Explanation:**
**Port security** limits the number of MAC addresses on a port, preventing MAC flooding attacks.

---

If you'd like, I can also organize these answers in a table or explain any question further!
